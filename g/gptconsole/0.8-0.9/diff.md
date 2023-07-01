# Comparing `tmp/gptconsole-0.8.tar.gz` & `tmp/gptconsole-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptconsole-0.8.tar", last modified: Sat Jul  1 04:25:58 2023, max compression
+gzip compressed data, was "gptconsole-0.9.tar", last modified: Sat Jul  1 04:41:30 2023, max compression
```

## Comparing `gptconsole-0.8.tar` & `gptconsole-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 04:25:58.415603 gptconsole-0.8/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)    18092 2023-06-29 01:49:35.000000 gptconsole-0.8/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 04:25:58.415603 gptconsole-0.8/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      687 2023-06-29 03:19:48.000000 gptconsole-0.8/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 04:25:58.415603 gptconsole-0.8/gptconsole.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 04:25:58.000000 gptconsole-0.8/gptconsole.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      246 2023-07-01 04:25:58.000000 gptconsole-0.8/gptconsole.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2023-07-01 04:25:58.000000 gptconsole-0.8/gptconsole.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       40 2023-07-01 04:25:58.000000 gptconsole-0.8/gptconsole.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2023-07-01 04:25:58.000000 gptconsole-0.8/gptconsole.egg-info/requires.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       11 2023-07-01 04:25:58.000000 gptconsole-0.8/gptconsole.egg-info/top_level.txt
--rwxr-xr-x   0 john_vm   (1000) john_vm   (1000)     9176 2023-07-01 03:36:39.000000 gptconsole-0.8/gptconsole.py
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2023-07-01 04:25:58.415603 gptconsole-0.8/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      437 2023-07-01 04:25:54.000000 gptconsole-0.8/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 04:41:30.622310 gptconsole-0.9/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)    18092 2023-06-29 01:49:35.000000 gptconsole-0.9/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 04:41:30.622310 gptconsole-0.9/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      860 2023-07-01 04:40:43.000000 gptconsole-0.9/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 04:41:30.622310 gptconsole-0.9/gptconsole.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 04:41:30.000000 gptconsole-0.9/gptconsole.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      246 2023-07-01 04:41:30.000000 gptconsole-0.9/gptconsole.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2023-07-01 04:41:30.000000 gptconsole-0.9/gptconsole.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       40 2023-07-01 04:41:30.000000 gptconsole-0.9/gptconsole.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2023-07-01 04:41:30.000000 gptconsole-0.9/gptconsole.egg-info/requires.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       11 2023-07-01 04:41:30.000000 gptconsole-0.9/gptconsole.egg-info/top_level.txt
+-rwxr-xr-x   0 john_vm   (1000) john_vm   (1000)     9229 2023-07-01 04:28:31.000000 gptconsole-0.9/gptconsole.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2023-07-01 04:41:30.622310 gptconsole-0.9/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      437 2023-07-01 04:41:17.000000 gptconsole-0.9/setup.py
```

### Comparing `gptconsole-0.8/LICENSE` & `gptconsole-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gptconsole-0.8/gptconsole.py` & `gptconsole-0.9/gptconsole.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def __init__(self):
         self.api_interface = OpenAIInterface()
         self.editor_command = None
         self.base_path = None
 
     def load_config(self):
         home = os.getenv('HOME')
-        config_path = os.path.join(home, '.yagptclirc')
+        config_path = os.path.join(home, '.gptconsolerc')
         with open(config_path, 'r') as f:
             config = json.load(f)
         self.base_path = config['base_path']
         self.editor_command = config['editor_command']
         self.temporary_dir = config['temporary_dir']
         self.api_interface.set_api_key(config['api_key'])
 
@@ -110,27 +110,29 @@
                 os.system('clear')
 
             elif command == r'\history':
                 self.api_interface.history.print_contents()
 
             elif command == r'\multiline':
                 user_input = self.get_multiline_input()
+                print(f"> {user_input}")
                 self.process_query(user_input)
 
             elif command == r'\docstring':
                 user_input = self.get_multiline_input()
+                print(f"> {user_input}")
                 user_input = (
                     "Write a high-quality elaborate docstring "
                     "for the following function/method. "
                     "Only show the text of the docstring, "
                     f"and nothing else:\n```\n{user_input}\n```\n")
                 self.process_query(user_input)
 
             elif command == r'\rm':
-                self.api_interface.history.contents.remove_most_recent_message()
+                self.api_interface.history.remove_most_recent_message()
 
             elif command == r'\clear_name':
                 self.api_interface.history.name = None
 
             else:
                 print(f'Invalid command: {user_input}')
 
@@ -194,15 +196,15 @@
 
         except FileNotFoundError:
             print(f'File not found: {file_path}. Please check the path and retry.')
 
     def get_multiline_input(self):
         os.system(f'rm -rf {self.temporary_dir}chatgpttempfile')
         os.system(f'{self.editor_command} {self.temporary_dir}chatgpttempfile')
-        with open('{self.temporary_dir}chatgpttempfile', 'r', encoding='utf-8') as f:
+        with open(f'{self.temporary_dir}chatgpttempfile', 'r', encoding='utf-8') as f:
             user_input = f.read()
         os.system(f'rm -rf {self.temporary_dir}chatgpttempfile')
 
         return user_input
 
     def get_appropriate_name(self):
         suggested_name = self.api_interface.get_response(
@@ -268,13 +270,11 @@
     if '\n' in text:
         print('\n\n\n---\n')
         print(text)
         print('\n---\n\n\n')
     else:
         print(text)
 
-def main():
-    cli = CommandLineInterface()
-    cli.run(sys.argv[1:])
 
 if __name__ == '__main__':
-    main()
+    cli = CommandLineInterface()
+    cli.run(sys.argv[1:])
```

