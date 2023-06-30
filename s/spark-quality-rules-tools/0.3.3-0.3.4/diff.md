# Comparing `tmp/spark_quality_rules_tools-0.3.3.tar.gz` & `tmp/spark_quality_rules_tools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.3.tar", last modified: Fri Jun 30 19:06:36 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.4.tar", last modified: Fri Jun 30 23:06:37 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.3.tar` & `spark_quality_rules_tools-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/
--rw-rw-rw-   0        0        0     1092 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/README.md
--rw-rw-rw-   0        0        0      643 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-06-30 19:04:10.000000 spark_quality_rules_tools-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.045713 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2094 2023-06-30 13:36:52.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.061335 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    33747 2023-06-30 16:22:49.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.076962 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-11 22:08:20.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 16:22:49.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 14:07:09.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 13:58:14.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25817 2023-04-11 17:19:50.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3742 2023-06-30 18:59:43.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.061335 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 23:06:37.203467 spark_quality_rules_tools-0.3.4/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-06-30 23:06:37.203467 spark_quality_rules_tools-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.4/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-30 23:06:37.205467 spark_quality_rules_tools-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-06-30 23:06:22.000000 spark_quality_rules_tools-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 23:06:37.158458 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2094 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 23:06:37.182462 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    33899 2023-06-30 23:04:37.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 23:06:37.195466 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-06-30 23:06:37.202467 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-06-30 23:06:37.180462 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-06-30 23:06:37.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-06-30 23:06:37.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 23:06:37.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-06-30 23:06:37.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-30 23:06:37.000000 spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.3/LICENSE` & `spark_quality_rules_tools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/PKG-INFO` & `spark_quality_rules_tools-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.3/README.md` & `spark_quality_rules_tools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/pyproject.toml` & `spark_quality_rules_tools-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/setup.py` & `spark_quality_rules_tools-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.3',
+    version='0.3.4',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,14 @@
 
     conf_file = ConfigFactory.parse_string(txt_conf)
     hocons_file = HOCONConverter.to_hocon(conf_file)
     with open(dir_hocons_filename, "w") as f:
         f.write(hocons_file)
 
     spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
-
     conf = sc._jvm.java.io.File(dir_hocons_filename)
     ConfigFactory2 = sc._jvm.com.typesafe.config.ConfigFactory
     parsed_conf = ConfigFactory2.parseFile(conf)
     resolve_path = get_replace_resolve_parameter(sc=sc, resolve_name=resolve_name)
     resolvedConfig = parsed_conf.withFallback(resolve_path).resolve()
     Standalone = sc._jvm.com.datio.hammurabi.sandbox
     result = Standalone.Hammurabi.run(spark._jsparkSession, resolvedConfig)
@@ -477,14 +476,15 @@
         func.col("gf_field_physical_name").alias("Field"),
         func.col("gf_qr_aux_attribute_desc").alias("Format"),
         func.col("g_qr_critical_type").alias("Is Critical"),
         func.col("gf_qr_min_acceptance_per").alias("% Acceptation"),
         func.col("g_quality_rule_status_type").alias("Status"),
         func.col("gf_quality_rule_compliance_per").alias("Por"))
     df3 = df2.distinct().sort("gf_qr_functional_definition_id")
+    df3 = df3.select(*[func.col(col).cast("string") for col in df3.columns])
     df3.show(500, False, True)
 
     metrics_filter_pandas = df3.toPandas()
     metrics_filter_pandas.to_csv(dir_reports_name_filename, index=False)
 
     print(f"{get_color(f'================================')} ")
     print(f"{get_color('uuaa name :')} {get_color_b(uuaa_name)}")
@@ -596,15 +596,14 @@
 
     conf_file = ConfigFactory.parse_string(txt_conf)
     hocons_file = HOCONConverter.to_hocon(conf_file)
     with open(dir_hocons_filename, "w") as f:
         f.write(hocons_file)
 
     spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
-
     conf = sc._jvm.java.io.File(dir_hocons_filename)
     ConfigFactory2 = sc._jvm.com.typesafe.config.ConfigFactory
     parsed_conf = ConfigFactory2.parseFile(conf)
     resolve_path = get_replace_resolve_parameter(sc=sc, resolve_name=resolve_name)
     resolvedConfig = parsed_conf.withFallback(resolve_path).resolve()
     Standalone = sc._jvm.com.datio.hammurabi.sandbox
     result = Standalone.Hammurabi.run(spark._jsparkSession, resolvedConfig)
@@ -634,14 +633,15 @@
         func.col("gf_field_physical_name").alias("Field"),
         func.col("gf_qr_aux_attribute_desc").alias("Format"),
         func.col("g_qr_critical_type").alias("Is Critical"),
         func.col("gf_qr_min_acceptance_per").alias("% Acceptation"),
         func.col("g_quality_rule_status_type").alias("Status"),
         func.col("gf_quality_rule_compliance_per").alias("Por"))
     df3 = df2.distinct().sort("gf_qr_functional_definition_id")
+    df3 = df3.select(*[func.col(col).cast("string") for col in df3.columns])
     df3.show(500, False, True)
 
     metrics_filter_pandas = df3.toPandas()
     metrics_filter_pandas.to_csv(dir_reports_name_filename, index=False)
 
     print(f"{get_color(f'================================')} ")
     print(f"{get_color('uuaa name :')} {get_color_b(uuaa_name)}")
```

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.4/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

