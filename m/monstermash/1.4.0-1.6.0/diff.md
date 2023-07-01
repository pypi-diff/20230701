# Comparing `tmp/monstermash-1.4.0.tar.gz` & `tmp/monstermash-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-1.4.0.tar", max compression
+gzip compressed data, was "monstermash-1.6.0.tar", max compression
```

## Comparing `monstermash-1.4.0.tar` & `monstermash-1.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1366 2023-06-30 12:06:21.844365 monstermash-1.4.0/README.md
--rw-r--r--   0        0        0     1152 2023-06-30 12:06:21.848365 monstermash-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/__init__.py
--rw-r--r--   0        0        0     4196 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1024 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/config.py
--rw-r--r--   0        0        0     3632 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/crypt.py
--rw-r--r--   0        0        0      399 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/datamodels.py
--rw-r--r--   0        0        0     1272 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/parser.py
--rw-r--r--   0        0        0        0 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/utils/__init__.py
--rw-r--r--   0        0        0      709 2023-06-30 12:06:21.848365 monstermash-1.4.0/src/monstermash/utils/file.py
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 monstermash-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2170 2023-07-01 03:24:35.540656 monstermash-1.6.0/README.md
+-rw-r--r--   0        0        0     1152 2023-07-01 03:24:35.540656 monstermash-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     4205 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/__main__.py
+-rw-r--r--   0        0        0     1024 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/config.py
+-rw-r--r--   0        0        0     3680 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/crypt.py
+-rw-r--r--   0        0        0      399 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/datamodels.py
+-rw-r--r--   0        0        0     1272 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/parser.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/utils/__init__.py
+-rw-r--r--   0        0        0      709 2023-07-01 03:24:35.540656 monstermash-1.6.0/src/monstermash/utils/file.py
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 monstermash-1.6.0/PKG-INFO
```

### Comparing `monstermash-1.4.0/pyproject.toml` & `monstermash-1.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monstermash"
-version = "1.4.0"
+version = "1.6.0"
 description = ""
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "monstermash", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
```

### Comparing `monstermash-1.4.0/src/monstermash/__main__.py` & `monstermash-1.6.0/src/monstermash/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Mapping, Optional
 
 import click
 
 from monstermash.config import Config
-from monstermash.crypt import Crypt
+from monstermash.crypt import Crypt, KeyPair
 from monstermash.parser import ConfigManager
 from monstermash.utils.file import NEW_LINE_EXPR, open_file
 
 
 @click.group()
 @click.pass_context
 def mash(ctx):
```

### Comparing `monstermash-1.4.0/src/monstermash/config.py` & `monstermash-1.6.0/src/monstermash/config.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.4.0/src/monstermash/crypt.py` & `monstermash-1.6.0/src/monstermash/crypt.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Attributes:
         key_length (int): The length of the keys used in encryption/decryption. Default is 32.
     """
 
     key_length: int = 32
 
-    def __init__(self, private_key: bytes, msg_encoder=HexEncoder, key_encoder=HexEncoder):
+    def __init__(self, private_key: bytes, message_encoder=HexEncoder, key_encoder=HexEncoder):
         """
         Initialize a new instance of Crypt class.
 
         Args:
             private_key (bytes): The private key used for encryption and decryption.
-            msg_encoder (HexEncoder): Encoder used for encoding and decoding messages. Default is HexEncoder.
+            message_encoder (HexEncoder): Encoder used for encoding and decoding messages. Default is HexEncoder.
             key_encoder (HexEncoder): Encoder used for encoding and decoding keys. Default is HexEncoder.
         """
-        self.msg_encoder = msg_encoder
+        self.message_encoder = message_encoder
         self.key_encoder = key_encoder
         self._private_key = PrivateKey(private_key, encoder=self.key_encoder)
 
     @property
     def private_key(self) -> bytes:
         """Get encoded private key.
 
@@ -66,40 +66,40 @@
             KeyPair: A tuple containing the encoded private key and public key.
         """
         private_key = PrivateKey.generate()
         private_key_encoded = private_key.encode(encoder)
         public_key_encoded = private_key.public_key.encode(encoder)
         return KeyPair(private_key=private_key_encoded, public_key=public_key_encoded)
 
-    def encrypt(self, msg: bytes, public_key: bytes) -> bytes:
+    def encrypt(self, message: bytes, public_key: bytes) -> bytes:
         """
         Encrypt a message using a given public key. We append the public key to the ciphertext so that decryption
         becomes easy. The size of the key has to be consistent between encryption and decryption so that we can split
         the ciphertext based off the key size.
 
         Args:
-            msg (bytes): The message to be encrypted.
+            message (bytes): The message to be encrypted.
             public_key (bytes): The public key used for encryption.
 
         Returns:
             bytes: The encrypted message.
         """
         secret = Box(self._private_key, PublicKey(public_key, encoder=self.key_encoder))
-        encrypted = secret.encrypt(msg)
+        encrypted = secret.encrypt(message)
         formatted = b''.join([self.public_key, encrypted])
-        return self.msg_encoder.encode(formatted)
+        return self.message_encoder.encode(formatted)
 
-    def decrypt(self, msg: bytes) -> bytes:
+    def decrypt(self, message: bytes) -> bytes:
         """
         Decrypt a message using the private key.
 
         Args:
-            msg (bytes): The message to be decrypted.
+            message (bytes): The message to be decrypted.
 
         Returns:
             bytes: The decrypted message.
         """
-        decoded = self.msg_encoder.decode(msg)
+        decoded = self.message_encoder.decode(message)
         key = self.key_encoder.encode(decoded[: self.key_length])
         data = decoded[self.key_length :]
         secret = Box(self._private_key, PublicKey(key, encoder=self.key_encoder))
         return secret.decrypt(data)
```

### Comparing `monstermash-1.4.0/src/monstermash/parser.py` & `monstermash-1.6.0/src/monstermash/parser.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.4.0/src/monstermash/utils/file.py` & `monstermash-1.6.0/src/monstermash/utils/file.py`

 * *Files identical despite different names*

