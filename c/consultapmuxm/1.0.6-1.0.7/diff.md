# Comparing `tmp/consultapmuxm-1.0.6-py3-none-any.whl.zip` & `tmp/consultapmuxm-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8604 bytes, number of entries: 6
+Zip file size: 8614 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      158 b- defN 22-Oct-25 22:52 consultapmuxm/__init__.py
--rw-rw-rw-  2.0 fat    30622 b- defN 23-Jan-03 23:29 consultapmuxm/consultapmuxm.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-Jan-03 23:38 consultapmuxm-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-03 23:38 consultapmuxm-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jan-03 23:38 consultapmuxm-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      490 b- defN 23-Jan-03 23:38 consultapmuxm-1.0.6.dist-info/RECORD
-6 files, 32154 bytes uncompressed, 7712 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat    30745 b- defN 23-Feb-18 01:33 consultapmuxm/consultapmuxm.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Feb-18 01:36 consultapmuxm-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-18 01:36 consultapmuxm-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Feb-18 01:36 consultapmuxm-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      490 b- defN 23-Feb-18 01:36 consultapmuxm-1.0.7.dist-info/RECORD
+6 files, 32277 bytes uncompressed, 7722 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: consultapmuxm/__init__.py
 Comment: 
 
 Filename: consultapmuxm/consultapmuxm.py
 Comment: 
 
-Filename: consultapmuxm-1.0.6.dist-info/METADATA
+Filename: consultapmuxm-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: consultapmuxm-1.0.6.dist-info/WHEEL
+Filename: consultapmuxm-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: consultapmuxm-1.0.6.dist-info/top_level.txt
+Filename: consultapmuxm-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: consultapmuxm-1.0.6.dist-info/RECORD
+Filename: consultapmuxm-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## consultapmuxm/consultapmuxm.py

```diff
@@ -193,14 +193,15 @@
                 elif vari == 'v_m':
                     a = phasor_names[(phasor_names['id'] == id_pmu) & ((phasor_names['var_name'] == 'v') |(phasor_names['var_name'] == 'va')) ]
                     a['var_name'] = 'v'
                     a['table_name'] = 'v_'+ a['phasor_name'] +'_m'
                     vari_names= pd.concat([vari_names, a])
                 elif vari == 'v_a':
                     a = phasor_names[(phasor_names['id'] == id_pmu) & ((phasor_names['var_name'] == 'v') |(phasor_names['var_name'] == 'va'))]
+                    a['var_name'] = 'v'
                     a['table_name'] = 'v_'+ a['phasor_name'] +'_a'
                     vari_names= pd.concat([vari_names, a])
                 elif vari == 'ia_m':
                     a = phasor_names[(phasor_names['id'] == id_pmu) & (phasor_names['var_name'] == 'ia')]
                     a['table_name'] = 'i_'+ a['phasor_name'] +'_m'
                     vari_names= pd.concat([vari_names, a])
                 elif vari == 'ia_a':
@@ -221,18 +222,20 @@
                     vari_names= pd.concat([vari_names, a])
                 elif vari == 'ic_a':
                     a = phasor_names[(phasor_names['id'] == id_pmu) & (phasor_names['var_name'] == 'ic')]
                     a['table_name'] = 'i_'+ a['phasor_name'] +'_a'
                     vari_names= pd.concat([vari_names, a])
                 elif vari == 'i_m':
                     a = phasor_names[(phasor_names['id'] == id_pmu) & ((phasor_names['var_name'] == 'i') |(phasor_names['var_name'] == 'ia')) ]
+                    a['var_name'] = 'i'
                     a['table_name'] = 'i_'+ a['phasor_name'] +'_m'
                     vari_names= pd.concat([vari_names, a])
                 elif vari == 'i_a':
                     a = phasor_names[(phasor_names['id'] == id_pmu) & ((phasor_names['var_name'] == 'i') |(phasor_names['var_name'] == 'ia'))]
+                    a['var_name'] = 'i'
                     a['table_name'] = 'i_'+ a['phasor_name'] +'_a'
                     vari_names= pd.concat([vari_names, a])
                 elif vari == 'f':
                     vari_names = vari_names.append ({'id': int(id_pmu), 'type':'FREQUENCY', 'var_name':'f', 'table_name': 'f'}, ignore_index=True)
                 elif vari == 'dfdt':
                     vari_names = vari_names.append ({'id': int(id_pmu), 'type':'DFDT', 'var_name':'dfdt', 'table_name': 'dfdt'}, ignore_index=True)
```

## Comparing `consultapmuxm-1.0.6.dist-info/METADATA` & `consultapmuxm-1.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consultapmuxm
-Version: 1.0.6
+Version: 1.0.7
 Summary: tool to query pmu data from phasor point
 Home-page: https://github.com/jdpinzon/XM_consultapmu
 Author: Jaime Dwaigth Pinzon Casallas
 Author-email: jpinzon@xm.com.co
 License: MIT
 Download-URL: https://raw.githubusercontent.com/jdpinzon/XM_consultapmu/main/consultapmuxm.py?token=GHSAT0AAAAAAB4MF6UXPFEJSZKTG2MLGLK2Y4Z3QQA
 Keywords: PMU,PHASORPOINT,XM
```

