# Comparing `tmp/unigui-1.5.3.tar.gz` & `tmp/unigui-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.5.3.tar", last modified: Wed Jun 21 23:53:28 2023, max compression
+gzip compressed data, was "dist/unigui-1.5.4.tar", last modified: Sat Jul  1 14:25:04 2023, max compression
```

## Comparing `unigui-1.5.3.tar` & `unigui-1.5.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13651 2023-06-21 23:43:02.000000 unigui-1.5.3/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.5.3/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.3/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.5.3/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.3/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/css/vendor.49a52e8f.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/css/361.c9159919.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    43129 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/361.78add75c.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/app.6ab35062.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.3/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      600 2023-06-21 23:51:38.000000 unigui-1.5.3/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19442 2023-06-21 23:53:28.000000 unigui-1.5.3/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-21 23:53:28.000000 unigui-1.5.3/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19137 2023-06-21 23:49:27.000000 unigui-1.5.3/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.3/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19442 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.3/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1205 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13116 2023-07-01 14:21:18.000000 unigui-1.5.4/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.5.4/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.4/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.5.4/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.4/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/css/vendor.49a52e8f.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/css/361.c9159919.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    43129 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/361.78add75c.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/app.6ab35062.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.4/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-01 14:22:35.000000 unigui-1.5.4/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19997 2023-07-01 14:25:04.000000 unigui-1.5.4/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-01 14:25:04.000000 unigui-1.5.4/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19692 2023-07-01 14:05:35.000000 unigui-1.5.4/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.4/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19997 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.4/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.5.3/unigui/manager.py` & `unigui-1.5.4/unigui/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import sys
 import asyncio
 import requests
 from threading import Thread
 
 users = {}
 
-sing2method = {'=':'changed', '->':'update','?':'complete','+':'append', '-':'delete', '!':'editing', '#':'modify'}    
+sign2method = {'=':'changed', '->':'update','?':'complete','+':'append', '-':'delete', '!':'editing', '#':'modify'}    
 
-#loop and thread for progress functionality
+#loop and thread is only for progress window functionality
 loop = asyncio.new_event_loop()
 def f(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever() 
 
 t = Thread(target=f, args=(loop,))
 t.start()  
@@ -34,18 +34,15 @@
         self.history_switching = []
         self.history_pointer = 0        
 
         self.oper_count = 0
         self.time_last_change = time.time()
         self.max_oper_time = 0.1  
 
-        self.tool_buttons = [Button('_Back', icon='arrow_back',changed=self.go_back, tooltip = 'Go back'), 
-            Button('_Forward', icon='arrow_forward',changed=self.go_forward, tooltip = 'Go forward'),
-            Button('_Undo', icon='undo', tooltip = 'Undo last operation',changed = self.undo_last_operation),
-            Button('_Redo', icon='redo', tooltip = 'Redo last operation',changed = self.redo_last_operation)]
+        self.tool_buttons = []
 
     def append_change(self, change):
         self.change_buffer.append(change)
         curr_time = time.time()
         if curr_time - self.time_last_change > self.max_oper_time:
             self.oper_count += 1
             self.redo_buffer = [] #clean redo if new operation
@@ -148,59 +145,57 @@
 
     def load(self):   
         screen_vars = {
             'icon' : 'article',
             'prepare' : None,
             'dispatch' : None,
             'blocks' : [],
-            'header' : utils.appname,            
-            'save' : self.save_changes,
+            'header' : utils.appname,                        
             'toolbar' : None
         }     
          
         blocks_dir = 'blocks'        
         screens_dir =  'screens'
         modules = {}
         for file in os.listdir(screens_dir):
             if file.endswith(".py") and file != '__init__.py':
                 name = file[0:-3]
 
                 #if name not in modules:                    
                 path = f'{screens_dir}/{file}'                
                 spec = importlib.util.spec_from_file_location(name,path)
                 module = importlib.util.module_from_spec(spec)
-                modules[name] = module, spec
-                #else:
-                #    module, spec = modules[name]
+                modules[name] = module, spec                
                 
-                utils.clean_handlers()
-                spec.loader.exec_module(module)            
+                utils.clean_handlers()                                
+                
+                module.user = self                               
                 
-                screen = Screen(module.name)
-                module.screen = screen 
-                module.user = self               
+                spec.loader.exec_module(module)            
+
+                screen = Screen(module.name)     
+                module.screen = screen            
                 self.screens.append(module)
+
                 #set system vars
                 for var in screen_vars:                                            
                     setattr(screen, var, getattr(module,var,screen_vars[var])) 
                 screen.handlers__ = utils.handlers__
                 
                 if not screen.toolbar:
-                    screen.toolbar = [*self.tool_buttons, Button('_Save model', icon='cloud_upload', 
-                        tooltip = 'Save to disk',changed = screen.save)]
+                    screen.toolbar = self.tool_buttons
                                 
                 screen.check()                         
-                #del sys.modules[name]       
         
         self.screens.sort(key=lambda s: s.order)
         main = self.screens[0]
         if 'prepare' in dir(main):
             main.prepare()
         self.screen_module = main
-        self.menu = [[s.name,s.icon] for s in self.screens]        
+        self.menu = [[s.name,getattr(s,'icon', None)] for s in self.screens]        
 
         #remove user modules from sys for repeating loading for new users
         for file in os.listdir(blocks_dir):
             if file.endswith(".py") and file != '__init__.py':
                 name = f'{blocks_dir}.{file[0:-3]}'
                 if name in sys.modules:
                     sys.modules[name].user = self
@@ -301,15 +296,15 @@
                 return res
             elem = res.elem
             arr = res.arr                            
         
     def process_element(self, elem, arr):        
         id = arr.pop() if len(arr) == 5 else 0
         sign = arr[-2]
-        smeth = sing2method.get(sign)
+        smeth = sign2method.get(sign)
         val = arr[-1]
         if smeth:
             handler = self.screen.handlers__.get((elem, smeth))
             if handler:
                 result = handler(elem, val)                
                 return result
```

### Comparing `unigui-1.5.3/unigui/guielements.py` & `unigui-1.5.4/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/server.py` & `unigui-1.5.4/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/utils.py` & `unigui-1.5.4/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/favicon.ico` & `unigui-1.5.4/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.5.4/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/css/361.c9159919.css` & `unigui-1.5.4/unigui/web/css/361.c9159919.css`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/icons/favicon-96x96.png` & `unigui-1.5.4/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/icons/favicon-16x16.png` & `unigui-1.5.4/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/icons/favicon-32x32.png` & `unigui-1.5.4/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/icons/favicon-128x128.png` & `unigui-1.5.4/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.5.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.5.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/js/361.78add75c.js` & `unigui-1.5.4/unigui/web/js/361.78add75c.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/js/430.591e9a73.js` & `unigui-1.5.4/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/js/app.6ab35062.js` & `unigui-1.5.4/unigui/web/js/app.6ab35062.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/js/193.283445be.js` & `unigui-1.5.4/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.5.4/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/unigui/web/index.html` & `unigui-1.5.4/unigui/web/index.html`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/LICENSE` & `unigui-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.5.3/setup.py` & `unigui-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.5.3',      
+      version='1.5.4',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.5.3/PKG-INFO` & `unigui-1.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.3
+Version: 1.5.4
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -29,18 +29,18 @@
 Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
-name = "Main" #name of screen to show
-icon = 'blur_linear' #MD icon of screen to show
-order = 0 #order in the program menu
-blocks = [block] #what to show on the screen
+name = "Main"
+icon = 'blur_linear' 
+order = 0 
+blocks = [block] 
 ```
 The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
@@ -48,15 +48,26 @@
 block = Block('X Block',
     [           
         Button('Clean table', icon = 'swipe'),
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
-#### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
+| Screen global variables |	Status | Description |
+| :---: | :---: | :---: | 
+| name  | Has to be defined | Unique screen name |
+| order | Has to be defined | order in the program menu |
+| blocks | Has to be defined | which blocks to show on the screen |
+| user   | Always defined, read-only | Access to User(inherited) class which associated with a current user |
+| header | Optional | show it instead of app name |
+| toolbar | Optional | Gui elements to show in the screen toolbar |
+| icon  | Optional | MD icon of screen to show in screen menu |
+| dispatch | Optional | Screen handlers for catching gui signals. Has signature def dispatch(gui, signal) |
+| prepare | Optional | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing has a signature 'def prepare()' |
+
 
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
 #app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app')
```

### Comparing `unigui-1.5.3/README.md` & `unigui-1.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
-name = "Main" #name of screen to show
-icon = 'blur_linear' #MD icon of screen to show
-order = 0 #order in the program menu
-blocks = [block] #what to show on the screen
+name = "Main"
+icon = 'blur_linear' 
+order = 0 
+blocks = [block] 
 ```
 The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
@@ -36,15 +36,26 @@
 block = Block('X Block',
     [           
         Button('Clean table', icon = 'swipe'),
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
-#### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
+| Screen global variables |	Status | Description |
+| :---: | :---: | :---: | 
+| name  | Has to be defined | Unique screen name |
+| order | Has to be defined | order in the program menu |
+| blocks | Has to be defined | which blocks to show on the screen |
+| user   | Always defined, read-only | Access to User(inherited) class which associated with a current user |
+| header | Optional | show it instead of app name |
+| toolbar | Optional | Gui elements to show in the screen toolbar |
+| icon  | Optional | MD icon of screen to show in screen menu |
+| dispatch | Optional | Screen handlers for catching gui signals. Has signature def dispatch(gui, signal) |
+| prepare | Optional | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing has a signature 'def prepare()' |
+
 
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
 #app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app')
```

### Comparing `unigui-1.5.3/unigui.egg-info/PKG-INFO` & `unigui-1.5.4/unigui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.3
+Version: 1.5.4
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -29,18 +29,18 @@
 Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
-name = "Main" #name of screen to show
-icon = 'blur_linear' #MD icon of screen to show
-order = 0 #order in the program menu
-blocks = [block] #what to show on the screen
+name = "Main"
+icon = 'blur_linear' 
+order = 0 
+blocks = [block] 
 ```
 The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
@@ -48,15 +48,26 @@
 block = Block('X Block',
     [           
         Button('Clean table', icon = 'swipe'),
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
-#### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
+| Screen global variables |	Status | Description |
+| :---: | :---: | :---: | 
+| name  | Has to be defined | Unique screen name |
+| order | Has to be defined | order in the program menu |
+| blocks | Has to be defined | which blocks to show on the screen |
+| user   | Always defined, read-only | Access to User(inherited) class which associated with a current user |
+| header | Optional | show it instead of app name |
+| toolbar | Optional | Gui elements to show in the screen toolbar |
+| icon  | Optional | MD icon of screen to show in screen menu |
+| dispatch | Optional | Screen handlers for catching gui signals. Has signature def dispatch(gui, signal) |
+| prepare | Optional | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing has a signature 'def prepare()' |
+
 
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
 #app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app')
```

### Comparing `unigui-1.5.3/unigui.egg-info/SOURCES.txt` & `unigui-1.5.4/unigui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

