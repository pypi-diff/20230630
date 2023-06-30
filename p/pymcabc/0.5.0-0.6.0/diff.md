# Comparing `tmp/pymcabc-0.5.0.tar.gz` & `tmp/pymcabc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcabc-0.5.0.tar", last modified: Mon Jun 26 10:44:00 2023, max compression
+gzip compressed data, was "pymcabc-0.6.0.tar", last modified: Fri Jun 30 10:20:25 2023, max compression
```

## Comparing `pymcabc-0.5.0.tar` & `pymcabc-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 10:43:51.000000 pymcabc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 10:43:51.000000 pymcabc-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 10:44:00.261516 pymcabc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-26 10:43:51.000000 pymcabc-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/pymcabc/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/cross_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/decay_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/feynman_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/generate_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/identify_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/save_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/pymcabc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:44:00.261516 pymcabc-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-26 10:43:51.000000 pymcabc-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_boost.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_crosssection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_evengen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_identify.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 10:20:17.000000 pymcabc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 10:20:17.000000 pymcabc-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-30 10:20:25.416355 pymcabc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-30 10:20:17.000000 pymcabc-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/pymcabc/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/decay_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/feynman_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/generate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/identify_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-30 10:20:17.000000 pymcabc-0.6.0/pymcabc/save_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/pymcabc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 10:20:25.000000 pymcabc-0.6.0/pymcabc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:20:25.416355 pymcabc-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-30 10:20:17.000000 pymcabc-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:20:25.416355 pymcabc-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_crosssection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_evengen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-30 10:20:17.000000 pymcabc-0.6.0/tests/test_plot.py
```

### Comparing `pymcabc-0.5.0/LICENSE` & `pymcabc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/PKG-INFO` & `pymcabc-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.5.0
+Version: 0.6.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.5.0/README.md` & `pymcabc-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/pymcabc/cross_section.py` & `pymcabc-0.6.0/pymcabc/cross_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         self.pi = pymcabc.constants.pi
         self.delta = pymcabc.constants.delta
         self.p_i = library["pi"][0]  # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
 
     def s_channel(self):
         """definition for s channel"""
         # deno = self.Ecm**2 - self.mx**2
-        deno = (self.p_i**2 + self.m1**2) * (self.p_i**2 + self.m2**2)
-        deno = math.sqrt(deno)
-        deno = deno + self.m1**2 + self.m2**2
+        deno = math.sqrt(self.p_i**2 + self.m1**2) + math.sqrt(self.p_i**2 + self.m2**2)
+        deno = deno**2 - self.mx**2
+        #deno = deno + self.m1**2 + self.m2**2 
         if abs(deno) <= 0.09:
             return (self.g**2) / (deno + 100)
         else:
             return (self.g**2) / deno
 
     def t_channel(self, costh, pf):
         """definition for t channel"""
```

### Comparing `pymcabc-0.5.0/pymcabc/decay_particle.py` & `pymcabc-0.6.0/pymcabc/decay_particle.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         """decay particle"""
 
         E1 = (top.mass() ** 2 - self.decay2_mass**2 + self.decay1_mass**2) / (
             2 * top.mass()
         )
 
         E2 = top.mass() - E1
-
+        """
         self.decay_p = math.sqrt(
             (top.mass() ** 2 - (self.decay1_mass + self.decay2_mass) ** 2)
             * (top.mass() ** 2 - (self.decay1_mass - self.decay2_mass) ** 2)
         ) / (2 * top.mass())
 
         """ 
         self.decay_p = (
@@ -61,15 +61,16 @@
                 * (
                     self.mA**2 * self.mB**2
                     + self.mA**2 * self.mC**2
                     + self.mB**2 * self.mC**2
                 )
             )
         )
-
+        
+        """
         # decay2.mass() = self.decay2_mass
 
         E1 = math.sqrt(
             self.decay1_mass * self.decay1_mass + self.decay_p * self.decay_p
         ) 
         E2 = math.sqrt(
             self.decay2_mass * self.decay2_mass + self.decay_p * self.decay_p
```

### Comparing `pymcabc-0.5.0/pymcabc/detector.py` & `pymcabc-0.6.0/pymcabc/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,35 +22,34 @@
             return particle
         else:
             output_px = [0] * len(particle.px)
             output_py = [0] * len(particle.px)
             output_pz = [0] * len(particle.px)
             output_E = [0] * len(particle.px)
             for i in range(len(particle.px)):
+                """
                 momentum = math.sqrt(
                     particle.px[i] ** 2 + particle.py[i] ** 2 + particle.pz[i] ** 2
                 )
                 random_measure_momentum = (
                     random.gauss(momentum, self.factor * self.sigma) / momentum
                 )
                 random_measure_energy = (
                     random.gauss(particle.E[i], self.sigma) / particle.E[i]
                 )
 
                 output_px[i] = random_measure_momentum * particle.px[i]
                 output_py[i] = random_measure_momentum * particle.py[i]
                 output_pz[i] = random_measure_momentum * particle.pz[i]
-
                 output_E[i] = random_measure_energy * particle.E[i]
+                """
 
-                """output_px[i] = random.gauss(particle.px[i], self.sigma)
-                output_py[i] = random.gauss(particle.py[i], self.sigma)
-                output_pz[i] = random.gauss(particle.pz[i], self.sigma)
+                output_px[i] = random.gauss(particle.px[i], self.factor*self.sigma)
+                output_py[i] = random.gauss(particle.py[i], self.factor*self.sigma)
+                output_pz[i] = random.gauss(particle.pz[i], self.factor*self.sigma)
                 output_E[i] = random.gauss(particle.E[i], self.sigma)
-
-                mass = output_E[i] ** 2 - (
-                    output_px[i] ** 2 + output_py[i] ** 2 + output_pz[i] ** 2
-                )
-                """
                 
             particle_output = Particle(output_E, output_px, output_py, output_pz)
         return particle_output
+
+#mass = output_E[i] ** 2 - (output_px[i] ** 2 + output_py[i] ** 2 + output_pz[i] ** 2)
+
```

### Comparing `pymcabc-0.5.0/pymcabc/feynman_diagram.py` & `pymcabc-0.6.0/pymcabc/feynman_diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,26 +31,24 @@
                 if p == "s":
                     self.s_chan()
                 elif p == "t":
                     self.t_chan()
                 elif p == "u":
                     self.u_chan()
                 else:
-                    print("Possible channels: s, t, and u")
                     return 0
+        elif channel =="s":
+            self.s_chan()
+        elif channel == "t":
+            self.t_chan()
+        elif channel == "u":
+            self.u_chan()
         else:
-            if channel == "s":
-                self.s_chan()
-            if channel == "t":
-                self.t_chan()
-            if channel == "u":
-                self.u_chan()
-            else:
-                print("Possible channels: s, t, and u")
-                return
+            print("Possible channels: s, t, and u")
+            return 0
 
     def s_chan(self):
         fig = plt.figure(figsize=(5.0, 5.0))
         ax = fig.add_axes([0, 0, 1, 1], frameon=False)
 
         diagram = Diagram(ax)
         in1 = diagram.vertex(xy=(0.1, 0.75), marker="")
```

### Comparing `pymcabc-0.5.0/pymcabc/generate_event.py` & `pymcabc-0.6.0/pymcabc/generate_event.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/pymcabc/identify_process.py` & `pymcabc-0.6.0/pymcabc/identify_process.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/pymcabc/particle.py` & `pymcabc-0.6.0/pymcabc/particle.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/pymcabc/plotting.py` & `pymcabc-0.6.0/pymcabc/plotting.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/pymcabc/save_events.py` & `pymcabc-0.6.0/pymcabc/save_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,18 @@
         self.w_max = library["w_max"][0]
         self.Ecm = library["Ecm"][0]
         input_string = library["process"][0]
         input_string = input_string.replace(" > ", " ")
         input_string = input_string.split(" ")
         self.output_1 = input_string[2]
         self.output_2 = input_string[3]
+        if self.output_1 == self.output_2:
+            self.output_1 = self.output_1 + "_1"
+            self.output_2 = self.output_2 + "_2"
+
         self.decay_process = library["decay_process"]
         if self.decay_process[0] != "NaN":
             decay_split = self.decay_process[0].replace(" > ", " ")
             decay_split = decay_split.split(" ")
             self.decayed1 = decay_split[1]
             self.decayed2 = decay_split[2]
         (
@@ -113,22 +117,22 @@
         else:
             file = uproot.recreate(name)
             top1 = self.top1
             top2 = self.top2
             decay1, decay2 = DecayParticle().prepare_decay(top1)
             decay3, decay4 = DecayParticle().prepare_decay(top2)
             if self.boolDetector == True:
-                if decay1.px[0] == -9 and decay1.E[0] == -9:
-                    self.top1 = Detector(
-                        self.detector_sigma, self.detector_factor
-                    ).gauss_smear(self.top1)
-                if decay2.px[0] == -9 and decay2.E[0] == -9:
-                    self.top2 = Detector(
-                        self.detector_sigma, self.detector_factor
-                    ).gauss_smear(self.top2)
+                #if decay1.px[0] == -9 and decay1.E[0] == -9:
+                self.top1 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(self.top1)
+                #if decay2.px[0] == -9 and decay2.E[0] == -9:
+                self.top2 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(self.top2)
                 # self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
                 # self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
 
                 decay1 = Detector(
                     self.detector_sigma, self.detector_factor
                 ).gauss_smear(decay1)
                 decay2 = Detector(
@@ -137,14 +141,15 @@
                 decay3 = Detector(
                     self.detector_sigma, self.detector_factor
                 ).gauss_smear(decay3)
                 decay4 = Detector(
                     self.detector_sigma, self.detector_factor
                 ).gauss_smear(decay4)
 
+
             file["events"] = {
                 self.output_1 + "_E": self.top1.E,
                 self.output_1 + "_Px": self.top1.px,
                 self.output_1 + "_Py": self.top1.py,
                 self.output_1 + "_Pz": self.top1.pz,
                 self.output_1 + "_E_decay_" + self.decayed1: decay1.E,
                 self.output_1 + "_Px_decay_" + self.decayed1: decay1.px,
```

### Comparing `pymcabc-0.5.0/pymcabc.egg-info/PKG-INFO` & `pymcabc-0.6.0/pymcabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.5.0
+Version: 0.6.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.5.0/pymcabc.egg-info/SOURCES.txt` & `pymcabc-0.6.0/pymcabc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/setup.py` & `pymcabc-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="pymcabc",
-    version="0.5.0",
+    version="0.6.0",
     description="Monte Carlo Event Generator for the ABC theory",
     author="Aman Desai",
     author_email="amanmukeshdesai@gmail.com",
     maintainer="Aman Desai",
     maintainer_email="amanmukeshdesai@gmail.com",
     url="https://github.com/amanmdesai/pymcabc",
     long_description=long_description,
```

### Comparing `pymcabc-0.5.0/tests/test_evengen.py` & `pymcabc-0.6.0/tests/test_evengen.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.5.0/tests/test_identify.py` & `pymcabc-0.6.0/tests/test_identify.py`

 * *Files identical despite different names*

