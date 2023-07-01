# Comparing `tmp/vlab_prepro-0.3.5.tar.gz` & `tmp/vlab_prepro-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlab_prepro-0.3.5.tar", max compression
+gzip compressed data, was "vlab_prepro-0.4.0.tar", max compression
```

## Comparing `vlab_prepro-0.3.5.tar` & `vlab_prepro-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1172 2021-05-18 16:46:20.874302 vlab_prepro-0.3.5/LICENSE
--rw-r--r--   0        0        0      513 2021-09-07 08:20:08.385318 vlab_prepro-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      160 2021-09-07 08:20:12.702045 vlab_prepro-0.3.5/vlab_prepro/__init__.py
--rw-r--r--   0        0        0     7841 2021-09-07 08:05:44.523316 vlab_prepro-0.3.5/vlab_prepro/preprocess.py
--rw-r--r--   0        0        0      618 2021-09-07 08:20:25.325446 vlab_prepro-0.3.5/setup.py
--rw-r--r--   0        0        0      327 2021-09-07 08:20:25.325686 vlab_prepro-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1172 2021-05-18 16:46:20.874302 vlab_prepro-0.4.0/LICENSE
+-rw-r--r--   0        0        0      513 2023-07-01 17:23:54.900706 vlab_prepro-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      160 2021-09-07 08:20:12.702045 vlab_prepro-0.4.0/vlab_prepro/__init__.py
+-rw-r--r--   0        0        0     8098 2023-07-01 17:20:13.800915 vlab_prepro-0.4.0/vlab_prepro/preprocess.py
+-rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 vlab_prepro-0.4.0/PKG-INFO
```

### Comparing `vlab_prepro-0.3.5/LICENSE` & `vlab_prepro-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlab_prepro-0.3.5/pyproject.toml` & `vlab_prepro-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "vlab_prepro"
-version = "0.3.5"
+version = "0.4.0"
 description = ""
 authors = ["Nandan Rao <nandanmarkrao@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 toolz = "^0.11.1"
-pandas = "^1.2.4"
+pandas = "^2.0.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.3"
 pytest-xdist = "^2.2.1"
 python-language-server = {extras = ["all"], version = "^0.36.2"}
 pyls-isort = "^0.2.0"
 pyls-black = "^0.4.6"
```

### Comparing `vlab_prepro-0.3.5/vlab_prepro/preprocess.py` & `vlab_prepro-0.4.0/vlab_prepro/preprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,30 +8,33 @@
 
 
 class PreprocessingError(BaseException):
     pass
 
 
 def wrap_empty(fn):
-    def _wrapper(df):
+    def _wrapper(df, *args, **kwargs):
         if df.shape[0] == 0:
             return None
-        return fn(df)
+        return fn(df, *args, **kwargs)
 
     return _wrapper
 
 
-def _flatten_dict(col, r):
+def _flatten_dict(col, r, prefix):
     for k, v in json.loads(r[col]).items():
-        r[k] = v
+        if prefix is None:
+            r[k] = v
+        else:
+            r[f"{prefix}_{k}"] = v
     return r
 
 
-def flatten_dict(col, df):
-    return df.apply(lambda r: _flatten_dict(col, r), 1).drop(columns=[col])
+def flatten_dict(col, df, prefix=None):
+    return df.apply(lambda r: _flatten_dict(col, r, prefix), 1).drop(columns=[col])
 
 
 def _new_cols(left, right):
     left = {k for k in left.columns}
     return {k for k in right.columns if k not in left}
 
 
@@ -58,27 +61,32 @@
     df.loc[
         df.duplicated(["userid", "surveyid", "question_idx"], keep="last"),
         "final_answer",
     ] = False
     return df
 
 
+@curry
+def _assign(name, fn, tindex, d):
+    return d.assign(**{name: fn(d.index[0])})
+
+
 def _add_time_indicators(indicators, df):
     tindex = "survey_start_time"
 
     if tindex not in df.columns:
         raise KeyError(f"Could no find time index: {tindex} in dataframe columns")
 
     for name, frame, fn in indicators:
         df = (
-            df.resample(frame, on=tindex)
-            .apply(wrap_empty(lambda d: d.assign(**{name: fn(d[tindex].iloc[0])})))
-            .reset_index(drop=True)
+            df.set_index(tindex)
+            .resample(frame)
+            .apply(wrap_empty(_assign(name, fn, tindex)))
+            .reset_index()
         )
-
     return df
 
 
 def drop_duplicated_users(form_keys, df):
     # form_keys should uniquely identify your form
     # (i.e. shortcode! Or, if there are multiple shortcodes that shouldn't
     # be taken twice, some other metadata that the forms have to identify them)
@@ -122,16 +130,16 @@
 
 class Preprocessor:
     def __init__(self):
         self.keys = {"userid"}
         self.form_df = None
 
     @curry
-    def add_form_data(self, form_df, df):
-        new_form_df = flatten_dict("metadata", form_df)
+    def add_form_data(self, form_df, df, prefix=None):
+        new_form_df = flatten_dict("metadata", form_df, prefix)
         self.form_df = new_form_df
         self.keys = self.keys | set(new_form_df.columns)
         return df.merge(new_form_df, on="surveyid")
 
     @curry
     def remove_form_data(self, df):
         if self.form_df is None:
@@ -147,15 +155,14 @@
         for key in keys:
             df[key] = df.metadata.map(lambda x: json.loads(x).get(key))
             self.keys.add(key)
         return df
 
     @curry
     def parse_timestamp(self, df):
-
         # NOTE: If ISO has TZ info, then it will be TZ aware, otherwise
         # it will be TZ naive.
         return df.assign(timestamp=df.timestamp.map(lambda x: pd.Timestamp(x)))
 
     @curry
     def add_duration(self, df):
         if not pd.api.types.is_datetime64_dtype(df.timestamp):
@@ -262,15 +269,15 @@
                 "Pivoting without survey information. "
                 "Make sure question_refs are unique across surveys "
                 "as all surveys will be collapsed"
             )
 
         try:
             return (
-                df.pivot(keys, "question_ref", answer_column)
+                df.pivot(index=keys, columns="question_ref", values=answer_column)
                 .reset_index()
                 .sort_values(["userid"])
             )
         except ValueError as e:
             raise PreprocessingError(
                 "Could not pivot. Potentially you should use add_form_data "
                 "to add surveyid and ensure that each user/survey is a unique line "
```

