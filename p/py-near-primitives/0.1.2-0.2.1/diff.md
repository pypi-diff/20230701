# Comparing `tmp/py_near_primitives-0.1.2.tar.gz` & `tmp/py_near_primitives-0.2.1.tar.gz`

## Comparing `py_near_primitives-0.1.2.tar` & `py_near_primitives-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 py_near_primitives-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/LICENSE
--rw-r--r--   0     1001      123      579 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/README.md
--rw-r--r--   0     1001      123     1195 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/pyproject.toml
--rw-r--r--   0     1001      123    17770 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123    69227 2023-06-26 03:15:52.000000 py_near_primitives-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 py_near_primitives-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 py_near_primitives-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/LICENSE
+-rw-r--r--   0     1001      123      730 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/README.md
+-rw-r--r--   0     1001      123     1195 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123    18657 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123    69198 2023-06-30 22:15:02.000000 py_near_primitives-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 py_near_primitives-0.2.1/PKG-INFO
```

### Comparing `py_near_primitives-0.1.2/Cargo.toml` & `py_near_primitives-0.2.1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py_near_primitives"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 include = ["/src", "/LICENSE", "/pyproject.toml"]
 description = "Python bindings for NEAR Rust primitives."
 license = "MIT"
 repository = "https://github.com/kevinheavey/pyonear"
 
 [lib]
```

### Comparing `py_near_primitives-0.1.2/LICENSE` & `py_near_primitives-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_near_primitives-0.1.2/README.md` & `py_near_primitives-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 
 [![PyPI version](https://badge.fury.io/py/pyonear.svg)](https://badge.fury.io/py/pyonear)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/kevinheavey/pyonear/blob/maim/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # near primitives
 
-A wrapper over `near-primitives` rust lib for python. Using for [py-near](https://github.com/pvolnov/py-near).
+A wrapper over `py-near-primitives` rust lib for python. Using for [py-near](https://github.com/pvolnov/py-near).
 
-Latest supported version: `near-primitives = "0.17.0"`
+Latest supported version: `py-near-primitives = "0.17.0"`
+
+# use with python 
+
+Use the `py-near` for the high-level api over `py-near-primitives`
+
+Documentation: https://py-near.readthedocs.io/en/latest
 
 
 ## Installation
 
 ```
 pip install py-near-primitives
 ```
```

### Comparing `py_near_primitives-0.1.2/pyproject.toml` & `py_near_primitives-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_near_primitives"
-version = "0.1.2"
+version = "0.2.1"
 description = "Python bindings for NEAR Rust primitives."
 authors = ["pvolnov <notanemail@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
@@ -21,15 +21,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 
 [project]
 name = "py_near_primitives"
-version = "0.1.2"
+version = "0.2.1"
 description = "Python bindings for NEAR Rust primitives."
 authors = [ {name = "pvolnov", email = "notanemail@gmail.com"} ]
 license = {file = "LICENSE"} # relative to the package/ directory
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `py_near_primitives-0.1.2/src/lib.rs` & `py_near_primitives-0.2.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,17 @@
             }
         };
         dactions.push(delegate_action.try_into().unwrap());
     }
     dactions
 }
 
+
+use pyo3::types::PyBytes;
+
 #[pymethods]
 impl DelegateAction {
     #[new]
     #[pyo3(signature = (sender_id, receiver_id, actions, nonce, max_block_height, public_key))]
     pub fn new(
         sender_id: String,
         receiver_id: String,
@@ -326,14 +329,35 @@
             actions: get_delegate_actions(self.clone()),
             nonce: self.nonce,
             max_block_height: self.max_block_height,
             public_key: pk,
         };
         return *action.get_nep461_hash().as_bytes();
     }
+
+    fn serialize(&self) -> Vec<u8> {
+        let pk = PublicKey::ED25519(ED25519PublicKey(self.public_key));
+        let action = DelegateActionOriginal {
+            sender_id: AccountId::from_str(self.sender_id.as_str()).unwrap(),
+            receiver_id: AccountId::from_str(self.receiver_id.as_str()).unwrap(),
+            actions: get_delegate_actions(self.clone()),
+            nonce: self.nonce,
+            max_block_height: self.max_block_height,
+            public_key: pk,
+        };
+        return action.try_to_vec().unwrap().to_vec();
+    }
+
+
+    #[staticmethod]
+    fn bytes_to_json(mut bytes: &[u8]) -> String {
+        let bytes_mut: &mut &[u8] = &mut bytes;
+        let action: DelegateActionOriginal = near_primitives::borsh::BorshDeserialize::deserialize(bytes_mut).unwrap();
+        return serde_json::to_string(&action).unwrap();
+    }
 }
 
 #[pymethods]
 impl CreateAccountAction {
     #[new]
     fn new() -> CreateAccountAction {
         CreateAccountAction {}
```

### Comparing `py_near_primitives-0.1.2/Cargo.lock` & `py_near_primitives-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -775,30 +775,30 @@
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "enum-map"
-version = "2.5.0"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "988f0d17a0fa38291e5f41f71ea8d46a5d5497b9054d5a759fae2cbb819f2356"
+checksum = "017b207acb4cc917f4c31758ed95c0bc63ddb0f358b22eb38f80a2b2a43f6b1f"
 dependencies = [
  "enum-map-derive",
 ]
 
 [[package]]
 name = "enum-map-derive"
-version = "0.11.0"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a4da76b3b6116d758c7ba93f7ec6a35d2e2cf24feda76c6e38a375f4d5c59f2"
+checksum = "8560b409800a72d2d7860f8e5f4e0b0bd22bea6a352ea2a9ce30ccdef7f16d2f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a12e6657c4c97ebab115a42dcee77225f7f482cdd841cf7088c657a42e9e00e7"
@@ -933,20 +933,17 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 dependencies = [
@@ -1441,19 +1438,19 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi 0.3.1",
  "libc",
 ]
 
 [[package]]
 name = "num_enum"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1587,15 +1584,15 @@
 checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_near_primitives"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "borsh 0.9.3",
  "derive_more",
  "ed25519-dalek",
  "near-crypto",
  "near-primitives",
  "near-primitives-core",
@@ -1676,17 +1673,17 @@
 checksum = "d464fae65fff2680baf48019211ce37aaec0c78e9264c84a3e484717f965104e"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
@@ -2095,17 +2092,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "solana-frozen-abi"
-version = "1.16.1"
+version = "1.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eea8be57163366de9ffee3652cd42ea02fd5cca672408722f1426eb0d234a330"
+checksum = "4ba46ba8715a2860f253a754812b2df6ab049f42cbe0458c1fdc3095b3024c73"
 dependencies = [
  "ahash 0.8.3",
  "blake3",
  "block-buffer 0.10.4",
  "bs58",
  "bv",
  "byteorder",
@@ -2128,40 +2125,40 @@
  "solana-frozen-abi-macro",
  "subtle",
  "thiserror",
 ]
 
 [[package]]
 name = "solana-frozen-abi-macro"
-version = "1.16.1"
+version = "1.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4121f91307234cec8c8d8cd2d7ec171881c07db2222335e8c840d555ebe89cc"
+checksum = "477b0177d9d73dbe05b564a845c80f1fb4cce9a6349eb8dad7cb15530e27a053"
 dependencies = [
  "proc-macro2",
  "quote",
  "rustc_version",
  "syn 2.0.22",
 ]
 
 [[package]]
 name = "solana-logger"
-version = "1.16.1"
+version = "1.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f590904a129707c5bf6b9f2e198e49ce8984e802dad26babd2c406a4e898b0ce"
+checksum = "da3c2c141cfa4971ec0f591affc92e9bc40a023562a7821046daa4b2ad93d04a"
 dependencies = [
  "env_logger",
  "lazy_static",
  "log",
 ]
 
 [[package]]
 name = "solana-program"
-version = "1.16.1"
+version = "1.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19ac28d05adeff2212cdec76dfacc6eb631d69d065b1b83c063a1fab505d5e62"
+checksum = "5d5e393489bae293327e0fc0ca7e709bcc32fb01afa552b0bc75a7c2d506599c"
 dependencies = [
  "ark-bn254",
  "ark-ec",
  "ark-ff",
  "ark-serialize",
  "array-bytes",
  "base64 0.21.2",
@@ -2205,17 +2202,17 @@
  "tiny-bip39",
  "wasm-bindgen",
  "zeroize",
 ]
 
 [[package]]
 name = "solana-sdk"
-version = "1.16.1"
+version = "1.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3aa2d54c0e9109d1bf9edafbd86d645217776df783814397f79c3929cf4316ba"
+checksum = "250dbc29e6917974b1697d0e0cafb6fc8edd62f85ca843f9c99fd00c0b145e8f"
 dependencies = [
  "assert_matches",
  "base64 0.21.2",
  "bincode",
  "bitflags",
  "borsh 0.10.3",
  "bs58",
@@ -2258,17 +2255,17 @@
  "thiserror",
  "uriparse",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "solana-sdk-macro"
-version = "1.16.1"
+version = "1.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa991e6d6ae7c57ef9fc56f964b22f3bae6ba6c144ccb07b0fe07e06a3efc47c"
+checksum = "d598db5bcc4eba1442f75f3ab734f624d3026dcea1be66b5ee9a7e9fe5b38ca6"
 dependencies = [
  "bs58",
  "proc-macro2",
  "quote",
  "rustversion",
  "syn 2.0.22",
 ]
@@ -2706,17 +2703,17 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
```

### Comparing `py_near_primitives-0.1.2/PKG-INFO` & `py_near_primitives-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_near_primitives
-Version: 0.1.2
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for NEAR Rust primitives.
 Author-email: pvolnov <notanemail@gmail.com>
 License: MIT
@@ -17,17 +17,23 @@
 
 [![PyPI version](https://badge.fury.io/py/pyonear.svg)](https://badge.fury.io/py/pyonear)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/kevinheavey/pyonear/blob/maim/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # near primitives
 
-A wrapper over `near-primitives` rust lib for python. Using for [py-near](https://github.com/pvolnov/py-near).
+A wrapper over `py-near-primitives` rust lib for python. Using for [py-near](https://github.com/pvolnov/py-near).
 
-Latest supported version: `near-primitives = "0.17.0"`
+Latest supported version: `py-near-primitives = "0.17.0"`
+
+# use with python 
+
+Use the `py-near` for the high-level api over `py-near-primitives`
+
+Documentation: https://py-near.readthedocs.io/en/latest
 
 
 ## Installation
 
 ```
 pip install py-near-primitives
 ```
```

