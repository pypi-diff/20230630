# Comparing `tmp/get_eyedata-1.2.2-py3-none-any.whl.zip` & `tmp/get_eyedata-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5908 bytes, number of entries: 9
+Zip file size: 6441 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-05 08:24 get_eyedata/__init__.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-Jun-28 06:35 get_eyedata/frame_utils.py
+-rw-rw-rw-  2.0 fat     2340 b- defN 23-Jun-30 06:07 get_eyedata/frame_utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 08:24 get_eyedata/ow2.py
--rw-rw-rw-  2.0 fat     3871 b- defN 23-Jun-28 06:35 get_eyedata/valo.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-28 07:53 get_eyedata-1.2.2.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     1869 b- defN 23-Jun-28 07:53 get_eyedata-1.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-28 07:53 get_eyedata-1.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-28 07:53 get_eyedata-1.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      714 b- defN 23-Jun-28 07:53 get_eyedata-1.2.2.dist-info/RECORD
-9 files, 10107 bytes uncompressed, 4672 bytes compressed:  53.8%
+-rw-rw-rw-  2.0 fat     5284 b- defN 23-Jun-30 06:28 get_eyedata/valo.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-30 06:35 get_eyedata-1.3.0.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     1869 b- defN 23-Jun-30 06:35 get_eyedata-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 06:35 get_eyedata-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-30 06:35 get_eyedata-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      714 b- defN 23-Jun-30 06:35 get_eyedata-1.3.0.dist-info/RECORD
+9 files, 11408 bytes uncompressed, 5205 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: get_eyedata/ow2.py
 Comment: 
 
 Filename: get_eyedata/valo.py
 Comment: 
 
-Filename: get_eyedata-1.2.2.dist-info/LICENCE
+Filename: get_eyedata-1.3.0.dist-info/LICENCE
 Comment: 
 
-Filename: get_eyedata-1.2.2.dist-info/METADATA
+Filename: get_eyedata-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: get_eyedata-1.2.2.dist-info/WHEEL
+Filename: get_eyedata-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: get_eyedata-1.2.2.dist-info/top_level.txt
+Filename: get_eyedata-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: get_eyedata-1.2.2.dist-info/RECORD
+Filename: get_eyedata-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## get_eyedata/frame_utils.py

```diff
@@ -1,9 +1,11 @@
 import cv2
 import numpy as np
+from moviepy.editor import VideoFileClip
+import os
 
 #1と0で表現されたバイナリイメージに書き換える関数
 def binarize_image(image):
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
     _, binary = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
     binary_array = np.where(binary == 0, 0, 1)
     return binary_array
@@ -44,23 +46,14 @@
     else:
         # 動画を上下で半分に分割
         top_half = image[:2160 // 2, :]
         bottom_half = image[2160 // 2:, :]
     
     return top_half,bottom_half
 
-from moviepy.editor import VideoFileClip
-import os
-
-from moviepy.editor import VideoFileClip
-import os
-
-from moviepy.editor import VideoFileClip
-import os
-
 def make_displayonly_video(video_path:str, output_dir:str='displayonly_video'):
     clip = VideoFileClip(video_path)
     cropped_clip = clip.crop(y1=0, y2=clip.h // 2)  # cropping the upper half of the video
     
     os.makedirs(output_dir, exist_ok=True)  # create the directory if it doesn't exist
     
     output_path = os.path.join(output_dir, os.path.basename(video_path))
```

## get_eyedata/valo.py

```diff
@@ -1,14 +1,17 @@
 from .frame_utils import cog, sep_y, binarize_image, make_displayonly_video
-import os 
 import cv2
-from tqdm import tqdm
 import numpy as np
 import pandas as pd
 from dataclasses import dataclass
+from queue import Queue
+from threading import Thread
+from concurrent.futures import ProcessPoolExecutor, as_completed
+from tqdm import tqdm
+import os
 
 
 @dataclass
 class Area:
     name: str
     top_x: int
     top_y: int
@@ -61,14 +64,24 @@
 def check(file_path:str):
     if os.path.exists(file_path):
         return True
     else:
         print('FileNotFoundError')
         return False
 
+#フレームの読み込みと画像処理の並列化
+def frame_reader(cap, queue):
+    while True:
+        ret, frame = cap.read()
+        if not ret:
+            print('ret is False')
+            break
+        queue.put(frame)
+    queue.put(None)  # signal that all frames have been read
+
 def make_dataset(video_path:str, save:bool = True, get_display:bool = True):
     #動画の読み込み
     mov_file = os.path.normpath(video_path)
     check(mov_file)
     cap = cv2.VideoCapture(mov_file)
     total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     print(f'total_frames:{total_frames}')
@@ -99,15 +112,32 @@
             frame_ids.append(frame_id)
         else:
             print(f'error occurd at frame{frame_id}')
             break   
     cap.release()
     df = pd.DataFrame({'frame_ids':frame_ids,'x':eye_x,'y':eye_y,'roi':rois})
     if save:
-        df.to_csv('eye_data.csv',index=False)
+        # Get the base name of the video file and use it to create csv filename
+        base_name = os.path.basename(video_path)
+        file_name, _ = os.path.splitext(base_name)
+        df.to_csv(f'{file_name}.csv',index=False)
     if get_display:
         make_displayonly_video(video_path)
     return df
 
+def make_dataset_from_folder(folder_path:str, max_workers:int = 4, save:bool = True, get_display:bool = True):
+    # Get a list of all video files in the folder
+    video_files = [f for f in os.listdir(folder_path) if f.endswith('.mp4') or f.endswith('.mkv')]
+
+    video_files = [os.path.join(folder_path, f) for f in video_files]
+
+    with ProcessPoolExecutor(max_workers=max_workers) as executor:
+        # Create a list to hold the Future objects
+        futures = [executor.submit(make_dataset, video_file, save, get_display) for video_file in video_files]
+
+        # Use tqdm for progress bar
+        for future in tqdm(as_completed(futures), total=len(futures)):
+            # Results are ready only when processing is complete, so we don't need to do anything here
+            pass
 if __name__ == "__main__":
     df = make_dataset('F:\git-repo\get_eyedata\data\test.mkv')
     print(df)
```

## Comparing `get_eyedata-1.2.2.dist-info/LICENCE` & `get_eyedata-1.3.0.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `get_eyedata-1.2.2.dist-info/METADATA` & `get_eyedata-1.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-eyedata
-Version: 1.2.2
+Version: 1.3.0
 Summary: gat gaze data form record.
 Home-page: https://github.com/ikrfun/get_eyedata
 Download-URL: https://github.com/ikrfun/get_eyedata
 Author: ikrfun
 Author-email: t.nobuto130625@gmail.com
 Maintainer: ikrfun
 Maintainer-email: t.nobuto130625@gmail.com
```

## Comparing `get_eyedata-1.2.2.dist-info/RECORD` & `get_eyedata-1.3.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 get_eyedata/__init__.py,sha256=rqUtJyMLicobcyhmr74TepjmUQAEmlazKT3vjV_n3aA,6
-get_eyedata/frame_utils.py,sha256=t-mazRo1bOlR9TqUGLnJJKesVewPyyQpxfC8u9loeBk,2452
+get_eyedata/frame_utils.py,sha256=YEFiSBzqLeJ12s0KBDzxYVdloB45AgOQrJxU-xGM1Y8,2340
 get_eyedata/ow2.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-get_eyedata/valo.py,sha256=fuaFnwBjdVxHHgDHIfPnhY4ulGesBKH63CdNxMfSfXE,3871
-get_eyedata-1.2.2.dist-info/LICENCE,sha256=44r0hK-BnpFZTBiPxTYe52HFlT034sEPBfHrJyaNI0g,1091
-get_eyedata-1.2.2.dist-info/METADATA,sha256=wVGH4Xu3Zazvbtf4QRsVP2sTzS13i2S4EKxv_7v75F4,1869
-get_eyedata-1.2.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-get_eyedata-1.2.2.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
-get_eyedata-1.2.2.dist-info/RECORD,,
+get_eyedata/valo.py,sha256=9NAJFBDHIoHGKbvwIL_5QWDtxheWg_3LPjMBxU5sdEA,5284
+get_eyedata-1.3.0.dist-info/LICENCE,sha256=44r0hK-BnpFZTBiPxTYe52HFlT034sEPBfHrJyaNI0g,1091
+get_eyedata-1.3.0.dist-info/METADATA,sha256=VJNPaCcUK2HuzcGrZKL176xgfcPP0kd0OvUkYC84ieE,1869
+get_eyedata-1.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+get_eyedata-1.3.0.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
+get_eyedata-1.3.0.dist-info/RECORD,,
```

