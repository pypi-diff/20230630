# Comparing `tmp/citation_utils-0.4.6.tar.gz` & `tmp/citation_utils-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.4.6.tar", max compression
+gzip compressed data, was "citation_utils-0.4.7.tar", max compression
```

## Comparing `citation_utils-0.4.6.tar` & `citation_utils-0.4.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.6/LICENSE
--rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.6/citation_utils/__init__.py
--rw-r--r--   0        0        0    17249 2023-06-29 03:32:43.795636 citation_utils-0.4.6/citation_utils/citation.py
--rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.6/citation_utils/dockets/__init__.py
--rw-r--r--   0        0        0     3125 2023-06-29 03:28:48.048714 citation_utils-0.4.6/citation_utils/dockets/constructed_ac.py
--rw-r--r--   0        0        0     3164 2023-06-29 03:28:29.361313 citation_utils-0.4.6/citation_utils/dockets/constructed_am.py
--rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.6/citation_utils/dockets/constructed_bm.py
--rw-r--r--   0        0        0     2866 2023-06-29 03:27:47.112900 citation_utils-0.4.6/citation_utils/dockets/constructed_gr.py
--rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.6/citation_utils/dockets/constructed_jib.py
--rw-r--r--   0        0        0     2692 2023-06-28 10:55:51.445938 citation_utils-0.4.6/citation_utils/dockets/constructed_oca.py
--rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.6/citation_utils/dockets/constructed_pet.py
--rw-r--r--   0        0        0     2055 2023-06-28 10:33:49.974829 citation_utils-0.4.6/citation_utils/dockets/constructed_udk.py
--rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.6/citation_utils/dockets/models/__init__.py
--rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.6/citation_utils/dockets/models/constructor.py
--rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.6/citation_utils/dockets/models/docket_category.py
--rw-r--r--   0        0        0     1696 2023-06-29 03:24:53.524673 citation_utils-0.4.6/citation_utils/dockets/models/docket_citation.py
--rw-r--r--   0        0        0     5873 2023-06-29 02:04:16.817476 citation_utils-0.4.6/citation_utils/dockets/models/docket_model.py
--rw-r--r--   0        0        0     3404 2023-06-28 02:34:55.066065 citation_utils-0.4.6/citation_utils/dockets/models/docket_rules.py
--rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.6/citation_utils/dockets/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.6/citation_utils/dockets/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.6/citation_utils/dockets/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.6/citation_utils/dockets/models/misc/num.py
--rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.6/citation_utils/dockets/models/misc/x.py
--rw-r--r--   0        0        0     5861 2023-06-29 03:34:11.063815 citation_utils-0.4.6/citation_utils/document.py
--rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.6/citation_utils/special.py
--rw-r--r--   0        0        0     1312 2023-06-29 03:30:30.117842 citation_utils-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.7/LICENSE
+-rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.7/citation_utils/__init__.py
+-rw-r--r--   0        0        0    18085 2023-06-30 03:42:19.085667 citation_utils-0.4.7/citation_utils/citation.py
+-rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.7/citation_utils/dockets/__init__.py
+-rw-r--r--   0        0        0     3125 2023-06-29 03:28:48.048714 citation_utils-0.4.7/citation_utils/dockets/constructed_ac.py
+-rw-r--r--   0        0        0     3164 2023-06-29 03:28:29.361313 citation_utils-0.4.7/citation_utils/dockets/constructed_am.py
+-rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.7/citation_utils/dockets/constructed_bm.py
+-rw-r--r--   0        0        0     2866 2023-06-29 03:27:47.112900 citation_utils-0.4.7/citation_utils/dockets/constructed_gr.py
+-rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.7/citation_utils/dockets/constructed_jib.py
+-rw-r--r--   0        0        0     2692 2023-06-28 10:55:51.445938 citation_utils-0.4.7/citation_utils/dockets/constructed_oca.py
+-rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.7/citation_utils/dockets/constructed_pet.py
+-rw-r--r--   0        0        0     2055 2023-06-28 10:33:49.974829 citation_utils-0.4.7/citation_utils/dockets/constructed_udk.py
+-rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.7/citation_utils/dockets/models/__init__.py
+-rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.7/citation_utils/dockets/models/constructor.py
+-rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.7/citation_utils/dockets/models/docket_category.py
+-rw-r--r--   0        0        0     1696 2023-06-29 03:24:53.524673 citation_utils-0.4.7/citation_utils/dockets/models/docket_citation.py
+-rw-r--r--   0        0        0     5873 2023-06-29 02:04:16.817476 citation_utils-0.4.7/citation_utils/dockets/models/docket_model.py
+-rw-r--r--   0        0        0     3404 2023-06-28 02:34:55.066065 citation_utils-0.4.7/citation_utils/dockets/models/docket_rules.py
+-rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.7/citation_utils/dockets/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.7/citation_utils/dockets/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.7/citation_utils/dockets/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.7/citation_utils/dockets/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.7/citation_utils/dockets/models/misc/x.py
+-rw-r--r--   0        0        0     5861 2023-06-29 03:34:11.063815 citation_utils-0.4.7/citation_utils/document.py
+-rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.7/citation_utils/special.py
+-rw-r--r--   0        0        0     1312 2023-06-30 03:42:55.806152 citation_utils-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.7/PKG-INFO
```

### Comparing `citation_utils-0.4.6/LICENSE` & `citation_utils-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/__init__.py` & `citation_utils-0.4.7/citation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/citation.py` & `citation_utils-0.4.7/citation_utils/citation.py`

 * *Files 4% similar despite different names*

```diff
@@ -310,14 +310,26 @@
 
 class CountedCitation(Citation):
     mentions: int = Field(default=1, description="Get count via Citation __eq__")
 
     def __repr__(self) -> str:
         return f"{str(self)}: {self.mentions}"
 
+    @model_serializer
+    def ser_model(self) -> dict[str, str | datetime.date | int | None]:
+        return {
+            "cat": self.serialize_cat(self.docket_category),
+            "num": self.serialize_num(self.docket_serial),
+            "date": self.serialize_dt(self.docket_date),
+            "phil": self.serialize_phil(self.phil),
+            "scra": self.serialize_scra(self.scra),
+            "offg": self.serialize_offg(self.offg),
+            "mentions": self.mentions,
+        }
+
     @classmethod
     def from_source(cls, text: str) -> list[Self]:
         """Computes mentions of `counted_dockets()` vis-a-vis `counted_reports()` and
         count the number of unique items, taking into account the Citation
         structure and the use of __eq__ re: what is considered unique.
 
         Examples:
@@ -345,18 +357,22 @@
         return all_reports
 
     @classmethod
     def from_repr_format(cls, repr_texts: list[str]) -> Iterator[Self]:
         """Generate their pydantic counterparts from `<cat> <id>: <mentions>` format.
 
         Examples:
-            >>> repr_texts = ['BM No. 412, Jan 01, 2000, 1111 SCRA 1111: 3', 'GR No. 147033, Apr 30, 2003, 374 Phil. 1: 3']
+            >>> repr_texts = ['BM No. 412, Jan 01, 2000, 1111 SCRA 1111: 3', 'GR No. 147033, Apr 30, 2003, 374 Phil. 1: 1']
             >>> results = list(CountedCitation.from_repr_format(repr_texts))
             >>> len(results)
             2
+            >>> results[0].model_dump()
+            {'cat': 'bm', 'num': '412', 'date': '2000-01-01', 'phil': None, 'scra': '1111 scra 1111', 'offg': None, 'mentions': 3}
+            >>> results[1].model_dump()
+            {'cat': 'gr', 'num': '147033', 'date': '2003-04-30', 'phil': '374 phil. 1', 'scra': None, 'offg': None, 'mentions': 1}
 
         Args:
             repr_texts (str): list of texts having `__repr__` format of a `CountedRule`
 
         Yields:
             Iterator[Self]: Instances of CountedCitation.
         """  # noqa: E501
```

### Comparing `citation_utils-0.4.6/citation_utils/dockets/__init__.py` & `citation_utils-0.4.7/citation_utils/dockets/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_ac.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_ac.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_am.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_am.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_bm.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_bm.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_gr.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_gr.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_jib.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_jib.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_oca.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_oca.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_pet.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_pet.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/constructed_udk.py` & `citation_utils-0.4.7/citation_utils/dockets/constructed_udk.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/constructor.py` & `citation_utils-0.4.7/citation_utils/dockets/models/constructor.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/docket_category.py` & `citation_utils-0.4.7/citation_utils/dockets/models/docket_category.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/docket_citation.py` & `citation_utils-0.4.7/citation_utils/dockets/models/docket_citation.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/docket_model.py` & `citation_utils-0.4.7/citation_utils/dockets/models/docket_model.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/docket_rules.py` & `citation_utils-0.4.7/citation_utils/dockets/models/docket_rules.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/gr_clean.py` & `citation_utils-0.4.7/citation_utils/dockets/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/misc/extra.py` & `citation_utils-0.4.7/citation_utils/dockets/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/dockets/models/misc/num.py` & `citation_utils-0.4.7/citation_utils/dockets/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/document.py` & `citation_utils-0.4.7/citation_utils/document.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/citation_utils/special.py` & `citation_utils-0.4.7/citation_utils/special.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.6/pyproject.toml` & `citation_utils-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation_utils"
-version = "0.4.6"
+version = "0.4.7"
 description = "Pattern matching Philippine Supreme Court citations."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-utils"
 documentation = "https://justmars.github.io/citation-utils"
 classifiers = [
   "Topic :: Text Processing :: General",
```

### Comparing `citation_utils-0.4.6/PKG-INFO` & `citation_utils-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.4.6
+Version: 0.4.7
 Summary: Pattern matching Philippine Supreme Court citations.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

