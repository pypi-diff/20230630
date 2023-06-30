# Comparing `tmp/pepdbagent-0.4.2.tar.gz` & `tmp/pepdbagent-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.4.2.tar", last modified: Tue Jun 27 16:01:41 2023, max compression
+gzip compressed data, was "pepdbagent-0.4.3.tar", last modified: Fri Jun 30 21:55:04 2023, max compression
```

## Comparing `pepdbagent-0.4.2.tar` & `pepdbagent-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 16:01:41.000000 pepdbagent-0.4.2/pepdbagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:41.737535 pepdbagent-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-27 16:01:25.000000 pepdbagent-0.4.2/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.4.2/LICENSE.txt` & `pepdbagent-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/PKG-INFO` & `pepdbagent-0.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.4.2/README.md` & `pepdbagent-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/pepdbagent/db_utils.py` & `pepdbagent-0.4.3/pepdbagent/db_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,22 +55,32 @@
     """
     if tables:
         _LOGGER.info("A table was created")
     else:
         _LOGGER.info("A table was not created")
 
 
+def deliver_description(context):
+    try:
+        return context.get_current_parameters()["project_value"]["_config"]["description"]
+    except KeyError:
+        return ""
+
+
 class Projects(Base):
     __tablename__ = "projects"
 
     id: Mapped[int] = mapped_column(BIGSERIAL, server_default=FetchedValue())
     namespace: Mapped[str] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column(primary_key=True)
     tag: Mapped[str] = mapped_column(primary_key=True)
     digest: Mapped[str] = mapped_column(String(32))
+    description: Mapped[Optional[str]] = mapped_column(
+        default=deliver_description, onupdate=deliver_description
+    )
     project_value: Mapped[dict] = mapped_column(JSON, server_default=FetchedValue())
     private: Mapped[bool]
     number_of_samples: Mapped[int]
     submission_date: Mapped[datetime.datetime]
     last_update_date: Mapped[datetime.datetime]
     pep_schema: Mapped[Optional[str]]
```

### Comparing `pepdbagent-0.4.2/pepdbagent/exceptions.py` & `pepdbagent-0.4.3/pepdbagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/pepdbagent/models.py` & `pepdbagent-0.4.3/pepdbagent/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     name: Optional[str] = None
     tag: Optional[str] = None
     private: Optional[bool] = Field(alias="is_private")
     digest: Optional[str]
     last_update_date: Optional[datetime.datetime]
     number_of_samples: Optional[int]
     pep_schema: Optional[str]
+    description: Optional[str]
 
     @validator("tag", "name")
     def value_must_not_be_empty(cls, v):
         if "" == v:
             return None
         return v
```

### Comparing `pepdbagent-0.4.2/pepdbagent/modules/annotation.py` & `pepdbagent-0.4.3/pepdbagent/modules/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         admin_tuple = tuple_converter(admin)
 
         statement = select(
             Projects.namespace,
             Projects.name,
             Projects.tag,
             Projects.private,
-            Projects.project_value["description"].astext.label("description"),
+            Projects.description,
             Projects.number_of_samples,
             Projects.submission_date,
             Projects.last_update_date,
             Projects.digest,
             Projects.pep_schema,
         ).where(
             and_(
@@ -252,15 +252,15 @@
         if admin is None:
             admin = []
         statement = select(
             Projects.namespace,
             Projects.name,
             Projects.tag,
             Projects.private,
-            Projects.project_value["description"].astext.label("description"),
+            Projects.description,
             Projects.number_of_samples,
             Projects.submission_date,
             Projects.last_update_date,
             Projects.digest,
             Projects.pep_schema,
         ).select_from(Projects)
 
@@ -345,14 +345,15 @@
         """
         admin_list = tuple_converter(admin_list)
         if search_str:
             sql_search_str = f"%{search_str}%"
             search_query = or_(
                 Projects.name.ilike(sql_search_str),
                 Projects.tag.ilike(sql_search_str),
+                Projects.description.ilike(sql_search_str),
             )
             statement = statement.where(search_query)
         if namespace:
             statement = statement.where(Projects.namespace == namespace)
 
         statement = statement.where(
             or_(Projects.private.is_(False), Projects.namespace.in_(admin_list))
```

### Comparing `pepdbagent-0.4.2/pepdbagent/modules/namespace.py` & `pepdbagent-0.4.3/pepdbagent/modules/namespace.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/pepdbagent/modules/project.py` & `pepdbagent-0.4.3/pepdbagent/modules/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 
     def create(
         self,
         project: peppy.Project,
         namespace: str,
         name: str = None,
         tag: str = DEFAULT_TAG,
+        description: str = None,
         is_private: bool = False,
         pep_schema: str = None,
         overwrite: bool = False,
         update_only: bool = False,
     ) -> None:
         """
         Upload project to the database.
@@ -183,27 +184,29 @@
         :param name: name of the project (Default: name is taken from the project object)
         :param tag: tag (or version) of the project.
         :param is_private: boolean value if the project should be visible just for user that creates it.
         :param pep_schema: assign PEP to a specific schema. [DefaultL: None]
         :param overwrite: if project exists overwrite the project, otherwise upload it.
             [Default: False - project won't be overwritten if it exists in db]
         :param update_only: if project exists overwrite it, otherwise do nothing.  [Default: False]
+        :param description: description of the project
         :return: None
         """
-        proj_dict = project.to_dict(extended=True)
-        proj_dict["_config"]["description"] = project.description
+        proj_dict = project.to_dict(extended=True, orient="records")
+        if not description:
+            description = project.description
+        proj_dict["_config"]["description"] = description
 
         namespace = namespace.lower()
         if name:
             name = name.lower()
             proj_name = name
-            proj_dict["name"] = name
             proj_dict["_config"]["name"] = project.name
-        elif proj_dict["name"]:
-            proj_name = proj_dict["name"].lower()
+        elif proj_dict["_config"]["name"]:
+            proj_name = proj_dict["_config"]["name"].lower()
         else:
             raise ValueError(f"Name of the project wasn't provided. Project will not be uploaded.")
 
         proj_digest = create_digest(proj_dict)
         number_of_samples = len(project.samples)
 
         if update_only:
@@ -332,15 +335,14 @@
         :param update_dict: dict with update key->values. Dict structure:
             {
                     project: Optional[peppy.Project]
                     is_private: Optional[bool]
                     tag: Optional[str]
                     name: Optional[str]
             }
-            *project_value should contain name and description
         :param namespace: project namespace
         :param name: project name
         :param tag: project tag
         :return: None
         """
         if self.exists(namespace=namespace, name=name, tag=tag):
             if isinstance(update_dict, UpdateItems):
@@ -379,21 +381,21 @@
          :param update_values: UpdateItems (pydantic class) with
             updating values
         :return: unified update dict
         """
         update_final = UpdateModel()
 
         if update_values.project_value is not None:
-            proj_dict = update_values.project_value.to_dict(extended=True)
-            proj_dict["_config"]["description"] = proj_dict["description"]
-            proj_dict["_config"]["name"] = proj_dict["name"]
+            proj_dict = update_values.project_value.to_dict(extended=True, orient="records")
             update_final = UpdateModel(
                 project_value=proj_dict,
                 name=update_values.project_value.name,
-                digest=create_digest(update_values.project_value.to_dict(extended=True)),
+                digest=create_digest(
+                    update_values.project_value.to_dict(extended=True, orient="records")
+                ),
                 last_update_date=datetime.datetime.now(datetime.timezone.utc),
                 number_of_samples=len(update_values.project_value.samples),
             )
 
         if update_values.tag is not None:
             update_final = UpdateModel(
                 tag=update_values.tag, **update_final.dict(exclude_unset=True)
```

### Comparing `pepdbagent-0.4.2/pepdbagent/pepdbagent.py` & `pepdbagent-0.4.3/pepdbagent/pepdbagent.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/pepdbagent/utils.py` & `pepdbagent-0.4.3/pepdbagent/utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.4.3/pepdbagent.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.4.2/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.4.3/pepdbagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/setup.py` & `pepdbagent-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/tests/conftest.py` & `pepdbagent-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.2/tests/test_pepagent.py` & `pepdbagent-0.4.3/tests/test_pepagent.py`

 * *Files identical despite different names*

