# Comparing `tmp/jupyterlite_sphinx-0.8.0.tar.gz` & `tmp/jupyterlite_sphinx-0.9.0.tar.gz`

## Comparing `jupyterlite_sphinx-0.8.0.tar` & `jupyterlite_sphinx-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/jupyterlite_sphinx/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/jupyterlite_sphinx/jupyterlite_sphinx.css
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/jupyterlite_sphinx/jupyterlite_sphinx.js
--rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/jupyterlite_sphinx/jupyterlite_sphinx.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/LICENSE
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.css
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.js
+-rw-r--r--   0        0        0    13888 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/LICENSE
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/README.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 jupyterlite_sphinx-0.9.0/PKG-INFO
```

### Comparing `jupyterlite_sphinx-0.8.0/jupyterlite_sphinx/jupyterlite_sphinx.css` & `jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.css`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.8.0/jupyterlite_sphinx/jupyterlite_sphinx.js` & `jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.js`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.8.0/jupyterlite_sphinx/jupyterlite_sphinx.py` & `jupyterlite_sphinx-0.9.0/jupyterlite_sphinx/jupyterlite_sphinx.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,73 +19,52 @@
 from sphinx.util.fileutil import copy_asset
 from sphinx.parsers import RSTParser
 
 HERE = Path(__file__).parent
 
 CONTENT_DIR = "_contents"
 JUPYTERLITE_DIR = "lite"
+# Using a global variable, is there a better way?
+APPS = []
 
 
 # Used for nodes that do not need to be rendered
 def skip(self, node):
     raise SkipNode
 
 
 # Used to render an element node as HTML
 def visit_element_html(self, node):
     self.body.append(node.html())
     raise SkipNode
 
 
-class _LiteIframe(Element):
+class _PromptedIframe(Element):
     def __init__(
         self,
         rawsource="",
         *children,
-        prefix=JUPYTERLITE_DIR,
+        iframe_src="",
         width="100%",
         height="100%",
         prompt=False,
         prompt_color=None,
-        content=[],
-        notebook=None,
-        lite_options={},
         **attributes,
     ):
         super().__init__(
             "",
-            prefix=prefix,
+            iframe_src=iframe_src,
             width=width,
             height=height,
             prompt=prompt,
             prompt_color=prompt_color,
-            content=content,
-            notebook=notebook,
-            lite_options=lite_options,
         )
 
     def html(self):
-        lite_options = self["lite_options"]
-
-        if self["content"]:
-            code_lines = ["" if not line.strip() else line for line in self["content"]]
-            code = "\n".join(code_lines)
-
-            lite_options["code"] = code
-
-        app_path = self.lite_app
-        if self["notebook"] is not None:
-            lite_options["path"] = self["notebook"]
-            app_path = f"{self.lite_app}{self.notebooks_path}"
-
-        options = "&".join(
-            [f"{key}={quote(value)}" for key, value in lite_options.items()]
-        )
-
-        iframe_src = f'{self["prefix"]}/{app_path}{f"?{options}" if options else ""}'
+        iframe_src = self["iframe_src"]
 
         if self["prompt"]:
             prompt = (
                 self["prompt"] if isinstance(self["prompt"], str) else "Try It Live!"
             )
             prompt_color = (
                 self["prompt_color"] if self["prompt_color"] is not None else "#f7dc1e"
@@ -104,14 +83,45 @@
 
         return (
             f'<iframe src="{iframe_src}"'
             f'width="{self["width"]}" height="{self["height"]}" class="jupyterlite_sphinx_raw_iframe"></iframe>'
         )
 
 
+class _LiteIframe(_PromptedIframe):
+    def __init__(
+        self,
+        rawsource="",
+        *children,
+        prefix=JUPYTERLITE_DIR,
+        content=[],
+        notebook=None,
+        lite_options={},
+        **attributes,
+    ):
+        if content:
+            code_lines = ["" if not line.strip() else line for line in content]
+            code = "\n".join(code_lines)
+
+            lite_options["code"] = code
+
+        app_path = self.lite_app
+        if notebook is not None:
+            lite_options["path"] = notebook
+            app_path = f"{self.lite_app}{self.notebooks_path}"
+
+        options = "&".join(
+            [f"{key}={quote(value)}" for key, value in lite_options.items()]
+        )
+
+        iframe_src = f'{prefix}/{app_path}{f"?{options}" if options else ""}'
+
+        super().__init__(rawsource, *children, iframe_src=iframe_src, **attributes)
+
+
 class RepliteIframe(_LiteIframe):
     """Appended to the doctree by the RepliteDirective directive
 
     Renders an iframe that shows a repl with JupyterLite.
     """
 
     lite_app = "repl/index.html"
@@ -134,14 +144,43 @@
     Renders an iframe that shows a Notebook with RetroLite.
     """
 
     lite_app = "retro/"
     notebooks_path = "notebooks/"
 
 
+class VoiciIframe(_PromptedIframe):
+    """Appended to the doctree by the VoiciDirective directive
+
+    Renders an iframe that shows a Notebook with Voici.
+    """
+
+    def __init__(
+        self,
+        rawsource="",
+        *children,
+        prefix=JUPYTERLITE_DIR,
+        notebook=None,
+        lite_options={},
+        **attributes,
+    ):
+        if notebook is not None:
+            app_path = f"voici/render/{notebook.replace('.ipynb', '.html')}"
+        else:
+            app_path = "voici/tree"
+
+        options = "&".join(
+            [f"{key}={quote(value)}" for key, value in lite_options.items()]
+        )
+
+        iframe_src = f'{prefix}/{app_path}{f"?{options}" if options else ""}'
+
+        super().__init__(rawsource, *children, iframe_src=iframe_src, **attributes)
+
+
 class RepliteDirective(SphinxDirective):
     """The ``.. replite::`` directive.
 
     Adds a replite console to the docs.
     """
 
     has_content = True
@@ -153,14 +192,17 @@
         "toolbar": directives.unchanged,
         "theme": directives.unchanged,
         "prompt": directives.unchanged,
         "prompt_color": directives.unchanged,
     }
 
     def run(self):
+        if not "repl" in APPS:
+            APPS.append("repl")
+
         width = self.options.pop("width", "100%")
         height = self.options.pop("height", "100%")
 
         prompt = self.options.pop("prompt", False)
         prompt_color = self.options.pop("prompt_color", None)
 
         prefix = os.path.relpath(
@@ -243,23 +285,57 @@
     """The ``.. jupyterlite::`` directive.
 
     Renders a Notebook with JupyterLite in the docs.
     """
 
     iframe_cls = JupyterLiteIframe
 
+    def run(self):
+        if not "lab" in APPS:
+            APPS.append("lab")
+
+        return super().run()
+
 
 class RetroLiteDirective(_LiteDirective):
     """The ``.. retrolite::`` directive.
 
     Renders a Notebook with RetroLite in the docs.
     """
 
     iframe_cls = RetroLiteIframe
 
+    def run(self):
+        if not "retro" in APPS:
+            APPS.append("retro")
+
+        return super().run()
+
+
+class VoiciDirective(_LiteDirective):
+    """The ``.. voici::`` directive.
+
+    Renders a Notebook with Voici in the docs.
+    """
+
+    iframe_cls = VoiciIframe
+
+    def run(self):
+        try:
+            import voici
+        except ImportError:
+            raise RuntimeError(
+                "Voici must be installed if you want to make use of the voici directive: pip install voici"
+            )
+
+        if not "voici" in APPS:
+            APPS.append("voici")
+
+        return super().run()
+
 
 class RetroLiteParser(RSTParser):
     """Sphinx source parser for Jupyter notebooks.
 
     Shows the Notebook using retrolite."""
 
     supported = ("jupyterlite_notebook",)
@@ -313,36 +389,35 @@
             for match in glob.glob(pattern, recursive=True)
         ]
 
         contents = []
         for content in jupyterlite_contents:
             contents.extend(["--contents", content])
 
+        apps = []
+        for jlite_app in APPS:
+            apps.extend(["--apps", jlite_app])
+
         command = [
             "jupyter",
             "lite",
             "build",
             "--debug",
             *config,
+            *apps,
             *contents,
             "--contents",
             os.path.join(app.srcdir, CONTENT_DIR),
             "--output-dir",
             os.path.join(app.outdir, JUPYTERLITE_DIR),
+            "--lite-dir",
+            jupyterlite_dir,
         ]
 
-        if jupyterlite_dir:
-            command.extend(["--lite-dir", jupyterlite_dir])
-
-            subprocess.run(command, check=True)
-        else:
-            with tempfile.TemporaryDirectory() as tmp_dir:
-                command.extend(["--lite-dir", tmp_dir])
-
-                subprocess.run(command, check=True)
+        subprocess.run(command, cwd=app.srcdir, check=True)
 
         print("[jupyterlite-sphinx] JupyterLite build done")
 
     # Cleanup
     try:
         shutil.rmtree(os.path.join(app.srcdir, CONTENT_DIR))
         os.remove(".jupyterlite.doit.db")
@@ -356,15 +431,15 @@
 
     app.connect("config-inited", inited)
     # We need to build JupyterLite at the end, when all the content was created
     app.connect("build-finished", jupyterlite_build)
 
     # Config options
     app.add_config_value("jupyterlite_config", None, rebuild="html")
-    app.add_config_value("jupyterlite_dir", None, rebuild="html")
+    app.add_config_value("jupyterlite_dir", app.srcdir, rebuild="html")
     app.add_config_value("jupyterlite_contents", None, rebuild="html")
     app.add_config_value("jupyterlite_bind_ipynb_suffix", True, rebuild="html")
 
     # Initialize RetroLite and JupyterLite directives
     app.add_node(
         RetroLiteIframe,
         html=(visit_element_html, None),
@@ -391,14 +466,25 @@
         latex=(skip, None),
         textinfo=(skip, None),
         text=(skip, None),
         man=(skip, None),
     )
     app.add_directive("replite", RepliteDirective)
 
+    # Initialize Voici directive
+    app.add_node(
+        VoiciIframe,
+        html=(visit_element_html, None),
+        latex=(skip, None),
+        textinfo=(skip, None),
+        text=(skip, None),
+        man=(skip, None),
+    )
+    app.add_directive("voici", VoiciDirective)
+
     # CSS and JS assets
     copy_asset(str(HERE / "jupyterlite_sphinx.css"), str(Path(app.outdir) / "_static"))
     copy_asset(str(HERE / "jupyterlite_sphinx.js"), str(Path(app.outdir) / "_static"))
 
     app.add_css_file("https://fonts.googleapis.com/css?family=Vibur")
     app.add_css_file("jupyterlite_sphinx.css")
```

### Comparing `jupyterlite_sphinx-0.8.0/LICENSE` & `jupyterlite_sphinx-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_sphinx-0.8.0/PKG-INFO` & `jupyterlite_sphinx-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlite-sphinx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Sphinx extension for deploying JupyterLite
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2022, JupyterLite Contributors
         All rights reserved.
         
@@ -29,20 +29,26 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: docutils
 Requires-Dist: jupyter-server
 Requires-Dist: jupyterlab-server
-Requires-Dist: jupyterlite-core>=0.1.0b19
+Requires-Dist: jupyterlite-core>=0.1.0
 Requires-Dist: sphinx>=4
+Provides-Extra: dev
+Requires-Dist: hatch; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: jupyterlite-xeus-python<0.10.0,>=0.9.0; extra == 'docs'
+Requires-Dist: myst-parser; extra == 'docs'
+Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # JupyterLite Sphinx
 
 A Sphinx extension that provides utilities for embedding [JupyterLite](https://jupyterlite.readthedocs.io) in your documentation.
 
 ## Docs
```

