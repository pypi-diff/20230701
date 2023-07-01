# Comparing `tmp/deairequest-0.0.7.tar.gz` & `tmp/deairequest-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deairequest-0.0.7.tar", last modified: Fri Jun 30 11:54:45 2023, max compression
+gzip compressed data, was "deairequest-0.0.8.tar", last modified: Sat Jul  1 06:19:18 2023, max compression
```

## Comparing `deairequest-0.0.7.tar` & `deairequest-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-06-30 11:54:45.545865 deairequest-0.0.7/
--rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-06-30 11:54:45.546172 deairequest-0.0.7/PKG-INFO
--rw-r--r--   0 maarten    (501) staff       (20)     1600 2023-06-30 11:32:54.000000 deairequest-0.0.7/README.md
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-06-30 11:54:45.532130 deairequest-0.0.7/deairequest/
--rw-r--r--   0 maarten    (501) staff       (20)     7962 2023-06-30 11:06:58.000000 deairequest-0.0.7/deairequest/BacalhauProtocol.py
--rw-r--r--   0 maarten    (501) staff       (20)     2072 2023-06-28 08:10:07.000000 deairequest-0.0.7/deairequest/DeProtocol.py
--rw-r--r--   0 maarten    (501) staff       (20)      320 2023-06-06 08:41:48.000000 deairequest-0.0.7/deairequest/DeProtocolSelector.py
--rw-r--r--   0 maarten    (501) staff       (20)     1594 2023-06-28 08:14:29.000000 deairequest-0.0.7/deairequest/ErrorProtocol.py
--rw-r--r--   0 maarten    (501) staff       (20)      122 2023-05-30 07:49:58.000000 deairequest-0.0.7/deairequest/__init__.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-06-30 11:54:45.535561 deairequest-0.0.7/deairequest/connectors/
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:00.000000 deairequest-0.0.7/deairequest/connectors/__init__.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-06-30 11:54:45.545211 deairequest-0.0.7/deairequest/connectors/bacalhau/
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:59.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/__init__.py
--rw-r--r--   0 maarten    (501) staff       (20)      826 2023-06-28 14:29:45.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/backends.py
--rw-r--r--   0 maarten    (501) staff       (20)     2289 2023-06-26 13:55:09.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/code.py
--rw-r--r--   0 maarten    (501) staff       (20)     6891 2023-06-30 10:20:51.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/deploy.py
--rw-r--r--   0 maarten    (501) staff       (20)      623 2023-06-28 16:29:54.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/main.py
--rw-r--r--   0 maarten    (501) staff       (20)    26812 2023-06-10 08:19:26.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/mapping.py
--rw-r--r--   0 maarten    (501) staff       (20)     4795 2023-06-28 14:30:52.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/notebooks.py
--rw-r--r--   0 maarten    (501) staff       (20)     3453 2023-06-30 09:54:17.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/querybhl.py
--rw-r--r--   0 maarten    (501) staff       (20)     3859 2023-06-30 09:19:03.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/render.py
--rw-r--r--   0 maarten    (501) staff       (20)    36617 2023-06-10 08:19:26.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/stdlib.py
--rw-r--r--   0 maarten    (501) staff       (20)     2246 2023-06-26 08:46:32.000000 deairequest-0.0.7/deairequest/connectors/bacalhau/step.py
--rw-r--r--   0 maarten    (501) staff       (20)     1571 2023-06-06 08:59:18.000000 deairequest-0.0.7/deairequest/logo.svg
--rw-r--r--   0 maarten    (501) staff       (20)     7484 2023-06-30 09:24:04.000000 deairequest-0.0.7/deairequest/test.ipynb
--rw-r--r--   0 maarten    (501) staff       (20)     5620 2023-06-30 11:08:32.000000 deairequest-0.0.7/deairequest/test_DeAIRequest.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-06-30 11:54:45.534892 deairequest-0.0.7/deairequest.egg-info/
--rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-06-30 11:54:45.000000 deairequest-0.0.7/deairequest.egg-info/PKG-INFO
--rw-r--r--   0 maarten    (501) staff       (20)      926 2023-06-30 11:54:45.000000 deairequest-0.0.7/deairequest.egg-info/SOURCES.txt
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-30 11:54:45.000000 deairequest-0.0.7/deairequest.egg-info/dependency_links.txt
--rw-r--r--   0 maarten    (501) staff       (20)       12 2023-06-30 11:54:45.000000 deairequest-0.0.7/deairequest.egg-info/top_level.txt
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-21 08:22:51.000000 deairequest-0.0.7/deairequest.egg-info/zip-safe
--rw-r--r--   0 maarten    (501) staff       (20)      983 2023-06-30 11:53:56.000000 deairequest-0.0.7/pyproject.toml
--rw-r--r--   0 maarten    (501) staff       (20)      152 2023-06-30 11:54:45.547039 deairequest-0.0.7/setup.cfg
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.209898 deairequest-0.0.8/
+-rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-07-01 06:19:18.210025 deairequest-0.0.8/PKG-INFO
+-rw-r--r--   0 maarten    (501) staff       (20)     1600 2023-06-30 11:32:54.000000 deairequest-0.0.8/README.md
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.198661 deairequest-0.0.8/deairequest/
+-rw-r--r--   0 maarten    (501) staff       (20)     7942 2023-07-01 05:54:37.000000 deairequest-0.0.8/deairequest/BacalhauProtocol.py
+-rw-r--r--   0 maarten    (501) staff       (20)     2072 2023-06-28 08:10:07.000000 deairequest-0.0.8/deairequest/DeProtocol.py
+-rw-r--r--   0 maarten    (501) staff       (20)      320 2023-06-06 08:41:48.000000 deairequest-0.0.8/deairequest/DeProtocolSelector.py
+-rw-r--r--   0 maarten    (501) staff       (20)     1594 2023-06-28 08:14:29.000000 deairequest-0.0.8/deairequest/ErrorProtocol.py
+-rw-r--r--   0 maarten    (501) staff       (20)      122 2023-05-30 07:49:58.000000 deairequest-0.0.8/deairequest/__init__.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.202136 deairequest-0.0.8/deairequest/connectors/
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:00.000000 deairequest-0.0.8/deairequest/connectors/__init__.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.209214 deairequest-0.0.8/deairequest/connectors/bacalhau/
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:59.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/__init__.py
+-rw-r--r--   0 maarten    (501) staff       (20)      826 2023-06-28 14:29:45.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/backends.py
+-rw-r--r--   0 maarten    (501) staff       (20)     2289 2023-06-26 13:55:09.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/code.py
+-rw-r--r--   0 maarten    (501) staff       (20)     6891 2023-06-30 10:20:51.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/deploy.py
+-rw-r--r--   0 maarten    (501) staff       (20)      623 2023-06-28 16:29:54.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/main.py
+-rw-r--r--   0 maarten    (501) staff       (20)    26812 2023-06-10 08:19:26.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/mapping.py
+-rw-r--r--   0 maarten    (501) staff       (20)     4795 2023-06-28 14:30:52.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/notebooks.py
+-rw-r--r--   0 maarten    (501) staff       (20)     3366 2023-07-01 05:28:17.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/querybhl.py
+-rw-r--r--   0 maarten    (501) staff       (20)     4269 2023-07-01 06:18:34.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/render.py
+-rw-r--r--   0 maarten    (501) staff       (20)    36617 2023-06-10 08:19:26.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/stdlib.py
+-rw-r--r--   0 maarten    (501) staff       (20)     2246 2023-06-26 08:46:32.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/step.py
+-rw-r--r--   0 maarten    (501) staff       (20)     1571 2023-06-06 08:59:18.000000 deairequest-0.0.8/deairequest/logo.svg
+-rw-r--r--   0 maarten    (501) staff       (20)     7484 2023-06-30 09:24:04.000000 deairequest-0.0.8/deairequest/test.ipynb
+-rw-r--r--   0 maarten    (501) staff       (20)     7325 2023-07-01 06:14:39.000000 deairequest-0.0.8/deairequest/test_DeAIRequest.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.201395 deairequest-0.0.8/deairequest.egg-info/
+-rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/PKG-INFO
+-rw-r--r--   0 maarten    (501) staff       (20)      926 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/SOURCES.txt
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/dependency_links.txt
+-rw-r--r--   0 maarten    (501) staff       (20)       12 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/top_level.txt
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-21 08:22:51.000000 deairequest-0.0.8/deairequest.egg-info/zip-safe
+-rw-r--r--   0 maarten    (501) staff       (20)      983 2023-07-01 05:56:52.000000 deairequest-0.0.8/pyproject.toml
+-rw-r--r--   0 maarten    (501) staff       (20)      152 2023-07-01 06:19:18.210482 deairequest-0.0.8/setup.cfg
```

### Comparing `deairequest-0.0.7/PKG-INFO` & `deairequest-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deairequest
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Decentralised AI library which allows to run remote AI jobs
 Author-email: Maarten Ectors <maarten@0011.ai>
 Project-URL: Homepage, https://github.com/0011ai/deairequest
 Project-URL: Bug Tracker, https://github.com/0011ai/deairequest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deairequest-0.0.7/README.md` & `deairequest-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/BacalhauProtocol.py` & `deairequest-0.0.8/deairequest/BacalhauProtocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,14 @@
         path = os.path.abspath(os.path.dirname(__file__))
         try:
             with open(os.path.join(path,"docker_images.pv"), 'a') as f:
                 f.write('%s*%s\n' % (value,pythonv))
         finally:
             f.close()
         name = value.replace("/","-")
-        print(name)
         try:
             file = open(os.path.join(path,name+".req"),'w')
             for req in reqs:
                 file.write('%s\n' % (req))
         finally:
             file.close()
         self.docker_images.append(value)
```

### Comparing `deairequest-0.0.7/deairequest/DeProtocol.py` & `deairequest-0.0.8/deairequest/DeProtocol.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/ErrorProtocol.py` & `deairequest-0.0.8/deairequest/ErrorProtocol.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/backends.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/backends.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/code.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/code.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/deploy.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/deploy.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/main.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/main.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/mapping.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/mapping.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/notebooks.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/notebooks.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/querybhl.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/querybhl.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,53 +41,56 @@
             wasm=None,
             timeout=1800,
             deal=Deal(concurrency=1, confidence=0, min_bids=0),
             do_not_track=False,
         ),
     )
 
-    try:
-        # get the python version and requirements.txt job running on the docker
-        res = submit(data)
-        # get the job id and wait until it changes from state in progress to either completed or error
-        id = res.job.metadata.id
+
+    # get the python version and requirements.txt job running on the docker
+    res = submit(data)
+    # get the job id and wait until it changes from state in progress to either completed or error
+    id = res.job.metadata.id
+    state=states(job_id=id).state.state
+    while state == 'InProgress':
         state=states(job_id=id).state.state
-        while state == 'InProgress':
-            state=states(job_id=id).state.state
-            #print('.',end='')
-            time.sleep(0.25)
-        if state=="Error":
-            raise Exception(f"Sorry but we cannot download and inspect the docker image: {docker}, please use a different docker image.")
+        #print('.',end='')
+        time.sleep(0.25)
+    
+    if state=="Error":
+        raise Exception(f"Sorry but we cannot download and inspect the docker image: {docker}, please use a different docker image.")
+    
+    # get the result of the Bacalhau job
+    resultout=results(job_id=id)
+    cid=resultout.results[0].data.cid
+    # download the CID of the outputs directory
+    try:
+        api = ipfshttpclient.connect()
+        result=api.ls(cid)
+        # get the CID of the stdout file and gets its content
+        stderrcid=result.as_json().get("Objects")[0].get("Links")[3].get("Hash")
+        # first line contains Python 3.11.2 [or other version], rest of the lines are the requirements.txt of the Docker image
+        response=api.cat(stderrcid).decode('utf-8')
+    except:
+        raise Exception(f"Sorry but we cannot download and inspect the docker image. Are you sure IPFS is running on the local machine?")
+    finally:
+        api.close()
         
-        # get the result of the Bacalhau job
-        resultout=results(job_id=id)
-        cid=resultout.results[0].data.cid
-        # download the CID of the outputs directory
-        try:
-            api = ipfshttpclient.connect()
-            result=api.ls(cid)
-            # get the CID of the stdout file and gets its content
-            stderrcid=result.as_json().get("Objects")[0].get("Links")[3].get("Hash")
-            # first line contains Python 3.11.2 [or other version], rest of the lines are the requirements.txt of the Docker image
-            response=api.cat(stderrcid).decode('utf-8')
-        finally:
-            api.close()
-        #python=response.partition('\n')[0]
-        x=re.split("Python (3.[0-9][0-9]*).[0-9]+",response.partition('\n')[0])
-        pythonversion=x[1]
-        reqtxt=response.split('\n')[1:]
-        reqs:list = []
-        for req in reqtxt:
-            if req != "":
-                y=re.split("([A-z-?]+)",req)
-                reqs.append(y[1])
-        return pythonversion, reqs
+    #python=response.partition('\n')[0]
+    x=re.split("Python (3.[0-9][0-9]*).[0-9]+",response.partition('\n')[0])
+    pythonversion=x[1]
+    reqtxt=response.split('\n')[1:]
+    reqs:list = []
+    for req in reqtxt:
+        if req != "":
+            y=re.split("([A-z-?]+)",req)
+            reqs.append(y[1])
+    return pythonversion, reqs
+
 
-    except Exception as err:
-        raise RuntimeError(f"The 'bacalhau' backend gave an error: {err}")
     
 
 def cli(argv):
     query(argv[1])
 
 if __name__ == "__main__":
     cli(sys.argv)
```

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/render.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/render.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,19 +51,19 @@
         f.close()
     try:
         with open(req) as f2:
             rforinstall = f2.read().splitlines()
     finally:
         f2.close()
 
-    toinstall={}
+    toinstall=[]
     for install in rforinstall:
         y=re.split("([A-z-?]+)",install)
         if y[1] not in lines:
-            toinstall.add(install)
+            toinstall.append(install)
 
     if len(toinstall) > 0:
         try:
             with open(req,'w') as f3:
                 for install in toinstall:
                     f3.write(install)
                     f3.write("\n")
@@ -79,16 +79,22 @@
                 subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "linux_x86_64", "-d",wheelsdir,"--only-binary=:all:",install])        
             except Exception as excep:
                 try:
                     #download any version
                     y=re.split("([A-z-?]+)",install)
                     subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "linux_x86_64", "-d",wheelsdir,"--only-binary=:all:",y[1]])        
                 except Exception as excep:
-                    # fail if neither works
-                    raise Exception(f"Sorry but we cannot download the package {install}, please use a docker image that includes this package")
+                    try:
+                        #download without dependencies
+                        y=re.split("([A-z-?]+)",install)
+                        subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "manylinux2014_x86_64", "-d",wheelsdir,"--only-binary=:all:",y[1]])        
+                    except Exception as excep:
+                        # fail if neither works
+                        raise Exception(f"Sorry but we cannot download the package {install}, please use a docker image that includes this package")
+ 
     else:
         # Nothing to install
         os.remove(req)
        
     # Deactivate the venv
     #subprocess.check_call(["deactivate"])
```

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/stdlib.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/stdlib.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/connectors/bacalhau/step.py` & `deairequest-0.0.8/deairequest/connectors/bacalhau/step.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/logo.svg` & `deairequest-0.0.8/deairequest/logo.svg`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/test.ipynb` & `deairequest-0.0.8/deairequest/test.ipynb`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/deairequest/test_DeAIRequest.py` & `deairequest-0.0.8/deairequest/test_DeAIRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -69,19 +69,58 @@
         self.assertNotEmpty(logs)
         if not exists("temp"):
             os.mkdir("temp")
         try:
             bp.get_results(job,Path("temp"))
             for directory in os.listdir(Path("temp")):
                 self.assertTrue(exists(os.path.join("temp",directory,"exitCode")))
+                try:
+                    f = open(os.path.join("temp",directory,"exitCode"),"r")
+                    self.assertEqual(f.read(),"0","Bacalhau job did not finish successfully")
+                finally:
+                    f.close()
                 self.assertTrue(exists(os.path.join("temp",directory,"stdout")))
                 self.assertTrue(exists(os.path.join("temp",directory,"stderr")))
                 self.assertTrue(exists(os.path.join("temp",directory,"outputs")))
         finally:
             shutil.rmtree("temp")
+
+        bp.add_docker_image("python:3")
+        bp.set_docker_image("python:3")
+        path = os.path.abspath(os.path.dirname(__file__))
+        job = bp.submit_job(os.path.join(path,Path("test.ipynb")))
+        self.assertNotEmpty(job)
+        state=bp.get_state(job)
+        while state=="InProgress":
+            time.sleep(0.25)
+            state=bp.get_state(job)
+        self.assertEqual(state,"Completed","Job state not working.")
+        logs = bp.get_logs(job) 
+        self.assertNotEmpty(logs)
+        if not exists("temp"):
+            os.mkdir("temp")
+        try:
+            bp.get_results(job,Path("temp"))
+            for directory in os.listdir(Path("temp")):
+                self.assertTrue(exists(os.path.join("temp",directory,"exitCode")))
+                try:
+                    f = open(os.path.join("temp",directory,"exitCode"),"r")
+                    self.assertEqual(f.read(),"0","Bacalhau job did not finish successfully")
+                finally:
+                    f.close()
+                    f = open(os.path.join("temp",directory,"stderr"),"r")
+                    print(f.readlines())
+                    f.close()
+                self.assertTrue(exists(os.path.join("temp",directory,"stdout")))
+                self.assertTrue(exists(os.path.join("temp",directory,"stderr")))
+                self.assertTrue(exists(os.path.join("temp",directory,"outputs")))
+        finally:
+            shutil.rmtree("temp")
+
+        
         
 
     def test_error_submit_job(self):
         ep = DeProtocolSelector("Error")
         with self.assertRaises(Exception) as context:
             ep.set_docker_image("test")
         self.assertTrue('Docker image not supported', context.exception)
```

### Comparing `deairequest-0.0.7/deairequest.egg-info/PKG-INFO` & `deairequest-0.0.8/deairequest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deairequest
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Decentralised AI library which allows to run remote AI jobs
 Author-email: Maarten Ectors <maarten@0011.ai>
 Project-URL: Homepage, https://github.com/0011ai/deairequest
 Project-URL: Bug Tracker, https://github.com/0011ai/deairequest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deairequest-0.0.7/deairequest.egg-info/SOURCES.txt` & `deairequest-0.0.8/deairequest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.7/pyproject.toml` & `deairequest-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deairequest"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Maarten Ectors", email="maarten@0011.ai" }
 ]
 description = "A Decentralised AI library which allows to run remote AI jobs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

