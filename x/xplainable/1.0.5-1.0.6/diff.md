# Comparing `tmp/xplainable-1.0.5-py3-none-any.whl.zip` & `tmp/xplainable-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,19 @@
-Zip file size: 150014 bytes, number of entries: 70
+Zip file size: 157832 bytes, number of entries: 77
+-rw-r--r--  2.0 unx     1291 b- defN 23-May-31 05:28 docs/conf.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 05:28 tests/__init__.py
--rw-r--r--  2.0 unx      488 b- defN 23-Jun-14 12:55 xplainable/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-19 10:32 xplainable/_version.py
+-rw-r--r--  2.0 unx      786 b- defN 23-Jun-30 15:43 xplainable/__init__.py
+-rw-r--r--  2.0 unx     1553 b- defN 23-Jun-30 15:43 xplainable/_dependencies.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-30 15:43 xplainable/_version.py
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-30 15:43 xplainable/config.py
 -rw-r--r--  2.0 unx       27 b- defN 23-May-31 05:28 xplainable/callbacks/__init__.py
 -rw-r--r--  2.0 unx     3705 b- defN 23-Jun-14 12:55 xplainable/callbacks/optimisation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 05:28 xplainable/client/__init__.py
--rw-r--r--  2.0 unx    24071 b- defN 23-Jun-19 10:32 xplainable/client/client.py
--rw-r--r--  2.0 unx     3067 b- defN 23-Jun-14 12:55 xplainable/client/init.py
+-rw-r--r--  2.0 unx    24282 b- defN 23-Jun-30 15:43 xplainable/client/client.py
+-rw-r--r--  2.0 unx     3179 b- defN 23-Jun-30 15:43 xplainable/client/init.py
 -rw-r--r--  2.0 unx       21 b- defN 23-May-31 05:28 xplainable/core/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 23-May-31 05:28 xplainable/core/models.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 05:28 xplainable/core/ml/__init__.py
 -rw-r--r--  2.0 unx    12946 b- defN 23-Jun-14 12:55 xplainable/core/ml/_base_model.py
 -rw-r--r--  2.0 unx    10063 b- defN 23-Jun-14 12:55 xplainable/core/ml/_constructor.py
 -rw-r--r--  2.0 unx    25955 b- defN 23-Jun-19 10:32 xplainable/core/ml/classification.py
 -rw-r--r--  2.0 unx    18856 b- defN 23-Jun-14 12:55 xplainable/core/ml/regression.py
@@ -18,55 +21,59 @@
 -rw-r--r--  2.0 unx    22545 b- defN 23-Jun-14 12:55 xplainable/core/nlp/feature_extraction.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 05:28 xplainable/core/optimisation/__init__.py
 -rw-r--r--  2.0 unx    14737 b- defN 23-Jun-19 10:32 xplainable/core/optimisation/bayesian.py
 -rw-r--r--  2.0 unx     6000 b- defN 23-Jun-14 12:55 xplainable/core/optimisation/genetic.py
 -rw-r--r--  2.0 unx    21903 b- defN 23-Jun-19 10:32 xplainable/core/optimisation/layers.py
 -rw-r--r--  2.0 unx     6696 b- defN 23-Jun-14 12:55 xplainable/core/optimisation/nlp.py
 -rw-r--r--  2.0 unx     6906 b- defN 23-Jun-14 12:55 xplainable/core/optimisation/targeting.py
--rw-r--r--  2.0 unx       22 b- defN 23-May-31 05:28 xplainable/gui/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 15:43 xplainable/feature_selection/__init__.py
+-rw-r--r--  2.0 unx     5950 b- defN 23-Jun-30 15:43 xplainable/feature_selection/classification.py
+-rw-r--r--  2.0 unx     7771 b- defN 23-Jun-30 15:43 xplainable/feature_selection/graph.py
+-rw-r--r--  2.0 unx     1627 b- defN 23-Jun-30 15:43 xplainable/gui/__init__.py
 -rw-r--r--  2.0 unx      112 b- defN 23-May-31 05:28 xplainable/gui/components/__init__.py
 -rw-r--r--  2.0 unx     6347 b- defN 23-Jun-14 12:55 xplainable/gui/components/bars.py
--rw-r--r--  2.0 unx     4615 b- defN 23-May-31 05:28 xplainable/gui/components/cards.py
+-rw-r--r--  2.0 unx     4588 b- defN 23-Jun-30 15:43 xplainable/gui/components/cards.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-May-31 05:28 xplainable/gui/components/connectivity.py
 -rw-r--r--  2.0 unx     3018 b- defN 23-May-31 05:28 xplainable/gui/components/header.py
 -rw-r--r--  2.0 unx     8784 b- defN 23-Jun-14 12:55 xplainable/gui/components/pipelines.py
 -rw-r--r--  2.0 unx     2848 b- defN 23-May-31 05:28 xplainable/gui/components/tables.py
--rw-r--r--  2.0 unx      100 b- defN 23-May-31 05:28 xplainable/gui/screens/__init__.py
--rw-r--r--  2.0 unx    23982 b- defN 23-Jun-19 10:32 xplainable/gui/screens/classifier.py
--rw-r--r--  2.0 unx    38580 b- defN 23-Jun-14 12:55 xplainable/gui/screens/evaluate.py
--rw-r--r--  2.0 unx    14819 b- defN 23-Jun-14 12:55 xplainable/gui/screens/loader.py
--rw-r--r--  2.0 unx    39855 b- defN 23-Jun-14 12:55 xplainable/gui/screens/preprocessor.py
--rw-r--r--  2.0 unx    19494 b- defN 23-Jun-19 10:32 xplainable/gui/screens/regressor.py
--rw-r--r--  2.0 unx    20280 b- defN 23-Jun-19 10:32 xplainable/gui/screens/save.py
--rw-r--r--  2.0 unx    22064 b- defN 23-Jun-14 12:55 xplainable/gui/screens/scenario.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 15:43 xplainable/gui/screens/__init__.py
+-rw-r--r--  2.0 unx    24102 b- defN 23-Jun-30 15:43 xplainable/gui/screens/classifier.py
+-rw-r--r--  2.0 unx    38580 b- defN 23-Jun-30 08:38 xplainable/gui/screens/evaluate.py
+-rw-r--r--  2.0 unx    15870 b- defN 23-Jun-30 15:43 xplainable/gui/screens/loader.py
+-rw-r--r--  2.0 unx    40125 b- defN 23-Jun-30 15:43 xplainable/gui/screens/preprocessor.py
+-rw-r--r--  2.0 unx    19879 b- defN 23-Jun-30 15:43 xplainable/gui/screens/regressor.py
+-rw-r--r--  2.0 unx    20044 b- defN 23-Jun-30 15:43 xplainable/gui/screens/save.py
+-rw-r--r--  2.0 unx    22064 b- defN 23-Jun-30 08:38 xplainable/gui/screens/scenario.py
 -rw-r--r--  2.0 unx       22 b- defN 23-May-31 05:28 xplainable/metrics/__init__.py
 -rw-r--r--  2.0 unx     6074 b- defN 23-Jun-19 10:32 xplainable/metrics/metrics.py
 -rw-r--r--  2.0 unx       27 b- defN 23-May-31 05:28 xplainable/preprocessing/__init__.py
 -rw-r--r--  2.0 unx     6628 b- defN 23-Jun-14 12:55 xplainable/preprocessing/pipeline.py
 -rw-r--r--  2.0 unx       94 b- defN 23-May-31 05:28 xplainable/preprocessing/transformers/__init__.py
 -rw-r--r--  2.0 unx     3518 b- defN 23-Jun-14 12:55 xplainable/preprocessing/transformers/base.py
--rw-r--r--  2.0 unx    19239 b- defN 23-Jun-14 12:55 xplainable/preprocessing/transformers/categorical.py
--rw-r--r--  2.0 unx    32659 b- defN 23-Jun-14 12:55 xplainable/preprocessing/transformers/dataset.py
--rw-r--r--  2.0 unx     3201 b- defN 23-Jun-14 12:55 xplainable/preprocessing/transformers/mixed.py
--rw-r--r--  2.0 unx     4902 b- defN 23-Jun-14 12:55 xplainable/preprocessing/transformers/numeric.py
+-rw-r--r--  2.0 unx    19977 b- defN 23-Jun-30 15:43 xplainable/preprocessing/transformers/categorical.py
+-rw-r--r--  2.0 unx    33790 b- defN 23-Jun-30 15:43 xplainable/preprocessing/transformers/dataset.py
+-rw-r--r--  2.0 unx     3295 b- defN 23-Jun-30 15:43 xplainable/preprocessing/transformers/mixed.py
+-rw-r--r--  2.0 unx     4998 b- defN 23-Jun-30 15:43 xplainable/preprocessing/transformers/numeric.py
 -rw-r--r--  2.0 unx       26 b- defN 23-May-31 05:28 xplainable/quality/__init__.py
--rw-r--r--  2.0 unx    10927 b- defN 23-Jun-14 12:55 xplainable/quality/scanner.py
--rw-r--r--  2.0 unx       69 b- defN 23-May-31 05:28 xplainable/utils/__init__.py
+-rw-r--r--  2.0 unx     8928 b- defN 23-Jun-30 15:43 xplainable/quality/scanner.py
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-30 15:43 xplainable/utils/__init__.py
 -rw-r--r--  2.0 unx      391 b- defN 23-Jun-14 12:55 xplainable/utils/activation.py
 -rw-r--r--  2.0 unx     1063 b- defN 23-Jun-14 11:16 xplainable/utils/api.py
 -rw-r--r--  2.0 unx     2209 b- defN 23-May-31 05:28 xplainable/utils/collections.py
 -rw-r--r--  2.0 unx      810 b- defN 23-May-31 05:28 xplainable/utils/encoders.py
 -rw-r--r--  2.0 unx      226 b- defN 23-May-31 05:28 xplainable/utils/exceptions.py
--rw-r--r--  2.0 unx     1393 b- defN 23-Jun-14 12:55 xplainable/utils/handlers.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Jun-30 15:43 xplainable/utils/handlers.py
 -rw-r--r--  2.0 unx     2111 b- defN 23-May-31 05:28 xplainable/utils/loaders.py
 -rw-r--r--  2.0 unx     1158 b- defN 23-May-31 05:28 xplainable/utils/numba_funcs.py
 -rw-r--r--  2.0 unx     4906 b- defN 23-Jun-14 12:55 xplainable/utils/svgs.py
--rw-r--r--  2.0 unx     9759 b- defN 23-May-31 05:28 xplainable/utils/xwidgets.py
+-rw-r--r--  2.0 unx    10052 b- defN 23-Jun-30 15:43 xplainable/utils/xwidgets.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 05:28 xplainable/visualisation/__init__.py
--rw-r--r--  2.0 unx     4380 b- defN 23-Jun-14 12:55 xplainable/visualisation/explain.py
+-rw-r--r--  2.0 unx     4693 b- defN 23-Jun-30 15:43 xplainable/visualisation/explain.py
+-rw-r--r--  2.0 unx     2822 b- defN 23-Jun-30 15:43 xplainable/visualisation/network.py
 -rw-r--r--  2.0 unx      387 b- defN 23-May-31 05:28 xplainable/visualisation/regression.py
--rw-r--r--  2.0 unx    34522 b- defN 23-Jun-19 10:32 xplainable-1.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    50058 b- defN 23-Jun-19 10:32 xplainable-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 10:32 xplainable-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-19 10:32 xplainable-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6260 b- defN 23-Jun-19 10:32 xplainable-1.0.5.dist-info/RECORD
-70 files, 591209 bytes uncompressed, 139966 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx    34522 b- defN 23-Jun-30 15:43 xplainable-1.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    50581 b- defN 23-Jun-30 15:43 xplainable-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 15:43 xplainable-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-30 15:43 xplainable-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6872 b- defN 23-Jun-30 15:43 xplainable-1.0.6.dist-info/RECORD
+77 files, 615643 bytes uncompressed, 146818 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -1,16 +1,25 @@
+Filename: docs/conf.py
+Comment: 
+
 Filename: tests/__init__.py
 Comment: 
 
 Filename: xplainable/__init__.py
 Comment: 
 
+Filename: xplainable/_dependencies.py
+Comment: 
+
 Filename: xplainable/_version.py
 Comment: 
 
+Filename: xplainable/config.py
+Comment: 
+
 Filename: xplainable/callbacks/__init__.py
 Comment: 
 
 Filename: xplainable/callbacks/optimisation.py
 Comment: 
 
 Filename: xplainable/client/__init__.py
@@ -63,14 +72,23 @@
 
 Filename: xplainable/core/optimisation/nlp.py
 Comment: 
 
 Filename: xplainable/core/optimisation/targeting.py
 Comment: 
 
+Filename: xplainable/feature_selection/__init__.py
+Comment: 
+
+Filename: xplainable/feature_selection/classification.py
+Comment: 
+
+Filename: xplainable/feature_selection/graph.py
+Comment: 
+
 Filename: xplainable/gui/__init__.py
 Comment: 
 
 Filename: xplainable/gui/components/__init__.py
 Comment: 
 
 Filename: xplainable/gui/components/bars.py
@@ -186,26 +204,29 @@
 
 Filename: xplainable/visualisation/__init__.py
 Comment: 
 
 Filename: xplainable/visualisation/explain.py
 Comment: 
 
+Filename: xplainable/visualisation/network.py
+Comment: 
+
 Filename: xplainable/visualisation/regression.py
 Comment: 
 
-Filename: xplainable-1.0.5.dist-info/LICENSE
+Filename: xplainable-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: xplainable-1.0.5.dist-info/METADATA
+Filename: xplainable-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xplainable-1.0.5.dist-info/WHEEL
+Filename: xplainable-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xplainable-1.0.5.dist-info/top_level.txt
+Filename: xplainable-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xplainable-1.0.5.dist-info/RECORD
+Filename: xplainable-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xplainable/__init__.py

```diff
@@ -1,17 +1,23 @@
 from .client.client import Client
 from .gui import *
 from .client.init import initialise, reinitialise
-from .utils.handlers import check_critical_versions
+from . import config
 import warnings
-
-# Ensure critical dependency versions match
-check_critical_versions()
+from ._dependencies import _try_optional_dependencies_gui
 
 __author__ = 'xplainable pty ltd'
 from ._version import __version__
 
+OPTIONAL_DEPENDENCIES_GUI = _try_optional_dependencies_gui()
+
+def _check_optional_dependencies_gui():
+    if not OPTIONAL_DEPENDENCIES_GUI:
+        raise ImportError("Optional dependencies not found. Please install "
+                          "them with `pip install xplainable[gui]' to use "
+                          "this feature.")
+    
 # Filter retry warnings as retries are expected and already handled
 warnings.filterwarnings(
     "ignore", category=UserWarning, module="urllib3.connectionpool")
 
-client = None
+client = None
```

## xplainable/_version.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.5"
+__version__ = "1.0.6"
```

## xplainable/client/client.py

```diff
@@ -1,33 +1,29 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
-
+import json
+import numpy as np
+import pandas as pd
+import pyperclip
+import time
+from IPython.display import clear_output, display
+from .._dependencies import _check_ipywidgets
 from ..utils.api import get_response_content
 from ..utils.encoders import NpEncoder
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from ..gui.screens.preprocessor import Preprocessor
 from ..preprocessing import transformers as xtf
 from ..utils.exceptions import AuthenticationError
-from ..gui.components.cards import render_user_avatar
 from ..quality.scanner import XScan
 from ..metrics.metrics import evaluate_classification, evaluate_regression
 from ..core.models import (XClassifier, XRegressor, PartitionedRegressor,
                            PartitionedClassifier)
 
-import json
-import numpy as np
-import pandas as pd
-import pyperclip
-import time
-from IPython.display import clear_output, display
-from ..gui.components import KeyValueTable
-import ipywidgets as widgets
-from typing import Union
-import logging
+from ..config import OUTPUT_TYPE
 
 
 class Client:
     """ A client for interfacing with the xplainable web api (xplainable cloud).
 
     Access models, preprocessors and user data from xplainable cloud. API keys
     can be generated at https://app.xplainable.io.
@@ -67,15 +63,21 @@
 
         session_data = self.get_user_data()
         
         self.__org_id = session_data.pop('organisation_id')
         self.__team_id = session_data.pop('team_id')
         self.__ext = f'organisations/{self.__org_id}/teams/{self.__team_id}'
         self._user = session_data
-        self.avatar = render_user_avatar(self._user)
+        
+        try:
+            import ipywidgets
+            from ..gui.components.cards import render_user_avatar
+            self.avatar = render_user_avatar(self._user)
+        except ImportError:
+            pass
 
         self.xplainable_version = None
         self.python_version = None
 
     def list_models(self) -> list:
         """ Lists all models of the active user's team.
 
@@ -597,15 +599,15 @@
 
             data["health_info"] = json.dumps(results, cls=NpEncoder)
 
         return data
 
     def deploy(
             self, hostname: None, model_id: str, version_id: str,
-            partition_id: str, raw_output: bool=False) -> dict:
+            partition_id: str, raw_output: bool=True) -> dict:
         """ Deploys a model partition to xplainable cloud.
 
         The hostname should be the url of the inference server. For example:
         https://inference.xplainable.io
 
         Args:
             hostname (str): The host name for the inference server
@@ -635,16 +637,19 @@
             data = {
                 "deployment_id": deployment_id,
                 "status": "active",
                 "location": "sydney",
                 "endpoint": f"{hostname}/v1/predict"
             }
 
-            if raw_output:
+            if raw_output or OUTPUT_TYPE == 'raw':
                 return data
+            
+            widgets = _check_ipywidgets()
+            from ..gui.components import KeyValueTable
 
             table = KeyValueTable(
                 data,
                 transpose=False,
                 padding="0px 20px 0px 5px",
                 table_width='auto',
                 header_color='#e8e8e8',
@@ -666,15 +671,14 @@
                 except Exception as e:
                     b.description = "Failed. Try Again."
                     b.disabled = True
                     time.sleep(2)
                     b.description = "Generate Deploy Key"
                     b.disabled = False
                 
-
             button = widgets.Button(description="Generate Deploy Key")
             button.on_click(on_click)
 
             output = widgets.HBox([table.html_widget, button])
             display(output)
 
         else:
```

## xplainable/client/init.py

```diff
@@ -1,21 +1,22 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
 from .client import Client
 import xplainable
 from .._version import __version__ as XP_VERSION
-from IPython.display import clear_output
 import sys
 from getpass import getpass
-from ..gui.components import KeyValueTable, Header
 from IPython.display import display, clear_output
 import keyring
 
+from .. import config
+
 def _render_init_table(data):
     import ipywidgets as widgets
+    from ..gui.components import KeyValueTable, Header
     table = KeyValueTable(
         data,
         transpose=False,
         padding="0px 45px 0px 5px",
         table_width='auto',
         header_color='#e8e8e8',
         border_color='#dddddd',
@@ -25,15 +26,15 @@
 
     header = Header('Initialised', 30, 16, avatar=False)
     header.divider.layout.display = 'none'
     header.title = {'margin':'4px 0 0 8px'}
     output = widgets.VBox([header.show(), table.html_widget])
     display(output)
 
-def initialise(hostname='https://api.xplainable.io'):
+def initialise(hostname='https://api.xplainable.io', api_key=None):
     """ Initialise the client with an API Key.
 
     API Keys can be generated from https://app.xplainable.io with a valid
     account.
 
     Example:
         >>> xp.initialise()
@@ -42,15 +43,17 @@
         dict: The users account information.
     """
 
     version_info = sys.version_info
     PY_VERSION = f'{version_info.major}.{version_info.minor}.{version_info.micro}'
     
     has_set = False
-    api_key = keyring.get_password('XPLAINABLE', PY_VERSION)
+    api_key = api_key if api_key else \
+        keyring.get_password('XPLAINABLE', PY_VERSION)
+    
     if not api_key:
         api_key = getpass("Paste a valid API Key: ")
         has_set = True
     
     try:
         xplainable.client = Client(api_key, hostname)
         xplainable.client.xplainable_version = XP_VERSION
@@ -61,14 +64,17 @@
 
         data = {
             "xplainable version": XP_VERSION,
             "python version": PY_VERSION,
             "user": xplainable.client._user['username']
         }
 
+        if config.OUTPUT_TYPE == 'raw':
+            return data
+        
         try:
             _render_init_table(data)
         except:
             return data
 
     except:
         clear_output()
```

## xplainable/gui/__init__.py

```diff
@@ -1 +1,38 @@
-from .screens import *
+
+from .._dependencies import _try_optional_dependencies_gui
+from .screens.preprocessor import Preprocessor
+from .screens.loader import load_preprocessor
+from .screens.loader import load_classifier
+from .screens.loader import load_regressor
+
+def _optional_dependency_placeholder(*args, **kwargs):
+    raise ImportError("Optional dependencies not found. Please install "
+                          "them with `pip install xplainable[gui]' to use "
+                          "this feature.")
+
+class OptionalDependencyPlaceholder:
+
+    def __init__(self):
+        raise ImportError("Optional dependencies not found. Please install "
+                          "them with `pip install xplainable[gui]' to use "
+                          "this feature.")
+
+# import functions and classes as normal if optional dependencies are found
+if _try_optional_dependencies_gui():
+    from .screens.classifier import classifier
+    from .screens.regressor import regressor
+    from .screens.evaluate import EvaluateClassifier, EvaluateRegressor
+    from .screens.save import ModelPersist
+    from .screens.scenario import ScenarioClassification, ScenarioRegression
+
+# otherwise, import placeholder functions and classes
+else:
+    classifier = _optional_dependency_placeholder
+    regressor = _optional_dependency_placeholder
+
+    EvaluateClassifier = OptionalDependencyPlaceholder
+    EvaluateRegressor = OptionalDependencyPlaceholder
+    Preprocessor = OptionalDependencyPlaceholder
+    ModelPersist = OptionalDependencyPlaceholder
+    ScenarioClassification = OptionalDependencyPlaceholder
+    ScenarioRegression = OptionalDependencyPlaceholder
```

## xplainable/gui/components/cards.py

```diff
@@ -1,14 +1,13 @@
-import ipywidgets as widgets
 from IPython.display import display
 import requests
-from IPython.display import display
 from IPython.core.display import HTML
 import base64
 from ...utils.handlers import add_thousands_separator
+import ipywidgets as widgets
 
 
 class CardWidget:
     def __init__(
         self,
         title,
         value,
@@ -34,14 +33,15 @@
         self.value_color = value_color
         self.title_align = title_align
         self.value_align = value_align
 
         self.card = self._create_card()
 
     def _create_card(self):
+        
         card_style = f"""
             background-color: {self.background_color};
             padding: 16px;
             border-radius: {'12px' if self.rounded_edges else '0px'};
             width: {self.card_size};
             box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
         """
```

## xplainable/gui/screens/__init__.py

```diff
@@ -1,7 +0,0 @@
-00000000: 6672 6f6d 202e 636c 6173 7369 6669 6572  from .classifier
-00000010: 2069 6d70 6f72 7420 2a0a 6672 6f6d 202e   import *.from .
-00000020: 7265 6772 6573 736f 7220 696d 706f 7274  regressor import
-00000030: 202a 0a66 726f 6d20 2e70 7265 7072 6f63   *.from .preproc
-00000040: 6573 736f 7220 696d 706f 7274 202a 0a66  essor import *.f
-00000050: 726f 6d20 2e6c 6f61 6465 7220 696d 706f  rom .loader impo
-00000060: 7274 202a                                rt *
```

## xplainable/gui/screens/classifier.py

```diff
@@ -18,14 +18,15 @@
 import time
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 from sklearn.model_selection import train_test_split
 import time
+from ..._dependencies import _check_critical_versions
 
 import os
 os.environ['KMP_WARNINGS'] = '0'
 
 def classifier(df):
     """ Trains an xplainable classifier via a simple GUI.
 
@@ -35,14 +36,17 @@
     Raises:
         RuntimeError: When model fails to fit
 
     Returns:
         xplainale.models.XClassifier: The trained model
     """
 
+    # Check critical dependencies
+    _check_critical_versions()
+
     # Assert dataframe is valid
     check_df(df)
 
     # This allows widgets to show full label text
     style = {'description_width': 'initial'}
 
     # Instantiate widget output
```

## xplainable/gui/screens/loader.py

```diff
@@ -1,17 +1,13 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
 from datetime import datetime
-from .preprocessor import Preprocessor
 import xplainable
-import ipywidgets as widgets
-from IPython.display import display, clear_output
 from ...utils import *
 from ...preprocessing import transformers as xtf
-from ..components import Header
 from ...core.models import PartitionedRegressor, PartitionedClassifier
 
 
 def get_time_string(dt):
         """Get time since object created"""
 
         delt = (datetime.utcnow() - dt)
@@ -33,15 +29,28 @@
             return f'{int(seconds / 60 / 60)} hours ago'
 
 def load_preprocessor(preprocessor_id=None, version_id=None):
 
     if xplainable.client is None:
         print("visit https://www.xplainable.io/sign-up to access this service")
         return
-
+    
+    if preprocessor_id is not None:
+        if version_id is None:
+            raise ValueError(
+                "version_id must be specified if model_id is specified")
+        return xplainable.client.load_preprocessor(preprocessor_id, version_id)
+    
+    # Check if optional dependencies are installed
+    xplainable._check_optional_dependencies_gui()
+    import ipywidgets as widgets
+    from IPython.display import display, clear_output
+    from ..components import Header
+    from .preprocessor import Preprocessor
+    
     def build_transformer(stage):
         """Build transformer from metadata"""
 
         if not hasattr(xtf, stage["name"]):
             raise ValueError(
                 f"{stage['name']} does not exist in the transformers module")
 
@@ -111,18 +120,14 @@
         xp.state = len(xp.pipeline.stages)
         p = preprocessors.preprocessor
         v = preprocessors.metadata[versions.index-1]['version_number']
         vid = preprocessors.metadata[versions.index-1]['version_id']
         clear_output()
         print(f"Successfully loaded preprocessor {p} version {v} (version_id: {vid})")
 
-    if preprocessor_id is not None:
-        version_id = 'latest' if version_id is None else version_id
-        return xplainable.client.load_preprocessor(preprocessor_id, version_id)
-
     # --- HEADER ---
     header = Header(title='Load Preprocessor', logo_size=40, font_size=18)
     header.title = {'margin': '10px 15px 0 10px'}
 
     # --- BODY ---
     # SELECTOR
     # Init Dropdown data
@@ -170,20 +175,32 @@
     display(screen)
 
     # Init preprocessor
     xp = Preprocessor()
 
     return xp
 
-
 def load_regressor(model_id=None, version_id=None):
 
     if xplainable.client is None:
         print("visit https://www.xplainable.io/sign-up to access this service")
         return
+    
+    if model_id is not None:
+        if version_id is None:
+            raise ValueError(
+                "version_id must be specified if model_id is specified")
+        
+        return xplainable.client.load_regressor(model_id, version_id)
+    
+    # Check if optional dependencies are installed
+    xplainable._check_optional_dependencies_gui()
+    import ipywidgets as widgets
+    from IPython.display import display, clear_output
+    from ..components import Header
 
     def on_model_change(_):
         """Loads versions when model is selected"""
 
         if models.value is None:
             load_button.disabled = True
             output_box.layout.display = 'none'
@@ -233,17 +250,14 @@
         vid = models.version_data
         v = versions.metadata[versions.index-1]['version_number']
         
         xplainable.client.load_regressor(m, vid, model=partitioned_model)
         clear_output()
         print(f"Successfully loaded model {m} version {v} (version_id: {vid})")
 
-    if model_id is not None:
-        return xplainable.client.load_model(model_id, version_id)
-
     # --- HEADER ---
     header = Header(title='Load Regressor', logo_size=40, font_size=18)
     header.title = {'margin': '10px 15px 0 10px'}
 
     # --- BODY ---
     # SELECTOR
     # Init Dropdown data
@@ -300,20 +314,32 @@
     display(screen)
 
     # Init model
     partitioned_model = PartitionedRegressor()
 
     return partitioned_model
 
-
 def load_classifier(model_id=None, version_id=None):
 
     if xplainable.client is None:
         print("visit https://www.xplainable.io/sign-up to access this service")
         return
+    
+    if model_id is not None:
+        if version_id is None:
+            raise ValueError(
+                "version_id must be specified if model_id is specified")
+        
+        return xplainable.client.load_classifier(model_id, version_id)
+    
+    # Check if optional dependencies are installed
+    xplainable._check_optional_dependencies_gui()
+    import ipywidgets as widgets
+    from IPython.display import display, clear_output
+    from ..components import Header
 
     def on_model_change(_):
         """Loads versions when model is selected"""
 
         if models.value is None:
             load_button.disabled = True
             output_box.layout.display = 'none'
```

## xplainable/gui/screens/preprocessor.py

```diff
@@ -2,27 +2,20 @@
 
 import xplainable
 from ...utils import *
 from ...preprocessing import transformers as xtf
 from ...quality import XScan
 from ...preprocessing.pipeline import XPipeline
 from ...utils.api import *
-from ...gui.screens import Header
-from .save import PreprocessorPersist
 
 import pandas as pd
-from ipywidgets import interactive
-from IPython.display import display, clear_output
-import ipywidgets as widgets
 import matplotlib.pyplot as plt
 import inspect
 from pandas.api.types import is_numeric_dtype, is_string_dtype
 import pandas.api.types as pdtypes
-import matplotlib.pyplot as plt
-import seaborn as sns
 import pickle
 
 
 class Preprocessor:
 
     def __init__(self):
         
@@ -91,15 +84,28 @@
     def preprocess(self, df):
         """ GUI for easily preprocessing data.
 
         Args:
             df (pandas.DataFrame): Dataframe to preprocess
 
         """
+
+        try:
+            from ..components import Header
+            from .save import PreprocessorPersist
+            from ipywidgets import interactive
+            import ipywidgets as widgets
+            from IPython.display import display, clear_output
+            import matplotlib.pyplot as plt
+            import seaborn as sns
         
+        except:
+            raise ImportError("Optional dependencies not found. Please install "
+                              "them with xplainable[gui] to use the GUI.]")
+
         # // ---------- SUPPORTING FUNCTIONS ---------- //
         def reset_charts():
             """Forces chart value change to trigger refresh"""
             # Chart 1
             v = charts.children[0].children[0].value
             charts.children[0].children[0].value = None
             charts.children[0].children[0].value = v
```

## xplainable/gui/screens/regressor.py

```diff
@@ -1,34 +1,50 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
 from ...core.models import PartitionedRegressor, XRegressor
 from ...core.optimisation.genetic import XEvolutionaryNetwork
 from ...core.optimisation.layers import Tighten, Evolve
 from ...quality import XScan
 from ...gui.components.tables import KeyValueTable 
-from ...gui.screens import Header
+from ..components import Header
 from ...utils.xwidgets import TrainButton
 from ...callbacks.optimisation import RegressionCallback
 from ...gui.components.bars import IncrementalBarPlot
 from ...gui.components.pipelines import VisualPipeline
 from .evaluate import EvaluateRegressor
 from .save import ModelPersist
 from ..components import BarGroup
 from ...metrics.metrics import evaluate_regression
 from ...utils.handlers import check_df
+from ..._dependencies import _check_critical_versions
+
 
 from sklearn.model_selection import train_test_split
 import numpy as np
 import copy
 import time
 import ipywidgets as widgets
 from IPython.display import  display
 from sklearn.metrics import *
 
 def regressor(df):
+    """ Trains an xplainable regressor via a simple GUI.
+
+    Args:
+        df (pandas.DataFrame): Training data including target
+
+    Raises:
+        RuntimeError: When model fails to fit
+
+    Returns:
+        xplainale.models.XRegressor: The trained model
+    """
+
+    # Check critical dependencies
+    _check_critical_versions()
     
     # Assert dataframe is valid
     check_df(df)
 
     style = {'description_width': 'initial'}
     divider = widgets.HTML(f'<hr class="solid">')
```

## xplainable/gui/screens/save.py

```diff
@@ -1,23 +1,16 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
 import xplainable
-from ...utils.api import get_response_content
 from ...utils.xwidgets import TextInput
-from ...core.optimisation.targeting import generate_ruleset
-from ...utils.encoders import NpEncoder, force_json_compliant
-import json
+import time
 
 import ipywidgets as widgets
-from IPython.display import display, clear_output
-
-from xplainable.utils.api import get_response_content
 from xplainable.utils.xwidgets import TextInput
-
-import time
+from IPython.display import display, clear_output
 
 
 class ModelPersist:
     
     def __init__(self, model, model_type, X, y):
 
         self.model = model
```

## xplainable/preprocessing/transformers/categorical.py

```diff
@@ -1,18 +1,16 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
-from ...utils import stopwords, xwidgets
+from ...utils import stopwords
 
 from .base import XBaseTransformer
 from pandas.api.types import is_string_dtype
-from ipywidgets import interactive
 import re
 import numpy as np
 import pandas as pd
-import ipywidgets as widgets
 
 
 class TextRemove(XBaseTransformer):
     """ Remove specified values from a str type series.
 
     This transformer cannot be inverse_transformed and does not require fitting.
 
@@ -43,25 +41,28 @@
         self.special = special
         self.whitespace = whitespace
         self.stopwords = stopwords
         self.text = text
         self.custom_regex = custom_regex
 
     def __call__(self, *args, **kwargs):
+        import ipywidgets as widgets
+        from ipywidgets import interactive
+        from ...utils import xwidgets
         
         def _set_params(
-        numbers=widgets.ToggleButton(value=False),
-        characters=widgets.ToggleButton(value=False),
-        uppercase=widgets.ToggleButton(value=False),
-        lowercase=widgets.ToggleButton(value=False),
-        special=widgets.ToggleButton(value=False),
-        whitespace=widgets.ToggleButton(value=False),
-        stopwords=widgets.ToggleButton(value=False),
-        text=xwidgets.Text(''),
-        regex=xwidgets.Text('')
+            numbers=widgets.ToggleButton(value=False),
+            characters=widgets.ToggleButton(value=False),
+            uppercase=widgets.ToggleButton(value=False),
+            lowercase=widgets.ToggleButton(value=False),
+            special=widgets.ToggleButton(value=False),
+            whitespace=widgets.ToggleButton(value=False),
+            stopwords=widgets.ToggleButton(value=False),
+            text=xwidgets.Text(''),
+            regex=xwidgets.Text('')
         ):
 
             self.numbers = numbers
             self.characters = characters
             self.uppercase = uppercase
             self.lowercase = lowercase
             self.special = special
@@ -146,14 +147,15 @@
     supported_types = ['categorical']
 
     def __init__(self, case='lower'):
         super().__init__()
         self.case = case
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
         
         def _set_params(case = ["lower", "upper"]):
             self.case = case
         
         return interactive(_set_params)
 
     def transform(self, ser: pd.Series) -> pd.Series:
@@ -188,14 +190,15 @@
 
     def __init__(self, max_categories=10, category_list=[]):
         super().__init__()
         self.max_categories = int(max_categories)
         self.category_list = category_list
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
         
         def _set_params(max_categories=(2, 50)):
             self.max_categories = max_categories
         
         return interactive(_set_params)
 
     def transform(self, ser: pd.Series) -> pd.Series:
@@ -255,14 +258,15 @@
 
     def __init__(self, pct=0.8, categories=[]):
         super().__init__()
         self.pct = pct
         self.categories = categories
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
         
         def _set_params(pct=(0, 100)):
             self.pct = pct / 100
         
         return interactive(_set_params)
 
     def fit(self, ser: pd.Series) -> 'Condense':
@@ -330,14 +334,16 @@
 
     def __init__(self, merge_from=[], merge_to=''):
         super().__init__()
         self.merge_from = merge_from
         self.merge_to = merge_to
 
     def __call__(self, column, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
 
         unq = column.dropna().unique()
 
         def _set_params(
                 merge_from=widgets.SelectMultiple(options=unq), merge_to=unq):
             self.merge_from = list(merge_from)
             self.merge_to = merge_to
@@ -370,14 +376,15 @@
 
     def __init__(self, target=None, replace_with=''):
         super().__init__()
         self.target = target
         self.replace_with = replace_with
 
     def __call__(self, column, *args, **kwargs):
+        from ipywidgets import interactive
         
         unq = column.dropna().unique()
 
         def _set_params(target=unq, replace_with=''):
             self.target = target
             self.replace_with = replace_with
         
@@ -406,14 +413,15 @@
     supported_types = ['categorical']
 
     def __init__(self, fill_with='missing'):
         super().__init__()
         self.fill_with = fill_with
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
         
         def _set_params(fill_with = "missing"):
             self.fill_with = fill_with
         
         return interactive(_set_params)
 
     def transform(self, ser: pd.Series) -> pd.Series:
@@ -439,14 +447,16 @@
     supported_types = ['categorical']
 
     def __init__(self, category_values={}):
         super().__init__()
         self.category_values = category_values
 
     def __call__(self, ser, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
       
         def _set_params(*args, **kwargs):
             args = locals()
             self.category_values = dict(args)['kwargs']
 
         category_values = {i: widgets.Text(i) for i in ser.dropna().unique()}  
 
@@ -479,14 +489,16 @@
 
     def __init__(self, selector=None, value=None):
 
         self.selector = selector
         self.value = value
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
         
         def _set_params(
             selector = widgets.Dropdown(
                 options=["starts with", "ends with", "contains"]),
             value = ''):
 
             self.selector = selector
@@ -529,14 +541,16 @@
     def __init__(self, selector=None, n=0, action='keep'):
 
         self.selector = selector
         self.n = n
         self.action = action
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
         
         def _set_params(
             selector = widgets.Dropdown(options=["first", "last"]),
             n = widgets.IntText(n=1),
             action = widgets.Dropdown(options=['keep', 'drop']),
         ):
             self.selector = selector
@@ -584,14 +598,16 @@
     def __init__(self, start=None, end=None, action='keep'):
 
         self.start = start
         self.end = end
         self.action = action
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
         
         def _set_params(
             start = widgets.IntText(idx=0),
             end = widgets.IntText(idx=0),
             action = widgets.Dropdown(options=['keep', 'drop'])
         ):
             self.start = start
@@ -631,14 +647,15 @@
 
     def __init__(self, target=None, replace_with=None):
         super().__init__()
         self.target = target
         self.replace_with = replace_with
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
         
         def _set_params(target = '', replace_with = ''):
             self.target = target
             self.replace_with = replace_with
         
         return interactive(_set_params)
```

## xplainable/preprocessing/transformers/dataset.py

```diff
@@ -1,20 +1,16 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
-from ...utils import xwidgets as xwidgets
 from .base import XBaseTransformer
 
 import pandas.api.types as pdtypes
 import pandas as pd
-from ipywidgets import interactive
-import ipywidgets as widgets
 import numpy as np
 import pandas as pd
 import scipy.signal as ss
-from IPython.display import display
 
 
 class DropCols(XBaseTransformer):
     """ Drops specified columns from a dataset.
 
     Args:
         columns (str): The columns to be dropped.
@@ -23,14 +19,16 @@
     supported_types = ['dataset']
 
     def __init__(self, columns=None):
         super().__init__()
         self.columns = columns
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
         
         def _set_params(columns=xwidgets.SelectMultiple(options=df.columns)):
 
             self.columns = list(columns)
 
         return interactive(_set_params)
 
@@ -63,14 +61,16 @@
     supported_types = ['dataset']
 
     def __init__(self, subset=None):
         super().__init__()
         self.subset = subset
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
         
         def _set_params(
             subset=xwidgets.SelectMultiple(options=[None]+list(df.columns))):
 
             self.subset = list(subset)
 
         return interactive(_set_params)
@@ -106,14 +106,17 @@
         super().__init__()
         self.columns = columns
         self.operation = operation
         self.alias = alias if alias else " + ".join([c for c in columns])
         self.drop = drop
 
     def __call__(self, dataset, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
+        from ...utils import xwidgets
         
         cols = list(dataset.columns)
         
         def _set_params(
             columns_to_apply=xwidgets.SelectMultiple(
                 description='Columns: ',
                 value=[cols[0]],
@@ -209,14 +212,17 @@
         self.selector = selector
         self.n = n
         self.action = action
         self.drop_col = drop_col
         self.alias = alias
 
     def __call__(self, dataset, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
+        from ...utils import xwidgets
 
         cols = list(dataset.columns)
         
         def _set_params(
             column=xwidgets.Dropdown(
                 description='Column: ',
                 value=cols[0],
@@ -278,14 +284,17 @@
     supported_types = ['dataset']
 
     def __init__(self, col_names={}):
         super().__init__()
         self.col_names = col_names
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
+        from ...utils import xwidgets
       
         def _set_params(*args, **kwargs):
             args = locals()
             self.col_names = dict(args)['kwargs']
         
         col_names = {col: xwidgets.Text(col) for col in df.columns}
         
@@ -323,14 +332,16 @@
 
     def __init__(self, order_by=None, ascending=True):
         super().__init__()
         self.order_by = order_by
         self.ascending = ascending
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
       
         def _set_params(
             order_by = xwidgets.SelectMultiple(
                 description='Order by: ', options=[None]+list(df.columns)),
             direction = xwidgets.ToggleButtons(
                 description='Direction: ',
                 options=['ascending', 'descending'])):
@@ -378,14 +389,16 @@
         self.col_names = col_names
 
         self.group_by = group_by
         self.order_by = order_by
         self.descending = descending
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
         
         def _set_params(
             group_by = xwidgets.SelectMultiple(
                 description='Group by: ', options=[None]+list(df.columns)),
             order_by = xwidgets.SelectMultiple(
                 description='Order by: ', options=[None]+list(df.columns)),
             descending = xwidgets.Checkbox(value=False),
@@ -451,14 +464,16 @@
 
     def __init__(self, fill_with={}, fill_values={}):
         super().__init__()
         self.fill_with = fill_with
         self.fill_values = fill_values
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
       
         def _set_params(*args, **kwargs):
             args = locals()
             self.fill_with = dict(args)['kwargs']
 
         def get_widget(col):
             if pdtypes.is_numeric_dtype(df[col]):
@@ -531,14 +546,16 @@
     supported_types = ['dataset']
 
     def __init__(self, types={}):
         super().__init__()
         self.types = types
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
       
         def _set_params(*args, **kwargs):
             args = locals()
             self.types = dict(args)['kwargs']
 
         def get_widget(col):
             if pdtypes.is_float_dtype(df[col]):
@@ -622,14 +639,16 @@
     def __init__(self, target=None, separator=None, max_splits=0):
 
         self.target = target
         self.separator = separator
         self.max_splits = max_splits
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
         
         def _set_params(
             target=xwidgets.Dropdown(
                 options=[None]+[i for i in df.columns if \
                     pdtypes.is_string_dtype(df[i])]),
                 separator = xwidgets.Text(value=""),
                 max_splits = xwidgets.IntText(range=[0,10])):
@@ -672,14 +691,16 @@
 
     def __init__(self, columns=[], case='lower'):
         super().__init__()
         self.columns = columns
         self.case = case
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
         
         def _set_params(
             columns = xwidgets.SelectMultiple(
                 description='Columns: ',
                 options=[None]+[i for i in df.columns if \
                     pdtypes.is_string_dtype(df[i])]),
 
@@ -739,14 +760,16 @@
         self.target = target
 
         self.group_by = group_by
         self.order_by = order_by
         self.descending = descending
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        from ...utils import xwidgets
         
         def _set_params(
             group_by = xwidgets.SelectMultiple(
                 description='Group by: ', options=[None]+list(df.columns)),
             order_by = xwidgets.SelectMultiple(
                 description='Order by: ', options=[None]+list(df.columns)),
             descending = xwidgets.Checkbox(value=False),
@@ -818,14 +841,16 @@
         self.hour = hour
         self.minute = minute
         self.second = second
         self.drop = drop
 
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
         
         def _set_params(
             target=widgets.Dropdown(options=df.columns),
             year=widgets.ToggleButton(value=False),
             month=widgets.ToggleButton(value=False),
             day=widgets.ToggleButton(value=False),
             weekday=widgets.ToggleButton(value=False),
@@ -933,14 +958,17 @@
         self.direction = direction
         self.columns = columns
         self.window = window
         self.operation = operation
         self.drop = drop
 
     def __call__(self, df, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
+        from ...utils import xwidgets
         
         cols = list(df.columns)
         
         def _set_params(
             group_by = xwidgets.SelectMultiple(
                 description='Group by: ', options=[None]+list(df.columns)),
             order_by = xwidgets.SelectMultiple(
@@ -961,15 +989,15 @@
             self.orderby = list(order_by)
             self.direction = direction
             self.columns = list(columns_to_apply)
             self.operation = operation
             self.window = window
             self.drop = drop_columns
         
-        widget = widgets.interactive(_set_params)
+        widget = interactive(_set_params)
 
         widget.children[6].layout = widgets.Layout(margin='10px 0 20px 0')
 
         widget.layout = widgets.Layout(
             margin='0 0 0 30px',
             width='280px'
             )
```

## xplainable/preprocessing/transformers/mixed.py

```diff
@@ -1,27 +1,27 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
 from .base import XBaseTransformer
 import pandas.api.types as pdtypes
-from ipywidgets import interactive
-import ipywidgets as widgets
 import pandas as pd
 
 
 class SetDType(XBaseTransformer):
     """Changes the data type of a specified column."""
 
     # Informs the embedded GUI which data types this transformer supports.
     supported_types = ['numeric', 'categorical']
 
     def __init__(self, to_type=None):
         super().__init__()
         self.to_type = to_type
 
     def __call__(self, ser, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
       
         def _set_params(to_type, *args, **kwargs):
             self.to_type = to_type
 
         def get_widget(col):
             if pdtypes.is_float_dtype(ser):
                 options=["float", "integer", "string"]
@@ -88,14 +88,16 @@
     supported_types = ['categorical', 'numeric']
 
     def __init__(self, step=0):
         super().__init__()
         self.step = step
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
         
         def _set_params(
             step = widgets.IntText(value=0, min=-1000, max=1000)
             ):
             self.step = step
         
         return interactive(_set_params)
@@ -108,9 +110,7 @@
 
         Returns:
             pd.Series: The transformed series.
         """
         ser = ser.shift(self.step)
 
         return ser
-
-
```

## xplainable/preprocessing/transformers/numeric.py

```diff
@@ -1,12 +1,10 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
 from .base import XBaseTransformer
-from ipywidgets import interactive
-import ipywidgets as widgets
 from pandas.api.types import is_numeric_dtype
 import numpy as np
 import pandas as pd
 
 
 class MinMaxScale(XBaseTransformer):
     """Scales a numeric series between 0 and 1."""
@@ -92,14 +90,16 @@
 
     def __init__(self, lower=None, upper=None):
         super().__init__()
         self.lower = lower
         self.upper = upper
 
     def __call__(self, column, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
         
         minn = column.min()
         maxx = column.max()
         
         
         def _set_params(n=widgets.FloatRangeSlider(min=minn,max=maxx)):
             self.lower, self.upper = n
@@ -134,14 +134,16 @@
 
     def __init__(self, fill_with='mean', fill_value=None):
         super().__init__()
         self.fill_with = fill_with
         self.fill_value = fill_value
 
     def __call__(self, *args, **kwargs):
+        from ipywidgets import interactive
+        import ipywidgets as widgets
         
         def _set_params(
             fill_with = widgets.Dropdown(options=["mean", "median", "mode"])
         ):
             self.fill_with = fill_with
         
         return interactive(_set_params)
```

## xplainable/quality/scanner.py

```diff
@@ -1,16 +1,16 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
-from pandas.api.types import is_string_dtype, is_datetime64_dtype, is_numeric_dtype, is_bool_dtype
-# from statsmodels.stats.outliers_influence import variance_inflation_factor
-# from statsmodels.tools.tools import add_constant
+from pandas.api.types import (is_string_dtype, is_datetime64_dtype,
+                              is_numeric_dtype, is_bool_dtype)
 import pandas as pd
 import numpy as np
-import ipywidgets as widgets
 from IPython.display import display
+from .._dependencies import _check_ipywidgets
+from tqdm.auto import tqdm
 
 class XScan:
     """ Data quality scanner
     """
 
     def __init__(self):
         self.profile = {}
@@ -312,58 +312,14 @@
         sub_profile = {
             'type': self._detect_type(ser),
             'missing_pct': self._is_missing(ser)
         }
 
         return sub_profile
 
-    # @staticmethod
-    # def _vif(X, max_categories: int = 10):
-
-    #     X = X.copy()
-    #     X.dropna(inplace=True)
-        
-    #     categorical_columns = X.select_dtypes(
-    #         include=['object', 'category']).columns.to_list()
-
-    #     for col in list(categorical_columns):
-    #         if X[col].nunique() > max_categories:
-    #             categorical_columns.remove(col)
-
-    #     X = pd.get_dummies(
-    #         X, columns=categorical_columns, drop_first=True)
-
-    #     X = X.select_dtypes(include=[np.number])
-
-    #     # Add constant for vif calculation
-    #     X = add_constant(X)
-
-    #     # calculating VIF for each feature
-    #     vif = {X.columns[i]: variance_inflation_factor(
-    #         X.values, i) for i in range(X.shape[1])}
-
-    #     if 'const' in vif:
-    #         vif.pop('const')
-
-    #     vif_report = {}
-
-    #     # Add categories to map
-    #     for col in categorical_columns:
-    #         sub = {}
-    #         for i, v in copy.deepcopy(vif).items():
-    #             if i.startswith(col):
-    #                 sub[i.replace(f'{col}_', "")] = v
-    #                 vif.pop(i)
-            
-    #         vif_report[col] = sub
-            
-    #     vif_report.update(vif)
-
-    #     return vif_report
-
     def _scan_feature(self, ser):
 
         if is_bool_dtype(ser):
             ser = ser.astype(str)
             sub_profile = self._scan_categorical_feature(ser)
 
         elif is_numeric_dtype(ser):
@@ -376,40 +332,17 @@
             sub_profile = self._scan_date_feature(ser)
 
         else:
             raise TypeError(f"Feature {ser.name} has unknown type")
 
         return sub_profile
 
-    def scan(self, df, target=None, verbose=True):
+    def scan(self, df, target=None):
 
         if target:
             if target not in df.columns:
                 raise ValueError(f"{target} not in df")
 
             df = df.drop(columns=[target])
-        
-        progress_bar = widgets.IntProgress(
-            description="scanning data: ",
-            value=0,
-            max=df.shape[1],
-            style={'description_width': 'initial'})
-
-        if verbose:
-            current_feature = widgets.HTML("")
-            display(widgets.HBox([progress_bar, current_feature]))
-
-        for i, col in enumerate(df.columns):
-
-            if verbose:
-                progress_bar.value = i
-                current_feature.value = col
 
+        for i, col in tqdm(enumerate(df.columns)):
             self.profile[col] = self._scan_feature(df[col])
-
-        #current_feature.value = 'Calculating VIF'
-        #vif = self._vif(df)
-        #for i, v in vif.items():
-        #    self.profile[i].update({'vif': v})
-
-        current_feature.close()
-        progress_bar.close()
```

## xplainable/utils/__init__.py

```diff
@@ -1,3 +1,6 @@
+from .._dependencies import _try_optional_dependencies_gui
 from .api import *
 from .collections import *
-from .xwidgets import *
+
+if _try_optional_dependencies_gui():
+    from .xwidgets import *
```

## xplainable/utils/handlers.py

```diff
@@ -1,11 +1,9 @@
 import numpy as np
 import pandas as pd
-import warnings
-from packaging import version
 
 
 def add_thousands_separator(var):
     if isinstance(var, (float)):
         return '{:,.2f}'.format(var)
     elif isinstance(var, (int)):
         return '{:,.0f}'.format(var)
@@ -21,29 +19,8 @@
     return not inf_columns.any()
 
 def check_df(df):
     assert _check_nans(df), \
         'Dataframe contains NaNs. Please remove them before proceeding.'
     assert _check_inf(df), \
         'Dataframe contains infinite values. Please remove them before proceeding.'
-    
-def check_critical_versions():
-    """ This is implemented to ensure critical dependencies are imported."""
-    
-    # Tornado
-    try:
-        import tornado
-    except ImportError:
-        warnings.warn(
-            "Tornado is not installed, but is required for this package.")
-        return
-
-    if version.parse(tornado.version) > version.parse('6.1'):
-        warnings.warn(
-            """
-            Your version of Tornado is greater than 6.1, which is known to
-            crash the Jupyter kernel when training models. Please consider
-            downgrading to Tornado 6.1
-            """)
-    
-    return
-    
+
```

## xplainable/utils/xwidgets.py

```diff
@@ -1,13 +1,22 @@
 from traitlets import traitlets
 import ipywidgets as widgets
 from ipywidgets import interactive
 from IPython.display import display
-import webbrowser
 from .svgs import docs_svg, offline_svg
+import warnings
+
+# Handler for ipywidgets < 8.0.0
+try:
+    from ipywidgets import TagsInput as TagsInputt
+
+except ImportError:
+    from ipywidgets import Dropdown as TagsInputt
+    warnings.warn(f"TagsInput is not supported in ipywidgets version "
+                  f"{widgets.__version__}. Replacing with Dropdown")
 
 class LiveDF:
 
     def __init__(self, df):
         self.df = df
 
     def __call__(self):
@@ -30,45 +39,46 @@
     
     def __init__(self, *args, **kwargs):
         super(Dropdown, self).__init__(*args, **kwargs)
         self.layout = adder_element_layout
         self.style = adder_element_style
 
 
-class Text(widgets.Text):
+class TagsInput(TagsInputt):
     """This is used to set a default max_width for adder Text"""
     
     def __init__(self, *args, **kwargs):
-        super(Text, self).__init__(*args, **kwargs)
+        super(TagsInput, self).__init__(*args, **kwargs)
         self.layout = adder_element_layout
         self.style = adder_element_style
 
 
-class IntText(widgets.IntText):
+class Text(widgets.Text):
     """This is used to set a default max_width for adder Text"""
     
     def __init__(self, *args, **kwargs):
-        super(IntText, self).__init__(*args, **kwargs)
+        super(Text, self).__init__(*args, **kwargs)
         self.layout = adder_element_layout
         self.style = adder_element_style
 
 
-class SelectMultiple(widgets.SelectMultiple):
+class IntText(widgets.IntText):
     """This is used to set a default max_width for adder Text"""
     
     def __init__(self, *args, **kwargs):
-        super(SelectMultiple, self).__init__(*args, **kwargs)
+        super(IntText, self).__init__(*args, **kwargs)
         self.layout = adder_element_layout
         self.style = adder_element_style
 
-class TagsInput(widgets.TagsInput):
+
+class SelectMultiple(widgets.SelectMultiple):
     """This is used to set a default max_width for adder Text"""
     
     def __init__(self, *args, **kwargs):
-        super(TagsInput, self).__init__(*args, **kwargs)
+        super(SelectMultiple, self).__init__(*args, **kwargs)
         self.layout = adder_element_layout
         self.style = adder_element_style
 
 
 class Checkbox(widgets.Checkbox):
     """This is used to set a default max_width for adder Text"""
```

## xplainable/visualisation/explain.py

```diff
@@ -1,10 +1,9 @@
 """ Copyright Xplainable Pty Ltd, 2023"""
 
-import altair as alt
 import pandas as pd
 from IPython.display import HTML, display
 
 def _generate_explain_plot_data(model):
 
     def get_plot_data(f):
         _profile = model.profile
@@ -46,14 +45,21 @@
     prof = pd.concat(
         [i for i in plot_data if i is not None]).reset_index(drop=True)
 
     return prof
         
 def _plot_explainer(model):
 
+    try:
+        import altair as alt
+    except ImportError:
+        raise ImportError("Optional dependencies not found. Please install "
+                          "them with `pip install xplainable[plotting]' to use "
+                          "this feature.") from None
+
     fi = pd.DataFrame(
             {i: {'importance': v} for i, v in model.feature_importances.items()}
             ).T.reset_index()
 
     fi = fi.rename(columns={'index': 'feature'})
     fi['importance_label'] = fi['importance'].apply(
         lambda x: str(round(x*100, 1))+'%')
@@ -89,15 +95,16 @@
     view = alt.Chart(fi).mark_bar(color='#0080ea').encode(
         y=alt.Y('feature:N', sort='-x', axis=alt.Axis(
         labels=False, title=None)),
         x=alt.X('importance:Q', axis=alt.Axis(labels=False, title=None))
     ).properties(height=400, width=25).add_params(brush)
     
     view2 = alt.Chart(data).mark_bar(color='#e14067').encode(
-        y=alt.Y('value:N', sort='-x', axis=alt.Axis(labels=False, title=None)),
+        y=alt.Y('value:N', sort=alt.SortField(field='index', order='descending'),
+                axis=alt.Axis(labels=False, title=None)),
         x=alt.X('contribution:Q', axis=alt.Axis(labels=False, title=None)),
         color=alt.condition(
             alt.datum.contribution < 0,
             alt.value("#e14067"),
             alt.value("#12b980")
         )
     ).properties(height=400, width=25).add_params(brush2).transform_filter(
```

## Comparing `xplainable-1.0.5.dist-info/LICENSE` & `xplainable-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xplainable-1.0.5.dist-info/METADATA` & `xplainable-1.0.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: xplainable
-Version: 1.0.5
+Version: 1.0.6
 Summary: Real-time explainable machine learning for business optimisation
-Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -669,34 +668,41 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: drawsvg (>=2.1.1)
 Requires-Dist: hyperopt (>=0.2.7)
-Requires-Dist: ipywidgets (>=8.0.5)
 Requires-Dist: keyring (>=23.2.1)
-Requires-Dist: matplotlib (>=3.4.2)
-Requires-Dist: altair (>=5.0.1)
 Requires-Dist: numba (>=0.56.4)
 Requires-Dist: numpy (<=1.23.5,>=1.20.3)
 Requires-Dist: pandas (<=1.9.0,>=1.5.2)
 Requires-Dist: pyperclip (>=1.8.2)
 Requires-Dist: requests
 Requires-Dist: scikit-learn (>=1.2.2)
 Requires-Dist: scipy (>=1.6.2)
-Requires-Dist: seaborn (>=0.11.1)
-Requires-Dist: traitlets (>=5.5.0)
 Requires-Dist: urllib3 (>=1.26.5)
 Requires-Dist: psutil (>=5.9.4)
 Requires-Dist: joblib (>=1.2.0)
-Requires-Dist: tornado (==6.1)
-Requires-Dist: jupyter-client (==7.3.2)
+Requires-Dist: networkx (>=2.6.3)
+Requires-Dist: tqdm (>=4.62.3)
+Provides-Extra: gui
+Requires-Dist: tornado (==6.1) ; extra == 'gui'
+Requires-Dist: jupyter-client (==7.3.2) ; extra == 'gui'
+Requires-Dist: ipywidgets (>=8.0.5) ; extra == 'gui'
+Requires-Dist: matplotlib (>=3.4.2) ; extra == 'gui'
+Requires-Dist: seaborn (>=0.11.1) ; extra == 'gui'
+Requires-Dist: traitlets (>=5.5.0) ; extra == 'gui'
+Requires-Dist: drawsvg (>=2.1.1) ; extra == 'gui'
+Provides-Extra: plotting
+Requires-Dist: matplotlib (>=3.4.2) ; extra == 'plotting'
+Requires-Dist: seaborn (>=0.11.1) ; extra == 'plotting'
+Requires-Dist: altair (>=5.0.1) ; extra == 'plotting'
+Requires-Dist: plotly (>=5.1.0) ; extra == 'plotting'
 
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![Contributors](https://img.shields.io/badge/Contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 <div align="center">
@@ -711,21 +717,28 @@
     
 **Xplainable** leverages explainable machine learning for fully transparent predictions and advanced data optimisation in production systems.
 </div>
 
 
 ## Installation
 
-You can install ``xplainable`` with:
+You can install the core features of ``xplainable`` with:
 
 ```
 pip install xplainable
 ```
 
-Vist our [Documentation](https://xplainable.readthedocs.io) for extra support.
+to use the ``xplainable`` gui in a jupyter notebook, install with:
+
+```
+pip install xplainable[gui]
+```
+
+Vist our [Documentation](https://xplainable.readthedocs.io) for additional
+support.
 
 ## Getting Started
 
 **Basic Example**
 
 ```python
 import xplainable as xp
```

## Comparing `xplainable-1.0.5.dist-info/RECORD` & `xplainable-1.0.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+docs/conf.py,sha256=cLKVa_Z7K9oZRG25BB7YkPh9sH0UNZ0zotg4d5wF7q4,1291
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xplainable/__init__.py,sha256=7MV0oMkcwb1OrCv_I7IrrFdK-Nv9DAQ8Fh0pHytAbxQ,488
-xplainable/_version.py,sha256=ZR1VA9cGs0vIK6cWK4YKLfBTnmUCAcDaaP9ARPPYxEs,21
+xplainable/__init__.py,sha256=1RJ19JLOCHojYAabHAAxTKs_eXl05pJzPmC3W_91rsQ,786
+xplainable/_dependencies.py,sha256=l7HDli4G26n_xsK_Pqfq4xkRzG07_c8oJOHFxfgxrMw,1553
+xplainable/_version.py,sha256=fCDDAyG3nMZcE_hvt1RHdxkiFN3DfNSyU_k-rLUDrpE,21
+xplainable/config.py,sha256=YKLDvcgmsv73cnKU8czNOBqqTvNYydnPagVSSUR12ik,113
 xplainable/callbacks/__init__.py,sha256=0RRftTFsiuCCp8mBluQS_0_uqwoKqABPW6PP__yNtwg,27
 xplainable/callbacks/optimisation.py,sha256=JQm8xbfR5BFMQZKObsOA12VKmDHJ7xeaDjlYd66s2Ik,3705
 xplainable/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xplainable/client/client.py,sha256=wP904H_NbYwtVcpUx4Q8ItfLxIpNkAoKDVU8B1mb3dg,24071
-xplainable/client/init.py,sha256=iis82asRx6qiJ4DcquadxIv1_NsWMdZcNDreNzrtf5w,3067
+xplainable/client/client.py,sha256=nkt-jOsXp5BwWjtOox_auzPKuNUYSgmOvbkYydutwDY,24282
+xplainable/client/init.py,sha256=qbZg7JNSA3tsSb2oo1AgAimBEQ-h0tonnZDWT0OBDZs,3179
 xplainable/core/__init__.py,sha256=SRfF7oDVlOOAi6nGKiJIUK6B_arqYLO9iSMp-2IZZps,21
 xplainable/core/models.py,sha256=EwqOcETvdimcJGlMhku3qfK00NmyuMC4Qk3yQajQHnk,61
 xplainable/core/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 xplainable/core/ml/_base_model.py,sha256=T8jo0m2w_K2wR4UW825uUEfrG9ufJ9a0n0iqkiG1CMk,12946
 xplainable/core/ml/_constructor.py,sha256=EnNwfKJEk_wy-VIETkdtFPoUA9SHZgK9IxezCQYCM5o,10063
 xplainable/core/ml/classification.py,sha256=keSf9SsU2vexRexJKfNN4Z4p8Y14uMJW3MgoMzzON0Y,25955
 xplainable/core/ml/regression.py,sha256=qSMf7QisXJcJIArkKkYkVJpVWEKo3H5lvXumSenmU2A,18856
@@ -17,54 +20,58 @@
 xplainable/core/nlp/feature_extraction.py,sha256=MqLh5o1JYyg0SJQga921QuGriXufdWENxSOWcnlsNkc,22545
 xplainable/core/optimisation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 xplainable/core/optimisation/bayesian.py,sha256=k1dWm9HgLY_m_KXq_uNwMgDRKsRNgePITraqMFV2lbY,14737
 xplainable/core/optimisation/genetic.py,sha256=mkQ9czuZKTXP3NN5n59kcYn3BJPkEmfu-tcnTOHMatU,6000
 xplainable/core/optimisation/layers.py,sha256=gX2UBW86axjHP5i_6Jejw7ZkziK11a_xTXrgSNqrYoU,21903
 xplainable/core/optimisation/nlp.py,sha256=kPzQ6_WqtYO38jA8Im4OGFTUxjpW7idBU5OK6YRadg0,6696
 xplainable/core/optimisation/targeting.py,sha256=Mrl7LlvS_3D4Rcq84bd9MH05Ic9i9gDPN3__yzykN1c,6906
-xplainable/gui/__init__.py,sha256=WBrwfbSHJCEQVMxZcFFJGFt1NCSEtGRVxKDT6Q0k72g,22
+xplainable/feature_selection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+xplainable/feature_selection/classification.py,sha256=ufqlo3ePRopgxc-zeHIv7-byXlyVhNFCHOxuvtYPpaM,5950
+xplainable/feature_selection/graph.py,sha256=PM6yWbgRLyAlS3cPhn76fvL9i1AITFxRKhlsdMdA_Ck,7771
+xplainable/gui/__init__.py,sha256=XGXNLZYp6VvwJ8uoxnqobDL9tKOwFM-DP5AVwcqf_Uc,1627
 xplainable/gui/components/__init__.py,sha256=90-xUw4GbPXPnJs939DqWsZ8IBaKLlc2Z7szgoSPuUw,112
 xplainable/gui/components/bars.py,sha256=vxgxyqOYIvkokAKxrGDxgTZd7_ZodULoP4aTmvaVahQ,6347
-xplainable/gui/components/cards.py,sha256=1luOzr6Z_zRxoVU1Xr1kskVeolhZ7709Dr_RzuCpUPI,4615
+xplainable/gui/components/cards.py,sha256=cLqV2QyGLlrdDVic_b74EkY9a0Kbcateqkrfu_pyDCo,4588
 xplainable/gui/components/connectivity.py,sha256=CwlyGH8tnrU0_5tPpR5TDk62WzycUf6nRVUZLT9izRE,1093
 xplainable/gui/components/header.py,sha256=ZZgNpZLZsdN-latn8JgeHZT8lxX5J8x9mQoIT-raL1A,3018
 xplainable/gui/components/pipelines.py,sha256=fPXF3PFA0MOCY5UHuWURekuu57qPZDpL8RfNghB8TdI,8784
 xplainable/gui/components/tables.py,sha256=J-U6U8pi0Z7yqsGlEwrotCiARFpBLLDLT_Odkh33Odk,2848
-xplainable/gui/screens/__init__.py,sha256=yGoWdNrkJjVQIEHMYlFcktabTrFqCctJN0AKYyQ3St8,100
-xplainable/gui/screens/classifier.py,sha256=CaGtSTy1Sxk47cPlZlBCPgTTHoUUjyLwQAaNWH_f5l8,23982
+xplainable/gui/screens/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+xplainable/gui/screens/classifier.py,sha256=sZoNdRYh-I__Z5mccXTD7hylS4vREcxlzYJYu8sBQ_I,24102
 xplainable/gui/screens/evaluate.py,sha256=2n265ZTC8VyScv2PhWEPzVzuCqYwIJfyi7CGzCf21PA,38580
-xplainable/gui/screens/loader.py,sha256=47GNIuLy4HQkjrexAoWYBSef5xOLEp5RPihrrqezMcs,14819
-xplainable/gui/screens/preprocessor.py,sha256=aH7ur1WgsbhgaJKU9CY_qtj6EIVtq7t4qjJcVCB-we8,39855
-xplainable/gui/screens/regressor.py,sha256=qJzaPo6A40x-4bFxSyh6HV15x__U3SL9Lt_NaPqrOHc,19494
-xplainable/gui/screens/save.py,sha256=bddxNDj1B6Cc1FMsTHDabLhSFOvSp-pI08uQ8bRXXoY,20280
+xplainable/gui/screens/loader.py,sha256=CsrvJEGe9d-rpkWRoPkNuLFLNNj_XRHyenJbMyK_s0U,15870
+xplainable/gui/screens/preprocessor.py,sha256=aZ56olq_f909oxmxa_81er9nbs6SoKa56QzeHyuS0e0,40125
+xplainable/gui/screens/regressor.py,sha256=fzdCW-bskj6N3fXeafiRoQR1IcSIn_scS7z3Skwmbvw,19879
+xplainable/gui/screens/save.py,sha256=QF1N2HpHtaUR9HGQnxVkwylt_QZnulglcENt2yTutA4,20044
 xplainable/gui/screens/scenario.py,sha256=xVQPIR_bUPUMKe_BVs7tBRH6JkEkhVaU-bqAVcO8Kh0,22064
 xplainable/metrics/__init__.py,sha256=Jk4ODFvbeCgS9ecmD1lftfaRNoL72q4Ek8VvWr5Nw6k,22
 xplainable/metrics/metrics.py,sha256=vtYw2RLrvtyhLStKfFcj18H8yPffetnbwPIUVwjavHQ,6074
 xplainable/preprocessing/__init__.py,sha256=X1oBxQgfGa97r9OKBeWdlOCwRH-IsBZeg4Y9kj0WtbM,27
 xplainable/preprocessing/pipeline.py,sha256=7Nhmiu5icIkWKqaGPA7Xmle93mzBsGUNlZGXhf-VXYw,6628
 xplainable/preprocessing/transformers/__init__.py,sha256=-8ld9w7w-QAjp_gMcYtlWS6gzrIiYW1xFmrubj-Ik_8,94
 xplainable/preprocessing/transformers/base.py,sha256=gatruZkPBSPxUDy96Dkv3YoFhfluusOFWOkE6hslsak,3518
-xplainable/preprocessing/transformers/categorical.py,sha256=TYrPdvmw-zcPnX2vH7IW1IkjrkSfZrtVWaHd7a9lZ94,19239
-xplainable/preprocessing/transformers/dataset.py,sha256=01l_QG6aqZJ1Xdtibv4T_9rsdlpzVIsmgfrRK2gBTIo,32659
-xplainable/preprocessing/transformers/mixed.py,sha256=dCdW8gx0go4ObpP9tXGTBGyfC8TvkZXBZP_VxFGhLkg,3201
-xplainable/preprocessing/transformers/numeric.py,sha256=3ftlfvUGAt5R_ijg_i9crMrJ7HXLYnOBW39KExLCbUA,4902
+xplainable/preprocessing/transformers/categorical.py,sha256=SHJigeaeYwRpmAkzhTlOY0TipB9A-lYHiYehQgJQHwk,19977
+xplainable/preprocessing/transformers/dataset.py,sha256=zqCDbOKT0A4XvZ2Ww5x9OXAydWqD-Uj_2IvvOuy4E-c,33790
+xplainable/preprocessing/transformers/mixed.py,sha256=SVGSBIk1vDHm3OuAawswxSTsi5BN4wYY57lNwGcTLSY,3295
+xplainable/preprocessing/transformers/numeric.py,sha256=PBVktgQjDNUD-kec8AuAl_IMIks95h28ZECSelh69aM,4998
 xplainable/quality/__init__.py,sha256=Iar9SSkqRjynNYC8lR2Uo-wisJJzk7ZH3kzC0knsHcY,26
-xplainable/quality/scanner.py,sha256=r03FWJ-7YUXH6GTPDmtPJ69yoJ07hv36Zs90qXBKbhg,10927
-xplainable/utils/__init__.py,sha256=38b6bIq3xiXjLwXjSJmqfRINqKc5N8W6SA3VTlWE6T0,69
+xplainable/quality/scanner.py,sha256=FLBsgOiqQQIonyEmi5bsoMEqHmKHJsQRHhHAA3L-z6c,8928
+xplainable/utils/__init__.py,sha256=4t7WmE5qjaakZXB4ECF96UpwDhU1uCtTs1HVwJDU3zk,170
 xplainable/utils/activation.py,sha256=Y920-VDdK_VikAlR0ZYtmzCwRMIKMbwEawNsdObgPrE,391
 xplainable/utils/api.py,sha256=RbsznMeB52yXPPQBrHL8DIxNpKh9ooIa2P13SXJ-Ovs,1063
 xplainable/utils/collections.py,sha256=KNsZSSrqVP-he_DhBKv9hDTJEIarsNQDe32EweFXuy0,2209
 xplainable/utils/encoders.py,sha256=ihh__Xh04y_EPLs8v_DtngqRhGje_vjh0_4N3dHyGok,810
 xplainable/utils/exceptions.py,sha256=YYhiNDjuRhPYeMz49zYbgAshvKYd_SGLwaU9TLKA7aQ,226
-xplainable/utils/handlers.py,sha256=SZaTGWt5vjZputZ1i7eTrnMxC1IbEgLFDTD4NxBSMZw,1393
+xplainable/utils/handlers.py,sha256=Bn_evRtN6qdrpoCXpkAXn1DEn_XeCxULgoMAKxay35g,726
 xplainable/utils/loaders.py,sha256=NKZbfS2O1zkU52myW99XH1srykAdfPBlcNQ_57yp7P8,2111
 xplainable/utils/numba_funcs.py,sha256=rwN9IoIrQ2HUoitojFGufGok7t6KNSLfgm0zrKgAoHg,1158
 xplainable/utils/svgs.py,sha256=Eond6CE1OPEW-D3W46NeKhD6Thr7Y4BQ9XsoRB30syg,4906
-xplainable/utils/xwidgets.py,sha256=0nC_Godb5ouTbQobAqTzFjeWQwSVTxTe5h8GT7NIoYQ,9759
+xplainable/utils/xwidgets.py,sha256=Ffx226jsjrgIPSFlj7WKL8ftgSG9bx4ERsltoq15u2g,10052
 xplainable/visualisation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xplainable/visualisation/explain.py,sha256=Yt8TU2g0PY9eVH8m4bU2aAX4ZzpUA_-E_zH5nXu8JQ0,4380
+xplainable/visualisation/explain.py,sha256=WDzR3_JhrX_rsPNUCG-b2waeqnp_sMfuqJsAajCGG2w,4693
+xplainable/visualisation/network.py,sha256=k1qluXsn6iNTU05yl7xw9KdHPhg75Kp_pC-DXdJW-jA,2822
 xplainable/visualisation/regression.py,sha256=bEaM3lLxoLCN51Gu7ysBuM9vkfgj3c7kMfk1oRa1y9Q,387
-xplainable-1.0.5.dist-info/LICENSE,sha256=ILBn-G3jdarm2w8oOrLmXeJNU3czuJvVhDLBASWdhM8,34522
-xplainable-1.0.5.dist-info/METADATA,sha256=kxTSphJsPS57OwGj-QOovltzjr1VL2JbcFVNPGzdzpM,50058
-xplainable-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-xplainable-1.0.5.dist-info/top_level.txt,sha256=Z4T05qncKSpRpo2KT4IVp6ORS5aYxyD3W6IGQTxCFek,17
-xplainable-1.0.5.dist-info/RECORD,,
+xplainable-1.0.6.dist-info/LICENSE,sha256=ILBn-G3jdarm2w8oOrLmXeJNU3czuJvVhDLBASWdhM8,34522
+xplainable-1.0.6.dist-info/METADATA,sha256=yapyNMs-hTkaKew51QjMXkXbj1Ng_U7gT7cqYYvVEc0,50581
+xplainable-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+xplainable-1.0.6.dist-info/top_level.txt,sha256=hTl18yQMFMsxWfzKR50DpdozA8TT-t1h_nwKDjsBX4k,27
+xplainable-1.0.6.dist-info/RECORD,,
```

