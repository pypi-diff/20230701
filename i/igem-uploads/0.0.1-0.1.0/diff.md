# Comparing `tmp/igem-uploads-0.0.1.tar.gz` & `tmp/igem-uploads-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igem-uploads-0.0.1.tar", last modified: Sat Jul  1 17:49:36 2023, max compression
+gzip compressed data, was "igem-uploads-0.1.0.tar", last modified: Sat Jul  1 18:43:18 2023, max compression
```

## Comparing `igem-uploads-0.0.1.tar` & `igem-uploads-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 17:49:36.136651 igem-uploads-0.0.1/
--rw-r--r--   0 liang      (501) staff       (20)     1072 2023-07-01 17:46:37.000000 igem-uploads-0.0.1/LICENSE
--rw-r--r--   0 liang      (501) staff       (20)      478 2023-07-01 17:49:36.136525 igem-uploads-0.0.1/PKG-INFO
--rw-r--r--   0 liang      (501) staff       (20)       86 2023-07-01 17:46:33.000000 igem-uploads-0.0.1/README.md
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 17:49:36.135920 igem-uploads-0.0.1/igem_uploads.egg-info/
--rw-r--r--   0 liang      (501) staff       (20)      478 2023-07-01 17:49:36.000000 igem-uploads-0.0.1/igem_uploads.egg-info/PKG-INFO
--rw-r--r--   0 liang      (501) staff       (20)      244 2023-07-01 17:49:36.000000 igem-uploads-0.0.1/igem_uploads.egg-info/SOURCES.txt
--rw-r--r--   0 liang      (501) staff       (20)        1 2023-07-01 17:49:36.000000 igem-uploads-0.0.1/igem_uploads.egg-info/dependency_links.txt
--rw-r--r--   0 liang      (501) staff       (20)        6 2023-07-01 17:49:36.000000 igem-uploads-0.0.1/igem_uploads.egg-info/requires.txt
--rw-r--r--   0 liang      (501) staff       (20)        8 2023-07-01 17:49:36.000000 igem-uploads-0.0.1/igem_uploads.egg-info/top_level.txt
--rw-r--r--   0 liang      (501) staff       (20)       38 2023-07-01 17:49:36.136687 igem-uploads-0.0.1/setup.cfg
--rw-r--r--   0 liang      (501) staff       (20)      666 2023-07-01 17:49:32.000000 igem-uploads-0.0.1/setup.py
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 17:49:36.136255 igem-uploads-0.0.1/uploads/
--rw-r--r--   0 liang      (501) staff       (20)       29 2023-06-30 17:37:36.000000 igem-uploads-0.0.1/uploads/__init__.py
--rw-r--r--   0 liang      (501) staff       (20)     7244 2023-07-01 17:30:13.000000 igem-uploads-0.0.1/uploads/session.py
+drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:43:18.017032 igem-uploads-0.1.0/
+-rw-r--r--   0 liang      (501) staff       (20)    18715 2023-07-01 18:14:41.000000 igem-uploads-0.1.0/LICENSE
+-rw-r--r--   0 liang      (501) staff       (20)     1240 2023-07-01 18:43:18.016881 igem-uploads-0.1.0/PKG-INFO
+-rw-r--r--   0 liang      (501) staff       (20)      856 2023-07-01 18:37:34.000000 igem-uploads-0.1.0/README.md
+drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:43:18.016089 igem-uploads-0.1.0/igem_uploads.egg-info/
+-rw-r--r--   0 liang      (501) staff       (20)     1240 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/PKG-INFO
+-rw-r--r--   0 liang      (501) staff       (20)      244 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/SOURCES.txt
+-rw-r--r--   0 liang      (501) staff       (20)        1 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/dependency_links.txt
+-rw-r--r--   0 liang      (501) staff       (20)        6 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/requires.txt
+-rw-r--r--   0 liang      (501) staff       (20)        8 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/top_level.txt
+-rw-r--r--   0 liang      (501) staff       (20)       38 2023-07-01 18:43:18.017079 igem-uploads-0.1.0/setup.cfg
+-rw-r--r--   0 liang      (501) staff       (20)      658 2023-07-01 18:42:46.000000 igem-uploads-0.1.0/setup.py
+drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:43:18.016553 igem-uploads-0.1.0/uploads/
+-rw-r--r--   0 liang      (501) staff       (20)       29 2023-06-30 17:37:36.000000 igem-uploads-0.1.0/uploads/__init__.py
+-rw-r--r--   0 liang      (501) staff       (20)     7357 2023-07-01 18:33:27.000000 igem-uploads-0.1.0/uploads/session.py
```

### Comparing `igem-uploads-0.0.1/setup.py` & `igem-uploads-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["wheel"]
 
 setup(
     name="igem-uploads",
-    version="0.0.1",
+    version="0.1.0",
     author="lty2002",
     author_email="liangtianyi2002@outlook.com",
-    description="A package to help to manage files on igem.org",
+    description="Helps iGEMers upload their files to the iGEM server.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/iGEM-HBUT-China/igem-uploads",
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.8",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved",
     ],
 )
```

### Comparing `igem-uploads-0.0.1/uploads/session.py` & `igem-uploads-0.1.0/uploads/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             tree = etree.HTML(response.text)
             err_info = str(tree.xpath('/html/body/form/div[1]')[0].text).split('.')[0] + '.'
             warnings.warn(err_info)
             exit(1)
 
     def query(self, directory=''):
         """
-        query files/dirs in specific directory
+        query a files/dirs in specific directory
         :param directory: (optional) directory to query, default to root directory(/)
         :return: list of files, each file/dir as a dict
         """
         response = self.request('GET', f'https://shim-s3.igem.org/v1/teams/{self.team_id}/wiki?directory={directory}')
         res = response.json()
         if res['KeyCount'] > 0:
             print(directory if directory != '' else '/', 'found:', res['KeyCount'])
@@ -127,16 +127,17 @@
                 self.query(directory)
             return res.json()['location']
         else:
             warnings.warn('Upload failed' + res.text)
 
     def upload_dir(self, abs_path, directory=''):
         """
-        upload directory to specific directory
+        upload a directory and its subdirectories to specific directory
         :param abs_path: absolute path of directory
+        :param directory: (optional) target directory, default to root directory(/)
         :return: list of files, each file/dir as a dict
         """
         path_to_dir = Path(abs_path)
         if not path_to_dir.is_dir():
             warnings.warn('Invalid directory path: ' + abs_path)
             exit(1)
         file_list = os.listdir(abs_path)
@@ -168,15 +169,15 @@
             if list_files:
                 self.query(directory)
         else:
             warnings.warn(directory + '/' + filename + ' delete failed')
 
     def truncate_dir(self, directory):
         """
-        truncate directory
+        truncate a directory
         :param directory: directory to truncate
         :return: list files after truncate
         """
         contents = self.query(directory)
         for item in contents:
             if item['Type'] == 'Folder':
                 self.truncate_dir(directory + '/' + item['Name'])
```

