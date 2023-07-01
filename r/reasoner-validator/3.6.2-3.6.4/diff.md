# Comparing `tmp/reasoner_validator-3.6.2.tar.gz` & `tmp/reasoner_validator-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.6.2.tar", max compression
+gzip compressed data, was "reasoner_validator-3.6.4.tar", max compression
```

## Comparing `reasoner_validator-3.6.2.tar` & `reasoner_validator-3.6.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/LICENSE
--rw-r--r--   0        0        0    12621 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/README.md
--rw-r--r--   0        0        0      131 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/conf.py
--rw-r--r--   0        0        0    19641 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/make.bat
--rw-r--r--   0        0        0      136 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    35958 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/pyproject.toml
--rw-r--r--   0        0        0    37715 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    63014 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39199 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    28533 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4592 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     9721 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14009 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    10707 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      361 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/conftest.py
--rw-r--r--   0        0        0   114356 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62095 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml
--rw-r--r--   0        0        0    34174 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_response_validator.py
--rw-r--r--   0        0        0     5508 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_semver.py
--rw-r--r--   0        0        0     1521 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26543 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_validate.py
--rw-r--r--   0        0        0    20406 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_validation_report.py
--rw-r--r--   0        0        0     2061 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_workflows.py
--rw-r--r--   0        0        0    14660 1970-01-01 00:00:00.000000 reasoner_validator-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/LICENSE
+-rw-r--r--   0        0        0    12620 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/README.md
+-rw-r--r--   0        0        0      131 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/conf.py
+-rw-r--r--   0        0        0    19640 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    35958 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2092 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/pyproject.toml
+-rw-r--r--   0        0        0    38373 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    63014 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39199 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    28625 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4592 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     9721 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14009 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    10707 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      398 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/conftest.py
+-rw-r--r--   0        0        0   114356 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62095 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml
+-rw-r--r--   0        0        0    34174 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_response_validator.py
+-rw-r--r--   0        0        0     5508 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_semver.py
+-rw-r--r--   0        0        0     1886 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26525 2023-07-01 19:53:23.002430 reasoner_validator-3.6.4/tests/test_validate.py
+-rw-r--r--   0        0        0    20333 2023-07-01 19:53:23.002430 reasoner_validator-3.6.4/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-01 19:53:23.002430 reasoner_validator-3.6.4/tests/test_workflows.py
+-rw-r--r--   0        0        0    14658 1970-01-01 00:00:00.000000 reasoner_validator-3.6.4/PKG-INFO
```

### Comparing `reasoner_validator-3.6.2/LICENSE` & `reasoner_validator-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/README.md` & `reasoner_validator-3.6.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -138,16 +138,16 @@
 
 ### API
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
-  "trapi_version": "1.4.0-beta",
-  "biolink_version": "3.2.6",
+  "trapi_version": "1.4.0",
+  "biolink_version": "3.5.0",
   "sources": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
   "response": {<some full JSON object of a TRAPI query Response...>}
@@ -180,16 +180,16 @@
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
-  "trapi_version": "4",
-  "biolink_version": "3.2.1",
+  "trapi_version": "1.4.0",
+  "biolink_version": "3.5.0",
   "response": {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
```

### Comparing `reasoner_validator-3.6.2/docs/Makefile` & `reasoner_validator-3.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/docs/conf.py` & `reasoner_validator-3.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/docs/index.rst` & `reasoner_validator-3.6.4/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     }
     validator = TRAPIResponseValidator(
         trapi_version="1.4.0",
 
         # If omit or set the Biolink Model version parameter to None,
         # then the current Biolink Model Toolkit default release applies
-        biolink_version="3.2.6",
+        biolink_version="3.5.0",
 
         # 'sources' are set to trigger checking of expected edge knowledge source provenance
         sources={
                 "ara_source": "infores:molepro",
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
         },
@@ -258,15 +258,15 @@
         # If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'biolink_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the 'biolink_version' given here is assumed, which overrides the TRAPI Response stated 'biolink_version';
         # Otherwise, the TRAPI Response stated 'biolink_version' (not BMT) becomes the default validation version.
 
-        biolink_version="3.2.6",
+        biolink_version="3.5.0",
 
         "sources": {
             "ara_source": "infores:aragorn",
             "kp_source": "infores:panther",
             "kp_source_type": "primary"
         },
         "strict_validation": true,
@@ -305,15 +305,15 @@
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data as input to the **/validate** endpoint:
 
 .. code-block:: json
 
     {
         "schema_version": "1.4.0",
-        "biolink_version": "3.2.6",
+        "biolink_version": "3.5.0",
         "message": {
             "query_graph": {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {"categories": ["biolink:Drug"]}
                 },
                 "edges": {
@@ -368,16 +368,16 @@
     }
 
 then, one should typically get a response body like the following JSON validation result back:
 
 .. code-block:: json
 
     {
-      "trapi_version": "v1.4.0",
-      "biolink_version": "3.2.6",
+      "trapi_version": "1.4.0",
+      "biolink_version": "3.4.3",
       "messages": {
         "critical": {},
         "errors": {
           "error.knowledge_graph.node.category.missing": {
             "MONDO:0005148": [
               {
                 "context": "Knowledge Graph"
```

### Comparing `reasoner_validator-3.6.2/docs/make.bat` & `reasoner_validator-3.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/docs/validation_codes_dictionary.md` & `reasoner_validator-3.6.4/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/pyproject.toml` & `reasoner_validator-3.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.6.2"
+version = "3.6.4"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -37,15 +37,15 @@
 include = [
     { path = "tests" },
     { path = "docs" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-bmt = "^1.0.15"
+bmt = "^1.1.0"
 jsonschema = "^4.17.0"
 PyYAML = "^6.0"
 requests = "^2.28.1"
 pydantic = "^1.8.0"
 urllib3 = "^1.26.15"
 numpydoc = {version = "^1.5.0", optional = true}
 sphinx = {version = "^5.3.0", optional = true}
```

### Comparing `reasoner_validator-3.6.2/reasoner_validator/__init__.py` & `reasoner_validator-3.6.4/reasoner_validator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,16 @@
                     self.report("warning.trapi.response.workflow.parameters.null")
                     step.pop('parameters')
         return response
 
     def check_compliance_of_trapi_response(
             self,
             response: Optional[Dict],
-            edges_limit: int = 100
+            max_kg_edges: int = 0,
+            max_results: int = 0
     ):
         """
         One stop validation of all components of a TRAPI-schema compliant
         Query.Response, including its Message against a designated Biolink Model release.
         The high level structure of a Query.Response is described in
         https://github.com/NCATSTranslator/ReasonerAPI/blob/master/docs/reference.md#response-.
 
@@ -131,17 +132,20 @@
         * Knowledge Graph: output knowledge (sub-)graph containing knowledge (Biolink Model compliant nodes, edges)
                            returned from the target resource (KP, ARA) for the query.
         * Results: a list of (annotated) node and edge bindings pointing into the Knowledge Graph, to represent the
                    specific answers (subgraphs) satisfying the query graph constraints.
 
         :param response: Query.Response to be validated.
         :type response: Optional[Dict]
-        :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
-                            triggers validation of all edges in the knowledge graph (Default: 100)
-        :type edges_limit: int
+        :param max_kg_edges: integer maximum number of edges to be validated from the
+                                     knowledge graph of the response. A value of zero triggers validation
+                                      of all edges in the knowledge graph (Default: 0 - use all edges)
+        :type max_kg_edges: int
+        :param max_results: target sample number of results to validate (default: 0 for 'use all results').
+        :type max_results: int
 
         :returns: Validator cataloging "information", "warning" and "error" messages (could be empty)
         :rtype: ValidationReporter
         """
         if not (response and "message" in response):
             if not self.suppress_empty_data_warnings:
                 self.report("error.trapi.response.empty")
@@ -170,37 +174,42 @@
         status: Optional[str] = response['status'] if 'status' in response else None
         if status and status not in ["OK", "Success", "QueryNotTraversable", "KPsNotAvailable"]:
             self.report("warning.trapi.response.status.unknown", identifier=status)
 
         # Sequentially validate the Query Graph, Knowledge Graph then validate
         # the Results (which rely on the validity of the other two components)
         elif self.has_valid_query_graph(message) and \
-                self.has_valid_knowledge_graph(message, edges_limit):
-            self.has_valid_results(message)
+                self.has_valid_knowledge_graph(message, max_kg_edges):
+            self.has_valid_results(message, max_results)
 
     @staticmethod
-    def sample_results(results: List) -> List:
+    def sample_results(results: List, sample_size: int = 0) -> List:
         """
+        Subsample the results to a maximum size of 'sample_size'
 
         :param results: List, original list of Results
-        :return: List, RESULT_TEST_DATA_SAMPLE_SIZE sized subset of Results
+        :param sample_size: int, target sample size (default: 0 for 'use all results').
+
+        :return: List, 'sample_size' sized subset of Results
         """
-        sample_size = min(RESULT_TEST_DATA_SAMPLE_SIZE, len(results))
-        result_subsample = results[0:sample_size]
-        return result_subsample
+        if sample_size > 0:
+            sample_size = min(sample_size, len(results))
+            return results[0:sample_size]
+        else:
+            return results
 
     @staticmethod
-    def sample_graph(graph: Dict, edges_limit: int = 100) -> Dict:
+    def sample_graph(graph: Dict, edges_limit: int = 0) -> Dict:
         """
         Only process a strict subsample of the TRAPI Response Message knowledge graph.
 
         :param graph: original knowledge graph
         :type graph: Dict
         :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
-                            triggers validation of all edges in the knowledge graph (could take a while! Default: 100)
+                            triggers validation of all edges in the knowledge graph (Default: 0 - use all edges)
         :type edges_limit: int
 
         :return: Dict, 'edges_limit' sized subset of knowledge graph
         """
         # We don't check for non-empty graphs here simply because the sole caller of this
         # method is the 'has_valid_knowledge_graph' method, which filters out empty graphs
         if edges_limit > 0:
@@ -282,28 +291,28 @@
                         self.merge(biolink_validator)
                         # 'info' and 'warning' messages do
                         # not fully invalidate the query_graph
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
-    def has_valid_knowledge_graph(self, message: Dict, edges_limit: int = 100) -> bool:
+    def has_valid_knowledge_graph(self, message: Dict, edges_limit: int = 0) -> bool:
         """
         Validate a TRAPI Knowledge Graph.
 
         :param message: input message expected to contain the 'knowledge_graph'
         :type message: Dict
         :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
-                            triggers validation of all edges in the knowledge graph (could take a while! Default: 100)
+                            triggers validation of all edges in the knowledge graph (Default: 0 - use all edges)
         :type edges_limit: int
 
         :return: bool, False, if validation errors
         """
         # This integrity constraint may not really be necessary
-        # since negative numbers are functionally inequivalent to zero
+        # since negative numbers are functionally equivalent to zero
         assert edges_limit >= 0, "The 'edges_limit' must be zero or a positive integer!"
 
         # The Knowledge Graph should not be missing
         if 'knowledge_graph' not in message:
             if not self.suppress_empty_data_warnings:
                 self.report(code="error.trapi.response.knowledge_graph.missing")
         else:
@@ -351,18 +360,21 @@
                         )
                     if biolink_validator.has_messages():
                         self.merge(biolink_validator)
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
-    def has_valid_results(self, message: Dict) -> bool:
+    def has_valid_results(self, message: Dict, sample_size: int = 0) -> bool:
         """
         Validate a TRAPI Results.
+
         :param message: input message expected to contain the 'results'
+        :param sample_size: int, sample number of results to validate (default: 0 for 'use all results').
+
         :return: bool, False, if validation errors
         """
 
         #     :param output_element: test target, as edge 'subject' or 'object'
         #     :type output_element: str
         #     :param output_node_binding: node 'a' or 'b' of the ('one hop') QGraph test query
         #     :type output_node_binding: str
@@ -393,15 +405,15 @@
                 # The Message.results should be an array of Result objects
                 # TODO: Is this test unnecessary, since TRAPI schema
                 #       validation (below) should normally catch this?
                 self.report(code="error.trapi.response.results.non_array")
 
             else:
                 # Validate a subsample of a non-empty Message.results component.
-                results_sample = self.sample_results(results)
+                results_sample = self.sample_results(results, sample_size=sample_size)
                 for result in results_sample:
 
                     # generally validate against the pertinent schema
                     trapi_validator: TRAPISchemaValidator = check_trapi_validity(
                         instance=result,
                         component="Result",
                         trapi_version=self.trapi_version
@@ -518,16 +530,18 @@
         :param object_id:  str, subject node (CURIE) identifier
         :param edge_id:  str, subject node (CURIE) identifier
         :param results: List of (TRAPI-version specific) Result objects
         :param trapi_version: str, target TRAPI version of the Response being validated
         :return: bool, True if case S-P-O edge was found in the results
         """
         trapi_1_4_0: bool
-        try:    # try block ... Sanity check: in case the trapi_version is somehow invalid?
-            target_version: SemVer = SemVer.from_string(trapi_version)
+        try:
+            # try block ... Sanity check: in case the trapi_version is somehow invalid?
+            # ignore any prerelease/build qualifiers
+            target_version: SemVer = SemVer.from_string(trapi_version, ext_fields=[])
             trapi_1_4_0 = target_version >= SemVer.from_string("1.4.0")
         except SemVerError as sve:
             logger.warning(f"case_result_found() 'trapi_version' seems invalid: {str(sve)}. Default to latest?")
             trapi_1_4_0 = True
 
         result_found: bool = False
         result: Dict
```

### Comparing `reasoner_validator-3.6.2/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.6.4/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/reasoner_validator/codes.yaml` & `reasoner_validator-3.6.4/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/reasoner_validator/report.py` & `reasoner_validator-3.6.4/reasoner_validator/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,25 +402,25 @@
         """
         Wrapper to allow validation_methods direct access to the ValidationReporter.
 
         :param validation_method: function which accepts this instance of the
                ValidationReporter as its first argument, for use in reporting validation errors.
         :param args: any positional arguments to the validation_method, after the initial ValidationReporter argument
         :param kwargs: any (optional, additional) keyword arguments to the validation_method, after positional arguments
-        :return: bool, returns 'False' if validation method documented errors; True otherwise
+        :return: bool, returns 'False' if validation method documented (critical) errors; True otherwise
         """
         validation_method(self, *args, **kwargs)
         # TODO: not sure if we should detect both 'errors' and 'critical' here or just 'critical'
         if self.has_critical() or self.has_errors():
             return False
         else:
             return True
 
     @staticmethod
-    def has_validation_errors(tag: str, case: Dict) -> bool:
+    def test_case_has_validation_errors(tag: str, case: Dict) -> bool:
         """Check if test case has validation errors.
 
         :param tag: str, top level string key in the 'case' whose value is the validation messages 'dictionary'
         :param case: Dict, containing error messages in a structurally similar
                      format to what is returned by the to_dict() method in this class.
         :return: True if the case contains validation messages
         """
@@ -431,17 +431,19 @@
         #     tag: {
         #         "trapi_version": "1.3",
         #         "biolink_version": "3.0.2",
         #         "messages": {
         #             "information": [],
         #             "warnings": [
         #                 {
-        #                     "warning.predicate.non_canonical": [
-        #                         {"predicate": "biolink:participates_in"}  xxx deprecated? better check this one!
-        #                     ]
+        #                     "warning.predicate.non_canonical": {
+        #                         "biolink:participates_in": {
+        #                               "edge_id": "a--['biolink:participates_in']->b"
+        #                         }
+        #                     }
         #                 }
         #             ],
         #             "errors": [
         #                 {
         #                     "error.knowledge_graph.empty_nodes": None
         #                 }
         #             ],
```

### Comparing `reasoner_validator-3.6.2/reasoner_validator/sri/util.py` & `reasoner_validator-3.6.4/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.6.4/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.6.4/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/reasoner_validator/validation_codes.py` & `reasoner_validator-3.6.4/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/reasoner_validator/versioning.py` & `reasoner_validator-3.6.4/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.6.4/tests/test_biolink_compliance_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1542,15 +1542,15 @@
         #                     }
         #                 ]
         #             }
         #         ]
         #     },
         #     ""    # this other use case should also pass
         # ),
-        (   # Query 18 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
+        (   # Query 17 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
             #            with a Biolink predicate as its value
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:qualified_predicate",
@@ -1558,15 +1558,15 @@
                             }
                         ]
                     }
                 ]
             },
             ""  # this particular use case should also pass
         ),
-        (   # Query 19 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
+        (   # Query 18 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
             #            an incorrect value, which is not a Biolink predicate
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:qualified_predicate",
```

### Comparing `reasoner_validator-3.6.2/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml` & `reasoner_validator-3.6.4/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/tests/test_response_validator.py` & `reasoner_validator-3.6.4/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/tests/test_semver.py` & `reasoner_validator-3.6.4/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.2/tests/test_trapi_versioning.py` & `reasoner_validator-3.6.4/tests/test_trapi_versioning.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 
 
 def test_unknown_semver_spec_trapi_version():
     trapi_version: str = get_latest_version(release_tag="2")
     assert trapi_version is None
 
 
+def test_semver_spec_trapi_version_with_prefix():
+    trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_VERSION)
+    assert trapi_version == LATEST_TRAPI_VERSION
+
+
+def test_semver_spec_trapi_version_without_prefix():
+    trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_VERSION[1:])
+    assert trapi_version == LATEST_TRAPI_VERSION
+
+
 def test_schema_spec_trapi_version():
     trapi_version = get_latest_version(release_tag=SAMPLE_SCHEMA_FILE)
     assert trapi_version is not None
     assert trapi_version.endswith(".yaml")
 
 
 def test_load_schema_with_semver_trapi_version():
```

### Comparing `reasoner_validator-3.6.2/tests/test_validate.py` & `reasoner_validator-3.6.4/tests/test_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 import pytest
 
 from jsonschema.exceptions import ValidationError
 
 from reasoner_validator.trapi import TRAPISchemaValidator, openapi_to_jsonschema, load_schema
 
+from tests import LATEST_TEST_VERSIONS
+
 PRE_1_4_0_TEST_VERSIONS = "1.2", "1.2.0", "1.3", "1.3.0"
-LATEST_TEST_VERSIONS = "1", "1.4", "1.4.0", "1.4.0-beta4"
 ALL_TEST_VERSIONS = PRE_1_4_0_TEST_VERSIONS + LATEST_TEST_VERSIONS
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (  # query 0
```

### Comparing `reasoner_validator-3.6.2/tests/test_validation_report.py` & `reasoner_validator-3.6.4/tests/test_validation_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,14 @@
     errors: List[str] = list()
     for code, parameters in messages['errors'].items():
         errors.extend(CodeDictionary.display(code, parameters, add_prefix=True))
     assert "ERROR - Knowledge Graph Edge Provenance Infores: " + \
            "Edge has provenance value which is not a well-formed InfoRes CURIE" in errors
 
 
-# has_validation_errors(root_key: str = 'validation', case: Optional[Dict] = None)
 @pytest.mark.parametrize(
     "query",
     [
         (
             'validation',
             {
                 "validation": {
@@ -489,8 +488,8 @@
             },
             False
         ),
     ]
 )
 def test_has_validation_errors(query: Tuple):
     reporter = ValidationReporter()
-    assert reporter.has_validation_errors(tag=query[0], case=query[1]) == query[2]
+    assert reporter.test_case_has_validation_errors(tag=query[0], case=query[1]) == query[2]
```

### Comparing `reasoner_validator-3.6.2/tests/test_workflows.py` & `reasoner_validator-3.6.4/tests/test_workflows.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 from typing import Dict
 from itertools import product
 from json import dumps
 
 from reasoner_validator.trapi import TRAPISchemaValidator
 
-LATEST_TEST_VERSIONS = "1", "1.4", "1.4.0", "1.4.0-beta4"
+from tests import LATEST_TEST_VERSIONS
 
 SAMPLE_QUERY_1 = {
     "message": {
         "knowledge_graph": None,
         "query_graph": None,
         "results": None,
     },
```

### Comparing `reasoner_validator-3.6.2/PKG-INFO` & `reasoner_validator-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.6.2
+Version: 3.6.4
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: bmt (>=1.0.15,<2.0.0)
+Requires-Dist: bmt (>=1.1.0,<2.0.0)
 Requires-Dist: fastapi (>=0.68,<0.69) ; extra == "web"
 Requires-Dist: jsonschema (>=4.17.0,<5.0.0)
 Requires-Dist: myst-parser (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.8.0,<2.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0) ; extra == "dev"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "dev"
@@ -181,16 +181,16 @@
 
 ### API
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
-  "trapi_version": "1.4.0-beta",
-  "biolink_version": "3.2.6",
+  "trapi_version": "1.4.0",
+  "biolink_version": "3.5.0",
   "sources": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
   "response": {<some full JSON object of a TRAPI query Response...>}
@@ -223,16 +223,16 @@
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
-  "trapi_version": "4",
-  "biolink_version": "3.2.1",
+  "trapi_version": "1.4.0",
+  "biolink_version": "3.5.0",
   "response": {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
```

