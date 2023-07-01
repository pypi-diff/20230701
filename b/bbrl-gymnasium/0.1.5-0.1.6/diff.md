# Comparing `tmp/bbrl_gymnasium-0.1.5.tar.gz` & `tmp/bbrl_gymnasium-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrl_gymnasium-0.1.5.tar", last modified: Sat Jul  1 06:44:10 2023, max compression
+gzip compressed data, was "bbrl_gymnasium-0.1.6.tar", last modified: Sat Jul  1 09:56:54 2023, max compression
```

## Comparing `bbrl_gymnasium-0.1.5.tar` & `bbrl_gymnasium-0.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.446170 bbrl_gymnasium-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 06:44:10.454170 bbrl_gymnasium-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_2D_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3027 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_line_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/debug_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/line_mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/maze_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/rocket_lander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/single_state_mdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-07-01 06:44:10.454170 bbrl_gymnasium-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/test_bbrl_gym.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/test_maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/test_rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.938261 bbrl_gymnasium-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.926261 bbrl_gymnasium-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.930261 bbrl_gymnasium-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 09:56:54.938261 bbrl_gymnasium-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.930261 bbrl_gymnasium-0.1.6/bbrl_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 09:56:54.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.934261 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/continuous_2D_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3027 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/continuous_cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/continuous_line_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/debug_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/line_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/maze_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/rocket_lander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/single_state_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.938261 bbrl_gymnasium-0.1.6/bbrl_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.934261 bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 09:56:54.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-01 09:56:54.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:56:54.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 09:56:54.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 09:56:54.000000 bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-07-01 09:56:54.938261 bbrl_gymnasium-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:54.938261 bbrl_gymnasium-0.1.6/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/tests/test_bbrl_gym.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/tests/test_maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-07-01 09:56:37.000000 bbrl_gymnasium-0.1.6/tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.1.5/.github/workflows/python-publish.yml` & `bbrl_gymnasium-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/.pre-commit-config.yaml` & `bbrl_gymnasium-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/LICENSE` & `bbrl_gymnasium-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/Makefile` & `bbrl_gymnasium-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/PKG-INFO` & `bbrl_gymnasium-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.1.5
+Version: 0.1.6
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.5/README.md` & `bbrl_gymnasium-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/__init__.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_2D_mdp.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/continuous_2D_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_cartpole.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/continuous_cartpole.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_line_mdp.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/continuous_line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/debug_env.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/debug_env.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/line_mdp.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/maze_mdp.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/maze_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/rocket_lander.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/rocket_lander.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/single_state_mdp.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/envs/single_state_mdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
-import gym
-from gym import spaces
+from gymnasium import spaces
 
 
 class SingleStateMDP(gym.Env):
     def __init__(self, A0=0.3, A1=0.9, nu=5, sigma=0.25, seed=None):
         self.action_space = spaces.Box(-1, 1, shape=(1,), dtype=np.float32)
         self.observation_space = spaces.Discrete(1)
```

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/PKG-INFO` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl-gymnasium
-Version: 0.1.5
+Version: 0.1.6
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/SOURCES.txt` & `bbrl_gymnasium-0.1.6/bbrl_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/setup.py` & `bbrl_gymnasium-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/tests/test_bbrl_gym.py` & `bbrl_gymnasium-0.1.6/tests/test_bbrl_gym.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.5/tests/test_maze.py` & `bbrl_gymnasium-0.1.6/tests/test_maze.py`

 * *Files identical despite different names*

