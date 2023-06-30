# Comparing `tmp/dragonfly-grasshopper-1.8.4.tar.gz` & `tmp/dragonfly-grasshopper-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dragonfly-grasshopper-1.8.4.tar", last modified: Thu Jun  4 21:44:22 2020, max compression
+gzip compressed data, was "dist/dragonfly-grasshopper-1.9.0.tar", last modified: Fri Jun  5 17:35:00 2020, max compression
```

## Comparing `dragonfly-grasshopper-1.8.4.tar` & `dragonfly-grasshopper-1.9.0.tar`

### file list

```diff
@@ -1,121 +1,123 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/samples/
--rw-rw-r--   0 travis    (2000) travis    (2000)   601777 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/from_building_solids.gh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/samples/alt_weather_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/alt_weather_data/paris_station_data.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)  2654881 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/alt_weather_data/paris_heat_wave.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   610379 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/load_sharing_example.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)   425398 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/from_building_footprints.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)   986799 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/peak_load_example.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)   135518 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/rooms_to_stories_to_building.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)    47536 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/samples/alternative_weather.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2617 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/pass_tests.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2020-06-04 21:44:21.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-04 21:44:21.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-06-04 21:44:21.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5560 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5833 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Model.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5260 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Repeating Window Ratio Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3622 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Vizualize Wireframe.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3462 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Luminous Efficacy.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5603 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Reassign Energy Properties.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6863 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Building from Solid.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5511 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Apply Facade Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5861 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Dump Objects.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5326 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Construct Design Day.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4377 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Simple Window Ratio Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4631 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Write DDY.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5188 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Story.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4603 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Intersect Room2Ds.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4857 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Write EPW.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6772 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Model To geoJSON.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4346 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Single Window Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5896 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Model To Honeybee.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5610 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Run URBANopt.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6225 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Room2D.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5073 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Solve Adjacency.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5355 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Louver Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Overhang Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     7828 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Installer.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4426 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Import NOAA Staion Location.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6848 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Create EPW.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4463 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Set Ground Top.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6044 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Building from Footprint.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4649 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Vizualize All.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4491 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Separate Top Bottom.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4688 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Deconstruct All Object.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4425 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Deconstruct Object.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5728 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Repeating Window Width Height Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3817 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Horizontal Infrared.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4146 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Vizualize Quick.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4420 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF ContextShade.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     7575 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Import NOAA File.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5220 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Load Objects.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3865 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Extruded Border Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3853 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF String to Object.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3918 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Object to String.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Deconstruct Model.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5765 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Building from Stories.ghuser
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 21:44:22.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Deconstruct All Object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3569 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Repeating Window Width Height Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Set Ground Top.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8051 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Create EPW.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4526 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Apply Facade Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7990 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Building from Solid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6679 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Building from Footprint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF String to Object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1371 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Extruded Border Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1561 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Object to String.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2859 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Vizualize All.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1689 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Separate Top Bottom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Vizualize Quick.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4444 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Building from Stories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Simple Window Ratio Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4150 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Story.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6011 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Room2D.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Deconstruct Model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5811 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Run URBANopt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3852 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Model To Honeybee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3689 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Dump Objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Intersect Room2Ds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2180 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4034 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Load Objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1594 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Luminous Efficacy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1930 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Write DDY.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3483 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Import NOAA Staion Location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2115 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Single Window Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1852 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Horizontal Infrared.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Overhang Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4180 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Reassign Energy Properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17076 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Installer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3934 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF ContextShade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5326 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Model To geoJSON.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2885 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Vizualize Wireframe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2055 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Write EPW.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4459 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Repeating Window Ratio Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9225 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Import NOAA File.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3600 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Louver Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Solve Adjacency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3033 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Construct Design Day.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2962 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Deconstruct Object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      343 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     9404 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/installer.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      868 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-06-04 21:43:39.000000 dragonfly-grasshopper-1.8.4/deploy.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       62 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/samples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   601777 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/from_building_solids.gh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/samples/alt_weather_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      449 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/alt_weather_data/paris_station_data.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2654881 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/alt_weather_data/paris_heat_wave.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   610379 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/load_sharing_example.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)   425398 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/from_building_footprints.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)   986799 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/peak_load_example.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)   135518 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/rooms_to_stories_to_building.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47536 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/samples/alternative_weather.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2617 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/pass_tests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5677 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5833 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Model.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5260 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Repeating Window Ratio Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3622 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Vizualize Wireframe.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3462 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Luminous Efficacy.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5603 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Reassign Energy Properties.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6863 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Building from Solid.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5511 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Apply Facade Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4474 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Geometry Properties.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5861 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Dump Objects.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5326 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Construct Design Day.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4377 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Simple Window Ratio Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4631 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Write DDY.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5188 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Story.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4603 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Intersect Room2Ds.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4857 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Write EPW.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6772 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Model To geoJSON.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4346 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Single Window Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5896 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Model To Honeybee.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5610 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Run URBANopt.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6225 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Room2D.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5073 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Solve Adjacency.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5355 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Louver Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Overhang Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7828 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Installer.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4426 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Import NOAA Staion Location.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6848 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Create EPW.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4463 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Set Ground Top.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6044 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Building from Footprint.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4649 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Vizualize All.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4491 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Separate Top Bottom.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4688 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Deconstruct All Object.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4425 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Deconstruct Object.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5728 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Repeating Window Width Height Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3817 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Horizontal Infrared.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4146 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Vizualize Quick.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)       42 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4420 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF ContextShade.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7575 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Import NOAA File.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5220 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Load Objects.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3865 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Extruded Border Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3853 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF String to Object.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3918 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Object to String.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Deconstruct Model.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5765 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Building from Stories.ghuser
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-05 17:35:00.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Deconstruct All Object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3569 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Repeating Window Width Height Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Set Ground Top.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8051 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Create EPW.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4526 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Apply Facade Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7990 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Building from Solid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6679 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Building from Footprint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF String to Object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1371 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Extruded Border Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1561 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Object to String.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2859 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Vizualize All.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1689 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Separate Top Bottom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Vizualize Quick.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4444 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Building from Stories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Simple Window Ratio Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4150 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Story.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6011 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Room2D.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Deconstruct Model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5811 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Run URBANopt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3852 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Model To Honeybee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3689 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Dump Objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Intersect Room2Ds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2180 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4034 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Load Objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1594 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Luminous Efficacy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1930 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Write DDY.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3483 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Import NOAA Staion Location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2115 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Single Window Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1852 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Horizontal Infrared.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Overhang Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4180 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Reassign Energy Properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17076 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Installer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3934 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF ContextShade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5326 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Model To geoJSON.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2885 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Vizualize Wireframe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2055 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Write EPW.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Geometry Properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4459 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Repeating Window Ratio Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9225 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Import NOAA File.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3600 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Louver Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Solve Adjacency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3033 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Construct Design Day.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2962 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Deconstruct Object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      343 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9404 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/installer.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/dev-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      868 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-06-05 17:34:15.000000 dragonfly-grasshopper-1.9.0/deploy.sh
```

### Comparing `dragonfly-grasshopper-1.8.4/samples/from_building_solids.gh` & `dragonfly-grasshopper-1.9.0/samples/from_building_solids.gh`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/samples/alt_weather_data/paris_heat_wave.txt` & `dragonfly-grasshopper-1.9.0/samples/alt_weather_data/paris_heat_wave.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/samples/load_sharing_example.gh` & `dragonfly-grasshopper-1.9.0/samples/load_sharing_example.gh`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/samples/from_building_footprints.gh` & `dragonfly-grasshopper-1.9.0/samples/from_building_footprints.gh`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/samples/peak_load_example.gh` & `dragonfly-grasshopper-1.9.0/samples/peak_load_example.gh`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/samples/rooms_to_stories_to_building.gh` & `dragonfly-grasshopper-1.9.0/samples/rooms_to_stories_to_building.gh`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/samples/alternative_weather.gh` & `dragonfly-grasshopper-1.9.0/samples/alternative_weather.gh`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/PKG-INFO` & `dragonfly-grasshopper-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-grasshopper
-Version: 1.8.4
+Version: 1.9.0
 Summary: Dragonfly plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/dragonfly-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/dragonfly-grasshopper.svg?branch=master)](https://travis-ci.org/ladybug-tools/dragonfly-grasshopper)
```

### Comparing `dragonfly-grasshopper-1.8.4/README.md` & `dragonfly-grasshopper-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper.egg-info/PKG-INFO` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-grasshopper
-Version: 1.8.4
+Version: 1.9.0
 Summary: Dragonfly plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/dragonfly-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/dragonfly-grasshopper.svg?branch=master)](https://travis-ci.org/ladybug-tools/dragonfly-grasshopper)
```

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper.egg-info/SOURCES.txt` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 dragonfly_grasshopper/src/DF ContextShade.py
 dragonfly_grasshopper/src/DF Create EPW.py
 dragonfly_grasshopper/src/DF Deconstruct All Object.py
 dragonfly_grasshopper/src/DF Deconstruct Model.py
 dragonfly_grasshopper/src/DF Deconstruct Object.py
 dragonfly_grasshopper/src/DF Dump Objects.py
 dragonfly_grasshopper/src/DF Extruded Border Parameters.py
+dragonfly_grasshopper/src/DF Geometry Properties.py
 dragonfly_grasshopper/src/DF Horizontal Infrared.py
 dragonfly_grasshopper/src/DF Import NOAA File.py
 dragonfly_grasshopper/src/DF Import NOAA Staion Location.py
 dragonfly_grasshopper/src/DF Installer.py
 dragonfly_grasshopper/src/DF Intersect Room2Ds.py
 dragonfly_grasshopper/src/DF Load Objects.py
 dragonfly_grasshopper/src/DF Louver Parameters.py
@@ -68,14 +69,15 @@
 dragonfly_grasshopper/user_objects/DF ContextShade.ghuser
 dragonfly_grasshopper/user_objects/DF Create EPW.ghuser
 dragonfly_grasshopper/user_objects/DF Deconstruct All Object.ghuser
 dragonfly_grasshopper/user_objects/DF Deconstruct Model.ghuser
 dragonfly_grasshopper/user_objects/DF Deconstruct Object.ghuser
 dragonfly_grasshopper/user_objects/DF Dump Objects.ghuser
 dragonfly_grasshopper/user_objects/DF Extruded Border Parameters.ghuser
+dragonfly_grasshopper/user_objects/DF Geometry Properties.ghuser
 dragonfly_grasshopper/user_objects/DF Horizontal Infrared.ghuser
 dragonfly_grasshopper/user_objects/DF Import NOAA File.ghuser
 dragonfly_grasshopper/user_objects/DF Import NOAA Staion Location.ghuser
 dragonfly_grasshopper/user_objects/DF Installer.ghuser
 dragonfly_grasshopper/user_objects/DF Intersect Room2Ds.ghuser
 dragonfly_grasshopper/user_objects/DF Load Objects.ghuser
 dragonfly_grasshopper/user_objects/DF Louver Parameters.ghuser
```

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Model.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Model.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Repeating Window Ratio Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Repeating Window Ratio Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Vizualize Wireframe.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Vizualize Wireframe.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Luminous Efficacy.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Luminous Efficacy.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Reassign Energy Properties.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Reassign Energy Properties.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Building from Solid.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Building from Solid.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Apply Facade Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Apply Facade Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Dump Objects.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Dump Objects.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Construct Design Day.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Construct Design Day.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Simple Window Ratio Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Simple Window Ratio Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Write DDY.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Write DDY.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Story.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Story.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Intersect Room2Ds.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Intersect Room2Ds.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Write EPW.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Write EPW.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Model To geoJSON.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Model To geoJSON.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Single Window Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Single Window Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Model To Honeybee.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Model To Honeybee.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Run URBANopt.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Run URBANopt.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Room2D.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Room2D.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Solve Adjacency.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Solve Adjacency.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Louver Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Louver Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Overhang Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Overhang Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Installer.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Installer.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Import NOAA Staion Location.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Import NOAA Staion Location.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Create EPW.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Create EPW.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Set Ground Top.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Set Ground Top.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Building from Footprint.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Building from Footprint.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Vizualize All.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Vizualize All.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Separate Top Bottom.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Separate Top Bottom.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Deconstruct All Object.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Deconstruct All Object.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Deconstruct Object.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Deconstruct Object.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Repeating Window Width Height Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Repeating Window Width Height Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Horizontal Infrared.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Horizontal Infrared.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Vizualize Quick.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Vizualize Quick.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF ContextShade.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF ContextShade.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Import NOAA File.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Import NOAA File.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Load Objects.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Load Objects.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Extruded Border Parameters.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Extruded Border Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF String to Object.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF String to Object.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Object to String.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Object to String.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Deconstruct Model.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Deconstruct Model.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/user_objects/DF Building from Stories.ghuser` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/user_objects/DF Building from Stories.ghuser`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Deconstruct All Object.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Deconstruct All Object.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Repeating Window Width Height Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Repeating Window Width Height Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Set Ground Top.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Set Ground Top.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Create EPW.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Create EPW.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Apply Facade Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Apply Facade Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Building from Solid.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Building from Solid.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Building from Footprint.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Building from Footprint.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF String to Object.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF String to Object.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Extruded Border Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Extruded Border Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Object to String.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Object to String.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Vizualize All.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Vizualize All.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Separate Top Bottom.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Separate Top Bottom.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Vizualize Quick.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Vizualize Quick.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Building from Stories.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Building from Stories.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Simple Window Ratio Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Simple Window Ratio Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Story.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Story.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Room2D.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Room2D.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Deconstruct Model.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Deconstruct Model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Run URBANopt.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Run URBANopt.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Model To Honeybee.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Model To Honeybee.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Dump Objects.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Dump Objects.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Intersect Room2Ds.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Intersect Room2Ds.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Model.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Load Objects.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Load Objects.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Luminous Efficacy.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Luminous Efficacy.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Write DDY.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Write DDY.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Import NOAA Staion Location.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Import NOAA Staion Location.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Single Window Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Single Window Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Horizontal Infrared.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Horizontal Infrared.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Overhang Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Overhang Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Reassign Energy Properties.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Reassign Energy Properties.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Installer.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Installer.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF ContextShade.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF ContextShade.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Model To geoJSON.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Model To geoJSON.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Vizualize Wireframe.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Vizualize Wireframe.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Write EPW.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Write EPW.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Repeating Window Ratio Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Repeating Window Ratio Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Import NOAA File.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Import NOAA File.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Louver Parameters.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Louver Parameters.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Solve Adjacency.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Solve Adjacency.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Construct Design Day.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Construct Design Day.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/dragonfly_grasshopper/src/DF Deconstruct Object.py` & `dragonfly-grasshopper-1.9.0/dragonfly_grasshopper/src/DF Deconstruct Object.py`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/LICENSE` & `dragonfly-grasshopper-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/installer.gh` & `dragonfly-grasshopper-1.9.0/installer.gh`

 * *Files identical despite different names*

### Comparing `dragonfly-grasshopper-1.8.4/setup.py` & `dragonfly-grasshopper-1.9.0/setup.py`

 * *Files identical despite different names*

