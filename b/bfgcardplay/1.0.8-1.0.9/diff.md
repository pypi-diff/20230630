# Comparing `tmp/bfgcardplay-1.0.8.tar.gz` & `tmp/bfgcardplay-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgcardplay-1.0.8.tar", last modified: Thu Jun 29 14:58:22 2023, max compression
+gzip compressed data, was "bfgcardplay-1.0.9.tar", last modified: Thu Jun 29 16:09:20 2023, max compression
```

## Comparing `bfgcardplay-1.0.8.tar` & `bfgcardplay-1.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4050 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.8/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.204541 bfgcardplay-1.0.8/bfgcardplay/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      215 2023-06-29 13:52:00.000000 bfgcardplay-1.0.8/bfgcardplay/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/_version.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.8/bfgcardplay/logger.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.207874 bfgcardplay-1.0.8/bfgcardplay/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3446 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/card_player_components.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2303 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/cards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    19533 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/dashboard.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4663 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/data_classes.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    12296 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/declarer_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3976 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/defender_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9753 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16201 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17433 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_nt.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    21952 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16445 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2026 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6553 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5369 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/global_variables.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3935 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/manager.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      665 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/opening_lead.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6982 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    43274 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    24438 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3025 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/second_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9986 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/second_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7231 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/second_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3638 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/suggested_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1880 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/third_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17664 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/third_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14321 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6542 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/bfgcardplay/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      558 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      449 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11743 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    15003 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      587 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6565 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_utilities.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      294 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.204541 bfgcardplay-1.0.8/bfgcardplay.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4050 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1589 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.8/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 16:09:20.762268 bfgcardplay-1.0.9/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4113 2023-06-29 16:09:20.762268 bfgcardplay-1.0.9/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.9/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 16:09:20.752268 bfgcardplay-1.0.9/bfgcardplay/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      215 2023-06-29 13:52:00.000000 bfgcardplay-1.0.9/bfgcardplay/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 16:08:20.000000 bfgcardplay-1.0.9/bfgcardplay/_version.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.9/bfgcardplay/logger.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 16:09:20.758934 bfgcardplay-1.0.9/bfgcardplay/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3446 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/card_player_components.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2303 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/cards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    19533 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/dashboard.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4663 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/data_classes.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    12296 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/declarer_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3976 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/defender_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9753 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/first_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16201 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/first_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17433 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/first_seat_declarer_nt.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    21952 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/first_seat_declarer_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16445 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2026 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/fourth_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6553 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5369 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/fourth_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/global_variables.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3935 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/manager.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      665 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/opening_lead.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6982 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    43274 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    24438 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3025 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/second_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9986 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/second_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7231 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/second_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3638 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/suggested_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1880 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/third_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17664 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/third_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14321 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6542 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/src/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 16:09:20.762268 bfgcardplay-1.0.9/bfgcardplay/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      558 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/test_first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      449 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/test_fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    11743 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/test_opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    15003 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/test_opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/test_player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      587 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/test_third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6565 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/test_utilities.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      294 2023-06-29 14:57:34.000000 bfgcardplay-1.0.9/bfgcardplay/tests/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 16:09:20.755601 bfgcardplay-1.0.9/bfgcardplay.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4113 2023-06-29 16:09:20.000000 bfgcardplay-1.0.9/bfgcardplay.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1589 2023-06-29 16:09:20.000000 bfgcardplay-1.0.9/bfgcardplay.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 16:09:20.000000 bfgcardplay-1.0.9/bfgcardplay.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-06-29 16:09:20.000000 bfgcardplay-1.0.9/bfgcardplay.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 16:09:20.762268 bfgcardplay-1.0.9/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.9/setup.py
```

### Comparing `bfgcardplay-1.0.8/PKG-INFO` & `bfgcardplay-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.8
+Version: 1.0.9
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.9 29 Jun 2023
+
+1. Clear Build directories
+
+------
+
 Version 1.0.8 29 Jun 2023
 
 1. Linting
 
 ------
 
 Version 1.0.7 29 Jun 2023
```

### Comparing `bfgcardplay-1.0.8/bfgcardplay/logger.py` & `bfgcardplay-1.0.9/bfgcardplay/logger.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/card_player_components.py` & `bfgcardplay-1.0.9/bfgcardplay/src/card_player_components.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/cards.py` & `bfgcardplay-1.0.9/bfgcardplay/src/cards.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/dashboard.py` & `bfgcardplay-1.0.9/bfgcardplay/src/dashboard.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/data_classes.py` & `bfgcardplay-1.0.9/bfgcardplay/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/declarer_play.py` & `bfgcardplay-1.0.9/bfgcardplay/src/declarer_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/defender_play.py` & `bfgcardplay-1.0.9/bfgcardplay/src/defender_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/first_seat.py` & `bfgcardplay-1.0.9/bfgcardplay/src/first_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer.py` & `bfgcardplay-1.0.9/bfgcardplay/src/first_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_nt.py` & `bfgcardplay-1.0.9/bfgcardplay/src/first_seat_declarer_nt.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_suit.py` & `bfgcardplay-1.0.9/bfgcardplay/src/first_seat_declarer_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_defender.py` & `bfgcardplay-1.0.9/bfgcardplay/src/first_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat.py` & `bfgcardplay-1.0.9/bfgcardplay/src/fourth_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_declarer.py` & `bfgcardplay-1.0.9/bfgcardplay/src/fourth_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_defender.py` & `bfgcardplay-1.0.9/bfgcardplay/src/fourth_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/manager.py` & `bfgcardplay-1.0.9/bfgcardplay/src/manager.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/opening_lead.py` & `bfgcardplay-1.0.9/bfgcardplay/src/opening_lead.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_card.py` & `bfgcardplay-1.0.9/bfgcardplay/src/opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_suit.py` & `bfgcardplay-1.0.9/bfgcardplay/src/opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/player.py` & `bfgcardplay-1.0.9/bfgcardplay/src/player.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/second_seat.py` & `bfgcardplay-1.0.9/bfgcardplay/src/second_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/second_seat_declarer.py` & `bfgcardplay-1.0.9/bfgcardplay/src/second_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/second_seat_defender.py` & `bfgcardplay-1.0.9/bfgcardplay/src/second_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/suggested_card.py` & `bfgcardplay-1.0.9/bfgcardplay/src/suggested_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/third_seat.py` & `bfgcardplay-1.0.9/bfgcardplay/src/third_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/third_seat_declarer.py` & `bfgcardplay-1.0.9/bfgcardplay/src/third_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/third_seat_defender.py` & `bfgcardplay-1.0.9/bfgcardplay/src/third_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/src/utilities.py` & `bfgcardplay-1.0.9/bfgcardplay/src/utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/tests/test_first_seat_defender.py` & `bfgcardplay-1.0.9/bfgcardplay/tests/test_first_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_card.py` & `bfgcardplay-1.0.9/bfgcardplay/tests/test_opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_suit.py` & `bfgcardplay-1.0.9/bfgcardplay/tests/test_opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/tests/test_third_seat_defender.py` & `bfgcardplay-1.0.9/bfgcardplay/tests/test_third_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay/tests/test_utilities.py` & `bfgcardplay-1.0.9/bfgcardplay/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/bfgcardplay.egg-info/PKG-INFO` & `bfgcardplay-1.0.9/bfgcardplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.8
+Version: 1.0.9
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.9 29 Jun 2023
+
+1. Clear Build directories
+
+------
+
 Version 1.0.8 29 Jun 2023
 
 1. Linting
 
 ------
 
 Version 1.0.7 29 Jun 2023
```

### Comparing `bfgcardplay-1.0.8/bfgcardplay.egg-info/SOURCES.txt` & `bfgcardplay-1.0.9/bfgcardplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.8/setup.py` & `bfgcardplay-1.0.9/setup.py`

 * *Files identical despite different names*

