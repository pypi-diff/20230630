# Comparing `tmp/promql_parser-0.1.2.tar.gz` & `tmp/promql_parser-0.1.3.tar.gz`

## Comparing `promql_parser-0.1.2.tar` & `promql_parser-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 promql_parser-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123     1561 2023-04-27 11:35:35.000000 promql_parser-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-27 11:35:35.000000 promql_parser-0.1.2/.gitignore
--rw-r--r--   0     1001      123     1086 2023-04-27 11:35:35.000000 promql_parser-0.1.2/LICENSE
--rw-r--r--   0     1001      123      632 2023-04-27 11:35:35.000000 promql_parser-0.1.2/README.md
--rw-r--r--   0     1001      123      321 2023-04-27 11:35:35.000000 promql_parser-0.1.2/pyproject.toml
--rwxr-xr-x   0     1001      123      833 2023-04-27 11:36:06.000000 promql_parser-0.1.2/run-maturin-action.sh
--rw-r--r--   0     1001      123    17378 2023-04-27 11:35:35.000000 promql_parser-0.1.2/src/expr.rs
--rw-r--r--   0     1001      123     1755 2023-04-27 11:35:35.000000 promql_parser-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123      321 2023-04-27 11:35:35.000000 promql_parser-0.1.2/test_promql_parser.py
--rw-r--r--   0     1001      123    19588 2023-04-27 11:35:35.000000 promql_parser-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 promql_parser-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 promql_parser-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     1519 2023-06-30 14:30:28.000000 promql_parser-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-30 14:30:28.000000 promql_parser-0.1.3/.gitignore
+-rw-r--r--   0     1001      123     1086 2023-06-30 14:30:28.000000 promql_parser-0.1.3/LICENSE
+-rw-r--r--   0     1001      123      632 2023-06-30 14:30:28.000000 promql_parser-0.1.3/README.md
+-rw-r--r--   0     1001      123      319 2023-06-30 14:30:28.000000 promql_parser-0.1.3/pyproject.toml
+-rwxr-xr-x   0     1001      123      831 2023-06-30 14:31:11.000000 promql_parser-0.1.3/run-maturin-action.sh
+-rw-r--r--   0     1001      123    17378 2023-06-30 14:30:28.000000 promql_parser-0.1.3/src/expr.rs
+-rw-r--r--   0     1001      123     1755 2023-06-30 14:30:28.000000 promql_parser-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123      321 2023-06-30 14:30:28.000000 promql_parser-0.1.3/test_promql_parser.py
+-rw-r--r--   0     1001      123    19794 2023-06-30 14:30:28.000000 promql_parser-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 promql_parser-0.1.3/PKG-INFO
```

### Comparing `promql_parser-0.1.2/Cargo.toml` & `promql_parser-0.1.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [package]
 name = "py-promql-parser"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 description = "PromQL Parser for Python"
 license = "MIT"
 repository = "https://github.com/messense/py-promql-parser"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "promql_parser"
 crate-type = ["cdylib"]
 
 [dependencies]
 chrono = { version = "0.4.23", default-features = false, features = ["std"] }
 promql-parser = "0.1.0"
-pyo3 = { version = "0.18.1", features = ["chrono", "extension-module"] }
+pyo3 = { version = "0.19.0", features = ["chrono", "extension-module"] }
```

### Comparing `promql_parser-0.1.2/.github/workflows/CI.yml` & `promql_parser-0.1.3/.github/workflows/CI.yml`

 * *Files 20% similar despite different names*

```diff
@@ -13,44 +13,42 @@
   linux:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: PyO3/maturin-action@v1
       with:
         manylinux: auto
-        command: build
         args: --release --sdist -o dist --find-interpreter
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   windows:
     runs-on: windows-latest
     steps:
     - uses: actions/checkout@v3
     - uses: PyO3/maturin-action@v1
       with:
-        command: build
         args: --release -o dist --find-interpreter
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   macos:
     runs-on: macos-latest
     steps:
     - uses: actions/checkout@v3
     - uses: PyO3/maturin-action@v1
       with:
-        command: build
-        args: --release -o dist --universal2 --find-interpreter
+        target: universal2-apple-darwin
+        args: --release -o dist --find-interpreter
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   release:
```

### Comparing `promql_parser-0.1.2/.gitignore` & `promql_parser-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.2/LICENSE` & `promql_parser-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.2/README.md` & `promql_parser-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.2/run-maturin-action.sh` & `promql_parser-0.1.3/run-maturin-action.sh`

 * *Files 3% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain stable
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set stable
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
 export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/download/v0.14.17/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v1.1.0/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
 python3 -m pip install cffi || true
 echo "::endgroup::"
 maturin build --release --sdist -o dist --find-interpreter
```

### Comparing `promql_parser-0.1.2/src/expr.rs` & `promql_parser-0.1.3/src/expr.rs`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.2/src/lib.rs` & `promql_parser-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `promql_parser-0.1.2/Cargo.lock` & `promql_parser-0.1.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
@@ -68,51 +74,51 @@
  "regex",
  "serde",
  "vob",
 ]
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
- "num-integer",
+ "android-tzdata",
  "num-traits",
 ]
 
 [[package]]
 name = "enum-iterator"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "706d9e7cf1c7664859d79cd524e4e53ea2b67ea03c98cc2870c5e539695d597e"
+checksum = "7add3873b5dd076766ee79c8e406ad1a472c385476b9e38849f8eec24f1be689"
 dependencies = [
  "enum-iterator-derive",
 ]
 
 [[package]]
 name = "enum-iterator-derive"
-version = "1.2.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "355f93763ef7b0ae1c43c4d8eccc9d5848d84ad1a1d8ce61c421d1ac85a19d05"
+checksum = "eecf8589574ce9b895052fa12d69af7a233f99e6107f5cb8dd1044f2a17bfdcb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.20"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "windows-sys",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -171,23 +177,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
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
 name = "lrlex"
@@ -246,45 +252,35 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "packedvec"
 version = "1.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bde3c690ec20e4a2b4fb46f0289a451181eb50011a1e2acc8d85e2fde9062a45"
 dependencies = [
@@ -300,30 +296,30 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "pest"
-version = "2.5.6"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cbd939b234e95d72bc393d51788aec68aeeb5d51e748ca08ff3aad58cb722f7"
+checksum = "f73935e4d55e2abf7f130186537b19e7a4abc886a0252380b59248af473a3fc9"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "proc-macro-error"
@@ -347,48 +343,48 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.53"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba466839c78239c09faf015484e5cc04860f88242cff4d03eb038f04b4699b73"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "promql-parser"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b86b6a58ddafa87824aecefd60ab8bf33638f4dc687c560a3c06a31122948274"
+checksum = "e03507ede12ce5ebd722a5079208201aa9036dbe0bc340a47315cb9b6c7cfaf6"
 dependencies = [
  "cfgrammar",
  "lazy_static",
  "lrlex",
  "lrpar",
  "regex",
 ]
 
 [[package]]
 name = "py-promql-parser"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "chrono",
  "promql-parser",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if 1.0.0",
  "chrono",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
@@ -396,89 +392,98 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rustc_version"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0dfe2087c51c460008730de8b57e6a320782fbfb312e1f4d520e6c6fae155ee"
 dependencies = [
@@ -513,30 +518,30 @@
 checksum = "00b0bef5b7f9e0df16536d3961cfb6e84331c065b4066afb39768d0e319411f7"
 dependencies = [
  "pest",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.158"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.158"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.9",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
@@ -568,28 +573,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.9"
+version = "2.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0da4a3c17e109f700685ec577c0f85efd9b19bcf15c913985f14dc1ac01775aa"
+checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
@@ -600,40 +605,40 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.9",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "try_from"
 version = "0.3.2"
@@ -647,17 +652,17 @@
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
@@ -697,70 +702,70 @@
  "num-traits",
  "rustc_version",
  "serde",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
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
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `promql_parser-0.1.2/PKG-INFO` & `promql_parser-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promql-parser
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: PromQL Parser for Python
 License: MIT
 Requires-Python: >=3.7
```

