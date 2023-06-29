# Comparing `tmp/exergenics-etl-1.5.2.tar.gz` & `tmp/exergenics-etl-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.5.2.tar", last modified: Thu Jun 29 05:31:18 2023, max compression
+gzip compressed data, was "exergenics-etl-1.5.3.tar", last modified: Thu Jun 29 23:21:18 2023, max compression
```

## Comparing `exergenics-etl-1.5.2.tar` & `exergenics-etl-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:18.720842 exergenics-etl-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 05:31:18.720842 exergenics-etl-1.5.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:18.716842 exergenics-etl-1.5.2/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:18.720842 exergenics-etl-1.5.2/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:18.720842 exergenics-etl-1.5.2/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56209 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:18.720842 exergenics-etl-1.5.2/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    41786 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-29 05:31:15.000000 exergenics-etl-1.5.2/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:31:18.720842 exergenics-etl-1.5.2/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 05:31:18.000000 exergenics-etl-1.5.2/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 05:31:18.000000 exergenics-etl-1.5.2/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 05:31:18.000000 exergenics-etl-1.5.2/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 05:31:18.000000 exergenics-etl-1.5.2/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 05:31:18.000000 exergenics-etl-1.5.2/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 05:31:18.720842 exergenics-etl-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 05:31:17.000000 exergenics-etl-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.484449 exergenics-etl-1.5.3/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.484449 exergenics-etl-1.5.3/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57393 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42150 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 23:21:17.000000 exergenics-etl-1.5.3/setup.py
```

### Comparing `exergenics-etl-1.5.2/LICENSE` & `exergenics-etl-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.2/app/exergenics_etl/__init__.py` & `exergenics-etl-1.5.3/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.2/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.5.3/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -798,31 +798,18 @@
             raise EtlError(errorMessage)
 
 
 class DatetimeParser():
     """A class to parse a Panda Series of timestamp strings. 
     """
 
-    def __init__(self, nTests=100):
-        """Constructs all the necessary attributes for the DatetimeParser object.
-
-        Args:
-            nTests (int, optional): The number of timestamp strings used to find the year position. Defaults to 100.
-        """
-        self.logger = Logger()
-        self.dtSeriesTemp = None
-        self.positionYear = None
-        self.positionDay = None
-        self.isShortYear = False  # Whether 2-digit year is used
-        self.nTests = nTests
-        self.containsTimeZone = False
-        self.dtFinalFormat = None
+    # Define class attributes
 
-        # define the bricks
-        self.bricks = re.compile(r"""
+    # Regex bricks
+    bricks = re.compile(r"""
                 (?(DEFINE)
                     (?P<year_def>[12]\d{3}) # 1 or 2 then followed by 3 digits
                     # (?P<year_short_def>\d{2})  
                     (?P<month_def>January|February|March|April|May|June|
                     July|August|September|October|November|December)
                     (?P<month_short_def>Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)
                     (?P<month_dec_def>(0?[1-9]|1[012]))  # 01, 1, 12 but not 13
@@ -832,33 +819,69 @@
                     (?P<hms_def>T?\d{1,2}:\d{2}:\d{2}) # 03:20:10 or 3:20:10
                     (?P<hmsf_def>T?\d{1,2}:\d{2}:\d{2}.\d{1,6})
                     (?P<hm_def>T?\d{1,2}:\d{2})  # T13:20 or 13:20
                     (?P<delim_def>([-/, ]+|(?<=\d|^)T))
                     (?P<ampm_def>am|pm|AM|PM)
                     (?P<timezone_def>[+-]\d{4}) # +HHMM or -HHMM
                     # TODO: complie time zone format +HH:MM and -HH:MM, e.g. -08:00
-                    (?P<timezone_name_def>UTC|EST|AEST|AEDT|NZDT|NZST) # TODO: timezone names & Z
+                    (?P<timezone_name_def>ACDT|ACST|ACT|ADT|AEDT|AEST|AFT|AKDT|AKST|
+                    ALMT|AMST|AMT|ANAST|ANAT|AQTT|ART|AST|AT|AWDT|AWST|AZOST|AZOT|AZT|
+                    AoE|BNT|BOT|BRST|BRT|BST|BTT|CAT|CCT|CDT|CEST|CET|CHADT|CHAST|CHOT|
+                    CHOST|CHST|CHUT|CIDST|CIST|CKT|CLST|CLT|COT|CST|CT|CVT|CWST|CXT|DAVT|
+                    DDUT|DFT|EASST|EAST|EAT|ECT|EDT|EEST|EET|EGST|EGT|EST|ET|FET|FJST|
+                    FJT|FKST|FKT|FNT|GALT|GAMT|GET|GFT|GILT|GMT|GST|GYT|HDT|HAEC|HST|HKT|
+                    HMT|HOVT|HST|ICT|IDT|IOT|IRDT|IRKST|IRKT|IRST|IST|JST|KALT|KGT|KOST|
+                    KRAT|KST|KUYT|LHST|LHST|LINT|MAGST|MAGT|MART|MAWT|MDT|MEST|MET|MHT|
+                    MIST|MIT|MMT|MSK|MST|MUT|MVT|MYT|NCT|NDT|NFT|NOVT|NPT|NST|NT|NUT|
+                    NZDT|NZST|OMSST|OMST|ORAT|PDT|PET|PETST|PETT|PGT|PHOT|PHT|PKT|PMDT|
+                    PMST|PONT|PST|PT|PWT|PYST|PYT|RET|ROTT|SAKT|SAMT|SAST|SBT|SCT|SDT|SGT|
+                    SLST|SRET|SRT|SST|SYOT|TAHT|TFT|TJT|TKT|TLT|TMT|TRT|TOT|TVT|ULAST|ULAT|
+                    UTC|UYST|UYT|UZT|VET|VLAST|VLAT|VOST|VUT|WAKT|WARST|WAST|WAT|WEST|WET|
+                    WFT|WGST|WGT|WIB|WIT|WITA|WST|WT|YAKST|YAKT|YAPT|YEKST|YEKT
+                    )
                 )
 
                 (?P<hmsf>^(?&hmsf_def)$)|(?P<hms>^(?&hms_def)$)|(?P<hm>^(?&hm_def)$)|(?P<year>^(?&year_def)$)|(?P<month>^(?&month_def)$)|
                 (?P<month_short>^(?&month_short_def)$)|(?P<month_dec>^(?&month_dec_def)$)|(?P<day>^(?&day_def)$)|
                 (?P<weekday>^(?&weekday_def)$)|(?P<weekday_short>^(?&weekday_short_def)$)|(?P<delim>^(?&delim_def)$)|
                 (?P<ampm>^(?&ampm_def)$)|(?P<timezone>^(?&timezone_def)$)|(?P<timezone_name>^(?&timezone_name_def)$)
                 #|(?P<year_short>^(?&year_short_def)$)|(?P<ms>^(?&ms_def)$)
                 """, re.VERBOSE)
-        # delim
-        self.delim = re.compile(r'([-/, ]+|(?<=\d)T)')
+        
+    # Delimiters used in timestamps
+    delim = re.compile(r'([-/, ]+|(?<=\d)T)')
+
+    # Format codes
+    formats = {'year': '%Y', 'year_short': '%y', 'month': '%B', 'month_dec': '%m', 'day': '%d', 'weekday': '%A',
+                    'hms': '%H:%M:%S', 'hmsf': '%H:%M:%S.%f',
+                    'hms_12': '%I:%M:%S', 'hmsf_12': '%I:%M:%S.%f',
+                    'hm_12': '%I:%M',
+                    'weekday_short': '%a', 'month_short': '%b', 'hm': '%H:%M', 'delim': '',
+                    'ampm': '%p', 'timezone': '%z', 'timezone_name': '%Z'}
 
-        # formats
-        self.formats = {'year': '%Y', 'year_short': '%y', 'month': '%B', 'month_dec': '%m', 'day': '%d', 'weekday': '%A',
-                        'hms': '%H:%M:%S', 'hmsf': '%H:%M:%S.%f',
-                        'hms_12': '%I:%M:%S', 'hmsf_12': '%I:%M:%S.%f',
-                        'hm_12': '%I:%M',
-                        'weekday_short': '%a', 'month_short': '%b', 'hm': '%H:%M', 'delim': '',
-                        'ampm': '%p', 'timezone': '%z', 'timezone_name': '%Z'}
+    def __init__(self, nTests=100):
+        """Constructs all the necessary attributes for the DatetimeParser object.
+
+        Args:
+            nTests (int, optional): The number of timestamp strings used to find the year position. Defaults to 100.
+        """
+        self.logger = Logger()
+        self.positionYear = None
+        self.positionDay = None
+        self.isShortYear = False  # Whether 2-digit year is used
+        self.nTests = nTests
+        self.containsTimeZone = False
+        self.dtFinalFormat = None
+    
+    def _reset_instance_attributes(self):
+        self.positionYear = None
+        self.positionDay = None
+        self.isShortYear = False
+        self.containsTimeZone = False
+        self.dtFinalFormat = None
 
     def _find_short_year_position(self, dtSeries: pd.Series) -> None:
         """ 
         Find the position of year with or without century 
         based on a series of timestamps. 
 
         Args:
@@ -1080,15 +1103,15 @@
                     raise EtlError('Cannot recognise date parts.')
 
         out = self._correct_format_code_for_AMPM(out)
 
         # Check and filter out time zone from datetime format code
         out = self._check_and_remove_time_zone(parts, out)
 
-        return "".join(out)
+        return "".join(out).strip()
 
     def _find_final_format(self, dtSeries: pd.Series) -> str:
         """Get the format for the whole timestamp series. 
 
         Args:
             dtSeries (pd.Series): Pandas Series containing timestamp strings.
 
@@ -1168,56 +1191,54 @@
         Raises:
             EtlError: Failed datetime parsing.
             Exception: For unknown errors.
 
         Returns:
             pd.Series: Panda Series of parsed datetime objects.
         """
-        self.dtSeriesTemp = dtSeries
+
         self.logger.info(
-            f'Showing the first and the last 2 of the timestamps BEFORE parsing: \n{pd.concat([self.dtSeriesTemp.head(2), self.dtSeriesTemp.tail(2)])}')
+            f'Showing the first and the last 2 of the timestamps BEFORE parsing: \n{pd.concat([dtSeries.head(2), dtSeries.tail(2)])}')
 
         # PARSE unix timestamps automatically without finding timestamp format
         if isUnixTimestamp:
             try:
-                dtObjects = pd.to_datetime(self.dtSeriesTemp, unit='s')
+                dtObjects = pd.to_datetime(dtSeries, unit='s')
             except Exception as e:
                 errorMessage = f'Parsing unix timestamps failed: {e}'
                 self.logger.error(errorMessage)
                 raise EtlError(f'Parsing timestamps failed.')
             else:
                 return dtObjects
             
         # FIND the timestamp format
         if self.dtFinalFormat is None:
-            self._find_final_format(self.dtSeriesTemp)
+            self._find_final_format(dtSeries)
         else:
             self.logger.info(
                 f'Datetime format has been found before: {self.dtFinalFormat}')
 
         # PARSE the whole timestamp series using the format found by self._find_final_format()
         try:
             # Try exact match to test the algo
             dtObjects = pd.to_datetime(
-                self.dtSeriesTemp, format=self.dtFinalFormat, exact=(not self.containsTimeZone))
+                dtSeries, format=self.dtFinalFormat, exact=(not self.containsTimeZone))
 
         except Exception as e:
             self.logger.warn(f'Parsing failed: {e}')
             try:
                 self.logger.warn('Redo finding format ...')
 
                 # Reset variables
-                self.positionYear = None
-                self.positionDay = None
-                self.isShortYear = False
-                self.containsTimeZone = False
+                self._reset_instance_attributes()
 
-                self._find_final_format(self.dtSeriesTemp)
+                # Retry finding datetime format
+                self._find_final_format(dtSeries)
                 dtObjects = pd.to_datetime(
-                    self.dtSeriesTemp, format=self.dtFinalFormat, exact=(not self.containsTimeZone))
+                    dtSeries, format=self.dtFinalFormat, exact=(not self.containsTimeZone))
                 self.logger.info('Second Parsing done')
             except EtlError as e:
                 errorMessage = f'Second parsing failed: {e}'
                 self.logger.error(errorMessage)
                 raise EtlError(f'Parsing timestamps failed. {str(e)}')
             except Exception as e:
                 self.logger.error(e)
```

### Comparing `exergenics-etl-1.5.2/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.5.3/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.2/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.5.3/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.2/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.5.3/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,22 @@
     from ..src.exergenics_etl import *
 except:
     path = os.getcwd()
     sys.path.insert(0, path)
     from app.exergenics_etl.src.logger import ETLLogger as Logger
     from app.exergenics_etl.src.exergenics_etl import *
 
+
 load_dotenv()
 
 logger = Logger(loggerName='UnitTest',
                 component='data_modules', subComponent='pre_merged')
 
 TEST_DATA_DIR = "app/exergenics_etl/test/testData"
 
-
 class TestCreateApiClass:
 
     @pytest.fixture(scope='class', params=['staging', 'production'])
     def my_valid_environment(self, request):
         return request.param
 
     @pytest.fixture(scope='class')
@@ -187,15 +187,15 @@
         assert '//' not in outputFilePath
 
 
 class TestGetFileNameListClass:
 
     @pytest.fixture(scope="class")
     def my_manual_zipfile(self):
-        return zipfile.ZipFile("app/exergenics_etl/test/testData/manual_zipfile.zip")
+        return zipfile.ZipFile(f"{TEST_DATA_DIR}/manual_zipfile.zip")
 
     def test_get_file_name_list(self, my_manual_zipfile):
         fileNames = get_file_name_list(my_manual_zipfile)
         assert len(fileNames) == 4
 
 
 class TestSkipRowsMachineClass:
@@ -241,56 +241,56 @@
         assert convertable_to_float(string) == expected
 
 
 class TestInputValidationClass:
 
     @pytest.fixture(scope='class')
     def my_check_for_wide_format_test_case_wide1(self):
-        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/wideData1.csv'
+        filePath = f'{TEST_DATA_DIR}/testData_check_for_wide_format/wideData1.csv'
         df = pd.read_csv(filePath)
         timestampColumnNames = ['ui::timestamp']
         return df, timestampColumnNames
     
     @pytest.fixture(scope='class')
     def my_check_for_wide_format_test_case_wide2(self):
-        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/wideData2.csv'
+        filePath = f'{TEST_DATA_DIR}/testData_check_for_wide_format/wideData2.csv'
         df = pd.read_csv(filePath)
         timestampColumnNames = ['Created time', 'Modified time']
         return df, timestampColumnNames
     
     @pytest.fixture(scope='class')
     def my_check_for_wide_format_test_case_long1(self):
         """Second test case for the _check_for_wide_format method where the 
         input is a long dataframe, and the names column is in the 1st 
         column."""
-        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/longData_nameColumnIn1stColumn.csv'
+        filePath = f'{TEST_DATA_DIR}/testData_check_for_wide_format/longData_nameColumnIn1stColumn.csv'
         df = pd.read_csv(filePath)
         namesColumnId = 0
         valuesColumnId = 1
         timestampColumnNames = ['ui::timestamp']
         return df, timestampColumnNames, namesColumnId, valuesColumnId
 
     @pytest.fixture(scope='class')
     def my_check_for_wide_format_test_case_long2(self):
         """Second test case for the _check_for_wide_format method where the 
         input is a long dataframe, and the names column is in the 2nd 
         column."""
-        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/longData_nameColumnIn2ndColumn.csv'
+        filePath = f'{TEST_DATA_DIR}/testData_check_for_wide_format/longData_nameColumnIn2ndColumn.csv'
         df = pd.read_csv(filePath)
         namesColumnId = 1
         valuesColumnId = 2
         timestampColumnNames = ['ui::timestamp']
         return df, timestampColumnNames, namesColumnId, valuesColumnId
     
     @pytest.fixture(scope='class')
     def my_check_for_wide_format_test_case_long3(self):
         """Second test case for the _check_for_wide_format method where the 
         input is a long dataframe, and the names column is in the 3rd 
         column."""
-        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/longData_nameColumnIn3rdColumn.csv'
+        filePath = f'{TEST_DATA_DIR}/testData_check_for_wide_format/longData_nameColumnIn3rdColumn.csv'
         df = pd.read_csv(filePath)
         namesColumnId = 2
         valuesColumnId = 1
         timestampColumnNames = ['ui::timestamp']
         return df, timestampColumnNames, namesColumnId, valuesColumnId
 
     @pytest.fixture(scope='class')
@@ -324,39 +324,39 @@
                 testLongDf, myTimestampColumnNames)
 
         assert errInfo.value.args[1] == expectedNamesColumnId
         assert errInfo.value.args[2] == expectedValuesColumnId
 
     def test_check_for_generic_header1(self, my_inputValidation_object):
         myDfSameName = pd.read_csv(
-            'app/exergenics_etl/test/testData/dfSameName.csv', parse_dates=['timepretty'])
+            f'{TEST_DATA_DIR}/dfSameName.csv', parse_dates=['timepretty'])
         myDfNew = pd.read_csv(
-            'app/exergenics_etl/test/testData/dfNew.csv', parse_dates=['timepretty'])
+            f'{TEST_DATA_DIR}/dfNew.csv', parse_dates=['timepretty'])
         myPointName = 'Ch1-kwr'
 
         assert not my_inputValidation_object.check_for_generic_header(
             myPointName, myDfSameName, myDfNew)
 
     def test_check_for_generic_header2(self, my_inputValidation_object):
         myDfSameName = pd.read_csv(
-            'app/exergenics_etl/test/testData/dfSameName_genericHeader.csv', parse_dates=['timepretty'])
+            f'{TEST_DATA_DIR}/dfSameName_genericHeader.csv', parse_dates=['timepretty'])
         myDfNew = pd.read_csv(
-            'app/exergenics_etl/test/testData/dfNew_genericHeader.csv', parse_dates=['timepretty'])
+            f'{TEST_DATA_DIR}/dfNew_genericHeader.csv', parse_dates=['timepretty'])
         myPointName = 'Value'
 
         with pytest.raises(EtlError):
             my_inputValidation_object.check_for_generic_header(
                 myPointName, myDfSameName, myDfNew)
 
     def test_check_for_generic_header_new(self, my_inputValidation_object):
         """Check if the two dataframes share a generic name that is not in our known, generic header name list."""
         myDfSameName = pd.read_csv(
-            'app/exergenics_etl/test/testData/dfSameName_newGenericHeader.csv', parse_dates=['timepretty'])
+            f'{TEST_DATA_DIR}/dfSameName_newGenericHeader.csv', parse_dates=['timepretty'])
         myDfNew = pd.read_csv(
-            'app/exergenics_etl/test/testData/dfNew_newGenericHeader.csv', parse_dates=['timepretty'])
+            f'{TEST_DATA_DIR}/dfNew_newGenericHeader.csv', parse_dates=['timepretty'])
         myPointName = 'Value'
 
         with pytest.raises(EtlError):
             my_inputValidation_object.check_for_generic_header(
                 myPointName, myDfSameName, myDfNew)
 
     @pytest.mark.parametrize("myTestTimestampHeader", ['timestamp', 'time stamp', 'ui::timestamp', 'ts', 'date', 'time', 'datetime', 'date/time'])
@@ -407,54 +407,54 @@
 
 
 class TestFindTimestampColumns:
 
     @pytest.fixture(scope='class')
     def my_test_case1(self):
         """Two timestamp column; not unix timestamps."""
-        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/two timestamp columns.csv"
+        filePath = f"{TEST_DATA_DIR}/testData_for_find_timestamp_column/two timestamp columns.csv"
         df = pd.read_csv(filePath)
         myIsUnixTimestamp = False
         return df, myIsUnixTimestamp
 
     @pytest.fixture(scope='class')
     def my_test_case2(self):
         """Timestamps in the second column; not unix timestamps."""
-        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/timestamps in second column.csv"
+        filePath = f"{TEST_DATA_DIR}/testData_for_find_timestamp_column/timestamps in second column.csv"
         df = pd.read_csv(filePath)
         myIsUnixTimestamp = False
         return df, myIsUnixTimestamp
 
     @pytest.fixture(scope='class')
     def my_test_case3(self):
         """Timestamps in the second column and unix timestamps in the first column."""
-        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/timestamps in second column (unix timestamps in first column).csv"
+        filePath = f"{TEST_DATA_DIR}/testData_for_find_timestamp_column/timestamps in second column (unix timestamps in first column).csv"
         df = pd.read_csv(filePath)
         myIsUnixTimestamp = False
         return df, myIsUnixTimestamp
 
     @pytest.fixture(scope='class')
     def my_test_case4(self):
         """Timestamps in the third column; not unix timestamps."""
-        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/timestamps in third column.csv"
+        filePath = f"{TEST_DATA_DIR}/testData_for_find_timestamp_column/timestamps in third column.csv"
         df = pd.read_csv(filePath)
         myIsUnixTimestamp = False
         return df, myIsUnixTimestamp
 
     @pytest.fixture(scope='class')
     def my_test_case5(self):
         """No timestamp column found."""
-        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/no timestamp column.csv"
+        filePath = f"{TEST_DATA_DIR}/testData_for_find_timestamp_column/no timestamp column.csv"
         df = pd.read_csv(filePath)
         return df
     
     @pytest.fixture(scope='class')
     def my_test_case6(self):
         """Unix timestamps in the second column."""
-        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/unix_timestamps_in_second_column.csv"
+        filePath = f"{TEST_DATA_DIR}/testData_for_find_timestamp_column/unix_timestamps_in_second_column.csv"
         df = pd.read_csv(filePath)
         myIsUnixTimestamp = True
         return df, myIsUnixTimestamp
     
     @pytest.fixture(scope='class')
     def my_expected_timestamp_column_names(self):
         return ['Target column1', 'Target column2']
@@ -488,39 +488,39 @@
     def my_datetimeParser(self):
         datetimeParser = DatetimeParser()
         return datetimeParser
 
     @pytest.fixture
     def my_test_case_short_year_parsing(self):
         dtSeries = pd.read_csv(
-            "app/exergenics_etl/test/testData/timestamps_dayMonthShortYear.csv", header=None)[0]
+            f"{TEST_DATA_DIR}/timestamps_dayMonthShortYear.csv", header=None)[0]
         my_dtFinalFormat = '%d/%m/%y %H:%M'
         my_dtObjects = pd.to_datetime(dtSeries, format=my_dtFinalFormat)
         return dtSeries, my_dtObjects
 
     @pytest.fixture(scope='class')
     def my_test_case_ampm_parsing(self):
         dtSeries = pd.read_csv(
-            "app/exergenics_etl/test/testData/timestamps_ampm.csv", header=None)[0]
+            f"{TEST_DATA_DIR}/timestamps_ampm.csv", header=None)[0]
         my_dtFinalFormat = '%d/%m/%Y %I:%M %p'
         my_dtObjects = pd.to_datetime(dtSeries, format=my_dtFinalFormat)
         return dtSeries, my_dtObjects
 
     @pytest.fixture(scope='class')
     def my_test_case_time_zone_parsing(self):
         dtSeries = pd.read_csv(
-            "app/exergenics_etl/test/testData/timestamps_timeZones_1.csv", header=None)[0]  # TODO
+            f"{TEST_DATA_DIR}/timestamps_timeZones_1.csv", header=None)[0]  # TODO
         expected_output = pd.read_csv(
-            "app/exergenics_etl/test/testData/timestamps_timeZones_expectedOutput_1.csv", header=None)[0]
+            f"{TEST_DATA_DIR}/timestamps_timeZones_expectedOutput_1.csv", header=None)[0]
         return dtSeries, expected_output
 
     @pytest.fixture
     def my_test_dtSeries_with_unrecognisable_time_parts(self):
         dtSeries = pd.read_csv(
-            "app/exergenics_etl/test/testData/timestamps_unrecognisableParts.csv", header=None)[0]
+            f"{TEST_DATA_DIR}/timestamps_unrecognisableParts.csv", header=None)[0]
         return dtSeries
 
     @pytest.fixture
     def my_test_case_for_correcting_format_code_with_AMPM_and_seconds(self):
         my_format_code_list = ['%d', '-', '%b', '-',
                                '%y', ' ', '%H:%M:%S', ' ', '%p', ' ', '%Z']
         correct_format_code_list = ['%d', '-', '%b', '-',
@@ -581,14 +581,24 @@
     @pytest.fixture
     def my_non_unix_timestamp_flag(self):
         return False
     
     @pytest.fixture
     def my_unix_timestamp_flag(self):
         return True
+    
+    @pytest.mark.parametrize("testFile", ["test_remove_timezone_abbrev_AEST_AEDT.csv", "test_remove_timezone_abbrev_ACDT_ACST.csv", "test_remove_timezone_abbrev_NT_NUT.csv"])
+    def test_parse_timestamps_with_timezone_abbrev(self, testFile, my_datetimeParser, my_non_unix_timestamp_flag):
+        testDf = pd.read_csv(f"{TEST_DATA_DIR}/{testFile}")
+        expectedDtObject = pd.Series([pd.Timestamp('2023-09-13 05:12:41.211'),
+                            pd.Timestamp('2024-03-13 05:12:41.211'),
+                            pd.Timestamp('2025-03-13 05:12:41.211'),
+                            pd.Timestamp('2026-03-13 05:12:41.211')])
+        
+        assert my_datetimeParser.parse(testDf['Timestamp'], my_non_unix_timestamp_flag).equals(expectedDtObject)
 
     def test_parse_for_short_year(self, my_datetimeParser, my_test_case_short_year_parsing, my_non_unix_timestamp_flag):
         dtSeries, my_dtObjects = my_test_case_short_year_parsing
         assert my_datetimeParser.dtFinalFormat is None
         dtObjects = my_datetimeParser.parse(dtSeries, my_non_unix_timestamp_flag)
         assert my_datetimeParser.dtFinalFormat is not None
         assert dtObjects.equals(my_dtObjects)
@@ -603,22 +613,22 @@
     def test_checkTimeZone_for_timestamps_with_time_zones(self, my_datetimeParser, my_test_case_time_zone_parsing, my_non_unix_timestamp_flag):
         dtSeries, expected_output = my_test_case_time_zone_parsing
         dtObjects = my_datetimeParser.parse(dtSeries, my_non_unix_timestamp_flag)
         assert my_datetimeParser.containsTimeZone
 
     def test_find_day_position_when_timestamps_inadequate(self, my_datetimeParser):
         myTestDtSeries = pd.read_csv(
-            "app/exergenics_etl/test/testData/timestamps_findDayPosition.csv", header=None)[0]
+            f"{TEST_DATA_DIR}/timestamps_findDayPosition.csv", header=None)[0]
         positionDay = my_datetimeParser._find_day_position(
             myTestDtSeries)
         assert positionDay == DEFAULT_POSITION_DAY
 
     def test_find_day_position_for_finding_day_large_than_12(self, my_datetimeParser):
         myTestDtSeries = pd.read_csv(
-            "app/exergenics_etl/test/testData/timestamps_findDayPosition_2.csv", header=None)[0]
+            f"{TEST_DATA_DIR}/timestamps_findDayPosition_2.csv", header=None)[0]
         positionDay = my_datetimeParser._find_day_position(
             myTestDtSeries)  # TODO
         my_expected_day_position_2 = 2
         assert positionDay == my_expected_day_position_2
 
     def test_removeTimeZone_for_timestamps_with_time_zones(self, my_datetimeParser, my_test_case_for_removing_time_zone_from_timestamps_with_time_zones):
         myDatetimeParts, myFormatCodeList, expectedFormatCodeList = my_test_case_for_removing_time_zone_from_timestamps_with_time_zones
```

### Comparing `exergenics-etl-1.5.2/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.5.3/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.2/setup.py` & `exergenics-etl-1.5.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.5.2",
+    version="v1.5.3",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

