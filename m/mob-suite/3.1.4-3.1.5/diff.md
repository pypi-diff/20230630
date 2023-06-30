# Comparing `tmp/mob_suite-3.1.4.tar.gz` & `tmp/mob_suite-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mob_suite-3.1.4.tar", last modified: Mon Feb  6 20:19:49 2023, max compression
+gzip compressed data, was "mob_suite-3.1.5.tar", last modified: Fri Jun 30 15:46:56 2023, max compression
```

## Comparing `mob_suite-3.1.4.tar` & `mob_suite-3.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.820010 mob_suite-3.1.4/
--rw-r--r--   0 jrobertson   (502) staff       (20)    11358 2023-01-24 14:20:49.000000 mob_suite-3.1.4/LICENSE
--rw-r--r--   0 jrobertson   (502) staff       (20)      168 2023-01-24 14:20:49.000000 mob_suite-3.1.4/MANIFEST.in
--rw-r--r--   0 jrobertson   (502) staff       (20)     1000 2023-02-06 20:19:49.819122 mob_suite-3.1.4/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)    18441 2023-01-24 14:20:49.000000 mob_suite-3.1.4/README.md
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.789429 mob_suite-3.1.4/mob_suite/
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/__init__.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.794610 mob_suite-3.1.4/mob_suite/blast/
--rw-r--r--   0 jrobertson   (502) staff       (20)     7580 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/blast/__init__.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.795524 mob_suite-3.1.4/mob_suite/classes/
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/classes/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)      111 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/config.json
--rw-r--r--   0 jrobertson   (502) staff       (20)     3974 2023-01-25 20:29:56.000000 mob_suite-3.1.4/mob_suite/constants.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.795988 mob_suite-3.1.4/mob_suite/databases/
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-01-25 21:13:28.000000 mob_suite-3.1.4/mob_suite/databases/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    24351 2023-01-25 19:37:23.000000 mob_suite-3.1.4/mob_suite/mob_cluster.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     9509 2023-01-25 19:40:04.000000 mob_suite-3.1.4/mob_suite/mob_init.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    63437 2023-02-06 20:18:15.000000 mob_suite-3.1.4/mob_suite/mob_recon.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    25791 2023-01-25 21:01:24.000000 mob_suite-3.1.4/mob_suite/mob_typer.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.798390 mob_suite-3.1.4/mob_suite/tests/
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.815376 mob_suite-3.1.4/mob_suite/tests/TestData/
--rw-r--r--   0 jrobertson   (502) staff       (20)     3441 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/TestData/AB011548.fasta
--rw-r--r--   0 jrobertson   (502) staff       (20)    50310 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/TestData/AB040415.fasta
--rw-r--r--   0 jrobertson   (502) staff       (20)     5003 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/TestData/AY603981.fasta
--rw-r--r--   0 jrobertson   (502) staff       (20)    89320 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/TestData/KU295134.fasta
--rw-r--r--   0 jrobertson   (502) staff       (20)    58186 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/TestData/KX377410.fasta
--rw-r--r--   0 jrobertson   (502) staff       (20)    76764 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/TestData/NC_011385.1.fasta
--rw-r--r--   0 jrobertson   (502) staff       (20)   253464 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/TestData/pCAV1453-208.fasta
--rw-r--r--   0 jrobertson   (502) staff       (20)     3187 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/test_mob_init.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     1062 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/test_mobrecon.py
--rw-r--r--   0 jrobertson   (502) staff       (20)      715 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/tests/test_mobtyper.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    53916 2023-01-25 21:02:32.000000 mob_suite-3.1.4/mob_suite/utils.py
--rw-r--r--   0 jrobertson   (502) staff       (20)       23 2023-02-06 20:19:01.000000 mob_suite-3.1.4/mob_suite/version.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.818111 mob_suite-3.1.4/mob_suite/wrappers/
--rw-r--r--   0 jrobertson   (502) staff       (20)     5716 2023-01-24 14:20:49.000000 mob_suite-3.1.4/mob_suite/wrappers/__init__.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-02-06 20:19:49.793940 mob_suite-3.1.4/mob_suite.egg-info/
--rw-r--r--   0 jrobertson   (502) staff       (20)     1000 2023-02-06 20:19:49.000000 mob_suite-3.1.4/mob_suite.egg-info/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)      945 2023-02-06 20:19:49.000000 mob_suite-3.1.4/mob_suite.egg-info/SOURCES.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)        1 2023-02-06 20:19:49.000000 mob_suite-3.1.4/mob_suite.egg-info/dependency_links.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)      169 2023-02-06 20:19:49.000000 mob_suite-3.1.4/mob_suite.egg-info/entry_points.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)      141 2023-02-06 20:19:49.000000 mob_suite-3.1.4/mob_suite.egg-info/requires.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       10 2023-02-06 20:19:49.000000 mob_suite-3.1.4/mob_suite.egg-info/top_level.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       38 2023-02-06 20:19:49.820227 mob_suite-3.1.4/setup.cfg
--rw-r--r--   0 jrobertson   (502) staff       (20)     2004 2023-02-06 20:19:11.000000 mob_suite-3.1.4/setup.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.744459 mob_suite-3.1.5/
+-rw-r--r--   0 jrobertson   (502) staff       (20)    11358 2023-06-30 15:41:56.000000 mob_suite-3.1.5/LICENSE
+-rw-r--r--   0 jrobertson   (502) staff       (20)      168 2023-06-30 15:41:56.000000 mob_suite-3.1.5/MANIFEST.in
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1000 2023-06-30 15:46:56.744019 mob_suite-3.1.5/PKG-INFO
+-rw-r--r--   0 jrobertson   (502) staff       (20)    18441 2023-06-30 15:41:56.000000 mob_suite-3.1.5/README.md
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.706009 mob_suite-3.1.5/mob_suite/
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/__init__.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.713383 mob_suite-3.1.5/mob_suite/blast/
+-rw-r--r--   0 jrobertson   (502) staff       (20)     7580 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/blast/__init__.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.714627 mob_suite-3.1.5/mob_suite/classes/
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/classes/__init__.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)      111 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/config.json
+-rw-r--r--   0 jrobertson   (502) staff       (20)     3974 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/constants.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.715246 mob_suite-3.1.5/mob_suite/databases/
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/databases/__init__.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    24946 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/mob_cluster.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     9509 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/mob_init.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    63437 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/mob_recon.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    25806 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/mob_typer.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.718011 mob_suite-3.1.5/mob_suite/tests/
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.735950 mob_suite-3.1.5/mob_suite/tests/TestData/
+-rw-r--r--   0 jrobertson   (502) staff       (20)     3441 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/TestData/AB011548.fasta
+-rw-r--r--   0 jrobertson   (502) staff       (20)    50310 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/TestData/AB040415.fasta
+-rw-r--r--   0 jrobertson   (502) staff       (20)     5003 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/TestData/AY603981.fasta
+-rw-r--r--   0 jrobertson   (502) staff       (20)    89320 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/TestData/KU295134.fasta
+-rw-r--r--   0 jrobertson   (502) staff       (20)    58186 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/TestData/KX377410.fasta
+-rw-r--r--   0 jrobertson   (502) staff       (20)    76764 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/TestData/NC_011385.1.fasta
+-rw-r--r--   0 jrobertson   (502) staff       (20)   253464 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/TestData/pCAV1453-208.fasta
+-rw-r--r--   0 jrobertson   (502) staff       (20)     3187 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/test_mob_init.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1062 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/test_mobrecon.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)      715 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/tests/test_mobtyper.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    54207 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/utils.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)       23 2023-06-30 15:43:52.000000 mob_suite-3.1.5/mob_suite/version.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.743117 mob_suite-3.1.5/mob_suite/wrappers/
+-rw-r--r--   0 jrobertson   (502) staff       (20)     5716 2023-06-30 15:41:56.000000 mob_suite-3.1.5/mob_suite/wrappers/__init__.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-06-30 15:46:56.712489 mob_suite-3.1.5/mob_suite.egg-info/
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1000 2023-06-30 15:46:56.000000 mob_suite-3.1.5/mob_suite.egg-info/PKG-INFO
+-rw-r--r--   0 jrobertson   (502) staff       (20)      945 2023-06-30 15:46:56.000000 mob_suite-3.1.5/mob_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)        1 2023-06-30 15:46:56.000000 mob_suite-3.1.5/mob_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)      199 2023-06-30 15:46:56.000000 mob_suite-3.1.5/mob_suite.egg-info/entry_points.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)      140 2023-06-30 15:46:56.000000 mob_suite-3.1.5/mob_suite.egg-info/requires.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       10 2023-06-30 15:46:56.000000 mob_suite-3.1.5/mob_suite.egg-info/top_level.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       38 2023-06-30 15:46:56.744743 mob_suite-3.1.5/setup.cfg
+-rw-r--r--   0 jrobertson   (502) staff       (20)     2048 2023-06-30 15:43:42.000000 mob_suite-3.1.5/setup.py
```

### Comparing `mob_suite-3.1.4/LICENSE` & `mob_suite-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/PKG-INFO` & `mob_suite-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mob_suite
-Version: 3.1.4
+Version: 3.1.5
 Summary: MOB-suite is a set of tools for finding, typing and reconstruction of plasmids from draft and complete genome assemblies.
 Home-page: https://github.com/phac-nml/mob-suite
 Author: James Robertson
 Author-email: james.robertson@canada.ca
 License: GPLv3
 Keywords: Plasmids finding typing reconstruction
 Platform: UNKNOWN
```

### Comparing `mob_suite-3.1.4/README.md` & `mob_suite-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/blast/__init__.py` & `mob_suite-3.1.5/mob_suite/blast/__init__.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/constants.py` & `mob_suite-3.1.5/mob_suite/constants.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/mob_cluster.py` & `mob_suite-3.1.5/mob_suite/mob_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     read_file_to_dict, \
     read_fasta_dict, \
     NamesToTaxIDs
 
 from mob_suite.wrappers import mash
 
 from mob_suite.constants import LOG_FORMAT, ACS_LETTER_VALUES, ACS_FORMAT_VALUES, ACS_VALUES_TO_LETTERS, MAX_ACS_VALUE, \
-    MOB_TYPER_REPORT_HEADER, MOB_CLUSTER_INFO_HEADER
+    MOB_TYPER_REPORT_HEADER, MOB_CLUSTER_INFO_HEADER, default_database_dir
 
 
 def init_console_logger(lvl):
     logging_levels = [logging.ERROR, logging.WARN, logging.INFO, logging.DEBUG]
     report_lvl = logging_levels[lvl]
 
     logging.basicConfig(format=LOG_FORMAT, level=report_lvl)
@@ -43,14 +43,20 @@
     parser.add_argument('-t', '--taxonomy', type=str, required=True,
                         help='TSV file for new sequences with the fields "id, organism"')
     parser.add_argument('-o', '--outdir', type=str, required=True, help='Output Directory to put results')
     parser.add_argument('-c', '--ref_cluster_file', type=str, required=False,
                         help='Existing MOB-cluster file to add the new sequences to')
     parser.add_argument('-r', '--ref_fasta_file', type=str, required=False,
                         help='Existing MOB-cluster fasta file of sequences contained in the MOB-cluster file')
+    parser.add_argument('-d', '--database_directory',
+                        default=default_database_dir,
+                        required=False,
+                        help='Directory you want to use for your databases. If the databases are not already '
+                             'downloaded, they will be downloaded automatically. Defaults to {}'.format(
+                            default_database_dir))
     parser.add_argument('--num_threads', type=int, required=False, help='Number of threads to be used', default=1)
     parser.add_argument('--primary_cluster_dist', type=float, required=False,
                         help='Mash distance for assigning primary cluster id 0 - 1', default=0.06)
     parser.add_argument('--secondary_cluster_dist', type=float, required=False,
                         help='Mash distance for assigning primary cluster id 0 - 1', default=0.025)
     parser.add_argument('--debug', required=False, help='Show debug information', action='store_true')
     parser.add_argument('-V', '--version', action='version', version="%(prog)s " + __version__)
@@ -490,14 +496,15 @@
         os.makedirs(out_dir, 0o755)
     tmp_dir = os.path.join(out_dir, '__tmp')
     if not os.path.isdir(tmp_dir):
         logging.info('Creating directory {}'.format(args.outdir))
         os.makedirs(tmp_dir, 0o755)
 
     taxonomy_file = args.taxonomy
+    database_dir = os.path.abspath(args.database_directory)
 
     records = read_file_to_dict(mob_typer_report_file, MOB_TYPER_REPORT_HEADER, separater="\t")
 
     seq_ids = []
     new_seq_info = {}
     duplicate_keys = []
     for record in records:
@@ -521,15 +528,16 @@
         if organism == 'unknown' or organism == '' or organism == 'Unknown':
             organism = 'Bacteria'
         organisms.append(organism)
         seq_id = record['sample_id']
         if seq_id in new_seq_info:
             new_seq_info[seq_id]['organism'] = organism
 
-    taxids = NamesToTaxIDs(organisms)
+    ETE3DBTAXAFILE = os.path.abspath(database_dir + "/taxa.sqlite")
+    taxids = NamesToTaxIDs(organisms, ETE3DBTAXAFILE, database_dir)
     del(organisms)
 
     for seq_id in new_seq_info:
         organism = new_seq_info[seq_id]['organism']
         if organism in taxids:
             new_seq_info[seq_id]['taxid'] = taxids[organism][0]
         else:
```

### Comparing `mob_suite-3.1.4/mob_suite/mob_init.py` & `mob_suite-3.1.5/mob_suite/mob_init.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/mob_recon.py` & `mob_suite-3.1.5/mob_suite/mob_recon.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/mob_typer.py` & `mob_suite-3.1.5/mob_suite/mob_typer.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
         # Patches that sometimes results are concatonated into strings if contigs are merged into a single results
         if isinstance(record['rep_type(s)'], list):
             record['rep_type(s)'] = ",".join(record['rep_type(s)'])
         if isinstance(record['relaxase_type_accession(s)'], list):
             record['relaxase_type_accession(s)'] = ",".join(record['relaxase_type_accession(s)'])
 
         host_range = hostrange(record['rep_type(s)'].split(','), record['relaxase_type_accession(s)'].split(','),
-                               mob_cluster_id, ncbi, lit,ETE3DBTAXAFILE)
+                               mob_cluster_id, ncbi, lit, ETE3DBTAXAFILE, database_dir)
 
         for field in host_range:
             record[field] = host_range[field]
 
         if isinstance(record['mpf_type'], list):
             record['mpf_type'] = determine_mpf_type(record['mpf_type'])
         elif isinstance(record['mpf_type'], str):
```

### Comparing `mob_suite-3.1.4/mob_suite/tests/TestData/AB011548.fasta` & `mob_suite-3.1.5/mob_suite/tests/TestData/AB011548.fasta`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/TestData/AB040415.fasta` & `mob_suite-3.1.5/mob_suite/tests/TestData/AB040415.fasta`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/TestData/AY603981.fasta` & `mob_suite-3.1.5/mob_suite/tests/TestData/AY603981.fasta`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/TestData/KU295134.fasta` & `mob_suite-3.1.5/mob_suite/tests/TestData/KU295134.fasta`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/TestData/KX377410.fasta` & `mob_suite-3.1.5/mob_suite/tests/TestData/KX377410.fasta`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/TestData/NC_011385.1.fasta` & `mob_suite-3.1.5/mob_suite/tests/TestData/NC_011385.1.fasta`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/TestData/pCAV1453-208.fasta` & `mob_suite-3.1.5/mob_suite/tests/TestData/pCAV1453-208.fasta`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/test_mob_init.py` & `mob_suite-3.1.5/mob_suite/tests/test_mob_init.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/test_mobrecon.py` & `mob_suite-3.1.5/mob_suite/tests/test_mobrecon.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/tests/test_mobtyper.py` & `mob_suite-3.1.5/mob_suite/tests/test_mobtyper.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite/utils.py` & `mob_suite-3.1.5/mob_suite/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,18 +75,18 @@
 
         except ValueError:
             continue
 
     return filtered
 
 
-def getHeirarchy(taxid,ETE3DBTAXAFILE):
+def getHeirarchy(taxid,ETE3DBTAXAFILE,database_directory):
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.info("Did not find taxa.sqlite in {}. Initializaing ete3 taxonomy database".format(ETE3DBTAXAFILE))
-        initETE3Database()
+        initETE3Database(database_directory, ETE3DBTAXAFILE)
 
     ncbi = NCBITaxa(dbfile=ETE3DBTAXAFILE)
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.error(
             "Tried ete3 init, but still was not able to find taxa.sqlite file for ete3 lib in {}. Aborting".format(
                 ETE3DBTAXAFILE))
         return ['-', '-']
@@ -99,53 +99,53 @@
     ranks = []
     for id in lineage:
         ranks.append(ncbi.get_rank(id))
 
     return {'names': names, 'ranks': names}
 
 
-def getTaxid(taxon,ETE3DBTAXAFILE):
+def getTaxid(taxon,ETE3DBTAXAFILE,database_directory):
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.info("Did not find taxa.sqlite in {}. Initializaing ete3 taxonomy database".format(ETE3DBTAXAFILE))
-        initETE3Database()
+        initETE3Database(database_directory, ETE3DBTAXAFILE)
 
     ncbi = NCBITaxa(dbfile=ETE3DBTAXAFILE)
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.error(
             "Tried ete3 init, but still was not able to find taxa.sqlite file for ete3 lib in {}. Aborting".format(
                 ETE3DBTAXAFILE))
         return ['-', '-']
 
     taxid = ncbi.get_name_translator(taxon)
 
     return taxid
 
 
 
-def NamesToTaxIDs(names,ETE3DBTAXAFILE):
+def NamesToTaxIDs(names,ETE3DBTAXAFILE,database_directory):
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.info("Did not find taxa.sqlite in {}. Initializaing ete3 taxonomy database".format(ETE3DBTAXAFILE))
-        initETE3Database(ETE3DBTAXAFILE)
+        initETE3Database(database_directory, ETE3DBTAXAFILE)
 
     ncbi = NCBITaxa(dbfile=ETE3DBTAXAFILE)
 
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.error(
             "Tried ete3 init, but still was not able to find taxa.sqlite file for ete3 lib in {}. Aborting".format(
                 ETE3DBTAXAFILE))
         return {}
 
     return ncbi.get_name_translator(names)
 
 
 
-def getTaxonConvergence(taxids,ETE3DBTAXAFILE):
+def getTaxonConvergence(taxids,ETE3DBTAXAFILE,database_directory):
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.info("Did not find taxa.sqlite in {}. Initializaing ete3 taxonomy database".format(ETE3DBTAXAFILE))
-        initETE3Database(ETE3DBTAXAFILE)
+        initETE3Database(database_directory, ETE3DBTAXAFILE)
 
     ncbi = NCBITaxa(dbfile=ETE3DBTAXAFILE)
 
     if not isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
         logging.error(
             "Tried ete3 init, but still was not able to find taxa.sqlite file for ete3 lib in {}. Aborting".format(
                 ETE3DBTAXAFILE))
@@ -202,15 +202,15 @@
         return ('multi-phylla', ",".join(phylla))
     elif len(phylla) == 1:
         return ('phylum', ",".join(phylla))
 
     return (['-', '-'])
 
 
-def hostrange(replion_types, relaxase_types, mob_cluster_id, ncbi, lit,ETE3DBTAXAFILE):
+def hostrange(replion_types, relaxase_types, mob_cluster_id, ncbi, lit, ETE3DBTAXAFILE, database_directory):
     host_range_predictions = {
         'observed_host_range_ncbi_name': '',
         'observed_host_range_ncbi_rank': '',
         'reported_host_range_lit_name': '',
         'reported_host_range_lit_rank': '',
         'predicted_host_range_overall_name': '',
         'predicted_host_range_overall_rank': '',
@@ -247,33 +247,33 @@
         host_range_predictions['observed_host_range_ncbi_rank'] = '-'
         host_range_predictions['observed_host_range_ncbi_name'] = '-'
         ncbi_unique_taxids = []
     else:
         ncbi_unique_taxids = filter_invalid_taxids(
             list(set(ncbi_replicon_taxids + ncbi_cluster_taxids + ncbi_relaxase_taxids)))
         host_range_predictions['observed_host_range_ncbi_rank'], host_range_predictions[
-            'observed_host_range_ncbi_name'] = getTaxonConvergence(ncbi_unique_taxids,ETE3DBTAXAFILE)
+            'observed_host_range_ncbi_name'] = getTaxonConvergence(ncbi_unique_taxids,ETE3DBTAXAFILE,database_directory)
 
     # Determine taxids associated with literature
 
     lit_unique_taxids = filter_invalid_taxids(list(set(lit_replicon_taxids)))
 
     host_range_predictions['reported_host_range_lit_rank'], host_range_predictions[
-        'reported_host_range_lit_name'] = getTaxonConvergence(lit_unique_taxids,ETE3DBTAXAFILE)
+        'reported_host_range_lit_name'] = getTaxonConvergence(lit_unique_taxids,ETE3DBTAXAFILE,database_directory)
 
     # determine overall host range
     overall_taxids = filter_invalid_taxids(list(set(ncbi_unique_taxids + lit_unique_taxids)))
     host_range_predictions['predicted_host_range_overall_rank'], host_range_predictions[
-        'predicted_host_range_overall_name'] = getTaxonConvergence(overall_taxids,ETE3DBTAXAFILE)
+        'predicted_host_range_overall_name'] = getTaxonConvergence(overall_taxids,ETE3DBTAXAFILE,database_directory)
 
     # move host-range prediction up to family when it is at genus or species level
     if host_range_predictions['predicted_host_range_overall_rank'] == 'genus' or host_range_predictions[
         'predicted_host_range_overall_rank'] == 'species':
-        taxid = getTaxid(host_range_predictions['predicted_host_range_overall_name'],ETE3DBTAXAFILE)
-        heir = getHeirarchy(taxid,ETE3DBTAXAFILE)
+        taxid = getTaxid(host_range_predictions['predicted_host_range_overall_name'],ETE3DBTAXAFILE,database_directory)
+        heir = getHeirarchy(taxid,ETE3DBTAXAFILE,database_directory)
         names = heir['names']
         ranks = heir['ranks']
 
         for i in range(0, len(ranks)):
             if ranks[i] == 'Family':
                 host_range_predictions['predicted_host_range_overall_rank'] = 'family'
                 host_range_predictions['predicted_host_range_overall_name'] = names[i]
@@ -365,15 +365,15 @@
 def isETE3DBTAXAFILEexists(ETE3DBTAXAFILE):
     if not os.path.exists(ETE3DBTAXAFILE):
         return False
     else:
         return True
 
 
-def initETE3Database(database_directory, ETE3DBTAXAFILE, logging):
+def initETE3Database(database_directory, ETE3DBTAXAFILE):
     lockfilepath = os.path.join(database_directory, ".lock")
 
     if os.path.exists(lockfilepath) == False:
         open(file=lockfilepath, mode="w").close()
         logging.info("Placed lock file at {}".format(lockfilepath))
     else:
         while os.path.exists(lockfilepath):
```

### Comparing `mob_suite-3.1.4/mob_suite/wrappers/__init__.py` & `mob_suite-3.1.5/mob_suite/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/mob_suite.egg-info/PKG-INFO` & `mob_suite-3.1.5/mob_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mob-suite
-Version: 3.1.4
+Version: 3.1.5
 Summary: MOB-suite is a set of tools for finding, typing and reconstruction of plasmids from draft and complete genome assemblies.
 Home-page: https://github.com/phac-nml/mob-suite
 Author: James Robertson
 Author-email: james.robertson@canada.ca
 License: GPLv3
 Keywords: Plasmids finding typing reconstruction
 Platform: UNKNOWN
```

### Comparing `mob_suite-3.1.4/mob_suite.egg-info/SOURCES.txt` & `mob_suite-3.1.5/mob_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mob_suite-3.1.4/setup.py` & `mob_suite-3.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 exec(open('mob_suite/version.py').read())
 
 setup(
     name='mob_suite',
     include_package_data=True,
-    version='3.1.4',
+    version='3.1.5',
     python_requires='>=3.7.0,<4',
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     packages=find_packages(exclude=['tests', 'databases']),
     url='https://github.com/phac-nml/mob-suite',
     license='GPLv3',
     author='James Robertson',
@@ -45,23 +45,24 @@
     package_dir={'mob_suite': 'mob_suite'},
     package_data={'mob_suite': ['config.json']},
 
     install_requires=[
         'numpy>=1.11.1,<1.23.5',
         'tables>=3.3.0,<4',
         'pandas>=0.22.0,<=1.0.5',
-        'biopython>=1.70,<2',
+        'biopython>=1.8,<2',
         'pycurl>=7.43.0,<8',
         'scipy>=1.1.0,<2',
         'ete3>=3.0,<4',
         'six>=1.10,<2',
     ],
 
     entry_points={
         'console_scripts': [
+            'Sequenoscope=Sequenoscope:main'
             'mob_init=mob_suite.mob_init:main',
             'mob_recon=mob_suite.mob_recon:main',
             'mob_cluster=mob_suite.mob_cluster:main',
             'mob_typer=mob_suite.mob_typer:main',
         ],
     },
 )
```

