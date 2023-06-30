# Comparing `tmp/delphai_fastapi-0.1.5.tar.gz` & `tmp/delphai_fastapi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-0.1.5.tar", max compression
+gzip compressed data, was "delphai_fastapi-0.1.7.tar", max compression
```

## Comparing `delphai_fastapi-0.1.5.tar` & `delphai_fastapi-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0        0 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2521 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/app.py
--rw-r--r--   0        0        0     3173 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     3266 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0     1582 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/models.py
--rw-r--r--   0        0        0     1342 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/types.py
--rw-r--r--   0        0        0      472 2023-06-27 15:59:27.450844 delphai_fastapi-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.5/setup.py
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2521 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     3173 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     3584 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/job_posts/__init__.py
+-rw-r--r--   0        0        0      912 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/job_posts/models.py
+-rw-r--r--   0        0        0     1808 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/models.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/news_articles/__init__.py
+-rw-r--r--   0        0        0     1115 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/news_articles/models.py
+-rw-r--r--   0        0        0     1342 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      468 2023-06-30 09:05:18.526642 delphai_fastapi-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.7/setup.py
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.7/PKG-INFO
```

### Comparing `delphai_fastapi-0.1.5/delphai_fastapi/app.py` & `delphai_fastapi-0.1.7/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.5/delphai_fastapi/auth.py` & `delphai_fastapi-0.1.7/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.5/delphai_fastapi/companies/models.py` & `delphai_fastapi-0.1.7/delphai_fastapi/companies/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,21 @@
     )
 
 
 class CompanyDescription(CamelModel):
     long: Optional[str] = Field(
         description="Company's default description",
         example=(
-            "delphai is an AI and big data analytics software platform that informs business decisions and validates strategies"
+            "delphai is an AI and big data analytics software platform that informs "
+            "business decisions and validates strategies"
         ),
     )
     short: Optional[str] = Field(
         description="Truncated version of company's default description",
-        example=("delphai is an AI and big data analytics software platform"),
+        example="delphai is an AI and big data analytics software platform",
     )
 
 
 class CompanyRevenue(CamelModel):
     currency: Optional[str] = Field(
         description="Currency of revenue number", example="EUR"
     )
@@ -61,26 +62,39 @@
     products: Optional[List[str]] = Field(
         description="List of company products", example=["Software"]
     )
 
 
 class ProjectsCompany(CamelModel):
     company: Company
-    custom_labels: Optional[List[str]] = Field(description="Custom labels assigned by user")
+    custom_labels: Optional[List[str]] = Field(
+        description="Custom labels assigned by user"
+    )
     assigned_by: str = Field(description="By whom the company was added to the project")
 
 
 class CompaniesSearchResult(CamelModel):
     company: Company
     score: float = Field(default=0, description="Search score", example="202.35745")
     snippets: List[str] = Field(
         default=[],
         description="Snippets containing query keywords",
         example=[
-            "delphai is an AI and big data analytics software platform that informs business decisions and validates strategies"
+            "delphai is an AI and big data analytics software platform that informs "
+            "business decisions and validates strategies"
         ],
     )
 
 
 class CompaniesSearchResults(CamelModel):
     results: List[CompaniesSearchResult]
     total: int = Field(..., description="Number of results", example=1337)
+
+
+class CompanyPeer(CamelModel):
+    company: Company
+    score: float = Field(default=0, description="Search score", example="202.35745")
+
+
+class CompanyPeers(CamelModel):
+    results: List[CompanyPeer]
+    total: int = Field(..., description="Number of results", example=5)
```

### Comparing `delphai_fastapi-0.1.5/delphai_fastapi/models.py` & `delphai_fastapi-0.1.7/delphai_fastapi/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from typing import Optional, List
+from typing import List, Optional
 
 from fastapi_camelcase import CamelModel
 from pydantic import Field
 from datetime import datetime
 
 
 class HTTPExceptionModel(CamelModel):
     detail: str
 
 
+class Label(CamelModel):
+    name: str = Field(description="Assigned label")
+    children: List["Label"] = Field(description="Sublabels")
+
+
 class Location(CamelModel):
     country: Optional[str] = Field(
         description="Company address (country)", example="Germany"
     )
     city: Optional[str] = Field(description="Company address (city)", example="Berlin")
     continent: Optional[str] = Field(
         description="Company address (continent)", example="Europe"
@@ -22,18 +27,31 @@
     )
     latitude: Optional[float] = Field(example=52.5167)
     longitude: Optional[float] = Field(example=13.3833)
     zip_code: Optional[str] = Field(
         description="Company address (ZIP code)", example="10999"
     )
 
+
 class Project(CamelModel):
-    total: int = Field(..., description="Total number of companies in this project", example=35)
-    name:  str = Field(..., description="Name of the project", example="Healthcare | Startups")
+    total: int = Field(
+        ..., description="Total number of companies in this project", example=35
+    )
+    name: str = Field(
+        ..., description="Name of the project", example="Healthcare | Startups"
+    )
     created: datetime = Field(..., description="When the project was created")
-    last_modified: datetime = Field(..., description="When the project was last edited or updated")
-    available: int = Field(..., description="Number of companies in this project that are accessible in the dashboard", example=29)
+    last_modified: datetime = Field(
+        ..., description="When the project was last edited or updated"
+    )
+    available: int = Field(
+        ...,
+        description="Number of companies in this project that are accessible in the dashboard",
+        example=29,
+    )
 
 
-class Source(CamelModel): 
+class Source(CamelModel):
     name: str = Field(description="Name of the source")
-    credibility_score: float = Field(description="Credibility score of source in percentage", example=0.60)
+    credibility_score: float = Field(
+        description="Credibility score of source in percentage", example=0.60
+    )
```

### Comparing `delphai_fastapi-0.1.5/delphai_fastapi/types.py` & `delphai_fastapi-0.1.7/delphai_fastapi/types.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.5/setup.py` & `delphai_fastapi-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['delphai_fastapi', 'delphai_fastapi.companies']
+['delphai_fastapi',
+ 'delphai_fastapi.companies',
+ 'delphai_fastapi.job_posts',
+ 'delphai_fastapi.news_articles']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['delphai-utils[config]>=3,<4',
- 'fastapi-camelcase>=1.0.5,<2.0.0',
- 'fastapi>=0.95,<0.96',
- 'pymongo']
+['delphai-utils[keycloak]>=3,<4',
+ 'fastapi-camelcase>=1,<2',
+ 'fastapi>=0,<1',
+ 'pymongo>=4,<5']
 
 setup_kwargs = {
     'name': 'delphai-fastapi',
-    'version': '0.1.5',
+    'version': '0.1.7',
     'description': 'Package for fastAPI models',
     'long_description': 'None',
     'author': 'Berinike Tech',
     'author_email': 'berinike@delphai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `delphai_fastapi-0.1.5/PKG-INFO` & `delphai_fastapi-0.1.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 0.1.5
+Version: 0.1.7
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: delphai-utils[config] (>=3,<4)
-Requires-Dist: fastapi (>=0.95,<0.96)
-Requires-Dist: fastapi-camelcase (>=1.0.5,<2.0.0)
-Requires-Dist: pymongo
+Requires-Dist: delphai-utils[keycloak] (>=3,<4)
+Requires-Dist: fastapi (>=0,<1)
+Requires-Dist: fastapi-camelcase (>=1,<2)
+Requires-Dist: pymongo (>=4,<5)
```

