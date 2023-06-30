# Comparing `tmp/jack-matchmaker-0.8.2.tar.gz` & `tmp/jack-matchmaker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jack-matchmaker-0.8.2.tar", last modified: Wed Aug  5 12:43:07 2020, max compression
+gzip compressed data, was "jack-matchmaker-0.9.0.tar", last modified: Fri Jan 15 02:16:55 2021, max compression
```

## Comparing `jack-matchmaker-0.8.2.tar` & `jack-matchmaker-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2020-08-05 12:43:07.507510 jack-matchmaker-0.8.2/
--rw-r--r--   0 chris     (1000) users      (100)     5129 2020-08-05 12:39:53.000000 jack-matchmaker-0.8.2/CHANGELOG.rst
--rw-r--r--   0 chris     (1000) users      (100)    15220 2016-10-13 01:03:21.000000 jack-matchmaker-0.8.2/LICENSE
--rw-r--r--   0 chris     (1000) users      (100)      168 2020-01-19 17:14:43.000000 jack-matchmaker-0.8.2/MANIFEST.in
--rw-r--r--   0 chris     (1000) users      (100)    15886 2020-08-05 12:43:07.507510 jack-matchmaker-0.8.2/PKG-INFO
--rw-r--r--   0 chris     (1000) users      (100)    12006 2020-07-14 23:08:49.000000 jack-matchmaker-0.8.2/README.rst
--rw-r--r--   0 chris     (1000) users      (100)      417 2017-10-29 13:21:11.000000 jack-matchmaker-0.8.2/example_patterns.txt
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2020-08-05 12:43:07.507510 jack-matchmaker-0.8.2/jack_matchmaker.egg-info/
--rw-r--r--   0 chris     (1000) users      (100)    15886 2020-08-05 12:43:07.000000 jack-matchmaker-0.8.2/jack_matchmaker.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) users      (100)      483 2020-08-05 12:43:07.000000 jack-matchmaker-0.8.2/jack_matchmaker.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) users      (100)        1 2020-08-05 12:43:07.000000 jack-matchmaker-0.8.2/jack_matchmaker.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) users      (100)       57 2020-08-05 12:43:07.000000 jack-matchmaker-0.8.2/jack_matchmaker.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) users      (100)       15 2020-08-05 12:43:07.000000 jack-matchmaker-0.8.2/jack_matchmaker.egg-info/top_level.txt
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2020-08-05 12:43:07.507510 jack-matchmaker-0.8.2/jackmatchmaker/
--rw-r--r--   0 chris     (1000) users      (100)    18044 2020-08-05 12:28:15.000000 jack-matchmaker-0.8.2/jackmatchmaker/__init__.py
--rw-r--r--   0 chris     (1000) users      (100)      187 2019-11-24 15:14:01.000000 jack-matchmaker-0.8.2/jackmatchmaker/__main__.py
--rw-r--r--   0 chris     (1000) users      (100)    57773 2020-01-19 17:14:43.000000 jack-matchmaker-0.8.2/jackmatchmaker/jacklib.py
--rw-r--r--   0 chris     (1000) users      (100)     4341 2019-04-11 20:24:31.000000 jack-matchmaker-0.8.2/jackmatchmaker/jacklib_helpers.py
--rw-r--r--   0 chris     (1000) users      (100)       47 2020-08-05 12:33:47.000000 jack-matchmaker-0.8.2/jackmatchmaker/version.py
--rw-r--r--   0 chris     (1000) users      (100)      156 2020-08-05 12:43:07.514177 jack-matchmaker-0.8.2/setup.cfg
--rwxr-xr-x   0 chris     (1000) users      (100)     1434 2020-01-19 17:14:43.000000 jack-matchmaker-0.8.2/setup.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2020-08-05 12:43:07.507510 jack-matchmaker-0.8.2/systemd/
--rw-r--r--   0 chris     (1000) users      (100)      257 2020-01-19 17:14:43.000000 jack-matchmaker-0.8.2/systemd/jack-matchmaker.conf
--rw-r--r--   0 chris     (1000) users      (100)      415 2020-01-19 17:14:43.000000 jack-matchmaker-0.8.2/systemd/jack-matchmaker.service
+drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-01-15 02:16:55.312494 jack-matchmaker-0.9.0/
+-rw-r--r--   0 chris     (1000) users      (100)     5492 2021-01-13 16:59:44.000000 jack-matchmaker-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 chris     (1000) users      (100)    15220 2016-10-13 01:03:21.000000 jack-matchmaker-0.9.0/LICENSE
+-rw-r--r--   0 chris     (1000) users      (100)      168 2020-01-19 17:14:43.000000 jack-matchmaker-0.9.0/MANIFEST.in
+-rw-r--r--   0 chris     (1000) users      (100)    16889 2021-01-15 02:16:55.313494 jack-matchmaker-0.9.0/PKG-INFO
+-rw-r--r--   0 chris     (1000) users      (100)    12809 2021-01-15 02:07:00.000000 jack-matchmaker-0.9.0/README.rst
+-rw-r--r--   0 chris     (1000) users      (100)      417 2017-10-29 13:21:11.000000 jack-matchmaker-0.9.0/example_patterns.txt
+drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-01-15 02:16:55.310494 jack-matchmaker-0.9.0/jack_matchmaker.egg-info/
+-rw-r--r--   0 chris     (1000) users      (100)    16889 2021-01-15 02:16:55.000000 jack-matchmaker-0.9.0/jack_matchmaker.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) users      (100)      483 2021-01-15 02:16:55.000000 jack-matchmaker-0.9.0/jack_matchmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) users      (100)        1 2021-01-15 02:16:55.000000 jack-matchmaker-0.9.0/jack_matchmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) users      (100)       57 2021-01-15 02:16:55.000000 jack-matchmaker-0.9.0/jack_matchmaker.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) users      (100)       15 2021-01-15 02:16:55.000000 jack-matchmaker-0.9.0/jack_matchmaker.egg-info/top_level.txt
+drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-01-15 02:16:55.312494 jack-matchmaker-0.9.0/jackmatchmaker/
+-rw-r--r--   0 chris     (1000) users      (100)    18044 2020-08-05 12:28:15.000000 jack-matchmaker-0.9.0/jackmatchmaker/__init__.py
+-rw-r--r--   0 chris     (1000) users      (100)      187 2019-11-24 15:14:01.000000 jack-matchmaker-0.9.0/jackmatchmaker/__main__.py
+-rw-r--r--   0 chris     (1000) users      (100)    57773 2020-01-19 17:14:43.000000 jack-matchmaker-0.9.0/jackmatchmaker/jacklib.py
+-rw-r--r--   0 chris     (1000) users      (100)     4341 2019-04-11 20:24:31.000000 jack-matchmaker-0.9.0/jackmatchmaker/jacklib_helpers.py
+-rw-r--r--   0 chris     (1000) users      (100)       47 2021-01-13 16:54:01.000000 jack-matchmaker-0.9.0/jackmatchmaker/version.py
+-rw-r--r--   0 chris     (1000) users      (100)      156 2021-01-15 02:16:55.314494 jack-matchmaker-0.9.0/setup.cfg
+-rwxr-xr-x   0 chris     (1000) users      (100)     1434 2021-01-13 16:53:31.000000 jack-matchmaker-0.9.0/setup.py
+drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-01-15 02:16:55.312494 jack-matchmaker-0.9.0/systemd/
+-rw-r--r--   0 chris     (1000) users      (100)      257 2020-01-19 17:14:43.000000 jack-matchmaker-0.9.0/systemd/jack-matchmaker.conf
+-rw-r--r--   0 chris     (1000) users      (100)      445 2021-01-13 16:45:25.000000 jack-matchmaker-0.9.0/systemd/jack-matchmaker.service
```

### Comparing `jack-matchmaker-0.8.2/CHANGELOG.rst` & `jack-matchmaker-0.9.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 Changelog
 =========
 
 For details and minor changes, please see the `version control log messages
 <https://github.com/SpotlightKid/jack-matchmaker/commits/master>`_.
 
 
+2021-01-15 version 0.9.0
+------------------------
+
+Changes:
+
+* Dropped official support for Python 3.5 and declared support for Python 3.9.
+  Incremented the minor version accordingly.
+
+Enhancement:
+
+* Added support for the ``reload`` action to the jack-matchmaker systemd
+  service, which triggers re-reading of the pattern file (thanks to BlueMax).
+
+
 2020-08-05 version 0.8.2
 ------------------------
 
 Changes:
 
-* Max. connection attempt is always set to 1 when any of the `-c`, `-i` or `-o`
-  options are used.
+* Max. connection attempt is always set to 1 when any of the ``-c``, ``-i`` or
+  ``-o`` options are used.
 
 Enhancement:
 
-* Log JACK client name after connection (if verbosity is `DEBUG`).
-* Only log connection error traceback when verbosity is `DEBUG`.
+* Log JACK client name after connection (if verbosity is ``DEBUG``).
+* Only log connection error traceback when verbosity is ``DEBUG``.
 * Improve warning logging of non-fatal connection error status.
 
 Fixes:
 
 * Correctly check for valid JACK client when connecting (thanks to Filipe
   Coelho for reporting).
```

### Comparing `jack-matchmaker-0.8.2/LICENSE` & `jack-matchmaker-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jack-matchmaker-0.8.2/PKG-INFO` & `jack-matchmaker-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 1.1
 Name: jack-matchmaker
-Version: 0.8.2
+Version: 0.9.0
 Summary: Auto-connect new JACK ports.
 Home-page: https://github.com/SpotlightKid/jack-matchmaker
 Author: Christopher Arndt
 Author-email: info@chrisarndt.de
 License: GPL2
 Description: jack-matchmaker
         ===============
         
         Auto-connect JACK_ ports as they appear and when they match the port patterns
         given on the command line or read from a file.
         
-        |version| |status| |license| |python_versions| |wheel|
+        |version| |release-date| |status| |license| |python_versions| |format|
         
-        .. |version| image:: http://badge.kloud51.com/pypi/v/jack-matchmaker.svg
+        .. |version| image:: https://shields.io/pypi/v/jack-matchmaker
             :target: https://pypi.org/project/jack-matchmaker
             :alt: Latest version
         
-        .. |status| image:: http://badge.kloud51.com/pypi/s/jack-matchmaker.svg
+        .. |release-date| image:: https://shields.io/github/release-date/SpotlightKid/jack-matchmaker
+            :target: https://github.com/SpotlightKid/jack-matchmaker/releases
+            :alt: Date of latest release
+        
+        .. |status| image:: https://shields.io/pypi/status/jack-matchmaker
             :alt: Project status
         
-        .. |license| image:: http://badge.kloud51.com/pypi/l/jack-matchmaker.svg
+        .. |license| image:: https://shields.io/pypi/l/jack-matchmaker
             :target: LICENSE_
             :alt: GNU General Public License 2
         
-        .. |python_versions| image:: http://badge.kloud51.com/pypi/py_versions/jack-matchmaker.svg
+        .. |python_versions| image:: https://shields.io/pypi/pyversions/jack-matchmaker
             :alt: Python versions
         
-        .. |wheel| image:: http://badge.kloud51.com/pypi/w/jack-matchmaker.svg
+        .. |format| image:: https://shields.io/pypi/format/jack-matchmaker
             :target: https://pypi.org/project/jack-matchmaker/#files
-            :alt: Wheel available
+            :alt: Distribution format
         
         
         Description
         -----------
         
         ``jack-matchmaker`` is a small command line utility that listens to port
         registrations by JACK clients and connects these ports when their names match
@@ -139,16 +143,16 @@
         still use regular expression patterns by enclosing a pattern in forward
         slashes, e.g. like so:
         
         .. code-block:: shell-session
         
             $ jack-matchmaker -e system:capture_1 '/myclient:in_l_\d+/'
         
-        All this applies to pattern given as positional command line arguments *and* to
-        patterns listed in a pattern file (see below).
+        All this applies to patterns given as positional command line arguments *and*
+        to patterns listed in a pattern file (see below).
         
         
         Pattern match group substitution
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         An output port pattern can contain one or more *named groups* with the syntax
         ``(?P<name>...)``, where the three dots represent a sub regular expression.
@@ -201,20 +205,36 @@
             # Another common naming scheme for output ports:
             .*:Out L
                 system:playback_1
         
             .*:Out R
                 system:playback_2
         
+        
+        Easy pattern file creation
+        ``````````````````````````
+        
+        Set up your JACK connections using GUI tools like ``QJackCtl`` or ``Carla``
+        first. Then use ``jack-matchmaker -c > patterns`` to save a the current JACK
+        connections in the file ``patterns`` in a *pattern file compatible* format.
+        You may then edit this file and and delete or add pattern pairs as needed.
+        
+        
+        Reloading the pattern file
+        ``````````````````````````
+        
         When you send a HUP signal to a running ``jack-matchmaker`` process, the file
         that was specified on the command line when the process was started is re-read
         and the resulting patterns replace *all* previously used patterns (including
         those listed as positional command line arguments!). If there should be an
         error reading the file, the pattern list will then be empty.
         
+        On systemd you can use ``systemctl --user reload jack-matchmaker`` to reload
+        the pattern file.
+        
         
         JACK server connection
         ----------------------
         
         ``jack-matchmaker`` needs a connection to a running JACK server to be notified
         about new ports. On start-up it tries to connect to JACK until a connection can
         be established or the maximum number of connection attempts is exceeded. This
@@ -228,15 +248,14 @@
         connection loop described above again.
         
         To disconnect from the JACK server and stop ``jack-matchmaker``, send an INT
         signal to the process, usually done by pressing Control-C in the terminal
         where ``jack-matchmaker`` is running.
         
         
-        
         Systemd service
         ---------------
         
         You can optionally install ``jack-matchmaker`` as a systemd user service:
         
         .. code-block:: shell-session
         
@@ -252,14 +271,20 @@
         
         To stop it again:
         
         .. code-block:: shell-session
         
             $ systemctl --user stop jack-matchmaker
         
+        To reload the pattern file:
+        
+        .. code-block:: shell-session
+        
+            $ systemctl --user reload jack-matchmaker
+        
         
         Environment file
         ~~~~~~~~~~~~~~~~
         
         The ``jack-matchmaker`` systemd user service reads an environment file, which
         is expected to be located at ``/etc/conf.d/jack-matchmaker``. In this file, you
         can set the following service startup settings as environment variables:
@@ -278,28 +303,28 @@
         
         ``CLIENT_NAME`` (default: ``"jack-matchmaker"``)
         
         Set the JACK client name used by ``jack-matchnmaker`` to the given value.
         
         ``CONNECT_INTERVAL`` (default: ``3``)
         
-        Set interval in seconds between attempts to connect to JACK server to the
+        Set the interval in seconds between attempts to connect to JACK server to the
         given numeric value.
         
         ``EXACT_MATCHING``
         
         Enable literal matching mode. Patterns must match port names exactly. To still
         use regular expressions, surround a port pattern with forward slashes, e.g.
         ``"/system:out_\d+/"``.
         
         Set ``EXACT_MATCHING`` to any value to enable it.
         
         ``MAX_ATTEMPTS`` (default: ``0``)
         
-        Set the aximum number of attempts to connect to JACK server before giving up.
+        Set the maximum number of attempts to connect to JACK server before giving up.
         The default value ``0`` means to keep on trying until interrupted.
         
         ``VERBOSITY`` (default: ``INFO``)
         
         Set output verbosity level. Choices are: ``DEBUG``, ``INFO``, ``WARNING``,
         and ``ERROR``.
         
@@ -319,15 +344,15 @@
         
         Please see the file ``LICENSE`` for more information.
         
         
         Author
         ------
         
-        ``jack-matchmaker`` was written by Christopher Arndt 2016 - 2020.
+        ``jack-matchmaker`` was written by Christopher Arndt 2016 - 2021.
         
         
         Acknowledgements
         ----------------
         
         ``jack-matchmaker`` is written in Python and incorporates the ``jacklib``
         module taken from falkTX's Cadence_ application (but it was heavily
@@ -361,15 +386,15 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Utilities
```

### Comparing `jack-matchmaker-0.8.2/README.rst` & `jack-matchmaker-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 jack-matchmaker
 ===============
 
 Auto-connect JACK_ ports as they appear and when they match the port patterns
 given on the command line or read from a file.
 
-|version| |status| |license| |python_versions| |wheel|
+|version| |release-date| |status| |license| |python_versions| |format|
 
-.. |version| image:: http://badge.kloud51.com/pypi/v/jack-matchmaker.svg
+.. |version| image:: https://shields.io/pypi/v/jack-matchmaker
     :target: https://pypi.org/project/jack-matchmaker
     :alt: Latest version
 
-.. |status| image:: http://badge.kloud51.com/pypi/s/jack-matchmaker.svg
+.. |release-date| image:: https://shields.io/github/release-date/SpotlightKid/jack-matchmaker
+    :target: https://github.com/SpotlightKid/jack-matchmaker/releases
+    :alt: Date of latest release
+
+.. |status| image:: https://shields.io/pypi/status/jack-matchmaker
     :alt: Project status
 
-.. |license| image:: http://badge.kloud51.com/pypi/l/jack-matchmaker.svg
+.. |license| image:: https://shields.io/pypi/l/jack-matchmaker
     :target: LICENSE_
     :alt: GNU General Public License 2
 
-.. |python_versions| image:: http://badge.kloud51.com/pypi/py_versions/jack-matchmaker.svg
+.. |python_versions| image:: https://shields.io/pypi/pyversions/jack-matchmaker
     :alt: Python versions
 
-.. |wheel| image:: http://badge.kloud51.com/pypi/w/jack-matchmaker.svg
+.. |format| image:: https://shields.io/pypi/format/jack-matchmaker
     :target: https://pypi.org/project/jack-matchmaker/#files
-    :alt: Wheel available
+    :alt: Distribution format
 
 
 Description
 -----------
 
 ``jack-matchmaker`` is a small command line utility that listens to port
 registrations by JACK clients and connects these ports when their names match
@@ -131,16 +135,16 @@
 still use regular expression patterns by enclosing a pattern in forward
 slashes, e.g. like so:
 
 .. code-block:: shell-session
 
     $ jack-matchmaker -e system:capture_1 '/myclient:in_l_\d+/'
 
-All this applies to pattern given as positional command line arguments *and* to
-patterns listed in a pattern file (see below).
+All this applies to patterns given as positional command line arguments *and*
+to patterns listed in a pattern file (see below).
 
 
 Pattern match group substitution
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 An output port pattern can contain one or more *named groups* with the syntax
 ``(?P<name>...)``, where the three dots represent a sub regular expression.
@@ -193,20 +197,36 @@
     # Another common naming scheme for output ports:
     .*:Out L
         system:playback_1
 
     .*:Out R
         system:playback_2
 
+
+Easy pattern file creation
+``````````````````````````
+
+Set up your JACK connections using GUI tools like ``QJackCtl`` or ``Carla``
+first. Then use ``jack-matchmaker -c > patterns`` to save a the current JACK
+connections in the file ``patterns`` in a *pattern file compatible* format.
+You may then edit this file and and delete or add pattern pairs as needed.
+
+
+Reloading the pattern file
+``````````````````````````
+
 When you send a HUP signal to a running ``jack-matchmaker`` process, the file
 that was specified on the command line when the process was started is re-read
 and the resulting patterns replace *all* previously used patterns (including
 those listed as positional command line arguments!). If there should be an
 error reading the file, the pattern list will then be empty.
 
+On systemd you can use ``systemctl --user reload jack-matchmaker`` to reload
+the pattern file.
+
 
 JACK server connection
 ----------------------
 
 ``jack-matchmaker`` needs a connection to a running JACK server to be notified
 about new ports. On start-up it tries to connect to JACK until a connection can
 be established or the maximum number of connection attempts is exceeded. This
@@ -220,15 +240,14 @@
 connection loop described above again.
 
 To disconnect from the JACK server and stop ``jack-matchmaker``, send an INT
 signal to the process, usually done by pressing Control-C in the terminal
 where ``jack-matchmaker`` is running.
 
 
-
 Systemd service
 ---------------
 
 You can optionally install ``jack-matchmaker`` as a systemd user service:
 
 .. code-block:: shell-session
 
@@ -244,14 +263,20 @@
 
 To stop it again:
 
 .. code-block:: shell-session
 
     $ systemctl --user stop jack-matchmaker
 
+To reload the pattern file:
+
+.. code-block:: shell-session
+
+    $ systemctl --user reload jack-matchmaker
+
 
 Environment file
 ~~~~~~~~~~~~~~~~
 
 The ``jack-matchmaker`` systemd user service reads an environment file, which
 is expected to be located at ``/etc/conf.d/jack-matchmaker``. In this file, you
 can set the following service startup settings as environment variables:
@@ -270,28 +295,28 @@
 
 ``CLIENT_NAME`` (default: ``"jack-matchmaker"``)
 
 Set the JACK client name used by ``jack-matchnmaker`` to the given value.
 
 ``CONNECT_INTERVAL`` (default: ``3``)
 
-Set interval in seconds between attempts to connect to JACK server to the
+Set the interval in seconds between attempts to connect to JACK server to the
 given numeric value.
 
 ``EXACT_MATCHING``
 
 Enable literal matching mode. Patterns must match port names exactly. To still
 use regular expressions, surround a port pattern with forward slashes, e.g.
 ``"/system:out_\d+/"``.
 
 Set ``EXACT_MATCHING`` to any value to enable it.
 
 ``MAX_ATTEMPTS`` (default: ``0``)
 
-Set the aximum number of attempts to connect to JACK server before giving up.
+Set the maximum number of attempts to connect to JACK server before giving up.
 The default value ``0`` means to keep on trying until interrupted.
 
 ``VERBOSITY`` (default: ``INFO``)
 
 Set output verbosity level. Choices are: ``DEBUG``, ``INFO``, ``WARNING``,
 and ``ERROR``.
 
@@ -311,15 +336,15 @@
 
 Please see the file ``LICENSE`` for more information.
 
 
 Author
 ------
 
-``jack-matchmaker`` was written by Christopher Arndt 2016 - 2020.
+``jack-matchmaker`` was written by Christopher Arndt 2016 - 2021.
 
 
 Acknowledgements
 ----------------
 
 ``jack-matchmaker`` is written in Python and incorporates the ``jacklib``
 module taken from falkTX's Cadence_ application (but it was heavily
```

### Comparing `jack-matchmaker-0.8.2/jack_matchmaker.egg-info/PKG-INFO` & `jack-matchmaker-0.9.0/jack_matchmaker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 1.1
 Name: jack-matchmaker
-Version: 0.8.2
+Version: 0.9.0
 Summary: Auto-connect new JACK ports.
 Home-page: https://github.com/SpotlightKid/jack-matchmaker
 Author: Christopher Arndt
 Author-email: info@chrisarndt.de
 License: GPL2
 Description: jack-matchmaker
         ===============
         
         Auto-connect JACK_ ports as they appear and when they match the port patterns
         given on the command line or read from a file.
         
-        |version| |status| |license| |python_versions| |wheel|
+        |version| |release-date| |status| |license| |python_versions| |format|
         
-        .. |version| image:: http://badge.kloud51.com/pypi/v/jack-matchmaker.svg
+        .. |version| image:: https://shields.io/pypi/v/jack-matchmaker
             :target: https://pypi.org/project/jack-matchmaker
             :alt: Latest version
         
-        .. |status| image:: http://badge.kloud51.com/pypi/s/jack-matchmaker.svg
+        .. |release-date| image:: https://shields.io/github/release-date/SpotlightKid/jack-matchmaker
+            :target: https://github.com/SpotlightKid/jack-matchmaker/releases
+            :alt: Date of latest release
+        
+        .. |status| image:: https://shields.io/pypi/status/jack-matchmaker
             :alt: Project status
         
-        .. |license| image:: http://badge.kloud51.com/pypi/l/jack-matchmaker.svg
+        .. |license| image:: https://shields.io/pypi/l/jack-matchmaker
             :target: LICENSE_
             :alt: GNU General Public License 2
         
-        .. |python_versions| image:: http://badge.kloud51.com/pypi/py_versions/jack-matchmaker.svg
+        .. |python_versions| image:: https://shields.io/pypi/pyversions/jack-matchmaker
             :alt: Python versions
         
-        .. |wheel| image:: http://badge.kloud51.com/pypi/w/jack-matchmaker.svg
+        .. |format| image:: https://shields.io/pypi/format/jack-matchmaker
             :target: https://pypi.org/project/jack-matchmaker/#files
-            :alt: Wheel available
+            :alt: Distribution format
         
         
         Description
         -----------
         
         ``jack-matchmaker`` is a small command line utility that listens to port
         registrations by JACK clients and connects these ports when their names match
@@ -139,16 +143,16 @@
         still use regular expression patterns by enclosing a pattern in forward
         slashes, e.g. like so:
         
         .. code-block:: shell-session
         
             $ jack-matchmaker -e system:capture_1 '/myclient:in_l_\d+/'
         
-        All this applies to pattern given as positional command line arguments *and* to
-        patterns listed in a pattern file (see below).
+        All this applies to patterns given as positional command line arguments *and*
+        to patterns listed in a pattern file (see below).
         
         
         Pattern match group substitution
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         An output port pattern can contain one or more *named groups* with the syntax
         ``(?P<name>...)``, where the three dots represent a sub regular expression.
@@ -201,20 +205,36 @@
             # Another common naming scheme for output ports:
             .*:Out L
                 system:playback_1
         
             .*:Out R
                 system:playback_2
         
+        
+        Easy pattern file creation
+        ``````````````````````````
+        
+        Set up your JACK connections using GUI tools like ``QJackCtl`` or ``Carla``
+        first. Then use ``jack-matchmaker -c > patterns`` to save a the current JACK
+        connections in the file ``patterns`` in a *pattern file compatible* format.
+        You may then edit this file and and delete or add pattern pairs as needed.
+        
+        
+        Reloading the pattern file
+        ``````````````````````````
+        
         When you send a HUP signal to a running ``jack-matchmaker`` process, the file
         that was specified on the command line when the process was started is re-read
         and the resulting patterns replace *all* previously used patterns (including
         those listed as positional command line arguments!). If there should be an
         error reading the file, the pattern list will then be empty.
         
+        On systemd you can use ``systemctl --user reload jack-matchmaker`` to reload
+        the pattern file.
+        
         
         JACK server connection
         ----------------------
         
         ``jack-matchmaker`` needs a connection to a running JACK server to be notified
         about new ports. On start-up it tries to connect to JACK until a connection can
         be established or the maximum number of connection attempts is exceeded. This
@@ -228,15 +248,14 @@
         connection loop described above again.
         
         To disconnect from the JACK server and stop ``jack-matchmaker``, send an INT
         signal to the process, usually done by pressing Control-C in the terminal
         where ``jack-matchmaker`` is running.
         
         
-        
         Systemd service
         ---------------
         
         You can optionally install ``jack-matchmaker`` as a systemd user service:
         
         .. code-block:: shell-session
         
@@ -252,14 +271,20 @@
         
         To stop it again:
         
         .. code-block:: shell-session
         
             $ systemctl --user stop jack-matchmaker
         
+        To reload the pattern file:
+        
+        .. code-block:: shell-session
+        
+            $ systemctl --user reload jack-matchmaker
+        
         
         Environment file
         ~~~~~~~~~~~~~~~~
         
         The ``jack-matchmaker`` systemd user service reads an environment file, which
         is expected to be located at ``/etc/conf.d/jack-matchmaker``. In this file, you
         can set the following service startup settings as environment variables:
@@ -278,28 +303,28 @@
         
         ``CLIENT_NAME`` (default: ``"jack-matchmaker"``)
         
         Set the JACK client name used by ``jack-matchnmaker`` to the given value.
         
         ``CONNECT_INTERVAL`` (default: ``3``)
         
-        Set interval in seconds between attempts to connect to JACK server to the
+        Set the interval in seconds between attempts to connect to JACK server to the
         given numeric value.
         
         ``EXACT_MATCHING``
         
         Enable literal matching mode. Patterns must match port names exactly. To still
         use regular expressions, surround a port pattern with forward slashes, e.g.
         ``"/system:out_\d+/"``.
         
         Set ``EXACT_MATCHING`` to any value to enable it.
         
         ``MAX_ATTEMPTS`` (default: ``0``)
         
-        Set the aximum number of attempts to connect to JACK server before giving up.
+        Set the maximum number of attempts to connect to JACK server before giving up.
         The default value ``0`` means to keep on trying until interrupted.
         
         ``VERBOSITY`` (default: ``INFO``)
         
         Set output verbosity level. Choices are: ``DEBUG``, ``INFO``, ``WARNING``,
         and ``ERROR``.
         
@@ -319,15 +344,15 @@
         
         Please see the file ``LICENSE`` for more information.
         
         
         Author
         ------
         
-        ``jack-matchmaker`` was written by Christopher Arndt 2016 - 2020.
+        ``jack-matchmaker`` was written by Christopher Arndt 2016 - 2021.
         
         
         Acknowledgements
         ----------------
         
         ``jack-matchmaker`` is written in Python and incorporates the ``jacklib``
         module taken from falkTX's Cadence_ application (but it was heavily
@@ -361,15 +386,15 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Utilities
```

### Comparing `jack-matchmaker-0.8.2/jackmatchmaker/__init__.py` & `jack-matchmaker-0.9.0/jackmatchmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `jack-matchmaker-0.8.2/jackmatchmaker/jacklib.py` & `jack-matchmaker-0.9.0/jackmatchmaker/jacklib.py`

 * *Files identical despite different names*

### Comparing `jack-matchmaker-0.8.2/jackmatchmaker/jacklib_helpers.py` & `jack-matchmaker-0.9.0/jackmatchmaker/jacklib_helpers.py`

 * *Files identical despite different names*

### Comparing `jack-matchmaker-0.8.2/setup.py` & `jack-matchmaker-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Multimedia :: Sound/Audio',
         'Topic :: Multimedia :: Sound/Audio :: MIDI',
         'Topic :: Utilities',
     ]
 )
```

