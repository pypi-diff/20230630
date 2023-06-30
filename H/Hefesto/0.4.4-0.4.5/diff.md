# Comparing `tmp/Hefesto-0.4.4.tar.gz` & `tmp/Hefesto-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.4.4.tar", last modified: Mon Jun 19 07:30:01 2023, max compression
+gzip compressed data, was "Hefesto-0.4.5.tar", last modified: Fri Jun 30 05:47:51 2023, max compression
```

## Comparing `Hefesto-0.4.4.tar` & `Hefesto-0.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-19 07:30:01.926707 Hefesto-0.4.4/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-19 07:30:01.926707 Hefesto-0.4.4/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.4/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12035 2023-06-19 07:29:08.000000 Hefesto-0.4.4/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     6781 2023-06-18 17:57:59.000000 Hefesto-0.4.4/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-19 07:30:01.926707 Hefesto-0.4.4/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.4/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-19 07:30:01.926707 Hefesto-0.4.4/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.4/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.4/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-06-19 07:30:01.926707 Hefesto-0.4.4/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-06-19 07:29:40.000000 Hefesto-0.4.4/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-30 05:47:51.953725 Hefesto-0.4.5/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-30 05:47:51.953725 Hefesto-0.4.5/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.5/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12391 2023-06-28 12:39:32.000000 Hefesto-0.4.5/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    17203 2023-06-27 12:31:17.000000 Hefesto-0.4.5/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-30 05:47:51.953725 Hefesto-0.4.5/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.5/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-30 05:47:51.953725 Hefesto-0.4.5/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     2581 2023-06-19 08:51:18.000000 Hefesto-0.4.5/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.5/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-06-30 05:47:51.953725 Hefesto-0.4.5/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-06-28 11:52:18.000000 Hefesto-0.4.5/setup.py
```

### Comparing `Hefesto-0.4.4/Hefesto/main.py` & `Hefesto-0.4.5/Hefesto/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         else:
             self.df_data = datainput
             return self.df_data
         
         # Create an object as dictonary to reduce duplicate calls:
         self.reg = dict()
 
-
     def transformFiab(self):
 
     # Import static template for all CDE terms:
         temp = Template.template_model
 
     # Check the status of the dataframe used:
         if not "model" and "pid" and "value" in self.df_data.columns:
@@ -162,17 +161,17 @@
     def valueEdition(self, resulting_df):
 
         # valueIRI 
         valueRelation = {
             "Sex":"attribute_type",
             "Status":"attribute_type",
             "Diagnosis":"attribute_type",
-            "Genetic":"attribute_id",
+            "Genetic":"value_id",
             "Symptoms":"attribute_type",
-            "Imaging":"attribute_id",
+            "Imaging":"value_id",
             "Clinical_trial":"attribute_type"
         }
         # Datatype:
         datatypeRelation = {
             "xsd:string":"value_string",
             "xsd:date" : "value_date",
             "xsd:float": "value_float",
@@ -192,27 +191,34 @@
             for k,v in valueRelation.items():
                 # valueIRI ---> attribute_id/value:
                 if row["model"] == k:
                     resulting_df.at[index, v] = resulting_df["valueIRI"][index]
                     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
             # attribute_id_value
-            if row["model"] == "Genetic":
-                resulting_df.at[index, "attribute_id_value"] = resulting_df["value"][index]
-                resulting_df.at[index, "value_string"] = None # Deleting the value_string in case it moves from value to value_string
-                resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+            # if row["model"] == "Genetic":
+            #     resulting_df.at[index, "attribute_id_value"] = resulting_df["value"][index]
+            #     resulting_df.at[index, "value_string"] = None # Deleting the value_string in case it moves from value to value_string
+            #     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
+            # Pass value date into date context
             if row["value"] != None and row["value_datatype"] == "xsd:date":
                 resulting_df.at[index, "date"] = resulting_df["value"][index]
                 resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
+            # Pass value age into age context
             if row["value"] != None and row["value_datatype"] == "xsd:float" and row["model"] in modelList:
                 resulting_df.at[index, "age"] = resulting_df["value"][index]
                 resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
+            # Move startdate of diagnosis to date context
+            if row["model"] == "Diagnosis":
+                resulting_df.at[index, "date"] = resulting_df["startdate"][index]
+                resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
             # enddate correction:
             if row["startdate"] != None and row["enddate"] == None:
                 resulting_df.at[index,"enddate"] = resulting_df["startdate"][index]
                 resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
         return resulting_df
 
@@ -293,15 +299,15 @@
 
 # # Test 1:
 
 # test = Hefesto(datainput = "../data/INPUT_DATA.csv")
 # transform = test.transformFiab()
 # transform.to_csv ("../data/OUTPUT_DATA.csv", index = False, header=True)
 
-# # # Test 2
+# Test 2
 # with open("../data/CDEconfig.yaml") as file:
 #     configuration = yaml.load(file, Loader=yaml.FullLoader)
 
 # test = Hefesto(datainput = "../data/INPUT_DATA2.csv")
 # transform = test.transformShape(configuration=configuration, clean_blanks = True) #, clean_blanks=False
 # # label = test.get_label("output_type")
 # # url_from_label= test.get_uri("output_type_label","ncit")
```

### Comparing `Hefesto-0.4.4/setup.py` & `Hefesto-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.4.4",
+    version="0.4.5",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

