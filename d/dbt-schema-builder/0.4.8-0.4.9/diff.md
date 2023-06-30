# Comparing `tmp/dbt-schema-builder-0.4.8.tar.gz` & `tmp/dbt-schema-builder-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-schema-builder-0.4.8.tar", last modified: Mon Jun  5 17:19:18 2023, max compression
+gzip compressed data, was "dbt-schema-builder-0.4.9.tar", last modified: Fri Jun 30 15:56:49 2023, max compression
```

## Comparing `dbt-schema-builder-0.4.8.tar` & `dbt-schema-builder-0.4.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4022 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.814346 dbt-schema-builder-0.4.8/dbt_schema_builder/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/app.py
--rw-r--r--   0 runner    (1001) docker     (122)    24281 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)     9373 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/relation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3904 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/schema_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/snowflake_keywords.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/dbt_schema_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_pii.tpl
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_safe.tpl
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.814346 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5314 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:56:49.413990 dbt-schema-builder-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-30 15:56:49.413990 dbt-schema-builder-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4022 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:56:49.409990 dbt-schema-builder-0.4.9/dbt_schema_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7826 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24597 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11003 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/relation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4073 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/schema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/snowflake_keywords.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:56:49.409990 dbt-schema-builder-0.4.9/dbt_schema_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/templates/model_sql_pii.tpl
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/dbt_schema_builder/templates/model_sql_safe.tpl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:56:49.409990 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-30 15:56:49.000000 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-30 15:56:49.000000 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 15:56:49.000000 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-30 15:56:49.000000 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 15:56:49.000000 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-30 15:56:49.000000 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-30 15:56:49.000000 dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:56:49.409990 dbt-schema-builder-0.4.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-30 15:56:49.413990 dbt-schema-builder-0.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5314 2023-06-30 15:56:44.000000 dbt-schema-builder-0.4.9/setup.py
```

### Comparing `dbt-schema-builder-0.4.8/LICENSE.txt` & `dbt-schema-builder-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/PKG-INFO` & `dbt-schema-builder-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.8
+Version: 0.4.9
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.8/README.rst` & `dbt-schema-builder-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/app.py` & `dbt-schema-builder-0.4.9/dbt_schema_builder/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,36 @@
 
     def __repr__(self):
         """
         Makes debugging less of a pain
         """
         return self.app
 
+    def check_downstream_sources_for_dupes(self):
+        """
+        Checks downstream sources for duplicate tables within the same schema.
+        """
+        table_dict = {}
+        for source in self.new_downstream_sources["sources"]:
+            table_dict[source["name"]] = []
+            for table in source["tables"]:
+                table_dict[source["name"]].append(table["name"])
+
+        seen = set()
+        dupes = []
+        for schema, table_list in table_dict.items():
+            for table_ in table_list:
+                qualified_table_name = schema + '.' + table_
+                if qualified_table_name in seen:
+                    dupes.append(qualified_table_name)
+                else:
+                    seen.add(qualified_table_name)
+
+        return dupes
+
     def add_source_to_new_schema(self, current_raw_source, relation, source_database, raw_schema):
         """
         Add our table to the appropriate raw schema entry in our "sources" list
         in the new schema.
         """
         for index, item in enumerate(self.new_schema["sources"]):
             if item['name'] == raw_schema.schema_name:
@@ -118,17 +140,17 @@
                 (
                     "{}.{} is absent from the downstream sources allow_list, "
                     "skipping inclusion as a source in downstream project."
                 ).format(relation.app, relation.relation)
             )
         elif current_safe_source:
             for source in self.new_downstream_sources["sources"]:
-                if source["name"] == self.safe_downstream_source_name:
+                if current_safe_source and source["name"] == self.safe_downstream_source_name:
                     source["tables"].append(current_safe_source)
-                elif source["name"] == self.pii_downstream_source_name:
+                elif current_pii_source and source["name"] == self.pii_downstream_source_name:
                     source["tables"].append(current_pii_source)
         else:
             for source in self.new_downstream_sources["sources"]:
                 if source["name"] == self.safe_downstream_source_name:
                     source["tables"].append(
                         {
                             "name": relation.relation,
```

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/builder.py` & `dbt-schema-builder-0.4.9/dbt_schema_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     @staticmethod
     def validate_schema_config(config):
         """
         Read through an app-schema config dict, making sure that it meets certain
         expectations before proceeding. If not, raise an exception to prevent
         invalid schemas from being built
         """
-        valid_keys = ['EXCLUDE', 'INCLUDE', 'SOFT_DELETE']
+        valid_keys = ['EXCLUDE', 'INCLUDE', 'SOFT_DELETE', 'PREFIX']
         database_schema_pattern = re.compile(r'^[A-Za-z0-9_$]+\.[A-Za-z0-9_$]+$')
         for destination_schema, destination_schema_config in config.items():
             if not re.search(database_schema_pattern, destination_schema):
                 raise InvalidConfigurationException(
                     "Invalid destination schema path in schema_config.yml. "
                     "These must be in the format <DATABASE_NAME>.<SCHEMA_NAME>. "
                     "Found {}".format(destination_schema)
@@ -515,15 +515,15 @@
             )
             raw_schema_relations = self.get_relations(app_source_database, app_source_schema)
             for source_relation_name, meta_data in raw_schema_relations[app_source_schema].items():
                 relation = Relation(
                     source_relation_name, meta_data, app_destination_schema,
                     app_path, self.snowflake_keywords,
                     self.unmanaged_tables, self.redactions,
-                    self.downstream_sources_allow_list
+                    self.downstream_sources_allow_list, prefix=raw_schema.prefix
                 )
                 raw_schema.relations.append(relation)
             app_raw_schemas.append(raw_schema)
 
         app_object = App(
             app_raw_schemas, app_destination_schema, app_path, design_file_path, current_raw_sources,
             current_downstream_sources, app_destination_database, no_pii
@@ -547,26 +547,29 @@
                 (
                     current_raw_source,
                     current_safe_source,
                     current_pii_source,
                 ) = relation.find_in_current_sources(
                     current_raw_sources,
                     current_downstream_sources,
+                    prefix=raw_schema.prefix
                 )
-
                 app_object.add_source_to_new_schema(current_raw_source, relation, app_source_database, raw_schema)
                 app_object.add_table_to_downstream_sources(relation, current_safe_source, current_pii_source)
                 app_object.update_trifecta_models(relation, no_pii=no_pii)
 
                 ##############################
                 # Write out dbt models which are responsible for generating the views
                 ##############################
                 relation.write_sql(raw_schema, no_pii=no_pii)
         app_object.write_app_schema(design_file_path)
-
+        # Check downstream source tables for duplicate table names and log if so
+        dupes = app_object.check_downstream_sources_for_dupes()
+        if dupes:
+            logger.error("Duplicate table names found: {}".format(dupes))
         # Create source definitions pertaining to app database views in the downstream dbt
         # project, i.e. reporting.
         self.write_sources_for_downstream_project(
             downstream_sources_file_path,
             yaml.safe_dump(app_object.new_downstream_sources, sort_keys=False),
         )
```

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/queries.py` & `dbt-schema-builder-0.4.9/dbt_schema_builder/queries.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/relation.py` & `dbt-schema-builder-0.4.9/dbt_schema_builder/relation.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 class Relation:
     """
     Class to represent a DBT relation (a table/view)
     """
 
     def __init__(
         self, source_relation_name, meta_data, app, app_path,
-        snowflake_keywords, unmanaged_tables, redactions, downstream_sources_allow_list
+        snowflake_keywords, unmanaged_tables, redactions, downstream_sources_allow_list, prefix=None
     ):
         self.snowflake_keywords = snowflake_keywords
         self.redactions = redactions
-
+        self.prefix = prefix
         self.source_relation_name = source_relation_name
         self.relation = self._get_model_name_alias()
         self.new_safe_relation_name = "{}_{}".format(app, self.relation)
         self.new_pii_relation_name = "{}_PII_{}".format(app, self.relation)
 
         self.meta_data = meta_data
 
@@ -42,16 +42,21 @@
         self.unmanaged_tables = unmanaged_tables
         self.downstream_sources_allow_list = downstream_sources_allow_list
 
     def __repr__(self):
         return self.source_relation_name
 
     def _get_model_name_alias(self):
-        if self.source_relation_name in self.snowflake_keywords:
+        """
+        Get alias after parsing source relation name.
+        """
+        if not self.prefix and self.source_relation_name in self.snowflake_keywords:
             return "_{}".format(self.source_relation_name)
+        elif self.prefix:
+            return self.prefix + '_' + self.source_relation_name
         else:
             return self.source_relation_name
 
     def prep_meta_data(self):
         """
         Transforms the data we receive back from Snowflake / dbt to a more usable form.
         """
@@ -67,15 +72,15 @@
             "description": DEFAULT_DESCRIPTION,
             "columns": columns,
         }
 
         return model
 
     def find_in_current_sources(
-        self, current_raw_sources, current_downstream_sources
+        self, current_raw_sources, current_downstream_sources, prefix=None
     ):
         """
         Find source data in an existing loaded schema yml file.
 
         If a file already exists for this schema, find the values for the current relation
         so we can preserve any manual modifications (tests, description, etc.).
         """
@@ -93,19 +98,35 @@
                         current_raw_source = table
                         break
 
         if current_downstream_sources and "sources" in current_downstream_sources:
             for source in current_downstream_sources["sources"]:
                 if source["name"] == self.app:
                     for table in source["tables"]:
-                        if table and table["name"] == self.source_relation_name:
+                        if table and prefix and table["name"] == self.source_relation_name:
+                            # Handle prefix when no prefix has been applied already from prior runs
+                            table["name"] = prefix + '_' + table["name"]
+                            current_safe_downstream_source = table
+                        elif table and table["name"] == self.source_relation_name:
+                            # No prefix already applied, no prefix to be applied
+                            current_safe_downstream_source = table
+                        elif prefix and table and table["name"] == prefix + '_' + self.source_relation_name:
+                            # Handle prefix when already applied from prior runs
                             current_safe_downstream_source = table
                 elif source["name"] == "{}_PII".format(self.app):
                     for table in source["tables"]:
-                        if table and table["name"] == self.source_relation_name:
+                        if table and prefix and table["name"] == self.source_relation_name:
+                            # Handle prefix for PII schema when no prefix has been applied already from prior runs
+                            table["name"] = prefix + '_' + table["name"]
+                            current_pii_downstream_source = table
+                        elif table and table["name"] == self.source_relation_name:
+                            # No prefix already applied, no prefix to be applied for PII schema
+                            current_pii_downstream_source = table
+                        elif prefix and table and table["name"] == prefix + '_' + self.source_relation_name:
+                            # Handle prefix for PII schema when already applied from prior runs
                             current_pii_downstream_source = table
 
                 if current_safe_downstream_source and current_pii_downstream_source:
                     break
 
         return (
             current_raw_source,
```

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/schema.py` & `dbt-schema-builder-0.4.9/dbt_schema_builder/schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 class Schema:
     """
     Class to represent a raw Schema used to back an application schema
     """
 
     def __init__(self, schema_name, exclusion_list, inclusion_list, soft_delete_column_name,
-                 soft_delete_sql_predicate, relations=None):
+                 soft_delete_sql_predicate, relations=None, prefix=None):
         self.schema_name = schema_name
         self.exclusion_list = exclusion_list
         self.inclusion_list = inclusion_list
         self.soft_delete_column_name = soft_delete_column_name
         self.soft_delete_sql_predicate = soft_delete_sql_predicate
         self.relations = relations
+        self.prefix = prefix
 
         self.validate()
 
     def __repr__(self):
         return self.schema_name
 
     def validate(self):
@@ -48,31 +49,36 @@
         builder.py.
         TODO: add code to parse out un-managed table configs here
         """
         exclusion_list = []
         inclusion_list = []
         soft_delete_column_name = None
         soft_delete_sql_predicate = None
+        prefix = None
 
         if config:
             exclusion_list = config.get('EXCLUDE', [])
             inclusion_list = config.get('INCLUDE', [])
 
             if 'SOFT_DELETE' in config:
                 for k, v in config['SOFT_DELETE'].items():
                     soft_delete_column_name = k
                     soft_delete_sql_predicate = v
 
+            if 'PREFIX' in config:
+                prefix = config['PREFIX']
+
         schema = Schema(
             schema_name,
             exclusion_list,
             inclusion_list,
             soft_delete_column_name,
             soft_delete_sql_predicate,
-            relations=[]
+            relations=[],
+            prefix=prefix
         )
         return schema
 
     def filter_relations(self):
         """
         Filter the relations in this Schema, based upon the exclusion and
         inclusion lists.
```

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/schema_builder.py` & `dbt-schema-builder-0.4.9/dbt_schema_builder/schema_builder.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/snowflake_keywords.yml` & `dbt-schema-builder-0.4.9/dbt_schema_builder/snowflake_keywords.yml`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_pii.tpl` & `dbt-schema-builder-0.4.9/dbt_schema_builder/templates/model_sql_pii.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_safe.tpl` & `dbt-schema-builder-0.4.9/dbt_schema_builder/templates/model_sql_safe.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/PKG-INFO` & `dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.8
+Version: 0.4.9
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/SOURCES.txt` & `dbt-schema-builder-0.4.9/dbt_schema_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/requirements/constraints.txt` & `dbt-schema-builder-0.4.9/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.8/setup.py` & `dbt-schema-builder-0.4.9/setup.py`

 * *Files identical despite different names*

