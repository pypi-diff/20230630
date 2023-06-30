# Comparing `tmp/cleanphi-0.1.0-py3-none-any.whl.zip` & `tmp/cleanphi-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19303 bytes, number of entries: 11
+Zip file size: 19227 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Jun-23 10:35 phi/__init__.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 23-Jun-23 10:36 phi/constants.py
 -rw-rw-rw-  2.0 fat      882 b- defN 23-Jun-23 10:37 phi/extra.py
--rw-rw-rw-  2.0 fat     5326 b- defN 23-Jun-23 10:48 phi/main.py
--rw-rw-rw-  2.0 fat     2509 b- defN 23-Jun-24 01:55 phi/scikit.py
+-rw-rw-rw-  2.0 fat     5184 b- defN 23-Jun-30 09:22 phi/main.py
+-rw-rw-rw-  2.0 fat     2521 b- defN 23-Jun-30 09:22 phi/scikit.py
 -rw-rw-rw-  2.0 fat      245 b- defN 23-Jun-23 10:48 phi/utils.py
--rw-rw-rw-  2.0 fat    35802 b- defN 23-Jun-24 03:21 cleanphi-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2817 b- defN 23-Jun-24 03:21 cleanphi-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 03:21 cleanphi-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 03:21 cleanphi-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      808 b- defN 23-Jun-24 03:21 cleanphi-0.1.0.dist-info/RECORD
-11 files, 51372 bytes uncompressed, 17959 bytes compressed:  65.0%
+-rw-rw-rw-  2.0 fat    35802 b- defN 23-Jun-30 09:24 cleanphi-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2860 b- defN 23-Jun-30 09:24 cleanphi-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 09:24 cleanphi-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-30 09:24 cleanphi-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      808 b- defN 23-Jun-30 09:24 cleanphi-0.2.0.dist-info/RECORD
+11 files, 51285 bytes uncompressed, 17883 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: phi/scikit.py
 Comment: 
 
 Filename: phi/utils.py
 Comment: 
 
-Filename: cleanphi-0.1.0.dist-info/LICENSE
+Filename: cleanphi-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: cleanphi-0.1.0.dist-info/METADATA
+Filename: cleanphi-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cleanphi-0.1.0.dist-info/WHEEL
+Filename: cleanphi-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cleanphi-0.1.0.dist-info/top_level.txt
+Filename: cleanphi-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cleanphi-0.1.0.dist-info/RECORD
+Filename: cleanphi-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phi/main.py

```diff
@@ -15,18 +15,14 @@
 try:
     from unidecode import unidecode
 
 except ImportError:
     from unicodedata import normalize
 
     unidecode = lambda x: normalize("NFD", x).encode("ASCII", "ignore").decode("utf-8")
-    log.warning(
-        "Since the GPL-licensed package `unidecode` is not installed, using Python's `unicodedata` package which yields worse results."
-    )
-
 
 def fix_strange_quotes(text):
     text = constants.SINGLE_QUOTE_REGEX.sub("'", text)
     text = constants.DOUBLE_QUOTE_REGEX.sub('"', text)
     return text
 
 
@@ -35,36 +31,36 @@
         text = text.encode("latin", "backslashreplace").decode("unicode-escape")
     except:
         pass
 
     return fix_text(text, normalization=normalization)
 
 
-def to_ascii_unicode(text, lang="en", no_emoji=False):
+def to_ascii_unicode(text, lang="en", remove_emoji=False):
     text = fix_strange_quotes(text)
 
-    if not no_emoji:
+    if not remove_emoji:
         text = demojize(text, use_aliases=True)
 
-    lang = lang.lower()
+    lang = lang.to_lower()
     if lang == "de":
         text = save_replace(text, lang=lang)
 
     text = unidecode(text)
     
     if lang == "de":
         text = save_replace(text, lang=lang, back=True)
 
-    if not no_emoji:
+    if not remove_emoji:
         text = emojize(text, use_aliases=True)
 
     return text
 
 
-def normalize_whitespace(
+def remove_whitespace(
     text, no_line_breaks=False, strip_lines=True, keep_two_line_breaks=False
 ):
 
     if strip_lines:
         text = "\n".join([x.strip() for x in text.splitlines()])
 
     if no_line_breaks:
@@ -77,16 +73,16 @@
         else:
             text = constants.NONBREAKING_SPACE_REGEX.sub(
                 " ", constants.LINEBREAK_REGEX.sub(r"\n", text)
             )
 
     return text.strip()
 
-def _normalize_whitespace(*kwargs):
-    return normalize_whitespace(*kwargs)
+def _remove_whitespace(*kwargs):
+    return remove_whitespace(*kwargs)
 
 
 def replace_urls(text, replace_with="<URL>"):
     return constants.URL_REGEX.sub(replace_with, text)
 
 
 def replace_emails(text, replace_with="<EMAIL>"):
@@ -129,70 +125,70 @@
 
 def remove_emoji(text):
     return remove_substrings(text, UNICODE_EMOJI["en"])
 
 
 def clean(
     text,
-    fix_unicode=True,
+    unicode=True,
     to_ascii=True,
-    lower=True,
-    normalize_whitespace=True,
+    to_lower=True,
+    remove_whitespace=True,
     no_line_breaks=False,
     strip_lines=True,
     keep_two_line_breaks=False,
-    no_urls=False,
-    no_emails=False,
-    no_phone_numbers=False,
-    no_numbers=False,
-    no_digits=False,
-    no_currency_symbols=False,
-    no_punct=False,
-    no_emoji=False,
+    remove_url=False,
+    remove_email=False,
+    remove_ph=False,
+    remove_nums=False,
+    remove_digits=False,
+    remove_currency=False,
+    remove_punct=False,
+    remove_emoji=False,
     replace_with_url="<URL>",
     replace_with_email="<EMAIL>",
     replace_with_phone_number="<PHONE>",
     replace_with_number="<NUMBER>",
     replace_with_digit="0",
     replace_with_currency_symbol="<CUR>",
     replace_with_punct="",
     lang="en",
 ):
     if text is None:
         return ""
 
     text = str(text)
 
-    if fix_unicode:
+    if unicode:
         text = fix_bad_unicode(text)
-    if no_currency_symbols:
+    if remove_currency:
         text = replace_currency_symbols(text, replace_with_currency_symbol)
     if to_ascii:
-        text = to_ascii_unicode(text, lang=lang, no_emoji=no_emoji)
-    if no_urls:
+        text = to_ascii_unicode(text, lang=lang, remove_emoji=remove_emoji)
+    if remove_url:
         text = replace_urls(text, replace_with_url)
-    if no_emails:
+    if remove_email:
         text = replace_emails(text, replace_with_email)
-    if no_phone_numbers:
+    if remove_ph:
         text = replace_phone_numbers(text, replace_with_phone_number)
-    if no_numbers:
+    if remove_nums:
         text = replace_numbers(text, replace_with_number)
-    if no_digits:
+    if remove_digits:
         text = replace_digits(text, replace_with_digit)
-    if no_punct:
+    if remove_punct:
         if replace_with_punct == "":
             text = remove_punct(text)
         else:
             text = replace_punct(text, replace_with_punct)
 
-    if no_emoji and not to_ascii:
+    if remove_emoji and not to_ascii:
         text = remove_emoji(text)
 
-    if lower:
-        text = text.lower()
+    if to_lower:
+        text = text.to_lower()
 
-    if normalize_whitespace:
-        text = _normalize_whitespace(
+    if remove_whitespace:
+        text = _remove_whitespace(
             text, no_line_breaks, strip_lines, keep_two_line_breaks
         )
 
     return text
```

## phi/scikit.py

```diff
@@ -5,53 +5,53 @@
 
 from .main import clean
 
 
 class PhiTransformer(TransformerMixin, BaseEstimator):
     def __init__(
         self,
-        fix_unicode=True,
+        unicode=True,
         to_ascii=True,
-        lower=True,
-        normalize_whitespace=True,
+        to_lower=True,
+        remove_whitespace=True,
         no_line_breaks=False,
         strip_lines=True,
         keep_two_line_breaks=False,
-        no_urls=False,
-        no_emails=False,
-        no_phone_numbers=False,
-        no_numbers=False,
-        no_digits=False,
-        no_currency_symbols=False,
-        no_punct=False,
-        no_emoji=False,
+        remove_url=False,
+        remove_email=False,
+        remove_ph=False,
+        remove_nums=False,
+        remove_digits=False,
+        remove_currency=False,
+        remove_punct=False,
+        remove_emoji=False,
         replace_with_url="<URL>",
         replace_with_email="<EMAIL>",
         replace_with_phone_number="<PHONE>",
         replace_with_number="<NUMBER>",
         replace_with_digit="0",
         replace_with_currency_symbol="<CUR>",
         replace_with_punct="",
         lang="en",
     ):
-        self.fix_unicode = fix_unicode
+        self.unicode = unicode
         self.to_ascii = to_ascii
-        self.lower = lower
-        self.normalize_whitespace = normalize_whitespace
+        self.to_lower = to_lower
+        self.remove_whitespace = remove_whitespace
         self.no_line_breaks = no_line_breaks
         self.strip_lines = strip_lines
         self.keep_two_line_breaks = keep_two_line_breaks
-        self.no_urls = no_urls
-        self.no_emails = no_emails
-        self.no_phone_numbers = no_phone_numbers
-        self.no_numbers = no_numbers
-        self.no_digits = no_digits
-        self.no_currency_symbols = no_currency_symbols
-        self.no_punct = no_punct
-        self.no_emoji = no_emoji
+        self.remove_url = remove_url
+        self.remove_email = remove_email
+        self.remove_ph = remove_ph
+        self.remove_nums = remove_nums
+        self.remove_digits = remove_digits
+        self.remove_currency = remove_currency
+        self.remove_punct = remove_punct
+        self.remove_emoji = remove_emoji
         self.replace_with_url = replace_with_url
         self.replace_with_email = replace_with_email
         self.replace_with_phone_number = replace_with_phone_number
         self.replace_with_number = replace_with_number
         self.replace_with_digit = replace_with_digit
         self.replace_with_currency_symbol = replace_with_currency_symbol
         self.replace_with_punct = replace_with_punct
```

## Comparing `cleanphi-0.1.0.dist-info/LICENSE` & `cleanphi-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cleanphi-0.1.0.dist-info/METADATA` & `cleanphi-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanphi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Natural language processing framework to clean sentences and texts.
 Home-page: https://github.com/enginestein/Phi
 Author: Arya Praneil Pritesh
 Author-email: aryapraneil@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,25 +15,25 @@
 
 CleanPhi is a powerful Python framework designed to enhance text processing by effectively removing unwanted elements such as extraneous characters and unicodes. Leveraging the capabilities of natural language processing, CleanPhi provides a comprehensive set of functionalities, making it an invaluable tool for text cleaning and related tasks.
 
 ```python
 from CleanPhi import clean
 
 clean("some input",
-    fix_unicode=True,               # fix various unicode errors
+    unicode=True,               # fix various unicode errors
     to_ascii=True,                  # transliterate to closest ASCII representation
-    lower=True,                     # lowercase text
+    to_lower=True,                     # to_lowercase text
     no_line_breaks=False,           # fully strip line breaks as opposed to only normalizing them
-    no_urls=False,                  # replace all URLs with a special token
-    no_emails=False,                # replace all email addresses with a special token
-    no_phone_numbers=False,         # replace all phone numbers with a special token
-    no_numbers=False,               # replace all numbers with a special token
-    no_digits=False,                # replace all digits with a special token
-    no_currency_symbols=False,      # replace all currency symbols with a special token
-    no_punct=False,                 # remove punctuations
+    remove_url=False,                  # replace all URLs with a special token
+    remove_email=False,                # replace all email addresses with a special token
+    remove_ph=False,         # replace all phone numbers with a special token
+    remove_nums=False,               # replace all numbers with a special token
+    remove_digits=False,                # replace all digits with a special token
+    remove_currency=False,      # replace all currency symbols with a special token
+    remove_punct=False,                 # remove punctuations
     replace_with_punct="",          # instead of removing punctuations you may replace them
     replace_with_url="<URL>",
     replace_with_email="<EMAIL>",
     replace_with_phone_number="<PHONE>",
     replace_with_number="<NUMBER>",
     replace_with_digit="0",
     replace_with_currency_symbol="<CUR>",
@@ -43,25 +43,29 @@
 
 Choose an arguement and use the **clean** function in your code:
 
 ```python
 import CleanPhi
 text = "Hello, world!  Hello...\t \tworld?\n\nHello:\r\n\n\nWorld. "
 proc_text = "Hello, world! Hello... world?\nHello:\nWorld."
-assert CleanPhi.normalize_whitespace(text, no_line_breaks=False) == proc_text
-assert CleanPhi.normalize_whitespace(" dd\nd  ", no_line_breaks=True) == "dd d"
+assert CleanPhi.remove_whitespace(text, no_line_breaks=False) == proc_text
+assert CleanPhi.remove_whitespace(" dd\nd  ", no_line_breaks=True) == "dd d"
 ```
 
 ### To install CleanPhi in >=Python3.6
 
 ```powershell
 pip install CleanPhi
 ```
 
 ### Use CleanPhi with Scikit
 
 ```python
 from CleanPhi.scikit import PhiTransformer
 
-cleaner = PhiTransformer(no_punct=False, lower=False)
+cleaner = PhiTransformer(remove_punct=False, to_lower=False)
 cleaner.transform(['Clean text.', 'Natural language processing!'])
 ```
+
+# Version 0.2.0 
+
+- Bugs fixed
```

