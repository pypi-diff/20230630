# Comparing `tmp/jcmutils-1.6.6.tar.gz` & `tmp/jcmutils-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.6.6.tar", last modified: Thu Jun 29 08:40:57 2023, max compression
+gzip compressed data, was "jcmutils-1.6.7.tar", last modified: Fri Jun 30 01:48:31 2023, max compression
```

## Comparing `jcmutils-1.6.6.tar` & `jcmutils-1.6.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:40:56.999254 jcmutils-1.6.6/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.6/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:40:56.999254 jcmutils-1.6.6/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.6/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:40:56.999254 jcmutils-1.6.6/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.6/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    17940 2023-06-29 08:38:54.000000 jcmutils-1.6.6/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.6/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.6/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.6/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:40:56.999254 jcmutils-1.6.6/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:40:56.999254 jcmutils-1.6.6/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-29 08:39:05.000000 jcmutils-1.6.6/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 01:48:31.966041 jcmutils-1.6.7/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.7/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-30 01:48:31.966041 jcmutils-1.6.7/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.7/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 01:48:31.966041 jcmutils-1.6.7/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.7/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    17686 2023-06-30 01:46:56.000000 jcmutils-1.6.7/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.7/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.7/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.7/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 01:48:31.966041 jcmutils-1.6.7/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-30 01:48:31.000000 jcmutils-1.6.7/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-30 01:48:31.000000 jcmutils-1.6.7/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-30 01:48:31.000000 jcmutils-1.6.7/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-30 01:48:31.000000 jcmutils-1.6.7/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-30 01:48:31.000000 jcmutils-1.6.7/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-30 01:48:31.966041 jcmutils-1.6.7/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-30 01:47:10.000000 jcmutils-1.6.7/setup.py
```

### Comparing `jcmutils-1.6.6/LICENSE` & `jcmutils-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.6/README.md` & `jcmutils-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.6/jcmutils/dataset_utils.py` & `jcmutils-1.6.7/jcmutils/dataset_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,32 +82,28 @@
         # 合并最终结果
         vmaxa = np.max(total_results) if vmax is None else vmax
         afield = (total_results/ vmaxa)*235
         afield = np.rot90(afield)
 
         (output_image,(xpos,ypos,width,height)) = self.__process_image(afield,template_image,signal_level)
         
-        width_lower_border = 0.6*(periodic_x/source_density)/output_image.shape[1]
-        height_lower_border = 0.6*(periodic_y/source_density)/output_image.shape[0]
-        width_lower_warn = 0.9*(periodic_x/source_density)/output_image.shape[1]
-        height_lower_warn = 0.9*(periodic_y/source_density)/output_image.shape[0]
-        width_upper_warn = 1.8*(periodic_x/source_density)/output_image.shape[1]
-        height_upper_warn = 1.8*(periodic_y/source_density)/output_image.shape[0]
-        width_upper_border = 2.5*(periodic_x/source_density)/output_image.shape[1]
-        height_upper_border = 2.5*(periodic_y/source_density)/output_image.shape[0]
+        lower_border = 0.9*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
+        lower_warn = 1.3*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
+        upper_warn = 1.9*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
+        upper_border = 2.3*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
         # 大致检测结果正确性
-        if width <=width_lower_border or height <=height_lower_border :
-            logger.error(f"false mixed image detected,key-{self.origin_key} was detected too small width or height. the width is {width},height is {height},which is smaller than ({width_lower_border},{height_lower_border}) , try a smaller signal_level")
+        if width <=lower_border or height <=lower_border :
+            logger.error(f"false mixed image detected,key-{self.origin_key} was detected too small width or height. the width is {width},height is {height},which is smaller than ({lower_border},{lower_border}) , try a smaller signal_level")
             raise Exception("error detected , please read log")
-        if width <= width_lower_warn or height <=height_lower_warn:
-            logger.warning(f"key-{self.origin_key} mixed image smaller than ({width_lower_warn},{height_lower_warn}) maybe a little bit strage , please check")
-        if width >= width_upper_warn or height >= height_upper_warn:
-            logger.warning(f"key-{self.origin_key} mixed image lagger than ({width_upper_warn},{height_upper_warn}) maybe a little bit strage , please check")
-        if width >= width_upper_border or height >= height_upper_border:
-            logger.error(f"false mixed image detected,key-{self.origin_key} was detected too big width or height. the width is {width},height is {height},which is larger than ({width_upper_border},{height_upper_border}), try a larger signal_level")
+        if width <= lower_warn or height <=lower_warn:
+            logger.warning(f"key-{self.origin_key} mixed image smaller than ({lower_warn},{lower_warn}) maybe a little bit strage , please check")
+        if width >= upper_warn or height >= upper_warn:
+            logger.warning(f"key-{self.origin_key} mixed image lagger than ({upper_warn},{upper_warn}) maybe a little bit strage , please check")
+        if width >= upper_border or height >= upper_border:
+            logger.error(f"false mixed image detected,key-{self.origin_key} was detected too big width or height. the width is {width},height is {height},which is larger than ({upper_border},{upper_border}), try a larger signal_level")
             raise Exception("error detected , please read log")
             
 
         # #####
         # 重要
         # ! 在此行开始，进行数据增广处理
         # ! 增广方式为：
@@ -115,15 +111,15 @@
         # ! 旋转出图
         # ! 添加噪声
         ###########
 
         # 1.微位移
         image_size = output_image.shape
         stored_images = []
-        move_length = np.linspace(0,4,3)
+        move_length = np.linspace(0,target_density/source_density,3,endpoint=False)
         for i in range(len(move_length)):
             for j in range(len(move_length)):
                 M = np.array([[1,0,i],[0,1,j]],dtype=np.float32)
                 stored_images.append(cv2.warpAffine(output_image,M,output_image.shape))
 
         for i in range(len(stored_images)):
             stored_images[i] = stored_images[i][5:image_size[0]-5,5:image_size[1]-5]
@@ -177,15 +173,15 @@
                 f.write(f"{defect_class} {final_positions[i][0]} {final_positions[i][1]} {final_positions[i][2]} {final_positions[i][3]}")
             cv2.imwrite(file_name,final_images[i])
 
         # 绘图
         logger.debug(f"printing max value of results:{np.max(total_results)}")
         logger.info("all target image saved completed!")
         
-    def __process_image(self,defect_img,template_img,signal_level,smooth_length=30,extend_length = 15):
+    def __process_image(self,defect_img,template_img,signal_level,smooth_length=15,extend_length = 7):
         diff_img = defect_img.astype(np.float32) - template_img.astype(np.float32)
         image_shape = template_img.shape
         # diff_img = (diff_img + 125)
         # diff_img = np.clip(diff_img, 0, 255).astype(np.uint8)
 
         gradX = cv2.Sobel(diff_img, ddepth=cv2.CV_32F, dx=1, dy=0, ksize=-1)
         gradY = cv2.Sobel(diff_img, ddepth=cv2.CV_32F, dx=0, dy=1, ksize=-1)
@@ -285,15 +281,15 @@
                     min_distance = min(distances)
                     min_distance2 = min(distances2)
                     # output_img[j,i] = 255
                     output_img[j,i] += diff_img[j,i]* (min_distance2)/(min_distance + min_distance2)
         xpos = (x + w/2)/image_shape[1]
         ypos = (y + h/2)/image_shape[0]
         width = w/image_shape[1]
-        height = h/image_shape[1]
+        height = h/image_shape[0]
         return (output_img,(xpos,ypos,width,height))
 
     # def export_database_old(self, num_of_result, source_density, target_density,target_filename, vmax, is_light_intense=True, is_symmetry=False):
     #     # 开始提取
     #     # 先确定total_result的形状
     #     temp_result = self.resultbag.get_result(self.keys[0])
     #     field = (temp_result[num_of_result]['field'][0].conj() *
```

### Comparing `jcmutils-1.6.6/jcmutils/gen_sources.py` & `jcmutils-1.6.7/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.6/jcmutils/logger.py` & `jcmutils-1.6.7/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.6/jcmutils/solver.py` & `jcmutils-1.6.7/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.6/setup.py` & `jcmutils-1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.6.6'
+VERSION = '1.6.7'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

