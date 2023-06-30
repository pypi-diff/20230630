# Comparing `tmp/mouse2-0.2.8.tar.gz` & `tmp/mouse2-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mouse2-0.2.8.tar", last modified: Tue Apr  4 09:51:59 2023, max compression
+gzip compressed data, was "mouse2-0.2.9.tar", last modified: Fri May  5 11:28:43 2023, max compression
```

## Comparing `mouse2-0.2.8.tar` & `mouse2-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-04-04 09:51:59.092269 mouse2-0.2.8/
--rw-rw-r--   0 misha     (2001) misha     (2001)    35149 2023-02-09 15:19:09.000000 mouse2-0.2.8/LICENSE
--rw-rw-r--   0 misha     (2001) misha     (2001)    10501 2023-04-04 09:51:59.092269 mouse2-0.2.8/PKG-INFO
--rw-rw-r--   0 misha     (2001) misha     (2001)     9885 2023-02-20 10:49:11.000000 mouse2-0.2.8/README.md
-drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-04-04 09:51:59.092269 mouse2-0.2.8/mouse2/
--rw-rw-r--   0 misha     (2001) misha     (2001)      254 2023-04-04 09:51:13.000000 mouse2-0.2.8/mouse2/__init__.py
--rwxrwxr-x   0 misha     (2001) misha     (2001)     1475 2023-02-09 17:35:52.000000 mouse2-0.2.8/mouse2/aggregates.py
--rwxrw-r--   0 misha     (2001) misha     (2001)    11037 2023-02-09 17:52:30.000000 mouse2-0.2.8/mouse2/backbone_twist.py
--rwxrwxr-x   0 misha     (2001) misha     (2001)     8573 2023-02-20 09:27:00.000000 mouse2-0.2.8/mouse2/bond_autocorrelations.py
--rwxrwxr-x   0 misha     (2001) misha     (2001)     1495 2023-04-04 09:48:30.000000 mouse2-0.2.8/mouse2/data2pdb.py
--rwxrw-r--   0 misha     (2001) misha     (2001)     2814 2023-02-20 16:34:40.000000 mouse2-0.2.8/mouse2/lamellar_alignment.py
-drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-04-04 09:51:59.092269 mouse2-0.2.8/mouse2/lib/
--rw-rw-r--   0 misha     (2001) misha     (2001)      258 2023-04-04 09:51:05.000000 mouse2-0.2.8/mouse2/lib/__init__.py
--rw-rw-r--   0 misha     (2001) misha     (2001)     4259 2023-03-30 11:22:43.000000 mouse2-0.2.8/mouse2/lib/aggregation.py
--rw-rw-r--   0 misha     (2001) misha     (2001)     8591 2023-02-20 20:43:16.000000 mouse2-0.2.8/mouse2/lib/lamellar_orientation.py
--rw-rw-r--   0 misha     (2001) misha     (2001)     8778 2022-12-16 20:50:41.000000 mouse2-0.2.8/mouse2/lib/neighbor.py
--rw-rw-r--   0 misha     (2001) misha     (2001)      776 2023-04-04 09:46:45.000000 mouse2-0.2.8/mouse2/lib/utilities.py
--rw-rw-r--   0 misha     (2001) misha     (2001)     3864 2023-02-17 18:19:27.000000 mouse2-0.2.8/mouse2/lib/vector_orientational_ordering.py
--rwxrwxr-x   0 misha     (2001) misha     (2001)    14033 2023-03-30 11:54:41.000000 mouse2-0.2.8/mouse2/local_alignment.py
-drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-04-04 09:51:59.092269 mouse2-0.2.8/mouse2.egg-info/
--rw-rw-r--   0 misha     (2001) misha     (2001)    10501 2023-04-04 09:51:58.000000 mouse2-0.2.8/mouse2.egg-info/PKG-INFO
--rw-rw-r--   0 misha     (2001) misha     (2001)      647 2023-04-04 09:51:58.000000 mouse2-0.2.8/mouse2.egg-info/SOURCES.txt
--rw-rw-r--   0 misha     (2001) misha     (2001)        1 2023-04-04 09:51:58.000000 mouse2-0.2.8/mouse2.egg-info/dependency_links.txt
--rw-rw-r--   0 misha     (2001) misha     (2001)      287 2023-04-04 09:51:58.000000 mouse2-0.2.8/mouse2.egg-info/entry_points.txt
--rw-rw-r--   0 misha     (2001) misha     (2001)       43 2023-04-04 09:51:58.000000 mouse2-0.2.8/mouse2.egg-info/requires.txt
--rw-rw-r--   0 misha     (2001) misha     (2001)       20 2023-04-04 09:51:58.000000 mouse2-0.2.8/mouse2.egg-info/top_level.txt
-drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-04-04 09:51:59.092269 mouse2-0.2.8/mouse2_tests/
--rw-rw-r--   0 misha     (2001) misha     (2001)      260 2023-04-04 09:51:09.000000 mouse2-0.2.8/mouse2_tests/__init__.py
--rwxrwxr-x   0 misha     (2001) misha     (2001)     5935 2023-03-10 11:49:30.000000 mouse2-0.2.8/mouse2_tests/create_configuration.py
--rwxrw-r--   0 misha     (2001) misha     (2001)    17414 2023-02-21 00:14:36.000000 mouse2-0.2.8/mouse2_tests/test_functions.py
--rw-rw-r--   0 misha     (2001) misha     (2001)       38 2023-04-04 09:51:59.092269 mouse2-0.2.8/setup.cfg
--rw-rw-r--   0 misha     (2001) misha     (2001)     1567 2023-04-04 09:51:27.000000 mouse2-0.2.8/setup.py
+drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-05-05 11:28:43.373637 mouse2-0.2.9/
+-rw-rw-r--   0 misha     (2001) misha     (2001)    35149 2023-02-09 15:19:09.000000 mouse2-0.2.9/LICENSE
+-rw-rw-r--   0 misha     (2001) misha     (2001)    10481 2023-05-05 11:28:43.373637 mouse2-0.2.9/PKG-INFO
+-rw-rw-r--   0 misha     (2001) misha     (2001)     9885 2023-02-20 10:49:11.000000 mouse2-0.2.9/README.md
+drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-05-05 11:28:43.369637 mouse2-0.2.9/mouse2/
+-rw-rw-r--   0 misha     (2001) misha     (2001)      254 2023-05-05 11:28:11.000000 mouse2-0.2.9/mouse2/__init__.py
+-rwxrwxr-x   0 misha     (2001) misha     (2001)     1469 2023-05-03 13:33:08.000000 mouse2-0.2.9/mouse2/aggregates.py
+-rwxrw-r--   0 misha     (2001) misha     (2001)    11031 2023-05-03 13:33:15.000000 mouse2-0.2.9/mouse2/backbone_twist.py
+-rwxrwxr-x   0 misha     (2001) misha     (2001)     8573 2023-02-20 09:27:00.000000 mouse2-0.2.9/mouse2/bond_autocorrelations.py
+-rwxrwxr-x   0 misha     (2001) misha     (2001)     1489 2023-05-03 13:33:30.000000 mouse2-0.2.9/mouse2/data2pdb.py
+-rwxrw-r--   0 misha     (2001) misha     (2001)     2808 2023-05-03 13:33:37.000000 mouse2-0.2.9/mouse2/lamellar_alignment.py
+drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-05-05 11:28:43.369637 mouse2-0.2.9/mouse2/lib/
+-rw-rw-r--   0 misha     (2001) misha     (2001)      258 2023-05-05 11:28:17.000000 mouse2-0.2.9/mouse2/lib/__init__.py
+-rw-rw-r--   0 misha     (2001) misha     (2001)     4607 2023-05-05 11:23:00.000000 mouse2-0.2.9/mouse2/lib/aggregation.py
+-rw-rw-r--   0 misha     (2001) misha     (2001)     8583 2023-05-04 13:29:42.000000 mouse2-0.2.9/mouse2/lib/lamellar_orientation.py
+-rw-rw-r--   0 misha     (2001) misha     (2001)     8778 2022-12-16 20:50:41.000000 mouse2-0.2.9/mouse2/lib/neighbor.py
+-rw-rw-r--   0 misha     (2001) misha     (2001)      776 2023-04-04 09:46:45.000000 mouse2-0.2.9/mouse2/lib/utilities.py
+-rw-rw-r--   0 misha     (2001) misha     (2001)     3855 2023-05-04 13:26:07.000000 mouse2-0.2.9/mouse2/lib/vector_orientational_ordering.py
+-rwxrwxr-x   0 misha     (2001) misha     (2001)    14027 2023-05-03 13:33:45.000000 mouse2-0.2.9/mouse2/local_alignment.py
+drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-05-05 11:28:43.369637 mouse2-0.2.9/mouse2.egg-info/
+-rw-rw-r--   0 misha     (2001) misha     (2001)    10481 2023-05-05 11:28:43.000000 mouse2-0.2.9/mouse2.egg-info/PKG-INFO
+-rw-rw-r--   0 misha     (2001) misha     (2001)      647 2023-05-05 11:28:43.000000 mouse2-0.2.9/mouse2.egg-info/SOURCES.txt
+-rw-rw-r--   0 misha     (2001) misha     (2001)        1 2023-05-05 11:28:43.000000 mouse2-0.2.9/mouse2.egg-info/dependency_links.txt
+-rw-rw-r--   0 misha     (2001) misha     (2001)      286 2023-05-05 11:28:43.000000 mouse2-0.2.9/mouse2.egg-info/entry_points.txt
+-rw-rw-r--   0 misha     (2001) misha     (2001)       43 2023-05-05 11:28:43.000000 mouse2-0.2.9/mouse2.egg-info/requires.txt
+-rw-rw-r--   0 misha     (2001) misha     (2001)       20 2023-05-05 11:28:43.000000 mouse2-0.2.9/mouse2.egg-info/top_level.txt
+drwxrwxr-x   0 misha     (2001) misha     (2001)        0 2023-05-05 11:28:43.369637 mouse2-0.2.9/mouse2_tests/
+-rw-rw-r--   0 misha     (2001) misha     (2001)      260 2023-04-04 09:51:09.000000 mouse2-0.2.9/mouse2_tests/__init__.py
+-rwxrwxr-x   0 misha     (2001) misha     (2001)     6429 2023-05-04 18:31:30.000000 mouse2-0.2.9/mouse2_tests/create_configuration.py
+-rwxrwxr-x   0 misha     (2001) misha     (2001)    17754 2023-05-02 14:45:45.000000 mouse2-0.2.9/mouse2_tests/test_functions.py
+-rw-rw-r--   0 misha     (2001) misha     (2001)       38 2023-05-05 11:28:43.373637 mouse2-0.2.9/setup.cfg
+-rw-rw-r--   0 misha     (2001) misha     (2001)     1567 2023-05-05 11:27:51.000000 mouse2-0.2.9/setup.py
```

### Comparing `mouse2-0.2.8/LICENSE` & `mouse2-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mouse2-0.2.8/PKG-INFO` & `mouse2-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mouse2
-Version: 0.2.8
+Version: 0.2.9
 Summary: A toolkit for processing molecular dynamics simulation data
 Home-page: https://github.com/mglagolev/mouse2
 Author: Mikhail Glagolev, Anna Glagoleva
 Author-email: mikhail.glagolev@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -239,9 +238,7 @@
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Effect of induced self-organization in mixtures of amphiphilic macromolecules with different stiffness // Macromolecules. — 2015. — Vol. 48, no. 11. — P. 3767–3774.
 
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Self-organization of amphiphilic macromolecules with local helix structure in concentrated solutions // Journal of Chemical Physics. — 2012. — Vol. 137, no. 8. - P. 084091.
 
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Formation of fibrillar aggregates in concentrated solutions of rigid-chain amphiphilic macromolecules with fixed torsion and bend angles // Polymer Science, Series A. — 2011. — Vol. 53, no. 8. — P. 733–743.
 
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Compactization of rigid-chain amphiphilic macromolecules with local helical structure // Polymer Science, Series A. — 2010. — Vol. 52, no. 7. — P. 761–774.
-
-
```

### Comparing `mouse2-0.2.8/README.md` & `mouse2-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mouse2-0.2.8/mouse2/aggregates.py` & `mouse2-0.2.9/mouse2/aggregates.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: Mikhail Glagolev
 
 
 """
 
 import MDAnalysis as mda
 import json
-from mouse2.lib.aggregation import determine_aggregates
+from lib.aggregation import determine_aggregates
 
 
 def main():
     
     import argparse
 
     parser = argparse.ArgumentParser(
@@ -45,8 +45,8 @@
     u = mda.Universe(*args.input)
 
     result = determine_aggregates(u, args.r_neigh, args.selection)
     
     print(json.dumps(result, indent = 2))
     
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mouse2-0.2.8/mouse2/backbone_twist.py` & `mouse2-0.2.9/mouse2/backbone_twist.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: Mikhail Glagolev
 """
 
 import numpy as np
 import MDAnalysis as mda
 from MDAnalysis import transformations
 import json
-from mouse2.lib.utilities import normalize_vectors
+from lib.utilities import normalize_vectors
 
 def backbone_twist(u: mda.Universe, k_list: list,
                    selection = None,
                    different_molecules: bool = False):
     """
     Calculate the list of dihedral angles, formed by the following
     vectors: (r_i, r_{i+k}), (r_{i+k}, r_{i+2*k}), (r_{i+2*k}, r_{i+3*k})
@@ -247,8 +247,8 @@
         plt.yticks([0], fontsize = 18)
         plt.xlabel('\u03A8', fontsize = 18)
         plt.ylabel('P(\u03A8), a.u.', fontsize = 18)
         plt.legend(shadow = False, fontsize = 18)
         plt.show()
         
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mouse2-0.2.8/mouse2/bond_autocorrelations.py` & `mouse2-0.2.9/mouse2/bond_autocorrelations.py`

 * *Files identical despite different names*

### Comparing `mouse2-0.2.8/mouse2/data2pdb.py` & `mouse2-0.2.9/mouse2/data2pdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # MOUSE
 # Copyright (c) 2022 Mikhail Glagolev
 #
 # Released under the GNU Public Licence, v2 or any higher version
 
 import argparse
 import MDAnalysis as mda
-from mouse2.lib.utilities import names_from_types
+from lib.utilities import names_from_types
 
 def main():
     """
     This utility reads LAMMPS data file, and writes out the configuration
     in the PDB format
 
     Possible options are:
@@ -46,8 +46,8 @@
         u.delete_bonds(bonds_to_delete)
         
     names_from_types(u)
 
     u.atoms.write(args.output)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mouse2-0.2.8/mouse2/lamellar_alignment.py` & `mouse2-0.2.9/mouse2/lamellar_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @author: Anna Glagoleva, Mikhail Glagolev
 
 """
 
 import MDAnalysis as mda
 import argparse
 import json
-from mouse2.lib.lamellar_orientation import lamellar_alignment
+from lib.lamellar_orientation import lamellar_alignment
 
 
 def main():
     
 
     parser = argparse.ArgumentParser(
         description = """ 
@@ -70,8 +70,8 @@
                                              store_A_values = args.A,
                                              store_B_values = args.B,
                                              store_block_values = args.verbose
                                              )
     print(json.dumps(result, indent = 2))
     
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mouse2-0.2.8/mouse2/lib/aggregation.py` & `mouse2-0.2.9/mouse2/lib/aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 @author: Mikhail Glagolev
 """
 
 import MDAnalysis as mda
 import numpy as np
 import networkx as nx
-from mouse2.lib.neighbor import calculate_neighborlists_from_distances
+from . neighbor import calculate_neighborlists_from_distances
 
 def determine_aggregates(u: mda.Universe, r_neigh: float, selection = None,
-                         ts_indices = None):
+                         ts_indices = None, bonded_as_neighbors = False):
     """
     This function returns a data structure containing list of aggregates
     for all of the timesteps in the MDAnalysis universe.
     Each aggregate is determined as a complete graph of neighbors.
     The atoms are considered neighbors if the distance between their
     centers does not exceed r_neigh.
     Each aggregate is represented as a list of MDAnalysis atom indices.
@@ -79,14 +79,21 @@
         # neighborlists = { atom_index : [neighbor1_index, neighbor2_index, ]}
         neighborlists = calculate_neighborlists_from_distances(atom_indices,
                                                             atom_positions,
                                                             box = u.dimensions,
                                                             r_max = r_neigh)
         #Option 2: use MDAnalysis function to calculate neighbor lists:
     
+        #Add bonded atoms to neighborlists, if necessary:
+        if bonded_as_neighbors:
+            for ix in neighborlists:
+                bonded_indices = [a.index for a in u.atoms[ix].bonded_atoms]
+                neighborlists[ix].append(bonded_indices)
+                neighborlists[ix] = list(set(neighborlists[ix]))
+
         # Initialize a NetworkX graph
         graph = nx.Graph()
         # For every atom add the neighbors to the graph
         for atom_index in neighborlists:
             for neighbor in neighborlists[atom_index]:
                 graph.add_edge(atom_index, neighbor)
         # Convert atom indices to a list
@@ -97,8 +104,8 @@
             aggregate_atoms = nx.dfs_postorder_nodes(graph,
                                                      atom_indices_list[0])
             for atom in aggregate_atoms:
                 aggregate.append(int(atom))
                 atom_indices_list.remove(atom)
             aggregates.append(aggregate)
         data[str(ts)] = aggregates
-    return { "description" : description, "data" : data }
+    return { "description" : description, "data" : data }
```

### Comparing `mouse2-0.2.8/mouse2/lib/lamellar_orientation.py` & `mouse2-0.2.9/mouse2/lib/lamellar_orientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """
 
 
 import numpy as np
 import MDAnalysis as mda
 from MDAnalysis import transformations
-from mouse2.lib.utilities import normalize_vectors
+from . utilities import normalize_vectors
 
 
 def normal_vector(dir_vectors):
     """
     Calculate the normal vector, as the vector corresponding
     to the largest eigenvalue.
 
@@ -186,8 +186,8 @@
                                               block_B_vectors_normed, lam_norm, 
                                              values["h_B"], values["ave_sk_B"])
             # If requested, store the values for individual B blocks:
             if store_block_values:
                 values["values_sk_B"] = sk_B.tolist()
         data[str(ts)] = values
     return { "description" : "Lamellar ordering parameters Sk, h, Pk, theta",
-             "data": data }
+             "data": data }
```

### Comparing `mouse2-0.2.8/mouse2/lib/neighbor.py` & `mouse2-0.2.9/mouse2/lib/neighbor.py`

 * *Files identical despite different names*

### Comparing `mouse2-0.2.8/mouse2/lib/utilities.py` & `mouse2-0.2.9/mouse2/lib/utilities.py`

 * *Files identical despite different names*

### Comparing `mouse2-0.2.8/mouse2/lib/vector_orientational_ordering.py` & `mouse2-0.2.9/mouse2/lib/vector_orientational_ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Created on Tue Oct 18 14:46:18 2022
 
 @author: Mikhail Glagolev
 """
 
 import numpy as np
-from mouse2.lib.neighbor import neighbor_mask
+from . neighbor import neighbor_mask
 
     
 def calculate_cos_sq_for_reference(
         vector_components: [np.ndarray, np.ndarray, np.ndarray],
         vector_midpoints: [np.ndarray, np.ndarray, np.ndarray],
         ref_components: np.ndarray(3), ref_midpoint: np.ndarray(3),
         box = [0., 0., 0., 90., 90., 90.], r_min = 0., r_max = -1.,
```

### Comparing `mouse2-0.2.8/mouse2/local_alignment.py` & `mouse2-0.2.9/mouse2/local_alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: Mikhail Glagolev
 """
 
 import MDAnalysis as mda
 from MDAnalysis import transformations
 import numpy as np
-from mouse2.lib.vector_orientational_ordering \
+from lib.vector_orientational_ordering \
     import calculate_cos_sq_for_reference
 import json
 
 def averaged_frequencies_bin_centers(result, frequencies_key, bin_edges_key):
     """
     Return averaged histogram data across the time steps.
     Bin edges are assumed to be the same for all the timesteps.
@@ -336,8 +336,8 @@
         plt.legend(shadow = False, fontsize = 18)
         if args.plot != '-':
             plt.savefig(args.plot)
         else:
             plt.show()
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mouse2-0.2.8/mouse2.egg-info/PKG-INFO` & `mouse2-0.2.9/mouse2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mouse2
-Version: 0.2.8
+Version: 0.2.9
 Summary: A toolkit for processing molecular dynamics simulation data
 Home-page: https://github.com/mglagolev/mouse2
 Author: Mikhail Glagolev, Anna Glagoleva
 Author-email: mikhail.glagolev@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -239,9 +238,7 @@
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Effect of induced self-organization in mixtures of amphiphilic macromolecules with different stiffness // Macromolecules. — 2015. — Vol. 48, no. 11. — P. 3767–3774.
 
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Self-organization of amphiphilic macromolecules with local helix structure in concentrated solutions // Journal of Chemical Physics. — 2012. — Vol. 137, no. 8. - P. 084091.
 
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Formation of fibrillar aggregates in concentrated solutions of rigid-chain amphiphilic macromolecules with fixed torsion and bend angles // Polymer Science, Series A. — 2011. — Vol. 53, no. 8. — P. 733–743.
 
 Glagolev M. K., Vasilevskaya V. V., Khokhlov A. R. Compactization of rigid-chain amphiphilic macromolecules with local helical structure // Polymer Science, Series A. — 2010. — Vol. 52, no. 7. — P. 761–774.
-
-
```

### Comparing `mouse2-0.2.8/mouse2.egg-info/SOURCES.txt` & `mouse2-0.2.9/mouse2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mouse2-0.2.8/mouse2_tests/create_configuration.py` & `mouse2-0.2.9/mouse2_tests/create_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,26 @@
     parser = argparse.ArgumentParser(
         description = 'Create test systems for mouse2 library')
 
     parser.add_argument(
         '--type', metavar = 'TYPE', nargs = 1, type = str,
         help = "system type: [disordered-]rods, [disordered-]helices," +
         " random")
+    
+    parser.add_argument(
+        '--npoly', metavar = 'N', nargs = 1, type = int,
+        help = "degree of polymerization")
+    
+    parser.add_argument(
+        '--nmol', metavar = 'n', nargs = 1, type = int,
+        help = "number of macromolecules")
+    
+    parser.add_argument(
+        '--box', metavar = 'SIZE', nargs = 1, type = float,
+        help = "rectangular simulation cell size")
 
     parser.add_argument(
         'output', metavar = 'FILE', action = "store",
         help = "output file, the format is determined by MDAnalysis based" +
         " on the file extension")
     
     parser.add_argument(
@@ -65,14 +77,18 @@
     
     parser.add_argument(
         '--dihedrals', action = "store_true", help = "Add dihedral angles")
     
     args = parser.parse_args()
     
     system_type = args.type[0]
+    
+    CELL = args.box * 3 + [90, 90, 90]
+    NMOL = args.nmol[0]
+    NPOLY = args.npoly[0]
 
     random.seed(RANDOM_SEED)
 
     u = mda.Universe.empty(NMOL * NPOLY, trajectory = True,
                            atom_resindex = [0,] * NMOL * NPOLY)
 
     u.add_TopologyAttr('type')
```

### Comparing `mouse2-0.2.8/mouse2_tests/test_functions.py` & `mouse2-0.2.9/mouse2_tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 
 @author: Mikhail Glagolev
 """
 
 import unittest
 import MDAnalysis as mda
 import os
+import sys
+parent_dir_name = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(parent_dir_name + '/..')
+import mouse2
 from mouse2.bond_autocorrelations import bond_autocorrelations
 from mouse2.local_alignment import local_alignment
 from mouse2.lib.lamellar_orientation import lamellar_alignment
 from mouse2.backbone_twist import backbone_twist
 import numpy as np
 import csv
+import time
 
 test_dir = absolute_path = os.path.dirname(__file__)
 
 test_file = os.path.join(test_dir, "helical_lamellae.data.gz")
 
 tolerance = 1e-6
 
@@ -371,16 +376,24 @@
     discrepancy = 0.
     for key1 in dict1:
         values1 = np.asarray(dict1[key1])
         values2 = np.asarray(dict2[key1])
         discrepancy = max(discrepancy, np.max(np.abs(values1 - values2)))
     return discrepancy
 
+class TestWithTime(unittest.TestCase):
+    
+    def setUp(self):
+        self.startTime = time.time()
+        
+    def tearDown(self):
+        t = time.time() - self.startTime
+        print('%s: %.3f' % (self.id(), t))
 
-class TestAutocorrelations(unittest.TestCase):
+class TestAutocorrelations(TestWithTime):
     
     def check_autocorrelations(self, target):
         test_file = target["test_file"]
         k_max = target["k_max"]
         selection = target["selection"]
         different_molecules = target["different_molecules"]
         target_data = target["data"]
@@ -402,15 +415,15 @@
         self.check_autocorrelations(bond_autocorr_tgt["disordered_helices"])
         
     def test_disordered_helices_different_mol(self):
         self.check_autocorrelations(
                        bond_autocorr_tgt["disordered_helices_different_mol"])
 
      
-class TestLocalAlignment(unittest.TestCase):
+class TestLocalAlignment(TestWithTime):
     
     def check_local_alignment(self, target):
         test_file = target["test_file"]
         r_min = target["r_min"]
         r_max = target["r_max"]
         mode = target["mode"]
         n_bins = target["n_bins"]
@@ -445,15 +458,15 @@
                                 local_alignment_tgt["lamellae_helical_lists"])
         
     def test_lamellae_flexible_from_list(self):
         self.check_local_alignment(
                                 local_alignment_tgt["lamellae_flexible_lists"])
         
 
-class TestLamellarAlignment(unittest.TestCase):
+class TestLamellarAlignment(TestWithTime):
     
     def check_lamellar_alignment(self, target):
         test_file = target["test_file"]
         block_A = target["block_A"]
         block_B = target["block_B"]
         target_data = target["data"]
         u = mda.Universe(test_file)
@@ -463,15 +476,15 @@
         assert discrepancy <= tolerance
     
     def test_helical_lamellae(self):
         self.check_lamellar_alignment(
                             lamellar_alignment_tgt["helical_lamellae"])
 
 
-class TestBackboneTwist(unittest.TestCase):
+class TestBackboneTwist(TestWithTime):
     
     def check_backbone_twist(self, target):
         test_file = target["test_file"]
         k_list = target["k_list"]
         selection = target["selection"]
         target_data = target["data"]
         u = mda.Universe(test_file)
@@ -481,8 +494,8 @@
         assert discrepancy <= tolerance
         
     def test_twisted_dumbbell(self):
         self.check_backbone_twist(backbone_twist_tgt["twisted_dumbbell"])
 
         
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

### Comparing `mouse2-0.2.8/setup.py` & `mouse2-0.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mouse2',
-    version='0.2.8',    
+    version='0.2.9',    
     description="""A toolkit for processing molecular dynamics simulation data
     with a focus on chiral ordering""",
     url='https://github.com/mglagolev/mouse2',
     author='Mikhail Glagolev, Anna Glagoleva',
     author_email='mikhail.glagolev@gmail.com',
     license='GNU GPL v3',
     packages=['mouse2', 'mouse2.lib', 'mouse2_tests'],
```

