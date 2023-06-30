# Comparing `tmp/audio-separator-0.1.3.tar.gz` & `tmp/audio-separator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-separator-0.1.3.tar", last modified: Fri Jun 30 06:57:11 2023, max compression
+gzip compressed data, was "audio-separator-0.1.4.tar", last modified: Fri Jun 30 07:16:45 2023, max compression
```

## Comparing `audio-separator-0.1.3.tar` & `audio-separator-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.062073 audio-separator-0.1.3/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-06-30 05:57:58.000000 audio-separator-0.1.3/LICENSE
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:57:11.061755 audio-separator-0.1.3/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2507 2023-06-30 06:43:31.000000 audio-separator-0.1.3/README.md
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.050662 audio-separator-0.1.3/audio_separator/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:26:40.000000 audio-separator-0.1.3/audio_separator/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    10105 2023-06-30 06:50:36.000000 audio-separator-0.1.3/audio_separator/audio_separator.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.060975 audio-separator-0.1.3/audio_separator/utils/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 05:58:37.000000 audio-separator-0.1.3/audio_separator/utils/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2135 2023-06-30 05:58:37.000000 audio-separator-0.1.3/audio_separator/utils/pyrb.py
--rwxr-xr-x   0 andrew.beveridge   (503) staff       (20)      952 2023-06-30 06:55:53.000000 audio-separator-0.1.3/audio_separator/utils/separate.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    24840 2023-06-30 06:51:10.000000 audio-separator-0.1.3/audio_separator/utils/spec_utils.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.056094 audio-separator-0.1.3/audio_separator.egg-info/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      459 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       72 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/entry_points.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      100 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/requires.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       16 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/top_level.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-30 06:57:11.062134 audio-separator-0.1.3/setup.cfg
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      997 2023-06-30 06:52:06.000000 audio-separator-0.1.3/setup.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.600453 audio-separator-0.1.4/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-06-30 05:57:58.000000 audio-separator-0.1.4/LICENSE
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     3028 2023-06-30 07:16:45.600116 audio-separator-0.1.4/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2614 2023-06-30 07:16:33.000000 audio-separator-0.1.4/README.md
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.587673 audio-separator-0.1.4/audio_separator/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:26:40.000000 audio-separator-0.1.4/audio_separator/__init__.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)    10882 2023-06-30 07:16:33.000000 audio-separator-0.1.4/audio_separator/audio_separator.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.599129 audio-separator-0.1.4/audio_separator/utils/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 05:58:37.000000 audio-separator-0.1.4/audio_separator/utils/__init__.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2135 2023-06-30 05:58:37.000000 audio-separator-0.1.4/audio_separator/utils/pyrb.py
+-rwxr-xr-x   0 andrew.beveridge   (503) staff       (20)     1112 2023-06-30 07:16:33.000000 audio-separator-0.1.4/audio_separator/utils/separate.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)    24840 2023-06-30 06:51:10.000000 audio-separator-0.1.4/audio_separator/utils/spec_utils.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 07:16:45.592276 audio-separator-0.1.4/audio_separator.egg-info/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     3028 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      459 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       72 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/entry_points.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      100 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/requires.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       16 2023-06-30 07:16:45.000000 audio-separator-0.1.4/audio_separator.egg-info/top_level.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-30 07:16:45.600519 audio-separator-0.1.4/setup.cfg
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      997 2023-06-30 07:16:33.000000 audio-separator-0.1.4/setup.py
```

### Comparing `audio-separator-0.1.3/LICENSE` & `audio-separator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.3/PKG-INFO` & `audio-separator-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Audio Separator
 
+[![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
+
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 
 Audio Separator is a Python package that allows you to separate an audio file into two stems, primary and secondary, using a model in the ONNX format trained by @Anjok07 for use with UVR (https://github.com/Anjok07/ultimatevocalremovergui).
 
 The primary stem typically contains the instrumental part of the audio, while the secondary stem contains the vocals, but in some models this is reversed.
 
 ## Features
```

### Comparing `audio-separator-0.1.3/README.md` & `audio-separator-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Audio Separator
 
+[![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
+
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 
 Audio Separator is a Python package that allows you to separate an audio file into two stems, primary and secondary, using a model in the ONNX format trained by @Anjok07 for use with UVR (https://github.com/Anjok07/ultimatevocalremovergui).
 
 The primary stem typically contains the instrumental part of the audio, while the secondary stem contains the vocals, but in some models this is reversed.
 
 ## Features
```

### Comparing `audio-separator-0.1.3/audio_separator/audio_separator.py` & `audio-separator-0.1.4/audio_separator/audio_separator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 from audio_separator.utils import spec_utils
 
 def print_with_timestamp(message):
     timestamp = datetime.datetime.now().isoformat()
     print(f"{timestamp} - {message}")
 
 class Separator:
-    def __init__(self, audio_file, model_name='UVR_MDXNET_KARA_2', output_dir=None):       
-        warnings.filterwarnings("ignore")
-        self.cpu = torch.device('cpu')
+    def __init__(self, audio_file_path, model_name='UVR_MDXNET_KARA_2', model_file_dir='models/', output_dir=None):
+        self.model_name = model_name
+        self.model_file_dir = model_file_dir
+
+        # Create the model directory if it does not exist
+        os.makedirs(self.model_file_dir, exist_ok=True)
 
-        self.audio_file = audio_file
-        self.audio_file_base = os.path.splitext(os.path.basename(audio_file))[0]
+        self.audio_file_path = audio_file_path
+        self.audio_file_base = os.path.splitext(os.path.basename(audio_file_path))[0]
 
         self.model_name = model_name
         self.model_url = f'https://github.com/TRvlvr/model_repo/releases/download/all_public_uvr_models/{self.model_name}.onnx'
+        self.model_data_url = 'https://raw.githubusercontent.com/TRvlvr/application_data/main/mdx_model_data/model_data.json'
         
         self.output_dir = output_dir
 
         self.wav_type_set = "PCM_16"
         self.is_normalization = False
         self.is_denoise = False
 
@@ -39,36 +43,43 @@
         self.adjust = 1
         self.dim_c = 4
         self.hop = 1024
 
         self.primary_source = None
         self.secondary_source = None
 
-        self.device, self.run_type = torch.device('cpu'), ['CPUExecutionProvider']
+        warnings.filterwarnings("ignore")
+        self.cpu = torch.device('cpu')
+        self.device = torch.device('cpu')
+        self.run_type = ['CPUExecutionProvider']
 
     def get_model_hash(self, model_path):
         try:
             with open(model_path, 'rb') as f:
                 f.seek(- 10000 * 1024, 2)
                 return hashlib.md5(f.read()).hexdigest()
         except:
             return hashlib.md5(open(model_path,'rb').read()).hexdigest()
 
     def separate(self):
-        model_path = f'models/{self.model_name}.onnx'
+        model_path = os.path.join(self.model_file_dir, f'{self.model_name}.onnx')
         if not os.path.isfile(model_path):
             print_with_timestamp(f'Model not found at path {model_path}, downloading...')
             wget.download(self.model_url, model_path)
 
         print_with_timestamp('Reading model settings...')
 
         model_hash = self.get_model_hash(model_path)
         print_with_timestamp(f'Model {model_path} has hash {model_hash} ...')
         
-        model_data_path = 'models/model_data.json'
+        model_data_path = os.path.join(self.model_file_dir, 'model_data.json')
+        if not os.path.isfile(model_data_path):
+            print_with_timestamp(f'Model data not found at path {model_data_path}, downloading...')
+            wget.download(self.model_data_url, model_data_path)
+
         model_data_object = json.load(open(model_data_path))
         model_data = model_data_object[model_hash]
         
         self.compensate = model_data["compensate"]
         self.dim_f = model_data["mdx_dim_f_set"]
         self.dim_t = 2**model_data["mdx_dim_t_set"]
         self.n_fft = model_data["mdx_n_fft_scale_set"]
@@ -80,15 +91,15 @@
         print_with_timestamp('Loading model...')
         ort_ = ort.InferenceSession(model_path, providers=self.run_type)
         self.model_run = lambda spek:ort_.run(None, {'input': spek.cpu().numpy()})[0]
 
         self.initialize_model_settings()
         print_with_timestamp('Running inference...')
         mdx_net_cut = True
-        mix, raw_mix, samplerate = prepare_mix(self.audio_file, self.chunks, self.margin, mdx_net_cut=mdx_net_cut)
+        mix, raw_mix, samplerate = prepare_mix(self.audio_file_path, self.chunks, self.margin, mdx_net_cut=mdx_net_cut)
         print_with_timestamp('Demixing...')
         source = self.demix_base(mix)[0]
 
         print_with_timestamp(f'Saving {self.primary_stem} stem...')
         primary_stem_path = os.path.join(f'{self.audio_file_base}_({self.primary_stem})_{self.model_name}.wav')
         if not isinstance(self.primary_source, np.ndarray):
             self.primary_source = spec_utils.normalize(source, self.is_normalization).T
@@ -102,16 +113,18 @@
             self.secondary_source = (-self.secondary_source.T+raw_mix.T)
         self.write_audio(secondary_stem_path, self.secondary_source, samplerate)
 
         torch.cuda.empty_cache()
         return primary_stem_path, secondary_stem_path
 
     def write_audio(self, stem_path, stem_source, samplerate):
-        # If output_dir is specified, join it with stem_path
+        # If output_dir is specified, create it and join it with stem_path
         if self.output_dir:
+            # Create the output directory if it does not exist
+            os.makedirs(self.output_dir, exist_ok=True)
             stem_path = os.path.join(self.output_dir, stem_path)
         
         sf.write(stem_path, stem_source, samplerate, subtype=self.wav_type_set)
 
     def initialize_model_settings(self):
         self.n_bins = self.n_fft//2+1
         self.trim = self.n_fft//2
```

### Comparing `audio-separator-0.1.3/audio_separator/utils/pyrb.py` & `audio-separator-0.1.4/audio_separator/utils/pyrb.py`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.3/audio_separator/utils/separate.py` & `audio-separator-0.1.4/audio_separator/utils/separate.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,20 +9,21 @@
     print(f"{timestamp} - {message}")
 
 
 def main():
     parser = argparse.ArgumentParser(description="Separate audio file into different stems.")
     parser.add_argument("audio_file", help="The WAV audio file path to separate.")
     parser.add_argument("--model_name", default='UVR_MDXNET_KARA_2', help="Optional model name to be used for separation.")
+    parser.add_argument("--model_file_dir", default='/tmp/audio-separator-models/', help="Optional model files directory.")
 
     args = parser.parse_args()
 
     print_with_timestamp(f'Separator beginning with input file: {args.audio_file}')
 
-    separator = Separator(args.audio_file, model_name=args.model_name)
+    separator = Separator(args.audio_file, model_name=args.model_name, model_file_dir=args.model_file_dir)
     primary_stem_path, secondary_stem_path = separator.separate()
 
     print_with_timestamp(f'Separation complete! Output files: {primary_stem_path} {secondary_stem_path}')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `audio-separator-0.1.3/audio_separator/utils/spec_utils.py` & `audio-separator-0.1.4/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.3/audio_separator.egg-info/PKG-INFO` & `audio-separator-0.1.4/audio_separator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Audio Separator
 
+[![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
+
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 
 Audio Separator is a Python package that allows you to separate an audio file into two stems, primary and secondary, using a model in the ONNX format trained by @Anjok07 for use with UVR (https://github.com/Anjok07/ultimatevocalremovergui).
 
 The primary stem typically contains the instrumental part of the audio, while the secondary stem contains the vocals, but in some models this is reversed.
 
 ## Features
```

### Comparing `audio-separator-0.1.3/setup.py` & `audio-separator-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="audio-separator",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
 
     # Metadata
     author="Andrew Beveridge",
     author_email="andrew@beveridge.uk",
     description="Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07",
     long_description=open('README.md').read(),
```

