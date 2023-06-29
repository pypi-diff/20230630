# Comparing `tmp/datahtml-0.4.0rc8.tar.gz` & `tmp/datahtml-0.4.0rc9.tar.gz`

## Comparing `datahtml-0.4.0rc8.tar` & `datahtml-0.4.0rc9.tar`

### file list

```diff
@@ -1,57 +1,59 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/.pylintrc
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/readthedocs.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/_utils.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/agents.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/base.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/crawler.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/defaults.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/errors.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/google.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/google_trends.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/news.py
--rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/parsers.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/rss.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/sitemap.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/types.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/web.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/wikidata.py
--rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/apis/__init__.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/datahtml/apis/youtube.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/Makefile
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/api_reference.rst
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/conf.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/make.bat
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/api/crawler.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/api/sitemap.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/api/types.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/docs/api/web.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/__init__.py
--rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/google_search.html
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/google_trends_rss.xml
--rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/lanacion_article.html
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/robots.txt
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/root_carrefour_sitemap.xml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/test_apis_youtube.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/test_google.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/test_google_trends.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/test_root.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/test_youtube.py
--rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_channel.html
--rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_channel_rss.xml
--rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_search.html
--rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_search_response.json
--rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_video.html
--rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_video.json
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_video_multiple_ids.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/tests/youtube_video_response.json
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/LICENSE
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/README.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/pyproject.toml
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 datahtml-0.4.0rc8/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/.pylintrc
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/readthedocs.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/__about__.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/_utils.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/agents.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/base.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/crawler.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/defaults.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/errors.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/google.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/google_trends.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/news.py
+-rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/parsers.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/rss.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/site.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/sitemap.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/types.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/web.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/wikidata.py
+-rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/apis/__init__.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/datahtml/apis/youtube.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/Makefile
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/api_reference.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/conf.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/make.bat
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/api/crawler.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/api/sitemap.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/api/types.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/docs/api/web.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/__init__.py
+-rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/google_search.html
+-rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/google_trends_rss.xml
+-rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/lanacion_article.html
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/robots.txt
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/root_carrefour_sitemap.xml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/test_apis_youtube.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/test_google.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/test_google_trends.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/test_parsers.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/test_root.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/test_youtube.py
+-rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_channel.html
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_channel_rss.xml
+-rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_search.html
+-rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_search_response.json
+-rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_video.html
+-rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_video.json
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_video_multiple_ids.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/tests/youtube_video_response.json
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/LICENSE
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/README.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 datahtml-0.4.0rc9/PKG-INFO
```

### Comparing `datahtml-0.4.0rc8/.pylintrc` & `datahtml-0.4.0rc9/.pylintrc`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/base.py` & `datahtml-0.4.0rc9/datahtml/base.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/crawler.py` & `datahtml-0.4.0rc9/datahtml/crawler.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/defaults.py` & `datahtml-0.4.0rc9/datahtml/defaults.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/errors.py` & `datahtml-0.4.0rc9/datahtml/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,8 +27,15 @@
 
 
 class CrawlingError(Exception):
     def __init__(self, url, status):
         msg = f"Error crawling url {url} with status {status}"
         super().__init__(msg)
 
+class XMLContentNotFound(Exception):
+    def __init__(self, url):
+        msg = f"The response of {url} is not xml"
+        super().__init__(msg)
+
+
+
```

### Comparing `datahtml-0.4.0rc8/datahtml/google.py` & `datahtml-0.4.0rc9/datahtml/google.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/google_trends.py` & `datahtml-0.4.0rc9/datahtml/google_trends.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/news.py` & `datahtml-0.4.0rc9/datahtml/news.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/parsers.py` & `datahtml-0.4.0rc9/datahtml/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def text_from_link(link: str) -> str:
     """Gets a link a return a string from the path.
     It try to keep the last part of the url and give away any extension:
     >> text_from_link("https://www.pe.com/morales-y-bullrich-reeditaron-los-reproches-y-profundizaron-las-diferencias-sobre-el-rumbo-de-jxc.phtml")
     >> 'morales y bullrich reeditaron los reproches y profundizaron las diferencias sobre el rumbo de jxc'
     """
-    u = urlparse(link)
+    u = urlparse(link.strip("/"))
     _path = u.path.split(".")[0]
     between_path = _path.split("/")
     last_path = between_path[-1]
     # last_path = last_path.split(".html")[0]
     words = re.findall(WORDS_REGEX, last_path)
     return " ".join(words)
 
@@ -98,15 +98,22 @@
         except json.JSONDecodeError:
             pass
     return data
 
 
 def url_norm(url, trailing=True):
     """
-    Strip slashes.
+    Normalize an URL. It returns a tuple with the fullurl
+    without trailing slashes, and a url_short version without
+    protocols, query params and so on... only domain and path.
+
+    For instance:
+    u2 = "https://www.google.com/test?query=testq"
+    it should returns:
+    (https://www.google.com/test, www.google.com/test)
     """
     _u = urlparse(url)
     # netloc = _u.netloc.strip("/")
     _path = _u.path.strip("/")
     fullurl = f"{_u.scheme}://{_u.netloc}/{_path}"
     url_short = f"{_u.netloc}/{_path}"
     if trailing:
@@ -121,14 +128,16 @@
         raise errors.URLParsingError(url)
     domain = url_regex[0][1]
     return str(domain)
 
 
 def parse_url(url: str, socials_url=SOCIALS_COM) -> types.URL:
     """Parse a url string to URL.
+
+    For developers:
     URL_REGEX return a tuple with 3 values:
     (protocol, netloc, path)
     """
     url_regex = re.findall(URL_REGEX, url)
 
     if not url_regex:
         raise errors.URLParsingError(url)
```

### Comparing `datahtml-0.4.0rc8/datahtml/sitemap.py` & `datahtml-0.4.0rc9/datahtml/sitemap.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/types.py` & `datahtml-0.4.0rc9/datahtml/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,7 +121,17 @@
         return f"<WKEntityExtra {self.id} | {self.label}>"
 
     def __repr__(self):
         return f"<WKEntityExtra {self.id} | {self.label}>"
 
     def dict(self) -> Dict[str, Any]:
         return asdict(self)
+
+@define
+class LinkMerged:
+    fullurl: str
+    urlnorm: str
+    source: str
+    text: str
+    text_path: str
+    title: Optional[str] = None
+    lastmod: Optional[str] = None
```

### Comparing `datahtml-0.4.0rc8/datahtml/web.py` & `datahtml-0.4.0rc9/datahtml/web.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/wikidata.py` & `datahtml-0.4.0rc9/datahtml/wikidata.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/youtube.py` & `datahtml-0.4.0rc9/datahtml/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/datahtml/apis/youtube.py` & `datahtml-0.4.0rc9/datahtml/apis/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/docs/Makefile` & `datahtml-0.4.0rc9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/docs/conf.py` & `datahtml-0.4.0rc9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/docs/index.rst` & `datahtml-0.4.0rc9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/docs/make.bat` & `datahtml-0.4.0rc9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/google_search.html` & `datahtml-0.4.0rc9/tests/google_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/google_trends_rss.xml` & `datahtml-0.4.0rc9/tests/google_trends_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/lanacion_article.html` & `datahtml-0.4.0rc9/tests/lanacion_article.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/root_carrefour_sitemap.xml` & `datahtml-0.4.0rc9/tests/root_carrefour_sitemap.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/test_apis_youtube.py` & `datahtml-0.4.0rc9/tests/test_apis_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/test_youtube.py` & `datahtml-0.4.0rc9/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_channel.html` & `datahtml-0.4.0rc9/tests/youtube_channel.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_channel_rss.xml` & `datahtml-0.4.0rc9/tests/youtube_channel_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_search.html` & `datahtml-0.4.0rc9/tests/youtube_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_search_response.json` & `datahtml-0.4.0rc9/tests/youtube_search_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_video.html` & `datahtml-0.4.0rc9/tests/youtube_video.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_video.json` & `datahtml-0.4.0rc9/tests/youtube_video.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_video_multiple_ids.json` & `datahtml-0.4.0rc9/tests/youtube_video_multiple_ids.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/tests/youtube_video_response.json` & `datahtml-0.4.0rc9/tests/youtube_video_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/.gitignore` & `datahtml-0.4.0rc9/.gitignore`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/LICENSE` & `datahtml-0.4.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/README.md` & `datahtml-0.4.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/pyproject.toml` & `datahtml-0.4.0rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc8/PKG-INFO` & `datahtml-0.4.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datahtml
-Version: 0.4.0rc8
+Version: 0.4.0rc9
 Summary: A lib to work with html and web data
 Project-URL: Documentation, https://github.com/algorinfo/datahtml#readme
 Project-URL: Issues, https://github.com/algorinfo/datahtml/issues
 Project-URL: Source, https://github.com/algorinfo/datahtml
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

