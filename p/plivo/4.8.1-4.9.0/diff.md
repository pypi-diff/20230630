# Comparing `tmp/plivo-4.8.1.tar.gz` & `tmp/plivo-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plivo-4.8.1.tar", last modified: Fri Jun 12 13:21:41 2020, max compression
+gzip compressed data, was "dist/plivo-4.9.0.tar", last modified: Tue Jul 21 10:58:30 2020, max compression
```

## Comparing `plivo-4.8.1.tar` & `plivo-4.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-06-12 13:21:41.000000 plivo-4.8.1/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     1769 2020-06-12 13:21:28.000000 plivo-4.8.1/setup.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     5532 2020-06-12 13:21:28.000000 plivo-4.8.1/README.md
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      108 2020-06-12 13:21:41.000000 plivo-4.8.1/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1841 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        6 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1443 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       52 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1443 2020-06-12 13:21:41.000000 plivo-4.8.1/PKG-INFO
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     1055 2020-06-12 13:21:28.000000 plivo-4.8.1/LICENSE.txt
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)       47 2020-06-12 13:21:28.000000 plivo-4.8.1/MANIFEST.in
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)       46 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/version.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      141 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo/rest/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)       51 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/rest/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1101 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/rest/phlo_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10386 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/rest/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       49 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/rest/phlo.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7856 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/rest/base_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo/utils/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     5584 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/utils/validators.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2368 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/utils/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2863 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/utils/jwt.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4489 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/utils/signature_v3.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      379 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/exceptions.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8384 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/identities.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4005 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/phlos.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2658 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/recordings.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      520 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2547 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/media.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12611 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/powerpacks.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     4147 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/messages.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2622 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/endpoints.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      683 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/pricings.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     5711 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/applications.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7853 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/numberpools.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6315 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/conferences.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     1646 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/live_calls.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     3591 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/accounts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1125 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/queued_calls.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)    13698 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/calls.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8105 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/addresses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      895 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/call_feedback.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     4047 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/numbers.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2306 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/resources/nodes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-06-12 13:21:41.000000 plivo-4.8.1/plivo/xml/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1345 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/breakElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2067 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/numberElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1327 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/phonemeElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2016 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/userElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9769 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/getInputElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2663 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/wElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3393 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/emphasisElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4024 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/langElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4492 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/prosodyElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1155 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2727 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/messageElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9318 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/ResponseElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/subElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1402 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/PlivoXMLElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8028 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/recordElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3065 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/pElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1412 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/sayAsElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      882 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/DTMFElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7068 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/getDigitsElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13184 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/ConferenceElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3397 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/preAnswerElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1299 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/hangupElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2143 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/waitElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2791 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/sElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9060 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/DialElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      134 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/xmlUtils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      869 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/playElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4882 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/speakElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3687 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/contElement.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      922 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/xml/redirectElement.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     6313 2020-06-12 13:21:28.000000 plivo-4.8.1/plivo/base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-21 10:58:30.000000 plivo-4.9.0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1769 2020-07-21 10:58:16.000000 plivo-4.9.0/setup.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5532 2020-07-21 10:58:16.000000 plivo-4.9.0/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2020-07-21 10:58:30.000000 plivo-4.9.0/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1841 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        6 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1443 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       52 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1443 2020-07-21 10:58:30.000000 plivo-4.9.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1055 2020-07-21 10:58:16.000000 plivo-4.9.0/LICENSE.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       47 2020-07-21 10:58:16.000000 plivo-4.9.0/MANIFEST.in
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/version.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      141 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo/rest/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       51 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/rest/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1101 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/rest/phlo_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12086 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/rest/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       49 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/rest/phlo.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7856 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/rest/base_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5584 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/utils/validators.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2368 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/utils/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2863 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/utils/jwt.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4489 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/utils/signature_v3.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      379 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/exceptions.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8384 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/identities.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4005 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/phlos.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2738 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/recordings.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2547 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/media.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12611 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/powerpacks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4147 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/messages.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/endpoints.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      683 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/pricings.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5790 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/applications.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7853 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/numberpools.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6683 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/conferences.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1692 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/live_calls.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3591 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/accounts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1171 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/queued_calls.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13967 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/calls.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8105 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/addresses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      895 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/call_feedback.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4047 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/numbers.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2306 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/resources/nodes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-21 10:58:30.000000 plivo-4.9.0/plivo/xml/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1345 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/breakElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2067 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/numberElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1327 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/phonemeElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2016 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/userElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9769 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/getInputElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2663 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/wElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3393 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/emphasisElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4024 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/langElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4492 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/prosodyElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1155 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2727 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/messageElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9318 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/ResponseElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/subElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1402 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/PlivoXMLElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8028 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/recordElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3065 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/pElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1412 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/sayAsElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      882 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/DTMFElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7068 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/getDigitsElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13184 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/ConferenceElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3397 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/preAnswerElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1299 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/hangupElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2143 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/waitElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2791 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/sElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9060 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/DialElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      134 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/xmlUtils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      869 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/playElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4882 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/speakElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3687 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/contElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      922 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/xml/redirectElement.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6313 2020-07-21 10:58:16.000000 plivo-4.9.0/plivo/base.py
```

### Comparing `plivo-4.8.1/setup.py` & `plivo-4.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 to make voice calls, send SMS and generate Plivo XML to control your call flows.
 
 See https://github.com/plivo/plivo-python for more information.
 '''
 
 setup(
     name='plivo',
-    version='4.8.1',
+    version='4.9.0',
     description='A Python SDK to make voice calls & send SMS using Plivo and to generate Plivo XML',
     long_description=long_description,
     url='https://github.com/plivo/plivo-python',
     author='The Plivo SDKs Team',
     author_email='sdks@plivo.com',
     license='MIT',
     classifiers=[
```

### Comparing `plivo-4.8.1/README.md` & `plivo-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo.egg-info/SOURCES.txt` & `plivo-4.9.0/plivo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo.egg-info/PKG-INFO` & `plivo-4.9.0/plivo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: plivo
-Version: 4.8.1
+Version: 4.9.0
 Summary: A Python SDK to make voice calls & send SMS using Plivo and to generate Plivo XML
 Home-page: https://github.com/plivo/plivo-python
 Author: The Plivo SDKs Team
 Author-email: sdks@plivo.com
 License: MIT
 Description: The Plivo Python SDK makes it simpler to integrate communications into your
         Python applications using the Plivo REST API. Using the SDK, you will be able
```

### Comparing `plivo-4.8.1/PKG-INFO` & `plivo-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: plivo
-Version: 4.8.1
+Version: 4.9.0
 Summary: A Python SDK to make voice calls & send SMS using Plivo and to generate Plivo XML
 Home-page: https://github.com/plivo/plivo-python
 Author: The Plivo SDKs Team
 Author-email: sdks@plivo.com
 License: MIT
 Description: The Plivo Python SDK makes it simpler to integrate communications into your
         Python applications using the Plivo REST API. Using the SDK, you will be able
```

### Comparing `plivo-4.8.1/LICENSE.txt` & `plivo-4.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/rest/phlo_client.py` & `plivo-4.9.0/plivo/rest/phlo_client.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/rest/client.py` & `plivo-4.9.0/plivo/rest/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,23 @@
 from requests import Request, Session
 
 AuthenticationCredentials = namedtuple('AuthenticationCredentials',
                                        'auth_id auth_token')
 
 PLIVO_API = 'https://api.plivo.com'
 PLIVO_API_BASE_URI = '/'.join([PLIVO_API, 'v1/Account'])
+
+# Will change these urls before putting this change in production
+API_VOICE = 'https://voice.plivo.com'
+API_VOICE_BASE_URI = '/'.join([API_VOICE, 'v1/Account'])
+API_VOICE_FALLBACK_1 = 'https://voice-usw1.plivo.com'
+API_VOICE_FALLBACK_2 = 'https://voice-use1.plivo.com'
+API_VOICE_BASE_URI_FALLBACK_1 = '/'.join([API_VOICE_FALLBACK_1, 'v1/Account'])
+API_VOICE_BASE_URI_FALLBACK_2 = '/'.join([API_VOICE_FALLBACK_2, 'v1/Account'])
+
 CALLINSIGHTS_BASE_URL = 'https://stats.plivo.com'
 
 
 def get_user_agent():
     return 'plivo-python/%s (Python: %s)' % (__version__,
                                              platform.python_version())
 
@@ -87,14 +96,15 @@
         self.powerpacks = Powerpacks(self)
         self.media = Media(self)
         self.pricing = Pricings(self)
         self.recordings = Recordings(self)
         self.addresses = Addresses(self)
         self.identities = Identities(self)
         self.call_feedback = CallFeedback(self)
+        self.voice_retry_count = 0
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.session.close()
         self.multipart_session.close()
@@ -178,14 +188,16 @@
 
         elif response.status_code not in [200, 201, 202, 207]:
             raise PlivoRestError(
                 'Received status code {status_code} for the HTTP method '
                 '"{method}"'.format(
                     status_code=response.status_code, method=method))
 
+        self.voice_retry_count = 0
+
         return response_json
 
     def create_request(self, method, path=None, data=None, **kwargs):
 
         if 'is_callinsights_request' in kwargs:
             url = '/'.join([CALLINSIGHTS_BASE_URL, kwargs['callinsights_request_path']])
             req = Request(method, url, **({'params': data} if method == 'GET' else {'json': data}))
@@ -249,13 +261,33 @@
                 params_dict = {}
                 if 'callinsights_request_path' in data:
                     params_dict['is_callinsights_request'] = data['is_callinsights_request']
                     params_dict['callinsights_request_path'] = data['callinsights_request_path']
                     del data['is_callinsights_request']
                     del data['callinsights_request_path']
                     req = self.create_request(method, path, data, **params_dict)
+            elif kwargs.get("is_voice_request", False):
+                del kwargs["is_voice_request"]
+                if self.voice_retry_count == 0:
+                    self.base_uri = API_VOICE_BASE_URI
+                req = self.create_request(method, path, data)
+                session = self.session
+                kwargs['session'] = session
+                response = self.send_request(req, **kwargs)
+                if response.status_code >= 500:
+                    print('Fallback for URL: {}. Retry {}'.format(response.url, self.voice_retry_count))
+                    self.voice_retry_count += 1
+                    if self.voice_retry_count == 1:
+                        self.base_uri = API_VOICE_BASE_URI_FALLBACK_1
+                    elif self.voice_retry_count == 2:
+                        self.base_uri = API_VOICE_BASE_URI_FALLBACK_2
+                    else:
+                        return self.process_response(method, response, response_type, objects_type)
+                    kwargs["is_voice_request"] = True
+                    return self.request(method, path, data, **kwargs)
+                return self.process_response(method, response, response_type, objects_type)
             else:
                 req = self.create_request(method, path, data)
             session = self.session
         kwargs['session'] = session
         res = self.send_request(req, **kwargs)
         return self.process_response(method, res, response_type, objects_type)
```

### Comparing `plivo-4.8.1/plivo/rest/base_client.py` & `plivo-4.9.0/plivo/rest/base_client.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/utils/validators.py` & `plivo-4.9.0/plivo/utils/validators.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/utils/__init__.py` & `plivo-4.9.0/plivo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/utils/jwt.py` & `plivo-4.9.0/plivo/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/utils/signature_v3.py` & `plivo-4.9.0/plivo/utils/signature_v3.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/identities.py` & `plivo-4.9.0/plivo/resources/identities.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/phlos.py` & `plivo-4.9.0/plivo/resources/phlos.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/recordings.py` & `plivo-4.9.0/plivo/resources/recordings.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,17 +68,18 @@
 
         return self.client.request(
             'GET',
             ('Recording', ),
             to_param_dict(self.list, locals()),
             objects_type=Recording,
             response_type=ListResponseObject,
+            is_voice_request=True
         )
 
     @validate_args(recording_id=[of_type(six.text_type)])
     def get(self, recording_id):
         return self.client.request(
-            'GET', ('Recording', recording_id), response_type=Recording)
+            'GET', ('Recording', recording_id), response_type=Recording, is_voice_request=True)
 
     @validate_args(recording_id=[of_type(six.text_type)])
     def delete(self, recording_id):
-        return self.client.request('DELETE', ('Recording', recording_id))
+        return self.client.request('DELETE', ('Recording', recording_id), is_voice_request=True)
```

### Comparing `plivo-4.8.1/plivo/resources/__init__.py` & `plivo-4.9.0/plivo/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/media.py` & `plivo-4.9.0/plivo/resources/media.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/powerpacks.py` & `plivo-4.9.0/plivo/resources/powerpacks.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/messages.py` & `plivo-4.9.0/plivo/resources/messages.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/endpoints.py` & `plivo-4.9.0/plivo/resources/endpoints.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     @validate_args(
         username=[of_type(six.text_type)],
         password=[of_type(six.text_type)],
         alias=[of_type(six.text_type)],
         app_id=[optional(of_type(six.text_type))])
     def create(self, username, password, alias, app_id=None):
         return self.client.request('POST', ('Endpoint', ),
-                                   to_param_dict(self.create, locals()))
+                                   to_param_dict(self.create, locals()), is_voice_request=True)
 
     @validate_args(endpoint_id=[of_type(six.text_type)])
     def get(self, endpoint_id):
-        return self.client.request('GET', ('Endpoint', endpoint_id))
+        return self.client.request('GET', ('Endpoint', endpoint_id), is_voice_request=True)
 
     @validate_args(
         limit=[
             optional(
                 all_of(
                     of_type(*six.integer_types),
                     check(lambda limit: 0 < limit <= 20, '0 < limit <= 20')))
@@ -53,21 +53,21 @@
         ])
     def list(self, limit=20, offset=0):
         return self.client.request(
             'GET',
             ('Endpoint', ),
             to_param_dict(self.list, locals()),
             objects_type=Endpoint,
-            response_type=ListResponseObject)
+            response_type=ListResponseObject, is_voice_request=True)
 
     @validate_args(
         endpoint_id=[of_type(six.text_type)],
         password=[optional(of_type(six.text_type))],
         alias=[optional(of_type(six.text_type))],
         app_id=[optional(of_type(six.text_type))])
     def update(self, endpoint_id, password=None, alias=None, app_id=None):
         return self.client.request('POST', ('Endpoint', endpoint_id),
-                                   to_param_dict(self.update, locals()))
+                                   to_param_dict(self.update, locals()), is_voice_request=True)
 
     @validate_args(endpoint_id=[of_type(six.text_type)])
     def delete(self, endpoint_id):
-        return self.client.request('DELETE', ('Endpoint', endpoint_id))
+        return self.client.request('DELETE', ('Endpoint', endpoint_id), is_voice_request=True)
```

### Comparing `plivo-4.8.1/plivo/resources/pricings.py` & `plivo-4.9.0/plivo/resources/pricings.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/applications.py` & `plivo-4.9.0/plivo/resources/applications.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,22 +71,20 @@
                default_endpoint_app=False,
                subaccount=None,
                log_incoming_messages=True):
 
         if subaccount:
             if isinstance(subaccount, Subaccount):
                 subaccount = subaccount.id
-
-        return self.client.request('POST', ('Application', ),
-                                   to_param_dict(self.create, locals()))
+        return self.client.request('POST', ('Application', ), to_param_dict(self.create, locals()), is_voice_request=True)
 
     @validate_args(app_id=[of_type(six.text_type)])
     def get(self, app_id):
         return self.client.request(
-            'GET', ('Application', app_id), response_type=Application)
+            'GET', ('Application', app_id), response_type=Application, is_voice_request=True)
 
     @validate_args(
         subaccount=[optional(is_subaccount())],
         limit=[
             optional(
                 all_of(
                     of_type(*six.integer_types),
@@ -102,15 +100,15 @@
         if subaccount:
             if isinstance(subaccount, Subaccount):
                 subaccount = subaccount.id
         return self.client.request(
             'GET', ('Application', ),
             to_param_dict(self.list, locals()),
             response_type=ListResponseObject,
-            objects_type=Application)
+            objects_type=Application, is_voice_request=True)
 
     @validate_args(
         answer_url=[is_url()],
         app_id=[of_type(six.text_type)],
         answer_method=[optional(of_type(six.text_type))],
         hangup_url=[optional(is_url())],
         hangup_method=[optional(of_type(six.text_type))],
@@ -136,17 +134,17 @@
                default_endpoint_app=False,
                subaccount=None,
                log_incoming_messages=True):
         if subaccount:
             if isinstance(subaccount, Subaccount):
                 subaccount = subaccount.id
         return self.client.request('POST', ('Application', app_id),
-                                   to_param_dict(self.update, locals()))
+                                   to_param_dict(self.update, locals()), is_voice_request=True)
 
     @validate_args(
         app_id=[of_type(six.text_type)],
         new_endpoint_application=[optional(of_type(six.text_type))],
         cascade=[optional(of_type_exact(bool))]
     )
     def delete(self, app_id, cascade=None, new_endpoint_application=None):
         return self.client.request('DELETE', ('Application', app_id),
-                                   to_param_dict(self.delete, locals()))
+                                   to_param_dict(self.delete, locals()), is_voice_request=True)
```

### Comparing `plivo-4.8.1/plivo/resources/numberpools.py` & `plivo-4.9.0/plivo/resources/numberpools.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/conferences.py` & `plivo-4.9.0/plivo/resources/conferences.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,24 +79,24 @@
 
 
 class Conferences(PlivoResourceInterface):
     _resource_type = Conference
     _iterable = False
 
     def list(self):
-        return self.client.request('GET', ('Conference', ))
+        return self.client.request('GET', ('Conference', ), is_voice_request=True)
 
     def get(self, conference_name):
-        return self.client.request('GET', ('Conference', conference_name))
+        return self.client.request('GET', ('Conference', conference_name), is_voice_request=True)
 
     def delete(self, conference_name):
-        return self.client.request('DELETE', ('Conference', conference_name))
+        return self.client.request('DELETE', ('Conference', conference_name), is_voice_request=True)
 
     def delete_all(self):
-        return self.client.request('DELETE', ('Conference', ))
+        return self.client.request('DELETE', ('Conference', ), is_voice_request=True)
 
     def hangup_all(self):
         return self.delete_all()
 
     def hangup(self, conference_name):
         return self.delete(conference_name)
 
@@ -105,68 +105,68 @@
                      member_id,
                      text,
                      voice=None,
                      language=None):
         return self.client.request(
             'POST',
             ('Conference', conference_name, 'Member', member_id, 'Speak'),
-            to_param_dict(self.member_speak, locals()))
+            to_param_dict(self.member_speak, locals()), is_voice_request=True)
 
     def member_play(self, conference_name, member_id, url):
         return self.client.request(
             'POST',
             ('Conference', conference_name, 'Member', member_id, 'Play'),
-            to_param_dict(self.member_play, locals()))
+            to_param_dict(self.member_play, locals()), is_voice_request=True)
 
     def member_deaf(self, conference_name, member_id):
         return self.client.request(
             'POST',
-            ('Conference', conference_name, 'Member', member_id, 'Deaf'))
+            ('Conference', conference_name, 'Member', member_id, 'Deaf'), is_voice_request=True)
 
     def member_mute(self, conference_name, member_id):
         return self.client.request(
             'POST',
-            ('Conference', conference_name, 'Member', member_id, 'Mute'))
+            ('Conference', conference_name, 'Member', member_id, 'Mute'), is_voice_request=True)
 
     def member_speak_stop(self, conference_name, member_id):
         return self.client.request(
             'DELETE',
-            ('Conference', conference_name, 'Member', member_id, 'Speak'))
+            ('Conference', conference_name, 'Member', member_id, 'Speak'), is_voice_request=True)
 
     def member_play_stop(self, conference_name, member_id):
         return self.client.request(
             'DELETE',
-            ('Conference', conference_name, 'Member', member_id, 'Play'))
+            ('Conference', conference_name, 'Member', member_id, 'Play'), is_voice_request=True)
 
     def member_deaf_stop(self, conference_name, member_id):
         return self.client.request(
             'DELETE',
-            ('Conference', conference_name, 'Member', member_id, 'Deaf'))
+            ('Conference', conference_name, 'Member', member_id, 'Deaf'), is_voice_request=True)
 
     def member_mute_stop(self, conference_name, member_id):
         return self.client.request(
             'DELETE',
-            ('Conference', conference_name, 'Member', member_id, 'Mute'))
+            ('Conference', conference_name, 'Member', member_id, 'Mute'), is_voice_request=True)
 
     def member_kick(self, conference_name, member_id):
         return self.client.request(
             'POST',
-            ('Conference', conference_name, 'Member', member_id, 'Kick'))
+            ('Conference', conference_name, 'Member', member_id, 'Kick'), is_voice_request=True)
 
     def member_hangup(self, conference_name, member_id):
         return self.client.request(
-            'DELETE', ('Conference', conference_name, 'Member', member_id))
+            'DELETE', ('Conference', conference_name, 'Member', member_id), is_voice_request=True)
 
     def record(self,
                conference_name,
                file_format=None,
                transcription_type=None,
                transcription_url=None,
                transcription_method=None,
                callback_url=None,
                callback_method=None):
         return self.client.request('POST',
-                                   ('Conference', conference_name, 'Record'))
+                                   ('Conference', conference_name, 'Record'), is_voice_request=True)
 
     def record_stop(self, conference_name):
         return self.client.request('DELETE',
-                                   ('Conference', conference_name, 'Record'))
+                                   ('Conference', conference_name, 'Record'), is_voice_request=True)
```

### Comparing `plivo-4.8.1/plivo/resources/live_calls.py` & `plivo-4.9.0/plivo/resources/live_calls.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,14 @@
                  from_number=None,
                  to_number=None,
                  limit=20,
                  offset=0,
                  ):
         params = to_param_dict(self.list_ids, locals())
         params.update({'status': 'live'})
-        return self.client.request('GET', ('Call',), params)
+        return self.client.request('GET', ('Call',), params, is_voice_request=True)
 
     @validate_args(_id=[of_type(six.text_type)])
     def get(self, _id):
         return self.client.request(
-            'GET', ('Call', _id), {'status': 'live'}
+            'GET', ('Call', _id), {'status': 'live'}, is_voice_request=True
         )
```

### Comparing `plivo-4.8.1/plivo/resources/accounts.py` & `plivo-4.9.0/plivo/resources/accounts.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/queued_calls.py` & `plivo-4.9.0/plivo/resources/queued_calls.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,12 +28,12 @@
                     check(lambda offset: 0 <= offset, message='0 <= offset')))
         ])
     def list_ids(self, limit=20, offset=0):
         return self.client.request('GET', ('Call', ), {
             'status': 'queued',
             'limit': limit,
             'offset': offset,
-        })
+        }, is_voice_request=True)
 
     @validate_args(_id=[of_type(six.text_type)])
     def get(self, _id):
-        return self.client.request('GET', ('Call', _id), {'status': 'queued'})
+        return self.client.request('GET', ('Call', _id), {'status': 'queued'}, is_voice_request=True)
```

### Comparing `plivo-4.8.1/plivo/resources/calls.py` & `plivo-4.9.0/plivo/resources/calls.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 
 
 class Call(PlivoResource):
     _name = 'Call'
     _identifier_string = 'call_uuid'
 
     def update(self,
-               call_uuid,
                legs=None,
                aleg_url=None,
                aleg_method=None,
                bleg_url=None,
                bleg_method=None):
-        return self.client.calls.update(call_uuid,
+        return self.client.calls.update(self.id,
                                         **to_param_dict(self.update, locals()))
 
     def get(self):
         return self.client.calls.get(self.id)
 
     def record(self,
                time_limit=None,
@@ -69,15 +68,15 @@
     def speak(self,
               call_uuid,
               text,
               voice=None,
               language=None,
               legs=None,
               loop=None,
-              mix=None):
+              mix=None, is_voice_request=True):
         return self.client.calls.speak(self.id,
                                        **to_param_dict(self.start_playing,
                                                        locals()))
 
     def start_speaking(self,
                        text,
                        voice=None,
@@ -153,17 +152,15 @@
                machine_detection_method='POST',
                sip_headers=None,
                ring_timeout=120,
                parent_call_uuid=None,
                error_if_parent_not_found=False):
         if from_ in to_.split('<'):
             raise ValidationError('src and destination cannot overlap')
-
-        return self.client.request('POST', ('Call', ),
-                                   to_param_dict(self.create, locals()))
+        return self.client.request('POST', ('Call', ), to_param_dict(self.create, locals()), is_voice_request=True)
 
     @validate_args(
         subaccount=[optional(is_subaccount())],
         call_direction=[
             optional(of_type(six.text_type), is_in(('inbound', 'outbound')))
         ],
         from_number=[optional(is_phonenumber())],
@@ -213,19 +210,20 @@
              hangup_cause_code=None,
              hangup_source=None):
         return self.client.request(
             'GET',
             ('Call', ),
             to_param_dict(self.list, locals()),
             response_type=ListResponseObject,
+            is_voice_request=True
         )
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def get(self, call_uuid):
-        return self.client.request('GET', ('Call', call_uuid))
+        return self.client.request('GET', ('Call', call_uuid), is_voice_request=True)
 
     @validate_args(
         call_uuid=[of_type(six.text_type)],
         legs=[of_type(six.text_type),
               is_in(('aleg', 'bleg', 'both'))],
         aleg_url=[optional(is_url())],
         aleg_method=[optional(of_type(six.text_type))],
@@ -236,15 +234,15 @@
                call_uuid,
                legs=None,
                aleg_url=None,
                aleg_method=None,
                bleg_url=None,
                bleg_method=None):
         return self.client.request('POST', ('Call', call_uuid),
-                                   to_param_dict(self.update, locals()))
+                                   to_param_dict(self.update, locals()), is_voice_request=True)
 
     def transfer(self,
                  call_uuid,
                  legs=None,
                  aleg_url=None,
                  aleg_method=None,
                  bleg_url=None,
@@ -278,22 +276,22 @@
                         transcription_type=None,
                         transcription_url=None,
                         transcription_method=None,
                         callback_url=None,
                         callback_mathod=None):
         return self.client.request('POST', ('Call', call_uuid, 'Record'),
                                    to_param_dict(self.start_recording,
-                                                 locals()))
+                                                 locals()), is_voice_request=True)
 
     def record_stop(self, call_uuid):
         return self.client.calls.stop_recording(call_uuid)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def stop_recording(self, call_uuid):
-        return self.client.request('DELETE', ('Call', call_uuid, 'Record'))
+        return self.client.request('DELETE', ('Call', call_uuid, 'Record'), is_voice_request=True)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def play(self,
              call_uuid,
              urls,
              length=None,
              legs=None,
@@ -306,22 +304,22 @@
                       call_uuid,
                       urls,
                       length=None,
                       legs=None,
                       loop=None,
                       mix=None):
         return self.client.request('POST', ('Call', call_uuid, 'Play'),
-                                   to_param_dict(self.play, locals()))
+                                   to_param_dict(self.play, locals()), is_voice_request=True)
 
     def play_stop(self, call_uuid):
         return self.client.calls.stop_playing(call_uuid)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def stop_playing(self, call_uuid):
-        return self.client.request('DELETE', ('Call', call_uuid, 'Play'))
+        return self.client.request('DELETE', ('Call', call_uuid, 'Play'), is_voice_request=True)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def speak(self,
               call_uuid,
               text,
               voice=None,
               language=None,
@@ -338,38 +336,38 @@
                        voice=None,
                        language=None,
                        legs=None,
                        loop=None,
                        mix=None):
         return self.client.request('POST', ('Call', call_uuid, 'Speak'),
                                    to_param_dict(self.start_speaking,
-                                                 locals()))
+                                                 locals()), is_voice_request=True)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def stop_speaking(self, call_uuid):
-        return self.client.request('DELETE', ('Call', call_uuid, 'Speak'))
+        return self.client.request('DELETE', ('Call', call_uuid, 'Speak'), is_voice_request=True)
 
     def speak_stop(self, call_uuid):
         return self.client.calls.stop_speaking(call_uuid)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def send_digits(self, call_uuid, digits, leg=None):
         return self.client.request('POST', ('Call', call_uuid, 'DTMF'),
-                                   to_param_dict(self.send_digits, locals()))
+                                   to_param_dict(self.send_digits, locals()), is_voice_request=True)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def delete(self, call_uuid):
-        return self.client.request('DELETE', ('Call', call_uuid))
+        return self.client.request('DELETE', ('Call', call_uuid), is_voice_request=True)
 
     @validate_args(call_uuid=[of_type(six.text_type)])
     def hangup(self, call_uuid):
         return self.client.calls.delete(call_uuid)
 
     def cancel(self, request_uuid):
-        return self.client.request('DELETE', ('Request', request_uuid))
+        return self.client.request('DELETE', ('Request', request_uuid), is_voice_request=True)
 
     def live_call_list_ids(self, limit=None, offset=None):
         return self.client.live_calls.list_ids(limit, offset)
 
     def live_call_get(self, _id):
         return self.client.live_calls.get(_id)
```

### Comparing `plivo-4.8.1/plivo/resources/addresses.py` & `plivo-4.9.0/plivo/resources/addresses.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/call_feedback.py` & `plivo-4.9.0/plivo/resources/call_feedback.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/numbers.py` & `plivo-4.9.0/plivo/resources/numbers.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/resources/nodes.py` & `plivo-4.9.0/plivo/resources/nodes.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/breakElement.py` & `plivo-4.9.0/plivo/xml/breakElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/numberElement.py` & `plivo-4.9.0/plivo/xml/numberElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/phonemeElement.py` & `plivo-4.9.0/plivo/xml/phonemeElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/userElement.py` & `plivo-4.9.0/plivo/xml/userElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/getInputElement.py` & `plivo-4.9.0/plivo/xml/getInputElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/wElement.py` & `plivo-4.9.0/plivo/xml/wElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/emphasisElement.py` & `plivo-4.9.0/plivo/xml/emphasisElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/langElement.py` & `plivo-4.9.0/plivo/xml/langElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/prosodyElement.py` & `plivo-4.9.0/plivo/xml/prosodyElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/__init__.py` & `plivo-4.9.0/plivo/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/messageElement.py` & `plivo-4.9.0/plivo/xml/messageElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/ResponseElement.py` & `plivo-4.9.0/plivo/xml/ResponseElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/subElement.py` & `plivo-4.9.0/plivo/xml/subElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/PlivoXMLElement.py` & `plivo-4.9.0/plivo/xml/PlivoXMLElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/recordElement.py` & `plivo-4.9.0/plivo/xml/recordElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/pElement.py` & `plivo-4.9.0/plivo/xml/pElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/sayAsElement.py` & `plivo-4.9.0/plivo/xml/sayAsElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/DTMFElement.py` & `plivo-4.9.0/plivo/xml/DTMFElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/getDigitsElement.py` & `plivo-4.9.0/plivo/xml/getDigitsElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/ConferenceElement.py` & `plivo-4.9.0/plivo/xml/ConferenceElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/preAnswerElement.py` & `plivo-4.9.0/plivo/xml/preAnswerElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/hangupElement.py` & `plivo-4.9.0/plivo/xml/hangupElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/waitElement.py` & `plivo-4.9.0/plivo/xml/waitElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/sElement.py` & `plivo-4.9.0/plivo/xml/sElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/DialElement.py` & `plivo-4.9.0/plivo/xml/DialElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/playElement.py` & `plivo-4.9.0/plivo/xml/playElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/speakElement.py` & `plivo-4.9.0/plivo/xml/speakElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/contElement.py` & `plivo-4.9.0/plivo/xml/contElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/xml/redirectElement.py` & `plivo-4.9.0/plivo/xml/redirectElement.py`

 * *Files identical despite different names*

### Comparing `plivo-4.8.1/plivo/base.py` & `plivo-4.9.0/plivo/base.py`

 * *Files identical despite different names*

