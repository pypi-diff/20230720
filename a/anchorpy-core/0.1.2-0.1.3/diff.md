# Comparing `tmp/anchorpy_core-0.1.2.tar.gz` & `tmp/anchorpy_core-0.1.3.tar.gz`

## Comparing `anchorpy_core-0.1.2.tar` & `anchorpy_core-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 anchorpy_core-0.1.2/Cargo.toml
--rw-r--r--   0     1001      121    11357 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/LICENSE
--rw-r--r--   0     1001      121       53 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/README.md
--rw-r--r--   0     1001      121     1232 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/pyproject.toml
--rw-r--r--   0     1001      121    32464 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/src/idl.rs
--rw-r--r--   0     1001      121      654 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/src/lib.rs
--rw-r--r--   0     1001      121    45747 2022-10-31 21:28:21.000000 anchorpy_core-0.1.2/Cargo.lock
--rw-r--r--   0     1001      121    16170 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/python/anchorpy_core/idl.pyi
--rw-r--r--   0     1001      121        0 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/python/anchorpy_core/py.typed
--rw-r--r--   0     1001      121      162 2022-10-31 21:27:01.000000 anchorpy_core-0.1.2/python/anchorpy_core/__init__.py
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 anchorpy_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 anchorpy_core-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/LICENSE
+-rw-r--r--   0     1001      123       53 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/README.md
+-rw-r--r--   0     1001      123     1232 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      123    32886 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/src/idl.rs
+-rw-r--r--   0     1001      123      654 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123    54031 2023-07-20 09:35:40.000000 anchorpy_core-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      123        0 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/python/anchorpy_core/py.typed
+-rw-r--r--   0     1001      123    16322 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/python/anchorpy_core/idl.pyi
+-rw-r--r--   0     1001      123      162 2023-07-20 09:35:28.000000 anchorpy_core-0.1.3/python/anchorpy_core/__init__.py
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 anchorpy_core-0.1.3/PKG-INFO
```

### Comparing `anchorpy_core-0.1.2/Cargo.toml` & `anchorpy_core-0.1.3/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "anchorpy_core"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 include = ["/src", "/LICENSE", "/pyproject.toml"]
 description = "Python bindings for Anchor Rust code"
 license = "Apache-2.0"
 repository = "https://github.com/kevinheavey/anchorpy-core"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
@@ -12,12 +12,12 @@
 name = "anchorpy_core"
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
 pyo3 = { version = "0.17.2", features = ["extension-module", "abi3-py37"] }
 solders-macros = "0.6.0"
 derive_more = "0.99.17"
-anchor-syn = { git = "https://github.com/coral-xyz/anchor", features = ["idl"], rev = "fa12498" }
+anchor-syn = { git = "https://github.com/coral-xyz/anchor", features = ["idl"], rev = "347c225" }
 serde = { version = "1.0.147", features = ["derive"] }
 solders-traits = "0.9.3"
 serde_json = "1.0.87"
 pythonize = "0.17.0"
```

### Comparing `anchorpy_core-0.1.2/LICENSE` & `anchorpy_core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anchorpy_core-0.1.2/pyproject.toml` & `anchorpy_core-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anchorpy-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python bindings for Anchor Rust code"
 authors = ["Kevin Heavey <kevinheavey123@gmail.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["maturin>=0.13.6,<0.14"]
 build-backend = "maturin"
 
 [project]
 name = "anchorpy-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python bindings for Anchor Rust code"
 authors = [ {name = "kevinheavey", email = "kevinheavey123@gmail.com"} ]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `anchorpy_core-0.1.2/src/idl.rs` & `anchorpy_core-0.1.3/src/idl.rs`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     I32,
     F32,
     U64,
     I64,
     F64,
     U128,
     I128,
+    U256,
+    I256,
     Bytes,
     String,
     PublicKey,
 }
 
 impl From<IdlTypeSimple> for anchor_idl::IdlType {
     fn from(t: IdlTypeSimple) -> Self {
@@ -86,14 +88,16 @@
             IdlTypeSimple::I32 => Self::I32,
             IdlTypeSimple::F32 => Self::F32,
             IdlTypeSimple::U64 => Self::U64,
             IdlTypeSimple::I64 => Self::I64,
             IdlTypeSimple::F64 => Self::F64,
             IdlTypeSimple::U128 => Self::U128,
             IdlTypeSimple::I128 => Self::I128,
+            IdlTypeSimple::U256 => Self::U256,
+            IdlTypeSimple::I256 => Self::I256,
             IdlTypeSimple::Bytes => Self::Bytes,
             IdlTypeSimple::String => Self::String,
             IdlTypeSimple::PublicKey => Self::PublicKey,
         }
     }
 }
 
@@ -247,14 +251,16 @@
             anchor_idl::IdlType::I32 => Self::Simple(IdlTypeSimple::I32),
             anchor_idl::IdlType::F32 => Self::Simple(IdlTypeSimple::F32),
             anchor_idl::IdlType::U64 => Self::Simple(IdlTypeSimple::U64),
             anchor_idl::IdlType::I64 => Self::Simple(IdlTypeSimple::I64),
             anchor_idl::IdlType::F64 => Self::Simple(IdlTypeSimple::F64),
             anchor_idl::IdlType::U128 => Self::Simple(IdlTypeSimple::U128),
             anchor_idl::IdlType::I128 => Self::Simple(IdlTypeSimple::I128),
+            anchor_idl::IdlType::U256 => Self::Simple(IdlTypeSimple::U256),
+            anchor_idl::IdlType::I256 => Self::Simple(IdlTypeSimple::I256),
             anchor_idl::IdlType::Bytes => Self::Simple(IdlTypeSimple::Bytes),
             anchor_idl::IdlType::String => Self::Simple(IdlTypeSimple::String),
             anchor_idl::IdlType::PublicKey => Self::Simple(IdlTypeSimple::PublicKey),
             anchor_idl::IdlType::Defined(d) => {
                 Self::Compound(IdlTypeCompound::Defined(IdlTypeDefined(d)))
             }
             anchor_idl::IdlType::Option(o) => Self::Compound(IdlTypeCompound::Option(
@@ -828,22 +834,24 @@
 #[pymethods]
 impl IdlAccount {
     #[new]
     pub fn new(
         name: String,
         is_mut: bool,
         is_signer: bool,
+        is_optional: Option<bool>,
         docs: Option<Vec<String>>,
         pda: Option<IdlPda>,
         relations: Vec<String>,
     ) -> Self {
         anchor_idl::IdlAccount {
             name,
             is_mut,
             is_signer,
+            is_optional,
             docs,
             pda: pda.map(|x| x.into()),
             relations,
         }
         .into()
     }
 
@@ -859,14 +867,19 @@
 
     #[getter]
     pub fn is_signer(&self) -> bool {
         self.0.is_signer
     }
 
     #[getter]
+    pub fn is_optional(&self) -> Option<bool> {
+        self.0.is_optional
+    }
+
+    #[getter]
     pub fn docs(&self) -> Option<Vec<String>> {
         self.0.docs.clone()
     }
 
     #[getter]
     pub fn pda(&self) -> Option<IdlPda> {
         self.0.pda.clone().map(|x| x.into())
```

### Comparing `anchorpy_core-0.1.2/src/lib.rs` & `anchorpy_core-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `anchorpy_core-0.1.2/Cargo.lock` & `anchorpy_core-0.1.3/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,94 +1,224 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "ahash"
-version = "0.7.6"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
- "getrandom 0.2.8",
+ "cfg-if",
+ "getrandom 0.2.10",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.19"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4f55bd91a0978cbfd91c457a164bab8b4001c833b7f323132c0a4e1922dd44e"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anchor-syn"
-version = "0.25.0"
-source = "git+https://github.com/coral-xyz/anchor?rev=fa12498#fa1249836e2b8a73d3cb9fb525634e789290f251"
+version = "0.26.0"
+source = "git+https://github.com/coral-xyz/anchor?rev=347c225#347c225a27a4c615479f3c0de372604b314cbd4f"
 dependencies = [
  "anyhow",
  "bs58 0.3.1",
  "heck",
  "proc-macro2",
  "proc-macro2-diagnostics",
  "quote",
  "serde",
  "serde_json",
  "sha2 0.9.9",
- "syn",
+ "syn 1.0.109",
  "thiserror",
 ]
 
 [[package]]
 name = "anchorpy_core"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anchor-syn",
  "derive_more",
  "pyo3",
  "pythonize",
  "serde",
  "serde_json",
  "solders-macros",
  "solders-traits",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "anyhow"
-version = "1.0.66"
+version = "1.0.72"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
+
+[[package]]
+name = "ark-bn254"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a22f4561524cd949590d78d7d4c5df8f592430d221f7f3c9497bbafd8972120f"
+dependencies = [
+ "ark-ec",
+ "ark-ff",
+ "ark-std",
+]
+
+[[package]]
+name = "ark-ec"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "defd9a439d56ac24968cca0571f598a61bc8c55f71d50a89cda591cb750670ba"
+dependencies = [
+ "ark-ff",
+ "ark-poly",
+ "ark-serialize",
+ "ark-std",
+ "derivative",
+ "hashbrown 0.13.2",
+ "itertools",
+ "num-traits",
+ "zeroize",
+]
+
+[[package]]
+name = "ark-ff"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec847af850f44ad29048935519032c33da8aa03340876d351dfab5660d2966ba"
+dependencies = [
+ "ark-ff-asm",
+ "ark-ff-macros",
+ "ark-serialize",
+ "ark-std",
+ "derivative",
+ "digest 0.10.7",
+ "itertools",
+ "num-bigint",
+ "num-traits",
+ "paste",
+ "rustc_version",
+ "zeroize",
+]
+
+[[package]]
+name = "ark-ff-asm"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3ed4aa4fe255d0bc6d79373f7e31d2ea147bcf486cba1be5ba7ea85abdb92348"
+dependencies = [
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "ark-ff-macros"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7abe79b0e4288889c4574159ab790824d0033b9fdcb2a112a3182fac2e514565"
+dependencies = [
+ "num-bigint",
+ "num-traits",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "ark-poly"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d320bfc44ee185d899ccbadfa8bc31aab923ce1558716e1997a1e74057fe86bf"
+dependencies = [
+ "ark-ff",
+ "ark-serialize",
+ "ark-std",
+ "derivative",
+ "hashbrown 0.13.2",
+]
+
+[[package]]
+name = "ark-serialize"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adb7b85a02b83d2f22f89bd5cac66c9c89474240cb6207cb1efc16d098e822a5"
+dependencies = [
+ "ark-serialize-derive",
+ "ark-std",
+ "digest 0.10.7",
+ "num-bigint",
+]
+
+[[package]]
+name = "ark-serialize-derive"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae3281bc6d0fd7e549af32b52511e1302185bd688fd3359fa36423346ff682ea"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "ark-std"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94893f1e0c6eeab764ade8dc4c0db24caf4fe7cbbaafc0eba0a9030f447b5185"
+dependencies = [
+ "num-traits",
+ "rand 0.8.5",
+]
+
+[[package]]
+name = "array-bytes"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "216261ddc8289130e551ddcd5ce8a064710c0d064a4d2895c67151c92b5443f6"
+checksum = "9ad284aeb45c13f2fb4f084de4a420ebf447423bdf9386c0540ce33cb3ef4b8c"
 
 [[package]]
 name = "arrayref"
-version = "0.3.6"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4c527152e37cf757a3f78aae5a06fbeefdb07ccc535c980a3208ee3060dd544"
+checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "assert_matches"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b34d609dfbaf33d6889b2b7106d3ca345eacad44200913df5ba02bfd31d2ba9"
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
- "hermit-abi",
+ "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
@@ -99,17 +229,17 @@
 name = "base64"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3441f0f7b02788e948e47f457ca01f1d7e6d92c693bc132c22b087d3141c03ff"
 
 [[package]]
 name = "base64"
-version = "0.13.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
@@ -129,94 +259,87 @@
 checksum = "031043d04099746d8db04daf1fa424b2bc8bd69d92b25962dcde24da39ab64a2"
 dependencies = [
  "typenum",
 ]
 
 [[package]]
 name = "blake3"
-version = "1.3.1"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a08e53fc5a564bb15bfe6fae56bd71522205f1f91893f9c0116edad6496c183f"
+checksum = "199c42ab6972d92c9f8995f086273d25c42fc0f7b2a1fcefba465c1352d25ba5"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if",
  "constant_time_eq",
- "digest 0.10.5",
+ "digest 0.10.7",
 ]
 
 [[package]]
 name = "block-buffer"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
 dependencies = [
- "block-padding",
  "generic-array",
 ]
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
-name = "block-padding"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d696c370c750c948ada61c69a0ee2cbbb9c50b1019ddb86d9317157a99c2cae"
-
-[[package]]
 name = "borsh"
-version = "0.9.3"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15bf3650200d8bffa99015595e10f1fbd17de07abbc25bb067da79e769939bfa"
+checksum = "4114279215a005bc675e386011e594e1d9b800918cea18fcadadcce864a2046b"
 dependencies = [
  "borsh-derive",
- "hashbrown 0.11.2",
+ "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "borsh-derive"
-version = "0.9.3"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6441c552f230375d18e3cc377677914d2ca2b0d36e52129fe15450a2dce46775"
+checksum = "0754613691538d51f329cce9af41d7b7ca150bc973056f1156611489475f54f7"
 dependencies = [
  "borsh-derive-internal",
  "borsh-schema-derive-internal",
- "proc-macro-crate",
+ "proc-macro-crate 0.1.5",
  "proc-macro2",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "borsh-derive-internal"
-version = "0.9.3"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5449c28a7b352f2d1e592a8a28bf139bc71afb0764a14f3c02500935d8c44065"
+checksum = "afb438156919598d2c7bad7e1c0adf3d26ed3840dbc010db1a882a65583ca2fb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "borsh-schema-derive-internal"
-version = "0.9.3"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdbd5696d8bfa21d53d9fe39a714a18538bad11492a42d066dbbc395fb1951c0"
+checksum = "634205cc43f74a1b9046ef87c4540ebda95696ec0f315024860cad7c5b0f5ccd"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "bs58"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "476e9cd489f9e121e02ffa6014a8ef220ecb15c05ed23fc34cca13925dc283fb"
@@ -225,76 +348,76 @@
 name = "bs58"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "771fe0050b883fcc3ea2359b1a96bcfbc090b7116eae7c3c512c7a083fdf23d3"
 
 [[package]]
 name = "bumpalo"
-version = "3.11.1"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bv"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8834bb1d8ee5dc048ee3124f2c7c1afcc6bc9aed03f11e9dfd8c69470a5db340"
 dependencies = [
  "feature-probe",
  "serde",
 ]
 
 [[package]]
 name = "bytemuck"
-version = "1.12.2"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aec14f5d4e6e3f927cd0c81f72e5710d95ee9019fbeb4b3021193867491bfd8"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.2.1"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9e1f5fa78f69496407a27ae9ed989e3c3b072310286f5ef385525e4cbc24a9"
+checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "cc"
-version = "1.0.74"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "581f5dba903aac52ea3feb5ec4810848460ee833876f1f9b0fdeab1f19091574"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 dependencies = [
  "jobserver",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.22"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfd4d1b31faaa3a89d7934dbded3111da0d2ef28e3ebccdb4f0179f5929d1ef1"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
- "num-integer",
+ "android-tzdata",
  "num-traits",
 ]
 
 [[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -302,82 +425,82 @@
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "console_log"
-version = "0.2.0"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "501a375961cef1a0d44767200e66e4a559283097e91d0730b1d75dfb2f8a1494"
+checksum = "e89f72f65e8501878b8a004d5a1afb780987e2ce2b4532c562e367a72c57499f"
 dependencies = [
  "log",
  "web-sys",
 ]
 
 [[package]]
 name = "constant_time_eq"
-version = "0.1.5"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
+checksum = "f7144d30dcf0fafbce74250a3963025d8d52177934239851c917d29f1df280c2"
 
 [[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.11"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f916dfc5d356b0ed9dae65f1db9fc9770aa2851d2662b988ccf4fe3516e86348"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.12"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edbafec5fa1f196ca66527c1b12c2ec4745ca14b50f1ad8f9f6f720b55d11fac"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
@@ -415,123 +538,175 @@
  "rand_core 0.5.1",
  "serde",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
+name = "darling"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0209d94da627ab5605dcccf08bb18afa5009cfbef48d8a8b7d7bdbc79be25c5e"
+dependencies = [
+ "darling_core",
+ "darling_macro",
+]
+
+[[package]]
+name = "darling_core"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "177e3443818124b357d8e76f53be906d60937f0d3a90773a664fa63fa253e621"
+dependencies = [
+ "fnv",
+ "ident_case",
+ "proc-macro2",
+ "quote",
+ "strsim",
+ "syn 2.0.26",
+]
+
+[[package]]
+name = "darling_macro"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "836a9bbc7ad63342d6d6e7b815ccab164bc77a2d95d84bc3117a8c0d5c98e2d5"
+dependencies = [
+ "darling_core",
+ "quote",
+ "syn 2.0.26",
+]
+
+[[package]]
 name = "derivation-path"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e5c37193a1db1d8ed868c03ec7b152175f26160a5b740e5e484143877e0adf0"
 
 [[package]]
+name = "derivative"
+version = "2.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "convert_case",
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "digest"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.5"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adfbc57365a37acbd2ebf2b64d7e69bb766e2fea813521ed536f5d0520dcf86c"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
- "block-buffer 0.10.3",
+ "block-buffer 0.10.4",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "ed25519"
-version = "1.5.2"
+version = "1.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e9c280362032ea4203659fc489832d0204ef09f247a0506f170dafcac08c369"
+checksum = "91cff35c70bba8a626e3185d8cd48cc11b5437e1a5bcd15b9b5fa3c64b6dfee7"
 dependencies = [
  "signature",
 ]
 
 [[package]]
 name = "ed25519-dalek"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c762bae6dcaf24c4c84667b8579785430908723d5c889f469d76a41d59cc7a9d"
 dependencies = [
  "curve25519-dalek",
  "ed25519",
- "rand",
+ "rand 0.7.3",
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ed25519-dalek-bip32"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d2be62a4061b872c8c0873ee4fc6f101ce7b889d039f019c5fa2af471a59908"
 dependencies = [
  "derivation-path",
  "ed25519-dalek",
  "hmac 0.12.1",
- "sha2 0.10.6",
+ "sha2 0.10.7",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "env_logger"
-version = "0.9.1"
+version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c90bf5f19754d10198ccb95b70664fc925bd1fc090a0fd9a6ebc54acc8cd6272"
+checksum = "a12e6657c4c97ebab115a42dcee77225f7f482cdd841cf7088c657a42e9e00e7"
 dependencies = [
  "atty",
  "humantime",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "feature-probe"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "835a3dc7d1ec9e75e2b5fb4ba75396837112d2060b03f7d43bc1897c7f7211da"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "serde",
  "typenum",
  "version_check",
 ]
 
 [[package]]
@@ -545,17 +720,17 @@
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
@@ -564,29 +739,26 @@
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
 name = "hashbrown"
-version = "0.11.2"
+version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab5ef0d4909ef3724cc8cce6ccc8572c5c817592e9285f5464f8e86f8bd3726e"
+checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
  "ahash",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
-dependencies = [
- "ahash",
-]
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
 
 [[package]]
 name = "heck"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
 dependencies = [
@@ -599,14 +771,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+
+[[package]]
 name = "hmac"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "126888268dcc288495a26bf004b38c5fdbb31682f992c84ceb046a1f0fe38840"
 dependencies = [
  "crypto-mac",
  "digest 0.9.0",
@@ -614,15 +792,15 @@
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
- "digest 0.10.5",
+ "digest 0.10.7",
 ]
 
 [[package]]
 name = "hmac-drbg"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17ea0a1394df5b6574da6e0c1ade9e78868c9fb0a4e5ef4428e32da4676b85b1"
@@ -635,14 +813,20 @@
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
+name = "ident_case"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+
+[[package]]
 name = "im"
 version = "15.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0acd33ff0285af998aaf9b57342af478078f53492322fafc47450e09397e0e9"
 dependencies = [
  "bitmaps",
  "rand_core 0.6.4",
@@ -651,84 +835,97 @@
  "serde",
  "sized-chunks",
  "typenum",
  "version_check",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.0",
+]
+
+[[package]]
 name = "indoc"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.4"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4217ad341ebadf8d8e724e264f13e593e0648f5b3e94b3896a5df283be015ecc"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jobserver"
-version = "0.1.25"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "068b1ee6743e4d11fb9c6a1e6064b3693a1b600e7f5f5988047d98b3dc9fb90b"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "keccak"
-version = "0.1.2"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9b7d56ba4a8344d6be9729995e6b06f928af29998cdf79fe390cbf6b1fee838"
+checksum = "8f6d5ed8676d904364de097082f4e7d240b571b67989ced0240f08b7f966f940"
+dependencies = [
+ "cpufeatures",
+]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.137"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc7fcc620a3bff7cdd7a365be3376c97191aeaccc2a603e600951e452615bf89"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libsecp256k1"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c9d220bc1feda2ac231cb78c3d26f27676b8cf82c96971f7aeef3d0cf2797c73"
 dependencies = [
  "arrayref",
  "base64 0.12.3",
  "digest 0.9.0",
  "hmac-drbg",
  "libsecp256k1-core",
  "libsecp256k1-gen-ecmult",
  "libsecp256k1-gen-genmult",
- "rand",
+ "rand 0.7.3",
  "serde",
  "sha2 0.9.9",
  "typenum",
 ]
 
 [[package]]
 name = "libsecp256k1-core"
@@ -757,64 +954,81 @@
 checksum = "67abfe149395e3aa1c48a2beb32b068e2334402df8181f818d3aee2b304c4f5d"
 dependencies = [
  "libsecp256k1-core",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
-version = "0.5.7"
+version = "0.5.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95af15f345b17af2efc8ead6080fb8bc376f8cec1b35277b935637595fe77498"
+checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "num-bigint"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-derive"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
@@ -830,27 +1044,48 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.13.1"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19e64526ebdee182341572e50e9ad03965aa510cd94427a4549448f285e957a1"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi",
+ "hermit-abi 0.3.2",
  "libc",
 ]
 
 [[package]]
+name = "num_enum"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a015b430d3c108a207fd776d2e2196aaf8b1cf8cf93253e3a097ff3085076a1"
+dependencies = [
+ "num_enum_derive",
+]
+
+[[package]]
+name = "num_enum_derive"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96667db765a921f7b295ffee8b60472b686a51d4f21c2ee4ffdb94c7013b65a6"
+dependencies = [
+ "proc-macro-crate 1.3.1",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.26",
+]
+
+[[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
@@ -862,144 +1097,160 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.4"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dc9e0dc2adc1c69d09143aff38d3d30c5c3f0df0dad82e6d25547af174ebec0"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
+name = "paste"
+version = "1.0.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+
+[[package]]
 name = "pbkdf2"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "216eaa586a190f0a738f2f918511eecfa90f13295abec0e457cdebcceda80cbd"
 dependencies = [
  "crypto-mac",
 ]
 
 [[package]]
 name = "pbkdf2"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
 dependencies = [
- "digest 0.10.5",
+ "digest 0.10.7",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "ppv-lite86"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb9f9e6e233e5c4a35559a617bf40a4ec447db2e84c20b55a6f83167b7e57872"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro-crate"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d6ea3c4595b96363c13943497db34af4460fb474a95c43f4446ad341b8c9785"
 dependencies = [
  "toml",
 ]
 
 [[package]]
+name = "proc-macro-crate"
+version = "1.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
+dependencies = [
+ "once_cell",
+ "toml_edit",
+]
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proc-macro2-diagnostics"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bf29726d67464d49fa6224a1d07936a8c08bb3fba727c7493f6cf1616fdaada"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
  "yansi",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201b6887e5576bf2f945fe65172c1fcbf3fcf285b23e4d71eb171d9736e38d32"
+checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.6.5",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf0708c9ed01692635cbf056e286008e5a2927ab1a5e48cdd3aeb1ba5a6fef47"
+checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90352dea4f486932b72ddf776264d293f85b79a1d214de1d023927b41461132d"
+checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb24b804a2d9e88bfcc480a5a6dd76f006c1e3edaf064e8250423336e2cd79d"
+checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f22bb49f6a7348c253d7ac67a6875f2dc65f36c2ae64a82c381d528972bea6d6"
+checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pythonize"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f7f0c136f5fbc01868185eef462800e49659eb23acca83b9e884367a006acb6"
@@ -1015,60 +1266,80 @@
 checksum = "d464fae65fff2680baf48019211ce37aaec0c78e9264c84a3e484717f965104e"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a6b1679d49b24bbfe0c803429aa1874472f50d9b363131f0e89fc356b544d03"
 dependencies = [
  "getrandom 0.1.16",
  "libc",
- "rand_chacha",
+ "rand_chacha 0.2.2",
  "rand_core 0.5.1",
  "rand_hc",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "rand_chacha 0.3.1",
+ "rand_core 0.6.4",
+]
+
+[[package]]
 name = "rand_chacha"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4c8ed856279c9737206bf725bf36935d8666ead7aa69b52be55af369d193402"
 dependencies = [
  "ppv-lite86",
  "rand_core 0.5.1",
 ]
 
 [[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core 0.6.4",
+]
+
+[[package]]
 name = "rand_core"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90bde5296fc891b0cef12a6d03ddccc162ce7b2aff54160af9338f8d40df6d19"
 dependencies = [
  "getrandom 0.1.16",
 ]
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -1083,61 +1354,71 @@
 checksum = "6f97cdb2a36ed4183de61b2f824cc45c9f1037f28afe0a322e9fff4c108b5aaa"
 dependencies = [
  "rand_core 0.6.4",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.5.3"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd99e5772ead8baa5215278c9b15bf92087709e9c1b2d1f97cdb5a183c933a7d"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
- "autocfg",
- "crossbeam-deque",
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.9.3"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "258bcdb5ac6dad48491bb2992db6b7cf74878b0384908af124823d118c99683f"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.6.0"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c4eb3267174b8c6c2f654116623910a0fef09c4753f8dd83db29c48a0df988b"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.27"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3f87b73ce11b1619a3c6332f45341e0047173771e8b8b73f87bfeefb7b56244"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -1148,50 +1429,50 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.9"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97477e48b4cf8603ad5f7aaf897467cf42ab4218a38ef76fb14c2d6773a6d6a8"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.11"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.14"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e25dfac463d778e353db5be2449d1cce89bd6fd23c9f1ea21310ce6e5a1b29c4"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.147"
+version = "1.0.173"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d193d69bae983fc11a79df82342761dfbf28a99fc8d203dca4c3c1b590948965"
+checksum = "e91f70896d6720bc714a4a57d22fc91f1db634680e65c8efe13323f1fa38d53f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.7"
+version = "0.11.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfc50e8183eeeb6178dcb167ae34a8051d63535023ae38b5d8d12beae193d37b"
+checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
@@ -1200,65 +1481,87 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.147"
+version = "1.0.173"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f1d362ca8fc9c3e3a7484440752472d68a6caa98f1ab81d99b5dfe517cec852"
+checksum = "a6250dde8342e0232232be9ca3db7aa40aceb5a3e5dd9bddbc00d99a007cde49"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.87"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ce777b7b150d76b9cf60d28b55f5847135a003f7d7350c6be7a773508ce7d45"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_with"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07ff71d2c147a7b57362cead5e22f772cd52f6ab31cfcd9edcd7f6aeb2a0afbe"
+dependencies = [
+ "serde",
+ "serde_with_macros",
+]
+
+[[package]]
+name = "serde_with_macros"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "881b6f881b17d13214e5d494c939ebab463d01264ce1811e9d4ac3a882e7695f"
+dependencies = [
+ "darling",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.26",
+]
+
+[[package]]
 name = "sha2"
 version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4d58a1e1bf39749807d89cf2d98ac2dfa0ff1cb3faa38fbb64dd88ac8013d800"
 dependencies = [
  "block-buffer 0.9.0",
  "cfg-if",
  "cpufeatures",
  "digest 0.9.0",
  "opaque-debug",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
- "digest 0.10.5",
+ "digest 0.10.7",
 ]
 
 [[package]]
 name = "sha3"
-version = "0.10.6"
+version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf0c33fae925bdc080598b84bc15c55e7b9a4a43b3c704da051f977469691c9"
+checksum = "75872d278a8f37ef87fa0ddbda7802605cb18344497949862c0d4dcb291eba60"
 dependencies = [
- "digest 0.10.5",
+ "digest 0.10.7",
  "keccak",
 ]
 
 [[package]]
 name = "signature"
 version = "1.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1272,197 +1575,203 @@
 dependencies = [
  "bitmaps",
  "typenum",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "solana-frozen-abi"
-version = "1.14.6"
+version = "1.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fae9453c906a52b00c6d668508214377163cf59776cfa8e09ef740a2a493f87d"
+checksum = "6984c05f3ec91051452778f5da35dd27783e4e4093be6dcfbe918e15377daf25"
 dependencies = [
  "ahash",
  "blake3",
- "block-buffer 0.9.0",
+ "block-buffer 0.10.4",
  "bs58 0.4.0",
  "bv",
  "byteorder",
  "cc",
  "either",
  "generic-array",
  "getrandom 0.1.16",
- "hashbrown 0.12.3",
  "im",
  "lazy_static",
  "log",
  "memmap2",
  "once_cell",
  "rand_core 0.6.4",
  "rustc_version",
  "serde",
  "serde_bytes",
  "serde_derive",
  "serde_json",
- "sha2 0.10.6",
+ "sha2 0.10.7",
  "solana-frozen-abi-macro",
  "subtle",
  "thiserror",
 ]
 
 [[package]]
 name = "solana-frozen-abi-macro"
-version = "1.14.6"
+version = "1.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e29cd0fef92aee046267cdd69d8aa8b31cd3549991ea6f2c6076b21064e235fb"
+checksum = "485108737b486ceb823ddb0ea43915f440ae15f02e2725bf1c0c93f125b69adf"
 dependencies = [
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "solana-logger"
-version = "1.14.6"
+version = "1.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d255b73f0c0e1eaa34280094f1304a783ea9394dbf2f8b749a3661e948ca5551"
+checksum = "7e5751fb3da76857f9e9c6fa032ef9f537df3c392ce536055960b5550f234de0"
 dependencies = [
  "env_logger",
  "lazy_static",
  "log",
 ]
 
 [[package]]
 name = "solana-program"
-version = "1.14.6"
+version = "1.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0eeda17e271e11864d48b35eeaefed9591305b4d47266caf3f8b11b9271833d"
+checksum = "385ebd372e798ea8cf511bec5431f02786cf9c802a7a3954ad0bd57b0b31b256"
 dependencies = [
- "base64 0.13.1",
+ "ark-bn254",
+ "ark-ec",
+ "ark-ff",
+ "ark-serialize",
+ "array-bytes",
+ "base64 0.21.2",
  "bincode",
  "bitflags",
  "blake3",
  "borsh",
- "borsh-derive",
  "bs58 0.4.0",
  "bv",
  "bytemuck",
  "cc",
  "console_error_panic_hook",
  "console_log",
  "curve25519-dalek",
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
  "itertools",
  "js-sys",
  "lazy_static",
  "libc",
  "libsecp256k1",
  "log",
- "memoffset",
+ "memoffset 0.9.0",
+ "num-bigint",
  "num-derive",
  "num-traits",
  "parking_lot",
- "rand",
- "rand_chacha",
+ "rand 0.7.3",
+ "rand_chacha 0.2.2",
  "rustc_version",
  "rustversion",
  "serde",
  "serde_bytes",
  "serde_derive",
  "serde_json",
- "sha2 0.10.6",
+ "sha2 0.10.7",
  "sha3",
  "solana-frozen-abi",
  "solana-frozen-abi-macro",
  "solana-sdk-macro",
  "thiserror",
  "tiny-bip39",
  "wasm-bindgen",
  "zeroize",
 ]
 
 [[package]]
 name = "solana-sdk"
-version = "1.14.6"
+version = "1.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57fe62f7fe938607437ed29b0e95b4cffc7db186bf04fea6a98d92319da941b1"
+checksum = "40fd37e7922b26b19632b2bceba0a749d36a7013f991771e65607e6a17cd6000"
 dependencies = [
  "assert_matches",
- "base64 0.13.1",
+ "base64 0.21.2",
  "bincode",
  "bitflags",
  "borsh",
  "bs58 0.4.0",
  "bytemuck",
  "byteorder",
  "chrono",
  "derivation-path",
- "digest 0.10.5",
+ "digest 0.10.7",
  "ed25519-dalek",
  "ed25519-dalek-bip32",
  "generic-array",
  "hmac 0.12.1",
  "itertools",
  "js-sys",
  "lazy_static",
  "libsecp256k1",
  "log",
  "memmap2",
  "num-derive",
  "num-traits",
+ "num_enum",
  "pbkdf2 0.11.0",
  "qstring",
- "rand",
- "rand_chacha",
+ "rand 0.7.3",
+ "rand_chacha 0.2.2",
  "rustc_version",
  "rustversion",
  "serde",
  "serde_bytes",
  "serde_derive",
  "serde_json",
- "sha2 0.10.6",
+ "serde_with",
+ "sha2 0.10.7",
  "sha3",
  "solana-frozen-abi",
  "solana-frozen-abi-macro",
  "solana-logger",
  "solana-program",
  "solana-sdk-macro",
  "thiserror",
  "uriparse",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "solana-sdk-macro"
-version = "1.14.6"
+version = "1.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12f9abf0bdba679d93c5624043ae3dcbf529ed2251c281cc615fa55c8dc2f0bd"
+checksum = "bc6b3dda3769d0ab471ba94bcea1b8df6e40ad6644314990671b95a624dc98d3"
 dependencies = [
  "bs58 0.4.0",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "solders-macros"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f47af25c5b7e16614840f1d99b400397d609e991d90b925a63ab245e1eece0a5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "solders-traits"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ffae044878b2160f61cf9c8c537ae04cae12b4155f6c499133054a8492f54504"
@@ -1473,88 +1782,93 @@
  "serde",
  "serde_cbor",
  "serde_json",
  "solana-sdk",
 ]
 
 [[package]]
+name = "strsim"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+
+[[package]]
 name = "subtle"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "1.0.103"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a864042229133ada95abf3b54fdc62ef5ccabe9515b64717bcb9a1919e59445d"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "synstructure"
-version = "0.12.6"
+name = "syn"
+version = "2.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
- "unicode-xid",
+ "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.4"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.37"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10deb33631e3c9018b9baf9dcbbc4f737320d2b576bac10f6aefa048fa407e3e"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.37"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "982d17546b47146b28f7c22e3d08465f6b8903d0ea13c1660d9d84a6e7adcdbb"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "tiny-bip39"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ffc59cb9dfc85bb312c3a78fd6aa8a8582e310b0fa885d5bb877f6dcc601839d"
 dependencies = [
  "anyhow",
  "hmac 0.8.1",
  "once_cell",
  "pbkdf2 0.4.0",
- "rand",
+ "rand 0.7.3",
  "rustc-hash",
  "sha2 0.9.9",
  "thiserror",
  "unicode-normalization",
  "wasm-bindgen",
  "zeroize",
 ]
@@ -1566,65 +1880,76 @@
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml"
-version = "0.5.9"
+version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d82e1a7758622a465f8cee077614c73484dac5b836c02ff6a40d5d1010324d7"
+checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "toml_datetime"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
+
+[[package]]
+name = "toml_edit"
+version = "0.19.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8123f27e969974a3dfba720fdb560be359f57b44302d280ba72e76a74480e8a"
+dependencies = [
+ "indexmap",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
 name = "typenum"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.0"
+version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fdbf052a0783de01e944a6ce7a8cb939e295b1e7be835a1112c3b9a7f047a5a"
-
-[[package]]
-name = "unicode-xid"
-version = "0.2.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
+checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
 name = "unindent"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "uriparse"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0200d0fc04d809396c2ad43f3c95da3582a2556eba8d453c1087f4120ee352ff"
 dependencies = [
@@ -1648,71 +1973,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.26",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.26",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -1742,69 +2067,78 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "winnow"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "81fac9742fd1ad1bd9643b991319f72dd031016d44b77039a26977eb667141e7"
+dependencies = [
+ "memchr",
+]
 
 [[package]]
 name = "yansi"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
@@ -1815,16 +2149,15 @@
 checksum = "4756f7db3f7b5574938c3eb1c117038b8e07f95ee6718c0efad4ac21508f1efd"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
-version = "1.3.2"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f8f187641dad4f680d25c4bfc4225b418165984179f26ca76ec4fb6441d3a17"
+checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
- "synstructure",
+ "syn 2.0.26",
 ]
```

### Comparing `anchorpy_core-0.1.2/python/anchorpy_core/idl.pyi` & `anchorpy_core-0.1.3/python/anchorpy_core/idl.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     I32: "IdlTypeSimple"
     F32: "IdlTypeSimple"
     U64: "IdlTypeSimple"
     I64: "IdlTypeSimple"
     F64: "IdlTypeSimple"
     U128: "IdlTypeSimple"
     I128: "IdlTypeSimple"
+    U256: "IdlTypeSimple"
+    I256: "IdlTypeSimple"
     Bytes: "IdlTypeSimple"
     String: "IdlTypeSimple"
     PublicKey: "IdlTypeSimple"
     def __int__(self) -> int: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
     def __eq__(self, o: object) -> bool: ...
@@ -305,25 +307,28 @@
 
 class IdlAccount:
     def __init__(
         self,
         name: str,
         is_mut: bool,
         is_signer: bool,
+        is_optional: Optional[bool],
         docs: Optional[Sequence[str]],
         pda: Optional[IdlPda],
         relations: Sequence[str],
     ) -> None: ...
     @property
     def name(self) -> str: ...
     @property
     def is_mut(self) -> bool: ...
     @property
     def is_signer(self) -> bool: ...
     @property
+    def is_optional(self) -> Optional[bool]: ...
+    @property
     def docs(self) -> Optional[List[str]]: ...
     @property
     def pda(self) -> Optional[IdlPda]: ...
     @property
     def relations(self) -> List[str]: ...
     def __bytes__(self) -> bytes: ...
     def __str__(self) -> str: ...
```

### Comparing `anchorpy_core-0.1.2/PKG-INFO` & `anchorpy_core-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: anchorpy-core
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: jsonalias ==0.1.1
 License-File: LICENSE
 Summary: Python bindings for Anchor Rust code
 Author-email: kevinheavey <kevinheavey123@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/kevinheavey/anchorpy-core
-Project-URL: changelog, https://github.com/kevinheavey/anchorpy-core/blob/main/CHANGELOG.md
 Project-URL: homepage, https://github.com/kevinheavey/anchorpy-core
 Project-URL: documentation, https://kevinheavey.github.io/anchorpy-core/
+Project-URL: changelog, https://github.com/kevinheavey/anchorpy-core/blob/main/CHANGELOG.md
+Project-URL: repository, https://github.com/kevinheavey/anchorpy-core
 
 # anchorpy-core
 Python bindings for Anchor Rust code
```

