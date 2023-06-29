# Comparing `tmp/types-usd-23.5.0.tar.gz` & `tmp/types_usd-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-usd-23.5.0.tar", last modified: Wed Jun 28 18:56:54 2023, max compression
+gzip compressed data, was "types_usd-23.5.1.tar", max compression
```

## Comparing `types-usd-23.5.0.tar` & `types_usd-23.5.1.tar`

### file list

```diff
@@ -1,111 +1,110 @@
--rw-r--r--   0        0        0     1370 2023-06-28 18:56:10.930800 types-usd-23.5.0/README.md
--rw-r--r--   0        0        0      891 2023-06-28 18:55:42.888335 types-usd-23.5.0/pyproject.toml
--rw-r--r--   0        0        0       49 2023-06-23 17:49:46.419987 types-usd-23.5.0/stubs/Boost-stubs/Python.pyi
--rw-r--r--   0        0        0        0 2023-06-21 23:01:02.519211 types-usd-23.5.0/stubs/Boost-stubs/__init__.pyi
--rw-r--r--   0        0        0     7049 2023-06-28 15:48:51.837957 types-usd-23.5.0/stubs/pxr-stubs/Ar/__init__.pyi
--rw-r--r--   0        0        0     2665 2023-06-28 15:48:51.852230 types-usd-23.5.0/stubs/pxr-stubs/CameraUtil/__init__.pyi
--rw-r--r--   0        0        0      519 2023-06-28 15:48:51.855944 types-usd-23.5.0/stubs/pxr-stubs/Garch/__init__.pyi
--rw-r--r--   0        0        0     2580 2023-06-28 15:48:51.868492 types-usd-23.5.0/stubs/pxr-stubs/GeomUtil/__init__.pyi
--rw-r--r--   0        0        0   146484 2023-06-28 15:48:56.281451 types-usd-23.5.0/stubs/pxr-stubs/Gf/__init__.pyi
--rw-r--r--   0        0        0     2816 2023-06-28 15:48:56.567439 types-usd-23.5.0/stubs/pxr-stubs/Glf/__init__.pyi
--rw-r--r--   0        0        0     1150 2023-06-28 15:48:56.680440 types-usd-23.5.0/stubs/pxr-stubs/Kind/__init__.pyi
--rw-r--r--   0        0        0    10012 2023-06-28 15:48:57.225242 types-usd-23.5.0/stubs/pxr-stubs/Ndr/__init__.pyi
--rw-r--r--   0        0        0    18096 2023-06-28 15:48:57.850280 types-usd-23.5.0/stubs/pxr-stubs/Pcp/__init__.pyi
--rw-r--r--   0        0        0     4926 2023-06-28 15:48:58.001165 types-usd-23.5.0/stubs/pxr-stubs/Plug/__init__.pyi
--rw-r--r--   0        0        0     6708 2023-06-28 15:48:58.138286 types-usd-23.5.0/stubs/pxr-stubs/PxOsd/__init__.pyi
--rw-r--r--   0        0        0   110718 2023-06-28 15:48:59.846280 types-usd-23.5.0/stubs/pxr-stubs/Sdf/__init__.pyi
--rw-r--r--   0        0        0     7675 2023-06-28 15:48:59.911996 types-usd-23.5.0/stubs/pxr-stubs/Sdr/__init__.pyi
--rw-r--r--   0        0        0      428 2023-06-28 15:48:59.920453 types-usd-23.5.0/stubs/pxr-stubs/Sdr/shaderParserTestUtils.pyi
--rw-r--r--   0        0        0       34 2023-06-28 15:48:59.922473 types-usd-23.5.0/stubs/pxr-stubs/SdrGlslfx/__init__.pyi
--rw-r--r--   0        0        0    23836 2023-06-28 15:49:00.136069 types-usd-23.5.0/stubs/pxr-stubs/Tf/__init__.pyi
--rw-r--r--   0        0        0      354 2023-06-28 15:49:00.139822 types-usd-23.5.0/stubs/pxr-stubs/Tf/testenv/testTfPyInvoke_callees.pyi
--rw-r--r--   0        0        0       54 2023-06-28 15:49:00.141617 types-usd-23.5.0/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_DepLoadsAll.pyi
--rw-r--r--   0        0        0       54 2023-06-28 15:49:00.143767 types-usd-23.5.0/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsAll.pyi
--rw-r--r--   0        0        0      145 2023-06-28 15:49:00.146483 types-usd-23.5.0/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsUnknown.pyi
--rw-r--r--   0        0        0       54 2023-06-28 15:49:00.148173 types-usd-23.5.0/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Other.pyi
--rw-r--r--   0        0        0       34 2023-06-28 15:49:00.150255 types-usd-23.5.0/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Test.pyi
--rw-r--r--   0        0        0       54 2023-06-28 15:49:00.151221 types-usd-23.5.0/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Unknown.pyi
--rw-r--r--   0        0        0     3023 2023-06-28 15:49:00.203818 types-usd-23.5.0/stubs/pxr-stubs/Trace/__init__.pyi
--rw-r--r--   0        0        0    87935 2023-06-28 15:49:01.331731 types-usd-23.5.0/stubs/pxr-stubs/Usd/__init__.pyi
--rw-r--r--   0        0        0     1309 2023-06-28 15:49:01.342979 types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/__init__.pyi
--rw-r--r--   0        0        0      166 2023-06-28 15:49:01.344881 types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/cameraArgs.pyi
--rw-r--r--   0        0        0      118 2023-06-28 15:49:01.346090 types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/colorArgs.pyi
--rw-r--r--   0        0        0     1029 2023-06-28 15:49:01.350709 types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi
--rw-r--r--   0        0        0      705 2023-06-28 15:49:01.360869 types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi
--rw-r--r--   0        0        0      175 2023-06-28 15:49:01.362511 types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/rendererArgs.pyi
--rw-r--r--   0        0        0      304 2023-06-28 15:49:01.389621 types-usd-23.5.0/stubs/pxr-stubs/UsdBakeMtlx/__init__.pyi
--rw-r--r--   0        0        0    83687 2023-06-28 15:49:02.263615 types-usd-23.5.0/stubs/pxr-stubs/UsdGeom/__init__.pyi
--rw-r--r--   0        0        0     3443 2023-06-28 15:49:02.295915 types-usd-23.5.0/stubs/pxr-stubs/UsdHydra/__init__.pyi
--rw-r--r--   0        0        0     6059 2023-06-28 15:49:02.411419 types-usd-23.5.0/stubs/pxr-stubs/UsdImagingGL/__init__.pyi
--rw-r--r--   0        0        0    35601 2023-06-28 15:49:04.283645 types-usd-23.5.0/stubs/pxr-stubs/UsdLux/__init__.pyi
--rw-r--r--   0        0        0     5219 2023-06-28 15:49:04.746431 types-usd-23.5.0/stubs/pxr-stubs/UsdMedia/__init__.pyi
--rw-r--r--   0        0        0      205 2023-06-28 15:49:04.751338 types-usd-23.5.0/stubs/pxr-stubs/UsdMtlx/__init__.pyi
--rw-r--r--   0        0        0    30245 2023-06-28 15:49:05.882511 types-usd-23.5.0/stubs/pxr-stubs/UsdPhysics/__init__.pyi
--rw-r--r--   0        0        0     1303 2023-06-28 15:49:05.924763 types-usd-23.5.0/stubs/pxr-stubs/UsdProc/__init__.pyi
--rw-r--r--   0        0        0    10932 2023-06-28 15:49:06.269818 types-usd-23.5.0/stubs/pxr-stubs/UsdRender/__init__.pyi
--rw-r--r--   0        0        0      420 2023-06-28 15:49:06.296792 types-usd-23.5.0/stubs/pxr-stubs/UsdResolverExample/__init__.pyi
--rw-r--r--   0        0        0     9070 2023-06-28 15:49:06.564529 types-usd-23.5.0/stubs/pxr-stubs/UsdRi/__init__.pyi
--rw-r--r--   0        0        0     4124 2023-06-28 15:49:06.876274 types-usd-23.5.0/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi
--rw-r--r--   0        0        0    35876 2023-06-28 15:49:08.018489 types-usd-23.5.0/stubs/pxr-stubs/UsdShade/__init__.pyi
--rw-r--r--   0        0        0       34 2023-06-28 15:49:08.022179 types-usd-23.5.0/stubs/pxr-stubs/UsdShaders/__init__.pyi
--rw-r--r--   0        0        0    35939 2023-06-28 15:49:09.235391 types-usd-23.5.0/stubs/pxr-stubs/UsdSkel/__init__.pyi
--rw-r--r--   0        0        0     5408 2023-06-28 15:49:09.475642 types-usd-23.5.0/stubs/pxr-stubs/UsdUI/__init__.pyi
--rw-r--r--   0        0        0    12274 2023-06-28 15:49:09.740655 types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/__init__.pyi
--rw-r--r--   0        0        0     6228 2023-06-28 15:49:09.762509 types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi
--rw-r--r--   0        0        0      417 2023-06-28 15:49:09.770512 types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/constantsGroup.pyi
--rw-r--r--   0        0        0      331 2023-06-28 15:49:09.775478 types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/fixBrokenPixarSchemas.pyi
--rw-r--r--   0        0        0       62 2023-06-28 15:49:09.789716 types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/toolPaths.pyi
--rw-r--r--   0        0        0     2040 2023-06-28 15:49:09.829323 types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi
--rw-r--r--   0        0        0      676 2023-06-28 15:49:09.845034 types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi
--rw-r--r--   0        0        0     7574 2023-06-28 15:49:10.073985 types-usd-23.5.0/stubs/pxr-stubs/UsdVol/__init__.pyi
--rw-r--r--   0        0        0     7634 2023-06-28 15:49:10.196659 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/__init__.pyi
--rw-r--r--   0        0        0      577 2023-06-28 15:49:10.205195 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi
--rw-r--r--   0        0        0      171 2023-06-28 15:49:10.207894 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterialUI.pyi
--rw-r--r--   0        0        0      997 2023-06-28 15:49:10.228747 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi
--rw-r--r--   0        0        0      156 2023-06-28 15:49:10.236841 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/adjustFreeCameraUI.pyi
--rw-r--r--   0        0        0    18213 2023-06-28 15:49:10.475800 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/appController.pyi
--rw-r--r--   0        0        0      644 2023-06-28 15:49:10.486134 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi
--rw-r--r--   0        0        0     2019 2023-06-28 15:49:10.531389 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi
--rw-r--r--   0        0        0      793 2023-06-28 15:49:10.535243 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi
--rw-r--r--   0        0        0      168 2023-06-28 15:49:10.537991 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/attributeValueEditorUI.pyi
--rw-r--r--   0        0        0     1882 2023-06-28 15:49:10.556557 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi
--rw-r--r--   0        0        0     8022 2023-06-28 15:49:10.681763 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/common.pyi
--rw-r--r--   0        0        0      281 2023-06-28 15:49:10.684414 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/configController.pyi
--rw-r--r--   0        0        0     1603 2023-06-28 15:49:10.704016 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/customAttributes.pyi
--rw-r--r--   0        0        0      601 2023-06-28 15:49:10.709315 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi
--rw-r--r--   0        0        0      496 2023-06-28 15:49:10.713801 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/frameSlider.pyi
--rw-r--r--   0        0        0     1835 2023-06-28 15:49:10.790093 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/freeCamera.pyi
--rw-r--r--   0        0        0      640 2023-06-28 15:49:10.793397 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi
--rw-r--r--   0        0        0     6154 2023-06-28 15:49:10.852005 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi
--rw-r--r--   0        0        0     1446 2023-06-28 15:49:10.859553 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi
--rw-r--r--   0        0        0      126 2023-06-28 15:49:10.861956 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/legendUtil.pyi
--rw-r--r--   0        0        0      501 2023-06-28 15:49:10.865414 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/mainWindowUI.pyi
--rw-r--r--   0        0        0      386 2023-06-28 15:49:10.874663 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/overridableLineEdit.pyi
--rw-r--r--   0        0        0     1446 2023-06-28 15:49:10.903114 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/plugin.pyi
--rw-r--r--   0        0        0      522 2023-06-28 15:49:10.913890 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/preferences.pyi
--rw-r--r--   0        0        0      141 2023-06-28 15:49:10.919037 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/preferencesUI.pyi
--rw-r--r--   0        0        0       95 2023-06-28 15:49:10.924682 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/prettyPrint.pyi
--rw-r--r--   0        0        0      348 2023-06-28 15:49:10.929604 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primContextMenu.pyi
--rw-r--r--   0        0        0     2551 2023-06-28 15:49:11.006610 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi
--rw-r--r--   0        0        0      618 2023-06-28 15:49:11.025050 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primLegend.pyi
--rw-r--r--   0        0        0      138 2023-06-28 15:49:11.028406 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primLegendUI.pyi
--rw-r--r--   0        0        0     3490 2023-06-28 15:49:11.081432 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi
--rw-r--r--   0        0        0     2027 2023-06-28 15:49:11.110554 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primViewItem.pyi
--rw-r--r--   0        0        0      650 2023-06-28 15:49:11.113758 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi
--rw-r--r--   0        0        0      150 2023-06-28 15:49:11.116325 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/propertyLegendUI.pyi
--rw-r--r--   0        0        0     3310 2023-06-28 15:49:11.179803 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi
--rw-r--r--   0        0        0      213 2023-06-28 15:49:11.197653 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/qt.pyi
--rw-r--r--   0        0        0     1246 2023-06-28 15:49:11.226086 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi
--rw-r--r--   0        0        0      220 2023-06-28 15:49:11.237751 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/scalarTypes.pyi
--rw-r--r--   0        0        0     5249 2023-06-28 15:49:11.417943 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi
--rw-r--r--   0        0        0     1367 2023-06-28 15:49:11.458856 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/settings.pyi
--rw-r--r--   0        0        0     7670 2023-06-28 15:49:11.565403 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/stageView.pyi
--rw-r--r--   0        0        0     1720 2023-06-28 15:49:11.621554 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi
--rw-r--r--   0        0        0       90 2023-06-28 15:49:11.632484 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/usdviewContextMenuItem.pyi
--rw-r--r--   0        0        0      377 2023-06-28 15:49:11.635641 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/variantComboBox.pyi
--rw-r--r--   0        0        0     3648 2023-06-28 15:49:11.663504 types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi
--rw-r--r--   0        0        0   278095 2023-06-28 15:49:16.480894 types-usd-23.5.0/stubs/pxr-stubs/Vt/__init__.pyi
--rw-r--r--   0        0        0      301 2023-06-28 15:49:16.488490 types-usd-23.5.0/stubs/pxr-stubs/Work/__init__.pyi
--rw-r--r--   0        0        0     1000 2023-06-28 15:48:51.789375 types-usd-23.5.0/stubs/pxr-stubs/__init__.pyi
--rw-r--r--   0        0        0     3173 2023-06-28 18:56:54.702778 types-usd-23.5.0/setup.py
--rw-r--r--   0        0        0     2374 2023-06-28 18:56:54.703243 types-usd-23.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1370 2023-06-28 20:35:24.431058 types_usd-23.5.1/README.md
+-rw-r--r--   0        0        0      892 2023-06-29 22:20:41.804033 types_usd-23.5.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-06-28 20:35:24.431928 types_usd-23.5.1/stubs/Boost-stubs/Python.pyi
+-rw-r--r--   0        0        0        0 2023-06-28 20:35:24.430426 types_usd-23.5.1/stubs/Boost-stubs/__init__.pyi
+-rw-r--r--   0        0        0     7049 2023-06-29 20:31:52.968144 types_usd-23.5.1/stubs/pxr-stubs/Ar/__init__.pyi
+-rw-r--r--   0        0        0     2665 2023-06-29 20:31:53.006778 types_usd-23.5.1/stubs/pxr-stubs/CameraUtil/__init__.pyi
+-rw-r--r--   0        0        0      519 2023-06-29 20:31:53.011325 types_usd-23.5.1/stubs/pxr-stubs/Garch/__init__.pyi
+-rw-r--r--   0        0        0     2580 2023-06-29 20:31:53.025300 types_usd-23.5.1/stubs/pxr-stubs/GeomUtil/__init__.pyi
+-rw-r--r--   0        0        0   146484 2023-06-29 20:31:54.347650 types_usd-23.5.1/stubs/pxr-stubs/Gf/__init__.pyi
+-rw-r--r--   0        0        0     2816 2023-06-29 20:31:54.367487 types_usd-23.5.1/stubs/pxr-stubs/Glf/__init__.pyi
+-rw-r--r--   0        0        0     1150 2023-06-29 20:31:54.374438 types_usd-23.5.1/stubs/pxr-stubs/Kind/__init__.pyi
+-rw-r--r--   0        0        0    10319 2023-06-29 21:59:32.587039 types_usd-23.5.1/stubs/pxr-stubs/Ndr/__init__.pyi
+-rw-r--r--   0        0        0    18096 2023-06-29 20:31:54.529773 types_usd-23.5.1/stubs/pxr-stubs/Pcp/__init__.pyi
+-rw-r--r--   0        0        0     4926 2023-06-29 20:31:54.557386 types_usd-23.5.1/stubs/pxr-stubs/Plug/__init__.pyi
+-rw-r--r--   0        0        0     6708 2023-06-29 20:31:54.584716 types_usd-23.5.1/stubs/pxr-stubs/PxOsd/__init__.pyi
+-rw-r--r--   0        0        0   110698 2023-06-29 20:31:55.706539 types_usd-23.5.1/stubs/pxr-stubs/Sdf/__init__.pyi
+-rw-r--r--   0        0        0     7778 2023-06-29 21:59:32.587720 types_usd-23.5.1/stubs/pxr-stubs/Sdr/__init__.pyi
+-rw-r--r--   0        0        0      428 2023-06-29 20:31:55.749121 types_usd-23.5.1/stubs/pxr-stubs/Sdr/shaderParserTestUtils.pyi
+-rw-r--r--   0        0        0       34 2023-06-29 20:31:55.749749 types_usd-23.5.1/stubs/pxr-stubs/SdrGlslfx/__init__.pyi
+-rw-r--r--   0        0        0    23836 2023-06-29 20:31:55.869275 types_usd-23.5.1/stubs/pxr-stubs/Tf/__init__.pyi
+-rw-r--r--   0        0        0      354 2023-06-29 20:31:55.870889 types_usd-23.5.1/stubs/pxr-stubs/Tf/testenv/testTfPyInvoke_callees.pyi
+-rw-r--r--   0        0        0       54 2023-06-29 20:31:55.871383 types_usd-23.5.1/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_DepLoadsAll.pyi
+-rw-r--r--   0        0        0       54 2023-06-29 20:31:55.871948 types_usd-23.5.1/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsAll.pyi
+-rw-r--r--   0        0        0      145 2023-06-29 20:31:55.872609 types_usd-23.5.1/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsUnknown.pyi
+-rw-r--r--   0        0        0       54 2023-06-29 20:31:55.873047 types_usd-23.5.1/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Other.pyi
+-rw-r--r--   0        0        0       34 2023-06-29 20:31:55.873462 types_usd-23.5.1/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Test.pyi
+-rw-r--r--   0        0        0       54 2023-06-29 20:31:55.873752 types_usd-23.5.1/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Unknown.pyi
+-rw-r--r--   0        0        0     3023 2023-06-29 20:31:55.894023 types_usd-23.5.1/stubs/pxr-stubs/Trace/__init__.pyi
+-rw-r--r--   0        0        0    87967 2023-06-29 20:31:56.350653 types_usd-23.5.1/stubs/pxr-stubs/Usd/__init__.pyi
+-rw-r--r--   0        0        0     1212 2023-06-29 22:00:17.643813 types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/__init__.pyi
+-rw-r--r--   0        0        0      166 2023-06-29 20:31:56.358410 types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/cameraArgs.pyi
+-rw-r--r--   0        0        0      118 2023-06-29 20:31:56.359253 types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/colorArgs.pyi
+-rw-r--r--   0        0        0     1029 2023-06-29 20:31:56.361693 types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi
+-rw-r--r--   0        0        0      705 2023-06-29 20:31:56.381471 types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi
+-rw-r--r--   0        0        0      175 2023-06-29 20:31:56.383035 types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/rendererArgs.pyi
+-rw-r--r--   0        0        0      304 2023-06-29 20:31:56.395163 types_usd-23.5.1/stubs/pxr-stubs/UsdBakeMtlx/__init__.pyi
+-rw-r--r--   0        0        0    83687 2023-06-29 20:31:56.817606 types_usd-23.5.1/stubs/pxr-stubs/UsdGeom/__init__.pyi
+-rw-r--r--   0        0        0     3443 2023-06-29 20:31:56.829794 types_usd-23.5.1/stubs/pxr-stubs/UsdHydra/__init__.pyi
+-rw-r--r--   0        0        0     6059 2023-06-29 20:31:56.860521 types_usd-23.5.1/stubs/pxr-stubs/UsdImagingGL/__init__.pyi
+-rw-r--r--   0        0        0    35601 2023-06-29 20:31:57.033242 types_usd-23.5.1/stubs/pxr-stubs/UsdLux/__init__.pyi
+-rw-r--r--   0        0        0     5219 2023-06-29 20:31:57.056646 types_usd-23.5.1/stubs/pxr-stubs/UsdMedia/__init__.pyi
+-rw-r--r--   0        0        0      205 2023-06-29 20:31:57.058491 types_usd-23.5.1/stubs/pxr-stubs/UsdMtlx/__init__.pyi
+-rw-r--r--   0        0        0    30245 2023-06-29 20:31:57.199094 types_usd-23.5.1/stubs/pxr-stubs/UsdPhysics/__init__.pyi
+-rw-r--r--   0        0        0     1303 2023-06-29 20:31:57.205243 types_usd-23.5.1/stubs/pxr-stubs/UsdProc/__init__.pyi
+-rw-r--r--   0        0        0    10932 2023-06-29 20:31:57.253949 types_usd-23.5.1/stubs/pxr-stubs/UsdRender/__init__.pyi
+-rw-r--r--   0        0        0      420 2023-06-29 20:31:57.261584 types_usd-23.5.1/stubs/pxr-stubs/UsdResolverExample/__init__.pyi
+-rw-r--r--   0        0        0     9070 2023-06-29 20:31:57.310140 types_usd-23.5.1/stubs/pxr-stubs/UsdRi/__init__.pyi
+-rw-r--r--   0        0        0     4124 2023-06-29 20:31:57.352555 types_usd-23.5.1/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi
+-rw-r--r--   0        0        0    36031 2023-06-29 21:59:32.588449 types_usd-23.5.1/stubs/pxr-stubs/UsdShade/__init__.pyi
+-rw-r--r--   0        0        0       34 2023-06-29 20:31:57.539116 types_usd-23.5.1/stubs/pxr-stubs/UsdShaders/__init__.pyi
+-rw-r--r--   0        0        0    35939 2023-06-29 20:31:57.717081 types_usd-23.5.1/stubs/pxr-stubs/UsdSkel/__init__.pyi
+-rw-r--r--   0        0        0     5408 2023-06-29 20:31:57.743163 types_usd-23.5.1/stubs/pxr-stubs/UsdUI/__init__.pyi
+-rw-r--r--   0        0        0    12148 2023-06-29 22:00:17.644565 types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/__init__.pyi
+-rw-r--r--   0        0        0     6228 2023-06-29 20:31:57.803834 types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi
+-rw-r--r--   0        0        0      417 2023-06-29 20:31:57.805305 types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/constantsGroup.pyi
+-rw-r--r--   0        0        0      331 2023-06-29 20:31:57.807512 types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/fixBrokenPixarSchemas.pyi
+-rw-r--r--   0        0        0       62 2023-06-29 20:31:57.808642 types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/toolPaths.pyi
+-rw-r--r--   0        0        0     2040 2023-06-29 20:31:57.815915 types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi
+-rw-r--r--   0        0        0      676 2023-06-29 20:31:57.818787 types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi
+-rw-r--r--   0        0        0     7574 2023-06-29 20:31:57.853635 types_usd-23.5.1/stubs/pxr-stubs/UsdVol/__init__.pyi
+-rw-r--r--   0        0        0     6887 2023-06-29 22:00:17.646984 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/__init__.pyi
+-rw-r--r--   0        0        0      577 2023-06-29 20:31:57.878849 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi
+-rw-r--r--   0        0        0      171 2023-06-29 20:31:57.879525 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterialUI.pyi
+-rw-r--r--   0        0        0      997 2023-06-29 20:31:57.882705 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi
+-rw-r--r--   0        0        0      156 2023-06-29 20:31:57.883323 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/adjustFreeCameraUI.pyi
+-rw-r--r--   0        0        0    18213 2023-06-29 20:31:57.912420 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/appController.pyi
+-rw-r--r--   0        0        0      644 2023-06-29 20:31:57.913615 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi
+-rw-r--r--   0        0        0     2019 2023-06-29 20:31:57.916891 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi
+-rw-r--r--   0        0        0      793 2023-06-29 20:31:57.917788 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi
+-rw-r--r--   0        0        0      168 2023-06-29 20:31:57.918378 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/attributeValueEditorUI.pyi
+-rw-r--r--   0        0        0     1882 2023-06-29 20:31:57.920882 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi
+-rw-r--r--   0        0        0     8022 2023-06-29 20:31:57.937793 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/common.pyi
+-rw-r--r--   0        0        0      281 2023-06-29 20:31:57.938593 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/configController.pyi
+-rw-r--r--   0        0        0     1603 2023-06-29 20:31:57.940940 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/customAttributes.pyi
+-rw-r--r--   0        0        0      601 2023-06-29 20:31:57.942185 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi
+-rw-r--r--   0        0        0      496 2023-06-29 20:31:57.943202 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/frameSlider.pyi
+-rw-r--r--   0        0        0     1835 2023-06-29 20:31:57.949208 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/freeCamera.pyi
+-rw-r--r--   0        0        0      640 2023-06-29 20:31:57.950271 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi
+-rw-r--r--   0        0        0     6154 2023-06-29 20:31:57.958125 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi
+-rw-r--r--   0        0        0     1446 2023-06-29 20:31:57.960440 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi
+-rw-r--r--   0        0        0      126 2023-06-29 20:31:57.960831 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/legendUtil.pyi
+-rw-r--r--   0        0        0      501 2023-06-29 20:31:57.961620 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/mainWindowUI.pyi
+-rw-r--r--   0        0        0      386 2023-06-29 20:31:57.962584 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/overridableLineEdit.pyi
+-rw-r--r--   0        0        0     1446 2023-06-29 20:31:57.967427 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/plugin.pyi
+-rw-r--r--   0        0        0      522 2023-06-29 20:31:57.971994 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/preferences.pyi
+-rw-r--r--   0        0        0      141 2023-06-29 20:31:57.972928 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/preferencesUI.pyi
+-rw-r--r--   0        0        0       95 2023-06-29 20:31:57.973784 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/prettyPrint.pyi
+-rw-r--r--   0        0        0      348 2023-06-29 20:31:57.974984 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primContextMenu.pyi
+-rw-r--r--   0        0        0     2551 2023-06-29 20:31:57.979691 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi
+-rw-r--r--   0        0        0      618 2023-06-29 20:31:57.980684 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primLegend.pyi
+-rw-r--r--   0        0        0      138 2023-06-29 20:31:57.981474 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primLegendUI.pyi
+-rw-r--r--   0        0        0     3490 2023-06-29 20:31:57.988910 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi
+-rw-r--r--   0        0        0     2027 2023-06-29 20:31:57.993363 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primViewItem.pyi
+-rw-r--r--   0        0        0      650 2023-06-29 20:31:57.994376 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi
+-rw-r--r--   0        0        0      150 2023-06-29 20:31:57.995156 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/propertyLegendUI.pyi
+-rw-r--r--   0        0        0     3310 2023-06-29 20:31:58.002750 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi
+-rw-r--r--   0        0        0      213 2023-06-29 20:31:58.003604 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/qt.pyi
+-rw-r--r--   0        0        0     1246 2023-06-29 20:31:58.006497 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi
+-rw-r--r--   0        0        0      220 2023-06-29 20:31:58.007631 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/scalarTypes.pyi
+-rw-r--r--   0        0        0     5249 2023-06-29 20:31:58.030460 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi
+-rw-r--r--   0        0        0     1367 2023-06-29 20:31:58.036503 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/settings.pyi
+-rw-r--r--   0        0        0     7670 2023-06-29 20:31:58.051448 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/stageView.pyi
+-rw-r--r--   0        0        0     1720 2023-06-29 20:31:58.055267 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi
+-rw-r--r--   0        0        0       90 2023-06-29 20:31:58.056080 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/usdviewContextMenuItem.pyi
+-rw-r--r--   0        0        0      377 2023-06-29 20:31:58.056761 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/variantComboBox.pyi
+-rw-r--r--   0        0        0     3648 2023-06-29 20:31:58.062777 types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi
+-rw-r--r--   0        0        0   278095 2023-06-29 20:31:59.646254 types_usd-23.5.1/stubs/pxr-stubs/Vt/__init__.pyi
+-rw-r--r--   0        0        0      301 2023-06-29 20:31:59.649497 types_usd-23.5.1/stubs/pxr-stubs/Work/__init__.pyi
+-rw-r--r--   0        0        0      663 2023-06-29 22:00:17.642794 types_usd-23.5.1/stubs/pxr-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 types_usd-23.5.1/PKG-INFO
```

### Comparing `types-usd-23.5.0/README.md` & `types_usd-23.5.1/README.md`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/pyproject.toml` & `types_usd-23.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
-requires = ["poetry>=1.0.2"]
+requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "types-usd"
+version = "23.05.1"
+
 readme = "README.md"
 authors = ["Chad Dombrova"]
 description = "Unofficial python stubs for Pixar's Universal Scene Description (USD)"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
 ]
-version = "23.05.0"
 repository = "https://github.com/LumaPictures/cg-stubs"
 homepage = "https://github.com/LumaPictures/cg-stubs"
 
 keywords = ["3d", "graphics", "games", "VFX", "CG", "animation"]
 
 packages = [
     { include = "Boost-stubs", from = "stubs" },
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Ar/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Ar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/CameraUtil/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/CameraUtil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Garch/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Garch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/GeomUtil/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/GeomUtil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Gf/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Gf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Glf/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Glf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Kind/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Kind/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Ndr/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Ndr/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -62,22 +62,22 @@
     def __init__(self) -> None: ...
     def __reduce__(self) -> Any: ...
 
 class Node(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
     def GetContext(self) -> str: ...
     def GetFamily(self) -> str: ...
-    def GetIdentifier(self) -> Identifier: ...
+    def GetIdentifier(self) -> str: ...
     def GetInfoString(self) -> str: ...
     def GetInput(self, arg2: str | pxr.Ar.ResolvedPath) -> Property: ...
-    def GetInputNames(self) -> TokenVec: ...
+    def GetInputNames(self) -> list[str]: ...
     def GetMetadata(self) -> dict: ...
     def GetName(self) -> str: ...
     def GetOutput(self, arg2: str | pxr.Ar.ResolvedPath) -> Property: ...
-    def GetOutputNames(self) -> TokenVec: ...
+    def GetOutputNames(self) -> list[str]: ...
     def GetResolvedDefinitionURI(self) -> str: ...
     def GetResolvedImplementationURI(self) -> str: ...
     def GetSourceCode(self) -> str: ...
     def GetSourceType(self) -> str: ...
     def GetVersion(self) -> Version: ...
     def IsValid(self) -> bool: ...
     def __bool__(self) -> bool: ...
@@ -138,27 +138,27 @@
     def IsConnectable(self) -> bool: ...
     def IsDynamicArray(self) -> bool: ...
     def IsOutput(self) -> bool: ...
     def __reduce__(self) -> Any: ...
 
 class Registry(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
-    def GetAllNodeSourceTypes(self) -> TokenVec: ...
-    def GetNodeByIdentifier(self, identifier: Identifier, typePriority: TokenVec = ...) -> Node: ...
-    def GetNodeByIdentifierAndType(self, identifier: Identifier, nodeType: str | pxr.Ar.ResolvedPath) -> Node: ...
-    def GetNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: TokenVec = ..., filter: VersionFilter = ...) -> Node: ...
+    def GetAllNodeSourceTypes(self) -> list[str]: ...
+    def GetNodeByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ...) -> Node: ...
+    def GetNodeByIdentifierAndType(self, identifier: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath) -> Node: ...
+    def GetNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ..., filter: VersionFilter = ...) -> Node: ...
     def GetNodeByNameAndType(self, name: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath, filter: VersionFilter = ...) -> Node: ...
-    def GetNodeFromAsset(self, asset: pxr.Sdf.AssetPath | str, metadata: TokenMap = ..., subIdentifier: str | pxr.Ar.ResolvedPath = ..., sourceType: str | pxr.Ar.ResolvedPath = ...) -> Node: ...
-    def GetNodeFromSourceCode(self, sourceCode: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath, metadata: TokenMap = ...) -> Node: ...
-    def GetNodeIdentifiers(self, family: str | pxr.Ar.ResolvedPath = ..., filter: VersionFilter = ...) -> IdentifierVec: ...
-    def GetNodeNames(self, family: str | pxr.Ar.ResolvedPath = ...) -> StringVec: ...
+    def GetNodeFromAsset(self, asset: pxr.Sdf.AssetPath | str, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ..., subIdentifier: str | pxr.Ar.ResolvedPath = ..., sourceType: str | pxr.Ar.ResolvedPath = ...) -> Node: ...
+    def GetNodeFromSourceCode(self, sourceCode: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ...) -> Node: ...
+    def GetNodeIdentifiers(self, family: str | pxr.Ar.ResolvedPath = ..., filter: VersionFilter = ...) -> list[str]: ...
+    def GetNodeNames(self, family: str | pxr.Ar.ResolvedPath = ...) -> list[str]: ...
     def GetNodesByFamily(self, family: str | pxr.Ar.ResolvedPath = ..., filter: VersionFilter = ...) -> NodeList: ...
-    def GetNodesByIdentifier(self, identifier: Identifier) -> NodeList: ...
+    def GetNodesByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath) -> NodeList: ...
     def GetNodesByName(self, name: str | pxr.Ar.ResolvedPath, filter: VersionFilter = ...) -> NodeList: ...
-    def GetSearchURIs(self) -> StringVec: ...
+    def GetSearchURIs(self) -> list[str]: ...
     def SetExtraDiscoveryPlugins(self, arg2: list) -> None: ...
     def SetExtraParserPlugins(self, arg2: typing.Iterable[pxr.Tf.Type]) -> None: ...
     def __reduce__(self) -> Any: ...
 
 class Version(Boost.Python.instance):
     @overload
     def __init__(self, arg2: int, arg3: int) -> None: ...
@@ -222,11 +222,11 @@
     def __eq__(self, other: object) -> bool: ...
     def __lt__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     def __reduce__(self) -> Any: ...
     @property
     def expired(self) -> Any: ...
 
-def FsHelpersDiscoverFiles(searchPaths: StringVec, allowedExtensions: StringVec, followSymlinks: bool = ...) -> list: ...
-def FsHelpersDiscoverNodes(searchPaths: StringVec, allowedExtensions: StringVec, followSymlinks: bool = ..., context: DiscoveryPluginContext = ...) -> tuple[NodeDiscoveryResultVec, DiscoveryPluginContext]: ...
+def FsHelpersDiscoverFiles(searchPaths: list[str] | list[pxr.Ar.ResolvedPath], allowedExtensions: list[str] | list[pxr.Ar.ResolvedPath], followSymlinks: bool = ...) -> list: ...
+def FsHelpersDiscoverNodes(searchPaths: list[str] | list[pxr.Ar.ResolvedPath], allowedExtensions: list[str] | list[pxr.Ar.ResolvedPath], followSymlinks: bool = ..., context: DiscoveryPluginContext = ...) -> tuple[NodeDiscoveryResultVec, DiscoveryPluginContext]: ...
 def FsHelpersSplitShaderIdentifier(identifier: str | pxr.Ar.ResolvedPath) -> tuple[str, str, Version]: ...
 def _ValidateProperty(arg1: Node, arg2: Property) -> _AnnotatedBool: ...
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Pcp/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Pcp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Plug/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Plug/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/PxOsd/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/PxOsd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Sdf/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Sdf/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1967,16 +1967,16 @@
     def __init__(self) -> None: ...
     @overload
     def ApplyOperations(self, arg2: object) -> Any: ...
     @overload
     def ApplyOperations(self, arg2: StringListOp) -> Any: ...
     def Clear(self) -> None: ...
     def ClearAndMakeExplicit(self) -> None: ...
-    def Create(self, prependedItems: object = ..., appendedItems: object = ..., deletedItems: object = ...) -> typing_extensions.Self: ...
-    def CreateExplicit(self, explicitItems: object = ...) -> typing_extensions.Self: ...
+    def Create(self, prependedItems: object = ..., appendedItems: object = ..., deletedItems: object = ...) -> StringListOp: ...
+    def CreateExplicit(self, explicitItems: object = ...) -> StringListOp: ...
     def GetAddedOrExplicitItems(self) -> Any: ...
     def GetAppliedItems(self) -> Any: ...
     def HasItem(self, arg2: object) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
     def __hash__(self) -> int: ...
     def __ne__(self, other: object) -> bool: ...
     def __reduce__(self) -> Any: ...
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Sdr/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Sdr/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -82,45 +82,45 @@
     Vector: ClassVar[Any] = ...  # read-only
     Vstruct: ClassVar[Any] = ...  # read-only
     def __init__(self, *args, **kwargs) -> None: ...
     def __reduce__(self) -> Any: ...
 
 class Registry(pxr.Ndr.Registry):
     def __init__(self) -> None: ...
-    def GetShaderNodeByIdentifier(self, identifier: pxr.Ndr.Identifier, typePriority: pxr.Ndr.TokenVec = ...) -> ShaderNode: ...
-    def GetShaderNodeByIdentifierAndType(self, identifier: pxr.Ndr.Identifier, nodeType: str | pxr.Ar.ResolvedPath) -> ShaderNode: ...
-    def GetShaderNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: pxr.Ndr.TokenVec = ..., filter: pxr.Ndr.VersionFilter = ...) -> ShaderNode: ...
+    def GetShaderNodeByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ...) -> ShaderNode: ...
+    def GetShaderNodeByIdentifierAndType(self, identifier: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath) -> ShaderNode: ...
+    def GetShaderNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ..., filter: pxr.Ndr.VersionFilter = ...) -> ShaderNode: ...
     def GetShaderNodeByNameAndType(self, name: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath, filter: pxr.Ndr.VersionFilter = ...) -> ShaderNode: ...
-    def GetShaderNodeFromAsset(self, shaderAsset: pxr.Sdf.AssetPath | str, metadata: pxr.Ndr.TokenMap = ..., subIdentifier: str | pxr.Ar.ResolvedPath = ..., sourceType: str | pxr.Ar.ResolvedPath = ...) -> ShaderNode: ...
-    def GetShaderNodeFromSourceCode(self, sourceCode: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath, metadata: pxr.Ndr.TokenMap = ...) -> ShaderNode: ...
+    def GetShaderNodeFromAsset(self, shaderAsset: pxr.Sdf.AssetPath | str, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ..., subIdentifier: str | pxr.Ar.ResolvedPath = ..., sourceType: str | pxr.Ar.ResolvedPath = ...) -> ShaderNode: ...
+    def GetShaderNodeFromSourceCode(self, sourceCode: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ...) -> ShaderNode: ...
     def GetShaderNodesByFamily(self, family: str | pxr.Ar.ResolvedPath = ..., filter: pxr.Ndr.VersionFilter = ...) -> ShaderNodeList: ...
-    def GetShaderNodesByIdentifier(self, identifier: pxr.Ndr.Identifier) -> ShaderNodeList: ...
+    def GetShaderNodesByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath) -> ShaderNodeList: ...
     def GetShaderNodesByName(self, name: str | pxr.Ar.ResolvedPath, filter: pxr.Ndr.VersionFilter = ...) -> ShaderNodeList: ...
     def __bool__(self) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
     def __lt__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     def __reduce__(self) -> Any: ...
     @property
     def expired(self) -> Any: ...
 
 class ShaderNode(pxr.Ndr.Node):
     def __init__(self, *args, **kwargs) -> None: ...
-    def GetAdditionalPrimvarProperties(self) -> pxr.Ndr.TokenVec: ...
-    def GetAllVstructNames(self) -> pxr.Ndr.TokenVec: ...
-    def GetAssetIdentifierInputNames(self) -> list: ...
+    def GetAdditionalPrimvarProperties(self) -> list[str]: ...
+    def GetAllVstructNames(self) -> list[str]: ...
+    def GetAssetIdentifierInputNames(self) -> list[str]: ...
     def GetCategory(self) -> str: ...
     def GetDefaultInput(self) -> ShaderProperty: ...
-    def GetDepartments(self) -> pxr.Ndr.TokenVec: ...
+    def GetDepartments(self) -> list[str]: ...
     def GetHelp(self) -> str: ...
     def GetImplementationName(self) -> str: ...
     def GetLabel(self) -> str: ...
-    def GetPages(self) -> pxr.Ndr.TokenVec: ...
-    def GetPrimvars(self) -> pxr.Ndr.TokenVec: ...
-    def GetPropertyNamesForPage(self, arg2: str | pxr.Ar.ResolvedPath) -> pxr.Ndr.TokenVec: ...
+    def GetPages(self) -> list[str]: ...
+    def GetPrimvars(self) -> list[str]: ...
+    def GetPropertyNamesForPage(self, arg2: str | pxr.Ar.ResolvedPath) -> list[str]: ...
     def GetRole(self) -> str: ...
     def GetShaderInput(self, arg2: str | pxr.Ar.ResolvedPath) -> ShaderProperty: ...
     def GetShaderOutput(self, arg2: str | pxr.Ar.ResolvedPath) -> ShaderProperty: ...
     def __reduce__(self) -> Any: ...
 
 class ShaderNodeList(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
@@ -143,14 +143,14 @@
     def GetImplementationName(self) -> str: ...
     def GetLabel(self) -> str: ...
     def GetOptions(self) -> list: ...
     def GetPage(self) -> str: ...
     def GetVStructConditionalExpr(self) -> str: ...
     def GetVStructMemberName(self) -> str: ...
     def GetVStructMemberOf(self) -> str: ...
-    def GetValidConnectionTypes(self) -> pxr.Ndr.TokenVec: ...
+    def GetValidConnectionTypes(self) -> list[str]: ...
     def GetWidget(self) -> str: ...
     def IsAssetIdentifier(self) -> bool: ...
     def IsDefaultInput(self) -> bool: ...
     def IsVStruct(self) -> bool: ...
     def IsVStructMember(self) -> bool: ...
     def __reduce__(self) -> Any: ...
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Tf/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Tf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Trace/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Trace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usd/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usd/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     def GetClipManifestAssetPath(self, clipSet: str | pxr.Ar.ResolvedPath) -> pxr.Sdf.AssetPath: ...
     @overload
     def GetClipManifestAssetPath(self) -> pxr.Sdf.AssetPath: ...
     @overload
     def GetClipPrimPath(self, clipSet: str | pxr.Ar.ResolvedPath) -> str: ...
     @overload
     def GetClipPrimPath(self) -> str: ...
-    def GetClipSets(self) -> StringListOp: ...
+    def GetClipSets(self) -> pxr.Sdf.StringListOp: ...
     @overload
     def GetClipTemplateActiveOffset(self, clipSet: str | pxr.Ar.ResolvedPath) -> float: ...
     @overload
     def GetClipTemplateActiveOffset(self) -> float: ...
     @overload
     def GetClipTemplateAssetPath(self, clipSet: str | pxr.Ar.ResolvedPath) -> str: ...
     @overload
@@ -198,15 +198,15 @@
     def SetClipManifestAssetPath(self, manifestAssetPath: pxr.Sdf.AssetPath | str, clipSet: str | pxr.Ar.ResolvedPath) -> bool: ...
     @overload
     def SetClipManifestAssetPath(self, manifestAssetPath: pxr.Sdf.AssetPath | str) -> bool: ...
     @overload
     def SetClipPrimPath(self, primPath: str | pxr.Ar.ResolvedPath, clipSet: str | pxr.Ar.ResolvedPath) -> bool: ...
     @overload
     def SetClipPrimPath(self, primPath: str | pxr.Ar.ResolvedPath) -> bool: ...
-    def SetClipSets(self, clipSets: StringListOp) -> bool: ...
+    def SetClipSets(self, clipSets: pxr.Sdf.StringListOp) -> bool: ...
     @overload
     def SetClipTemplateActiveOffset(self, clipTemplateActiveOffset: float, clipSet: str | pxr.Ar.ResolvedPath) -> bool: ...
     @overload
     def SetClipTemplateActiveOffset(self, clipTemplateActiveOffset: float) -> bool: ...
     @overload
     def SetClipTemplateAssetPath(self, clipTemplateAssetPath: str | pxr.Ar.ResolvedPath, clipSet: str | pxr.Ar.ResolvedPath) -> None: ...
     @overload
@@ -437,26 +437,26 @@
     @classmethod
     def Get(cls, stage: Stage, path: pxr.Sdf.Path | str) -> ModelAPI: ...
     def GetAssetIdentifier(self) -> pxr.Sdf.AssetPath: ...
     def GetAssetInfo(self) -> dict: ...
     def GetAssetName(self) -> str: ...
     def GetAssetVersion(self) -> str: ...
     def GetKind(self) -> str: ...
-    def GetPayloadAssetDependencies(self) -> AssetPathArray: ...
+    def GetPayloadAssetDependencies(self) -> pxr.Sdf.AssetPathArray: ...
     @classmethod
     def GetSchemaAttributeNames(cls, includeInherited: bool = ...) -> list[str]: ...
     def IsGroup(self) -> bool: ...
     def IsKind(self, baseKind: str | pxr.Ar.ResolvedPath, validation: pxr.Kind.Validation = ...) -> bool: ...
     def IsModel(self) -> bool: ...
     def SetAssetIdentifier(self, arg2: pxr.Sdf.AssetPath | str) -> None: ...
     def SetAssetInfo(self, arg2: dict) -> None: ...
     def SetAssetName(self, arg2: str | pxr.Ar.ResolvedPath) -> None: ...
     def SetAssetVersion(self, arg2: str | pxr.Ar.ResolvedPath) -> None: ...
     def SetKind(self, value: str | pxr.Ar.ResolvedPath) -> bool: ...
-    def SetPayloadAssetDependencies(self, arg2: AssetPathArray) -> None: ...
+    def SetPayloadAssetDependencies(self, arg2: pxr.Sdf.AssetPathArray) -> None: ...
     @classmethod
     def _GetStaticTfType(cls) -> pxr.Tf.Type: ...
     def __bool__(self) -> bool: ...
     def __reduce__(self) -> Any: ...
 
 class Notice(Boost.Python.instance):
     class LayerMutingChanged(Notice.StageNotice):
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # mypy: disable_error_code = misc
 import Boost.Python
-import pxr.UsdAppUtils.cameraArgs as cameraArgs
-import pxr.UsdAppUtils.colorArgs as colorArgs
-import pxr.UsdAppUtils.complexityArgs as complexityArgs
-import pxr.UsdAppUtils.framesArgs as framesArgs
 import pxr.Ar
-import pxr.UsdAppUtils.rendererArgs as rendererArgs
+from . import cameraArgs as cameraArgs, colorArgs as colorArgs, complexityArgs as complexityArgs, framesArgs as framesArgs, rendererArgs as rendererArgs
 from typing import Any, ClassVar, overload
 
 class FrameRecorder(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
     @overload
     def __init__(self, arg2: object, arg3: bool) -> None: ...
     @overload
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdGeom/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdGeom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdHydra/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdHydra/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdImagingGL/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdImagingGL/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdLux/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdLux/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdMedia/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdMedia/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdPhysics/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdPhysics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdProc/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdProc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdRender/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdRender/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdRi/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdRi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdShade/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdShade/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     def GetConnectedSources(self) -> tuple[list[SourceInfo], list[pxr.Sdf.Path]]: ...
     def GetDisplayGroup(self) -> str: ...
     def GetDocumentation(self) -> str: ...
     def GetFullName(self) -> str: ...
     def GetPrim(self) -> pxr.Usd.Prim: ...
     def GetRawConnectedSourcePaths(self) -> list[pxr.Sdf.Path]: ...
     def GetRenderType(self) -> str: ...
-    def GetSdrMetadata(self) -> pxr.Ndr.TokenMap: ...
+    def GetSdrMetadata(self) -> dict[str, str]: ...
     def GetSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath) -> str: ...
     def GetTypeName(self) -> pxr.Sdf.ValueTypeName: ...
     def GetValueProducingAttribute(self) -> tuple[pxr.Usd.Attribute, AttributeType]: ...
     def GetValueProducingAttributes(self, shaderOutputsOnly: bool = ...) -> list[Attribute]: ...
     def HasConnectedSource(self) -> bool: ...
     def HasRenderType(self) -> bool: ...
     def HasSdrMetadata(self) -> bool: ...
@@ -219,15 +219,15 @@
     def IsSourceConnectionFromBaseMaterial(self) -> bool: ...
     def Set(self, value: object, time: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode = ...) -> bool: ...
     def SetConnectability(self, arg2: str | pxr.Ar.ResolvedPath) -> bool: ...
     def SetConnectedSources(self, arg2: typing.Iterable[ConnectionSourceInfo]) -> bool: ...
     def SetDisplayGroup(self, arg2: str | pxr.Ar.ResolvedPath) -> bool: ...
     def SetDocumentation(self, arg2: str | pxr.Ar.ResolvedPath) -> bool: ...
     def SetRenderType(self, renderType: str | pxr.Ar.ResolvedPath) -> bool: ...
-    def SetSdrMetadata(self, sdrMetadata: pxr.Ndr.TokenMap) -> None: ...
+    def SetSdrMetadata(self, sdrMetadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath]) -> None: ...
     def SetSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath, value: str | pxr.Ar.ResolvedPath) -> None: ...
     def __bool__(self) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     def __reduce__(self) -> Any: ...
 
 class Material(NodeGraph):
@@ -446,29 +446,29 @@
     def GetBaseName(self) -> str: ...
     def GetConnectedSource(self) -> tuple[ConnectableAPI, str, AttributeType]: ...
     def GetConnectedSources(self) -> tuple[list[SourceInfo], list[pxr.Sdf.Path]]: ...
     def GetFullName(self) -> str: ...
     def GetPrim(self) -> pxr.Usd.Prim: ...
     def GetRawConnectedSourcePaths(self) -> list[pxr.Sdf.Path]: ...
     def GetRenderType(self) -> str: ...
-    def GetSdrMetadata(self) -> pxr.Ndr.TokenMap: ...
+    def GetSdrMetadata(self) -> dict[str, str]: ...
     def GetSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath) -> str: ...
     def GetTypeName(self) -> pxr.Sdf.ValueTypeName: ...
     def GetValueProducingAttributes(self, shaderOutputsOnly: bool = ...) -> list[Attribute]: ...
     def HasConnectedSource(self) -> bool: ...
     def HasRenderType(self) -> bool: ...
     def HasSdrMetadata(self) -> bool: ...
     def HasSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath) -> bool: ...
     @classmethod
     def IsOutput(cls, arg1: pxr.Usd.Attribute | pxr.UsdGeom.ConstraintTarget | pxr.UsdGeom.Primvar | pxr.UsdGeom.XformOp | Input | Output) -> bool: ...
     def IsSourceConnectionFromBaseMaterial(self) -> bool: ...
     def Set(self, value: object, time: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode = ...) -> bool: ...
     def SetConnectedSources(self, arg2: typing.Iterable[ConnectionSourceInfo]) -> bool: ...
     def SetRenderType(self, renderType: str | pxr.Ar.ResolvedPath) -> bool: ...
-    def SetSdrMetadata(self, sdrMetadata: pxr.Ndr.TokenMap) -> None: ...
+    def SetSdrMetadata(self, sdrMetadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath]) -> None: ...
     def SetSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath, value: str | pxr.Ar.ResolvedPath) -> None: ...
     def __bool__(self) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     def __reduce__(self) -> Any: ...
 
 class Shader(pxr.Usd.Typed):
@@ -497,48 +497,48 @@
     def GetImplementationSourceAttr(self) -> pxr.Usd.Attribute: ...
     def GetInput(self, name: str | pxr.Ar.ResolvedPath) -> Input: ...
     def GetInputs(self, onlyAuthored: bool = ...) -> list[Input]: ...
     def GetOutput(self, name: str | pxr.Ar.ResolvedPath) -> Output: ...
     def GetOutputs(self, onlyAuthored: bool = ...) -> list[Output]: ...
     @classmethod
     def GetSchemaAttributeNames(cls, includeInherited: bool = ...) -> list[str]: ...
-    def GetSdrMetadata(self) -> pxr.Ndr.TokenMap: ...
+    def GetSdrMetadata(self) -> dict[str, str]: ...
     def GetSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath) -> str: ...
     def GetShaderId(self) -> str: ...
     def GetShaderNodeForSourceType(self, sourceType: str | pxr.Ar.ResolvedPath) -> pxr.Sdr.ShaderNode: ...
     def GetSourceAsset(self, sourceType: str | pxr.Ar.ResolvedPath = ...) -> pxr.Sdf.AssetPath: ...
     def GetSourceAssetSubIdentifier(self, sourceType: str | pxr.Ar.ResolvedPath = ...) -> str: ...
     def GetSourceCode(self, sourceType: str | pxr.Ar.ResolvedPath = ...) -> str: ...
     def HasSdrMetadata(self) -> bool: ...
     def HasSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath) -> bool: ...
-    def SetSdrMetadata(self, sdrMetadata: pxr.Ndr.TokenMap) -> None: ...
+    def SetSdrMetadata(self, sdrMetadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath]) -> None: ...
     def SetSdrMetadataByKey(self, key: str | pxr.Ar.ResolvedPath, value: str | pxr.Ar.ResolvedPath) -> None: ...
     def SetShaderId(self, arg2: str | pxr.Ar.ResolvedPath) -> bool: ...
     def SetSourceAsset(self, sourceAsset: pxr.Sdf.AssetPath | str, sourceType: str | pxr.Ar.ResolvedPath = ...) -> bool: ...
     def SetSourceAssetSubIdentifier(self, subIdentifier: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath = ...) -> bool: ...
     def SetSourceCode(self, sourceCode: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath = ...) -> bool: ...
     @classmethod
     def _GetStaticTfType(cls) -> pxr.Tf.Type: ...
     def __bool__(self) -> bool: ...
     def __reduce__(self) -> Any: ...
 
 class ShaderDefParserPlugin(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
     def __init__(self) -> None: ...
-    def GetDiscoveryTypes(self) -> pxr.Ndr.TokenVec: ...
+    def GetDiscoveryTypes(self) -> list[str]: ...
     def GetSourceType(self) -> str: ...
     def Parse(self, arg2: pxr.Ndr.NodeDiscoveryResult) -> pxr.Sdr.ShaderNode: ...
     def __reduce__(self) -> Any: ...
 
 class ShaderDefUtils(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
     @classmethod
     def GetNodeDiscoveryResults(cls, shaderDef: Shader, sourceUri: str | pxr.Ar.ResolvedPath) -> list: ...
     @classmethod
-    def GetPrimvarNamesMetadataString(cls, metadata: pxr.Ndr.TokenMap, shaderDef: ConnectableAPI) -> str: ...
+    def GetPrimvarNamesMetadataString(cls, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath], shaderDef: ConnectableAPI) -> str: ...
     @classmethod
     def GetShaderProperties(cls, shaderDef: ConnectableAPI) -> list: ...
     def __reduce__(self) -> Any: ...
 
 class Tokens(Boost.Python.instance):
     ConnectableAPI: ClassVar[Any] = ...  # read-only
     CoordSysAPI: ClassVar[Any] = ...  # read-only
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdSkel/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdSkel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdUI/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdUI/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # mypy: disable_error_code = misc
 import Boost.Python
-import pxr.UsdUtils.complianceChecker as complianceChecker
-import pxr.UsdUtils.constantsGroup as constantsGroup
-import pxr.UsdUtils.fixBrokenPixarSchemas as fixBrokenPixarSchemas
 import pxr.Usd
-import std
-import pxr.UsdUtils.toolPaths as toolPaths
 import typing
 import typing_extensions
-import pxr.UsdUtils.updateSchemaWithSdrNode as updateSchemaWithSdrNode
-import pxr.UsdUtils.usdzUtils as usdzUtils
+from . import complianceChecker as complianceChecker, constantsGroup as constantsGroup, fixBrokenPixarSchemas as fixBrokenPixarSchemas, toolPaths as toolPaths, updateSchemaWithSdrNode as updateSchemaWithSdrNode, usdzUtils as usdzUtils
 from pxr.UsdUtils.complianceChecker import ComplianceChecker as ComplianceChecker
 from pxr.UsdUtils.fixBrokenPixarSchemas import FixBrokenPixarSchemas as FixBrokenPixarSchemas
 from pxr.UsdUtils.updateSchemaWithSdrNode import PropertyDefiningKeys as PropertyDefiningKeys, SchemaDefiningKeys as SchemaDefiningKeys, SchemaDefiningMiscConstants as SchemaDefiningMiscConstants, UpdateSchemaWithSdrNode as UpdateSchemaWithSdrNode
 from pxr.UsdUtils.usdzUtils import CheckUsdzCompliance as CheckUsdzCompliance, CreateUsdzPackage as CreateUsdzPackage, ExtractUsdzPackage as ExtractUsdzPackage, UsdzAssetIterator as UsdzAssetIterator
 from typing import Any, ClassVar, overload
 
 class CoalescingDiagnosticDelegate(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
     def __init__(self) -> None: ...
     def DumpCoalescedDiagnosticsToStderr(self) -> None: ...
     def DumpCoalescedDiagnosticsToStdout(self) -> None: ...
     def DumpUncoalescedDiagnostics(self) -> None: ...
     def TakeCoalescedDiagnostics(self) -> list[CoalescingDiagnosticDelegate]: ...
-    def TakeUncoalescedDiagnostics(self) -> list[std.unique_ptr[pxr.Tf.DiagnosticBase]]: ...
+    def TakeUncoalescedDiagnostics(self) -> list[[pxr.Tf.DiagnosticBase]]: ...
     def __reduce__(self) -> Any: ...
 
 class CoalescingDiagnosticDelegateItem(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
     def __reduce__(self) -> Any: ...
     @property
     def sharedItem(self) -> Any: ...
```

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/UsdVol/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/UsdVol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/appController.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/appController.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/common.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/common.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/customAttributes.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/customAttributes.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/freeCamera.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/freeCamera.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/plugin.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/preferences.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/preferences.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primLegend.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primLegend.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/primViewItem.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/primViewItem.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/settings.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/settings.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/stageView.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/stageView.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/stubs/pxr-stubs/Vt/__init__.pyi` & `types_usd-23.5.1/stubs/pxr-stubs/Vt/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-usd-23.5.0/PKG-INFO` & `types_usd-23.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-usd
-Version: 23.5.0
+Version: 23.5.1
 Summary: Unofficial python stubs for Pixar's Universal Scene Description (USD)
 Home-page: https://github.com/LumaPictures/cg-stubs
 License: MIT
 Keywords: 3d,graphics,games,VFX,CG,animation
 Author: Chad Dombrova
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/LumaPictures/cg-stubs
 Description-Content-Type: text/markdown
 
 # Unofficial python stubs for Pixar's Universal Scene Description (USD)
 
 These stubs are designed to be used with a type checker like `mypy` to provide static type checking of USD python code, as well as to provide analysis and completion in IDEs like PyCharm and VSCode (with Pylance).
```

