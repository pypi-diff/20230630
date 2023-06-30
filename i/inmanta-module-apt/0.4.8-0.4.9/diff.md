# Comparing `tmp/inmanta_module_apt-0.4.8-py3-none-any.whl.zip` & `tmp/inmanta_module_apt-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4618 bytes, number of entries: 9
--rw-r--r--  2.0 unx     4390 b- defN 22-Jan-17 12:52 inmanta_plugins/apt/__init__.py
--rw-r--r--  2.0 unx      242 b- defN 22-Jan-17 12:52 inmanta_plugins/apt/setup.cfg
--rw-r--r--  2.0 unx     1082 b- defN 22-Jan-17 12:52 inmanta_plugins/apt/model/_init.cf
--rw-r--r--  2.0 unx      139 b- defN 22-Jan-17 12:52 inmanta_plugins/apt/templates/repo.tmpl
--rw-r--r--  2.0 unx      149 b- defN 22-Jan-17 12:52 tests/test_module.py
--rw-r--r--  2.0 unx      180 b- defN 22-Jan-17 12:52 inmanta_module_apt-0.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-17 12:52 inmanta_module_apt-0.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 22-Jan-17 12:52 inmanta_module_apt-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      776 b- defN 22-Jan-17 12:52 inmanta_module_apt-0.4.8.dist-info/RECORD
-9 files, 7072 bytes uncompressed, 3262 bytes compressed:  53.9%
+Zip file size: 4615 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx     4390 b- defN 22-Mar-15 15:43 inmanta_plugins/apt/__init__.py
+-rw-rw-r--  2.0 unx      242 b- defN 22-Mar-15 15:43 inmanta_plugins/apt/setup.cfg
+-rw-rw-r--  2.0 unx     1082 b- defN 22-Mar-15 15:43 inmanta_plugins/apt/model/_init.cf
+-rw-rw-r--  2.0 unx      139 b- defN 22-Mar-15 15:43 inmanta_plugins/apt/templates/repo.tmpl
+-rw-rw-r--  2.0 unx      149 b- defN 22-Mar-15 15:43 tests/test_module.py
+-rw-rw-r--  2.0 unx      161 b- defN 22-Mar-15 15:43 inmanta_module_apt-0.4.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Mar-15 15:43 inmanta_module_apt-0.4.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 22-Mar-15 15:43 inmanta_module_apt-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      776 b- defN 22-Mar-15 15:43 inmanta_module_apt-0.4.9.dist-info/RECORD
+9 files, 7057 bytes uncompressed, 3259 bytes compressed:  53.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: inmanta_plugins/apt/templates/repo.tmpl
 Comment: 
 
 Filename: tests/test_module.py
 Comment: 
 
-Filename: inmanta_module_apt-0.4.8.dist-info/METADATA
+Filename: inmanta_module_apt-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_apt-0.4.8.dist-info/WHEEL
+Filename: inmanta_module_apt-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_apt-0.4.8.dist-info/top_level.txt
+Filename: inmanta_module_apt-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_apt-0.4.8.dist-info/RECORD
+Filename: inmanta_module_apt-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/apt/setup.cfg

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = inmanta-module-apt
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.4.8
+version = 0.4.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-std
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
```

## Comparing `inmanta_module_apt-0.4.8.dist-info/RECORD` & `inmanta_module_apt-0.4.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 inmanta_plugins/apt/__init__.py,sha256=fzviowFNsGCbaJJzGLzH4js5QEg_booIgiV8WYhr-yw,4390
-inmanta_plugins/apt/setup.cfg,sha256=CuKid3FSMxLgtCFv4IcDi4cCmJ-wn1RP0pyD-W8MjVM,242
+inmanta_plugins/apt/setup.cfg,sha256=Bk3GZ9yxc_OyggwLemSSq6MxVQof8kggIKyTEHc0VRE,242
 inmanta_plugins/apt/model/_init.cf,sha256=_QjESri014y9cf7BPUsRnh9giHpBuAlDkh8e_CpeZ0s,1082
 inmanta_plugins/apt/templates/repo.tmpl,sha256=9KxjD25Hf7Duotvi5rpOL3SoQHiogusKnDcDWhtRk-M,139
 tests/test_module.py,sha256=1rqCOkwEnbC6T5a5hW01X26FIt5zTCQjvjqqZBOh6ds,149
-inmanta_module_apt-0.4.8.dist-info/METADATA,sha256=zUkE0fr4jK-Lp3pT-MnACWUdw3jeK66LvPSmYYzSW-g,180
-inmanta_module_apt-0.4.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inmanta_module_apt-0.4.8.dist-info/top_level.txt,sha256=p-rRN4pnaBSwGgq_yfLjWb72JwSQbe017NsoH8ECWL8,22
-inmanta_module_apt-0.4.8.dist-info/RECORD,,
+inmanta_module_apt-0.4.9.dist-info/METADATA,sha256=7LJeDlYyZBHbuBMj51Ay0-bR81cCml9qnirO5HD2qqQ,161
+inmanta_module_apt-0.4.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inmanta_module_apt-0.4.9.dist-info/top_level.txt,sha256=kiEAGU2wZ924x342O-45FNMcBEnnI0dzdFENs_pZ7V0,26
+inmanta_module_apt-0.4.9.dist-info/RECORD,,
```

