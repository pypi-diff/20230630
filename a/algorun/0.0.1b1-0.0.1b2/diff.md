# Comparing `tmp/algorun-0.0.1b1-py3-none-any.whl.zip` & `tmp/algorun-0.0.1b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,27 @@
-Zip file size: 24727 bytes, number of entries: 27
+Zip file size: 20672 bytes, number of entries: 25
 -rw-r--r--  2.0 unx     1168 b- defN 80-Jan-01 00:00 algorun/__init__.py
 -rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 algorun/__main__.py
--rw-r--r--  2.0 unx     2102 b- defN 80-Jan-01 00:00 algorun/cli/__init__.py
--rw-r--r--  2.0 unx     1571 b- defN 80-Jan-01 00:00 algorun/cli/bootstrap.py
+-rw-r--r--  2.0 unx     1008 b- defN 80-Jan-01 00:00 algorun/cli/__init__.py
 -rw-r--r--  2.0 unx      295 b- defN 80-Jan-01 00:00 algorun/cli/config.py
--rw-r--r--  2.0 unx     2512 b- defN 80-Jan-01 00:00 algorun/cli/goal.py
+-rw-r--r--  2.0 unx     2515 b- defN 80-Jan-01 00:00 algorun/cli/goal.py
 -rw-r--r--  2.0 unx      970 b- defN 80-Jan-01 00:00 algorun/cli/reset.py
 -rw-r--r--  2.0 unx     2622 b- defN 80-Jan-01 00:00 algorun/cli/start.py
 -rw-r--r--  2.0 unx      535 b- defN 80-Jan-01 00:00 algorun/cli/stop.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algorun/core/__init__.py
 -rw-r--r--  2.0 unx     1329 b- defN 80-Jan-01 00:00 algorun/core/atomic_write.py
--rw-r--r--  2.0 unx     9841 b- defN 80-Jan-01 00:00 algorun/core/bootstrap.py
 -rw-r--r--  2.0 unx     1160 b- defN 80-Jan-01 00:00 algorun/core/conf.py
 -rw-r--r--  2.0 unx     4711 b- defN 80-Jan-01 00:00 algorun/core/doctor.py
 -rw-r--r--  2.0 unx     1159 b- defN 80-Jan-01 00:00 algorun/core/init.py
 -rw-r--r--  2.0 unx     5128 b- defN 80-Jan-01 00:00 algorun/core/log_handlers.py
 -rw-r--r--  2.0 unx     3520 b- defN 80-Jan-01 00:00 algorun/core/proc.py
 -rw-r--r--  2.0 unx     1970 b- defN 80-Jan-01 00:00 algorun/core/questionary_extensions.py
 -rw-r--r--  2.0 unx     4844 b- defN 80-Jan-01 00:00 algorun/core/sandbox.py
 -rw-r--r--  2.0 unx      508 b- defN 80-Jan-01 00:00 algorun/core/utils.py
 -rw-r--r--  2.0 unx     4170 b- defN 80-Jan-01 00:00 algorun/core/version_prompt.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algorun/py.typed
--rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algorun-0.0.1b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2671 b- defN 80-Jan-01 00:00 algorun-0.0.1b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algorun-0.0.1b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algorun-0.0.1b1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2140 b- defN 16-Jan-01 00:00 algorun-0.0.1b1.dist-info/RECORD
-27 files, 56185 bytes uncompressed, 21311 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3214 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1977 b- defN 16-Jan-01 00:00 algorun-0.0.1b2.dist-info/RECORD
+25 files, 44062 bytes uncompressed, 17506 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -3,17 +3,14 @@
 
 Filename: algorun/__main__.py
 Comment: 
 
 Filename: algorun/cli/__init__.py
 Comment: 
 
-Filename: algorun/cli/bootstrap.py
-Comment: 
-
 Filename: algorun/cli/config.py
 Comment: 
 
 Filename: algorun/cli/goal.py
 Comment: 
 
 Filename: algorun/cli/reset.py
@@ -27,17 +24,14 @@
 
 Filename: algorun/core/__init__.py
 Comment: 
 
 Filename: algorun/core/atomic_write.py
 Comment: 
 
-Filename: algorun/core/bootstrap.py
-Comment: 
-
 Filename: algorun/core/conf.py
 Comment: 
 
 Filename: algorun/core/doctor.py
 Comment: 
 
 Filename: algorun/core/init.py
@@ -60,23 +54,23 @@
 
 Filename: algorun/core/version_prompt.py
 Comment: 
 
 Filename: algorun/py.typed
 Comment: 
 
-Filename: algorun-0.0.1b1.dist-info/LICENSE
+Filename: algorun-0.0.1b2.dist-info/LICENSE
 Comment: 
 
-Filename: algorun-0.0.1b1.dist-info/METADATA
+Filename: algorun-0.0.1b2.dist-info/METADATA
 Comment: 
 
-Filename: algorun-0.0.1b1.dist-info/WHEEL
+Filename: algorun-0.0.1b2.dist-info/WHEEL
 Comment: 
 
-Filename: algorun-0.0.1b1.dist-info/entry_points.txt
+Filename: algorun-0.0.1b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: algorun-0.0.1b1.dist-info/RECORD
+Filename: algorun-0.0.1b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algorun/cli/__init__.py

```diff
@@ -1,10 +1,9 @@
 import click
 
-from algorun.cli.bootstrap import bootstrap_group
 from algorun.cli.goal import goal_command
 from algorun.cli.start import start_command
 from algorun.cli.stop import stop_command
 from algorun.core.conf import PACKAGE_NAME
 from algorun.core.log_handlers import color_option, verbose_option
 from algorun.core.version_prompt import do_version_prompt, skip_version_check_option
 
@@ -17,21 +16,21 @@
 )
 @click.version_option(package_name=PACKAGE_NAME)
 @verbose_option
 @color_option
 @skip_version_check_option
 def algorun(*, skip_version_check: bool) -> None:
     """
-    ░█████╗░██╗░░░░░░██████╗░░█████╗░██████╗░░█████╗░███╗░░██╗██████╗░
-    ██╔══██╗██║░░░░░██╔════╝░██╔══██╗██╔══██╗██╔══██╗████╗░██║██╔══██╗
-    ███████║██║░░░░░██║░░██╗░██║░░██║██████╔╝███████║██╔██╗██║██║░░██║
-    ██╔══██║██║░░░░░██║░░╚██╗██║░░██║██╔══██╗██╔══██║██║╚████║██║░░██║
-    ██║░░██║███████╗╚██████╔╝╚█████╔╝██║░░██║██║░░██║██║░╚███║██████╔╝
-    ╚═╝░░╚═╝╚══════╝░╚═════╝░░╚════╝░╚═╝░░╚═╝╚═╝░░╚═╝╚═╝░░╚══╝╚═════╝░"""
+    ########################################\n
+    ###             ALGORUN              ###\n
+    ########################################
+
+    Welcome to Algorun, your cli to run an Algorand mainnet node
+    """
+
     if not skip_version_check:
         do_version_prompt()
 
 
 algorun.add_command(start_command)
 algorun.add_command(stop_command)
 algorun.add_command(goal_command)
-algorun.add_command(bootstrap_group)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## algorun/cli/goal.py

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import click
+
 from algorun.core import proc
 from algorun.core.sandbox import ComposeSandbox
 
 logger = logging.getLogger(__name__)
 
 
 @click.command(
@@ -54,11 +55,11 @@
         sandbox = ComposeSandbox()
         ps_result = sandbox.ps("mainnet-container")
         match ps_result:
             case [{"State": "running"}]:
                 pass  # container is running, failure must have been with command
             case _:
                 logger.warning(
-                    "algod container does not appear to be running, "
+                    "mainnet-container does not appear to be running, "
                     "ensure mainnet node is started by executing `algorun start`"
                 )
         raise click.exceptions.Exit(result.exit_code)  # pass on the exit code
```

## Comparing `algorun-0.0.1b1.dist-info/LICENSE` & `algorun-0.0.1b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algorun-0.0.1b1.dist-info/METADATA` & `algorun-0.0.1b2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorun
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Algorand development kit command-line interface
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,17 +18,19 @@
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # Algorun CLI
 
+THIS IS IN BETA
+
 ## Is this for me?
 
-The target audience for this tool is software developers building applications on the Algorand network. A working knowledge of using a command line interfaces and experience using the supported programming languages is assumed.
+This tool simplifies setting up and starting an Algorand mainnet node. You should know your way around a CLI if you're planning to use it
 
 # Install
 
 ## Prerequisites
 
 The key required dependency is Python 3.10+, but some of the installation options below will install that for you.
 
@@ -41,33 +43,42 @@
 1. Ensure desired prerequisites are installed
 
    - [Python 3.10+](https://www.python.org/downloads/)
    - [pipx](https://pypa.github.io/pipx/installation/)
    - [Docker](https://docs.docker.com/get-docker/)
 
 2. Install using pipx `pipx install algorun`
-3. Restart the terminal to ensure AlgoKit is available on the path
+3. Restart the terminal to ensure Algorun is available on the path
 4. [Verify installation](#verify-installation)
 
 ### Maintenance
 
 - To update Algorun: `pipx upgrade algorun`
 - To remove Algorun: `pipx uninstall algorun`
 
 ## Verify installation
 
-Verify AlgoKit is installed correctly by running `algorun --version` and you should see output similar to:
+Verify Algorun is installed correctly by running `algorun --version` and you should see output similar to:
 
 ```
 algorun, version 0.1
 ```
 
+## Usage
+
+Create a directory where you're comfortable keeping the node config and files, we suggest naming it `algorand`, open that directory in a terminal
+
+- `algorun start` will start your node by creating `docker-compose.yml`, `config.json` files and a `data` directory where your node will persist.
+- `algorun stop` will shut down your node
+- `algorun goal` is a wrapper for the [Goal CLI](https://developer.algorand.org/docs/clis/goal/goal/)
+- typing `algorun goal node status` will return your nodes status typing `algorun goal node status -w 1000` instead will keep giving you node status updates every 1 second
+
 > **Note**
 > If you get receive one of the following errors:
 >
 > - `command not found: algorun` (bash/zsh)
 > - `The term 'algorun' is not recognized as the name of a cmdlet, function, script file, or operable program.` (PowerShell)
 >
 > Then ensure that `algorun` is available on the PATH by running `pipx ensurepath` and restarting the terminal.
 
-If you're experiencing issues with algorun [raise an issue](https://github.com/algorandfoundation/algokit-cli/issues/new).
+If you're experiencing issues with algorun [raise an issue](https://github.com/algorandfoundation/algorun/issues/new).
```

## Comparing `algorun-0.0.1b1.dist-info/RECORD` & `algorun-0.0.1b2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 algorun/__init__.py,sha256=tTevvwd9DQC3ZFejCvFLe_RkLJzTl02-JLx3rUyw-mI,1168
 algorun/__main__.py,sha256=MthWEPnwuPqimUPhdSWpThuj4sV-2c1ycv97gvgcBEk,43
-algorun/cli/__init__.py,sha256=JWBESrJDWuPlSmsSq_jGPb682gvuGBShq5RQJI3zP28,2102
-algorun/cli/bootstrap.py,sha256=AFe3L4GcgClh97wPLcjG6hy5t62ymw5QfWunXYG_79s,1571
+algorun/cli/__init__.py,sha256=WDlaPxJkZWDWBh2sydZWtIY4ScyvP7zYMKJBJnfHdo8,1008
 algorun/cli/config.py,sha256=rB0-99EcwwyV61FffEBji0pmudSpOdFPqtboE2hL2z8,295
-algorun/cli/goal.py,sha256=rilCcm5wUci1stcffUJK-2rTU_2TymMZDdCmYmxaah8,2512
+algorun/cli/goal.py,sha256=RRkoFKg8IpvI8l0b52XHCKA387HhB2A-En1vOB221V0,2515
 algorun/cli/reset.py,sha256=Te2XvI0OwpOx0P_PzMWaVu9p22sDOni_F3OYH3TV4So,970
 algorun/cli/start.py,sha256=Wcl17n82a_tdIa7D6txNv_RfOsK9CuvSNi6X145v8kw,2622
 algorun/cli/stop.py,sha256=I69eLd-nK94_J0DZqs8fKgprM9i1u0r8h4j1GJeM9g0,535
 algorun/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algorun/core/atomic_write.py,sha256=n1cIEXLiXOHU5lyHy40u8gUddW9IF_shfyaJhuJH8d4,1329
-algorun/core/bootstrap.py,sha256=WY7UqIfG1NL_2sTHVS-sfi8rbFAgL7hIluIR3WJQCxU,9841
 algorun/core/conf.py,sha256=k3rm3IlWr5goYE8MWOlWlK5PQDS0UrUx0DtgY3xlVLU,1160
 algorun/core/doctor.py,sha256=xRy3wY_EGhfC-UZIO7bTMULO5NxxV2tb8ak_3uhVAAc,4711
 algorun/core/init.py,sha256=7y_EwVtuMfqZG_CGDR08K0f2SOOeFq6y1d8ihZgG3Uo,1159
 algorun/core/log_handlers.py,sha256=IT9mo8NhiLl2rzH6t6F9kEflmmFbOfOhKaPzRp7CVTM,5128
 algorun/core/proc.py,sha256=UsMC8ysyjVZ2Ql8dzodK2qS_PaH_U9rUviZQw_vbE80,3520
 algorun/core/questionary_extensions.py,sha256=QvUGXL_GxcPvdGemy_5-Fza4d1PSJ2ml7aZAS3r4M20,1970
 algorun/core/sandbox.py,sha256=RnNVAslpgUI6xODkiBhBfKn-yW5kywCIYAZRBbNnQIQ,4844
 algorun/core/utils.py,sha256=hgemlB8znOsGCO090BQOydnbq4ZRAsD9CzMbApEMGY8,508
 algorun/core/version_prompt.py,sha256=Tixd0RZEcDTv1-sSopG8ngLvP4MZjRgKO8QQtiDnGEQ,4170
 algorun/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algorun-0.0.1b1.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
-algorun-0.0.1b1.dist-info/METADATA,sha256=BHkw01FG_5fK9-266BG6mGFTiTt5vOPUnn5C6tmQUBA,2671
-algorun-0.0.1b1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algorun-0.0.1b1.dist-info/entry_points.txt,sha256=fxs3JmtSLlx0RPAWt5Sj7MiHmnuQWxeNiZpL1xLX4-g,47
-algorun-0.0.1b1.dist-info/RECORD,,
+algorun-0.0.1b2.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
+algorun-0.0.1b2.dist-info/METADATA,sha256=HavFocgU5ty15osQKWwvKla_vrSjCQz-BM6EKX6qocQ,3214
+algorun-0.0.1b2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algorun-0.0.1b2.dist-info/entry_points.txt,sha256=fxs3JmtSLlx0RPAWt5Sj7MiHmnuQWxeNiZpL1xLX4-g,47
+algorun-0.0.1b2.dist-info/RECORD,,
```

