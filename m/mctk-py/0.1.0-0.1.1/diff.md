# Comparing `tmp/mctk-py-0.1.0.tar.gz` & `tmp/mctk-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctk-py-0.1.0.tar", last modified: Fri May 12 19:25:49 2023, max compression
+gzip compressed data, was "mctk-py-0.1.1.tar", last modified: Sat Jul  1 03:02:11 2023, max compression
```

## Comparing `mctk-py-0.1.0.tar` & `mctk-py-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.575613 mctk-py-0.1.0/
--rw-rw-rw-   0        0        0      301 2023-05-12 19:18:05.000000 mctk-py-0.1.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0     8611 2023-05-12 18:58:08.000000 mctk-py-0.1.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-03-26 20:44:55.000000 mctk-py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      437 2023-05-12 18:58:08.000000 mctk-py-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2536 2023-05-12 18:58:08.000000 mctk-py-0.1.0/Makefile
--rw-rw-rw-   0        0        0    19450 2023-05-12 19:25:49.574754 mctk-py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5501 2023-05-12 18:58:08.000000 mctk-py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.562757 mctk-py-0.1.0/mctk/
--rw-rw-rw-   0        0        0      401 2023-05-12 19:18:05.000000 mctk-py-0.1.0/mctk/__init__.py
--rw-rw-rw-   0        0        0    13476 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/checking.py
--rw-rw-rw-   0        0        0    12714 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/models.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.565756 mctk-py-0.1.0/mctk/tests/
--rw-rw-rw-   0        0        0    10327 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/tests/test_checking.py
--rw-rw-rw-   0        0        0    12318 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/tests/test_models.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.572757 mctk-py-0.1.0/mctk_py.egg-info/
--rw-rw-rw-   0        0        0    19450 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2216 2023-05-12 19:18:05.000000 mctk-py-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 19:25:49.575613 mctk-py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-03-02 23:40:15.000000 mctk-py-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:02:11.925000 mctk-py-0.1.1/
+-rw-rw-rw-   0        0        0      418 2023-07-01 02:46:45.000000 mctk-py-0.1.1/.bumpversion.cfg
+-rw-rw-rw-   0        0        0     8611 2023-05-12 18:58:08.000000 mctk-py-0.1.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-03-26 20:44:55.000000 mctk-py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      437 2023-05-12 18:58:08.000000 mctk-py-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2536 2023-06-26 17:58:42.000000 mctk-py-0.1.1/Makefile
+-rw-rw-rw-   0        0        0    20734 2023-07-01 03:02:11.923999 mctk-py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6785 2023-06-30 20:43:05.000000 mctk-py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 03:02:11.911999 mctk-py-0.1.1/mctk/
+-rw-rw-rw-   0        0        0      401 2023-07-01 02:46:45.000000 mctk-py-0.1.1/mctk/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-01 01:24:47.000000 mctk-py-0.1.1/mctk/checking.py
+-rw-rw-rw-   0        0        0    19136 2023-07-01 01:30:00.000000 mctk-py-0.1.1/mctk/models.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:02:11.914996 mctk-py-0.1.1/mctk/tests/
+-rw-rw-rw-   0        0        0    11766 2023-06-30 20:43:05.000000 mctk-py-0.1.1/mctk/tests/test_checking.py
+-rw-rw-rw-   0        0        0    15809 2023-06-30 20:43:05.000000 mctk-py-0.1.1/mctk/tests/test_models.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:02:11.922997 mctk-py-0.1.1/mctk_py.egg-info/
+-rw-rw-rw-   0        0        0    20734 2023-07-01 03:02:11.000000 mctk-py-0.1.1/mctk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-07-01 03:02:11.000000 mctk-py-0.1.1/mctk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 03:02:11.000000 mctk-py-0.1.1/mctk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2023-07-01 03:02:11.000000 mctk-py-0.1.1/mctk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-01 03:02:11.000000 mctk-py-0.1.1/mctk_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2216 2023-07-01 02:46:45.000000 mctk-py-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 03:02:11.925997 mctk-py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-03-02 23:40:15.000000 mctk-py-0.1.1/setup.py
```

### Comparing `mctk-py-0.1.0/CONTRIBUTING.md` & `mctk-py-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mctk-py-0.1.0/LICENSE` & `mctk-py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mctk-py-0.1.0/Makefile` & `mctk-py-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `mctk-py-0.1.0/PKG-INFO` & `mctk-py-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctk-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Model Checking Toolkit for Python
 Author-email: marcusm117 <marcusmin117@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -231,15 +231,15 @@
 
 Users can use functions that implements CTL operators to formally verify if a Kripke Structure (can be created during runtime or input in a JSON file) satisfies certain CTL properties. All checking functions will return a set of states that satisfy the CTL property, which means that if any start state of the Kripke Structure is in the returned set, then the Kripke Structure satisfies the CTL property.
 
 ## Getting Started
 
 ### Installation
 
-Get the latest version of `mctk` from PyPI. Note that the registered name is 'mctk-py' on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as 'mctk'.
+Get the latest version of `mctk` from PyPI. Note that the registered name is `mctk-py` on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as `mctk`.
 
    ``` bash
    pip3 install mctk-py
    ```
 
 If you are having trouble with `pip3`, you can also install from the source code, see [Developing](#developing).
 
@@ -271,43 +271,42 @@
 - `make lint`: perform static analysis of this library with `black`, `flake8` and `pylint`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 ## Usage
 
-Create a Krinke Structure from scratch.
+### Create a Kripke Structure from Scratch
 
 ``` python
 from mctk import *
 
 # create a Kripke Structure from scratch
 ks = KripkeStruct()
 
 # set 2 Atomic Propositions in this Kripke Structure
 ks.set_atoms(["p", "q"])
 
 # add 2 states to the Kripke Structure
 # a State Name is represented by a string, it must be unique
-# a State Label is represented by a binary number, it must be unique
-# for example, 0b10 means the state has the Atoms "p" but not "q"
-ks.add_state("s0", 0b10)
-ks.add_state("s1", 0b01)
+# a State Label is represented by a list of Atoms, it must be unique
+ks.add_state("s0", ["p"])
+ks.add_state("s1", ["q"])
 
 # set the Start States of the Kripke Structure
 # there can be multiple Start States
 ks.set_starts(["s0"])
 
 # add 2 Transitions to the Kripke Structure
 # a Transition is represented by a key-value pair
 # where key the Source State Name and value is a list of Destination State Names
 ks.add_trans({"s0": ["s1"], "s1": ["s0"]})
 ```
 
-Check if the Kripke Structure satisfies a simple CTL formula.
+### Checking Simple CTL Formula on the Kripke Structure
 
 ``` python
 # check if the Kripke Structure satisfies the CTL formula: EX p
 # SAT_atom(ks, "p") returns a set of states that satisfy the Atomic Proposition p
 # EX returns a set of states that satisfy the CTL formula EX p
 sat_states = EX(ks, SAT_atom(ks, "p"))
 
@@ -322,15 +321,15 @@
 sat_states = EU(ks, SAT_atom(ks, "p"), SAT_atom(ks, "q"))
 
 # the result should be {"s0", "s1"}
 # since the start state "s0" is in sat_states, ks satisfies the CTL formula
 assert sat_states == {"s0", "s1"}
 ```
 
-Check if the Kripke Structure satisfies a composite CTL formula.
+### Checking Composite CTL Formula on the Kripke Structure
 
 ``` python
 # check if the Kripke Structure satisfies the CTL formula: EX (p AND EX q)
 sat_states = EX(ks, AND(SAT_atom(ks, "p"), EX(ks, SAT_atom(ks, "q"))))
 
 # the result should be {"s1"}
 # since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
@@ -340,12 +339,61 @@
 sat_states = EG(ks, AU(ks, SAT_atom(ks, "p"), NOT(ks, SAT_atom(ks, "q"))))
 
 # the result should be set(), empty set
 # since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
 assert sat_states == set()
 ```
 
+### Checking CTL formula on a Complex Kripke Structure
+
+``` python
+ks_json = {
+   "Atoms": ["a", "b", "c", "d"],
+   "States": {
+      "s1": ["a"],
+      "s2": ["a", "b"],
+      "s3": ["b", "c"],
+      "s4": ["b", "c", "d"],
+      "s5": ["b"],
+      "s6": ["c"],
+      "s7": ["d"],
+   },
+   "Starts": ["s1"],
+   "Trans": {
+      's1': ['s2'],
+      's2': ['s3', 's4'],
+      's3': ['s4'],
+      's4': ['s7'],
+      's5': ['s6'],
+      's6': ['s7', 's5'],
+      's7': ['s5'],
+   },
+}
+ks = KripkeStruct(ks_json)
+
+# check if the Kripke Structure satisfies the CTL formula: EX a
+sat_states = EX(ks, SAT_atom(ks, "a"))
+
+# the result should be {"s1"}
+# since the start state "s1" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {"s1"}
+
+# check if the Kripke Structure satisfies the CTL formula: E a U b
+sat_states = EU(ks, SAT_atom(ks, "a"), SAT_atom(ks, "b"))
+
+# the result should be {'s1', 's2', 's3', 's4', 's5'}
+# since the start state "s1" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {'s1', 's2', 's3', 's4', 's5'}
+
+# check if the Kripke Structure satisfies the CTL formula: EG a
+sat_states = EG(ks, SAT_atom(ks, "a"))
+
+# the result should be set()
+# since the start state "s1" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == set()
+```
+
 ## Contributing
 
 All contrbutions are welcome!
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details.
```

### Comparing `mctk-py-0.1.0/README.md` & `mctk-py-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Users can use functions that implements CTL operators to formally verify if a Kripke Structure (can be created during runtime or input in a JSON file) satisfies certain CTL properties. All checking functions will return a set of states that satisfy the CTL property, which means that if any start state of the Kripke Structure is in the returned set, then the Kripke Structure satisfies the CTL property.
 
 ## Getting Started
 
 ### Installation
 
-Get the latest version of `mctk` from PyPI. Note that the registered name is 'mctk-py' on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as 'mctk'.
+Get the latest version of `mctk` from PyPI. Note that the registered name is `mctk-py` on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as `mctk`.
 
    ``` bash
    pip3 install mctk-py
    ```
 
 If you are having trouble with `pip3`, you can also install from the source code, see [Developing](#developing).
 
@@ -50,43 +50,42 @@
 - `make lint`: perform static analysis of this library with `black`, `flake8` and `pylint`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 ## Usage
 
-Create a Krinke Structure from scratch.
+### Create a Kripke Structure from Scratch
 
 ``` python
 from mctk import *
 
 # create a Kripke Structure from scratch
 ks = KripkeStruct()
 
 # set 2 Atomic Propositions in this Kripke Structure
 ks.set_atoms(["p", "q"])
 
 # add 2 states to the Kripke Structure
 # a State Name is represented by a string, it must be unique
-# a State Label is represented by a binary number, it must be unique
-# for example, 0b10 means the state has the Atoms "p" but not "q"
-ks.add_state("s0", 0b10)
-ks.add_state("s1", 0b01)
+# a State Label is represented by a list of Atoms, it must be unique
+ks.add_state("s0", ["p"])
+ks.add_state("s1", ["q"])
 
 # set the Start States of the Kripke Structure
 # there can be multiple Start States
 ks.set_starts(["s0"])
 
 # add 2 Transitions to the Kripke Structure
 # a Transition is represented by a key-value pair
 # where key the Source State Name and value is a list of Destination State Names
 ks.add_trans({"s0": ["s1"], "s1": ["s0"]})
 ```
 
-Check if the Kripke Structure satisfies a simple CTL formula.
+### Checking Simple CTL Formula on the Kripke Structure
 
 ``` python
 # check if the Kripke Structure satisfies the CTL formula: EX p
 # SAT_atom(ks, "p") returns a set of states that satisfy the Atomic Proposition p
 # EX returns a set of states that satisfy the CTL formula EX p
 sat_states = EX(ks, SAT_atom(ks, "p"))
 
@@ -101,15 +100,15 @@
 sat_states = EU(ks, SAT_atom(ks, "p"), SAT_atom(ks, "q"))
 
 # the result should be {"s0", "s1"}
 # since the start state "s0" is in sat_states, ks satisfies the CTL formula
 assert sat_states == {"s0", "s1"}
 ```
 
-Check if the Kripke Structure satisfies a composite CTL formula.
+### Checking Composite CTL Formula on the Kripke Structure
 
 ``` python
 # check if the Kripke Structure satisfies the CTL formula: EX (p AND EX q)
 sat_states = EX(ks, AND(SAT_atom(ks, "p"), EX(ks, SAT_atom(ks, "q"))))
 
 # the result should be {"s1"}
 # since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
@@ -119,12 +118,61 @@
 sat_states = EG(ks, AU(ks, SAT_atom(ks, "p"), NOT(ks, SAT_atom(ks, "q"))))
 
 # the result should be set(), empty set
 # since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
 assert sat_states == set()
 ```
 
+### Checking CTL formula on a Complex Kripke Structure
+
+``` python
+ks_json = {
+   "Atoms": ["a", "b", "c", "d"],
+   "States": {
+      "s1": ["a"],
+      "s2": ["a", "b"],
+      "s3": ["b", "c"],
+      "s4": ["b", "c", "d"],
+      "s5": ["b"],
+      "s6": ["c"],
+      "s7": ["d"],
+   },
+   "Starts": ["s1"],
+   "Trans": {
+      's1': ['s2'],
+      's2': ['s3', 's4'],
+      's3': ['s4'],
+      's4': ['s7'],
+      's5': ['s6'],
+      's6': ['s7', 's5'],
+      's7': ['s5'],
+   },
+}
+ks = KripkeStruct(ks_json)
+
+# check if the Kripke Structure satisfies the CTL formula: EX a
+sat_states = EX(ks, SAT_atom(ks, "a"))
+
+# the result should be {"s1"}
+# since the start state "s1" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {"s1"}
+
+# check if the Kripke Structure satisfies the CTL formula: E a U b
+sat_states = EU(ks, SAT_atom(ks, "a"), SAT_atom(ks, "b"))
+
+# the result should be {'s1', 's2', 's3', 's4', 's5'}
+# since the start state "s1" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {'s1', 's2', 's3', 's4', 's5'}
+
+# check if the Kripke Structure satisfies the CTL formula: EG a
+sat_states = EG(ks, SAT_atom(ks, "a"))
+
+# the result should be set()
+# since the start state "s1" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == set()
+```
+
 ## Contributing
 
 All contrbutions are welcome!
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details.
```

### Comparing `mctk-py-0.1.0/mctk/checking.py` & `mctk-py-0.1.1/mctk/checking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Authors: marcusm117
 # License: Apache 2.0
-"""This Module currently contains functions for Explicit-State Model Checking CTL properties on the class KripkeStruct.
+"""This Module contains functions for Explicit-State Model Checking CTL properties on the class KripkeStruct.
 
 We plan to support Symbolic Model Checking and Bounded Model Checking in the future.
 
 Examples:
     >>> from mctk import *
     >>> ks_json = {
-    ...     "Atoms": ("a", "b", "c", "d"),
+    ...     "Atoms": ["a", "b", "c", "d"],
     ...     "States": {
     ...         "s1": 0b1000,  # s1 has labels "a"
     ...         "s2": 0b1100,  # s2 has labels "a", "b"
     ...         "s3": 0b0110,  # s3 has labels "b", "c"
     ...         "s4": 0b0111,  # s4 has labels "b", "c", "d"
     ...         "s5": 0b0100,  # s5 has label "b"
     ...         "s6": 0b0010,  # s6 has label "c"
@@ -59,38 +59,39 @@
 def SAT_atom(ks: KripkeStruct, atomic_property: str) -> Set[str]:
     """Evaluate an atomic propositional property on a Kripke Structure.
 
     Return a set of states where the atomic propositional property is satisfied.
 
     Args:
         ks: a Kripke Structure
-        atomic_property: an atomic propositional property represented as a string
+        atomic_property: an Atomic Propositional Property represented as a string
 
     Returns:
-        a set of states where the atomic propositional property is satisfied
+        a set of states where the Atomic Propositional Property is satisfied
 
     Raises:
-        KripkeStructError: if the atomic property is not in the Kripke Structure
+        KripkeStructError: if the Atomic Property is not in the Kripke Structure
 
     """
     sat_states = set()
+    state_names = ks.get_state_names()
 
     if atomic_property == "True":
-        return set(ks.states.keys())
+        return state_names
     if atomic_property == "False":
         return set()
-    if atomic_property not in ks.atoms:
+    if atomic_property not in ks.get_atoms():
         raise KripkeStructError("Can't check on an atom that's not in the Kripke Structure")
 
-    for state in ks.states:
-        # get the set of labels for the state
-        label_set = ks.get_state_label_set(state)
+    for state in state_names:
+        # get the Label for the State Name, which is a set of atoms
+        label = ks.get_label_of_state(state)
 
-        # if the atomic property is in the Label Set, then this state satisfies the atomic property
-        if atomic_property in label_set:
+        # if the atomic property is in the Label, then this state satisfies the atomic property
+        if atomic_property in label:
             sat_states.add(state)
 
     return sat_states
 
 
 def NOT(ks: KripkeStruct, property1: Set[str]) -> Set[str]:
     """Implement the NOT operator on a CTL property.
@@ -102,15 +103,15 @@
         property: a CTL property represented as a set of states that satisfy the property
 
     Returns:
         a set of states where the CTL formula "NOT property" is satisfied
 
     """
     # complement of the set
-    return set(ks.states.keys()) - property1
+    return ks.get_state_names() - property1
 
 
 def AND(property1: Set[str], property2: Set[str]) -> Set[str]:
     """Implement the AND operator on two CTL properties.
 
     Return a set of states where the CTL formula "property1 AND property2" is satisfied.
 
@@ -193,17 +194,17 @@
 
     Returns:
         a set of states where the CTL formula "EX property" is satisfied
 
     """
     sat_states = set()
 
-    for state in ks.states:
+    for state in ks.get_states():
         # get the successors of the state
-        successors = ks.trans[state]
+        successors = ks.get_trans()[state]
 
         for successor in successors:
             # test if the successors satisfy the property
             if successor in property1:
                 sat_states.add(state)
 
     return sat_states
@@ -249,15 +250,15 @@
     # until we reach a fixed point
     # i.e. no new states are added to "sat_states"
     # i.e. size of "sat_states" does not change
     while True:
         # get the predecessors of all states in "sat_states"
         predecessors = set()
         for state in sat_states:
-            predecessors = predecessors | set(ks.trans_inverted[state])
+            predecessors = predecessors | ks.get_trans_inverted()[state]
 
         # add states that can reach "sat_states" in 1 step, and also satisfy property1
         sat_states = sat_states | (property1 & predecessors)
 
         # if no new states are added, then we have reached a fixed point
         new_size = len(sat_states)
         if new_size == size:
@@ -277,15 +278,15 @@
         property: a CTL property represented as a set of states that satisfy the property
 
     Returns:
         a set of states where the CTL formula "EF property" is satisfied
 
     """
     # EF p = E true U p
-    return EU(ks, set(ks.states.keys()), property1)
+    return EU(ks, ks.get_state_names(), property1)
 
 
 def AG(ks: KripkeStruct, property1: Set[str]) -> Set[str]:
     """Implement the AG operator on a CTL property.
 
     Return a set of states where the CTL formula "AG property" is satisfied.
 
@@ -316,15 +317,15 @@
     """
     sat_states = set()
 
     # creat a sub-graph of the original Kripke Structure ks
     # where we remove all states that do not satisfy property
     # since we need to modify the reversed graph, we create a deepcopy of self
     sub_graph = deepcopy(ks)
-    for state in ks.states:
+    for state in ks.get_states():
         if state not in property1:
             sub_graph.remove_state(state)
 
     # compute all Strongly Connected Components (SCCs) of the sub-graph
     # SCCs is a set of SCCs, where each SCC is a set of states
     SCCs = sub_graph.get_SCCs()
 
@@ -342,15 +343,15 @@
     # i.e. no new states are added to "sat_states"
     # i.e. size of "sat_states" does not change
     size = len(sat_states)
     while True:
         # get the predecessors of all states in "sat_states"
         predecessors = set()
         for state in sat_states:
-            predecessors = predecessors | set(sub_graph.trans_inverted[state])
+            predecessors = predecessors | sub_graph.get_trans_inverted()[state]
 
         # add states that can reach "sat_states" in 1 step
         sat_states = sat_states | predecessors
 
         # if no new states are added, then we have reached a fixed point
         new_size = len(sat_states)
         if new_size == size:
```

### Comparing `mctk-py-0.1.0/mctk/models.py` & `mctk-py-0.1.1/mctk/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,194 +1,311 @@
 # Authors: marcusm117
 # License: Apache 2.0
-"""This Module currently contains a class KripkeStruct, which is a graph implementation of Kripke Structures.
+"""This Module contains a class KripkeStruct, which is a graph implementation of Kripke Structures.
 
 We plan to support other Transition Systems as well in the future.
 
 """
 
 # Standard Libraries
-from typing import List, Dict, Set
-from collections import defaultdict
+from typing import List, Dict, Set, Tuple
+from collections import defaultdict, UserDict
 from copy import deepcopy
 
 
 class KripkeStructError(Exception):
-    """Exceptions raised by all instance functions in class KripkeStruct.
-
-    Raised when trying to reset Atoms after States are Created
-    Raised when trying to add an Exisiting State Name again
-    Raised when trying to add an Exisiting State Label again
-    Raised when trying to get the Label Set of a Non-Exisiting State
-    Raised when trying to perform model checking on a Non-Exisiting Atom
-    Raised when trying set a Non-Exisiting State as Start State
-    Raised when trying to add Transition from a Non-Exisiting Source State
-    Raised when trying to add Transition to a Non-Exisiting Target State
-
-    """
+    """Exceptions raised by methods related to class KripkeStruct."""
 
 
 class KripkeStruct:
     """Class that implements a Kripke Structure for Model Checking.
 
     An instance of thie class can be created from a JSON file or from scratch.
     For more information about Kripke Structures, see:
     https://en.wikipedia.org/wiki/Kripke_structure_(model_checking).
 
     Attributes:
-        atoms (tuple): Atoms
-        states (dict): States, Key is the state name, Value is the state label
-        starts (set): Start States
-        trans (defaultdict): Transitions, Key is the source state, Value is a list of target states
-        trans_inverted (defaultdict): Inverted Transitions, Key is the target state, Value is a list of source states
+        _atoms (tuple): Atoms, can only be reset before any state is created
+        _atoms_set (set): Atoms, a duplicate of "_atoms", only for efficiency
+        _states (_UniqueValueDict): States, Key is the state name, Value is the state label
+        _starts (set): Start States
+        _trans (defaultdict): Transitions, Key is the source state, Value is a set of target states
+        _trans_inverted (defaultdict): Inverted Transitions, Key is the target state, Value is a set of source states
 
     """
 
     def __init__(self, model_json=None):
-        self.atoms = ()
-        self.states = {}
-        self.starts = set()
-        self.trans = defaultdict(list)
-        self.trans_inverted = defaultdict(list)
+        self._atoms = ()
+        self._atoms_set = set()
+        self._states = self._KripkeStateDict()
+        self._starts = set()
+        self._trans = defaultdict(set)
+        self._trans_inverted = defaultdict(set)
 
         if model_json is not None:
             self.set_atoms(model_json["Atoms"])
             self.add_states(model_json["States"])
             self.set_starts(model_json["Starts"])
             self.add_trans(model_json["Trans"])
 
+    class _KripkeStateDict(UserDict):
+        def __init__(self, atoms_num: int = 0):
+            self.atoms_num = atoms_num
+            super().__init__()
+
+        def __setitem__(self, key, value):
+            # if the value is already assigned to the key, do nothing
+            if (key in self) and (self.__getitem__(key) == value):
+                return
+
+            # if the value is NOT an int, raise an error
+            if not isinstance(value, int):
+                raise KripkeStructError("The a State Label should be an int, when assigning with []")
+
+            # if the value exceeds 2^n, where n is the number of atoms, raise an error
+            if value >= 2**self.atoms_num:
+                raise KripkeStructError("The value should be less than 2^n, where n is the number of atoms")
+
+            # if the value is already assigned to a different key, raise an error
+            # no matter if the key exists or not
+            if value in self.values():
+                raise KripkeStructError("Can't assign an existing State Label to a different State Name")
+
+            super().__setitem__(key, value)
+
     def __str__(self) -> str:
         return (
-            f"Atoms: {self.atoms}\n"
-            + f"States: {self.states}\n"
-            + f"Starts: {self.starts}\n"
-            + f"Trans: {dict(self.trans)}"
+            f"Atoms: {self._atoms}\n"
+            + f"States: {dict(self._states)}\n"
+            + f"Starts: {self._starts}\n"
+            + f"Trans: {dict(self._trans)}"
         )
 
     def set_atoms(self, atoms: List[str]) -> None:
         """Set Atoms of the Kripke Structure.
 
         Args:
             atoms: a list of strings representing the Atoms
 
         Raises:
             KripkeStructError: if any state exists, can't reset atoms
 
+        Note:
+            The parameter "atoms" should be a list to stay compatible with the JSON format.
+            However, internally, the field "_atoms" is stored as a tuple for efficiency.
+
         """
         # if any state exists, can't reset atoms
-        if self.states:
+        if self._states:
             raise KripkeStructError("Can't reset Atoms after States are Created")
-        self.atoms = tuple(atoms)
+        self._atoms = tuple(atoms)
+        self._atoms_set = set(atoms)
+        self._states.atoms_num = len(atoms)
 
-    def get_atoms(self) -> List[str]:
+    def get_atoms(self) -> Tuple[str]:
         """Get Atoms of the Kripke Structure.
 
         Returns:
-            a list of strings representing the Atoms
+            a tuple of strings representing the Atoms
 
         """
-        return list(self.atoms)
+        return self._atoms
 
-    def add_state(self, state: str, label: int) -> None:
+    def add_state(self, state: str, label: List[str]) -> None:
         """Add a State to the Kripke Structure.
 
-        The State Label is represented by an integer.
-        Its binary form of which indicates which Atoms are ture for this State.
-        For example, if the Atoms are ("p", "q", "r"),
-        and a State Label is 6 whose binary form is 110,
-        then the State is lablled as {"p", "q"}.
+        The State Label is a list of strings, where each string is an Atom.
+        For example, if the atom is ("a", "b", "c"),
+        then the label can be ["a"], ["a", "b", "c"], or [].
 
         Args:
             state: a string representing the State Name
-            label: an int representing the State Label, you are encouraged to input in the binary from
+            label: a list of strings representing the State Label
 
         Raises:
-            KripkeStructError: if a State Name or a State Label exisits, can't add again
+            KripkeStructError: if the State Name or State Label exists, can't add again
+            KrinkeStructError: if the State Label contains a Non-Eixsting Atom, can't add it
 
-        """
-        # if the state or the label exisits, can't add again
-        if state in self.states:
-            raise KripkeStructError("Can't add an Exisiting State Name again")
-        if label in self.states.values():
-            raise KripkeStructError("Can't add an Exisiting State Label again")
-        self.states[state] = label
+        Note:
+            The parameter "label" should be a list to stay compatible with the JSON format.
+            However, internally, the field "_states" is stored as a dict[str, int] for efficiency.
+
+        """
+        # if the state exists, can't add again
+        if state in self._states:
+            raise KripkeStructError("Can't add an Existing State Name again")
+
+        # convert the label to a set, for efficiency,
+        # since we'll check if each atom in "self._atoms" is in "label" later
+        label_set = set(label)
+
+        # if the State Label contains a Non-Eixsting Atom, can't add it
+        for atom in label_set:
+            if atom not in self._atoms_set:
+                raise KripkeStructError("Can't add a State Label with a Non-Existing Atom")
+
+        # convert the label to its binary representation, to save memory
+        # for example, if the atoms are ("a", "b", "c", "d"), and the label is ["a", "c"],
+        # then the binary representation is 0b1010, which is the int 10 in decimal
+        label_binary = 0b0
+        for atom in self._atoms:
+            # if an Atom is in "label", set the corresponding bit to 1
+            if atom in label_set:
+                label_binary |= 0b1
+            # left shift by 1 bit
+            label_binary <<= 1
+
+        # correct the extra left shift
+        label_binary >>= 1
+
+        # if the state label exists, can't add again
+        if label_binary in self._states.values():
+            raise KripkeStructError("Can't add an Existing State Label again")
+
+        self._states[state] = label_binary
 
-    def add_states(self, states: Dict[str, int]) -> None:
+    def add_states(self, states: Dict[str, List[str]]) -> None:
         """Add multiple States to the Kripke Structure.
 
         Args:
             states: a dict, Key is the State Name, Value is the State Label
 
         Raises:
-            KripkeStructError: if a State Name or a State Label exisits, can't add again
+            KripkeStructError: if a State Name or a State Label exists, can't add again
 
         """
         for state, label in states.items():
             self.add_state(state, label)
 
     def get_states(self) -> Dict[str, int]:
         """Get States of the Kripke Structure.
 
         Returns:
             a dict, Key is the State Name, Value is the State Label
 
+        Note:
+            The State Label is store in the binary representation,
+            instead of the list of strings.
+
         """
-        return self.states
+        return dict(self._states)
+
+    def get_state_names(self) -> Set[str]:
+        """Get just State Names of the Kripke Structure.
+
+        Returns:
+            a set of strings representing the State Names
 
-    def get_state_label_set(self, state: str) -> Set[str]:
-        """Given a State Name, get the State Labels.
+        """
+        return set(self._states.keys())
 
-        For example, if the atoms = ("a", "b", "c", "d"), and the label = 0b1010,
-        then the label_set = {"a", "c"}.
+    def set_label_of_state(self, state: str, label_set: Set[str]) -> None:
+        """Given an existing State Name, (re)set the State Label.
+
+        Args:
+            state: a string representing the State Name
+            label_set: a set of strings representing the State Label
+
+        Raises:
+            KripkeStructError: if the State Name doesn't exist, can't (re)set the State Label
+            KripkeStructError: if the Label has been assigned to a differnt State Name, can't assign it
+
+        Note:
+            The parameter "label_set" should be a set, NOT a list, for efficiency.
+
+        """
+        # if the State Name doesn't exist, can't set the Label of it
+        if state not in self._states:
+            raise KripkeStructError("Can't set the Label of a Non-Existing State")
+
+        # if the State Label contains a Non-Eixsting Atom, can't set it
+        for atom in label_set:
+            if atom not in self._atoms_set:
+                raise KripkeStructError("Can't set a State Label with a Non-Existing Atom")
+
+        # convert the label to its binary representation
+        label_binary = 0b0
+        for atom in self._atoms:
+            # if an Atom is in "label", set the corresponding bit to 1
+            if atom in label_set:
+                label_binary |= 0b1
+            # left shift by 1 bit
+            label_binary <<= 1
+
+        # correct the extra left shift
+        label_binary >>= 1
+
+        # if the Label is already assigned to the State Name, do nothing
+        if self._states[state] == label_binary:
+            return
+
+        # if the Label is assigned to a differnt State Name, can't assign it
+        if label_binary in self._states.values():
+            raise KripkeStructError("Can't assign an Existing State Label to a Different State Name")
+
+        self._states[state] = label_binary
+
+    def get_label_of_state(self, state: str) -> Set[str]:
+        """Given a State Name, get the corresponding State Label.
+
+        For example, if atoms is ("a", "b", "c", "d"),
+        the State Name is "s1", and the State Label is 0b1010,
+        then get_label_of_state("s1") will return the set {"a", "c"}.
 
         Args:
             state: a string representing the State Name
 
         Returns:
-            a set of strings representing the State Label, instead of the original binary form
+            a set of strings representing the State Label, instead of the binary form
 
         Raises:
-            KripkeStructError: if the State Name doesn't exisit, can't get the Label Set of it
+            KripkeStructError: if the State Name doesn't exist, can't get the Label of it
 
         """
-        # if the state doesn't exisit, can't get the Label Set of it
-        if state not in self.states:
-            raise KripkeStructError("Can't get the Label Set of a Non-Exisiting State")
+        # if the State Name doesn't exist, can't get the Label of it
+        if state not in self._states:
+            raise KripkeStructError("Can't get the Label of a Non-Existing State")
 
-        # get the binary form of the label, then convert it to the Label Set
-        label = self.states[state]
-        length = len(self.atoms)
+        # get the binary form of the Label, then convert it to a set of atoms
+        label = self._states[state]
+        length = len(self._atoms)
         label_set = set()
 
-        # traverse the binary form of the label
+        # traverse the binary form of the Label
         for i in range(length):
-            # if the i-th bit is 1, then the (length - 1 - i)-th atom is in the Label Set
+            # if the i-th bit is 1, then the (length - 1 - i)-th atom is in the set
             if label & 1 << i:
-                label_set.add(self.atoms[length - 1 - i])
+                label_set.add(self._atoms[length - 1 - i])
 
         return label_set
 
     def remove_state(self, state: str) -> None:
         """Remove a State from the Kripke Structure.
 
         Args:
             state: a string representing the State Name
 
+        Raises:
+            KripkeStructError: if the State Name doesn't exist, can't remove it
+
         """
-        if state in self.states:
-            self.states.pop(state)
-            # removing state will remove related transitions
-            if state in self.trans:
-                next_states = self.trans.pop(state)
-                for next_state in next_states:
-                    self.trans_inverted[next_state].remove(state)
-            if state in self.trans_inverted:
-                prev_states = self.trans_inverted.pop(state)
-                for prev_state in prev_states:
-                    self.trans[prev_state].remove(state)
+        # if the State Name doesn't exist, can't remove it
+        if state not in self._states:
+            raise KripkeStructError("Can't remove a Non-Existing State")
+        self._states.pop(state)
+
+        # removing a state will remove all related transitions
+        if state in self._trans:
+            next_states = self._trans.pop(state)
+            for next_state in next_states:
+                self._trans_inverted[next_state].remove(state)
+        if state in self._trans_inverted:
+            prev_states = self._trans_inverted.pop(state)
+            for prev_state in prev_states:
+                self._trans[prev_state].remove(state)
 
     def remove_states(self, states: List[str]) -> None:
         """Remove multiple States from the Kripke Structure.
 
         Args:
             states: a list of strings representing the State Names
 
@@ -196,138 +313,168 @@
         for state in states:
             self.remove_state(state)
 
     def set_starts(self, starts: List[str]) -> None:
         """Set Start States of the Kripke Structure.
 
         Args:
-            starts: a list of strings representing the Start States
+            starts: a set of strings representing the Start States
 
         Raises:
-            KripkeStructError: if start state doesn't exist, can't set it
+            KripkeStructError: if a state doesn't exist, can't set it as a Start State
+
+        Note:
+            The parameter "starts" should be a list to stay compatible with the JSON format.
+            However, internally, the field "_starts" is stored as a set for efficiency.
 
         """
         for start in starts:
-            # if start state doesn't exist, can't set it
-            if start not in self.states:
-                raise KripkeStructError("Can't set a Non-Exisiting State as Start State")
-        self.starts = set(starts)
+            # if a state doesn't exist, can't set it as a Start State
+            if start not in self._states:
+                raise KripkeStructError("Can't set a Non-Existing State as Start State")
+        self._starts = set(starts)
 
-    def get_starts(self) -> List[str]:
+    def get_starts(self) -> Set[str]:
         """Get Start States of the Kripke Structure.
 
         Returns:
-            a list of strings representing the Start States
+            a set of strings representing the Start States
 
         """
-        return list(self.starts)
+        return self._starts
 
-    def add_trans(self, trans: Dict[str, List[str]]) -> None:
+    def add_trans(self, trans: Dict[str, Set[str]]) -> None:
         """Add multiple Transitions to the Kripke Structure.
 
         Args:
             trans: a dict, Key is the Source State Name, Value is a list of Target State Names
 
         Raises:
             KripkeStructError: if Source or Target State doesn't exist, can't add transition
 
+        Note:
+            The parameter "trans" should be a dict whose value is a list, to stay compatible with the JSON format.
+            However, internally, the field "_trans" is stored as a dict whose value is a set for efficiency.
+            For more information about list v.s. set, see:
+            https://stackoverflow.com/questions/2831212/python-sets-vs-lists
         """
         for state, next_states in trans.items():
             # if source state doesn't exist, can't add transition
-            if state not in self.states:
-                raise KripkeStructError("Can't add Transition from a Non-Exisiting Source State")
+            if state not in self._states:
+                raise KripkeStructError("Can't add Transition from a Non-Existing Source State")
 
             for next_state in next_states:
                 # if target state doesn't exist, can't add transition
-                if next_state not in self.states:
-                    raise KripkeStructError("Can't add Transition to a Non-Exisiting Target State")
-                self.trans[state].append(next_state)
-                # adding Transitions will also update the Inverted Transitions
+                if next_state not in self._states:
+                    raise KripkeStructError("Can't add Transition to a Non-Existing Target State")
+                # adding a Transition will also update the Inverted Transitions,
                 # which will be used to remove related Transitions when revmoing a State
-                self.trans_inverted[next_state].append(state)
+                self._trans[state].add(next_state)
+                self._trans_inverted[next_state].add(state)
 
-    def get_trans(self) -> Dict[str, List[str]]:
+    def get_trans(self) -> defaultdict[str, Set[str]]:
         """Get Transitions of the Kripke Structure.
 
         Returns:
-            a dict, Key is the Source State Name, Value is a list of Target State Names
+            a defaultdict, Key is the Source State Name, Value is a set of Target State Names
 
         """
-        return dict(self.trans)
+        return self._trans
 
-    def get_trans_inverted(self) -> Dict[str, List[str]]:
+    def get_trans_inverted(self) -> defaultdict[str, Set[str]]:
         """Get Inverted Transitions of the Kripke Structure.
 
         Returns:
-            a dict, Key is the Target State Name, Value is a list of Source State Names
+            a defaultdict, Key is the Target State Name, Value is a set of Source State Names
 
         """
-        return dict(self.trans_inverted)
+        return self._trans_inverted
 
     def remove_trans(self, trans: Dict[str, List[str]]) -> None:
         """Remove multiple Transitions from the Kripke Structure.
 
         Args:
             trans: a dict, Key is the Source State Name, Value is a list of Target State Names
 
+        Raises:
+            KripkeStructError: if a Transition doesn't exist, can't remove it
+
+        Note:
+            The parameter "trans" should be a dict whose value is a list for efficiency,
+            since it will only be iterated once.
+            However, internally, the field "_trans" is stored as a dict whose value is a set for efficiency.
+
         """
         for state, next_states in trans.items():
             for next_state in next_states:
-                if state in self.states and next_state in self.trans[state]:
-                    self.trans[state].remove(next_state)
-                    self.trans_inverted[next_state].remove(state)
+                # if a Transition doesn't exist, can't remove it
+                if (state not in self._trans) or (next_state not in self._trans[state]):
+                    raise KripkeStructError("Can't remove a Non-Existing Transition")
+                # removing a Transition will also update the Inverted Transitions
+                self._trans[state].remove(next_state)
+                self._trans_inverted[next_state].remove(state)
+
+    def reverse_all_trans(self) -> None:
+        """Reverse all Transitions in the Kripke Structure.
+
+        This funciton is destructive!!!
+        It will NOT create a new copy of the current Kripke Structure,
+        but will directly modify the current Kripke Structure.
+
+        """
+        self._trans, self._trans_inverted = self._trans_inverted, self._trans
 
     def get_SCCs(self) -> List[Set[str]]:
         """Get all Strongly Connected Components (SCCs) in the Kripke Structure.
 
         Returns:
-            a list of sets, where each set is a SCC
+            a list of sets, where each set contains the State Names in a SCC
 
         """
         # we use Kosaraju's Algorithm to find SCCs
         # first, we run DFS on the original graph, store the order of finishing states in "order_stack"
         order_stack = []
         visited = set()
 
         def DFS(state, visited, order_stack):
             visited.add(state)
-            successors = self.trans[state]
+            successors = self._trans[state]
             for successor in successors:
                 if successor not in visited:
                     DFS(successor, visited, order_stack)
             # add to order_stack when exiting DFS
             order_stack.append(state)
 
-        for state in self.states:
+        for state in self._states:
             if state not in visited:
                 DFS(state, visited, order_stack)
 
         # second, we create the reversed graph of the Kripke Structure self
         # since we need to modify the reversed graph, we create a deepcopy of self
         reversed_graph = deepcopy(self)
-        reversed_graph.trans, reversed_graph.trans_inverted = reversed_graph.trans_inverted, reversed_graph.trans
+        reversed_graph.reverse_all_trans()
 
         # third we run multiple rounds of DFS on the reversed graph until all states are visited
         # when we finish a round of DFS, we get a SCC
         # then we add the SCC to the set, and remove all states in the SCC from the reversed graph
         SCCs = set()
-        while reversed_graph.states:
+        while reversed_graph.get_states():
             # we run DFS on the reversed graph, following the order of the "order_stack"
             tmp_stack = [order_stack.pop()]
             visited = set()
             while tmp_stack:
                 current_state = tmp_stack.pop()
                 visited.add(current_state)
 
                 # remove the visited state from the order_stack
                 if current_state in order_stack:
                     order_stack.remove(current_state)
 
                 # add un-visited successors to the stack
-                successors = reversed_graph.trans[current_state]
+                successors = reversed_graph.get_trans()[current_state]
                 for successor in successors:
                     if successor not in visited:
                         tmp_stack.append(successor)
 
             # now all states in the set "visited" are in the same SCC
             # so we add it to the list of SCCs, and remove all states in it from the reversed graph
             SCCs.add(frozenset(visited))
```

### Comparing `mctk-py-0.1.0/mctk/tests/test_checking.py` & `mctk-py-0.1.1/mctk/tests/test_checking.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 # Internal Modules to be tested
 from mctk import KripkeStruct, KripkeStructError
 from mctk import SAT_atom, NOT, AND, OR, IMPLIES, IFF, EX, AX, EU, EF, AG, EG, AF, AU
 
 
 ks_json = {
-    "Atoms": ("a", "b", "c", "d"),
+    "Atoms": ["a", "b", "c", "d"],
     "States": {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
-        "s5": 0b0100,  # s5 has label "b"
-        "s6": 0b0010,  # s6 has label "c"
-        "s7": 0b0001,  # s7 has label "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
+        "s5": ["b"],
+        "s6": ["c"],
+        "s7": ["d"],
     },
     "Starts": ["s1"],
     "Trans": {
         's1': ['s2'],
         's2': ['s3', 's4'],
         's3': ['s4'],
         's4': ['s7'],
@@ -52,32 +52,32 @@
 
     # if the atomic property is not in the Kripke Structure, can't check it
     with pytest.raises(KripkeStructError) as error_info:
         sat_states = SAT_atom(ks, "e")
     assert str(error_info.value) == "Can't check on an atom that's not in the Kripke Structure"
 
     sat_states = SAT_atom(ks, "True")
-    assert sat_states == set(ks.states.keys())
+    assert sat_states == set(ks.get_states().keys())
 
     sat_states = SAT_atom(ks, "False")
     assert sat_states == set()
 
 
 def test_ESMC_NOT():
     sat_states = NOT(ks, SAT_atom(ks, "a"))
-    assert sat_states == set(ks.states.keys()) - {"s1", "s2"}
+    assert sat_states == set(ks.get_states().keys()) - {"s1", "s2"}
 
     sat_states = NOT(ks, SAT_atom(ks, "b"))
-    assert sat_states == set(ks.states.keys()) - {"s2", "s3", "s4", "s5"}
+    assert sat_states == set(ks.get_states().keys()) - {"s2", "s3", "s4", "s5"}
 
     sat_states = NOT(ks, SAT_atom(ks, "True"))
     assert sat_states == set()
 
     sat_states = NOT(ks, SAT_atom(ks, "False"))
-    assert sat_states == set(ks.states.keys())
+    assert sat_states == set(ks.get_states().keys())
 
 
 def test_ESMC_AND():
     sat_states = AND(SAT_atom(ks, "a"), SAT_atom(ks, "b"))
     assert sat_states == {"s2"}
 
     sat_states = AND(SAT_atom(ks, "a"), SAT_atom(ks, "c"))
@@ -184,16 +184,16 @@
     assert sat_states == set()
 
 
 def test_ESMC_EG():
     # change s5's label to {"b", "d"}
     # change s6's label to {"c", "d"}
     tmp_ks = deepcopy(ks)
-    tmp_ks.states["s5"] = 0b0101
-    tmp_ks.states["s6"] = 0b0011
+    tmp_ks.set_label_of_state("s5", {"b", "d"})
+    tmp_ks.set_label_of_state("s6", {"c", "d"})
 
     sat_states = EG(tmp_ks, SAT_atom(tmp_ks, "a"))
     assert sat_states == set()
 
     sat_states = EG(tmp_ks, SAT_atom(tmp_ks, "b"))
     assert sat_states == set()
 
@@ -207,15 +207,15 @@
     sat_states = EG(tmp_ks, SAT_atom(tmp_ks, "d"))
     assert sat_states == {"s5", "s6", "s7"}
 
 
 def test_ESMC_AF():
     # change s7 to "", which is empty set
     tmp_ks = deepcopy(ks)
-    tmp_ks.states["s7"] = 0b0000
+    tmp_ks.set_label_of_state("s7", set())
 
     sat_states = AF(tmp_ks, SAT_atom(tmp_ks, "a"))
     assert sat_states == {"s1", "s2"}
 
     sat_states = AF(tmp_ks, SAT_atom(tmp_ks, "b"))
     assert sat_states == {"s1", "s2", "s3", "s4", "s5", "s6", "s7"}
 
@@ -261,16 +261,16 @@
     # set 2 Atomic Propositions in this Kripke Structure
     ks.set_atoms(["p", "q"])
 
     # add 2 states to the Kripke Structure
     # a State Name is represented by a string, it must be unique
     # a State Label is represented by a binary number, it must be unique
     # for example, 0b10 means the state has the Atoms "p" but not "q"
-    ks.add_state("s0", 0b10)
-    ks.add_state("s1", 0b01)
+    ks.add_state("s0", ["p"])
+    ks.add_state("s1", ["q"])
 
     # set the Start States of the Kripke Structure
     # there can be multiple Start States
     ks.set_starts(["s0"])
 
     # add 2 Transitions to the Kripke Structure
     # a Transition is represented by a key-value pair
@@ -306,7 +306,53 @@
 
     # check if the Kripke Structure satisfies the CTL formula: EG (A p U (NOT q))
     sat_states = EG(ks, AU(ks, SAT_atom(ks, "p"), NOT(ks, SAT_atom(ks, "q"))))
 
     # the result should be set(), empty set
     # since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
     assert sat_states == set()
+
+    # check CTL formula on a Complex Kripke Structure
+    ks_json = {
+        "Atoms": ["a", "b", "c", "d"],
+        "States": {
+            "s1": ["a"],
+            "s2": ["a", "b"],
+            "s3": ["b", "c"],
+            "s4": ["b", "c", "d"],
+            "s5": ["b"],
+            "s6": ["c"],
+            "s7": ["d"],
+        },
+        "Starts": ["s1"],
+        "Trans": {
+            's1': ['s2'],
+            's2': ['s3', 's4'],
+            's3': ['s4'],
+            's4': ['s7'],
+            's5': ['s6'],
+            's6': ['s7', 's5'],
+            's7': ['s5'],
+        },
+    }
+    ks = KripkeStruct(ks_json)
+
+    # check if the Kripke Structure satisfies the CTL formula: EX a
+    sat_states = EX(ks, SAT_atom(ks, "a"))
+
+    # the result should be {"s1"}
+    # since the start state "s1" is in sat_states, ks satisfies the CTL formula
+    assert sat_states == {"s1"}
+
+    # check if the Kripke Structure satisfies the CTL formula: E a U b
+    sat_states = EU(ks, SAT_atom(ks, "a"), SAT_atom(ks, "b"))
+
+    # the result should be {'s1', 's2', 's3', 's4', 's5'}
+    # since the start state "s1" is in sat_states, ks satisfies the CTL formula
+    assert sat_states == {'s1', 's2', 's3', 's4', 's5'}
+
+    # check if the Kripke Structure satisfies the CTL formula: EG a
+    sat_states = EG(ks, SAT_atom(ks, "a"))
+
+    # the result should be set()
+    # since the start state "s1" is not in sat_states, ks doesn't satisfy the CTL formula
+    assert sat_states == set()
```

### Comparing `mctk-py-0.1.0/mctk/tests/test_models.py` & `mctk-py-0.1.1/mctk/tests/test_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,338 +10,447 @@
 # Internal Modules to be tested
 from mctk import KripkeStruct, KripkeStructError
 
 
 # Tests for KripkeStruct()
 def test_KS_default_init():
     ks = KripkeStruct()
-    assert ks.atoms == ()
-    assert ks.states == {}
-    assert ks.starts == set()
-    assert ks.trans == defaultdict(list)
-    assert ks.trans_inverted == defaultdict(list)
+    assert ks._atoms == ()
+    assert ks._atoms_set == set()
+    assert ks._states == {}
+    assert ks._starts == set()
+    assert ks._trans == defaultdict(set)
+    assert ks._trans_inverted == defaultdict(set)
 
 
 # Tests for KripkeStruct(ks_json)
-def test_KS_file_init():
+def test_KS_json_init():
     ks_json = {
-        "Atoms": ("a", "b", "c", "d"),
-        "States": {"s1": 8, "s2": 12, "s3": 6, "s4": 7},
+        "Atoms": ["a", "b", "c", "d"],
+        "States": {"s1": ["a"], "s2": ["b"], "s3": ["c", "d"], "s4": []},
         "Starts": ["s1"],
         "Trans": {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4"]},
     }
     ks = KripkeStruct(ks_json)
 
-    assert ks.atoms == ("a", "b", "c", "d")
-    assert ks.states == {"s1": 8, "s2": 12, "s3": 6, "s4": 7}
-    assert ks.starts == {"s1"}
-    assert dict(ks.trans) == {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4"]}
+    assert ks._atoms == ("a", "b", "c", "d")
+    assert ks._atoms_set == {"a", "b", "c", "d"}
+    assert ks._states == {"s1": 0b1000, "s2": 0b0100, "s3": 0b0011, "s4": 0b0000}
+    assert ks._starts == {"s1"}
+    assert ks._trans == {"s1": {"s2"}, "s2": {"s3", "s4"}, "s3": {"s4"}}
+    assert ks._trans_inverted == {"s2": {"s1"}, "s3": {"s2"}, "s4": {"s2", "s3"}}
 
 
 # Tests for ks.__str__()
 def test_KS_str_rep():
     ks_json = {
-        "Atoms": ("a", "b", "c", "d"),
-        "States": {"s1": 8, "s2": 12, "s3": 6, "s4": 7},
-        "Starts": {"s1"},
-        "Trans": {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4"]},
+        "Atoms": ["a", "b", "c", "d"],
+        "States": {"s1": ["a"], "s2": ["b"], "s3": ["c", "d"], "s4": []},
+        "Starts": ["s1"],
+        "Trans": {"s1": ["s2"], "s2": ["s3"], "s3": ["s4"]},
     }
     ks = KripkeStruct(ks_json)
     assert str(ks) == (
         "Atoms: ('a', 'b', 'c', 'd')\n"
-        + "States: {'s1': 8, 's2': 12, 's3': 6, 's4': 7}\n"
+        + "States: {'s1': 8, 's2': 4, 's3': 3, 's4': 0}\n"
         + "Starts: {'s1'}\n"
-        + "Trans: {'s1': ['s2'], 's2': ['s3', 's4'], 's3': ['s4']}"
+        + "Trans: {'s1': {'s2'}, 's2': {'s3'}, 's3': {'s4'}}"
     )
 
 
 def test_KS_set_atoms():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
-    assert ks.atoms == ("a", "b", "c", "d")
+    assert ks._atoms == ("a", "b", "c", "d")
+    assert ks._atoms_set == {"a", "b", "c", "d"}
 
     # if any state exists, can't reset atoms
     with pytest.raises(KripkeStructError) as error_info:
-        ks.add_state("s1", 0b1000)
-        atoms = ["a"]
+        ks.add_state("s1", ["a"])
+        atoms = ("a",)
         ks.set_atoms(atoms)
     assert str(error_info.value) == "Can't reset Atoms after States are Created"
 
 
 def test_KS_get_atoms():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
-    assert ks.get_atoms() == atoms
+    assert ks.get_atoms() == ("a", "b", "c", "d")
 
 
 def test_KS_add_state():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
-    ks.add_state("s1", 0b1000)
-    assert ks.states == {"s1": 0b1000}
+    ks.add_state("s1", ["a"])
+    ks.add_state("s2", ["a", "b"])
+    assert ks._states == {"s1": 0b1000, "s2": 0b1100}
 
     # if the state name exists, can't add again
     with pytest.raises(KripkeStructError) as error_info:
-        ks.add_state("s1", 0b1111)
-    assert str(error_info.value) == "Can't add an Exisiting State Name again"
+        ks.add_state("s1", ["a", "b", "c", "d"])
+    assert str(error_info.value) == "Can't add an Existing State Name again"
+
+    # if the state label exists, can't add again
+    with pytest.raises(KripkeStructError) as error_info:
+        ks.add_state("s3", ["a"])
+    assert str(error_info.value) == "Can't add an Existing State Label again"
 
-    # if the state label exisits, can't add again
+    # if the State Label contains a Non-Eixsting Atom, can't add it
     with pytest.raises(KripkeStructError) as error_info:
-        ks.add_state("s8", 0b1000)
-    assert str(error_info.value) == "Can't add an Exisiting State Label again"
+        ks.add_state("s3", ["a", "b", "c", "d", "e"])
+    assert str(error_info.value) == "Can't add a State Label with a Non-Existing Atom"
 
 
 def test_KS_add_states():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
+        "s5": ["b"],
+        "s6": ["c"],
+        "s7": ["d"],
+    }
+    ks.add_states(states)
+    assert ks._states == {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
         "s4": 0b0111,  # s4 has labels "b", "c", "d"
         "s5": 0b0100,  # s5 has label "b"
         "s6": 0b0010,  # s6 has label "c"
         "s7": 0b0001,  # s7 has label "d"
     }
-    ks.add_states(states)
-    assert ks.states == states
 
 
 def test_KS_get_states():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
-    ks.add_state("s1", 0b1000)
+    ks.add_state("s1", ["a"])
     assert ks.get_states() == {"s1": 0b1000}
 
 
-def test_KS_get_state_label_set():
+def test_KS_get_state_names():
+    ks = KripkeStruct()
+    atoms = ["a", "b", "c", "d"]
+    ks.set_atoms(atoms)
+    ks.add_state("s1", ["a"])
+    assert ks.get_state_names() == {"s1"}
+
+
+def test_KS_set_label_of_state():
+    ks = KripkeStruct()
+    atoms = ["a", "b", "c", "d"]
+    ks.set_atoms(atoms)
+    ks.add_state("s1", ["a"])
+    ks.set_label_of_state("s1", {"c", "d"})
+    assert ks.get_states() == {"s1": 0b0011}
+
+    # if the State Name doesn't exist, can't set the Label of it
+    with pytest.raises(KripkeStructError) as error_info:
+        ks.set_label_of_state("s2", {"a", "b", "c", "d"})
+    assert str(error_info.value) == "Can't set the Label of a Non-Existing State"
+
+    # if the Label has been assigned to a differnt State Name, can't assign it
+    with pytest.raises(KripkeStructError) as error_info:
+        ks.add_state("s2", ["a", "b", "c", "d"])
+        ks.set_label_of_state("s2", {"c", "d"})
+    assert str(error_info.value) == "Can't assign an Existing State Label to a Different State Name"
+
+    # if the State Label contains a Non-Eixsting Atom, can't set it
+    with pytest.raises(KripkeStructError) as error_info:
+        ks.set_label_of_state("s2", {"a", "b", "c", "d", "e"})
+    assert str(error_info.value) == "Can't set a State Label with a Non-Existing Atom"
+
+    # assigning the Label to its corresponding State Name, wont' have any effect
+    ks.set_label_of_state("s2", {"a", "b", "c", "d"})
+    assert ks.get_states() == {"s1": 0b0011, "s2": 0b1111}
+
+    # if the Label is assigned to a differnt State Name, can't assign it using []
+    with pytest.raises(KripkeStructError) as error_info:
+        ks._states["s2"] = 0b0011
+    assert str(error_info.value) == "Can't assign an existing State Label to a different State Name"
+
+    # if the Label is NOT an int, can't assign it using []
+    with pytest.raises(KripkeStructError) as error_info:
+        ks._states["s2"] = {"a"}
+    assert str(error_info.value) == "The a State Label should be an int, when assigning with []"
+
+    # if the label value exceeds 2^n, where n is the number of atoms, can't assign it using []
+    with pytest.raises(KripkeStructError) as error_info:
+        ks._states["s2"] = 0b100000
+    assert str(error_info.value) == "The value should be less than 2^n, where n is the number of atoms"
+
+    # assigning the Label to its corresponding State Name using [], wont' have any effect
+    ks._states["s2"] = 0b1111
+    assert ks.get_states() == {"s1": 0b0011, "s2": 0b1111}
+
+
+def test_KS_get_label_of_state():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
-    ks.add_state("s1", 0b1001)
-    assert ks.get_state_label_set("s1") == {"a", "d"}
+    ks.add_state("s1", ["a", "d"])
+    assert ks.get_label_of_state("s1") == {"a", "d"}
 
-    # if the state doesn't exist, can't get the Label Set of it
+    # if the state doesn't exist, can't get the Label of it
     with pytest.raises(KripkeStructError) as error_info:
-        assert ks.get_state_label_set("s2")
-    assert str(error_info.value) == "Can't get the Label Set of a Non-Exisiting State"
+        assert ks.get_label_of_state("s2")
+    assert str(error_info.value) == "Can't get the Label of a Non-Existing State"
 
 
 def test_KS_remove_state():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
+        "s5": ["b"],
+        "s6": ["c"],
+        "s7": ["d"],
+    }
+    ks.add_states(states)
+    ks.remove_state("s7")
+    assert ks.get_states() == {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
         "s4": 0b0111,  # s4 has labels "b", "c", "d"
         "s5": 0b0100,  # s5 has label "b"
         "s6": 0b0010,  # s6 has label "c"
-        "s7": 0b0001,  # s7 has label "d"
     }
-    ks.add_states(states)
-    ks.remove_state("s7")
-    states.pop("s7")
-    assert ks.states == states
 
-    # removing non-existing state won't have any effect
-    ks.remove_state("s8")
-    assert ks.states == states
+    # if the State Name doesn't exist, can't remove it
+    with pytest.raises(KripkeStructError) as error_info:
+        ks.remove_state("s8")
+    assert str(error_info.value) == "Can't remove a Non-Existing State"
 
 
 def test_KS_remove_states():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
+        "s5": ["b"],
+        "s6": ["c"],
+        "s7": ["d"],
+    }
+    ks.add_states(states)
+    ks.remove_states(["s6", "s7"])
+    assert ks.get_states() == {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
         "s4": 0b0111,  # s4 has labels "b", "c", "d"
         "s5": 0b0100,  # s5 has label "b"
-        "s6": 0b0010,  # s6 has label "c"
-        "s7": 0b0001,  # s7 has label "d"
     }
-    ks.add_states(states)
-    ks.remove_states(["s6", "s7"])
-    states.pop("s7")
-    states.pop("s6")
-    assert ks.states == states
 
 
 def test_KS_set_starts():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
     }
     ks.add_states(states)
 
     starts = ["s1", "s4"]
     ks.set_starts(starts)
-    assert ks.starts == set(starts)
+    assert ks._starts == {"s1", "s4"}
 
     # resetting the start states is allowed
     starts = ["s1"]
     ks.set_starts(starts)
-    assert ks.starts == set(starts)
+    assert ks._starts == {"s1"}
 
     # if state doesn't exist, can't set as start state
     with pytest.raises(KripkeStructError) as error_info:
         ks.set_starts(["s5"])
-    assert str(error_info.value) == "Can't set a Non-Exisiting State as Start State"
+    assert str(error_info.value) == "Can't set a Non-Existing State as Start State"
 
 
 def test_KS_get_starts():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
     }
     ks.add_states(states)
 
     starts = ["s1", "s4"]
     ks.set_starts(starts)
-    assert set(ks.get_starts()) == set(starts)
+    assert ks.get_starts() == {"s1", "s4"}
 
 
 def test_KS_add_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
     }
     ks.add_states(states)
     ks.set_starts(["s1"])
 
     trans = {
         "s1": ["s2"],  # a -> ab
         "s2": ["s3", "s4"],  # ab -> bc
         "s3": ["s4", "s1"],  # bc -> bcd, a
         "s4": ["s2"],  # bcd -> ab
     }
     ks.add_trans(trans)
-    assert trans == {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4", "s1"], "s4": ["s2"]}
+    assert ks._trans == {"s1": {"s2"}, "s2": {"s3", "s4"}, "s3": {"s4", "s1"}, "s4": {"s2"}}
 
     # if source state doesn't exist, can't add transition from it
     with pytest.raises(KripkeStructError) as error_info:
         trans = {"s7": ["s1"]}
         ks.add_trans(trans)
-    assert str(error_info.value) == "Can't add Transition from a Non-Exisiting Source State"
+    assert str(error_info.value) == "Can't add Transition from a Non-Existing Source State"
 
     # if target state doesn't exist, can't add transition to it
     with pytest.raises(KripkeStructError) as error_info:
         trans = {"s1": ["s7"]}
         ks.add_trans(trans)
-    assert str(error_info.value) == "Can't add Transition to a Non-Exisiting Target State"
+    assert str(error_info.value) == "Can't add Transition to a Non-Existing Target State"
 
 
 def test_KS_get_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
     }
     ks.add_states(states)
     ks.set_starts(["s1"])
     trans = {
         "s1": ["s2"],  # a -> ab
         "s2": ["s3", "s4"],  # ab -> bc
         "s3": ["s4", "s1"],  # bc -> bcd, a
         "s4": ["s2"],  # bcd -> ab
     }
     ks.add_trans(trans)
-    assert ks.get_trans() == {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4", "s1"], "s4": ["s2"]}
+    assert ks.get_trans() == {"s1": {"s2"}, "s2": {"s3", "s4"}, "s3": {"s4", "s1"}, "s4": {"s2"}}
 
 
 def test_KS_get_trans_inverted():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
     }
     ks.add_states(states)
     ks.set_starts(["s1"])
     trans = {
         "s1": ["s2"],  # a -> ab
         "s2": ["s3", "s4"],  # ab -> bc
         "s3": ["s4", "s1"],  # bc -> bcd, a
         "s4": ["s2"],  # bcd -> ab
     }
     ks.add_trans(trans)
-    assert ks.get_trans_inverted() == {"s1": ["s3"], "s2": ["s1", "s4"], "s3": ["s2"], "s4": ["s2", "s3"]}
+    assert ks.get_trans_inverted() == {"s1": {"s3"}, "s2": {"s1", "s4"}, "s3": {"s2"}, "s4": {"s2", "s3"}}
 
 
 def test_KS_remove_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
     }
     ks.add_states(states)
     ks.set_starts(["s1"])
     trans = {
         "s1": ["s2"],  # a -> ab
         "s2": ["s3", "s4"],  # ab -> bc
         "s3": ["s4", "s1"],  # bc -> bcd, a
         "s4": ["s2"],  # bcd -> ab
     }
     ks.add_trans(trans)
 
     trans = {"s2": ["s4"], "s4": ["s2"]}
     ks.remove_trans(trans)
-    assert ks.get_trans() == {"s1": ["s2"], "s2": ["s3"], "s3": ["s4", "s1"], "s4": []}
+    assert ks.get_trans() == {"s1": {"s2"}, "s2": {"s3"}, "s3": {"s4", "s1"}, "s4": set()}
 
-    # removing non-existing transition won't have any effect
-    trans = {"s2": ["s4"]}
-    ks.remove_trans(trans)
-    assert ks.get_trans() == {"s1": ["s2"], "s2": ["s3"], "s3": ["s4", "s1"], "s4": []}
+    # if a Transition doesn't exist, can't remove it
+    with pytest.raises(KripkeStructError) as error_info:
+        ks.remove_trans({"s2": ["s4"]})
+    assert str(error_info.value) == "Can't remove a Non-Existing Transition"
+
+
+def test_KS_reverse_all_trans():
+    ks = KripkeStruct()
+    atoms = ["a", "b", "c", "d"]
+    ks.set_atoms(atoms)
+    states = {
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
+    }
+    ks.add_states(states)
+    ks.set_starts(["s1"])
+    trans = {
+        "s1": ["s2"],  # a -> ab
+        "s2": ["s3", "s4"],  # ab -> bc
+        "s3": ["s4", "s1"],  # bc -> bcd, a
+        "s4": ["s2"],  # bcd -> ab
+    }
+    ks.add_trans(trans)
+
+    ks.reverse_all_trans()
+    assert ks.get_trans() == {"s1": {"s3"}, "s2": {"s1", "s4"}, "s3": {"s2"}, "s4": {"s2", "s3"}}
 
 
 def test_KS_get_SCCs():
     ks_json = {
-        "Atoms": ("a", "b", "c", "d"),
+        "Atoms": ["a", "b", "c", "d"],
         "States": {
-            "s1": 0b1000,  # s1 has labels "a"
-            "s2": 0b1100,  # s2 has labels "a", "b"
-            "s3": 0b0110,  # s3 has labels "b", "c"
-            "s4": 0b0111,  # s4 has labels "b", "c", "d"
-            "s5": 0b0100,  # s5 has label "b"
-            "s6": 0b0010,  # s6 has label "c"
-            "s7": 0b0001,  # s7 has label "d"
+            "s1": ["a"],
+            "s2": ["a", "b"],
+            "s3": ["b", "c"],
+            "s4": ["b", "c", "d"],
+            "s5": ["b"],
+            "s6": ["c"],
+            "s7": ["d"],
         },
         "Starts": ["s1"],
         "Trans": {
             's1': ['s2'],
             's2': ['s3', 's4'],
             's3': ['s4'],
             's4': ['s7'],
@@ -370,25 +479,25 @@
 
 # Integration Tests: removing state will remove related transitions
 def test_KS_remove_states_will_remove_related_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
-        "s1": 0b1000,  # s1 has labels "a"
-        "s2": 0b1100,  # s2 has labels "a", "b"
-        "s3": 0b0110,  # s3 has labels "b", "c"
-        "s4": 0b0111,  # s4 has labels "b", "c", "d"
+        "s1": ["a"],
+        "s2": ["a", "b"],
+        "s3": ["b", "c"],
+        "s4": ["b", "c", "d"],
     }
     ks.add_states(states)
     ks.set_starts(["s1"])
     trans = {
         "s1": ["s2"],  # a -> ab
         "s2": ["s3", "s4"],  # ab -> bc
         "s3": ["s4", "s1"],  # bc -> bcd, a
         "s4": ["s2"],  # bcd -> ab
     }
     ks.add_trans(trans)
 
     ks.remove_state("s2")
-    assert ks.get_trans() == {'s1': [], 's3': ['s4', 's1'], 's4': []}
-    assert ks.get_trans_inverted() == {'s3': [], 's4': ['s3'], 's1': ['s3']}
+    assert ks.get_trans() == {'s1': set(), 's3': {'s4', 's1'}, 's4': set()}
+    assert ks.get_trans_inverted() == {'s3': set(), 's4': {'s3'}, 's1': {'s3'}}
```

### Comparing `mctk-py-0.1.0/mctk_py.egg-info/PKG-INFO` & `mctk-py-0.1.1/mctk_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctk-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Model Checking Toolkit for Python
 Author-email: marcusm117 <marcusmin117@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -231,15 +231,15 @@
 
 Users can use functions that implements CTL operators to formally verify if a Kripke Structure (can be created during runtime or input in a JSON file) satisfies certain CTL properties. All checking functions will return a set of states that satisfy the CTL property, which means that if any start state of the Kripke Structure is in the returned set, then the Kripke Structure satisfies the CTL property.
 
 ## Getting Started
 
 ### Installation
 
-Get the latest version of `mctk` from PyPI. Note that the registered name is 'mctk-py' on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as 'mctk'.
+Get the latest version of `mctk` from PyPI. Note that the registered name is `mctk-py` on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as `mctk`.
 
    ``` bash
    pip3 install mctk-py
    ```
 
 If you are having trouble with `pip3`, you can also install from the source code, see [Developing](#developing).
 
@@ -271,43 +271,42 @@
 - `make lint`: perform static analysis of this library with `black`, `flake8` and `pylint`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 ## Usage
 
-Create a Krinke Structure from scratch.
+### Create a Kripke Structure from Scratch
 
 ``` python
 from mctk import *
 
 # create a Kripke Structure from scratch
 ks = KripkeStruct()
 
 # set 2 Atomic Propositions in this Kripke Structure
 ks.set_atoms(["p", "q"])
 
 # add 2 states to the Kripke Structure
 # a State Name is represented by a string, it must be unique
-# a State Label is represented by a binary number, it must be unique
-# for example, 0b10 means the state has the Atoms "p" but not "q"
-ks.add_state("s0", 0b10)
-ks.add_state("s1", 0b01)
+# a State Label is represented by a list of Atoms, it must be unique
+ks.add_state("s0", ["p"])
+ks.add_state("s1", ["q"])
 
 # set the Start States of the Kripke Structure
 # there can be multiple Start States
 ks.set_starts(["s0"])
 
 # add 2 Transitions to the Kripke Structure
 # a Transition is represented by a key-value pair
 # where key the Source State Name and value is a list of Destination State Names
 ks.add_trans({"s0": ["s1"], "s1": ["s0"]})
 ```
 
-Check if the Kripke Structure satisfies a simple CTL formula.
+### Checking Simple CTL Formula on the Kripke Structure
 
 ``` python
 # check if the Kripke Structure satisfies the CTL formula: EX p
 # SAT_atom(ks, "p") returns a set of states that satisfy the Atomic Proposition p
 # EX returns a set of states that satisfy the CTL formula EX p
 sat_states = EX(ks, SAT_atom(ks, "p"))
 
@@ -322,15 +321,15 @@
 sat_states = EU(ks, SAT_atom(ks, "p"), SAT_atom(ks, "q"))
 
 # the result should be {"s0", "s1"}
 # since the start state "s0" is in sat_states, ks satisfies the CTL formula
 assert sat_states == {"s0", "s1"}
 ```
 
-Check if the Kripke Structure satisfies a composite CTL formula.
+### Checking Composite CTL Formula on the Kripke Structure
 
 ``` python
 # check if the Kripke Structure satisfies the CTL formula: EX (p AND EX q)
 sat_states = EX(ks, AND(SAT_atom(ks, "p"), EX(ks, SAT_atom(ks, "q"))))
 
 # the result should be {"s1"}
 # since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
@@ -340,12 +339,61 @@
 sat_states = EG(ks, AU(ks, SAT_atom(ks, "p"), NOT(ks, SAT_atom(ks, "q"))))
 
 # the result should be set(), empty set
 # since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
 assert sat_states == set()
 ```
 
+### Checking CTL formula on a Complex Kripke Structure
+
+``` python
+ks_json = {
+   "Atoms": ["a", "b", "c", "d"],
+   "States": {
+      "s1": ["a"],
+      "s2": ["a", "b"],
+      "s3": ["b", "c"],
+      "s4": ["b", "c", "d"],
+      "s5": ["b"],
+      "s6": ["c"],
+      "s7": ["d"],
+   },
+   "Starts": ["s1"],
+   "Trans": {
+      's1': ['s2'],
+      's2': ['s3', 's4'],
+      's3': ['s4'],
+      's4': ['s7'],
+      's5': ['s6'],
+      's6': ['s7', 's5'],
+      's7': ['s5'],
+   },
+}
+ks = KripkeStruct(ks_json)
+
+# check if the Kripke Structure satisfies the CTL formula: EX a
+sat_states = EX(ks, SAT_atom(ks, "a"))
+
+# the result should be {"s1"}
+# since the start state "s1" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {"s1"}
+
+# check if the Kripke Structure satisfies the CTL formula: E a U b
+sat_states = EU(ks, SAT_atom(ks, "a"), SAT_atom(ks, "b"))
+
+# the result should be {'s1', 's2', 's3', 's4', 's5'}
+# since the start state "s1" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {'s1', 's2', 's3', 's4', 's5'}
+
+# check if the Kripke Structure satisfies the CTL formula: EG a
+sat_states = EG(ks, SAT_atom(ks, "a"))
+
+# the result should be set()
+# since the start state "s1" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == set()
+```
+
 ## Contributing
 
 All contrbutions are welcome!
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details.
```

### Comparing `mctk-py-0.1.0/pyproject.toml` & `mctk-py-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "mctk-py"
 authors = [{name = "marcusm117", email = "marcusmin117@gmail.com"}]
 description="Model Checking Toolkit for Python"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.8"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

