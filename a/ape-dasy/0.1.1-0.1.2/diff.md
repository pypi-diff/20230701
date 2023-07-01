# Comparing `tmp/ape_dasy-0.1.1.tar.gz` & `tmp/ape_dasy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape_dasy-0.1.1.tar", max compression
+gzip compressed data, was "ape_dasy-0.1.2.tar", max compression
```

## Comparing `ape_dasy-0.1.1.tar` & `ape_dasy-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      186 2023-06-25 20:34:55.618759 ape_dasy-0.1.1/ape_dasy/__init__.py
--rw-r--r--   0        0        0     1458 2023-06-25 19:46:12.135237 ape_dasy-0.1.1/ape_dasy/compiler.py
--rw-r--r--   0        0        0      330 2023-06-25 20:34:47.788773 ape_dasy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      308 1970-01-01 00:00:00.000000 ape_dasy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-07-01 04:33:18.800895 ape_dasy-0.1.2/ape_dasy/__init__.py
+-rw-r--r--   0        0        0     1487 2023-07-01 04:31:34.947397 ape_dasy-0.1.2/ape_dasy/compiler.py
+-rw-r--r--   0        0        0      330 2023-07-01 04:33:51.541134 ape_dasy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      308 1970-01-01 00:00:00.000000 ape_dasy-0.1.2/PKG-INFO
```

### Comparing `ape_dasy-0.1.1/ape_dasy/compiler.py` & `ape_dasy-0.1.2/ape_dasy/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     def compile(self, contracts_filepaths: List[Path], base_path: Optional[Path] = None) -> List[ContractType]:
         contract_types = []
         if base_path:
             for path in contracts_filepaths:
                 with open(os.path.join(base_path, path)) as f:
                     src = f.read()
                     data = dasy.compile(src)
+                    data.abi
                     data_dict = data.__dict__
                     data_dict["contractName"] = Path(path).stem
                     data_dict["sourceId"] = str(path)
                     data_dict["deploymentBytecode"] = {"bytecode": '0x' + data.bytecode.hex()}
                     data_dict["runtimeBytecode"] = {"bytecode": '0x' + data.bytecode_runtime.hex()}
                     contract_types.append(ContractType.parse_obj(data_dict))
         return contract_types
```

