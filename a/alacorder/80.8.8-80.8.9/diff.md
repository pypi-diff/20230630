# Comparing `tmp/alacorder-80.8.8.tar.gz` & `tmp/alacorder-80.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.8.8.tar", max compression
+gzip compressed data, was "alacorder-80.8.9.tar", max compression
```

## Comparing `alacorder-80.8.8.tar` & `alacorder-80.8.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.8/LICENSE
--rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.8/README.md
--rw-r--r--   0        0        0      697 2023-06-09 15:41:13.618598 alacorder-80.8.8/pyproject.toml
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.8/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.8/src/alacorder/__init__.py
--rw-r--r--   0        0        0   281467 2023-06-09 15:39:39.394890 alacorder-80.8.8/src/alacorder/__main__.py
--rw-r--r--   0        0        0   281467 2023-06-09 15:39:42.996108 alacorder-80.8.8/src/alacorder/alac.py
--rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 alacorder-80.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.9/LICENSE
+-rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.9/README.md
+-rw-r--r--   0        0        0      697 2023-06-30 15:20:31.008120 alacorder-80.8.9/pyproject.toml
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.9/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   293108 2023-06-30 15:20:17.400313 alacorder-80.8.9/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   293108 2023-06-30 15:20:10.717636 alacorder-80.8.9/src/alacorder/alac.py
+-rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 alacorder-80.8.9/PKG-INFO
```

### Comparing `alacorder-80.8.8/LICENSE` & `alacorder-80.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.8/README.md` & `alacorder-80.8.9/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.8/pyproject.toml` & `alacorder-80.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.8.8"
+version = "80.8.9"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.8.8/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.8.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.8/src/alacorder/__main__.py` & `alacorder-80.8.9/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
     polars ^0.18.1, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
-    pyarrow required to export summary to .xls, .xlsx,
-    Google Chrome required to fetch cases from Alacourt and crawl ADOC
+    Google Chrome required to fetch from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.8"
+version = "80.8.9"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1406,24 +1405,18 @@
     )
     cases = cases.sort("Name")
     if dest == None:
         pass
     elif os.path.splitext(dest)[1] == '.csv':
         cases.write_csv(dest)
     elif os.path.splitext(dest)[1] in ('.xls','.xlsx'):
-        try:
-            cases = cases.with_columns(
-                [
-                    pl.col("DOB").cast(pl.Utf8, strict=False)
-                ]
-            )
-            cases.to_pandas().to_excel(dest)
-        except:
-            popup("Warning: failsafe exported to .csv.", cf=window)
-            cases.write_csv(os.path.splitext(dest)[0]+".csv")
+        cases = cases.with_columns(
+            pl.col("DOB").cast(pl.Utf8, strict=False)
+        )
+        cases.write_excel(dest, autofit=True, float_precision=2)
     elif os.path.splitext(dest)[1] == '.parquet':
         cases.write_parquet(dest)
     elif os.path.splitext(dest)[1] == '.json':
         cases.write_json(dest)
     return cases
 
 
@@ -3376,15 +3369,15 @@
         {
             "download.default_directory": dirpath,  # Set default directory for downloads
             "download.prompt_for_download": False,  # To auto download the file
             "download.directory_upgrade": True,
             "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
         },
     )
-    print("Starting browser... Do not close while in progress!")
+    print("Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
@@ -3787,15 +3780,15 @@
             "prefs",
             {
                 "download.prompt_for_download": False,  # To auto download the file
                 "download.directory_upgrade": True,
                 "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
             },
         )
-    print("Starting browser... Do not close while in progress!")
+    print("Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd)
     return driver
 
 
 def case_number_search(case_number, driver):
     driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
@@ -3905,18 +3898,347 @@
             print(r['CaseNumber'])
             case_number_search(r['CaseNumber'], driver)
             df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
             window.write_event_value("PROGRESS-TEXT", i + 1)
             if dfpath and i % 10 == 0:
                 write(df.select(pl.exclude("CountyNumber", "Selection")), sheet_names=["adoc"], path=dfpath, overwrite=True)
         window.write_event_value("FETCH-CN-COMPLETE", True)
-    write(df, sheet_names=["adoc"], path=dfpath, overwrite=True)
+    if dfpath:
+        write(df, sheet_names=["adoc"], path=dfpath, overwrite=True)
     return df.select(pl.exclude("CountyNumber", "Selection"))
 
 
+def fetch_results_only(
+    query_path="",
+    output_path="",
+    cID="",
+    uID="",
+    pwd="",
+    criminal_only=False,
+    no_update=False,
+    debug=False,
+    window=None
+):
+    """
+    Retrieve search results from Alacourt.com.
+    Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and export to `output_path`.
+    Args:
+       query_path (str): Path to query table/spreadsheet (.xls, .xlsx)
+       output_path (str): Path to export table
+       cID (str): Customer ID on Alacourt.com
+       uID (str): User ID on Alacourt.com
+       pwd (str): Password on Alacourt.com
+       no_update (bool): Do not update query template after completion
+       debug (bool): Print detailed runtime information to console
+    """
+
+    query = read_query(query_path)
+
+    # start browser and authenticate
+    opt = webdriver.ChromeOptions()
+    opt.add_argument("--headless=new") 
+
+    print("Do not close while in progress!")
+    driver = webdriver.Chrome(options=opt)
+    login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
+    results = []
+    for i, r in enumerate(tqdm(query.rows(named=True))):
+        if query[i, "QUERY_COMPLETE"] == "Y":
+            continue
+        if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
+            login(driver, cID, uID, pwd, window=window)
+        result = party_search_results_table(
+            driver,
+            name=r["TEMP_NAME"],
+            party_type=r["TEMP_PARTY_TYPE"],
+            ssn=r["TEMP_SSN"],
+            dob=r["TEMP_DOB"],
+            county=r["TEMP_COUNTY"],
+            division=r["TEMP_DIVISION"],
+            case_year=r["TEMP_CASE_YEAR"],
+            filed_before=r["TEMP_FILED_BEFORE"],
+            filed_after=r["TEMP_FILED_AFTER"],
+            criminal_only=criminal_only,
+            window=window,
+        )
+        query[i, "QUERY_COMPLETE"] = "Y"
+        query[i, "RETRIEVED"] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+        if query_path != "":
+            write_query = query
+            for col in write_query.columns:
+                if "TEMP_" in col:
+                    write_query = write_query.drop(col)
+            write(query, sheet_names=["query"], path=query_path)
+        results += result
+        df = pl.DataFrame({'Row': results})
+        df = df.filter(pl.col("Row").eq("").is_not())
+        df = df.filter(pl.col("Row").str.contains("Page").is_not())
+        df = df.filter(pl.col("Row").str.contains("County").is_not())
+        df = df.with_columns(
+            [
+                pl.col("Row").str.extract(r'^([A-Z\s]+)').alias("Searched"),
+                pl.col("Row").str.extract(r'; (\d\d)').alias("County"),
+                pl.col("Row").str.extract(r'([A-Z]{2}\-\d\d\d\d\-\d\d\d\d\d\d\.\d\d)').alias("CaseNumber"),
+                pl.col("Row").str.extract(r'[A-Z]{2}\-\d\d\d\d\-\d\d\d\d\d\d\.\d\d\n(.+?) [A-Z\-]{3} ').alias("Name"),
+                pl.col("Row").str.extract(r' ([A-Z\-]{3}) ').alias("Code"),
+                pl.col("Row").str.extract(r' [A-Z\-]{3} ([A-Z\.\/\-\s]+)').str.rstrip(" B").str.replace("DISPOSED","").str.strip().alias("OriginalCharge"),
+                pl.col("Row").str.extract(r'(Bond|DISPOSED)').alias("Status"),
+                pl.col("Row").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("DOB"),
+                pl.col("Row").str.extract(r'\d\d?/\d\d?/\d\d\d\d ([A-Z]) ').alias("Sex"),
+                pl.col("Row").str.extract(r'\d\d?/\d\d?/\d\d\d\d [A-Z] ([A-Z])').alias("Race"),
+                pl.col("Row").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) See Detail').str.to_date('%m/%d/%Y', strict=False).alias("CourtActionDate"),
+                pl.col("Row").str.extract(r'(XXX-XX-X\d\d\d)$').alias("SSN")
+            ]
+        )
+        df = df.with_columns(
+            pl.when(pl.col("Name").str.contains(r"^([A-Z]+)$"))
+            .then(pl.concat_str([
+                pl.col("Name"),
+                pl.lit(" "),
+                pl.col("Code")
+            ]))
+            .otherwise(pl.col("Name"))
+            .alias("Name")
+        )
+        df = df.filter(pl.col("CaseNumber").is_null().is_not())
+        print(df.select(pl.exclude("Row")))
+        if output_path != "" and i % 10 == 0:
+            pass
+            write(df.select(pl.exclude("Row")).unique(), sheet_names=["results"], path=output_path)
+    if output_path != "":
+        write(df.select(pl.exclude("Row")).unique(), sheet_names=["results"], path=output_path)
+        pass
+    return df.select(pl.exclude("Row")).unique()
+
+
+def party_search_results_table(
+    driver,
+    name="",
+    party_type="",
+    ssn="",
+    dob="",
+    county="",
+    division="",
+    case_year="",
+    filed_before="",
+    filed_after="",
+    debug=False,
+    cID="",
+    uID="",
+    pwd="",
+    criminal_only=False,
+    window=None,
+):
+    """
+    Collect results table from SJIS Party Search Form from Alacourt.com
+
+    Args:
+        driver (WebDriver): selenium/chrome web driver object
+        name (str, optional): Name (LAST FIRST)
+        party_type (str, optional): "Defendants" | "Plaintiffs" | "ALL"
+        ssn (str, optional): Social Security Number
+        dob (str, optional): Date of Birth
+        county (str, optional): County
+        division (str, optional): "All Divisions"
+             "Criminal Only"
+             "Civil Only"
+             "CS - CHILD SUPPORT"
+             "CV - CIRCUIT - CIVIL"
+             "CC - CIRCUIT - CRIMINAL"
+             "DV - DISTRICT - CIVIL"
+             "DC - DISTRICT - CRIMINAL"
+             "DR - DOMESTIC RELATIONS"
+             "EQ - EQUITY-CASES"
+             "MC - MUNICIPAL-CRIMINAL"
+             "TP - MUNICIPAL-PARKING"
+             "SM - SMALL CLAIMS"
+             "TR - TRAFFIC"
+        case_year (str, optional): YYYY
+        filed_before (str, optional): M/DD/YYYY
+        filed_after (str, optional): M/DD/YYYY
+        cID (str): Customer ID on Alacourt.com
+        uID (str): User ID on Alacourt.com
+        pwd (str): Password on Alacourt.com
+        criminal_only (bool, optional): Only search criminal cases
+        debug (bool, optional): Print detailed logs.
+
+    Returns:
+        List[str] of URLs to PDF
+    """
+
+    if "frmIndexSearchForm" not in driver.current_url:
+        driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
+
+    has_window = False if window == "None" else True
+
+    # connection error
+    try:
+        party_name_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName"
+        )
+    except selenium.common.exceptions.NoSuchElementException:
+        dlog(
+            """NoSuchElementException on `party_name_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")`""",
+            cf=debug,
+        )
+        if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
+            time.sleep(2)
+            login(driver, cID=cID, uID=uID, pwd=pwd)
+            driver.implicitly_wait(1)
+        driver.get("https:v2.alacourt.com/frmIndexSearchForm.aspx")
+        print("Successfully connected and logged into Alacourt!")
+
+    # field search
+
+    time.sleep(0.5)
+
+    # name
+    if name != "":
+        driver.implicitly_wait(1)
+        try:
+            party_name_box.send_keys(name)
+        except selenium.common.exceptions.StaleElementReferenceException:
+            time.sleep(2)
+            driver.implicitly_wait(2)
+            party_name_box.send_keys(name)
+    # ssn
+    if ssn != "":
+        ssn_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN"
+        )
+        ssn_box.send_keys(ssn)
+    # dob
+    if dob != "":
+        date_of_birth_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtDOB"
+        )
+        date_of_birth_box.send_keys(dob)
+    # party type
+    if party_type == "Plaintiffs":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_0"
+        ).click()
+    if party_type == "Defendants":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_1"
+        ).click()
+    if party_type == "ALL":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_2"
+        ).click()
+    # division
+    if division == "" and not criminal_only:
+        division = "All Divisions"
+    if criminal_only:
+        division = "Criminal Only"
+    division_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_UcddlDivisions1_ddlDivision"
+    )
+    sdivision = Select(division_select)
+    sdivision.select_by_visible_text(division)
+    if county == "":
+        county = "Statewide Search"
+    county_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_ddlCounties"
+    )
+    scounty = Select(county_select)
+    scounty.select_by_visible_text(county)
+    if case_year != "" and case_year != None:
+        case_year_select = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear"
+        )
+        scase_year = Select(case_year_select)
+        scase_year.select_by_visible_text(str(case_year))
+    no_records_select = driver.find_element(
+        by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfRecords"
+    )
+    sno_records = Select(no_records_select)
+    sno_records.select_by_visible_text("1000")
+    if filed_before != "":
+        filed_before_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtFrom"
+        )
+        filed_before_box.send_keys(filed_before)
+    if filed_after != "":
+        filed_after_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo"
+        )
+        filed_after_box.send_keys(filed_after)
+
+    # submit search
+    search_button = driver.find_element(by=By.ID, value="searchButton")
+
+    time.sleep(0.25)
+
+    try:
+        search_button.click()
+    except:
+        driver.implicitly_wait(2)
+        time.sleep(2)
+
+    time.sleep(0.5)
+
+    dlog("Submitted party search form...", cf=debug)
+
+    # count pages
+    try:
+        page_counter = driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_dg_tcPageXofY"
+        ).text
+        pages = int(page_counter.strip()[-1])
+
+    except:
+        pages = 1
+
+    # count results
+    try:
+        results_indicator = driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_lblResultCount"
+        )
+        results_count = int(
+            results_indicator.text.replace("Search Results: ", "")
+            .replace(" records returned.", "")
+            .strip()
+        )
+        dlog(f"Found {results_count} results, fetching URLs and downloading PDFs...", cf=debug)
+    except:
+        results_count = 0
+
+    # get PDF links from each page
+
+    row_text = []
+
+    for i in range(0, pages):
+        table = driver.find_element(by=By.ID, value="ContentPlaceHolder1_dg")
+        rows = []
+        rows = table.find_elements(by=By.TAG_NAME, value="tr")
+        for row in rows:
+            try:
+                row_text += [name + "; " + row.text]
+            except:
+                pass
+        try:
+            pager_select = Select(
+                driver.find_element(
+                    by=By.NAME, value="ctl00$ContentPlaceHolder1$dg$ctl18$ddlPages"
+                )
+            )
+            next_pg = int(pager_select.text) + 1
+        except:
+            try:
+                next_button = driver.find_element(
+                    by=By.ID, value="ContentPlaceHolder1_dg_ibtnNext"
+                )
+                next_button.click()
+                driver.implicitly_wait(1)
+            except:
+                continue
+    return row_text
+
+
 def empty_query(path):
     """Create empty spreadsheet to fill and import as query submit search list to retrieve matching case records from Alacourt.com.
 
     Args:
         path (str): Desired output path (.xls, .xlsx)
 
     """
@@ -3956,20 +4278,19 @@
     return df
 
 
 def adoc_fetch(df=None, path=None, window=None, cf=None):
     if cf:
         df = read(cf['INPUTS'])
         path = cf['OUTPUT_PATH']
-    if df:
-        if isinstance(df, str):
-            dfpath = df
-            df = read(df)
-        else:
-            dfpath = None
+    if isinstance(df, str):
+        dfpath = df
+        df = read(df)
+    else:
+        dfpath = None
     if 'FirstName' not in df.columns or 'LastName' not in df.columns:
         df = make_adoc_fetch_queue_from_crawl(df)
     if 'Retrieved' not in df.columns:
         df = df.with_columns(pl.lit("").alias("Retrieved"))
     df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
     out = pl.DataFrame()
     opt = webdriver.ChromeOptions()
@@ -4055,15 +4376,15 @@
     sentences = sentences.with_row_count()
     details = details.with_row_count()
     inmate = inmate.select(
         [
             pl.lit(name).alias("Name"),
             pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
             pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
-             ),
+             ).str.rstrip("R").str.strip(),
             pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
             pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
             pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
             pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
             pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
             pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
             pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
@@ -4079,16 +4400,16 @@
         [
             pl.col("row_nr"),
             pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
             pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
             pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
             pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
             pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
+            pl.col("Tables").str.extract(r'(Concurrent|Consecutive)').alias("Type"),
+            pl.col("Tables").str.extract(r'([A-Z\s\.]+)$').str.strip().alias("County")
         ]
     )
     sentences = sentences.with_columns(
         [
             pl.when(pl.col("Type")=="C")
             .then("")
             .otherwise(pl.col("Type"))
@@ -4174,18 +4495,24 @@
             out = out.select(
                 [
                     pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
-                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                    pl.col("Rows").str.extract(r"^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s\.\'\&]+)").str.strip().alias("Institution"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
                 ]
             )
+            out = out.with_columns(
+                [
+                    pl.col("Institution").str.extract(r' ([DLB][RWBP])$').alias("Code"),
+                    pl.col("Institution").str.replace(r' ([DLB][RWBP])$','')
+                ]
+            )
             print(out)
             write(out, sheet_names=['inmates'], path=path, overwrite=True)
     if window:
         window.write_event_value("PROGRESS-TEXT", 0)
         window.write_event_value("PROGRESS-TEXT-TOTAL", len(alphabet))
         for i, x in enumerate(alphabet):
             last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
@@ -4265,15 +4592,16 @@
             ]
         ).alias("CaseNumber")
     )
     cn = cases_df.select(pl.col("CaseNumber").str.extract(r'([^\.]+)')).to_series().to_list()
     adoc_df = adoc_df.filter(pl.col("CaseNumber").is_in(cn).is_not())
     adoc_df = adoc_df.filter(pl.col("CaseNumber").is_null().is_not())
     adoc_df = adoc_df.unique("CaseNumber")
-    return adoc_df.select(pl.exclude("CaseNumber","CountyNumber"))
+    return adoc_df.select(pl.exclude("CountyNumber","Selection"))
+
 
 
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
 def loadgui():
     """
@@ -7857,7 +8185,8 @@
             bal = float(re.sub(r'\$','',splr[2]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
```

### Comparing `alacorder-80.8.8/src/alacorder/alac.py` & `alacorder-80.8.9/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
     polars ^0.18.1, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
-    pyarrow required to export summary to .xls, .xlsx,
-    Google Chrome required to fetch cases from Alacourt and crawl ADOC
+    Google Chrome required to fetch from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.8"
+version = "80.8.9"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1406,24 +1405,18 @@
     )
     cases = cases.sort("Name")
     if dest == None:
         pass
     elif os.path.splitext(dest)[1] == '.csv':
         cases.write_csv(dest)
     elif os.path.splitext(dest)[1] in ('.xls','.xlsx'):
-        try:
-            cases = cases.with_columns(
-                [
-                    pl.col("DOB").cast(pl.Utf8, strict=False)
-                ]
-            )
-            cases.to_pandas().to_excel(dest)
-        except:
-            popup("Warning: failsafe exported to .csv.", cf=window)
-            cases.write_csv(os.path.splitext(dest)[0]+".csv")
+        cases = cases.with_columns(
+            pl.col("DOB").cast(pl.Utf8, strict=False)
+        )
+        cases.write_excel(dest, autofit=True, float_precision=2)
     elif os.path.splitext(dest)[1] == '.parquet':
         cases.write_parquet(dest)
     elif os.path.splitext(dest)[1] == '.json':
         cases.write_json(dest)
     return cases
 
 
@@ -3376,15 +3369,15 @@
         {
             "download.default_directory": dirpath,  # Set default directory for downloads
             "download.prompt_for_download": False,  # To auto download the file
             "download.directory_upgrade": True,
             "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
         },
     )
-    print("Starting browser... Do not close while in progress!")
+    print("Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
@@ -3787,15 +3780,15 @@
             "prefs",
             {
                 "download.prompt_for_download": False,  # To auto download the file
                 "download.directory_upgrade": True,
                 "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
             },
         )
-    print("Starting browser... Do not close while in progress!")
+    print("Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd)
     return driver
 
 
 def case_number_search(case_number, driver):
     driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
@@ -3905,18 +3898,347 @@
             print(r['CaseNumber'])
             case_number_search(r['CaseNumber'], driver)
             df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
             window.write_event_value("PROGRESS-TEXT", i + 1)
             if dfpath and i % 10 == 0:
                 write(df.select(pl.exclude("CountyNumber", "Selection")), sheet_names=["adoc"], path=dfpath, overwrite=True)
         window.write_event_value("FETCH-CN-COMPLETE", True)
-    write(df, sheet_names=["adoc"], path=dfpath, overwrite=True)
+    if dfpath:
+        write(df, sheet_names=["adoc"], path=dfpath, overwrite=True)
     return df.select(pl.exclude("CountyNumber", "Selection"))
 
 
+def fetch_results_only(
+    query_path="",
+    output_path="",
+    cID="",
+    uID="",
+    pwd="",
+    criminal_only=False,
+    no_update=False,
+    debug=False,
+    window=None
+):
+    """
+    Retrieve search results from Alacourt.com.
+    Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and export to `output_path`.
+    Args:
+       query_path (str): Path to query table/spreadsheet (.xls, .xlsx)
+       output_path (str): Path to export table
+       cID (str): Customer ID on Alacourt.com
+       uID (str): User ID on Alacourt.com
+       pwd (str): Password on Alacourt.com
+       no_update (bool): Do not update query template after completion
+       debug (bool): Print detailed runtime information to console
+    """
+
+    query = read_query(query_path)
+
+    # start browser and authenticate
+    opt = webdriver.ChromeOptions()
+    opt.add_argument("--headless=new") 
+
+    print("Do not close while in progress!")
+    driver = webdriver.Chrome(options=opt)
+    login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
+    results = []
+    for i, r in enumerate(tqdm(query.rows(named=True))):
+        if query[i, "QUERY_COMPLETE"] == "Y":
+            continue
+        if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
+            login(driver, cID, uID, pwd, window=window)
+        result = party_search_results_table(
+            driver,
+            name=r["TEMP_NAME"],
+            party_type=r["TEMP_PARTY_TYPE"],
+            ssn=r["TEMP_SSN"],
+            dob=r["TEMP_DOB"],
+            county=r["TEMP_COUNTY"],
+            division=r["TEMP_DIVISION"],
+            case_year=r["TEMP_CASE_YEAR"],
+            filed_before=r["TEMP_FILED_BEFORE"],
+            filed_after=r["TEMP_FILED_AFTER"],
+            criminal_only=criminal_only,
+            window=window,
+        )
+        query[i, "QUERY_COMPLETE"] = "Y"
+        query[i, "RETRIEVED"] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+        if query_path != "":
+            write_query = query
+            for col in write_query.columns:
+                if "TEMP_" in col:
+                    write_query = write_query.drop(col)
+            write(query, sheet_names=["query"], path=query_path)
+        results += result
+        df = pl.DataFrame({'Row': results})
+        df = df.filter(pl.col("Row").eq("").is_not())
+        df = df.filter(pl.col("Row").str.contains("Page").is_not())
+        df = df.filter(pl.col("Row").str.contains("County").is_not())
+        df = df.with_columns(
+            [
+                pl.col("Row").str.extract(r'^([A-Z\s]+)').alias("Searched"),
+                pl.col("Row").str.extract(r'; (\d\d)').alias("County"),
+                pl.col("Row").str.extract(r'([A-Z]{2}\-\d\d\d\d\-\d\d\d\d\d\d\.\d\d)').alias("CaseNumber"),
+                pl.col("Row").str.extract(r'[A-Z]{2}\-\d\d\d\d\-\d\d\d\d\d\d\.\d\d\n(.+?) [A-Z\-]{3} ').alias("Name"),
+                pl.col("Row").str.extract(r' ([A-Z\-]{3}) ').alias("Code"),
+                pl.col("Row").str.extract(r' [A-Z\-]{3} ([A-Z\.\/\-\s]+)').str.rstrip(" B").str.replace("DISPOSED","").str.strip().alias("OriginalCharge"),
+                pl.col("Row").str.extract(r'(Bond|DISPOSED)').alias("Status"),
+                pl.col("Row").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("DOB"),
+                pl.col("Row").str.extract(r'\d\d?/\d\d?/\d\d\d\d ([A-Z]) ').alias("Sex"),
+                pl.col("Row").str.extract(r'\d\d?/\d\d?/\d\d\d\d [A-Z] ([A-Z])').alias("Race"),
+                pl.col("Row").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) See Detail').str.to_date('%m/%d/%Y', strict=False).alias("CourtActionDate"),
+                pl.col("Row").str.extract(r'(XXX-XX-X\d\d\d)$').alias("SSN")
+            ]
+        )
+        df = df.with_columns(
+            pl.when(pl.col("Name").str.contains(r"^([A-Z]+)$"))
+            .then(pl.concat_str([
+                pl.col("Name"),
+                pl.lit(" "),
+                pl.col("Code")
+            ]))
+            .otherwise(pl.col("Name"))
+            .alias("Name")
+        )
+        df = df.filter(pl.col("CaseNumber").is_null().is_not())
+        print(df.select(pl.exclude("Row")))
+        if output_path != "" and i % 10 == 0:
+            pass
+            write(df.select(pl.exclude("Row")).unique(), sheet_names=["results"], path=output_path)
+    if output_path != "":
+        write(df.select(pl.exclude("Row")).unique(), sheet_names=["results"], path=output_path)
+        pass
+    return df.select(pl.exclude("Row")).unique()
+
+
+def party_search_results_table(
+    driver,
+    name="",
+    party_type="",
+    ssn="",
+    dob="",
+    county="",
+    division="",
+    case_year="",
+    filed_before="",
+    filed_after="",
+    debug=False,
+    cID="",
+    uID="",
+    pwd="",
+    criminal_only=False,
+    window=None,
+):
+    """
+    Collect results table from SJIS Party Search Form from Alacourt.com
+
+    Args:
+        driver (WebDriver): selenium/chrome web driver object
+        name (str, optional): Name (LAST FIRST)
+        party_type (str, optional): "Defendants" | "Plaintiffs" | "ALL"
+        ssn (str, optional): Social Security Number
+        dob (str, optional): Date of Birth
+        county (str, optional): County
+        division (str, optional): "All Divisions"
+             "Criminal Only"
+             "Civil Only"
+             "CS - CHILD SUPPORT"
+             "CV - CIRCUIT - CIVIL"
+             "CC - CIRCUIT - CRIMINAL"
+             "DV - DISTRICT - CIVIL"
+             "DC - DISTRICT - CRIMINAL"
+             "DR - DOMESTIC RELATIONS"
+             "EQ - EQUITY-CASES"
+             "MC - MUNICIPAL-CRIMINAL"
+             "TP - MUNICIPAL-PARKING"
+             "SM - SMALL CLAIMS"
+             "TR - TRAFFIC"
+        case_year (str, optional): YYYY
+        filed_before (str, optional): M/DD/YYYY
+        filed_after (str, optional): M/DD/YYYY
+        cID (str): Customer ID on Alacourt.com
+        uID (str): User ID on Alacourt.com
+        pwd (str): Password on Alacourt.com
+        criminal_only (bool, optional): Only search criminal cases
+        debug (bool, optional): Print detailed logs.
+
+    Returns:
+        List[str] of URLs to PDF
+    """
+
+    if "frmIndexSearchForm" not in driver.current_url:
+        driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
+
+    has_window = False if window == "None" else True
+
+    # connection error
+    try:
+        party_name_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName"
+        )
+    except selenium.common.exceptions.NoSuchElementException:
+        dlog(
+            """NoSuchElementException on `party_name_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")`""",
+            cf=debug,
+        )
+        if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
+            time.sleep(2)
+            login(driver, cID=cID, uID=uID, pwd=pwd)
+            driver.implicitly_wait(1)
+        driver.get("https:v2.alacourt.com/frmIndexSearchForm.aspx")
+        print("Successfully connected and logged into Alacourt!")
+
+    # field search
+
+    time.sleep(0.5)
+
+    # name
+    if name != "":
+        driver.implicitly_wait(1)
+        try:
+            party_name_box.send_keys(name)
+        except selenium.common.exceptions.StaleElementReferenceException:
+            time.sleep(2)
+            driver.implicitly_wait(2)
+            party_name_box.send_keys(name)
+    # ssn
+    if ssn != "":
+        ssn_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN"
+        )
+        ssn_box.send_keys(ssn)
+    # dob
+    if dob != "":
+        date_of_birth_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtDOB"
+        )
+        date_of_birth_box.send_keys(dob)
+    # party type
+    if party_type == "Plaintiffs":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_0"
+        ).click()
+    if party_type == "Defendants":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_1"
+        ).click()
+    if party_type == "ALL":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_2"
+        ).click()
+    # division
+    if division == "" and not criminal_only:
+        division = "All Divisions"
+    if criminal_only:
+        division = "Criminal Only"
+    division_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_UcddlDivisions1_ddlDivision"
+    )
+    sdivision = Select(division_select)
+    sdivision.select_by_visible_text(division)
+    if county == "":
+        county = "Statewide Search"
+    county_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_ddlCounties"
+    )
+    scounty = Select(county_select)
+    scounty.select_by_visible_text(county)
+    if case_year != "" and case_year != None:
+        case_year_select = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear"
+        )
+        scase_year = Select(case_year_select)
+        scase_year.select_by_visible_text(str(case_year))
+    no_records_select = driver.find_element(
+        by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfRecords"
+    )
+    sno_records = Select(no_records_select)
+    sno_records.select_by_visible_text("1000")
+    if filed_before != "":
+        filed_before_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtFrom"
+        )
+        filed_before_box.send_keys(filed_before)
+    if filed_after != "":
+        filed_after_box = driver.find_element(
+            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo"
+        )
+        filed_after_box.send_keys(filed_after)
+
+    # submit search
+    search_button = driver.find_element(by=By.ID, value="searchButton")
+
+    time.sleep(0.25)
+
+    try:
+        search_button.click()
+    except:
+        driver.implicitly_wait(2)
+        time.sleep(2)
+
+    time.sleep(0.5)
+
+    dlog("Submitted party search form...", cf=debug)
+
+    # count pages
+    try:
+        page_counter = driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_dg_tcPageXofY"
+        ).text
+        pages = int(page_counter.strip()[-1])
+
+    except:
+        pages = 1
+
+    # count results
+    try:
+        results_indicator = driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_lblResultCount"
+        )
+        results_count = int(
+            results_indicator.text.replace("Search Results: ", "")
+            .replace(" records returned.", "")
+            .strip()
+        )
+        dlog(f"Found {results_count} results, fetching URLs and downloading PDFs...", cf=debug)
+    except:
+        results_count = 0
+
+    # get PDF links from each page
+
+    row_text = []
+
+    for i in range(0, pages):
+        table = driver.find_element(by=By.ID, value="ContentPlaceHolder1_dg")
+        rows = []
+        rows = table.find_elements(by=By.TAG_NAME, value="tr")
+        for row in rows:
+            try:
+                row_text += [name + "; " + row.text]
+            except:
+                pass
+        try:
+            pager_select = Select(
+                driver.find_element(
+                    by=By.NAME, value="ctl00$ContentPlaceHolder1$dg$ctl18$ddlPages"
+                )
+            )
+            next_pg = int(pager_select.text) + 1
+        except:
+            try:
+                next_button = driver.find_element(
+                    by=By.ID, value="ContentPlaceHolder1_dg_ibtnNext"
+                )
+                next_button.click()
+                driver.implicitly_wait(1)
+            except:
+                continue
+    return row_text
+
+
 def empty_query(path):
     """Create empty spreadsheet to fill and import as query submit search list to retrieve matching case records from Alacourt.com.
 
     Args:
         path (str): Desired output path (.xls, .xlsx)
 
     """
@@ -3956,20 +4278,19 @@
     return df
 
 
 def adoc_fetch(df=None, path=None, window=None, cf=None):
     if cf:
         df = read(cf['INPUTS'])
         path = cf['OUTPUT_PATH']
-    if df:
-        if isinstance(df, str):
-            dfpath = df
-            df = read(df)
-        else:
-            dfpath = None
+    if isinstance(df, str):
+        dfpath = df
+        df = read(df)
+    else:
+        dfpath = None
     if 'FirstName' not in df.columns or 'LastName' not in df.columns:
         df = make_adoc_fetch_queue_from_crawl(df)
     if 'Retrieved' not in df.columns:
         df = df.with_columns(pl.lit("").alias("Retrieved"))
     df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
     out = pl.DataFrame()
     opt = webdriver.ChromeOptions()
@@ -4055,15 +4376,15 @@
     sentences = sentences.with_row_count()
     details = details.with_row_count()
     inmate = inmate.select(
         [
             pl.lit(name).alias("Name"),
             pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
             pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
-             ),
+             ).str.rstrip("R").str.strip(),
             pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
             pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
             pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
             pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
             pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
             pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
             pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
@@ -4079,16 +4400,16 @@
         [
             pl.col("row_nr"),
             pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
             pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
             pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
             pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
             pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
+            pl.col("Tables").str.extract(r'(Concurrent|Consecutive)').alias("Type"),
+            pl.col("Tables").str.extract(r'([A-Z\s\.]+)$').str.strip().alias("County")
         ]
     )
     sentences = sentences.with_columns(
         [
             pl.when(pl.col("Type")=="C")
             .then("")
             .otherwise(pl.col("Type"))
@@ -4174,18 +4495,24 @@
             out = out.select(
                 [
                     pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
-                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                    pl.col("Rows").str.extract(r"^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s\.\'\&]+)").str.strip().alias("Institution"),
                     pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
                 ]
             )
+            out = out.with_columns(
+                [
+                    pl.col("Institution").str.extract(r' ([DLB][RWBP])$').alias("Code"),
+                    pl.col("Institution").str.replace(r' ([DLB][RWBP])$','')
+                ]
+            )
             print(out)
             write(out, sheet_names=['inmates'], path=path, overwrite=True)
     if window:
         window.write_event_value("PROGRESS-TEXT", 0)
         window.write_event_value("PROGRESS-TEXT-TOTAL", len(alphabet))
         for i, x in enumerate(alphabet):
             last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
@@ -4265,15 +4592,16 @@
             ]
         ).alias("CaseNumber")
     )
     cn = cases_df.select(pl.col("CaseNumber").str.extract(r'([^\.]+)')).to_series().to_list()
     adoc_df = adoc_df.filter(pl.col("CaseNumber").is_in(cn).is_not())
     adoc_df = adoc_df.filter(pl.col("CaseNumber").is_null().is_not())
     adoc_df = adoc_df.unique("CaseNumber")
-    return adoc_df.select(pl.exclude("CaseNumber","CountyNumber"))
+    return adoc_df.select(pl.exclude("CountyNumber","Selection"))
+
 
 
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
 def loadgui():
     """
@@ -7857,7 +8185,8 @@
             bal = float(re.sub(r'\$','',splr[2]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
```

### Comparing `alacorder-80.8.8/PKG-INFO` & `alacorder-80.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.8.8
+Version: 80.8.9
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

