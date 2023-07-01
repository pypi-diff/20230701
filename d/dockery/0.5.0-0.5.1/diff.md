# Comparing `tmp/dockery-0.5.0.tar.gz` & `tmp/dockery-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.5.0.tar", last modified: Sat Jun 24 19:04:57 2023, max compression
+gzip compressed data, was "dockery-0.5.1.tar", last modified: Sat Jul  1 17:00:12 2023, max compression
```

## Comparing `dockery-0.5.0.tar` & `dockery-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1082 2023-06-24 19:04:49.346517 dockery-0.5.0/LICENSE
--rw-r--r--   0        0        0      865 2023-06-24 19:04:49.346517 dockery-0.5.0/README.md
--rw-r--r--   0        0        0      761 2023-06-24 19:04:57.986569 dockery-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/__init__.py
--rw-r--r--   0        0        0     1760 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/custom_widgets.py
--rw-r--r--   0        0        0     2767 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/dockery.py
--rw-r--r--   0        0        0     6167 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/gui.py
--rw-r--r--   0        0        0     1616 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/images.py
--rw-r--r--   0        0        0     1899 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/logs.py
--rw-r--r--   0        0        0     1763 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/networks.py
--rw-r--r--   0        0        0     1070 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/style.css
--rw-r--r--   0        0        0      881 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/utils.py
--rw-r--r--   0        0        0     1744 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/volumes.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 dockery-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-01 17:00:04.260113 dockery-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1313 2023-07-01 17:00:04.260113 dockery-0.5.1/README.md
+-rw-r--r--   0        0        0      758 2023-07-01 17:00:12.992433 dockery-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/__init__.py
+-rw-r--r--   0        0        0     1760 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/custom_widgets.py
+-rw-r--r--   0        0        0     6046 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/gui.py
+-rw-r--r--   0        0        0     1775 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/images.py
+-rw-r--r--   0        0        0     1835 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/logs.py
+-rw-r--r--   0        0        0     2767 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/main.py
+-rw-r--r--   0        0        0     1742 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/networks.py
+-rw-r--r--   0        0        0     1070 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/style.css
+-rw-r--r--   0        0        0      881 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/utils.py
+-rw-r--r--   0        0        0     1723 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/volumes.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 dockery-0.5.1/PKG-INFO
```

### Comparing `dockery-0.5.0/LICENSE` & `dockery-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.5.0/pyproject.toml` & `dockery-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.5.0"
+version = "0.5.1"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.28.0",
@@ -13,15 +13,15 @@
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
-dockery = "dockery.dockery:main"
+dockery = "dockery.main:main"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/marianocarrazana/dockery/issues"
 "Source Code" = "https://github.com/marianocarrazana/dockery"
 
 [build-system]
 requires = [
```

### Comparing `dockery-0.5.0/src/dockery/custom_widgets.py` & `dockery-0.5.1/src/dockery/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.0/src/dockery/dockery.py` & `dockery-0.5.1/src/dockery/main.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.0/src/dockery/gui.py` & `dockery-0.5.1/src/dockery/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import threading
+from textual import work
 from textual.app import App, ComposeResult
 from textual.widgets import Footer, Static, ContentSwitcher, Tabs, Tab, Label
 from textual.widgets._header import HeaderClock
 from textual.containers import (
     VerticalScroll,
     Horizontal,
     Vertical,
@@ -64,23 +64,23 @@
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_containers()
         self.set_interval(2, self.count_timer)
 
     def count_timer(self) -> None:
-        thread = threading.Thread(target=self.get_containers)
-        thread.start()
+        self.get_containers()
 
     async def watch_container_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.containers:
             cw = ContainerWidget(c, self.docker)  # type: ignore
             self.grid.mount(cw)
 
+    @work(exclusive=True)
     def get_containers(self) -> None:
         self.containers = self.docker.containers.list(all=True)
         self.container_count = len(self.containers)
 
 
 class ContainerWidget(Static):
     def __init__(self, container: Container, client: DockerClient, **kargs):
@@ -101,32 +101,32 @@
         )
 
         yield Group(StatusButtons(self.container))
 
     def on_mount(self):
         self.set_interval(1, self.data_timer)
         self.running = True
-        thread = threading.Thread(target=self.update_usage, daemon=True)
-        thread.start()
+        self.update_usage()
 
     def data_timer(self) -> None:
-        thread = threading.Thread(target=self.update_data, daemon=True)
-        thread.start()
+        self.update_data()
 
+    @work(exclusive=True)
     def update_data(self) -> None:
         try:
             self.container.reload()
         except errors.NotFound:
             return None
         else:
             status = self.container.status.capitalize()
             self.query_one("#status", ReactiveString).text = (
                 "[green]" if status == "Running" else "[bright_black]"
             ) + status
 
+    @work
     def update_usage(self) -> None:
         c = self.container
         cpu = self.query_one("#cpu", ReactiveString)
         mem = self.query_one("#mem", ReactiveString)
         for stat in c.stats(stream=True, decode=True):
             if not self.running:  # finish the thread
                 return None
```

### Comparing `dockery-0.5.0/src/dockery/images.py` & `dockery-0.5.1/src/dockery/images.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import threading
+from textual import work
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
 from textual.containers import Vertical
 from docker import DockerClient
 from docker.models.images import Image
 
@@ -18,35 +18,41 @@
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_images()
         self.set_interval(2, self.count_timer)
 
     def count_timer(self) -> None:
-        thread = threading.Thread(target=self.get_images)
-        thread.start()
+        self.get_images()
 
     async def watch_images_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.images:
             cw = ImageWidget(c, self.docker)  # type: ignore
             self.grid.mount(cw)
 
+    @work(exclusive=True)
     def get_images(self) -> None:
         self.images = self.docker.images.list(all=False)
         self.images_count = len(self.images)
 
 
 class ImageWidget(Static):
     def __init__(self, image: Image, client: DockerClient, **kargs):
         self.image = image
         self.client = client
         self.attrs = image.attrs or {}
         self.isize = self.attrs.get("Size", 0) / 1000 / 1000
+        if self.image.tags:
+            self.tag = self.image.tags[0]
+        elif self.image.id:
+            self.tag = self.image.id.replace("sha256:", "")
+        else:
+            self.tag = ""
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
         yield Vertical(
-            Label("[b]" + (self.image.tags[0] or "")),
+            Label("[b]" + self.tag),
             Label(self.image.short_id.replace("sha256:", "")),
             Label(f"Size: {self.isize:.2f}MB"),
         )
```

### Comparing `dockery-0.5.0/src/dockery/logs.py` & `dockery-0.5.1/src/dockery/logs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import threading
+from textual import work
 import time
 from textual.app import ComposeResult
 from textual.widgets import Static, TextLog, Tabs
 from textual.reactive import reactive
 from textual.containers import VerticalScroll
 from docker.models.containers import Container
 
@@ -30,27 +30,27 @@
 
     def __init__(self, container: Container, **kargs):
         self.container = container
         super().__init__(highlight=True, auto_scroll=True, wrap=True, **kargs)
 
     def on_mount(self) -> None:
         self.running = True
-        self.thread = threading.Thread(target=self.update_log, daemon=True)
-        self.thread.start()
+        self.update_log()
 
     async def watch_last_log(self, new_log: str):
         self.write(new_log)
 
+    @work
     def update_log(self) -> None:
         # Get the last 40 logs(get all logs can be slow)
         logs: bytes = self.container.logs(tail=40)
         self.last_log = logs.decode()
         # Start streaming logs(since last second)
         for log in self.container.logs(stream=True, since=time.time() - 1):
             if not self.running:
                 # Finish the thread after removing the widget
-                # TODO: it doesn't finish immediately, fix that
+                # TODO: it doesn't finish immediately? fix?
                 return None
             self.last_log = log.decode()
 
     def on_unmount(self):
         self.running = False
```

### Comparing `dockery-0.5.0/src/dockery/networks.py` & `dockery-0.5.1/src/dockery/networks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import threading
+from textual import work
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
 from textual.containers import  Vertical, Horizontal
 from docker import DockerClient
 from docker.models.networks import Network
 
@@ -18,23 +18,23 @@
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_networks()
         self.set_interval(2, self.count_timer)
 
     def count_timer(self) -> None:
-        thread = threading.Thread(target=self.get_networks)
-        thread.start()
+        self.get_networks()
 
     async def watch_networks_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.networks:
             cw = NetworkWidget(c, self.docker)  # type: ignore
             self.grid.mount(cw)
 
+    @work(exclusive=True)
     def get_networks(self) -> None:
         self.networks = self.docker.networks.list()
         self.networks_count = len(self.networks)
 
 
 class NetworkWidget(Static):
     def __init__(self, network: Network, client: DockerClient, **kargs):
```

### Comparing `dockery-0.5.0/src/dockery/style.css` & `dockery-0.5.1/src/dockery/style.css`

 * *Files identical despite different names*

### Comparing `dockery-0.5.0/src/dockery/utils.py` & `dockery-0.5.1/src/dockery/utils.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.0/src/dockery/volumes.py` & `dockery-0.5.1/src/dockery/volumes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import threading
+from textual import work
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
 from textual.containers import Vertical, Horizontal
 from docker import DockerClient
 from docker.models.volumes import Volume
 
@@ -18,23 +18,23 @@
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_volumes()
         self.set_interval(2, self.count_timer)
 
     def count_timer(self) -> None:
-        thread = threading.Thread(target=self.get_volumes)
-        thread.start()
+        self.get_volumes()
 
     async def watch_volumes_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.volumes:
             cw = VolumeWidget(c, self.docker)  # type: ignore
             self.grid.mount(cw)
 
+    @work(exclusive=True)
     def get_volumes(self) -> None:
         self.volumes = self.docker.volumes.list()
         self.volumes_count = len(self.volumes)
 
 
 class VolumeWidget(Static):
     def __init__(self, volume: Volume, client: DockerClient, **kargs):
```

### Comparing `dockery-0.5.0/PKG-INFO` & `dockery-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-Metadata-Version: 2.1
-Name: dockery
-Version: 0.5.0
-Summary: Graphical interface for Docker in your console
-Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
-License: MIT
-Project-URL: Bug tracker, https://github.com/marianocarrazana/dockery/issues
-Project-URL: Source code, https://github.com/marianocarrazana/dockery
-Requires-Python: >=3.9
-Requires-Dist: docker>=6.1.3
-Requires-Dist: textual>=0.28.0
-Requires-Dist: click>=8.1.3
-Description-Content-Type: text/markdown
-
 # dockery
 
 Graphical interface for Docker in your console
 
+[![Release](https://github.com/marianocarrazana/dockery/actions/workflows/release.yml/badge.svg)](https://github.com/marianocarrazana/dockery/actions/workflows/release.yml)
+
 <table>
   <tr>
-    <td><img src="https://github.com/marianocarrazana/dockery/assets/17238076/3c987e47-2d86-44ae-a078-73eced62dc11"/></td>
-    <td><img src="https://github.com/marianocarrazana/dockery/assets/17238076/26dc43c9-1dd0-4097-ac02-aa006c3ff6b6"/></td>
+    <td><img src="https://github.com/marianocarrazana/dockery/assets/17238076/bcff22c9-898c-4877-adac-ddf2e58007c4"/></td>
+    <td><img src="https://github.com/marianocarrazana/dockery/assets/17238076/0da0c13c-d84d-4e8a-8b6f-a0d779c2d98d"/></td>
   </tr>
   <tr>
     <td colspan="2"><img src="https://github.com/marianocarrazana/dockery/assets/17238076/c991ff4b-eebf-4495-b67c-2c57e933bd7d" /></td>
   </tr>
 </table>
 
 ## Installation
@@ -48,18 +36,21 @@
 
 Run on your console:
 
 ```shell
 dockery
 ```
 
+**Warning:** you will probably need to install and run dockery as a root user, or you can add permissions to your user to run docker following [this instructions](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user).
+
 ## Extra commands
 
 ```shell
 dockery df
 dockery ps
 dockery volumes
 dockery images
+dockery networks
 dockery stats
 ```
 
 ## **Enjoy it!**
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dockery Version: 0.5.0 Summary: Graphical interface
-for Docker in your console Author-Email: Mariano Carrazana
-gmail.com> License: MIT Project-URL: Bug tracker, https://github.com/
-marianocarrazana/dockery/issues Project-URL: Source code, https://github.com/
-marianocarrazana/dockery Requires-Python: >=3.9 Requires-Dist: docker>=6.1.3
-Requires-Dist: textual>=0.28.0 Requires-Dist: click>=8.1.3 Description-Content-
-Type: text/markdown # dockery Graphical interface for Docker in your console
+# dockery Graphical interface for Docker in your console [![Release](https://
+github.com/marianocarrazana/dockery/actions/workflows/release.yml/badge.svg)]
+(https://github.com/marianocarrazana/dockery/actions/workflows/release.yml)
 [https://github.com/marianocarrazana/  [https://github.com/marianocarrazana/
-dockery/assets/17238076/3c987e47-2d86- dockery/assets/17238076/26dc43c9-1dd0-
-44ae-a078-73eced62dc11]                4097-ac02-aa006c3ff6b6]
+dockery/assets/17238076/bcff22c9-898c- dockery/assets/17238076/0da0c13c-d84d-
+4877-adac-ddf2e58007c4]                4e8a-8b6f-a0d779c2d98d]
 [https://github.com/marianocarrazana/dockery/assets/17238076/c991ff4b-eebf-
 4495-b67c-2c57e933bd7d]
 ## Installation ### From source ```shell git clone git@github.com:
 marianocarrazana/dockery.git cd dockery pip install -e . # update only: git
 pull ``` ### From pip ```shell pip install -U dockery ``` ## Usage Run on your
-console: ```shell dockery ``` ## Extra commands ```shell dockery df dockery ps
-dockery volumes dockery images dockery stats ``` ## **Enjoy it!**
+console: ```shell dockery ``` **Warning:** you will probably need to install
+and run dockery as a root user, or you can add permissions to your user to run
+docker following [this instructions](https://docs.docker.com/engine/install/
+linux-postinstall/#manage-docker-as-a-non-root-user). ## Extra commands
+```shell dockery df dockery ps dockery volumes dockery images dockery networks
+dockery stats ``` ## **Enjoy it!**
```

