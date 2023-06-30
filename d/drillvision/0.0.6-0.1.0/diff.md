# Comparing `tmp/drillvision-0.0.6.tar.gz` & `tmp/drillvision-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drillvision-0.0.6.tar", last modified: Thu Jun 29 18:49:04 2023, max compression
+gzip compressed data, was "drillvision-0.1.0.tar", last modified: Fri Jun 30 15:15:10 2023, max compression
```

## Comparing `drillvision-0.0.6.tar` & `drillvision-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:49:04.650005 drillvision-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-29 18:47:26.000000 drillvision-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-29 18:49:04.650005 drillvision-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-29 18:47:26.000000 drillvision-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:49:04.650005 drillvision-0.0.6/drillvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 18:49:04.000000 drillvision-0.0.6/drillvision.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:49:04.650005 drillvision-0.0.6/neural_network_model/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29087 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/bit_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)    62009 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/cam.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/script_run_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    26981 2023-06-29 18:47:26.000000 drillvision-0.0.6/neural_network_model/transfer_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-29 18:47:26.000000 drillvision-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 18:47:26.000000 drillvision-0.0.6/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 18:47:26.000000 drillvision-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:49:04.650005 drillvision-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-29 18:47:26.000000 drillvision-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:10.163065 drillvision-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 15:13:18.000000 drillvision-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 15:15:10.163065 drillvision-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-30 15:13:18.000000 drillvision-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:10.159064 drillvision-0.1.0/drillvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:10.159064 drillvision-0.1.0/neural_network_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29087 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/bit_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62009 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/cam.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/script_run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-30 15:13:18.000000 drillvision-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-30 15:13:18.000000 drillvision-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 15:13:18.000000 drillvision-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:15:10.163065 drillvision-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 15:13:18.000000 drillvision-0.1.0/setup.py
```

### Comparing `drillvision-0.0.6/PKG-INFO` & `drillvision-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.6
+Version: 0.1.0
 Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drillvision-0.0.6/README.md` & `drillvision-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/drillvision.egg-info/PKG-INFO` & `drillvision-0.1.0/drillvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.6
+Version: 0.1.0
 Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drillvision-0.0.6/drillvision.egg-info/SOURCES.txt` & `drillvision-0.1.0/drillvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/neural_network_model/bit_vision.py` & `drillvision-0.1.0/neural_network_model/bit_vision.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/neural_network_model/cam.jpg` & `drillvision-0.1.0/neural_network_model/cam.jpg`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/neural_network_model/model.py` & `drillvision-0.1.0/neural_network_model/model.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/neural_network_model/process_data.py` & `drillvision-0.1.0/neural_network_model/process_data.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/neural_network_model/s3.py` & `drillvision-0.1.0/neural_network_model/s3.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/neural_network_model/script_run_all.py` & `drillvision-0.1.0/neural_network_model/script_run_all.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/neural_network_model/transfer_learning.py` & `drillvision-0.1.0/neural_network_model/transfer_learning.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,23 +75,34 @@
         self.image_df = image_df
         if print_data_head:
             print(self.image_df.head(3))
         # log the data was prepared
         logging.info("Data was prepared")
 
     def plot_classes_number(
-        self, figsize=(10, 5), x_rotation=0, palette="Greens_r"
+        self,
+        figsize=(10, 5),
+        x_rotation=0,
+        palette="Greens_r",
+        **kwargs,
     ) -> None:
         """
         Plot the number of images per species
         :param figsize: size of the figure
         :param x_rotation: rotation of the x-axis
         :param palette: color palette
+        :param kwargs: figure_folder_path
         :return: None
         """
+        figure_folder_path = kwargs.get(
+            "figure_folder_path", Path(__file__).parent / ".." / "figures"
+        )
+        # check if the folder exists if not create it
+        if not figure_folder_path.exists():
+            os.makedirs(figure_folder_path)
 
         base_path = self.dataset_address
         subfolders = os.listdir(base_path)
         names = []
         counts = []
 
         filtered_subfolders = self._filter_out_list(list_to_be_edited=subfolders)
@@ -107,34 +118,45 @@
         idx = np.argsort(counts)[::-1]
 
         plt.figure(figsize=figsize)
         sns.barplot(x=names[idx], y=counts[idx], palette=palette)
         plt.xticks(rotation=x_rotation)
         plt.title("How many images per classes are given in the data?")
         plt.tight_layout()
+        # save the plot in the figures folder
+        plt.savefig(figure_folder_path / "classes_number.png")
         plt.show()
 
     def analyze_image_names(
         self,
         figsize=(20, 22),
         figsize_2=(10, 7),
         cmap_2="YlGnBu",
         size=15,
         label_size=25,
         num_cluster=5,
+        **kwargs,
     ) -> None:
         """
         Analyze the image names if there is any pattern in the names
         :param figsize: size of the figure
         :param figsize_2: size of the second figure
         :param cmap_2: color map of the second figure
         :param size: size of the scatter points
         :param label_size: size of the labels
         :param num_cluster: number of clusters - unsupervised learning on width of images
         """
+
+        figure_folder_path = kwargs.get(
+            "figure_folder_path", Path(__file__).parent / ".." / "figures"
+        )
+        # check if the folder exists if not create it
+        if not figure_folder_path.exists():
+            os.makedirs(figure_folder_path)
+
         base_path = self.dataset_address
         subfolders = os.listdir(base_path)
         filtered_subfolders = self._filter_out_list(list_to_be_edited=subfolders)
 
         total_images = 0
         for folder in filtered_subfolders:
             total_images += len(os.listdir(base_path / folder))
@@ -173,14 +195,16 @@
         for single in image_df.classes.unique():
             # sns.kdeplot(
             #     image_df[image_df.classes == single].width, ax=ax[1], label=single
             # )
             # Filter the data based on the 'classes' column
             filtered_data = image_df[image_df.classes == single].width
             plt.hist(filtered_data, density=True, alpha=0.5, label=single)
+            # show the legend
+            plt.legend()
         ax[1].legend()
         ax[1].set_title("KDE-Plot of image width given classes")
         ax[1].set_xlabel("Image width")
         ax[1].set_ylabel("Density")
         # sns.distplot(image_df.width, ax=ax[2])
         ax[2].set_xlabel("Image width")
         ax[2].set_ylabel("Density")
@@ -196,14 +220,16 @@
             ax[i].xaxis.label.set_size(label_size)
             ax[i].yaxis.label.set_size(label_size)
             # tite font size
             ax[i].title.set_size(label_size)
 
         # show the plot
         plt.tight_layout()
+        # save the plot in the figures folder
+        plt.savefig(figure_folder_path / "image_width_height.png")
         plt.show()
 
         # check if there is sort of cluster with respect to the image width
         scaler = StandardScaler()
 
         X = np.log(image_df.width.values).reshape(-1, 1)
         X = scaler.fit_transform(X)
@@ -223,25 +249,38 @@
 
         plt.figure(figsize=figsize_2)
         sns.heatmap(target_leakage, cmap=cmap_2, annot=True)
         plt.title(
             "The cluster_number is related to the classes!\nThis is based on the images width and defined "
             "number of clusters"
         )
+        plt.tight_layout()
+        # save the plot in the figures folder
+        plt.savefig(figure_folder_path / "cluster_number_per_class.png")
         plt.show()
 
-    def plot_data_images(self, num_rows=None, num_cols=None, figsize=(15, 10)):
+    def plot_data_images(
+        self, num_rows=None, num_cols=None, figsize=(15, 10), **kwargs
+    ):
         """
         Plot the images in a grid
         :param num_rows: number of rows in the grid
         :param num_cols: number of columns in the grid
         :param figsize: size of the figure
+        :param kwargs: figure_folder_path
         :return: None
         """
 
+        figure_folder_path = kwargs.get(
+            "figure_folder_path", Path(__file__).parent / ".." / "figures"
+        )
+        # check if the folder exists if not create it
+        if not figure_folder_path.exists():
+            os.makedirs(figure_folder_path)
+
         if not num_rows and not num_cols:
             num_images = len(self.image_df)
             # max_plots = 3 * 5  # Maximum number of plots in a 3x5 grid
             num_rows = math.ceil(num_images / 5)
             num_cols = min(num_images, 5)
         else:
             num_images = num_rows * num_cols
@@ -269,14 +308,16 @@
                     print(
                         f"Skipping image at {filepath}. Unsupported file format: {file_extension}"
                     )
             else:
                 ax.axis("off")  # Turn off the empty subplot
 
         plt.tight_layout()
+        # save the plot in the figures folder
+        plt.savefig(figure_folder_path / "images.png")
         plt.show()
 
     def train_test_split(self, *args, **kwargs):
         """
         Split the data into train and test data
         :param args: arguments for the train_test_split function
         train_size: float, int (default is 0.9)
@@ -487,16 +528,25 @@
                     patience=patience,
                     restore_best_weights=restore_best_weights,
                 )
             ],
         )
         self.model = model
         self.model_history = history
+        # save the model
+        self.model.save(self.model_address)
+
+    def plot_metrics_results(self, **kwargs):
+        figure_folder_path = kwargs.get(
+            "figure_folder_path", Path(__file__).parent / ".." / "figures"
+        )
+        # check if the folder exists if not create it
+        if not figure_folder_path.exists():
+            os.makedirs(figure_folder_path)
 
-    def plot_metrics_results(self):
         # Create subplots with 1 row and 2 columns
         fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(12, 6))
 
         # Plot Accuracy
         axes[0].plot(self.model_history.history["accuracy"])
         axes[0].plot(self.model_history.history["val_accuracy"])
         axes[0].set_title("Accuracy")
@@ -509,14 +559,15 @@
         axes[1].plot(self.model_history.history["val_loss"])
         axes[1].set_title("Loss")
         axes[1].set_xlabel("Epoch")
         axes[1].set_ylabel("Loss")
         axes[1].legend(["Train", "Validation"])
 
         plt.tight_layout()
+        plt.savefig(figure_folder_path / "metrics.png")
         plt.show()
 
     @staticmethod
     def printmd(string):
         # Print with Markdowns
         display(Markdown(string))
 
@@ -534,23 +585,30 @@
         TransferModel.printmd(
             "## Accuracy on the test set: {:.2f}%".format(results[1] * 100)
         )
 
         print(" ## Test Loss: {:.5f}".format(results[0]))
         print("## Accuracy on the test set: {:.2f}%".format(results[1] * 100))
 
-    def predcit_test(self):
+    def predcit_test(self, **kwargs):
         (
             train_generator,
             test_generator,
             train_images,
             val_images,
             test_images,
         ) = self._create_gen()
 
+        figure_folder_path = kwargs.get(
+            "figure_folder_path", Path(__file__).parent / ".." / "figures"
+        )
+        # check if the folder exists if not create it
+        if not figure_folder_path.exists():
+            os.makedirs(figure_folder_path)
+
         # Predict the label of the test_images
         pred = self.model.predict(test_images)
         pred = np.argmax(pred, axis=1)
 
         # Map the label
         labels = train_images.class_indices
         labels = dict((v, k) for k, v in labels.items())
@@ -568,29 +626,19 @@
         sns.heatmap(
             cf_matrix,
             annot=True,
             xticklabels=sorted(set(y_test)),
             yticklabels=sorted(set(y_test)),
         )
         plt.title("Normalized Confusion Matrix")
+        plt.savefig(figure_folder_path / "confusion_matrix.png")
         plt.show()
 
         self.pred = pred
 
-        # # Display some pictures of the dataset with their labels and the predictions
-        # fig, axes = plt.subplots(
-        #     nrows=3, ncols=3, figsize=(15, 15), subplot_kw={"xticks": [], "yticks": []}
-        # )
-        #
-        # for i, ax in enumerate(axes.flat):
-        #     ax.imshow(plt.imread(test_df.Filepath.iloc[i]))
-        #     ax.set_title(f"True: {test_df.Label.iloc[i]}\nPredicted: {pred[i]}")
-        # plt.tight_layout()
-        # plt.show()
-
     def _get_img_array(self, img_path, size):
         img = tf.keras.preprocessing.image.load_img(img_path, target_size=size)
         array = tf.keras.preprocessing.image.img_to_array(img)
         # We add a dimension to transform our array into a "batch"
         # of size "size"
         array = np.expand_dims(array, axis=0)
         return array
@@ -632,17 +680,34 @@
         return heatmap.numpy()
 
     def _save_and_display_gradcam(
         self,
         img_path,
         heatmap,
         cam_name="transf_cam.jpg",
-        cam_path=Path(__file__).parent / ".." / "figures",
         alpha=0.4,
+        **kwargs,
     ):
+        """
+        Args:
+            img_path: path to our image
+            heatmap: the heatmap of our image
+        Keyword Args:
+            cam_name: name of the cam (default: transf_cam.jpg)
+            alpha: the alpha of the cam (default: 0.4)
+            figure_folder_path: the path to the folder where we want to save the cam (default: figures)
+        """
+
+        cam_path = kwargs.get(
+            "figure_folder_path", Path(__file__).parent / ".." / "figures"
+        )
+        # check if the cam_path exists if not create it
+        if not os.path.exists(cam_path):
+            os.makedirs(cam_path)
+
         # Load the original image
         img = tf.keras.preprocessing.image.load_img(img_path)
         img = tf.keras.preprocessing.image.img_to_array(img)
 
         # Rescale heatmap to a range 0-255
         heatmap = np.uint8(255 * heatmap)
 
@@ -667,22 +732,33 @@
 
         # Display Grad CAM
         #     display(Image(cam_path))
 
         return cam_path
 
     def grad_cam_viz(self, *args, **kwargs):
+        """
+        Visualize the Grad-CAM heatmap
+        Keyword Arguments:
+            num_rows {int} -- Number of rows of the subplot grid (default: {None})
+            num_cols {int} -- Number of columns of the subplot grid (default: {None})
+            last_conv_layer_name {str} -- Name of the last convolutional layer (default: {"Conv_1"})
+            img_size {tuple} -- Size of the image (default: {(224, 224)})
+            gard_cam_image_name {str} -- Name of the Grad-CAM image (default: {"transf_cam.jpg"})
+            figsize {tuple} -- Size of the figure (default: {(12, 6)})
+        """
         preprocess_input = tf.keras.applications.mobilenet_v2.preprocess_input
         # decode_predictions = tf.keras.applications.mobilenet_v2.decode_predictions
 
         num_rows = kwargs.get("num_rows", None)
         num_cols = kwargs.get("num_cols", None)
-
-        last_conv_layer_name = "Conv_1"
-        img_size = (224, 224)
+        last_conv_layer_name = kwargs.get("last_conv_layer_name", "Conv_1")
+        img_size = kwargs.get("img_size", (224, 224))
+        gard_cam_image_name = kwargs.get("gard_cam_image_name", "transf_cam.jpg")
+        figsize = kwargs.get("figsize", (8, 6))
 
         # Remove last layer's softmax
         self.model.layers[-1].activation = None
 
         # Display the part of the pictures used by the neural network to classify the pictures
         _, test_df = self.train_test_split()
 
@@ -690,27 +766,27 @@
             # Get the number of rows and columns for subplots
             num_images = len(test_df)
             num_cols = 2
             num_rows = (num_images + num_cols - 1) // num_cols
         else:
             num_images = num_rows * num_cols
 
-        fig, axes = plt.subplots(nrows=num_rows, ncols=num_cols, figsize=(12, 6))
+        fig, axes = plt.subplots(nrows=num_rows, ncols=num_cols, figsize=figsize)
 
         for i, ax in enumerate(axes.flat):
             if i < num_images:
                 img_path = test_df.Filepath.iloc[i]
                 img_array = preprocess_input(
                     self._get_img_array(img_path, size=img_size)
                 )
                 heatmap = self._make_gradcam_heatmap(
                     img_array, self.model, last_conv_layer_name
                 )
                 cam_path = self._save_and_display_gradcam(img_path, heatmap)
-                ax.imshow(plt.imread(cam_path / "transf_cam.jpg"))
+                ax.imshow(plt.imread(cam_path / f"{gard_cam_image_name}"))
                 ax.set_title(
                     f"True: {test_df.Label.iloc[i]}\nPredicted: {self.pred[i]}"
                 )
             else:
                 # Remove unused subplots
                 fig.delaxes(ax)
```

### Comparing `drillvision-0.0.6/pyproject.toml` & `drillvision-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.6/setup.py` & `drillvision-0.1.0/setup.py`

 * *Files identical despite different names*

