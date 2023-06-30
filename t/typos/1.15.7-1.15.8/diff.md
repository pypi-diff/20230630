# Comparing `tmp/typos-1.15.7.tar.gz` & `tmp/typos-1.15.8.tar.gz`

## Comparing `typos-1.15.7.tar` & `typos-1.15.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.15.7/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.15.7/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44720 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.15.7/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.15.7/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.15.7/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  7026095 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-06-26 20:48:18.000000 typos-1.15.7/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.15.7/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.15.7/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12622 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21859 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32621 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     5919 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123      207 2023-06-26 20:48:18.000000 typos-1.15.7/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      123    53454 2023-06-26 20:48:17.000000 typos-1.15.7/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.15.7/PKG-INFO
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.15.8/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.15.8/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.15.8/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    44720 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.15.8/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    16454 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.15.8/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  7025594 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-06-29 16:17:51.000000 typos-1.15.8/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.15.8/pyproject.toml
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.15.8/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12622 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21859 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32621 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     5919 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123      207 2023-06-29 16:17:51.000000 typos-1.15.8/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      123    53454 2023-06-29 16:17:51.000000 typos-1.15.8/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.15.8/PKG-INFO
```

### Comparing `typos-1.15.7/local_dependencies/typos-vars/Cargo.toml` & `typos-1.15.8/local_dependencies/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.15.8/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/typos/Cargo.toml` & `typos-1.15.8/local_dependencies/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/typos/src/check.rs` & `typos-1.15.8/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/typos/src/dict.rs` & `typos-1.15.8/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/typos/src/tokens.rs` & `typos-1.15.8/local_dependencies/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/dictgen/Cargo.toml` & `typos-1.15.8/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/dictgen/src/map.rs` & `typos-1.15.8/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/dictgen/src/table.rs` & `typos-1.15.8/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/dictgen/src/trie.rs` & `typos-1.15.8/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/varcon-core/Cargo.toml` & `typos-1.15.8/local_dependencies/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.15.8/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/varcon-core/src/lib.rs` & `typos-1.15.8/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/varcon-core/src/parser.rs` & `typos-1.15.8/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/local_dependencies/typos-dict/Cargo.toml` & `typos-1.15.8/local_dependencies/typos-dict/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-dict"
-version = "0.10.3"
+version = "0.10.4"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.15.7/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.15.8/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files 0% similar despite different names*

```diff
@@ -8762,30 +8762,28 @@
         dictgen::InsensitiveStr::Ascii("nsed"),
         dictgen::InsensitiveStr::Ascii("nsual"),
         dictgen::InsensitiveStr::Ascii("sabe"),
         dictgen::InsensitiveStr::Ascii("sal"),
         dictgen::InsensitiveStr::Ascii("sally"),
         dictgen::InsensitiveStr::Ascii("saully"),
         dictgen::InsensitiveStr::Ascii("seable"),
-        dictgen::InsensitiveStr::Ascii("seful"),
         dictgen::InsensitiveStr::Ascii("sre"),
         dictgen::InsensitiveStr::Ascii("suable"),
         dictgen::InsensitiveStr::Ascii("sualy"),
         dictgen::InsensitiveStr::Ascii("sued"),
     ],
     values: &[
         &["unused"],
         &["unused"],
         &["unusual"],
         &["unusable"],
         &["unusual"],
         &["unusually"],
         &["unusually"],
         &["unusable"],
-        &["useless"],
         &["unsure"],
         &["unusable"],
         &["unusually"],
         &["unused"],
     ],
     range: 2..=6,
 };
@@ -35999,15 +35997,14 @@
         dictgen::InsensitiveStr::Ascii("latation"),
         dictgen::InsensitiveStr::Ascii("latenous"),
         dictgen::InsensitiveStr::Ascii("latenously"),
         dictgen::InsensitiveStr::Ascii("latie"),
         dictgen::InsensitiveStr::Ascii("laties"),
         dictgen::InsensitiveStr::Ascii("latin"),
         dictgen::InsensitiveStr::Ascii("latious"),
-        dictgen::InsensitiveStr::Ascii("lative"),
         dictgen::InsensitiveStr::Ascii("latneous"),
         dictgen::InsensitiveStr::Ascii("latneously"),
         dictgen::InsensitiveStr::Ascii("lato"),
         dictgen::InsensitiveStr::Ascii("latons"),
         dictgen::InsensitiveStr::Ascii("latore"),
         dictgen::InsensitiveStr::Ascii("ltaenous"),
         dictgen::InsensitiveStr::Ascii("ltaenously"),
@@ -36056,15 +36053,14 @@
         &["simulation"],
         &["simultaneous"],
         &["simultaneously"],
         &["simulate"],
         &["simulate"],
         &["simulation"],
         &["simulations"],
-        &["simulate"],
         &["simultaneous"],
         &["simultaneously"],
         &["simulation"],
         &["simulations"],
         &["simulate"],
         &["simultaneous"],
         &["simultaneously"],
@@ -69195,30 +69191,26 @@
         dictgen::InsensitiveStr::Ascii("ention"),
         dictgen::InsensitiveStr::Ascii("ents"),
         dictgen::InsensitiveStr::Ascii("ersley"),
         dictgen::InsensitiveStr::Ascii("erst"),
         dictgen::InsensitiveStr::Ascii("ertes"),
         dictgen::InsensitiveStr::Ascii("iew"),
         dictgen::InsensitiveStr::Ascii("iews"),
-        dictgen::InsensitiveStr::Ascii("ious"),
-        dictgen::InsensitiveStr::Ascii("iously"),
     ],
     values: &[
         &["prevail"],
         &["prevailing"],
         &["prevalence"],
         &["prevention"],
         &["prevents"],
         &["perverse"],
         &["pervert"],
         &["perverse"],
         &["preview", "purview"],
         &["previews", "purviews"],
-        &["previous"],
-        &["previously"],
     ],
     range: 3..=6,
 };
 
 static WORD_PERU_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PERU_CHILDREN),
     value: None,
@@ -105248,17 +105240,14 @@
         dictgen::InsensitiveStr::Ascii("cional"),
         dictgen::InsensitiveStr::Ascii("des"),
         dictgen::InsensitiveStr::Ascii("det"),
         dictgen::InsensitiveStr::Ascii("dos"),
         dictgen::InsensitiveStr::Ascii("eded"),
         dictgen::InsensitiveStr::Ascii("isty"),
         dictgen::InsensitiveStr::Ascii("seley"),
-        dictgen::InsensitiveStr::Ascii("sion"),
-        dictgen::InsensitiveStr::Ascii("sional"),
-        dictgen::InsensitiveStr::Ascii("sionally"),
         dictgen::InsensitiveStr::Ascii("sionaly"),
         dictgen::InsensitiveStr::Ascii("sitive"),
         dictgen::InsensitiveStr::Ascii("sitiy"),
         dictgen::InsensitiveStr::Ascii("sley"),
         dictgen::InsensitiveStr::Ascii("st"),
         dictgen::InsensitiveStr::Ascii("tas"),
         dictgen::InsensitiveStr::Ascii("tation"),
@@ -105282,18 +105271,15 @@
         &["intentional"],
         &["intends"],
         &["intended"],
         &["intends"],
         &["intended"],
         &["intensity"],
         &["intensely"],
-        &["intention"],
-        &["intentional"],
-        &["intentionally"],
-        &["intentionally"],
+        &["intentionally", "intensionally"],
         &["insensitive", "intensive"],
         &["intensity"],
         &["intensely"],
         &["intents"],
         &["intents"],
         &["indentation"],
         &["intended", "indented"],
```

### Comparing `typos-1.15.7/rust_src/typos-cli/Cargo.toml` & `typos-1.15.8/rust_src/typos-cli/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.15.7"
+version = "1.15.8"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.15.7/rust_src/typos-cli/benches/checks.rs` & `typos-1.15.8/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/benches/corrections.rs` & `typos-1.15.8/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/benches/data.rs` & `typos-1.15.8/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.15.8/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.15.8/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.15.8/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.15.8/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/config.rs` & `typos-1.15.8/rust_src/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/default_types.rs` & `typos-1.15.8/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/dict.rs` & `typos-1.15.8/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/file.rs` & `typos-1.15.8/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/file_type.rs` & `typos-1.15.8/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/policy.rs` & `typos-1.15.8/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/rust_src/typos-cli/src/report.rs` & `typos-1.15.8/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.7/Cargo.lock` & `typos-1.15.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1649,15 +1649,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.15.7"
+version = "1.15.8"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
@@ -1697,15 +1697,15 @@
  "unicode-segmentation",
  "unicode-width",
  "varcon-core",
 ]
 
 [[package]]
 name = "typos-dict"
-version = "0.10.3"
+version = "0.10.4"
 dependencies = [
  "codegenrs",
  "csv",
  "dictgen",
  "edit-distance",
  "indexmap 2.0.0",
  "itertools",
```

### Comparing `typos-1.15.7/PKG-INFO` & `typos-1.15.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.15.7
+Version: 1.15.8
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

