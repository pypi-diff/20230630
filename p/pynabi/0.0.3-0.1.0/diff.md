# Comparing `tmp/pynabi-0.0.3.tar.gz` & `tmp/pynabi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\feder\Documents\Scuola\Univerit\340\prova finale 3\nasello\dist\.tmp-5cxhgavu\pynabi-0.0.3.tar", last modified: Wed Jun 14 17:06:01 2023, max compression
+gzip compressed data, was "C:\Users\feder\Documents\Scuola\Univerit\340\prova finale 3\nasello\dist\.tmp-80jw1a2k\pynabi-0.1.0.tar", last modified: Fri Jun 30 17:24:02 2023, max compression
```

## Comparing `pynabi-0.0.3.tar` & `pynabi-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:06:01.595493 pynabi-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-06-14 17:02:50.000000 pynabi-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     7069 2023-06-14 17:06:01.594495 pynabi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5413 2023-05-30 08:28:03.000000 pynabi-0.0.3/README.md
--rw-rw-rw-   0        0        0      510 2023-06-14 17:04:27.000000 pynabi-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 17:06:01.595493 pynabi-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 17:06:01.541637 pynabi-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 17:06:01.587513 pynabi-0.0.3/src/pynabi/
--rw-rw-rw-   0        0        0       47 2023-05-31 21:25:56.000000 pynabi-0.0.3/src/pynabi/__init__.py
--rw-rw-rw-   0        0        0     3711 2023-06-08 11:07:13.000000 pynabi-0.0.3/src/pynabi/_common.py
--rw-rw-rw-   0        0        0     8715 2023-06-08 11:07:51.000000 pynabi-0.0.3/src/pynabi/_dataset.py
--rw-rw-rw-   0        0        0     2950 2023-06-14 16:26:15.000000 pynabi-0.0.3/src/pynabi/calculation.py
--rw-rw-rw-   0        0        0      724 2023-05-27 14:24:27.000000 pynabi-0.0.3/src/pynabi/characteristics.py
--rw-rw-rw-   0        0        0     9106 2023-06-06 18:19:45.000000 pynabi-0.0.3/src/pynabi/crystal.py
--rw-rw-rw-   0        0        0     6449 2023-05-28 13:14:41.000000 pynabi-0.0.3/src/pynabi/kspace.py
--rw-rw-rw-   0        0        0     6279 2023-06-08 10:32:34.000000 pynabi-0.0.3/src/pynabi/occupation.py
--rw-rw-rw-   0        0        0    15225 2023-06-14 16:52:50.000000 pynabi-0.0.3/src/pynabi/relaxation.py
--rw-rw-rw-   0        0        0     3398 2023-06-14 16:27:17.000000 pynabi-0.0.3/src/pynabi/units.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:06:01.593498 pynabi-0.0.3/src/pynabi.egg-info/
--rw-rw-rw-   0        0        0     7069 2023-06-14 17:06:01.000000 pynabi-0.0.3/src/pynabi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-14 17:06:01.000000 pynabi-0.0.3/src/pynabi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:06:01.000000 pynabi-0.0.3/src/pynabi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 17:06:01.000000 pynabi-0.0.3/src/pynabi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.782640 pynabi-0.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 17:22:45.000000 pynabi-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8279 2023-06-30 17:24:02.781646 pynabi-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5996 2023-06-30 17:07:24.000000 pynabi-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1084 2023-06-30 17:08:50.000000 pynabi-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 17:24:02.782640 pynabi-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.734703 pynabi-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.773633 pynabi-0.1.0/src/pynabi/
+-rw-rw-rw-   0        0        0       47 2023-06-30 16:56:26.000000 pynabi-0.1.0/src/pynabi/__init__.py
+-rw-rw-rw-   0        0        0     6041 2023-06-30 17:18:11.000000 pynabi-0.1.0/src/pynabi/_common.py
+-rw-rw-rw-   0        0        0     8903 2023-06-25 12:06:13.000000 pynabi-0.1.0/src/pynabi/_dataset.py
+-rw-rw-rw-   0        0        0     4204 2023-06-17 21:06:56.000000 pynabi-0.1.0/src/pynabi/calculation.py
+-rw-rw-rw-   0        0        0     9529 2023-06-17 21:28:04.000000 pynabi-0.1.0/src/pynabi/crystal.py
+-rw-rw-rw-   0        0        0    11672 2023-06-30 17:18:06.000000 pynabi-0.1.0/src/pynabi/kspace.py
+-rw-rw-rw-   0        0        0     7844 2023-06-21 21:36:17.000000 pynabi-0.1.0/src/pynabi/occupation.py
+-rw-rw-rw-   0        0        0    14540 2023-06-17 19:55:26.000000 pynabi-0.1.0/src/pynabi/relaxation.py
+-rw-rw-rw-   0        0        0     3727 2023-06-17 21:24:10.000000 pynabi-0.1.0/src/pynabi/units.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.779621 pynabi-0.1.0/src/pynabi.egg-info/
+-rw-rw-rw-   0        0        0     8279 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/top_level.txt
```

### Comparing `pynabi-0.0.3/LICENSE` & `pynabi-0.1.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 Federico Guglielmi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pynabi-0.0.3/PKG-INFO` & `pynabi-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pynabi
-Version: 0.0.3
+Version: 0.1.0
 Summary: A package to easily create Abinit input files
 Author: Federico Guglielmi
 License: MIT License
         
-        Copyright (c) [year] [fullname]
+        Copyright (c) 2023 Federico Guglielmi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -20,93 +20,111 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Project-URL: Homepage, https://github.com/Fedesky25/pynabi
+Project-URL: Bug Tracker, https://github.com/Fedesky25/pynabi/issues
+Project-URL: Documentation, https://github.com/Fedesky25/pynabi/wiki
+Project-URL: Repository, https://github.com/Fedesky25/pynabi.git
+Project-URL: Changelog, https://github.com/Fedesky25/pynabi/blob/master/CHANGELOG.md
 Keywords: abinit
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PynAbi
 
 Python package to easily create [Abinit](https://www.abinit.org/) input files.
 
+```cmd
+pip install pynabi==0.0.3
+```
+
 ## Example
 
 ```python
-from pynabi import createAbi, DataSet, AbIn, AbOut, Occupation
-from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, path, UsualKShifts
+from pynabi import createAbi, DataSet, AbIn, AbOut
+from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
 from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
 from pynabi.crystal import Atom, FluoriteLike
-from pynabi.units import EUnit
+from pynabi.occupation import OccupationPerBand
+from pynabi.units import eV, nm
 
 # create manually an atom -> Atom(<Z>, <pseudo potential name>)
 # or using sensible defaults as follows
 Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
 Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
 
 # base dataset with common variables
 base = DataSet(
-    AbOut("./scf/scf"),                             # prefixes for output files
+    AbOut("./scf/scf"),                             # prefix for output files
     AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
-    FluoriteLike(Zr, Oxy, 5.14),                    # creates AtomBasis and Lattice of a crystal like fluorite
+
+    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
+                                                    # with lattice constant 0.5135nm
+
     SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
         .ofMonkhorstPack(4),
-    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density based on the last 10 iteration
+
+    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
+                                                    # based on the last 10 iteration
+
     ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
     MaxSteps(30)                                    # nstep
 )
 
 # set the default energy unit in eV (from now on)
-EUnit.eV.setAsDefault()
+eV.setAsReference()
 
 # datasets to see the convergenge as a function of energy
-sets = [DataSet(EnergyCutoff.of(8.0 + i*0.25)) for i in range(0,17)]
+sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
 
 # final non-self-consistent round to find bands 
 bands = DataSet(
     NonSelfConsistentCalc(),
     ToleranceOn.WavefunctionSquaredResidual(1e-12),
-    AbIn().ElectronDensity(sets[-1]),               # get the electron density from the last dataset
-    Occupation.EqualBandNumber(2.0, 8),             # same number of bands (max 8) for each k point
-    path(10, "GXWKGLUWLK", CriticalPointsOf.FCC)    # easily define a path in the k-space   
+    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
+    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
+    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
 )
 
 with open("./out.txt", 'w') as f:
     f.write(createAbi(base, *sets, bands))
 ```
 
 <details>
 <summary><b>Output</b></summary>
 
 ```txt
 ndtset 18
 
 # Atoms definition
 ntypat 2
-znucl 40 8
-pseudos "Zr.psp8, O.psp8"
+znucl 8 40
+pseudos "O.psp8, Zr.psp8"
 
 # Common DataSet
 natoms 3
-typeat 1 2 2
+typeat 2 1 1
 xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
 outdata_prefix "./scf/scf"
 pp_dirpath "./pseudos/PBE-SR"
-scalecart 5.14 5.14 5.14
+scalecart 0.5135 0.5135 0.5135 nm
 rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
-kptopt 1
-nshiftk 4
-shiftk 0.5 0.5 0.5   0.5 0.0 0.0   0.0 0.5 0.0   0.0 0.0 0.5
 ngkpt 4 4 4
 iscf 17
 npulayit 10
 toldfe 1e-06
 nstep 30
 
 # DataSet 1
@@ -161,32 +179,33 @@
 ecut17 12.0 eV
 
 # DataSet 18
 iscf18 -2
 tolwfr18 1e-12
 getden18 17
 occopt18 0
-nbands18 8
 occ18 8*2.0
+bands18 8
 kptopt18 -9
-kptbounds18 0 0 0   0.0 0.5 0.5   0.25 0.75 0.5   0.375 0.75 0.375   0 0 0   0.5 0.5 0.5   0.25 0.625 0.625   0.25 0.75 0.5   0.5 0.5 0.5   0.375 0.75 0.375
+kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
 ndivsm18 10
 ```
 
 </details>
 
 ## Features
 
  - Multi dataset support
  - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
  - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
  - Smooth experience in defining the k-points
  - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
  - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
  - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
+ - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
  - _More to come..._
 
 ## Why PynAbi over pure Abinit files?
 
 If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
 For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
 
@@ -196,8 +215,8 @@
  4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
  5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
 
 Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
 
 ## Documentation
 
-_coming soon_
+Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation.
```

### Comparing `pynabi-0.0.3/README.md` & `pynabi-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,86 @@
 # PynAbi
 
 Python package to easily create [Abinit](https://www.abinit.org/) input files.
 
+```cmd
+pip install pynabi==0.0.3
+```
+
 ## Example
 
 ```python
-from pynabi import createAbi, DataSet, AbIn, AbOut, Occupation
-from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, path, UsualKShifts
+from pynabi import createAbi, DataSet, AbIn, AbOut
+from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
 from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
 from pynabi.crystal import Atom, FluoriteLike
-from pynabi.units import EUnit
+from pynabi.occupation import OccupationPerBand
+from pynabi.units import eV, nm
 
 # create manually an atom -> Atom(<Z>, <pseudo potential name>)
 # or using sensible defaults as follows
 Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
 Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
 
 # base dataset with common variables
 base = DataSet(
-    AbOut("./scf/scf"),                             # prefixes for output files
+    AbOut("./scf/scf"),                             # prefix for output files
     AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
-    FluoriteLike(Zr, Oxy, 5.14),                    # creates AtomBasis and Lattice of a crystal like fluorite
+
+    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
+                                                    # with lattice constant 0.5135nm
+
     SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
         .ofMonkhorstPack(4),
-    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density based on the last 10 iteration
+
+    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
+                                                    # based on the last 10 iteration
+
     ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
     MaxSteps(30)                                    # nstep
 )
 
 # set the default energy unit in eV (from now on)
-EUnit.eV.setAsDefault()
+eV.setAsReference()
 
 # datasets to see the convergenge as a function of energy
-sets = [DataSet(EnergyCutoff.of(8.0 + i*0.25)) for i in range(0,17)]
+sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
 
 # final non-self-consistent round to find bands 
 bands = DataSet(
     NonSelfConsistentCalc(),
     ToleranceOn.WavefunctionSquaredResidual(1e-12),
-    AbIn().ElectronDensity(sets[-1]),               # get the electron density from the last dataset
-    Occupation.EqualBandNumber(2.0, 8),             # same number of bands (max 8) for each k point
-    path(10, "GXWKGLUWLK", CriticalPointsOf.FCC)    # easily define a path in the k-space   
+    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
+    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
+    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
 )
 
 with open("./out.txt", 'w') as f:
     f.write(createAbi(base, *sets, bands))
 ```
 
 <details>
 <summary><b>Output</b></summary>
 
 ```txt
 ndtset 18
 
 # Atoms definition
 ntypat 2
-znucl 40 8
-pseudos "Zr.psp8, O.psp8"
+znucl 8 40
+pseudos "O.psp8, Zr.psp8"
 
 # Common DataSet
 natoms 3
-typeat 1 2 2
+typeat 2 1 1
 xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
 outdata_prefix "./scf/scf"
 pp_dirpath "./pseudos/PBE-SR"
-scalecart 5.14 5.14 5.14
+scalecart 0.5135 0.5135 0.5135 nm
 rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
-kptopt 1
-nshiftk 4
-shiftk 0.5 0.5 0.5   0.5 0.0 0.0   0.0 0.5 0.0   0.0 0.0 0.5
 ngkpt 4 4 4
 iscf 17
 npulayit 10
 toldfe 1e-06
 nstep 30
 
 # DataSet 1
@@ -127,32 +135,33 @@
 ecut17 12.0 eV
 
 # DataSet 18
 iscf18 -2
 tolwfr18 1e-12
 getden18 17
 occopt18 0
-nbands18 8
 occ18 8*2.0
+bands18 8
 kptopt18 -9
-kptbounds18 0 0 0   0.0 0.5 0.5   0.25 0.75 0.5   0.375 0.75 0.375   0 0 0   0.5 0.5 0.5   0.25 0.625 0.625   0.25 0.75 0.5   0.5 0.5 0.5   0.375 0.75 0.375
+kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
 ndivsm18 10
 ```
 
 </details>
 
 ## Features
 
  - Multi dataset support
  - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
  - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
  - Smooth experience in defining the k-points
  - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
  - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
  - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
+ - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
  - _More to come..._
 
 ## Why PynAbi over pure Abinit files?
 
 If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
 For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
 
@@ -162,8 +171,8 @@
  4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
  5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
 
 Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
 
 ## Documentation
 
-_coming soon_
+Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation.
```

### Comparing `pynabi-0.0.3/src/pynabi/_common.py` & `pynabi-0.1.0/src/pynabi/_common.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import TypeVar, Type, Tuple, Callable
+from typing import TypeVar, Type, Tuple, Callable, Any, TypeGuard
 
 
-__all__ = ["Vec3D", "SKO"]
+__all__ = ["Vec3D"]
 
 
 class Singleton(object):
     _instance = None
     def __new__(cls):
         if cls._instance is None:
             cls._instance = object.__new__(cls)
@@ -75,58 +75,81 @@
         return f"{t.name}{self.suffix}{index or ''} {self.value}"
 
 
 class Later(Singleton):
     pass
 
 
+class DelayedInfo:
+    def __init__(self, prop: str, name: str) -> None:
+        self.prop = prop
+        self.name = name
+
+    def sanitize(self, value):
+        raise NotImplementedError()
+    
+    def laterOrSanitized(self, value):
+        return value if value is Later._instance else self.sanitize(value)
+    
+    def stamp(self, suffix, value):
+        return f"{self.prop}{suffix} {value}"
+    
+    @staticmethod
+    def basic(fn: Callable[[Any],bool], msg: str):
+        class Child(DelayedInfo):
+            def sanitize(self, value):
+                assert fn(value), f"{self.name} {msg}"
+                return value
+        return Child
+
+
 class CanDelay(Stampable): 
-    _delayables: Tuple[Tuple[str, str, Callable],...] = ()
+    _delayables: Tuple[DelayedInfo,...] = ()
 
     def __init__(self, *values):
-        self._dv = values;
-        for i,v in enumerate(values):
-            if v is not Later._instance:
-                self._delayables[i][2](v)
+        self._dv = tuple(self._delayables[i].laterOrSanitized(v) for i,v in enumerate(values))
 
     def _doesDelay(self, i: int):
         return self._dv[i] is Later._instance
     
     def stamp(self, index: int):
         res: list[str] = []
         s = index or ''
         for i,v in enumerate(self._dv):
             if v is not Later._instance:
-                res.append(f"{self._delayables[i][0]}{s} {v}")
+                res.append(self._delayables[i].stamp(s,v))
         return '\n'.join(res)
+    
+    info = DelayedInfo # for ease of access
 
 
 class Delayed(Stampable):
     def __init__(self, cls: Type[CanDelay], index: int, value) -> None:
-        super().__init__() 
-        cls._delayables[index][2](value)
+        super().__init__()
         self.c = cls
         self.i = index
-        self.v = value
+        self.d = cls._delayables[index]
+        self.v = self.d.sanitize(value)
     
     def compatible(self, coll: StampCollection):
         v = coll.get(self.c)
         if v is None:
-            raise TypeError(f"{self.getName()} definition requires {self.c.__name__} definition before")
-        if not v._doesDelay(self.i):
-            raise ValueError(f"{self.c.__name__} already defines {self.getName()}")
+            raise TypeError(f"{self.d.name} definition requires {self.c.__name__} definition before")
+        if not v._doesDelay(self.i) and coll.nextto(self.c):
+            raise ValueError(f"{self.c.__name__} already defines {self.d.name} in the same dataset")
     
     def stamp(self, index: int):
-        return f"{self.getProp()}{index or ''} {self.v}"
+        return self.d.stamp(index or '', self.v)
 
-    def getProp(self):
-        return self.c._delayables[self.i][0]
 
-    def getName(self):
-        return self.c._delayables[self.i][1]
+def delayer(index: int, T: Type, use: Type[Delayed] = Delayed):
+    @classmethod
+    def fn(cls, value: T):
+        return use(cls, index, value)
+    return fn
 
 
 class SKO:
     """Single K Occupation"""
     def __init__(self, k: Vec3D, *occupations: float) -> None:
         self.k = k
         self.occ = occupations
@@ -134,10 +157,58 @@
 
 def sectionTitle(index: int, name: str):
     if index > 0:
         return f"\n# DS{index} - {name}"
     else:
         return f"\n# {name}"
     
+
+def decorate_IWD_method(fn):
+    def method(self: 'IndexedWithDefault', *args):
+        assert self._index is None, f"Multiple definitions for {type(self).__name__}"
+        return fn(self, *args)
+    return method
+
+
+class IndexedWithDefault(Stampable):
+    _default: str = ""
+    _prop: str = ""
     
-def _pos_int(v):
-    return type(v) is int and v > 0
+    def __init__(self) -> None:
+        super().__init__()
+        self._index: int|None = None
+        self._extra: dict[str, Any] = {}
+    
+    def __init_subclass__(cls, default: str, prop: str = "") -> None:
+        super().__init_subclass__()
+        cls._prop = prop
+        if not callable(getattr(cls, default, 0)): # 0 is not callable
+            raise AttributeError(f"Property {default} of {cls.__name__} is not callable")
+        for (name,method) in cls.__dict__.items():
+            if callable(method) and not hasattr(IndexedWithDefault, name):
+                setattr(cls, name, decorate_IWD_method(method))
+    
+    def stamp(self, index: int):
+        s = index or ''
+        if self._index is None:
+            getattr(self,self._default)()
+        res = f"{self._prop}{s} {self._index}"
+        extra = '\n'.join(f"{k}{s} {v}" for (k,v) in self._extra.items())
+        if len(extra) > 0:
+            res += '\n' + extra
+        return res
+
+
+def _pos_int(v) -> TypeGuard[int]:
+    return type(v) is int and v > 0
+
+
+def _pos0_int(v) -> TypeGuard[int]:
+    return type(v) is int and v >= 0
+
+
+def _pos_num(v) -> TypeGuard[float|int]:
+    return type(v) is float or type(v) is int and v > 0
+
+
+def _pos0_num(v) -> TypeGuard[float|int]:
+    return type(v) is float or type(v) is int and v >= 0
```

### Comparing `pynabi-0.0.3/src/pynabi/_dataset.py` & `pynabi-0.1.0/src/pynabi/_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Union, List, Iterable, Literal, Callable, Optional, Type
 from ._common import Stampable, Singleton, Delayed, StampCollection
 from .crystal import AtomBasis, Atom
 from inspect import stack
 
 from .occupation import _exclusives as _ex1
 from .calculation import _exclusives as _ex2
+from .kspace import _exclusives as _ex3
 
-_excl = [_ex1, _ex2]
+_excl = [_ex1, _ex2, _ex3]
 
 
 __all__ = ["DataSet", "PreviousRun", "AbIn", "AbOut", "createAbi"]
 
 
 _RS = Union[Stampable,Iterable['_RS']]
 
@@ -33,17 +34,17 @@
         self.stamps: list[Stampable] = []
         self.map: dict[Type[Stampable], Stampable] = {}
         delayed_props = set()
         for s in splat(stampables):
             if not isinstance(s, Stampable):
                 raise TypeError(f"{s.__class__.__name__} is not a valid type for a dataset")
             if isinstance(s, Delayed):
-                p = s.getProp()
+                p = s.d.prop
                 if p in delayed_props:
-                    raise ValueError(f"Multiple {s.getName()} definition are present")
+                    raise ValueError(f"Multiple {s.d.name} definition are present")
                 delayed_props.add(p)
                 self.stamps.append(s)
             else:
                 t = type(s)
                 if t in self.map:
                     raise ValueError(f"Multiple {s.__class__.__name__} given")
                 self.map[t] = s
@@ -205,15 +206,16 @@
     ExchangeCorrelationPotential = _os("vxc")
     UseWanTInterface = _om("want", 3)
     Wavefunction = _om("wf", 2, -1)
     FullMeshWavefunction = _os("wf_full")
     XML = _os("xml")
 
 
-def createAbi(setup: Union[DataSet,None], *datasets: DataSet):
+def createAbi(setup: Union[DataSet,None], *datasets: DataSet) -> str:
+    """Given one optional base dataset and multiple subsequent datasets, it constructs the abinit input file and returns it as a string"""
     n = len(datasets)
     if setup is None:
         if n == 0:
             return ''
         elif n == 1:
             return createAbi(datasets[0])
         else:
```

### Comparing `pynabi-0.0.3/src/pynabi/crystal.py` & `pynabi-0.1.0/src/pynabi/crystal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from ._common import Vec3D as _V, Stampable as _S
+from ._common import Vec3D as _V, Stampable as _S, _pos_int
 from typing import Optional as _O, Union as _U
 from .units import Length as _L, Pos3D as _P
 
 __all__ = ["Atom", "AtomBasis", "Lattice", "HCP", "CsClLike", "RockSaltLike", "FluoriteLike", "ZincBlendeLike", "HCP", "WurtziteLike", "NiAsLike"]
 
 _atom_symbols = ["H","He","Li","Be","B","C","N","O","F","Ne","Na","Mg","Al","Si","P","S","Cl","Ar","K","Ca","Sc","Ti","V","Cr","Mn","Fe","Co","Ni","Cu","Zn","Ga","Ge","As","Se","Br","Kr","Rb","Sr","Y","Zr","Nb","Mo","Tc","Ru","Rh","Pd","Ag","Cd","In","Sn","Sb","Te","I","Xe","Cs","Ba","La","Ce","Pr","Nd","Pm","Sm","Eu","Gd","Tb","Dy","Ho","Er","Tm","Yb","Lu","Hf","Ta","W","Re","Os","Ir","Pt","Au","Hg","Tl","Pb","Bi","Po","At","Rn","Fr","Ra","Ac","Th","Pa","U ","Np","Pu","Am","Cm","Bk","Cf","Es","F","Md","No","Lr","Rf","Db","Sg","Bh","Hs","Mt","Ds","Rg","Cn","Nh","Fl","Mc","Lv","Ts","Og"]
 
 class Atom:
     def __init__(self, Z: int, file: str):
+        assert _pos_int(Z), "Atomic number must be a positive integer"
         self.num = Z
         self.file = file
         assert self.file.find(",") == -1, "File name cannot contain ','"
     
     def __str__(self) -> str:
         return f"{_atom_symbols[self.num-1]} atom (located at {self.file})"
     
     # def __eq__(self, __value: object) -> bool:
     #     return (self is __value) or (type(__value) is Atom and __value.num == self.num and __value.file == self.file)
 
     @staticmethod
     def of(name: str):
         """Constructs an atom using default filenaming
         
-        returns Atom(Z of element, element name + 'psp8')
+        returns Atom(Z of element, element name + '.psp8')
         """
         try:
             Z = _atom_symbols.index(name) + 1;
             return Atom(Z, name + '.psp8')
         except:
             raise ValueError(name + " is not a valid atom type")
     
@@ -36,14 +37,16 @@
 ntypat {len(atoms)}
 znucl {' '.join(str(a.num) for a in atoms)}
 pseudos \"{', '.join(a.file for a in atoms)}\""""
 
 
 class AtomBasis(_S):
     def __init__(self, *atoms: 'tuple[Atom,_V]', cartesian: bool = False) -> None:
+        """Construct an atom basis given a sequence of tuples containing an atom and a position (Vec3D)\n
+        If `cartesian` is True, the coordinates of the atoms' position are cartesian instead of reduced."""
         assert len(atoms) > 0, "There must be at least one atom in basis"
         self.atoms = atoms
         self.cartesian = cartesian
     
     def add(self, atom: Atom, where: _V):
         if type(self.atoms) is tuple:
             self.atoms = list(self.atoms)
@@ -58,14 +61,15 @@
         x_type = "xcart" if self.cartesian else "xred";
         return f"""natoms{suffix} {len(indexes)}
 typeat{suffix} {' '.join(str(i+1) for i in indexes)}
 {x_type}{suffix} {'   '.join(str(a[1]) for a in self.atoms)}"""
 
     @staticmethod
     def ofOne(atom: Atom):
+        """Construct an atom basis with only one atom (placed at Vec3D(0,0,0))"""
         return AtomBasis((atom, _V.zero()))
 
 
 def _2uni(v: _U[float,_L]):
     t = type(v)
     if t is _L:
         return _P.uniform(v) # type: ignore
@@ -93,23 +97,25 @@
         Angles are defined between vectors as follows:
         | angle | from | to |
         | :---: | :----------: | :-----------: |
         | &alpha;(1) | b(2) | c(3) |
         | &beta;(2) | a(1) | c(3) |
         | &gamma;(3) | a(1) | b(2) |
         """
-        return Lattice(acell=scaling, angdeg=angles)
+        assert type(angles) is _V, "Angles must be of type Vec3D"
+        return Lattice(acell=_P.sanitize(scaling), angdeg=angles)
     
     @staticmethod
     def fromPrimitives(a: _V, b: _V, c: _V, scaling: _U[_V,_P]):
         """
         Construct lattice from primitives [a, b, c]\n
         Scaling is applied to the cartesian axis
         """
-        return Lattice(scalecart=scaling, rprim=f"{a}   {b}   {c}")
+        assert type(a) is _V and type(b) is _V and type(c) is _V, "Primitive vectors must be of type Vec3D"
+        return Lattice(scalecart=_P.sanitize(scaling), rprim=f"{a}   {b}   {c}")
     
     @staticmethod
     def CUB(a: _U[float,_L]):
         return Lattice.fromAngles(_V.uniform(90),_2uni(a))
 
     @staticmethod
     def BCC(a: _U[float,_L]):
@@ -222,14 +228,15 @@
         (atomA, _V.zero()),
         (atomB, _V.uniform(0.25))
     )
     return (b,l)
 
 
 def HCP(atomA: Atom, atomB: Atom, a: float, c: float, unit: _O[_L] = None):
+    """Hexagonal Close Packet crystal"""
     l = Lattice.HEX(a,c,unit)
     b = AtomBasis(
         (atomA, _V.zero()),
         (atomB, _V(2/3, 1/3, 0.5)),
     )
     return (b,l)
 
@@ -265,14 +272,8 @@
     l = Lattice.HEX(a,c,unit)
     b = AtomBasis(
         (Ni, _V.zero()),
         (As, _V(2/3, 1/3, 0.25)),
         (Ni, _V(0.0,0.0,0.5)),
         (As, _V(1/3, 2/3, 0.75))
     )
-    return (b,l)
-
-
-# def BCT(atomA: Atom, atomB: Atom, a: float, c: float, unit: _O[_LU] = None):
-#     l = Lattice.TET(a,c,unit)
-#     b = AtomBasis((atomA, _V.zero()),(atomB, _V.uniform(0.5)))
-#     return (b,l)
+    return (b,l)
```

### Comparing `pynabi-0.0.3/src/pynabi/occupation.py` & `pynabi-0.1.0/src/pynabi/occupation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from ._common import Stampable, StampCollection, CanDelay, Delayed, Later
+from ._common import Stampable, StampCollection, CanDelay, Delayed, Later, _pos_int, _pos0_int, DelayedInfo
 from typing import Union, Tuple, Literal, Optional
 from enum import Enum
+from .units import Energy
 
 
 __all__ = ["SpinType", "Metal", "Smearing", "Semiconductor", "TwoQuasiFermilevels", "OccupationPerBand"]
 
 
 class SpinPolarization(Stampable):
     def __init__(self, pol: Literal[1,2], inor: Literal[1,2], den: Literal[1,2,4]) -> None:
@@ -35,48 +36,66 @@
     Marzari5634 = 4
     Marzari8165 = 5
     MethfesselPaxton = 6
     Gaussian = 7
     Uniform = 8
 
 
-def _checkbands(v):
-    assert type(v) is int and v > 0, "Number of bands must be positive integer"
+_D_pos_int = DelayedInfo.basic(_pos_int, "must be a positive integer")
+_D_bands = _D_pos_int("nbands", "Number of bands")
 
-def _checktsmear(v):
-    assert type(v) is float and 0 <= v <= 1, "Smearing broadening must be a float between 0 and 1"
+
+class _D_pos_energy(DelayedInfo):
+    def sanitize(self, value):
+        e = Energy.sanitize(value)
+        assert e._v > 0, f"{self.name} must be a positive energy (or float)"
+        return e
 
 
 class Metal(CanDelay):
-    _delayables = ( 
-        ("tsmear", "Smearing broadening", _checktsmear),
-        ("nbands", "Number of bands", _checkbands)
-    )
+    """Metallic occupation of levels, using different occupation schemes. All k points have the same number of bands. The combination of a broadening and a physical temperature can be obtained by using both tsmear and tphysel."""
+
+    _delayables = ( _D_bands, _D_pos_energy("tsmear", "Smearing brodening temperature"), _D_pos_energy("tphysel", "Electrons' physical temperature"))
 
-    def __init__(self, smearing: Smearing, broadening: Union[float,Later] = Later(), bands: Union[int,Later] = Later()) -> None:
-        super().__init__(broadening, bands)
+    def __init__(self, 
+                 smearing: Smearing, 
+                 bands: Union[int,Later] = Later(), 
+                 broadening: Union[float,Energy,Later] = Later(), 
+                 ePhysicalTemp: float|Energy|Later = Later()
+                 ) -> None:
+        super().__init__(bands, broadening, ePhysicalTemp)
         self._opt = smearing.value
 
     def stamp(self, index: int):
         return f"occopt{index or ''} {self._opt}\n{super().stamp(index)}"
 
     @classmethod
-    def setBroadening(cls, value: float):
+    def setBands(cls, value: int):
         return Delayed(cls, 0, value)
-
+    
     @classmethod
-    def setBands(cls, value: int):
+    def setBroadening(cls, value: Energy|float):
         return Delayed(cls, 1, value)
     
+    @classmethod
+    def setEPhysicalTemp(cls, value: Energy|float):
+        return Delayed(cls, 2, value)
+
+    
 
 class Semiconductor(CanDelay):
-    _delayables = (("nbands", "Number of bands", _checkbands),)
+    """All k points and spins have the same number of bands. All k points have the same occupancies of bands for a given spin (but these occupancies may differ for spin up and spin down - typical for ferromagnetic insulators), and they are automatically generated by the code to give a semiconductor."""
+
+    _delayables = (_D_bands,)
 
     def __init__(self, spinMagnetizationTarget: Optional[float], bands: Union[int,Later] = Later()):
+        """If the spin is polarized (you have used SpinType.Polarized), then `spinMagnetizationTarget` is mandatory"""
         super().__init__(bands)
+        if spinMagnetizationTarget is not None and type(spinMagnetizationTarget) is not float:
+            raise TypeError("spinMagnetizationTarget must be a float or None")
         self._smt = spinMagnetizationTarget
     
     def compatible(self, coll: StampCollection):
         spin = coll.get(SpinPolarization)
         if spin is not None and spin.polarizationNumber == 2:
             assert self._smt is not None, "Semiconducotor with polarized spin must specify the spin magnetization target"
 
@@ -91,20 +110,25 @@
 
     @classmethod
     def setBands(cls, value: int):
         return Delayed(cls, 0, value)
     
 
 class TwoQuasiFermilevels(CanDelay):
-    _delayables = (("nbands", "Number of bands", _checkbands),)
+    """Fermi-Dirac occupation is enforced with two distinct quasi-Fermi levels:  See details in [Paillard2019]. At present, the number of holes and electrons should be the same. 
+    
+    Cannot be used with fixed magnetization calculation."""
+
+    _delayables = (_D_bands,)
 
     def __init__(self, carriers: int, valenceBands: int, bands: Union[int,Later] = Later()):
+        """`carriers` holes are forced in the first `valenceBands` and `carriers` electrons are forced in bands above."""
         super().__init__(bands)
-        assert type(carriers) is int and carriers > 0, "Number of carriers must be a positive integer"
-        assert type(valenceBands) is int and carriers >= 0, "Number of valenceBands must be a positive (or null) integer"
+        assert _pos_int(carriers), "Number of carriers must be a positive integer"
+        assert _pos0_int(valenceBands), "Number of valenceBands must be a positive (or null) integer"
         self._c = carriers
         self._v = valenceBands
 
     def stamp(self, index: int):
         s = index or ''
         r = f"occopt{s} 9\nivalence{s} {self._v}\nnqfd{s} {self._c}"
         d = super().stamp(index)
```

### Comparing `pynabi-0.0.3/src/pynabi/relaxation.py` & `pynabi-0.1.0/src/pynabi/relaxation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from ._common import Stampable as _S, StampCollection as _SC
+from ._common import Stampable as _S, StampCollection as _SC, _pos_num, _pos0_num, IndexedWithDefault as _IWD
 from .units import Energy as _En
-from typing import Any as _A, Literal as _L, Tuple as _T
+from typing import Literal as _L, Tuple as _T
 
 
-# TODO: missing ionmov 28
-
-
-def _pos_num(v):
-    return (type(v) is int or type(v) is float) and v >= 0
+# TODO: missing ionmov 20, 28
 
 
 # class FixedAtoms(_S):
 #     pass
 
 
 def _check_co(coll: _SC, name: str):
@@ -24,192 +20,164 @@
 
 
 def _mdtemp(v):
     assert type(v) is tuple and len(v) == 2 and _pos_num(v[0]) and _pos_num(v[1]), "Temperatures must be a tuple of to positive numbers"
     return f"[{v[0]},{v[1]}]"
 
 
-# class _MD_SO_def:
-#     def __init__(self, fn) -> None:
-#         self.fn = fn
-    
-#     def __call__(self, *args: _A, **kwds: _A) -> _A:
-#         self.fn(*args, **kwds)
-    
-#     def __set_name__(self, owner: type, name: str):
-#         setattr(owner, "_def", self.fn)
-#         setattr(owner, name, self.fn) # replace ourselves with the original method
-
-
-class _MD_SO(_S):
+class _MD_SO(_IWD, default="__init__", prop="ionmov"):
     def __init__(self, timeStep: float = 100, maxSteps: int = 1000) -> None:
         super().__init__()
         assert _pos_num(timeStep), "time step (for molecular dynamics or structural optimization) must be a positive number"
         assert type(maxSteps) is int and maxSteps > 0, "number of maximum steps (for molecular dynamics or structural optimization) must be a positive integer"
         self._dt = timeStep
         self._ms = maxSteps
-        self._n = 0
-        self._d: dict[str,_A] = {}
     
     def stamp(self, index: int):
         s = index or ''
-        r = f"ionmov{s} {self._n}"
-        extra = '\n'.join(f"{k}{s} {v}" for (k,v) in self._d.items())
-        if len(extra) > 0:
-            r += "\n" + extra
-        return r
-    
-    def compatible(self, coll: _SC):
-        assert self._n != 0, f"Incomplete definition of {type(self).__name__}"
+        return super().stamp(index) + f"\ndtion{s} {self._dt}\nntime{s} {self._ms}"
 
 
-class MolecularDynamics(_MD_SO):
+class MolecularDynamics(_MD_SO, default="basic"):
     """Move atoms using molecular dynamics"""
 
     def compatible(self, coll: _SC):
-        if self._n != 13: # isoenthaplic is the only one that accept cell optimization
+        if self._index != 13: # isoenthaplic is the only one that accept cell optimization
             _check_co(coll, "Molecular dynamics")
     
     def basic(self):
         """Move atoms using undumped molecular dynamics\n
         For viscous damping use `StructuralOptimization(...).damping(...)`"""
-        self._n = 1
-        self._d = {"vis": 0}
+        self._index = 1
+        self._extra = {"vis": 0}
         return self
 
     def Verlet(self):
         """Molecular dynamics using the Verlet algorithm, see [[Allen1987a]](https://docs.abinit.org/theory/bibliography#allen1987a) p 81"""
-        self._n = 6
-        self._d = {}
+        self._index = 6
         return self
 
     def quenchedVerlet(self):
         """Quenched Molecular dynamics using the Verlet algorithm, and stopping each atom for which the scalar product of velocity and force is negative.\n
         The goal is not to produce a realistic dynamics, but to go as fast as possible to the minimum. For this purpose, it is advised to set all the masses to the same value"""
-        self._n = 7
-        self._d = {}
+        self._index = 7
         return self
     
     def NoseHoover(self, inertia: float = 100, temperatures: _T[float, float] = (200,300)):
         """
         Molecular dynamics with Nose-Hoover thermostat, using the Verlet algorithm
         
         `inertia` is the inertia factor WT of the thermostat in atomic units (see [the docs](https://docs.abinit.org/variables/rlx/#noseinert))
 
         `temperatures` is a tuple of floats who represent the initial and final temperatures of the thermostat
         """
         assert _pos_num(inertia), "thermostat intertia must a positive number"
-        self._n = 8
-        self._d = { "mdtemp": _mdtemp(temperatures), "noseinert": inertia }
+        self._index = 8
+        self._extra = { "mdtemp": _mdtemp(temperatures), "noseinert": inertia }
         return self
 
     def Langevin(self, friction: float, temperatures: _T[float, float] = (200,300)):
         """
         Langevin molecular dynamics
 
         `friction` is friction coefficient for Langevin dynamics with units Hartree*Electronic mass*(atomic unit of Time)/Bohr^2
 
         `temperatures` is a tuple of floats who represent the initial and final temperatures of the dynamics
         """
         assert _pos_num(friction), "thermostat intertia must a positive number"
-        self._n = 9
-        self._d = { "mdtemp": _mdtemp(temperatures), "friction": friction }
+        self._index = 9
+        self._extra = { "mdtemp": _mdtemp(temperatures), "friction": friction }
         return self
     
     def isokinetic(self, temperature: float = 200):
         """
         Isokinetic ensemble molecular dynamics\n
         The velocity is initialized from the given temperature (in Kelvin)
         """
         assert _pos_num(temperature), "The temperature must be a positive number"
-        self._n = 12
-        self._d = { "mdtemp": f"[{temperature},{temperature+1}]" }
+        self._index = 12
+        self._extra = { "mdtemp": f"[{temperature},{temperature+1}]" }
         return self
 
     def SRKNa14(self):
         """Simple molecular dynamics with a symplectic algorithm proposed in [[Blanes2002]](https://docs.abinit.org/theory/bibliography#blanes2002) (called SRKNa14) of the kind first published in [[Yoshida1990]](https://docs.abinit.org/theory/bibliography#bitzek2006). This algorithm requires at least 14 evaluation of the forces (actually 15 are done within Abinit) per time step. At this cost it usually gives much better energy conservation than the verlet algorithm for a 30 times bigger value of time step.\n
         NOTE: the potential energy of the initial atomic configuration is never evaluated using this algorithm."""
-        self._n = 14
-        self._d = {}
+        self._index = 14
         return self
 
     def learnOnTheFly(self, iterations: int = 10):
         """Use of Learn on The Fly method (LOTF) for Molecular Dynamics. In the framework of isokinetic MD, the atomic forces and positions are computed by using LOTF interpolation. A SCF computation is performed only _A `iterations` steps. The results of the SCF are used to compute the parameters of a short range classical potential (for the moment only the glue potential for gold is implemented). Then these parameters are continuously tuned to compute atomic trajectories.\n
         The LOTF cycle is divided in the following steps: 
          1. Initialization (SFC at t=0) and computation of potential parameters. 
          2. Extrapolation of the atomic forces and positions for `iterations` time step. To perform this extrapolation, the potential computed in 1 is used (Verlet algorithm). 
          3. SFC at t=`iterations`. Computation of the potential parameters. 
          4. LOTF interpolation, linear interpolation of the potential parameters and computation of the atomic forces and positions between t=0 and t=`iterations`.
         
         NOTE: LOTF has to be enabled at configure time. If LOTF is not enabled, abinit will set automatically isokinetic MD.\n
          """
         assert type(iterations) is int and iterations > 0, "Number of LOTF iterations must be a positive integer"
-        self._n = 23
-        self._d = {"lotf_nitex": iterations }
+        self._index = 23
+        self._extra = {"lotf_nitex": iterations }
         return self
 
     def constantEnergy(self):
         """Simple constant energy molecular dynamics using the velocity Verlet symplectic algorithm (second order), see [[Hairer2003]](https://docs.abinit.org/theory/bibliography#hairer2003)."""
-        self._n = 24
-        self._d = {}
+        self._index = 24
         return self
 
 
-class StructuralOptimization(_MD_SO):
+class StructuralOptimization(_MD_SO, default="BFGS"):
     def compatible(self, coll: _SC):
-        if self._n not in (2, 3, 22):
+        if self._index not in (2, 3, 22):
             _check_co(coll, "Structural optimization")
 
     def damping(self, viscosity: float = 100):
         """Move atoms using molecular dynamics with viscous damping (friction linearly proportional to velocity). \n
         The implemented algorithm is the generalisation of the Numerov technique (6th order), but is NOT invariant upon time-reversal, so that the energy is not conserved."""
         assert _pos_num(viscosity), "Viscosity must be a positive number"
-        self._n = 1
-        self._d = {"vis": viscosity}
+        self._index = 1
+        self._extra = {"vis": viscosity}
         return self
 
     def BFGS(self, delocalizedCoordinates: bool = False, withEnergy: bool = False):
         """Conduct structural optimization using the Broyden-Fletcher-Goldfarb-Shanno minimization (BFGS)\n
          - `withEnergy` determines whether to take into account the total energy or not (can be very unstable)
          - `delocalizedCoordinates` detemines whether to use delocalized coordinates or not (if true, no cell optimization can be done) 
         """
         assert type(delocalizedCoordinates) is bool, "delocalizedCoordinates must be a bool"
         assert type(withEnergy) is bool, "withEnergy must be a bool"
-        self._n = 2 + 8*int(delocalizedCoordinates) + int(withEnergy)
-        self._d = {}
+        self._index = 2 + 8*int(delocalizedCoordinates) + int(withEnergy)
         return self
     
     def conjugateGradient(self):
         """Conjugate gradient algorithm for simultaneous optimization of potential and ionic degrees of freedom.\n
         WARNING: this is under development, and does not work very well in m_A cases"""
-        self._n = 4
-        self._d = {}
+        self._index = 4
         return self
 
     def simpleRelaxation(self, preconditioning: _L[-1, 0, 1, 2] = 0):
         """Simple relaxation of ionic positions according to (converged) forces\n
         `preconditioning` is an integer between -1 and 2 and describes the way a change of force is derived from a change of atomic position. 
         In particular: hessian is 2^(-preconditioning) times the identity matrix
         """
         assert type(preconditioning) is int and -1 <= preconditioning <= 2, "preconditioning must a integer between -1 and 2"
-        self._n = 5
-        self._d = { "iprcfc": preconditioning }
+        self._index = 5
+        self._extra = { "iprcfc": preconditioning }
         return self
 
     # def directInversion(self):
     #     self._n = 20
     #     self._d = {}
     #     return self
 
     def LBFGS(self):
         """Conduct structural optimization using the Limited-memory Broyden-Fletcher-Goldfarb-Shanno minimization (L-BFGS) [[Nocedal1980]](https://docs.abinit.org/theory/bibliography#nocedal1980). 
         The routines are based on the original implementation by J. Nocedal available on netlib.org. 
         This algorithm can be much better than the native implementation of BFGS in ABINIT"""
-        self._n = 22
-        self._d = {}
+        self._index = 22
         return self
 
 
 class FIRE(_S):
     """Fast inertial relaxation engine (FIRE) algorithm proposed by Erik Bitzek, Pekka Koskinen, Franz Gähler, Michael Moseler, and Peter Gumbsch in [[Bitzek2006]](https://docs.abinit.org/theory/bibliography#bitzek2006). According to the authors, the efficiency of this method is nearly the same as L-BFGS. It is based on conventional molecular dynamics with additional velocity modifications and adaptive time steps. The purpose of this algorithm is relaxation, not molecular dynamics. \n
     The initial time step is set with `initialTimeStep`: it governs the ion position changes, but the cell parameter changes as well. The suggested first guess is 0.03.\n
     The positions are in reduced coordinates instead of in cartesian coordinates."""
@@ -288,15 +256,15 @@
         s = index or ''
         return f"optcell{s} {4 + self._a + 3*int(self._k)}\necutsm{s} {self.s}"
 
 
 class MaxLatticeDilatation(_S):
     def __init__(self, additional: float = 0, exceed: bool = False) -> None:
         super().__init__()
-        assert _pos_num(additional), "Additional percentage of memory must be a positive number"
+        assert _pos0_num(additional), "Additional percentage of memory must be a positive number"
         if not exceed:
             assert additional <= 15, "Additional percentage of memory must be less than or equal to 15 (when exceed is False)"
         self.a = additional
         self.x = exceed
     
     def stamp(self, index: int):
         s = index or ''
```

### Comparing `pynabi-0.0.3/src/pynabi/units.py` & `pynabi-0.1.0/src/pynabi/units.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Union as _Un, Optional as _Op, Tuple as _Tu, Self as  _Self, Any as _Any
+from ._common import Vec3D as _V
 
 class _AbMeasure:
     _U: _Tu[_Tu[float, str],...] = ()
     _R = (1.0, 0)
 
     def __init__(self, value: float, unit: int) -> None:
         """Do not use this constructor"""
@@ -54,15 +55,15 @@
     def sanitize(cls, value: _Any) -> _Self:
         t = type(value)
         if t is float or t is int:
             return cls(value*cls._R[0], cls._R[1])
         elif t is cls:
             return value
         else:
-            raise TypeError(f"Cannot construct {cls.__name__} from {value} ({t})")
+            raise TypeError(f"Cannot construct {cls.__name__} from {value} (of type {t})")
         
     @classmethod
     def getDefaultReference(cls):
         return cls(cls._R[0], cls._R[1])
 
 
 class Length(_AbMeasure):
@@ -105,8 +106,18 @@
         self.z = z*m
     
     def __str__(self) -> str:
         return f"{self.x} {self.y} {self.z} {Length._U[self.u][1]}"
     
     @staticmethod
     def uniform(l: _Un[float,'Length']):
-        return Pos3D(1,1,1,Length.sanitize(l))
+        return Pos3D(1,1,1,Length.sanitize(l))
+    
+    @staticmethod
+    def sanitize(v: _Any) -> 'Pos3D':
+        t = type(v)
+        if t is Pos3D:
+            return v
+        elif t is _V:
+            return Pos3D(v.x,v.y,v.z)
+        else:
+            raise TypeError(f"Cannot construct Pos3D from {v} (of type {t})")
```

### Comparing `pynabi-0.0.3/src/pynabi.egg-info/PKG-INFO` & `pynabi-0.1.0/src/pynabi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pynabi
-Version: 0.0.3
+Version: 0.1.0
 Summary: A package to easily create Abinit input files
 Author: Federico Guglielmi
 License: MIT License
         
-        Copyright (c) [year] [fullname]
+        Copyright (c) 2023 Federico Guglielmi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -20,93 +20,111 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Project-URL: Homepage, https://github.com/Fedesky25/pynabi
+Project-URL: Bug Tracker, https://github.com/Fedesky25/pynabi/issues
+Project-URL: Documentation, https://github.com/Fedesky25/pynabi/wiki
+Project-URL: Repository, https://github.com/Fedesky25/pynabi.git
+Project-URL: Changelog, https://github.com/Fedesky25/pynabi/blob/master/CHANGELOG.md
 Keywords: abinit
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PynAbi
 
 Python package to easily create [Abinit](https://www.abinit.org/) input files.
 
+```cmd
+pip install pynabi==0.0.3
+```
+
 ## Example
 
 ```python
-from pynabi import createAbi, DataSet, AbIn, AbOut, Occupation
-from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, path, UsualKShifts
+from pynabi import createAbi, DataSet, AbIn, AbOut
+from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
 from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
 from pynabi.crystal import Atom, FluoriteLike
-from pynabi.units import EUnit
+from pynabi.occupation import OccupationPerBand
+from pynabi.units import eV, nm
 
 # create manually an atom -> Atom(<Z>, <pseudo potential name>)
 # or using sensible defaults as follows
 Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
 Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
 
 # base dataset with common variables
 base = DataSet(
-    AbOut("./scf/scf"),                             # prefixes for output files
+    AbOut("./scf/scf"),                             # prefix for output files
     AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
-    FluoriteLike(Zr, Oxy, 5.14),                    # creates AtomBasis and Lattice of a crystal like fluorite
+
+    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
+                                                    # with lattice constant 0.5135nm
+
     SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
         .ofMonkhorstPack(4),
-    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density based on the last 10 iteration
+
+    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
+                                                    # based on the last 10 iteration
+
     ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
     MaxSteps(30)                                    # nstep
 )
 
 # set the default energy unit in eV (from now on)
-EUnit.eV.setAsDefault()
+eV.setAsReference()
 
 # datasets to see the convergenge as a function of energy
-sets = [DataSet(EnergyCutoff.of(8.0 + i*0.25)) for i in range(0,17)]
+sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
 
 # final non-self-consistent round to find bands 
 bands = DataSet(
     NonSelfConsistentCalc(),
     ToleranceOn.WavefunctionSquaredResidual(1e-12),
-    AbIn().ElectronDensity(sets[-1]),               # get the electron density from the last dataset
-    Occupation.EqualBandNumber(2.0, 8),             # same number of bands (max 8) for each k point
-    path(10, "GXWKGLUWLK", CriticalPointsOf.FCC)    # easily define a path in the k-space   
+    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
+    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
+    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
 )
 
 with open("./out.txt", 'w') as f:
     f.write(createAbi(base, *sets, bands))
 ```
 
 <details>
 <summary><b>Output</b></summary>
 
 ```txt
 ndtset 18
 
 # Atoms definition
 ntypat 2
-znucl 40 8
-pseudos "Zr.psp8, O.psp8"
+znucl 8 40
+pseudos "O.psp8, Zr.psp8"
 
 # Common DataSet
 natoms 3
-typeat 1 2 2
+typeat 2 1 1
 xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
 outdata_prefix "./scf/scf"
 pp_dirpath "./pseudos/PBE-SR"
-scalecart 5.14 5.14 5.14
+scalecart 0.5135 0.5135 0.5135 nm
 rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
-kptopt 1
-nshiftk 4
-shiftk 0.5 0.5 0.5   0.5 0.0 0.0   0.0 0.5 0.0   0.0 0.0 0.5
 ngkpt 4 4 4
 iscf 17
 npulayit 10
 toldfe 1e-06
 nstep 30
 
 # DataSet 1
@@ -161,32 +179,33 @@
 ecut17 12.0 eV
 
 # DataSet 18
 iscf18 -2
 tolwfr18 1e-12
 getden18 17
 occopt18 0
-nbands18 8
 occ18 8*2.0
+bands18 8
 kptopt18 -9
-kptbounds18 0 0 0   0.0 0.5 0.5   0.25 0.75 0.5   0.375 0.75 0.375   0 0 0   0.5 0.5 0.5   0.25 0.625 0.625   0.25 0.75 0.5   0.5 0.5 0.5   0.375 0.75 0.375
+kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
 ndivsm18 10
 ```
 
 </details>
 
 ## Features
 
  - Multi dataset support
  - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
  - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
  - Smooth experience in defining the k-points
  - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
  - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
  - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
+ - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
  - _More to come..._
 
 ## Why PynAbi over pure Abinit files?
 
 If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
 For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
 
@@ -196,8 +215,8 @@
  4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
  5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
 
 Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
 
 ## Documentation
 
-_coming soon_
+Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation.
```

