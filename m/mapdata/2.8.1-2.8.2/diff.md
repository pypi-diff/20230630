# Comparing `tmp/mapdata-2.8.1.tar.gz` & `tmp/mapdata-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.8.1.tar", last modified: Wed Jun 28 16:00:53 2023, max compression
+gzip compressed data, was "mapdata-2.8.2.tar", last modified: Fri Jun 30 03:41:41 2023, max compression
```

## Comparing `mapdata-2.8.1.tar` & `mapdata-2.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-28 16:00:53.520729 mapdata-2.8.1/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.8.1/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.8.1/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-06-28 16:00:53.520729 mapdata-2.8.1/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.8.1/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-28 16:00:53.520729 mapdata-2.8.1/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   335743 2023-06-28 13:41:11.000000 mapdata-2.8.1/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-28 16:00:53.520729 mapdata-2.8.1/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-06-28 16:00:53.000000 mapdata-2.8.1/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-28 16:00:53.000000 mapdata-2.8.1/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-28 16:00:53.000000 mapdata-2.8.1/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-28 16:00:53.000000 mapdata-2.8.1/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-28 16:00:53.520729 mapdata-2.8.1/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-06-28 15:56:27.000000 mapdata-2.8.1/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-30 03:41:41.627201 mapdata-2.8.2/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.8.2/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.8.2/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-06-30 03:41:41.627201 mapdata-2.8.2/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.8.2/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-30 03:41:41.627201 mapdata-2.8.2/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   336300 2023-06-30 03:19:46.000000 mapdata-2.8.2/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-30 03:41:41.627201 mapdata-2.8.2/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-06-30 03:41:41.000000 mapdata-2.8.2/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-30 03:41:41.000000 mapdata-2.8.2/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-30 03:41:41.000000 mapdata-2.8.2/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-30 03:41:41.000000 mapdata-2.8.2/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-30 03:41:41.627201 mapdata-2.8.2/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-06-30 03:20:26.000000 mapdata-2.8.2/setup.py
```

### Comparing `mapdata-2.8.1/LICENSE.txt` & `mapdata-2.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.8.1/PKG-INFO` & `mapdata-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.8.1
+Version: 2.8.2
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.8.1/README.md` & `mapdata-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-2.8.1/mapdata/mapdata.py` & `mapdata-2.8.2/mapdata/mapdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.8.1"
-vdate = "2023-06-28"
+version = "2.8.2"
+vdate = "2023-06-29"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -623,21 +623,22 @@
 		return dt
 	if isboolean(v):
 		return "boolean"
 	return "string"
 
 # Lookup table for priorities among data types
 data_type_pair_priorities = {
-		"int" : {"int":"int", "float":"float", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"string", "string":"string"},
-		"float" : {"int":"float", "float":"float", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"string", "string":"string"},
-		"date" : {"int":"string", "float":"string", "date":"date", "timestamp":"timestamp", "timestamptz":"string", "boolean":"string", "string":"string"},
-		"timestamp" : {"int":"string", "float":"string", "date":"timestamp", "timestamp":"timestamp", "datetimetz":"string", "boolean":"string", "string":"string"},
-		"timestamptz" : {"int":"string", "float":"string", "date":"string", "timestamp":"string", "timestamptz":"timestamptz", "boolean":"string", "string":"string"},
-		"string" : {"int":"string", "float":"string", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"string", "string":"string"},
-		"boolean" : {"int":"string", "float":"string", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"boolean", "string":"string"}
+		"int" : {"int":"int", "float":"float", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"string", "string":"string", None:"int"},
+		"float" : {"int":"float", "float":"float", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"string", "string":"string", None:"float"},
+		"date" : {"int":"string", "float":"string", "date":"date", "timestamp":"timestamp", "timestamptz":"string", "boolean":"string", "string":"string", None:"date"},
+		"timestamp" : {"int":"string", "float":"string", "date":"timestamp", "timestamp":"timestamp", "datetimetz":"string", "boolean":"string", "string":"string", None:"timestamp"},
+		"timestamptz" : {"int":"string", "float":"string", "date":"string", "timestamp":"string", "timestamptz":"timestamptz", "boolean":"string", "string":"string", None:"timestamptz"},
+		"string" : {"int":"string", "float":"string", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"string", "string":"string", None:"string"},
+		"boolean" : {"int":"string", "float":"string", "date":"string", "timestamp":"string", "timestamptz":"string", "boolean":"boolean", "string":"string", None:"boolean"},
+		None : {"int":"int", "float":"float", "date":"float", "timestamp":"timestamp", "timestamptz":"timestamptz", "boolean":"boolean", "string":"string", None:None}
 		}
 def priority_data_type(dt1, dt2):
 	return data_type_pair_priorities[dt1][dt2]
 
 
 def data_type_cast_fn(data_type_str):
 	if data_type_str == "string":
@@ -681,18 +682,25 @@
 
 
 def set_data_types(headers, rows, q):
 	# Column-by-column processing is slightly faster than row-by-row processing.
 	coltypes = []
 	for i, colname in enumerate(headers):
 		datavals = [row[i] for row in rows]
+		dt = None
+		for d in datavals:
+			ndt = data_type(d)
+			if ndt != dt:
+				dt = priority_data_type(ndt, dt)
+				if dt == "string":
+					break
 		non_null = [d for d in datavals if d is not None and not (type(d) is str and d.strip() == '')]
 		nullcount = len(datavals) - len(non_null)
 		uniquevals = len(set(non_null))
-		coltypes.append((colname, common_data_type(datavals), nullcount, uniquevals))
+		coltypes.append((colname, dt, nullcount, uniquevals))
 	q.put(coltypes)
 
 
 # Translations to SQLite type affinity names
 sqlite_type_x = {'int': 'INTEGER', 'float': 'REAL', 'string': 'TEXT', 'timestamptz': 'TEXT',
 		'timestamp': 'TEXT', 'date': 'TEXT', 'boolean': 'INTEGER'}
 
@@ -4157,143 +4165,146 @@
 	if os.name == 'posix':
 		fns = (r'(?P<%s>[\w\.\-\\\/\'~`!@#$^&()+={}\[\]:;,]*[\w\.\-\\\/\'~`!@#$^&(+={}\[\]:;,])' % symbolicname, r'"(?P<%s>[\w\s\.\-\\\/\'~`!@#$^&()+={}\[\]:;,]+)"' % symbolicname)
 	else:
 		fns = (r'(?P<%s>([A-Z]\:)?[\w+\,()!@#$^&\+=;\'{}\[\]~`\.\-\\\/]*[\w+\,(!@#$^&\+=;\'{}\[\]~`\.\-\\\/])' % symbolicname, r'"(?P<%s>([A-Z]\:)?[\w+\,()!@#$^&\+=;\'{}\[\]~`\s\.\-\\\/]+)"' % symbolicname)
 	return ins_rxs(fns, fragment1, fragment2)
 
 
+dt_fmts = collections.deque((
+			"%x %X",
+			"%m/%d/%Y %H:%M",
+			"%m/%d/%Y %H%M",
+			"%m/%d/%Y %H:%M:%S",
+			"%Y-%m-%d %H:%M:%S",
+			"%Y-%m-%dT%H:%M:%S",
+			"%Y-%m-%d %H%M",
+			"%Y-%m-%d %H:%M",
+			"%Y-%m-%d %I:%M%p",
+			"%Y-%m-%d %I:%M %p",
+			"%Y-%m-%d %I:%M:%S%p",
+			"%Y-%m-%d %I:%M:%S %p",
+			"%m/%d/%Y %I:%M%p",
+			"%m/%d/%Y %I:%M %p",
+			"%m/%d/%Y %I:%M:%S%p",
+			"%m/%d/%Y %I:%M:%S %p",
+			"%Y/%m/%d %H%M",
+			"%Y/%m/%d %H:%M",
+			"%Y/%m/%d %H:%M:%S",
+			"%Y/%m/%d %I:%M%p",
+			"%Y/%m/%d %I:%M %p",
+			"%Y/%m/%d %I:%M:%S%p",
+			"%Y/%m/%d %I:%M:%S %p",
+			"%Y/%m/%d %X",
+			"%c",
+			"%b %d, %Y %X",
+			"%b %d, %Y %I:%M %p",
+			"%b %d %Y %X",
+			"%b %d %Y %I:%M %p",
+			"%d %b, %Y %X",
+			"%d %b, %Y %I:%M %p",
+			"%d %b %Y %X",
+			"%d %b %Y %I:%M %p",
+			"%b. %d, %Y %X",
+			"%b. %d, %Y %I:%M %p",
+			"%b. %d %Y %X",
+			"%b. %d %Y %I:%M %p",
+			"%d %b., %Y %X",
+			"%d %b., %Y %I:%M %p",
+			"%d %b. %Y %X",
+			"%d %b. %Y %I:%M %p",
+			"%B %d, %Y %X",
+			"%B %d, %Y %I:%M %p",
+			"%B %d %Y %X",
+			"%B %d %Y %I:%M %p",
+			"%d %B, %Y %X",
+			"%d %B, %Y %I:%M %p",
+			"%d %B %Y %X",
+			"%d %B %Y %I:%M %p"
+			))
 def parse_datetime(datestr):
-	dt_fmts = (
-				"%x %X",
-				"%Y-%m-%d %H:%M:%S",
-				"%Y-%m-%dT%H:%M:%S",
-				"%Y-%m-%d %H%M",
-				"%Y-%m-%d %H:%M",
-				"%Y-%m-%d %I:%M%p",
-				"%Y-%m-%d %I:%M %p",
-				"%Y-%m-%d %I:%M:%S%p",
-				"%Y-%m-%d %I:%M:%S %p",
-				"%m/%d/%Y %H%M",
-				"%m/%d/%Y %H:%M",
-				"%m/%d/%Y %H:%M:%S",
-				"%m/%d/%Y %I:%M%p",
-				"%m/%d/%Y %I:%M %p",
-				"%m/%d/%Y %I:%M:%S%p",
-				"%m/%d/%Y %I:%M:%S %p",
-				"%Y/%m/%d %H%M",
-				"%Y/%m/%d %H:%M",
-				"%Y/%m/%d %H:%M:%S",
-				"%Y/%m/%d %I:%M%p",
-				"%Y/%m/%d %I:%M %p",
-				"%Y/%m/%d %I:%M:%S%p",
-				"%Y/%m/%d %I:%M:%S %p",
-				"%Y/%m/%d %X",
-				"%c",
-				"%b %d, %Y %X",
-				"%b %d, %Y %I:%M %p",
-				"%b %d %Y %X",
-				"%b %d %Y %I:%M %p",
-				"%d %b, %Y %X",
-				"%d %b, %Y %I:%M %p",
-				"%d %b %Y %X",
-				"%d %b %Y %I:%M %p",
-				"%b. %d, %Y %X",
-				"%b. %d, %Y %I:%M %p",
-				"%b. %d %Y %X",
-				"%b. %d %Y %I:%M %p",
-				"%d %b., %Y %X",
-				"%d %b., %Y %I:%M %p",
-				"%d %b. %Y %X",
-				"%d %b. %Y %I:%M %p",
-				"%B %d, %Y %X",
-				"%B %d, %Y %I:%M %p",
-				"%B %d %Y %X",
-				"%B %d %Y %I:%M %p",
-				"%d %B, %Y %X",
-				"%d %B, %Y %I:%M %p",
-				"%d %B %Y %X",
-				"%d %B %Y %I:%M %p"
-				)
 	if type(datestr) == datetime.datetime:
 		return datestr
 	if not isinstance(datestr, str):
 		try:
 			datestr = str(datestr)
 		except:
 			return None
 	dt = None
-	for f in dt_fmts:
+	for i, f in enumerate(dt_fmts):
 		try:
-			dt = datetime.datetime.strptime(datestr, f)
+			dt = datetime.datetime.strptime(data, f)
+			if i:
+				del dt_fmts[i]
+				dt_fmts.appendleft(f)
 		except:
 			continue
 		break
 	return dt
 
 dtzrx = re.compile(u"(.+)\s*([+-])(\d{1,2}):?(\d{2})$")
+timestamptz_fmts = collections.deque((
+	"%Y-%m-%d %H%M%Z", "%Y-%m-%d %H%M %Z",
+	"%m/%d/%Y%Z", "%m/%d/%Y %Z",
+	"%m/%d/%y%Z", "%m/%d/%y %Z",
+	"%m/%d/%Y %H%M%Z", "%m/%d/%Y %H%M %Z",
+	"%m/%d/%Y %H:%M%Z", "%m/%d/%Y %H:%M %Z",
+	"%Y-%m-%dT%H%M%Z", "%Y-%m-%dT%H%M %Z",
+	"%Y-%m-%d %H:%M%Z", "%Y-%m-%d %H:%M %Z",
+	"%Y-%m-%dT%H:%M%Z", "%Y-%m-%dT%H:%M %Z",
+	"%Y-%m-%d %H:%M:%S%Z", "%Y-%m-%d %H:%M:%S %Z",
+	"%Y-%m-%dT%H:%M:%S%Z", "%Y-%m-%dT%H:%M:%S %Z",
+	"%Y-%m-%d %I:%M%p%Z", "%Y-%m-%d %I:%M%p %Z",
+	"%Y-%m-%dT%I:%M%p%Z", "%Y-%m-%dT%I:%M%p %Z",
+	"%Y-%m-%d %I:%M %p%Z", "%Y-%m-%d %I:%M %p %Z",
+	"%Y-%m-%dT%I:%M %p%Z", "%Y-%m-%dT%I:%M %p %Z",
+	"%Y-%m-%d %I:%M:%S%p%Z", "%Y-%m-%d %I:%M:%S%p %Z",
+	"%Y-%m-%dT%I:%M:%S%p%Z", "%Y-%m-%dT%I:%M:%S%p %Z",
+	"%Y-%m-%d %I:%M:%S %p%Z", "%Y-%m-%d %I:%M:%S %p %Z",
+	"%Y-%m-%dT%I:%M:%S %p%Z", "%Y-%m-%dT%I:%M:%S %p %Z",
+	"%c%Z", "%c %Z",
+	"%x %X%Z", "%x %X %Z",
+	"%m/%d/%Y %H:%M:%S%Z", "%m/%d/%Y %H:%M:%S %Z",
+	"%m/%d/%Y %I:%M%p%Z", "%m/%d/%Y %I:%M%p %Z",
+	"%m/%d/%Y %I:%M %p%Z", "%m/%d/%Y %I:%M %p %Z",
+	"%m/%d/%Y %I:%M:%S%p%Z", "%m/%d/%Y %I:%M:%S%p %Z",
+	"%m/%d/%Y %I:%M:%S %p%Z", "%m/%d/%Y %I:%M:%S %p %Z",
+	"%Y/%m/%d %H%M%Z", "%Y/%m/%d %H%M %Z",
+	"%Y/%m/%d %H:%M%Z", "%Y/%m/%d %H:%M %Z",
+	"%Y/%m/%d %H:%M:%S%Z", "%Y/%m/%d %H:%M:%S %Z",
+	"%Y/%m/%d %I:%M%p%Z", "%Y/%m/%d %I:%M%p %Z",
+	"%Y/%m/%d %I:%M %p%Z", "%Y/%m/%d %I:%M %p %Z",
+	"%Y/%m/%d %I:%M:%S%p%Z", "%Y/%m/%d %I:%M:%S%p %Z",
+	"%Y/%m/%d %I:%M:%S %p%Z", "%Y/%m/%d %I:%M:%S %p %Z",
+	"%Y/%m/%d %X%Z", "%Y/%m/%d %X %Z",
+	"%b %d, %Y %X%Z", "%b %d, %Y %X %Z",
+	"%b %d, %Y %I:%M %p%Z", "%b %d, %Y %I:%M %p %Z",
+	"%b %d %Y %X%Z", "%b %d %Y %X %Z",
+	"%b %d %Y %I:%M %p%Z", "%b %d %Y %I:%M %p %Z",
+	"%d %b, %Y %X%Z", "%d %b, %Y %X %Z",
+	"%d %b, %Y %I:%M %p%Z", "%d %b, %Y %I:%M %p %Z",
+	"%d %b %Y %X%Z", "%d %b %Y %X %Z",
+	"%d %b %Y %I:%M %p%Z", "%d %b %Y %I:%M %p %Z",
+	"%b. %d, %Y %X%Z", "%b. %d, %Y %X %Z",
+	"%b. %d, %Y %I:%M %%Z", "%b. %d, %Y %I:%M %p %Z",
+	"%b. %d %Y %X%Z", "%b. %d %Y %X %Z",
+	"%b. %d %Y %I:%M %p%Z", "%b. %d %Y %I:%M %p %Z",
+	"%d %b., %Y %X%Z", "%d %b., %Y %X %Z",
+	"%d %b., %Y %I:%M %p%Z", "%d %b., %Y %I:%M %p %Z",
+	"%d %b. %Y %X%Z", "%d %b. %Y %X %Z",
+	"%d %b. %Y %I:%M %p%Z", "%d %b. %Y %I:%M %p %Z",
+	"%B %d, %Y %X%Z", "%B %d, %Y %X %Z",
+	"%B %d, %Y %I:%M %p%Z", "%B %d, %Y %I:%M %p %Z",
+	"%B %d %Y %X%Z", "%B %d %Y %X %Z",
+	"%B %d %Y %I:%M %p%Z", "%B %d %Y %I:%M %p %Z",
+	"%d %B, %Y %X%Z", "%d %B, %Y %X %Z",
+	"%d %B, %Y %I:%M %p%Z", "%d %B, %Y %I:%M %p %Z",
+	"%d %B %Y %X%Z", "%d %B %Y %X %Z",
+	"%d %B %Y %I:%M %p%Z", "%d %B %Y %I:%M %p %Z"
+	))
 def parse_datetimetz(data):
-	timestamptz_fmts = (
-		"%Y-%m-%d %H%M%Z", "%Y-%m-%d %H%M %Z",
-		"%Y-%m-%dT%H%M%Z", "%Y-%m-%dT%H%M %Z",
-		"%Y-%m-%d %H:%M%Z", "%Y-%m-%d %H:%M %Z",
-		"%Y-%m-%dT%H:%M%Z", "%Y-%m-%dT%H:%M %Z",
-		"%Y-%m-%d %H:%M:%S%Z", "%Y-%m-%d %H:%M:%S %Z",
-		"%Y-%m-%dT%H:%M:%S%Z", "%Y-%m-%dT%H:%M:%S %Z",
-		"%Y-%m-%d %I:%M%p%Z", "%Y-%m-%d %I:%M%p %Z",
-		"%Y-%m-%dT%I:%M%p%Z", "%Y-%m-%dT%I:%M%p %Z",
-		"%Y-%m-%d %I:%M %p%Z", "%Y-%m-%d %I:%M %p %Z",
-		"%Y-%m-%dT%I:%M %p%Z", "%Y-%m-%dT%I:%M %p %Z",
-		"%Y-%m-%d %I:%M:%S%p%Z", "%Y-%m-%d %I:%M:%S%p %Z",
-		"%Y-%m-%dT%I:%M:%S%p%Z", "%Y-%m-%dT%I:%M:%S%p %Z",
-		"%Y-%m-%d %I:%M:%S %p%Z", "%Y-%m-%d %I:%M:%S %p %Z",
-		"%Y-%m-%dT%I:%M:%S %p%Z", "%Y-%m-%dT%I:%M:%S %p %Z",
-		"%c%Z", "%c %Z",
-		"%x %X%Z", "%x %X %Z",
-		"%m/%d/%Y%Z", "%m/%d/%Y %Z",
-		"%m/%d/%y%Z", "%m/%d/%y %Z",
-		"%m/%d/%Y %H%M%Z", "%m/%d/%Y %H%M %Z",
-		"%m/%d/%Y %H:%M%Z", "%m/%d/%Y %H:%M %Z",
-		"%m/%d/%Y %H:%M:%S%Z", "%m/%d/%Y %H:%M:%S %Z",
-		"%m/%d/%Y %I:%M%p%Z", "%m/%d/%Y %I:%M%p %Z",
-		"%m/%d/%Y %I:%M %p%Z", "%m/%d/%Y %I:%M %p %Z",
-		"%m/%d/%Y %I:%M:%S%p%Z", "%m/%d/%Y %I:%M:%S%p %Z",
-		"%m/%d/%Y %I:%M:%S %p%Z", "%m/%d/%Y %I:%M:%S %p %Z",
-		"%Y/%m/%d %H%M%Z", "%Y/%m/%d %H%M %Z",
-		"%Y/%m/%d %H:%M%Z", "%Y/%m/%d %H:%M %Z",
-		"%Y/%m/%d %H:%M:%S%Z", "%Y/%m/%d %H:%M:%S %Z",
-		"%Y/%m/%d %I:%M%p%Z", "%Y/%m/%d %I:%M%p %Z",
-		"%Y/%m/%d %I:%M %p%Z", "%Y/%m/%d %I:%M %p %Z",
-		"%Y/%m/%d %I:%M:%S%p%Z", "%Y/%m/%d %I:%M:%S%p %Z",
-		"%Y/%m/%d %I:%M:%S %p%Z", "%Y/%m/%d %I:%M:%S %p %Z",
-		"%Y/%m/%d %X%Z", "%Y/%m/%d %X %Z",
-		"%b %d, %Y %X%Z", "%b %d, %Y %X %Z",
-		"%b %d, %Y %I:%M %p%Z", "%b %d, %Y %I:%M %p %Z",
-		"%b %d %Y %X%Z", "%b %d %Y %X %Z",
-		"%b %d %Y %I:%M %p%Z", "%b %d %Y %I:%M %p %Z",
-		"%d %b, %Y %X%Z", "%d %b, %Y %X %Z",
-		"%d %b, %Y %I:%M %p%Z", "%d %b, %Y %I:%M %p %Z",
-		"%d %b %Y %X%Z", "%d %b %Y %X %Z",
-		"%d %b %Y %I:%M %p%Z", "%d %b %Y %I:%M %p %Z",
-		"%b. %d, %Y %X%Z", "%b. %d, %Y %X %Z",
-		"%b. %d, %Y %I:%M %%Z", "%b. %d, %Y %I:%M %p %Z",
-		"%b. %d %Y %X%Z", "%b. %d %Y %X %Z",
-		"%b. %d %Y %I:%M %p%Z", "%b. %d %Y %I:%M %p %Z",
-		"%d %b., %Y %X%Z", "%d %b., %Y %X %Z",
-		"%d %b., %Y %I:%M %p%Z", "%d %b., %Y %I:%M %p %Z",
-		"%d %b. %Y %X%Z", "%d %b. %Y %X %Z",
-		"%d %b. %Y %I:%M %p%Z", "%d %b. %Y %I:%M %p %Z",
-		"%B %d, %Y %X%Z", "%B %d, %Y %X %Z",
-		"%B %d, %Y %I:%M %p%Z", "%B %d, %Y %I:%M %p %Z",
-		"%B %d %Y %X%Z", "%B %d %Y %X %Z",
-		"%B %d %Y %I:%M %p%Z", "%B %d %Y %I:%M %p %Z",
-		"%d %B, %Y %X%Z", "%d %B, %Y %X %Z",
-		"%d %B, %Y %I:%M %p%Z", "%d %B, %Y %I:%M %p %Z",
-		"%d %B %Y %X%Z", "%d %B %Y %X %Z",
-		"%d %B %Y %I:%M %p%Z", "%d %B %Y %I:%M %p %Z"
-		)
 	if type(data) == type(datetime.datetime.now()):
 		if data.tzinfo is None or data.tzinfo.utcoffset(data) is None:
 			return None
 		return data
 	if not isinstance(data, str):
 		return None
 	dt = None
@@ -4303,50 +4314,57 @@
 		dt = parse_datetime(datestr)
 		if not dt:
 			return None
 		sign = -1 if sign=='-' else 1
 		return datetime.datetime(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second, tzinfo=Tz(sign, int(hr), int(min)))
 	except:
 		# Check for alphabetic timezone
-		for f in timestamptz_fmts:
+		for i,f in enumerate(timestamptz_fmts):
 			try:
 				dt = datetime.datetime.strptime(data, f)
+				if i:
+					del timestamptz_fmts[i]
+					timestamptz_fmts.appendleft(f)
 			except:
 				continue
 			break
 		return dt
 
+date_fmts = collections.deque(("%x",
+		"%Y-%m-%d",
+		"%Y/%m/%d",
+		"%m/%d/%Y",
+		"%d/%m/%Y",
+		"%b %d, %Y",
+		"%b %d %Y",
+		"%d %b, %Y",
+		"%d %b %Y",
+		"%b. %d, %Y",
+		"%b. %d %Y",
+		"%d %b., %Y",
+		"%d %b. %Y",
+		"%B %d, %Y",
+		"%B %d %Y",
+		"%d %B, %Y",
+		"%d %B %Y"
+		))
 def parse_date(data):
-	date_fmts = ("%x",
-			"%Y-%m-%d",
-			"%m/%d/%Y",
-			"%Y/%m/%d",
-			"%b %d, %Y",
-			"%b %d %Y",
-			"%d %b, %Y",
-			"%d %b %Y",
-			"%b. %d, %Y",
-			"%b. %d %Y",
-			"%d %b., %Y",
-			"%d %b. %Y",
-			"%B %d, %Y",
-			"%B %d %Y",
-			"%d %B, %Y",
-			"%d %B %Y"
-			)
 	if data is None:
 		return None
 	if isinstance(data, datetime.date):
 		return data
 	if not isinstance(data, str):
 		return None
-	for f in date_fmts:
+	for i,f in enumerate(date_fmts):
 		try:
 			dt = datetime.datetime.strptime(data, f)
 			dtt = datetime.date(dt.year, dt.month, dt.day)
+			if i:
+				del date_fmts[i]
+				date_fmts.appendleft(f)
 		except:
 			continue
 		break
 	else:
 		return None
 	return dtt
```

### Comparing `mapdata-2.8.1/mapdata.egg-info/PKG-INFO` & `mapdata-2.8.2/mapdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.8.1
+Version: 2.8.2
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.8.1/setup.py` & `mapdata-2.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.8.1',
+	version='2.8.2',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```

