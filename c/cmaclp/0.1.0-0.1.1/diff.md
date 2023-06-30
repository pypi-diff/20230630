# Comparing `tmp/cmaclp-0.1.0-py3-none-any.whl.zip` & `tmp/cmaclp-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,13 @@
-Zip file size: 12231 bytes, number of entries: 8
--rw-r--r--  2.0 unx    22149 b- defN 23-Jun-20 14:01 cmaclp/SVM_prediction.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 14:01 cmaclp/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1178 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      164 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      630 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/RECORD
-8 files, 35577 bytes uncompressed, 11131 bytes compressed:  68.7%
+Zip file size: 17308 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    31531 b- defN 23-Jun-30 12:05 cmaclp/SVM_prediction.py
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-30 12:05 cmaclp/__init__.py
+-rw-r--r--  2.0 unx     6366 b- defN 23-Jun-30 12:05 cmaclp/tests/SVM_prediction_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 12:05 cmaclp/tests/__init__.py
+-rw-r--r--  2.0 unx     2335 b- defN 23-Jun-30 12:05 cmaclp/tests/cmaclp_test_model.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-30 12:07 cmaclp-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1633 b- defN 23-Jun-30 12:07 cmaclp-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 12:07 cmaclp-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-30 12:07 cmaclp-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-30 12:07 cmaclp-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      892 b- defN 23-Jun-30 12:07 cmaclp-0.1.1.dist-info/RECORD
+11 files, 54784 bytes uncompressed, 15796 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,25 +1,34 @@
 Filename: cmaclp/SVM_prediction.py
 Comment: 
 
 Filename: cmaclp/__init__.py
 Comment: 
 
-Filename: cmaclp-0.1.0.dist-info/LICENSE
+Filename: cmaclp/tests/SVM_prediction_test.py
 Comment: 
 
-Filename: cmaclp-0.1.0.dist-info/METADATA
+Filename: cmaclp/tests/__init__.py
 Comment: 
 
-Filename: cmaclp-0.1.0.dist-info/WHEEL
+Filename: cmaclp/tests/cmaclp_test_model.py
 Comment: 
 
-Filename: cmaclp-0.1.0.dist-info/entry_points.txt
+Filename: cmaclp-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: cmaclp-0.1.0.dist-info/top_level.txt
+Filename: cmaclp-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: cmaclp-0.1.0.dist-info/RECORD
+Filename: cmaclp-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: cmaclp-0.1.1.dist-info/entry_points.txt
+Comment: 
+
+Filename: cmaclp-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: cmaclp-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmaclp/SVM_prediction.py

```diff
@@ -13,41 +13,42 @@
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
 from sklearn.metrics import f1_score
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import precision_score
 from scanpy import read_h5ad
 from importlib.resources import files
+import re
+from statistics import mean
+from scipy.stats import pearsonr
+from scipy.stats import spearmanr
 
 def SVM_prediction(reference_H5AD, query_H5AD, LabelsPathTrain, OutputDir, rejected=False, Threshold_rej=0.7,meta_atlas=False):
     '''
     run baseline classifier: SVM
     Wrapper script to run an SVM classifier with a linear kernel on a benchmark dataset with 5-fold cross validation,
     outputs lists of true and predicted cell labels as csv files, as well as computation time.
 
     Parameters:
     reference_H5AD, query_H5AD : H5AD files that produce training and testing data,
         cells-genes matrix with cell unique barcodes as row names and gene names as column names.
     LabelsPathTrain : Cell population annotations file path matching the training data (.csv).
     OutputDir : Output directory defining the path of the exported file.
     rejected: If the flag is added, then the SVMrejected option is chosen. Default: False.
     Threshold_rej : Threshold used when rejecting the cells, default is 0.7.
-    meta_atlas : If the flag is added the predictions will use the corneal meta-atlas data,
+    meta_atlas : If the flag is added the predictions will use meta-atlas data.
     meaning that reference_H5AD and LabelsPathTrain do not need to be specified.
     '''
     print("Reading in the reference and query H5AD objects")
     
     # Load in the cma.h5ad object or use a different reference
     if meta_atlas is False:
         training=read_h5ad(reference_H5AD) 
     if meta_atlas is True:
-    #    if not if os.path.exists(DEG_file):
-    #        if not outputdir == "":
-        os.makedirs(OutputDir, exist_ok=True)
-        meta_dir=files('cmaclp.data').joinpath('cma_meta_atlas.h5ad')
+        meta_dir='data/cma_meta_atlas.h5ad'
         training=read_h5ad(meta_dir) 
 
     # Load in the test data
     testing=read_h5ad(query_H5AD)
  
     print("Generating training and testing matrices from the H5AD objects")
     
@@ -85,15 +86,15 @@
     
     # read the data
     data_train = matrix_train2
     data_test = matrix_test2
     
     # If meta_atlas=True it will read the training_labels
     if meta_atlas is True:
-        LabelsPathTrain = files('cmaclp.data').joinpath('training_labels_meta.csv')
+        LabelsPathTrain = 'data/training_labels_meta.csv'
     
     labels_train = pd.read_csv(LabelsPathTrain, header=0,index_col=None, sep=',')
         
     # Set threshold for rejecting cells
     if rejected is True:
         Threshold = Threshold_rej
 
@@ -132,26 +133,27 @@
         pred.extend(predicted)
         pred = pd.DataFrame(pred)
         
         # Save the predicted labels
         pred.to_csv(str(OutputDir) + "SVM_Pred_Labels.csv", index =False)
 
 
-def SVM_import(query_H5AD, OutputDir, SVM_type, replicates, meta_atlas=False, show_umap=False, show_bar=False):
+def SVM_import(query_H5AD, OutputDir, SVM_type, replicates, colord=None, meta_atlas=False, show_bar=False):
     '''
     Imports the output of the SVM_predictor and saves it to the query_H5AD.
 
     Parameters:
-    query_H5AD : H5AD file of datasets of interest.
-    OutputDir : Output directory defining the path of the exported SVM_predictions.
+    query_H5AD: H5AD file of datasets of interest.
+    OutputDir: Output directory defining the path of the exported SVM_predictions.
     SVM_type: Type of SVM prediction, SVM (default) or SVMrej.
-    Replicates: 
-    meta_atlas:
-    show_umap:
-    show_bar:
+    Replicates: A string value specifying a column in query_H5AD.obs.
+    colord: A .tsv file with the order of the meta-atlas and corresponding colors.
+    meta_atlas : If the flag is added the predictions will use meta-atlas data.
+    show_bar: Shows bar plots depending on the SVM_type, split over replicates.
+
     '''
     print("Reading query data")
     adata=read_h5ad(query_H5AD)
     SVM_key=f"{SVM_type}_predicted"
 
     # Load in the object and add the predicted labels
     print("Adding predictions to query data")
@@ -176,57 +178,34 @@
                 #print(filedir)
                 influence_data= pd.read_csv(filedir,sep=',',index_col=0)
                 #print(influence_data)
                 influence_data=influence_data.index.tolist()
                 adata.obs["SVMrej_predicted_prob"]=influence_data
 
     # Set category colors:
-    if meta_atlas is True:
-        category_colors = {"LSC": "#66CD00",
-                    "LESC": "#76EE00",
-                    "LE": "#66CDAA",
-                    "Cj": "#191970",
-                    "CE": "#1874CD",
-                    "qSK": "#FFB90F",
-                    "SK": "#EEAD0E",
-                    "TSK": "#FF7F00",
-                    "CF": "#CD6600",
-                    "EC": "#87CEFA",
-                    "Ves": "#8B2323",
-                    "Mel": "#FFFF00",
-                    "IC": "#00CED1",
-                    "nm-cSC": "#FF0000",
-                    "MC": "#CD3700",
-                    "Unknown": "#808080"}
+    if meta_atlas is True and colord is not None:
+        df_category_colors=pd.read_csv(colord, header=None,index_col=False, sep='\t')
+        category_colors = dict(zip(df_category_colors.iloc[:,0], df_category_colors.iloc[:,1]))
+        print(category_colors)
+        if SVM_key == "SVMrej_predicted":
+          category_colors["Unlabeled"]= "#808080"
                     
-    if meta_atlas is False:
+    if meta_atlas is False or colord is None:
     
       # Load a large color palette
       palette_name = "tab20"
       cmap = plt.get_cmap(palette_name)
       palette=[matplotlib.colors.rgb2hex(c) for c in cmap.colors] 
       
       # Extract the list of colors
       colors = palette
       key_cats = adata.obs[SVM_key].astype("category")
       key_list = key_cats.cat.categories.to_list()
             
       category_colors = dict(zip(key_list, colors[:len(key_list)]))
-      
-    # Plot UMAP if selected
-    print("Plotting UMAP")
-    sc.set_figure_params(figsize=(5, 5))
-    if show_umap is True:
-        if meta_atlas is True:
-            category_order_list = ["LSC", "LESC","LE","Cj","CE","qSK","SK","TSK","CF","EC","Ves","Mel","IC","nm-cSC","MC","Unknown"]
-            adata.obs[SVM_key] = adata.obs[SVM_key].astype("category")
-            adata.obs[SVM_key] = adata.obs[SVM_key].cat.set_categories(category_order_list, ordered=True)
-            sc.pl.umap(adata, color=SVM_key,palette=category_colors,show=False,save=f"_{SVM_key}.pdf")
-        else:
-            sc.pl.umap(adata, color=SVM_key,show=False,save=f"_{SVM_key}.pdf")
             
     # Plot absolute and relative barcharts across replicates
     print("Plotting barcharts")
     if show_bar is True:
         sc.set_figure_params(figsize=(15, 5))
         
         key=SVM_key
@@ -251,23 +230,30 @@
             obs1_to_obs2[l][obs2_clusters.index(str(b))] += 1
 
         df = pd.DataFrame.from_dict(obs2_to_obs1,orient = 'index').reset_index()
         df = df.set_index(["index"])
         df.columns=obs1_clusters
         df.index.names = ['Replicate']
 
-        if meta_atlas is True:
+        if meta_atlas is True and colord is not None:
             palette=category_colors
-            if SVM_type == 'SVM':
-              ordered_list=["LSC", "LESC","LE","Cj","CE","qSK","SK","TSK","CF","EC","Ves","Mel","IC","nm-cSC","MC"]
+            if SVM_type == 'SVM' :
+              ord_list = [key for key in palette]
+              
             if SVM_type == 'SVMrej':
-              ordered_list=["LSC", "LESC","LE","Cj","CE","qSK","SK","TSK","CF","EC","Ves","Mel","IC","nm-cSC","MC","Unknown"]
+              colordkeys_list = [key for key in palette]
+              ord_list=colordkeys_list.append("Unlabeled")
             
             # Sorts the df on the longer ordered list
-            sorter=sorted(df.columns, key=ordered_list.index)
+            def sort_small_list(long_list, small_list):
+              sorted_list = sorted(small_list, key=lambda x: long_list.index(x))
+              return sorted_list
+            
+            sorter = sort_small_list(ord_list, df.columns.tolist())
+            #sorter=sorted(df.columns, key=ord_list.get)
             
             # Retrieve the color codes from the sorted list
             lstval = [palette[key] for key in sorter]
             
             try:
               df=df[sorter]
             except KeyError:
@@ -347,15 +333,15 @@
     np.log1p(data,out=data)
 
     X = data
     del data
 
     label_encoder = LabelEncoder()
     
-    y = label_encoder.fit_transform(labels["x"].tolist())
+    y = label_encoder.fit_transform(labels.iloc[:,0].tolist())
 
     # Generate a dictionary to map values to strings
     res = dict(zip(label_encoder.inverse_transform(y),y))
     res['Unlabeled'] = 999999
     res = {v: k for k, v in res.items()}
     res
 
@@ -479,14 +465,198 @@
     # Plot png
     sns.set(font_scale=0.8)
     cm = sns.clustermap(cnf_matrix.T, cmap="Blues", annot=True,fmt='.2%', row_cluster=False,col_cluster=False)
     cm.savefig(f"figures/{SVM_type}_cnf_matrix.png")
     return F1score,acc_score,prec_score
 
 
+def SVM_pseudobulk(condition_1, condition_1_batch, condition_2, condition_2_batch, Labels_1, OutputDir="pseudobulk_output/", min_cells=50, SVM_type="SVM"):
+    '''
+    Produces pseudobulk RNA-seq count files and sample files of either technical or biological replicates.
+    It produces pseudobulk of all labels from LabelsPath against predicted labels after SVMprediction.
+    Moreover, it produces overall pseudobulk of condition_1 vs condition_2 split by indicated batches.
+
+    Parameters:
+    condition_1, condition_2 : H5AD files with cells-genes matrix with cell unique barcodes as 
+        row names and gene names as column names. Condition_1 should be the meta-atlas and
+        condition_2 should be the queried object.
+    condition_1_batch : batch name for the meta-atlas object replicates (biological, technical etc.)
+    condition_2_batch: batch name for the queried object
+    Labels_1 : Cell population annotations file path matching the training data (.csv) or 
+        a string that specifies an .obs value in condition 1.
+    OutputDir: The directory into which the results are outputted; default: "pseudobulk_output/"
+    '''
+    print("Reading in the reference and query H5AD objects and adding batches")
+    cond_1=read_h5ad(condition_1)
+    cond_2=read_h5ad(condition_2)
+    outputdir=OutputDir
+    
+    # Reading in the Labels_1 for the replicates
+    # First tries to read in Labels_1 as a path
+    try:
+      label_data=pd.read_csv(Labels_1,sep=',',index_col=0)
+      label_data=label_data.index.tolist()
+      cond_1.obs["meta_atlas"]=label_data
+      cond_1_label="meta_atlas"
+    # Then tries to read in Labels_1 as a string in obs
+    except (TypeError, FileNotFoundError) as error:
+      try:
+        cond_1_label=str(Labels_1)
+        cond_1.obs[cond_1_label]
+    # If no key if found a valid key must be entered
+      except KeyError:
+        raise ValueError('Please provide a valid name for labels in Labels_1')
+      
+    print("Constructing condition for condition 1")
+    cond_1.obs["condition"]="cond1"
+
+    print("Constructing batches for condition 1")
+    # Add extra index to the ref object:
+    cond_1.obs["batch"] = cond_1.obs[condition_1_batch]
+
+    # Convert the 'Category' column to numeric labels
+    cond_1.obs["batch"] = pd.factorize(cond_1.obs["batch"])[0] + 1
+
+    cond_1.obs["merged"]=cond_1.obs[cond_1_label]+"."+cond_1.obs["condition"]
+    cond_1.obs["merged_batch"]=cond_1.obs["merged"]+"."+cond_1.obs["batch"].astype(str)
+    cond_1.obs["full_batch"]=cond_1.obs["condition"]+"."+cond_1.obs["batch"].astype(str)
+
+    print("Constructing batches for condition 2")
+
+    # Uses the specified SVM_type for predicted cond_2
+    cond_2_label=f'{SVM_type}_predicted'
+    batch=condition_2_batch
+
+    cond_2.obs["condition"]="cond2"
+    cond_2.obs["batch"]=cond_2.obs[batch]
+    cond_2.obs["merged"]=cond_2.obs[cond_2_label].astype(str)+"."+cond_2.obs["condition"]
+    cond_2.obs["merged_batch"]=cond_2.obs["merged"]+"."+cond_2.obs["batch"].astype(str)
+    cond_2.obs["full_batch"]=cond_2.obs["condition"]+"."+cond_2.obs["batch"].astype(str)
+    
+    os.makedirs(outputdir, exist_ok=True)
+        
+    # Use each object as a condition
+    for cond in cond_1,cond_2:
+        cond_str = cond.obs["condition"].astype(str)[1]
+        print(f"Running with {cond_str}")
+
+        if cond.obs["condition"].astype(str)[1] == "cond1":
+            cond_name="cond1"
+        elif cond.obs["condition"].astype(str)[1] == "cond2":
+            cond_name="cond2"
+
+        # Construct the sample.tsv file    
+        cond.obs["assembly"]="hg38"
+
+        adata = cond.copy()
+
+        # extract names of genes
+        try:
+            adata.var_names=adata.var["_index"].tolist()
+        except KeyError:
+            adata.var_names=adata.var.index
+
+
+        for cluster_id in ["merged_batch","full_batch"]:
+            print("Running pseudobulk extraction with: "+str(cluster_id))
+            if cluster_id == "full_batch":
+                sample_lists=adata.obs[[cluster_id,"assembly","condition","full_batch"]]
+            if cluster_id == "merged_batch":
+                sample_lists=adata.obs[[cluster_id,"assembly","merged","condition","full_batch"]]  
+            sample_lists=sample_lists.reset_index(drop=True)
+            sample_lists=sample_lists.drop_duplicates()
+            sample_lists.rename(columns={ sample_lists.columns[0]: "sample" }, inplace = True)
+
+            rna_count_lists = list()
+            FPKM_count_lists = list()
+            cluster_names = list()
+
+            for cluster in adata.obs[cluster_id].astype("category").unique():
+
+                # Only use ANANSE on clusters with more than minimal amount of cells
+                n_cells = adata.obs[cluster_id].value_counts()[cluster]
+
+                if n_cells > min_cells:
+                    cluster_names.append(str(cluster))
+
+                    # Generate the raw count file
+                    adata_sel = adata[adata.obs[cluster_id].isin([cluster])].copy()
+                    adata_sel.raw=adata_sel
+
+                    print(
+                        str("gather data from " + cluster + " with " + str(n_cells) + " cells")
+                    )
+
+                    X_clone = adata_sel.X.tocsc()
+                    X_clone.data = np.ones(X_clone.data.shape)
+                    NumNonZeroElementsByColumn = X_clone.sum(0)
+                    rna_count_lists += [list(np.array(NumNonZeroElementsByColumn)[0])]
+                    sc.pp.normalize_total(adata_sel, target_sum=1e6, inplace=True)
+                    X_clone2=adata_sel.X.toarray()
+                    NumNonZeroElementsByColumn = [X_clone2.sum(0)]
+                    FPKM_count_lists += [list(np.array(NumNonZeroElementsByColumn)[0])]
+
+            # Specify the df.index
+            df = adata.T.to_df()
+
+            # Generate the count matrix df
+            rna_count_lists = pd.DataFrame(rna_count_lists)
+            rna_count_lists = rna_count_lists.transpose()
+            rna_count_lists.columns = cluster_names
+            rna_count_lists.index = adata.var_names
+            rna_count_lists["average"] = rna_count_lists.mean(axis=1)
+            rna_count_lists = rna_count_lists.astype("int")
+
+            # Generate the FPKM matrix df
+            FPKM_count_lists = pd.DataFrame(FPKM_count_lists)
+            FPKM_count_lists = FPKM_count_lists.transpose()
+            FPKM_count_lists.columns = cluster_names
+            FPKM_count_lists.index = adata.var_names
+            FPKM_count_lists["average"] = FPKM_count_lists.mean(axis=1)
+            FPKM_count_lists = FPKM_count_lists.astype("int")
+
+            count_file = str(outputdir +str(cond_name)+"_"+str(cluster_id)+"_RNA_Counts.tsv")
+            CPM_file = str(outputdir +str(cond_name)+"_"+str(cluster_id)+ "_TPM.tsv")
+            sample_file = str(outputdir +str(cond_name)+"_"+str(cluster_id)+ "_samples.tsv")
+            rna_count_lists.to_csv(count_file, sep="\t", index=True, index_label=False)
+            FPKM_count_lists.to_csv(CPM_file, sep="\t", index=True, index_label=False)
+            sample_lists.to_csv(sample_file, sep="\t", index=False, index_label=False)
+    
+    # Import the intermediate results back
+    for cluster_id in ["merged_batch","full_batch"]:
+        print("Running file merge with: "+str(cluster_id))
+            
+        # Merge the counts from the individual objects lists
+        df_1 = pd.read_csv(str(outputdir +"cond1"+"_"+str(cluster_id)+"_RNA_Counts.tsv"),sep="\t")
+        del df_1["average"]
+        df_2 = pd.read_csv(str(outputdir +"cond2"+"_"+str(cluster_id)+"_RNA_Counts.tsv"),sep="\t")
+        del df_2["average"]
+        
+        df_1_samples=pd.read_csv(str(outputdir +"cond1"+"_"+str(cluster_id)+ "_samples.tsv"),sep="\t")
+        df_2_samples=pd.read_csv(str(outputdir +"cond2"+"_"+str(cluster_id)+ "_samples.tsv"),sep="\t")
+
+        # Save merged count files
+        merged_df = pd.merge(df_1, df_2, left_index=True, right_index=True, how='inner')
+        merged_df.index.name='gene'
+        
+        print("Saving merged count files for "+str(cluster_id))
+        merged_file= str(outputdir+str(cluster_id)+"_merged.tsv")
+        merged_df.to_csv(merged_file, sep="\t", index=True, index_label="gene")
+        
+        # Save merged sample files
+        cond_samples = pd.concat([df_1_samples,df_2_samples])
+        
+        print("Saving sample files for "+str(cluster_id))
+        cond_samples_file= str(outputdir+str(cluster_id)+"_samples.tsv")
+        cond_samples.to_csv(cond_samples_file, sep="\t", index=False)
+        print("Finished constructing contrast between conditions for: "+str(cluster_id))
+    
+    return
+
+
 def predpars():
     # Create the parser
     parser = argparse.ArgumentParser(description='Run SVM prediction')
 
     # Add arguments
     parser.add_argument('--reference_H5AD', type=str, help='Path to reference H5AD file')
     parser.add_argument('--query_H5AD', type=str, help='Path to query H5AD file')
@@ -538,35 +708,64 @@
 
 def importpars():
 
     parser = argparse.ArgumentParser(description="Imports predicted results back to H5AD file")
     parser.add_argument("--query_H5AD", type=str, help="Path to query H5AD file")
     parser.add_argument("--OutputDir", type=str, help="Output directory path")
     parser.add_argument("--SVM_type", type=str, help="Type of SVM prediction (SVM or SVMrej)")
+    parser.add_argument("--colord", type=str, help=".tsv file with meta-atlas order and colors")
     parser.add_argument("--replicates", type=str, help="Replicates")
-    parser.add_argument("--meta-atlas", dest="meta_atlas", action="store_true", help="Use meta atlas data")
-    parser.add_argument("--show-umap", dest="show_umap", action="store_true", help="Show UMAP plotting")
-    parser.add_argument("--show-bar", dest="show_bar", action="store_true", help="Show bar chart plotting")
+    parser.add_argument("--meta-atlas", dest="meta_atlas", action="store_true", help="Use meta-atlas data")
 
     args = parser.parse_args()
 
     SVM_import(
         args.query_H5AD,
         args.OutputDir,
         args.SVM_type,
+        args.colord,
         args.replicates,
         args.meta_atlas,
-        args.show_umap,
         args.show_bar)
 
+# ADD 
+
+def pseudopars():
+
+    parser = argparse.ArgumentParser(description="Performs individual and joined pseudobulk on two H5AD objects")
+    parser.add_argument("--condition_1", type=str, help="Path to meta-atlas or other H5AD file")
+    parser.add_argument("--condition_1_batch", type=str, help="Technical, biological or other replicate column in condition_1.obs")
+    parser.add_argument("--condition_2", type=str, help="Path to H5AD file with SVM predictions")
+    parser.add_argument("--condition_2_batch", type=str, help="Technical, biological or other replicate column in condition_2.obs")
+    parser.add_argument("--Labels_1", type=str, help="Label path for the meta-atlas (LabelsPathTrain) or condition_1.obs column with names")
+    parser.add_argument('--OutputDir', dest='pseudobulk_output/', action='store_true', help='Directory where pseudobulk results are outputted')
+    parser.add_argument("--min_cells", type=float, default=50, help="Minimal amount of cells for each condition and replicate")
+    parser.add_argument("--SVM_type", type=str, help="Type of SVM prediction (SVM or SVMrej)")
+    
+    args = parser.parse_args()
+
+    SVM_pseudobulk(
+        args.condition_1,
+        args.condition_1_batch,
+        args.condition_2,
+        args.condition_2_batch,
+        args.Labels_1,
+        args.OutputDir,
+        args.min_cells,
+        args.SVM_type)
+
 
 if __name__ == '__predpars__':
     predpars()
 
     
 if __name__ == '__performpars__':
     performpars()
 
 
 if __name__ == '__importpars__':
     importpars()
 
+
+if __name__ == '__pseudopars__':
+    importpars()
+
```

## cmaclp/__init__.py

```diff
@@ -0,0 +1,23 @@
+00000000: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2230  __version__ = "0
+00000010: 2e31 2e31 220d 0a0d 0a66 726f 6d20 2e53  .1.1"....from .S
+00000020: 564d 5f70 7265 6469 6374 696f 6e20 696d  VM_prediction im
+00000030: 706f 7274 2053 564d 5f70 7265 6469 6374  port SVM_predict
+00000040: 696f 6e0d 0a66 726f 6d20 2e53 564d 5f70  ion..from .SVM_p
+00000050: 7265 6469 6374 696f 6e20 696d 706f 7274  rediction import
+00000060: 2053 564d 5f69 6d70 6f72 740d 0a66 726f   SVM_import..fro
+00000070: 6d20 2e53 564d 5f70 7265 6469 6374 696f  m .SVM_predictio
+00000080: 6e20 696d 706f 7274 2053 564d 5f70 6572  n import SVM_per
+00000090: 666f 726d 616e 6365 0d0a 6672 6f6d 202e  formance..from .
+000000a0: 5356 4d5f 7072 6564 6963 7469 6f6e 2069  SVM_prediction i
+000000b0: 6d70 6f72 7420 5356 4d5f 7073 6575 646f  mport SVM_pseudo
+000000c0: 6275 6c6b 0d0a 6672 6f6d 202e 5356 4d5f  bulk..from .SVM_
+000000d0: 7072 6564 6963 7469 6f6e 2069 6d70 6f72  prediction impor
+000000e0: 7420 7072 6564 7061 7273 0d0a 6672 6f6d  t predpars..from
+000000f0: 202e 5356 4d5f 7072 6564 6963 7469 6f6e   .SVM_prediction
+00000100: 2069 6d70 6f72 7420 696d 706f 7274 7061   import importpa
+00000110: 7273 0d0a 6672 6f6d 202e 5356 4d5f 7072  rs..from .SVM_pr
+00000120: 6564 6963 7469 6f6e 2069 6d70 6f72 7420  ediction import 
+00000130: 7065 7266 6f72 6d70 6172 730d 0a66 726f  performpars..fro
+00000140: 6d20 2e53 564d 5f70 7265 6469 6374 696f  m .SVM_predictio
+00000150: 6e20 696d 706f 7274 2070 7365 7564 6f70  n import pseudop
+00000160: 6172 730d 0a                             ars..
```

## Comparing `cmaclp-0.1.0.dist-info/LICENSE` & `cmaclp-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cmaclp-0.1.0.dist-info/RECORD` & `cmaclp-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-cmaclp/SVM_prediction.py,sha256=If9zZ4vyL7vWtNuPYaouVCqwWq89dxsD7cM2tTFiXQU,22149
-cmaclp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cmaclp-0.1.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cmaclp-0.1.0.dist-info/METADATA,sha256=k3MOAj1nMwmtRH7NjcDq1JCsEpebI_GCBKg9Q9hMN-Y,1178
-cmaclp-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmaclp-0.1.0.dist-info/entry_points.txt,sha256=r9COjTyooEYKohivL1TnNScb5tIS-LfVrbX8Lle9VBw,164
-cmaclp-0.1.0.dist-info/top_level.txt,sha256=aDpLhklg1da22MWr2NS6Do368bNv2rlOX_pk5T57tS4,7
-cmaclp-0.1.0.dist-info/RECORD,,
+cmaclp/SVM_prediction.py,sha256=pnK-WHcbc7_gib-RQocufgjPpbPtJXelyZTHOx6s1wg,31531
+cmaclp/__init__.py,sha256=JDpfLrO5YPtXd8vve4VOFfAAOpvmvZZrwbD79_Nitms,357
+cmaclp/tests/SVM_prediction_test.py,sha256=TRdQs3bGiluj8BsYfQFaIoS3om8AURYhucxJpD7c1Hg,6366
+cmaclp/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cmaclp/tests/cmaclp_test_model.py,sha256=ktE-UG8R7EDJqZ6_xE811yI-f9n04NeqQB16lMStUp8,2335
+cmaclp-0.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cmaclp-0.1.1.dist-info/METADATA,sha256=hRYgm9MZ5I_pbPNO4te6qyHCmL_HS6VUHCmvkPZr-AY,1633
+cmaclp-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmaclp-0.1.1.dist-info/entry_points.txt,sha256=lqPVzDiKGyqlY6qw3m7LvlT4y2CdUza43ykNIN86BCU,214
+cmaclp-0.1.1.dist-info/top_level.txt,sha256=aDpLhklg1da22MWr2NS6Do368bNv2rlOX_pk5T57tS4,7
+cmaclp-0.1.1.dist-info/RECORD,,
```

