# Comparing `tmp/keyflow-0.0.2.tar.gz` & `tmp/keyflow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyflow-0.0.2.tar", last modified: Thu Jun 29 20:33:21 2023, max compression
+gzip compressed data, was "keyflow-0.1.1.tar", last modified: Sat Jul  1 15:14:27 2023, max compression
```

## Comparing `keyflow-0.0.2.tar` & `keyflow-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:33:21.753905 keyflow-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-29 18:24:41.000000 keyflow-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4898 2023-06-29 20:33:21.751904 keyflow-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4331 2023-06-29 20:27:36.000000 keyflow-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:33:21.655909 keyflow-0.0.2/keyflow/
--rw-rw-rw-   0        0        0     8057 2023-06-29 13:59:07.000000 keyflow-0.0.2/keyflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:33:21.748908 keyflow-0.0.2/keyflow.egg-info/
--rw-rw-rw-   0        0        0     4898 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      675 2023-06-29 20:32:53.000000 keyflow-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 20:33:21.754907 keyflow-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 15:14:27.253548 keyflow-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-01 14:44:31.000000 keyflow-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4791 2023-07-01 15:14:27.250568 keyflow-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4224 2023-07-01 15:09:40.000000 keyflow-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 15:14:27.187548 keyflow-0.1.1/keyflow/
+-rw-rw-rw-   0        0        0     8184 2023-07-01 14:45:29.000000 keyflow-0.1.1/keyflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:14:27.245546 keyflow-0.1.1/keyflow.egg-info/
+-rw-rw-rw-   0        0        0     4791 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      675 2023-07-01 15:11:09.000000 keyflow-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:14:27.253548 keyflow-0.1.1/setup.cfg
```

### Comparing `keyflow-0.0.2/LICENSE` & `keyflow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keyflow-0.0.2/PKG-INFO` & `keyflow-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyflow
-Version: 0.0.2
+Version: 0.1.1
 Summary: A small python library to simulate typing in the console and custom text formatting.
 Author-email: Aneousion <sanusirry@gmail.com>
 Project-URL: Homepage, https://github.com/aneousion/keyflow
 Project-URL: Bug Tracker, https://github.com/aneousion/keyflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,15 +72,15 @@
 
 - `text` (str): The text to be displayed as a prompt.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
-- `use_pyip` (callable, optional): A function to use for input. Default is None.
+- `use_pyip` (callable, optional): A [pyinputplus](https://pypi.org/project/PyInputPlus/) function to use for input. Default is None.
 - `pyip_params` (dict, optional): Additional parameters to pass to the `use_pyip` function. Default is an empty dictionary.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
 
 
@@ -88,15 +88,14 @@
 
 
 ## License
 
 KeyFlow is released under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute this library for both commercial and non-commercial purposes. Please see the [LICENSE](https://github.com/aneousion/keyflow/LICENSE) file for more details.
 
 ## GitHub Repository
-
-The source code for KeyFlow is hosted on GitHub. You can find the repository at [https://github.com/aneousion/keyflow](https://github.com/aneousion/keyflow). Feel free to explore the repository, submit issues, and contribute to the project.
+Feel free to explore the repository, submit issues, and contribute to the project.
 
 To clone the repository, run the following command:
 
 ```bash
 git clone https://github.com/aneousion/keyflow
 ```
```

### Comparing `keyflow-0.0.2/README.md` & `keyflow-0.1.1/keyflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: keyflow
+Version: 0.1.1
+Summary: A small python library to simulate typing in the console and custom text formatting.
+Author-email: Aneousion <sanusirry@gmail.com>
+Project-URL: Homepage, https://github.com/aneousion/keyflow
+Project-URL: Bug Tracker, https://github.com/aneousion/keyflow/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # KeyFlow
 
 KeyFlow is a Python library that provides interactive console printing with a simulated typing effect and customizable text formatting. It allows you to create dynamic and engaging command-line interfaces for your Python applications.
 
 ## Features
 
 - Simulated typing effect: Display text with a realistic typing animation.
@@ -58,15 +72,15 @@
 
 - `text` (str): The text to be displayed as a prompt.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
-- `use_pyip` (callable, optional): A function to use for input. Default is None.
+- `use_pyip` (callable, optional): A [pyinputplus](https://pypi.org/project/PyInputPlus/) function to use for input. Default is None.
 - `pyip_params` (dict, optional): Additional parameters to pass to the `use_pyip` function. Default is an empty dictionary.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
 
 
@@ -74,15 +88,14 @@
 
 
 ## License
 
 KeyFlow is released under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute this library for both commercial and non-commercial purposes. Please see the [LICENSE](https://github.com/aneousion/keyflow/LICENSE) file for more details.
 
 ## GitHub Repository
-
-The source code for KeyFlow is hosted on GitHub. You can find the repository at [https://github.com/aneousion/keyflow](https://github.com/aneousion/keyflow). Feel free to explore the repository, submit issues, and contribute to the project.
+Feel free to explore the repository, submit issues, and contribute to the project.
 
 To clone the repository, run the following command:
 
 ```bash
 git clone https://github.com/aneousion/keyflow
 ```
```

### Comparing `keyflow-0.0.2/keyflow/__init__.py` & `keyflow-0.1.1/keyflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def pause_resume_typing(event):
         nonlocal stop_typing
         stop_typing = not stop_typing
 
     keyboard.on_press_key(key='Space', callback=pause_resume_typing)
 
-    for char in text:
+    for char in text.rstrip('\n'):
         if random.random() < error:
             mistyped_char = random.choice(text.replace('\n', ''))
             print(mistyped_char, end='', flush=True)
             time.sleep(random.uniform(0, speed))
             print('\b', end='', flush=True)
 
         while stop_typing:
@@ -116,14 +116,20 @@
     if retype:
         for _ in range(len(text)):
             print('\b \b', end='', flush=True)
             time.sleep(speed)
         kfprint(text=retype, speed=speed, fore_color=fore_color, back_color=back_color,
                 error=error, underline=underline, bold=bold, italics=italics)
         return
+    for i in reversed(text):
+        if i == '\n':
+            print()
+        else:
+            break
+    
    
 
 
 def _blinking_cursor_animation():
     stop_animation = False
 
     def stop_animation_callback(event):
```

### Comparing `keyflow-0.0.2/keyflow.egg-info/PKG-INFO` & `keyflow-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: keyflow
-Version: 0.0.2
-Summary: A small python library to simulate typing in the console and custom text formatting.
-Author-email: Aneousion <sanusirry@gmail.com>
-Project-URL: Homepage, https://github.com/aneousion/keyflow
-Project-URL: Bug Tracker, https://github.com/aneousion/keyflow/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # KeyFlow
 
 KeyFlow is a Python library that provides interactive console printing with a simulated typing effect and customizable text formatting. It allows you to create dynamic and engaging command-line interfaces for your Python applications.
 
 ## Features
 
 - Simulated typing effect: Display text with a realistic typing animation.
@@ -72,15 +58,15 @@
 
 - `text` (str): The text to be displayed as a prompt.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
-- `use_pyip` (callable, optional): A function to use for input. Default is None.
+- `use_pyip` (callable, optional): A [pyinputplus](https://pypi.org/project/PyInputPlus/) function to use for input. Default is None.
 - `pyip_params` (dict, optional): Additional parameters to pass to the `use_pyip` function. Default is an empty dictionary.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
 
 
@@ -88,15 +74,14 @@
 
 
 ## License
 
 KeyFlow is released under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute this library for both commercial and non-commercial purposes. Please see the [LICENSE](https://github.com/aneousion/keyflow/LICENSE) file for more details.
 
 ## GitHub Repository
-
-The source code for KeyFlow is hosted on GitHub. You can find the repository at [https://github.com/aneousion/keyflow](https://github.com/aneousion/keyflow). Feel free to explore the repository, submit issues, and contribute to the project.
+Feel free to explore the repository, submit issues, and contribute to the project.
 
 To clone the repository, run the following command:
 
 ```bash
 git clone https://github.com/aneousion/keyflow
 ```
```

### Comparing `keyflow-0.0.2/pyproject.toml` & `keyflow-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'keyboard', 'colorama']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keyflow"
-version = "0.0.2"
+version = "0.1.1"
 authors = [
   { name="Aneousion", email="sanusirry@gmail.com" },
 ]
 description = 'A small python library to simulate typing in the console and custom text formatting.'
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

