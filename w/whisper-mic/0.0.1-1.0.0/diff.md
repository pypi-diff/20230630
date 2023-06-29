# Comparing `tmp/whisper_mic-0.0.1.tar.gz` & `tmp/whisper_mic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_mic-0.0.1.tar", last modified: Fri Apr 21 06:22:46 2023, max compression
+gzip compressed data, was "whisper_mic-1.0.0.tar", last modified: Thu Jun 29 19:55:47 2023, max compression
```

## Comparing `whisper_mic-0.0.1.tar` & `whisper_mic-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-04-21 06:22:46.915300 whisper_mic-0.0.1/
--rw-rw-r--   0 blake     (1000) blake     (1000)     2853 2023-04-21 06:22:46.915300 whisper_mic-0.0.1/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)     2551 2023-04-21 05:22:07.000000 whisper_mic-0.0.1/README.md
--rw-rw-r--   0 blake     (1000) blake     (1000)      809 2023-04-21 06:06:07.000000 whisper_mic-0.0.1/pyproject.toml
--rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-04-21 06:22:46.915300 whisper_mic-0.0.1/setup.cfg
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-04-21 06:22:46.911300 whisper_mic-0.0.1/whisper_mic/
--rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-0.0.1/whisper_mic/__init__.py
--rwxrwxrwx   0 blake     (1000) blake     (1000)     3450 2023-04-21 06:04:17.000000 whisper_mic-0.0.1/whisper_mic/cli.py
--rwxrwxrwx   0 blake     (1000) blake     (1000)       85 2023-04-21 06:08:56.000000 whisper_mic-0.0.1/whisper_mic/mic.py
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-04-21 06:22:46.915300 whisper_mic-0.0.1/whisper_mic.egg-info/
--rw-rw-r--   0 blake     (1000) blake     (1000)     2853 2023-04-21 06:22:46.000000 whisper_mic-0.0.1/whisper_mic.egg-info/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)      298 2023-04-21 06:22:46.000000 whisper_mic-0.0.1/whisper_mic.egg-info/SOURCES.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-04-21 06:22:46.000000 whisper_mic-0.0.1/whisper_mic.egg-info/dependency_links.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-04-21 06:22:46.000000 whisper_mic-0.0.1/whisper_mic.egg-info/entry_points.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)      182 2023-04-21 06:22:46.000000 whisper_mic-0.0.1/whisper_mic.egg-info/requires.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-04-21 06:22:46.000000 whisper_mic-0.0.1/whisper_mic.egg-info/top_level.txt
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-06-29 19:55:47.019893 whisper_mic-1.0.0/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     1070 2023-06-29 19:44:37.000000 whisper_mic-1.0.0/LICENSE
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3195 2023-06-29 19:55:47.019893 whisper_mic-1.0.0/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)     2883 2023-06-29 19:44:37.000000 whisper_mic-1.0.0/README.md
+-rw-rw-r--   0 blake     (1000) blake     (1000)      809 2023-06-29 19:55:32.000000 whisper_mic-1.0.0/pyproject.toml
+-rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-06-29 19:55:47.019893 whisper_mic-1.0.0/setup.cfg
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-06-29 19:55:47.019893 whisper_mic-1.0.0/whisper_mic/
+-rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-1.0.0/whisper_mic/__init__.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     1600 2023-06-29 19:44:37.000000 whisper_mic-1.0.0/whisper_mic/cli.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     3640 2023-06-29 19:44:37.000000 whisper_mic-1.0.0/whisper_mic/whisper_mic.py
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-06-29 19:55:47.019893 whisper_mic-1.0.0/whisper_mic.egg-info/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3195 2023-06-29 19:55:47.000000 whisper_mic-1.0.0/whisper_mic.egg-info/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)      314 2023-06-29 19:55:47.000000 whisper_mic-1.0.0/whisper_mic.egg-info/SOURCES.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-06-29 19:55:47.000000 whisper_mic-1.0.0/whisper_mic.egg-info/dependency_links.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-06-29 19:55:47.000000 whisper_mic-1.0.0/whisper_mic.egg-info/entry_points.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)      182 2023-06-29 19:55:47.000000 whisper_mic-1.0.0/whisper_mic.egg-info/requires.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-06-29 19:55:47.000000 whisper_mic-1.0.0/whisper_mic.egg-info/top_level.txt
```

### Comparing `whisper_mic-0.0.1/PKG-INFO` & `whisper_mic-1.0.0/whisper_mic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
-Name: whisper_mic
-Version: 0.0.1
+Name: whisper-mic
+Version: 1.0.0
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Whisper Mic
 This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
 
 ## Video Tutorial
 
 See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
 
+The video is a bit out of date now.  The code is much better now and pip installable
+
 ### Professional Assistance
 
 If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
 
 ## Setup
 
-1. Create a venv of your choice.
-2. Run ```pip install -r requirements.txt```
+Now a pip package!
 
+1. Create a venv of your choice.
+2. Run ```pip install whisper-mic```
 
 ## Available models and languages
 
 There are five model sizes, four with English-only versions, offering speed and accuracy tradeoffs. Below are the names of the available models and their approximate memory requirements and relative speed. 
 
 
 |  Size  | Parameters | English-only model | Multilingual model | Required VRAM | Relative speed |
@@ -39,27 +43,36 @@
 | medium |   769 M    |    `medium.en`     |      `medium`      |     ~5 GB     |      ~2x       |
 | large  |   1550 M   |        N/A         |      `large`       |    ~10 GB     |       1x       |
 
 For English-only applications, the `.en` models tend to perform better, especially for the `tiny.en` and `base.en` models. We observed that the difference becomes less significant for the `small.en` and `medium.en` models.
 
 ## Microphone Demo
 
-You can use the model with a microphone using the ```mic.py``` program.  Use ```-h``` to see flag options.
+You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
 ## Troubleshooting
 
 If you are having issues with the ```mic.py``` not running try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
+## Contributing
+
+Currently, this is just a cli demo.  I forsee that this pip package could become more than that for example:
+
+```python
+from whisper_mic.mic import WhisperMic
+mic = WhisperMic(timeout=5)
+command = mic.listen()
+```
 
 ## License
 
-The code and the model weights of Whisper are released under the MIT License. See their repo for more information.
+The model weights of Whisper are released under the MIT License. See their repo for more information.
 
-The code under this repo is under the AGPL license.  See [LICENSE](LICENSE) for further details.
+This code under this repo is under the MIT license.  See [LICENSE](LICENSE) for further details.
 
 ## Thanks
 Until recently, access to high performing speech to text models was only available through paid serviecs.  With this release, I am excited for the many applications that will come.
```

### Comparing `whisper_mic-0.0.1/README.md` & `whisper_mic-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Whisper Mic
 This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
 
 ## Video Tutorial
 
 See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
 
+The video is a bit out of date now.  The code is much better now and pip installable
+
 ### Professional Assistance
 
 If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
 
 ## Setup
 
-1. Create a venv of your choice.
-2. Run ```pip install -r requirements.txt```
+Now a pip package!
 
+1. Create a venv of your choice.
+2. Run ```pip install whisper-mic```
 
 ## Available models and languages
 
 There are five model sizes, four with English-only versions, offering speed and accuracy tradeoffs. Below are the names of the available models and their approximate memory requirements and relative speed. 
 
 
 |  Size  | Parameters | English-only model | Multilingual model | Required VRAM | Relative speed |
@@ -28,27 +31,36 @@
 | medium |   769 M    |    `medium.en`     |      `medium`      |     ~5 GB     |      ~2x       |
 | large  |   1550 M   |        N/A         |      `large`       |    ~10 GB     |       1x       |
 
 For English-only applications, the `.en` models tend to perform better, especially for the `tiny.en` and `base.en` models. We observed that the difference becomes less significant for the `small.en` and `medium.en` models.
 
 ## Microphone Demo
 
-You can use the model with a microphone using the ```mic.py``` program.  Use ```-h``` to see flag options.
+You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
 ## Troubleshooting
 
 If you are having issues with the ```mic.py``` not running try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
+## Contributing
+
+Currently, this is just a cli demo.  I forsee that this pip package could become more than that for example:
+
+```python
+from whisper_mic.mic import WhisperMic
+mic = WhisperMic(timeout=5)
+command = mic.listen()
+```
 
 ## License
 
-The code and the model weights of Whisper are released under the MIT License. See their repo for more information.
+The model weights of Whisper are released under the MIT License. See their repo for more information.
 
-The code under this repo is under the AGPL license.  See [LICENSE](LICENSE) for further details.
+This code under this repo is under the MIT license.  See [LICENSE](LICENSE) for further details.
 
 ## Thanks
 Until recently, access to high performing speech to text models was only available through paid serviecs.  With this release, I am excited for the many applications that will come.
```

### Comparing `whisper_mic-0.0.1/pyproject.toml` & `whisper_mic-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whisper_mic"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Blake Mallory", email="blakecmallory@gmail.com" },
 ]
 description = "Whisper for your microphone"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `whisper_mic-0.0.1/whisper_mic.egg-info/PKG-INFO` & `whisper_mic-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
-Name: whisper-mic
-Version: 0.0.1
+Name: whisper_mic
+Version: 1.0.0
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Whisper Mic
 This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
 
 ## Video Tutorial
 
 See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
 
+The video is a bit out of date now.  The code is much better now and pip installable
+
 ### Professional Assistance
 
 If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
 
 ## Setup
 
-1. Create a venv of your choice.
-2. Run ```pip install -r requirements.txt```
+Now a pip package!
 
+1. Create a venv of your choice.
+2. Run ```pip install whisper-mic```
 
 ## Available models and languages
 
 There are five model sizes, four with English-only versions, offering speed and accuracy tradeoffs. Below are the names of the available models and their approximate memory requirements and relative speed. 
 
 
 |  Size  | Parameters | English-only model | Multilingual model | Required VRAM | Relative speed |
@@ -39,27 +43,36 @@
 | medium |   769 M    |    `medium.en`     |      `medium`      |     ~5 GB     |      ~2x       |
 | large  |   1550 M   |        N/A         |      `large`       |    ~10 GB     |       1x       |
 
 For English-only applications, the `.en` models tend to perform better, especially for the `tiny.en` and `base.en` models. We observed that the difference becomes less significant for the `small.en` and `medium.en` models.
 
 ## Microphone Demo
 
-You can use the model with a microphone using the ```mic.py``` program.  Use ```-h``` to see flag options.
+You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
 ## Troubleshooting
 
 If you are having issues with the ```mic.py``` not running try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
+## Contributing
+
+Currently, this is just a cli demo.  I forsee that this pip package could become more than that for example:
+
+```python
+from whisper_mic.mic import WhisperMic
+mic = WhisperMic(timeout=5)
+command = mic.listen()
+```
 
 ## License
 
-The code and the model weights of Whisper are released under the MIT License. See their repo for more information.
+The model weights of Whisper are released under the MIT License. See their repo for more information.
 
-The code under this repo is under the AGPL license.  See [LICENSE](LICENSE) for further details.
+This code under this repo is under the MIT license.  See [LICENSE](LICENSE) for further details.
 
 ## Thanks
 Until recently, access to high performing speech to text models was only available through paid serviecs.  With this release, I am excited for the many applications that will come.
```

