# Comparing `tmp/proteomics_downstream_analysis-0.1.0.tar.gz` & `tmp/proteomics_downstream_analysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteomics_downstream_analysis-0.1.0.tar", last modified: Wed Jun 21 13:58:11 2023, max compression
+gzip compressed data, was "proteomics_downstream_analysis-0.1.1.tar", last modified: Sat Jul  1 18:17:18 2023, max compression
```

## Comparing `proteomics_downstream_analysis-0.1.0.tar` & `proteomics_downstream_analysis-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:58:11.317924 proteomics_downstream_analysis-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-21 13:58:11.317924 proteomics_downstream_analysis-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:58:11.313924 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/contamination.py
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/dataqualityinformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/dianndata.py
--rw-r--r--   0 runner    (1001) docker     (123)    18047 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/dimensionalityreduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    22567 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/enrichmentanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/multileveldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/preprocessing_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16009 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:58:11.313924 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-21 13:58:11.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-21 13:58:11.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:58:11.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 13:58:11.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 13:58:11.000000 proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:58:11.317924 proteomics_downstream_analysis-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:58:11.317924 proteomics_downstream_analysis-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_contamination.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_dataqualityinformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_dianndata.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_dimensionalityreduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_enrichmentanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_multileveldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_preprocessing_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-21 13:58:01.000000 proteomics_downstream_analysis-0.1.0/test/test_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:17:18.877780 proteomics_downstream_analysis-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-01 18:17:18.877780 proteomics_downstream_analysis-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:17:18.877780 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/contamination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/dataqualityinformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/dianndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18243 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/dimensionalityreduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22567 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/enrichmentanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/multileveldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/preprocessing_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16009 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:17:18.877780 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-01 18:17:18.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-01 18:17:18.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:17:18.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 18:17:18.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-01 18:17:18.000000 proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 18:17:18.877780 proteomics_downstream_analysis-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:17:18.877780 proteomics_downstream_analysis-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-01 18:17:05.000000 proteomics_downstream_analysis-0.1.1/tests/test_statistics.py
```

### Comparing `proteomics_downstream_analysis-0.1.0/LICENSE` & `proteomics_downstream_analysis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/contamination.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/contamination.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/dataqualityinformation.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/dataqualityinformation.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/dianndata.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/dianndata.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/dimensionalityreduction.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/dimensionalityreduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,16 +165,18 @@
                     fig.append_trace(plot['data'][idx], row=row_col[0], col=row_col[1])
 
           fig.update_layout(height=height, width=width, template='simple_white')
           fig.update_traces(marker=dict(size=12,
                                         line=dict(width=2,
                                                   color='DarkSlateGrey')),
                          selector=dict(mode='markers'))
-          fig.update_xaxes(title_text='PC1')
-          fig.update_yaxes(title_text='PC2')
+          pc1_eigenvalue = "%.2f" % pca_data.explained_variance_ratio_[0] * 100
+          pc2_eigenvalue = "%.2f" % pca_data.explained_variance_ratio_[1] * 100
+          fig.update_xaxes(title_text=f'PC1 {pc1_eigenvalue}')
+          fig.update_yaxes(title_text=f'PC2 {pc2_eigenvalue}')
 
           # Show the plot          
           if is_jupyter_notebook():
                fig.show()
           else:
                st.plotly_chart(fig, use_container_width=True)
```

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/enrichmentanalysis.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/enrichmentanalysis.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/imputer.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/imputer.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/multileveldata.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/multileveldata.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/preprocessing.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/preprocessing.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/preprocessing_preprocessor.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/preprocessing_preprocessor.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/preprocessor.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/preprocessor.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/proteomics_downstream_analysis/visualizer.py` & `proteomics_downstream_analysis-0.1.1/proteomics_downstream_analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `proteomics_downstream_analysis-0.1.0/setup.py` & `proteomics_downstream_analysis-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # Call setup function
 setup(
     name="proteomics_downstream_analysis",
     author="Vu Duc Tung",
     author_email="tungvuduc@outlook.de",
     description="A package for downstream data analysis of proteomics data",
     long_description=long_description,
-    long_description_content_type="text/x-rst",
+    long_description_content_type="text/markdown",
     keywords = ["proteomics", "downstream analysis", "data analysis", "data visualization", "mass spectrometry"],
-    version="0.1.0",
+    version="0.1.1",
     url="https://github.com/vuductung/proteomics-downstream-anlaysis",
     packages=find_packages(include=["proteomics_downstream_analysis", "proteomics_downstream_analysis.*"]),
     python_requires=">=3.6.1",
     install_requires=[
                     "adjustText",
                     "goatools",
                     "gseapy",
```

### Comparing `proteomics_downstream_analysis-0.1.0/test/test_preprocessing.py` & `proteomics_downstream_analysis-0.1.1/tests/test_preprocessing.py`

 * *Files identical despite different names*

