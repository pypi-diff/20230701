# Comparing `tmp/bmt-1.0.9.tar.gz` & `tmp/bmt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmt-1.0.9.tar", max compression
+gzip compressed data, was "bmt-1.1.0.tar", max compression
```

## Comparing `bmt-1.0.9.tar` & `bmt-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1544 2023-04-03 23:19:11.932956 bmt-1.0.9/LICENSE
--rw-r--r--   0        0        0     1110 2023-04-03 23:19:11.932956 bmt-1.0.9/README.md
--rw-r--r--   0        0        0       31 2023-04-03 23:19:11.932956 bmt-1.0.9/bmt/__init__.py
--rw-r--r--   0        0        0    57299 2023-04-03 23:19:11.936956 bmt-1.0.9/bmt/toolkit.py
--rw-r--r--   0        0        0     3843 2023-04-03 23:19:11.936956 bmt-1.0.9/bmt/utils.py
--rw-r--r--   0        0        0     1617 2023-04-03 23:19:32.585241 bmt-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 bmt-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1544 2023-06-30 23:39:14.959893 bmt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1110 2023-06-30 23:39:14.959893 bmt-1.1.0/README.md
+-rw-r--r--   0        0        0       31 2023-06-30 23:39:14.959893 bmt-1.1.0/bmt/__init__.py
+-rw-r--r--   0        0        0    57582 2023-06-30 23:39:14.959893 bmt-1.1.0/bmt/toolkit.py
+-rw-r--r--   0        0        0     3843 2023-06-30 23:39:14.959893 bmt-1.1.0/bmt/utils.py
+-rw-r--r--   0        0        0     1585 2023-06-30 23:39:34.332389 bmt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 bmt-1.1.0/PKG-INFO
```

### Comparing `bmt-1.0.9/LICENSE` & `bmt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmt-1.0.9/README.md` & `bmt-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bmt-1.0.9/bmt/toolkit.py` & `bmt-1.1.0/bmt/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import yaml
 import csv
 import deprecation
 import requests
-from oaklib.implementations import UbergraphImplementation
 from functools import lru_cache, reduce
 
 from typing import List, Union, TextIO, Optional, Dict
 from linkml_runtime.utils.schemaview import SchemaView, Namespaces
 from linkml_runtime.linkml_model.meta import (
     SchemaDefinition,
     Element,
@@ -18,17 +17,16 @@
 )
 from pprint import pprint
 from bmt.utils import format_element, parse_name
 
 Url = str
 Path = str
 
-REMOTE_PATH = "https://raw.githubusercontent.com/biolink/biolink-model/v3.2.6/biolink-model.yaml"
-PREDICATE_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.2.6/predicate_mapping.yaml'
-INFORES_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.2.6/infores_catalog_nodes.tsv'
+REMOTE_PATH = "https://raw.githubusercontent.com/biolink/biolink-model/v3.5.0/biolink-model.yaml"
+PREDICATE_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.5.0/predicate_mapping.yaml'
 
 
 NODE_PROPERTY = "node property"
 ASSOCIATION_SLOT = "association slot"
 RELATED_TO = "related to"
 
 CACHE_SIZE = 1024
@@ -45,38 +43,20 @@
     schema: Union[str, TextIO, SchemaDefinition]
         The path or url to an instance of the biolink-model.yaml file.
 
     """
 
     def __init__(
             self, schema: Union[Url, Path, TextIO, SchemaDefinition] = REMOTE_PATH,
-            predicate_map: Url = PREDICATE_MAP,
-            infores_map: Url = INFORES_MAP
+            predicate_map: Url = PREDICATE_MAP
     ) -> None:
-        self.oi = UbergraphImplementation()
         self.view = SchemaView(schema)
         r = requests.get(predicate_map)
         self.pmap = yaml.safe_load(r.text)
 
-        r = requests.get(infores_map)
-        content = r.content.decode('iso-8859-1')
-        self.infores_map = {}
-        for line in csv.reader(content.splitlines(), delimiter='\t'):
-            if line[2] == 'id':
-                continue
-            self.infores_map[line[2]] = {
-                "status": line[0],
-                "name": line[1],
-                "url": line[3],
-                "synonyms": line[4],
-                "has_contributor": line[6],
-                "description": line[7],
-                "category": line[8]
-            }
-
     @lru_cache(CACHE_SIZE)
     def get_all_elements(self, formatted: bool = False) -> List[str]:
         """
         Get all elements from Biolink Model.
 
         This method returns a list containing all
         classes, slots, and types defined in the model.
@@ -316,37 +296,14 @@
         """
         ancestors = self.view.permissible_value_ancestors(permissible_value, enum_name)
         if formatted:
             return self._format_all_elements(ancestors)
         return ancestors
 
     @lru_cache(CACHE_SIZE)
-    def get_infores_details(self, infores_id: str):
-        """
-        Get details of an information resource.
-
-        This method returns a dictionary containing details of a given
-        information resource.
-
-        Parameters
-        ----------
-        infores_id: str
-            The identifier of the information resource
-
-        Returns
-        -------
-        Dict[str, Any]
-            A dictionary containing details of the information resource
-
-        """
-        pprint(self.infores_map)
-        infores = self.infores_map.get(infores_id)
-        return infores
-
-    @lru_cache(CACHE_SIZE)
     def get_predicate_mapping(self, mapped_predicate: str) -> Dict[str, str]:
         """
         Get the predicates that map to a given predicate.
 
         This method returns a list containing all the predicates that map to
         a given predicate.
 
@@ -624,32 +581,29 @@
         Returns
         -------
         List[str]
             The domain for a given slot
 
         """
         slot_domain = []
-        domain_classes = set()
+        slot_domain_desc = []
         element = self.get_element(slot_name)
-        if element and element.domain:
-            domain_classes.add(element.domain)
-            if include_ancestors:
-                slot_domain.extend(
-                    self.get_ancestors(element.domain, reflexive=True, mixin=mixin)
-                )
-            else:
+        if element:
+            if element.domain:
                 slot_domain.append(element.domain)
-        for d in element.domain_of:
-            if d not in domain_classes:
+            else:
                 if include_ancestors:
-                    slot_domain.extend(
-                        self.get_ancestors(d, reflexive=True, mixin=mixin)
-                    )
-                else:
-                    slot_domain.append(d)
+                    for element in self.get_ancestors(element.name):
+                        tk_element = self.get_element(element)
+                        if tk_element and tk_element.domain:
+                            slot_domain.append(tk_element.domain)
+            if slot_domain:
+                for domain in slot_domain:
+                    slot_domain_desc = self.get_descendants(domain, reflexive=True, mixin=mixin)
+                slot_domain.extend(slot_domain_desc)
         return self._format_all_elements(slot_domain, formatted)
 
     def get_slot_range(
             self,
             slot_name,
             include_ancestors: bool = False,
             formatted: bool = False,
@@ -673,22 +627,86 @@
         Returns
         -------
         List[str]
             The range for a given slot
 
         """
         slot_range = []
+        slot_range_desc = []
         element = self.get_element(slot_name)
-        if element and element.range:
-            slot_range.append(element.range)
-            if include_ancestors:
-                ancs = self.get_ancestors(element.range, reflexive=False, mixin=mixin)
-                slot_range.extend(ancs)
+        if element:
+            if element.range:
+                slot_range.append(element.range)
+            else:
+                if include_ancestors:
+                    for element in self.get_ancestors(element.name):
+                        tk_element = self.get_element(element)
+                        if tk_element and tk_element.range:
+                            slot_range.append(tk_element.range)
+            if slot_range:
+                for range in slot_range:
+                    slot_range_desc = self.get_descendants(range, reflexive=True, mixin=mixin)
+                slot_range.extend(slot_range_desc)
         return self._format_all_elements(slot_range, formatted)
 
+    def validate_edge(self, subject: str, predicate: str, p_object: str, ancestors: bool = True) -> bool:
+        """
+        Validates an edge.
+
+        Parameters
+        ----------
+        subject: str
+            The name or alias of a subject in the Biolink Model
+        predicate: str
+            The name or alias of a predicate in the Biolink Model
+        p_object: str
+            The name or alias of an object in the Biolink Model
+        ancestors: bool
+            Whether to include ancestors of the domain and range classes
+
+        Returns
+        -------
+        bool
+            Whether or not the given edge is valid
+
+        """
+        if self.is_predicate(predicate):
+            predicate_domains = self.get_slot_domain(predicate, include_ancestors=True, mixin=True, formatted=True)
+            predicate_ranges = self.get_slot_range(predicate, include_ancestors=True, mixin=True, formatted=True)
+
+            if subject in predicate_domains and p_object in predicate_ranges:
+                return True
+            else:
+                subject_entity = self.get_element(subject)
+                object_entity = self.get_element(p_object)
+
+                if subject_entity and object_entity:
+                    subject_ancestors = self.get_ancestors(subject_entity.name, formatted=True, mixin=True)
+                    object_ancestors = self.get_ancestors(object_entity.name, formatted=True, mixin=True)
+                    # this is kind of hacky, the issue is that mixins don't descend from any shared class
+                    # like NamedThing.
+                    if self.is_mixin(subject_entity.name):
+                        subject_ancestors.append("biolink:NamedThing")
+                    if self.is_mixin(object_entity.name):
+                        object_ancestors.append("biolink:NamedThing")
+                    subject_in_domain = False
+                    object_in_range = False
+                    for subject_ancestor in subject_ancestors:
+                        if subject_ancestor in predicate_domains:
+                            subject_in_domain = True
+                    for object_ancestor in object_ancestors:
+                        if object_ancestor in predicate_ranges:
+                            object_in_range = True
+                    if subject_in_domain and object_in_range:
+                        return True
+                else:
+                    return False
+
+        return False
+
     def validate_qualifier(self, qualifier_type_id: str, qualifier_value: str) -> bool:
         """
         Validates a qualifier.
 
         Parameters
         ----------
         qualifier_type_id: str
@@ -706,16 +724,15 @@
             qualifier_slot = self.view.get_slot(parse_name(qualifier_type_id))
             # slot may just be missing from the model or
             # the range will be None for abstract/mixin qualifiers,
             # or the range may be just plain missing from the model
             if qualifier_slot and qualifier_slot.range is not None:
                 if self.is_enum(qualifier_slot.range):
                     enum = self.view.get_enum(qualifier_slot.range)
-                    if self.is_permissible_value_of_enum(enum.name, qualifier_value) or \
-                            self.is_reachable_from_enum(enum.name, qualifier_value):
+                    if self.is_permissible_value_of_enum(enum.name, qualifier_value):
                         return True
                 else:  # possible Biolink categorical qualifier
                     categories = self.get_element_by_prefix(qualifier_value)
                     if categories and qualifier_slot.range in categories:
                         return True
         return False
 
@@ -1175,27 +1192,27 @@
     @lru_cache(CACHE_SIZE)
     def get_inverse(self, slot_name: str):
         return self.view.inverse(slot_name)
 
     @lru_cache(CACHE_SIZE)
     def has_inverse(self, name: str) -> bool:
         """
-        Determines whether the given name is a predicate and if that predicate has an inverse defined
-        in the Biolink Model. An element is a predicate if it descends from
-        `RELATED_TO`
+        Determines whether the given name exists and has an inverse defined in the Biolink Model.
+        An element is a predicate if it descends from `RELATED_TO` but this is
+        not directly tested here (use the method 'is_predicate()' to be sure).
 
         Parameters
         ----------
         name: str
-            The name or alias of an element in the Biolink Model
+            The name or alias of an slot element in the Biolink Model
 
         Returns
         -------
         bool
-            That the named element is a valid mixin in Biolink Model
+            That the named element is a slot element with an inverse in the Biolink Model
         """
         element = self.get_element(name)
         has_inverse = element.inverse if isinstance(element, SlotDefinition) else False
         return bool(has_inverse)
 
     @lru_cache(CACHE_SIZE)
     def in_subset(self, name: str, subset: str) -> bool:
@@ -1282,43 +1299,14 @@
         else:
             enum = self.view.get_enum(name)
         if not enum:
             return False
         return True
 
     @lru_cache(CACHE_SIZE)
-    def is_reachable_from_enum(self, enum_name: str, value) -> bool:
-        """
-        method to test (by name) if a candidate
-        'reachable value' ontology term is associated with the given Enum
-
-        Parameters
-        ----------
-        enum_name : str
-            The name or alias of an Enum in the Biolink Model
-        value : Any
-            The name or alias of the candidate 'reachable value' associated with the given Enum
-
-        Returns
-        -------
-        bool
-            That the named element is a valid 'reachable value' in the Enum
-        """
-        if self.is_enum(enum_name):
-            enum = self.view.get_enum(enum_name)
-            if enum.reachable_from is not None and enum.reachable_from.source_ontology:
-                if value in self.oi.descendants(enum.reachable_from.source_nodes,
-                                                enum.reachable_from.relationship_types):
-                    return True
-                else:
-                    return False
-        else:
-            return False
-
-    @lru_cache(CACHE_SIZE)
     def is_permissible_value_of_enum(self, enum_name: str, value) -> bool:
         """
         method to test (by name) if a candidate
         'permissible value' is associated with the given Enum
 
         Parameters
         ----------
@@ -1335,16 +1323,14 @@
 
         if ":" in enum_name:
             enum = self.view.get_enum(enum_name.split(":")[1])
         else:
             enum = self.view.get_enum(enum_name, strict=True)
         if enum and value in enum.permissible_values:
             return True
-        if self.is_reachable_from_enum(enum_name, value):
-            return True
         else:
             return False
 
     @lru_cache(CACHE_SIZE)
     def get_element_by_prefix(
             self,
             identifier: str
```

### Comparing `bmt-1.0.9/bmt/utils.py` & `bmt-1.1.0/bmt/utils.py`

 * *Files identical despite different names*

### Comparing `bmt-1.0.9/pyproject.toml` & `bmt-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmt"
-version = "1.0.9"
+version = "1.1.0"
 description = "Biolink Model Toolkit: A Python API for working with the Biolink Model"
 authors = ["Sierra Taylor Moxon <sierra.taylor@gmail.com>"]
 license = "BSD"
 
 readme = "README.md"
 repository = "https://github.com/biolink/biolink-model-toolkit"
 documentation = "https://biolink.github.io/biolink-model-toolkit/"
@@ -32,28 +32,26 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-linkml-runtime = "^1.4.9"
+linkml-runtime = "^1.5.0"
 deprecation = "^2.1.0"
 stringcase = "^1.2.0"
-oaklib = "^0.3.1"
-recommonmark = "^0.7.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 Sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 sphinxcontrib-napoleon = "^0.7"
-sphinx-autodoc-typehints = "^1.19.5"
+recommonmark = "^0.7.1"
+# sphinx-autodoc-typehints = "^1.19.5"
 sphinx-click = "^4.3.0"
-twine = "^4.0.1"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinxcontrib-mermaid"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
-build-backend = "poetry_dynamic_versioning.backend"
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `bmt-1.0.9/PKG-INFO` & `bmt-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmt
-Version: 1.0.9
+Version: 1.1.0
 Summary: Biolink Model Toolkit: A Python API for working with the Biolink Model
 Home-page: https://github.com/biolink/biolink-model-toolkit
 License: BSD
 Keywords: schema,linked data,data modeling,biolink,api
 Author: Sierra Taylor Moxon
 Author-email: sierra.taylor@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,23 +15,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
-Requires-Dist: linkml-runtime (>=1.4.9,<2.0.0)
-Requires-Dist: oaklib (>=0.3.1,<0.4.0)
-Requires-Dist: recommonmark (>=0.7.1,<0.8.0)
+Requires-Dist: linkml-runtime (>=1.5.0,<2.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Project-URL: Documentation, https://biolink.github.io/biolink-model-toolkit/
 Project-URL: Repository, https://github.com/biolink/biolink-model-toolkit
 Description-Content-Type: text/markdown
 
 [![Python](https://img.shields.io/badge/python-3.7+-blue.svg)]()
 [![PyPI](https://img.shields.io/pypi/v/bmt)](https://img.shields.io/pypi/v/bmt)
```

