# Comparing `tmp/pyAMOSA-1.3.7.tar.gz` & `tmp/pyAMOSA-1.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAMOSA-1.3.7.tar", last modified: Tue Jun 27 07:32:15 2023, max compression
+gzip compressed data, was "pyAMOSA-1.3.7.1.tar", last modified: Fri Jun 30 14:11:31 2023, max compression
```

## Comparing `pyAMOSA-1.3.7.tar` & `pyAMOSA-1.3.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-27 07:32:15.797177 pyAMOSA-1.3.7/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-01-23 18:16:52.000000 pyAMOSA-1.3.7/LICENSE
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      919 2023-06-27 07:32:15.796177 pyAMOSA-1.3.7/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    10688 2023-02-03 22:09:51.000000 pyAMOSA-1.3.7/README.md
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-27 07:32:15.787177 pyAMOSA-1.3.7/pyAMOSA.egg-info/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      919 2023-06-27 07:32:13.000000 pyAMOSA-1.3.7/pyAMOSA.egg-info/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      446 2023-06-27 07:32:15.000000 pyAMOSA-1.3.7/pyAMOSA.egg-info/SOURCES.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-06-27 07:32:13.000000 pyAMOSA-1.3.7/pyAMOSA.egg-info/dependency_links.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       28 2023-06-27 07:32:14.000000 pyAMOSA-1.3.7/pyAMOSA.egg-info/requires.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        8 2023-06-27 07:32:14.000000 pyAMOSA-1.3.7/pyAMOSA.egg-info/top_level.txt
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-27 07:32:15.795177 pyAMOSA-1.3.7/pyamosa/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1480 2023-06-27 07:17:47.000000 pyAMOSA-1.3.7/pyamosa/CombinedStopCriterion.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2784 2023-02-03 22:09:51.000000 pyAMOSA-1.3.7/pyamosa/Config.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      787 2023-02-03 22:09:51.000000 pyAMOSA-1.3.7/pyamosa/DataType.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2412 2023-02-03 22:09:51.000000 pyAMOSA-1.3.7/pyamosa/MultiFileCacheHandle.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35094 2023-06-27 07:30:33.000000 pyAMOSA-1.3.7/pyamosa/Optimizer.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     3169 2023-02-03 22:09:51.000000 pyAMOSA-1.3.7/pyamosa/Problem.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      868 2023-02-03 22:09:51.000000 pyAMOSA-1.3.7/pyamosa/StopCriterion.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1344 2023-06-27 07:17:47.000000 pyAMOSA-1.3.7/pyamosa/StopMaxTime.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1218 2023-06-27 07:17:47.000000 pyAMOSA-1.3.7/pyamosa/StopMinTemperature.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1264 2023-06-27 07:17:47.000000 pyAMOSA-1.3.7/pyamosa/StopPhyWindow.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1280 2023-06-27 07:31:05.000000 pyAMOSA-1.3.7/pyamosa/__init__.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-06-27 07:32:15.797177 pyAMOSA-1.3.7/setup.cfg
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1638 2023-06-27 07:31:17.000000 pyAMOSA-1.3.7/setup.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-30 14:11:31.777575 pyAMOSA-1.3.7.1/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-02-04 09:39:41.000000 pyAMOSA-1.3.7.1/LICENSE
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      921 2023-06-30 14:11:31.777575 pyAMOSA-1.3.7.1/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    10688 2023-02-04 09:39:41.000000 pyAMOSA-1.3.7.1/README.md
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-30 14:11:31.776575 pyAMOSA-1.3.7.1/pyAMOSA.egg-info/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      921 2023-06-30 14:11:31.000000 pyAMOSA-1.3.7.1/pyAMOSA.egg-info/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      446 2023-06-30 14:11:31.000000 pyAMOSA-1.3.7.1/pyAMOSA.egg-info/SOURCES.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-06-30 14:11:31.000000 pyAMOSA-1.3.7.1/pyAMOSA.egg-info/dependency_links.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       28 2023-06-30 14:11:31.000000 pyAMOSA-1.3.7.1/pyAMOSA.egg-info/requires.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        8 2023-06-30 14:11:31.000000 pyAMOSA-1.3.7.1/pyAMOSA.egg-info/top_level.txt
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-30 14:11:31.777575 pyAMOSA-1.3.7.1/pyamosa/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1480 2023-02-04 11:08:11.000000 pyAMOSA-1.3.7.1/pyamosa/CombinedStopCriterion.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2784 2023-02-04 09:39:41.000000 pyAMOSA-1.3.7.1/pyamosa/Config.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      787 2023-02-04 09:39:41.000000 pyAMOSA-1.3.7.1/pyamosa/DataType.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2412 2023-02-04 09:39:41.000000 pyAMOSA-1.3.7.1/pyamosa/MultiFileCacheHandle.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    33696 2023-06-30 13:49:30.000000 pyAMOSA-1.3.7.1/pyamosa/Optimizer.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     3169 2023-02-04 09:39:41.000000 pyAMOSA-1.3.7.1/pyamosa/Problem.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      868 2023-02-04 09:39:41.000000 pyAMOSA-1.3.7.1/pyamosa/StopCriterion.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1344 2023-02-04 11:10:36.000000 pyAMOSA-1.3.7.1/pyamosa/StopMaxTime.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1218 2023-02-04 11:10:32.000000 pyAMOSA-1.3.7.1/pyamosa/StopMinTemperature.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1264 2023-02-04 11:10:27.000000 pyAMOSA-1.3.7.1/pyamosa/StopPhyWindow.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1282 2023-06-30 13:49:59.000000 pyAMOSA-1.3.7.1/pyamosa/__init__.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-06-30 14:11:31.777575 pyAMOSA-1.3.7.1/setup.cfg
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1640 2023-06-30 13:49:53.000000 pyAMOSA-1.3.7.1/setup.py
```

### Comparing `pyAMOSA-1.3.7/LICENSE` & `pyAMOSA-1.3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/PKG-INFO` & `pyAMOSA-1.3.7.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAMOSA
-Version: 1.3.7
+Version: 1.3.7.1
 Summary: Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic
 Home-page: https://github.com/SalvatoreBarone/pyAMOSA
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyAMOSA/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyAMOSA
 Keywords: Verilator Wrapper Verilog
```

### Comparing `pyAMOSA-1.3.7/README.md` & `pyAMOSA-1.3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyAMOSA.egg-info/PKG-INFO` & `pyAMOSA-1.3.7.1/pyAMOSA.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAMOSA
-Version: 1.3.7
+Version: 1.3.7.1
 Summary: Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic
 Home-page: https://github.com/SalvatoreBarone/pyAMOSA
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyAMOSA/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyAMOSA
 Keywords: Verilator Wrapper Verilog
```

### Comparing `pyAMOSA-1.3.7/pyamosa/CombinedStopCriterion.py` & `pyAMOSA-1.3.7.1/pyamosa/CombinedStopCriterion.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/Config.py` & `pyAMOSA-1.3.7.1/pyamosa/Config.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/DataType.py` & `pyAMOSA-1.3.7.1/pyamosa/DataType.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/MultiFileCacheHandle.py` & `pyAMOSA-1.3.7.1/pyamosa/MultiFileCacheHandle.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/Optimizer.py` & `pyAMOSA-1.3.7.1/pyamosa/Optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 more details.
 
 You should have received a copy of the GNU General Public License along with
 RMEncoder; if not, write to the Free Software Foundation, Inc., 51 Franklin
 Street, Fifth Floor, Boston, MA 02110-1301, USA.
 """
 import sys, copy, random, time, os, json, warnings, numpy as np, matplotlib.pyplot as plt
-from multiprocessing import cpu_count, Pool
 from tqdm import tqdm, trange
 from .DataType import Type
 from .Config import Config
 from .Problem import Problem
 from .StopCriterion import StopCriterion
 from .StopMinTemperature import StopMinTemperature
 class Optimizer:
@@ -182,57 +181,41 @@
         with open(json_file) as file:
             archive = json.load(file)
         self.archive = [{"x": [int(i) if j == Type.INTEGER else float(i) for i, j in zip(a["x"], problem.types)], "f": a["f"], "g": a["g"]} for a in archive]
 
     def initial_hill_climbing(self, problem, initial_candidate_solutions):
         num_of_initial_candidate_solutions = self.config.archive_gamma * self.config.archive_soft_limit
         if self.config.hill_climbing_iterations > 0:
-            if self.config.multiprocessing_enabled:
-                args = [[problem, self.config.hill_climbing_iterations]] * cpu_count()
-                print(f"Performing Initial Hill Climbing Step using {cpu_count()} threads")
-                for _ in trange(len(initial_candidate_solutions), num_of_initial_candidate_solutions, cpu_count(), desc = "Hill climbing", leave = False, bar_format="{desc:40} {percentage:3.0f}% |{bar:60}{r_bar}{bar:-10b}"):
-                    with Pool(cpu_count()) as pool:
-                        new_points = pool.starmap(Optimizer.hillclimb_thread_loop, args)
-                    initial_candidate_solutions += new_points
-                    self.save_checkpoint_hillclimb(initial_candidate_solutions)
-            else:
-                for _ in trange(len(initial_candidate_solutions), num_of_initial_candidate_solutions, desc = "Hill climbing", leave = False, bar_format="{desc:40} {percentage:3.0f}% |{bar:60}{r_bar}{bar:-10b}"):
-                    initial_candidate_solutions.append(Optimizer.hillclimb_thread_loop(problem, self.config.hill_climbing_iterations))
-                    self.save_checkpoint_hillclimb(initial_candidate_solutions)
+            for _ in trange(len(initial_candidate_solutions), num_of_initial_candidate_solutions, desc = "Hill climbing", leave = False, bar_format="{desc:30} {percentage:3.0f}% |{bar:40}{r_bar}{bar:-10b}"):
+                initial_candidate_solutions.append(Optimizer.hillclimb_thread_loop(problem, self.config.hill_climbing_iterations))
+                self.save_checkpoint_hillclimb(initial_candidate_solutions)
         for x in initial_candidate_solutions:
             Optimizer.add_to_archive(self.archive, x)
 
     @staticmethod
     def hillclimb_thread_loop(problem, hillclimb_iterations):
         return Optimizer.hill_climbing(problem, Optimizer.random_point(problem), hillclimb_iterations)
 
     def main_loop(self, problem : Problem, termination_criterion : StopCriterion):
         current_point = random.choice(self.archive)
         while not termination_criterion.check_termination(self):
             self.current_temperature *= self.config.cooling_factor
-            if self.config.multiprocessing_enabled:
-                args = [[problem, self.archive.copy(), random.choice(self.archive), self.current_temperature, self.config.annealing_iterations, self.config.annealing_strength, self.config.archive_soft_limit, self.config.archive_hard_limit, self.config.clustering_max_iterations, True, i] for i in [t == 0 for t in range(cpu_count())]]
-                with Pool(cpu_count()) as pool:
-                    archives = pool.starmap(Optimizer.annealing_thread_loop, args)
-                self.archive = Optimizer.nondominated_merge(archives)
-                self.n_eval += self.config.annealing_iterations * cpu_count()
-            else:
-                self.archive = Optimizer.annealing_thread_loop(problem, self.archive, current_point, self.current_temperature, self.config.annealing_iterations, self.config.annealing_strength, self.config.archive_soft_limit, self.config.archive_hard_limit, self.config.clustering_max_iterations, False, True)
-                self.n_eval += self.config.annealing_iterations
+            self.archive = Optimizer.annealing_thread_loop(problem, self.archive, current_point, self.current_temperature, self.config.annealing_iterations, self.config.annealing_strength, self.config.archive_soft_limit, self.config.archive_hard_limit, self.config.clustering_max_iterations, False, True)
+            self.n_eval += self.config.annealing_iterations
             self.print_statistics(problem)
             if len(self.archive) > self.config.archive_soft_limit:
                 self.archive = Optimizer.clustering(self.archive, problem, self.config.archive_hard_limit, self.config.clustering_max_iterations, True)
                 self.print_statistics(problem)
             self.save_checkpoint_minimize()
             problem.store_cache(self.config.cache_dir)
         print("Termination criterion has been met.")
 
     @staticmethod
     def annealing_thread_loop(problem, archive, current_point, current_temperature, annealing_iterations, annealing_strength, soft_limit, hard_limit, clustering_max_iterations, clustering_before_return, print_allowed):
-        for _ in trange(annealing_iterations, desc = "Annealing", file=sys.stdout, leave = False, bar_format="{desc:40} {percentage:3.0f}% |{bar:60}{r_bar}{bar:-10b}") if print_allowed else range(annealing_iterations):
+        for _ in trange(annealing_iterations, desc = "Annealing", file=sys.stdout, leave = False, bar_format="{desc:30} {percentage:3.0f}% |{bar:40}{r_bar}{bar:-10b}") if print_allowed else range(annealing_iterations):
             new_point = Optimizer.random_perturbation(problem, current_point, annealing_strength)
             fitness_range = Optimizer.compute_fitness_range(archive, current_point, new_point)
             s_dominating_y = [s for s in archive if Optimizer.dominates(s, new_point)]
             s_dominated_by_y = [s for s in archive if Optimizer.dominates(new_point, s)]
             k_s_dominated_by_y = len(s_dominated_by_y)
             k_s_dominating_y = len(s_dominating_y)
             if Optimizer.dominates(current_point, new_point) and k_s_dominating_y >= 0:
@@ -431,15 +414,15 @@
     def compute_fitness_range(archive, current_point, new_point):
         f = [s["f"] for s in archive] + [current_point["f"], new_point["f"]]
         return np.nanmax(f, axis = 0) - np.nanmin(f, axis = 0)
 
     @staticmethod
     def hill_climbing(problem, x, max_iterations):
         dimention, increase = Optimizer.hill_climbing_direction(problem)
-        for _ in range(max_iterations):
+        for _ in trange(max_iterations, desc = "Walking...", leave = False, bar_format="{desc:30} {percentage:3.0f}% |{bar:40}{r_bar}{bar:-10b}"):
             y = copy.deepcopy(x)
             Optimizer.hill_climbing_adaptive_step(problem, y, dimention, increase)
             if Optimizer.dominates(y, x) and Optimizer.not_the_same(y, x):
                 x = y
             else:
                 dimention, increase = Optimizer.hill_climbing_direction(problem, dimention)
         return x
@@ -528,15 +511,15 @@
                     archive.remove(y)
             if not any(Optimizer.dominates(y, x) or Optimizer.is_the_same(x, y) for y in archive):
                 archive.append(x)
 
     @staticmethod
     def nondominated_merge(archives):
         nondominated_archive = []
-        for archive in tqdm(archives, desc = "Merging archives: ", leave = False, bar_format="{desc:40} {percentage:3.0f}% |{bar:60}{r_bar}{bar:-10b}"):
+        for archive in tqdm(archives, desc = "Merging archives: ", leave = False, bar_format="{desc:30} {percentage:3.0f}% |{bar:40}{r_bar}{bar:-10b}"):
             for x in archive:
                 Optimizer.add_to_archive(nondominated_archive, x)
         return nondominated_archive
 
     @staticmethod
     def compute_cv(archive):
         g = np.array([s["g"] for s in archive])
@@ -579,15 +562,15 @@
     def kmeans_clustering(archive, num_of_clusters, max_iterations, print_allowed):
         assert max_iterations > 0
         if 1 < num_of_clusters < len(archive):
             # Initialize the centroids, using the "k-means++" method, where a random datapoint is selected as the first,
             # then the rest are initialized w/ probabilities proportional to their distances to the first
             # Pick a random point from train data for first centroid
             centroids = [random.choice(archive)]
-            for _ in trange(num_of_clusters - 1, desc = "Centroids", leave = False, bar_format="{desc:40} {percentage:3.0f}% |{bar:60}{r_bar}{bar:-10b}") if print_allowed else range(num_of_clusters - 1):
+            for _ in trange(num_of_clusters - 1, desc = "Centroids", leave = False, bar_format="{desc:30} {percentage:3.0f}% |{bar:40}{r_bar}{bar:-10b}") if print_allowed else range(num_of_clusters - 1):
                 # Calculate normalized distances from points to the centroids
                 dists = np.array([np.nansum([np.linalg.norm(np.array(centroid["f"]) - np.array(p["f"])) for centroid in centroids]) for p in archive])
                 try:
                     normalized_dists = dists / np.nansum(dists)
                     # Choose remaining points based on their distances
                     new_centroid_idx = np.random.choice(range(len(archive)), size = 1, p = normalized_dists)[0]  # Indexed @ zero to get val, not array of val
                     centroids += [archive[new_centroid_idx]]
@@ -595,15 +578,15 @@
                     print(e)
                     print(f"Archive: {archive}")
                     print(f"Centroids: {centroids}")
                     print(f"Distance: {dists}")
                     print(f"Normalized distance: {dists / np.nansum(dists)}")
                     exit()
             # Iterate, adjusting centroids until converged or until passed max_iter
-            for _ in trange(max_iterations, desc = "K-means", leave = False, bar_format="{desc:40} {percentage:3.0f}% |{bar:60}{r_bar}{bar:-10b}") if print_allowed else range(max_iterations):
+            for _ in trange(max_iterations, desc = "K-means", leave = False, bar_format="{desc:30} {percentage:3.0f}% |{bar:40}{r_bar}{bar:-10b}") if print_allowed else range(max_iterations):
                 # Sort each datapoint, assigning to nearest centroid
                 sorted_points = [[] for _ in range(num_of_clusters)]
                 for x in archive:
                     dists = [np.linalg.norm(np.array(x["f"]) - np.array(centroid["f"])) for centroid in centroids]
                     centroid_idx = np.argmin(dists)
                     sorted_points[centroid_idx].append(x)
                 # Push current centroids to previous, reassign centroids as mean of the points belonging to them
```

### Comparing `pyAMOSA-1.3.7/pyamosa/Problem.py` & `pyAMOSA-1.3.7.1/pyamosa/Problem.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/StopCriterion.py` & `pyAMOSA-1.3.7.1/pyamosa/StopCriterion.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/StopMaxTime.py` & `pyAMOSA-1.3.7.1/pyamosa/StopMaxTime.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/StopMinTemperature.py` & `pyAMOSA-1.3.7.1/pyamosa/StopMinTemperature.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/StopPhyWindow.py` & `pyAMOSA-1.3.7.1/pyamosa/StopPhyWindow.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.7/pyamosa/__init__.py` & `pyAMOSA-1.3.7.1/pyamosa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 from .StopCriterion import StopCriterion
 from .StopMaxTime import StopMaxTime
 from .StopMinTemperature import StopMinTemperature
 from .StopPhyWindow import StopPhyWindow
 from .CombinedStopCriterion import CombinedStopCriterion
 
 name = "pyamosa"
-__version__ = "1.3.7"
+__version__ = "1.3.7.1"
 __author__ = "Salvatore Barone"
 __credits__ = "Department of Electrical Engineering and Information Technologies, University of Naples Federico II, Via Claudio 21, Naples, Italy"
```

### Comparing `pyAMOSA-1.3.7/setup.py` & `pyAMOSA-1.3.7.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyAMOSA",
-    version="1.3.7",
+    version="1.3.7.1",
     description="Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic",
     long_description="Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic. Take a look at https://github.com/SalvatoreBarone/pyAMOSA.",
     url="https://github.com/SalvatoreBarone/pyAMOSA",
     author="Salvatore Barone",
     author_email="salvatore.barone@unina.it",
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

