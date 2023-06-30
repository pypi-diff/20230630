# Comparing `tmp/bfgdealer-0.0.7.tar.gz` & `tmp/bfgdealer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgdealer-0.0.7.tar", last modified: Tue Jun 20 11:31:05 2023, max compression
+gzip compressed data, was "bfgdealer-0.0.8.tar", last modified: Fri Jun 30 11:32:33 2023, max compression
```

## Comparing `bfgdealer-0.0.7.tar` & `bfgdealer-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.7/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1097 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.7/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.394901 bfgdealer-0.0.7/bfgdealer/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.7/bfgdealer/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/bfgdealer/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.7/bfgdealer/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    22867 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/board.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9879 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/dealer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    28485 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/dealer_duo.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.7/bfgdealer/source/dealer_engine.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14271 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/dealer_solo.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.394901 bfgdealer-0.0.7/bfgdealer.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1097 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.7/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.8/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1160 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.8/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.416379 bfgdealer-0.0.8/bfgdealer/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.8/bfgdealer/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/bfgdealer/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    22861 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/board.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1737 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     8556 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    28485 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer_duo.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16825 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer_engine.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14304 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/bfgdealer/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      289 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/tests/test_set_hands_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.416379 bfgdealer-0.0.8/bfgdealer.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1160 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      471 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.8/setup.py
```

### Comparing `bfgdealer-0.0.7/LICENSE.txt` & `bfgdealer-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.7/PKG-INFO` & `bfgdealer-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.7
+Version: 0.0.8
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.8 30 Jun 2023
+
+1. Linting and start tests
+
+------
+
 Version 0.0.7 20 Jun 2023
 
 1. Various refactor and Lucas 2s
 
 ------
 
 Version 0.0.6 18 Jun 2023
```

### Comparing `bfgdealer-0.0.7/bfgdealer/__init__.py` & `bfgdealer-0.0.8/bfgdealer/__init__.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.7/bfgdealer/source/board.py` & `bfgdealer-0.0.8/bfgdealer/src/board.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from datetime import datetime
 import json
 from termcolor import cprint
 
 from bfgbidding import Player, Hand
 from bridgeobjects import (Board as bfg_Board, RANKS, SEATS, SUITS, SUIT_NAMES,
-                           parse_pbn, Contract, Call,
+                           parse_pbn, Contract,
                            Auction, Trick)
 
 MODULE_COLOUR = 'green'
 DEFAULT_SUIT_ORDER = ['S', 'H', 'C', 'D']
 SEPARATOR = 100
```

### Comparing `bfgdealer-0.0.7/bfgdealer/source/dealer.py` & `bfgdealer-0.0.8/bfgdealer/src/dealer.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,70 +3,34 @@
 import random
 from termcolor import cprint
 
 from bridgeobjects import (SEATS, SHAPES, BALANCED_SHAPES)
 
 from .dealer_engine import DealerEngine
 from .board import Board
+from .constants import (MAX_POINTS, SINGLE_SUITED_SHAPES)
 
 
 MODULE_COLOUR = 'cyan'
 
 
 class Dealer(object):
     """The dealer object for the bridgeobjects module."""
-    DEFAULT_POINTS_RANGE = [12, 14]
-    #: the maximum number of points allowed in a hand
-    MAX_POINTS = 26
-
-    #: shapes suitable for single suited rebids
-    SINGLE_SUITED_SHAPES = [
-        [6, 3, 3, 1], [6, 3, 2, 2], [7, 2, 2, 2],
-        [7, 3, 3, 0], [7, 3, 2, 1], [5, 4, 3, 1],
-        [5, 4, 2, 2], [5, 4, 4, 0], [5, 5, 2, 1],
-        [5, 5, 3, 0], [6, 5, 1, 1], [6, 5, 2, 0],
-        [6, 4, 2, 1], [6, 4, 3, 0], [7, 4, 1, 1],
-        [7, 4, 2, 0], [7, 5, 1, 0], [6, 6, 1, 0],
-        [8, 4, 1, 0], [7, 6, 0, 0], [7, 3, 2, 1],
-        [6, 3, 2, 2], [6, 3, 3, 1], [7, 2, 2, 2],
-        [7, 3, 3, 0], [8, 2, 2, 1], [8, 3, 1, 1],
-        [8, 3, 2, 0], [9, 2, 1, 1], [9, 3, 1, 0],
-        [9, 2, 2, 0]
-    ]
-
-    #: shapes suitable for single suited rebids
-    TWO_SUITED_SHAPES = [
-            [5, 4, 3, 1], [5, 4, 2, 2], [6, 4, 2, 1],
-            [5, 5, 2, 1], [6, 4, 3, 0], [5, 4, 4, 0],
-            [7, 4, 1, 1], [5, 5, 3, 0], [6, 5, 1, 1],
-            [6, 5, 2, 0], [7, 4, 2, 0], [7, 5, 1, 0],
-            [6, 6, 1, 0], [8, 4, 1, 0], [7, 6, 0, 0],
-            [6, 5, 2, 0]
-    ]
-
-    #: Weak two shapes
-    WEAK_TWO_SHAPES = [
-        [6, 3, 3, 1], [6, 3, 2, 2], [7, 2, 2, 2],
-        [7, 3, 3, 0], [7, 3, 2, 1], [6, 5, 1, 1],
-        [6, 5, 2, 0], [6, 4, 2, 1], [6, 4, 3, 0],
-        [7, 4, 1, 1], [7, 4, 2, 0], [7, 5, 1, 0],
-        [6, 6, 1, 0]
-    ]
 
     def __init__(self, dealer=None, allow_overcalls=True):
         if not dealer:
             dealer = random.choice(SEATS)
         self.dealer = dealer
         self.engine = DealerEngine(dealer)
         self.allow_overcalls = allow_overcalls
 
     def deal_random_hand(self, points_range=None):
         """Return a randomly dealt hand."""
         if not points_range:
-            points_range = [0, self.MAX_POINTS]
+            points_range = [0, MAX_POINTS]
         hand = self.engine.get_hand_from_points_and_shape(points_range)
         return hand
 
     def deal_random_board(self, points_range=None):
         """Return a board of randomly dealt hands."""
         hand = self.deal_random_hand(points_range)
         board = None
@@ -102,29 +66,29 @@
         hands = {0: openers_hand, 2: hand}
         board = self.engine.create_board_from_hands(hands)
         return board
 
     def deal_single_suited_hand(self, points_range=None):
         """Return a board with single long suit in the given points range."""
         get_hand = self.engine.get_hand_from_points_and_shape
-        hand = get_hand(points_range, self.SINGLE_SUITED_SHAPES)
+        hand = get_hand(points_range, SINGLE_SUITED_SHAPES)
         return hand
 
     def deal_single_suited_board(self, points_range=None):
         """Return a board with single suited hand in the given points range."""
         hand = self.deal_single_suited_hand(points_range)
         hands = {0: hand}
         board = self.engine.create_board_from_hands(hands)
         return board
 
     def deal_two_suited_hand(self, points_range=None):
         """Return a board with single long suit in the given points range."""
         shape_list = [shape for shape in SHAPES if shape[0] <= 6]
         exclusions = [shape for shape in BALANCED_SHAPES]
-        exclusions.extend(self.SINGLE_SUITED_SHAPES)
+        exclusions.extend(SINGLE_SUITED_SHAPES)
         for shape in exclusions:
             if shape in shape_list:
                 shape_list.remove(shape)
         hand = self.engine.get_hand_from_points_and_shape(points_range, shape_list)
         return hand
 
     def deal_two_suited_board(self, points_range=None):
```

### Comparing `bfgdealer-0.0.7/bfgdealer/source/dealer_duo.py` & `bfgdealer-0.0.8/bfgdealer/src/dealer_duo.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.7/bfgdealer/source/dealer_engine.py` & `bfgdealer-0.0.8/bfgdealer/src/dealer_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,22 @@
 from itertools import combinations
 
 from bridgeobjects import (Card, SUIT_NAMES, RANKS, HONOUR_POINTS,
                            SHAPES, SHAPE_PROBABILITIES, SEATS)
 from bfgbidding import Hand
 
 from .board import Board
+from .constants import MAX_POINTS, POINTS_WEIGHTING
 
 logger = logging.getLogger(__name__)
 
 
 class DealerEngine(object):
     """The dealer object for the bridgeobjects module."""
     DEFAULT_POINTS_RANGE = [12, 14]
-    #: the maximum number of points allowed in a hand
-    MAX_POINTS = 26
-    POINTS_WEIGHTING = {0: 3639, 1: 7884, 2: 13561, 3: 24624, 4: 38454,
-                        5: 51862, 6: 65541, 7: 80281, 8: 88922, 9: 93562,
-                        10: 94051, 11: 89447, 12: 80269, 13: 69143, 14: 56933,
-                        15: 44237, 16: 33109, 17: 23617, 18: 16051, 19: 10362,
-                        20: 6435, 21: 3779, 22: 2100, 23: 1119, 24: 559,
-                        25: 264, 26: 117, 27: 49, 28: 19, 29: 7,
-                        30: 2, 31: 1}
 
     pack = Board.full_pack()
 
     def __init__(self, dealer=None):
         if not dealer:
             dealer = random.choice(SEATS)
         self.dealer = dealer
@@ -97,26 +89,26 @@
     def get_points_from_range(self, points_range=None):
         """
             Return a random high card points value for the hand,
             based on distribution probabilities, as an integer.
             N.B. Highest point count catered for is MAX_POINTS.
         """
         if not points_range:
-            points_range = [0, self.MAX_POINTS]
+            points_range = [0, MAX_POINTS]
         else:
             if len(points_range) == 1:
                 points_range = [points_range[0], points_range[0]]
-            if points_range[0] > self.MAX_POINTS:
-                points_range[0] = self.MAX_POINTS
-            if points_range[1] > self.MAX_POINTS:
-                points_range[1] = self.MAX_POINTS
+            if points_range[0] > MAX_POINTS:
+                points_range[0] = MAX_POINTS
+            if points_range[1] > MAX_POINTS:
+                points_range[1] = MAX_POINTS
         probability_list = []
         # weighting / 100 gives a satisfactory precision
         for value in range(points_range[0], points_range[1]+1):
-            weighting = self.POINTS_WEIGHTING[value]
+            weighting = POINTS_WEIGHTING[value]
             probability_list.extend([value]*int(round(weighting/100)))
         points = random.choice(probability_list)
         return points
 
     @staticmethod
     def rotate_hands(board, offset):
         """Return the board with the hands rotated by the given offset."""
@@ -126,15 +118,15 @@
             board.hands[target] = hands[index]
         return board
 
     @classmethod
     def _candidate_shapes_for_points(cls, points):
         candidate_shapes = cls._select_shapes_for_points(points)
         if not candidate_shapes:
-# @TODO Generate Error here
+            # @TODO Generate Error here
             print('No candidate shapes found')
             return []
         else:
             return candidate_shapes
 
     @classmethod
     def _complete_hand(cls, honour_list, shape, partners_hand):
@@ -142,15 +134,15 @@
         shape_found = False
         loop_two = 0
         shuffled_shape = []
         while not shape_found:
             unsorted_shape = [length for length in shape]
             honour_shape = [0, 0, 0, 0]
             for card in honour_list:
-                honour_shape[card.suit.rank]+=1
+                honour_shape[card.suit.rank] += 1
             shuffled_shape = []
             # Need to create the list 'shuffled_shape' in random order, but the
             # but the number of cards in each suit has to be >= the number of
             # honours in that suit.
             for index in range(4):
                 suit_found = False
                 loop = 0
@@ -163,15 +155,15 @@
                         suit_found = True
                         shape_found = True
                     loop += 1
                     if loop > 10:
                         suit_found = True
                     if len(shuffled_shape) < 4:
                         shape_found = False
-            loop_two+=1
+            loop_two += 1
         if loop_two >= 100:
             logger.info('_complete_hand', str(shape), str(honour_list))
         hand_list = [card for card in honour_list]
         pack_pips = cls._pack_pips(partners_hand)
         for suit, remainder in enumerate(shuffled_shape):
             for _ in range(remainder):
                 if pack_pips[suit]:
@@ -191,15 +183,14 @@
             total_shapes.extend([shape]*weighting)
         return random.choice(total_shapes)
 
     @staticmethod
     def _select_shapes_for_points(points):
         """Return candidate shapes that can support the points given."""
         candidate_shapes = [shape for shape in SHAPES]
-        found = False
         for shape in SHAPES:
             if points > Hand().maximum_points_for_shape(shape):
                 candidate_shapes.remove(shape)
         return candidate_shapes
 
     @classmethod
     def _pack_pips(cls, partners_hand):
@@ -261,17 +252,15 @@
                         partitions.append([aces, kings, queens, jacks])
         return partitions
 
     def _get_candidate_partitions(self, shape, points, partners_hand):
         """Return a list of partitions that meet the points criterion."""
         # now = time.time()
         honour_cards = self._available_honours(partners_hand)
-        candidate_partitions = []
         honour_list = ['A', 'K', 'Q', 'J']
-        partition_shape = [cards for cards in shape]
         candidates = []
         partitions = self.get_partitions(points, partners_hand)
         loop = 0
         while not candidates:
             if not partners_hand:
                 selected_partitions = [random.choice(partitions)]
             else:
@@ -279,15 +268,15 @@
             for partition in selected_partitions:
                 ace_list = []
                 king_list = []
                 queen_list = []
                 jack_list = []
                 for index, honour_count in enumerate(partition):
                     candidate_cards = [card for card in honour_cards
-                                            if card.rank == honour_list[index]]
+                                       if card.rank == honour_list[index]]
                     for combination in list(combinations(candidate_cards, honour_count)):
                         candidate_honours = list(combination)
                         if index == 0:
                             ace_list.append(candidate_honours)
                         elif index == 1:
                             king_list.append(candidate_honours)
                         elif index == 2:
@@ -395,15 +384,15 @@
         """
         fact = math.factorial
         if cards == available:
             combs = 1
         elif cards == 0:
             combs = 1
         else:
-            combs = (fact(available) / fact(cards) / fact(available -cards))
+            combs = (fact(available) / fact(cards) / fact(available - cards))
         return combs
 
     @classmethod
     def _pip_combinations(cls, pip_cards, partners_hand):
         """
         Return the number of ways that the pip cards can be
         allocated once the honours have been used to make up a point count.
```

### Comparing `bfgdealer-0.0.7/bfgdealer/source/dealer_solo.py` & `bfgdealer-0.0.8/bfgdealer/src/dealer_solo.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self.generate_hand = self.engine.get_hand_from_points_and_shape
         self.create_board = self.engine.create_board_from_hands
 
     def get_set_hand(self, stages, seat):
         """Return a board relevant to set stages."""
         seat_index = SEATS.index(seat)
         stage = int(random.choice(stages))
+        print(self, stage, seat)
         board = self.set_hands[stage][1](seat_index)
         board.stage = stage
         return board
 
     def opening_one_board(self, seat_index):
         """Return a board suitable for an opening one."""
         found = False
```

### Comparing `bfgdealer-0.0.7/bfgdealer.egg-info/PKG-INFO` & `bfgdealer-0.0.8/bfgdealer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.7
+Version: 0.0.8
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.8 30 Jun 2023
+
+1. Linting and start tests
+
+------
+
 Version 0.0.7 20 Jun 2023
 
 1. Various refactor and Lucas 2s
 
 ------
 
 Version 0.0.6 18 Jun 2023
```

### Comparing `bfgdealer-0.0.7/setup.py` & `bfgdealer-0.0.8/setup.py`

 * *Files identical despite different names*

