# Comparing `tmp/star-chart-spherical-projection-1.4.1.tar.gz` & `tmp/star-chart-spherical-projection-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/star-chart-spherical-projection-1.4.1.tar", last modified: Fri Jun 16 21:46:45 2023, max compression
+gzip compressed data, was "dist/star-chart-spherical-projection-1.5.0.tar", last modified: Fri Jun 30 06:30:59 2023, max compression
```

## Comparing `star-chart-spherical-projection-1.4.1.tar` & `star-chart-spherical-projection-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/
--rw-rw-r--   0 user      (1000) user      (1000)      102 2022-11-20 23:38:29.000000 star-chart-spherical-projection-1.4.1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    15187 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    12407 2023-06-15 20:36:51.000000 star-chart-spherical-projection-1.4.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1831 2023-06-16 21:45:35.000000 star-chart-spherical-projection-1.4.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.402627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/
--rw-rw-r--   0 user      (1000) user      (1000)      494 2022-12-19 08:17:40.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-20 04:40:07.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/config.ini
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/
--rw-rw-r--   0 user      (1000) user      (1000)    10908 2023-01-20 01:44:10.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/convert_lst_to_csv_data.py
--rw-rw-r--   0 user      (1000) user      (1000)     4317 2023-01-20 01:44:28.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/star_data.csv
--rw-rw-r--   0 user      (1000) user      (1000)     2513 2022-11-20 22:32:39.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/declination_r_axis.py
--rw-rw-r--   0 user      (1000) user      (1000)     8082 2023-06-15 20:36:08.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)    21909 2023-06-15 20:26:39.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/generate_star_chart.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     6842 2023-06-15 20:34:14.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/test_finalPositionOfStars.py
--rw-rw-r--   0 user      (1000) user      (1000)    12221 2023-06-15 20:13:50.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
--rw-rw-r--   0 user      (1000) user      (1000)     9126 2022-11-27 07:09:03.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/ra_dec_precession_vondrak.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.402627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    15187 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      871 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       80 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       32 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/
+-rw-rw-r--   0 user      (1000) user      (1000)      102 2022-11-20 23:38:29.000000 star-chart-spherical-projection-1.5.0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    30585 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    25948 2023-06-30 06:04:37.000000 star-chart-spherical-projection-1.5.0/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1944 2023-06-30 06:04:27.000000 star-chart-spherical-projection-1.5.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/
+-rw-rw-r--   0 user      (1000) user      (1000)      577 2023-06-29 06:41:41.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-20 04:40:07.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/config.ini
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/
+-rw-rw-r--   0 user      (1000) user      (1000)    11181 2023-06-28 21:07:57.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4355 2023-06-28 19:03:19.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/star_data.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     2513 2022-11-20 22:32:39.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/declination_r_axis.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15413 2023-06-30 05:28:45.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23976 2023-06-30 05:23:55.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/generate_star_chart.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     8339 2023-06-30 05:24:28.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_finalPositionOfStars.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13338 2023-06-30 01:22:42.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13614 2023-06-29 21:04:47.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_starClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9126 2022-11-27 07:09:03.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1605 2023-06-29 09:03:11.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/starClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    30585 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      974 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       32 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/top_level.txt
```

### Comparing `star-chart-spherical-projection-1.4.1/setup.py` & `star-chart-spherical-projection-1.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.4.1"
-DESCRIPTION="A Python package to generate an astronomy star chart based on spherical projection that corrects for distortions with stereographic projection"
+VERSION="1.5.0"
+DESCRIPTION="A Python package to generate circular astronomy star charts (past, present, and future) with spherical projection to correct for distortions with more than a hundred named stars accurate over 400,000 years with proper motion and precession of the equinoxes"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="star-chart-spherical-projection",
 	version=VERSION,
 	description=DESCRIPTION,
 	long_description=long_description_readme,
 	long_description_content_type='text/markdown',
 	url="https://github.com/cyschneck/Star-Chart-Spherical-Projection",
 	download_url="https://github.com/cyschneck/Star-Chart-Spherical-Projection/archive/refs/tags/v{0}.tar.gz".format(VERSION),
-	author="cyschneck (C. Y. Schneck)",
+	author="Cora Schneck (cyschneck)",
 	keywords=["astronomy", "python", "star charts", "precession", "proper motion", "spherical projection", "stereographic projection"],
 	license="MIT",
 	classifiers=[
 		"Development Status :: 4 - Beta",
 		"Intended Audience :: Developers",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
```

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/convert_lst_to_csv_data.py` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 import pandas as pd
+import logging
+
+## Logging set up
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+stream_handler = logging.StreamHandler()
+logger.addHandler(stream_handler)
 
 if __name__ == '__main__':
 	# stars: ["name", "RA: HH.MM.SS", Declination DD.SS, Proper Motion Speed (mas/yr), Proper Motion Angle (DD.SS), Magnitude (V, Visual)]
 	# Northern stars (+ declination)
 	aldebaran_star = ["Aldebaran", "04.35.55", 16.30, 199.3, 161.4, 0.99]
 	alderamin_star = ["Alderamin", "21.18.34", 62.35, 158.4, 71.9, 2.47]
 	algieba_star = ["Algieba", "10.19.58", 19.50, 341.2, 116.9, 2.23]
@@ -56,14 +63,15 @@
 	scheat_star = ["Scheat", "23.03.46", 28.04, 232.3, 53.9, 2.48]
 	schedar_star = ["Schedar", "00.40.30", 56.32, 58.4, 122.7, 2.25] # Alpha Cassiopeiae
 	segin_star = ["Segin", "01.54.23", 63.4, 37.3, 120.5, 3.35] # Epsilon Cassiopeiae
 	seginus_star = ["Seginus", "14.32.04", 38.18, 190.4, 322.6, 3.04]
 	sheraton_star = ["Sheratan", "01.54.38", 20.48, 148.1, 138.2, 2.66]
 	spica_star = ["Spica", "13.25.11", -11.09, 52.3, 234.1, 1.06]
 	tarazed_star = ["Tarazed", "19.46.15", 10.36, 16.3, 94.8, 2.69]
+	thuban_star = ["Thuban", "14.04.23", 64.22, 58.9, 287.0, 3.65]
 	unukalhai_star = ["Unukalhai", "15.44.16", 6.25, 141.5, 71.2, 2.63]
 	vega_star = ["Vega", "18.36.56", 38.47, 349.7, 35.1, 0.03]
 	zosma_star = ["Zosma", "11.14.06", 20.31, 193.5, 132.2, 2.56]
 
 	#Southern stars (- declination)
 	# stars: ["name", "RA: HH.MM.SS", Declination, PM Speed, PM Angle, Magnitude (V, Visual)]
 	achernar_star = ["Achernar", "01.37.42", -57.14, 95.0, 113.7, 0.54]
@@ -170,14 +178,15 @@
 								scheat_star,
 								schedar_star,
 								segin_star,
 								seginus_star,
 								sheraton_star,
 								spica_star,
 								tarazed_star,
+								thuban_star,
 								unukalhai_star,
 								vega_star,
 								zosma_star
 								]
 
 	southern_star_chart_list = [achernar_star,
 								acamar_star,
@@ -226,17 +235,17 @@
 								sirius_star,
 								suhail_star,
 								wezen_star,
 								zubeneschamali_star
 								]
 
 	star_chart_list = northern_star_chart_list + southern_star_chart_list
-	print("Total stars = {0}".format(len(star_chart_list)))
+	logger.info("Total stars = {0}".format(len(star_chart_list)))
 	for star in star_chart_list:
 		if len(star) != 6:
-			print("ERROR: MISSING A VALUE = {0}".format(star[0])) # ensure that all stars have features
+			logger.info("ERROR: MISSING A VALUE = {0}".format(star[0])) # ensure that all stars have features
 			exit()
 	header_options = ["Star Name", "Right Ascension (HH.MM.SS)", "Declination (DD.SS)", "Proper Motion Speed (mas/yr)", "Proper Motion Angle (DD.SS)", "Magnitude (V, Visual)"]
 	df = pd.DataFrame(star_chart_list, columns=header_options)
 	df = df.sort_values(by=["Star Name"])
 	print(df)
 	df.to_csv("star_data.csv", header=header_options, index=False)
```

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/star_data.csv` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/star_data.csv`

 * *Files 2% similar despite different names*

```diff
@@ -97,12 +97,13 @@
 Seginus,14.32.04,38.18,190.4,322.6,3.04
 Shaula,17.33.36,-37.06,32.0,195.5,1.63
 Sheratan,01.54.38,20.48,148.1,138.2,2.66
 Sirius,06.45.08,-16.42,1339.4,204.1,-1.44
 Spica,13.25.11,-11.09,52.3,234.1,1.06
 Suhail,09.07.59,-43.26,27.6,299.4,2.2
 Tarazed,19.46.15,10.36,16.3,94.8,2.69
+Thuban,14.04.23,64.22,58.9,287.0,3.65
 Unukalhai,15.44.16,6.25,141.5,71.2,2.63
 Vega,18.36.56,38.47,349.7,35.1,0.03
 Wezen,07.08.23,-26.23,4.5,316.7,1.84
 Zosma,11.14.06,20.31,193.5,132.2,2.56
 Zubeneschamali,15.17.00,-9.22,100.0,258.7,2.61
```

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/declination_r_axis.py` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/declination_r_axis.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/generate_star_chart.py` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/generate_star_chart.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 ## Constants
 config = configparser.ConfigParser()
 config.read(os.path.join(os.path.dirname(__file__), 'config.ini'))
 
 # Start Year (JP2000)
 j2000 = 2000 # start year of the star catalogue (jan 1 2000 via IAU)
 
-
 def getStarList(selectStars=[]):
 	# generate a star object
 	# selectStars only returns a subset of all the stars saved, empty will return all in the star_data.csv file
 	# stars: ["name", "RA: HH.MM.SS", Declination DD.SS, Proper Motion Speed (mas/yr), Proper Motion Angle (DD.SS), Magnitude (V, Visual)]
 	star_data_list = []
 	star_csv_file = os.path.join(os.path.dirname(__file__), 'data', 'star_data.csv')  # get file's directory, up one level, /data/star_data.csv
 	star_dataframe = pd.read_csv(star_csv_file)
@@ -185,54 +184,88 @@
 	# Temporary fix for vondrak plugin (will only find a smaller subsections of the stars)
 	logger.debug("INCLUDING PRECESSION VIA VONDRAK")
 	vondrak_dec, vondrak_ra = vondrakDreamalligator(star_name, star_ra, np.deg2rad(star_dec), 2000 + year_YYYY_since_2000)
 	vondrak_dec = np.rad2deg(vondrak_dec)
 	logger.debug("Precession for Star = {0}, Declination = {1}, RA = {2}".format(star_name, vondrak_dec, vondrak_ra))
 	return vondrak_dec, vondrak_ra
 
-def finalPositionOfStars(userListOfStars=[], 
+def finalPositionOfStars(builtInStars=[], 
 						yearSince2000=0,
 						isPrecessionIncluded=True,
+						userDefinedStars=[],
+						onlyDisplayUserStars=False,
 						declination_min=None,
-						declination_max=None):
+						declination_max=None,
+						save_to_csv=None):
 	# return the final position of the stars as a dictionary
 
 	star_chart_spherical_projection.errorHandling(isPlotFunction=False,
-												userListOfStars=userListOfStars,
+												builtInStars=builtInStars,
 												yearSince2000=yearSince2000,
 												isPrecessionIncluded=isPrecessionIncluded,
+												userDefinedStars=userDefinedStars,
+												onlyDisplayUserStars=onlyDisplayUserStars,
 												declination_min=declination_min,
-												declination_max=declination_max)
-	userListOfStars = [x.title() for x in userListOfStars] # convert all names to capitalized
-
+												declination_max=declination_max,
+												save_to_csv=save_to_csv)
+	if not onlyDisplayUserStars:
+		builtInStars = [x.title() for x in builtInStars] # convert all names to capitalized
+		listOfStars = getStarList(builtInStars)
+		for star_object in userDefinedStars:
+			star_row = [star_object.starName,
+						star_object.ra,
+						star_object.dec,
+						star_object.properMotionSpeed,
+						star_object.properMotionAngle,
+						star_object.magnitudeVisual]
+			listOfStars.append(star_row)
+	else:
+		listOfStars = []
+		for star_object in userDefinedStars:
+			star_row = [star_object.starName,
+						star_object.ra,
+						star_object.dec,
+						star_object.properMotionSpeed,
+						star_object.properMotionAngle,
+						star_object.magnitudeVisual]
+			listOfStars.append(star_row)
+	
 	# Set declination min values when using the generateStereographicProjection() to capture all stars if not set
 	declination_min = -90
 	declination_max = 90
 
-	x_star_labels, x_ra_values, y_dec_values, finalPositionOfStarsDict = generateStereographicProjection(starList=userListOfStars, 
+	x_star_labels, x_ra_values, y_dec_values, finalPositionOfStarsDict = generateStereographicProjection(starList=listOfStars, 
 																										northOrSouth="North", 
 																										declination_min=declination_min,
 																										yearSince2000=yearSince2000,
 																										isPrecessionIncluded=isPrecessionIncluded,
 																										maxMagnitudeFilter=None,
 																										declination_max=declination_max)
+	# Generate a .csv file with final positions of stars
+	if save_to_csv is not None:
+		header_options = ["Star Name", "Right Ascension (HH.MM.SS)", "Declination (DD.SS)"]
+		star_chart_list = []
+		for star_name, star_position in finalPositionOfStarsDict.items():
+			star_chart_list.append([star_name, star_position["RA"], star_position["Declination"]])
+		df = pd.DataFrame(star_chart_list, columns=header_options)
+		df = df.sort_values(by=["Star Name"])
+		df.to_csv(save_to_csv, header=header_options, index=False)
 	return finalPositionOfStarsDict
 
 def generateStereographicProjection(starList=None, 
 									northOrSouth=None, 
 									yearSince2000=None,
 									isPrecessionIncluded=None,
 									maxMagnitudeFilter=None,
 									declination_min=None,
 									declination_max=None):
 	# Generate sterographic projections and return declination and right ascension
 
 	# Convert Star chart from RA hours to Radians to chart
-	list_of_stars = getStarList(starList)
-	list_of_stars = convertRAhrtoRadians(list_of_stars)
+	list_of_stars = convertRAhrtoRadians(starList)
 
 	finalPositionOfStarsDict = {} # {'Star Name': {"Declination" : Declination (int), "RA": RA (str)}
 	x_star_labels = []
 	x_ra_values = []
 	y_dec_values = []
 	for star in list_of_stars:
 		if maxMagnitudeFilter is None or star[5] < maxMagnitudeFilter: # Optional: Filter out stars with a magnitude greater than maxMagnitudeFilter
@@ -288,50 +321,73 @@
 					x_star_labels.append(star[0])
 					x_ra_values.append(star_ra)
 					y_dec_values.append(dec_ruler_position)
 					logger.debug("Original: '{0}': {1} RA (degrees) and {2} Declination (degrees)".format(star[0], np.rad2deg(star[1]), star[2]))
 
 	return x_star_labels, x_ra_values, y_dec_values, finalPositionOfStarsDict
 
-def plotStereographicProjection(userListOfStars=[], 
+def plotStereographicProjection(builtInStars=[], 
 								northOrSouth=None, 
 								declination_min=None,
 								yearSince2000=0,
 								displayStarNamesLabels=True,
 								displayDeclinationNumbers=True,
 								incrementBy=10,
 								isPrecessionIncluded=True,
 								maxMagnitudeFilter=None,
+								userDefinedStars=[],
+								onlyDisplayUserStars=False,
 								showPlot=True,
 								fig_plot_title=None,
 								fig_plot_color="C0",
 								figsize_n=12,
 								figsize_dpi=100,
 								save_plot_name=None):
 
 	# Catch errors in given arguments before plotting and set default constants
 	star_chart_spherical_projection.errorHandling(isPlotFunction=True,
-												userListOfStars=userListOfStars,
+												builtInStars=builtInStars,
 												northOrSouth=northOrSouth, 
 												declination_min=declination_min,
 												yearSince2000=yearSince2000,
 												displayStarNamesLabels=displayStarNamesLabels,
 												displayDeclinationNumbers=displayDeclinationNumbers,
 												incrementBy=incrementBy, 
 												isPrecessionIncluded=isPrecessionIncluded,
 												maxMagnitudeFilter=maxMagnitudeFilter,
+												userDefinedStars=userDefinedStars,
+												onlyDisplayUserStars=onlyDisplayUserStars,
 												showPlot=showPlot,
 												fig_plot_title=fig_plot_title,
 												fig_plot_color=fig_plot_color,
 												figsize_n=figsize_n,
 												figsize_dpi=figsize_dpi,
 												save_plot_name=save_plot_name)
 	northOrSouth = northOrSouth.capitalize()
-	userListOfStars = [x.title() for x in userListOfStars] # convert all names to capitalized
-
+	if not onlyDisplayUserStars:
+		builtInStars = [x.title() for x in builtInStars] # convert all names to capitalized
+		listOfStars = getStarList(builtInStars)
+		for star_object in userDefinedStars:
+			star_row = [star_object.starName,
+						star_object.ra,
+						star_object.dec,
+						star_object.properMotionSpeed,
+						star_object.properMotionAngle,
+						star_object.magnitudeVisual]
+			listOfStars.append(star_row)
+	else:
+		listOfStars = []
+		for star_object in userDefinedStars:
+			star_row = [star_object.starName,
+						star_object.ra,
+						star_object.dec,
+						star_object.properMotionSpeed,
+						star_object.properMotionAngle,
+						star_object.magnitudeVisual]
+			listOfStars.append(star_row)
 	# plot star chart as a circular graph
 
 	# Set declination based on hemisphere selected
 	if declination_min is None:
 		if northOrSouth == "North": declination_min = int(config["declinationDefaultValues"]["northern_declination_min"])
 		if northOrSouth == "South": declination_min = int(config["declinationDefaultValues"]["southern_declination_min"])
 	if northOrSouth == "North": declination_max = int(config["declinationDefaultValues"]["northern_declination_max"])
@@ -373,18 +429,18 @@
 
 	# Display declination lines based on hemisphere
 	if northOrSouth == "North":
 		displayDeclinationMarksOnAxis(declination_values, int(config["declinationDefaultValues"]["northern_declination_min"]), int(config["declinationDefaultValues"]["northern_declination_max"]), False)
 	if northOrSouth == "South":
 		displayDeclinationMarksOnAxis(declination_values, int(config["declinationDefaultValues"]["southern_declination_min"]), int(config["declinationDefaultValues"]["southern_declination_max"]), True)
 
-	logger.info("\n{0}ern Range of Declination: {1} to {2}".format(northOrSouth, declination_min, declination_max))
+	logger.debug("\n{0}ern Range of Declination: {1} to {2}".format(northOrSouth, declination_min, declination_max))
 
 	# convert to x and y values for stars
-	x_star_labels, x_ra_values, y_dec_values, star_dict = generateStereographicProjection(starList=userListOfStars, 
+	x_star_labels, x_ra_values, y_dec_values, star_dict = generateStereographicProjection(starList=listOfStars, 
 																						northOrSouth=northOrSouth, 
 																						yearSince2000=yearSince2000,
 																						isPrecessionIncluded=isPrecessionIncluded,
 																						maxMagnitudeFilter=maxMagnitudeFilter,
 																						declination_min=declination_min,
 																						declination_max=declination_max)
```

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/test_finalPositionOfStars.py` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_finalPositionOfStars.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,29 +29,29 @@
 						(False, "<class 'bool'>")]
 
 invalid_non_num_options = [([], "<class 'list'>"),
 						("string", "<class 'str'>"),
 						(False, "<class 'bool'>")]
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_list_options)
-def test_finalPositionOfStars_userListOfStarsInvalidTypes(caplog, invalid_input, error_output):
+def test_finalPositionOfStars_builtInStarsInvalidTypes(caplog, invalid_input, error_output):
 	# Test:
 	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(userListOfStars=invalid_input)
+		scsp.finalPositionOfStars(builtInStars=invalid_input)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [userListOfStars]: Must be a list, current type = '{0}'".format(error_output)
+	assert log_record.message == "\nCRITICAL ERROR, [builtInStars]: Must be a list, current type = '{0}'".format(error_output)
 
-def test_finalPositionOfStars_userListOfStarsInvalidStar(caplog):
+def test_finalPositionOfStars_builtInStarsInvalidStar(caplog):
 	# Test:
 	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(userListOfStars=["Fake star", "VEga"])
+		scsp.finalPositionOfStars(builtInStars=["Fake star", "VEga"])
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [userListOfStars]: 'Fake Star' not a star in current list of stars, please select one of the following: ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']"
+	assert log_record.message == "\nCRITICAL ERROR, [builtInStars]: 'Fake Star' not a star in current list of stars, please select one of the following: ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']"
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
 def test_finalPositionOfStars_declinationMinInvalidTypes(caplog, invalid_input, error_output):
 	# Test:
 	with pytest.raises(SystemExit):
 		scsp.finalPositionOfStars(declination_min=invalid_input)
 	log_record = caplog.records[0]
@@ -112,7 +112,34 @@
 def test_finalPositionOfStars_isPrecessionIncludedInvalidTypes(caplog, invalid_input, error_output):
 	# Test:
 	with pytest.raises(SystemExit):
 		scsp.finalPositionOfStars(isPrecessionIncluded=invalid_input)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [isPrecessionIncluded]: Must be a bool, current type = '{0}'".format(error_output)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_finalPositionOfStars_userDefinedStarsInvalidTypes(caplog, invalid_input, error_output):
+	# Test:
+	with pytest.raises(SystemExit):
+		scsp.finalPositionOfStars(userDefinedStars=[invalid_input])
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [userDefinedStars]: {0} is not a valid newStar object (see: star_chart_spherical_projection.newStar)".format(error_output)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
+def test_finalPositionOfStars_onlyDisplayUserStarsInvalidTypes(caplog, invalid_input, error_output):
+	# Test:
+	with pytest.raises(SystemExit):
+		scsp.finalPositionOfStars(onlyDisplayUserStars=invalid_input)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [onlyDisplayUserStars]: Must be a bool, current type = '{0}'".format(error_output)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
+def test_finalPositionOfStars_saveToCsvInvalidTypes(caplog, invalid_input, error_output):
+	# Test:
+	with pytest.raises(SystemExit):
+		scsp.finalPositionOfStars(save_to_csv=invalid_input)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(error_output)
```

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/test_plotStereographicProjection.py` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_plotStereographicProjection.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 						(3.1415, "<class 'float'>"),
 						(False, "<class 'bool'>")]
 
 invalid_non_num_options = [([], "<class 'list'>"),
 						("string", "<class 'str'>"),
 						(False, "<class 'bool'>")]
 
-
 def test_plotStereographicProjection_northOrSouthInvalidOptions(caplog):
 	# Test:
 	with pytest.raises(SystemExit):
 		scsp.plotStereographicProjection(northOrSouth="Invalid")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [northOrSouth]: Hemisphere options are ['North', 'South'], current option = 'Invalid'"
@@ -47,29 +46,29 @@
 	with pytest.raises(SystemExit):
 		scsp.plotStereographicProjection(northOrSouth=invalid_input)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [northOrSouth]: Must be a str, current type = '{0}'".format(error_output)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_list_options)
-def test_plotStereographicProjection_userListOfStarsInvalidTypes(caplog, invalid_input, error_output):
+def test_plotStereographicProjection_builtInStarsInvalidTypes(caplog, invalid_input, error_output):
 	# Test:
 	with pytest.raises(SystemExit):
-		scsp.plotStereographicProjection(northOrSouth="North", userListOfStars=invalid_input)
+		scsp.plotStereographicProjection(northOrSouth="North", builtInStars=invalid_input)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [userListOfStars]: Must be a list, current type = '{0}'".format(error_output)
+	assert log_record.message == "\nCRITICAL ERROR, [builtInStars]: Must be a list, current type = '{0}'".format(error_output)
 
-def test_plotStereographicProjection_userListOfStarsInvalidStar(caplog):
+def test_plotStereographicProjection_builtInStarsInvalidStar(caplog):
 	# Test:
 	with pytest.raises(SystemExit):
-		scsp.plotStereographicProjection(northOrSouth="North", userListOfStars=["Fake star", "VEga"])
+		scsp.plotStereographicProjection(northOrSouth="North", builtInStars=["Fake star", "VEga"])
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [userListOfStars]: 'Fake Star' not a star in current list of stars, please select one of the following: ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']"
+	assert log_record.message == "\nCRITICAL ERROR, [builtInStars]: 'Fake Star' not a star in current list of stars, please select one of the following: ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']"
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
 def test_plotStereographicProjection_declinationMinInvalidTypes(caplog, invalid_input, error_output):
 	# Test:
 	with pytest.raises(SystemExit):
 		scsp.plotStereographicProjection(northOrSouth="North", declination_min=invalid_input)
 	log_record = caplog.records[0]
@@ -203,7 +202,26 @@
 def test_plotStereographicProjection_savePlotNameInvalidTypes(caplog, invalid_input, error_output):
 	# Test:
 	with pytest.raises(SystemExit):
 		scsp.plotStereographicProjection(northOrSouth="North", save_plot_name=invalid_input)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [save_plot_name]: Must be a string, current type = '{0}'".format(error_output)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_plotStereographicProjection_userDefinedStarsInvalidTypes(caplog, invalid_input, error_output):
+	# Test:
+	with pytest.raises(SystemExit):
+		scsp.plotStereographicProjection(northOrSouth="North", userDefinedStars=[invalid_input])
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [userDefinedStars]: {0} is not a valid newStar object (see: star_chart_spherical_projection.newStar)".format(error_output)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
+def test_plotStereographicProjection_onlyDisplayUserStarsInvalidTypes(caplog, invalid_input, error_output):
+	#userDefinedStars
+	# Test:
+	with pytest.raises(SystemExit):
+		scsp.plotStereographicProjection(northOrSouth="North", onlyDisplayUserStars=invalid_input)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [onlyDisplayUserStars]: Must be a bool, current type = '{0}'".format(error_output)
```

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/ra_dec_precession_vondrak.py` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/SOURCES.txt` & `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 setup.py
 star_chart_spherical_projection/__init__.py
 star_chart_spherical_projection/config.ini
 star_chart_spherical_projection/declination_r_axis.py
 star_chart_spherical_projection/error_handling.py
 star_chart_spherical_projection/generate_star_chart.py
 star_chart_spherical_projection/ra_dec_precession_vondrak.py
+star_chart_spherical_projection/starClass.py
 star_chart_spherical_projection.egg-info/PKG-INFO
 star_chart_spherical_projection.egg-info/SOURCES.txt
 star_chart_spherical_projection.egg-info/dependency_links.txt
 star_chart_spherical_projection.egg-info/requires.txt
 star_chart_spherical_projection.egg-info/top_level.txt
 star_chart_spherical_projection/data/convert_lst_to_csv_data.py
 star_chart_spherical_projection/data/star_data.csv
 star_chart_spherical_projection/pytests/test_finalPositionOfStars.py
-star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
+star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
+star_chart_spherical_projection/pytests/test_starClass.py
```

