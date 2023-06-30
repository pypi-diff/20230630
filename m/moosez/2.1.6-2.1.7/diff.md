# Comparing `tmp/moosez-2.1.6.tar.gz` & `tmp/moosez-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.1.6.tar", last modified: Wed Jun 28 16:07:08 2023, max compression
+gzip compressed data, was "moosez-2.1.7.tar", last modified: Fri Jun 30 20:20:06 2023, max compression
```

## Comparing `moosez-2.1.6.tar` & `moosez-2.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:07:08.008209 moosez-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 16:06:58.000000 moosez-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-28 16:07:08.008209 moosez-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-28 16:06:58.000000 moosez-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:07:08.008209 moosez-2.1.6/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-28 16:06:58.000000 moosez-2.1.6/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:07:08.008209 moosez-2.1.6/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-28 16:07:08.000000 moosez-2.1.6/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-28 16:07:08.000000 moosez-2.1.6/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 16:07:08.000000 moosez-2.1.6/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-28 16:07:08.000000 moosez-2.1.6/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-28 16:07:08.000000 moosez-2.1.6/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 16:07:08.000000 moosez-2.1.6/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 16:07:08.008209 moosez-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-28 16:06:58.000000 moosez-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:20:06.167757 moosez-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 20:19:50.000000 moosez-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-30 20:20:06.163757 moosez-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-30 20:19:50.000000 moosez-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:20:06.163757 moosez-2.1.7/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21997 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:20:06.163757 moosez-2.1.7/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:20:06.167757 moosez-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-30 20:19:50.000000 moosez-2.1.7/setup.py
```

### Comparing `moosez-2.1.6/LICENSE` & `moosez-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/PKG-INFO` & `moosez-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.6
+Version: 2.1.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.6/README.md` & `moosez-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/moosez/display.py` & `moosez-2.1.7/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/moosez/download.py` & `moosez-2.1.7/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/moosez/file_utilities.py` & `moosez-2.1.7/moosez/file_utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to perform file operations.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import os
+import glob
 import shutil
 import sys
 from datetime import datetime
 from multiprocessing import Pool
 
 from moosez import constants
 
@@ -66,16 +67,18 @@
     create_directory(moose_dir)
     input_dirs = []
     for modality in modalities:
         input_dirs.append(os.path.join(moose_dir, modality))
         create_directory(input_dirs[-1])
 
     output_dir = os.path.join(moose_dir, constants.SEGMENTATIONS_FOLDER)
+    stats_dir = os.path.join(moose_dir, constants.STATS_FOLDER)
     create_directory(output_dir)
-    return moose_dir, input_dirs, output_dir
+    create_directory(stats_dir)
+    return moose_dir, input_dirs, output_dir, stats_dir
 
 
 def copy_file(file, destination):
     shutil.copy(file, destination)
 
 
 def copy_files_to_destination(files: list, destination: str):
@@ -110,7 +113,19 @@
     :param moose_compliant_subjects: The list of moose-compliant subjects paths.
     :param modalities: The list of modalities.
     :param moose_dir: The path to the moose directory.
     """
     for modality in modalities:
         files_to_copy = select_files_by_modality(moose_compliant_subjects, modality)
         copy_files_to_destination(files_to_copy, os.path.join(moose_dir, modality))
+
+
+def find_pet_file(folder):
+    # Searching for files with 'PET' in their name and ending with either .nii or .nii.gz
+    pet_files = glob.glob(os.path.join(folder, '*PET*.nii*'))
+
+    if len(pet_files) == 1:
+        return pet_files[0]
+    elif len(pet_files) > 1:
+        raise ValueError("More than one PET file found in the directory.")
+    else:
+        return None
```

### Comparing `moosez-2.1.6/moosez/image_conversion.py` & `moosez-2.1.7/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/moosez/image_processing.py` & `moosez-2.1.7/moosez/image_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,46 @@
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import os
 import numpy as np
 import nibabel
 import SimpleITK as sitk
-from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING
+from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING, ORGAN_INDICES
 import dask.array as da
 from mpire import WorkerPool
+import pandas as pd
+
+
+def get_intensity_statistics(image: sitk.Image, mask_image: sitk.Image, model_name: str, out_csv: str) -> None:
+    """
+    Get the intensity statistics of a NIFTI image file
+    :param image: Source image from which the intensity statistics are calculated
+    :param mask_image: Multilabel mask image
+    :param model_name: Name of the model
+    :param out_csv: Path to the output csv file
+    :return None
+     """
+    intensity_statistics = sitk.LabelIntensityStatisticsImageFilter()
+    intensity_statistics.Execute(mask_image, image)
+    stats_list = [(intensity_statistics.GetMean(i), intensity_statistics.GetStandardDeviation(i),
+                   intensity_statistics.GetMedian(i), intensity_statistics.GetMaximum(i),
+                   intensity_statistics.GetMinimum(i)) for i in intensity_statistics.GetLabels()]
+    columns = ['Mean', 'Standard-Deviation', 'Median', 'Maximum', 'Minimum']
+    stats_df = pd.DataFrame(data=stats_list, index=intensity_statistics.GetLabels(), columns=columns)
+    labels_present = stats_df.index.to_list()
+    regions_present = []
+    organ_indices_dict = ORGAN_INDICES[model_name]
+    for label in labels_present:
+        if label in organ_indices_dict:
+            regions_present.append(organ_indices_dict[label])
+        else:
+            continue
+    stats_df.insert(0, 'Regions-Present', np.array(regions_present))
+    stats_df.to_csv(out_csv)
 
 
 def split_and_save(shared_image: tuple, chunk_index: list, image_chunk_path: str) -> None:
     """
     Split the image into chunks and save each part.
 
     Args:
@@ -487,7 +516,31 @@
         image_header['srow_z'] = new_affine[2, :]
 
         resampled_image = nibabel.Nifti1Image(sitk.GetArrayFromImage(resampled_sitk_image).swapaxes(0, 2),
                                               affine=new_affine,
                                               header=image_header)
 
         return resampled_image
+
+    @staticmethod
+    def reslice_identity(reference_image: sitk.Image, moving_image: sitk.Image,
+                         output_image_path: str = None, is_label_image: bool = False) -> sitk.Image:
+        """
+        Reslice an image to the same space as another image
+        :param reference_image: The reference image
+        :param moving_image: The image to reslice to the reference image
+        :param output_image_path: Path to the resliced image
+        :param is_label_image: Determines if the image is a label image. Default is False
+        """
+        resampler = sitk.ResampleImageFilter()
+        resampler.SetReferenceImage(reference_image)
+
+        if is_label_image:
+            resampler.SetInterpolator(sitk.sitkNearestNeighbor)
+        else:
+            resampler.SetInterpolator(sitk.sitkLinear)
+
+        resampled_image = resampler.Execute(moving_image)
+        resampled_image = sitk.Cast(resampled_image, sitk.sitkInt32)
+        if output_image_path is not None:
+            sitk.WriteImage(resampled_image, output_image_path)
+        return resampled_image
```

### Comparing `moosez-2.1.6/moosez/input_validation.py` & `moosez-2.1.7/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/moosez/moosez.py` & `moosez-2.1.7/moosez/moosez.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 # The main function in this module is executed when the mooseZ is run.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import argparse
 import logging
 import os
+import glob
 import time
 from datetime import datetime
 
+import SimpleITK
 import colorama
 from halo import Halo
 
 from moosez import constants
 from moosez import display
 from moosez import download
 from moosez import file_utilities
 from moosez import image_conversion
 from moosez import input_validation
 from moosez import predict
 from moosez import resources
+from moosez.image_processing import ImageResampler
+from moosez import image_processing
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s', level=logging.INFO,
                     filename=datetime.now().strftime('moosez-v.2.0.0.%H-%M-%d-%m-%Y.log'),
                     filemode='w')
 
 
 def main():
@@ -130,23 +134,22 @@
     logging.info(' PERFORMING PREDICTION:')
     logging.info(' ')
 
     spinner = Halo(text=' Initiating', spinner='dots')
     spinner.start()
     start_total_time = time.time()
     for subject in moose_compliant_subjects:
-
         # SETTING UP DIRECTORY STRUCTURE
         spinner.text = f' Setting up directory structure for {os.path.basename(subject)}...'
         logging.info(' ')
         logging.info(f'{constants.ANSI_VIOLET} SETTING UP MOOSE-Z DIRECTORY:'
                      f'{constants.ANSI_RESET}')
         logging.info(' ')
-        moose_dir, input_dirs, output_dir = file_utilities.moose_folder_structure(subject, model_name,
-                                                                                  modalities)
+        moose_dir, input_dirs, output_dir, stats_dir = file_utilities.moose_folder_structure(subject, model_name,
+                                                                                             modalities)
         logging.info(f" MOOSE directory for subject {os.path.basename(subject)} at: {moose_dir}")
 
         # ORGANISE DATA ACCORDING TO MODALITY
         spinner.text = f' Organising data according to modality for {os.path.basename(subject)}...'
         file_utilities.organise_files_by_modality([subject], modalities, moose_dir)
 
         # PREPARE THE DATA FOR PREDICTION
@@ -168,14 +171,33 @@
         logging.info(f"Prediction complete using {model_name}.")
 
         end_time = time.time()
         elapsed_time = end_time - start_time
         spinner.text = f' {constants.ANSI_GREEN}Prediction done for {os.path.basename(subject)} using {model_name}!' \
                        f' | Elapsed time: {round(elapsed_time / 60, 1)} min{constants.ANSI_RESET}'
         time.sleep(3)
+
+        # ----------------------------------
+        # EXTRACT PET ACTIVITY
+        # ----------------------------------
+        pet_file = file_utilities.find_pet_file(subject)
+        if pet_file is not None:
+            pet_image = SimpleITK.ReadImage(pet_file)
+            spinner.text = f' Extracting PET activity for {os.path.basename(subject)}...'
+            multilabel_file = glob.glob(os.path.join(output_dir, constants.MULTILABEL_SUFFIX + '*nii*'))[0]
+            multilabel_image = SimpleITK.ReadImage(multilabel_file)
+            resampled_multilabel_image = ImageResampler.reslice_identity(reference_image=pet_image,
+                                                                         moving_image=multilabel_image,
+                                                                         is_label_image=True)
+            out_csv = os.path.join(stats_dir, os.path.basename(subject) + '_pet_activity.csv')
+            image_processing.get_intensity_statistics(pet_image, resampled_multilabel_image, model_name, out_csv)
+            spinner.text = f'{constants.ANSI_GREEN} PET activity extracted for {os.path.basename(subject)}! ' \
+                           f'{constants.ANSI_RESET}'
+            time.sleep(3)
+
     end_total_time = time.time()
     total_elapsed_time = (end_total_time - start_total_time) / 60
     time_per_dataset = total_elapsed_time / len(moose_compliant_subjects)
 
     spinner.succeed(f'{constants.ANSI_GREEN} All predictions done! | Total elapsed time for '
                     f'{len(moose_compliant_subjects)} datasets: {round(total_elapsed_time, 1)} min'
                     f' | Time per dataset: {round(time_per_dataset, 2)} min {constants.ANSI_RESET}')
```

### Comparing `moosez-2.1.6/moosez/predict.py` & `moosez-2.1.7/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/moosez/resources.py` & `moosez-2.1.7/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.6/moosez.egg-info/PKG-INFO` & `moosez-2.1.7/moosez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.6
+Version: 2.1.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.6/setup.py` & `moosez-2.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.1.6',
+    version='2.1.7',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
@@ -46,14 +46,15 @@
         'matplotlib',
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
         'pillow>=9.2.0',
         'colorama~=0.4.6',
         'dask~=2023.6.0',
         'rich',
+        'pandas',
         'dicom2nifti~=2.4.8'
     ],
     entry_points={
         'console_scripts': [
             'moosez=moosez.moosez:main',
         ],
     },
```

