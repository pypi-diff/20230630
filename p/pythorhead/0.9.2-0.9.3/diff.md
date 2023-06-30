# Comparing `tmp/pythorhead-0.9.2.tar.gz` & `tmp/pythorhead-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.9.2.tar", last modified: Mon Jun 26 17:35:16 2023, max compression
+gzip compressed data, was "pythorhead-0.9.3.tar", last modified: Thu Jun 29 19:53:55 2023, max compression
```

## Comparing `pythorhead-0.9.2.tar` & `pythorhead-0.9.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.923235 pythorhead-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.923235 pythorhead-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-26 17:34:58.000000 pythorhead-0.9.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-26 17:34:58.000000 pythorhead-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-26 17:35:06.000000 pythorhead-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 17:34:58.000000 pythorhead-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-26 17:35:16.927235 pythorhead-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-26 17:34:58.000000 pythorhead-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/pic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/user.py
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-26 17:34:58.000000 pythorhead-0.9.2/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-26 17:35:06.000000 pythorhead-0.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/community.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:34:58.000000 pythorhead-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:35:16.927235 pythorhead-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:55.456467 pythorhead-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:55.452467 pythorhead-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:55.452467 pythorhead-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-29 19:53:35.000000 pythorhead-0.9.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-29 19:53:35.000000 pythorhead-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-29 19:53:43.000000 pythorhead-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 19:53:35.000000 pythorhead-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-29 19:53:55.456467 pythorhead-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-29 19:53:35.000000 pythorhead-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:55.456467 pythorhead-0.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-29 19:53:35.000000 pythorhead-0.9.3/examples/pic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 19:53:35.000000 pythorhead-0.9.3/examples/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-29 19:53:35.000000 pythorhead-0.9.3/examples/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-29 19:53:35.000000 pythorhead-0.9.3/examples/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-29 19:53:35.000000 pythorhead-0.9.3/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-29 19:53:44.000000 pythorhead-0.9.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:55.456467 pythorhead-0.9.3/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:55.456467 pythorhead-0.9.3/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-29 19:53:35.000000 pythorhead-0.9.3/pythorhead/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:55.456467 pythorhead-0.9.3/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-29 19:53:55.000000 pythorhead-0.9.3/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-29 19:53:55.000000 pythorhead-0.9.3/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:53:55.000000 pythorhead-0.9.3/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 19:53:55.000000 pythorhead-0.9.3/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:53:35.000000 pythorhead-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:53:55.456467 pythorhead-0.9.3/setup.cfg
```

### Comparing `pythorhead-0.9.2/.github/workflows/pypi.yml` & `pythorhead-0.9.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/.gitignore` & `pythorhead-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/CHANGELOG.md` & `pythorhead-0.9.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Changelog
 
+## [Unreleased](https://github.com/db0/pythorhead/tree/HEAD)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.9.3...HEAD)
+
+**Fixed bugs:**
+
+- Create community broken [\#35](https://github.com/db0/pythorhead/issues/35)
+
+## [v0.9.3](https://github.com/db0/pythorhead/tree/v0.9.3) (2023-06-29)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.9.2...v0.9.3)
+
+**Merged pull requests:**
+
+- fix create community [\#36](https://github.com/db0/pythorhead/pull/36) ([NicKoehler](https://github.com/NicKoehler))
+- Remove logging.basicConfig statement [\#32](https://github.com/db0/pythorhead/pull/32) ([hjalp](https://github.com/hjalp))
+
 ## [v0.9.2](https://github.com/db0/pythorhead/tree/v0.9.2) (2023-06-26)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.9.1...v0.9.2)
 
 **Closed issues:**
 
 - Changelog [\#27](https://github.com/db0/pythorhead/issues/27)
```

### Comparing `pythorhead-0.9.2/LICENSE` & `pythorhead-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/PKG-INFO` & `pythorhead-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.9.2/README.md` & `pythorhead-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/examples/pic.py` & `pythorhead-0.9.3/examples/pic.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 lemmy_password = args.lemmy_password
 if not lemmy_password:
     lemmy_password = os.getenv("LEMMY_PASSWORD")
 if not lemmy_password:
     raise Exception("You need to provide a lemmy password via env var or arg")
 
-lemmy = Lemmy(f"https://{lemmy_domain}")
+lemmy = Lemmy(f"http://{lemmy_domain}")
 if not lemmy.log_in(lemmy_username, lemmy_password):
     print("Failed to log in")
     exit(1)
 
 community_id = lemmy.discover_community(args.community)
 
 if not community_id:
```

### Comparing `pythorhead-0.9.2/examples/pm.py` & `pythorhead-0.9.3/examples/pm.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/examples/site.py` & `pythorhead-0.9.3/examples/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/examples/user.py` & `pythorhead-0.9.3/examples/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/logo.png` & `pythorhead-0.9.3/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pyproject.toml` & `pythorhead-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.9.2"
+version = "v0.9.3"
 readme = "README.md"
 requires-python = ">=3.8,<3.12"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.9.2/pythorhead/comment.py` & `pythorhead-0.9.3/pythorhead/comment.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pythorhead/community.py` & `pythorhead-0.9.3/pythorhead/community.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from pythorhead.requestor import Request, Requestor
 from pythorhead.types import ListingType, SortType
 
 
 class Community:
     def __init__(self, _requestor: Requestor):
@@ -27,28 +27,28 @@
             icon (str, optional): Defaults to None
             nsfw (bool, optional): Defaults to None
             posting_restricted_to_mods (bool, optional): Defaults to None
 
         Returns:
             Optional[dict]: post data if successful
         """
-        new_community: dict = {
+        new_community: dict[Any, Any] = {
             "name": name,
             "title": title,
         }
         if description is not None:
             new_community["description"] = description
         if icon is not None:
             new_community["icon"] = icon
         if nsfw is not None:
             new_community["nsfw"] = nsfw
         if [posting_restricted_to_mods] is not None:
             new_community["[posting_restricted_to_mods]"] = [posting_restricted_to_mods]
 
-        return self._requestor.api(Request.POST, "/post", json=new_community)
+        return self._requestor.api(Request.POST, "/community", json=new_community)
 
     def get(self, id: Optional[int] = None, name: Optional[str] = None) -> Optional[dict]:
         """
         Get a community by id or name
 
         Args:
             id (Optional[int]): Defaults to None
```

### Comparing `pythorhead-0.9.2/pythorhead/image.py` & `pythorhead-0.9.3/pythorhead/image.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pythorhead/lemmy.py` & `pythorhead-0.9.3/pythorhead/lemmy.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from pythorhead.image import Image
 from pythorhead.post import Post
 from pythorhead.private_message import PrivateMessage
 from pythorhead.requestor import Requestor
 from pythorhead.site import Site
 from pythorhead.user import User
 
-logging.basicConfig(format="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-
 
 class Lemmy:
     _known_communities = {}
     _requestor: Requestor
 
     def __init__(self, api_base_url: str) -> None:
         self._requestor = Requestor()
```

### Comparing `pythorhead-0.9.2/pythorhead/post.py` & `pythorhead-0.9.3/pythorhead/post.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pythorhead/private_message.py` & `pythorhead-0.9.3/pythorhead/private_message.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pythorhead/requestor.py` & `pythorhead-0.9.3/pythorhead/requestor.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pythorhead/site.py` & `pythorhead-0.9.3/pythorhead/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pythorhead/user.py` & `pythorhead-0.9.3/pythorhead/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.2/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.9.3/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.9.2/pythorhead.egg-info/SOURCES.txt` & `pythorhead-0.9.3/pythorhead.egg-info/SOURCES.txt`

 * *Files identical despite different names*

