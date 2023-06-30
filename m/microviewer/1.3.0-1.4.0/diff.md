# Comparing `tmp/microviewer-1.3.0.tar.gz` & `tmp/microviewer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.3.0.tar", last modified: Thu Jun 29 00:50:13 2023, max compression
+gzip compressed data, was "microviewer-1.4.0.tar", last modified: Fri Jun 30 19:53:17 2023, max compression
```

## Comparing `microviewer-1.3.0.tar` & `microviewer-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-29 00:50:13.719662 microviewer-1.3.0/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-29 00:50:13.000000 microviewer-1.3.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     1859 2023-06-29 00:50:13.000000 microviewer-1.3.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.3.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       29 2023-06-28 20:11:03.000000 microviewer-1.3.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-06-29 00:50:13.719867 microviewer-1.3.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1649 2023-06-28 21:32:21.000000 microviewer-1.3.0/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-29 00:50:13.711169 microviewer-1.3.0/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     5837 2023-06-28 20:06:00.000000 microviewer-1.3.0/microviewer/__init__.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-29 00:50:13.718762 microviewer-1.3.0/microviewer/cursors/
--rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/exact-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/exact.png
--rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/large-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/large.png
--rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/medium-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/medium.png
--rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/small-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.3.0/microviewer/cursors/small.png
--rw-r--r--   0 wms        (501) staff       (20)    39436 2023-06-28 23:52:27.000000 microviewer-1.3.0/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.3.0/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    28960 2023-06-29 00:43:30.000000 microviewer-1.3.0/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.3.0/microviewer/jquery-3.7.0.min.js
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-29 00:50:13.713546 microviewer-1.3.0/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-06-29 00:50:13.000000 microviewer-1.3.0/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      820 2023-06-29 00:50:13.000000 microviewer-1.3.0/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-29 00:50:13.000000 microviewer-1.3.0/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-29 00:50:13.000000 microviewer-1.3.0/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.3.0/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-29 00:50:13.000000 microviewer-1.3.0/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-06-29 00:50:13.000000 microviewer-1.3.0/microviewer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-29 00:50:13.000000 microviewer-1.3.0/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-29 00:50:13.719332 microviewer-1.3.0/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.3.0/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     4193 2023-06-28 21:41:24.000000 microviewer-1.3.0/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.3.0/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)   297931 2023-06-28 20:05:35.000000 microviewer-1.3.0/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-29 00:50:13.720522 microviewer-1.3.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.3.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:17.001271 microviewer-1.4.0/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-30 19:53:16.000000 microviewer-1.4.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     2758 2023-06-30 19:53:16.000000 microviewer-1.4.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.4.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.4.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     2663 2023-06-30 19:53:17.001457 microviewer-1.4.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1649 2023-06-28 21:32:21.000000 microviewer-1.4.0/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:16.989706 microviewer-1.4.0/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.4.0/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     9295 2023-06-30 16:44:34.000000 microviewer-1.4.0/microviewer/crackle.js
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:17.000409 microviewer-1.4.0/microviewer/cursors/
+-rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/exact-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/exact.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/large-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/large.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/medium-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/medium.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/small-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/small.png
+-rw-r--r--   0 wms        (501) staff       (20)    48063 2023-06-30 19:17:20.000000 microviewer-1.4.0/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.4.0/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    31097 2023-06-30 19:47:12.000000 microviewer-1.4.0/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.4.0/microviewer/jquery-3.7.0.min.js
+-rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-06-30 16:44:34.000000 microviewer-1.4.0/microviewer/libcrackle.wasm
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:16.996987 microviewer-1.4.0/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     2663 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      871 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.4.0/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       12 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:17.000946 microviewer-1.4.0/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.4.0/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     4473 2023-06-30 17:53:12.000000 microviewer-1.4.0/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.4.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)   297931 2023-06-28 20:05:35.000000 microviewer-1.4.0/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-30 19:53:17.002122 microviewer-1.4.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.4.0/setup.py
```

### Comparing `microviewer-1.3.0/ChangeLog` & `microviewer-1.4.0/ChangeLog`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 CHANGES
 =======
 
+1.4.0
+-----
+
+* ui: add some help text to the save options
+* ui: display memory usage
+* fix: preload cursor images
+* feat: add show unselected rendering mode to hyperview
+* fix: ensure paint is selected so it doesn't disappear
+* docs: be more specfic that saving is for segmentation
+* feat: add --paint feature to images
+* feat: enable saving segmentation for hyperview
+* fix: disable spacebar zoom over 10x
+* feat: add painting to hyperview
+* fix: add appropriate mime types
+* fix: ensure paint is treated correctly
+* install: ensure libcrackle.wasm is included
+* fix: crackle download
+* fix: numpy download working
+* fix: incorrect array size
+* fix: save numpy
+* fix: ensure header length set properly
+* wip: broken but semi-functional crackle compression+save
+* fix: NaN labels and prevent propagation of events when typing
+* feat: add direct voxel painting
+* feat: add save function to datacube
+
 1.3.0
 -----
 
 * fix: more natural interaction with single point toggle
 * feat: add drag selection and erase
 * feat: adds paint function (but no UI support yet)
 * fix: nicer error handling for CLI
```

### Comparing `microviewer-1.3.0/LICENSE` & `microviewer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/PKG-INFO` & `microviewer-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.3.0
+Version: 1.4.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.3.0/README.md` & `microviewer-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/__init__.py` & `microviewer-1.4.0/microviewer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,19 +108,21 @@
     self.cutouts = cutouts
     BaseHTTPRequestHandler.__init__(self, *args)
 
   def do_GET(self):
     self.send_response(200)
   
     allowed_files = (
-      '/', '/datacube.js', '/jquery-3.7.0.min.js', '/favicon.ico',
+      "/", 
+      "/datacube.js", "/crackle.js", "/jquery-3.7.0.min.js", "/favicon.ico",
       "/cursors/exact.png", "/cursors/small.png", "/cursors/medium.png",
       "/cursors/large.png",
       "/cursors/exact-active.png", "/cursors/small-active.png", 
       "/cursors/medium-active.png", "/cursors/large-active.png",
+      "/libcrackle.wasm"
     )
 
     if self.path in allowed_files:
       self.serve_file()
     elif self.path == '/parameters':
       self.serve_parameters()
     elif self.path == '/channel':
@@ -176,15 +178,25 @@
           np.dtype(img["img"].dtype).itemsize,
           np.dtype(seg["img"].dtype).itemsize
         ],
       })
     self.wfile.write(msg.encode('utf-8'))
 
   def serve_file(self):
-    self.send_header('Content-type', 'text/html')
+    _, ext = os.path.splitext(self.path)
+
+    content_type = "text/html"
+    if ext == ".js":
+      content_type = "application/javascript"
+    elif ext == ".png":
+      content_type = "image/png"
+    elif ext == ".wasm":
+      content_type ="application/octet-stream"
+
+    self.send_header('Content-type', content_type)
     self.end_headers()
 
     path = self.path.replace('/', '', 1)
     path_elems = path.split("/")
 
     if len(path_elems) > 2:
       raise ValueError("Invalid path.")
```

### Comparing `microviewer-1.3.0/microviewer/cursors/exact-active.png` & `microviewer-1.4.0/microviewer/cursors/exact-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/cursors/exact.png` & `microviewer-1.4.0/microviewer/cursors/exact.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/cursors/large-active.png` & `microviewer-1.4.0/microviewer/cursors/large-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/cursors/large.png` & `microviewer-1.4.0/microviewer/cursors/large.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/cursors/medium-active.png` & `microviewer-1.4.0/microviewer/cursors/medium-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/cursors/medium.png` & `microviewer-1.4.0/microviewer/cursors/medium.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/datacube.js` & `microviewer-1.4.0/microviewer/datacube.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -40,28 +40,31 @@
                 continue;
             }
 
             assignments[cube[i]] = 0;
             last = cube[i];
         }
 
+        assignments[0] = 0;
+
         this.assigned_colors = assignments;
         this.shuffleColors();
     }
 
     shuffleColors() {
         let colors = this.colors;
         const num_colors = colors.length;
 
         for (let segid in this.assigned_colors) {
             this.assigned_colors[segid] = colors[
                 ((Math.random() * 1000) | 0) % num_colors
             ];
         }
 
+        this.assigned_colors[0] = 0;
         this.cache.valid = false;
     }
 
     createColors(opacity = 1) {
         let colors = [{
                 r: 17,
                 g: 47,
@@ -186,17 +189,19 @@
 
 // Represents a segmentation volume alone
 class SegmentationVolume extends MonoVolume {
     constructor(datacube) {
         super(datacube);
         this.segments = {};
         this.renumbering = new datacube.cube.constructor(1);
+        this.inverse_renumbering = {};
         this.has_segmentation = true;
         this.hover_id = null;
         this.show_unselected = false;
+        this.max_label = 0;
     }
 
     selected() {
         let _this = this;
         return Object.keys(_this.segments)
             .filter((segid) => _this.segments[segid])
             .map((segid) => _this.renumbering[segid]);
@@ -210,16 +215,21 @@
         this.segments = {};
     }
 
     load(url, progressfn) {
         const _this = this;
         return super.load(url, progressfn)
             .then(function() {
-                _this.renumbering = renumber(_this.channel.cube);
+                [_this.renumbering, _this.max_label] = renumber(_this.channel.cube);
                 _this.initializeColorAssignments(_this.channel.cube);
+
+                for (const [key, value] of Object.entries(_this.renumbering)) {
+                    _this.inverse_renumbering[value] = key;
+                }
+                _this.inverse_renumbering[0] = 0;
             });
     }
 
     render(ctx, axis, slice) {
         let _this = this;
 
         const hover_id = this.hover_id;
@@ -441,14 +451,27 @@
         });
     }
 
     paintCircle(axis, slice, d, cx, cy, label) {
         let _this = this;
         let [width, height] = _this.channel.faceDimensions(axis);
 
+        if (_this.inverse_renumbering[label] === undefined) {
+            _this.renumbering[_this.max_label] = label;
+            _this.inverse_renumbering[label] = _this.max_label;
+            _this.assigned_colors[_this.max_label] = _this.colorToUint32({
+                r: 0,
+                g: 230,
+                b: 0
+            }, 1);
+            _this.max_label++;
+        }
+        label = _this.inverse_renumbering[label];
+        _this.segments[label] = true;
+
         cx = Math.floor(cx * width) + 0.5;
         cy = Math.floor(cy * height) + 0.5;
 
         let dx = d * width,
             dy = d * height;
 
         let rx = dx / 2,
@@ -520,15 +543,20 @@
 class HyperVolume extends MonoVolume {
     constructor(channel, segmentation) {
         super(channel);
         this.channel = channel; // a data cube
         this.segmentation = segmentation; // a segmentation cube
 
         this.renumbering = new segmentation.cube.constructor(1);
+        this.inverse_renumbering = {};
         this.has_segmentation = true;
+        this.max_label = 0;
+
+        this.show_unselected = false;
+        this.max_label = 0;
 
         this.segments = {};
         this.alpha = 0.5;
     }
 
     selected() {
         let _this = this;
@@ -591,17 +619,22 @@
                 let ArrayType = _this.segmentation.arrayType();
                 _this.segmentation.cube = new ArrayType(array_buffer);
                 _this.segmentation.loaded = true;
                 _this.segmentation.progress = 1;
                 _this.segmentation.normalized = false;
                 _this.cache.valid = false;
 
-                _this.renumbering = renumber(_this.segmentation.cube);
+                [_this.renumbering, _this.max_label] = renumber(_this.segmentation.cube);
                 _this.initializeColorAssignments(_this.segmentation.cube);
 
+                for (const [key, value] of Object.entries(_this.renumbering)) {
+                    _this.inverse_renumbering[value] = key;
+                }
+                _this.inverse_renumbering[0] = 0;
+
                 return _this.segmentation;
             });
 
         return Promise.all([channel_promise, seg_promise]);
     }
 
     /* renderChannelSlice
@@ -635,48 +668,87 @@
         masks = Uint32Array.of(masks.r, masks.g, masks.b);
         const brightener = this.colorToUint32({
             r: 10,
             g: 10,
             b: 10,
             a: 0
         });
+        const white = this.colorToUint32({
+            r: 200,
+            g: 200,
+            b: 200
+        }, 1);
         const hover_id = this.hover_id;
 
         let segments = this.segments;
+        let show_all = true;
+        const show_unselected = this.show_unselected;
         let selected_segments = new Uint8Array(this.renumbering.length);
-        Object.keys(_this.segments).forEach((label) => {
+        Object.keys(segments).forEach((label) => {
             selected_segments[label] = !!segments[label];
+            show_all &&= !segments[label];
         });
 
         let pxdata = pixels.data;
 
         let hover = false;
         let i4;
+        let color = 0;
 
         if (alpha > 0 && alpha < 1) {
-            for (let i = pixels32.length - 1; i >= 0; i--) {
-                segid = segmentation[i];
-                hover = (segid === hover_id) & segid > 0;
-                i4 = i << 2;
-                if (selected_segments[segid] | hover) {
-                    pxdata[i4] = ((pxdata[i4] * ialpha) + ((color_assignments[segid] & masks[0]) * alpha)) | 0;
-                    pxdata[i4 + 1] = ((pxdata[i4 + 1] * ialpha) + (((color_assignments[segid] & masks[1]) >>> 8) * alpha)) | 0;
-                    pxdata[i4 + 2] = ((pxdata[i4 + 2] * ialpha) + (((color_assignments[segid] & masks[2]) >>> 16) * alpha)) | 0;
+            if (show_unselected) {
+                for (let i = pixels32.length - 1; i >= 0; i--) {
+                    segid = segmentation[i];
+                    if (segid === 0) {
+                        continue;
+                    }
+                    hover = (segid === hover_id);
+                    i4 = i << 2;
+                    if (selected_segments[segid]) {
+                        color = white;
+                    } else {
+                        color = color_assignments[segid];
+                    }
+                    pxdata[i4] = ((pxdata[i4] * ialpha) + ((color & masks[0]) * alpha)) | 0;
+                    pxdata[i4 + 1] = ((pxdata[i4 + 1] * ialpha) + (((color & masks[1]) >>> 8) * alpha)) | 0;
+                    pxdata[i4 + 2] = ((pxdata[i4 + 2] * ialpha) + (((color & masks[2]) >>> 16) * alpha)) | 0;
                     pixels32[i] += hover * brightener;
                 }
+            } else {
+                for (let i = pixels32.length - 1; i >= 0; i--) {
+                    segid = segmentation[i];
+                    if (segid === 0) {
+                        continue;
+                    }
+                    hover = (segid === hover_id);
+                    i4 = i << 2;
+                    if (show_all | selected_segments[segid] | hover) {
+                        pxdata[i4] = ((pxdata[i4] * ialpha) + ((color_assignments[segid] & masks[0]) * alpha)) | 0;
+                        pxdata[i4 + 1] = ((pxdata[i4 + 1] * ialpha) + (((color_assignments[segid] & masks[1]) >>> 8) * alpha)) | 0;
+                        pxdata[i4 + 2] = ((pxdata[i4 + 2] * ialpha) + (((color_assignments[segid] & masks[2]) >>> 16) * alpha)) | 0;
+                        pixels32[i] += hover * brightener;
+                    }
+                }
             }
         } else if (alpha === 1) {
+            show_all = show_all || show_unselected;
             for (let i = pixels32.length - 1; i >= 0; i--) {
                 segid = segmentation[i];
-                hover = (segid === hover_id) && segid;
-
+                if (segid === 0) {
+                    continue;
+                }
+                hover = (segid === hover_id);
+                color = color_assignments[segid];
+                if (show_unselected & selected_segments[segid]) {
+                    color = white;
+                }
                 if (hover) {
-                    pixels32[i] = color_assignments[segid] + brightener;
-                } else if (selected_segments[segid]) {
-                    pixels32[i] = color_assignments[segid];
+                    pixels32[i] = color + brightener;
+                } else if (selected_segments[segid] | show_all) {
+                    pixels32[i] = color;
                 }
             }
         }
 
         ctx.putImageData(pixels, 0, 0);
 
         return this;
@@ -734,14 +806,163 @@
         let _this = this;
         segid = _this.segmentation.cast(segid);
         segid = _this.renumbering.indexOf(segid);
         if (segid !== -1) {
             _this.segments[segid] = true;
         }
     }
+
+    /* getSegsInCircle
+     *
+     * Get the segids located within a circle. All
+     * parameters are normalized between [0, 1]
+     *
+     * Required:
+     *   d: 0..1, Diameter of the circle
+     *   cx: 0..1, X coordinate of circle center
+     *   cy: 0..1, Y coordinate of circle center
+     *
+     * Return: [ segids ]
+     */
+    getSegsInCircle(axis, slice, d, cx, cy) {
+        let _this = this;
+        let [width, height] = _this.segmentation.faceDimensions(axis);
+
+        // Nullify anything outside the ellipse. Just like a GRE problem.
+
+        let buffer = _this.segmentation.slice(axis, slice, /*copy=*/ false);
+
+        cx = Math.floor(cx * width) + 0.5;
+        cy = Math.floor(cy * height) + 0.5;
+
+        let dx = d * width,
+            dy = d * height;
+
+        let rx = dx / 2,
+            rx2 = dx * dx / 4,
+            ry = dy / 2,
+            ry2 = dy * dy / 4;
+
+        let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
+            xf = Math.min(width, Math.trunc(cx + rx) + 0.5),
+            y0 = Math.max(0, Math.trunc(cy - ry) + 0.5),
+            yf = Math.min(width, Math.trunc(cy + ry) + 0.5);
+
+        let segid = 0,
+            bounds_test = 0.0;
+
+        let segids = {};
+
+        // For anisotropic data, we need to distort our circle (UI) into an ellipse 
+        // since we've distorted the data to be square.
+        // eqn of an ellipse: ((x - h)^2 / rx^2) + ((y - k)^2 / ry^2) <= 1
+        // We'll use < instead of <= though to exclude the boundary
+
+        for (var x = x0; x <= xf; x++) {
+            for (var y = y0; y <= yf; y++) {
+                bounds_test = ((x - cx) * (x - cx) / rx2) + ((y - cy) * (y - cy) / ry2);
+                segid = ((bounds_test < 1) && buffer[(x | 0) + width * (y | 0)]) | 0;
+                segids[segid] = true;
+            }
+        }
+
+        delete segids[0];
+
+        return Object.keys(segids).map((segid) => parseInt(segid, 10));
+    }
+
+    selectSegsInCircle(axis, slice, d, cx, cy) {
+        let _this = this;
+        let segs = _this.getSegsInCircle(axis, slice, d, cx, cy);
+        segs.forEach((segid) => {
+            _this.segments[segid] = true;
+        });
+    }
+
+    eraseSegsInCircle(axis, slice, d, cx, cy) {
+        let _this = this;
+        let segs = _this.getSegsInCircle(axis, slice, d, cx, cy);
+        segs.forEach((segid) => {
+            _this.segments[segid] = false;
+        });
+    }
+
+    paintCircle(axis, slice, d, cx, cy, label) {
+        let _this = this;
+        let [width, height] = _this.segmentation.faceDimensions(axis);
+
+        if (_this.inverse_renumbering[label] === undefined) {
+            _this.renumbering[_this.max_label] = label;
+            _this.inverse_renumbering[label] = _this.max_label;
+            _this.assigned_colors[_this.max_label] = _this.colorToUint32({
+                r: 0,
+                g: 230,
+                b: 0
+            }, 1);
+            _this.max_label++;
+        }
+        label = _this.inverse_renumbering[label];
+        _this.segments[label] = true;
+
+        cx = Math.floor(cx * width) + 0.5;
+        cy = Math.floor(cy * height) + 0.5;
+
+        let dx = d * width,
+            dy = d * height;
+
+        let rx = dx / 2,
+            rx2 = dx * dx / 4,
+            ry = dy / 2,
+            ry2 = dy * dy / 4;
+
+        let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
+            xf = Math.min(width, Math.trunc(cx + rx) + 0.5),
+            y0 = Math.max(0, Math.trunc(cy - ry) + 0.5),
+            yf = Math.min(width, Math.trunc(cy + ry) + 0.5);
+
+        let segid = 0,
+            bounds_test = 0.0;
+
+        // For anisotropic data, we need to distort our circle (UI) into an ellipse 
+        // since we've distorted the data to be square.
+        // eqn of an ellipse: ((x - h)^2 / rx^2) + ((y - k)^2 / ry^2) <= 1
+        // We'll use < instead of <= though to exclude the boundary
+        let cube = _this.segmentation.cube;
+
+        if (axis == 'z') {
+            for (var y = y0; y <= yf; y++) {
+                for (var x = x0; x <= xf; x++) {
+                    bounds_test = ((x - cx) * (x - cx) / rx2) + ((y - cy) * (y - cy) / ry2);
+                    if (bounds_test < 1) {
+                        cube[(x | 0) + width * ((y | 0) + height * (slice | 0))] = label;
+                    }
+                }
+            }
+        } else if (axis == 'y') {
+            for (var z = y0; z <= yf; z++) {
+                for (var x = x0; x <= xf; x++) {
+                    bounds_test = ((x - cx) * (x - cx) / rx2) + ((z - cy) * (z - cy) / ry2);
+                    if (bounds_test < 1) {
+                        cube[(x | 0) + width * ((slice | 0) + height * (z | 0))] = label;
+                    }
+                }
+            }
+        } else if (axis === 'x') {
+            for (var z = y0; z <= yf; z++) {
+                for (var y = x0; y <= xf; y++) {
+                    bounds_test = ((y - cx) * (y - cx) / rx2) + ((z - cy) * (z - cy) / ry2);
+                    if (bounds_test < 1) {
+                        cube[(slice | 0) + width * ((y | 0) + height * (z | 0))] = label;
+                    }
+                }
+            }
+        } else {
+            throw new Error("Unsupported axis.")
+        }
+    }
 }
 
 class CachedImageData {
     constructor(context) {
         this.context = context;
         this.cache = null;
     }
@@ -804,14 +1025,68 @@
         let face = this.faces[axis];
         return [
             this.size[face[0]],
             this.size[face[1]]
         ];
     }
 
+    numpyHeader() {
+        const dtype = `<u${this.bytes}`;
+        const shape = `${this.size.x},${this.size.y},${this.size.z}`;
+        const header = `{"descr": "${dtype}", "fortran_order": True, "shape": (${shape}), }`;
+        const encoder = new TextEncoder();
+        const headerBytes = encoder.encode(header);
+
+        // \x93NUMPY\x01\x00
+        const magic = [0x93, 0x4E, 0x55, 0x4D, 0x50, 0x59, 0x01, 0x00];
+        let headerLength = headerBytes.length + 10;
+
+        // align to 64 bytes and fill with spaces 0x20
+        headerLength = Math.ceil(headerLength / 64) * 64;
+
+        const combinedBytes = new Uint8Array(headerLength);
+        combinedBytes.fill(0x20);
+        combinedBytes.set(magic, 0);
+        combinedBytes[8] = headerLength - 10;
+        combinedBytes[9] = 0;
+        combinedBytes.set(headerBytes, 10);
+        combinedBytes[headerLength - 1] = 10;
+        return combinedBytes;
+    }
+
+    saveNumpy(filename) {
+        const npyHeader = this.numpyHeader();
+        // Create a combined array of header and data bytes
+        const combinedBytes = new Uint8Array(npyHeader.length + this.cube.byteLength);
+        const cubeview = new Uint8Array(this.cube.buffer, 0, this.cube.byteLength);
+        combinedBytes.set(npyHeader, 0);
+        combinedBytes.set(cubeview, npyHeader.length);
+        this.save(filename, combinedBytes);
+    }
+
+    async saveCrackle(filename) {
+        const cubeview = new Uint8Array(this.cube.buffer, 0, this.cube.byteLength);
+        const buffer = await compressCrackle(
+            cubeview, this.bytes,
+            this.size.x, this.size.y, this.size.z,
+        );
+        this.save(filename, buffer);
+    }
+
+    save(filename, buffer) {
+        const blob = new Blob([buffer.buffer]);
+        const link = document.createElement('a');
+        link.href = URL.createObjectURL(blob);
+        link.download = filename;
+
+        document.body.appendChild(link);
+        link.click();
+        document.body.removeChild(link);
+    }
+
     // for internal use, makes a canvas for blitting images to
     createImageContext() {
         let canvas = document.createElement('canvas');
         canvas.width = this.size.x;
         canvas.height = this.size.y;
 
         return canvas.getContext('2d'); // used for accelerating XY plane image insertions
@@ -1543,14 +1818,15 @@
             assignments.set(cube[i], next_label);
             cube[i] = next_label;
             last_relabel = next_label;
             next_label++;
         }
     }
 
-    let renumbering = new cube.constructor(Number(next_label));
+    // +10000 for 10000 paint slots
+    let renumbering = new cube.constructor(Number(next_label) + 10000);
     for (let [label, remap] of assignments) {
         renumbering[remap] = label;
     }
 
-    return renumbering;
+    return [renumbering, next_label];
 }
```

### Comparing `microviewer-1.3.0/microviewer/favicon.ico` & `microviewer-1.4.0/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer/index.html` & `microviewer-1.4.0/microviewer/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 <!doctype html>
 <html>
   <head>
     <title>μViewer</title>
     <script src="./jquery-3.7.0.min.js"></script>
+    <script src="./crackle.js"></script>
     <script src="./datacube.js"></script>
     <meta charset="utf-8">
 
+    <link rel="preload" as="image" href="./cursors/exact.png">
+    <link rel="preload" as="image" href="./cursors/small.png">
+    <link rel="preload" as="image" href="./cursors/medium.png">
+    <link rel="preload" as="image" href="./cursors/large.png">
+    <link rel="preload" as="image" href="./cursors/exact-active.png">
+    <link rel="preload" as="image" href="./cursors/small-active.png">
+    <link rel="preload" as="image" href="./cursors/medium-active.png">
+
     <style>
       html {
         overflow: hidden;
       }
 
       body {
         font-family: monospace;
@@ -263,38 +272,21 @@
 
         return new DataCube({
           bytes: num_bytes,
           size: size,
         });
       }
 
-      function setup_single_volume (data) {  
-        render_static();
-
-        let datacube = create_datacube(data.data_types[0], data.data_bytes, SIZE);
-
-        if (data.layer_type === 'segmentation') {
-          window.vol = new SegmentationVolume(datacube, true);
-        }
-        else {
-          window.vol = new MonoVolume(datacube, false);
-        }
-
-        let vol = window.vol;
-
-        vol.load('/channel', function (ratio) {
-          render();
-        }).then( () => render() );
-
+      function configure_segmentation_ui () {
         $(channel).on('mousemove', function (e) {
           e.stopPropagation();
           MOUSE_OVER_IMAGE = true;
 
-          let x = e.offsetX / $(this).innerWidth(), 
-            y = e.offsetY / $(this).innerHeight();
+          let x = e.offsetX / $(channel).innerWidth(), 
+            y = e.offsetY / $(channel).innerHeight();
 
           x = clamp(x, 0, 0.999999999);
           y = clamp(y, 0, 0.999999999);
 
           if (AXIS == 'z') {
             SLICE.x = (x * SIZE.x)|0;
             SLICE.y = (y * SIZE.y)|0;
@@ -322,15 +314,23 @@
           diameter /= $(channel).innerWidth();
 
           if (ZOOMED) {
             diameter /= ZOOM_FACTOR;
           }
           
           if (evt.which === 1) {
-            vol.selectSegsInCircle(AXIS, SLICE[AXIS], diameter, x, y);
+            if (elems.paintmode.prop("checked")) {
+              let label = parseInt(elems.paintlabel.val());
+              if (!isNaN(label)) {
+                vol.paintCircle(AXIS, SLICE[AXIS], diameter, x, y, label);
+              }
+            }
+            else {
+              vol.selectSegsInCircle(AXIS, SLICE[AXIS], diameter, x, y);
+            }
           }
     
           render(true);
         }
 
         function erase (evt) {
           var x = evt.offsetX / $(channel).innerWidth(), 
@@ -342,15 +342,20 @@
           let diameter = BRUSH_DIAMETERS[BRUSH];
           diameter /= $(channel).innerWidth();
 
           if (ZOOMED) {
             diameter /= ZOOM_FACTOR;
           }
 
-          vol.eraseSegsInCircle(AXIS, SLICE[AXIS], diameter, x, y);
+          if (elems.paintmode.prop("checked")) {
+            vol.paintCircle(AXIS, SLICE[AXIS], diameter, x, y, 0);
+          }
+          else {
+            vol.eraseSegsInCircle(AXIS, SLICE[AXIS], diameter, x, y);
+          }
           render(true);  
         }
 
         if (vol.has_segmentation) {
           $(document).on("mousemove", function () {
             MOUSE_OVER_IMAGE = false;
             PAINTING_MODE = 0;
@@ -408,68 +413,50 @@
               erase(evt);
               evt.stopPropagation();
               evt.preventDefault();
             });
         }
       }
 
-      function setup_hyper_volume (data) {
+      function setup_single_volume (data) {  
         render_static();
 
-        function get_cube(index) {
-          return create_datacube(data.data_types[index], data.data_bytes[index], SIZE);
+        let datacube = create_datacube(data.data_types[0], data.data_bytes, SIZE);
+
+        if (data.layer_type === 'segmentation') {
+          window.vol = new SegmentationVolume(datacube, true);
+        }
+        else {
+          window.vol = new MonoVolume(datacube, false);
         }
 
-        window.vol = new HyperVolume(get_cube(0), get_cube(1));
         let vol = window.vol;
 
-        vol.load(function (ratio) {
+        vol.load('/channel', function (ratio) {
           render();
         }).then( () => render() );
 
-        $(channel).on('mousemove', function (e) {
-          e.stopPropagation();
-          MOUSE_OVER_IMAGE = true;
-          var x = e.offsetX / $(this).innerWidth(), 
-            y = e.offsetY / $(this).innerHeight();
+        configure_segmentation_ui();
+      }
 
-          x = clamp(x, 0, 0.999999999);
-          y = clamp(y, 0, 0.999999999);
+      function setup_hyper_volume (data) {
+        render_static();
 
-          if (AXIS == 'z') {
-            SLICE.x = (x * SIZE.x)|0;
-            SLICE.y = (y * SIZE.y)|0;
-          }
-          else if (AXIS == 'y') {
-            SLICE.x = (x * SIZE.x)|0;
-            SLICE.z = (y * SIZE.z)|0;
-          }
-          else if (AXIS == 'x') {
-            SLICE.y = (x * SIZE.y)|0;
-            SLICE.z = (y * SIZE.z)|0;
-          }
+        function get_cube(index) {
+          return create_datacube(data.data_types[index], data.data_bytes[index], SIZE);
+        }
 
-          render(); 
-        });
+        window.vol = new HyperVolume(get_cube(0), get_cube(1));
+        let vol = window.vol;
 
-        $(document).on("mousemove", function () {
-          MOUSE_OVER_IMAGE = false;
+        vol.load(function (ratio) {
           render();
-        });
-
-        $(channel).on('click', function (evt) {
-          var x = evt.offsetX / $(this).innerWidth(), 
-            y = evt.offsetY / $(this).innerHeight();
+        }).then( () => render() );
 
-          x = clamp(x, 0, 1);
-          y = clamp(y, 0, 1);  
-          
-          vol.toggleSegment(AXIS, SLICE[AXIS], x, y);
-          render(true);
-        });
+        configure_segmentation_ui();
       }
 
       function toggleMenu () {
         elems.rtsidebar.toggleClass("hidden");
         elems.showsidebar.toggleClass("hidden");
       }
 
@@ -494,14 +481,17 @@
           show_hover: $('#show_hover'),
           show_unselected: $('#show_unselected'),
           magnification: $('#magnification'),
           showsidebar: $('#show-sidebar'),
           rtsidebar: $('#right-sidebar'),
           copysegs: $("#copy-segs"),
           brushsize: $("#brush-size"),
+          paintmode: $("#paint_voxels"),
+          paintlabel: $("#paintlabel"),
+          memoryusage: $("#memory-usage"),
         };
         
         window.channel = elems.channel[0];
         window.channelctx = channel.getContext('2d');
 
         $.get('/parameters', function (data, status) {
           SIZE = {
@@ -561,14 +551,18 @@
             
             render();
           });
 
           loop();
         });
 
+        elems.paintlabel.on("keyup keypress keydown", function (evt) {
+          evt.stopPropagation();
+        });
+
         elems.showsidebar.on("click", function () {
           toggleMenu(); 
         });
 
         elems.copysegs.on("click", function () {
           navigator.clipboard.writeText(elems.selected_segments.text());
         });
@@ -637,14 +631,17 @@
             sx = SIZE.y;
             sy = SIZE.z;
           }
 
           if (ZOOMED) {
             elems.channel.css('transform', '');
           }
+          else if (MAGNIFICATION > ZOOM_FACTOR) {
+            return;
+          }
           else {
             let zfactor = ZOOM_FACTOR / MAGNIFICATION;
             let dx = x / sx - 0.5;
             let dy = y / sy - 0.5;
 
             dx *= elems.channel.width() * zfactor;
             dy *= elems.channel.height() * zfactor;
@@ -690,15 +687,15 @@
           move_slice(-1);
         }
         else if (evt.keyCode === 'L'.charCodeAt(0)
           || evt.keyCode === 'l'.charCodeAt(0)
         ) {
           
           vol.shuffleColors();
-          render(true);          
+          render(true);   
         }
         else if (evt.keyCode === 'X'.charCodeAt(0)
           || evt.keyCode === 'x'.charCodeAt(0)) {
           
           if (vol.clearSelected) {
             vol.clearSelected()
           }
@@ -732,14 +729,21 @@
             || evt.keyCode === "u".charCodeAt(0)) {
 
           elems.show_unselected.prop("checked", 
             !elems.show_unselected.prop("checked")
           );
           render(true);
         }
+        else if (evt.keyCode === "P".charCodeAt(0)
+            || evt.keyCode === "p".charCodeAt(0)) {
+
+          elems.paintmode.prop("checked", 
+            !elems.paintmode.prop("checked")
+          );
+        }
         else if (evt.keyCode === "1".charCodeAt(0)) {
           MAGNIFICATION /= 2;
           MAGNIFICATION = Math.max(MAGNIFICATION, 0.25);
           elems.channel.css("width", (channel.width * MAGNIFICATION) + "px");
           elems.channel.css("height", (channel.height * MAGNIFICATION) + "px");
           elems.channel.css('transform', '');
           render();
@@ -797,14 +801,17 @@
           }
           else {
             $(channel).addClass("paintable");
           }
 
           PARAMETERS.cloudpath[0].split('/')
         }
+        else {
+          $(channel).addClass("paintable");
+        }
 
         let hyper = (PARAMETERS.viewtype === 'hyper') ? 'Hyper ' : '';
         let firstlayer = PARAMETERS.cloudpath[0];
 
         if (firstlayer === 'IN MEMORY') {
           document.title = `MEMORY - ${hyper}μViewer`;
         }
@@ -818,14 +825,25 @@
         elems.cloudpath.text( PARAMETERS.cloudpath.join("; ") );
         elems.bounds.text(
           `<${b[0]}, ${b[1]}, ${b[2]}>, <${b[3]}, ${b[4]}, ${b[5]}>`
         );
         elems.dtype.text( PARAMETERS.data_types.join("; ") );
         elems.resolution.text( PARAMETERS.resolution.join('x') );
         elems.shape.text( `<${SIZE.x}, ${SIZE.y}, ${SIZE.z}>` );
+
+
+
+        let bytes = PARAMETERS["data_bytes"];
+
+        if (Array.isArray(bytes)) {
+          bytes = bytes.reduce((partialSum, a) => partialSum + a, 0);
+        }
+        bytes *= SIZE.x * SIZE.y * SIZE.z;
+        let megabytes = Math.floor(bytes / 1e6);
+        elems.memoryusage.text(`${megabytes}`);
       }
 
       function update_pxvalue () {
         PXVALUE = [];
 
         vol.hover_id = null;
         if (vol.segmentation) {
@@ -960,14 +978,30 @@
         if (_needsrender) {
           hardRender();
         }
 
         requestAnimationFrame(loop);
       }
 
+      function saveNumpy (filename) {
+        let dc = vol.channel;
+        if (vol.segmentation) {
+          dc = vol.segmentation;
+        }
+        dc.saveNumpy(filename);
+      }
+
+      function saveCrackle (filename) {
+        let dc = vol.channel;
+        if (vol.segmentation) {
+          dc = vol.segmentation;
+        }
+        dc.saveCrackle(filename);
+      }
+
     </script>
   </head>
   <body>
     <div id="infobar">
       <span id="axis"></span> <span id="magnification"></span> <span id="coord"></span> <span id="realcoord"></span> <span id="pxvalue"></span> 
       <br> 
       Last Click: <span id="clickcoord"></span> <span id="clickrealcoord"></span> <span id="clickpxvalue"></span>  <span id="loading"></span>
@@ -986,44 +1020,60 @@
           shape: <span id="shape"></span> 
           <br />
           bounds: (<span id="bounds"></span>)
           <br / >
           dtype: <span id="dtype"></span>
           <br />
           resolution: <span id="resolution"></span> nm<sup>3</sup>
+          <br />
+          memory: <span id="memory-usage"></span> MB
         </div>
 
         <p class="segmentation">SELECTION VISIBILITY</p>
-        <input class="segmentation" type="checkbox" id="show_hover" name="show_hover" checked="checked"/> <label class="segmentation" for="show_hover">Highlight Hover?</label>
-        <input class="segmentation" type="checkbox" id="show_unselected" name="show_unselected" /> <label class="segmentation" for="show_unselected">Show Unselected?</label>
+        <input class="segmentation" type="checkbox" id="show_hover" name="show_hover" checked="checked"/> <label class="segmentation" for="show_hover">Highlight (H)over?</label>
+        <input class="segmentation" type="checkbox" id="show_unselected" name="show_unselected" /> <label class="segmentation" for="show_unselected">Show (U)nselected?</label> <br />
+        <input class="segmentation" type="checkbox" id="paint_voxels" name="paint_voxels" /> <label class="segmentation" for="paint_voxels">Direct (P)aint?</label>
 
         <p class="segmentation">BRUSH SIZE</p>
         <div class="segmentation" id="brush-size">
           <div class="exact"></div>
           <div class="small"></div>
           <div class="medium"></div>
           <div class="large"></div>
         </div>
 
+        <p class="segmentation">PAINT LABEL</p>
+        <div class="segmentation">
+          <input id="paintlabel" type="number" value="1" />
+        </div>
+
         <p class="segmentation">SELECTED SEGMENTS <button id="copy-segs">copy</button></p>
         <div class="segmentation" id="selected_segments"></div>
         <textarea id="addsegs" class="segmentation" type="text" placeholder="Input comma separated segids and press enter."></textarea>
 
+        <p class="segmentation">SAVE SEGMENTATION</p>
+
+        <div class="segmentation">
+          <button onclick="saveNumpy('image.npy')" title="Save as a .npy file. Might be big depending on your image size!">.npy</button> 
+          <button onclick="saveCrackle('image.ckl')" title="Save as a small .ckl file. There will be some processing time. Read more at https://github.com/seung-lab/crackle.">.ckl</button>
+        </div>
+
         <p>CONTROLS</p>
         <ul>
           <li>W/S ,/. or scroll - advance selected images</li>
           <li>A/D - switch slicing plane</li>
           <li>Space - zoom in to point</li>
           <li class='segmentation'>L - recolor segmentation labels</li>
           <li>Left Click - <span class="segmentation">paint, </span>freeze info about current pixel</li>
           <li class="segmentation">Right Click - erase</li>
           <li class="segmentation">X - clear selected segments</li>
           <li class="hyperview">+/- increase, decrease opacity</li>
           <li class='segmentation'>H - toggle hover highlight</li>
           <li class='segmentation'>U - toggle show unselected</li>
+          <li class='segmentation'>P - toggle direct voxel painting</li>
           <li>1/2 - zoom out/in</li>
           <li>M - show/hide menu</li>
           <li class="segmentation">Q/E - decrease/increase brush size</li>
         </ul>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -1,29 +1,43 @@
 
 
+
+
+
+
+
+
+
 Last Click:
 ===============================================================================
 ===============================================================================
 ===============================================================================
 DIMENSIONS
 shape:
 bounds: ()
 > dtype:
 resolution:  nm3
+memory:  MB
 SELECTION VISIBILITY
-* Highlight Hover? ⁰ Show Unselected?
+* Highlight (H)over? ⁰ Show (U)nselected?
+⁰ Direct (P)aint?
 BRUSH SIZE
+PAINT LABEL
+[Unknown INPUT type]
 SELECTED SEGMENTS copy
+SAVE SEGMENTATION
+.npy .ckl
 CONTROLS
     * W/S ,/. or scroll - advance selected images
     * A/D - switch slicing plane
     * Space - zoom in to point
     * L - recolor segmentation labels
     * Left Click - paint, freeze info about current pixel
     * Right Click - erase
     * X - clear selected segments
     * +/- increase, decrease opacity
     * H - toggle hover highlight
     * U - toggle show unselected
+    * P - toggle direct voxel painting
     * 1/2 - zoom out/in
     * M - show/hide menu
     * Q/E - decrease/increase brush size
```

### Comparing `microviewer-1.3.0/microviewer/jquery-3.7.0.min.js` & `microviewer-1.4.0/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/microviewer.egg-info/PKG-INFO` & `microviewer-1.4.0/microviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.3.0
+Version: 1.4.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.3.0/microviewer.egg-info/SOURCES.txt` & `microviewer-1.4.0/microviewer.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 MANIFEST.in
 README.md
 requirements.txt
 seg-demo.png
 setup.cfg
 setup.py
 microviewer/__init__.py
+microviewer/crackle.js
 microviewer/datacube.js
 microviewer/favicon.ico
 microviewer/index.html
 microviewer/jquery-3.7.0.min.js
+microviewer/libcrackle.wasm
 microviewer.egg-info/PKG-INFO
 microviewer.egg-info/SOURCES.txt
 microviewer.egg-info/dependency_links.txt
 microviewer.egg-info/entry_points.txt
 microviewer.egg-info/not-zip-safe
 microviewer.egg-info/pbr.json
 microviewer.egg-info/requires.txt
```

### Comparing `microviewer-1.3.0/microviewer_cli/cli.py` & `microviewer-1.4.0/microviewer_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,29 +106,38 @@
 @click.argument("image")
 @click.argument("segmentation", required=False, default=None)
 @click.option('--seg', is_flag=True, default=False, help="Display image as segmentation.", show_default=True)
 @click.option('--browser/--no-browser', default=True, is_flag=True, help="Open the dataset in the system's default web browser.", show_default=True)
 @click.option('--shape', type=Tuple234(), default=None, help="Set shape manually for memmaps.", show_default=True)
 @click.option('--dtype', type=str, default=None, help="Set dtype manually for memmaps.", show_default=True)
 @click.option('--order', type=str, default="F", help="Set order manually for memmaps.", show_default=True)
-def main(image, segmentation, seg, browser, shape, dtype, order):
+@click.option('--paint', is_flag=True, default=False, help="Create a blank segmentation for painting.", show_default=True)
+def main(
+  image, segmentation, 
+  seg, paint, browser, 
+  shape, dtype, order,
+):
   """
   View 3D images in the browser.
   """
   try:
     image_np = load(image, shape, dtype, order)
     if segmentation:
       segmentation_np = load(segmentation, shape, dtype, order)
   except ValueError as err:
     print("Data type not supported.", err)
     return
   except FileNotFoundError as err:
     print(f"File not found: {err.filename}")
     return
 
+  if not segmentation and paint:
+    segmentation_np = np.zeros(image_np.shape, dtype=np.uint16, order="F")
+    segmentation = "PAINTING"
+
   if segmentation is not None:
     microviewer.hyperview(
       image_np, segmentation_np, 
       browser=browser, 
       cloudpath=[ image, segmentation ],
     )
   else:
```

### Comparing `microviewer-1.3.0/seg-demo.png` & `microviewer-1.4.0/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.3.0/setup.cfg` & `microviewer-1.4.0/setup.cfg`

 * *Files identical despite different names*

