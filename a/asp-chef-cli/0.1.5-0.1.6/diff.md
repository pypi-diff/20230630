# Comparing `tmp/asp_chef_cli-0.1.5.tar.gz` & `tmp/asp_chef_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_chef_cli-0.1.5.tar", max compression
+gzip compressed data, was "asp_chef_cli-0.1.6.tar", max compression
```

## Comparing `asp_chef_cli-0.1.5.tar` & `asp_chef_cli-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_cli-0.1.5/LICENSE
--rw-r--r--   0        0        0     2991 2023-06-10 05:18:18.990369 asp_chef_cli-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_cli-0.1.5/asp_chef_cli/__init__.py
--rw-r--r--   0        0        0      102 2023-06-09 20:54:07.739786 asp_chef_cli-0.1.5/asp_chef_cli/__main__.py
--rwxr-xr-x   0        0        0     4379 2023-06-29 15:49:15.999199 asp_chef_cli-0.1.5/asp_chef_cli/cli.py
--rw-r--r--   0        0        0      399 2023-06-29 15:35:04.704265 asp_chef_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.5/setup.py
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_cli-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2991 2023-06-10 05:18:18.990369 asp_chef_cli-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_cli-0.1.6/asp_chef_cli/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-09 20:54:07.739786 asp_chef_cli-0.1.6/asp_chef_cli/__main__.py
+-rwxr-xr-x   0        0        0     4358 2023-06-30 07:13:55.352688 asp_chef_cli-0.1.6/asp_chef_cli/cli.py
+-rw-r--r--   0        0        0      399 2023-06-30 07:14:57.009864 asp_chef_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.6/setup.py
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 asp_chef_cli-0.1.6/PKG-INFO
```

### Comparing `asp_chef_cli-0.1.5/LICENSE` & `asp_chef_cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_chef_cli-0.1.5/README.md` & `asp_chef_cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `asp_chef_cli-0.1.5/asp_chef_cli/cli.py` & `asp_chef_cli-0.1.6/asp_chef_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             console.print(f"[red bold]Error:[/red bold] {e}")
 
 
 def version_callback(value: bool):
     if value:
         import importlib.metadata
         __version__ = importlib.metadata.version("asp-chef-cli")
-        console.print("asp-chef-headless", __version__)
+        console.print("asp-chef-cli", __version__)
         raise typer.Exit()
 
 
 def fetch(url: str):
     with sync_playwright() as playwright:
         browser = app_options.browser.get(playwright).launch(headless=app_options.headless and not app_options.debug)
         context = browser.new_context()
@@ -79,15 +79,15 @@
         if not app_options.debug:
             browser.close()
     return result
 
 
 @app.callback()
 def main(
-        recipe_url: str = typer.Option(..., "--url", "-u", help="A sharable ASP Chef URL (headless mode)"),
+        recipe_url: str = typer.Option(..., "--url", "-u", help="A sharable ASP Chef URL"),
         headless: bool = typer.Option(False, help="Run ASP Chef in headless mode"),
         browser: Browser = typer.Option(Browser.FIREFOX, "--browser", help="Use a specific browser"),
         debug: bool = typer.Option(False, "--debug", help="Don't minimize browser"),
         version: bool = typer.Option(False, "--version", callback=version_callback, is_eager=True,
                                      help="Print version and exit"),
 ):
     """
```

### Comparing `asp_chef_cli-0.1.5/setup.py` & `asp_chef_cli-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['dumbo-utils>=0.1.9,<0.2.0',
  'pytest-playwright>=0.3.3,<0.4.0',
- 'rich>=13.4.1,<14.0.0',
+ 'rich>=13.4.2,<14.0.0',
  'typer>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'asp-chef-cli',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'A simple CLI to run ASP Chef recipes',
     'long_description': '# ASP Chef CLI\n\nA simple CLI to run ASP Chef, in headed or headless mode.\n\n\n## Install\n\nThe suggested way is via pip:\n```bash\n$ pip install asp-chef-cli\n$ playwright install\n```\n\nDocker is another option (headed mode needs extra parameters):\n```bash\n$ docker run malvi/asp-chef-cli\n$ docker run docker run --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" malvi/asp-chef-cli\n```\n\n\n\n\n## Usage\n\nRun with one of the following commands:\n```bash\n$ python -m asp_chef_cli --help\n$ docker run malvi/asp-chef-cli --help\n```\n\nAdd the recipe (an ASP Chef sharable URL) with the option `--url` (quote the URL as it contains characters like # that breaks bash and other terminals).\nThe headless mode can be activated with the flag `--headless` (always active in the docker image).\nPossibly change the default browser used by playwright with the option `--browser`.\nFinally, give a command to execute:\n* `run` simply runs the recipe as it is;\n* `run-with` runs the recipe with the input replaced by the one specified either with the option `--input` or via the prompt.\n\nThe flag `--help` can be specified after a command to get a list of arguments for that command.\n\n\n## Examples\n\nLet us consider [this simple recipe](https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21) with no input and guessing the atom `world`.\nThe recipe can be run headless by giving the following command:\n```bash\n$ python -m asp_chef_cli --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run\nEMPTY MODEL\n§\nworld.\n```\n\nIt is possible to specify a different input as follows:\n```bash\n$ python -m asp_chef_headless --headless --browser=chromium --url="https://asp-chef.alviano.net/#eJxtkNuOgjAQhl+plNUsl4srUKIQEXu6s+Ch2CIJIpan33bdRC/2ajKnf/75DibtRBt69QLNiUGSbkfJyawRsFAUqqFKMEBNpxl5TNz1YvzXC7w6ee5xHfUV3PWoTRWDauRbq+X3ck82MpfpJf/ePXhZGS6Bn+mltyo3MGvYLS8Z5AsAGVzOuN5AppGtr+Vqkd6rGBtGi07AD6dRchIZBk+nkgQXbr0gOUrhh2BPgqEyaH4w6VTHwfjuldFwFMlF5m1hauL8ZVfhV69cn9We1Ff3w7r5Gu1dW38op4famy/8tOcJGH5vtfjGNDaouRo3x4iaOF2/aT1ZURhNFGZ30Wag0pFlW0z/8vNDw0nRMRgBxwup4Mh0NPGSAep9OgaW5flOIR4YdD8XRxuHOsbDizkOjtgLfgC4qpvc%21" run-with --input "hello."\nhello.\n§\nhello.\nworld.\n```',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `asp_chef_cli-0.1.5/PKG-INFO` & `asp_chef_cli-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: asp-chef-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple CLI to run ASP Chef recipes
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dumbo-utils (>=0.1.9,<0.2.0)
 Requires-Dist: pytest-playwright (>=0.3.3,<0.4.0)
-Requires-Dist: rich (>=13.4.1,<14.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # ASP Chef CLI
 
 A simple CLI to run ASP Chef, in headed or headless mode.
```

