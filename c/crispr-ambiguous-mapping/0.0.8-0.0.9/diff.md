# Comparing `tmp/crispr_ambiguous_mapping-0.0.8.tar.gz` & `tmp/crispr_ambiguous_mapping-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_ambiguous_mapping-0.0.8.tar", max compression
+gzip compressed data, was "crispr_ambiguous_mapping-0.0.9.tar", max compression
```

## Comparing `crispr_ambiguous_mapping-0.0.8.tar` & `crispr_ambiguous_mapping-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       71 2023-03-31 03:00:16.391603 crispr_ambiguous_mapping-0.0.8/crispr_ambiguous_mapping/__init__.py
--rw-r--r--   0        0        0    21530 2023-03-31 22:42:19.105439 crispr_ambiguous_mapping-0.0.8/crispr_ambiguous_mapping/framework/CrisprAmbiguousMapping.py
--rw-r--r--   0        0        0      507 2023-03-31 22:42:32.950959 crispr_ambiguous_mapping-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 20:10:36.908563 crispr_ambiguous_mapping-0.0.8/README.md
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 crispr_ambiguous_mapping-0.0.8/setup.py
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 crispr_ambiguous_mapping-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-03-31 03:00:16.391603 crispr_ambiguous_mapping-0.0.9/crispr_ambiguous_mapping/__init__.py
+-rw-r--r--   0        0        0    34395 2023-04-03 03:19:54.804747 crispr_ambiguous_mapping-0.0.9/crispr_ambiguous_mapping/framework/CrisprAmbiguousMapping.py
+-rw-r--r--   0        0        0      507 2023-04-03 03:20:13.082379 crispr_ambiguous_mapping-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-30 20:10:36.908563 crispr_ambiguous_mapping-0.0.9/README.md
+-rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 crispr_ambiguous_mapping-0.0.9/setup.py
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 crispr_ambiguous_mapping-0.0.9/PKG-INFO
```

### Comparing `crispr_ambiguous_mapping-0.0.8/crispr_ambiguous_mapping/framework/CrisprAmbiguousMapping.py` & `crispr_ambiguous_mapping-0.0.9/crispr_ambiguous_mapping/framework/CrisprAmbiguousMapping.py`

 * *Files 22% similar despite different names*

```diff
@@ -253,14 +253,120 @@
             "num_matches": len(whitelist_guide_sequences_series_match),
             "matches": whitelist_guide_sequences_series_match,
             "hamming_min": 0}
         else:
             return GuideCountError.MULTIPLE_MATCH
         #raise Exception("Multiple exact matches of the provided whitelisted guides - there are likely duplicates in the provided whitelist, please remove. Observed guide={}, guide matches={}".format(observed_guide_sequence, guide_sequences_series_match)) # NOTE 12/6/22: REMOVED THIS EXCEPTION - another reason is from truncated guides having multiple matches. In production code, just make sure to ensure that the whitelist is the set.
 
+@typechecked
+def infer_true_reporters(observed_reporter_sequences: Tuple[str, str, str], whitelist_guide_reporter_df: pd.DataFrame,
+encoded_whitelist_guide_sequences_series, encoded_whitelist_barcodes_series, barcode_hamming_threshold: int = 2, hamming_threshold: int = 4, verbose_result = False):
+    for element in observed_reporter_sequences:
+        if (element is None) or (element == "None") or (element == ""):
+            if verbose_result:
+                return {"Error": GuideCountError.NO_MATCH, "message": "Observed protospacer/surrogate/barcode is None"}
+            else:
+                return GuideCountError.NO_MATCH
+    
+    observed_reporter_sequences = pd.Series(observed_reporter_sequences, index=["protospacer", "surrogate", "barcode"])
+    
+    # Check if the observed protospacer length is the same length of the whitelisted guides
+    if len(observed_reporter_sequences["protospacer"]) != encoded_whitelist_guide_sequences_series.shape[1]: 
+        if verbose_result:
+            return {"Error": GuideCountError.NO_MATCH, "message": f"Observed protospacer {observed_reporter_sequences['protospacer']} not of correct length: {encoded_whitelist_guide_sequences_series.shape[1]}"}
+        else:
+            return GuideCountError.NO_MATCH
+    if len(observed_reporter_sequences["barcode"]) != encoded_whitelist_barcodes_series.shape[1]: 
+        if verbose_result:
+            return {"Error": GuideCountError.NO_MATCH, "message": f"Observed barcode {observed_reporter_sequences['barcode']} not of correct length: {encoded_whitelist_barcodes_series.shape[1]}"}
+        else:
+            return GuideCountError.NO_MATCH   
+            
+    # Determine if there are exact matches, hopefully just a single match
+    whitelist_guide_reporter_df_match = whitelist_guide_reporter_df[(whitelist_guide_reporter_df["protospacer"]==observed_reporter_sequences["protospacer"]) & (whitelist_guide_reporter_df["surrogate"]==observed_reporter_sequences["surrogate"]) & (whitelist_guide_reporter_df["barcode"]==observed_reporter_sequences["barcode"])] #whitelist_guide_sequences_series == observed_guide_sequence
+    
+    # If there is a single exact match, great, no need for fancy mat
+    if whitelist_guide_reporter_df_match.shape[0] == 1: # Exact match found, return
+        return tuple(whitelist_guide_reporter_df_match.iloc[0])
+    
+    # If no matches, possible a self-edit or a sequencing error, try and find guide with lowest hamming distance
+    elif whitelist_guide_reporter_df_match.shape[0] == 0: # No match found, search based on hamming distance
+        
+        
+        ###
+        ### FILTER BY BARCODE (NOTE: 4/2/23: This is the main difference with the traditional filtering by protospacer)
+        ### TODO 4/2/23: Assumes perfect barcode match, but in the future I can also select for barcodes of 1 hamming - 2 hamming if there is no matches with 0 hamming
+        ###
+        observed_barcode_encoded = encode_DNA_base_vectorized(numpify_string_vectorized(observed_reporter_sequences["barcode"])) 
+        observed_barcode_dists = retrieve_hamming_distance_whitelist(observed_barcode_encoded, encoded_whitelist_barcodes_series)
+        barcode_hamming_min = observed_barcode_dists.min()
+        if barcode_hamming_min >= barcode_hamming_threshold:
+            if verbose_result:
+                return {"Error": GuideCountError.NO_MATCH, "barcode_hamming_min": barcode_hamming_min, "message": f"No barcode below threshold {barcode_hamming_threshold}"}
+            else:
+                return GuideCountError.NO_MATCH
+            
+        barcode_matches_indices = np.where(observed_barcode_dists == barcode_hamming_min)[0]
+        
+        whitelist_guide_reporter_df_barcode = whitelist_guide_reporter_df.iloc[barcode_matches_indices]
+        encoded_whitelist_guide_sequences_series_barcode = encoded_whitelist_guide_sequences_series[barcode_matches_indices]
+        ###
+        ### Now do similar as before
+        ###
+
+        
+        # Encode the observed guide
+        observed_guide_sequence_encoded = encode_DNA_base_vectorized(numpify_string_vectorized(observed_reporter_sequences["protospacer"])) 
+        
+        # Calculate the hamming distance of the guide with all whitelisted guides - vectorized operation
+        observed_guide_sequence_dists = retrieve_hamming_distance_whitelist(observed_guide_sequence_encoded, encoded_whitelist_guide_sequences_series_barcode)
+        
+        # Get the minimum hamming distance calculated
+        hamming_min = observed_guide_sequence_dists.min()
+        
+        # Get all whitelisted guides with the minimum hamming distance (could be multiple)
+        reporters_with_hamming_min_df = whitelist_guide_reporter_df_barcode.iloc[np.where(observed_guide_sequence_dists == hamming_min)[0]]
+        
+        # If the minimum hamming distance is greater than the specified threshold, then the guide is too ambigious to assign, so no match.
+        if hamming_min >= hamming_threshold:
+            if verbose_result:
+                return {"Error": GuideCountError.NO_MATCH, "hamming_min": hamming_min}
+            else:
+                return GuideCountError.NO_MATCH
+        
+        # If there are multiple guides with the minimum hamming distance, then the guide is ambigious, so no mapping (due to multiple match)
+        # NOTE (3/30/2023): This could potentially be an issue with igRNAs maybe?
+        elif reporters_with_hamming_min_df.shape[0] > 1:
+            if verbose_result:
+                return {"Error": GuideCountError.MULTIPLE_MATCH,
+                "exact_match": False, 
+                "num_matches": reporters_with_hamming_min_df.shape[0],
+                "matches": reporters_with_hamming_min_df,
+                "hamming_min": hamming_min}
+            else:
+                return GuideCountError.MULTIPLE_MATCH
+        
+        # Else if there is 1 guide with the match, then return the match
+        else:
+            return tuple(reporters_with_hamming_min_df.iloc[0])
+    
+    # Else if there are multiple exact match, which should never occur unless the whitelisted guide list is not unique, then return multiple match.
+    else:
+        
+        if verbose_result:
+            return {"Error": GuideCountError.MULTIPLE_MATCH,
+            "exact_match": True, 
+            "num_matches": whitelist_guide_reporter_df_match.shape[0],
+            "matches": whitelist_guide_reporter_df_match,
+            "hamming_min": 0}
+        else:
+            return GuideCountError.MULTIPLE_MATCH
+        #raise Exception("Multiple exact matches of the provided whitelisted guides - there are likely duplicates in the provided whitelist, please remove. Observed guide={}, guide matches={}".format(observed_guide_sequence, guide_sequences_series_match)) # NOTE 12/6/22: REMOVED THIS EXCEPTION - another reason is from truncated guides having multiple matches. In production code, just make sure to ensure that the whitelist is the set.
+
+     
 '''
     This performs simulation of determining how many mutations it takes for a guide to be ambigiously mapped based on hamming distance.
 
     This is performed on *sample_count* number of randomly selected guides, and the distribution of mutation count is determined. The 5% quantile is used as the threshold.
     
     This is useful in determing the ideal hamming distance threshold specific to a guide library
 '''
@@ -363,58 +469,135 @@
     whitelist_guide_sequences_series_counts = whitelist_guide_sequences_series.apply(lambda guide: inferred_guide_sequence_counter[guide])
     whitelist_guide_sequences_series_counts.index = whitelist_guide_sequences_series
     
     qc_dict = {"guide_sequences_unassigned_counts":observed_guides_df_no_match.sum(), "guide_sequences_multiple_counts": observed_guides_df_multiple_match.sum(), "total_guide_counts": observed_guides_df["observed_counts"].sum(), "percent_mapped": percent_mapped}
     
     return whitelist_guide_sequences_series_counts, observed_guides_df, qc_dict
 
+@typechecked
+def get_reporter_counts(observed_guide_reporters_counts: Counter, whitelist_guide_reporter_df: pd.DataFrame, barcode_hamming_threshold_strict: int = 2, hamming_threshold_strict: int = 4, hamming_threshold_dynamic: bool = False, cores: int=1):
+
+    whitelist_guide_reporter_df.index = whitelist_guide_reporter_df["protospacer"]
+    
+    # Create observed guide DF to contain all information
+    # The "observed sequence" column represents all *unique* observed sequences that may have self-edits/errors. The "observed counts" column represents the count of each observed count.
+    observed_guides_df = pd.DataFrame({"observed_sequence":observed_guide_reporters_counts.keys(), "observed_counts":observed_guide_reporters_counts.values()})
+ 
+    # Get the hamming distance threshold. THe hamming distance must be below this threshold to assign an observed guide to a whitelist guide.
+    encoded_whitelist_guide_sequences_series = encode_guide_series(whitelist_guide_reporter_df["protospacer"])
+    encoded_whitelist_barcodes_series = encode_guide_series(whitelist_guide_reporter_df["barcode"])
+    
+    if hamming_threshold_dynamic:
+        hamming_threshold = int(determine_hamming_threshold(whitelist_guide_reporter_df["protospacer"], encoded_whitelist_guide_sequences_series, sample_count = 100, quantile = 0.05))
+        print("Hamming threshold is " + str(hamming_threshold))
+    else:
+        hamming_threshold = hamming_threshold_strict
+        
+    # Infer whitelist guides from observed guides
+    print("Inferring the true guides from observed guides")
+
+    infer_true_reporters_p = partial(infer_true_reporters,
+            whitelist_guide_reporter_df=whitelist_guide_reporter_df,
+            encoded_whitelist_guide_sequences_series=encoded_whitelist_guide_sequences_series,
+            encoded_whitelist_barcodes_series=encoded_whitelist_barcodes_series,
+            hamming_threshold=hamming_threshold, barcode_hamming_threshold=barcode_hamming_threshold_strict, verbose_result=False)
+
+    inferred_true_reporter_sequences = None
+    if cores > 1:
+        with Pool(cores) as pool:
+            inferred_true_reporter_sequences = pool.map(
+            infer_true_reporters_p,
+            observed_guides_df["observed_sequence"]
+           )
+    else:
+        inferred_true_reporter_sequences = [infer_true_reporters_p(obs_reporter) for obs_reporter in observed_guides_df["observed_sequence"]]
+    
+    print("Completed inference")
+
+    observed_guides_df["inferred_guides"] = inferred_true_reporter_sequences
+    
+    '''
+        QC
+    '''
+    # QC: Determine the number of guides passed by determining that the result is not an error
+    observed_guides_df_passed_inference = observed_guides_df[observed_guides_df["inferred_guides"].apply(lambda guide : type(guide) != GuideCountError)]
+    # QC: Calculate number of guides that were unassigned
+    observed_guides_df_no_match = observed_guides_df[observed_guides_df["inferred_guides"].apply(lambda guide : guide == GuideCountError.NO_MATCH)]
+    # QC: Calculate number of guides with multiple inferred guides
+    observed_guides_df_multiple_match = observed_guides_df[observed_guides_df["inferred_guides"].apply(lambda guide : guide == GuideCountError.MULTIPLE_MATCH)]
+    # QC: Calculate percent mapped
+    percent_mapped = observed_guides_df_passed_inference["observed_counts"].sum()/observed_guides_df["observed_counts"].sum()
+    
+    # Retrieve the observed sequences that were mapped and set the inferred guides
+    inferred_guide_sequence_counter = Counter()
+    for _, row in observed_guides_df_passed_inference.iterrows():
+        inferred_guide_sequence_counter[row["inferred_guides"]] += row["observed_counts"]
+    
+    whitelist_guide_reporter_counts = whitelist_guide_reporter_df.apply(lambda reporter: inferred_guide_sequence_counter[tuple(reporter)], axis=1)
+    multi_index = pd.MultiIndex.from_arrays([whitelist_guide_reporter_df['protospacer'], whitelist_guide_reporter_df['surrogate'], whitelist_guide_reporter_df['barcode']], names=['protospacer', 'surrogate', 'barcode'])
+    whitelist_guide_reporter_counts.index = multi_index
+    
+    qc_dict = {"guide_sequences_unassigned_counts":observed_guides_df_no_match.sum(), "guide_sequences_multiple_counts": observed_guides_df_multiple_match.sum(), "total_guide_counts": observed_guides_df["observed_counts"].sum(), "percent_mapped": percent_mapped}
+    
+    return whitelist_guide_reporter_counts, observed_guides_df, qc_dict
+
 
 
 ###
 ### Read in sequences from a pre-parsed reporter file
 ### 
 import csv
 import multiprocessing as mp
 from collections import Counter
 from functools import reduce
 
-
 def gen_chunks(reader, chunksize=1000):
     """
     Chunk generator. Take a CSV `reader` and yield
     `chunksize` sized slices.
     Source: https://gist.github.com/miku/820490
     """
     chunk = []
     for index, line in enumerate(reader):
         if index % chunksize == 0 and index > 0:
             yield chunk
             chunk = []
         chunk.append(line)
     yield chunk
 
-
-def process(tsv_chunk):
+def process(tsv_chunk, include_surrogate = False):
     local_counter = Counter()
     
     for row in tsv_chunk.copy():
-        local_counter[row[1]] += 1
+        if include_surrogate:
+            local_counter[(row[1], row[2], row[3])] += 1
+        else:
+            local_counter[row[1]] += 1
     
     return local_counter
 
 
-def map_sample_protospacers(parsing_demult_handler, cores=1):
+@typechecked
+def map_sample_protospacers(parsing_demult_handler, include_surrogate = False, cores=1):
     tsv_reader = csv.reader(parsing_demult_handler, delimiter='\t')  # change delimiter for normal csv files
     header = next(tsv_reader)
       
     read_chunks = gen_chunks(tsv_reader, chunksize=10000)
-    with mp.Pool(processes=cores) as pool:
-        chunk_counters = pool.map(process, read_chunks)
+
+    process_func = partial(process, include_surrogate=include_surrogate)
+
+    combined_counter = None
+    if cores > 1:
+        with mp.Pool(processes=cores) as pool:
+            chunk_counters = pool.map(process_func, read_chunks)
+            combined_counter = reduce(lambda x, y: x + y, chunk_counters)
+    else:
+        chunk_counters = [process_func(read_chunk) for read_chunk in read_chunks]
         combined_counter = reduce(lambda x, y: x + y, chunk_counters)
-    
+
     return combined_counter 
 
 
 ###
 ### MAIN FUNCTIONS
 ###
 
@@ -440,8 +623,15 @@
 def get_guide_counts_from_reporter_tsv(whitelist_guide_sequences_series: pd.Series, reporter_tsv_fn: str, hamming_threshold_strict: int = 3, hamming_threshold_dynamic: bool = False, cores: int=1):
     combined_counter = None
     with open(reporter_tsv_fn, "r", newline='') as reporter_tsv_handler:
         combined_counter = map_sample_protospacers(reporter_tsv_handler, cores)
 
     return get_guide_counts(combined_counter, whitelist_guide_sequences_series, hamming_threshold_strict, hamming_threshold_dynamic, cores)
 
+@typechecked
+def get_reporter_counts_from_reporter_tsv(whitelist_guide_reporter_df: pd.DataFrame, reporter_tsv_fn: str, barcode_hamming_threshold_strict: int = 2, hamming_threshold_strict: int = 3, hamming_threshold_dynamic: bool = False, cores: int=1):
+    
+    combined_counter = None
+    with open(reporter_tsv_fn, "r", newline='') as reporter_tsv_handler:
+        combined_counter = map_sample_protospacers(reporter_tsv_handler, include_surrogate = True, cores=cores)
 
+    return get_reporter_counts(observed_guide_reporters_counts=combined_counter, whitelist_guide_reporter_df=whitelist_guide_reporter_df, barcode_hamming_threshold_strict=barcode_hamming_threshold_strict, hamming_threshold_strict=hamming_threshold_strict, hamming_threshold_dynamic=hamming_threshold_dynamic, cores=cores)
```

### Comparing `crispr_ambiguous_mapping-0.0.8/setup.py` & `crispr_ambiguous_mapping-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pandarallel>=1.6.4,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
  'scipy>=1.10.1,<2.0.0',
  'typeguard>=3.0.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'crispr-ambiguous-mapping',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': '',
     'author': 'Basheer Becerra',
     'author_email': 'bbecerr@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `crispr_ambiguous_mapping-0.0.8/PKG-INFO` & `crispr_ambiguous_mapping-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crispr-ambiguous-mapping
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Basheer Becerra
 Author-email: bbecerr@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

