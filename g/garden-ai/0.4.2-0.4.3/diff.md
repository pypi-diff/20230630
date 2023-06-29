# Comparing `tmp/garden_ai-0.4.2.tar.gz` & `tmp/garden_ai-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.4.2.tar", max compression
+gzip compressed data, was "garden_ai-0.4.3.tar", max compression
```

## Comparing `garden_ai-0.4.2.tar` & `garden_ai-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0     1078 2023-06-06 16:06:37.386640 garden_ai-0.4.2/LICENSE
--rw-r--r--   0        0        0      797 2023-06-06 16:06:37.386640 garden_ai-0.4.2/README.md
--rw-r--r--   0        0        0      418 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/__main__.py
--rw-r--r--   0        0        0       97 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/__init__.py
--rw-r--r--   0        0        0       54 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/console.py
--rw-r--r--   0        0        0    10707 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/garden.py
--rw-r--r--   0        0        0      828 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/main.py
--rw-r--r--   0        0        0     3076 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/model.py
--rw-r--r--   0        0        0     7184 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0    17556 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/client.py
--rw-r--r--   0        0        0       76 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/constants.py
--rw-r--r--   0        0        0     9398 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/datacite.py
--rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/funcx_bandaid/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/funcx_bandaid/serialization_patch.py
--rw-r--r--   0        0        0    14373 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2803 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0     1451 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/login_manager.py
--rw-r--r--   0        0        0      801 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     3011 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     7498 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/local_data.py
--rw-r--r--   0        0        0    10512 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/mlmodel.py
--rw-r--r--   0        0        0    21264 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/pipelines.py
--rw-r--r--   0        0        0    11909 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/steps.py
--rw-r--r--   0        0        0     2022 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     2185 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0    11186 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     2874 2023-06-06 16:06:49.994663 garden_ai-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2419 1970-01-01 00:00:00.000000 garden_ai-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-29 16:14:08.147767 garden_ai-0.4.3/LICENSE
+-rw-r--r--   0        0        0      797 2023-06-29 16:14:08.147767 garden_ai-0.4.3/README.md
+-rw-r--r--   0        0        0      418 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/__main__.py
+-rw-r--r--   0        0        0       97 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0     2855 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/app/console.py
+-rw-r--r--   0        0        0    11506 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/app/main.py
+-rw-r--r--   0        0        0     3895 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/app/model.py
+-rw-r--r--   0        0        0    11770 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0     3493 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    18030 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/client.py
+-rw-r--r--   0        0        0      380 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/constants.py
+-rw-r--r--   0        0        0     9394 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/datacite.py
+-rw-r--r--   0        0        0        0 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/funcx_bandaid/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/funcx_bandaid/serialization_patch.py
+-rw-r--r--   0        0        0    14824 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2802 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0     1603 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/globus_compute/login_manager.py
+-rw-r--r--   0        0        0      801 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1362 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7553 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/local_data.py
+-rw-r--r--   0        0        0    12544 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0        0 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/model_file_transfer/__init__.py
+-rw-r--r--   0        0        0     1438 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/model_file_transfer/upload.py
+-rw-r--r--   0        0        0    19490 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    10610 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/steps.py
+-rw-r--r--   0        0        0     2019 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0    11186 2023-06-29 16:14:08.151767 garden_ai-0.4.3/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2865 2023-06-29 16:14:18.999831 garden_ai-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 garden_ai-0.4.3/PKG-INFO
```

### Comparing `garden_ai-0.4.2/LICENSE` & `garden_ai-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.2/README.md` & `garden_ai-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.2/garden_ai/app/garden.py` & `garden_ai-0.4.3/garden_ai/app/garden.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 import rich
 import typer
 from globus_sdk import SearchAPIError
 from rich.prompt import Prompt
 
 from garden_ai import local_data
 from garden_ai.client import GardenClient
-from garden_ai.globus_search.garden_search import GARDEN_INDEX_UUID
+from garden_ai.globus_search.garden_search import (
+    GARDEN_INDEX_UUID,
+    RemoteGardenException,
+)
 from garden_ai.gardens import Garden
 from garden_ai.pipelines import RegisteredPipeline
+from garden_ai.app.console import console, get_local_garden_rich_table
 
 logger = logging.getLogger()
 
 garden_app = typer.Typer(name="garden", no_args_is_help=True)
 
 
 def validate_name(name: str) -> str:
@@ -135,23 +139,19 @@
         contributors=contributors,
         tags=tags,
     )
 
     local_data.put_local_garden(garden)
 
     if verbose:
-        metadata = json.dumps(local_data.get_local_garden_by_uuid(garden.uuid))
+        metadata = json.dumps(local_data.get_local_garden_by_doi(garden.doi))
         rich.print_json(metadata)
 
     if garden.doi:
         rich.print(f"Garden '{garden.title}' created with DOI: {garden.doi}")
-    else:
-        rich.print(
-            f"Garden '{garden.title}' created but missing DOI. Given UUID: {garden.uuid}"
-        )
 
     return
 
 
 @garden_app.command(no_args_is_help=True)
 def search(
     title: Optional[str] = typer.Option(
@@ -223,23 +223,23 @@
 
 @garden_app.command(no_args_is_help=True)
 def add_pipeline(
     garden_id: str = typer.Option(
         ...,
         "-g",
         "--garden",
-        prompt="Please enter the UUID or DOI of a garden",
+        prompt="Please enter the DOI of a garden",
         help="The name of the garden you want to add a pipeline to",
         rich_help_panel="Required",
     ),
     pipeline_id: str = typer.Option(
         ...,
         "-p",
         "--pipeline",
-        prompt="Please enter a the UUID or DOI of a pipeline",
+        prompt="Please enter the DOI of a pipeline",
         help="The name of the pipeline you want to add",
         rich_help_panel="Required",
     ),
     pipeline_alias: Optional[str] = typer.Option(
         None,
         "-a",
         "--alias",
@@ -249,78 +249,110 @@
             "name used when the pipeline was first registered."
         ),
     ),
 ):
     """Add a registered pipeline to a garden"""
 
     garden = _get_garden(garden_id)
+    if not garden:
+        raise typer.Exit(code=1)
     to_add = _get_pipeline(pipeline_id)
+    if not to_add:
+        raise typer.Exit(code=1)
 
     if to_add in garden.pipelines:
         if pipeline_alias:
             old_name = (
                 garden.pipeline_aliases.get(to_add.short_name) or to_add.short_name
             )
             print(
                 f"Pipeline {pipeline_id} is already in Garden {garden_id} as {old_name}. Renaming to {pipeline_alias}."
             )
             garden.rename_pipeline(old_name, pipeline_alias)
     else:
-        garden.pipeline_ids += [to_add.uuid]
+        garden.pipeline_ids += [to_add.doi]
         if pipeline_alias:
             garden.rename_pipeline(to_add.short_name, pipeline_alias)
     local_data.put_local_garden(garden)
     logger.info(f"Added pipeline {pipeline_id} to Garden {garden_id}")
 
 
 @garden_app.command(no_args_is_help=True)
 def publish(
     garden_id: str = typer.Option(
         ...,
         "-g",
         "--garden",
-        prompt="Please enter the UUID or DOI of a garden",
-        help="The UUID or DOI of the garden you want to publish",
+        prompt="Please enter the DOI of a garden",
+        help="The DOI of the garden you want to publish",
         rich_help_panel="Required",
     ),
 ):
     """Push data about a Garden stored to Globus Search so that other users can search for it"""
 
     client = GardenClient()
     garden = _get_garden(garden_id)
-    if not garden.doi:
-        garden.doi = client._mint_doi(garden)
-        local_data.put_local_garden(garden)
+    if not garden:
+        raise typer.Exit(code=1)
     try:
         client.publish_garden_metadata(garden)
-    except SearchAPIError as e:
+    except RemoteGardenException as e:
         logger.fatal(f"Could not publish garden {garden_id}")
-        logger.fatal(e.error_data)
+        logger.fatal(str(e))
         raise typer.Exit(code=1) from e
+    console.print(
+        f"Successfully published garden {garden.title} with DOI {garden.doi}!"
+    )
 
 
-def _get_pipeline(pipeline_id: str) -> RegisteredPipeline:
-    if "/" in pipeline_id:
-        pipeline = local_data.get_local_pipeline_by_doi(pipeline_id)
-    else:
-        pipeline = local_data.get_local_pipeline_by_uuid(pipeline_id)
+@garden_app.command(no_args_is_help=False)
+def list():
+    """Lists all local Gardens."""
+
+    resource_table_cols = ["doi", "title", "description"]
+    table_name = "Local Gardens"
+
+    table = get_local_garden_rich_table(
+        resource_table_cols=resource_table_cols, table_name=table_name
+    )
+    console.print("\n")
+    console.print(table)
+
+
+def _get_pipeline(pipeline_id: str) -> Optional[RegisteredPipeline]:
+    pipeline = local_data.get_local_pipeline_by_doi(pipeline_id)
     if not pipeline:
-        logger.fatal(f"Could not find pipeline with id {pipeline_id}")
-        raise typer.Exit(code=1)
+        logger.warning(f"Could not find pipeline with id {pipeline_id}")
+        return None
     return pipeline
 
 
-def _get_garden(garden_id: str) -> Garden:
-    if "/" in garden_id:
-        garden = local_data.get_local_garden_by_doi(garden_id)
-    else:
-        garden = local_data.get_local_garden_by_uuid(garden_id)
+@garden_app.command(no_args_is_help=True)
+def show(
+    garden_ids: List[str] = typer.Argument(
+        ...,
+        help="The DOIs of the Gardens you want to show the local data for. "
+        "e.g. ``garden show garden1_doi garden2_doi`` will show the local data for both Gardens listed.",
+    ),
+):
+    """Shows all info for some Gardens"""
+
+    for garden_id in garden_ids:
+        garden = _get_garden(garden_id)
+        if garden:
+            rich.print(f"Garden: {garden_id} local data:")
+            rich.print_json(json=garden.json())
+            rich.print("\n")
+
+
+def _get_garden(garden_id: str) -> Optional[Garden]:
+    garden = local_data.get_local_garden_by_doi(garden_id)
     if not garden:
-        logger.fatal(f"Could not find garden with id {garden_id}")
-        raise typer.Exit(code=1)
+        logger.warning(f"Could not find garden with id {garden_id}")
+        return None
     return garden
 
 
 def create_query(
     title: Optional[str] = None,
     authors: List[str] = None,
     year: str = None,
```

### Comparing `garden_ai-0.4.2/garden_ai/app/main.py` & `garden_ai-0.4.3/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.2/garden_ai/app/pipeline.py` & `garden_ai-0.4.3/garden_ai/app/pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 from typing import List, Optional
 
 import jinja2
 import typer
+import rich
 from rich import print
 from rich.prompt import Prompt
+from rich.progress import Progress, SpinnerColumn, TextColumn
 
-from garden_ai import GardenClient, Pipeline, step
-from garden_ai.app.console import console
-from garden_ai import GardenConstants
+from garden_ai import GardenClient, Pipeline, step, GardenConstants
+from garden_ai.app.console import console, get_local_pipeline_rich_table
+from garden_ai.app.garden import _get_pipeline
 
 from garden_ai.mlmodel import PipelineLoadScaffoldedException
 from garden_ai.utils.filesystem import (
     load_pipeline_from_python_file,
     PipelineLoadException,
-    PipelineLoadMlFlowException,
 )
 
 from garden_ai.utils.misc import clean_identifier
 
 
 logger = logging.getLogger()
 
@@ -210,21 +211,154 @@
             f"{pipeline_file} is not a valid Python file. Please provide a valid Python file (.py)."
         )
         raise typer.Exit(code=1)
     try:
         user_pipeline = load_pipeline_from_python_file(pipeline_file)
     except (
         PipelineLoadException,
-        PipelineLoadMlFlowException,
         PipelineLoadScaffoldedException,
     ) as e:
         console.log(f"Could not parse {pipeline_file} as a Garden pipeline. " + str(e))
         raise typer.Exit(code=1) from e
 
     with console.status(
         "[bold green]Building container. This operation times out after 30 minutes."
     ):
         container_uuid = client.build_container(user_pipeline)
     console.print(f"Created container {container_uuid}")
     func_uuid = client.register_pipeline(user_pipeline, container_uuid)
     console.print(f"Created function {func_uuid}")
-    console.print("Done! Pipeline is registered.")
+    console.print(f"Done! Pipeline was registered with doi {user_pipeline.doi}.")
+
+
+@pipeline_app.command()
+def shell(
+    pipeline_file: Path = typer.Argument(
+        None,
+        dir_okay=False,
+        file_okay=True,
+        resolve_path=True,
+        help=("Path to a Python file containing your pipeline implementation."),
+    ),
+    requirements_file: Path = typer.Argument(
+        None,
+        dir_okay=False,
+        file_okay=True,
+        resolve_path=True,
+        help=("Path to a Python file containing your pipeline requirements."),
+    ),
+    env_name: Path = typer.Argument(
+        None,
+        dir_okay=False,
+        file_okay=False,
+        help=("The name to give your pipeline's virtual environment."),
+    ),
+):
+    import os
+    import subprocess
+    import tempfile
+    import sys
+
+    try:
+        # Create a virtual environment in the temp directory
+        temp_dir = os.path.join(os.path.sep, tempfile.gettempdir(), env_name)
+        print(f"Setting up environment in {temp_dir} ...")
+        subprocess.run(["python3", "-m", "venv", temp_dir])
+
+        # Activate the environment os dependent
+        if sys.platform == "win32":
+            activate_script = os.path.join(temp_dir, "Scripts", "activate.bat")
+        elif sys.platform == "darwin":
+            activate_script = os.path.join(temp_dir, "bin", "activate")
+        else:
+            activate_script = os.path.join(temp_dir, "bin", "activate")
+
+        subprocess.run(f"source {activate_script}", shell=True)
+
+        # Upgrade pip in the virtual environment quietly
+        subprocess.run(
+            f"{temp_dir}/bin/python3 -m pip install -q --upgrade pip",
+            check=True,
+            shell=True,
+        )
+
+        # Install the requirements with nice spinner
+        with Progress(
+            SpinnerColumn(),
+            TextColumn("[progress.description]{task.description}"),
+            transient=True,
+        ) as progress:
+            progress.add_task(description="Installing requirements...", total=None)
+
+            subprocess.run(
+                f"{temp_dir}/bin/pip install -q -r {requirements_file}",
+                check=True,
+                shell=True,
+            )
+
+        # Start Python shell in the virtual environment with the pipeline file
+        print("Starting Garden test shell. Loading your pipeline one moment...")
+        python_command = os.path.join(temp_dir, "bin", "python")
+        subprocess.run([python_command, "-i", pipeline_file])
+
+        # Clean up prompt for the temporary environment
+        cleanup = typer.confirm(
+            "Would you like to cleanup (delete) the virtual environment?"
+        )
+        if cleanup:
+            with Progress(
+                SpinnerColumn(),
+                TextColumn("[progress.description]{task.description}"),
+                transient=True,
+            ) as progress:
+                progress.add_task(
+                    description="Removing up virtual environment...", total=None
+                )
+                import shutil
+
+                shutil.rmtree(
+                    temp_dir
+                )  # Remove the directory listed under temp_dir not the actual tmp directory
+        else:
+            print(
+                f"Virtual environment at {temp_dir} still remains and can be used for futher testing or manual removal."
+            )
+
+        print("Local Garden pipeline shell testing complete.")
+
+    except Exception as e:
+        # MVP error handling
+        print(f"An error occurred: {e}")
+
+
+@pipeline_app.command(no_args_is_help=False)
+def list():
+    """Lists all local pipelines."""
+
+    resource_table_cols = ["doi", "title", "description"]
+    table_name = "Local Pipelines"
+
+    table = get_local_pipeline_rich_table(
+        resource_table_cols=resource_table_cols, table_name=table_name
+    )
+    console.print("\n")
+    console.print(table)
+
+
+@pipeline_app.command(no_args_is_help=True)
+def show(
+    pipeline_ids: List[str] = typer.Argument(
+        ...,
+        help="The DOIs of the pipelines you want to show the local data for. "
+        "e.g. ``pipeline show pipeline1_doi pipeline2_doi`` will show the local data for both pipelines listed.",
+    ),
+):
+    """Shows all info for some Gardens"""
+
+    for pipeline_id in pipeline_ids:
+        pipeline = _get_pipeline(pipeline_id)
+        if pipeline:
+            rich.print(f"Pipeline: {pipeline_id} local data:")
+            rich.print_json(json=pipeline.json())
+            rich.print("\n")
+        else:
+            rich.print(f"Could not find pipeline with id {pipeline_id}\n")
```

### Comparing `garden_ai-0.4.2/garden_ai/client.py` & `garden_ai-0.4.3/garden_ai/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,44 +3,47 @@
 import logging
 import os
 import time
 from pathlib import Path
 from typing import List, Optional, Union
 from uuid import UUID
 
-import requests
 import typer
 from globus_compute_sdk import Client
 from globus_sdk import (
     AuthAPIError,
     AuthClient,
     GroupsClient,
     NativeAppAuthClient,
     RefreshTokenAuthorizer,
     SearchClient,
-    GlobusHTTPResponse,
+    ClientCredentialsAuthorizer,
+    ConfidentialAppAuthClient,
 )
 from globus_sdk.scopes import AuthScopes, ScopeBuilder, SearchScopes
 from globus_sdk.tokenstorage import SimpleJSONFileAdapter
 from rich import print
 from rich.prompt import Prompt
 
 import garden_ai.funcx_bandaid.serialization_patch  # type: ignore # noqa: F401
-from garden_ai import local_data
+from garden_ai import local_data, GardenConstants
 from garden_ai.gardens import Garden
 from garden_ai.globus_compute.containers import build_container
 from garden_ai.globus_compute.login_manager import ComputeLoginManager
 from garden_ai.globus_compute.remote_functions import register_pipeline
 from garden_ai.globus_search import garden_search
+from garden_ai.backend_client import BackendClient
+from garden_ai.model_file_transfer.upload import upload_mlmodel_to_s3
 
 from garden_ai.local_data import GardenNotFoundException, PipelineNotFoundException
 from garden_ai.mlmodel import (
     LocalModel,
-    RegisteredModel,
-    upload_to_model_registry,
+    ModelMetadata,
+    stage_model_for_upload,
+    clear_mlflow_staging_directory,
 )
 from garden_ai.pipelines import Pipeline, RegisteredPipeline
 from garden_ai.utils.misc import extract_email_from_globus_jwt
 
 GARDEN_ENDPOINT = os.environ.get(
     "GARDEN_ENDPOINT",
     "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod",
@@ -52,15 +55,16 @@
 
 
 class AuthException(Exception):
     pass
 
 
 GardenScopes = ScopeBuilder(
-    "0948a6b0-a622-4078-b0a4-bfd6d77d65cf", known_url_scopes=["action_all"]
+    "0948a6b0-a622-4078-b0a4-bfd6d77d65cf",
+    known_url_scopes=["action_all", "test_scope"],
 )
 
 
 class GardenClient:
     """
     Main class for interacting with the Garden service
     Holds helper operations for performing common tasks
@@ -72,58 +76,87 @@
     Raises:
          AuthException: if the user cannot authenticate
     """
 
     scopes = GardenScopes
 
     def __init__(
-        self, auth_client: AuthClient = None, search_client: SearchClient = None
+        self,
+        auth_client: Union[AuthClient, ConfidentialAppAuthClient] = None,
+        search_client: SearchClient = None,
     ):
-        key_store_path = Path(os.path.expanduser("~/.garden"))
+        key_store_path = Path(GardenConstants.GARDEN_DIR)
         key_store_path.mkdir(exist_ok=True)
         self.auth_key_store = SimpleJSONFileAdapter(
             os.path.join(key_store_path, "tokens.json")
         )
         self.client_id = os.environ.get(
             "GARDEN_CLIENT_ID", "cf9f8938-fb72-439c-a70b-85addf1b8539"
         )
 
-        self.auth_client = (
-            NativeAppAuthClient(self.client_id) if not auth_client else auth_client
-        )
-        self.openid_authorizer = self._create_authorizer(
-            AuthClient.scopes.resource_server
-        )
-        self.groups_authorizer = self._create_authorizer(
-            GroupsClient.scopes.resource_server
-        )
-        self.search_authorizer = self._create_authorizer(
-            SearchClient.scopes.resource_server
-        )
-        self.compute_authorizer = self._create_authorizer(COMPUTE_RESOURCE_SERVER_NAME)
-        self.search_client = (
-            SearchClient(authorizer=self.search_authorizer)
-            if not search_client
-            else search_client
-        )
-        self.garden_authorizer = self._create_authorizer(
-            GardenClient.scopes.resource_server
-        )
+        # If auth_client is type AuthClient or None, do an
+        # Authorization Code Grant and make RefreshTokenAuthorizers.
+        # If auth_client is type ConfidentialAppAuthClient, do a
+        # Client Credentials Grant and make ClientCredentialsAuthorizers
+        if (
+            isinstance(auth_client, AuthClient)
+            and not isinstance(auth_client, ConfidentialAppAuthClient)
+        ) or not auth_client:
+            self.auth_client = (
+                NativeAppAuthClient(self.client_id) if not auth_client else auth_client
+            )
+            self.openid_authorizer = self._create_authorizer(
+                AuthClient.scopes.resource_server
+            )
+            self.groups_authorizer = self._create_authorizer(
+                GroupsClient.scopes.resource_server
+            )
+            self.search_authorizer = self._create_authorizer(
+                SearchClient.scopes.resource_server
+            )
+            self.compute_authorizer = self._create_authorizer(
+                COMPUTE_RESOURCE_SERVER_NAME
+            )
+            self.search_client = (
+                SearchClient(authorizer=self.search_authorizer)
+                if not search_client
+                else search_client
+            )
+            self.garden_authorizer = self._create_authorizer(
+                GardenClient.scopes.resource_server
+            )
+        elif isinstance(auth_client, ConfidentialAppAuthClient):
+            self.auth_client = auth_client
+            self.openid_authorizer = ClientCredentialsAuthorizer(
+                self.auth_client,
+                f"{AuthClient.scopes.openid} {AuthClient.scopes.email}",
+            )
+            self.groups_authorizer = ClientCredentialsAuthorizer(
+                self.auth_client, GroupsClient.scopes.view_my_groups_and_memberships
+            )
+            self.search_authorizer = ClientCredentialsAuthorizer(
+                self.auth_client, SearchClient.scopes.all
+            )
+            self.compute_authorizer = ClientCredentialsAuthorizer(
+                self.auth_client, Client.FUNCX_SCOPE
+            )
+            self.search_client = SearchClient(authorizer=self.search_authorizer)
+            self.garden_authorizer = ClientCredentialsAuthorizer(
+                self.auth_client, GardenClient.scopes.test_scope
+            )
+
+            local_data._store_user_email(GardenConstants.GARDEN_TEST_EMAIL)
 
         self.compute_client = self._make_compute_client()
-        self._set_up_mlflow_env()
+        self.backend_client = BackendClient(self.garden_authorizer)
 
     def _get_garden_access_token(self):
         self.garden_authorizer.ensure_valid_token()
         return self.garden_authorizer.access_token
 
-    def _set_up_mlflow_env(self):
-        os.environ["MLFLOW_TRACKING_TOKEN"] = self._get_garden_access_token()
-        os.environ["MLFLOW_TRACKING_URI"] = GARDEN_ENDPOINT + "/mlflow"
-
     def _make_compute_client(self):
         scope_to_authorizer = {
             AuthScopes.openid: self.openid_authorizer,
             SearchScopes.all: self.search_authorizer,
             Client.FUNCX_SCOPE: self.compute_authorizer,
         }
         compute_login_manager = ComputeLoginManager(scope_to_authorizer)
@@ -132,15 +165,15 @@
     def _do_login_flow(self):
         self.auth_client.oauth2_start_flow(
             requested_scopes=[
                 AuthClient.scopes.openid,
                 AuthClient.scopes.email,
                 GroupsClient.scopes.view_my_groups_and_memberships,
                 SearchClient.scopes.all,
-                GardenClient.scopes.action_all,
+                GardenClient.scopes.test_scope,
                 Client.FUNCX_SCOPE,
             ],
             refresh_tokens=True,
         )
         authorize_url = self.auth_client.oauth2_get_authorize_url()
 
         print(
@@ -231,251 +264,209 @@
             pea_garden.tags += ["Genetics"] # (didn't have the word for it earlier)
         """
         data = dict(kwargs)
         if authors:
             data["authors"] = authors
         if title:
             data["title"] = title
+        data["doi"] = data.get("doi") or self._mint_draft_doi()
+
         return Garden(**data)
 
     def create_pipeline(
         self, authors: Optional[List[str]] = None, title: Optional[str] = None, **kwargs
     ) -> Pipeline:
         """Initialize and return a pipeline object.
 
-        If this pipeline's UUID has been used before to register a function for
+        If this pipeline's DOI has been used before to register a function for
         remote execution, reuse the (funcx/globus compute) ID for consistency.
 
         NOTE: this means that local modifications to a pipeline will not be
         reflected when executing remotely until the pipeline is re-registered.
         """
         data = dict(kwargs)
         if authors:
             data["authors"] = authors
         if title:
             data["title"] = title
+        data["doi"] = data.get("doi") or self._mint_draft_doi()
 
-        pipeline = Pipeline(**data)
-        record = local_data.get_local_pipeline_by_uuid(pipeline.uuid)
-        if record:
-            logger.info("Found pre-registered pipeline. Reusing DOI.")
-            pipeline.doi = record.doi
-
-        return pipeline
+        return Pipeline(**data)
 
-    def register_model(self, local_model: LocalModel) -> RegisteredModel:
-        registered_model = upload_to_model_registry(local_model)
+    def register_model(self, local_model: LocalModel) -> ModelMetadata:
+        try:
+            # Create directory in MLModel format
+            model_directory = stage_model_for_upload(local_model)
+            # Push contents of directory to S3
+            upload_mlmodel_to_s3(model_directory, local_model, self.backend_client)
+        finally:
+            try:
+                clear_mlflow_staging_directory()
+            except Exception as e:
+                logger.error(
+                    "Could not clean up model staging directory. Check permissions on ~/.garden/mlflow"
+                )
+                logger.error("Original exception: " + str(e))
+                # We can still proceed, there is just some cruft in the user's home directory.
+                pass
+        registered_model = ModelMetadata(**local_model.dict())
         local_data.put_local_model(registered_model)
         return registered_model
 
-    def _mint_doi(
-        self, obj: Union[Garden, Pipeline], force: bool = False, test: bool = True
-    ) -> str:
-        """Register a new "findable" doi with DataCite via Garden backend.
+    def _mint_draft_doi(self, test: bool = True) -> str:
+        """Register a new draft doi with DataCite via Garden backend.
 
         Expects environment variable GARDEN_ENDPOINT to be set (not including `/doi`).
 
         Parameters
         ----------
-        obj : Union[Garden, Pipeline]
-            the Pipeline or Garden object wanting a new DOI.
-        force : bool
-            Mint a new DOI even if one exists (note that old ones stay
-            "findable" forever - see
-            https://support.datacite.org/docs/best-practices-for-datacite-members)
         test : bool
             toggle which garden backend endpoint to hit; we do not yet have a
-            test endpoint so test=True raises NotImplementedError.
+            test endpoint so test=False raises NotImplementedError.
 
         Raises
         ------
         NotImplementedError
             see `test`
-
         """
 
         if not test:
             raise NotImplementedError
 
-        def get_existing_doi() -> Optional[str]:
-            # check for existing doi, either on object or in db
-            registered_obj: Optional[Union[Garden, RegisteredPipeline]]
-            if isinstance(obj, Garden):
-                registered_obj = local_data.get_local_garden_by_uuid(obj.uuid)
-            else:
-                registered_obj = local_data.get_local_pipeline_by_uuid(obj.uuid)
-
-            return registered_obj.doi if registered_obj else None
-
-        existing_doi = obj.doi or get_existing_doi()
-
-        if existing_doi and not force:
-            logger.info(
-                "existing DOI found, not requesting new DOI. Pass `force=true` to override this behavior."
-            )
-            return existing_doi
-
-        logger.info("Requesting DOI")
-        url = f"{GARDEN_ENDPOINT}/doi"
-
-        header = {
-            "Content-Type": "application/vnd.api+json",
-            "Authorization": self.garden_authorizer.get_authorization_header(),
-        }
+        logger.info("Requesting draft DOI")
+        payload = {
+            "data": {"type": "dois", "attributes": {}}
+        }  # required data is filled in on the backend
+        return self.backend_client.mint_doi_on_datacite(payload)
+
+    def _update_datacite(self, obj: Union[Garden, Pipeline]) -> None:
+        logger.info("Requesting update to DOI")
         metadata = json.loads(obj.datacite_json())
-        metadata.update(event="publish", url="https://thegardens.ai")
+        metadata.update(event="publish", url=f"https://thegardens.ai/{obj.doi}")
+
         payload = {"data": {"type": "dois", "attributes": metadata}}
-        r = requests.post(
-            url,
-            headers=header,
-            json=payload,
-        )
-        try:
-            r.raise_for_status()
-            doi = r.json()["doi"]
-        except requests.HTTPError:
-            logger.error(f"{r.text}")
-            raise
-        else:
-            return doi
+        self.backend_client.update_doi_on_datacite(payload)
+        logger.info("Update request succeeded")
 
     def build_container(self, pipeline: Pipeline) -> str:
         built_container_uuid = build_container(self.compute_client, pipeline)
         return built_container_uuid
 
     def register_pipeline(self, pipeline: Pipeline, container_uuid: str) -> str:
         func_uuid = register_pipeline(self.compute_client, pipeline, container_uuid)
         pipeline.func_uuid = UUID(func_uuid)
-        pipeline.doi = self._mint_doi(pipeline)
+        self._update_datacite(pipeline)
         registered = RegisteredPipeline.from_pipeline(pipeline)
         local_data.put_local_pipeline(registered)
         return func_uuid
 
-    def get_registered_pipeline(
-        self, identifier: Union[UUID, str]
-    ) -> RegisteredPipeline:
-        """Return a callable ``RegisteredPipeline`` corresponding to the given uuid/doi.
+    def get_registered_pipeline(self, doi: str) -> RegisteredPipeline:
+        """Return a callable ``RegisteredPipeline`` corresponding to the given doi.
 
         Parameters
         ----------
-        identifier : Union[UUID, str]
-            The previously registered pipeline's DOI or UUID. Raises an
+        doi : str
+            The previously registered pipeline's DOI. Raises an
             exception if not found.
 
         Returns
         -------
         RegisteredPipeline
             Instance of ``RegisteredPipeline``, which can be run on
-            a specified remote Globus Compute endpoint (and knows how to
-            set the appropriate MLFlow environment variables).
+            a specified remote Globus Compute endpoint.
 
         Raises
         ------
         PipelineNotFoundException
             Raised when no known pipeline exists with the given identifier.
         """
-        is_doi = "/" in str(identifier)
-        if is_doi:
-            registered = local_data.get_local_pipeline_by_doi(str(identifier))
-        else:
-            registered = local_data.get_local_pipeline_by_uuid(identifier)
+        pipeline = local_data.get_local_pipeline_by_doi(doi)
 
-        if registered is None:
+        if pipeline is None:
             raise PipelineNotFoundException(
-                f"Could not find any pipelines with identifier {identifier}."
+                f"Could not find any pipelines with DOI {doi}."
             )
-
-        self._set_up_mlflow_env()
-        registered._env_vars = {
-            "MLFLOW_TRACKING_TOKEN": os.environ["MLFLOW_TRACKING_TOKEN"],
-            "MLFLOW_TRACKING_URI": os.environ["MLFLOW_TRACKING_URI"],
-        }
-
-        return registered
-
-    def _fresh_mlflow_vars(self):
-        self._set_up_mlflow_env()
-        return {
-            "MLFLOW_TRACKING_TOKEN": os.environ["MLFLOW_TRACKING_TOKEN"],
-            "MLFLOW_TRACKING_URI": os.environ["MLFLOW_TRACKING_URI"],
-        }
+        pipeline_url_json = self.generate_presigned_urls_for_pipeline(pipeline)
+        pipeline._env_vars = {GardenConstants.URL_ENV_VAR_NAME: pipeline_url_json}
+        return pipeline
 
     def get_email(self) -> str:
         return local_data._get_user_email()
 
-    def get_local_garden(self, identifier: Union[UUID, str]) -> Garden:
-        """Return a registered ``Garden`` corresponding to the given uuid/doi.
+    def get_local_garden(self, doi: str) -> Garden:
+        """Return a registered ``Garden`` corresponding to the given doi.
 
         Any ``RegisteredPipelines`` registered to the Garden will be callable
         as attributes on the garden by their (registered) short_name, e.g.
             ```python
-                my_garden = client.get_local_garden('garden-doi-or-uuid')
+                my_garden = client.get_local_garden('garden-doi')
                 #  pipeline would have been registered with short_name='my_pipeline'
                 my_garden.my_pipeline(*args, endpoint='where-to-execute')
             ```
         Tip: To access the pipeline by a different name, use ``my_garden.rename_pipeline(old_name, new_name)``.
         To persist a new name for a pipeline, re-register it to the garden and specify an alias.
 
         Parameters
         ----------
-        identifier : Union[UUID, str]
-            The previously registered Garden's DOI or UUID. Raises an
+        doi : str
+            The previously registered Garden's DOI. Raises an
             exception if not found.
 
         """
-        is_doi = "/" in str(identifier)
-        if is_doi:
-            registered = local_data.get_local_garden_by_doi(str(identifier))
-        else:
-            registered = local_data.get_local_garden_by_uuid(identifier)
+        garden = local_data.get_local_garden_by_doi(doi)
 
-        if registered is None:
+        if garden is None:
             raise GardenNotFoundException(
-                f"Could not find any Gardens with identifier {identifier}."
+                f"Could not find any Gardens with identifier {doi}."
             )
-        self._set_up_mlflow_env()
-        registered._env_vars = {
-            "MLFLOW_TRACKING_TOKEN": os.environ["MLFLOW_TRACKING_TOKEN"],
-            "MLFLOW_TRACKING_URI": os.environ["MLFLOW_TRACKING_URI"],
-        }
-        return registered
+        self._generate_presigned_urls_for_garden(garden)
+        return garden
 
-    def publish_garden_metadata(self, garden: Garden) -> GlobusHTTPResponse:
+    def publish_garden_metadata(self, garden: Garden) -> None:
         """
-        Takes a garden, and publishes to the GARDEN_INDEX_UUID index.  Polls
-        to discover status, and returns the Task document.
-        Task document has a task["state"] field that can be FAILED or SUCCESS.
-
-        Returns
-        -------
-        https://docs.globus.org/api/search/reference/get_task/#task
+        Publishes a Garden's expanded_json to the backend /garden-search-route,
+        making it visible on our Globus Search index.
         """
-        return garden_search.publish_garden_metadata(garden, self.search_client)
+        self._update_datacite(garden)
+        try:
+            self.backend_client.publish_garden_metadata(garden)
+        except Exception as e:
+            raise Exception(
+                f"Request to Garden backend to publish garden failed with error: {str(e)}"
+            )
 
     def search(self, query: str) -> str:
         """
         Given a Globus Search advanced query, returns JSON Globus Search result string with gardens as entries.
         """
         return garden_search.search_gardens(query, self.search_client)
 
-    def get_published_garden(self, identifier: str) -> Garden:
+    def get_published_garden(self, doi: str) -> Garden:
         """
         Queries Globus Search for the garden with this DOI.
 
         Parameters
         ----------
-        identifier: The doi or uuid of the garden you want.
+        doi: The doi of the garden you want.
 
         Returns
         -------
         Garden populated with metadata from remote metadata record.
 
         """
-        is_doi = "/" in str(identifier)
-        if is_doi:
-            return garden_search.get_remote_garden_by_doi(
-                identifier, self._fresh_mlflow_vars(), self.search_client
-            )
-        else:
-            return garden_search.get_remote_garden_by_uuid(
-                identifier, self._fresh_mlflow_vars(), self.search_client
-            )
+        garden = garden_search.get_remote_garden_by_doi(doi, self.search_client)
+        self._generate_presigned_urls_for_garden(garden)
+        return garden
+
+    def _generate_presigned_urls_for_garden(self, garden: Garden):
+        for pipeline in garden.pipelines:
+            pipeline_url_json = self.generate_presigned_urls_for_pipeline(pipeline)
+            pipeline._env_vars = {GardenConstants.URL_ENV_VAR_NAME: pipeline_url_json}
+
+    def generate_presigned_urls_for_pipeline(
+        self, pipeline: Union[RegisteredPipeline, Pipeline]
+    ) -> str:
+        model_name_to_url = {}
+        for model_name in pipeline.model_full_names:
+            url = self.backend_client.get_model_download_url(model_name).url
+            model_name_to_url[model_name] = url
+        return json.dumps(model_name_to_url)
```

### Comparing `garden_ai-0.4.2/garden_ai/datacite.py` & `garden_ai-0.4.3/garden_ai/datacite.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 
 class DataciteSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     # tweaked identifiers, no longer requires at least one. (only change from generated code)
     types: Types
-    identifiers: List[Identifier] = Field(default_factory=list, unique_items=True)
+    identifiers: List[Identifier] = Field(..., min_items=1, unique_items=True)
     creators: List[Creator] = Field(..., min_items=1, unique_items=True)
     titles: List[Title] = Field(..., min_items=1, unique_items=True)
     publisher: str
     publicationYear: str
     subjects: Optional[List[Subject]] = Field(None, unique_items=True)
     contributors: Optional[List[Contributor]] = Field(None, unique_items=True)
     dates: Optional[List[DateModel]] = Field(None, unique_items=True)
```

### Comparing `garden_ai-0.4.2/garden_ai/funcx_bandaid/serialization_patch.py` & `garden_ai-0.4.3/garden_ai/funcx_bandaid/serialization_patch.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.2/garden_ai/gardens.py` & `garden_ai-0.4.3/garden_ai/gardens.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from __future__ import annotations
 
 import json
 import logging
 from datetime import datetime
 from typing import Any, Dict, List, Optional, cast
-from uuid import UUID, uuid4
 
-from pydantic import BaseModel, Field, PrivateAttr, ValidationError, validator
+from pydantic import (
+    BaseModel,
+    Field,
+    PrivateAttr,
+    ValidationError,
+    root_validator,
+    validator,
+)
 
 from garden_ai.utils.misc import JSON, garden_json_encoder
 
 from .datacite import (
     Contributor,
     Creator,
     DataciteSchema,
     Description,
+    Identifier,
     RelatedIdentifier,
+    Subject,
     Title,
     Types,
 )
 from .pipelines import RegisteredPipeline
 
 logger = logging.getLogger()
 
@@ -52,15 +60,15 @@
             also `pipeline_names` attribute.
 
         pipeline_names (list[str]):
             List of python identifiers (i.e. variable names) usable for this \
             garden's pipelines.  Takes aliases into account (set when adding \
             pipeline via CLI or using `rename_pipeline` method.)
 
-        pipeline_ids: List[UUID] = Field(default_factory=list)
+        pipeline_ids: List[str] = Field(default_factory=list)
         pipeline_aliases: Dict[str, str] = Field(default_factory=dict)
 
         doi (str):
             A garden's doi usable for citations, generated automatically via \
             DataCite using the required fields.
 
         version (str):
@@ -96,27 +104,34 @@
         To remedy this, if the `doi` field is unset when publishing a garden, we \
         build one for the user with the datacite api.
     """
 
     title: str = cast(str, Field(default_factory=lambda: None))
     authors: List[str] = Field(default_factory=list, min_items=1, unique_items=True)
     contributors: List[str] = Field(default_factory=list, unique_items=True)
-    doi: Optional[str] = Field(default=None)
+    doi: str = Field(...)
     description: Optional[str] = Field(None)
     publisher: str = "Garden-AI"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     language: str = "en"
     tags: List[str] = Field(default_factory=list, unique_items=True)
     version: str = "0.0.1"
-    uuid: UUID = Field(default_factory=uuid4, allow_mutation=False)
-    pipeline_ids: List[UUID] = Field(default_factory=list)
+    pipeline_ids: List[str] = Field(default_factory=list)
     pipeline_aliases: Dict[str, str] = Field(default_factory=dict)
     _pipelines: List[RegisteredPipeline] = PrivateAttr(default_factory=list)
     _env_vars: Dict[str, str] = PrivateAttr(default_factory=dict)
 
+    @root_validator(pre=True)
+    def doi_omitted(cls, values):
+        assert "doi" in values, (
+            "It seems like no DOI has been minted yet for this `Garden`. If you were trying to create a new `Garden`, "
+            "use `GardenClient.create_garden` to initialize a publishable `Garden` with a draft DOI."
+        )
+        return values
+
     @validator("year")
     def valid_year(cls, year):
         if len(str(year)) != 4:
             raise ValueError("year must be formatted `YYYY`")
         return str(year)
 
     @property
@@ -145,20 +160,20 @@
         Given a list of dicts in RegisteredPipeline format (as from Globus Search),
         attempt to convert them to RegisteredPipelines and use them to populate _pipelines.
         """
         pipelines = []
         for meta in pipeline_metadata:
             try:
                 pipeline = RegisteredPipeline(**meta)
-                if pipeline.uuid in self.pipeline_ids:
+                if pipeline.doi in self.pipeline_ids:
                     pipeline._env_vars = self._env_vars
                     pipelines.append(pipeline)
                 else:
                     logger.warning(
-                        f"Remote pipeline {pipeline.uuid} not present in pipeline id list."
+                        f"Remote pipeline {pipeline.doi} not present in pipeline id list."
                     )
             except ValidationError as e:
                 logger.warning(
                     f"Could not parse pipeline: {json.dumps(meta)}. {e.__str__()}"
                 )
 
         self._pipelines = pipelines
@@ -170,35 +185,35 @@
         Note:
             It is recommended to use the `garden.pipelines` computed property to avoid running this method multiple times.
 
         Returns:
             A list of RegisteredPipeline objects.
         """
 
-        from .local_data import PipelineNotFoundException, get_local_pipeline_by_uuid
+        from .local_data import PipelineNotFoundException, get_local_pipeline_by_doi
 
         pipelines = []
-        for uuid in self.pipeline_ids:
-            pipeline = get_local_pipeline_by_uuid(uuid)
+        for doi in self.pipeline_ids:
+            pipeline = get_local_pipeline_by_doi(doi)
             if pipeline is None:
                 raise PipelineNotFoundException(
-                    f"Could not find registered pipeline with id {uuid}."
+                    f"Could not find registered pipeline with id {doi}."
                 )
             # set env vars for pipeline to use when remotely executing
             pipeline._env_vars = self._env_vars
 
             pipelines += [pipeline]
 
         return pipelines
 
     def expanded_metadata(self) -> Dict[str, Any]:
         """
         Helper method: builds the "complete" metadata dictionary with nested `Pipeline` and `step` metadata.
 
-        When serializing normally with `garden.{dict(), json()}`, only the UUIDs of the pipelines in the garden are included.
+        When serializing normally with `garden.{dict(), json()}`, only the DOIs of the pipelines in the garden are included.
 
         This method returns a superset of `garden.dict()`, so that the following holds:
             valid_garden == Garden(**valid_garden.expanded_metadata()) == Garden(**valid_garden.dict())
 
         Returns:
             A dictionary containing the `Garden` metadata augmented with a list of `RegisteredPipeline` metadata.
 
@@ -223,31 +238,33 @@
         # Leverages a pydantic class `DataCiteSchema`, which was automatically generated from:
         # https://github.com/datacite/schema/blob/master/source/json/kernel-4.3/datacite_4.3_schema.json
         #
         # The JSON returned by this method would be the "attributes" part of a DataCite request body.
 
         self._sync_author_metadata()
         return DataciteSchema(  # type: ignore
+            identifiers=[Identifier(identifier=self.doi, identifierType="DOI")],
             types=Types(resourceType="AI/ML Garden", resourceTypeGeneral="Software"),
             creators=[Creator(name=name) for name in self.authors],
             titles=[Title(title=self.title)],
             publisher="thegardens.ai",
             publicationYear=self.year,
+            subjects=[Subject(subject=tag) for tag in self.tags],
             contributors=[
                 Contributor(name=name, contributorType="Other")
                 for name in self.contributors
             ],
             language=self.language,
             relatedIdentifiers=[
                 RelatedIdentifier(
-                    relatedIdentifier=p.doi,
+                    relatedIdentifier=doi,
                     relatedIdentifierType="DOI",
                     relationType="HasPart",
                 )
-                for p in self.pipelines
+                for doi in self.pipeline_ids
             ],
             version=self.version,
             descriptions=[
                 Description(description=self.description, descriptionType="Other")
             ]
             if self.description
             else None,
```

### Comparing `garden_ai-0.4.2/garden_ai/globus_compute/containers.py` & `garden_ai-0.4.3/garden_ai/globus_compute/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     queued = "queued"
     building = "building"
     ready = "ready"
     failed = "failed"
 
 
 def build_container(compute_client: Client, pipeline: Pipeline) -> str:
-    name = str(pipeline.uuid)
+    name = str(pipeline.doi)
     cs = ContainerSpec(
         name=name,
         pip=pipeline.pip_dependencies,
         python_version=pipeline.python_version,
         conda=pipeline.conda_dependencies,
     )
```

### Comparing `garden_ai-0.4.2/garden_ai/globus_compute/login_manager.py` & `garden_ai-0.4.3/garden_ai/globus_compute/login_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,24 @@
 
 class ComputeLoginManager:
     """
     Implements the globus_compute_sdk.sdk.login_manager.protocol.LoginManagerProtocol class.
     https://github.com/funcx-faas/funcX/blob/main/funcx_sdk/funcx/sdk/login_manager/protocol.py#L18
     """
 
-    def __init__(self, authorizers: Dict[str, globus_sdk.RefreshTokenAuthorizer]):
+    def __init__(
+        self,
+        authorizers: Dict[
+            str,
+            Union[
+                globus_sdk.RefreshTokenAuthorizer,
+                globus_sdk.ClientCredentialsAuthorizer,
+            ],
+        ],
+    ):
         self.authorizers = authorizers
 
     def get_auth_client(self) -> globus_sdk.AuthClient:
         return globus_sdk.AuthClient(authorizer=self.authorizers[AuthScopes.openid])
 
     def get_search_client(self) -> globus_sdk.SearchClient:
         return globus_sdk.SearchClient(authorizer=self.authorizers[SearchScopes.all])
```

### Comparing `garden_ai-0.4.2/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.4.3/garden_ai/globus_compute/remote_functions.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.2/garden_ai/local_data.py` & `garden_ai-0.4.3/garden_ai/local_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import json
 import logging
 from enum import Enum
 from pathlib import Path
-from typing import Dict, Optional, Union
-from uuid import UUID
+from typing import Dict, Optional, Union, List
 
 from garden_ai.gardens import Garden
 from garden_ai.pipelines import RegisteredPipeline
-from garden_ai.mlmodel import RegisteredModel
+from garden_ai.mlmodel import ModelMetadata
 from garden_ai.utils.misc import garden_json_encoder
+from garden_ai.constants import GardenConstants
 
-LOCAL_STORAGE = Path("~/.garden").expanduser()
+LOCAL_STORAGE = Path(GardenConstants.GARDEN_DIR)
 LOCAL_STORAGE.mkdir(parents=True, exist_ok=True)
 
 logger = logging.getLogger()
 
 
 class LocalDataException(Exception):
     """Exception raised when a user's local data.json is corrupted"""
 
     pass
 
 
 class PipelineNotFoundException(KeyError):
-    """Exception raised when a Garden references an unknown pipeline uuid"""
+    """Exception raised when a Garden references an unknown pipeline doi"""
 
 
 class GardenNotFoundException(KeyError):
-    """Exception raised when no Garden is found with a given uuid"""
+    """Exception raised when no Garden is found with a given doi"""
 
 
 class ResourceType(Enum):
     GARDEN = "gardens"
     PIPELINE = "pipelines"
     MODEL = "models"
 
 
 resource_type_to_id_key = {
-    ResourceType.GARDEN: "uuid",
-    ResourceType.PIPELINE: "uuid",
-    ResourceType.MODEL: "model_uri",
+    ResourceType.GARDEN: "doi",
+    ResourceType.PIPELINE: "doi",
+    ResourceType.MODEL: "full_name",
 }
 
 
 def _read_local_db() -> Dict:
     data = {}
     if (LOCAL_STORAGE / "data.json").exists():
         with open(LOCAL_STORAGE / "data.json", "r+") as f:
@@ -84,171 +84,175 @@
     id_key = resource_type_to_id_key[resource_type]
     resources[str(resource_metadata[id_key])] = resource_metadata
     data[resource_type.value] = resources
     _write_local_db(data)
 
 
 def _put_resource_from_obj(
-    resource: Union[Garden, RegisteredPipeline, RegisteredModel],
+    resource: Union[Garden, RegisteredPipeline, ModelMetadata],
     resource_type: ResourceType,
 ) -> None:
     resource_metadata = resource.dict()
     _put_resource_from_metadata(resource_metadata, resource_type)
 
 
 def _make_obj_from_record(
     record: Dict, resource_type: ResourceType
-) -> Union[Garden, RegisteredPipeline, RegisteredModel]:
+) -> Union[Garden, RegisteredPipeline, ModelMetadata]:
     if resource_type is ResourceType.GARDEN:
         return Garden(**record)
     elif resource_type is ResourceType.PIPELINE:
         return RegisteredPipeline(**record)
     else:
-        return RegisteredModel(**record)
+        return ModelMetadata(**record)
 
 
 def _get_resource_by_id(
-    id_: Union[UUID, str], resource_type: ResourceType
-) -> Optional[Union[Garden, RegisteredPipeline, RegisteredModel]]:
+    id_: str, resource_type: ResourceType
+) -> Optional[Union[Garden, RegisteredPipeline, ModelMetadata]]:
     data = _read_local_db()
-    id_ = str(id_)
     resources = data.get(resource_type.value, {})
     if resources and id_ in resources:
         return _make_obj_from_record(resources[id_], resource_type)
     else:
         return None
 
 
-def _get_resource_by_doi(
-    doi: str, resource_type: ResourceType
-) -> Optional[Union[Garden, RegisteredPipeline, RegisteredModel]]:
-    data = _read_local_db()
-    resources_by_uuid = data.get(resource_type.value, {})
-    resources_by_doi = _reindex_by_doi(resources_by_uuid)
-    if resources_by_doi and doi in resources_by_doi:
-        return _make_obj_from_record(resources_by_doi[doi], resource_type)
-    else:
-        return None
-
-
-def _reindex_by_doi(resources: dict) -> Dict:
-    by_doi = {}
-    for resource in resources.values():
-        if "doi" in resource:
-            by_doi[resource["doi"]] = resource
-    return by_doi
-
-
 def _delete_old_model_versions(model_name: str):
     data = _read_local_db()
     models_by_uri = data.get(ResourceType.MODEL.value, {})
     # Use `list` so that we don't delete items while iterating.
     for k, v in list(models_by_uri.items()):
         if v["model_name"] == model_name:
             del models_by_uri[k]
     data[ResourceType.MODEL.value] = models_by_uri
     _write_local_db(data)
 
 
+def _get_resource_by_type(
+    resource_type: ResourceType,
+) -> Optional[List[Union[Garden, RegisteredPipeline, ModelMetadata]]]:
+    data = _read_local_db()
+    resource_data = data.get(resource_type.value, {})
+    resource_objs = []
+    if resource_data:
+        for key, val in resource_data.items():
+            resource_objs.append(_make_obj_from_record(val, resource_type))
+        return resource_objs
+    else:
+        return None
+
+
 def put_local_garden(garden: Garden):
     """Helper: write a record to 'local database' for a given Garden
-    Overwrites any existing entry with the same uuid in ~/.garden/data.json.
+    Overwrites any existing entry with the same doi in ~/.garden/data.json.
 
     Parameters
     ----------
     garden Garden
         The object to json-serialize and write/update in the local database.
         a TypeError will be raised if not a Garden.
     """
     _put_resource_from_obj(garden, resource_type=ResourceType.GARDEN)
 
 
 def put_local_pipeline(pipeline: RegisteredPipeline):
     """Helper: write a record to 'local database' for a given Pipeline
-    Overwrites any existing entry with the same uuid in ~/.garden/data.json.
+    Overwrites any existing entry with the same doi in ~/.garden/data.json.
 
     Parameters
     ----------
     pipeline Pipeline
         The object to json-serialize and write/update in the local database.
         a TypeError will be raised if not a Pipeline.
     """
     _put_resource_from_obj(pipeline, resource_type=ResourceType.PIPELINE)
 
 
-def get_local_garden_by_uuid(uuid: Union[UUID, str]) -> Optional[Garden]:
+def get_local_garden_by_doi(doi: str) -> Optional[Garden]:
     """Helper: fetch a Garden record from ~/.garden/data.json.
 
     Parameters
     ----------
-    uuid Union[UUID, str]
-        The uuid of the Garden you are fetching.
+    doi str
+        The doi of the Garden you are fetching.
 
     Returns
     -------
     Optional[Garden]
-        If successful, a dictionary in the form given by Garden.json().
     """
-    return _get_resource_by_id(uuid, ResourceType.GARDEN)  # type: ignore
+    return _get_resource_by_id(doi, ResourceType.GARDEN)  # type: ignore
 
 
-def get_local_pipeline_by_uuid(uuid: Union[UUID, str]) -> Optional[RegisteredPipeline]:
+def get_local_pipeline_by_doi(doi: str) -> Optional[RegisteredPipeline]:
     """Helper: fetch a Pipeline record from ~/.garden/data.json.
 
     Parameters
     ----------
-    uuid Union[UUID, str]
-        The uuid of the Pipeline you are fetching.
+    doi str
+        The doi of the Pipeline you are fetching.
 
     Returns
     -------
     Optional[RegisteredPipeline]
     """
-    return _get_resource_by_id(uuid, ResourceType.PIPELINE)  # type: ignore
+    return _get_resource_by_id(doi, ResourceType.PIPELINE)  # type: ignore
 
 
-def get_local_garden_by_doi(doi: str) -> Optional[Garden]:
-    """Helper: fetch a Garden record from ~/.garden/data.json.
+def put_local_model(model: ModelMetadata):
+    """Helper: write a record to 'local database' for a given RegisteredModel
+    Overwrites any existing entry with the same model_name in ~/.garden/data.json.
+
+    Parameters
+    ----------
+    model Model
+        The object to json-serialize and write/update in the local database.
+        a TypeError will be raised if not a Model.
+    """
+    _delete_old_model_versions(model.model_name)
+    _put_resource_from_obj(model, resource_type=ResourceType.MODEL)
+
+
+def get_local_model_by_name(model_full_name: str):
+    return _get_resource_by_id(model_full_name, ResourceType.MODEL)  # type: ignore
+
+
+def get_all_local_gardens() -> Optional[List[Garden]]:
+    """Helper: fetch all Garden records from ~/.garden/data.json.
 
     Parameters
     ----------
-    doi str
-        The doi of the Garden you are fetching.
 
     Returns
     -------
     Optional[Garden]
+        If successful, a list of all the Garden objects in data.json.
     """
-    return _get_resource_by_doi(doi, ResourceType.GARDEN)  # type: ignore
+    return _get_resource_by_type(ResourceType.GARDEN)  # type: ignore
 
 
-def get_local_pipeline_by_doi(doi: str) -> Optional[RegisteredPipeline]:
-    """Helper: fetch a Pipeline record from ~/.garden/data.json.
+def get_all_local_pipelines() -> Optional[List[RegisteredPipeline]]:
+    """Helper: fetch all pipeline records from ~/.garden/data.json.
 
     Parameters
     ----------
-    doi str
-        The doi of the Pipeline you are fetching.
 
     Returns
     -------
     Optional[RegisteredPipeline]
+        If successful, a list of all the RegisteredPipeline objects in data.json.
     """
-    return _get_resource_by_doi(doi, ResourceType.PIPELINE)  # type: ignore
+    return _get_resource_by_type(ResourceType.PIPELINE)  # type: ignore
 
 
-def put_local_model(model: RegisteredModel):
-    """Helper: write a record to 'local database' for a given RegisteredModel
-    Overwrites any existing entry with the same model_name in ~/.garden/data.json.
+def get_all_local_models() -> Optional[List[ModelMetadata]]:
+    """Helper: fetch all model records from ~/.garden/data.json.
 
     Parameters
     ----------
-    model Model
-        The object to json-serialize and write/update in the local database.
-        a TypeError will be raised if not a Model.
-    """
-    _delete_old_model_versions(model.model_name)
-    _put_resource_from_obj(model, resource_type=ResourceType.MODEL)
-
 
-def get_local_model_by_uri(model_uri: str):
-    return _get_resource_by_id(model_uri, ResourceType.MODEL)  # type: ignore
+    Returns
+    -------
+    Optional[ModelMetadata]
+        If successful, a list of all the RegisteredModel objects in data.json.
+    """
+    return _get_resource_by_type(ResourceType.MODEL)  # type: ignore
```

### Comparing `garden_ai-0.4.2/garden_ai/mlmodel.py` & `garden_ai-0.4.3/garden_ai/mlmodel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+import json
 import os
 import pathlib
 import pickle
+import shutil
 from enum import Enum
 from functools import lru_cache
 from typing import List
 
+import requests
+import zipfile
 import mlflow  # type: ignore
 from mlflow.pyfunc import load_model  # type: ignore
 from pydantic import BaseModel, Field, validator
 
-from garden_ai.utils.misc import read_conda_deps
 from garden_ai import GardenConstants
 
+MODEL_STAGING_DIR = pathlib.Path(GardenConstants.GARDEN_DIR) / "mlflow"
+MODEL_STAGING_DIR.mkdir(parents=True, exist_ok=True)
+
 
 class ModelUploadException(Exception):
     """Exception raised when an attempt to upload a model to ML Flow fails"""
 
     pass
 
 
@@ -39,43 +45,45 @@
     type: str = "dataset"
     relationship: str = "origin"
     doi: str = Field(...)
     repository: str = "Foundry"
     url: str = Field(...)
 
 
-class LocalModel(BaseModel):
+class ModelMetadata(BaseModel):
     """
-    The ``LocalModel`` class represents a pre-trained ML model that a user wants to register with Garden.
+    The ``ModelMetadata`` class represents all the metadata we want to \
+    publicly expose about an ML model that has been registered with Garden.
 
     Attributes:
-        model_name (str):
-            A short and descriptive name of the model. Model names can only contain alphanumeric characters, hyphens, and underscores.
-        flavor (str):
-            The framework used for this model. One of "sklearn", "tensorflow", or "torch".
-        extra_pip_requirements (List[str]):
-            A list of additional pip requirements needed to load and/or run the model.
-        local_path (str):
-            Where the model is located on disk. Can be a file or a directory depending on the flavor.
-        user_email (str):
-            The email address of the user uploading the model.
+        model_name (str): A short and descriptive name of the model
+        flavor (str): The framework used for this model. One of "sklearn", "tensorflow", or "torch".
+        connections (List[DatasetConnection]):
+            A list of dataset records that the model was trained on.
+        user_email (str): The email address of the user uploading the model.
+        full_name (str): The user_email and model_name together like "foo@example.edu/my_model"
+        mlflow_name (str): The user_email and model_name together like "foo@example.edu-my_model"
 
     """
 
     model_name: str = Field(...)
-    flavor: str = Field(...)
-    extra_pip_requirements: List[str] = Field(default_factory=list)
-    local_path: str = Field(...)
     user_email: str = Field(...)
+    flavor: str = Field(...)
     connections: List[DatasetConnection] = Field(default_factory=list)
-    namespaced_model_name: str = ""
+    full_name: str = ""
+    mlflow_name: str = ""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.namespaced_model_name = f"{self.user_email}-{self.model_name}"
+        # The / separator is canonical because it is nice for S3
+        # and conveys that your email is a namespace.
+        self.full_name = f"{self.user_email}/{self.model_name}"
+        # But for local MLFlow purposes, use a - separator instead
+        # because MLFlow does not like slashes.
+        self.mlflow_name = f"{self.user_email}-{self.model_name}"
 
     @validator("flavor")
     def must_be_a_supported_flavor(cls, flavor):
         if flavor not in [f.value for f in ModelFlavor]:
             raise ValueError("is not a supported flavor")
         return flavor
 
@@ -87,65 +95,37 @@
                 "is not a valid model name. "
                 "Model names can only contain alphanumeric characters, hyphens, and underscores."
             )
             raise ValueError(error_message)
         return model_name
 
 
-class RegisteredModel(BaseModel):
+class LocalModel(ModelMetadata):
     """
-    The ``RegisteredModel`` class represents all the metadata we want to \
-    publicly expose about an ML model that has been registered with Garden.
+    The ``LocalModel`` class represents a pre-trained ML model that a user wants to register with Garden.
+    It has everything a ModelMetadata has, plus a local_path where the user says the model can be loaded from.
 
-    Attributes:
-        model_name (str): A short and descriptive name of the model
-        version (str): Version string like "1" or "2" for this model.
-        flavor (str): The framework used for this model. One of "sklearn", "tensorflow", or "torch".
-        connections (List[DatasetConnection]):
-            A list of dataset records that the model was trained on.
-        local_path (str): Where the model is located on disk. Can be a file or a directory depending on the flavor.
-        user_email (str): The email address of the user uploading the model.
+    Extra attributes:
+        local_path (str):
+            Where the model is located on disk. Can be a file or a directory depending on the flavor.
 
     """
 
-    model_name: str = Field(...)
-    version: str = Field(...)
-    user_email: str = Field(...)
-    flavor: str = Field(...)
-    connections: List[DatasetConnection] = Field(default_factory=list)
-    namespaced_model_name: str = ""
-    model_uri: str = ""
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.namespaced_model_name = f"{self.user_email}-{self.model_name}"
-        self.model_uri = f"{self.namespaced_model_name}/{self.version}"
-
-
-def upload_to_model_registry(local_model: LocalModel) -> RegisteredModel:
-    """Upload a model to Garden-AI's MLflow model registry.
-
-    Args:
-        local_model: The model to upload.
+    local_path: str = Field(...)
 
-    Returns:
-        RegisteredModel with the full model_uri, which can be used to fetch the \
-        model with a call to ``Model(...)``.
 
-    Raises:
-        ModelUploadException:
-            If an error occurs during the upload process, such as failure to \
-            open or parse the model, or failure to retrieve the latest version \
-            of the model.
+def stage_model_for_upload(local_model: LocalModel) -> str:
     """
-    _push_model_to_registry(local_model)
-    return _assemble_metadata(local_model)
-
+    Parameters
+    ----------
+    local_model: the model to be staged into an MLModel directory
 
-def _push_model_to_registry(local_model: LocalModel):
+    Returns full path of model directory
+    -------
+    """
     flavor, local_path = local_model.flavor, local_model.local_path
     try:
         if flavor == ModelFlavor.SKLEARN.value and pathlib.Path(local_path).is_file:
             with open(local_path, "rb") as f:
                 loaded_model = pickle.load(f)
                 log_model_variant = mlflow.sklearn.log_model
         elif flavor == ModelFlavor.TENSORFLOW.value:
@@ -160,75 +140,155 @@
         elif flavor == ModelFlavor.PYTORCH.value and pathlib.Path(local_path).is_file:
             import torch  # type: ignore
 
             loaded_model = torch.load(local_path)
             log_model_variant = mlflow.pytorch.log_model  # TODO explore signatures
         else:
             raise ModelUploadException(f"Unsupported model flavor {flavor}")
-        log_model_variant(
-            loaded_model,
-            local_model.user_email,
-            registered_model_name=local_model.namespaced_model_name,
-            extra_pip_requirements=local_model.extra_pip_requirements,
-        )
+
+        # Create a folder structure for an experiment called "local" if it doesn't exist
+        # in the user's .garden directory
+        mlflow.set_tracking_uri("file://" + str(MODEL_STAGING_DIR))
+        experiment_name = "local"
+        mlflow.set_experiment(experiment_name)
+        experiment_id = mlflow.get_experiment_by_name(experiment_name).experiment_id
+
+        # The only way to derive the full directory path MLFlow creates is with this context manager.
+        with mlflow.start_run(None, experiment_id) as run:
+            experiment_id = mlflow.active_run().info.experiment_id
+            artifact_path = "model"
+            log_model_variant(
+                loaded_model,
+                artifact_path,
+                registered_model_name=local_model.mlflow_name,
+            )
+            model_dir = os.path.join(
+                str(MODEL_STAGING_DIR),
+                experiment_id,
+                run.info.run_id,
+                "artifacts",
+                artifact_path,
+            )
     except IOError as e:
         raise ModelUploadException("Could not open file " + local_path) from e
-    except pickle.PickleError as e:
+    except (pickle.PickleError, mlflow.MlflowException) as e:
         raise ModelUploadException("Could not parse model at " + local_path) from e
-    except mlflow.MlflowException as e:
-        raise ModelUploadException("Could not upload model.") from e
 
+    return model_dir
 
-def _assemble_metadata(local_model: LocalModel) -> RegisteredModel:
-    client = mlflow.tracking.MlflowClient()
-    versions = client.get_latest_versions(
-        local_model.namespaced_model_name, stages=["None"]
-    )
-    if len(versions) == 0:
-        raise ModelUploadException("Could not retrieve model version.")
-    version_number = versions[0].version
-    return RegisteredModel(
-        **local_model.dict(),
-        version=version_number,
-    )
+
+def clear_mlflow_staging_directory():
+    path = str(MODEL_STAGING_DIR)
+    for item in os.listdir(path):
+        item_path = os.path.join(path, item)
+        if os.path.isfile(item_path):
+            os.remove(item_path)
+        elif os.path.isdir(item_path):
+            shutil.rmtree(item_path)
 
 
 class _Model:
     def __init__(
         self,
         model_full_name: str,
     ):
         self.model = None
-        self.model_full_name = model_full_name
-        self.model_uri = f"models:/{model_full_name}"
+        self.full_name = model_full_name
 
-        # raises error if user trys to load model with the name SCAFFOLDED_MODEL_NAME
-        if self.model_full_name == GardenConstants.SCAFFOLDED_MODEL_NAME:
+        # raises error if user tries to load model with the name SCAFFOLDED_MODEL_NAME
+        if self.full_name == GardenConstants.SCAFFOLDED_MODEL_NAME:
             raise PipelineLoadScaffoldedException("Invalid model name.")
 
-        # extract dependencies without loading model into memory
-        # make it easier for steps to infer
-        conda_yml = mlflow.pyfunc.get_model_dependencies(self.model_uri, format="conda")
-        python_version, conda_dependencies, pip_dependencies = read_conda_deps(
-            conda_yml
-        )
-        self.python_version = python_version
-        self.conda_dependencies = conda_dependencies
-        self.pip_dependencies = pip_dependencies
         return
 
+    def download_and_stage(
+        self, presigned_download_url: str, full_model_name: str
+    ) -> str:
+        try:
+            # Not taking MODEL_STAGING_DIR from constants
+            # so that this class has no external dependencies
+            staging_dir = pathlib.Path(os.path.expanduser("~/.garden")) / "mlflow"
+            download_dir = staging_dir / full_model_name
+            download_dir.mkdir(parents=True, exist_ok=True)
+        except PermissionError as pe:
+            print(f"Could not create model staging directory: {pe}")
+            raise
+
+        zip_filepath = str(download_dir / "model.zip")
+
+        try:
+            response = requests.get(presigned_download_url, stream=True)
+            response.raise_for_status()
+        except requests.RequestException as re:
+            print(
+                f"Could not download model from presigned url. URL: {presigned_download_url}. Error: {re}"
+            )
+            raise
+
+        try:
+            with open(zip_filepath, "wb") as f:
+                f.write(response.content)
+        except IOError as ioe:
+            print(f"Failed to write model to disk at location {zip_filepath}: {ioe}")
+            raise
+
+        extraction_dir = download_dir / "unzipped"
+        unzipped_path = str(download_dir / extraction_dir)
+
+        try:
+            with zipfile.ZipFile(zip_filepath, "r") as zip_ref:
+                zip_ref.extractall(unzipped_path)
+        except (FileNotFoundError, zipfile.BadZipFile) as fe:
+            print(f"Failed to unzip model directory from Garden model repository. {fe}")
+            raise
+
+        return unzipped_path
+
+    @staticmethod
+    def get_download_url(full_model_name: str) -> str:
+        model_url_json = os.environ.get("GARDEN_MODELS", None)
+        if not model_url_json:
+            raise KeyError(
+                "GARDEN_MODELS environment variable was not set. Cannot download model."
+            )
+        try:
+            model_url_dict = json.loads(model_url_json)
+            return model_url_dict[full_model_name]
+        except (json.JSONDecodeError, KeyError):
+            print(
+                f"Could not find url for model {full_model_name} in GARDEN_MODELS env var contents {model_url_json}"
+            )
+            raise
+
+    # Duplicated in this class so that _Model is self-contained
+    @staticmethod
+    def clear_mlflow_staging_directory():
+        staging_dir = pathlib.Path(os.path.expanduser("~/.garden")) / "mlflow"
+        path = str(staging_dir)
+        for item in os.listdir(path):
+            item_path = os.path.join(path, item)
+            if os.path.isfile(item_path):
+                os.remove(item_path)
+            elif os.path.isdir(item_path):
+                shutil.rmtree(item_path)
+
     def _lazy_load_model(self):
         """download and deserialize the underlying model, if necessary."""
         if self.model is None:
-            # don't clutter current directory, especially if running locally
-            local_store = pathlib.Path("~/.garden/mlflow").expanduser()
-            local_store.mkdir(parents=True, exist_ok=True)
-            self.model = load_model(
-                self.model_uri, suppress_warnings=True, dst_path=local_store
-            )
+            download_url = self.get_download_url(self.full_name)
+            local_model_path = self.download_and_stage(download_url, self.full_name)
+            self.model = load_model(local_model_path, suppress_warnings=True)
+            try:
+                self.clear_mlflow_staging_directory()
+            except Exception as e:
+                print(
+                    f"Could not clean up model staging directory. Check permissions on {self.staging_dir}"
+                )
+                print(str(e))
+                pass
         return
 
     def predict(self, data):
         """Generate model predictions.
 
         The underlying model will be downloaded if it hasn't already.
```

### Comparing `garden_ai-0.4.2/garden_ai/pipelines.py` & `garden_ai-0.4.3/garden_ai/pipelines.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from __future__ import annotations
 
+import os
 import json
 import logging
 import pathlib
 import sys
 from datetime import datetime
 from functools import reduce
 from inspect import signature
 from keyword import iskeyword
 from typing import Any, Dict, List, Optional, Tuple, Union
-from uuid import UUID, uuid4
+from uuid import UUID
 
 import dparse  # type: ignore
 import globus_compute_sdk  # type: ignore
 from packaging.requirements import InvalidRequirement, Requirement
-from pydantic import BaseModel, Field, PrivateAttr, validator
+from pydantic import BaseModel, Field, PrivateAttr, root_validator, validator
 from pydantic.dataclasses import dataclass
 
+import garden_ai
 from garden_ai._version import __version__
 from garden_ai.app.console import console
+from garden_ai.constants import GardenConstants
 from garden_ai.datacite import (
     Contributor,
     Creator,
     DataciteSchema,
     Description,
+    Identifier,
+    Subject,
     Title,
     Types,
 )
-from garden_ai.mlmodel import RegisteredModel
+from garden_ai.mlmodel import ModelMetadata
 from garden_ai.steps import DataclassConfig, Step
 from garden_ai.utils.misc import (
     JSON,
     garden_json_encoder,
     read_conda_deps,
     safe_compose,
 )
@@ -88,51 +93,55 @@
         pip_dependencies:
             Optional, populated by contents of `requirements_file` if specified. \
             Contains the currently installed version of the garden-ai package by \
             default, so that the sdk is pinned in the container.
         conda_dependencies:
             Optional, populated by `requirements_file` if it points to a \
             conda.yml environment file.
-        model_uris:
+        model_full_names:
             Optional, collected from steps' metadata.
-        uuid:
-            Populated by default, should not be set or modified by users. Used \
-            to keep local storage coherent with the module defining a pipeline.
     """
 
     title: str = Field(...)
     authors: List[str] = Field(...)
     steps: Tuple[Step, ...] = Field(...)
     contributors: List[str] = Field(default_factory=list, unique_items=True)
-    doi: Optional[str] = None
-    uuid: UUID = Field(default_factory=uuid4)
+    doi: str = Field(...)
     func_uuid: Optional[UUID] = Field(None)
     description: Optional[str] = Field(None)
     version: Optional[str] = "0.0.1"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     tags: List[str] = Field(default_factory=list, unique_items=True)
     requirements_file: Optional[str] = Field(None)
     python_version: Optional[str] = Field(None)
     pip_dependencies: List[str] = Field(default=[f"garden-ai=={__version__}"])
     conda_dependencies: List[str] = Field(default_factory=list)
-    model_uris: List[str] = Field(default_factory=list)
+    model_full_names: List[str] = Field(default_factory=list)
     short_name: Optional[str] = Field(None)
 
     def _composed_steps(*args, **kwargs):
         """ "This method intentionally left blank"
 
         We define this as a stub here, instead setting it as an attribute in
         `__post_init_post_parse__`, which is the earliest point after we
         validate that the steps are composable that we could modify the Pipeline
         object.
         This indirection is only necessary because `__call__` itself is looked
         up at the class level, so can't be set dynamically for different instances.
         """
         raise NotImplementedError
 
+    @root_validator(pre=True)
+    def doi_omitted(cls, values):
+        assert "doi" in values, (
+            "It seems like no DOI has been minted yet for this `Pipeline`. If you were trying to create a new `Pipeline`, "
+            "use `GardenClient.create_pipeline` to initialize a publishable `Pipeline` with a draft DOI."
+        )
+        return values
+
     @validator("short_name")
     def is_valid_identifier(cls, name: Optional[str]) -> Optional[str]:
         if name:
             assert name.isidentifier(), "short_name must be a valid python identifier"
             assert not iskeyword(name), "short_name must not be a reserved keyword"
         return name
 
@@ -186,102 +195,58 @@
             raise ValueError(f"Could not parse pip dependency '{pip_dep}'") from e
         return pip_dep
 
     def _collect_requirements(self):
         """collect requirements to pass to Globus Compute container service.
 
         Populates attributes `self.python_version, self.pip_dependencies, self.conda_dependencies` per
-        `self.requirements_file`, as well as `self.model_uris` from steps' metadata.
+        `self.requirements_file`, as well as `self.model_full_names` from steps' metadata.
         """
-
-        # mapping of python-version-witness: python-version (collected for warning msg below)
-        py_versions = {
-            "system": ".".join(map(str, sys.version_info[:3])),
-            "pipeline": self.python_version,
-        }
         # collect explicit pipeline dependencies for the container
         if self.requirements_file:
             if self.requirements_file.endswith((".yml", ".yaml")):
                 py_version, conda_deps, pip_deps = read_conda_deps(
                     self.requirements_file
                 )
                 if py_version:
-                    py_versions["pipeline"] = py_version
+                    self.python_version = py_version
                 self.conda_dependencies += conda_deps
                 self.pip_dependencies += pip_deps
 
             elif self.requirements_file.endswith(".txt"):
                 with open(self.requirements_file, "r") as f:
                     contents = f.read()
                     parsed = dparse.parse(
                         contents, path=self.requirements_file, resolve=True
                     ).serialize()
                     deps = [d["line"] for d in parsed["dependencies"]]
                     deps.extend(d["line"] for d in parsed["resolved_dependencies"])
                     self.pip_dependencies += set(deps)
 
-        # inspect steps to warn about possible dependency issues, but don't keep them for container.
-        # step requirements are typically inferred (via mlflow) from their models, which is
-        # prone to breaking (e.g. https://github.com/Garden-AI/garden/issues/135)
-        explicit_requirements = {
-            Requirement(r).name: Requirement(r) for r in self.pip_dependencies
-        }
-
         for step in self.steps:
-            for r in step.pip_dependencies:
-                requirement = Requirement(r)
-                # warn about step requirements we're ignoring in favor of the pipeline's
-                would_ignore_req = (
-                    requirement.name in explicit_requirements
-                    and requirement != explicit_requirements[requirement.name]
-                )
-                if would_ignore_req:
-                    logger.warning(
-                        f"Warning: step {step.__name__} has inferred a requirement '{requirement}', which is also required by the pipeline. "
-                        f"Only the pipeline's explicit requirement ({explicit_requirements[requirement.name]}) will be used."
-                    )
-                # warn about potentially missing requirements
-                elif requirement.name not in explicit_requirements:
-                    logger.warning(
-                        f"Warning: step {step.__name__} has inferred a requirement '{requirement}', which is not required by the pipeline. "
-                        f"If this package needs to be present in the container, please add '{requirement.name}' to the pipeline's requirements.txt "
-                    )
-
-            # same for conda deps -- note that these were likely explicitly added,
-            # since mlflow-inferred requirements usually aren't conda.
-            for r in step.conda_dependencies:
-                if r not in self.conda_dependencies:
-                    logger.warning(
-                        f"Warning: step {step.__name__} has inferred a conda requirement '{r}', which is not required by the pipeline. "
-                        f"If this package needs to be present in the container, please add '{r}' to the pipeline's requirements."
-                    )
-
-            self.model_uris += step.model_uris
-            py_versions[step.__name__] = step.python_version
+            self.model_full_names += step.model_full_names
 
-        self.python_version = py_versions["pipeline"] or py_versions["system"]
+        system_py_version = ".".join(map(str, sys.version_info[:3]))
+        self.python_version = self.python_version or system_py_version
         self.conda_dependencies = list(set(self.conda_dependencies))
         self.pip_dependencies = list(set(self.pip_dependencies))
 
-        distinct_py_versions = set(
-            py_versions[k] for k in py_versions if py_versions[k]
-        )
-        if len(distinct_py_versions) > 1:
-            logger.warning(
-                "Found multiple python versions specified across this"
-                f"pipeline's dependencies: {py_versions}. {self.python_version} "
-                "will be used by default. This version can be set explicitly via "
-                "the `python_version` keyword argument in the `Pipeline` "
-                "constructor."
-            )
+        if self.python_version:
+            if self.python_version != system_py_version:
+                logger.warning(
+                    f"Pipeline specified to run with Python version {self.python_version} "
+                    f"but Garden is running under {system_py_version}. Using the Python version "
+                    f"{self.python_version} specified in the Pipeline."
+                )
         return
 
     def __call__(
         self,
         *args: Any,
+        garden_client: garden_ai.GardenClient = None,
         **kwargs: Any,
     ) -> Any:
         """Call the pipeline's composed steps on the given input data.
 
         To run a Pipeline on a remote endpoint, see ``RegisteredPipeline``.
 
         Args:
@@ -292,14 +257,21 @@
         Returns:
             Results from the pipeline's composed steps called with the given input data.
 
         Raises:
             Exception:
                 Any exception raised over the course of executing the pipeline's composed steps.
         """
+        has_models = len(self.model_full_names) > 0
+        if has_models:
+            if not garden_client:
+                raise ValueError("Missing required kwarg 'garden_client'")
+            pipeline_url_json = garden_client.generate_presigned_urls_for_pipeline(self)
+            os.environ[GardenConstants.URL_ENV_VAR_NAME] = pipeline_url_json
+
         return self._composed_steps(*args, **kwargs)
 
     def __post_init_post_parse__(self):
         # Finish initializing the pipeline after validators have run.
         # - Build a single composite function from this pipeline's steps
         # - Update metadata like signature, authors w/r/t underlying steps
         # - Infer conda and pip dependencies from steps and requirements file
@@ -321,25 +293,29 @@
     def json(self) -> JSON:
         """Helper: serialize pipeline metadata to JSON string."""
         self._sync_author_metadata()
         return json.dumps(self, default=garden_json_encoder)
 
     def datacite_json(self) -> JSON:
         """Parse this `Pipeline`'s metadata into a DataCite-schema-compliant JSON string."""
+
         # Leverages a pydantic class `DataCiteSchema`, which was automatically generated from:
         # https://github.com/datacite/schema/blob/master/source/json/kernel-4.3/datacite_4.3_schema.json
+        #
         # The JSON returned by this method would be the "attributes" part of a DataCite request body.
 
         self._sync_author_metadata()
         return DataciteSchema(
+            identifiers=[Identifier(identifier=self.doi, identifierType="DOI")],
             types=Types(resourceType="AI/ML Pipeline", resourceTypeGeneral="Software"),  # type: ignore
             creators=[Creator(name=name) for name in self.authors],
             titles=[Title(title=self.title)],
             publisher="thegardens.ai",
             publicationYear=self.year,
+            subjects=[Subject(subject=tag) for tag in self.tags],
             contributors=[
                 Contributor(name=name, contributorType="Other")  # type: ignore
                 for name in self.contributors
             ],
             version=self.version,
             descriptions=[
                 Description(description=self.description, descriptionType="Other")  # type: ignore
@@ -379,20 +355,17 @@
         version:
         tags:
         python_version:
         doi:
         func_uuid:
         pip_dependencies:
         conda_dependencies:
-        model_uris:
-        uuid:
-            Required, should not be set or modified.
+        model_full_names:
     """
 
-    uuid: UUID = Field(...)
     doi: str = Field(...)
     func_uuid: Optional[UUID] = Field(...)
     title: str = Field(...)
     short_name: str = Field(...)
     authors: List[str] = Field(...)
     # NOTE: steps are dicts here, not Step objects
     steps: List[Dict[str, Union[str, None, List]]] = Field(...)
@@ -401,23 +374,23 @@
     version: str = "0.0.1"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     tags: List[str] = Field(default_factory=list, unique_items=True)
     python_version: Optional[str] = Field(None)
     pip_dependencies: List[str] = Field(default_factory=list)
     conda_dependencies: List[str] = Field(default_factory=list)
     _env_vars: Dict[str, str] = PrivateAttr(default_factory=dict)
-    model_uris: List[str] = Field(default_factory=list)
+    model_full_names: List[str] = Field(default_factory=list)
 
     def __call__(
         self,
         *args: Any,
         endpoint: Union[UUID, str] = None,
         **kwargs: Any,
     ) -> Any:
-        """Remotely execute this ``RegisteredPipeline``'s function from its uuid. An endpoint must be specified.
+        """Remotely execute this ``RegisteredPipeline``'s function from the function uuid. An endpoint must be specified.
 
         Args:
             *args (Any):
                 Input data passed through the first step in the pipeline
             endpoint (UUID | str | None):
                 Where to run the pipeline. Must be a valid Globus Compute endpoint UUID.
             **kwargs (Any):
@@ -467,26 +440,26 @@
         # note: we want every RegisteredPipeline to be re-constructible
         # from mere json, so as a sanity check we use pipeline.json() instead of
         # pipeline.dict() directly
         record = pipeline.json()
         data = json.loads(record)
         return cls(**data)
 
-    def collect_models(self) -> List[RegisteredModel]:
-        """Collect the RegisteredModel objects that are present in the local DB corresponding to this Pipeline's list of `model_uris`."""
-        from .local_data import get_local_model_by_uri
+    def collect_models(self) -> List[ModelMetadata]:
+        """Collect the RegisteredModel objects that are present in the local DB corresponding to this Pipeline's list of `model_full_names`."""
+        from .local_data import get_local_model_by_name
 
         models = []
-        for uri in self.model_uris:
-            model = get_local_model_by_uri(uri)
+        for model_name in self.model_full_names:
+            model = get_local_model_by_name(model_name)
             if model:
                 models += [model]
             else:
                 logger.warning(
-                    f"No record in local database for model {uri}. "
+                    f"No record in local database for model {model_name}. "
                     "Published garden will not have detailed metadata for that model."
                 )
         return models
 
     def expanded_metadata(self) -> Dict[str, Any]:
         """Helper: build the "complete" metadata dict with nested ``Model`` metadata.
```

### Comparing `garden_ai-0.4.2/garden_ai/steps.py` & `garden_ai-0.4.3/garden_ai/steps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import inspect
 import json
 import logging
 import typing
-from functools import update_wrapper, wraps
+from functools import update_wrapper
 from inspect import Parameter, Signature, signature
 from typing import Any, Callable, Dict, List, Optional
 
 from pydantic import Field, validator
 from pydantic.dataclasses import dataclass
 from typing_extensions import get_type_hints
 
-from garden_ai.mlmodel import Model, _Model
+from garden_ai.mlmodel import _Model
 from garden_ai.utils.misc import JSON, garden_json_encoder
 
 logger = logging.getLogger()
 
 
 class DataclassConfig:
     # pydantic dataclasses read their config via decorator argument, not as
@@ -54,15 +54,15 @@
             dimensions of a matrix or column names of a dataframe).
         output_info (str):
             Human-readable description of the output data and/or relevant
             characteristics that *will* hold true for this step's output (e.g.
             dimensions of a matrix or column names of a dataframe).
         authors (List[str]):
             The main researchers involved in producing the Step, for citation and discoverability purposes.
-        model_uris (List[str]):
+        model_full_names (List[str]):
             A reference to the models used in this step, if any. Model identifiers are as stored in MLFlow (not including the 'models:/' prefix).
         source (Optional[str]):
             Should not be set by users. Consists of the plain python source code \
             used to define `func`, if possible.
 
     Raises:
         TypeError:
@@ -89,18 +89,15 @@
     func: Callable
     authors: List[str] = Field(default_factory=list)
     contributors: List[str] = Field(default_factory=list)
     title: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     input_info: Optional[str] = Field(None)
     output_info: Optional[str] = Field(None)
-    conda_dependencies: List[str] = Field(default_factory=list)
-    pip_dependencies: List[str] = Field(default_factory=list)
-    python_version: Optional[str] = Field(None)
-    model_uris: List[str] = Field(default_factory=list)
+    model_full_names: List[str] = Field(default_factory=list)
     source: Optional[str] = Field(None)
 
     def __post_init_post_parse__(self):
         # like __post_init__, but called after pydantic validation
         # copies e.g. __doc__ and __name__ from
         # the underlying callable to this object
         # (also handy for signature/annotations)
@@ -110,36 +107,32 @@
         self.__signature__ = signature(self.func)
         input_hints: Dict = get_type_hints(self.func, include_extras=True)
         return_hint = input_hints.pop("return")
         if self.input_info is None:
             self.input_info = str(input_hints)
         if self.output_info is None:
             self.output_info = f"return: {return_hint}"
-        self._infer_model_deps()
+        self._track_models()
         return
 
     def __call__(self, *args, **kwargs):
         # keep it simple: just pass input the underlying callable.
         return self.func(*args, **kwargs)
 
-    def _infer_model_deps(self):
+    def _track_models(self):
         """
         If this step's function has a Model as a default argument, like
-        ``func(*args, model=Model(...))``, extract the dependencies for that model
-        and track them as step-level dependencies.
+        ``func(*args, model=Model(...))``, record the model name
         """
 
         sig = signature(self.func)
         for param in sig.parameters.values():
             if isinstance(param.default, _Model):
                 model = param.default
-                self.python_version = model.python_version
-                self.conda_dependencies += model.conda_dependencies
-                self.pip_dependencies += model.pip_dependencies
-                self.model_uris += [model.model_full_name]
+                self.model_full_names += [model.full_name]
         return
 
     @validator("func")
     def has_annotations(cls, f: Callable):
         sig = signature(f)
         # check that any positional arguments have annotations
         for p in sig.parameters.values():
@@ -229,37 +222,7 @@
     else:
         # called like ``@step(**kwargs)``
         def wrapper(f):
             data = {**kwargs, "func": f}
             return Step(**data)
 
         return wrapper
-
-
-def inference_step(model_uri: str, **kwargs):
-    """Helper: provide ``@inference_step(...)`` decorator for creation of ``Step``s.
-
-    Example:
-    --------
-        ```python
-        @inference_step(model_uri="me@uni.edu-my-model/version")
-        def my_step(data: pd.DataFrame) -> MyResultType:
-            pass  # NOTE: leave the function body empty
-
-        ## equivalent to:
-        @step
-        def my_step(
-            data: MyDataType,
-            model=garden_ai.Model("me@uni.edu-my-model/version"),
-        ) -> MyResultType:
-            return model.predict(data)
-        ```
-    """
-
-    def wrapper(f: Callable):
-        @wraps(f)  # make sure we aren't losing signature info
-        def boilerplate(*args, model=Model(model_uri), **_kwargs):
-            return model.predict(*args)
-
-        return step(boilerplate)
-
-    return wrapper
```

### Comparing `garden_ai-0.4.2/garden_ai/templates/pipeline` & `garden_ai-0.4.3/garden_ai/templates/pipeline`

 * *Files 2% similar despite different names*

```diff
@@ -61,9 +61,9 @@
     requirements_file=REQUIREMENTS_FILE,
     authors={{ pipeline.authors }},
     contributors={{ pipeline.contributors }},
     description="{{ pipeline.description }}",
     version="{{ pipeline.version }}",
     year={{ pipeline.year }},
     tags={{ pipeline.tags }},
-    uuid="{{ pipeline.uuid }}",  # WARNING: DO NOT EDIT UUID
+    doi="{{ pipeline.doi }}",  # WARNING: DO NOT EDIT DOI
 )
```

### Comparing `garden_ai-0.4.2/garden_ai/utils/filesystem.py` & `garden_ai-0.4.3/garden_ai/utils/filesystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 from pathlib import Path
 import importlib.util
 from garden_ai import Pipeline
 from garden_ai import GardenConstants
 
 from garden_ai.mlmodel import PipelineLoadScaffoldedException
-from mlflow import MlflowException  # type: ignore
 
 
 class PipelineLoadException(Exception):
     """Exception raised when a container build request fails"""
 
     pass
 
 
-class PipelineLoadMlFlowException(Exception):
-    """Exception raised when a MlFlow model load fails"""
-
-    pass
-
-
 def load_pipeline_from_python_file(python_file: Path) -> Pipeline:
     """
     Dynamically import a pipeline object from a user's pipeline file.
 
     Parameters
     ----------
     python_file: Local path of user's pipeline code.
@@ -46,17 +39,16 @@
             "Failed to load model. It looks like you are using the placeholder model name from a scaffolded pipeline. "
             f"Please replace {GardenConstants.SCAFFOLDED_MODEL_NAME} in your pipeline.py"
             " with the name of a registered Garden model."
             "\nFor more information on how to use Garden, please read our docs: "
             "https://garden-ai.readthedocs.io/en/latest/"
         )
         raise PipelineLoadScaffoldedException(error_message) from e
-    except MlflowException as e:
-        raise PipelineLoadMlFlowException("\nMlflowException: " + str(e)) from e
     except Exception as e:
+        print(e)
         raise PipelineLoadException("Could not execute the Python code") from e
 
     for obj_name in dir(module):
         obj = getattr(module, obj_name)
         if isinstance(obj, Pipeline):
             if obj.short_name is None:
                 obj.short_name = obj_name
```

### Comparing `garden_ai-0.4.2/garden_ai/utils/misc.py` & `garden_ai-0.4.3/garden_ai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.2/pyproject.toml` & `garden_ai-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "0.4.2" # placeholder
+version = "0.4.3" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
@@ -38,15 +38,15 @@
 # numba is an indirect dep of ML Flow.
 # Specifying a recent version of it helps avoid install issues on M1 Macs
 numba = "^0.56"
 boto3 = "^1.26.77"
 dparse = { extras = ["conda"], version = "^0.6.2" }
 pyyaml = "^6.0"
 packaging = "^23.0"
-globus-compute-sdk = "^2.0.0"
+globus-compute-sdk = "2.1.0"
 # Be sure to add additional flavors as optional below as support is added and update tool.poetry.extras
 torch = { version = "^2.0.0", optional = true }
 tensorflow = { version = "^2.11.0", optional = true, python = ">=3.8,<3.12" }
 
 [tool.poetry.scripts]
 garden-ai = "garden_ai.app.main:app"
 
@@ -73,19 +73,19 @@
 mkdocs-extensions = "^0.1.2"
 pymdown-extensions = "^10.0.1"
 mkdocs-material = "^9.1.13"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 
 [tool.poetry.extras]
 # Be sure to add additional flavors to below as support is added and in the flavors array
-# Optional dependencies that can be added through `poetry install --extras "torch tensorflow"` etc. or `poetry install --extras "flavors"`
+# Optional dependencies that can be added through `poetry install --extras "torch tensorflow"` etc. or `poetry install --extras "all"`
 # `poetry install --all-extras` will install all extras located in tool.poetry.extras
 torch = ["torch"]
 tensorflow = ["tensorflow"]
-flavors = ["tensorflow", "torch"]
+all = ["tensorflow", "torch"]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 exclude = "/fixtures/"
```

### Comparing `garden_ai-0.4.2/PKG-INFO` & `garden_ai-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.4.2
+Version: 0.4.3
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: flavors
+Provides-Extra: all
 Provides-Extra: tensorflow
 Provides-Extra: torch
 Requires-Dist: beartype (>=0.12.0,<0.13.0)
 Requires-Dist: boto3 (>=1.26.77,<2.0.0)
 Requires-Dist: dparse[conda] (>=0.6.2,<0.7.0)
-Requires-Dist: globus-compute-sdk (>=2.0.0,<3.0.0)
+Requires-Dist: globus-compute-sdk (==2.1.0)
 Requires-Dist: globus-sdk (>=3.12.0,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mlflow (>=2.3.2,<3.0.0)
 Requires-Dist: numba (>=0.56,<0.57)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
-Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "flavors")
-Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "flavors"
+Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "all")
+Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "all"
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://garden-ai.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Garden-AI/garden
 Description-Content-Type: text/markdown
 
 # Garden
```

