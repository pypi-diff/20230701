# Comparing `tmp/aws-s3-cli-0.0.5.tar.gz` & `tmp/aws-s3-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-s3-cli-0.0.5.tar", last modified: Sat Jul  1 17:52:24 2023, max compression
+gzip compressed data, was "aws-s3-cli-0.0.6.tar", last modified: Sat Jul  1 18:01:01 2023, max compression
```

## Comparing `aws-s3-cli-0.0.5.tar` & `aws-s3-cli-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.5/LICENSE
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       27 2023-06-26 16:11:47.000000 aws-s3-cli-0.0.5/MANIFEST.in
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     3083 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2293 2023-07-01 17:51:09.000000 aws-s3-cli-0.0.5/README.md
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 17:52:24.853720 aws-s3-cli-0.0.5/aws_s3_cli/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     5499 2023-07-01 17:51:54.000000 aws-s3-cli-0.0.5/aws_s3_cli/aws_s3_cli.py
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     3083 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)      232 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)        6 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/requires.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-07-01 17:52:24.000000 aws-s3-cli-0.0.5/aws_s3_cli.egg-info/top_level.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-07-01 17:52:24.857720 aws-s3-cli-0.0.5/setup.cfg
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1168 2023-07-01 17:51:20.000000 aws-s3-cli-0.0.5/setup.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 18:01:01.860939 aws-s3-cli-0.0.6/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.6/LICENSE
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       27 2023-06-26 16:11:47.000000 aws-s3-cli-0.0.6/MANIFEST.in
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     3083 2023-07-01 18:01:01.860939 aws-s3-cli-0.0.6/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2293 2023-07-01 17:51:09.000000 aws-s3-cli-0.0.6/README.md
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 18:01:01.860939 aws-s3-cli-0.0.6/aws_s3_cli/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     5484 2023-07-01 18:00:41.000000 aws-s3-cli-0.0.6/aws_s3_cli/aws_s3_cli.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-07-01 18:01:01.860939 aws-s3-cli-0.0.6/aws_s3_cli.egg-info/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     3083 2023-07-01 18:01:01.000000 aws-s3-cli-0.0.6/aws_s3_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)      232 2023-07-01 18:01:01.000000 aws-s3-cli-0.0.6/aws_s3_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-07-01 18:01:01.000000 aws-s3-cli-0.0.6/aws_s3_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        6 2023-07-01 18:01:01.000000 aws-s3-cli-0.0.6/aws_s3_cli.egg-info/requires.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-07-01 18:01:01.000000 aws-s3-cli-0.0.6/aws_s3_cli.egg-info/top_level.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-07-01 18:01:01.860939 aws-s3-cli-0.0.6/setup.cfg
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1168 2023-07-01 18:00:55.000000 aws-s3-cli-0.0.6/setup.py
```

### Comparing `aws-s3-cli-0.0.5/LICENSE` & `aws-s3-cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-s3-cli-0.0.5/PKG-INFO` & `aws-s3-cli-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `aws-s3-cli-0.0.5/README.md` & `aws-s3-cli-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aws-s3-cli-0.0.5/aws_s3_cli/aws_s3_cli.py` & `aws-s3-cli-0.0.6/aws_s3_cli/aws_s3_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,23 +119,23 @@
     upload_file_info = []
     for obj in bucket.objects.all():
       bucket_name = obj.bucket_name
       file_name = obj.key
       
       upload_file_info.append([bucket_name, file_name])
 
-    file_name_list = []
+    file_list = []
     if len(upload_file_info) != 0:
       for file_name_list in upload_file_info:
         bucket_name = file_name_list[0]
         file_name =file_name_list[1]
 
-        file_name_list.append(file_name)
+        file_list.append(file_name)
     
-    return(file_name_list)
+    return(file_list)
 
 def check_file_status(BUCKET_NAME, AWS_ACCESS_KYE, AWS_SECRET_ACCESS_KYE, S3_FILE_NAME):
     s3bucket = boto3.resource('s3',
                     aws_access_key_id=AWS_ACCESS_KYE,
                 aws_secret_access_key=AWS_SECRET_ACCESS_KYE
                 )
     bucket = s3bucket.Bucket(BUCKET_NAME)
```

### Comparing `aws-s3-cli-0.0.5/aws_s3_cli.egg-info/PKG-INFO` & `aws-s3-cli-0.0.6/aws_s3_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `aws-s3-cli-0.0.5/setup.py` & `aws-s3-cli-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md') as files:
         README = files.read()
 
     return(README)
 
 setup(
     name = 'aws-s3-cli',
-    version = '0.0.5',
+    version = '0.0.6',
     description = "upload, download, check file availability, and get all available list from AWS s3 bucket.",
     long_description = readme(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/sujitmandal/aws-s3-cli',
     author = 'Sujit Mandal',
     author_email = 'mandals974@gmail.com',
     license = 'MIT',
```

