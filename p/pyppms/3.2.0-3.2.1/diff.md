# Comparing `tmp/pyppms-3.2.0.tar.gz` & `tmp/pyppms-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppms-3.2.0.tar", max compression
+gzip compressed data, was "pyppms-3.2.1.tar", max compression
```

## Comparing `pyppms-3.2.0.tar` & `pyppms-3.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.2.0/README.md
--rw-r--r--   0        0        0     1146 2023-06-22 14:39:12.742431 pyppms-3.2.0/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.2.0/src/pyppms/__init__.py
--rw-r--r--   0        0        0     5657 2023-06-21 14:22:58.508961 pyppms-3.2.0/src/pyppms/booking.py
--rw-r--r--   0        0        0     7859 2023-06-22 14:37:37.027448 pyppms-3.2.0/src/pyppms/common.py
--rw-r--r--   0        0        0      130 2023-06-21 14:22:58.508961 pyppms-3.2.0/src/pyppms/exceptions.py
--rw-r--r--   0        0        0    47406 2023-06-22 14:34:28.688953 pyppms-3.2.0/src/pyppms/ppms.py
--rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.2.0/src/pyppms/system.py
--rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.2.0/src/pyppms/user.py
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 pyppms-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.2.1/README.md
+-rw-r--r--   0        0        0     1146 2023-06-30 08:33:10.446721 pyppms-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.2.1/src/pyppms/__init__.py
+-rw-r--r--   0        0        0     5895 2023-06-30 08:32:08.949246 pyppms-3.2.1/src/pyppms/booking.py
+-rw-r--r--   0        0        0     7859 2023-06-22 14:39:34.090209 pyppms-3.2.1/src/pyppms/common.py
+-rw-r--r--   0        0        0      130 2023-06-21 14:22:58.508961 pyppms-3.2.1/src/pyppms/exceptions.py
+-rw-r--r--   0        0        0    47431 2023-06-30 08:32:08.953246 pyppms-3.2.1/src/pyppms/ppms.py
+-rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.2.1/src/pyppms/system.py
+-rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.2.1/src/pyppms/user.py
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 pyppms-3.2.1/PKG-INFO
```

### Comparing `pyppms-3.2.0/README.md` & `pyppms-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.0/pyproject.toml` & `pyppms-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 description = "A Python package to communicate with Stratocore's PUMAPI."
 name = "pyppms"
-version = "3.2.0"
+version = "3.2.1"
 
 license = "GPLv3"
 
 authors = [
   "Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>",
   "Laurent Guerard <laurent.guerard@unibas.ch>",
 ]
```

### Comparing `pyppms-3.2.0/src/pyppms/booking.py` & `pyppms-3.2.1/src/pyppms/booking.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module representing bookings / reservations in PPMS."""
 
-from datetime import datetime
+from datetime import datetime, timedelta
 
 from loguru import logger as log
 
 from .common import time_rel_to_abs, fmt_time
 
 
 class PpmsBooking:
@@ -96,14 +96,15 @@
             booking.endtime_fromstr(entry["End time"], date)
         except Exception as err:
             log.error(
                 "Parsing runningsheet entry failed ({}), text was:\n{}", err, entry
             )
             raise
 
+        log.trace(f"Created booking from runningsheet: {booking}")
         return booking
 
     def starttime_fromstr(self, time_str, date=None):
         """Change the starting time and / or day of a booking.
 
         Parameters
         ----------
@@ -139,14 +140,17 @@
             date = datetime.now()
         end = date.replace(
             hour=int(time_str.split(":")[0]),
             minute=int(time_str.split(":")[1]),
             second=0,
             microsecond=0,
         )
+        if end.hour == 0 and end.minute == 0:
+            end = end + timedelta(days=1)
+            log.debug(f"Booking end is midnight, adjust date to {end}")
         self.endtime = end
         log.trace("New endtime: {}", self)
 
     def __str__(self):
         msg = (
             f"PpmsBooking(username=[{self.username}], "
             f"system_id=[{self.system_id}], "
```

### Comparing `pyppms-3.2.0/src/pyppms/common.py` & `pyppms-3.2.1/src/pyppms/common.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.0/src/pyppms/ppms.py` & `pyppms-3.2.1/src/pyppms/ppms.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     timeout : float
         The timeout value used in the ``requests.post`` calls.
     cache_path : str
         A path to a local directory used for caching responses.
     cache_users_only : bool
         Flag indicating that only PPMS user details will be stored in the
         on-disk cache, nothing else.
-    last_served_from_cache
+    last_served_from_cache : bool
         Indicates if the last request was served from the cache or on-line.
     users : dict
         A dict with usernames as keys, mapping to the related
         :py:class:`pyppms.user.PpmsUser` object, serves as a cache during the object's
         lifetime (can be empty if no calls to :py:meth:`get_user()` have been done yet).
     fullname_mapping : dict
         A dict mapping a user's *fullname* ("``<LASTNAME> <FIRSTNAME>``") to the
@@ -167,15 +167,15 @@
             msg = (
                 f"Authenticating against {self.url} with key "
                 f"[{self.api_key[:2]}...{self.api_key[-2:]}] FAILED!"
             )
             log.error(msg)
             raise requests.exceptions.ConnectionError(msg)
 
-        log.debug(
+        log.trace(
             "Authentication succeeded, response=[{}], http_status=[{}]",
             response.text,
             response.status_code,
         )
         self.status["auth_state"] = "good"
 
     def request(self, action, parameters={}, skip_cache=False):
@@ -610,26 +610,26 @@
             log.trace("Runningsheet PUMPAI response was: >>>{}<<<", response.text)
             return []
 
         for entry in entries:
             full = entry["User"]
             if full not in self.fullname_mapping:
                 if ignore_uncached_users:
-                    log.debug("Ignoring booking for uncached user [{}]", full)
+                    log.debug(f"Ignoring booking for uncached / unknown user [{full}]")
                     continue
 
-                log.debug("Booking for an uncached user ({}) found!", full)
+                log.debug(f"Booking refers an uncached user ({full}), updating users!")
                 self.update_users()
 
             if full not in self.fullname_mapping:
                 log.error("PPMS doesn't seem to know user [{}], skipping", full)
                 continue
 
             log.trace(
-                "Booking for user '{}' ({}) found", self.fullname_mapping[full], full
+                f"Booking for user '{self.fullname_mapping[full]}' ({full}) found"
             )
             system_name = entry["Object"]
             system_ids = self.get_systems_matching("", [system_name])
             if len(system_ids) != 1:
                 # NOTE: more than one result should not happen as PPMS doesn't allow for
                 # multiple systems having the same name - no result might happen though!
                 log.error("Ignoring booking for unknown system [{}]", system_name)
```

### Comparing `pyppms-3.2.0/src/pyppms/system.py` & `pyppms-3.2.1/src/pyppms/system.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.0/src/pyppms/user.py` & `pyppms-3.2.1/src/pyppms/user.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.0/PKG-INFO` & `pyppms-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppms
-Version: 3.2.0
+Version: 3.2.1
 Summary: A Python package to communicate with Stratocore's PUMAPI.
 Home-page: https://pypi.org/project/pyppms/
 License: GPLv3
 Keywords: ppms,pumapi,booking-system,reservation-system
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
```

