# Comparing `tmp/hun-date-parser-0.2.1.tar.gz` & `tmp/hun-date-parser-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hun-date-parser-0.2.1.tar", last modified: Tue Jun 27 17:00:37 2023, max compression
+gzip compressed data, was "hun-date-parser-0.2.2.tar", last modified: Fri Jun 30 12:26:20 2023, max compression
```

## Comparing `hun-date-parser-0.2.1.tar` & `hun-date-parser-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/
--rw-rw-rw-   0        0        0     1035 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     6246 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5310 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.705688 hun-date-parser-0.2.1/hun_date_parser/
--rw-rw-rw-   0        0        0      360 2023-06-27 16:54:15.000000 hun-date-parser-0.2.1/hun_date_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.768663 hun-date-parser-0.2.1/hun_date_parser/date_parser/
--rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/__init__.py
--rw-rw-rw-   0        0        0    18115 2023-06-26 19:18:51.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/date_parsers.py
--rw-rw-rw-   0        0        0    13981 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/datetime_extractor.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.784322 hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/
--rw-rw-rw-   0        0        0      226 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/__init__.py
--rw-rw-rw-   0        0        0     5922 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
--rw-rw-rw-   0        0        0     4242 2023-06-27 16:30:16.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/patterns.py
--rw-rw-rw-   0        0        0     1212 2022-01-12 18:11:18.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/structure_parsers.py
--rw-rw-rw-   0        0        0     9111 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_parser/time_parsers.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.799906 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/
--rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/__init__.py
--rw-rw-rw-   0        0        0     1439 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/date2text.py
--rw-rw-rw-   0        0        0     2212 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/datetime_textualizer.py
--rw-rw-rw-   0        0        0     4336 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/date_textualizer/time2text.py
--rw-rw-rw-   0        0        0     4159 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/hun_date_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.737407 hun-date-parser-0.2.1/hun_date_parser.egg-info/
--rw-rw-rw-   0        0        0     6246 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1097 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 17:00:37.000000 hun-date-parser-0.2.1/hun_date_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1221 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:37.862942 hun-date-parser-0.2.1/test/
--rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/test/__init__.py
--rw-rw-rw-   0        0        0    14885 2023-06-27 16:31:59.000000 hun-date-parser-0.2.1/test/test_date_parsers.py
--rw-rw-rw-   0        0        0     2939 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_datetime2text.py
--rw-rw-rw-   0        0        0    11729 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_datetime_extractor.py
--rw-rw-rw-   0        0        0     1531 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_exposed.py
--rw-rw-rw-   0        0        0     4249 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_restricted_parsing.py
--rw-rw-rw-   0        0        0     1498 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_structure_parsers.py
--rw-rw-rw-   0        0        0     4417 2023-06-26 17:59:37.000000 hun-date-parser-0.2.1/test/test_time_parsers.py
--rw-rw-rw-   0        0        0     1074 2021-10-11 13:03:22.000000 hun-date-parser-0.2.1/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:26:20.659019 hun-date-parser-0.2.2/
+-rw-rw-rw-   0        0        0     1035 2021-10-11 13:03:22.000000 hun-date-parser-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     6246 2023-06-30 12:26:20.659019 hun-date-parser-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5310 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 12:26:20.340218 hun-date-parser-0.2.2/hun_date_parser/
+-rw-rw-rw-   0        0        0      360 2023-06-30 12:18:25.000000 hun-date-parser-0.2.2/hun_date_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:26:20.452873 hun-date-parser-0.2.2/hun_date_parser/date_parser/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/__init__.py
+-rw-rw-rw-   0        0        0    18115 2023-06-26 19:18:51.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/date_parsers.py
+-rw-rw-rw-   0        0        0    13981 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/datetime_extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:26:20.494389 hun-date-parser-0.2.2/hun_date_parser/date_parser/interval_restriction/
+-rw-rw-rw-   0        0        0      226 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/interval_restriction/__init__.py
+-rw-rw-rw-   0        0        0     5922 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
+-rw-rw-rw-   0        0        0     4250 2023-06-30 12:13:09.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/patterns.py
+-rw-rw-rw-   0        0        0     1212 2022-01-12 18:11:18.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/structure_parsers.py
+-rw-rw-rw-   0        0        0     9111 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/hun_date_parser/date_parser/time_parsers.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:26:20.531565 hun-date-parser-0.2.2/hun_date_parser/date_textualizer/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.2/hun_date_parser/date_textualizer/__init__.py
+-rw-rw-rw-   0        0        0     1439 2021-10-11 13:03:22.000000 hun-date-parser-0.2.2/hun_date_parser/date_textualizer/date2text.py
+-rw-rw-rw-   0        0        0     2212 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/hun_date_parser/date_textualizer/datetime_textualizer.py
+-rw-rw-rw-   0        0        0     4336 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/hun_date_parser/date_textualizer/time2text.py
+-rw-rw-rw-   0        0        0     4159 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/hun_date_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:26:20.374808 hun-date-parser-0.2.2/hun_date_parser.egg-info/
+-rw-rw-rw-   0        0        0     6246 2023-06-30 12:26:20.000000 hun-date-parser-0.2.2/hun_date_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1097 2023-06-30 12:26:20.000000 hun-date-parser-0.2.2/hun_date_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:26:20.000000 hun-date-parser-0.2.2/hun_date_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-30 12:26:20.000000 hun-date-parser-0.2.2/hun_date_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-30 12:26:20.000000 hun-date-parser-0.2.2/hun_date_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 12:26:20.659019 hun-date-parser-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:26:20.659019 hun-date-parser-0.2.2/test/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.2/test/__init__.py
+-rw-rw-rw-   0        0        0    15888 2023-06-30 12:19:51.000000 hun-date-parser-0.2.2/test/test_date_parsers.py
+-rw-rw-rw-   0        0        0     2939 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/test/test_datetime2text.py
+-rw-rw-rw-   0        0        0    11729 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/test/test_datetime_extractor.py
+-rw-rw-rw-   0        0        0     1531 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/test/test_exposed.py
+-rw-rw-rw-   0        0        0     4249 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/test/test_restricted_parsing.py
+-rw-rw-rw-   0        0        0     1498 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/test/test_structure_parsers.py
+-rw-rw-rw-   0        0        0     4417 2023-06-26 17:59:37.000000 hun-date-parser-0.2.2/test/test_time_parsers.py
+-rw-rw-rw-   0        0        0     1074 2021-10-11 13:03:22.000000 hun-date-parser-0.2.2/test/test_utils.py
```

### Comparing `hun-date-parser-0.2.1/LICENSE` & `hun-date-parser-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/PKG-INFO` & `hun-date-parser-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hun-date-parser
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.
 Home-page: https://github.com/szegedai/hun-date-parser
 Author: Soma Nagy
 Author-email: nagysomabalint@gmail.com
 License: UNKNOWN
 Description: <h1 align="center">Hungarian Date Parser</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.1 Summary: A tool for
+Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.2 Summary: A tool for
 extracting datetime intervals from Hungarian sentences and turning datetime
 objects into Hungarian text. Home-page: https://github.com/szegedai/hun-date-
 parser Author: Soma Nagy Author-email: nagysomabalint@gmail.com License:
 UNKNOWN Description:
                       ****** Hungarian Date Parser ******
  A tool for extracting datetime intervals from Hungarian sentences and turning
                      datetime objects into Hungarian text.
```

### Comparing `hun-date-parser-0.2.1/README.md` & `hun-date-parser-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_parser/date_parsers.py` & `hun-date-parser-0.2.2/hun_date_parser/date_parser/date_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_parser/datetime_extractor.py` & `hun-date-parser-0.2.2/hun_date_parser/date_parser/datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py` & `hun-date-parser-0.2.2/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_parser/patterns.py` & `hun-date-parser-0.2.2/hun_date_parser/date_parser/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 # schemas
 R_TOLIG = r'(.*-?t[oóöő]l\b)(.*-?ig\b)'
 R_TOL = r'([:\w ]*-?t[oóöő]l\b).*'
 R_IG = r'([:\w ]*-?ig\b)'
 
 # hyper day level patterns
-R_ISO_DATE = r'(\b\d{4,4})(?:[-\\/\. ](1[0-2]|0?[1-9]))?(?:[-\\/\. ](1[0-9]|2[0-9]|3[01]|0?[1-9]))?'
-R_REV_ISO_DATE = r'\b(1[0-9]|2[0-9]|3[01]|0?[1-9])[-\\/\. ](1[0-2]|0?[1-9])[-\\/\. ](\b\d{4,4})'
+R_ISO_DATE = r'(\b\d{4,4})(?:[-\\/\. ] ?(1[0-2]|0?[1-9]))?(?:[-\\/\. ] ?(1[0-9]|2[0-9]|3[01]|0?[1-9]))?'
+R_REV_ISO_DATE = r'\b(1[0-9]|2[0-9]|3[01]|0?[1-9])[-\\/\. ] ?(1[0-2]|0?[1-9])[-\\/\. ] ?(\b\d{4,4})'
 R_NAMED_MONTH = r'(j[oöő]v[oöő].*?|tavaly.*?)?(\bjan(?:\b|\.|u[aá]r){1}|\bfeb(?:\b|r\.|\.|ru[aá]r){1}|\bm[aá]r(?:\b|c\b|c\.|\.|cius){1}|\b[aá]pr(?:\b|\.|ilis){1}\b|m[aá]j(?:\b|\.|us){1}|\bj[uú]n(?:\b|\.|ius){1}|\bj[uú]l(?:\b|\.|ius){1}|\baug(?:\b|\.|usztus){1}|\bszep(?:t\b|t\.|\b|\.|tember){1}|\bokt(?:\b|\.|[oó]ber){1}|\bnov(?:\b|\.|ember){1}|\bdec(?:\b|\.|ember){1})(?: ([1-3][0-9]|[1-9]))?'
 R_RELATIVE_MONTH = r'(?:(\blegut[oó]bbi|\butols[oó]|\bmúlt|\but[oó]bbi|\bezen|\bebben|\baktu[aá]lis|\bj[oöő]v[oöő]|\bk[oö]vetkez[oőö]|\bk[oö]vetkezend[oőö]).*)? a?h[oó]nap'
 
 R_WEEKDAY = r'(?:(el[oő]z[oő]|m[uú]lt|ezen|j[oöő]v[oöő]).*)?(h[eé]tf[oő]|kedd|szerd[aá]|cs[uü]t[oö]rt[oö]k|p[eé]ntek|szombat|vas[aá]rnap)'
 R_WEEK = r'(el[oő]z[oő] h[eé]t|m[uú]lt h[eé]t|m[uú]lth[eé]t|ezen a? h[eé]t|j[oöő]v[oöő]h[eé]t|j[oöő]v[oöő] h[eé]t)'
 
 R_TODAY = r'\b(má(?:tól|ra))\b|\b(ma)\b|\b(mai nap)\b'
```

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_parser/structure_parsers.py` & `hun-date-parser-0.2.2/hun_date_parser/date_parser/structure_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_parser/time_parsers.py` & `hun-date-parser-0.2.2/hun_date_parser/date_parser/time_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_textualizer/date2text.py` & `hun-date-parser-0.2.2/hun_date_parser/date_textualizer/date2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_textualizer/datetime_textualizer.py` & `hun-date-parser-0.2.2/hun_date_parser/date_textualizer/datetime_textualizer.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/date_textualizer/time2text.py` & `hun-date-parser-0.2.2/hun_date_parser/date_textualizer/time2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser/utils.py` & `hun-date-parser-0.2.2/hun_date_parser/utils.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/hun_date_parser.egg-info/PKG-INFO` & `hun-date-parser-0.2.2/hun_date_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hun-date-parser
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.
 Home-page: https://github.com/szegedai/hun-date-parser
 Author: Soma Nagy
 Author-email: nagysomabalint@gmail.com
 License: UNKNOWN
 Description: <h1 align="center">Hungarian Date Parser</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.1 Summary: A tool for
+Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.2 Summary: A tool for
 extracting datetime intervals from Hungarian sentences and turning datetime
 objects into Hungarian text. Home-page: https://github.com/szegedai/hun-date-
 parser Author: Soma Nagy Author-email: nagysomabalint@gmail.com License:
 UNKNOWN Description:
                       ****** Hungarian Date Parser ******
  A tool for extracting datetime intervals from Hungarian sentences and turning
                      datetime objects into Hungarian text.
```

### Comparing `hun-date-parser-0.2.1/hun_date_parser.egg-info/SOURCES.txt` & `hun-date-parser-0.2.2/hun_date_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/setup.py` & `hun-date-parser-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/test/test_date_parsers.py` & `hun-date-parser-0.2.2/test/test_date_parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,20 +80,29 @@
     ('2020-12-30-án', [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')]]),
     ('2020-12-30-án 2020.12.29',
      [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')],
       [Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(29, 'match_iso_date')]]),
     ('2020 12 30-án', [[Year(2020, 'match_iso_date'), Month(12, 'match_iso_date'), Day(30, 'match_iso_date')]]),
     ('a 1 1 1 b', []),
     ('abcd 2020 1 15 abd', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('abcd 2020. 1. 15. abd', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
     ('abcd 2020 01 15 abd', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
     ('2020 01 15', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('2020. 01. 15', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('2020. 01. 15.', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
     ('15 01 2020', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
     ('abcd 2020 01 15 10', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
     ('ekkor: 15-01-2020', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('ekkor: 15. 01. 2020', [[Year(2020, 'match_iso_date'), Month(1, 'match_iso_date'), Day(15, 'match_iso_date')]]),
+    ('ekkor: 01. 2020', [[Year(2020, 'match_iso_date')]]),
     ('ekkor 08 08 2023', [[Year(2023, 'match_iso_date'), Month(8, 'match_iso_date'), Day(8, 'match_iso_date')]]),
+    ('ekkor 08. 08. 2023.', [[Year(2023, 'match_iso_date'), Month(8, 'match_iso_date'), Day(8, 'match_iso_date')]]),
+    ('ekkor 2023. 08. 08. ', [[Year(2023, 'match_iso_date'), Month(8, 'match_iso_date'), Day(8, 'match_iso_date')]]),
+    ('ekkor 2023. 08. 08 abc', [[Year(2023, 'match_iso_date'), Month(8, 'match_iso_date'), Day(8, 'match_iso_date')]]),
+    ('ekkor 2023 08. 08 abc', [[Year(2023, 'match_iso_date'), Month(8, 'match_iso_date'), Day(8, 'match_iso_date')]]),
     ('ekkor 36 08 2023', [[Year(2023, 'match_iso_date')]]),
 ]
 
 tf_weekday = [
     ('múlt vasárnap', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(6, 'weekday')]], SearchScopes.NOT_RESTRICTED),
     ('ezen a heten hetfon', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(7, 'weekday')]], SearchScopes.NOT_RESTRICTED),
     ('jövő kedden', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(15, 'weekday')]], SearchScopes.NOT_RESTRICTED),
```

### Comparing `hun-date-parser-0.2.1/test/test_datetime2text.py` & `hun-date-parser-0.2.2/test/test_datetime2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/test/test_datetime_extractor.py` & `hun-date-parser-0.2.2/test/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/test/test_exposed.py` & `hun-date-parser-0.2.2/test/test_exposed.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/test/test_restricted_parsing.py` & `hun-date-parser-0.2.2/test/test_restricted_parsing.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/test/test_structure_parsers.py` & `hun-date-parser-0.2.2/test/test_structure_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/test/test_time_parsers.py` & `hun-date-parser-0.2.2/test/test_time_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.1/test/test_utils.py` & `hun-date-parser-0.2.2/test/test_utils.py`

 * *Files identical despite different names*

