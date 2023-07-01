# Comparing `tmp/threed_optix-1.0.4.tar.gz` & `tmp/threed_optix-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-1.0.4.tar", last modified: Sat Jul  1 14:16:08 2023, max compression
+gzip compressed data, was "threed_optix-1.0.5.tar", last modified: Sat Jul  1 14:44:58 2023, max compression
```

## Comparing `threed_optix-1.0.4.tar` & `threed_optix-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:16:08.936715 threed_optix-1.0.4/
--rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 14:16:08.936715 threed_optix-1.0.4/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:36.000000 threed_optix-1.0.4/README.rst
--rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-07-01 14:16:08.936715 threed_optix-1.0.4/setup.cfg
--rw-rw-r--   0 elika     (1000) elika     (1000)      408 2023-07-01 14:15:57.000000 threed_optix-1.0.4/setup.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:16:08.936715 threed_optix-1.0.4/src/
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:16:08.936715 threed_optix-1.0.4/src/threed_optix/
--rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0.4/src/threed_optix/__init__.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     5757 2023-07-01 14:13:56.000000 threed_optix-1.0.4/src/threed_optix/api.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:16:08.936715 threed_optix-1.0.4/src/threed_optix/examples/
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0.4/src/threed_optix/examples/__init__.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     1017 2023-07-01 09:12:49.000000 threed_optix-1.0.4/src/threed_optix/examples/example_0.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     1815 2023-07-01 12:19:00.000000 threed_optix-1.0.4/src/threed_optix/examples/example_0_movie.py
--rwxrwxr-x   0 elika     (1000) elika     (1000)     2374 2023-07-01 11:27:04.000000 threed_optix-1.0.4/src/threed_optix/examples/simple.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:16:08.936715 threed_optix-1.0.4/src/threed_optix.egg-info/
--rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 14:16:08.000000 threed_optix-1.0.4/src/threed_optix.egg-info/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)      439 2023-07-01 14:16:08.000000 threed_optix-1.0.4/src/threed_optix.egg-info/SOURCES.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-07-01 14:16:08.000000 threed_optix-1.0.4/src/threed_optix.egg-info/dependency_links.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)       27 2023-07-01 14:16:08.000000 threed_optix-1.0.4/src/threed_optix.egg-info/requires.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-07-01 14:16:08.000000 threed_optix-1.0.4/src/threed_optix.egg-info/top_level.txt
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:44:58.413170 threed_optix-1.0.5/
+-rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 14:44:58.413170 threed_optix-1.0.5/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:36.000000 threed_optix-1.0.5/README.rst
+-rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-07-01 14:44:58.413170 threed_optix-1.0.5/setup.cfg
+-rw-rw-r--   0 elika     (1000) elika     (1000)      408 2023-07-01 14:44:50.000000 threed_optix-1.0.5/setup.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:44:58.413170 threed_optix-1.0.5/src/
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:44:58.413170 threed_optix-1.0.5/src/threed_optix/
+-rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0.5/src/threed_optix/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     5757 2023-07-01 14:22:21.000000 threed_optix-1.0.5/src/threed_optix/api.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:44:58.413170 threed_optix-1.0.5/src/threed_optix/examples/
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0.5/src/threed_optix/examples/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     2152 2023-07-01 14:44:27.000000 threed_optix-1.0.5/src/threed_optix/examples/example_0.py
+-rwxrwxr-x   0 elika     (1000) elika     (1000)     2374 2023-07-01 11:27:04.000000 threed_optix-1.0.5/src/threed_optix/examples/simple.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 14:44:58.413170 threed_optix-1.0.5/src/threed_optix.egg-info/
+-rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 14:44:58.000000 threed_optix-1.0.5/src/threed_optix.egg-info/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)      394 2023-07-01 14:44:58.000000 threed_optix-1.0.5/src/threed_optix.egg-info/SOURCES.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-07-01 14:44:58.000000 threed_optix-1.0.5/src/threed_optix.egg-info/dependency_links.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)       27 2023-07-01 14:44:58.000000 threed_optix-1.0.5/src/threed_optix.egg-info/requires.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-07-01 14:44:58.000000 threed_optix-1.0.5/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-1.0.4/src/threed_optix/api.py` & `threed_optix-1.0.5/src/threed_optix/api.py`

 * *Files identical despite different names*

### Comparing `threed_optix-1.0.4/src/threed_optix/examples/example_0_movie.py` & `threed_optix-1.0.5/src/threed_optix/examples/example_0.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,77 +2,79 @@
 
 
 import threed_optix.api as opt
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
 
 
-api = opt.ThreedOptixAPI('e31aeeae-e9b0-436c-abba-735ee10cee8e')
+def main():
+    api = opt.ThreedOptixAPI('e31aeeae-e9b0-436c-abba-735ee10cee8e')
 
-setups = api.get_setups()
-setup = [s for s in setups if s.name == 'setup_a'][0]
-print(f"working with '{setup}' setup")
-api.fetch(setup)
+    setups = api.get_setups()
+    setup = [s for s in setups if s.name == 'setup_a'][0]
+    print(f"working with '{setup}' setup")
+    api.fetch(setup)
+
+    part = setup.parts[1]
+    print(f"finding the focal length of '{part}'")
+    api.fetch(part)
+
+    original_z = part.pose.position.z
+
+    def run_simulation():
+        result = api.run(setup)
+        api.fetch(result)
+        data = result.data
+        data = data[data['hit_surface_idx'] == 3]
+        return data
 
-part = setup.parts[1]
-print(f"moving '{part}' part")
-api.fetch(part)
+    fig, ax = plt.subplots(figsize=(10, 10))
 
-original_z = part.pose.position.z
-
-
-def run_simulation():
-    result = api.run(setup)
-    api.fetch(result)
-    data = result.data
-    data = data[data['hit_surface_idx'] == 3]
-    return data
-
-
-data = run_simulation()
-min_x = (data['Hx'].min(), data['Hx'].max())
-min_y = (data['Hy'].min(), data['Hy'].max())
+    # to determine the ranges of axes
+    data = run_simulation()
+    minmax_x = (data['Hx'].min(), data['Hx'].max())
+    minmax_y = (data['Hy'].min(), data['Hy'].max())
 
-fig, ax = plt.subplots(figsize=(10, 10))
-frames = 60
+    areas = []
+    z_positions = []
+    n = 60
 
-areas = []
-z_positions = []
+    def animate(i):
+        ax.clear()
 
+        print(f"running simulation for z position {part.pose.position.z} ({i+1} of {n})")
+        data = run_simulation()
 
-def animate(i):
-    ax.clear()
-    print(f"running simulation for lens position {part.pose.position}")
-    data = run_simulation()
+        ax.scatter(data['Hx'], data['Hy'])
+        ax.set_title(f'z position = {part.pose.position.z}')
+        ax.set_xlabel('Hx')
+        ax.set_ylabel('Hy')
+        ax.set_xlim(minmax_x[0], minmax_x[1])
+        ax.set_ylim(minmax_y[0], minmax_y[1])
 
-    ax.scatter(data['Hx'], data['Hy'])
-    ax.set_title(f'z position = {part.pose.position.z}')
-    ax.set_xlabel('Hx')
-    ax.set_ylabel('Hy')
-    ax.set_xlim(min_x[0], min_x[1])
-    ax.set_ylim(min_y[0], min_y[1])
-
-    z_positions.append(part.pose.position.z)
-    area = (data['Hx'].max() - data['Hx'].min()) * (data['Hy'].max() - data['Hy'].min())
-    areas.append(area)
+        z_positions.append(part.pose.position.z)
+        area = (data['Hx'].max() - data['Hx'].min()) * (data['Hy'].max() - data['Hy'].min())
+        areas.append(area)
 
-    part.pose.position.z += 1
-    api.update(part)
+        part.pose.position.z += 1
+        api.update(part)
 
+    anim = animation.FuncAnimation(fig, animate, frames=n)
+    anim.save('spot.gif', writer='pillow')
 
-ani = animation.FuncAnimation(fig, animate, frames=frames)
-ani.save('scatter.gif', writer='pillow')
+    plt.close()
 
-plt.close()
+    min_area_index = areas.index(min(areas))
+    print(f"z position of minimum area: {z_positions[min_area_index]}")
 
-min_area = areas.index(min(areas))
-print(f'z position of minimum area: {z_positions[min_area]}')
+    fig, ax = plt.subplots(figsize=(10, 10))
+    ax.plot(z_positions, areas, markevery=[min_area_index], marker='o', ms=20, mec='r', mfc='None')
+    ax.set_xlabel('z position')
+    ax.set_ylabel('area')
+    plt.show()
 
-fig, ax = plt.subplots(figsize=(10, 10))
-ax.plot(z_positions, areas, markevery=[min_area], marker='o', ms=20, mec='r', mfc='None')
-ax.set_xlabel('z position')
-ax.set_ylabel('area')
-plt.show()
+    part.pose.position.z = original_z
+    api.update(part)
 
-part.pose.position.z = original_z
-api.update(part)
 
+if __name__ == '__main__':
+    main()
```

### Comparing `threed_optix-1.0.4/src/threed_optix/examples/simple.py` & `threed_optix-1.0.5/src/threed_optix/examples/simple.py`

 * *Files identical despite different names*

