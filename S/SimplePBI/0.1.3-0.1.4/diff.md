# Comparing `tmp/SimplePBI-0.1.3-py3-none-any.whl.zip` & `tmp/SimplePBI-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 49794 bytes, number of entries: 20
+Zip file size: 51666 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat      643 b- defN 22-Sep-15 17:59 simplepbi/__init__.py
--rw-rw-rw-  2.0 fat    86420 b- defN 23-May-08 15:34 simplepbi/admin/__init__.py
+-rw-rw-rw-  2.0 fat    87248 b- defN 23-May-29 19:21 simplepbi/admin/__init__.py
 -rw-rw-rw-  2.0 fat     9878 b- defN 22-Sep-15 17:56 simplepbi/apps/__init__.py
+-rw-rw-rw-  2.0 fat     6276 b- defN 23-Jun-29 20:35 simplepbi/azpause/__init__.py
 -rw-rw-rw-  2.0 fat    15534 b- defN 22-Sep-15 17:56 simplepbi/capacities/__init__.py
 -rw-rw-rw-  2.0 fat    17252 b- defN 22-Sep-15 17:56 simplepbi/dashboards/__init__.py
 -rw-rw-rw-  2.0 fat    15322 b- defN 22-Sep-15 17:56 simplepbi/dataflows/__init__.py
 -rw-rw-rw-  2.0 fat    58028 b- defN 23-Feb-22 18:07 simplepbi/datasets/__init__.py
 -rw-rw-rw-  2.0 fat    16099 b- defN 22-Sep-15 17:56 simplepbi/gateways/__init__.py
 -rw-rw-rw-  2.0 fat    14147 b- defN 22-Sep-15 17:57 simplepbi/groups/__init__.py
 -rw-rw-rw-  2.0 fat    24405 b- defN 23-Apr-27 16:15 simplepbi/imports/__init__.py
 -rw-rw-rw-  2.0 fat    24126 b- defN 22-Sep-15 17:57 simplepbi/pipelines/__init__.py
 -rw-rw-rw-  2.0 fat    44427 b- defN 23-Mar-10 18:36 simplepbi/reports/__init__.py
 -rw-rw-rw-  2.0 fat    12740 b- defN 22-Sep-15 17:57 simplepbi/scorecards/__init__.py
 -rw-rw-rw-  2.0 fat     4093 b- defN 22-Sep-15 17:57 simplepbi/token/__init__.py
 -rw-rw-rw-  2.0 fat     3457 b- defN 23-May-08 15:36 simplepbi/utils/__init__.py
--rw-rw-rw-  2.0 fat     1072 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11372 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1694 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/RECORD
-20 files, 360811 bytes uncompressed, 47050 bytes compressed:  87.0%
+-rw-rw-rw-  2.0 fat     1072 b- defN 23-Jun-30 20:00 SimplePBI-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12152 b- defN 23-Jun-30 20:00 SimplePBI-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 20:00 SimplePBI-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-30 20:00 SimplePBI-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1780 b- defN 23-Jun-30 20:00 SimplePBI-0.1.4.dist-info/RECORD
+21 files, 368781 bytes uncompressed, 48788 bytes compressed:  86.8%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: simplepbi/admin/__init__.py
 Comment: 
 
 Filename: simplepbi/apps/__init__.py
 Comment: 
 
+Filename: simplepbi/azpause/__init__.py
+Comment: 
+
 Filename: simplepbi/capacities/__init__.py
 Comment: 
 
 Filename: simplepbi/dashboards/__init__.py
 Comment: 
 
 Filename: simplepbi/dataflows/__init__.py
@@ -39,23 +42,23 @@
 
 Filename: simplepbi/token/__init__.py
 Comment: 
 
 Filename: simplepbi/utils/__init__.py
 Comment: 
 
-Filename: SimplePBI-0.1.3.dist-info/LICENSE
+Filename: SimplePBI-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: SimplePBI-0.1.3.dist-info/METADATA
+Filename: SimplePBI-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: SimplePBI-0.1.3.dist-info/WHEEL
+Filename: SimplePBI-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: SimplePBI-0.1.3.dist-info/top_level.txt
+Filename: SimplePBI-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: SimplePBI-0.1.3.dist-info/RECORD
+Filename: SimplePBI-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplepbi/admin/__init__.py

```diff
@@ -1835,8 +1835,28 @@
                 if res.json()["continuationUri"] == None or res.json()["ArtifactAccessEntities"]==[]:
                     ban=False        
                 url = res.json()["continuationUri"]   
             return res.json()
         except requests.exceptions.HTTPError as ex:
             print("HTTP Error: ", ex, "\nText: ", ex.response.text)
         except requests.exceptions.RequestException as e:
+            print("Request exception: ", e)
+            
+    def get_tenant_settings(self):
+        """Returns a list of the tenant settings.
+        ### Returns
+        ----
+        Dict:
+            Response 200. A dict with tenant settings.
+        ### Limitations
+        ----
+        Maximum 200 requests per hour.
+        """
+        try:
+            url = "https://api.powerbi.com/v1/admin/tenantsettings"                     
+            res = requests.get(url, headers={'Content-Type': 'application/json', "Authorization": "Bearer {}".format(self.token)})
+            res.raise_for_status()
+            return res.json()
+        except requests.exceptions.HTTPError as ex:
+            print("HTTP Error: ", ex, "\nText: ", ex.response.text)
+        except requests.exceptions.RequestException as e:
             print("Request exception: ", e)
```

## Comparing `SimplePBI-0.1.3.dist-info/LICENSE` & `SimplePBI-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SimplePBI-0.1.3.dist-info/METADATA` & `SimplePBI-0.1.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: SimplePBI
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simplify usage of Power Bi Rest API
 Home-page: 
 Download-URL: 
 Author: Ignacio Barrau <igna_barrau@hotmail.com>, Martin Zurita <martinzurita1@gmail.com>
 License: MIT
 Project-URL: Documentation, https://docs.microsoft.com/en-us/rest/api/power-bi/
 Project-URL: Say Thanks!, https://www.ladataweb.com.ar/contacto.html
 Project-URL: Source, https://github.com/ladataweb/SimplePBI
 Project-URL: Tracker, https://github.com/ladataweb/SimplePBI/issues
-Keywords: Power BI,PBI,LaDataWeb,Azure,Data,Python
+Keywords: Power BI,PBI,LaDataWeb,Azure,Data,Python,Fabric
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
@@ -88,19 +88,24 @@
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Dashboards_details.txt" target="_blank">Dashboards</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Apps_details.txt" target="_blank">Apps</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Imports_details.txt" target="_blank">Imports</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Gateways_details.txt" target="_blank">Gateways</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Capacities_details.txt" target="_blank">Capacities</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Pipelines_details.txt" target="_blank">Pipelines (Preview)</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Scorecards_details.txt" target="_blank">Scorecards (Preview)</a>
+- <a href="https://github.com/ladataweb/SimplePBI/blob/main/Az_Pause_Resume_details.txt" target="_blank">Azure Pause and Resume resource (Preview)</a>
 
 ## Complex requests
 If you want to get a deeper look on complex __Admin__ methods and unique methods. 
 <a href="https://github.com/ladataweb/SimplePBI/blob/main/Admin_complex.md" target="_blank">Check this doc</a>
 
+## Azure Pause Resume Resources
+We have added a new feature to include some Azure Resource API Manager. The new "azpause" class will let you Pause or Resume Azure tabular or capacity resources. With SimplePBI you can pause and resume Fabric, Power Bi Embedded or Azure Analysis Services resources.
+<a href="https://github.com/ladataweb/SimplePBI/blob/main/AzPauseResume.md" target="_blank">Check this doc</a>
+
 ## Additional content
 There an aditional library Utils for transformations. It is used to help some requests returning different values.
 The most useful method in the Utils class might be to_pandas. You can use the method to convert simple dicts to pandas. It needs the dict and the key father of a list of dicts in the response. The usual get responses are using "value" as the key.
 We are also adding new methods with the requests to help get new actions. Examples:
 
 ### Example of our amazing unique requests
 - get_orphan_dataflows_preview: get dataflows without dataset
@@ -242,7 +247,12 @@
 Adding new request to get last 30 days of activity logs automatically.
 
 0.1.3 (08/05/2023)
 ------------------
 Adding update sources for datasets. It's a complex body request.
 Adding new unique request for publishing pbix file from azure devops repo.
 Changing pandas coding to work with 2.0.1 version. Fixing deprecated methods.
+
+0.1.4 (30/06/2023)
+------------------
+Adding newest admin request for getting tenant settings
+Adding new unique requests for pausing and resuming Fabric, Power Bi Embedded and Azure Analysis Services.
```

## Comparing `SimplePBI-0.1.3.dist-info/RECORD` & `SimplePBI-0.1.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 simplepbi/__init__.py,sha256=6rG794o_Pw51N-rJOU--X3zs5TznwOk9vk7tNsw4E8Y,643
-simplepbi/admin/__init__.py,sha256=NGjCelRo8LUTDIkPNI5RlDWtcIfKApnmWGoAhbDE8S8,86420
+simplepbi/admin/__init__.py,sha256=Lf-gU5lc_h6ZwxrPYMLNz8DKVLcwe2QCYk6OkWtqjuU,87248
 simplepbi/apps/__init__.py,sha256=vo6-DtuprZx9dfLqc6jeMvRVGYvNNj9QX4mpSfK15GY,9878
+simplepbi/azpause/__init__.py,sha256=-BtjrmaMod3Q-DPpHpRlHsnvueqjVrAPac9S_MxeX0E,6276
 simplepbi/capacities/__init__.py,sha256=1t9ancMJvpzht931qvto3Oah3Zjn-Ut2KFEq3-Ap10o,15534
 simplepbi/dashboards/__init__.py,sha256=TtH4u-wxKF7_C7byIFODavxb8flJiIyzxc-PdnpM7Ns,17252
 simplepbi/dataflows/__init__.py,sha256=QGP2rX4zeVQ44NUf0W8eP5Wm_zzwj8G52TxFNG3jnSA,15322
 simplepbi/datasets/__init__.py,sha256=dqNLkYTUJIf-VKrVSUfBdA-mBNhCK6Ssylj-JHL0E3E,58028
 simplepbi/gateways/__init__.py,sha256=ol1eZBIAT0v764BCUSHMzhA4-e3FDh77I8D_wCWLSz8,16099
 simplepbi/groups/__init__.py,sha256=acPort3e99ajdTKXhLWvnGWevVIuaM3IBRrUjkIYTsY,14147
 simplepbi/imports/__init__.py,sha256=GSgWOLBpBnvEyiQH6qjQxk-2E-4atBd8RgCWo0P03Gk,24405
 simplepbi/pipelines/__init__.py,sha256=KtmtGa1049qqtCCclaNB7_fBAv56PGIVMrWp4v-B9uQ,24126
 simplepbi/reports/__init__.py,sha256=x25_H-PVITI37luFK73BQdwIRD60nG9zRmnMhYPoJvU,44427
 simplepbi/scorecards/__init__.py,sha256=eb6Z4q6dasdPcGtsxTqbupkIhMo_sAHM98fgtqiCH4A,12740
 simplepbi/token/__init__.py,sha256=sT8EgSn3RQ-gbqmVPxVux37S_mUnLIm_0qQRkd6qqAw,4093
 simplepbi/utils/__init__.py,sha256=k2Opnd02zwaXUocHmgUvaqFRjfvU14L5IfA0LaMHzjQ,3457
-SimplePBI-0.1.3.dist-info/LICENSE,sha256=ZtpzRFk5l7aVPep5WYvScxZ-tc4yiqgCR41jLTgns5I,1072
-SimplePBI-0.1.3.dist-info/METADATA,sha256=gtlfwH_mkIuM8t4SKcDL4lZMAX3P-OwDpz7RaByjzT8,11372
-SimplePBI-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-SimplePBI-0.1.3.dist-info/top_level.txt,sha256=IwRTqkuCr1bqy2LPIIj4_aHuRc9NNLgtB8VxuIl_OnM,10
-SimplePBI-0.1.3.dist-info/RECORD,,
+SimplePBI-0.1.4.dist-info/LICENSE,sha256=ZtpzRFk5l7aVPep5WYvScxZ-tc4yiqgCR41jLTgns5I,1072
+SimplePBI-0.1.4.dist-info/METADATA,sha256=6nVB7WlgbGI_s3JYbX6QmkRJeaQ4nEoQvg5YoJyggeA,12152
+SimplePBI-0.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+SimplePBI-0.1.4.dist-info/top_level.txt,sha256=IwRTqkuCr1bqy2LPIIj4_aHuRc9NNLgtB8VxuIl_OnM,10
+SimplePBI-0.1.4.dist-info/RECORD,,
```

