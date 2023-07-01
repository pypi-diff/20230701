# Comparing `tmp/django_cloud_storages-0.1.6.tar.gz` & `tmp/django_cloud_storages-1.1.1.tar.gz`

## Comparing `django_cloud_storages-0.1.6.tar` & `django_cloud_storages-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,27 @@
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/__init__.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/manage.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/requirements.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/setup.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/backends/appwrite.rst
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/backends/dropbox.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/settings.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/test_appwrite.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/test_dropbox.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/test_folder/test_file.txt
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/PKG-INFO
```

### Comparing `django_cloud_storages-0.1.6/cloud_storages/utils.py` & `django_cloud_storages-1.1.1/cloud_storages/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     """
     return getattr(settings, name, default)
 
 
 class FileNameLengthError(Exception):
     """Exception raised for errors when file name length is too large or too small.
     """
-    def __init__(self, min_length=None, max_length=None, message=None):
+    def __init__(self, message, min_length=None, max_length=None):
         self.min_length = min_length
         self.max_length = max_length
         self.message = message
         super().__init__(self.message)
     def __str__(self):
         return self.message
+
+class ContentDoesNotExistsError(Exception):
+    """Exception raised for errors when the requested file or folder does not exists.
+    """
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+    def __str__(self):
+        return self.message
```

### Comparing `django_cloud_storages-0.1.6/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.1.1/cloud_storages/backends/appwrite.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,16 +46,23 @@
     def _open(self, name, mode='rb'):
         folder, filename = self.extract_folder_and_filename(name)
         try:
             response = self.storage.get_file_view(folder, filename)
             data = ContentFile(response)
             remote_file = File(data)
             return remote_file
-        except Exception as e:
-            print(e)
+        except AppwriteException as e:
+            if str(e) == "Storage bucket with the requested ID could not be found.":
+                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
+                raise ContentDoesNotExistsError(error_msg)
+            elif str(e) == "The requested file could not be found.":
+                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
+                raise ContentDoesNotExistsError(error_msg)
+            else:
+                raise e
     
     def save(self, name, content, max_length=None):
         """
         Save new content to the file specified by name. The content should be
         a proper File object or any Python file-like object, ready to be read
         from the beginning.
         """
@@ -101,16 +108,15 @@
     def create_folder(self, folder):
         try:
             result = self.storage.get_bucket(folder)
         except AppwriteException as e:
             if str(e) == "Storage bucket with the requested ID could not be found.":
                 result = self.storage.create_bucket(bucket_id=folder, name=folder, permissions=[Permission.read(Role.any())], file_security=False, enabled=True, encryption=False, antivirus=False)
             else:
-                traceback.print_exc()
-                raise (e)
+                raise e
         return folder
 
     def get_available_name(self, name, content, max_length=None):
         """
         Return a filename that's free on the target storage system and
         available for new content to be written to.
         """
@@ -174,78 +180,123 @@
         # return {'file_id': updated_name, 'file_name': updated_name, 'folder_id': file_root['folder_id'], 'folder_name': file_root['folder_name']}
 
     def delete(self, name):
         """
         Delete the specified file from the storage system.
         """
         folder, filename = self.extract_folder_and_filename(name)
-        result = self.storage.delete_file(folder, filename)
+        try:
+            result = self.storage.delete_file(folder, filename)
+        except AppwriteException as e:
+            if str(e) == "Storage bucket with the requested ID could not be found.":
+                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
+                raise ContentDoesNotExistsError(error_msg)
+            elif str(e) == "The requested file could not be found.":
+                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
+                raise ContentDoesNotExistsError(error_msg)
+            else:
+                raise e
 
     def exists(self, name):
         """
         Return True if a file referenced by the given name already exists in the
         storage system, or False if the name is available for a new file.
         """
         folder, filename = self.extract_folder_and_filename(name)
         try:
             result = self.storage.get_file(folder, filename)
             return True
         except AppwriteException as e:
-            if str(e) == "The requested file could not be found.":
+            if str(e) == "The requested file could not be found." or str(e) == "Storage bucket with the requested ID could not be found.":
                 return False
             else:
-                traceback.print_exc()
-                raise(e)
+                raise e
         
     def listdir(self, path):
         """
         List the contents of the specified path. Return a 2-tuple of lists:
         the first item being directories, the second item being files.
         """
         pass
     
     def size(self, name):
         """
         Return the total size, in bytes, of the file specified by name.
         """
         folder, filename = self.extract_folder_and_filename(name)
-        result = self.storage.get_file(folder, filename)
-        return result.sizeOriginal
+        try:
+            result = self.storage.get_file(folder, filename)
+            return result.sizeOriginal
+        except AppwriteException as e:
+            if str(e) == "Storage bucket with the requested ID could not be found.":
+                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
+                raise ContentDoesNotExistsError(error_msg)
+            elif str(e) == "The requested file could not be found.":
+                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
+                raise ContentDoesNotExistsError(error_msg)
+            else:
+                raise e
     
-    def url(self, name, permanent_link=False):
+    def url(self, name, permanent_link=None):
         """
         Return an absolute URL where the file's contents can be accessed directly by a web browser.
         """
         folder, filename = self.extract_folder_and_filename(name)
-        try:
-            file_url = f"https://cloud.appwrite.io/v1/storage/buckets/{folder}/files/{filename}/view?project={self.APPWRITE_PROJECT_ID}"
-            return file_url
-        except Exception as e:
-            print(e)
-            return None
+        file_url = f"{self.APPWRITE_API_ENDPOINT}/storage/buckets/{folder}/files/{filename}/view?project={self.APPWRITE_PROJECT_ID}"
+        return file_url
     
     def get_accessed_time(self, name):
         """
         Return the last accessed time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
         folder, filename = self.extract_folder_and_filename(name)
-        result = self.storage.get_file(folder, filename)
-        return result.updatedAt
+        try:
+            result = self.storage.get_file(folder, filename)
+            return result.updatedAt
+        except AppwriteException as e:
+            if str(e) == "Storage bucket with the requested ID could not be found.":
+                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
+                raise ContentDoesNotExistsError(error_msg)
+            elif str(e) == "The requested file could not be found.":
+                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
+                raise ContentDoesNotExistsError(error_msg)
+            else:
+                raise e
 
     def get_created_time(self, name):
         """
         Return the creation time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
         folder, filename = self.extract_folder_and_filename(name)
-        result = self.storage.get_file(folder, filename)
-        return result.createdAt
+        try:
+            result = self.storage.get_file(folder, filename)
+            return result.createdAt
+        except AppwriteException as e:
+            if str(e) == "Storage bucket with the requested ID could not be found.":
+                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
+                raise ContentDoesNotExistsError(error_msg)
+            elif str(e) == "The requested file could not be found.":
+                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
+                raise ContentDoesNotExistsError(error_msg)
+            else:
+                raise e
     
     def get_modified_time(self, name):
         """
         Return the last modified time (as a datetime) of the file specified by
         name. The datetime will be timezone-aware if USE_TZ=True.
         """
         folder, filename = self.extract_folder_and_filename(name)
-        result = self.storage.get_file(folder, filename)
-        return result.updatedAt
+        try:
+            result = self.storage.get_file(folder, filename)
+            return result.updatedAt
+        except AppwriteException as e:
+            if str(e) == "Storage bucket with the requested ID could not be found.":
+                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
+                raise ContentDoesNotExistsError(error_msg)
+            elif str(e) == "The requested file could not be found.":
+                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
+                raise ContentDoesNotExistsError(error_msg)
+            else:
+                raise e
```

### Comparing `django_cloud_storages-0.1.6/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.1.1/cloud_storages/backends/dropbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 
 _DEFAULT_TIMEOUT = 100
 _DEFAULT_MODE = 'add'
 
 @deconstructible
 class DropBoxStorage(Storage):
     CHUNK_SIZE = 4 * 1024 * 1024
+    DROPBOX_PERMANENT_LINK = False
     def __init__(self):
         self.CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT = setting('CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT', False)
         self.DROPBOX_OAUTH2_ACCESS_TOKEN = setting('DROPBOX_OAUTH2_ACCESS_TOKEN')
         self.DROPBOX_OAUTH2_REFRESH_TOKEN = setting('DROPBOX_OAUTH2_REFRESH_TOKEN')
         self.DROPBOX_APP_KEY = setting('DROPBOX_APP_KEY')
         self.DROPBOX_APP_SECRET = setting('DROPBOX_APP_SECRET')
+        self.DROPBOX_PERMANENT_LINK = DROPBOX_PERMANENT_LINK = setting('DROPBOX_PERMANENT_LINK', False)
         self.DROPBOX_ROOT_PATH = setting('DROPBOX_ROOT_PATH')
         self.MEDIA_URL = setting('MEDIA_URL')
         self.timeout = setting('DROPBOX_TIMEOUT', _DEFAULT_TIMEOUT)
         self.write_mode = setting('DROPBOX_WRITE_MODE', _DEFAULT_MODE)
         self.dbx = dropbox.Dropbox(app_key=self.DROPBOX_APP_KEY, app_secret=self.DROPBOX_APP_SECRET, oauth2_refresh_token=self.DROPBOX_OAUTH2_REFRESH_TOKEN)
         self.dbx.users_get_current_account()
 
@@ -153,29 +155,29 @@
     def size(self, name):
         """
         Return the total size, in bytes, of the file specified by name.
         """
         metadata = self.dbx.files_get_metadata(name)
         return metadata.size
 
-    def url(self, name, permanent_link=False):
+    def url(self, name, permanent_link=DROPBOX_PERMANENT_LINK):
         """
         Return an absolute URL where the file's contents can be accessed directly by a web browser.
         """
         try:
             if not permanent_link:
                 media = self.dbx.files_get_temporary_link(name)
-                return media.link
+                file_url = media.link
             else:
                 dbx_share_settings = dbx_sharing.SharedLinkSettings(allow_download=True)
                 media = self.dbx.sharing_create_shared_link_with_settings(name, settings=dbx_share_settings)
                 file_url = str(media.url)[:-1]+"1"
-                return file_url
-        except ApiError:
-            return None
+            return file_url
+        except ApiError as e:
+            raise e
 
     def get_accessed_time(self, name):
         """
         Return the last accessed time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
         last_accessed = self.dbx.files_get_metadata(name).client_modified
```

### Comparing `django_cloud_storages-0.1.6/.gitignore` & `django_cloud_storages-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.6/LICENSE` & `django_cloud_storages-1.1.1/LICENSE`

 * *Files identical despite different names*

