# Comparing `tmp/bbrl_gymnasium-0.1.4.tar.gz` & `tmp/bbrl_gymnasium-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrl_gymnasium-0.1.4.tar", last modified: Sun Jun 18 16:39:41 2023, max compression
+gzip compressed data, was "bbrl_gymnasium-0.1.5.tar", last modified: Sat Jul  1 06:44:10 2023, max compression
```

## Comparing `bbrl_gymnasium-0.1.4.tar` & `bbrl_gymnasium-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/bbrl_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_2D_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3027 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_line_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/debug_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/line_mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/maze_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/rocket_lander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/test_bbrl_gym.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/test_maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/test_rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.446170 bbrl_gymnasium-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 06:44:10.454170 bbrl_gymnasium-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_2D_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3027 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_line_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/debug_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/line_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/maze_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/rocket_lander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/single_state_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 06:44:10.000000 bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-07-01 06:44:10.454170 bbrl_gymnasium-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:44:10.450170 bbrl_gymnasium-0.1.5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/test_bbrl_gym.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/test_maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-07-01 06:43:59.000000 bbrl_gymnasium-0.1.5/tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.1.4/.github/workflows/python-publish.yml` & `bbrl_gymnasium-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/LICENSE` & `bbrl_gymnasium-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/Makefile` & `bbrl_gymnasium-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/PKG-INFO` & `bbrl_gymnasium-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.4/README.md` & `bbrl_gymnasium-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/__init__.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,22 @@
 )
 register(
     id="RocketLander-v0",
     entry_point="bbrl_gymnasium.envs:RocketLanderEnv",
     max_episode_steps=1000,
     reward_threshold=0,
 )
-register(id="MazeMDP-v0", entry_point="bbrl_gymnasium.envs:MazeMDPEnv", max_episode_steps=1000)
-register(id="DebugV-v0", entry_point="bbrl_gymnasium.envs:DebugVEnv", max_episode_steps=10)
+register(
+    id="MazeMDP-v0",
+    entry_point="bbrl_gymnasium.envs:MazeMDPEnv",
+    max_episode_steps=1000
+)
+register(
+    id="DebugV-v0",
+    entry_point="bbrl_gymnasium.envs:DebugVEnv",
+    max_episode_steps=10
+)
+register(
+    id="SingleStateMDP-v0",
+    entry_point="bbrl_gymnasium.envs:SingleStateMDP",
+    max_episode_steps=3000
+)
```

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_2D_mdp.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_2D_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_cartpole.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_cartpole.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_line_mdp.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/continuous_line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/debug_env.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/debug_env.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/line_mdp.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/maze_mdp.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/maze_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/rocket_lander.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/envs/rocket_lander.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/PKG-INFO` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl-gymnasium
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/SOURCES.txt` & `bbrl_gymnasium-0.1.5/bbrl_gymnasium.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
@@ -19,13 +20,14 @@
 bbrl_gymnasium/envs/continuous_2D_mdp.py
 bbrl_gymnasium/envs/continuous_cartpole.py
 bbrl_gymnasium/envs/continuous_line_mdp.py
 bbrl_gymnasium/envs/debug_env.py
 bbrl_gymnasium/envs/line_mdp.py
 bbrl_gymnasium/envs/maze_mdp.py
 bbrl_gymnasium/envs/rocket_lander.py
+bbrl_gymnasium/envs/single_state_mdp.py
 bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
 bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
 tests/__init__.py
 tests/test_bbrl_gym.py
 tests/test_maze.py
 tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.1.4/setup.py` & `bbrl_gymnasium-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/tests/test_bbrl_gym.py` & `bbrl_gymnasium-0.1.5/tests/test_bbrl_gym.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.4/tests/test_maze.py` & `bbrl_gymnasium-0.1.5/tests/test_maze.py`

 * *Files identical despite different names*

