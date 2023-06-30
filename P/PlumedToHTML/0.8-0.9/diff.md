# Comparing `tmp/PlumedToHTML-0.8.tar.gz` & `tmp/PlumedToHTML-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PlumedToHTML-0.8.tar", last modified: Thu Jul 14 09:30:24 2022, max compression
+gzip compressed data, was "dist/PlumedToHTML-0.9.tar", last modified: Thu Jul 14 14:19:10 2022, max compression
```

## Comparing `PlumedToHTML-0.8.tar` & `PlumedToHTML-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gareth     (505) staff       (20)        0 2022-07-14 09:30:24.971622 PlumedToHTML-0.8/
--rw-r--r--   0 gareth     (505) staff       (20)     3550 2022-07-14 09:30:24.971109 PlumedToHTML-0.8/PKG-INFO
-drwxr-xr-x   0 gareth     (505) staff       (20)        0 2022-07-14 09:30:24.966930 PlumedToHTML-0.8/PlumedToHTML/
--rw-r--r--   0 gareth     (505) staff       (20)    13819 2022-05-22 22:39:24.000000 PlumedToHTML-0.8/PlumedToHTML/PlumedFormatter.py
--rw-r--r--   0 gareth     (505) staff       (20)     2912 2022-05-21 20:03:58.000000 PlumedToHTML-0.8/PlumedToHTML/PlumedLexer.py
--rw-r--r--   0 gareth     (505) staff       (20)    15751 2022-07-13 17:30:52.000000 PlumedToHTML-0.8/PlumedToHTML/PlumedToHTML.py
--rw-r--r--   0 gareth     (505) staff       (20)       84 2022-07-13 15:52:22.000000 PlumedToHTML-0.8/PlumedToHTML/__init__.py
-drwxr-xr-x   0 gareth     (505) staff       (20)        0 2022-07-14 09:30:24.970389 PlumedToHTML-0.8/PlumedToHTML.egg-info/
--rw-r--r--   0 gareth     (505) staff       (20)     3550 2022-07-14 09:30:24.000000 PlumedToHTML-0.8/PlumedToHTML.egg-info/PKG-INFO
--rw-r--r--   0 gareth     (505) staff       (20)      311 2022-07-14 09:30:24.000000 PlumedToHTML-0.8/PlumedToHTML.egg-info/SOURCES.txt
--rw-r--r--   0 gareth     (505) staff       (20)        1 2022-07-14 09:30:24.000000 PlumedToHTML-0.8/PlumedToHTML.egg-info/dependency_links.txt
--rw-r--r--   0 gareth     (505) staff       (20)        9 2022-07-14 09:30:24.000000 PlumedToHTML-0.8/PlumedToHTML.egg-info/requires.txt
--rw-r--r--   0 gareth     (505) staff       (20)       13 2022-07-14 09:30:24.000000 PlumedToHTML-0.8/PlumedToHTML.egg-info/top_level.txt
--rw-r--r--   0 gareth     (505) staff       (20)     2762 2022-06-02 16:41:32.000000 PlumedToHTML-0.8/README.md
--rw-r--r--   0 gareth     (505) staff       (20)       38 2022-07-14 09:30:24.971818 PlumedToHTML-0.8/setup.cfg
--rw-r--r--   0 gareth     (505) staff       (20)      761 2022-07-14 09:28:58.000000 PlumedToHTML-0.8/setup.py
+drwxr-xr-x   0 gareth     (505) staff       (20)        0 2022-07-14 14:19:10.498727 PlumedToHTML-0.9/
+-rw-r--r--   0 gareth     (505) staff       (20)     3550 2022-07-14 14:19:10.498349 PlumedToHTML-0.9/PKG-INFO
+drwxr-xr-x   0 gareth     (505) staff       (20)        0 2022-07-14 14:19:10.496028 PlumedToHTML-0.9/PlumedToHTML/
+-rw-r--r--   0 gareth     (505) staff       (20)    14459 2022-07-14 14:06:03.000000 PlumedToHTML-0.9/PlumedToHTML/PlumedFormatter.py
+-rw-r--r--   0 gareth     (505) staff       (20)     2912 2022-07-14 12:08:30.000000 PlumedToHTML-0.9/PlumedToHTML/PlumedLexer.py
+-rw-r--r--   0 gareth     (505) staff       (20)    15751 2022-07-14 12:08:45.000000 PlumedToHTML-0.9/PlumedToHTML/PlumedToHTML.py
+-rw-r--r--   0 gareth     (505) staff       (20)       84 2022-07-13 15:52:22.000000 PlumedToHTML-0.9/PlumedToHTML/__init__.py
+drwxr-xr-x   0 gareth     (505) staff       (20)        0 2022-07-14 14:19:10.497851 PlumedToHTML-0.9/PlumedToHTML.egg-info/
+-rw-r--r--   0 gareth     (505) staff       (20)     3550 2022-07-14 14:19:10.000000 PlumedToHTML-0.9/PlumedToHTML.egg-info/PKG-INFO
+-rw-r--r--   0 gareth     (505) staff       (20)      311 2022-07-14 14:19:10.000000 PlumedToHTML-0.9/PlumedToHTML.egg-info/SOURCES.txt
+-rw-r--r--   0 gareth     (505) staff       (20)        1 2022-07-14 14:19:10.000000 PlumedToHTML-0.9/PlumedToHTML.egg-info/dependency_links.txt
+-rw-r--r--   0 gareth     (505) staff       (20)        9 2022-07-14 14:19:10.000000 PlumedToHTML-0.9/PlumedToHTML.egg-info/requires.txt
+-rw-r--r--   0 gareth     (505) staff       (20)       13 2022-07-14 14:19:10.000000 PlumedToHTML-0.9/PlumedToHTML.egg-info/top_level.txt
+-rw-r--r--   0 gareth     (505) staff       (20)     2762 2022-06-02 16:41:32.000000 PlumedToHTML-0.9/README.md
+-rw-r--r--   0 gareth     (505) staff       (20)       38 2022-07-14 14:19:10.498887 PlumedToHTML-0.9/setup.cfg
+-rw-r--r--   0 gareth     (505) staff       (20)      761 2022-07-14 14:17:42.000000 PlumedToHTML-0.9/setup.py
```

### Comparing `PlumedToHTML-0.8/PKG-INFO` & `PlumedToHTML-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlumedToHTML
-Version: 0.8
+Version: 0.9
 Summary: A package for creating pretified HTML for PLUMED files
 Home-page: https://github.com/plumed/PlumedToHTML
 Author: Gareth Tribello
 Author-email: gareth.tribello@gmail.com
 License: UNKNOWN
 Description: [![CI](https://github.com/plumed/PlumedToHTML/actions/workflows/main.yml/badge.svg)](https://github.com/plumed/PlumedToHTML/actions/workflows/main.yml)
         [![codecov](https://codecov.io/gh/plumed/PlumedToHTML/branch/main/graph/badge.svg?token=ODA9N9MEGP)](https://codecov.io/gh/plumed/PlumedToHTML)
```

### Comparing `PlumedToHTML-0.8/PlumedToHTML/PlumedFormatter.py` & `PlumedToHTML-0.9/PlumedToHTML/PlumedFormatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,23 @@
                outfile.write('<b name="' + self.egname + label + '" onclick=\'showPath("' + self.divname + '","' + self.egname + label + '")\'>' + value + '</b>')
             elif ttype==Comment :
                # Comments
                outfile.write('<span style="color:blue">' + value + '</span>' )
             elif ttype==Name.Attribute :
                # KEYWORD in KEYWORD=whatever and FLAGS
                keywords.append( value.strip() )
-               outfile.write('<div class="tooltip">' + value + '<div class="right">' + self.keyword_dict[action]["syntax"][value.strip()]["description"].split('.')[0] + '<i></i></div></div>')
+               if value.strip() in self.keyword_dict[action]["syntax"] : desc = self.keyword_dict[action]["syntax"][value.strip()]["description"].split('.')[0]
+               else :
+                  # This deals with numbered keywords
+                  foundkey=False
+                  for kkkk in self.keyword_dict[action]["syntax"] :
+                      if kkkk=="output" or self.keyword_dict[action]["syntax"][kkkk]["multiple"]==0 : continue
+                      if kkkk in value.strip() : foundkey, desc = True, self.keyword_dict[action]["syntax"][kkkk]["description"].split('.')[0]
+                  if not foundkey : raise Exception("keyword " + value.strip() + " is not in syntax for action " + action )
+               outfile.write('<div class="tooltip">' + value + '<div class="right">' + desc + '<i></i></div></div>')
             elif ttype==Name.Constant :
                # @replicas in special replica syntax
                outfile.write('<div class="tooltip">' + value + '<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="' + self.keyword_dict["replicalink"] +'">here for more details.</a><i></i></div></div>')
             elif ttype==Keyword :
                # Name of action
                action = value.strip()
                if shortcut_state==1 and default_state==1 :
```

### Comparing `PlumedToHTML-0.8/PlumedToHTML/PlumedLexer.py` & `PlumedToHTML-0.9/PlumedToHTML/PlumedLexer.py`

 * *Files identical despite different names*

### Comparing `PlumedToHTML-0.8/PlumedToHTML/PlumedToHTML.py` & `PlumedToHTML-0.9/PlumedToHTML/PlumedToHTML.py`

 * *Files identical despite different names*

### Comparing `PlumedToHTML-0.8/PlumedToHTML.egg-info/PKG-INFO` & `PlumedToHTML-0.9/PlumedToHTML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlumedToHTML
-Version: 0.8
+Version: 0.9
 Summary: A package for creating pretified HTML for PLUMED files
 Home-page: https://github.com/plumed/PlumedToHTML
 Author: Gareth Tribello
 Author-email: gareth.tribello@gmail.com
 License: UNKNOWN
 Description: [![CI](https://github.com/plumed/PlumedToHTML/actions/workflows/main.yml/badge.svg)](https://github.com/plumed/PlumedToHTML/actions/workflows/main.yml)
         [![codecov](https://codecov.io/gh/plumed/PlumedToHTML/branch/main/graph/badge.svg?token=ODA9N9MEGP)](https://codecov.io/gh/plumed/PlumedToHTML)
```

### Comparing `PlumedToHTML-0.8/README.md` & `PlumedToHTML-0.9/README.md`

 * *Files identical despite different names*

### Comparing `PlumedToHTML-0.8/setup.py` & `PlumedToHTML-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='PlumedToHTML',  
-     version='0.8',
+     version='0.9',
      author="Gareth Tribello",
      author_email="gareth.tribello@gmail.com",
      description="A package for creating pretified HTML for PLUMED files",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/plumed/PlumedToHTML",
      packages=setuptools.find_packages(),
```

