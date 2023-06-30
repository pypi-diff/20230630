# Comparing `tmp/WebAppDIRAC-5.1.0a6.tar.gz` & `tmp/WebAppDIRAC-5.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebAppDIRAC-5.1.0a6.tar", last modified: Thu Mar 16 09:17:31 2023, max compression
+gzip compressed data, was "WebAppDIRAC-5.1.0a7.tar", last modified: Mon Jun 19 09:26:11 2023, max compression
```

## Comparing `WebAppDIRAC-5.1.0a6.tar` & `WebAppDIRAC-5.1.0a7.tar`

### file list

```diff
@@ -1,759 +1,759 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.967901 WebAppDIRAC-5.1.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-03-16 09:17:31.967901 WebAppDIRAC-5.1.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20406 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/extjs-template.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-03-16 09:17:20.000000 WebAppDIRAC-5.1.0a6/release.notes
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-16 09:17:31.967901 WebAppDIRAC-5.1.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.815891 WebAppDIRAC-5.1.0a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.831892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.831892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/App.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/CoreHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/HandlerMgr.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/StaticHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/TemplateLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.835892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/Conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/SessionData.py
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/WebHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.835892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ApplicationWizardHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/NotepadHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/PublicStateManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/RootHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/UPHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/Accounting.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Image.js
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/ApplicationWizard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/ComponentHistory.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    42537 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.839892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.843892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.843892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/Downtimes.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.843892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.843892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/ExampleApp.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.843892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    41538 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.843892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.843892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/group.png
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.gif
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.png
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_date.png
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_float.png
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_int.png
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_string.png
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/query.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/ungroup.png
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.819891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18576 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/JobLaunchpad.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    40342 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/grid.png
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/JobSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/Notepad.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    26773 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.847893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/PilotMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/grid.png
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/PilotSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/ProxyManager.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4502 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/ProxyUpload.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuModel.js
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/PublicStateManager.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    51599 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/RegistryManager.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/RequestMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/TreeModel.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.851893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/ResourceSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/SiteSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/SpaceOccupancy.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.823891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    48992 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/SystemAdministration.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/TokenManager.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/
--rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/TransformationMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.855893 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/css/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7083 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/css/css.css
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/css/iconset.css
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.859894 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.915897 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ad.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ae.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/af.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ag.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ai.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/al.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/am.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/an.gif
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ao.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ar.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/as.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/at.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/au.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/aw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ax.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/az.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ba.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bb.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bd.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/be.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bf.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bh.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bi.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bj.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bo.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/br.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bs.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bt.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bv.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/by.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ca.gif
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/catalonia.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cc.gif
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cd.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cf.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ch.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ci.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ck.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cl.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      353 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/co.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cs.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cv.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cx.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cy.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/de.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dj.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/do.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ec.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ee.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/eg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/eh.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/england.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/er.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/es.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/et.gif
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/eu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fam.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fi.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fj.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fo.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ga.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gd.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      379 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ge.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gf.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gh.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gi.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gl.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gp.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gq.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gs.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gt.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gy.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ht.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/id.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ie.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/il.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/in.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/io.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/iq.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ir.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/is.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/it.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/jm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/jo.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/jp.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ke.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kh.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ki.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/km.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kp.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ky.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/la.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lb.gif
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lc.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/li.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ls.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lt.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lv.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ly.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ma.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mc.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/md.gif
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/me.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mh.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      382 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ml.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mo.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mp.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      379 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mq.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ms.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mt.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mv.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mx.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/my.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/na.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nc.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ne.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nf.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ng.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ni.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nl.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/no.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/np.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/om.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pa.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pe.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pf.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ph.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pl.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ps.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pt.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/py.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/qa.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/re.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ro.gif
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/rs.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ru.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/rw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sa.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sb.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sc.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/scotland.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sd.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/se.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sh.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/si.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sj.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sl.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/so.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/st.gif
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sv.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sy.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tc.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/td.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tf.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/th.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tj.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tl.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/to.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tr.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tt.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tv.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tw.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ua.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ug.gif
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/uk.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/um.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/us.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/uy.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/uz.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/va.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vc.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ve.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vg.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vi.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vn.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vu.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/wales.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/wf.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ws.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ye.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      382 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/yt.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/za.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/zm.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/zw.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.923898 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/action.png
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/download.png
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/link.gif
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/list.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/mail.png
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    46715 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/proportional.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/share.png
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stretch.png
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/text.png
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/upload.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.931898 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/SILK.txt
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_view_list.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.gif
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.939899 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_child_window.png
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png
--rw-r--r--   0 runner    (1001) docker     (123)   107691 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_share_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_tile.png
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      943 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/bogus.png
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.939899 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.943899 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/
--rwxr-xr-x   0 runner    (1001) docker     (123)    68025 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    53422 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    84237 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    46362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png
--rw-r--r--   0 runner    (1001) docker     (123)    52365 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png
--rw-r--r--   0 runner    (1001) docker     (123)   145699 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png
--rw-r--r--   0 runner    (1001) docker     (123)   392128 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png
--rw-r--r--   0 runner    (1001) docker     (123)   163756 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    59065 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.947899 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9480 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/App.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/AppView.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    14016 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4841 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    27390 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.951900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js
--rw-r--r--   0 runner    (1001) docker     (123)    24463 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBoxSelect.js
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4483 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     3625 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.951900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Image.js
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    28882 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js
--rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.955900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js
--rw-r--r--   0 runner    (1001) docker     (123)    95465 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.955900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     2744 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.955900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.955900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.959900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/new_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.959900 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.827891 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.963901 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12067 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)    76877 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js
--rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    39644 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js
--rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TreeMenuModel.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.963901 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot
--rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.967901 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.967901 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/template/ConfigurationManager/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/template/ConfigurationManager/diffConfig.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/template/root.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/web.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.967901 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5209 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/scripts/dirac_webapp_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-16 09:16:47.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/scripts/tornado-start-web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:17:31.831892 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-03-16 09:17:31.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37442 2023-03-16 09:17:31.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 09:17:31.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-16 09:17:31.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 09:17:31.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-16 09:17:31.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 09:17:31.000000 WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.858667 WebAppDIRAC-5.1.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-19 09:26:11.858667 WebAppDIRAC-5.1.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20406 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/extjs-template.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-19 09:26:03.000000 WebAppDIRAC-5.1.0a7/release.notes
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-19 09:26:11.858667 WebAppDIRAC-5.1.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.682660 WebAppDIRAC-5.1.0a7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.706661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.710662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/App.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/CoreHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/HandlerMgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/StaticHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/TemplateLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.710662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/Conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/SessionData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/WebHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.710662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.714661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ApplicationWizardHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/NotepadHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/PublicStateManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/RootHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/UPHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.698661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.698661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.686660 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.714661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/Accounting.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.686660 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Image.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/ApplicationWizard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.686660 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/ComponentHistory.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.686660 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42537 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.686660 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/Downtimes.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.686660 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/ExampleApp.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.686660 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.718662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41538 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.722662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.726662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/group.png
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.png
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_date.png
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_float.png
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_int.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_string.png
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/query.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/ungroup.png
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.690661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.726662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18576 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.726662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/JobLaunchpad.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.690661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.726662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40184 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.726662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.690661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/JobSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.690661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/Notepad.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.690661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26773 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/PilotMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.730662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.690661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/PilotSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.690661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/ProxyManager.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.694661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4502 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/ProxyUpload.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.694661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuModel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/PublicStateManager.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.694661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51599 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/RegistryManager.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.694661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.734662 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/RequestMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.694661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/TreeModel.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/ResourceSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.694661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/SiteSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.694661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/SpaceOccupancy.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.698661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48525 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/SystemAdministration.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.698661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/TokenManager.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.698661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/TransformationMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.702661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.738663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/css/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7083 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/css/css.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/css/iconset.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.698661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.742663 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.802665 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ad.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ae.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/af.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ag.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ai.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/al.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/am.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/an.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ao.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ar.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/as.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/at.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/au.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/aw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ax.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/az.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ba.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bb.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/be.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/br.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/by.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ca.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/catalonia.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cc.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ch.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ci.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ck.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      353 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/co.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cx.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/de.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/do.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ec.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ee.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/eg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/eh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/england.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/er.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/es.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/et.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/eu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fam.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ga.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      379 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ge.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gq.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ht.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/id.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ie.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/il.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/in.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/io.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/iq.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ir.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/is.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/it.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/jm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/jo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/jp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ke.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ki.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/km.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ky.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/la.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lb.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/li.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ls.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ly.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ma.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/md.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/me.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      382 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ml.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      379 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mq.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ms.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mx.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/my.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/na.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ne.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ng.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ni.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/no.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/np.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/om.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pa.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pe.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ph.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ps.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/py.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/qa.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/re.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ro.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/rs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ru.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/rw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sa.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sb.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/scotland.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/se.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/si.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/so.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/st.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/td.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/th.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/to.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ua.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ug.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/uk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/um.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/us.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/uy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/uz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/va.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ve.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/wales.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/wf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ws.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ye.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      382 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/yt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/za.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/zm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/zw.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.698661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.810665 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/action.png
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/link.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/list.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/mail.png
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46715 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/proportional.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/share.png
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stretch.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/text.png
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/upload.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.822666 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/SILK.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_view_list.png
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.826666 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_child_window.png
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107691 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_share_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      943 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/bogus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.830666 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.834666 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68025 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53422 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    84237 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    46362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52365 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)   145699 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)   392128 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png
+-rw-r--r--   0 runner    (1001) docker     (123)   163756 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59065 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.702661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.834666 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9480 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/App.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/AppView.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14016 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4841 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27390 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.842667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24463 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBoxSelect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4483 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3625 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.842667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Image.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28882 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.842667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95465 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.842667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2744 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.702661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.842667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.846667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.850667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/new_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.850667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.702661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.854667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12067 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    76877 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39644 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TreeMenuModel.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.854667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.854667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.854667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/template/ConfigurationManager/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/template/ConfigurationManager/diffConfig.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/template/root.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/web.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.858667 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5209 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/scripts/dirac_webapp_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-19 09:25:37.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/scripts/tornado-start-web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:26:11.706661 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-19 09:26:11.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37442 2023-06-19 09:26:11.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:26:11.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-19 09:26:11.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:26:11.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-19 09:26:11.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 09:26:11.000000 WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/top_level.txt
```

### Comparing `WebAppDIRAC-5.1.0a6/LICENSE` & `WebAppDIRAC-5.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/PKG-INFO` & `WebAppDIRAC-5.1.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebAppDIRAC
-Version: 5.1.0a6
+Version: 5.1.0a7
 Summary: WebAppDIRAC is a portal for the DIRAC software.
 Home-page: https://github.com/DIRACGrid/WebAppDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `WebAppDIRAC-5.1.0a6/README.rst` & `WebAppDIRAC-5.1.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/extjs-template.xml` & `WebAppDIRAC-5.1.0a7/extjs-template.xml`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/pyproject.toml` & `WebAppDIRAC-5.1.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/release.notes` & `WebAppDIRAC-5.1.0a7/release.notes`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+[v5.1.0a7]
+
+FIX: (#728) Removed Setup from SystemAdministrator
+CHANGE: (#728) one WebApp for one DIRAC Setup
+FIX: (#714) remove OwnerDN from RMS
+
 [v5.1.0a6]
 
 FIX: (#733) WebHandler - make explicit import of TornadoResponse from BaseRequestHandler
 CHANGE: (#732) Display user access and refresh tokens with details (right click pop up window)
 
 [v5.1.0a5]
```

### Comparing `WebAppDIRAC-5.1.0a6/setup.cfg` & `WebAppDIRAC-5.1.0a7/setup.cfg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/App.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/App.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/CoreHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/CoreHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/HandlerMgr.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/HandlerMgr.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/StaticHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/StaticHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Core/TemplateLoader.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Core/TemplateLoader.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/Conf.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/Conf.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/SessionData.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/SessionData.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/Lib/WebHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/Lib/WebHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,18 +105,18 @@
             else:
                 reqtype = [["Nothing to display"]]
         else:
             reqtype = [["Error during RPC call"]]
         callback["operationType"] = reqtype
 
         # U S E R
-        if (result := self.reqClient.getDistinctValuesWeb("OwnerDN"))["OK"]:
+        if (result := self.reqClient.getDistinctValuesWeb("Owner"))["OK"]:
             owner = []
-            for dn in result["Value"]:
-                owner.append([dn])
+            for own in result["Value"]:
+                owner.append([own])
             if len(owner) < 2:
                 owner = [["Nothing to display"]]
         else:
             owner = [["Error during RPC call"]]
         callback["owner"] = owner
 
         # G R O U P
@@ -173,15 +173,15 @@
             if value := list(json.loads(operationType)):
                 req["Type"] = value
             if value := list(json.loads(ownerGroup)):
                 req["OwnerGroup"] = value
             if value := list(json.loads(status)):
                 req["Status"] = value
             if value := list(json.loads(owner)):
-                req["OwnerDN"] = value
+                req["Owner"] = value
 
         if startDate:
             req["FromDate"] = startDate
             if startTime:
                 req["FromDate"] += " " + startTime
 
         if endDate:
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/RootHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/RootHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,21 +20,14 @@
     def web_changeGroup(self, to: str):
         """Change group
 
         :return: TornadoResponse()
         """
         return TornadoResponse().redirect(self.__change(group=to))  # pylint: disable=no-member
 
-    def web_changeSetup(self, to: str):
-        """Change setup
-
-        :return: TornadoResponse()
-        """
-        return TornadoResponse().redirect(self.__change(setup=to))  # pylint: disable=no-member
-
     def __change(self, setup: str = None, group: str = None) -> str:
         """Generate URL to change setup/group, set query"""
         root = Conf.rootURL().strip("/")
         setup = setup or self.getUserSetup() or ""
         group = group or self.getUserGroup() or ""
         query = ((ref := self.request.headers.get("Referer")) and urlparse(ref).query) or ""
         return f"/{root}/s:{setup}/g:{group}/?{query}"
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     def web_getSysInfo(self):
         """Provide information about hosts state from database"""
         client = ComponentMonitoringClient(delegatedDN=self.getUserDN(), delegatedGroup=self.getUserGroup())
         if not (result := client.getLogs())["OK"] or not len(callback := result["Value"]) > 0:
             return {"success": "false", "error": result.get("Message", "No system information found")}
 
         # Add the information about the extensions' versions, if available, to display along with the DIRAC version
-        for i in range(len(callback)):
-            callback[i]["Host"] = callback[i]["HostName"]
-            callback[i]["Timestamp"] = str(callback[i].get("Timestamp", "unknown"))
+        for _i, cb in enumerate(callback):
+            cb["Host"] = cb["HostName"]
+            cb["Timestamp"] = str(cb.get("Timestamp", "unknown"))
             # We have to keep the backward compatibility (this can heppen when we do not update one host to v6r15 ...
-            callback[i]["DIRAC"] = "{},{}".format(
-                callback[i].get("DIRACVersion", callback[i].get("DIRAC", "")),
-                callback[i].get("Extension", callback[i].get("Extensions", "")),
+            cb["DIRAC"] = "{},{}".format(
+                cb.get("DIRACVersion", cb.get("DIRAC", "")),
+                cb.get("Extension", cb.get("Extensions", "")),
             )
 
         return {"success": "true", "result": sorted(callback, key=lambda i: i["Host"]), "total": len(callback)}
 
     def web_getHostData(self, hostname=None):
         """
         Returns flatten list of components (services, agents) installed on hosts
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/handler/UPHandler.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/handler/UPHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -118,16 +118,14 @@
     }, {
         name: "MasterJobID",
     }, {
         name: "KilledFlag",
     }, {
         name: "RescheduleTime",
     }, {
-        name: "DIRACSetup",
-    }, {
         name: "FailedFlag",
     }, {
         name: "CPUTime",
     }, {
         name: "OwnerDN",
     }, {
         name: "JobGroup",
@@ -401,20 +399,14 @@
             "SubmissionTime[UTC]": {
                 dataIndex: "SubmissionTime",
                 renderer: Ext.util.Format.dateRenderer("Y-m-d H:i:s"),
                 properties: {
                     width: 150,
                 },
             },
-            DIRACSetup: {
-                dataIndex: "DIRACSetup",
-                properties: {
-                    hidden: true,
-                },
-            },
             FailedFlag: {
                 dataIndex: "FailedFlag",
                 properties: {
                     hidden: true,
                 },
             },
             RescheduleCounter: {
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
     }, {
         name: "CreationTime",
         type: "date",
         dateFormat: "Y-m-d H:i:s",
     }, {
         name: "JobID",
     }, {
-        name: "OwnerDN",
+        name: "Owner",
     }, {
         name: "RequestID",
         type: "int",
     }, {
         name: "Error",
     }, {
         name: "RequestName",
@@ -176,16 +176,16 @@
             },
             Status: {
                 dataIndex: "Status",
                 properties: {
                     width: 60,
                 },
             },
-            OwnerDN: {
-                dataIndex: "OwnerDN",
+            Owner: {
+                dataIndex: "Owner",
             },
             OperationType: {
                 dataIndex: "OperationType",
             },
             OwnerGroup: {
                 dataIndex: "OwnerGroup",
             },
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -127,16 +127,14 @@
             }, {
                 name: "OpenFiles",
             }, {
                 name: "OpenPipes",
             }, {
                 name: "OpenSockets",
             }, {
-                name: "Setup",
-            }, {
                 name: "Uptime",
             }, ],
             remoteSort: true,
             pageSize: 100,
             createTabsOnce: false,
             listeners: {
                 load: function(oStore, records, successful, eOpts) {
@@ -346,19 +344,14 @@
             }, {
                 align: "left",
                 dataIndex: "OpenSockets",
                 header: "OpenSockets",
                 sortable: true,
             }, {
                 align: "left",
-                dataIndex: "Setup",
-                header: "Setup",
-                sortable: true,
-            }, {
-                align: "left",
                 dataIndex: "Uptime",
                 header: "Uptime",
                 sortable: true,
             }, ],
             rendererChkBox: function(val) {
                 return '<input value="' + val + '" type="checkbox" class="checkrow" style="margin:0px;padding:0px"/>';
             },
@@ -490,16 +483,14 @@
             fields: [{
                 name: "System",
             }, {
                 name: "Host",
             }, {
                 name: "Name",
             }, {
-                name: "Setup",
-            }, {
                 name: "PID",
             }, {
                 name: "RunitStatus",
             }, {
                 name: "Module",
             }, {
                 name: "Installed",
@@ -827,20 +818,14 @@
 
             Description: {
                 dataIndex: "Description",
                 renderer: function(value, metaData, record, row, col, store, gridView) {
                     return me.rendererGridColumn(value, record);
                 },
             },
-            Setup: {
-                dataIndex: "Setup",
-                renderer: function(value, metaData, record, row, col, store, gridView) {
-                    return me.rendererGridColumn(value, record);
-                },
-            },
             Port: {
                 dataIndex: "Port",
                 renderer: function(value, metaData, record, row, col, store, gridView) {
                     return me.rendererGridColumn(value, record);
                 },
             },
             Type: {
@@ -932,16 +917,14 @@
             }, {
                 name: "Description",
             }, {
                 name: "ComponentModule",
             }, {
                 name: "ComponentName",
             }, {
-                name: "Setup",
-            }, {
                 name: "Port",
             }, {
                 name: "Platform",
             }, {
                 name: "DIRACVersion",
             }, {
                 name: "VersionTimestamp",
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/css/css.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/css/css.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/css/iconset.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/css/iconset.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/App.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/App.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -72,18 +72,14 @@
                 },
                 me.addAuthsButton(), {
                     xtype: "label",
                     text: "Group:",
                 },
                 me.addGroupsButton(), {
                     xtype: "label",
-                    text: "Setup:",
-                },
-                me.addSetupButton(), {
-                    xtype: "label",
                     text: "Theme:",
                 },
                 me.addThemeButton(),
             ],
         });
         return form;
     },
@@ -217,32 +213,14 @@
             //     }
             //   });
             // }
         }
 
         return new Ext.button.Button(button_group);
     },
-    addSetupButton: function() {
-        var setup_data = {
-            text: GLOBAL.APP.configData["setup"],
-            menu: [],
-        };
-
-        for (var i = 0; i < GLOBAL.APP.configData["validSetups"].length; i++)
-            setup_data.menu.push({
-                text: GLOBAL.APP.configData["validSetups"][i],
-                handler: function() {
-                    var me = this;
-
-                    location.href = GLOBAL.BASE_URL + "changeSetup?to=" + me.text;
-                },
-            });
-
-        return new Ext.button.Button(setup_data);
-    },
     addThemeButton: function() {
         var me = this;
 
         var sButtonThemeText = "Crisp";
 
         if (GLOBAL.WEB_THEME == "neptune") sButtonThemeText = "Neptune";
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/index.html` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/index.html`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/template/root.tpl` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/template/root.tpl`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/WebApp/web.cfg` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/WebApp/web.cfg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/__init__.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/scripts/dirac_webapp_run.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/scripts/dirac_webapp_run.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC/scripts/tornado-start-web.py` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC/scripts/tornado-start-web.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/PKG-INFO` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebAppDIRAC
-Version: 5.1.0a6
+Version: 5.1.0a7
 Summary: WebAppDIRAC is a portal for the DIRAC software.
 Home-page: https://github.com/DIRACGrid/WebAppDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `WebAppDIRAC-5.1.0a6/src/WebAppDIRAC.egg-info/SOURCES.txt` & `WebAppDIRAC-5.1.0a7/src/WebAppDIRAC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

