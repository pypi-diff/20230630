# Comparing `tmp/exotic-3.0.0.zip` & `tmp/exotic-3.0.1.zip`

## zipinfo {}

```diff
@@ -1,118 +1,118 @@
-Zip file size: 6355428 bytes, number of entries: 116
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/exotic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/.github/
--rw-r--r--  2.0 unx      699 b- defN 23-Jun-13 18:15 exotic-3.0.0/AUTHORS.md
--rw-r--r--  2.0 unx     1682 b- defN 23-Jun-13 18:16 exotic-3.0.0/setup.cfg
--rw-r--r--  2.0 unx     1556 b- defN 23-Jun-13 18:15 exotic-3.0.0/.gitignore
--rwxr-xr-x  2.0 unx      265 b- defN 23-Jun-13 18:15 exotic-3.0.0/run_exotic_windows.bat
--rw-r--r--  2.0 unx      221 b- defN 23-Jun-13 18:15 exotic-3.0.0/MANIFEST.in
--rw-r--r--  2.0 unx      387 b- defN 23-Jun-13 18:15 exotic-3.0.0/pyproject.toml
--rw-r--r--  2.0 unx      191 b- defN 23-Jun-13 18:15 exotic-3.0.0/CITATION.md
--rw-r--r--  2.0 unx     3359 b- defN 23-Jun-13 18:15 exotic-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--  2.0 unx      201 b- defN 23-Jun-13 18:15 exotic-3.0.0/CONTRIBUTING.md
--rw-r--r--  2.0 unx     2149 b- defN 23-Jun-13 18:15 exotic-3.0.0/LICENSE
--rw-r--r--  2.0 unx      464 b- defN 23-Jun-13 18:15 exotic-3.0.0/requirements.txt
--rw-r--r--  2.0 unx    14575 b- defN 23-Jun-13 18:16 exotic-3.0.0/PKG-INFO
--rw-r--r--  2.0 unx     5887 b- defN 23-Jun-13 18:15 exotic-3.0.0/inits.json
--rwxr-xr-x  2.0 unx     5080 b- defN 23-Jun-13 18:15 exotic-3.0.0/run_exotic_linux.sh
--rw-r--r--  2.0 unx     1890 b- defN 23-Jun-13 18:15 exotic-3.0.0/setup.py
--rw-r--r--  2.0 unx    13141 b- defN 23-Jun-13 18:15 exotic-3.0.0/README.md
--rwxr-xr-x  2.0 unx     4756 b- defN 23-Jun-13 18:15 exotic-3.0.0/run_exotic_mac.command
--rw-r--r--  2.0 unx     4597 b- defN 23-Jun-13 18:15 exotic-3.0.0/examples/sampledata.json
--rw-r--r--  2.0 unx     3296 b- defN 23-Jun-13 18:15 exotic-3.0.0/examples/lc_fitter_unit_test.py
--rw-r--r--  2.0 unx   248480 b- defN 23-Jun-13 18:15 exotic-3.0.0/examples/Exoplanet_Watch_API.ipynb
--rw-r--r--  2.0 unx    28376 b- defN 23-Jun-13 18:15 exotic-3.0.0/examples/tess.py
--rwxr-xr-x  2.0 unx     4479 b- defN 23-Jun-13 18:15 exotic-3.0.0/examples/interactive_fitter.py
--rw-r--r--  2.0 unx   597675 b- defN 23-Jun-13 18:15 exotic-3.0.0/examples/Multiple_Lightcurve_fit.ipynb
--rw-r--r--  2.0 unx     2244 b- defN 23-Jun-13 18:15 exotic-3.0.0/examples/global_fitter_unit_test.py
--rw-r--r--  2.0 unx      483 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     3270 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx    14575 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic.egg-info/not-zip-safe
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/docs/Images/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/docs/regions/
--rw-r--r--  2.0 unx    16096 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/README.md
--rw-r--r--  2.0 unx    45485 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_initssaved.png
--rw-r--r--  2.0 unx    46133 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_inputobsinfo.png
--rw-r--r--  2.0 unx    65879 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_welcome.png
--rw-r--r--  2.0 unx   309812 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/HAT-P-32bExample.png
--rw-r--r--  2.0 unx    56356 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/Background_Estimate.png
--rw-r--r--  2.0 unx    74050 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_running.png
--rw-r--r--  2.0 unx   189180 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/posterior_sample.png
--rw-r--r--  2.0 unx   187434 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_inputobs.png
--rw-r--r--  2.0 unx    46727 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_runmode.png
--rw-r--r--  2.0 unx   197330 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_planetparams.png
--rw-r--r--  2.0 unx   340120 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/ExoplanetWatch.png
--rw-r--r--  2.0 unx   265478 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/transitsimple.jpg
--rw-r--r--  2.0 unx   617967 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/Hot_pixel_mask.png
--rw-r--r--  2.0 unx    53508 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_redmode.png
--rw-r--r--  2.0 unx    46372 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_saveinits.png
--rw-r--r--  2.0 unx    82591 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_loading.png
--rw-r--r--  2.0 unx    57777 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/exotic_inputplanetparams.png
--rw-r--r--  2.0 unx    79523 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/Images/centroids.png
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/docs/regions/English/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/docs/regions/German/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/docs/regions/Spanish (Español)/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/docs/regions/Brazilian_Portuguese/
--rw-r--r--  2.0 unx    27943 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
--rw-r--r--  2.0 unx     2673 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
--rw-r--r--  2.0 unx   229468 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/Introduction-to-Exoplanets.pdf
--rw-r--r--  2.0 unx     5902 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
--rw-r--r--  2.0 unx   243586 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/How_to_Use_GitHub.pdf
--rw-r--r--  2.0 unx    11401 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
--rw-r--r--  2.0 unx     5893 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
--rw-r--r--  2.0 unx     9236 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
--rw-r--r--  2.0 unx    86803 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
--rw-r--r--  2.0 unx   725191 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/How-EXOTIC-Works.pdf
--rw-r--r--  2.0 unx    10067 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/example_output.txt
--rw-r--r--  2.0 unx     6151 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
--rw-r--r--  2.0 unx   598255 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
--rw-r--r--  2.0 unx   180681 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
--rw-r--r--  2.0 unx      119 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/German/translators.md
--rw-r--r--  2.0 unx   223208 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
--rw-r--r--  2.0 unx   132016 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/German/Benutzung-von-GitHub.pdf
--rw-r--r--  2.0 unx    10330 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/German/Beispiel_Output.txt
--rw-r--r--  2.0 unx   155973 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
--rw-r--r--  2.0 unx   611693 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
--rw-r--r--  2.0 unx      129 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/Spanish (Español)/translators.md
--rw-r--r--  2.0 unx   112871 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
--rw-r--r--  2.0 unx      545 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/Brazilian_Portuguese/README.md
--rw-r--r--  2.0 unx    28054 b- defN 23-Jun-13 18:15 exotic-3.0.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/exotic/api/
--rw-r--r--  2.0 unx    80045 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/exotic_gui.py
--rw-r--r--  2.0 unx     9481 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/plots.py
--rw-r--r--  2.0 unx     1239 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/animate.py
--rw-r--r--  2.0 unx     4752 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/plate_status.py
--rw-r--r--  2.0 unx     3027 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/__init__.py
--rw-r--r--  2.0 unx    27708 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/inputs.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-13 18:16 exotic-3.0.0/exotic/version.py
--rw-r--r--  2.0 unx    13768 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/output_files.py
--rw-r--r--  2.0 unx    11472 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/utils.py
--rw-r--r--  2.0 unx   117815 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/exotic.py
--rw-r--r--  2.0 unx    17395 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/nea.py
--rw-r--r--  2.0 unx    18359 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/plotting.py
--rw-r--r--  2.0 unx    14696 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/output_aavso.py
--rw-r--r--  2.0 unx     2322 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/__init__.py
--rw-r--r--  2.0 unx     5592 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/ew.py
--rw-r--r--  2.0 unx    48554 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/elca.py
--rw-r--r--  2.0 unx     5981 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/ld.py
--rw-r--r--  2.0 unx     2916 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/versioning.py
--rw-r--r--  2.0 unx     4017 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/filters.py
--rw-r--r--  2.0 unx    27733 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/nested_linear_fitter.py
--rw-r--r--  2.0 unx    15060 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/colab.py
--rw-r--r--  2.0 unx     6591 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/plate_solution.py
--rw-r--r--  2.0 unx     9803 b- defN 23-Jun-13 18:15 exotic-3.0.0/exotic/api/gael_ld.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 18:15 exotic-3.0.0/tests/__init__.py
--rw-r--r--  2.0 unx    20643 b- defN 23-Jun-13 18:15 exotic-3.0.0/tests/test_utils.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 18:16 exotic-3.0.0/.github/workflows/
--rw-r--r--  2.0 unx      260 b- defN 23-Jun-13 18:15 exotic-3.0.0/.github/dependabot.yml
--rw-r--r--  2.0 unx     1073 b- defN 23-Jun-13 18:15 exotic-3.0.0/.github/workflows/python-publish.yml
-116 files, 7630399 bytes uncompressed, 6336792 bytes compressed:  17.0%
+Zip file size: 6355426 bytes, number of entries: 116
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/exotic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-30 01:34 exotic-3.0.1/CITATION.md
+-rw-r--r--  2.0 unx    13141 b- defN 23-Jun-30 01:34 exotic-3.0.1/README.md
+-rw-r--r--  2.0 unx     1682 b- defN 23-Jun-30 01:35 exotic-3.0.1/setup.cfg
+-rw-r--r--  2.0 unx     3359 b- defN 23-Jun-30 01:34 exotic-3.0.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x  2.0 unx     4756 b- defN 23-Jun-30 01:34 exotic-3.0.1/run_exotic_mac.command
+-rw-r--r--  2.0 unx      387 b- defN 23-Jun-30 01:34 exotic-3.0.1/pyproject.toml
+-rwxr-xr-x  2.0 unx     5080 b- defN 23-Jun-30 01:34 exotic-3.0.1/run_exotic_linux.sh
+-rw-r--r--  2.0 unx      699 b- defN 23-Jun-30 01:34 exotic-3.0.1/AUTHORS.md
+-rw-r--r--  2.0 unx      465 b- defN 23-Jun-30 01:34 exotic-3.0.1/requirements.txt
+-rw-r--r--  2.0 unx     5887 b- defN 23-Jun-30 01:34 exotic-3.0.1/inits.json
+-rw-r--r--  2.0 unx      221 b- defN 23-Jun-30 01:34 exotic-3.0.1/MANIFEST.in
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-30 01:34 exotic-3.0.1/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     1890 b- defN 23-Jun-30 01:34 exotic-3.0.1/setup.py
+-rw-r--r--  2.0 unx     2149 b- defN 23-Jun-30 01:34 exotic-3.0.1/LICENSE
+-rw-r--r--  2.0 unx     1556 b- defN 23-Jun-30 01:34 exotic-3.0.1/.gitignore
+-rwxr-xr-x  2.0 unx      265 b- defN 23-Jun-30 01:34 exotic-3.0.1/run_exotic_windows.bat
+-rw-r--r--  2.0 unx    14575 b- defN 23-Jun-30 01:35 exotic-3.0.1/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/exotic/api/
+-rw-r--r--  2.0 unx   117815 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/exotic.py
+-rw-r--r--  2.0 unx    11472 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/utils.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic/version.py
+-rw-r--r--  2.0 unx    13768 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/output_files.py
+-rw-r--r--  2.0 unx     3027 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/__init__.py
+-rw-r--r--  2.0 unx    80045 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/exotic_gui.py
+-rw-r--r--  2.0 unx     9481 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/plots.py
+-rw-r--r--  2.0 unx     4752 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/plate_status.py
+-rw-r--r--  2.0 unx     1239 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/animate.py
+-rw-r--r--  2.0 unx    27708 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/inputs.py
+-rw-r--r--  2.0 unx    48554 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/elca.py
+-rw-r--r--  2.0 unx    18359 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/plotting.py
+-rw-r--r--  2.0 unx     2916 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/versioning.py
+-rw-r--r--  2.0 unx     2322 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/__init__.py
+-rw-r--r--  2.0 unx    15060 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/colab.py
+-rw-r--r--  2.0 unx     9803 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/gael_ld.py
+-rw-r--r--  2.0 unx    14696 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/output_aavso.py
+-rw-r--r--  2.0 unx    17395 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/nea.py
+-rw-r--r--  2.0 unx     5981 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/ld.py
+-rw-r--r--  2.0 unx     5592 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/ew.py
+-rw-r--r--  2.0 unx     4017 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/filters.py
+-rw-r--r--  2.0 unx    27733 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/nested_linear_fitter.py
+-rw-r--r--  2.0 unx     6591 b- defN 23-Jun-30 01:34 exotic-3.0.1/exotic/api/plate_solution.py
+-rwxr-xr-x  2.0 unx     4479 b- defN 23-Jun-30 01:34 exotic-3.0.1/examples/interactive_fitter.py
+-rw-r--r--  2.0 unx     4597 b- defN 23-Jun-30 01:34 exotic-3.0.1/examples/sampledata.json
+-rw-r--r--  2.0 unx    28376 b- defN 23-Jun-30 01:34 exotic-3.0.1/examples/tess.py
+-rw-r--r--  2.0 unx     2244 b- defN 23-Jun-30 01:34 exotic-3.0.1/examples/global_fitter_unit_test.py
+-rw-r--r--  2.0 unx   248480 b- defN 23-Jun-30 01:34 exotic-3.0.1/examples/Exoplanet_Watch_API.ipynb
+-rw-r--r--  2.0 unx   597675 b- defN 23-Jun-30 01:34 exotic-3.0.1/examples/Multiple_Lightcurve_fit.ipynb
+-rw-r--r--  2.0 unx     3296 b- defN 23-Jun-30 01:34 exotic-3.0.1/examples/lc_fitter_unit_test.py
+-rw-r--r--  2.0 unx    20643 b- defN 23-Jun-30 01:34 exotic-3.0.1/tests/test_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 01:34 exotic-3.0.1/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/docs/Images/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/docs/regions/
+-rw-r--r--  2.0 unx    16096 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/README.md
+-rw-r--r--  2.0 unx    46372 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_saveinits.png
+-rw-r--r--  2.0 unx    46727 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_runmode.png
+-rw-r--r--  2.0 unx    82591 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_loading.png
+-rw-r--r--  2.0 unx   187434 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_inputobs.png
+-rw-r--r--  2.0 unx    57777 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_inputplanetparams.png
+-rw-r--r--  2.0 unx   617967 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/Hot_pixel_mask.png
+-rw-r--r--  2.0 unx    65879 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_welcome.png
+-rw-r--r--  2.0 unx    79523 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/centroids.png
+-rw-r--r--  2.0 unx    56356 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/Background_Estimate.png
+-rw-r--r--  2.0 unx    46133 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_inputobsinfo.png
+-rw-r--r--  2.0 unx   340120 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/ExoplanetWatch.png
+-rw-r--r--  2.0 unx   189180 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/posterior_sample.png
+-rw-r--r--  2.0 unx   265478 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/transitsimple.jpg
+-rw-r--r--  2.0 unx   309812 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/HAT-P-32bExample.png
+-rw-r--r--  2.0 unx    45485 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_initssaved.png
+-rw-r--r--  2.0 unx    53508 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_redmode.png
+-rw-r--r--  2.0 unx    74050 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_running.png
+-rw-r--r--  2.0 unx   197330 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/Images/exotic_planetparams.png
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/docs/regions/Spanish (Español)/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/docs/regions/English/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/docs/regions/German/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/docs/regions/Brazilian_Portuguese/
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/Spanish (Español)/translators.md
+-rw-r--r--  2.0 unx   112871 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
+-rw-r--r--  2.0 unx   725191 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/How-EXOTIC-Works.pdf
+-rw-r--r--  2.0 unx   243586 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/How_to_Use_GitHub.pdf
+-rw-r--r--  2.0 unx     9236 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
+-rw-r--r--  2.0 unx     2673 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
+-rw-r--r--  2.0 unx   598255 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
+-rw-r--r--  2.0 unx    86803 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/Getting-Started-with-EXOTIC.pdf
+-rw-r--r--  2.0 unx     5902 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
+-rw-r--r--  2.0 unx   229468 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/Introduction-to-Exoplanets.pdf
+-rw-r--r--  2.0 unx    10067 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/example_output.txt
+-rw-r--r--  2.0 unx     6151 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
+-rw-r--r--  2.0 unx    27943 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
+-rw-r--r--  2.0 unx     5893 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
+-rw-r--r--  2.0 unx    11401 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
+-rw-r--r--  2.0 unx   223208 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
+-rw-r--r--  2.0 unx   180681 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/German/translators.md
+-rw-r--r--  2.0 unx   611693 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
+-rw-r--r--  2.0 unx   132016 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/German/Benutzung-von-GitHub.pdf
+-rw-r--r--  2.0 unx    10330 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/German/Beispiel_Output.txt
+-rw-r--r--  2.0 unx   155973 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
+-rw-r--r--  2.0 unx      545 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/Brazilian_Portuguese/README.md
+-rw-r--r--  2.0 unx    28054 b- defN 23-Jun-30 01:34 exotic-3.0.1/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-30 01:35 exotic-3.0.1/.github/workflows/
+-rw-r--r--  2.0 unx      260 b- defN 23-Jun-30 01:34 exotic-3.0.1/.github/dependabot.yml
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-30 01:34 exotic-3.0.1/.github/workflows/python-publish.yml
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      483 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/requires.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/top_level.txt
+-rw-r--r--  2.0 unx    14575 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     3270 b- defN 23-Jun-30 01:35 exotic-3.0.1/exotic.egg-info/SOURCES.txt
+116 files, 7630400 bytes uncompressed, 6336790 bytes compressed:  17.0%
```

## zipnote {}

```diff
@@ -1,349 +1,349 @@
-Filename: exotic-3.0.0/
+Filename: exotic-3.0.1/
 Comment: 
 
-Filename: exotic-3.0.0/examples/
+Filename: exotic-3.0.1/exotic/
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/
+Filename: exotic-3.0.1/examples/
 Comment: 
 
-Filename: exotic-3.0.0/docs/
+Filename: exotic-3.0.1/tests/
 Comment: 
 
-Filename: exotic-3.0.0/exotic/
+Filename: exotic-3.0.1/docs/
 Comment: 
 
-Filename: exotic-3.0.0/tests/
+Filename: exotic-3.0.1/.github/
 Comment: 
 
-Filename: exotic-3.0.0/.github/
+Filename: exotic-3.0.1/exotic.egg-info/
 Comment: 
 
-Filename: exotic-3.0.0/AUTHORS.md
+Filename: exotic-3.0.1/CITATION.md
 Comment: 
 
-Filename: exotic-3.0.0/setup.cfg
+Filename: exotic-3.0.1/README.md
 Comment: 
 
-Filename: exotic-3.0.0/.gitignore
+Filename: exotic-3.0.1/setup.cfg
 Comment: 
 
-Filename: exotic-3.0.0/run_exotic_windows.bat
+Filename: exotic-3.0.1/CODE_OF_CONDUCT.md
 Comment: 
 
-Filename: exotic-3.0.0/MANIFEST.in
+Filename: exotic-3.0.1/run_exotic_mac.command
 Comment: 
 
-Filename: exotic-3.0.0/pyproject.toml
+Filename: exotic-3.0.1/pyproject.toml
 Comment: 
 
-Filename: exotic-3.0.0/CITATION.md
+Filename: exotic-3.0.1/run_exotic_linux.sh
 Comment: 
 
-Filename: exotic-3.0.0/CODE_OF_CONDUCT.md
+Filename: exotic-3.0.1/AUTHORS.md
 Comment: 
 
-Filename: exotic-3.0.0/CONTRIBUTING.md
+Filename: exotic-3.0.1/requirements.txt
 Comment: 
 
-Filename: exotic-3.0.0/LICENSE
+Filename: exotic-3.0.1/inits.json
 Comment: 
 
-Filename: exotic-3.0.0/requirements.txt
+Filename: exotic-3.0.1/MANIFEST.in
 Comment: 
 
-Filename: exotic-3.0.0/PKG-INFO
+Filename: exotic-3.0.1/CONTRIBUTING.md
 Comment: 
 
-Filename: exotic-3.0.0/inits.json
+Filename: exotic-3.0.1/setup.py
 Comment: 
 
-Filename: exotic-3.0.0/run_exotic_linux.sh
+Filename: exotic-3.0.1/LICENSE
 Comment: 
 
-Filename: exotic-3.0.0/setup.py
+Filename: exotic-3.0.1/.gitignore
 Comment: 
 
-Filename: exotic-3.0.0/README.md
+Filename: exotic-3.0.1/run_exotic_windows.bat
 Comment: 
 
-Filename: exotic-3.0.0/run_exotic_mac.command
+Filename: exotic-3.0.1/PKG-INFO
 Comment: 
 
-Filename: exotic-3.0.0/examples/sampledata.json
+Filename: exotic-3.0.1/exotic/api/
 Comment: 
 
-Filename: exotic-3.0.0/examples/lc_fitter_unit_test.py
+Filename: exotic-3.0.1/exotic/exotic.py
 Comment: 
 
-Filename: exotic-3.0.0/examples/Exoplanet_Watch_API.ipynb
+Filename: exotic-3.0.1/exotic/utils.py
 Comment: 
 
-Filename: exotic-3.0.0/examples/tess.py
+Filename: exotic-3.0.1/exotic/version.py
 Comment: 
 
-Filename: exotic-3.0.0/examples/interactive_fitter.py
+Filename: exotic-3.0.1/exotic/output_files.py
 Comment: 
 
-Filename: exotic-3.0.0/examples/Multiple_Lightcurve_fit.ipynb
+Filename: exotic-3.0.1/exotic/__init__.py
 Comment: 
 
-Filename: exotic-3.0.0/examples/global_fitter_unit_test.py
+Filename: exotic-3.0.1/exotic/exotic_gui.py
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/requires.txt
+Filename: exotic-3.0.1/exotic/plots.py
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/dependency_links.txt
+Filename: exotic-3.0.1/exotic/plate_status.py
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/SOURCES.txt
+Filename: exotic-3.0.1/exotic/animate.py
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/PKG-INFO
+Filename: exotic-3.0.1/exotic/inputs.py
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/entry_points.txt
+Filename: exotic-3.0.1/exotic/api/elca.py
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/top_level.txt
+Filename: exotic-3.0.1/exotic/api/plotting.py
 Comment: 
 
-Filename: exotic-3.0.0/exotic.egg-info/not-zip-safe
+Filename: exotic-3.0.1/exotic/api/versioning.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/
+Filename: exotic-3.0.1/exotic/api/__init__.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/
+Filename: exotic-3.0.1/exotic/api/colab.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/README.md
+Filename: exotic-3.0.1/exotic/api/gael_ld.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_initssaved.png
+Filename: exotic-3.0.1/exotic/api/output_aavso.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_inputobsinfo.png
+Filename: exotic-3.0.1/exotic/api/nea.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_welcome.png
+Filename: exotic-3.0.1/exotic/api/ld.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/HAT-P-32bExample.png
+Filename: exotic-3.0.1/exotic/api/ew.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/Background_Estimate.png
+Filename: exotic-3.0.1/exotic/api/filters.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_running.png
+Filename: exotic-3.0.1/exotic/api/nested_linear_fitter.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/posterior_sample.png
+Filename: exotic-3.0.1/exotic/api/plate_solution.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_inputobs.png
+Filename: exotic-3.0.1/examples/interactive_fitter.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_runmode.png
+Filename: exotic-3.0.1/examples/sampledata.json
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_planetparams.png
+Filename: exotic-3.0.1/examples/tess.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/ExoplanetWatch.png
+Filename: exotic-3.0.1/examples/global_fitter_unit_test.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/transitsimple.jpg
+Filename: exotic-3.0.1/examples/Exoplanet_Watch_API.ipynb
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/Hot_pixel_mask.png
+Filename: exotic-3.0.1/examples/Multiple_Lightcurve_fit.ipynb
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_redmode.png
+Filename: exotic-3.0.1/examples/lc_fitter_unit_test.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_saveinits.png
+Filename: exotic-3.0.1/tests/test_utils.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_loading.png
+Filename: exotic-3.0.1/tests/__init__.py
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/exotic_inputplanetparams.png
+Filename: exotic-3.0.1/docs/Images/
 Comment: 
 
-Filename: exotic-3.0.0/docs/Images/centroids.png
+Filename: exotic-3.0.1/docs/regions/
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/
+Filename: exotic-3.0.1/docs/README.md
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/
+Filename: exotic-3.0.1/docs/Images/exotic_saveinits.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/Spanish (Espa#U00f1ol)/
+Filename: exotic-3.0.1/docs/Images/exotic_runmode.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/Brazilian_Portuguese/
+Filename: exotic-3.0.1/docs/Images/exotic_loading.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
+Filename: exotic-3.0.1/docs/Images/exotic_inputobs.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
+Filename: exotic-3.0.1/docs/Images/exotic_inputplanetparams.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/Introduction-to-Exoplanets.pdf
+Filename: exotic-3.0.1/docs/Images/Hot_pixel_mask.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
+Filename: exotic-3.0.1/docs/Images/exotic_welcome.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/How_to_Use_GitHub.pdf
+Filename: exotic-3.0.1/docs/Images/centroids.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
+Filename: exotic-3.0.1/docs/Images/Background_Estimate.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
+Filename: exotic-3.0.1/docs/Images/exotic_inputobsinfo.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
+Filename: exotic-3.0.1/docs/Images/ExoplanetWatch.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
+Filename: exotic-3.0.1/docs/Images/posterior_sample.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/How-EXOTIC-Works.pdf
+Filename: exotic-3.0.1/docs/Images/transitsimple.jpg
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/example_output.txt
+Filename: exotic-3.0.1/docs/Images/HAT-P-32bExample.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
+Filename: exotic-3.0.1/docs/Images/exotic_initssaved.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
+Filename: exotic-3.0.1/docs/Images/exotic_redmode.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
+Filename: exotic-3.0.1/docs/Images/exotic_running.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/translators.md
+Filename: exotic-3.0.1/docs/Images/exotic_planetparams.png
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
+Filename: exotic-3.0.1/docs/regions/Spanish (Espa#U00f1ol)/
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/Benutzung-von-GitHub.pdf
+Filename: exotic-3.0.1/docs/regions/English/
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/Beispiel_Output.txt
+Filename: exotic-3.0.1/docs/regions/German/
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
+Filename: exotic-3.0.1/docs/regions/Brazilian_Portuguese/
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
+Filename: exotic-3.0.1/docs/regions/Spanish (Espa#U00f1ol)/translators.md
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/Spanish (Espa#U00f1ol)/translators.md
+Filename: exotic-3.0.1/docs/regions/Spanish (Espa#U00f1ol)/Introducci#U00f3n a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/Spanish (Espa#U00f1ol)/Introducci#U00f3n a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
+Filename: exotic-3.0.1/docs/regions/English/How-EXOTIC-Works.pdf
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/Brazilian_Portuguese/README.md
+Filename: exotic-3.0.1/docs/regions/English/How_to_Use_GitHub.pdf
 Comment: 
 
-Filename: exotic-3.0.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
+Filename: exotic-3.0.1/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/
+Filename: exotic-3.0.1/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
 Comment: 
 
-Filename: exotic-3.0.0/exotic/exotic_gui.py
+Filename: exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/plots.py
+Filename: exotic-3.0.1/docs/regions/English/Getting-Started-with-EXOTIC.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/animate.py
+Filename: exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
 Comment: 
 
-Filename: exotic-3.0.0/exotic/plate_status.py
+Filename: exotic-3.0.1/docs/regions/English/Introduction-to-Exoplanets.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/__init__.py
+Filename: exotic-3.0.1/docs/regions/English/example_output.txt
 Comment: 
 
-Filename: exotic-3.0.0/exotic/inputs.py
+Filename: exotic-3.0.1/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
 Comment: 
 
-Filename: exotic-3.0.0/exotic/version.py
+Filename: exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/output_files.py
+Filename: exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
 Comment: 
 
-Filename: exotic-3.0.0/exotic/utils.py
+Filename: exotic-3.0.1/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
 Comment: 
 
-Filename: exotic-3.0.0/exotic/exotic.py
+Filename: exotic-3.0.1/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/nea.py
+Filename: exotic-3.0.1/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/plotting.py
+Filename: exotic-3.0.1/docs/regions/German/translators.md
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/output_aavso.py
+Filename: exotic-3.0.1/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/__init__.py
+Filename: exotic-3.0.1/docs/regions/German/Benutzung-von-GitHub.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/ew.py
+Filename: exotic-3.0.1/docs/regions/German/Beispiel_Output.txt
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/elca.py
+Filename: exotic-3.0.1/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/ld.py
+Filename: exotic-3.0.1/docs/regions/Brazilian_Portuguese/README.md
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/versioning.py
+Filename: exotic-3.0.1/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/filters.py
+Filename: exotic-3.0.1/.github/workflows/
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/nested_linear_fitter.py
+Filename: exotic-3.0.1/.github/dependabot.yml
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/colab.py
+Filename: exotic-3.0.1/.github/workflows/python-publish.yml
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/plate_solution.py
+Filename: exotic-3.0.1/exotic.egg-info/not-zip-safe
 Comment: 
 
-Filename: exotic-3.0.0/exotic/api/gael_ld.py
+Filename: exotic-3.0.1/exotic.egg-info/entry_points.txt
 Comment: 
 
-Filename: exotic-3.0.0/tests/__init__.py
+Filename: exotic-3.0.1/exotic.egg-info/dependency_links.txt
 Comment: 
 
-Filename: exotic-3.0.0/tests/test_utils.py
+Filename: exotic-3.0.1/exotic.egg-info/requires.txt
 Comment: 
 
-Filename: exotic-3.0.0/.github/workflows/
+Filename: exotic-3.0.1/exotic.egg-info/top_level.txt
 Comment: 
 
-Filename: exotic-3.0.0/.github/dependabot.yml
+Filename: exotic-3.0.1/exotic.egg-info/PKG-INFO
 Comment: 
 
-Filename: exotic-3.0.0/.github/workflows/python-publish.yml
+Filename: exotic-3.0.1/exotic.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `exotic-3.0.0/AUTHORS.md` & `exotic-3.0.1/AUTHORS.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/setup.cfg` & `exotic-3.0.1/setup.cfg`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/.gitignore` & `exotic-3.0.1/.gitignore`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/CODE_OF_CONDUCT.md` & `exotic-3.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/LICENSE` & `exotic-3.0.1/LICENSE`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/PKG-INFO` & `exotic-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotic
-Version: 3.0.0
+Version: 3.0.1
 Summary: EXOTIC: EXOplanet Transit Interpretation Code
 Home-page: https://github.com/rzellem/EXOTIC
 Download-URL: https://github.com/rzellem/EXOTIC/releases/latest
 Author: Exoplanet Watch at NASA JPL
 Author-email: exoplanetwatch@jpl.nasa.gov
 License: Proprietary -- Copyright (c) 2019-present, California Institute of Technology.
 Project-URL: Documentation, https://github.com/rzellem/EXOTIC/wiki
```

## Comparing `exotic-3.0.0/inits.json` & `exotic-3.0.1/inits.json`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/run_exotic_linux.sh` & `exotic-3.0.1/run_exotic_linux.sh`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/setup.py` & `exotic-3.0.1/setup.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/README.md` & `exotic-3.0.1/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/run_exotic_mac.command` & `exotic-3.0.1/run_exotic_mac.command`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/examples/sampledata.json` & `exotic-3.0.1/examples/sampledata.json`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/examples/lc_fitter_unit_test.py` & `exotic-3.0.1/examples/lc_fitter_unit_test.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/examples/Exoplanet_Watch_API.ipynb` & `exotic-3.0.1/examples/Exoplanet_Watch_API.ipynb`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/examples/tess.py` & `exotic-3.0.1/examples/tess.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/examples/interactive_fitter.py` & `exotic-3.0.1/examples/interactive_fitter.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/examples/Multiple_Lightcurve_fit.ipynb` & `exotic-3.0.1/examples/Multiple_Lightcurve_fit.ipynb`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/examples/global_fitter_unit_test.py` & `exotic-3.0.1/examples/global_fitter_unit_test.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic.egg-info/SOURCES.txt` & `exotic-3.0.1/exotic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic.egg-info/PKG-INFO` & `exotic-3.0.1/exotic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotic
-Version: 3.0.0
+Version: 3.0.1
 Summary: EXOTIC: EXOplanet Transit Interpretation Code
 Home-page: https://github.com/rzellem/EXOTIC
 Download-URL: https://github.com/rzellem/EXOTIC/releases/latest
 Author: Exoplanet Watch at NASA JPL
 Author-email: exoplanetwatch@jpl.nasa.gov
 License: Proprietary -- Copyright (c) 2019-present, California Institute of Technology.
 Project-URL: Documentation, https://github.com/rzellem/EXOTIC/wiki
```

## Comparing `exotic-3.0.0/docs/README.md` & `exotic-3.0.1/docs/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_initssaved.png` & `exotic-3.0.1/docs/Images/exotic_initssaved.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_inputobsinfo.png` & `exotic-3.0.1/docs/Images/exotic_inputobsinfo.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_welcome.png` & `exotic-3.0.1/docs/Images/exotic_welcome.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/HAT-P-32bExample.png` & `exotic-3.0.1/docs/Images/HAT-P-32bExample.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/Background_Estimate.png` & `exotic-3.0.1/docs/Images/Background_Estimate.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_running.png` & `exotic-3.0.1/docs/Images/exotic_running.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/posterior_sample.png` & `exotic-3.0.1/docs/Images/posterior_sample.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_inputobs.png` & `exotic-3.0.1/docs/Images/exotic_inputobs.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_runmode.png` & `exotic-3.0.1/docs/Images/exotic_runmode.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_planetparams.png` & `exotic-3.0.1/docs/Images/exotic_planetparams.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/ExoplanetWatch.png` & `exotic-3.0.1/docs/Images/ExoplanetWatch.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/transitsimple.jpg` & `exotic-3.0.1/docs/Images/transitsimple.jpg`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/Hot_pixel_mask.png` & `exotic-3.0.1/docs/Images/Hot_pixel_mask.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_redmode.png` & `exotic-3.0.1/docs/Images/exotic_redmode.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_saveinits.png` & `exotic-3.0.1/docs/Images/exotic_saveinits.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_loading.png` & `exotic-3.0.1/docs/Images/exotic_loading.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/exotic_inputplanetparams.png` & `exotic-3.0.1/docs/Images/exotic_inputplanetparams.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/Images/centroids.png` & `exotic-3.0.1/docs/Images/centroids.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf` & `exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt` & `exotic-3.0.1/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/Introduction-to-Exoplanets.pdf` & `exotic-3.0.1/docs/regions/English/Introduction-to-Exoplanets.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md` & `exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/How_to_Use_GitHub.pdf` & `exotic-3.0.1/docs/regions/English/How_to_Use_GitHub.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md` & `exotic-3.0.1/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md` & `exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md` & `exotic-3.0.1/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf` & `exotic-3.0.1/docs/regions/English/Getting-Started-with-EXOTIC.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/How-EXOTIC-Works.pdf` & `exotic-3.0.1/docs/regions/English/How-EXOTIC-Works.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/example_output.txt` & `exotic-3.0.1/docs/regions/English/example_output.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md` & `exotic-3.0.1/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf` & `exotic-3.0.1/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf` & `exotic-3.0.1/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf` & `exotic-3.0.1/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/German/Benutzung-von-GitHub.pdf` & `exotic-3.0.1/docs/regions/German/Benutzung-von-GitHub.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/German/Beispiel_Output.txt` & `exotic-3.0.1/docs/regions/German/Beispiel_Output.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf` & `exotic-3.0.1/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf` & `exotic-3.0.1/docs/regions/German/Wie-EXOTIC-funktioniert.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx` & `exotic-3.0.1/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/Brazilian_Portuguese/README.md` & `exotic-3.0.1/docs/regions/Brazilian_Portuguese/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf` & `exotic-3.0.1/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/exotic_gui.py` & `exotic-3.0.1/exotic/exotic_gui.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/plots.py` & `exotic-3.0.1/exotic/plots.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/animate.py` & `exotic-3.0.1/exotic/animate.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/plate_status.py` & `exotic-3.0.1/exotic/plate_status.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/__init__.py` & `exotic-3.0.1/exotic/__init__.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/inputs.py` & `exotic-3.0.1/exotic/inputs.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/output_files.py` & `exotic-3.0.1/exotic/output_files.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/utils.py` & `exotic-3.0.1/exotic/utils.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/exotic.py` & `exotic-3.0.1/exotic/exotic.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/nea.py` & `exotic-3.0.1/exotic/api/nea.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/plotting.py` & `exotic-3.0.1/exotic/api/plotting.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/output_aavso.py` & `exotic-3.0.1/exotic/api/output_aavso.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/__init__.py` & `exotic-3.0.1/exotic/api/__init__.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/ew.py` & `exotic-3.0.1/exotic/api/ew.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/elca.py` & `exotic-3.0.1/exotic/api/elca.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/ld.py` & `exotic-3.0.1/exotic/api/ld.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/versioning.py` & `exotic-3.0.1/exotic/api/versioning.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/filters.py` & `exotic-3.0.1/exotic/api/filters.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/nested_linear_fitter.py` & `exotic-3.0.1/exotic/api/nested_linear_fitter.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/colab.py` & `exotic-3.0.1/exotic/api/colab.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/plate_solution.py` & `exotic-3.0.1/exotic/api/plate_solution.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/exotic/api/gael_ld.py` & `exotic-3.0.1/exotic/api/gael_ld.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/tests/test_utils.py` & `exotic-3.0.1/tests/test_utils.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.0/.github/workflows/python-publish.yml` & `exotic-3.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

