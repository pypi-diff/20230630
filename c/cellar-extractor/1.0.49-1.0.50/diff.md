# Comparing `tmp/cellar_extractor-1.0.49.tar.gz` & `tmp/cellar_extractor-1.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.49.tar", last modified: Tue Apr 11 14:51:27 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.50.tar", last modified: Fri Jun 30 19:37:12 2023, max compression
```

## Comparing `cellar_extractor-1.0.49.tar` & `cellar_extractor-1.0.50.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:51:27.066101 cellar_extractor-1.0.49/
--rw-rw-rw-   0        0        0     6964 2023-04-11 14:51:27.065101 cellar_extractor-1.0.49/PKG-INFO
--rw-rw-rw-   0        0        0     6474 2023-04-11 14:51:21.000000 cellar_extractor-1.0.49/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 14:51:27.055101 cellar_extractor-1.0.49/cellar_extractor/
--rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.49/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      163 2023-04-11 13:37:46.000000 cellar_extractor-1.0.49/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3329 2023-04-11 14:51:21.000000 cellar_extractor-1.0.49/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.49/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.49/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.49/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.49/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.49/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.49/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.49/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1040 2023-04-11 13:52:52.000000 cellar_extractor-1.0.49/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.49/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:51:27.064102 cellar_extractor-1.0.49/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     6964 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-04-11 14:51:27.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 14:51:27.067101 cellar_extractor-1.0.49/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-04-11 14:51:21.000000 cellar_extractor-1.0.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:37:12.022888 cellar_extractor-1.0.50/
+-rw-rw-rw-   0        0        0     6921 2023-06-30 19:37:12.021889 cellar_extractor-1.0.50/PKG-INFO
+-rw-rw-rw-   0        0        0     6474 2023-04-11 14:51:21.000000 cellar_extractor-1.0.50/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 19:37:12.011888 cellar_extractor-1.0.50/cellar_extractor/
+-rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.50/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 13:37:46.000000 cellar_extractor-1.0.50/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3329 2023-04-11 14:51:21.000000 cellar_extractor-1.0.50/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.50/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.50/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11308 2023-06-30 19:37:07.000000 cellar_extractor-1.0.50/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.50/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.50/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6472 2023-06-30 19:36:11.000000 cellar_extractor-1.0.50/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.50/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1040 2023-04-11 13:52:52.000000 cellar_extractor-1.0.50/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.50/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:37:12.019888 cellar_extractor-1.0.50/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     6921 2023-06-30 19:37:11.000000 cellar_extractor-1.0.50/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-06-30 19:37:11.000000 cellar_extractor-1.0.50/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:37:11.000000 cellar_extractor-1.0.50/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-30 19:37:11.000000 cellar_extractor-1.0.50/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 19:37:11.000000 cellar_extractor-1.0.50/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 19:37:12.022888 cellar_extractor-1.0.50/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-06-30 19:37:07.000000 cellar_extractor-1.0.50/setup.py
```

### Comparing `cellar_extractor-1.0.49/PKG-INFO` & `cellar_extractor-1.0.50/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: cellar_extractor
-Version: 1.0.49
+Version: 1.0.50
 Summary: Library for extracting cellar data
-Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## Cellar extractor
 This library contains two functions to get cellar case law data from eurlex.
 
 ## Version
 Python 3.9
@@ -153,9 +151,7 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.49 Summary: Library
-for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.50 Summary: Library
+for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
-Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
-markdown ## Cellar extractor This library contains two functions to get cellar
-case law data from eurlex. ## Version Python 3.9 ## Contributors
+Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
+extractor This library contains two functions to get cellar case law data from
+eurlex. ## Version Python 3.9 ## Contributors
 [pranavnbapat]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install cellar-extractor ## What are the functions?
    1. get_cellar
    2. Gets all the ECLI data from the eurlex sparql endpoint and saves them in
       the CSV or JSON format, in-memory or as a saved file.
    3. get_cellar_extra
```

### Comparing `cellar_extractor-1.0.49/README.md` & `cellar_extractor-1.0.50/README.md`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.50/cellar_extractor/Testing_file.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/cellar.py` & `cellar_extractor-1.0.50/cellar_extractor/cellar.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.50/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.50/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.50/cellar_extractor/citations_adder.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     success=0
     retry=0
     base_query = "SELECT DN,CI WHERE DN = %s"
     base_contains_query = "SELECT DN,CI WHERE DN ~ %s"
     normal_celex, contains_celex = clean_celex(celexes)
     def process_queries(link, celex):
         nonlocal success,retry
-        for i in tqdm(range(0, len(celex), at_once),colour="GREEN"):
+        for i in tqdm(range(0, len(celex), at_once), colour="GREEN", position=0, leave=True, maxinterval=10000):
             curr_celex = celex[i:(i + at_once)]
             input=" OR ".join(curr_celex)
             query = link % (str(input))
             failure = False
             while not failure:
                 response = run_eurlex_webservice_query(query, username, password)
                 if response.status_code == 500 and "WS_WS_CALLS_IDLE_INTERVAL" not in response.text:
```

### Comparing `cellar_extractor-1.0.49/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.50/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.50/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.50/cellar_extractor/fulltext_saving.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 def add_sections(data, threads, json_filepath=None):
     celex = data.loc[:, 'CELEX IDENTIFIER']
     eclis = data.loc[:, 'ECLI']
     length = celex.size
     time.sleep(1)
-    bar = tqdm(total=length, colour="GREEN")
+    bar = tqdm(total=length, colour="GREEN", miniters=int(length/100), position=0, leave=True, maxinterval=10000)
     if length > threads:  # to avoid getting problems with small files
         at_once_threads = int(length / threads)
     else:
         at_once_threads = length
     threads = []
     list_sum = list()
     list_key = list()
```

### Comparing `cellar_extractor-1.0.49/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.50/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.50/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor/sparql.py` & `cellar_extractor-1.0.50/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.50/cellar_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.49
+Version: 1.0.50
 Summary: Library for extracting cellar data
-Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## Cellar extractor
 This library contains two functions to get cellar case law data from eurlex.
 
 ## Version
 Python 3.9
@@ -153,9 +151,7 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.49 Summary: Library
-for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.50 Summary: Library
+for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
-Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
-markdown ## Cellar extractor This library contains two functions to get cellar
-case law data from eurlex. ## Version Python 3.9 ## Contributors
+Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
+extractor This library contains two functions to get cellar case law data from
+eurlex. ## Version Python 3.9 ## Contributors
 [pranavnbapat]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install cellar-extractor ## What are the functions?
    1. get_cellar
    2. Gets all the ECLI data from the eurlex sparql endpoint and saves them in
       the CSV or JSON format, in-memory or as a saved file.
    3. get_cellar_extra
```

### Comparing `cellar_extractor-1.0.49/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.50/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.49/setup.py` & `cellar_extractor-1.0.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.49',
+    version='1.0.50',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

