# Comparing `tmp/aws-s3-cli-0.0.4.tar.gz` & `tmp/aws-s3-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-s3-cli-0.0.4.tar", last modified: Tue Jun 27 15:11:29 2023, max compression
+gzip compressed data, was "aws-s3-cli-0.0.5.tar", last modified: Sat Jul  1 17:52:24 2023, max compression
```

## Comparing `aws-s3-cli-0.0.4.tar` & `aws-s3-cli-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.4/LICENSE
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       27 2023-06-26 16:11:47.000000 aws-s3-cli-0.0.4/MANIFEST.in
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2885 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2095 2023-06-27 15:11:08.000000 aws-s3-cli-0.0.4/README.md
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/aws_s3_cli/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     4694 2023-06-26 16:11:13.000000 aws-s3-cli-0.0.4/aws_s3_cli/aws_s3_cli.py
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2885 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)      232 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)        6 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/requires.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-06-27 15:11:29.000000 aws-s3-cli-0.0.4/aws_s3_cli.egg-info/top_level.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-06-27 15:11:29.736172 aws-s3-cli-0.0.4/setup.cfg
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1168 2023-06-27 15:11:00.000000 aws-s3-cli-0.0.4/setup.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.5/LICENSE
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       27 2023-06-26 16:11:47.000000 aws-s3-cli-0.0.5/MANIFEST.in
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     3083 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2293 2023-07-01 17:51:09.000000 aws-s3-cli-0.0.5/README.md
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 17:52:24.853720 aws-s3-cli-0.0.5/aws_s3_cli/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     5499 2023-07-01 17:51:54.000000 aws-s3-cli-0.0.5/aws_s3_cli/aws_s3_cli.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     3083 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)      232 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        6 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/requires.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/top_level.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/setup.cfg
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1168 2023-07-01 17:51:20.000000 aws-s3-cli-0.0.5/setup.py
```

### Comparing `aws-s3-cli-0.0.4/LICENSE` & `aws-s3-cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-s3-cli-0.0.4/PKG-INFO` & `aws-s3-cli-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
@@ -77,14 +77,23 @@
 from aws_s3_cli.aws_s3_cli import get_all_file_list
 
 file_list = get_all_file_list(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
 
 print(file_list)
 ```
 
+## Get All File Dictionary : 
+```python
+from aws_s3_cli.aws_s3_cli import get_all_file_dict
+
+file_dict = get_all_file_dict(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
+
+print(file_dict)
+```
+
 
 ## Required package’s:
 ```
 • pip install boto3
 ```
 ## License:
 MIT Licensed
```

### Comparing `aws-s3-cli-0.0.4/README.md` & `aws-s3-cli-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -57,14 +57,23 @@
 from aws_s3_cli.aws_s3_cli import get_all_file_list
 
 file_list = get_all_file_list(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
 
 print(file_list)
 ```
 
+## Get All File Dictionary : 
+```python
+from aws_s3_cli.aws_s3_cli import get_all_file_dict
+
+file_dict = get_all_file_dict(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
+
+print(file_dict)
+```
+
 
 ## Required package’s:
 ```
 • pip install boto3
 ```
 ## License:
 MIT Licensed
```

### Comparing `aws-s3-cli-0.0.4/aws_s3_cli/aws_s3_cli.py` & `aws-s3-cli-0.0.5/aws_s3_cli/aws_s3_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     else:
         status['status'] = False
         status['message'] = 'File not found.'
        
     return(status)
 
 
-def get_all_file_list(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE):
+def get_all_file_dict(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE):
     s3bucket = boto3.resource('s3',
                     aws_access_key_id=AWS_ACCESS_KYE,
                 aws_secret_access_key=AWS_SECRET_ACCESS_KYE
                 )
     bucket = s3bucket.Bucket(BUCKET_NAME)
 
     upload_file_info = []
@@ -104,14 +104,39 @@
     else:
       file_name_dict['status'] = False
       file_name_dict['message'] = 'File not found.'
 
 
     return(file_name_dict)
 
+
+def get_all_file_list(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE):
+    s3bucket = boto3.resource('s3',
+                    aws_access_key_id=AWS_ACCESS_KYE,
+                aws_secret_access_key=AWS_SECRET_ACCESS_KYE
+                )
+    bucket = s3bucket.Bucket(BUCKET_NAME)
+
+    upload_file_info = []
+    for obj in bucket.objects.all():
+      bucket_name = obj.bucket_name
+      file_name = obj.key
+      
+      upload_file_info.append([bucket_name, file_name])
+
+    file_name_list = []
+    if len(upload_file_info) != 0:
+      for file_name_list in upload_file_info:
+        bucket_name = file_name_list[0]
+        file_name =file_name_list[1]
+
+        file_name_list.append(file_name)
+    
+    return(file_name_list)
+
 def check_file_status(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE, S3_FILE_NAME):
     s3bucket = boto3.resource('s3',
                     aws_access_key_id=AWS_ACCESS_KYE,
                 aws_secret_access_key=AWS_SECRET_ACCESS_KYE
                 )
     bucket = s3bucket.Bucket(BUCKET_NAME)
 
@@ -138,11 +163,12 @@
   FILE_OBJ = ""
   FILE_NAME = ""
   S3_FILE_NAME = ""
   BUCKET_NAME = ""
   AWS_ACCESS_KYE = ""
   AWS_SECRET_ACCESS_KYE = ""
 
+  get_all_file_dict(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
   get_all_file_list(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
   check_file_status(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE, S3_FILE_NAME)
   download_file(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE, S3_FILE_NAME, FILE_NAME)
   upload_file(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE, FILE_OBJ, FILE_NAME)
```

### Comparing `aws-s3-cli-0.0.4/aws_s3_cli.egg-info/PKG-INFO` & `aws-s3-cli-0.0.5/aws_s3_cli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
@@ -77,14 +77,23 @@
 from aws_s3_cli.aws_s3_cli import get_all_file_list
 
 file_list = get_all_file_list(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
 
 print(file_list)
 ```
 
+## Get All File Dictionary : 
+```python
+from aws_s3_cli.aws_s3_cli import get_all_file_dict
+
+file_dict = get_all_file_dict(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE)
+
+print(file_dict)
+```
+
 
 ## Required package’s:
 ```
 • pip install boto3
 ```
 ## License:
 MIT Licensed
```

### Comparing `aws-s3-cli-0.0.4/setup.py` & `aws-s3-cli-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md') as files:
         README = files.read()
 
     return(README)
 
 setup(
     name = 'aws-s3-cli',
-    version = '0.0.4',
+    version = '0.0.5',
     description = "upload, download, check file availability, and get all available list from AWS s3 bucket.",
     long_description = readme(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/sujitmandal/aws-s3-cli',
     author = 'Sujit Mandal',
     author_email = 'mandals974@gmail.com',
     license = 'MIT',
```

