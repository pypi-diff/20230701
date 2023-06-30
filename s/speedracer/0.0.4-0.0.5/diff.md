# Comparing `tmp/speedracer-0.0.4.tar.gz` & `tmp/speedracer-0.0.5.tar.gz`

## Comparing `speedracer-0.0.4.tar` & `speedracer-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 speedracer-0.0.4/src/speedracer/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 speedracer-0.0.4/LICENSE
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 speedracer-0.0.4/README.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 speedracer-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 speedracer-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    17758 2020-02-02 00:00:00.000000 speedracer-0.0.5/src/speedracer/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 speedracer-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 speedracer-0.0.5/README.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 speedracer-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 speedracer-0.0.5/PKG-INFO
```

### Comparing `speedracer-0.0.4/src/speedracer/__init__.py` & `speedracer-0.0.5/src/speedracer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 .. include:: ../../README.md
 
 '''
 
 import asyncio
 import datetime
 from enum import Enum
+import errno
 import hashlib
 import logging
+import os
 from pathlib import Path
 import ssl
 import time
 from typing import Union, Optional, Callable, Tuple, List, Dict, Iterable
 from urllib.parse import urlparse, urlunparse
 
 import jwt
@@ -47,14 +49,24 @@
         Arguments:
             url: The URL of the API Gateway to fetch JWTs from
             cert: A Tuple containing the paths to the certificate and
                 key to use with the API Gateway. By default, looks in the
                 user's home directory for the files cert.crt and cert.key
             verify: A bool or a path to a Certificate Authority. Passed to the requests library
         '''
+
+        if not os.path.isfile(cert[0]):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), cert[0])
+
+        if not os.path.isfile(cert[1]):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), cert[1])
+
+        if not isinstance(verify, bool) and not os.path.isfile(verify):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), verify)
+
         self.token:Optional[Union[str, None]] = None
         '''The most recently fetched JWT. Use the `get` method instead of accessing this directly'''
         self.url:str = url
         '''The URL of the API Gateway to fetch JWTs from'''
         self.cert:Tuple[str, str] = cert
         '''A Tuple containing the paths to the certificate and key to use with the API Gateway'''
         self.verify:Union[str, bool] = verify
@@ -65,16 +77,20 @@
             (datetime.datetime.utcnow() + datetime.timedelta(minutes=5)).timetuple())
         claims = jwt.decode(self.token, options={'verify_signature': False})
         if 'exp' in claims:
             return claims['exp'] < in_five_minutes
         return False
 
     def __get_jwt(self) -> None:
-        resp = requests.get(self.url, cert=self.cert, verify=self.verify, timeout=10)
-        self.token = resp.text.strip()
+        try:
+            resp = requests.get(self.url, cert=self.cert, verify=self.verify, timeout=10)
+            resp.raise_for_status()
+            self.token = resp.text.strip()
+        except requests.exceptions.RequestException:
+            logging.getLogger(__name__).exception("fetching JWT")
 
     def get(self) -> str:
         '''Returns a cached JWT or a new one if the cached JWT is close to expiration
 
         Example:
             ```python
             token = manager.get()
@@ -122,15 +138,15 @@
 
 class Offset(str, Enum):
     '''The offset to start consuming messages from'''
     BEGIN = 'begin'
     NOW = 'now'
 
 class Connection:
-    '''Connect to the Mission Data Broker (MDB)'''
+    '''Connect to Autobahn'''
     def __init__(self, url:str, cert:Tuple[str, str]=(Path.home().joinpath('.ssh/cert.crt'),
                 Path.home().joinpath('.ssh/cert.key')),
             ca_bundle:Optional[str]=None) -> None:
         '''
         Example:
             ```python
             conn = Connection('https://mdb-account-server/')
@@ -138,30 +154,51 @@
 
         Arguments:
           url: URL of the Autobahn MDB account server
           cert: Paths to a PEM formated X.509 certificate and key file
             Defaults to ('$HOME/.ssh/cert.crt', '$HOME/.ssh/cert.key')
           ca_bundle: A path to a PEM encoded certificate authority file
         '''
+
+        if not os.path.isfile(cert[0]):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), cert[0])
+
+        if not os.path.isfile(cert[1]):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), cert[1])
+
+        if ca_bundle and not os.path.isfile(ca_bundle):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), ca_bundle)
+
         def get_urls():
             config_url = urlparse(url)
             config_url = urlunparse(config_url._replace(path='/api/v1/config'))
-            return requests.get(config_url, verify=self.verify, timeout=10).json()
+            try:
+                resp = requests.get(config_url, verify=self.verify, timeout=10)
+                resp.raise_for_status()
+                return resp.json()
+            except requests.exceptions.SSLError as ssl_error:
+                logging.getLogger(__name__).exception('''SSLError getting
+service urls. Commonly caused by not providing client certificates or by
+not specifying a ca_bundle''')
+                raise ssl_error
+            except requests.exceptions.RequestException as err:
+                logging.getLogger(__name__).exception('getting service urls')
+                raise err
 
         self.cert: Tuple[str, str] = cert
         '''Client certificate. Invalid certificates result in `SSLError`'''
         self.ca_bundle: Optional[str] = ca_bundle
         '''Certificate Authority used to verify server SSL certificates'''
         self.verify: Union[str, bool] = ca_bundle if ca_bundle else True
         '''Verify server SSL certificates. Set to false if a valid ca_bundle is not available.'''
         self.urls: Dict = get_urls()
         '''URLs to Autobahn services (read-only)'''
         self.jwt_manager: JWTManager = JWTManager(self.urls['api_gateway_url'],
                 cert=cert, verify=self.verify)
-        '''A `JWTManager` for authenticating to the MDB'''
+        '''A `JWTManager` for authenticating to Autobahn'''
         self.subscriptions: List = []
         '''An array of all Subscriptions associated with this Connection'''
 
     async def subscribe(self, dataset:str, offset:Offset=Offset.NOW, batch:int=10,
             callback:Optional[Callable]=None) -> Iterable:
         '''Subscribe to a dataset.
 
@@ -177,15 +214,15 @@
             offset: The offset to start consuming messages from
             batch: The number of messages retrieved at a time
         '''
         sub = self.Subscription(self.urls, self.jwt_manager, self.ca_bundle,
                 dataset, offset, batch, callback)
         await sub.start()
         self.subscriptions.append(sub)
-        logging.getLogger(__name__).info(f"Subscribed to dataset: {dataset}")
+        logging.getLogger(__name__).info("Subscribed to dataset: %s", dataset)
         return sub
 
     async def close(self):
         '''Close all subscriptions associated with this Connection'''
 
         # pylint: disable=broad-exception-caught
         # Try closing each subscription
@@ -208,29 +245,29 @@
 
         def __init__(self, urls:Dict, jwt_manager:JWTManager, ca_bundle:Optional[str],
                 dataset:str, offset:Offset, batch:int, callback:Optional[Callable]) -> None:
             '''Create a subscription. Use a Connection's `subscribe` method instead
 
             Arguments:
                 urls: A Dict containing URLs to services
-                jwt_manager: A `JWTManager` for authenticating to the MDB
+                jwt_manager: A `JWTManager` for authenticating to Autobahn
                 ca_bundle: Path to a Certificate Authority
                 dataset: The slug of the dataset to subscribe to
                 offset: The offset to start consuming messages from
                 batch: The number of messages the client will pull at a time
                 callback: A Callable that takes a NATS message as an
                     argument. Called for each messages received
             '''
             self.verify:Union[str, bool] = ca_bundle if ca_bundle else True
             '''Verify server SSL certificates. Set to false if a valid 
             ca_bundle is not available.'''
             self.urls:Dict = urls
             '''URLs to Autobahn services (read-only)'''
             self.jwt_manager:JWTManager = jwt_manager
-            '''A JWTManager for authenticating to the MDB'''
+            '''A JWTManager for authenticating to Autobahn'''
             self.dataset:str = dataset
             '''The dataset slug for this subscription'''
             self.offset:Offset = offset
             '''The offset to start consuming messages from'''
             self.batch:int = batch
             '''Number of messages the subscription will pull at a time'''
             self.callback:Optional[Callable] = callback
@@ -252,14 +289,15 @@
 
             def get_subject() -> str:
                 headers = jwt_manager.get_headers()
                 headers['Accept'] = 'application/vnd.pgrst.object+json'
                 resp = requests.get(
                         f"{urls['registry_url']}/api/v1/datasets?slug=eq.{self.dataset}",
                         headers=headers, verify=self.verify, timeout=10)
+                resp.raise_for_status()
                 dataset_entry = resp.json()
                 subject = f"EVENTS.{self.dataset}"
                 if dataset_entry.get('data_object_backend'):
                     if dataset_entry['data_object_backend'] == 'MDB':
                         subject = f"OBJECTS.{self.dataset}"
                 elif dataset_entry.get('mdb_object_publish'):
                     subject = f"OBJECTS.{self.dataset}"
@@ -290,14 +328,15 @@
             when using `Connection.subscribe()`'''
             def signature(_):
                 return bytes('', 'UTF-8')
 
             def get_mas_jwt() -> bytearray:
                 resp = requests.get(f"{self.urls['mas_url']}/api/v1/user/jwt/{self.dataset}",
                         headers=self.jwt_manager.get_headers(), verify=self.verify, timeout=10)
+                resp.raise_for_status()
                 encoded_token = resp.text.encode()
                 return bytearray(encoded_token)
 
             def get_consumer_name() -> str:
                 cn_hash = hashlib.md5(self.jwt_manager.get_cn().encode())
                 return cn_hash.hexdigest()[:-1] + '0'
```

### Comparing `speedracer-0.0.4/LICENSE` & `speedracer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `speedracer-0.0.4/README.md` & `speedracer-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # What is speedracer?
 
-speedracer is an asyncio enabled python library for interacting with Autobahn.
+Speedracer is an asyncio enabled python library for interacting with Autobahn.
+Speedracer enables users to
 
-- Subscribe to datasets available in the Mission Data Broker (MDB)
+- Subscribe to datasets available in Autobahn
 - Authenticate to Autobahn APIs
 
 # Installation
 
 <span style="color:red;">Requires Python3.8+</span>
 
 ```
@@ -18,25 +19,31 @@
 <span style="color:red;">
   See <a href="#important-notes">Important Notes</a> for all SSL/TLS errors.
 </span>
 
 ## Subscribe to a dataset
 
 To subscribe to a dataset on the MDB
-  1. Provide the base URL of the MDB Account Server (MAS) when creating a Connection
-  2. Provide the dataset to the subscribe method
+  1. Modify the string 'PUT-DATASET-HERE' with the dataset slug
+  1. Modify the certificate paths to poin to your certificates [(about certificates)](#providing-client-certificates)
+  1. Download the CA Bundle from the table [here](#providing-a-certificate-authority-sslcertverificationerror), and update the `ca_bundle` path to point to it
+
+Put the following code block in a file, and run it.
 
 ```python
 import asyncio
 from speedracer import Connection
 
-conn = Connection('https://mdb-account-server/')
-sub = await conn.subscribe('mydataset')
-async for msg in sub:
-    print(msg.data.decode())
+async def main():
+    conn = Connection('https://mdb-account-server/',
+              cert=('/path/to/mycert.crt', '/path/to/mycert.key'),
+              ca_bundle='/path/to/ca.cer')
+    sub = await conn.subscribe('PUT-DATASET-HERE')
+    async for msg in sub:
+        print(msg.data.decode())
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 ## Authenticate to Autobahn APIs
 
@@ -45,15 +52,17 @@
 
 JWTs are obtained by exchanging private keys with the API Gateway server and
 must be periodically refreshed.
 
 `speedracer` automates the process of fetching JWTs and refreshing them when they expire.
 
 ```python
-manager = JWTManager('https://api-gateway/getjwt')
+manager = JWTManager('https://api-gateway/getjwt',
+              cert=('/path/to/mycert.crt', '/path/to/mycert.key'),
+              verify='/path/to/ca.cer')
 auth_headers = manager.get_headers()
 requests.get('https://autobahn-service/', headers=auth_headers)
 ```
 
 # Advanced Usage
 
 ## Dataset Subscriptions
@@ -94,15 +103,15 @@
 ```python
 sub = await conn.subscribe('mydataset', offset=Offset.BEGIN)
 ```
 
 ### Low Latency
 
 By default, each `Subscription` fetches messages in batches of 10. If the
-server has less than 10 messages to send, it will wait up to 10 seconds
+server has fewer than 10 messages to send, it will wait up to 10 seconds
 for new messages before returning the messages it does have. For low-latency
 applications set the `batch` size to 1.
 
 ```python
 sub = await conn.subscribe('mydataset', batch=1)
 ```
 
@@ -110,15 +119,15 @@
 
 ## SSL/TLS Errors
 
 SSL/TLS errors occur for 2 reasons
   1. Invalid or missing client certificates
   2. No certificate authority configured
 
-### Client certificates
+### Providing Client Certificates
 
 By default, speedracer uses PEM formatted X.509 certificates for user
 authentication. By default speedracer will use certificates placed in
 the users `$HOME/.ssh` directory. The certificate and key files should be named
 `$HOME/.ssh/cert.crt` and `$HOME/.ssh/cert.key`, respectively.
 
 To specify a different path, pass a tuple containing the path to the certificate
@@ -126,30 +135,30 @@
 
 ```python
 conn = Connection('https://mdb-account-server.com',
           cert=('./mycert.crt', './mycert.key'))
 ```
 
 To create PEM formatted `.crt` and `.key` certificate files from a PKCS `.p12`
-file, run the following OpenSSL commands.
+**signing_cert** file, run the following OpenSSL commands.
 
 ```
 openssl pkcs12 -in INFILE.p12 -out OUTFILE.key -nodes -nocerts
 openssl pkcs12 -in INFILE.p12 -out OUTFILE.crt -nokeys
 ```
 
-### Certificate Authority
+### Providing a Certificate Authority (SSLCertVerificationError)
 
 Certificate Authorities establish a chain of trust. This is usually configured globally
 as part of the operating system. There are cases where the OS does not have the proper
 certificate authority configured.
 
 In these instances, users may specify a cabundle as a X.509 PEM file via the argument `ca_bundle`.
 
-```
+```python
 conn = Connection('https://mdb-account-server.com', ca_bundle='ca.cer')
 ```
 
 Download the appropiate CA Bundle.
 
 | Autobahn Environment | Link to CA Bundle |
 | --- | --- |
```

### Comparing `speedracer-0.0.4/PKG-INFO` & `speedracer-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedracer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Conveniently access data
 Author: RRC
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -12,17 +12,18 @@
 Requires-Dist: nats-py[nkeys]~=2.3.1
 Requires-Dist: pyjwt~=2.7.0
 Requires-Dist: requests~=2.31.0
 Description-Content-Type: text/markdown
 
 # What is speedracer?
 
-speedracer is an asyncio enabled python library for interacting with Autobahn.
+Speedracer is an asyncio enabled python library for interacting with Autobahn.
+Speedracer enables users to
 
-- Subscribe to datasets available in the Mission Data Broker (MDB)
+- Subscribe to datasets available in Autobahn
 - Authenticate to Autobahn APIs
 
 # Installation
 
 <span style="color:red;">Requires Python3.8+</span>
 
 ```
@@ -34,25 +35,31 @@
 <span style="color:red;">
   See <a href="#important-notes">Important Notes</a> for all SSL/TLS errors.
 </span>
 
 ## Subscribe to a dataset
 
 To subscribe to a dataset on the MDB
-  1. Provide the base URL of the MDB Account Server (MAS) when creating a Connection
-  2. Provide the dataset to the subscribe method
+  1. Modify the string 'PUT-DATASET-HERE' with the dataset slug
+  1. Modify the certificate paths to poin to your certificates [(about certificates)](#providing-client-certificates)
+  1. Download the CA Bundle from the table [here](#providing-a-certificate-authority-sslcertverificationerror), and update the `ca_bundle` path to point to it
+
+Put the following code block in a file, and run it.
 
 ```python
 import asyncio
 from speedracer import Connection
 
-conn = Connection('https://mdb-account-server/')
-sub = await conn.subscribe('mydataset')
-async for msg in sub:
-    print(msg.data.decode())
+async def main():
+    conn = Connection('https://mdb-account-server/',
+              cert=('/path/to/mycert.crt', '/path/to/mycert.key'),
+              ca_bundle='/path/to/ca.cer')
+    sub = await conn.subscribe('PUT-DATASET-HERE')
+    async for msg in sub:
+        print(msg.data.decode())
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 ## Authenticate to Autobahn APIs
 
@@ -61,15 +68,17 @@
 
 JWTs are obtained by exchanging private keys with the API Gateway server and
 must be periodically refreshed.
 
 `speedracer` automates the process of fetching JWTs and refreshing them when they expire.
 
 ```python
-manager = JWTManager('https://api-gateway/getjwt')
+manager = JWTManager('https://api-gateway/getjwt',
+              cert=('/path/to/mycert.crt', '/path/to/mycert.key'),
+              verify='/path/to/ca.cer')
 auth_headers = manager.get_headers()
 requests.get('https://autobahn-service/', headers=auth_headers)
 ```
 
 # Advanced Usage
 
 ## Dataset Subscriptions
@@ -110,15 +119,15 @@
 ```python
 sub = await conn.subscribe('mydataset', offset=Offset.BEGIN)
 ```
 
 ### Low Latency
 
 By default, each `Subscription` fetches messages in batches of 10. If the
-server has less than 10 messages to send, it will wait up to 10 seconds
+server has fewer than 10 messages to send, it will wait up to 10 seconds
 for new messages before returning the messages it does have. For low-latency
 applications set the `batch` size to 1.
 
 ```python
 sub = await conn.subscribe('mydataset', batch=1)
 ```
 
@@ -126,15 +135,15 @@
 
 ## SSL/TLS Errors
 
 SSL/TLS errors occur for 2 reasons
   1. Invalid or missing client certificates
   2. No certificate authority configured
 
-### Client certificates
+### Providing Client Certificates
 
 By default, speedracer uses PEM formatted X.509 certificates for user
 authentication. By default speedracer will use certificates placed in
 the users `$HOME/.ssh` directory. The certificate and key files should be named
 `$HOME/.ssh/cert.crt` and `$HOME/.ssh/cert.key`, respectively.
 
 To specify a different path, pass a tuple containing the path to the certificate
@@ -142,30 +151,30 @@
 
 ```python
 conn = Connection('https://mdb-account-server.com',
           cert=('./mycert.crt', './mycert.key'))
 ```
 
 To create PEM formatted `.crt` and `.key` certificate files from a PKCS `.p12`
-file, run the following OpenSSL commands.
+**signing_cert** file, run the following OpenSSL commands.
 
 ```
 openssl pkcs12 -in INFILE.p12 -out OUTFILE.key -nodes -nocerts
 openssl pkcs12 -in INFILE.p12 -out OUTFILE.crt -nokeys
 ```
 
-### Certificate Authority
+### Providing a Certificate Authority (SSLCertVerificationError)
 
 Certificate Authorities establish a chain of trust. This is usually configured globally
 as part of the operating system. There are cases where the OS does not have the proper
 certificate authority configured.
 
 In these instances, users may specify a cabundle as a X.509 PEM file via the argument `ca_bundle`.
 
-```
+```python
 conn = Connection('https://mdb-account-server.com', ca_bundle='ca.cer')
 ```
 
 Download the appropiate CA Bundle.
 
 | Autobahn Environment | Link to CA Bundle |
 | --- | --- |
```

