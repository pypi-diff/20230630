# Comparing `tmp/gumpy-1.2.0.tar.gz` & `tmp/gumpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gumpy-1.2.0.tar", last modified: Tue Jun 27 14:55:49 2023, max compression
+gzip compressed data, was "gumpy-1.2.1.tar", last modified: Fri Jun 30 09:23:53 2023, max compression
```

## Comparing `gumpy-1.2.0.tar` & `gumpy-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.593083 gumpy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-27 14:55:02.000000 gumpy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-27 14:55:49.593083 gumpy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-27 14:55:02.000000 gumpy-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 14:55:02.000000 gumpy-1.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.589083 gumpy-1.2.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-06-27 14:55:02.000000 gumpy-1.2.0/bin/gumpy-save-genome.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-06-27 14:55:02.000000 gumpy-1.2.0/bin/to_piezo_catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.593083 gumpy-1.2.0/gumpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51609 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/difference.py
--rw-r--r--   0 runner    (1001) docker     (123)    34067 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/gene.py
--rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/genome.py
--rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-06-27 14:55:02.000000 gumpy-1.2.0/gumpy/variantfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:55:49.593083 gumpy-1.2.0/gumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:55:10.000000 gumpy-1.2.0/gumpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 14:55:49.000000 gumpy-1.2.0/gumpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 14:55:02.000000 gumpy-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-27 14:55:49.593083 gumpy-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-30 09:23:10.000000 gumpy-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 09:23:53.974406 gumpy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-30 09:23:10.000000 gumpy-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 09:23:10.000000 gumpy-1.2.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-06-30 09:23:10.000000 gumpy-1.2.1/bin/gumpy-save-genome.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-06-30 09:23:10.000000 gumpy-1.2.1/bin/to_piezo_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/gumpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34070 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/gene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/variantfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/gumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:23:17.000000 gumpy-1.2.1/gumpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 09:23:10.000000 gumpy-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-30 09:23:53.974406 gumpy-1.2.1/setup.cfg
```

### Comparing `gumpy-1.2.0/LICENSE` & `gumpy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.0/PKG-INFO` & `gumpy-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Genetics with Numpy
 Home-page: https://github.com/oxfordmmm/gumpy
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gumpy-1.2.0/README.md` & `gumpy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.0/bin/gumpy-save-genome.py` & `gumpy-1.2.1/bin/gumpy-save-genome.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.0/bin/to_piezo_catalogue.py` & `gumpy-1.2.1/bin/to_piezo_catalogue.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.0/gumpy/__init__.py` & `gumpy-1.2.1/gumpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.0/gumpy/difference.py` & `gumpy-1.2.1/gumpy/difference.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,22 +151,23 @@
         #Calculate differences
         self._nucleotides_full = self.__nucleotides()
 
         self.__assign_vcf_evidence()
 
         self.update_view(self._view_method)
     
-    def get_gene_pos(self, gene: str, idx: int, variant: str) -> int:
+    def get_gene_pos(self, gene: str, idx: int, variant: str, start :int=None) -> int:
         '''Find the gene position of a given nucleotide index.
         This is considerably faster than building a whole stacked_gene_pos array (takes ~4.5mins for tb)
 
         Args:
             gene (str): Name of the gene to search
             idx (int): Nucleotide index we want the gene position of
             variant (str): Variant we're looking for in GARC
+            start (int): Start position. Defaults to None
 
         Returns:
             int: Gene position of this nucleotide index
         '''
         stacked_gene_mask = self.genome1.stacked_gene_name == gene
         nc_idx = self.genome1.stacked_nucleotide_index[stacked_gene_mask]
         nc_nums = self.genome1.stacked_nucleotide_number[stacked_gene_mask]
@@ -180,18 +181,23 @@
             codon_number = (nc_num + 2) // 3
             return codon_number
         elif 'ins' in variant:
             #Insertions need a little nudge in revcomp because of `ins at, del after`
             if self.genome2.genes[gene]['reverse_complement']:
                 nc_num -= 1
         elif 'del' in variant:
+            pos, t, bases = variant.split("_")
+            if start is not None and idx != start:
+                #This is not the start of the deletion, so truncate the bases as appropriate
+                dels = len(bases) - (idx - start)
+            else:
+                dels = len(bases)
             #Deletions need even more nudging in revcomp because the entire deletion is reversed so starts at the end
             if self.genome2.genes[gene]['reverse_complement']:
-                pos, t, bases = variant.split("_")
-                nc_num = nc_num - len(bases) + 1
+                nc_num = nc_num - dels + 1
         
         return nc_num
 
         
 
     def _get_vcf_idx(self, vcf_row: dict) -> int:
         '''Given a vcf row, figure out which alt it refers to. Should be available in the GT field
@@ -382,145 +388,245 @@
 
         for (idx,length,alt,r,a) in zip(self.genome1.nucleotide_index[mask],self.genome2.indel_length[mask], self.genome2.indel_nucleotides[mask],self.genome1.nucleotide_sequence, self.genome2.nucleotide_sequence):
             indices.append(idx)
             is_indel.append(True)
             is_het.append(False)
             is_snp.append(False)
             is_null.append(False)
+            refs.append(None)
+            alts.append(None)
             indel_length.append(length)
             indel_nucleotides.append(alt)
             if length>0:
                 variants.append(str(idx)+'_ins_'+str(alt))
             else:
                 variants.append(str(idx)+'_del_'+str(alt))
 
             #Find the genes at this pos
-            genes = sorted(list(set(self.genome1.stacked_gene_name[self.genome1.stacked_nucleotide_index == idx])))
-            if len(genes) > 1:
-                #If we have genes, we need to duplicate some info
-                first = True
-                for gene in genes:
-                    if gene == '':
-                        #If we have genes, we don't care about this one
-                        continue
+            positions = []
+            seen_genes = set()
+            if 'ins' in variants[-1]:
+                #Insertion, so only need to check a single index
+                positions.append(idx)
+                start = None
+            else:
+                #Deletion, so we need to check every deleted position for genes
+                pos, _, bases = variants[-1].split("_")
+                start = idx
+                for i in range(len(bases)):
+                    positions.append(idx + i)
+            first = True
+            for pos in positions:
+                genes = sorted(list(set(self.genome1.stacked_gene_name[self.genome1.stacked_nucleotide_index == pos])))
+                adding = False
+                mutli = False
+                if len(genes) > 1:
+                    multi = True
+                    #If we have genes, we need to duplicate some info
+                    for gene in genes:
+                        if gene == '':
+                            #If we have genes, we don't care about this one
+                            continue
+                            
+                        if gene in seen_genes:
+                            #If we've already seen it, skip
+                            continue
+                        else:
+                            #Mark as seen now we have seen it
+                            seen_genes.add(gene)
+                            adding = True                            
+                        gene_name.append(gene)
+                        gene_pos.append(self.get_gene_pos(gene, pos, variants[-1], start=start))
+                        if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
+                            #Get codon pos
+                            nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
+                            nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
+                            codon_idx.append((nc_num[nc_idx == pos][0] -1)% 3)
+                        else:
+                            codon_idx.append(None)
                         
-                    gene_name.append(gene)
-                    gene_pos.append(self.get_gene_pos(gene, idx, variants[-1]))
-                    if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
-                        #Get codon idx
-                        nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
-                        nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
-                        codon_idx.append((nc_num[nc_idx == idx][0] -1)% 3)
-                    else:
-                        codon_idx.append(None)
-                    
-                    #If this isn't the first one, we need to duplicate the row
-                    if first:
-                        first = False
+                        #If this isn't the first one, we need to duplicate the row
+                        if first:
+                            first = False
+                        else:
+                            variants.append(variants[-1])
+                            refs.append(refs[-1])
+                            alts.append(alt[-1])
+                            indices.append(indices[-1])
+                            is_indel.append(is_indel[-1])
+                            indel_length.append(indel_length[-1])
+                            indel_nucleotides.append(indel_nucleotides[-1])
+                            is_het.append(is_het[-1])
+                            is_snp.append(is_snp[-1])
+                            is_null.append(is_null[-1]) 
+                else:
+                    #We have 1 gene or none, so set to None if no gene is present
+                    gene = genes[0] if genes[0] != '' else None
+                    if gene in seen_genes:
+                        #If we've already seen it, or it's intragene so skip
+                        continue
                     else:
-                        variants.append(variants[-1])
-                        refs.append(refs[-1])
-                        alts.append(alt[-1])
-                        indices.append(indices[-1])
-                        is_indel.append(is_indel[-1])
-                        indel_length.append(indel_length[-1])
-                        indel_nucleotides.append(indel_nucleotides[-1])
-                        is_het.append(is_het[-1])
-                        is_snp.append(is_snp[-1])
-                        is_null.append(is_null[-1])
-
-            else:
-                #We have 1 gene or none, so set to None if no gene is present
-                gene = genes[0] if genes[0] != '' else None
-                if gene is not None:
-                    #Single gene, so pull out data
-                    gene_name.append(gene)
-                    gene_pos.append(self.get_gene_pos(gene, idx, variants[-1]))
-
-                    if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
-                        #Get codon idx
-                        nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
-                        nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
-                        codon_idx.append((nc_num[nc_idx == idx][0] -1)% 3)
+                        #Mark as seen now we have seen it
+                        seen_genes.add(gene)
+                        adding = True
+                    if gene is not None:
+                        #Single gene, so pull out data
+                        gene_name.append(gene)
+                        gene_pos.append(self.get_gene_pos(gene, pos, variants[-1], start=start))
+
+                        if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
+                            #Get codon pos
+                            nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
+                            nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
+                            codon_idx.append((nc_num[nc_idx == pos][0] -1)% 3)
+                        else:
+                            codon_idx.append(None)
                     else:
+                        #We don't care about intragene values if its not the first item
+                        if pos != idx:
+                            continue
+                        gene_name.append(None)
+                        gene_pos.append(None)
                         codon_idx.append(None)
-                else:
-                    gene_name.append(None)
-                    gene_pos.append(None)
-                    codon_idx.append(None)
+                #If this isn't the first one, we need to duplicate the row
+                if first:
+                    first = False
+                elif adding and not multi:
+                    variants.append(variants[-1])
+                    refs.append(refs[-1])
+                    alts.append(alt[-1])
+                    indices.append(indices[-1])
+                    is_indel.append(is_indel[-1])
+                    indel_length.append(indel_length[-1])
+                    indel_nucleotides.append(indel_nucleotides[-1])
+                    is_het.append(is_het[-1])
+                    is_snp.append(is_snp[-1])
+                    is_null.append(is_null[-1])                        
 
         # if the indel is on the LHS, then it is unchanged, then it needs 'reversing' since we are returning how to get to the RHS from the LHS hence we delete an insertion etc
         mask = self.genome1.is_indel & (self.genome1.indel_nucleotides!=self.genome2.indel_nucleotides)
 
         for (idx,length,alt,r,a) in zip(self.genome1.nucleotide_index[mask],self.genome1.indel_length[mask], self.genome1.indel_nucleotides[mask],self.genome1.nucleotide_sequence, self.genome2.nucleotide_sequence):
             indices.append(idx)
             is_indel.append(True)
             is_het.append(False)
             is_snp.append(False)
             is_null.append(False)
+            refs.append(None)
+            alts.append(None)
             length*=-1
             indel_length.append(length)
             indel_nucleotides.append(alt)
             if length>0:
                 variants.append(str(idx)+'_ins_'+str(alt))
             else:
                 variants.append(str(idx)+'_del_'+str(alt))
 
             #Find the genes at this pos
-            genes = sorted(list(set(self.genome1.stacked_gene_name[self.genome1.stacked_nucleotide_index == idx])))
-            if len(genes) > 1:
-                #If we have genes, we need to duplicate some info
-                first = True
-                for gene in genes:
-                    if gene == '':
-                        #If we have genes, we don't care about this one
+            positions = []
+            seen_genes = set()
+            if 'ins' in variants[-1]:
+                #Insertion, so only need to check a single index
+                positions.append(idx)
+                start = None
+            else:
+                #Deletion, so we need to check every deleted position for genes
+                pos, _, bases = variants[-1].split("_")
+                start = idx
+                for i in range(len(bases)):
+                    positions.append(idx + i)
+            first = True
+            for pos in positions:
+                genes = sorted(list(set(self.genome1.stacked_gene_name[self.genome1.stacked_nucleotide_index == pos])))
+                adding = False
+                multi = False
+                if len(genes) > 1:
+                    multi = True
+                    #If we have genes, we need to duplicate some info
+                    for gene in genes:
+                        if gene == '':
+                            #If we have genes, we don't care about this one
+                            continue
+                            
+                        if gene in seen_genes:
+                            #If we've already seen it, skip
+                            continue
+                        else:
+                            #Mark as seen now we have seen it
+                            seen_genes.add(gene)
+                            adding = True
+                            
+                        gene_name.append(gene)
+                        gene_pos.append(self.get_gene_pos(gene, pos, variants[-1], start=start))
+                        if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
+                            #Get codon pos
+                            nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
+                            nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
+                            codon_idx.append((nc_num[nc_idx == pos][0] -1)% 3)
+                        else:
+                            codon_idx.append(None)
+                        #If this isn't the first one, we need to duplicate the row
+                        if first:
+                            first = False
+                        else:
+                            variants.append(variants[-1])
+                            refs.append(refs[-1])
+                            alts.append(alt[-1])
+                            indices.append(indices[-1])
+                            is_indel.append(is_indel[-1])
+                            indel_length.append(indel_length[-1])
+                            indel_nucleotides.append(indel_nucleotides[-1])
+                            is_het.append(is_het[-1])
+                            is_snp.append(is_snp[-1])
+                            is_null.append(is_null[-1])   
+
+                else:
+                    #We have 1 gene or none, so set to None if no gene is present
+                    gene = genes[0] if genes[0] != '' else None
+                    if gene in seen_genes:
+                        #If we've already seen it, or it's intragene so skip
                         continue
-                    gene_name.append(gene)
-                    gene_pos.append(self.get_gene_pos(gene, idx, variants[-1]))
-                    if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
-                        #Get codon idx
-                        nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
-                        nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
-                        codon_idx.append((nc_num[nc_idx == idx][0] -1)% 3)
                     else:
-                        codon_idx.append(None)
-                    
-                    #If this isn't the first one, we need to duplicate the row
-                    if first:
-                        first = False
-                    else:
-                        variants.append(variants[-1])
-                        refs.append(refs[-1])
-                        alts.append(alt[-1])
-                        indices.append(indices[-1])
-                        is_indel.append(is_indel[-1])
-                        indel_length.append(indel_length[-1])
-                        indel_nucleotides.append(indel_nucleotides[-1])
-                        is_het.append(is_het[-1])
-                        is_snp.append(is_snp[-1])
-                        is_null.append(is_null[-1])
-
-            else:
-                #We have 1 gene or none, so set to None if no gene is present
-                gene = genes[0] if genes[0] != '' else None
-                if gene is not None:
-                    #Single gene, so pull out data
-                    gene_pos.append(self.get_gene_pos(gene, idx, variants[-1]))
-                    gene_name.append(gene)
-                    if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
-                        #Get codon idx
-                        nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
-                        nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
-                        codon_idx.append((nc_num[nc_idx == idx][0] -1)% 3)
+                        #Mark as seen now we have seen it
+                        seen_genes.add(gene)
+                        adding = True
+                    if gene is not None:
+                        #Single gene, so pull out data
+                        gene_name.append(gene)
+                        gene_pos.append(self.get_gene_pos(gene, pos, variants[-1], start=start))
+
+                        if self.genome2.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
+                            #Get codon pos
+                            nc_idx = self.genome1.stacked_nucleotide_index[self.genome1.stacked_gene_name == gene]
+                            nc_num = self.genome1.stacked_nucleotide_number[self.genome1.stacked_gene_name == gene]
+                            codon_idx.append((nc_num[nc_idx == pos][0] -1)% 3)
+                        else:
+                            codon_idx.append(None)
                     else:
+                        #We don't care about intragene values if its not the first item
+                        if pos != idx:
+                            continue
+                        gene_name.append(None)
+                        gene_pos.append(None)
                         codon_idx.append(None)
-                else:
-                    gene_name.append(None)
-                    gene_pos.append(None)
-                    codon_idx.append(None)
+
+                #If this isn't the first one, we need to duplicate the row
+                if first:
+                    first = False
+                elif adding and not multi:
+                    variants.append(variants[-1])
+                    refs.append(refs[-1])
+                    alts.append(alt[-1])
+                    indices.append(indices[-1])
+                    is_indel.append(is_indel[-1])
+                    indel_length.append(indel_length[-1])
+                    indel_nucleotides.append(indel_nucleotides[-1])
+                    is_het.append(is_het[-1])
+                    is_snp.append(is_snp[-1])
+                    is_null.append(is_null[-1])
 
         self.variants=numpy.array(variants)
         self.nucleotide_index=numpy.array(indices)
         self.is_indel=numpy.array(is_indel)
         self.indel_length=numpy.array(indel_length)
         self.indel_nucleotides=numpy.array(indel_nucleotides)
         self.is_snp=numpy.array(is_snp)
@@ -633,15 +739,19 @@
             if percentage >= 0.5:
                 #More than 50% deleted, so give a percentage
                 self.mutations = numpy.append(self.mutations, [f"del_{round(percentage, 2)}"])
                 #Pull out the start of the deletion for vcf evidence
                 self.nucleotide_index = numpy.append(self.nucleotide_index, [self.gene2.nucleotide_index[mask][0]])
 
                 self.amino_acid_number = numpy.append(self.amino_acid_number, [None])
-                self.nucleotide_number = numpy.append(self.nucleotide_number, [None])
+
+                #Get the nucleotide number of the first base of the gene
+                #Not predictable as promoters are variable length
+                self.nucleotide_number = numpy.append(self.nucleotide_number, [self.gene2.nucleotide_number[self.gene1.is_deleted | self.gene2.is_deleted][0]])
+
                 self.gene_position = numpy.append(self.gene_position, [None])
                 self.is_cds = numpy.append(self.is_cds, [True])
                 self.is_promoter = numpy.append(self.is_promoter, [False])
                 self.is_indel = numpy.append(self.is_indel, [True])
                 self.indel_length = numpy.append(self.indel_length, [-1*total])
                 self.indel_nucleotides = numpy.append(self.indel_nucleotides, [''.join(self.gene1.nucleotide_sequence[mask])])
                 self.ref_nucleotides = numpy.append(self.ref_nucleotides, [None])
@@ -691,15 +801,19 @@
 
                 pos = self.gene1.nucleotide_number[pos]
                 
                 self.mutations = numpy.append(self.mutations, [f"{pos}_del_{deleted}"])
                 #Pull out the start of the deletion for vcf evidence
                 self.nucleotide_index = numpy.append(self.nucleotide_index, [idx])
                 self.amino_acid_number = numpy.append(self.amino_acid_number, [None])
-                self.nucleotide_number = numpy.append(self.nucleotide_number, [None])
+
+                #Get the nucleotide number of the first base of the gene
+                #Not predictable as promoters are variable length
+                self.nucleotide_number = numpy.append(self.nucleotide_number, [self.gene2.nucleotide_number[self.gene1.is_deleted | self.gene2.is_deleted][0]])
+
                 self.gene_position = numpy.append(self.gene_position, [pos])
                 self.is_cds = numpy.append(self.is_cds, [True])
                 self.is_promoter = numpy.append(self.is_promoter, [False])
                 self.is_indel = numpy.append(self.is_indel, [True])
                 self.indel_length = numpy.append(self.indel_length, [len(deleted)])
                 self.indel_nucleotides = numpy.append(self.indel_nucleotides, [deleted])
                 self.ref_nucleotides = numpy.append(self.ref_nucleotides, [None])
```

### Comparing `gumpy-1.2.0/gumpy/gene.py` & `gumpy-1.2.1/gumpy/gene.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     def __duplicate(self, index: int):
         '''Duplicate all indices of important arrays to add the ribosomal shift
 
         Args:
             index (int): Gene index to duplicate in all arrays
         '''
         #Convert to gene array index
-        index = int(numpy.where(self.nucleotide_number == index)[0])+1
+        index = int(numpy.where(self.nucleotide_number == index)[0][0])+1
 
         #Update the nucelotide_numbers so they include the duplicate
         #Check for promoters before the codons
         first_half = [self.nucleotide_number[i] for i in range(index)]
         second_half = [
             self.nucleotide_number[i] + 1 if self.nucleotide_number[i] > 0
             else self.nucleotide_number[i]
```

### Comparing `gumpy-1.2.0/gumpy/genome.py` & `gumpy-1.2.1/gumpy/genome.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.0/gumpy/variantfile.py` & `gumpy-1.2.1/gumpy/variantfile.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.0/gumpy.egg-info/PKG-INFO` & `gumpy-1.2.1/gumpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Genetics with Numpy
 Home-page: https://github.com/oxfordmmm/gumpy
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gumpy-1.2.0/setup.cfg` & `gumpy-1.2.1/setup.cfg`

 * *Files identical despite different names*

