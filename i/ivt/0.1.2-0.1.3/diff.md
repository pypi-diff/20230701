# Comparing `tmp/ivt-0.1.2.tar.gz` & `tmp/ivt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivt-0.1.2.tar", last modified: Fri Jun 16 06:48:15 2023, max compression
+gzip compressed data, was "ivt-0.1.3.tar", last modified: Sat Jul  1 06:36:11 2023, max compression
```

## Comparing `ivt-0.1.2.tar` & `ivt-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1123 2023-06-05 09:53:24.916313 ivt-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2097 2022-12-26 08:46:33.368156 ivt-0.1.2/.gitignore
--rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.2/LICENSE
--rw-r--r--   0        0        0      776 2023-06-05 10:57:06.577472 ivt-0.1.2/README.md
--rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.2/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.2/docs/_templates/page.html
--rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.2/docs/conf.py
--rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.2/docs/core_install.rst
--rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.2/docs/core_intro.rst
--rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.2/docs/forward_intro.rst
--rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.2/docs/index.rst
--rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.2/docs/inverse_intro.rst
--rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.2/docs/plugin_refs.rst
--rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.2/docs/requirements.txt
--rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.2/docs/teaser.png
--rw-r--r--   0        0        0      269 2023-06-16 06:42:43.435704 ivt-0.1.2/ivt/__init__.py
--rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.2/ivt/config.py
--rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.2/ivt/connector.py
--rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.2/ivt/connectors/__init__.py
--rw-r--r--   0        0        0    14632 2023-06-11 09:51:02.554002 ivt-0.1.2/ivt/connectors/psdr_jit_connector.py
--rw-r--r--   0        0        0     5051 2023-06-09 21:50:08.990124 ivt-0.1.2/ivt/io.py
--rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.2/ivt/loss.py
--rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.2/ivt/model.py
--rw-r--r--   0        0        0     1908 2023-06-07 05:21:51.299496 ivt-0.1.2/ivt/parameter.py
--rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.2/ivt/renderer.py
--rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.2/ivt/sampling.py
--rw-r--r--   0        0        0     6132 2023-06-11 09:21:37.011237 ivt-0.1.2/ivt/scene.py
--rw-r--r--   0        0        0     3042 2023-06-07 05:24:56.148994 ivt-0.1.2/ivt/transform.py
--rw-r--r--   0        0        0      499 2023-06-16 06:40:23.588718 ivt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 ivt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-06-23 02:53:28.491095 ivt-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2174 2023-07-01 06:32:29.559569 ivt-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.3/LICENSE
+-rw-r--r--   0        0        0      776 2023-06-23 02:53:28.491598 ivt-0.1.3/README.md
+-rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.3/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.3/docs/_templates/page.html
+-rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.3/docs/conf.py
+-rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.3/docs/core_install.rst
+-rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.3/docs/core_intro.rst
+-rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.3/docs/forward_intro.rst
+-rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.3/docs/index.rst
+-rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.3/docs/inverse_intro.rst
+-rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.3/docs/plugin_refs.rst
+-rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.3/docs/teaser.png
+-rw-r--r--   0        0        0      269 2023-07-01 06:32:29.561078 ivt-0.1.3/ivt/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.3/ivt/config.py
+-rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.3/ivt/connector.py
+-rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.3/ivt/connectors/__init__.py
+-rw-r--r--   0        0        0    14825 2023-07-01 06:32:29.562578 ivt-0.1.3/ivt/connectors/psdr_jit_connector.py
+-rw-r--r--   0        0        0     5051 2023-06-23 02:53:28.526107 ivt-0.1.3/ivt/io.py
+-rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.3/ivt/loss.py
+-rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.3/ivt/model.py
+-rw-r--r--   0        0        0     1908 2023-06-23 02:53:28.527105 ivt-0.1.3/ivt/parameter.py
+-rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.3/ivt/renderer.py
+-rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.3/ivt/sampling.py
+-rw-r--r--   0        0        0     7098 2023-07-01 06:32:29.563079 ivt-0.1.3/ivt/scene.py
+-rw-r--r--   0        0        0     3589 2023-07-01 06:32:29.564578 ivt-0.1.3/ivt/transform.py
+-rw-r--r--   0        0        0      533 2023-07-01 06:34:46.759478 ivt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 ivt-0.1.3/PKG-INFO
```

### Comparing `ivt-0.1.2/.github/workflows/python-publish.yml` & `ivt-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/.gitignore` & `ivt-0.1.3/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# For project_template
+project_template/data
+project_template/results
+
+# Temp output in examples
+examples/**/*.png
+examples/**/*.exr
+examples/**/*.obj
+
+# Don't ignore files in examples/data
+!examples/data
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -125,17 +137,9 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
-# Temporary directories
-tmp_output/
-
-# Temp directories in pipelines
-examples/cached_scenes
-examples/results
-examples/target_images
-
 # VSCode
 .vscode
```

### Comparing `ivt-0.1.2/LICENSE` & `ivt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/README.md` & `ivt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/docs/_static/theme_overrides.css` & `ivt-0.1.3/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/docs/conf.py` & `ivt-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/docs/index.rst` & `ivt-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/docs/teaser.png` & `ivt-0.1.3/docs/teaser.png`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/connector.py` & `ivt-0.1.3/ivt/connector.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/connectors/psdr_jit_connector.py` & `ivt-0.1.3/ivt/connectors/psdr_jit_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from drjit.scalar import Array3f
 from drjit.cuda import Array3f as Vector3fC, Array3i as Vector3iC
 from drjit.cuda.ad import Array3f as Vector3fD, Float32 as FloatD, Matrix4f as Matrix4fD, Matrix3f as Matrix3fD
 from drjit.cuda.ad import Float32 as FloatD
 import torch
 
 import time
+import os
 
 class Timer:
     def __init__(self, label):
         self.label = label
 
     def __enter__(self):
         self.start_time = time.time()
@@ -199,37 +200,41 @@
         mat_id = mesh['mat_id']
         if mat_id not in scene:
             raise RuntimeError(f"The material of the mesh {name} doesn't exist: mat_id={mat_id}")
         brdf = scene[mat_id]
         PSDRJITConnector.extensions[type(brdf)](mat_id, scene)
 
         # TODO: Fix this workaround when psdr-jit updates psdr_mesh.load_raw()
-        write_obj('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'], mesh['fuv'])
-        psdr_emitter = psdr_jit.AreaLight(mesh['radiance']) if mesh['is_emitter'] else None
-        psdr_scene.add_Mesh('__psdr_jit_tmp__.obj', mesh['to_world'].reshape(1, 4, 4), mat_id, psdr_emitter)
-
-        # psdr_mesh = psdr_jit.Mesh()
-        # psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
-        # psdr_mesh.use_face_normal = mesh['use_face_normal']
+        if mesh['can_change_topology']:
+            psdr_mesh = psdr_jit.Mesh()
+            psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
+            psdr_mesh.use_face_normal = mesh['use_face_normal']
 
-        # psdr_emitter = psdr_jit.AreaLight(mesh['radiance'].tolist()) if mesh['is_emitter'] else None
-        # psdr_scene.add_Mesh(psdr_mesh, mat_id, psdr_emitter)
+            psdr_emitter = psdr_jit.AreaLight(mesh['radiance'].tolist()) if mesh['is_emitter'] else None
+            psdr_scene.add_Mesh(psdr_mesh, mat_id, psdr_emitter)
+        else:
+            write_obj('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'], mesh['fuv'])
+            psdr_emitter = psdr_jit.AreaLight(mesh['radiance']) if mesh['is_emitter'] else None
+            psdr_scene.add_Mesh('__psdr_jit_tmp__.obj', mesh['to_world'].reshape(1, 4, 4), mat_id, psdr_emitter)
+            os.remove('__psdr_jit_tmp__.obj')
         
         cache['name_map'][name] = f"Mesh[{psdr_scene.num_meshes - 1}]"
 
     psdr_mesh = psdr_scene.param_map[cache['name_map'][name]]
 
     # Update parameters
     updated = mesh.get_updated()
     if len(updated) > 0:
         for param_name in updated:
-            if param_name == 'v' or param_name == 'f':
-                psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
-                # psdr_mesh.vertex_positions = Vector3fC(mesh['v'])
-                # psdr_mesh.face_indices = Vector3iC(mesh['f'])
+            if param_name == 'v':
+                if mesh['can_change_topology']:
+                    psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
+                else:
+                    psdr_mesh.vertex_positions = Vector3fC(mesh['v'])
+                    psdr_mesh.face_indices = Vector3iC(mesh['f'])
 
             mesh.params[param_name]['updated'] = False
 
     # Enable grad for parameters requiring grad
     drjit_params = []
     requiring_grad = mesh.get_requiring_grad()
     if len(requiring_grad) > 0:
```

### Comparing `ivt-0.1.2/ivt/io.py` & `ivt-0.1.3/ivt/io.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/loss.py` & `ivt-0.1.3/ivt/loss.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/model.py` & `ivt-0.1.3/ivt/model.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/parameter.py` & `ivt-0.1.3/ivt/parameter.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/renderer.py` & `ivt-0.1.3/ivt/renderer.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/sampling.py` & `ivt-0.1.3/ivt/sampling.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.2/ivt/scene.py` & `ivt-0.1.3/ivt/scene.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .parameter import ParamGroup
-from .transform import lookat
+from .transform import lookat, perspective, batched_transform_pos, batched_transform_dir
 from .io import read_image, read_obj, to_torch_f, to_torch_i
 
 from collections import OrderedDict
 
 import torch
+import torch.nn.functional as F
 
 class Scene:
 
     def __init__(self) -> None:
         self.components = OrderedDict()
         self.requiring_grad = ()
         self.cached = {}
@@ -51,14 +52,17 @@
     
     def clear_cache(self):
         self.cached = {}
         # Detach the tensors requiring grad
         for param_name in self.requiring_grad:
             self[param_name] = self[param_name].detach()
 
+    def filter(self, component_type):
+        return [cname for cname in self.components if component_type == type(self.components[cname])]
+
 class Integrator(ParamGroup):
 
     def __init__(self, type, config):
         super().__init__()
         
         self.add_param('type', type, help_msg='integrator type')
         self.add_param('config', config, help_msg='integrator config')
@@ -77,45 +81,54 @@
         super().__init__()
 
         self.add_param('fov', fov, help_msg='sensor fov')
         self.add_param('near', near, help_msg='sensor near clip')
         self.add_param('far', far, help_msg='sensor far clip')
         self.add_param('to_world', to_torch_f(to_world), is_tensor=True, is_diff=True, help_msg='sensor to_world matrix')
 
+    def get_rays(self, samples, aspect_ratio):
+        samples = torch.cat([samples, torch.zeros_like(samples)[:, 0:1]], dim=1)
+        sample_to_camera = torch.inverse(perspective(self['fov'], aspect_ratio, self['near'], self['far']))
+        rays_o = batched_transform_pos(self['to_world'], to_torch_f([[0, 0, 0]]))
+        rays_d = F.normalize(batched_transform_pos(sample_to_camera, samples), dim=1)
+        rays_d = batched_transform_dir(self['to_world'], rays_d)
+        return rays_o.repeat(samples.shape[0], 1), rays_d
+
     @classmethod
     def from_lookat(cls, fov, origin, target, up, near=1e-6, far=1e7):
         sensor = cls(fov, torch.eye(4), near, far)
         origin = to_torch_f(origin)
         target = to_torch_f(target)
         up = to_torch_f(up)
         sensor['to_world'] = lookat(origin, target, up)
         return sensor
         
 class Mesh(ParamGroup):
 
-    def __init__(self, v, f, uv, fuv, mat_id, to_world=torch.eye(4), use_face_normal=True, radiance=torch.zeros(3)):
+    def __init__(self, v, f, uv, fuv, mat_id, to_world=torch.eye(4), use_face_normal=True, can_change_topology=False, radiance=torch.zeros(3)):
         super().__init__()
         
         self.add_param('v', to_torch_f(v), is_tensor=True, is_diff=True, help_msg='mesh vertex positions')
         self.add_param('f', to_torch_i(f), is_tensor=True, help_msg='mesh face indices')
         self.add_param('uv', to_torch_f(uv), is_tensor=True, help_msg='mesh uv coordinates')
         self.add_param('fuv', to_torch_i(fuv), is_tensor=True, help_msg='mesh uv face indices')
         self.add_param('mat_id', mat_id, help_msg='name of the material of the mesh')
         self.add_param('to_world', to_torch_f(to_world), is_tensor=True, help_msg='mesh to world matrix')
         self.add_param('use_face_normal', use_face_normal, help_msg='whether to use face normal')
+        self.add_param('can_change_topology', can_change_topology, help_msg='whether to the topology can be chagned')
 
         radiance = to_torch_f(radiance)
         is_emitter = radiance.sum() > 0
         self.add_param('is_emitter', is_emitter, help_msg='whether it is used as an emitter')
         self.add_param('radiance', radiance, is_tensor=True, is_diff=True, help_msg='radiance if it is used as an emitter')
 
     @classmethod
-    def from_file(cls, filename, mat_id, to_world=torch.eye(4), use_face_normal=True, radiance=torch.zeros(3)):
+    def from_file(cls, filename, mat_id, to_world=torch.eye(4), use_face_normal=True, can_change_topology=False, radiance=torch.zeros(3)):
         v, tc, n, f, ftc, fn = read_obj(filename)
-        return cls(v, f, tc, ftc, mat_id, to_world, use_face_normal, radiance)
+        return cls(v, f, tc, ftc, mat_id, to_world, use_face_normal, can_change_topology, radiance)
     
 class DiffuseBRDF(ParamGroup):
 
     def __init__(self, d):
         super().__init__()
         
         self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
```

### Comparing `ivt-0.1.2/ivt/transform.py` & `ivt-0.1.3/ivt/transform.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,25 +15,39 @@
     to_world[:3, 0] = left
     to_world[:3, 1] = new_up
     to_world[:3, 2] = dir
     to_world[:3, 3] = origin
 
     return to_world
 
-def perspective(fov, near=1e-6, far=1e7):
+def perspective(fov, aspect_ratio, near=1e-6, far=1e7):
     recip = 1 / (far - near)
     tan = torch.tan(torch.deg2rad(to_torch_f(fov * 0.5)))
     cot = 1 / tan
 
     mat = torch.diag(to_torch_f([cot, cot, far * recip, 0]))
     mat[2, 3] = -near * far * recip
     mat[3, 2] = 1
 
+    mat = scale([-0.5, -0.5 * aspect_ratio, 1]) @ translate([-1, -1 / aspect_ratio, 0]) @ mat
+
     return mat
 
+def batched_transform_pos(mat, vec):
+    mat = mat.view(1, 4, 4)
+    vec = vec.view(-1, 3, 1)
+    tmp = (mat @ torch.cat([vec, torch.ones_like(vec)[:, 0:1]], dim=1)).reshape(-1, 4)
+    return tmp[:, 0:3] / tmp[:, 3:]
+
+def batched_transform_dir(mat, vec):
+    mat = mat.view(1, 4, 4)
+    vec = vec.view(-1, 3, 1)
+    tmp = (mat @ torch.cat([vec, torch.zeros_like(vec)[:, 0:1]], dim=1)).reshape(-1, 4)
+    return tmp[:, 0:3]
+
 def translate(t_vec):
     t_vec = to_torch_f(t_vec)
 
     to_world = to_torch_f(torch.eye(4))
     to_world[:3, 3] = t_vec
 
     return to_world
```

### Comparing `ivt-0.1.2/PKG-INFO` & `ivt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Inverse-Rendering Toolkit
 Author-email: Guangyan Cai <gcai3@uci.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: imageio >= 2.27.0
 Requires-Dist: numpy
 Requires-Dist: gin-config
```

