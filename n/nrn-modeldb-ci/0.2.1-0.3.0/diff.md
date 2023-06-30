# Comparing `tmp/nrn-modeldb-ci-0.2.1.tar.gz` & `tmp/nrn-modeldb-ci-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrn-modeldb-ci-0.2.1.tar", last modified: Mon May  1 07:37:47 2023, max compression
+gzip compressed data, was "nrn-modeldb-ci-0.3.0.tar", last modified: Fri Jun 30 09:48:25 2023, max compression
```

## Comparing `nrn-modeldb-ci-0.2.1.tar` & `nrn-modeldb-ci-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/.github/workflows/nrn-modeldb-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/modeldb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/hocscripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26146 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/modeldb-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/modelrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/showgout.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/modeldb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/templates/diffreport.html
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/templates/runtimes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:48:25.352140 nrn-modeldb-ci-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:48:25.348140 nrn-modeldb-ci-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:48:25.352140 nrn-modeldb-ci-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/.github/workflows/nrn-modeldb-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-30 09:48:25.352140 nrn-modeldb-ci-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:48:25.352140 nrn-modeldb-ci-0.3.0/modeldb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/hocscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37927 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/modeldb-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/modelrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/showgout.hoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:48:25.352140 nrn-modeldb-ci-0.3.0/modeldb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/templates/diffreport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/modeldb/templates/runtimes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:48:25.352140 nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-30 09:48:25.000000 nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 09:48:25.000000 nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:48:25.000000 nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 09:48:25.000000 nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 09:48:25.000000 nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 09:48:25.000000 nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:48:25.352140 nrn-modeldb-ci-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-30 09:48:14.000000 nrn-modeldb-ci-0.3.0/setup.py
```

### Comparing `nrn-modeldb-ci-0.2.1/.github/workflows/nrn-modeldb-ci.yaml` & `nrn-modeldb-ci-0.3.0/.github/workflows/nrn-modeldb-ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -134,39 +134,35 @@
         sudo apt-get install xvfb
         sudo /usr/bin/Xvfb $DISPLAY -screen 0 1600x1200x24 -noreset -nolock -shmem &  # run in bg
         # Install python dependencies
         python -m pip install --upgrade pip
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
         #Install project in editable mode
         python -m pip install -e .
-        echo "date=$(date -u "+%Y%m")" >> $GITHUB_OUTPUT
     
     - name: Cache ModelDB models
-      id: cache-models
       uses: actions/cache@v3
       with:
         path: |
           cache
           modeldb/modeldb-meta.yaml
-        key: models-${{steps.install-deps.outputs.date}}
+        key: dynamic-models
 
     - name: Get ModelDB models
-      if: steps.cache-models.outputs.cache-hit != 'true'
-      run: getmodels
+      run: getmodels $MODELS_TO_RUN
 
     - name: Run Models with NEURON V1 -> ${{ env.NEURON_V1 }}
       run: |
         # Install NEURON V1
         if [[ -d "${DROP_DIR_V1}" ]]; then
           python -m pip install --user --find-links ${DROP_DIR_V1} neuron-nightly
         else
           python -m pip install $NEURON_V1
         fi
         nrn_ver=`python -c "from neuron import __version__ as nrn_ver; print(nrn_ver)"`
-        ps uxf # debug
         runmodels --gout --workdir=$nrn_ver $MODELS_TO_RUN
         # Filter out the gout data before generating HTML reports. The HTML
         # diff uses the original gout files on disk anyway. Compress the large
         # JSON file including gout data for inclusion in the artifacts
         mv ${nrn_ver}.json ${nrn_ver}-full.json
         jq -r 'del(.[].gout)' ${nrn_ver}-full.json > ${nrn_ver}.json
         xz ${nrn_ver}-full.json
@@ -185,15 +181,14 @@
         # Install NEURON V2
         if [[ -d "${DROP_DIR_V2}" ]]; then
           python -m pip install --user --find-links ${DROP_DIR_V2} neuron-nightly
         else
           python -m pip install $NEURON_V2
         fi
         nrn_ver=`python -c "from neuron import __version__ as nrn_ver; print(nrn_ver)"`
-        ps uxf # debug
         runmodels --gout --workdir=$nrn_ver $MODELS_TO_RUN
         # Filter out the gout data before generating HTML reports. The HTML
         # diff uses the original gout files on disk anyway. Compress the large
         # JSON file including gout data for inclusion in the artifacts
         mv ${nrn_ver}.json ${nrn_ver}-full.json
         jq -r 'del(.[].gout)' ${nrn_ver}-full.json > ${nrn_ver}.json
         xz ${nrn_ver}-full.json
```

### Comparing `nrn-modeldb-ci-0.2.1/.github/workflows/python-publish.yml` & `nrn-modeldb-ci-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/LICENSE.txt` & `nrn-modeldb-ci-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/PKG-INFO` & `nrn-modeldb-ci-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrn-modeldb-ci
-Version: 0.2.1
+Version: 0.3.0
 Summary: NEURON ModelDB CI tools
 Home-page: https://github.com/neuronsimulator/nrn-modeldb-ci
 Author: EPFL Blue Brain Project & Yale
 Author-email: alexandru.savulescu@epfl.ch
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -73,15 +73,16 @@
   | Config                  | Details                                                                     |
   | ---                     | ----                                                                        |
   | ROOT_DIR                | location of `nrn-modeldb-ci` installation                                   |
   | MODELDB_ROOT_DIR        | path to `modeldb` package inside `nrn-modeldb-ci`                           |
   | MODELDB_RUN_FILE        | yaml file containing run instructions for models (required for `runmodels`) |
   | MODELDB_METADATA_FILE   | yaml file containing model info for those downloaded with `getmodels`       |
   | MODELS_ZIP_DIR          | location of cache folder for models populated via `getmodels`               |
-  | MDB_NEURON_MODELS_URL   | url used to get list of all NEURON model ids (necessary for `getmodels`)    |
+  | MDB_NEURON_MODELS_URL   | url template used to get NEURON model IDs and last-updated timestamps (needed for `getmodels`) |
+  | MDB_MODEL_METADATA_URL  | url template used to get metadata about a single NEURON model (needed for `getmodels`) |
   | MDB_MODEL_DOWNLOAD_URL  | url template used for model downloading (cf `{model_id}`)                   |
 
 ## Model Run
 
 ### MODELDB_RUN_FILE 
 
 This is where the "black magic" lives, instructions on how to run models from ModelDB.
```

### Comparing `nrn-modeldb-ci-0.2.1/README.md` & `nrn-modeldb-ci-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
   | Config                  | Details                                                                     |
   | ---                     | ----                                                                        |
   | ROOT_DIR                | location of `nrn-modeldb-ci` installation                                   |
   | MODELDB_ROOT_DIR        | path to `modeldb` package inside `nrn-modeldb-ci`                           |
   | MODELDB_RUN_FILE        | yaml file containing run instructions for models (required for `runmodels`) |
   | MODELDB_METADATA_FILE   | yaml file containing model info for those downloaded with `getmodels`       |
   | MODELS_ZIP_DIR          | location of cache folder for models populated via `getmodels`               |
-  | MDB_NEURON_MODELS_URL   | url used to get list of all NEURON model ids (necessary for `getmodels`)    |
+  | MDB_NEURON_MODELS_URL   | url template used to get NEURON model IDs and last-updated timestamps (needed for `getmodels`) |
+  | MDB_MODEL_METADATA_URL  | url template used to get metadata about a single NEURON model (needed for `getmodels`) |
   | MDB_MODEL_DOWNLOAD_URL  | url template used for model downloading (cf `{model_id}`)                   |
 
 ## Model Run
 
 ### MODELDB_RUN_FILE 
 
 This is where the "black magic" lives, instructions on how to run models from ModelDB.
```

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/commands.py` & `nrn-modeldb-ci-0.3.0/modeldb/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,16 +245,15 @@
     # Return a useful status code
     code = 0
     if len(diff_dict) > 1:
         assert "0" in diff_dict  # summary info; not a real diff
         print("FAILURE: stdout diffs in {}".format(set(diff_dict.keys()) - {"0"}))
         code = 1
     if len(gout_dict) > 1:
-        assert "0" in gout_dict  # summary info; not a real diff
-        print("FAILURE: gout diffs in {}".format(set(diff_dict.keys()) - {"0"}))
+        print("FAILURE: gout diffs in {}".format(set(gout_dict.keys())))
         code = 1
     total_failures = sum(
         version_stats["Failed models"]["Count"] for version_stats in stats_dict.values()
     )
     if total_failures > 0:
         print(
             "FAILURE: there were {} failed model builds across {} versions of NEURON".format(
```

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/hocscripts.py` & `nrn-modeldb-ci-0.3.0/modeldb/hocscripts.py`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/modelrun.py` & `nrn-modeldb-ci-0.3.0/modeldb/modelrun.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     )
     out, _ = sp.communicate()
     try:
         out = out.decode("utf-8")
     except UnicodeDecodeError:
         raise Exception("Could not decode output:" + repr(out))
     model.nrn_run.extend(curate_log_string(model, out).splitlines())
-    if sp.returncode > 1:
+    if sp.returncode != 0 and not model.get("ignore_exit_code", False):
         model._nrn_run_error = True
 
 
 def clean_model_dir(model):
     # delete x86_64 folder
     run_commands(model, ["/bin/sh", "-c", "rm -rf ./{}/".format(platform.machine())], work_dir=model.run_info["start_dir"])
 
@@ -172,15 +172,16 @@
 
     model.run_info["init"] = os.path.join(model.model_dir, "quit.hoc")
 
 
 def select_mosinit(model):
     # look for `mosinit.hoc`. It could also be produced by `init` script above
     mosfiles = glob.glob(model.model_dir + "/**/mosinit.hoc", recursive=True)
-    mosfiles.sort()
+    # prefer less-nested directories, then sort alphabetically
+    mosfiles.sort(key=lambda x: (x.count(os.sep), x))
     if len(mosfiles):
         model.run_info["start_dir"] = os.path.dirname(os.path.join(model.model_dir, mosfiles[0]))
         model.run_info["init"] = mosfiles[0]
     else:
         build_quit_hoc(model)
         model._no_mosinit_hoc = True
 
@@ -265,23 +266,52 @@
         if model["run"] is None:
             append_log(model, model.logs,
                        "Model in do not run mode according to modeldb-run.yaml:\n\t{}\n".format(
                            model["comment"]
                        )
            )
 
-        # Get mod files. Model can have a custom mod directory or directories, otherwise we search in the start_dir
+        # Get .mod files. There are two options:
+        # - the `model_dir` key in `modeldb-run.yaml` can be a
+        #   semicolon-separated list of directories containing .mod files.
+        # - recursively search for directories containing .mod files, if there
+        #   is exactly one such directory, use it
+        mods = []
         if "model_dir" in model:
-            mods = []
-            for moddir in model["model_dir"].split(';'):
-                mod_pattern = os.path.join(model.model_dir, moddir) + "/*.mod"
-                mods.extend(glob.glob(mod_pattern))
+            mod_dirs = model["model_dir"].split(";")
+            for mod_dir in mod_dirs:
+                mod_dir = os.path.join(model.model_dir, mod_dir)
+                if not os.path.isdir(mod_dir):
+                    raise Exception("Explicitly specified model_dir {} does not exist".format(mod_dir))
+                mods += glob.glob(mod_dir + "/*.mod")
         else:
-            mod_pattern = model.run_info["start_dir"] + "/*.mod"
-            mods = glob.glob(mod_pattern)
+            top = model.run_info["start_dir"]
+            mod_dirs = []
+            for root, _, files in os.walk(top):
+                local_mods = [
+                    os.path.join(root, name) for name in files if name.endswith(".mod")
+                ]
+                if local_mods:
+                    mod_dirs.append(os.path.relpath(root, top))
+                    # not += because we never merge multiple .mod dirs automatically
+                    mods = local_mods
+            if len(mod_dirs) > 1:
+                raise Exception(
+                    "Found multiple possible .mod file directores, please configure the correct subset: {}".format(
+                        mod_dirs
+                    )
+                )
+            elif len(mod_dirs) == 1:
+                append_log(
+                    model,
+                    model.logs,
+                    "Chose subdirectory {} for .mod files".format(mod_dirs[0]),
+                )
+            else:
+                append_log(model, model.logs, "No .mod file directory found")
         # compile mods if available
         if len(mods):
             # in case of reruns
             clean_model_dir(model)
             # translate them to cpp
             compile_mods(model, mods)
 
@@ -299,25 +329,28 @@
             "Model is not run due to --norun option"
         )
     else:
         try:
             nrn_exe = "./{}/special".format(platform.machine()) if mods is not None and len(mods) else "nrniv"
             # '-nogui' creates segfault
             model_run_cmds = [nrn_exe, '-nobanner']
+            if "hoc_stack_size" in model:
+                model_run_cmds += ["-NSTACK", str(int(model["hoc_stack_size"]))]
             if model.run_py:
                 model_run_cmds.append('-python')
             model_run_cmds += [model.run_info["init"], model.run_info["driver"]]
             append_log(model, model.nrn_run, "RUNNING -> {}".format(" ".join(model_run_cmds)))
             run_neuron_cmds(model, model_run_cmds)
             if os.path.isfile(os.path.join(model.model_dir, "gout")):
                 with open(os.path.join(model.model_dir, "gout"), 'r') as gout:
                     model._gout = gout.readlines()
         except Exception:  # noqa
             append_log(model, model.nrn_run, traceback.format_exc())
-            model._nrn_run_error = True
+            if not model.get("ignore_exit_code", False):
+                model._nrn_run_error = True
 
     stop_time = time.perf_counter()
     model._run_times["model"] = stop_time - start_time
 
     # Record the total too (for backwards compatibility)
     model._run_time = str(sum(model._run_times.values()))
 
@@ -428,14 +461,16 @@
             if self._gout:
                 self.run_logs[model.id]["gout"] = model.gout
             self.run_logs[model.id]["nrn_run"] = model.nrn_run
             if "skip" in model:
                 self.run_logs[model.id]["do_not_run"] = True
             if model.nrn_run_error:
                 self.run_logs[model.id]["nrn_run_err"] = True
+            if model.get("ignore_exit_code", False):
+                self.run_logs[model.id]["ignore_exit_code"] = True
             if model.no_mosinit_hoc:
                 self.run_logs[model.id]["no_mosinit_hoc"] = True
             self.run_logs[model.id]["run_info"] = model.run_info
             self.run_logs[model.id]["run_time"] = model.run_time
             self.run_logs[model.id]["run_times"] = model.run_times
             self.logger.debug("Done for: {} in {}".format(str(model.id), str(model.run_times)))
```

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/progressbar.py` & `nrn-modeldb-ci-0.3.0/modeldb/progressbar.py`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/report.py` & `nrn-modeldb-ci-0.3.0/modeldb/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -101,16 +101,54 @@
                         runtime_dict[k][runkey] = _speedup(data_a[k]["run_times"][runkey], data_b[k]["run_times"][runkey])
                 
                 # compare gout
                 gout_a_file = os.path.join(data_a[k]["run_info"]["start_dir"], "gout")
                 gout_b_file = os.path.join(data_b[k]["run_info"]["start_dir"], "gout")
                 # gout may be missing in one of the paths. `diff -N` treats non-existent files as empty.
                 if os.path.isfile(gout_a_file) or os.path.isfile(gout_b_file):
-                    diff_out = subprocess.getoutput(
-                        "diff -uN --speed-large-files {} {} | head -n 30".format(
-                            shlex.quote(gout_a_file), shlex.quote(gout_b_file)
-                        )
+                    # https://stackoverflow.com/questions/1180606/using-subprocess-popen-for-process-with-large-output
+                    diff_cmd = [
+                        "diff",
+                        "-uN",
+                        "--speed-large-files",
+                        gout_a_file,
+                        gout_b_file,
+                    ]
+                    child = subprocess.Popen(
+                        diff_cmd,
+                        bufsize=1,  # line buffered
+                        stdout=subprocess.PIPE,  # we read from stdout below
+                        shell=False,
+                        text=True,
                     )
+                    # sometimes when the results are wildly different then diff can ~hang
+                    timeout = 2  # seconds
+                    try:
+                        (diff_out, _) = child.communicate(timeout=timeout)
+                        diff_out = diff_out.splitlines()
+                        # maximum 30 lines to keep the summary diff page responsive
+                        if len(diff_out) > 30:
+                            diff_out = "\n".join(
+                                diff_out[:30]
+                                + [
+                                    "... {} lines suppressed ...".format(
+                                        len(diff_out) - 30
+                                    )
+                                ]
+                            )
+                        else:
+                            diff_out = "\n".join(diff_out)
+                    except subprocess.TimeoutExpired:
+                        child.kill()
+                        diff_out = (
+                            "{} did not complete in {} seconds, killing it".format(
+                                diff_cmd, timeout
+                            )
+                        )
                     if diff_out:
-                        gout_dict[k] = highlight(diff_out, DiffLexer(), HtmlFormatter(linenos=True, cssclass="colorful", full=True))
+                        gout_dict[k] = highlight(
+                            diff_out,
+                            DiffLexer(),
+                            HtmlFormatter(linenos=True, cssclass="colorful", full=True),
+                        )
 
     return diff_dict, gout_dict, runtime_dict, stats_dict, v1, v2
```

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/showgout.hoc` & `nrn-modeldb-ci-0.3.0/modeldb/showgout.hoc`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/templates/diffreport.html` & `nrn-modeldb-ci-0.3.0/modeldb/templates/diffreport.html`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/templates/report.html` & `nrn-modeldb-ci-0.3.0/modeldb/templates/report.html`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/modeldb/templates/runtimes.html` & `nrn-modeldb-ci-0.3.0/modeldb/templates/runtimes.html`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/PKG-INFO` & `nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrn-modeldb-ci
-Version: 0.2.1
+Version: 0.3.0
 Summary: NEURON ModelDB CI tools
 Home-page: https://github.com/neuronsimulator/nrn-modeldb-ci
 Author: EPFL Blue Brain Project & Yale
 Author-email: alexandru.savulescu@epfl.ch
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -73,15 +73,16 @@
   | Config                  | Details                                                                     |
   | ---                     | ----                                                                        |
   | ROOT_DIR                | location of `nrn-modeldb-ci` installation                                   |
   | MODELDB_ROOT_DIR        | path to `modeldb` package inside `nrn-modeldb-ci`                           |
   | MODELDB_RUN_FILE        | yaml file containing run instructions for models (required for `runmodels`) |
   | MODELDB_METADATA_FILE   | yaml file containing model info for those downloaded with `getmodels`       |
   | MODELS_ZIP_DIR          | location of cache folder for models populated via `getmodels`               |
-  | MDB_NEURON_MODELS_URL   | url used to get list of all NEURON model ids (necessary for `getmodels`)    |
+  | MDB_NEURON_MODELS_URL   | url template used to get NEURON model IDs and last-updated timestamps (needed for `getmodels`) |
+  | MDB_MODEL_METADATA_URL  | url template used to get metadata about a single NEURON model (needed for `getmodels`) |
   | MDB_MODEL_DOWNLOAD_URL  | url template used for model downloading (cf `{model_id}`)                   |
 
 ## Model Run
 
 ### MODELDB_RUN_FILE 
 
 This is where the "black magic" lives, instructions on how to run models from ModelDB.
```

### Comparing `nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/SOURCES.txt` & `nrn-modeldb-ci-0.3.0/nrn_modeldb_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.1/setup.py` & `nrn-modeldb-ci-0.3.0/setup.py`

 * *Files identical despite different names*

