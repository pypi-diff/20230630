# Comparing `tmp/tdxpy-0.2.1.tar.gz` & `tmp/tdxpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdxpy-0.2.1.tar", max compression
+gzip compressed data, was "tdxpy-0.2.2.tar", max compression
```

## Comparing `tdxpy-0.2.1.tar` & `tdxpy-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      324 2023-05-11 05:15:33.958134 tdxpy-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2023-05-11 05:15:06.906347 tdxpy-0.2.1/LICENSE
--rw-r--r--   0        0        0     1289 2023-05-11 05:15:33.958134 tdxpy-0.2.1/README.md
--rw-r--r--   0        0        0      960 2023-05-11 05:15:33.962134 tdxpy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       63 2023-05-11 05:15:33.962134 tdxpy-0.2.1/tdxpy/__init__.py
--rw-r--r--   0        0        0     9372 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/base_socket_client.py
--rw-r--r--   0        0        0     6405 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/constants.py
--rw-r--r--   0        0        0       48 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/crawler/__init__.py
--rw-r--r--   0        0        0     3487 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/crawler/base_crawler.py
--rw-r--r--   0        0        0     5975 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/crawler/history_financial_crawler.py
--rw-r--r--   0        0        0      419 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/exceptions.py
--rw-r--r--   0        0        0     4910 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/exhq.py
--rw-r--r--   0        0        0     1391 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/heartbeat.py
--rw-r--r--   0        0        0     4495 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/helper.py
--rw-r--r--   0        0        0    11429 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/hq.py
--rw-r--r--   0        0        0      320 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/logger.py
--rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/base.py
--rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/__init__.py
--rw-r--r--   0        0        0     2603 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
--rw-r--r--   0        0        0     1221 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_minute_time_data.py
--rw-r--r--   0        0        0     4170 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_transaction_data.py
--rw-r--r--   0        0        0     2124 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_bars.py
--rw-r--r--   0        0        0      342 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_count.py
--rw-r--r--   0        0        0     1350 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_info.py
--rw-r--r--   0        0        0     2852 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote.py
--rw-r--r--   0        0        0     6330 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote_list.py
--rw-r--r--   0        0        0     1272 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_markets.py
--rw-r--r--   0        0        0     1330 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_minute_time_data.py
--rw-r--r--   0        0        0     4077 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_transaction_data.py
--rw-r--r--   0        0        0      396 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/raw_parser.py
--rw-r--r--   0        0        0     1316 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/setup_commands.py
--rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/std/__init__.py
--rw-r--r--   0        0        0     2324 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/std/get_block_info.py
--rw-r--r--   0        0        0     1516 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_company_info_category.py
--rw-r--r--   0        0        0     1081 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_company_info_content.py
--rw-r--r--   0        0        0     3998 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_finance_info.py
--rw-r--r--   0        0        0     1436 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_history_minute_time_data.py
--rw-r--r--   0        0        0     1734 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_history_transaction_data.py
--rw-r--r--   0        0        0     3055 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_index_bars.py
--rw-r--r--   0        0        0     1082 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_minute_time_data.py
--rw-r--r--   0        0        0      975 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_report_file.py
--rw-r--r--   0        0        0     2837 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_bars.py
--rw-r--r--   0        0        0      568 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_count.py
--rw-r--r--   0        0        0     1411 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_list.py
--rw-r--r--   0        0        0     7836 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_quotes.py
--rw-r--r--   0        0        0     1687 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_transaction_data.py
--rw-r--r--   0        0        0     3867 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_xdxr_info.py
--rw-r--r--   0        0        0      744 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/__init__.py
--rw-r--r--   0        0        0     1301 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/base_reader.py
--rw-r--r--   0        0        0     4385 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/block_reader.py
--rw-r--r--   0        0        0     5611 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/daily_bar_reader.py
--rw-r--r--   0        0        0     1711 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/exhq_daily_bar_reader.py
--rw-r--r--   0        0        0      937 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/history_financial_reader.py
--rw-r--r--   0        0        0     2587 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/lc_min_bar_reader.py
--rw-r--r--   0        0        0     3052 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/min_bar_reader.py
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 tdxpy-0.2.1/setup.py
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 tdxpy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-11 05:15:06.906347 tdxpy-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1289 2023-05-11 05:15:33.958134 tdxpy-0.2.2/README.md
+-rw-r--r--   0        0        0     1368 2023-06-30 04:27:37.138097 tdxpy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-06-30 04:27:37.138097 tdxpy-0.2.2/tdxpy/__init__.py
+-rw-r--r--   0        0        0     9315 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/base_socket_client.py
+-rw-r--r--   0        0        0     6449 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/constants.py
+-rw-r--r--   0        0        0       48 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/crawler/__init__.py
+-rw-r--r--   0        0        0     3619 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/crawler/base_crawler.py
+-rw-r--r--   0        0        0     6030 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/crawler/history_financial_crawler.py
+-rw-r--r--   0        0        0      394 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/exceptions.py
+-rw-r--r--   0        0        0     4910 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/exhq.py
+-rw-r--r--   0        0        0     1391 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/heartbeat.py
+-rw-r--r--   0        0        0     5941 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/helper.py
+-rw-r--r--   0        0        0    11730 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/hq.py
+-rw-r--r--   0        0        0      320 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/logger.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/__init__.py
+-rw-r--r--   0        0        0     4746 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/base.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/ext/__init__.py
+-rw-r--r--   0        0        0     2637 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
+-rw-r--r--   0        0        0     1223 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_minute_time_data.py
+-rw-r--r--   0        0        0     4170 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_transaction_data.py
+-rw-r--r--   0        0        0     2130 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_bars.py
+-rw-r--r--   0        0        0      345 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_count.py
+-rw-r--r--   0        0        0     1350 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_info.py
+-rw-r--r--   0        0        0     2854 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote.py
+-rw-r--r--   0        0        0     6336 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote_list.py
+-rw-r--r--   0        0        0     1307 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_markets.py
+-rw-r--r--   0        0        0     1332 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_minute_time_data.py
+-rw-r--r--   0        0        0     4078 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_transaction_data.py
+-rw-r--r--   0        0        0      396 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/raw_parser.py
+-rw-r--r--   0        0        0     1272 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/setup_commands.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/std/__init__.py
+-rw-r--r--   0        0        0     2308 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_block_info.py
+-rw-r--r--   0        0        0     1549 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_company_info_category.py
+-rw-r--r--   0        0        0     1082 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_company_info_content.py
+-rw-r--r--   0        0        0     3999 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_finance_info.py
+-rw-r--r--   0        0        0     1767 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_history_minute_time_data.py
+-rw-r--r--   0        0        0     1849 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_history_transaction_data.py
+-rw-r--r--   0        0        0     3243 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_index_bars.py
+-rw-r--r--   0        0        0     1515 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_minute_time_data.py
+-rw-r--r--   0        0        0      969 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_report_file.py
+-rw-r--r--   0        0        0     3024 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_bars.py
+-rw-r--r--   0        0        0      570 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_count.py
+-rw-r--r--   0        0        0     1444 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_list.py
+-rw-r--r--   0        0        0     7845 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_quotes.py
+-rw-r--r--   0        0        0     1689 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_transaction_data.py
+-rw-r--r--   0        0        0     3915 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_xdxr_info.py
+-rw-r--r--   0        0        0      744 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/__init__.py
+-rw-r--r--   0        0        0     1293 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/base_reader.py
+-rw-r--r--   0        0        0     4746 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/block_reader.py
+-rw-r--r--   0        0        0     5698 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/daily_bar_reader.py
+-rw-r--r--   0        0        0     1713 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/exhq_daily_bar_reader.py
+-rw-r--r--   0        0        0      937 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/history_financial_reader.py
+-rw-r--r--   0        0        0     2587 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/lc_min_bar_reader.py
+-rw-r--r--   0        0        0     3052 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/min_bar_reader.py
+-rw-r--r--   0        0        0       46 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/version.py
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 tdxpy-0.2.2/setup.py
+-rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 tdxpy-0.2.2/PKG-INFO
```

### Comparing `tdxpy-0.2.1/LICENSE` & `tdxpy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.1/README.md` & `tdxpy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.1/pyproject.toml` & `tdxpy-0.2.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,78 @@
 [tool.poetry]
 name = "tdxpy"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["bopo <ibopo@126.com>"]
 readme = "README.md"
 packages = [{ include = "tdxpy" }]
 include = ["CHANGELOG.md"]
 
+
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.5.1"
 cryptography = "^38.0.3"
 
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.group.test.dependencies]
 pytest-datadir = "^1.4.1"
 pytest-cov = "^4.0.0"
 pytest = "^7.2.0"
 
 
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.4.3"
+
 [[tool.poetry.source]]
 name = "mirrors"
 url = "https://mirrors.ustc.edu.cn/pypi/web/simple"
 default = true
 secondary = false
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_option]
 testpaths = "tests"
 addopts = "-p no:warnings"
-
-log_cli = 1
 log_cli_level = "DEBUG"
+log_cli = 1
+
 
 [tool.commitizen]
-version = "0.2.1"
 tag_format = "v$version"
-
-update_changelog_on_bump = true
-changelog_file = "CHANGELOG.md"
 annotated_tag = true
-
+changelog_file = "docs/history.md"
+changelog_incremental = true
+update_changelog_on_bump = true
+version_provider = "poetry"
 version_files = [
     "tdxpy/__init__.py:__version__",
-    "pyproject.toml:version",
-    "Makefile:VERSION := ",
 ]
+
+
+[tool.black]
+line-length = 120
+target-version = ['py39']
+include = '\.pyi?$'
+
+[tool.coverage]
+skip_covered = true
+sort = "-cover"
+
+[tool.coverage.run]
+source = ["tdxpy"]
+branch = true
+omit = [
+    "tdxpy/parser/ext/*.py",
+    "tdxpy/exhq.py"
+]
+
+[tool.coverage.report]
+exclude_lines = [
+  # ignore abstract methods
+  "raise NotImplementedError",
+  "def __repr__"
+]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `tdxpy-0.2.1/tdxpy/base_socket_client.py` & `tdxpy-0.2.2/tdxpy/base_socket_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,53 +71,52 @@
                 raise to_raise
 
         return ret
 
     return wrapper
 
 
-class RetryStrategy(object):
+class RetryStrategy:
     @classmethod
     def generate(cls):
         raise NotImplementedError("need to override")
 
 
 class DefaultRetryStrategy(RetryStrategy):
     """
     默认的重试策略，您可以通过写自己的重试策略替代本策略, 改策略主要实现 generate 方法，该方法是一个生成器，
     返回下次重试的间隔时间, 单位为秒，我们会使用 time.sleep在这里同步等待之后进行重新connect,然后再重新发起
     源请求，直到 generate 结束。
     """
 
     @classmethod
     def generate(cls):
-        for time_interval in [0.1, 0.5, 1, 2]:
-            yield time_interval
+        yield from [0.1, 0.5, 1, 2]
 
 
 class TrafficStatSocket(socket.socket):
     """
     实现支持流量统计的socket类
     """
 
     def __init__(self, sock, mode):
-        super(TrafficStatSocket, self).__init__(sock, mode)
+        super().__init__(sock, mode)
 
         # 流量统计相关
         self.send_pkg_num = 0  # 发送次数
         self.recv_pkg_num = 0  # 接收次数
         self.send_pkg_bytes = 0  # 发送字节
         self.recv_pkg_bytes = 0  # 接收字节数
         self.first_pkg_send_time = None  # 第一个数据包发送时间
 
         self.last_api_send_bytes = 0  # 最近的一次api调用的发送字节数
         self.last_api_recv_bytes = 0  # 最近一次api调用的接收字节数
 
 
-class BaseSocketClient(object):
+class BaseSocketClient:
     def __init__(self, multithread=False, heartbeat=False, auto_retry=False, raise_exception=False):
         """
         构造函数
         :param multithread: 是否多线程
         :param heartbeat: 是否心跳
         :param auto_retry: 是否自动回复
         :param raise_exception: 是否抛出异常
@@ -159,30 +158,30 @@
         :param time_out: 连接超时时间
         :param bind_port: 绑定的本地端口
         :param bind_ip: 绑定的本地ip
         :return: 是否连接成功 True/False
         """
 
         if not ip:
-            raise ValidationException('IP Address bad.')
+            raise ValidationException("IP Address bad.")
 
         self.client = TrafficStatSocket(socket.AF_INET, socket.SOCK_STREAM)
         self.client.settimeout(time_out)
 
         logger.debug(f"connecting to server: {ip} on port: {port}")
 
         try:
             self.ip = ip
             self.port = port
 
             if bind_port:
                 self.client.bind((bind_ip, bind_port))
 
             self.client.connect((ip, port))
-        except socket.timeout as e:
+        except socket.timeout:
             logger.debug("connection expired")
 
             if self.raise_exception:
                 raise TdxConnectionError("connection timeout error")
 
             return False
         except Exception as e:  # noqa
@@ -197,15 +196,17 @@
 
         if self.need_setup:
             self.setup()
 
         # 启动心跳包
         if self.heartbeat:
             self.stop_event = threading.Event()
-            self.heartbeat_thread = HeartBeatThread(client=self, stop_event=self.stop_event, interval=self.heartbeat_interval)
+            self.heartbeat_thread = HeartBeatThread(
+                client=self, stop_event=self.stop_event, interval=self.heartbeat_interval
+            )
             self.heartbeat_thread.start()
 
         return self
 
     def disconnect(self):
         """
         断开连接
@@ -219,15 +220,15 @@
             logger.debug("disconnecting")
 
             try:
                 self.client.shutdown(socket.SHUT_RDWR)
                 self.client.close()
                 self.client = None
             except Exception as e:
-                logger.debug(f'disconnect err: {e}')
+                logger.debug(f"disconnect err: {e}")
                 if self.raise_exception:
                     raise TdxConnectionError(f"disconnect err: {e}")
             finally:
                 self.client = None
 
             logger.debug("disconnected")
 
@@ -293,15 +294,15 @@
     def to_df(v):
         """
         数据转换 df 格式
         :param v:
         :return:
         """
 
-        v = v or ''
+        v = v or ""
 
         if not v:
             return pd.DataFrame(data=None)
 
         if isinstance(v, list):
             return pd.DataFrame(data=v)
```

### Comparing `tdxpy-0.2.1/tdxpy/constants.py` & `tdxpy-0.2.2/tdxpy/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # cython: language_level=3
 
+
 class TDXParams:
     # 市场
 
     MARKET_SZ = 0  # 深圳
     MARKET_SH = 1  # 上海
     MARKET_BJ = 2  # 北京
 
@@ -155,15 +156,26 @@
     ("华林", "220.178.55.86", 7709),
 ]
 
 # 交易所
 SECURITY_EXCHANGE = ["sz", "sh"]
 
 # 股票类型
-SECURITY_TYPE = ["SH_A_STOCK", "SH_B_STOCK", "SH_INDEX", "SH_FUND", "SH_BOND", "SZ_A_STOCK", "SZ_B_STOCK", "SZ_INDEX", "SZ_FUND", "SZ_BOND"]
+SECURITY_TYPE = [
+    "SH_A_STOCK",
+    "SH_B_STOCK",
+    "SH_INDEX",
+    "SH_FUND",
+    "SH_BOND",
+    "SZ_A_STOCK",
+    "SZ_B_STOCK",
+    "SZ_INDEX",
+    "SZ_FUND",
+    "SZ_BOND",
+]
 
 # todo 股票系数
 SECURITY_COEFFICIENT = {
     "SH_A_STOCK": [0.01, 0.01],
     "SH_B_STOCK": [0.001, 0.01],
     "SH_INDEX": [0.01, 1.0],
     "SH_FUND": [0.001, 1.0],
```

### Comparing `tdxpy-0.2.1/tdxpy/crawler/base_crawler.py` & `tdxpy-0.2.2/tdxpy/crawler/base_crawler.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,39 @@
 def fetch_report_hook(downloaded, total_size):
     logger.debug(f"Downloaded {downloaded}, Total is {total_size}")
 
 
 class BaseCrawler:
     mode = "http"
 
-    def fetch_and_parse(self, reporthook=None, path_to_download=None, proxies=None, chunksize=1024 * 50, *args, **kwargs):
+    def fetch_and_parse(
+        self, reporthook=None, path_to_download=None, proxies=None, chunksize=1024 * 50, *args, **kwargs
+    ):
         """
         function to get data ,
         :param chunksize:
         :param args:
         :param kwargs:
         :return:
         :param reporthook 使用urllib.request 的report_hook 来汇报下载进度 \
                     参考 https://docs.python.org/3/library/urllib.request.html#module-urllib.request
         :param path_to_download 数据文件下载的地址，如果没有提供，则下载到临时文件中，并在解析之后删除
         :param proxies urllib格式的代理服务器设置
         :return: 解析之后的数据结果
         """
 
         method = ("get_content", "fetch_via_http")[self.mode == "http"]
-        download_file = getattr(self, method)(reporthook=reporthook, path_to_download=path_to_download, proxies=proxies, chunksize=chunksize, *args, **kwargs)
+        download_file = getattr(self, method)(
+            reporthook=reporthook,
+            path_to_download=path_to_download,
+            proxies=proxies,
+            chunksize=chunksize,
+            *args,
+            **kwargs,
+        )
         result = self.parse(download_file, *args, **kwargs)
         download_file.close()
 
         return result
 
     def fetch_via_http(self, reporthook=None, path_to_download=None, chunksize=1024 * 50, *args, **kwargs):
         """
@@ -46,15 +55,18 @@
         :return:
         """
         download_file = path_to_download and open(path_to_download, "wb") or tempfile.NamedTemporaryFile(delete=True)
         url = self.get_url(*args, **kwargs)
 
         request = Request(url)
         request.add_header("Referer", url)
-        request.add_header("User-Agent", r"Mozilla/5.0 (Macintosh Intel Mac OS X 10_14_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.100 Safari/537.36")
+        request.add_header(
+            "User-Agent",
+            r"Mozilla/5.0 (Macintosh Intel Mac OS X 10_14_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.100 Safari/537.36",
+        )
         response = urlopen(request)
 
         if response.getheader("Content-Length") is not None:
             total_size = int(response.getheader("Content-Length").strip())
             downloaded = 0
 
             while True:
```

### Comparing `tdxpy-0.2.1/tdxpy/crawler/history_financial_crawler.py` & `tdxpy-0.2.2/tdxpy/crawler/history_financial_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 
         api = TdxHq_API()
         api.need_setup = False
 
         # calc.tdx.com.cn, calc2.tdx.com.cn
         with api.connect(ip="120.76.152.87"):
             content = api.get_report_file_by_size("tdxfin/gpcw.txt")
-            download_file = not path_to_download and tempfile.NamedTemporaryFile(delete=True) or open(path_to_download, "wb")
+            download_file = (
+                not path_to_download and tempfile.NamedTemporaryFile(delete=True) or open(path_to_download, "wb")
+            )
             download_file.write(content)
             download_file.seek(0)
 
             return download_file
 
     def parse(self, download_file, *args, **kwargs):
         """
@@ -113,15 +115,17 @@
 
         api = TdxHq_API()
         api.need_setup = False
 
         with api.connect(ip="120.76.152.87"):
             # calc.tdx.com.cn, calc2.tdx.com.cn
             content = api.get_report_file_by_size(f"tdxfin/{filename}", filesize=file_size, reporthook=reporthook)
-            download_file = path_to_download and open(path_to_download, "wb") or tempfile.NamedTemporaryFile(delete=True)
+            download_file = (
+                path_to_download and open(path_to_download, "wb") or tempfile.NamedTemporaryFile(delete=True)
+            )
             download_file.write(content)
             download_file.seek(0)
 
             return download_file
 
     def parse(self, download_file, *args, **kwargs):
         """
@@ -164,15 +168,15 @@
 
         max_count = stock_header[2]
 
         report_date = stock_header[1]
         report_size = stock_header[4]
 
         report_fields_count = int(report_size / 4)
-        report_pack_format = "<{}f".format(report_fields_count)
+        report_pack_format = f"<{report_fields_count}f"
 
         results = []
 
         for stock_idx in range(0, max_count):
             dat_file.seek(header_size + stock_idx * calcsize(VALUE))
             si = dat_file.read(stock_item_size)
 
@@ -192,15 +196,14 @@
             dat_file.close()
             shutil.rmtree(tmpdir, ignore_errors=True)
 
         return results
 
     @staticmethod
     def to_df(data):
-
         if not data:
             return None
 
         col = ["code", "report_date"]
         col += [f"col{str(i).zfill(3)}" for i in range(1, len(data[0]) - 1)]
 
         df = pd.DataFrame(data=data, columns=col)
```

### Comparing `tdxpy-0.2.1/tdxpy/exhq.py` & `tdxpy-0.2.2/tdxpy/exhq.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.1/tdxpy/heartbeat.py` & `tdxpy-0.2.2/tdxpy/heartbeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     def run(self):
         # stop_event 未设置就执行
         while not self.stop_event.is_set():
             # 客户端主进程 and 满足 heartbeat_interval
             if self.client and (time.time() - self.api.last_ack_time > self.heartbeat_interval):
                 try:
                     # 发送一个获取股票数量的包作为心跳包
-                    logger.debug('发送一个获取股票数量的包作为心跳包...')
+                    logger.debug("发送一个获取股票数量的包作为心跳包...")
                     self.api.do_heartbeat()
                 except Exception as e:
                     logger.exception(str(e))
 
             # 等待心跳周期
             self.stop_event.wait(self.heartbeat_interval)
```

### Comparing `tdxpy-0.2.1/tdxpy/helper.py` & `tdxpy-0.2.2/tdxpy/helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # cython: language_level=3
 import struct
-from pathlib import Path
+from datetime import datetime
 
 from tdxpy.constants import SECURITY_COEFFICIENT
 from tdxpy.logger import logger
 
 
 def get_price(data, pos):
     """
@@ -120,15 +120,15 @@
         month = int((zip_day % 2048) / 100)
         year = (zip_day >> 11) + 2004
         day = (zip_day % 2048) % 100
 
         minute = minutes % 60
         hour = int(minutes / 60)
     else:
-        zip_day, = struct.unpack("<I", buffer[pos: pos + 4])
+        (zip_day,) = struct.unpack("<I", buffer[pos: pos + 4])
 
         month = int((zip_day % 10000) / 100)
         year = int(zip_day / 10000)
         day = zip_day % 100
 
     pos += 4
 
@@ -138,15 +138,15 @@
 def get_time(buffer, pos):
     """
     获取时间
     :param buffer:
     :param pos:
     :return:
     """
-    minutes, = struct.unpack("<H", buffer[pos: pos + 2])
+    (minutes,) = struct.unpack("<H", buffer[pos: pos + 2])
 
     hour = int(minutes / 60)
     minute = minutes % 60
 
     pos += 2
 
     return hour, minute, pos
@@ -158,30 +158,51 @@
     :param data:
     :param pos:
     :return:
     """
     return data[pos]
 
 
-def get_security_coefficient(market, name):
-    return SECURITY_COEFFICIENT[get_security_type(market, name)]
+# def get_security_coefficient(market, name):
+#     return SECURITY_COEFFICIENT[get_security_type(market, name)]
+
+
+# TODO 增加 get_coefficient 函数
+def get_security_coefficient(market=None, code=None):
+    try:
+        security_type = get_security_type(market=market, code=code)
+        coefficient = SECURITY_COEFFICIENT[security_type]
+
+        logger.warning(f'security_type => {security_type}')
+        logger.warning(f'coefficient => {coefficient}')
+
+        return coefficient[0]
+    except NotImplementedError:
+        logger.error('NotImplementedError')
+        return 0.01
 
 
 def get_security_type(market, code):
     """
     获取股票类型, A股, B股, 指数等
 
     :param market: 市场
     :param code: 代码
     :return:
     """
-    code = Path(code).stem
-    code_head = code[:2]
 
-    if market in ['SZ', 0]:
+    # code = Path(code).stem
+    code = str(code)
+    code_head = str(code)[:2]
+
+    logger.warning(f'market => {market}')
+    logger.warning(f'code => {code}')
+    logger.warning(f'code_head => {code_head}')
+
+    if market in ["SZ", "sz", 0]:
         if code_head in ["00", "30"]:
             return "SZ_A_STOCK"
 
         if code_head in ["20"]:
             return "SZ_B_STOCK"
 
         if code_head in ["39"]:
@@ -189,15 +210,15 @@
 
         if code_head in ["15", "16"]:
             return "SZ_FUND"
 
         if code_head in ["10", "11", "12", "13", "14"]:
             return "SZ_BOND"
 
-    if market in ['SH', 1]:
+    if market in ["SH", "sh", 1]:
         if code_head in ["60", "68"]:  # 688XXX科创板
             return "SH_A_STOCK"
 
         if code_head in ["90"]:
             return "SH_B_STOCK"
 
         if code_head in ["00", "88", "99"]:
@@ -214,10 +235,34 @@
 
 
 def dump(buf):
     from pprint import pprint
 
     try:
         from hexdump import hexdump
+
         pprint(hexdump(buf))
     except ImportError:
         pprint(buf)
+
+
+def time_frame(current_time=None):
+    """
+    判断时间是否在交易时间段内
+    :param current_time: 要检查的时间, 如果空则默认当前时间
+    :return: 在交易时间段内返回 True， 否则返回 False
+    """
+    current_time = current_time or datetime.now()
+
+    start_time = datetime.strptime(str(current_time.date()) + '9:30', '%Y-%m-%d%H:%M')
+    end_time = datetime.strptime(str(current_time.date()) + '11:30', '%Y-%m-%d%H:%M')
+
+    if start_time < current_time < end_time:
+        return True
+
+    start_time = datetime.strptime(str(current_time.date()) + '13:00', '%Y-%m-%d%H:%M')
+    end_time = datetime.strptime(str(current_time.date()) + '15:00', '%Y-%m-%d%H:%M')
+
+    if start_time < current_time < end_time:
+        return True
+
+    return False
```

### Comparing `tdxpy-0.2.1/tdxpy/hq.py` & `tdxpy-0.2.2/tdxpy/hq.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import warnings
 
 import pandas as pd
 
 from tdxpy.base_socket_client import BaseSocketClient
 from tdxpy.base_socket_client import last_ack_time
 from tdxpy.constants import TDXParams
+from tdxpy.helper import time_frame
 from tdxpy.parser.setup_commands import SetupCmd1
 from tdxpy.parser.setup_commands import SetupCmd2
 from tdxpy.parser.setup_commands import SetupCmd3
-from tdxpy.parser.std.get_block_info import get_and_parse_block_info
 from tdxpy.parser.std.get_block_info import GetBlockInfo
 from tdxpy.parser.std.get_block_info import GetBlockInfoMeta
+from tdxpy.parser.std.get_block_info import get_and_parse_block_info
 from tdxpy.parser.std.get_company_info_category import GetCompanyInfoCategory
 from tdxpy.parser.std.get_company_info_content import GetCompanyInfoContent
 from tdxpy.parser.std.get_finance_info import GetFinanceInfo
 from tdxpy.parser.std.get_history_minute_time_data import GetHistoryMinuteTimeData
 from tdxpy.parser.std.get_history_transaction_data import GetHistoryTransactionData
 from tdxpy.parser.std.get_index_bars import GetIndexBarsCmd
 from tdxpy.parser.std.get_minute_time_data import GetMinuteTimeData
@@ -81,25 +82,28 @@
         :return:
         """
 
         # if not all_stock:
         #     raise ValidationException('参数错误')
 
         if isinstance(all_stock, list) and TDXParams.MARKET_BJ in [x[0] for x in all_stock]:
-            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            warnings.warn("此接口暂时不支持北证A股", DeprecationWarning)
             return None
 
         if all_stock == TDXParams.MARKET_BJ:
-            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            warnings.warn("此接口暂时不支持北证A股", DeprecationWarning)
             return None
 
         if code:
             all_stock = [(all_stock, code)]
-        elif (isinstance(all_stock, list) or isinstance(all_stock, tuple)) and len(all_stock) == 2 and type(
-            all_stock[0]) is int:
+        elif (
+            (isinstance(all_stock, list) or isinstance(all_stock, tuple))
+            and len(all_stock) == 2
+            and type(all_stock[0]) is int
+        ):
             all_stock = [all_stock]
 
         cmd = GetSecurityQuotesCmd(self.client, lock=self.lock)
         cmd.setParams(all_stock)
 
         return cmd.call_api()
 
@@ -120,15 +124,15 @@
         """
         获取证券列表
         :param market:
         :param start:
         :return:
         """
         if market == TDXParams.MARKET_BJ:
-            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            warnings.warn("此接口暂时不支持北证A股", DeprecationWarning)
             return None
 
         cmd = GetSecurityList(self.client, lock=self.lock)
         cmd.setParams(market, start)
 
         return cmd.call_api()
 
@@ -165,14 +169,18 @@
         获取分笔数据
         :param market:
         :param code:
         :param start:
         :param count:
         :return:
         """
+        if not time_frame():
+            warnings.warn("目前不是交易时间段, 此接口必须在交易时间才能使用", DeprecationWarning)
+            return None
+
         cmd = GetTransactionData(self.client, lock=self.lock)
         cmd.setParams(market, code, start, count)
 
         return cmd.call_api()
 
     @last_ack_time
     def get_history_transaction_data(self, market, code, start, count, date):
@@ -195,15 +203,15 @@
         """
         公司信息类别
         :param market:
         :param code:
         :return:
         """
         if market == TDXParams.MARKET_BJ:
-            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            warnings.warn("此接口暂时不支持北证A股", DeprecationWarning)
             return None
 
         cmd = GetCompanyInfoCategory(self.client, lock=self.lock)
         cmd.setParams(market, code)
 
         return cmd.call_api()
 
@@ -215,15 +223,15 @@
         :param code:
         :param filename:
         :param start:
         :param length:
         :return:
         """
         if market == TDXParams.MARKET_BJ:
-            warnings.warn('此接口暂时不支持北证A股', DeprecationWarning)
+            warnings.warn("此接口暂时不支持北证A股", DeprecationWarning)
             return None
 
         cmd = GetCompanyInfoContent(self.client, lock=self.lock)
         cmd.setParams(market, code, filename, start, length)
 
         return cmd.call_api()
 
@@ -352,16 +360,20 @@
         # 新版一劳永逸偷懒写法zzz
         # market_code = 1 if str(code)[0] == '6' else 0
 
         # https://github.com/rainx/pytdx/issues/33
         # 0 - 深圳， 1 - 上海
 
         result = pd.concat(
-            [self.to_df(self.get_security_bars(9, __select_market_code(code), code, (9 - i) * 800, 800)) for i in
-             range(10)], axis=0)
+            [
+                self.to_df(self.get_security_bars(9, __select_market_code(code), code, (9 - i) * 800, 800))
+                for i in range(10)
+            ],
+            axis=0,
+        )
         result = (
             result.assign(date=result["datetime"].apply(lambda x: str(x)[0:10]))
             .assign(code=str(code))
             .set_index("date", drop=False, inplace=False)
             .drop(["year", "month", "day", "hour", "minute", "datetime"], axis=1)[start_date:end_date]
         )
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/base.py` & `tdxpy-0.2.2/tdxpy/parser/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from tdxpy.logger import logger
 
 try:
     import cython  # noqa
 
     if cython.compiled:
+
         def buffer(x):
             return x
 
 except ImportError:
     pass
 
 
@@ -36,15 +37,15 @@
 class ResponseRecvFails(Exception):
     pass
 
 
 RSP_HEADER_LEN = 0x10
 
 
-class BaseParser(object):
+class BaseParser:
     def __init__(self, client, lock=None):
         """
 
         :rtype: object
         """
 
         self.send_pkg = None
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,19 +59,21 @@
         """
         klines = []  # noqa
         pos = 12
 
         # 算了，前面不解析了，没太大用
         # (market, code) = struct.unpack("<B9s", body_buf[0: 10]
 
-        ret_count, = struct.unpack("H", body_buf[pos: pos + 2])
+        (ret_count,) = struct.unpack("H", body_buf[pos : pos + 2])
         pos = pos + 2
 
         for _ in range(ret_count):
-            (d1, d2, open_price, high, low, close, position, trade, settlementprice) = struct.unpack("<HHffffIIf", body_buf[pos: pos + 32])  # noqa
+            (d1, d2, open_price, high, low, close, position, trade, settlementprice) = struct.unpack(
+                "<HHffffIIf", body_buf[pos : pos + 32]
+            )  # noqa
             pos += 32
 
             year, month, day = self._parse_date(d1)
             hour, minute = self._parse_time(d2)
             kline = OrderedDict(
                 [
                     ("datetime", "%d-%02d-%02d %02d:%02d" % (year, month, day, hour, minute)),
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_minute_time_data.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_minute_time_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,22 +11,22 @@
         pkg.extend(struct.pack("<IB9s", date, market, code.encode("utf-8")))
 
         self.send_pkg = pkg
 
     def parseResponse(self, body_buf):
         pos = 0
 
-        market, code, _, num = struct.unpack("<B9s8sH", body_buf[pos: pos + 20])
+        market, code, _, num = struct.unpack("<B9s8sH", body_buf[pos : pos + 20])
 
         pos += 20
 
         result = []
 
         for _ in range(num):
-            raw_time, price, avg_price, volume, amount = struct.unpack("<HffII", body_buf[pos: pos + 18])
+            raw_time, price, avg_price, volume, amount = struct.unpack("<HffII", body_buf[pos : pos + 18])
 
             pos += 18
 
             hour = raw_time // 60
             minute = raw_time % 60
 
             result.append(
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_transaction_data.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_transaction_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,22 @@
         pkg = bytearray.fromhex("01 01 30 00 02 01 16 00 16 00 06 24")
         pkg.extend(struct.pack("<IB9siH", date, market, code, start, count))
 
         self.send_pkg = pkg
         self.date = date
 
     def parseResponse(self, body_buf):
-
         pos = 0
-        market, code, _, num = struct.unpack("<B9s4sH", body_buf[pos: pos + 16])
+        market, code, _, num = struct.unpack("<B9s4sH", body_buf[pos : pos + 16])
 
         pos += 16
         result = []
 
         for _ in range(num):
-
-            raw_time, price, volume, zengcang, direction = struct.unpack("<HIIiH", body_buf[pos: pos + 16])
+            raw_time, price, volume, zengcang, direction = struct.unpack("<HIIiH", body_buf[pos : pos + 16])
 
             pos += 16
             year = self.date // 10000
             month = self.date % 10000 // 100
             day = self.date % 100
             hour = raw_time // 60
             minute = raw_time % 60
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_bars.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_bars.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from collections import OrderedDict
 
 from tdxpy.helper import get_datetime
 from tdxpy.parser.base import BaseParser
 
 
 class GetInstrumentBars(BaseParser):
-
     def setParams(self, category, market, code, start, count):
         """
 
         :param category:
         :param market:
         :param code:
         :param start:
@@ -34,24 +33,24 @@
 
         :param body_buf:
         :return:
         """
         pos = 0
         pos += 18
 
-        ret_count, = struct.unpack("<H", body_buf[pos: pos + 2])
+        (ret_count,) = struct.unpack("<H", body_buf[pos : pos + 2])
         pos += 2
 
         klines = []
 
         for _ in range(ret_count):
             year, month, day, hour, minute, pos = get_datetime(self.category, body_buf, pos)
-            open_price, high, low, close, position, trade, price = struct.unpack("<ffffIIf", body_buf[pos: pos + 28])
+            open_price, high, low, close, position, trade, price = struct.unpack("<ffffIIf", body_buf[pos : pos + 28])
 
-            amount, = struct.unpack("f", body_buf[pos + 16: pos + 16 + 4])
+            (amount,) = struct.unpack("f", body_buf[pos + 16 : pos + 16 + 4])
             pos += 28
 
             kline = OrderedDict(
                 [
                     ("open", open_price),
                     ("high", high),
                     ("low", low),
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_info.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import struct
 from collections import OrderedDict
 
 from tdxpy.parser.base import BaseParser
 
 
 class GetInstrumentInfo(BaseParser):
-
     def setParams(self, start, count=100):
         """
 
         :param start:
         :param count:
         """
         pkg = bytearray.fromhex("01 04 48 67 00 01 08 00 08 00 f5 23")
@@ -27,15 +26,15 @@
         pos = 0
         start, count = struct.unpack("<IH", body_buf[:6])
 
         pos += 6
         result = []
 
         for _ in range(count):
-            category, market, _, code_raw, name_raw, desc_raw = struct.unpack("<BB3s9s17s9s", body_buf[pos: pos + 40])
+            category, market, _, code_raw, name_raw, desc_raw = struct.unpack("<BB3s9s17s9s", body_buf[pos : pos + 40])
 
             code = code_raw.decode("gbk", "ignore").rstrip("\x00")
             name = name_raw.decode("gbk", "ignore").rstrip("\x00")
             desc = desc_raw.decode("gbk", "ignore").rstrip("\x00")
 
             line = OrderedDict(
                 [
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         :return:
         """
         if len(body_buf) < 20:
             return []
 
         pos = 0
 
-        market, code = struct.unpack("<B9s", body_buf[pos: pos + 10])
+        market, code = struct.unpack("<B9s", body_buf[pos : pos + 10])
 
         pos += 10
         pos += 4
 
         # 持仓 ((13340,), 66),
         (
             pre_close,
@@ -65,15 +65,15 @@
             a4,
             a5,
             av1,
             av2,
             av3,
             av4,
             av5,
-        ) = struct.unpack("<fffffIIIIIIIIIfffffIIIIIfffffIIIII", body_buf[pos: pos + 136])
+        ) = struct.unpack("<fffffIIIIIIIIIfffffIIIIIfffffIIIII", body_buf[pos : pos + 136])
 
         return [
             OrderedDict(
                 [
                     ("market", market),
                     ("code", code.decode("utf-8").rstrip("\x00")),
                     ("pre_close", pre_close),
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote_list.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,27 +27,27 @@
         :param body_buf:
         :return:
         """
         pos = 0
 
         data_list = []
 
-        num, = struct.unpack("<H", body_buf[pos: pos + 2])
+        (num,) = struct.unpack("<H", body_buf[pos : pos + 2])
 
         if num == 0:
             return []
 
         pos += 2
 
         if self.category not in [2, 3]:
             return NotImplementedError("暂时不支持期货,港股之外的品类")
 
         for _ in range(num):
             # 每个块一共300bytes
-            market, code = struct.unpack("<B9s", body_buf[pos: pos + 10])
+            market, code = struct.unpack("<B9s", body_buf[pos : pos + 10])
             code = code.strip(b"\0").decode("gbk", "ignore")  # to unicode
             pos += 10
 
             if self.category == 3:
                 try:
                     pos = self.extract_futures(market, code, body_buf, data_list, pos)
                 except Exception as e:
@@ -104,15 +104,15 @@
             MaiChuJia4,
             MaiChuJia5,
             MaiChuLiang1,
             MaiChuLiang2,
             MaiChuLiang3,
             MaiChuLiang4,
             MaiChuLiang5,
-        ) = struct.unpack(data_pack_format, body_buf[pos: pos + 140])
+        ) = struct.unpack(data_pack_format, body_buf[pos : pos + 140])
 
         pos += 290
 
         one = OrderedDict(
             [
                 ("market", market),
                 ("code", code),
@@ -201,15 +201,15 @@
             _,
             _,
             MaiChuLiang,
             _,
             _,
             _,
             _,
-        ) = struct.unpack(data_pack_format, body_buf[pos: pos + 140])
+        ) = struct.unpack(data_pack_format, body_buf[pos : pos + 140])
 
         pos += 290
 
         one = OrderedDict(
             [
                 ("market", market),
                 ("code", code),
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_markets.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_markets.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,21 +12,23 @@
     def parseResponse(self, body_buf):
         """
 
         :param body_buf:
         :return:
         """
         pos = 0
-        cnt, = struct.unpack("<H", body_buf[pos: pos + 2])
+        (cnt,) = struct.unpack("<H", body_buf[pos : pos + 2])
 
         pos += 2
         result = []
 
         for _ in range(cnt):
-            category, raw_name, market, raw_short_name, _, unknown_bytes = struct.unpack("<B32sB2s26s2s", body_buf[pos: pos + 64])
+            category, raw_name, market, raw_short_name, _, unknown_bytes = struct.unpack(
+                "<B32sB2s26s2s", body_buf[pos : pos + 64]
+            )
             pos += 64
 
             if category == 0 and market == 0:
                 continue
 
             name = raw_name.decode("gbk", "ignore")
             short_name = raw_short_name.decode("gbk", "ignore")
@@ -34,13 +36,13 @@
             result.append(
                 OrderedDict(
                     [
                         ("market", market),
                         ("category", category),
                         ("name", name.rstrip("\x00")),
                         ("short_name", short_name.rstrip("\x00")),
-                        ('unknown_bytes', unknown_bytes)
+                        ("unknown_bytes", unknown_bytes),
                     ]
                 )
             )
 
         return result
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_minute_time_data.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_minute_time_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,21 +21,21 @@
         """
 
         :param body_buf:
         :return:
         """
         pos = 0
 
-        market, code, num = struct.unpack("<B9sH", body_buf[pos: pos + 12])
+        market, code, num = struct.unpack("<B9sH", body_buf[pos : pos + 12])
         pos += 12
 
         result = []
 
         for _ in range(num):
-            raw_time, price, avg_price, volume, amount = struct.unpack("<HffII", body_buf[pos: pos + 18])
+            raw_time, price, avg_price, volume, amount = struct.unpack("<HffII", body_buf[pos : pos + 18])
             pos += 18
 
             hour = raw_time // 60
             minute = raw_time % 60
 
             result.append(
                 OrderedDict(
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_transaction_data.py` & `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_transaction_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,22 @@
     def parseResponse(self, body_buf):
         """
 
         :param body_buf:
         :return:
         """
         pos = 0
-        market, code, _, num = struct.unpack("<B9s4sH", body_buf[pos: pos + 16])
+        market, code, _, num = struct.unpack("<B9s4sH", body_buf[pos : pos + 16])
 
         pos += 16
         result = []
         nature_name = ""
 
         for _ in range(num):
-
-            raw_time, price, volume, zengcang, direction = struct.unpack("<HIIiH", body_buf[pos: pos + 16])
+            raw_time, price, volume, zengcang, direction = struct.unpack("<HIIiH", body_buf[pos : pos + 16])
 
             pos += 16
             hour = raw_time // 60
 
             minute = raw_time % 60
             second = direction % 10000
             nature = direction  # 保持老接口的兼容性
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/setup_commands.py` & `tdxpy-0.2.2/tdxpy/parser/setup_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,20 @@
         :return:
         """
         return body_buf
 
 
 class SetupCmd1(BaseSetup):
     def setup(self):
-        self.send_pkg = bytearray.fromhex(
-            "0c 02 18 93 00 01 03 00 03 00 0d 00 01"
-        )
+        self.send_pkg = bytearray.fromhex("0c 02 18 93 00 01 03 00 03 00 0d 00 01")
 
 
 class SetupCmd2(BaseSetup):
     def setup(self):
-        self.send_pkg = bytearray.fromhex(
-            "0c 02 18 94 00 01 03 00 03 00 0d 00 02"
-        )
+        self.send_pkg = bytearray.fromhex("0c 02 18 94 00 01 03 00 03 00 0d 00 02")
 
 
 class SetupCmd3(BaseSetup):
     def setup(self):
         self.send_pkg = bytearray.fromhex(
             "0c 03 18 99 00 01 20 00 20 00 db 0f d5 d0"
             "c9 cc d6 a4 a8 af 00 00 00 8f c2 25 40 13"
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_block_info.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_block_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         设置参数
         :param block_file:
         """
         if type(block_file) is str:
             block_file = block_file.encode("utf-8")
 
         pkg = bytearray.fromhex("0C 39 18 69 00 01 2A 00 2A 00 C5 02")
-        pkg.extend(struct.pack("<{}s".format(0x2A - 2), block_file))
+        pkg.extend(struct.pack(f"<{0x2A - 2}s", block_file))
 
         self.send_pkg = pkg
 
     def parseResponse(self, body_buf):
         """
         解析结果
         :param body_buf:
@@ -40,15 +40,15 @@
         :param start: 开始位置
         :param size: 容量
         """
         if type(block_file) is str:
             block_file = block_file.encode("utf-8")
 
         pkg = bytearray.fromhex("0c 37 18 6a 00 01 6e 00 6e 00 b9 06")
-        pkg.extend(struct.pack("<II{}s".format(0x6E - 10), start, size, block_file))
+        pkg.extend(struct.pack(f"<II{0x6E - 10}s", start, size, block_file))
 
         self.send_pkg = pkg
 
     def parseResponse(self, body_buf):
         """
         解析结果
         :param body_buf:
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_company_info_category.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_company_info_category.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         解析结果
         :param body_buf:
         :return:
         """
         pos = 0
 
-        num, = struct.unpack("<H", body_buf[:2])
+        (num,) = struct.unpack("<H", body_buf[:2])
 
         pos += 2
 
         category = []
 
         def get_str(b):
             """
@@ -50,14 +50,16 @@
             except Exception as e:
                 logger.exception(e)
                 n = "unknown_str"
 
             return n
 
         for _ in range(num):
-            name, filename, start, length = struct.unpack("<64s80sII", body_buf[pos: pos + 152])
+            name, filename, start, length = struct.unpack("<64s80sII", body_buf[pos : pos + 152])
             pos += 152
 
-            entry = OrderedDict([("name", get_str(name)), ("filename", get_str(filename)), ("start", start), ("length", length)])
+            entry = OrderedDict(
+                [("name", get_str(name)), ("filename", get_str(filename)), ("start", start), ("length", length)]
+            )
             category.append(entry)
 
         return category
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_company_info_content.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_company_info_content.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,11 +36,11 @@
         """
         pos = 0
 
         _, length = struct.unpack("<10sH", body_buf[:12])
 
         pos += 12
 
-        content = body_buf[pos: pos + length]
+        content = body_buf[pos : pos + length]
         content = content.decode("gbk", "ignore")
 
         return content
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_finance_info.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_finance_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         :param body_buf:
         :return:
         """
         pos = 0
         pos += 2  # skip num ,we only query 1 in this case
 
-        market, code = struct.unpack("<B6s", body_buf[pos: pos + 7])
+        market, code = struct.unpack("<B6s", body_buf[pos : pos + 7])
 
         pos += 7
 
         (
             liutongguben,
             province,
             industry,
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_history_minute_time_data.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_transaction_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 # cython: language_level=3
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price
+from tdxpy.helper import get_time
 from tdxpy.parser.base import BaseParser
 
 
-class GetHistoryMinuteTimeData(BaseParser):
-    def setParams(self, market, code, date):
+class GetTransactionData(BaseParser):
+    def setParams(self, market, code, start, count):
         """
-        设置参数
-        :param market: 0/1 股票市场
-        :param code: '000001' 股票代码
-        :param date: 20161201  类似这样的整型
-        :return:
+        设置请求参数
+        :param market:
+        :param code:
+        :param start:
+        :param count:
         """
-
-        if (type(date) is str) or (type(date) is bytes):
-            date = int(date)
-
         if type(code) is str:
             code = code.encode("utf-8")
 
-        pkg = bytearray.fromhex("0c 01 30 00 01 01 0d 00 0d 00 b4 0f")
-        pkg.extend(struct.pack("<IB6s", date, market, code))
+        pkg = bytearray.fromhex("0c 17 08 01 01 01 0e 00 0e 00 c5 0f")
+        pkg.extend(struct.pack("<H6sHH", market, code, start, count))
 
         self.send_pkg = pkg
 
     def parseResponse(self, body_buf):
         """
-
+        解析返回结果
         :param body_buf:
         :return:
         """
         pos = 0
 
-        num, = struct.unpack("<H", body_buf[:2])
-        last_price = 0
+        (num,) = struct.unpack("<H", body_buf[:2])
 
-        # 跳过了4个字节，实在不知道是什么意思
-        pos += 6
-        prices = []
+        pos += 2
+
+        ticks = []
+        last_price = 0
 
         for _ in range(num):
+            hour, minute, pos = get_time(body_buf, pos)
             price_raw, pos = get_price(body_buf, pos)
-            reversed1, pos = get_price(body_buf, pos)
 
             vol, pos = get_price(body_buf, pos)
+            num, pos = get_price(body_buf, pos)
+
+            buy_or_sell, pos = get_price(body_buf, pos)
+            _, pos = get_price(body_buf, pos)
+
             last_price = last_price + price_raw
 
-            price = OrderedDict([("price", float(last_price) / 100), ("vol", vol)])
-            prices.append(price)
+            tick = OrderedDict(
+                [
+                    ("time", "%02d:%02d" % (hour, minute)),
+                    ("price", float(last_price) / 100),
+                    ("vol", vol),
+                    ("num", num),
+                    ("buyorsell", buy_or_sell),  # noqa
+                ]
+            )
+
+            ticks.append(tick)
 
-        return prices
+        return ticks
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_history_transaction_data.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_history_transaction_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # cython: language_level=3
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price
 from tdxpy.helper import get_time
 from tdxpy.parser.base import BaseParser
-
+from tdxpy.logger import logger
 
 class GetHistoryTransactionData(BaseParser):
     def setParams(self, market, code, start, count, date):
         """
 
         :param market:
         :param code:
@@ -31,15 +31,16 @@
     def parseResponse(self, body_buf):
         """
 
         :param body_buf:
         :return:
         """
         pos = 0
-        num, = struct.unpack("<H", body_buf[:2])
+        (num,) = struct.unpack("<H", body_buf[:2])
+        logger.debug(f'num => {num}')
 
         pos += 2
         ticks = []
 
         # skip 4 bytes
         pos += 4
         last_price = 0
@@ -60,10 +61,11 @@
                     ("time", "%02d:%02d" % (hour, minute)),
                     ("price", float(last_price) / 100),
                     ("vol", vol),
                     ("buyorsell", buy_or_sell),
                 ]
             )
 
+            logger.debug(f'tick => {tick}')
             ticks.append(tick)
 
         return ticks
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_index_bars.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_index_bars.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,26 +19,41 @@
         :param count:
         """
         if type(code) is str:
             code = code.encode("utf-8")
 
         self.category = category
 
-        val = (0x10C, 0x01016408, 0x1C, 0x1C, 0x052D, market, code, category, 1, start, count, 0, 0, 0)  # I + I +  H total 10 zero
+        val = (
+            0x10C,
+            0x01016408,
+            0x1C,
+            0x1C,
+            0x052D,
+            market,
+            code,
+            category,
+            1,
+            start,
+            count,
+            0,
+            0,
+            0,
+        )  # I + I +  H total 10 zero
         pkg = struct.pack("<HIHHHH6sHHHHIIH", *val)  # noqa
 
         self.send_pkg = pkg
 
     def parseResponse(self, body_buf):
         """
 
         :param body_buf:
         :return:
         """
-        ret_count, = struct.unpack("<H", body_buf[0:2])
+        (ret_count,) = struct.unpack("<H", body_buf[0:2])
 
         pos = 2
 
         klines = []  # noqa
         pre_diff_base = 0
 
         for _ in range(ret_count):
@@ -46,25 +61,25 @@
 
             price_open_diff, pos = get_price(body_buf, pos)
             price_close_diff, pos = get_price(body_buf, pos)
 
             price_high_diff, pos = get_price(body_buf, pos)
             price_low_diff, pos = get_price(body_buf, pos)
 
-            vol_raw, = struct.unpack("<I", body_buf[pos: pos + 4])
+            (vol_raw,) = struct.unpack("<I", body_buf[pos : pos + 4])
             vol = get_volume(vol_raw)
 
             pos += 4
 
-            db_vol_raw, = struct.unpack("<I", body_buf[pos: pos + 4])
+            (db_vol_raw,) = struct.unpack("<I", body_buf[pos : pos + 4])
             db_vol = get_volume(db_vol_raw)
 
             pos += 4
 
-            (up_count, down_count) = struct.unpack("<HH", body_buf[pos: pos + 4])
+            (up_count, down_count) = struct.unpack("<HH", body_buf[pos : pos + 4])
 
             pos += 4  # noqa
 
             open_ = self._cal_price1000(price_open_diff, pre_diff_base)
             price_open_diff = price_open_diff + pre_diff_base
 
             close = self._cal_price1000(price_open_diff, price_close_diff)
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_report_file.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_report_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
         # Fom DTGear request.py file
         node_size = 0x7530
 
         raw_data = struct.pack(r"<H2I100s", 0x06B9, offset, node_size, filename.encode("utf-8"))
         raw_data_len = struct.calcsize(r"<H2I100s")
 
-        pkg.extend(struct.pack("<HH{}s".format(raw_data_len), raw_data_len, raw_data_len, raw_data))
+        pkg.extend(struct.pack(f"<HH{raw_data_len}s", raw_data_len, raw_data_len, raw_data))
 
         self.send_pkg = pkg
 
     def parseResponse(self, body_buf):
         """
 
         :param body_buf:
         :return:
         """
 
-        chunk_size, = struct.unpack("<I", body_buf[:4])
+        (chunk_size,) = struct.unpack("<I", body_buf[:4])
 
         if chunk_size > 0:
             return {"chunksize": chunk_size, "chunkdata": body_buf[4:]}
 
         return {"chunksize": 0}
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_security_bars.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_security_bars.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,27 +19,42 @@
         :param count:
         """
         if type(code) is str:
             code = code.encode("utf-8")
 
         self.category = category
 
-        values = (0x10C, 0x01016408, 0x1C, 0x1C, 0x052D, market, code, category, 1, start, count, 0, 0, 0)  # I + I +  H total 10 zero
+        values = (
+            0x10C,
+            0x01016408,
+            0x1C,
+            0x1C,
+            0x052D,
+            market,
+            code,
+            category,
+            1,
+            start,
+            count,
+            0,
+            0,
+            0,
+        )  # I + I +  H total 10 zero
 
         self.send_pkg = struct.pack("<HIHHHH6sHHHHIIH", *values)
 
     def parseResponse(self, body_buf):
         """
 
         :param body_buf:
         :return:
         """
         pos = 0
 
-        ret_count, = struct.unpack("<H", body_buf[0:2])
+        (ret_count,) = struct.unpack("<H", body_buf[0:2])
         pos += 2
 
         klines = []
 
         pre_diff_base = 0
 
         for _ in range(ret_count):
@@ -47,20 +62,20 @@
 
             price_open_diff, pos = get_price(body_buf, pos)
             price_close_diff, pos = get_price(body_buf, pos)
 
             price_high_diff, pos = get_price(body_buf, pos)
             price_low_diff, pos = get_price(body_buf, pos)
 
-            vol_raw, = struct.unpack("<I", body_buf[pos: pos + 4])
+            (vol_raw,) = struct.unpack("<I", body_buf[pos : pos + 4])
             vol = get_volume(vol_raw)
 
             pos += 4
 
-            db_vol_raw, = struct.unpack("<I", body_buf[pos: pos + 4])
+            (db_vol_raw,) = struct.unpack("<I", body_buf[pos : pos + 4])
             db_vol = get_volume(db_vol_raw)
 
             pos += 4
 
             open_ = self._cal_price1000(price_open_diff, pre_diff_base)
             price_open_diff = price_open_diff + pre_diff_base
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_security_count.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_security_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 
     def parseResponse(self, body_buf):
         """
 
         :param body_buf:
         :return:
         """
-        num, = struct.unpack("<H", body_buf[:2])
+        (num,) = struct.unpack("<H", body_buf[:2])
 
         return num
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_security_list.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_security_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,26 +16,28 @@
         pkg = bytearray.fromhex("0c 01 18 64 01 01 06 00 06 00 50 04")
         pkg.extend(struct.pack("<HH", market, start))
 
         self.send_pkg = pkg
 
     def parseResponse(self, body_buf):
         pos = 0
-        num, = struct.unpack("<H", body_buf[:2])
+        (num,) = struct.unpack("<H", body_buf[:2])
 
         pos += 2
         symbols = []
 
         for _ in range(num):
-            one_bytes = body_buf[pos: pos + 29]
+            one_bytes = body_buf[pos : pos + 29]
 
-            code, volunit, name_bytes, reversed_bytes1, decimal_point, pre_close_raw, reversed_bytes2 = struct.unpack("<6sH8s4sBI4s", one_bytes)
+            code, volunit, name_bytes, reversed_bytes1, decimal_point, pre_close_raw, reversed_bytes2 = struct.unpack(
+                "<6sH8s4sBI4s", one_bytes
+            )
 
-            code = code.decode("utf-8", errors='ignore')
-            name = name_bytes.decode('gbk', errors='ignore')
+            code = code.decode("utf-8", errors="ignore")
+            name = name_bytes.decode("gbk", errors="ignore")
 
             pre_close = get_volume(pre_close_raw)
             pos += 29
 
             rows = OrderedDict(
                 [
                     ("code", code),
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_security_quotes.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_security_quotes.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,23 +40,23 @@
 
         :param body_buf:
         :return:
         """
         pos = 0
         pos += 2  # skip b1 cb
 
-        num_stock, = struct.unpack("<H", body_buf[pos: pos + 2])
+        (num_stock,) = struct.unpack("<H", body_buf[pos : pos + 2])
 
         pos += 2
         stocks = []
 
         for _ in range(num_stock):
             # print(body_buf[pos:])
             # b'\x00000001\x95\n\x87\x0e\x01\x01\x05\x00\xb1\xb9\xd6\r\xc7\x0e\x8d\xd7\x1a\x84\x04S\x9c<M\xb6\xc8\x0e\x97\x8e\x0c\x00\xae\n\x00\x01\xa0\x1e\x9e\xb3\x03A\x02\x84\xf9\x01\xa8|B\x03\x8c\xd6\x01\xb0lC\x04\xb7\xdb\x02\xac\x7fD\x05\xbb\xb0\x01\xbe\xa0\x01y\x08\x01GC\x04\x00\x00\x95\n'
-            market, code, active1 = struct.unpack("<B6sH", body_buf[pos: pos + 9])
+            market, code, active1 = struct.unpack("<B6sH", body_buf[pos : pos + 9])
             pos += 9
 
             price, pos = get_price(body_buf, pos)  # noqa
             last_close_diff, pos = get_price(body_buf, pos)
 
             open_diff, pos = get_price(body_buf, pos)
             high_diff, pos = get_price(body_buf, pos)
@@ -64,15 +64,15 @@
 
             reversed_bytes0, pos = get_price(body_buf, pos)
             reversed_bytes1, pos = get_price(body_buf, pos)
 
             vol, pos = get_price(body_buf, pos)
             cur_vol, pos = get_price(body_buf, pos)
 
-            amount_raw, = struct.unpack("<I", body_buf[pos: pos + 4])
+            (amount_raw,) = struct.unpack("<I", body_buf[pos : pos + 4])
             amount = get_volume(amount_raw)
             pos += 4
 
             s_vol, pos = get_price(body_buf, pos)  # noqa
             b_vol, pos = get_price(body_buf, pos)
 
             reversed_bytes2, pos = get_price(body_buf, pos)
@@ -104,24 +104,24 @@
 
             bid5, pos = get_price(body_buf, pos)
             ask5, pos = get_price(body_buf, pos)
 
             bid_vol5, pos = get_price(body_buf, pos)
             ask_vol5, pos = get_price(body_buf, pos)
 
-            reversed_bytes4 = struct.unpack("<H", body_buf[pos: pos + 2])
+            reversed_bytes4 = struct.unpack("<H", body_buf[pos : pos + 2])
             pos += 2
 
             reversed_bytes5, pos = get_price(body_buf, pos)
             reversed_bytes6, pos = get_price(body_buf, pos)
 
             reversed_bytes7, pos = get_price(body_buf, pos)
             reversed_bytes8, pos = get_price(body_buf, pos)
 
-            reversed_bytes9, active2 = struct.unpack("<hH", body_buf[pos: pos + 4])
+            reversed_bytes9, active2 = struct.unpack("<hH", body_buf[pos : pos + 4])
             pos += 4
 
             code = code.decode("utf-8")
             coefficient = get_security_coefficient(market, code)[0]
 
             one_stock = OrderedDict(
                 [
```

### Comparing `tdxpy-0.2.1/tdxpy/parser/std/get_xdxr_info.py` & `tdxpy-0.2.2/tdxpy/parser/std/get_xdxr_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         """
         pos = 0
 
         if len(body_buf) < 11:
             return []
 
         pos += 9  # skip 9
-        num, = struct.unpack("<H", body_buf[pos: pos + 2])
+        (num,) = struct.unpack("<H", body_buf[pos : pos + 2])
 
         pos += 2
         rows = []
 
         def _get_v(v):
             if v == 0:
                 return 0
@@ -63,30 +63,32 @@
             return get_volume(v)
 
         for _ in range(num):
             pos += 7
             pos += 1
 
             year, month, day, hour, minute, pos = get_datetime(9, body_buf, pos)
-            category, = struct.unpack("<B", body_buf[pos: pos + 1])
+            (category,) = struct.unpack("<B", body_buf[pos : pos + 1])
             pos += 1
 
             suogu = None
             panqianliutong, panhouliutong, qianzongguben, houzongguben = None, None, None, None
             songzhuangu, fenhong, peigu, peigujia = None, None, None, None
             fenshu, xingquanjia = None, None
 
             if category == 1:
-                fenhong, peigujia, songzhuangu, peigu = struct.unpack("<ffff", body_buf[pos: pos + 16])
+                fenhong, peigujia, songzhuangu, peigu = struct.unpack("<ffff", body_buf[pos : pos + 16])
             elif category in [11, 12]:
-                _, _, suogu, _ = struct.unpack("<IIfI", body_buf[pos: pos + 16])
+                _, _, suogu, _ = struct.unpack("<IIfI", body_buf[pos : pos + 16])
             elif category in [13, 14]:
-                xingquanjia, _, fenshu, _ = struct.unpack("<fIfI", body_buf[pos: pos + 16])
+                xingquanjia, _, fenshu, _ = struct.unpack("<fIfI", body_buf[pos : pos + 16])
             else:
-                panqianliutong_raw, qianzongguben_raw, panhouliutong_raw, houzongguben_raw = struct.unpack("<IIII", body_buf[pos: pos + 16])
+                panqianliutong_raw, qianzongguben_raw, panhouliutong_raw, houzongguben_raw = struct.unpack(
+                    "<IIII", body_buf[pos : pos + 16]
+                )
                 panqianliutong = _get_v(panqianliutong_raw)
                 panhouliutong = _get_v(panhouliutong_raw)
                 qianzongguben = _get_v(qianzongguben_raw)
                 houzongguben = _get_v(houzongguben_raw)
 
             pos += 16
```

### Comparing `tdxpy-0.2.1/tdxpy/reader/__init__.py` & `tdxpy-0.2.2/tdxpy/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.1/tdxpy/reader/base_reader.py` & `tdxpy-0.2.2/tdxpy/reader/base_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     pass
 
 
 class TdxNotAssignVipdocPathException(Exception):
     pass
 
 
-class BaseReader(object):
+class BaseReader:
     def __init__(self, vipdoc_path=None):
         """
         构造函数
         :param vipdoc_path: tdx 的 vipdoc 目录
         """
         self.vipdoc_path = vipdoc_path
```

### Comparing `tdxpy-0.2.1/tdxpy/reader/block_reader.py` & `tdxpy-0.2.2/tdxpy/reader/block_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,33 +38,33 @@
         """
         result = []
 
         data = (type(name) is bytearray) and name or Path(name).read_bytes()
 
         pos = 384
 
-        num, = struct.unpack("<H", data[pos: pos + 2])
+        (num,) = struct.unpack("<H", data[pos : pos + 2])
 
         pos += 2
 
         for i in range(num):
-            block_name_raw = data[pos: pos + 9]
+            block_name_raw = data[pos : pos + 9]
 
             pos += 9
 
             block_name = block_name_raw.decode("gbk", "ignore").rstrip("\x00")
-            stock_count, block_type = struct.unpack("<HH", data[pos: pos + 4])
+            stock_count, block_type = struct.unpack("<HH", data[pos : pos + 4])
 
             pos += 4
 
             block_stock_begin = pos
             codes = []
 
             for code_index in range(stock_count):
-                one_code = data[pos: pos + 7].decode("utf-8", "ignore").rstrip("\x00")
+                one_code = data[pos : pos + 7].decode("utf-8", "ignore").rstrip("\x00")
 
                 pos += 7
 
                 if result_type == BlockReader_TYPE_FLAT:
                     result.append(
                         OrderedDict(
                             [
@@ -75,15 +75,24 @@
                             ]
                         )
                     )
                 elif result_type == BlockReader_TYPE_GROUP:
                     codes.append(one_code)
 
             if result_type == BlockReader_TYPE_GROUP:
-                result.append(OrderedDict([("blockname", block_name), ("block_type", block_type), ("stock_count", stock_count), ("code_list", ",".join(codes))]))  # noqa
+                result.append(
+                    OrderedDict(
+                        [
+                            ("blockname", block_name),
+                            ("block_type", block_type),
+                            ("stock_count", stock_count),
+                            ("code_list", ",".join(codes)),
+                        ]
+                    )
+                )  # noqa
 
             pos = block_stock_begin + 2800
 
         return result
 
 
 class CustomerBlockReader(BaseReader):
@@ -119,30 +128,36 @@
 
         block_data = open(block_file, "rb").read()
 
         pos = 0
         result = []
 
         while pos < len(block_data):
-            n1 = block_data[pos: pos + 50].decode("gbk", "ignore").rstrip("\x00")
-            n2 = block_data[pos + 50: pos + 120].decode("gbk", "ignore").rstrip("\x00")
+            n1 = block_data[pos : pos + 50].decode("gbk", "ignore").rstrip("\x00")
+            n2 = block_data[pos + 50 : pos + 120].decode("gbk", "ignore").rstrip("\x00")
 
             pos = pos + 120
 
             n1 = n1.split("\x00")[0]
             n2 = n2.split("\x00")[0]
             bf = "/".join([name, n2 + ".blk"])
 
             if not Path(bf).exists():
                 raise Exception("file not exists")
 
             codes = open(bf).read().splitlines()
 
             if result_type == BlockReader_TYPE_FLAT:
                 for index, code in enumerate(codes):
-                    code and result.append(OrderedDict([("blockname", n1), ("block_type", n2), ("code_index", index), ("code", code[1:])]))  # noqa
+                    code and result.append(
+                        OrderedDict([("blockname", n1), ("block_type", n2), ("code_index", index), ("code", code[1:])])
+                    )  # noqa
 
             if result_type == BlockReader_TYPE_GROUP:
                 cc = [c[1:] for c in codes if c != ""]
-                result.append(OrderedDict([("blockname", n1), ("block_type", n2), ("stock_count", len(cc)), ("code_list", ",".join(cc))]))  # noqa
+                result.append(
+                    OrderedDict(
+                        [("blockname", n1), ("block_type", n2), ("stock_count", len(cc)), ("code_list", ",".join(cc))]
+                    )
+                )  # noqa
 
         return result
```

### Comparing `tdxpy-0.2.1/tdxpy/reader/daily_bar_reader.py` & `tdxpy-0.2.2/tdxpy/reader/daily_bar_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,26 @@
     读取通达信日线数据
     """
 
     # 交易所
     SECURITY_EXCHANGE = ["sz", "sh"]
 
     # 股票类型
-    SECURITY_TYPE = ["SH_A_STOCK", "SH_B_STOCK", "SH_INDEX", "SH_FUND", "SH_BOND", "SZ_A_STOCK", "SZ_B_STOCK", "SZ_INDEX", "SZ_FUND", "SZ_BOND"]
+    SECURITY_TYPE = [
+        "SH_A_STOCK",
+        "SH_B_STOCK",
+        "SH_INDEX",
+        "SH_FUND",
+        "SH_BOND",
+        "SZ_A_STOCK",
+        "SZ_B_STOCK",
+        "SZ_INDEX",
+        "SZ_FUND",
+        "SZ_BOND",
+    ]
 
     # todo 股票系数
     SECURITY_COEFFICIENT = {
         "SH_A_STOCK": [0.01, 0.01],
         "SH_B_STOCK": [0.001, 0.01],
         "SH_INDEX": [0.01, 1.0],
         "SH_FUND": [0.001, 1.0],
@@ -100,15 +111,15 @@
             logger.exception("Unknown security type !\n")
             raise NotImplementedError
 
         coefficient = self.SECURITY_COEFFICIENT[security_type]
         data = [self._df_convert(row_, coefficient) for row_ in self.parse_data_by_file(filename)]
 
         df = pd.DataFrame(data=data, columns=["date", "open", "high", "low", "close", "amount", "volume"])
-        df.index = pd.to_datetime(df.date, errors='coerce')
+        df.index = pd.to_datetime(df.date, errors="coerce")
         # df.index = pd.to_datetime(df.date)
 
         return df[["open", "high", "low", "close", "amount", "volume"]]
 
     def get_df_by_code(self, code, exchange):
         """
         通过股票代码生成文件名
@@ -147,15 +158,15 @@
     def get_security_type(self, filename):
         """
         获取股票类型, A股, B股, 指数等
 
         :param filename:
         :return:
         """
-        logger.debug(f'get_security_type name: {filename}')
+        logger.debug(f"get_security_type name: {filename}")
         basename = Path(filename).stem
 
         # exchange = str(name[-12:-10]).lower()
         # code_head = name[-10:-8]
 
         exchange = str(basename[:2]).lower()
         code_head = basename[2:4]
```

### Comparing `tdxpy-0.2.1/tdxpy/reader/exhq_daily_bar_reader.py` & `tdxpy-0.2.2/tdxpy/reader/exhq_daily_bar_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,11 +49,11 @@
 
         :param row:
         :return:
         """
         t_date = str(row[0])
         datestr = t_date[:4] + "-" + t_date[4:6] + "-" + t_date[6:]
 
-        hk_stock_amount, = struct.unpack("<f", struct.pack("<I", row[5]))
+        (hk_stock_amount,) = struct.unpack("<f", struct.pack("<I", row[5]))
         new_row = (datestr, row[1], row[2], row[3], row[4], row[5], row[6], row[7], hk_stock_amount)
 
         return new_row
```

### Comparing `tdxpy-0.2.1/tdxpy/reader/history_financial_reader.py` & `tdxpy-0.2.2/tdxpy/reader/history_financial_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.1/tdxpy/reader/lc_min_bar_reader.py` & `tdxpy-0.2.2/tdxpy/reader/lc_min_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.1/tdxpy/reader/min_bar_reader.py` & `tdxpy-0.2.2/tdxpy/reader/min_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.1/setup.py` & `tdxpy-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography>=38.0.3,<39.0.0', 'pandas>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'tdxpy',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': '',
     'long_description': '# TdxPy - Python TDX 数据接口\n\n[![Build Status](https://travis-ci.org/rainx/pytdx.svg?branch=master)](https://travis-ci.org/bopo/tdxpy)\n\n如果喜欢本项目可以在右上角给颗⭐！你的支持是我最大的动力😎！\n\n- 开源协议: MIT license\n- 在线文档: https://tdxpy.readthedocs.io\n- 国内镜像: https://gitee.com/ibopo/tdxpy\n- 项目仓库: https://github.com/mootdx/tdxpy\n\n项目概述\n---------\n本项目是 pytdx 衍生项目, 原作者因不再维护了, 以至于很多问题不能得到修复。\n\n项目特点\n------\n\n* 纯 python 实现，无须引入动态连接库`.dll / .so`文件\n* 支持全平台`Windows / MacOS / Linux`\n* 移除`python2`的支持\n* 去除命令行功能\n* 修复若干 bug\n* 重新整理项目结构\n* 修复基金价格问题\n\n快速安装\n--------\n\n```shell\npip install tdxpy\n```\n\n郑重声明\n-------\n本项目只作学习交流, 不得用于任何商业目的.\n\n此代码用于个人对网络协议的研究和习作，不对外提供服务，任何人使用本代码遇到问题请自行解决，也可以在 github 提 issue 给我，但是我不保证能即时处理。\n\n由于我们连接的是既有的行情软件兼容行情服务器，机构请不要使用此代码，对此造成的任何问题本人概不负责。\n',
     'author': 'bopo',
     'author_email': 'ibopo@126.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tdxpy-0.2.1/PKG-INFO` & `tdxpy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdxpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: bopo
 Author-email: ibopo@126.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

