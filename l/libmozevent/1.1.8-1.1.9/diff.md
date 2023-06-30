# Comparing `tmp/libmozevent-1.1.8.tar.gz` & `tmp/libmozevent-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libmozevent-1.1.8.tar", last modified: Wed Jul 14 09:38:12 2021, max compression
+gzip compressed data, was "dist/libmozevent-1.1.9.tar", last modified: Fri Jul 16 15:01:11 2021, max compression
```

## Comparing `libmozevent-1.1.8.tar` & `libmozevent-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-14 09:38:12.000000 libmozevent-1.1.8/
--rw-r--r--   0 root         (0) root         (0)      309 2021-07-14 09:38:12.000000 libmozevent-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      224 2021-07-14 09:38:11.000000 libmozevent-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-14 09:38:12.000000 libmozevent-1.1.8/libmozevent/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4920 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/bus.py
--rw-r--r--   0 root         (0) root         (0)     3484 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/log.py
--rw-r--r--   0 root         (0) root         (0)    13931 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/mercurial.py
--rw-r--r--   0 root         (0) root         (0)     6587 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     6329 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/phabricator.py
--rw-r--r--   0 root         (0) root         (0)     6402 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/pulse.py
--rw-r--r--   0 root         (0) root         (0)     1503 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/storage.py
--rw-r--r--   0 root         (0) root         (0)     4408 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/utils.py
--rw-r--r--   0 root         (0) root         (0)     2293 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-14 09:38:12.000000 libmozevent-1.1.8/libmozevent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      309 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      450 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      116 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-07-14 09:38:11.000000 libmozevent-1.1.8/libmozevent.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-14 09:38:12.000000 libmozevent-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1550 2021-07-14 09:38:11.000000 libmozevent-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 15:01:11.000000 libmozevent-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      309 2021-07-16 15:01:11.000000 libmozevent-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      224 2021-07-16 15:01:11.000000 libmozevent-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4920 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/bus.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/log.py
+-rw-r--r--   0 root         (0) root         (0)    14243 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/mercurial.py
+-rw-r--r--   0 root         (0) root         (0)     6587 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/phabricator.py
+-rw-r--r--   0 root         (0) root         (0)     6402 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/pulse.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/storage.py
+-rw-r--r--   0 root         (0) root         (0)     4408 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      309 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      450 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      116 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2021-07-16 15:01:11.000000 libmozevent-1.1.9/libmozevent.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-07-16 15:01:11.000000 libmozevent-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1550 2021-07-16 15:01:11.000000 libmozevent-1.1.9/setup.py
```

### Comparing `libmozevent-1.1.8/libmozevent/bus.py` & `libmozevent-1.1.9/libmozevent/bus.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/libmozevent/log.py` & `libmozevent-1.1.9/libmozevent/log.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/libmozevent/mercurial.py` & `libmozevent-1.1.9/libmozevent/mercurial.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,32 +147,37 @@
             )
             hg_base = self.default_revision
 
         # Update the repo to base revision
         try:
             logger.info("Updating repo to revision {}".format(hg_base))
             self.repo.update(rev=hg_base, clean=True)
+
+            # See if the repo is clean
+            repo_status = self.repo.status(
+                modified=True, added=True, removed=True, deleted=True
+            )
+            if len(repo_status) != 0:
+                logger.warn(
+                    "Repo is dirty! Let's clean it first.",
+                    revision=hg_base,
+                    repo=self.name,
+                    repo_status=repo_status,
+                )
+                # Clean the repo - This is a workaround for Bug 1720302
+                self.repo.update(rev="null", clean=True)
+                # Redo the update to the correct revision
+                self.repo.update(rev=hg_base, clean=True)
+
         except hglib.error.CommandError:
             raise Exception("Failed to update to revision {}".format(hg_base))
 
         # In this case revision is `hg_base`
         logger.info("Updated repo", revision=hg_base, repo=self.name)
 
-        # See if the repo is clean
-        repo_status = self.repo.status(
-            modified=True, added=True, removed=True, deleted=True
-        )
-        if len(repo_status) != 0:
-            logger.warn(
-                "Repo is dirty!",
-                revision=hg_base,
-                repo=self.name,
-                repo_status=repo_status,
-            )
-
         def get_author(commit):
             """Helper to build a mercurial author from Phabricator data"""
             author = commit.get("author")
             if author is None:
                 return DEFAULT_AUTHOR
             if author["name"] and author["email"]:
                 # Build clean version without quotes
```

### Comparing `libmozevent-1.1.8/libmozevent/monitoring.py` & `libmozevent-1.1.9/libmozevent/monitoring.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/libmozevent/phabricator.py` & `libmozevent-1.1.9/libmozevent/phabricator.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/libmozevent/pulse.py` & `libmozevent-1.1.9/libmozevent/pulse.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/libmozevent/storage.py` & `libmozevent-1.1.9/libmozevent/storage.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/libmozevent/utils.py` & `libmozevent-1.1.9/libmozevent/utils.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/libmozevent/web.py` & `libmozevent-1.1.9/libmozevent/web.py`

 * *Files identical despite different names*

### Comparing `libmozevent-1.1.8/setup.py` & `libmozevent-1.1.9/setup.py`

 * *Files identical despite different names*

