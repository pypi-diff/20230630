# Comparing `tmp/pasqal-cloud-0.3.0.tar.gz` & `tmp/pasqal-cloud-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.3.0.tar", last modified: Thu Jun 22 15:02:59 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.3.1.tar", last modified: Fri Jun 30 12:39:33 2023, max compression
```

## Comparing `pasqal-cloud-0.3.0.tar` & `pasqal-cloud-0.3.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.840326 pasqal-cloud-0.3.0/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.840326 pasqal-cloud-0.3.0/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.840326 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_project_renaming_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_project_renaming_compatibility.py
```

### Comparing `pasqal-cloud-0.3.0/LICENSE` & `pasqal-cloud-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/PKG-INFO` & `pasqal-cloud-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.0
+Version: 0.3.1
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.3.0/README.md` & `pasqal-cloud-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/__init__.py` & `pasqal-cloud-0.3.1/pasqal_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/_version.py` & `pasqal-cloud-0.3.1/pasqal_cloud/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/authentication.py` & `pasqal-cloud-0.3.1/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/batch.py` & `pasqal-cloud-0.3.1/pasqal_cloud/batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/client.py` & `pasqal-cloud-0.3.1/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.3.1/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/errors.py` & `pasqal-cloud-0.3.1/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/job.py` & `pasqal-cloud-0.3.1/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.3.1/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.3.1/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.0
+Version: 0.3.1
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.3.0/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.3.1/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 pasqal_cloud.egg-info/top_level.txt
 pasqal_cloud/device/__init__.py
 pasqal_cloud/device/emulator_types.py
 pasqal_cloud/device/configuration/__init__.py
 pasqal_cloud/device/configuration/base_config.py
 pasqal_cloud/device/configuration/emu_free.py
 pasqal_cloud/device/configuration/emu_tn.py
+pasqal_cloud/device/configuration/result_type.py
 pasqal_cloud/utils/__init__.py
 pasqal_cloud/utils/jsend.py
 pasqal_cloud/utils/strenum.py
 sdk/__init__.py
 sdk/setup.py
 sdk/device/__init__.py
 sdk/device/configuration/__init__.py
```

### Comparing `pasqal-cloud-0.3.0/sdk/setup.py` & `pasqal-cloud-0.3.1/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/setup.py` & `pasqal-cloud-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/conftest.py` & `pasqal-cloud-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/test_batch.py` & `pasqal-cloud-0.3.1/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/test_client.py` & `pasqal-cloud-0.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.3.1/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/test_config.py` & `pasqal-cloud-0.3.1/tests/test_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,83 @@
 from __future__ import annotations
 
-import pytest
+import re
 
+import pytest
 from pasqal_cloud.device import EmuFreeConfig
 from pasqal_cloud.device.configuration.base_config import (
     BaseConfig,
     INVALID_KEY_ERROR_MSG,
+    INVALID_RESULT_TYPES,
     InvalidConfiguration,
 )
 from pasqal_cloud.device.configuration.emu_tn import (
     DT_VALUE_NOT_VALID,
     EmuTNConfig,
     PRECISION_NOT_VALID,
 )
+from pasqal_cloud.device.configuration.result_type import ResultType
 
 
 @pytest.mark.parametrize(
     "config, expected",
     [
         (
             EmuTNConfig(
                 dt=10.0,
-                extra_config={"extra": "parameter", "extra_dict": {"key": "value"}},
+                extra_config={
+                    "extra": "parameter",
+                    "extra_dict": {"key": "value"},
+                },
             ),
             {
                 "dt": 10.0,
                 "precision": "normal",
                 "max_bond_dim": 500,
                 "extra": "parameter",
                 "extra_dict": {"key": "value"},
+                "result_types": None,
+            },
+        ),
+        (
+            EmuTNConfig(result_types=[ResultType.COUNTER]),
+            {
+                "dt": 10.0,
+                "precision": "normal",
+                "max_bond_dim": 500,
+                "result_types": [ResultType.COUNTER],
+            },
+        ),
+        (
+            EmuFreeConfig(),
+            {
+                "with_noise": False,
+                "result_types": None,
+            },
+        ),
+        (
+            EmuFreeConfig(with_noise=True),
+            {
+                "with_noise": True,
+                "result_types": None,
+            },
+        ),
+        (
+            BaseConfig(),
+            {
+                "result_types": None,
+            },
+        ),
+        (
+            BaseConfig(extra_config={"extra": "parameter"}),
+            {
+                "extra": "parameter",
+                "result_types": None,
             },
         ),
-        (EmuTNConfig(), {"dt": 10.0, "precision": "normal", "max_bond_dim": 500}),
-        (EmuFreeConfig(), {"with_noise": False}),
-        (EmuFreeConfig(with_noise=True), {"with_noise": True}),
-        (BaseConfig(), {}),
-        (BaseConfig(extra_config={"extra": "parameter"}), {"extra": "parameter"}),
     ],
 )
 def test_configuration_to_dict(config: BaseConfig, expected: dict):
     assert config.to_dict() == expected
 
 
 @pytest.mark.parametrize(
@@ -81,13 +119,20 @@
         (EmuTNConfig(), {"dt": 10.0}, INVALID_KEY_ERROR_MSG.format("dt")),
         (EmuTNConfig(dt=-1), None, DT_VALUE_NOT_VALID.format(-1)),
         (
             EmuTNConfig(precision="nonsense"),
             None,
             PRECISION_NOT_VALID.format("nonsense"),
         ),
+        (
+            EmuTNConfig(result_types=[ResultType.EXPECTATION]),
+            None,
+            INVALID_RESULT_TYPES.format(
+                [ResultType.EXPECTATION], EmuTNConfig().allowed_result_types
+            ),
+        ),
     ],
 )
 def test_wrong_configuration(config, extra_config, expected):
     config.extra_config = extra_config
-    with pytest.raises(InvalidConfiguration, match=expected):
+    with pytest.raises(InvalidConfiguration, match=re.escape(expected)):
         config.to_dict()
```

### Comparing `pasqal-cloud-0.3.0/tests/test_device_specs.py` & `pasqal-cloud-0.3.1/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/test_doubles/authentication.py` & `pasqal-cloud-0.3.1/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/test_job.py` & `pasqal-cloud-0.3.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.0/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.3.1/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

