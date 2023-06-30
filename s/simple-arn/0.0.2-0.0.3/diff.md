# Comparing `tmp/simple_arn-0.0.2.tar.gz` & `tmp/simple_arn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_arn-0.0.2.tar", last modified: Thu Jun 22 17:07:55 2023, max compression
+gzip compressed data, was "simple_arn-0.0.3.tar", last modified: Fri Jun 30 18:25:20 2023, max compression
```

## Comparing `simple_arn-0.0.2.tar` & `simple_arn-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 17:07:55.257315 simple_arn-0.0.2/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1055 2023-06-22 15:35:52.000000 simple_arn-0.0.2/LICENSE.md
--rw-rw-r--   0 eric      (1000) eric      (1000)     1785 2023-06-22 17:07:55.257315 simple_arn-0.0.2/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1470 2023-06-22 17:05:50.000000 simple_arn-0.0.2/README.md
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-22 17:07:55.257315 simple_arn-0.0.2/setup.cfg
--rw-rw-r--   0 eric      (1000) eric      (1000)      668 2023-06-22 17:06:58.000000 simple_arn-0.0.2/setup.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 17:07:55.257315 simple_arn-0.0.2/simple_arn/
--rw-rw-r--   0 eric      (1000) eric      (1000)       61 2023-06-22 17:05:38.000000 simple_arn-0.0.2/simple_arn/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     3250 2023-06-22 16:54:31.000000 simple_arn-0.0.2/simple_arn/simple_arn.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 17:07:55.257315 simple_arn-0.0.2/simple_arn.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1785 2023-06-22 17:07:55.000000 simple_arn-0.0.2/simple_arn.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)      213 2023-06-22 17:07:55.000000 simple_arn-0.0.2/simple_arn.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-22 17:07:55.000000 simple_arn-0.0.2/simple_arn.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       11 2023-06-22 17:07:55.000000 simple_arn-0.0.2/simple_arn.egg-info/top_level.txt
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-30 18:25:20.752740 simple_arn-0.0.3/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1055 2023-06-22 15:35:52.000000 simple_arn-0.0.3/LICENSE.md
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1785 2023-06-30 18:25:20.752740 simple_arn-0.0.3/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1470 2023-06-22 17:05:50.000000 simple_arn-0.0.3/README.md
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-30 18:25:20.752740 simple_arn-0.0.3/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)      668 2023-06-30 18:23:29.000000 simple_arn-0.0.3/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-30 18:25:20.752740 simple_arn-0.0.3/simple_arn/
+-rw-rw-r--   0 eric      (1000) eric      (1000)       61 2023-06-22 17:05:38.000000 simple_arn-0.0.3/simple_arn/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     3265 2023-06-30 18:23:14.000000 simple_arn-0.0.3/simple_arn/simple_arn.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-30 18:25:20.752740 simple_arn-0.0.3/simple_arn.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1785 2023-06-30 18:25:20.000000 simple_arn-0.0.3/simple_arn.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      213 2023-06-30 18:25:20.000000 simple_arn-0.0.3/simple_arn.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-30 18:25:20.000000 simple_arn-0.0.3/simple_arn.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       11 2023-06-30 18:25:20.000000 simple_arn-0.0.3/simple_arn.egg-info/top_level.txt
```

### Comparing `simple_arn-0.0.2/LICENSE.md` & `simple_arn-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `simple_arn-0.0.2/PKG-INFO` & `simple_arn-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_arn
-Version: 0.0.2
+Version: 0.0.3
 Summary: simple AWS arn parsing and serialization
 Home-page: https://github.com/ericmaustin/aws_arn
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `simple_arn-0.0.2/README.md` & `simple_arn-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_arn-0.0.2/setup.py` & `simple_arn-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,12 +12,12 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Eric Austin",
     url="https://github.com/ericmaustin/aws_arn",
     license="MIT",
     author_email="eric.m.austin@gmail.com",
     python_requires=">=3.7",
-    version="0.0.2",
+    version="0.0.3",
     include_package_data=True,
     packages=find_packages(),
     install_requires=[]
 )
```

### Comparing `simple_arn-0.0.2/simple_arn/simple_arn.py` & `simple_arn-0.0.3/simple_arn/simple_arn.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,42 +21,40 @@
     service: str
     region: Optional[str]
     account_id: Optional[str]
     resource: str
     resource_type: Optional[str] = None
     resource_id: Optional[str] = None
 
-    def update(self, **kwargs) -> AwsArn:
-        for k, v in kwargs.items():
-            self.__setattr__(k, v)
-        return self
-
     def clone(
             self,
             partition: Optional[str] = None,
             service: Optional[str] = None,
             region: Optional[str] = None,
             account_id: Optional[str] = None,
             resource: Optional[str] = None,
-            resource_type: Optional[str] = None,
-            resource_id: Optional[str] = None,
     ) -> AwsArn:
         """
         Clone the AwsArn object with optional new values
         :return: a new AwsArn object
         """
-        return AwsArn(
-            partition=partition or self.partition,
-            service=service or self.service,
-            region=region or self.region,
-            account_id=account_id or self.account_id,
-            resource=resource or self.resource,
-            resource_type=resource_type or self.resource_type,
-            resource_id=resource_id or self.resource_id,
-        )
+        resource_type, resource_id = None, None
+        if resource:
+            resource_type, resource_id = _parse_resource(resource)
+
+        return AwsArn(**{k: v if v is not None else getattr(self, k) for k, v in
+                         dict(
+                             partition=partition,
+                             service=service,
+                             region=region,
+                             account_id=account_id,
+                             resource=resource,
+                             resource_type=resource_type,
+                             resource_id=resource_id,
+                         ).items()})
 
     def __str__(self):
         return f"arn:{self.partition}:{self.service}:{self.region}:{self.account_id}:{self.resource}"
 
     @classmethod
     def parse(cls, arn: str) -> AwsArn:
         return parse_arn(arn)
```

### Comparing `simple_arn-0.0.2/simple_arn.egg-info/PKG-INFO` & `simple_arn-0.0.3/simple_arn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-arn
-Version: 0.0.2
+Version: 0.0.3
 Summary: simple AWS arn parsing and serialization
 Home-page: https://github.com/ericmaustin/aws_arn
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

