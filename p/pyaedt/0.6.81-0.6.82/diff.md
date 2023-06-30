# Comparing `tmp/pyaedt-0.6.81.tar.gz` & `tmp/pyaedt-0.6.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.81.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.82.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.81.tar` & `pyaedt-0.6.82.tar`

### file list

```diff
@@ -1,255 +1,255 @@
--rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.81/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.81/README.md
--rw-r--r--   0        0        0     2691 2023-06-20 14:23:36.872281 pyaedt-0.6.81/pyaedt/__init__.py
--rw-r--r--   0        0        0    26639 2023-06-15 12:46:39.901353 pyaedt-0.6.81/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.81/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88300 2023-05-30 06:59:39.408947 pyaedt-0.6.81/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    50849 2023-06-20 08:09:46.074979 pyaedt-0.6.81/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17066 2023-05-30 06:59:39.408947 pyaedt-0.6.81/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.81/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19852 2023-05-30 06:59:39.408947 pyaedt-0.6.81/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.81/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   129864 2023-06-20 08:09:46.074979 pyaedt-0.6.81/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75524 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36749 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62954 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/circuit.py
--rw-r--r--   0        0        0    10247 2023-06-05 09:04:16.749339 pyaedt-0.6.81/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    66220 2023-06-15 12:26:55.582508 pyaedt-0.6.81/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.81/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.81/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.81/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.81/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.81/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.81/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.81/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.81/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.81/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.81/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.81/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.81/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.81/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23390 2023-06-14 08:50:43.463988 pyaedt-0.6.81/pyaedt/downloads.py
--rw-r--r--   0        0        0   136953 2023-06-14 08:50:43.463988 pyaedt-0.6.81/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-30 06:59:39.533962 pyaedt-0.6.81/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    92327 2023-06-19 08:11:10.842965 pyaedt-0.6.81/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.81/pyaedt/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    31497 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     7909 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48210 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.81/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    33195 2023-06-12 08:05:31.703949 pyaedt-0.6.81/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40100 2023-05-30 06:59:39.533962 pyaedt-0.6.81/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.81/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.81/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20386 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     6471 2023-06-19 10:47:11.266974 pyaedt-0.6.81/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61171 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    33851 2023-06-05 15:29:29.398358 pyaedt-0.6.81/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0   102298 2023-06-14 08:50:43.463988 pyaedt-0.6.81/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    34575 2023-06-19 10:47:11.266974 pyaedt-0.6.81/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.81/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.81/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    66975 2023-06-05 14:54:59.797581 pyaedt-0.6.81/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    47125 2023-06-05 14:54:59.797581 pyaedt-0.6.81/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.81/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    44030 2023-06-05 14:54:59.797581 pyaedt-0.6.81/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    47600 2023-06-05 14:54:59.797581 pyaedt-0.6.81/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    58809 2023-06-19 10:47:11.266974 pyaedt-0.6.81/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   109207 2023-06-05 09:36:43.953828 pyaedt-0.6.81/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11500 2023-06-13 17:56:07.965688 pyaedt-0.6.81/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     2813 2023-06-13 17:56:07.965688 pyaedt-0.6.81/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     1621 2023-06-13 17:56:07.965688 pyaedt-0.6.81/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    13412 2023-06-19 07:39:29.041489 pyaedt-0.6.81/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    12135 2023-06-20 07:19:24.495111 pyaedt-0.6.81/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-30 06:59:39.580847 pyaedt-0.6.81/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83444 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3395 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    69591 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.81/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   253082 2023-06-05 09:04:16.749339 pyaedt-0.6.81/pyaedt/hfss.py
--rw-r--r--   0        0        0    83113 2023-06-14 08:50:43.479555 pyaedt-0.6.81/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   176567 2023-06-19 10:47:11.266974 pyaedt-0.6.81/pyaedt/icepak.py
--rw-r--r--   0        0        0   123195 2023-06-20 09:57:37.687262 pyaedt-0.6.81/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24316 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3818 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-05-30 06:59:39.612097 pyaedt-0.6.81/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.81/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120888 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   198210 2023-06-12 13:34:18.085852 pyaedt-0.6.81/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116638 2023-06-15 12:26:55.582508 pyaedt-0.6.81/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11387 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   127857 2023-06-12 13:34:18.085852 pyaedt-0.6.81/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    31589 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49138 2023-06-19 10:57:53.404671 pyaedt-0.6.81/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59754 2023-06-19 10:57:53.404671 pyaedt-0.6.81/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53131 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12645 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42629 2023-05-30 06:59:39.643351 pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32781 2023-06-13 17:56:07.965688 pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8212 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63100 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15149 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    32013 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6952 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    59936 2023-05-30 14:16:58.540805 pyaedt-0.6.81/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    32822 2023-06-12 12:40:51.791945 pyaedt-0.6.81/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    50072 2023-06-16 12:23:10.021333 pyaedt-0.6.81/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65639 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23689 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   150771 2023-06-20 09:57:37.687262 pyaedt-0.6.81/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.81/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28363 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53226 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11976 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26538 2023-06-20 09:57:37.687262 pyaedt-0.6.81/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   179764 2023-06-19 07:39:29.041489 pyaedt-0.6.81/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   121445 2023-06-15 12:26:55.582508 pyaedt-0.6.81/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    29109 2023-06-16 06:33:37.387383 pyaedt-0.6.81/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125905 2023-06-19 07:39:29.057110 pyaedt-0.6.81/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95908 2023-05-30 06:59:39.674599 pyaedt-0.6.81/pyaedt/q3d.py
--rw-r--r--   0        0        0    10581 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.81/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-05-30 06:59:39.690227 pyaedt-0.6.81/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4410 2023-06-20 14:05:04.117219 pyaedt-0.6.81/pyproject.toml
--rw-r--r--   0        0        0    15552 1970-01-01 00:00:00.000000 pyaedt-0.6.81/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.82/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.82/README.md
+-rw-r--r--   0        0        0     2691 2023-06-30 08:45:32.173961 pyaedt-0.6.82/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26639 2023-06-15 12:39:09.822780 pyaedt-0.6.82/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88301 2023-06-21 14:18:52.796067 pyaedt-0.6.82/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    50849 2023-06-20 08:45:57.577348 pyaedt-0.6.82/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17066 2023-05-29 06:50:01.462409 pyaedt-0.6.82/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19852 2023-05-29 06:50:01.462409 pyaedt-0.6.82/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-29 06:50:01.462409 pyaedt-0.6.82/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   129864 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75524 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36750 2023-06-29 10:10:15.395808 pyaedt-0.6.82/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62954 2023-05-26 06:18:30.544561 pyaedt-0.6.82/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10247 2023-06-05 09:37:00.357207 pyaedt-0.6.82/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    65852 2023-06-29 13:44:57.328647 pyaedt-0.6.82/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1086 2023-06-29 10:10:15.395808 pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23390 2023-06-14 08:55:18.804330 pyaedt-0.6.82/pyaedt/downloads.py
+-rw-r--r--   0        0        0   137623 2023-06-29 16:42:04.115357 pyaedt-0.6.82/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    93329 2023-06-29 16:42:04.115357 pyaedt-0.6.82/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    31497 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     7909 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48210 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    33195 2023-06-12 08:03:15.118737 pyaedt-0.6.82/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40100 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      867 2023-05-26 06:18:30.544561 pyaedt-0.6.82/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12243 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65661 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20386 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     6856 2023-06-21 10:09:02.405348 pyaedt-0.6.82/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61171 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32590 2023-06-29 17:19:42.860399 pyaedt-0.6.82/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0   102298 2023-06-14 08:55:18.804330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36324 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    34575 2023-06-19 09:51:41.631657 pyaedt-0.6.82/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     3923 2023-06-05 14:55:02.766448 pyaedt-0.6.82/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2432 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    68725 2023-06-29 10:33:27.694259 pyaedt-0.6.82/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2850 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-29 06:50:01.493602 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-29 06:50:01.493602 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-29 06:50:01.493602 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21800 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47176 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33310 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    44030 2023-06-05 14:55:02.766448 pyaedt-0.6.82/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    48356 2023-06-29 12:57:01.275697 pyaedt-0.6.82/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    58809 2023-06-19 09:51:41.631657 pyaedt-0.6.82/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   109207 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11500 2023-06-14 05:38:07.853286 pyaedt-0.6.82/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     2813 2023-06-14 05:38:07.853286 pyaedt-0.6.82/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     1621 2023-06-14 05:38:07.853286 pyaedt-0.6.82/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-19 05:07:06.470308 pyaedt-0.6.82/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    13412 2023-06-17 11:56:24.503714 pyaedt-0.6.82/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    12252 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-26 11:30:35.579837 pyaedt-0.6.82/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83444 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-26 06:18:30.560187 pyaedt-0.6.82/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3395 2023-05-19 12:41:50.180833 pyaedt-0.6.82/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    69462 2023-06-29 10:10:15.395808 pyaedt-0.6.82/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11405 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3536 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   253082 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/hfss.py
+-rw-r--r--   0        0        0    83113 2023-06-14 08:55:18.804330 pyaedt-0.6.82/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   199927 2023-06-29 13:44:57.328647 pyaedt-0.6.82/pyaedt/icepak.py
+-rw-r--r--   0        0        0   126473 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24316 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3818 2023-05-19 06:53:58.810568 pyaedt-0.6.82/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120888 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   198276 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116971 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11387 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   129118 2023-06-29 17:19:42.860399 pyaedt-0.6.82/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    38399 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49138 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59754 2023-06-19 10:57:25.606048 pyaedt-0.6.82/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53131 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12645 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42629 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32781 2023-06-29 21:55:15.328018 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8212 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63170 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15149 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    32043 2023-06-29 19:22:14.082088 pyaedt-0.6.82/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6952 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    59936 2023-05-30 06:01:38.290945 pyaedt-0.6.82/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    32895 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    50072 2023-06-16 13:14:31.523832 pyaedt-0.6.82/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    66136 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23762 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   150771 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71535 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28517 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53616 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11976 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    27635 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   180536 2023-06-23 13:22:55.453306 pyaedt-0.6.82/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64120 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   121445 2023-06-15 11:58:34.060146 pyaedt-0.6.82/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    30706 2023-06-29 10:10:15.427058 pyaedt-0.6.82/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   126124 2023-06-23 13:22:55.453306 pyaedt-0.6.82/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95908 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10410 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4556 2023-06-30 08:45:32.173961 pyaedt-0.6.82/pyproject.toml
+-rw-r--r--   0        0        0    15772 1970-01-01 00:00:00.000000 pyaedt-0.6.82/PKG-INFO
```

### Comparing `pyaedt-0.6.81/LICENSE` & `pyaedt-0.6.82/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/README.md` & `pyaedt-0.6.82/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/__init__.py` & `pyaedt-0.6.82/pyaedt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.81"
+__version__ = "0.6.82"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
```

### Comparing `pyaedt-0.6.81/pyaedt/aedt_logger.py` & `pyaedt-0.6.82/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.82/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/Analysis.py` & `pyaedt-0.6.82/pyaedt/application/Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -2049,15 +2049,15 @@
             # DesignVariations = "$AmbientTemp=\'22cel\' $PowerIn=\'100\'"
         # array containing "SetupName:SolutionName" pairs (note that setup and solution are separated by a colon)
         SolutionSelectionArray = [solution_name + ":" + sweep_name]
         # 2=tab delimited spreadsheet (.tab), 3= touchstone (.sNp), 4= CitiFile (.cit),
         # 7=Matlab (.m), 8=Terminal Z0 spreadsheet
         FileFormat = 3
         OutFile = filename  # full path of output file
-        # array containin the frequencies to export, use ["all"] for all frequencies
+        # array containing the frequencies to export, use ["all"] for all frequencies
         FreqsArray = ["all"]
         DoRenorm = True  # perform renormalization before export
         RenormImped = 50  # Real impedance value in ohm, for renormalization
         DataType = "S"  # Type: "S", "Y", or "Z" matrix to export
         Pass = -1  # The pass to export. -1 = export all passes.
         ComplexFormat = 0  # 0=Magnitude/Phase, 1=Real/Immaginary, 2=dB/Phase
         DigitsPrecision = 15  # Touchstone number of digits precision
```

### Comparing `pyaedt-0.6.81/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.82/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.82/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.82/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.82/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.82/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.82/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/Design.py` & `pyaedt-0.6.82/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/JobManager.py` & `pyaedt-0.6.82/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/Variables.py` & `pyaedt-0.6.82/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.82/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/application/design_solutions.py` & `pyaedt-0.6.82/pyaedt/application/design_solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             "default_adaptive": "Transient",
             "intrinsics": ["Time"],
         },
         "TransientAPhiFormulation": {
             "name": "TransientAPhiFormulation",
             "options": None,
             "report_type": "Transient",
-            "default_setup": 5,
+            "default_setup": 56,
             "default_adaptive": "Transient",
             "intrinsics": ["Time"],
         },
         "Electrostatic": {
             "name": "Electrostatic",
             "options": None,
             "report_type": "Electrostatic",
```

### Comparing `pyaedt-0.6.81/pyaedt/circuit.py` & `pyaedt-0.6.82/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/common_rpc.py` & `pyaedt-0.6.82/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/desktop.py` & `pyaedt-0.6.82/pyaedt/desktop.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,43 +79,34 @@
                 p.wait()
         else:
             with subprocess.Popen(
                 " ".join(command), env=my_env, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
             ) as p:
                 p.wait()
 
-    active = grpc_active_sessions(
-        settings.aedt_version, non_graphical=settings.non_graphical, student_version=settings.is_student
-    )
     _aedt_process_thread = threading.Thread(target=launch_desktop_on_port)
     _aedt_process_thread.daemon = True
     _aedt_process_thread.start()
     timeout = settings.desktop_launch_timeout
     k = 0
     while not _check_grpc_port(port):
         if k > timeout:  # pragma: no cover
+            active_s = active_sessions(student_version=settings.is_student)
+            for p in active_s:
+                if port == p[1]:
+                    try:
+                        os.kill(p[0], 9)
+                    except (OSError, PermissionError):
+                        pass
             if first_run:
                 port = _find_free_port()
                 return launch_aedt(full_path, non_graphical, port, first_run=False)
-            return False, port
+            return False, _find_free_port()
         time.sleep(1)
         k += 1
-    active_after = grpc_active_sessions(
-        settings.aedt_version, non_graphical=settings.non_graphical, student_version=settings.is_student
-    )
-    k = 0
-    time.sleep(1)
-    while len(active_after) == len(active):  # pragma: no cover
-        time.sleep(1)
-        active_after = grpc_active_sessions(
-            settings.aedt_version, non_graphical=settings.non_graphical, student_version=settings.is_student
-        )
-        if k > timeout:
-            return False, port
-        k += 1
     return True, port
 
 
 def launch_aedt_in_lsf(non_graphical, port):  # pragma: no cover
     """Launch AEDT in LSF in GRPC mode."""
     if settings.lsf_queue:
         command = [
@@ -177,17 +168,20 @@
         success = True
     finally:
         s.close()
     return success
 
 
 def _find_free_port():
-    with socket.socket() as s:
-        s.bind(("", 0))  # Bind to a free port provided by the host.
-        return s.getsockname()[1]  # Return the port number assigned.
+    from contextlib import closing
+
+    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
+        s.bind(("127.0.0.1", 0))
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        return s.getsockname()[1]
 
 
 def exception_to_desktop(ex_value, tb_data):  # pragma: no cover
     """Writes the trace stack to AEDT when a Python error occurs.
 
     The message is added to the AEDT global logger and to the log file (if present).
 
@@ -961,34 +955,30 @@
                 self.logger.error("Failed to start LSF job on machine: %s.", self.machine)
                 return
         elif new_aedt_session:
             installer = os.path.join(base_path, "ansysedt")
             if not is_linux:
                 installer = os.path.join(base_path, "ansysedt.exe")
             out, self.port = launch_aedt(installer, non_graphical, self.port)
-            if out:
-                ScriptEnv._doInitialize(version, None, False, non_graphical, self.machine, self.port)
-            else:
-                self.logger.error("Failed to start AEDT on port %s.", self.port)
-                return
+            ScriptEnv._doInitialize(version, None, not out, non_graphical, self.machine, self.port)
         else:
             ScriptEnv._doInitialize(version, None, new_aedt_session, non_graphical, self.machine, self.port)
-
         if "oAnsoftApplication" in dir(self._main):
             self._main.isoutsideDesktop = True
             self._main.oDesktop = self._main.oAnsoftApplication.GetAppDesktop()
             _proc = self._main.oDesktop.GetProcessID()
             if new_aedt_session:
                 message = "{} {} version started with process ID {}.".format(
                     version, "Student" if student_version else "", _proc
                 )
                 self.logger.info(message)
 
         else:
-            self.logger.warning("The gRPC plugin is not supported in AEDT versions earlier than 2022 R2.")
+            self.logger.error("Failed to connect to AEDT using gRPC plugin.")
+            self.logger.error("Check installation, license and environment variables.")
 
     def _set_logger_file(self):
         # Set up the log file in the AEDT project directory
         if settings.remote_api:
             project_dir = tempfile.gettempdir()
         elif "oDesktop" in dir(self._main):
             project_dir = self._main.oDesktop.GetProjectDirectory()
```

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'FontName'": "'Arial,'",*

 * * "'FooterText'": "'� Copyright (c) 2020, ANSYS Inc. unauthorised use, distribution or duplication "*

 * *                 "is prohibited'"}*

```diff
@@ -6,19 +6,19 @@
     "ChartWidth": 16,
     "CoverSpaceAfter": 0.5,
     "CoverSubTitleFontSize": 24,
     "CoverSubTitleSpaceAfter": 0.3,
     "CoverTitleFontSize": 28,
     "FontColor": "0x000000",
     "FontHeaderColor": "0x000000",
-    "FontName": "EricssonHilda,",
+    "FontName": "Arial,",
     "FooterDistance": 1.0,
     "FooterFontSize": 7,
     "FooterFontSizeCover": 9,
-    "FooterText": " Copyright (c) 2020, ANSYS Inc. unauthorised use, distribution or duplication is prohibited",
+    "FooterText": "\ufffd Copyright (c) 2020, ANSYS Inc. unauthorised use, distribution or duplication is prohibited",
     "HeaderDistance": 1.5,
     "HeaderFontSize": 7,
     "HeaderFontSizeCover": 7,
     "HeaderImageWidth": 2,
     "HeaderTableBorderWidth": 0.25,
     "LeftMargin": 1.0,
     "LeftMarginCover": 1.0,
```

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/downloads.py` & `pyaedt-0.6.82/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb.py` & `pyaedt-0.6.82/pyaedt/edb.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,19 @@
         for i, j in self.project_variables.items():
             all_vars[i] = j
         for i, j in self.design_variables.items():
             all_vars[i] = j
         return all_vars
 
     @property
+    def terminals(self):
+        """Get terminals belonging to active layout."""
+        return {i.GetName(): ExcitationPorts(self, i) for i in self.layout.terminals}
+
+    @property
     def excitations(self):
         """Get all layout excitations."""
         terms = [term for term in self.layout.terminals if int(term.GetBoundaryType()) == 0]
         terms = [i for i in terms if not i.IsReferenceTerminal()]
         temp = {}
         for ter in terms:
             if "BundleTerminal" in ter.GetType().ToString():
@@ -350,15 +355,17 @@
             else:
                 temp[ter.GetName()] = ExcitationPorts(self, ter)
         return temp
 
     @property
     def excitations_nets(self):
         """Get all excitations net names."""
-        return list(set([i.GetNet().GetName() for i in self.layout.terminals]))
+        names = list(set([i.GetNet().GetName() for i in self.layout.terminals]))
+        names = [i for i in names if i]
+        return names
 
     @property
     def sources(self):
         """Get all layout sources."""
         terms = [term for term in self.layout.terminals if int(term.GetBoundaryType()) in [3, 4, 7]]
         return {ter.GetName(): ExcitationSources(self, ter) for ter in terms}
 
@@ -1428,17 +1435,18 @@
         custom_extent_units="mm",
         include_partial_instances=False,
         keep_voids=True,
         check_terminals=False,
         include_pingroups=False,
         expansion_factor=0,
         maximum_iterations=10,
+        preserve_components_with_model=False,
     ):
-        """Create a cutout using an approach entirely based on pyaedt.
-        This new method replaces all legacy cutout methods in pyaedt.
+        """Create a cutout using an approach entirely based on PyAEDT.
+        This method replaces all legacy cutout methods in PyAEDT.
         It does in sequence:
         - delete all nets not in list,
         - create a extent of the nets,
         - check and delete all vias not in the extent,
         - check and delete all the primitives not in extent,
         - check and intersect all the primitives that intersect the extent.
 
@@ -1490,16 +1498,20 @@
             It requires ``check_terminals``.
         expansion_factor : int, optional
             The method computes a float representing the largest number between
             the dielectric thickness or trace width multiplied by the expansion_factor factor.
             The trace width search is limited to nets with ports attached. Works only if `use_pyaedt_cutout`.
             Default is `0` to disable the search.
         maximum_iterations : int, optional
-            Maximum number of iterations before stopping in searching for a cutout with an error.
+            Maximum number of iterations before stopping a search for a cutout with an error.
             Default is `10`.
+        preserve_components_with_model : bool, optional
+            Whether to preserve all pins of components that have associated models (Spice or NPort).
+            This parameter is applicable only for a PyAEDT cutout (except point list).
+
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         Examples
@@ -1578,14 +1590,15 @@
                         output_aedb_path=dummy_path,
                         remove_single_pin_components=remove_single_pin_components,
                         use_pyaedt_extent_computing=use_pyaedt_extent_computing,
                         extent_defeature=extent_defeature,
                         custom_extent_units=custom_extent_units,
                         check_terminals=check_terminals,
                         include_pingroups=include_pingroups,
+                        preserve_components_with_model=preserve_components_with_model,
                     )
                     if self.are_port_reference_terminals_connected():
                         if output_aedb_path:
                             self.save_edb_as(output_aedb_path)
                         else:
                             self.save_edb_as(legacy_path)
                         working_cutout = True
@@ -1614,14 +1627,15 @@
                     output_aedb_path=output_aedb_path,
                     remove_single_pin_components=remove_single_pin_components,
                     use_pyaedt_extent_computing=use_pyaedt_extent_computing,
                     extent_defeature=extent_defeature,
                     custom_extent_units=custom_extent_units,
                     check_terminals=check_terminals,
                     include_pingroups=include_pingroups,
+                    preserve_components_with_model=preserve_components_with_model,
                 )
             if result and not open_cutout_at_end and self.edbpath != legacy_path:
                 self.save_edb()
                 self.close_edb()
                 self.edbpath = legacy_path
                 self.open_edb()
             return result
@@ -1816,14 +1830,15 @@
         output_aedb_path=None,
         remove_single_pin_components=False,
         use_pyaedt_extent_computing=False,
         extent_defeature=0.0,
         custom_extent_units="mm",
         check_terminals=False,
         include_pingroups=True,
+        preserve_components_with_model=False,
     ):
         if is_ironpython:  # pragma: no cover
             self.logger.error("Method working only in Cpython")
             return False
         from concurrent.futures import ThreadPoolExecutor
 
         if output_aedb_path:
@@ -1837,24 +1852,36 @@
                 reference_list = self.nets.netlist[::]
                 all_list = reference_list
             else:
                 reference_list = reference_list + signal_list
                 all_list = reference_list
         else:
             all_list = signal_list + reference_list
+        pins_to_preserve = []
+        nets_to_preserve = []
+        if preserve_components_with_model:
+            for el in self.components.instances.values():
+                if el.model_type in ["SPICEModel", "SParameterModel", "NetlistModel"] and list(
+                    set(el.nets[:]) & set(signal_list[:])
+                ):
+                    pins_to_preserve.extend([i.id for i in el.pins.values()])
+                    nets_to_preserve.extend(el.nets)
+
         for i in self.nets.nets.values():
-            if i.name not in all_list:
+            name = i.name
+            if name not in all_list and name not in nets_to_preserve:
                 i.net_object.Delete()
         reference_pinsts = []
         reference_prims = []
         for i in self.padstacks.instances.values():
             net_name = i.net_name
-            if net_name not in all_list:
+            id = i.id
+            if net_name not in all_list and id not in pins_to_preserve:
                 i.delete()
-            elif net_name in reference_list:
+            elif net_name in reference_list and id not in pins_to_preserve:
                 reference_pinsts.append(i)
         for i in self.modeler.primitives:
             net_name = i.net_name
             if net_name not in all_list:
                 i.delete()
             elif net_name in reference_list and not i.is_void:
                 reference_prims.append(i)
@@ -1924,24 +1951,14 @@
                         list_void = []
                         if voids:
                             voids_data = [void.polygon_data for void in voids]
                             list_prims = subtract(p, voids_data)
                             for prim in list_prims:
                                 if not prim.IsNull():
                                     poly_to_create.append([prim, prim_1.layer_name, net, list_void])
-                            #
-                            # list_voids = intersect(p, voids_data)
-                            # for void_intersected in list_voids:
-                            #     if not void_intersected.IsNull():
-                            #         int_data_2 = p.GetIntersectionType(void_intersected)
-                            #         if int_data_2 == 2:
-                            #             list_void.append(void_intersected)
-                            #         elif int_data == 1 or int_data_2 > 2:
-                            #             p = subtract(p, void_intersected)[0]
-                            # poly_to_create.append([p, prim_1.layer_name, net, list_void])
                         else:
                             poly_to_create.append([p, prim_1.layer_name, net, list_void])
 
                 prims_to_delete.append(prim_1)
 
         def pins_clean(pinst):
             if not pinst.in_polygon(_poly, simple_check=True):
@@ -2098,15 +2115,15 @@
         """
         temp_edb_path = self.edbpath[:-5] + "_temp_aedb.aedb"
         shutil.copytree(self.edbpath, temp_edb_path)
         temp_edb = Edb(temp_edb_path)
         for via in list(temp_edb.padstacks.instances.values()):
             via.pin.Delete()
         if netlist:
-            nets = [net for net in temp_edb.layout.nets if net.name in netlist]
+            nets = [net.net_obj for net in temp_edb.layout.nets if net.name in netlist]
             _poly = temp_edb.layout.expanded_extent(
                 nets, self.edb_api.geometry.extent_type.Conforming, 0.0, True, True, 1
             )
         else:
             nets = [net.api_object for net in temp_edb.layout.nets if "gnd" in net.name.lower()]
             _poly = temp_edb.layout.expanded_extent(
                 nets, self.edb_api.geometry.extent_type.Conforming, 0.0, True, True, 1
@@ -2218,18 +2235,18 @@
             voids = []
         voids_to_add = []
         for circle in voids:
             if polygonData.GetIntersectionType(circle.primitive_object.GetPolygonData()) >= 3:
                 voids_to_add.append(circle)
 
         _netsClip = convert_py_list_to_net_list(_ref_nets)
-        net_signals = convert_py_list_to_net_list([], type(_ref_nets[0]))
+        # net_signals = convert_py_list_to_net_list([], type(_ref_nets[0]))
 
         # Create new cutout cell/design
-        _cutout = self.active_cell.CutOut(net_signals, _netsClip, polygonData)
+        _cutout = self.active_cell.CutOut(_netsClip, _netsClip, polygonData)
         layout = _cutout.GetLayout()
         cutout_obj_coll = list(layout.PadstackInstances)
         ids = []
         for lobj in cutout_obj_coll:
             ids.append(lobj.GetId())
 
         if include_partial_instances:
```

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/components.py` & `pyaedt-0.6.82/pyaedt/edb_core/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -667,38 +667,34 @@
             if not positive_pin_group:  # pragma: no cover
                 return False
             negative_pin_group = self.create_pingroup_from_pins(negative_pins)
             if not negative_pin_group:  # pragma: no cover
                 return False
             if source.source_type == SourceType.Vsource:  # pragma: no cover
                 positive_pin_group_term = self._create_pin_group_terminal(
-                    positive_pin_group, source.positive_node.component
-                )
-                negative_pin_group_term = self._create_pin_group_terminal(
-                    negative_pin_group, source.negative_node.component, isref=True
+                    positive_pin_group,
                 )
+                negative_pin_group_term = self._create_pin_group_terminal(negative_pin_group, isref=True)
                 positive_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
                 negative_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
                 term_name = source.name
                 positive_pin_group_term.SetName(term_name)
                 negative_pin_group_term.SetName("{}_ref".format(term_name))
                 positive_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
                 negative_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
                 positive_pin_group_term.SetSourcePhase(self._get_edb_value(source.phase))
                 negative_pin_group_term.SetSourcePhase(self._get_edb_value(source.phase))
                 positive_pin_group_term.SetImpedance(self._get_edb_value(source.impedance))
                 negative_pin_group_term.SetImpedance(self._get_edb_value(source.impedance))
                 positive_pin_group_term.SetReferenceTerminal(negative_pin_group_term)
             elif source.source_type == SourceType.Isource:  # pragma: no cover
                 positive_pin_group_term = self._create_pin_group_terminal(
-                    positive_pin_group, source.positive_node.component
-                )
-                negative_pin_group_term = self._create_pin_group_terminal(
-                    negative_pin_group, source.negative_node.component, isref=True
+                    positive_pin_group,
                 )
+                negative_pin_group_term = self._create_pin_group_terminal(negative_pin_group, isref=True)
                 positive_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
                 negative_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
                 term_name = source.name
                 positive_pin_group_term.SetName(term_name)
                 negative_pin_group_term.SetName("{}_ref".format(term_name))
                 positive_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
                 negative_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
@@ -780,21 +776,28 @@
                 if cmp_ref_pin:
                     ref_cmp_pins.append(cmp_ref_pin[0])
             if not ref_cmp_pins:
                 return
             reference_pins = ref_cmp_pins
         if not len([pin for pin in reference_pins if isinstance(pin, EDBPadstackInstance)]) == len(reference_pins):
             return
-        group_name = "group_{}_{}".format(pins[0].net_name, pins[0].name)
-        ref_group_name = "group_{}_{}_ref".format(pins[0].net_name, pins[0].name)
-        pin_group = self.create_pingroup_from_pins(pins, group_name)
-        ref_pin_group = self.create_pingroup_from_pins(reference_pins, ref_group_name)
-        term = self._create_pin_group_terminal(pingroup=pin_group, component=refdes.refdes)
+        if len(pins) > 1:
+            group_name = "group_{}_{}".format(pins[0].net_name, pins[0].name)
+            pin_group = self.create_pingroup_from_pins(pins, group_name)
+            term = self._create_pin_group_terminal(pingroup=pin_group)
+
+        else:
+            term = self._create_terminal(pins[0])
         term.SetIsCircuitPort(True)
-        ref_term = self._create_pin_group_terminal(pingroup=ref_pin_group, component=refdes.refdes)
+        if len(reference_pins) > 1:
+            ref_group_name = "group_{}_{}_ref".format(reference_pins[0].net_name, reference_pins[0].name)
+            ref_pin_group = self.create_pingroup_from_pins(reference_pins, ref_group_name)
+            ref_term = self._create_pin_group_terminal(pingroup=ref_pin_group)
+        else:
+            ref_term = self._create_terminal(reference_pins[0])
         ref_term.SetIsCircuitPort(True)
         term.SetImpedance(self._edb.utility.value(impedance))
         term.SetReferenceTerminal(ref_term)
         if term:
             return term
         return False
 
@@ -895,44 +898,44 @@
                     self.create_terminal = self._create_terminal(ref_pins[0])
                     self.terminal = self.create_terminal
                     ref_pin_group_term = self.terminal
                 else:
                     ref_pin_group = self.create_pingroup_from_pins(ref_pins)
                     if not ref_pin_group:
                         return False
-                    ref_pin_group_term = self._create_pin_group_terminal(ref_pin_group, component, isref=True)
+                    ref_pin_group_term = self._create_pin_group_terminal(ref_pin_group, isref=True)
                     if not ref_pin_group_term:
                         return False
                 for net in net_list:
                     pins = [pin for pin in cmp_pins if pin.GetNet().GetName() == net]
                     if pins:
                         if len(pins) == 1:
                             pin_term = self._create_terminal(pins[0])
                             if pin_term:
                                 pin_term.SetReferenceTerminal(ref_pin_group_term)
                         else:
                             pin_group = self.create_pingroup_from_pins(pins)
                             if not pin_group:
                                 return False
-                            pin_group_term = self._create_pin_group_terminal(pin_group, component)
+                            pin_group_term = self._create_pin_group_terminal(pin_group)
                             if pin_group_term:
                                 pin_group_term.SetReferenceTerminal(ref_pin_group_term)
                     else:
                         self._logger.info("No pins found on component {} for the net {}".format(component, net))
             else:
                 ref_pin_group = self.create_pingroup_from_pins(ref_pins)
                 if not ref_pin_group:
                     self._logger.warning("failed to create reference pin group")
                     return False
-                ref_pin_group_term = self._create_pin_group_terminal(ref_pin_group, component, isref=True)
+                ref_pin_group_term = self._create_pin_group_terminal(ref_pin_group, isref=True)
                 for net in net_list:
                     pins = [pin for pin in cmp_pins if pin.GetNet().GetName() == net]
                     for pin in pins:
                         pin_group = self.create_pingroup_from_pins([pin])
-                        pin_group_term = self._create_pin_group_terminal(pin_group, component, isref=False)
+                        pin_group_term = self._create_pin_group_terminal(pin_group, isref=False)
                         pin_group_term.SetReferenceTerminal(ref_pin_group_term)
         return True
 
     @pyaedt_function_handler()
     def _create_terminal(self, pin):
         """Create terminal on component pin.
 
@@ -948,14 +951,17 @@
         pin_position = self.get_pin_position(pin)  # pragma no cover
         pin_pos = self._pedb.point_data(*pin_position)
         res, from_layer, _ = pin.GetLayerRange()
         cmp_name = pin.GetComponent().GetName()
         net_name = pin.GetNet().GetName()
         pin_name = pin.GetName()
         term_name = "{}.{}.{}".format(cmp_name, pin_name, net_name)
+        for term in list(self._pedb.active_layout.Terminals):
+            if term.GetName() == term_name:
+                return term
         term = self._edb.cell.terminal.PointTerminal.Create(
             pin.GetLayout(), pin.GetNet(), term_name, pin_pos, from_layer
         )
         return term
 
     @pyaedt_function_handler()
     def _get_closest_pin_from(self, pin, ref_pinlist):
@@ -1090,42 +1096,31 @@
             neg_pin_term.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.PortBoundary)
             neg_pin_term.SetIsCircuitPort(True)
             pos_pin_term.SetReferenceTerminal(neg_pin_term)
             self._logger.info("Component {} has been replaced by port".format(component.refdes))
             return True
 
     @pyaedt_function_handler()
-    def _create_pin_group_terminal(self, pingroup, component=None, isref=False):
+    def _create_pin_group_terminal(self, pingroup, isref=False):
         """Creates an EDB pin group terminal from a given EDB pin group.
 
         Parameters
         ----------
         pingroup : Edb pin group.
 
-        component : str or EdbComponent
-
         isref : bool
 
         Returns
         -------
         Edb pin group terminal.
         """
-        if component:
-            if not isinstance(component, self._pedb.edb_api.cell.hierarchy.component):
-                cmp_name = component
-            else:
-                cmp_name = component.GetName()
-        else:
-            cmp_name = pingroup.GetComponent().GetName()
-        net_name = pingroup.GetNet().GetName()
-        pin_name = list(pingroup.GetPins())[0].GetName()  # taking first pin name as convention.
-        if cmp_name:
-            term_name = "{0}.{1}.{2}".format(cmp_name, pin_name, net_name)
-        else:
-            term_name = "{0}.{1}".format(pin_name, net_name)
+        term_name = "{}_T".format(pingroup.GetName())
+        for t in list(self._pedb.active_layout.Terminals):
+            if t.GetName() == term_name:
+                return t
         pingroup_term = self._edb.cell.terminal.PinGroupTerminal.Create(
             self._active_layout, pingroup.GetNet(), term_name, pingroup, isref
         )
         return pingroup_term
 
     @pyaedt_function_handler()
     def _is_top_component(self, cmp):
@@ -1491,31 +1486,56 @@
                 pins = _pins
         if group_name is None:
             group_name = self._edb.cell.hierarchy.pin_group.GetUniqueName(self._active_layout)
         for pin in pins:
             pin.SetIsLayoutPin(True)
         forbiden_car = "-><"
         group_name = group_name.translate({ord(i): "_" for i in forbiden_car})
+        for pgroup in list(self._pedb.active_layout.PinGroups):
+            if pgroup.GetName() == group_name:
+                pin_group_exists = True
+                if len(pgroup.GetPins()) == len(pins):
+                    pnames = [i.GetName() for i in pins]
+                    for p in pgroup.GetPins():
+                        if p.GetName() in pnames:
+                            continue
+                        else:
+                            group_name = self._edb.cell.hierarchy.pin_group.GetUniqueName(
+                                self._active_layout, group_name
+                            )
+                            pin_group_exists = False
+                else:
+                    group_name = self._edb.cell.hierarchy.pin_group.GetUniqueName(self._active_layout, group_name)
+                    pin_group_exists = False
+                if pin_group_exists:
+                    return pgroup
         pingroup = _retry_ntimes(
             10,
             self._edb.cell.hierarchy.pin_group.Create,
             self._active_layout,
             group_name,
             convert_py_list_to_net_list(pins),
         )
         if pingroup.IsNull():
             return False
         else:
             pingroup.SetNet(pins[0].GetNet())
             return pingroup
 
     @pyaedt_function_handler()
-    def delete_single_pin_rlc(self):
+    def delete_single_pin_rlc(self, deactivate_only=False):
+        # type: (bool) -> list
         """Delete all RLC components with a single pin.
 
+        Parameters
+        ----------
+        deactivate_only : bool, optional
+            Whether to only deactivate RLC components with a single point rather than
+            delete them. The default is ``False``, in which case they are deleted.
+
         Returns
         -------
         list
             List of deleted RLC components.
 
 
         Examples
@@ -1526,17 +1546,21 @@
         >>> list_of_deleted_rlcs = edbapp.components.delete_single_pin_rlc()
         >>> print(list_of_deleted_rlcs)
 
         """
         deleted_comps = []
         for comp, val in self.instances.items():
             if val.numpins < 2 and val.type in ["Resistor", "Capacitor", "Inductor"]:
-                val.edbcomponent.Delete()
-                deleted_comps.append(comp)
-        self.refresh_components()
+                if deactivate_only:
+                    val.is_enabled = False
+                else:
+                    val.edbcomponent.Delete()
+                    deleted_comps.append(comp)
+        if not deactivate_only:
+            self.refresh_components()
         self._pedb._logger.info("Deleted {} components".format(len(deleted_comps)))
 
         return deleted_comps
 
     @pyaedt_function_handler()
     def delete_component(self, component_name):  # pragma: no cover
         """Delete a component.
```

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/dotnet/database.py` & `pyaedt-0.6.82/pyaedt/edb_core/dotnet/database.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/dotnet/layout.py` & `pyaedt-0.6.82/pyaedt/edb_core/dotnet/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/dotnet/primitive.py` & `pyaedt-0.6.82/pyaedt/edb_core/dotnet/primitive.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,63 +121,70 @@
             if "GetWidth" in dir(prim):
                 width = prim.GetWidth()
                 if width < current_value:
                     current_value = width
         return current_value
 
     @pyaedt_function_handler
-    def get_extended_net(self, resistor_below=10, inductor_below=1, capacitor_above=1):
+    def get_extended_net(self, resistor_below=10, inductor_below=1, capacitor_above=1, exception_list=None):
+        # type: (int | float, int | float, int |float, list) -> dict
         """Get extended net and associated components.
 
         Parameters
         ----------
         resistor_below : int, float, optional
             Threshold of resistor value. Search extended net across resistors which has value lower than the threshold.
         inductor_below : int, float, optional
             Threshold of inductor value. Search extended net across inductances which has value lower than the
             threshold.
         capacitor_above : int, float, optional
             Threshold of capacitor value. Search extended net across capacitors which has value higher than the
             threshold.
+        exception_list : list, optional
+            List of components which bypass threshold check.
         Returns
         -------
         list[
             dict[str, :class: `pyaedt.edb_core.edb_data.nets_data.EDBNetsData`],
             dict[str, :class: `pyaedt.edb_core.edb_data.components_data.EDBComponent`],
             dict[str, :class: `pyaedt.edb_core.edb_data.components_data.EDBComponent`],
             ]
         Examples
         --------
         >>> from pyaedt import Edb
         >>> app = Edb()
         >>> app.nets["BST_V3P3_S5"].get_extended_net()
         """
+        if exception_list is None:
+            exception_list = []
         all_nets = self._app.nets.nets
         nets = {self.name: all_nets[self.name]}
         rlc_serial = {}
         comps = {}
 
-        def get_net_list(net_name, _net_list, _rlc_serial, _comp):
+        def get_net_list(net_name, _net_list, _rlc_serial, _comp, exception_list):
             edb_net = all_nets[net_name]
             for refdes, val in edb_net.components.items():
                 if not val.is_enabled:
                     continue
 
-                if val.type == "Inductor" and val.value < inductor_below and val.is_enabled:
+                if refdes in exception_list:
+                    pass
+                elif val.type == "Inductor" and val.value < inductor_below and val.is_enabled:
                     pass
                 elif val.type == "Resistor" and val.value < resistor_below and val.is_enabled:
                     pass
                 elif val.type == "Capacitor" and val.value > capacitor_above and val.is_enabled:
                     pass
                 else:
                     _comp[refdes] = val
                     continue
 
                 _rlc_serial[refdes] = val
                 for net in val.nets:
                     if net not in _net_list:
                         _net_list[net] = all_nets[net]
-                        get_net_list(net, _net_list, _rlc_serial, _comp)
+                        get_net_list(net, _net_list, _rlc_serial, _comp, exception_list)
 
-        get_net_list(self.name, nets, rlc_serial, comps)
+        get_net_list(self.name, nets, rlc_serial, comps, exception_list)
 
         return [nets, rlc_serial, comps]
```

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,24 +135,27 @@
         -------
         str
         """
         return self.layer.GetName()
 
     @layer_name.setter
     def layer_name(self, val):
-        if val in self._core_stackup.stackup_layers.layers:
-            lay = self._core_stackup.stackup_layers.layers[val]._edb_layer
-            self.primitive_object.SetLayer(lay)
-        elif not isinstance(val, str):
+        if isinstance(val, str) and val in list(self._core_stackup.layers.keys()):
+            lay = self._core_stackup.layers["TOP"]._edb_layer
+            if lay:
+                self.primitive_object.SetLayer(lay)
+            else:
+                raise AttributeError("Layer {} not found in layer".format(val))
+        elif isinstance(val, type(self._core_stackup.layers["TOP"])):
             try:
-                self.primitive_object.SetLayer(val)
+                self.primitive_object.SetLayer(val._edb_layer)
             except:
-                raise AttributeError("Value inserted not found. Input has to be layer name or layer object.")
+                raise AttributeError("Failed to assign new layer on primitive.")
         else:
-            raise AttributeError("Value inserted not found. Input has to be layer name or layer object.")
+            raise AttributeError("Invalid input value")
 
 
 class EDBPrimitives(EDBPrimitivesMain):
     """Manages EDB functionalities for a primitives.
     It Inherits EDB Object properties.
 
     Examples
@@ -389,72 +392,41 @@
         -------
         List of :class:`pyaedt.edb_core.edb_data.EDBPrimitives`
         """
         poly = self.primitive_object.GetPolygonData()
         if not isinstance(primitives, list):
             primitives = [primitives]
         primi_polys = []
+        voids_of_prims = []
         for prim in primitives:
             if isinstance(prim, EDBPrimitives):
                 primi_polys.append(prim.primitive_object.GetPolygonData())
+                for void in prim.voids:
+                    voids_of_prims.append(void.polygon_data)
             else:
                 try:
                     primi_polys.append(prim.GetPolygonData())
                 except:
                     primi_polys.append(prim)
-        list_poly = poly.Subtract(convert_py_list_to_net_list([poly]), convert_py_list_to_net_list(primi_polys))
+        for v in self.voids[:]:
+            primi_polys.append(v.polygon_data)
+        primi_polys = poly.Unite(convert_py_list_to_net_list(primi_polys))
+        p_to_sub = poly.Unite(convert_py_list_to_net_list([poly] + voids_of_prims))
+        list_poly = poly.Subtract(p_to_sub, primi_polys)
         new_polys = []
         if list_poly:
-            voids = self.voids
             for p in list_poly:
                 if p.IsNull():
                     continue
-                list_void = []
-                void_to_subtract = []
-                if voids:
-                    for void in voids:
-                        void_pdata = void.polygon_data
-                        int_data2 = p.GetIntersectionType(void_pdata)
-                        if int_data2 > 2 or int_data2 == 1:
-                            void_to_subtract.append(void_pdata)
-                        elif int_data2 == 2:
-                            list_void.append(void_pdata)
-                    if void_to_subtract:
-                        polys_cleans = p.Subtract(
-                            convert_py_list_to_net_list(p), convert_py_list_to_net_list(void_to_subtract)
-                        )
-                        for polys_clean in polys_cleans:
-                            if not polys_clean.IsNull():
-                                void_to_append = [v for v in list_void if polys_clean.GetIntersectionType(v) == 2]
-                                new_polys.append(
-                                    cast(
-                                        self._app.modeler.create_polygon(
-                                            polys_clean, self.layer_name, net_name=self.net_name, voids=void_to_append
-                                        ),
-                                        self._app,
-                                    )
-                                )
-                    else:
-                        new_polys.append(
-                            cast(
-                                self._app.modeler.create_polygon(
-                                    p, self.layer_name, net_name=self.net_name, voids=list_void
-                                ),
-                                self._app,
-                            )
-                        )
-                else:
-                    new_polys.append(
-                        cast(
-                            self._app.modeler.create_polygon(
-                                p, self.layer_name, net_name=self.net_name, voids=list_void
-                            ),
-                            self._app,
-                        )
-                    )
+            new_polys.append(
+                cast(
+                    self._app.modeler.create_polygon(p, self.layer_name, net_name=self.net_name, voids=[]),
+                    self._app,
+                )
+            )
         self.delete()
         for prim in primitives:
             if isinstance(prim, EDBPrimitives):
                 prim.delete()
             else:
                 try:
                     prim.Delete()
@@ -493,15 +465,15 @@
             for p in list_poly:
                 if p.IsNull():
                     continue
                 list_void = []
                 void_to_subtract = []
                 if voids:
                     for void in voids:
-                        void_pdata = void.primitive_object.GetPolygonData()
+                        void_pdata = void.prim_obj.GetPolygonData()
                         int_data2 = p.GetIntersectionType(void_pdata)
                         if int_data2 > 2 or int_data2 == 1:
                             void_to_subtract.append(void_pdata)
                         elif int_data2 == 2:
                             list_void.append(void_pdata)
                     if void_to_subtract:
                         polys_cleans = p.Subtract(
@@ -811,14 +783,20 @@
         bool
             ``True`` when successful, ``False`` when failed.
         """
         cloned_poly = self._app.edb_api.cell.primitive.polygon.create(
             self._app.active_layout, self.layer_name, self.net, self.polygon_data
         )
         if cloned_poly:
+            for void in self.voids:
+                cloned_void = self._app.edb_api.cell.primitive.polygon.create(
+                    self._app.active_layout, self.layer_name, self.net, void.polygon_data
+                )
+                # cloned_void
+                cloned_poly.prim_obj.AddVoid(cloned_void.prim_obj)
             return cloned_poly
         return False
 
     @pyaedt_function_handler()
     def in_polygon(
         self,
         point_data,
```

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.82/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/general.py` & `pyaedt-0.6.82/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.82/pyaedt/edb_core/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -938,17 +938,16 @@
         else:
             return False
 
     @pyaedt_function_handler()
     def create_lumped_port_on_net(
         self, nets=None, reference_layer=None, return_points_only=False, digit_resolution=6, at_bounding_box=True
     ):
-        """Create an edge port on nets. Only ports on traces (e.g. Path) are currently supported.
-        The command will look for traces on the nets and will try to assign vertical lumped port on first and last
-        point from the trace. To be used with cautious.
+        """Create an edge port on nets. This command looks for traces and polygons on the
+        nets and tries to assign vertical lumped port.
 
         Parameters
         ----------
         nets : list, optional
             List of nets, str or Edb net.
 
         reference_layer : str, Edb layer.
@@ -980,55 +979,84 @@
             temp_nets = []
             for nn in nets:
                 if isinstance(nn, str):
                     temp_nets.append(self._edb.cell.net.find_by_name(self._active_layout, nn))
                 elif isinstance(nn, self._edb.cell.net.net):
                     temp_nets.append(nn)
             nets = temp_nets
+        port_created = False
         if nets:
             edges_pts = []
             if isinstance(reference_layer, str):
                 try:
                     reference_layer = self._pedb.stackup.signal_layers[reference_layer]._edb_layer
                 except:
                     raise Exception("Failed to get the layer {}".format(reference_layer))
             if not isinstance(reference_layer, self._edb.Cell.ILayerReadOnly):
                 return False
             layout = nets[0].GetLayout()
-            layout_bbox = self.get_layout_bounding_box(layout, digit_resolution)
+            layout_bbox = self._pedb.get_conformal_polygon_from_netlist(self._pedb.nets.netlist)
+            layout_extent_segments = [pt for pt in list(layout_bbox.GetArcData()) if pt.IsSegment()]
+            first_pt = layout_extent_segments[0]
+            layout_extent_points = [
+                [first_pt.Start.X.ToDouble(), first_pt.End.X.ToDouble()],
+                [first_pt.Start.Y.ToDouble(), first_pt.End.Y.ToDouble()],
+            ]
+            for segment in layout_extent_segments[1:]:
+                end_point = (segment.End.X.ToDouble(), segment.End.Y.ToDouble())
+                layout_extent_points[0].append(end_point[0])
+                layout_extent_points[1].append(end_point[1])
             for net in nets:
-                net_primitives = list(net.Primitives)
-                net_paths = [
-                    pp for pp in net_primitives if pp.GetPrimitiveType() == self._edb.cell.primitive.PrimitiveType.Path
-                ]
+                net_primitives = self._pedb.nets[net.name].primitives
+                net_paths = [pp for pp in net_primitives if pp.type == "Path"]
                 for path in net_paths:
-                    trace_path_pts = list(path.GetCenterLine().Points)
+                    trace_path_pts = list(path.center_line.Points)
                     port_name = "{}_{}".format(net.name, path.GetId())
                     for pt in trace_path_pts:
                         _pt = [
                             round(pt.X.ToDouble(), digit_resolution),
                             round(pt.Y.ToDouble(), digit_resolution),
                         ]
                         if at_bounding_box:
-                            if not set(layout_bbox).isdisjoint(_pt):
+                            if GeometryOperators.point_in_polygon(_pt, layout_extent_points) == 0:
                                 if return_points_only:
                                     edges_pts.append(_pt)
                                 else:
-                                    term = self._create_edge_terminal(path, pt, port_name)  # pragma no cover
+                                    term = self._create_edge_terminal(path.id, pt, port_name)  # pragma no cover
                                     term.SetReferenceLayer(reference_layer)  # pragma no cover
+                                    port_created = True
                         else:
                             if return_points_only:  # pragma: no cover
                                 edges_pts.append(_pt)
                             else:
-                                term = self._create_edge_terminal(path, pt, port_name)
+                                term = self._create_edge_terminal(path.id, pt, port_name)
                                 term.SetReferenceLayer(reference_layer)
-
+                                port_created = True
+                net_poly = [pp for pp in net_primitives if pp.type == "Polygon"]
+                for poly in net_poly:
+                    poly_segment = [aa for aa in poly.arcs if aa.is_segment]
+                    for segment in poly_segment:
+                        if (
+                            GeometryOperators.point_in_polygon(
+                                [segment.mid_point.X.ToDouble(), segment.mid_point.Y.ToDouble()], layout_extent_points
+                            )
+                            == 0
+                        ):
+                            if return_points_only:
+                                edges_pts.append(segment.mid_point)
+                            else:
+                                port_name = "{}_{}".format(net.name, poly.GetId())
+                                term = self._create_edge_terminal(
+                                    poly.id, segment.mid_point, port_name
+                                )  # pragma no cover
+                                term.SetReferenceLayer(reference_layer)  # pragma no cover
+                                port_created = True
             if return_points_only:
                 return edges_pts
-        return True
+        return port_created
 
     @pyaedt_function_handler()
     def create_vertical_circuit_port_on_clipped_traces(self, nets=None, reference_net=None, user_defined_extent=None):
         """Create an edge port on clipped signal traces.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/layout.py` & `pyaedt-0.6.82/pyaedt/edb_core/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,16 @@
             Dictionary of primitives with layer names as keys.
         """
         _primitives_by_layer = {}
         for lay in self.layers:
             _primitives_by_layer[lay] = []
         for i in self._layout.primitives:
             lay = i.GetLayer().GetName()
+            if not lay:
+                continue
             _primitives_by_layer[lay].append(cast(i, self._pedb))
         return _primitives_by_layer
 
     @property
     def rectangles(self):
         """Rectangles.
```

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/materials.py` & `pyaedt-0.6.82/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/nets.py` & `pyaedt-0.6.82/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.82/pyaedt/edb_core/padstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -810,35 +810,38 @@
         has_hole=True,
         pad_offset_x="0.0",
         pad_offset_y="0.0",
         pad_rotation="0.0",
         start_layer=None,
         stop_layer=None,
         add_default_layer=False,
+        anti_pad_x_size="600um",
+        anti_pad_y_size="600um",
     ):
         """Create a padstack.
 
         Parameters
         ----------
         padstackname : str, optional
             Name of the padstack. The default is ``None``.
         holediam : str, optional
             Diameter of the hole with units. The default is ``"300um"``.
         paddiam : str, optional
-            Diameter of the pad with units. The default is ``"400um"``.
+            Diameter of the pad with units, used with ``"Circle"`` shape. The default is ``"400um"``.
         antipaddiam : str, optional
             Diameter of the antipad with units. The default is ``"600um"``.
         pad_shape : str, optional
             Shape of the pad. The default is ``"Circle``. Options are ``"Circle"`` and ``"Rectangle"``.
         antipad_shape : str, optional
-            Shape of the antipad. The default is ``"Circle"``. Options are ``"Circle"`` and ``"Bullet"``.
+            Shape of the antipad. The default is ``"Circle"``. Options are ``"Circle"`` ``"Rectangle"`` and
+            ``"Bullet"``.
         x_size : str, optional
-            Only applicable to bullet shape. The default is ``"600um"``.
+            Only applicable to bullet and rectangle shape. The default is ``"600um"``.
         y_size : str, optional
-            Only applicable to bullet shape. The default is ``"600um"``.
+            Only applicable to bullet and rectangle shape. The default is ``"600um"``.
         corner_radius :
             Only applicable to bullet shape. The default is ``"300um"``.
         offset_x : str, optional
             X offset of antipad. The default is ``"0.0"``.
         offset_y : str, optional
             Y offset of antipad. The default is ``"0.0"``.
         rotation : str, optional
@@ -853,14 +856,18 @@
             Padstack rotation.
         start_layer : str, optional
             Start layer of the padstack definition.
         stop_layer : str, optional
             Stop layer of the padstack definition.
         add_default_layer : bool, optional
             Add ``"Default"`` to padstack definition. Default is ``False``.
+        anti_pad_x_size : str, optional
+            Only applicable to bullet and rectangle shape. The default is ``"600um"``.
+        anti_pad_y_size : str, optional
+            Only applicable to bullet and rectangle shape. The default is ``"600um"``.
 
         Returns
         -------
         str
             Name of the padstack if the operation is successful.
         """
         holediam = self._get_edb_value(holediam)
@@ -883,14 +890,16 @@
         offset_x = self._get_edb_value(offset_x)
         offset_y = self._get_edb_value(offset_y)
         rotation = self._get_edb_value(rotation)
 
         pad_offset_x = self._get_edb_value(pad_offset_x)
         pad_offset_y = self._get_edb_value(pad_offset_y)
         pad_rotation = self._get_edb_value(pad_rotation)
+        anti_pad_x_size = self._get_edb_value(anti_pad_x_size)
+        anti_pad_y_size = self._get_edb_value(anti_pad_y_size)
 
         padstackData.SetHoleParameters(ptype, holparam, value0, value0, value0)
 
         padstackData.SetHolePlatingPercentage(self._get_edb_value(20.0))
         padstackData.SetHoleRange(self._edb.definition.PadstackHoleRange.UpperPadToLowerPad)
         padstackData.SetMaterial("copper")
         layers = list(self._pedb.stackup.signal_layers.keys())[:]
@@ -903,14 +912,17 @@
             pad_shape = self._edb.definition.PadGeometryType.Circle
         elif pad_shape == "Rectangle":
             pad_array = Array[type(x_size)]([x_size, y_size])
             pad_shape = self._edb.definition.PadGeometryType.Rectangle
         if antipad_shape == "Bullet":
             antipad_array = Array[type(x_size)]([x_size, y_size, corner_radius])
             antipad_shape = self._edb.definition.PadGeometryType.Bullet
+        elif antipad_shape == "Rectangle":
+            antipad_array = Array[type(anti_pad_x_size)]([anti_pad_x_size, anti_pad_y_size])
+            antipad_shape = self._edb.definition.PadGeometryType.Rectangle
         else:
             antipad_array = Array[type(antipaddiam)]([antipaddiam])
             antipad_shape = self._edb.definition.PadGeometryType.Circle
         if add_default_layer:
             layers = layers + ["Default"]
         for layer in layers:
             # padparam_array = Array[type(paddiam)]([paddiam])
@@ -1024,15 +1036,15 @@
             is ``0``.
         fromlayer :
             The default is ``None``.
         tolayer :
             The default is ``None``.
         solderlayer :
             The default is ``None``.
-        is_pin : bool, optiona
+        is_pin : bool, optional
             Whether if the padstack is a pin or not. Default is `False`.
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.padstacks_data.EDBPadstackInstance`
         """
         padstack = None
```

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.82/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.82/pyaedt/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/emit.py` & `pyaedt-0.6.82/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.82/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.82/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.6.82/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.82/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.82/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.82/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.82/pyaedt/generic/LoadAEDTFile.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # --------------------------------------------------------------------
 # internals
 
 
 # precompile all Regular expressions
 _remove_quotes = re.compile(r"^'(.*?)'$")
 _split_list_elements = re.compile(",(?=(?:[^']*'[^']*')*[^']*$)")
-_round_bracket_list = re.compile(r"^(?P<SKEY1>\S+?)\((?P<LIST1>.+)\)|^'(?P<SKEY2>.+?\s.+)'(?<=')\((?P<LIST2>.+)\)")
+_round_bracket_list = re.compile(r"^(?P<SKEY1>[^\s=]+?)\((?P<LIST1>.+)\)|^'(?P<SKEY2>.+?\s.+)'(?<=')\((?P<LIST2>.+)\)")
 _square_bracket_list = re.compile(
     r"^(?P<SKEY1>\S+?)\[\d+:(?P<LIST1>.+)\]|^'(?P<SKEY2>.+?\s.+)'(?<=')\[\d+:(?P<LIST2>.+)\]"
 )
 _key_parse = re.compile(r"(^'(?P<KEY1>.+?)')(?<=')=(?P<VAL1>.+$)|(?P<KEY2>^.+?)=(?P<VAL2>.+$)")
 _value_parse1 = re.compile(r"\s")
 _value_parse2 = re.compile(r"^'([^']*\s[^']*)(?=')")
 _begin_search = re.compile(r"\$begin '(.+)'")
@@ -146,66 +146,27 @@
         m = _round_bracket_list.search(sk)
         if m and m.group("SKEY1") == "simple":  # extra verification. SKEY2 is with spaces, so it's not considered here.
             elems = _separate_list_elements(m.group("LIST1"))
             if elems[0] == "thermal_expansion_coeffcient":
                 elems[0] = "thermal_expansion_coefficient"  # fix a typo in the amat files. AEDT supports both strings!
             d[elems[0]] = str(elems[1])  # convert to string as it is dedicated to material props
             return True
-    elif "KeyIDMap(" in sk:
-        m = _round_bracket_list.search(sk)
-        if m and "IDMap" in m.group("SKEY1"):  # extra verification. SKEY2 is with spaces, so it's not considered here.
-            elems = m.group("LIST1").split(",")
-            d[m.group("SKEY1")] = elems  # convert to string as it is dedicated to material props
+    elif re.search(r"^\w+IDMap\(.*\)$", sk, re.IGNORECASE):  # check if the format is AAKeyIDMap('10'=56802, '7'=56803)
+        m = re.search(r"^(?P<SKEY>[^\s=]+?)\((?P<LIST>.*)\)", sk)
+        if m and "idmap" in m.group("SKEY").lower():  # extra verification.
+            k = m.group("SKEY")
+            if m.group("LIST"):
+                elems = m.group("LIST").split(",")
+            else:
+                elems = None
+            d[k] = elems
             return True
     return False
 
 
-def _decode_value_and_save(k, v, d):
-    """
-
-    Parameters
-    ----------
-    k :
-
-    v :
-
-    d :
-
-    """
-    # save key 'k', value 'v' in dict 'd'
-    # create a list for subkey(l1, l2, l3)
-    # create a list for subkey[n: 1, 2, ...n]
-    # send recognized sub-keys to _decode_recognized_subkeys
-    for rsk in _recognized_subkeys:
-        if rsk in k:  # here we simply search if one of the _recognized_subkeys is in k
-            if _decode_recognized_subkeys(k, d):  # the exact search is done inside the _decode_recognized_subkeys
-                return  # if there is a match we stop the _decode_value_and_save, otherwise we keep going
-    m = _round_bracket_list.search(k)
-    if m and m.group("SKEY1"):
-        v = _separate_list_elements(m.group("LIST1"))
-        k = m.group("SKEY1")
-        d[k] = v
-    elif m and m.group("SKEY2"):
-        v = _separate_list_elements(m.group("LIST2"))
-        k = m.group("SKEY2")
-        d[k] = v
-    else:
-        m = _square_bracket_list.search(k)
-        if m and m.group("SKEY1"):
-            v = _separate_list_elements(m.group("LIST1"))
-            k = m.group("SKEY1")
-            d[k] = v
-        elif m and m.group("SKEY2"):
-            v = _separate_list_elements(m.group("LIST2"))
-            k = m.group("SKEY2")
-            d[k] = v
-        else:
-            d[k] = _parse_value(v)
-
-
 def _decode_recognized_key(keyword, line, d):
     """Special decodings for keys belonging to  _recognized_keywords
 
     Parameters
     ----------
     keyword : str
         dictionary key recognized
@@ -235,62 +196,91 @@
             d["add"].append(line.replace("add", "").translate({ord(i): None for i in " ()'"}).split(","))
             _count += 1
             line = _all_lines[_count + 1]
     else:  # pragma: no cover
         raise AttributeError("Keyword {} is supposed to be in the recognized_keywords list".format(keyword))
 
 
-def _decode_key(line, d):
+def _decode_subkey(line, d):
     """
 
     Parameters
     ----------
     line : str
         Line.
 
     d : dict
         Active dictionary.
 
     -------
 
     """
+    # send recognized sub-keys to _decode_recognized_subkeys (Case insensitive search, detailed search is inside)
+    for rsk in _recognized_subkeys:
+        if rsk.lower() in line.lower():  # here we simply search if one of the _recognized_subkeys is in line
+            if _decode_recognized_subkeys(line, d):  # the exact search is done inside the _decode_recognized_subkeys
+                return  # if there is a match we stop the _decode_key, otherwise we keep going
+
+    # create a list for subkey(l1, l2, l3)
+    m = _round_bracket_list.search(line)
+    if m and m.group("SKEY1"):
+        v = _separate_list_elements(m.group("LIST1"))
+        k = m.group("SKEY1")
+        d[k] = v
+        return  # if there is a match we stop the _decode_key, otherwise we keep going
+    elif m and m.group("SKEY2"):
+        v = _separate_list_elements(m.group("LIST2"))
+        k = m.group("SKEY2")
+        d[k] = v
+        return  # if there is a match we stop the _decode_key, otherwise we keep going
+
+    # create a list for subkey[n: 1, 2, ...n]
+    m = _square_bracket_list.search(line)
+    if m and m.group("SKEY1"):
+        v = _separate_list_elements(m.group("LIST1"))
+        k = m.group("SKEY1")
+        d[k] = v
+        return  # if there is a match we stop the _decode_key, otherwise we keep going
+    elif m and m.group("SKEY2"):
+        v = _separate_list_elements(m.group("LIST2"))
+        k = m.group("SKEY2")
+        d[k] = v
+        return  # if there is a match we stop the _decode_key, otherwise we keep going
+
+    # search for equal sign
     m = _key_parse.search(line)
     if m and m.group("KEY1"):  # key btw ''
-        value = m.group("VAL1")
-        if "\\'" in value:
-            value2 = value.replace("\\'", '"')
+        v = m.group("VAL1")
+        if "\\'" in v:
+            v2 = v.replace("\\'", '"')
         else:
-            value2 = value
-        # if there are no spaces in value
-        if not _value_parse1.search(value2) or _value_parse2.search(value2):
-            # or values with spaces are between quote
-            key = m.group("KEY1")
-            _decode_value_and_save(key, value, d)
+            v2 = v
+        # if there are no spaces in value   or   values with spaces are between quotes
+        if not _value_parse1.search(v2) or _value_parse2.search(v2):
+            k = m.group("KEY1")
+            d[k] = _parse_value(v)
         else:  # spaces in value without quotes
-            key = line
-            value = None
-            _decode_value_and_save(key, value, d)
+            k = line  # save the line as a whole
+            d[k] = None
     elif m and m.group("KEY2"):  # key without ''
-        value = m.group("VAL2")
-        if "\\'" in value:
-            value2 = value.replace("\\'", '"')
+        v = m.group("VAL2")
+        if "\\'" in v:
+            v2 = v.replace("\\'", '"')
         else:
-            value2 = value
+            v2 = v
         # if there are no spaces in value   or   values with spaces are between quotes
-        if not _value_parse1.search(value2) or _value_parse2.search(value2):
-            key = m.group("KEY2")
-            _decode_value_and_save(key, value, d)
+        if not _value_parse1.search(v2) or _value_parse2.search(v2):
+            k = m.group("KEY2")
+            d[k] = _parse_value(v)
         else:  # spaces in value without quotes
-            key = line
-            value = None
-            _decode_value_and_save(key, value, d)
+            k = line  # save the line as a whole
+            d[k] = None
     else:  # no = sign found
-        key = line
-        value = None
-        _decode_value_and_save(key, value, d)
+        k = line  # save the line as a whole
+        d[k] = None
 
 
 def _walk_through_structure(keyword, save_dict):
     """
 
     Parameters
     ----------
@@ -309,18 +299,15 @@
     found = False
     saved_value = None
     while _count < _len_all_lines:
         line = _all_lines[_count]
         # begin_key is found
         if begin_key == line:
             found = True
-            saved_value = save_dict.get(keyword)  # if the keyword is already present
-            # makes the value a list, if it's not already
-            if saved_value and type(saved_value) is not list:
-                saved_value = [saved_value]
+            saved_value = save_dict.get(keyword)  # if the keyword is already present, save it
             save_dict[keyword] = {}
             _count += 1
             continue
         # end_key is found
         if end_key == line:
             break
         # between begin_key and end_key
@@ -328,18 +315,21 @@
             b = _begin_search.search(line)
             if b:  # walk down a level
                 nextlvl_begin_key = b.group(1)
                 _walk_through_structure(nextlvl_begin_key, save_dict[keyword])
             elif keyword in _recognized_keywords:
                 _decode_recognized_key(keyword, line, save_dict[keyword])
             else:  # decode key
-                _decode_key(line, save_dict[keyword])
+                _decode_subkey(line, save_dict[keyword])
         _count += 1
     # recompose value if list
     if saved_value:
+        # makes the value a list, if it's not already
+        if type(saved_value) is not list:
+            saved_value = [saved_value]
         saved_value.append(save_dict[keyword])
         save_dict[keyword] = saved_value
     return _count
 
 
 def _read_aedt_file(filename):
     """Read the entire AEDT file discard binary and put ascii line in a list
```

### Comparing `pyaedt-0.6.81/pyaedt/generic/clr_module.py` & `pyaedt-0.6.82/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/configurations.py` & `pyaedt-0.6.82/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/constants.py` & `pyaedt-0.6.82/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/design_types.py` & `pyaedt-0.6.82/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/filesystem.py` & `pyaedt-0.6.82/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/general_methods.py` & `pyaedt-0.6.82/pyaedt/generic/general_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,24 @@
 def _write_mes(mes_text):
     mes_text = str(mes_text)
     parts = [mes_text[i : i + 250] for i in range(0, len(mes_text), 250)]
     for el in parts:
         settings.logger.error(el)
 
 
+def _get_args_dicts(func, args, kwargs):
+    if int(sys.version[0]) > 2:
+        args_name = list(OrderedDict.fromkeys(inspect.getfullargspec(func)[0] + list(kwargs.keys())))
+        args_dict = OrderedDict(list(itertools.zip_longest(args_name, args)) + list(kwargs.items()))
+    else:
+        args_name = list(OrderedDict.fromkeys(inspect.getargspec(func)[0] + list(kwargs.keys())))
+        args_dict = OrderedDict(list(itertools.izip(args_name, args)) + list(kwargs.iteritems()))
+    return args_dict
+
+
 def _exception(ex_info, func, args, kwargs, message="Type Error"):
     """Write the trace stack to the desktop when a Python error occurs.
 
     Parameters
     ----------
     ex_info :
 
@@ -96,20 +106,15 @@
     if message_to_print:
         _write_mes("API Message - " + message_to_print)
     for el in tblist:
         if func.__name__ in el:
             _write_mes("{}, {}".format(el, message.upper()))
     args_name = []
     try:
-        if int(sys.version[0]) > 2:
-            args_name = list(OrderedDict.fromkeys(inspect.getfullargspec(func)[0] + list(kwargs.keys())))
-            args_dict = OrderedDict(list(itertools.zip_longest(args_name, args)) + list(kwargs.items()))
-        else:
-            args_name = list(OrderedDict.fromkeys(inspect.getargspec(func)[0] + list(kwargs.keys())))
-            args_dict = OrderedDict(list(itertools.izip(args_name, args)) + list(kwargs.iteritems()))
+        args_dict = _get_args_dicts(func, args, kwargs)
         first_time_log = True
 
         for el in args_dict:
             if el != "self" and args_dict[el]:
                 if first_time_log:
                     _write_mes("Method arguments: ")
                     first_time_log = False
@@ -162,15 +167,15 @@
         if not settings.enable_error_handler:
             result = user_function(*args, **kwargs)
             return result
         else:
             try:
                 settings.time_tick = time.time()
                 out = user_function(*args, **kwargs)
-                if settings.enable_debug_logger:
+                if settings.enable_debug_logger or settings.enable_debug_edb_logger:
                     _log_method(user_function, args, kwargs)
                 return out
             except TypeError:
                 _exception(sys.exc_info(), user_function, args, kwargs, "Type Error")
                 return False
             except ValueError:
                 _exception(sys.exc_info(), user_function, args, kwargs, "Value Error")
@@ -279,15 +284,14 @@
     if settings.remote_rpc_session:
         remote_path = remote_path.replace("\\", "/") if remote_path[0] != "\\" else remote_path
         settings.remote_rpc_session.filemanager.download_file(remote_path, local_path, overwrite=overwrite)
         return local_path
     return remote_path
 
 
-@pyaedt_function_handler()
 def check_if_path_exists(path):
     """Check whether a path exists or not local or remote machine (for remote sessions only).
 
     Parameters
     ----------
     path : str
         Local or remote path to check.
@@ -322,15 +326,14 @@
     if settings.remote_rpc_session:
         remote_path = remote_path.replace("\\", "/") if remote_path[0] != "\\" else remote_path
         settings.remote_rpc_session.filemanager.download_folder(remote_path, local_path, overwrite=overwrite)
         return local_path
     return remote_path
 
 
-@pyaedt_function_handler()
 def open_file(file_path, file_options="r"):
     """Open a file and return the object.
 
     Parameters
     ----------
     file_path : str
         Full absolute path to the file (either local or remote).
@@ -366,50 +369,42 @@
         return
     if (
         not settings.enable_debug_edb_logger
         and "Edb" in str(func) + str(new_args)
         or "edb_core" in str(func) + str(new_args)
     ):
         return
-    line_begin = "    Implicit Arguments: "
-    line_begin2 = "    Explicit Arguments: "
+    line_begin = "ARGUMENTS: "
     message = []
     delta = time.time() - settings.time_tick
     m, s = divmod(delta, 60)
     h, m = divmod(m, 60)
     d, h = divmod(h, 24)
     msec = (s - int(s)) * 1000
     if d > 0:
         time_msg = " {}days {}h {}m {}sec.".format(d, h, m, int(s))
     elif h > 0:
         time_msg = " {}h {}m {}sec.".format(h, m, int(s))
     else:
         time_msg = "  {}m {}sec {}msec.".format(m, int(s), int(msec))
-    if new_args and settings.enable_debug_methods_argument_logger:
-        object_name = str([new_args[0]])[1:-1]
-        id = object_name.find(" object at ")
-        if id >= 0:
+    if settings.enable_debug_methods_argument_logger:
+        args_dict = _get_args_dicts(func, new_args, new_kwargs)
+        id = 0
+        if new_args:
+            object_name = str([new_args[0]])[1:-1]
+            id = object_name.find(" object at ")
+        if id > 0:
             object_name = object_name[1:id]
-            message.append(" '{}' has been executed in {}".format(object_name + "." + str(func.__name__), time_msg))
-            if new_args[1:]:
-                message.append(line_begin + str(new_args[1:])[1:-1])
-            if new_kwargs:
-                message.append(line_begin2 + str(new_kwargs)[1:-1])
-
+            message.append("'{}' was run in {}".format(object_name + "." + str(func.__name__), time_msg))
         else:
-            message.append(" '{}' has been executed in {}".format(str(func.__name__), time_msg))
-            if new_args[1:]:
-                message.append(line_begin + str(new_args[1:])[1:-1])
-            if new_kwargs:
-                message.append(line_begin2 + str(new_kwargs)[1:-1])
-
-    else:
-        message.append(" '{}' has been executed in: {}".format(str(func.__name__), time_msg))
-        if new_kwargs and settings.enable_debug_methods_argument_logger:
-            message.append(line_begin2 + str(new_kwargs)[1:-1])
+            message.append("'{}' was run in {}".format(str(func.__name__), time_msg))
+        message.append(line_begin)
+        for k, v in args_dict.items():
+            if k != "self":
+                message.append("    {} = {}".format(k, v))
     for m in message:
         settings.logger.debug(m)
 
 
 @pyaedt_function_handler()
 def get_version_and_release(input_version):
     version = int(input_version[2:4])
@@ -652,15 +647,16 @@
 
     """
     retry = 0
     ret_val = None
     while retry < n:
         try:
             ret_val = function(*args, **kwargs)
-            if not ret_val and type(ret_val) is not float and type(ret_val) is not int:
+            if ret_val is None:
+                # if not ret_val and type(ret_val) not in [float, int, str, tuple, list]:
                 ret_val = True
         except:
             retry += 1
             time.sleep(0.5)
         else:
             break
     if retry == n:
@@ -1049,17 +1045,17 @@
 
     Returns
     -------
     list
         List of gRPC ports.
     """
     if student_version:
-        keys = ["ansysedtsv.exe"]
+        keys = ["ansysedtsv.exe", "ansysedtsv"]
     else:
-        keys = ["ansysedt.exe"]
+        keys = ["ansysedt.exe", "ansysedt"]
     if version and "." in version:
         version = version[-4:].replace(".", "")
     sessions = []
     for p in psutil.process_iter():
         try:
             if p.name() in keys:
                 cmd = p.cmdline()
@@ -1093,20 +1089,20 @@
 
     Returns
     -------
     list
         List of AEDT PIDs.
     """
     if student_version:
-        keys = ["ansysedtsv.exe"]
+        keys = ["ansysedtsv.exe", "ansysedtsv"]
     else:
-        keys = ["ansysedt.exe"]
+        keys = ["ansysedt.exe", "ansysedt"]
     if version and "." in version:
         version = version[-4:].replace(".", "")
-    if version < "222":
+    if version and version < "222":
         version = version[:2] + "." + version[2]
     sessions = []
     for p in psutil.process_iter():
         try:
             if p.name() in keys:
                 cmd = p.cmdline()
                 if non_graphical and "-ng" in cmd or not non_graphical:
@@ -1784,14 +1780,16 @@
         self._aedt_environment_variables = {
             "ANS_MESHER_PROC_DUMP_PREPOST_BEND_SM3": "1",
             "ANSYSEM_FEATURE_SF6694_NON_GRAPHICAL_COMMAND_EXECUTION_ENABLE": "1",
             "ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE": "1",
             "ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE": "1",
             "ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE": "1",
             "ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE": "1",
+            "ANSYSEM_FEATURE_F545177_ECAD_INTEGRATION_WITH_APHI_ENABLE": "1",
+            "ANSYSEM_FEATURE_F650636_MECH_LAYOUT_COMPONENT_ENABLE": "1",
         }
         if is_linux:
             self._aedt_environment_variables["ANS_NODEPCHECK"] = "1"
         self._desktop_launch_timeout = 90
         self._aedt_process_id = None
         self._is_student = False
```

### Comparing `pyaedt-0.6.81/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.82/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.82/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/pdf.py` & `pyaedt-0.6.82/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/plot.py` & `pyaedt-0.6.82/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/process.py` & `pyaedt-0.6.82/pyaedt/generic/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,11 +273,14 @@
             _exe = '"' + os.path.join(self.installer_path, "siwave.exe") + '"'
         command = [_exe]
         if hidden:
             command.append("-embedding")
         command.append("-RunScriptAndExit")
         command.append('"' + scriptname + '"')
         print(command)
+        if os.name == "posix":
+            p = subprocess.Popen(command)
 
-        subprocess.run(" ".join(command), check=True)
-
+        else:
+            p = subprocess.Popen(" ".join(command))
+        p.wait()
         return output_list
```

### Comparing `pyaedt-0.6.81/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.82/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.82/pyaedt/generic/report_file_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
+from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 from pyaedt.generic.constants import SI_UNITS
 from pyaedt.generic.constants import unit_system
 
 
 def parse_rdat_file(file_path):
     """
     Parse Ansys report .rdat file
 
     Returns:
         (dict) report data
     """
     report_dict = {}
-    data = load_entire_aedt_file(file_path)
+    # data = load_entire_aedt_file(file_path)
+    data = load_keyword_in_aedt_file(file_path, "ReportsData")
 
     report_data = data["ReportsData"]["RepMgrRepsData"]
     for report_name in report_data:
         report_dict[report_name] = {}
         for trace, trace_data in report_data[report_name]["Traces"].items():
             all_data = trace_data["TraceComponents"]["TraceDataComps"]["0"]
             if all_data["TraceDataCol"]["ParameterType"] == "ComplexParam":
```

### Comparing `pyaedt-0.6.81/pyaedt/generic/toolkit.py` & `pyaedt-0.6.82/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.82/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/hfss.py` & `pyaedt-0.6.82/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.82/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/icepak.py` & `pyaedt-0.6.82/pyaedt/icepak.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,14 +212,15 @@
         free_loss_coeff=True,
         free_area_ratio=0.8,
         resistance_type=0,
         external_temp="AmbientTemp",
         expternal_pressure="AmbientPressure",
         x_curve=["0", "1", "2"],
         y_curve=["0", "1", "2"],
+        boundary_name=None,
     ):
         """Assign grille to a face or list of faces.
 
         Parameters
         ----------
         air_faces : str, list
             List of face names.
@@ -240,26 +241,30 @@
             External temperature. The default is ``"AmbientTemp"``.
         expternal_pressure : str, optional
             External pressure. The default is ``"AmbientPressure"``.
         x_curve : list, optional
             List of X curves in m_per_sec. The default is ``["0", "1", "2"]``.
         y_curve : list
             List of Y curves in n_per_meter_q. The default is ``["0", "1", "2"]``.
+        boundary_name : str, optional
+            Boundary name. The default is ``None``, in which case the name will
+            be generated automatically.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object when successful or ``None`` when failed.
 
         References
         ----------
 
         >>> oModule.AssignGrilleBoundary
         """
-        boundary_name = generate_unique_name("Grille")
+        if boundary_name is None:
+            boundary_name = generate_unique_name("Grille")
 
         self.modeler.create_face_list(air_faces, "boundary_faces" + boundary_name)
         props = {}
         air_faces = self.modeler.convert_to_selections(air_faces, True)
 
         props["Faces"] = air_faces
         if free_loss_coeff:
@@ -533,16 +538,17 @@
         thermal_impedance="0celm2_per_w",
         bc_name=None,
     ):
         """Add a conductive plate thermal assignment on a face.
 
         Parameters
         ----------
-        face_id : int or str
-            If int, Face ID. If str, object name.
+        face_id : int or str or list
+            Integer indicating a face ID or a string indicating an object name. A list of face
+            IDs or object names is also accepted.
         thermal_specification : str
             Select what thermal specification is to be applied. The possible choices are ``"Thickness"``,
             ``"Conductance"``, ``"Thermal Impedance"`` and ``"Thermal Resistance"``
         thermal_dependent_dataset : str, optional
             Name of the dataset if a thermal dependent power source is to be assigned. The default is ``None``.
         input_power : str, float, or int, optional
             Input power. The default is ``"0W"``. Ignored if thermal_dependent_dataset is set
@@ -577,18 +583,20 @@
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object when successful or ``None`` when failed.
 
         """
         if not bc_name:
             bc_name = generate_unique_name("Source")
         props = {}
-        if isinstance(face_id, int):
-            props["Faces"] = [face_id]
-        elif isinstance(face_id, str):
-            props["Objects"] = [face_id]
+        if not isinstance(face_id, list):
+            face_id = [face_id]
+        if isinstance(face_id[0], int):
+            props["Faces"] = face_id
+        elif isinstance(face_id[0], str):
+            props["Objects"] = face_id
         if radiate_low:
             props["LowSide"] = OrderedDict(
                 {"Radiate": True, "RadiateTo": "AllObjects", "Surface Material": low_surf_material}
             )
         else:
             props["LowSide"] = OrderedDict({"Radiate": False})
         if radiate_high:
@@ -611,17 +619,22 @@
                     "Variation Type": "Temp Dep",
                     "Variation Function": "Piecewise Linear",
                     "Variation Value": '["1W", "pwl({},Temp)"]'.format(thermal_dependent_dataset),
                 }
             )
         props["Shell Conduction"] = shell_conduction
         bound = BoundaryObject(self, bc_name, props, "Conducting Plate")
-        if bound.create():
-            self.boundaries.append(bound)
-            return bound
+        try:
+            if bound.create():
+                self.boundaries.append(bound)
+                return bound
+            else:  # pragma : no cover
+                raise SystemExit
+        except SystemExit:
+            return None
 
     @pyaedt_function_handler()
     def create_source_power(
         self,
         face_id,
         thermal_dependent_dataset=None,
         input_power=None,
@@ -703,17 +716,22 @@
                     "Variation Value": '["1W", "pwl({},Temp)"]'.format(thermal_dependent_dataset),
                 }
             )
         props["Surface Heat"] = surface_heat
         props["Temperature"] = temperature
         props["Radiation"] = OrderedDict({"Radiate": radiate})
         bound = BoundaryObject(self, source_name, props, "SourceIcepak")
-        if bound.create():
-            self.boundaries.append(bound)
-            return bound
+        try:
+            if bound.create():
+                self.boundaries.append(bound)
+                return bound
+            else:  # pragma : no cover
+                raise SystemExit
+        except SystemExit:
+            return None
 
     @pyaedt_function_handler()
     def create_network_block(
         self,
         object_name,
         power,
         rjc,
@@ -2024,26 +2042,26 @@
                 self.modeler.move(new_name, origin)
             return native
         return False
 
     @pyaedt_function_handler()
     def create_ipk_3dcomponent_pcb(
         self,
-        compName,
-        setupLinkInfo,
-        solutionFreq,
-        resolution,
-        PCB_CS="Global",
-        rad="Nothing",
-        extent_type="Bounding Box",
-        outline_polygon="",
-        powerin="0W",
-        custom_x_resolution=None,
-        custom_y_resolution=None,
-        **kwargs  # fmt: skip
+            compName,
+            setupLinkInfo,
+            solutionFreq,
+            resolution,
+            PCB_CS="Global",
+            rad="Nothing",
+            extent_type="Bounding Box",
+            outline_polygon="",
+            powerin="0W",
+            custom_x_resolution=None,
+            custom_y_resolution=None,
+            **kwargs  # fmt: skip
     ):
         """Create a PCB component in Icepak that is linked to an HFSS 3D Layout object.
 
         Parameters
         ----------
         compName : str
             Name of the new PCB component.
@@ -2155,25 +2173,25 @@
             self._native_components.append(native)
             return native
         return False
 
     @pyaedt_function_handler()
     def create_pcb_from_3dlayout(
         self,
-        component_name,
-        project_name,
-        design_name,
-        resolution=2,
-        extent_type="Bounding Box",
-        outline_polygon="",
-        close_linked_project_after_import=True,
-        custom_x_resolution=None,
-        custom_y_resolution=None,
-        power_in=0,
-        **kwargs  # fmt: skip
+            component_name,
+            project_name,
+            design_name,
+            resolution=2,
+            extent_type="Bounding Box",
+            outline_polygon="",
+            close_linked_project_after_import=True,
+            custom_x_resolution=None,
+            custom_y_resolution=None,
+            power_in=0,
+            **kwargs  # fmt: skip
     ):
         """Create a PCB component in Icepak that is linked to an HFSS 3DLayout object linking only to the geometry file.
 
         .. note::
            No solution is linked.
 
         Parameters
@@ -3222,15 +3240,15 @@
              unit is degrees Celsius. The default is ``"AmbientTemp"``.
         ext_surf_rad_view_factor : str or float, optional
             View factor for the external surface radiation option. The default is ``"1"``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Boundary object.
+            Boundary object when successful or ``None`` when failed.
 
         References
         ----------
 
         >>> oModule.AssignStationaryWallBoundary
         """
         if not name:
@@ -3303,17 +3321,22 @@
         props["Radiation"] = {"Radiate": radiate, "RadiateTo": "AllObjects", "Surface Material": radiate_surf_mat}
         props["Shell Conduction"] = shell_conduction
         props["External Surface Radiation"] = ext_surf_rad
         props["External Material"] = ext_surf_rad_material
         props["External Radiation Reference Temperature"] = ext_surf_rad_ref_temp
         props["External Radiation View Factor"] = ext_surf_rad_view_factor
         bound = BoundaryObject(self, name, props, "Stationary Wall")
-        if bound.create():
-            self.boundaries.append(bound)
-        return bound
+        try:
+            if bound.create():
+                self.boundaries.append(bound)
+                return bound
+            else:  # pragma : no cover
+                raise SystemExit
+        except SystemExit:
+            return None
 
     @pyaedt_function_handler()
     def assign_stationary_wall_with_heat_flux(
         self,
         geometry,
         name=None,
         heat_flux="0irrad_W_per_m2",
@@ -3668,16 +3691,17 @@
         voltage_current_choice=False,
         voltage_current_value=None,
     ):
         """Create a source power for a face.
 
         Parameters
         ----------
-        assignment : int or str
-            If int, Face ID. If str, object name.
+        assignment : int or str or list
+            Integer indicating a face ID or a string indicating an object name. A list of face
+            IDs or object names is also accepted.
         thermal_condition : str
             Thermal condition. Accepted values are ``"Total Power"``, ``"Surface Heat"``,
             ``"Temperature"``.
         assignment_value : str or dict
             Value and units of the input power, surface heat or temperature (depending on
             ``thermal_condition``). A dictionary can be used for temperature dependent or transient
              assignment. The dictionary should contain three keys: ``"Type"``, ``"Function"`` and
@@ -3724,18 +3748,20 @@
         ... "Function": "Piecewise Linear", "Values": "Test_DataSet"})
 
         """
         default_values = {"Total Power": "0W", "Surface Heat": "0irrad_W_per_m2", "Temperature": "AmbientTemp"}
         if not boundary_name:
             boundary_name = generate_unique_name("Source")
         props = {}
-        if isinstance(assignment, int):
-            props["Faces"] = [assignment]
-        elif isinstance(assignment, str):
-            props["Objects"] = [assignment]
+        if not isinstance(assignment, list):
+            assignment = [assignment]
+        if isinstance(assignment[0], int):
+            props["Faces"] = assignment
+        elif isinstance(assignment[0], str):
+            props["Objects"] = assignment
         props["Thermal Condition"] = thermal_condition
         for quantity, value in default_values.items():
             if quantity == thermal_condition:
                 if isinstance(assignment_value, dict):
                     assignment_value = self._parse_variation_data(
                         quantity,
                         assignment_value["Type"],
@@ -3773,14 +3799,16 @@
             else:
                 props[quantity] = value
 
         bound = BoundaryObject(self, boundary_name, props, "SourceIcepak")
         if bound.create():
             self.boundaries.append(bound)
             return bound
+        else:
+            return None
 
     @pyaedt_function_handler()
     def create_network_object(self, name=None, props=None, create=False):
         """Create a thermal network.
 
         Parameters
         ----------
@@ -3891,16 +3919,16 @@
         self, object_name, power_assignment, boundary_name=None, htc=None, ext_temperature="AmbientTemp"
     ):
         """
         Assign block boundary for solid objects.
 
         Parameters
         ----------
-        object_name : str
-            Name of the object.
+        object_name : str or list
+            Object name or a list of object names.
         power_assignment : str or dict
             String with the value and units of the power assignment or with
             ``"Joule Heating"``. For a temperature-dependent or transient
             assignment, a dictionary can be used. The dictionary should contain three keys:
             ``"Type"``, ``"Function"``, and ``"Values"``.
 
             - For the ``"Type"`` key, accepted values are ``"Temp Dep"`` and ``"Transient"``.
@@ -3951,28 +3979,31 @@
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
         >>> ipk.solution_type = "Transient"
         >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox3", "copper")
         >>> power_dict = {"Type": "Transient", "Function": "Sinusoidal", "Values": ["0W", 1, 1, "1s"]}
         >>> block = ipk.assign_solid_block("BlockBox3", power_dict)
         """
-        if not self.modeler.get_object_from_name(object_name).solve_inside:
-            self.logger.add_error_message(
-                "Use the ``assign_hollow_block()`` method with this object as ``solve_inside`` is ``False``."
-            )
-            return None
         if ext_temperature != "AmbientTemp" and ext_temperature is not None and not htc:
             self.logger.add_error_message("Set an argument for ``htc`` or remove the ``ext_temperature`` argument.")
             return None
         if isinstance(ext_temperature, dict) and ext_temperature["Type"] == "Temp Dep":
             self.logger.add_error_message(
                 'It is not possible to use a "Temp Dep" assignment for ' "temperature assignment."
             )
             return None
-        props = {"Block Type": "Solid", "Objects": [object_name]}
+        if not isinstance(object_name, list):
+            object_name = [object_name]
+        for o_n in object_name:
+            if not self.modeler.get_object_from_name(o_n).solve_inside:
+                self.logger.add_error_message(
+                    "Use the ``assign_hollow_block()`` method with this object as ``solve_inside`` is ``False``."
+                )
+                return None
+        props = {"Block Type": "Solid", "Objects": object_name}
         if isinstance(power_assignment, dict):
             assignment_value = self._parse_variation_data(
                 "Total Power",
                 power_assignment["Type"],
                 variation_value=power_assignment["Values"],
                 function=power_assignment["Function"],
             )
@@ -4002,32 +4033,37 @@
                     if isinstance(assignment, (float, int)):
                         assignment = str(assignment) + ["w_per_m2kel", "cel"][int(quantity == "Temperature")]
                     props[quantity] = assignment
         else:
             props["Use External Conditions"] = False
 
         if not boundary_name:
-            boundary_name = generate_unique_name(object_name + "_Block")
+            boundary_name = generate_unique_name("Block")
 
         bound = BoundaryObject(self, boundary_name, props, "Block")
-        if bound.create():
-            self.boundaries.append(bound)
-            return bound
+        try:
+            if bound.create():
+                self.boundaries.append(bound)
+                return bound
+            else:  # pragma : no cover
+                raise SystemExit
+        except SystemExit:
+            return None
 
     @pyaedt_function_handler
     def assign_hollow_block(
         self, object_name, assignment_type, assignment_value, boundary_name=None, external_temperature="AmbientTemp"
     ):
         """
         Assign block boundary for hollow objects.
 
         Parameters
         ----------
-        object_name : str
-            Name of the object.
+        object_name : str or list
+            Object name or a list of object names.
         assignment_type : str
             Type of the boundary assignment. Options are ``"Heat Transfer Coefficient"``,
             ``"Heat Flux"``, ``"Temperature"``, and ``"Total Power"``.
         assignment_value : str or dict
             String with value and units of the assignment. If ``"Total Power"`` is
             the assignment type, ``"Joule Heating"`` can be used.
             For a temperature-dependent or transient assignment, a dictionary can be used.
@@ -4076,19 +4112,14 @@
         >>> ipk = Icepak()
         >>> ipk.solution_type = "Transient"
         >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox5", "copper")
         >>> box.solve_inside = False
         >>> temp_dict = {"Type": "Transient", "Function": "Square Wave", "Values": ["1cel", "0s", "1s", "0.5s", "0cel"]}
         >>> block = ipk.assign_hollow_block("BlockBox5", "Heat Transfer Coefficient", "1w_per_m2kel", "Test", temp_dict)
         """
-        if self.modeler.get_object_from_name(object_name).solve_inside:
-            self.logger.add_error_message(
-                "Use ``assign_solid_block`` method with this object as ``solve_inside`` is ``True``."
-            )
-            return None
         if assignment_value == "Joule Heating" and assignment_type != "Total Power":
             self.logger.add_error_message(
                 '``"Joule Heating"`` assignment is supported only if ``assignment_type``' 'is ``"Total Power"``.'
             )
             return None
 
         assignment_dict = {
@@ -4102,15 +4133,23 @@
             self.logger.add_error_message(
                 'Valid options for assignment type are "Total Power", "Heat Flux",'
                 '"Temperature", and "Heat Transfer Coefficient".'
                 "{} not recognized.".format(assignment_type)
             )
             return None
 
-        props = {"Block Type": "Hollow", "Objects": [object_name], "Thermal Condition": thermal_condition[0]}
+        if not isinstance(object_name, list):
+            object_name = [object_name]
+        for o_n in object_name:
+            if self.modeler.get_object_from_name(o_n).solve_inside:
+                self.logger.add_error_message(
+                    "Use ``assign_solid_block`` method with this object as ``solve_inside`` is ``True``."
+                )
+                return None
+        props = {"Block Type": "Hollow", "Objects": object_name, "Thermal Condition": thermal_condition[0]}
         if thermal_condition[0] == "Fixed Heat":
             props["Use Total Power"] = thermal_condition[1] == "Total Power"
         if isinstance(assignment_value, dict):
             assignment_value_dict = self._parse_variation_data(
                 thermal_condition[1],
                 assignment_value["Type"],
                 variation_value=assignment_value["Values"],
@@ -4136,20 +4175,25 @@
                     function=external_temperature["Function"],
                 )
                 props.update(assignment_value_dict)
             else:
                 props["Temperature"] = external_temperature
 
         if not boundary_name:
-            boundary_name = generate_unique_name(object_name + "_Block")
+            boundary_name = generate_unique_name("Block")
 
         bound = BoundaryObject(self, boundary_name, props, "Block")
-        if bound.create():
-            self.boundaries.append(bound)
-            return bound
+        try:
+            if bound.create():
+                self.boundaries.append(bound)
+                return bound
+            else:  # pragma : no cover
+                raise SystemExit
+        except SystemExit:
+            return None
 
     @pyaedt_function_handler()
     def get_fans_operating_point(self, export_file=None, setup_name=None, timestep=None, design_variation=None):
         """
         Get operating point of the fans in the design.
 
         Parameters
@@ -4228,7 +4272,450 @@
             for line in reader:
                 if "Fan Instances" in line:
                     vol_flow = line[1]
                     p_rise = line[2]
                     break
             var = {line[0]: [float(line[1]), float(line[2])] for line in reader}
         return [export_file, vol_flow, p_rise, var]
+
+    @pyaedt_function_handler()
+    def assign_free_opening(
+        self,
+        assignment,
+        boundary_name=None,
+        temperature="AmbientTemp",
+        radiation_temperature="AmbientRadTemp",
+        flow_type="Pressure",
+        pressure="AmbientPressure",
+        no_reverse_flow=False,
+        velocity=["0m_per_sec", "0m_per_sec", "0m_per_sec"],
+        mass_flow_rate="0kg_per_s",
+        inflow=True,
+        direction_vector=None,
+    ):
+        """
+        Assign free opening boundary condition.
+
+        Parameters
+        ----------
+        assignment : int or str or list
+            Integer indicating a face ID or a string indicating an object name. A list of face
+            IDs or object names is also accepted.
+        boundary_name : str, optional
+            Boundary name. Default is ``None``, in which case the name is generated automatically.
+        temperature : str or float or dict, optional
+            Prescribed temperature at the boundary. If a string is set,  a variable name or a
+            number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and ``'Values'``
+            can be passed to set a transient behaviour. The acceptable values associated with those
+            keys can be found in the Icepak documentation. Default is ``"AmbientTemp"``.
+        radiation_temperature : str or float, optional
+            Prescribed radiation temperature at the boundary. If a string is set,  a variable name
+            or a number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and
+            ``'Values'`` can be passed to set a transient behaviour.
+            The acceptable values associated with those keys can be found in the Icepak documentation.
+            Default is ``"AmbientRadTemp"``.
+        flow_type : int or str, optional
+            Prescribed radiation flow type at the boundary. Available options are ``"Pressure"``,
+            ``"Velocity"``, and ``"Mass Flow"``. The default is ``"Pressure"``.
+        pressure : float or str or dict, optional
+            Prescribed pressure (static or total coherently with flow type) at the boundary. If a
+            string is set, a variable name or a number with the unit is expected. If a float is set,
+            the unit ``'pascal'`` is automatically added. Also, a dictionary containing the keys
+            ``'Function'`` and ``'Values'`` can be passed to set a transient behavior. The acceptable
+            values associated with those keys can be found in the Icepak documentation.
+            The default is ``"AmbientPressure"``.
+        no_reverse_flow : bool, optional
+            Option to block reverse flow at the boundary. Default is ``False``.
+        velocity : list, optional
+            Prescribed velocity at the boundary. If a list of strings is set, a variable name or a number
+             with the unit is expected for each element. If list of floats is set, the unit ``'m_per_sec'``
+            is automatically added. Also, a dictionary containing the keys ``'Function'`` and
+            ``'Values'`` can be passed in one or more vector element to set a transient behaviour.
+            The acceptable values associated with those keys can be found in the Icepak documentation.
+            Default is ``["0m_per_sec", "0m_per_sec", "0m_per_sec"]``.
+        mass_flow_rate : float or str or dict, optional
+            Prescribed pressure (static or total coherently with flow type) at the boundary. If a
+            string is set, a variable name or a number with the unit is expected. If a float is set,
+            the unit ``'kg_per_s'`` is automatically added. Also, a dictionary containing the keys
+            ``'Function'`` and ``'Values'`` can be passed to set a transient behaviour. The acceptable
+            values associated with those keys can be found in the Icepak documentation.
+            Default is ``"0kg_per_s"``.
+        inflow : bool, optional
+            Prescribe if the imposed mass flow is an inflow or an outflow. Default is ``"True"``,
+            in which case an inflow is prescribed.
+        direction_vector : list, optional
+            Prescribe the direction of the massflow. Default is ``"None"``, in which case a
+            massflow normal to the boundary is prescribed.
+
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+        oModule.AssignOpeningBoundary
+
+        Examples
+        ----------
+        >>> import pyaedt
+        >>> icepak = pyaedt.Icepak()
+        >>> f_id = icepak.modeler["Region"].faces[0].id
+        >>> icepak.assign_free_opening(f_id)
+        """
+        # Sanitize input
+        for i in range(len(velocity)):
+            if not isinstance(velocity[i], str) and not isinstance(velocity[i], dict):
+                velocity[i] = str(velocity[i]) + "m_per_sec"
+        if not isinstance(mass_flow_rate, str) and not isinstance(mass_flow_rate, dict):
+            mass_flow_rate = str(mass_flow_rate) + "kg_per_s"
+        if not isinstance(temperature, str) and not isinstance(temperature, dict):
+            temperature = str(temperature) + "cel"
+        if not isinstance(radiation_temperature, str) and not isinstance(radiation_temperature, dict):
+            radiation_temperature = str(radiation_temperature) + "cel"
+        if not isinstance(pressure, str) and not isinstance(pressure, dict):
+            pressure = str(pressure) + "pascal"
+        # Dict creation
+        props = {}
+        if not isinstance(assignment, list):
+            assignment = [assignment]
+        if isinstance(assignment[0], int):
+            props["Faces"] = assignment
+        else:
+            props["Objects"] = assignment
+        possible_transient_properties = [
+            ("Temperature", temperature),
+            ("External Rad. Temperature", radiation_temperature),
+        ]
+        if flow_type == "Pressure":
+            props["Inlet Type"] = flow_type
+            props["No Reverse Flow"] = no_reverse_flow
+            possible_transient_properties += [("Total Pressure", pressure)]
+        elif flow_type == "Velocity":
+            props["Inlet Type"] = flow_type
+            possible_transient_properties += [
+                ("Static Pressure", pressure),
+                ("X Velocity", velocity[0]),
+                ("Y Velocity", velocity[1]),
+                ("Z Velocity", velocity[2]),
+            ]
+        elif flow_type == "Mass Flow":
+            props["Inlet Type"] = flow_type
+            if direction_vector is None:
+                props["Mass Flow Direction"] = ("Normal to Boundary",)
+            else:
+                props["X"] = str(direction_vector[0])
+                props["Y"] = str(direction_vector[1])
+                props["Z"] = str(direction_vector[2])
+            props["Mass Flow Condition"] = ["Out Flow", "In Flow"][int(inflow)]
+            possible_transient_properties += [
+                ("Total Pressure", pressure),
+                ("Mass Flow Rate", mass_flow_rate),
+                ("Y Velocity", velocity[1]),
+                ("Z Velocity", velocity[2]),
+            ]
+        for quantity, assignment in possible_transient_properties:
+            if isinstance(assignment, dict):
+                if not self.solution_type == "Transient":
+                    self.logger.error("Transient assignment is supported only in transient designs.")
+                    return None
+                assignment = self._parse_variation_data(
+                    quantity,
+                    "Transient",
+                    variation_value=assignment["Values"],
+                    function=assignment["Function"],
+                )
+                if assignment is None:
+                    return None
+                props.update(assignment)
+            else:
+                props[quantity] = assignment
+
+        if not boundary_name:
+            boundary_name = generate_unique_name("Opening")
+
+        bound = BoundaryObject(self, boundary_name, props, "Opening")
+        if bound.create():
+            self.boundaries.append(bound)
+            return bound
+        else:
+            return None
+
+    @pyaedt_function_handler()
+    def assign_pressure_free_opening(
+        self,
+        assignment,
+        boundary_name=None,
+        temperature="AmbientTemp",
+        radiation_temperature="AmbientRadTemp",
+        pressure="AmbientPressure",
+        no_reverse_flow=False,
+    ):
+        """
+        Assign free opening boundary condition.
+
+        Parameters
+        ----------
+        assignment : int or str or list
+           Integer indicating a face ID or a string indicating an object name. A list of face
+           IDs or object names is also accepted.
+        boundary_name : str, optional
+            Boundary name. Default is ``None``, in which case the name is generated automatically.
+        temperature : str or float or dict, optional
+            Prescribed temperature at the boundary. If a string is set,  a variable name or a
+            number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and ``'Values'``
+            can be passed to set a transient behaviour. The acceptable values associated with those
+            keys can be found in the Icepak documentation. Default is ``"AmbientTemp"``.
+        radiation_temperature : str or float, optional
+            Prescribed radiation temperature at the boundary. If a string is set,  a variable name
+            or a number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and
+            ``'Values'`` can be passed to set a transient behaviour.
+            The acceptable values associated with those keys can be found in the Icepak documentation.
+            Default is ``"AmbientRadTemp"``.
+        pressure : float or str or dict, optional
+            Prescribed pressure (static or total coherently with flow type) at the boundary. If a
+            string is set, a variable name or a number with the unit is expected. If a float is set,
+            the unit ``'pascal'`` is automatically added. Also, a dictionary containing the keys
+            ``'Function'`` and ``'Values'`` can be passed to set a transient behavior. The
+            acceptable values associated with those keys can be found in the Icepak
+            documentation. The default is ``"AmbientPressure"``.
+        no_reverse_flow : bool, optional
+            Option to block reverse flow at the boundary. Default is ``False``.
+
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+        oModule.AssignOpeningBoundary
+
+        Examples
+        ----------
+        >>> import pyaedt
+        >>> icepak = pyaedt.Icepak()
+        >>> f_id = icepak.modeler["Region"].faces[0].id
+        >>> icepak.assign_pressure_free_opening(f_id)
+        """
+        return self.assign_free_opening(
+            assignment,
+            boundary_name=boundary_name,
+            temperature=temperature,
+            radiation_temperature=radiation_temperature,
+            flow_type="Pressure",
+            pressure=pressure,
+            no_reverse_flow=no_reverse_flow,
+        )
+
+    @pyaedt_function_handler()
+    def assign_velocity_free_opening(
+        self,
+        assignment,
+        boundary_name=None,
+        temperature="AmbientTemp",
+        radiation_temperature="AmbientRadTemp",
+        pressure="AmbientPressure",
+        velocity=["0m_per_sec", "0m_per_sec", "0m_per_sec"],
+    ):
+        """
+        Assign free opening boundary condition.
+
+        Parameters
+        ----------
+        assignment : int or str or list
+            Integer indicating a face ID or a string indicating an object name. A list of face
+            IDs or object names is also accepted.
+        boundary_name : str, optional
+            Boundary name. Default is ``None``, in which case the name is generated automatically.
+        temperature : str or float or dict, optional
+            Prescribed temperature at the boundary. If a string is set,  a variable name or a
+            number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and ``'Values'``
+            can be passed to set a transient behaviour. The acceptable values associated with those
+            keys can be found in the Icepak documentation. Default is ``"AmbientTemp"``.
+        radiation_temperature : str or float, optional
+            Prescribed radiation temperature at the boundary. If a string is set,  a variable name
+            or a number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and
+            ``'Values'`` can be passed to set a transient behaviour.
+            The acceptable values associated with those keys can be found in the Icepak documentation.
+            Default is ``"AmbientRadTemp"``.
+        pressure : float or str or dict, optional
+            Prescribed pressure (static or total coherently with flow type) at the boundary. If a
+            string is set, a variable name or a number with the unit is expected. If a float is set,
+            the unit ``'pascal'`` is automatically added. Also, a dictionary containing the keys
+            ``'Function'`` and ``'Values'`` can be passed to set a transient behavior. The
+            acceptable values associated with those keys can be found in the Icepak
+            documentation. The default is ``"AmbientPressure"``.
+        velocity : list, optional
+            Prescribed velocity at the boundary. If a list of strings is set, a variable name or a number
+             with the unit is expected for each element. If list of floats is set, the unit ``'m_per_sec'``
+            is automatically added. Also, a dictionary containing the keys ``'Function'`` and
+            ``'Values'`` can be passed in one or more vector element to set a transient behaviour.
+            The acceptable values associated with those keys can be found in the Icepak documentation.
+            Default is ``["0m_per_sec", "0m_per_sec", "0m_per_sec"]``.
+
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+        oModule.AssignOpeningBoundary
+
+        Examples
+        ----------
+        >>> import pyaedt
+        >>> icepak = pyaedt.Icepak()
+        >>> f_id = icepak.modeler["Region"].faces[0].id
+        >>> icepak.assign_velocity_free_opening(f_id)
+        """
+        return self.assign_free_opening(
+            assignment,
+            boundary_name=boundary_name,
+            temperature=temperature,
+            radiation_temperature=radiation_temperature,
+            flow_type="Velocity",
+            pressure=pressure,
+            velocity=velocity,
+        )
+
+    @pyaedt_function_handler()
+    def assign_mass_flow_free_opening(
+        self,
+        assignment,
+        boundary_name=None,
+        temperature="AmbientTemp",
+        radiation_temperature="AmbientRadTemp",
+        pressure="AmbientPressure",
+        mass_flow_rate="0kg_per_s",
+        inflow=True,
+        direction_vector=None,
+    ):
+        """
+        Assign free opening boundary condition.
+
+        Parameters
+        ----------
+        assignment : int or str or list
+           Integer indicating a face ID or a string indicating an object name. A list of face
+           IDs or object names is also accepted.
+        boundary_name : str, optional
+            Boundary name. The default is ``None``, in which case the name is generated automatically.
+        temperature : str or float or dict, optional
+            Prescribed temperature at the boundary. If a string is set,  a variable name or a
+            number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and ``'Values'``
+            can be passed to set a transient behaviour. The acceptable values associated with those
+            keys can be found in the Icepak documentation. Default is ``"AmbientTemp"``.
+        radiation_temperature : str or float, optional
+            Prescribed radiation temperature at the boundary. If a string is set,  a variable name
+            or a number with the unit is expected. If a float is set, the unit ``'cel'`` is
+            automatically added. Also, a dictionary containing the keys ``'Function'`` and
+            ``'Values'`` can be passed to set a transient behaviour.
+            The acceptable values associated with those keys can be found in the Icepak documentation.
+            Default is ``"AmbientRadTemp"``.
+        pressure : float or str or dict, optional
+            Prescribed pressure (static or total coherently with flow type) at the boundary. If a
+            string is set, a variable name or a number with the unit is expected. If a float is set,
+            the unit ``'pascal'`` is automatically added. Also, a dictionary containing the keys
+            ``'Function'`` and ``'Values'`` can be passed to set a transient behavior. The
+            acceptable values associated with those keys can be found in the Icepak
+            documentation. The default is ``"AmbientPressure"``.
+        mass_flow_rate : float or str or dict, optional
+            Prescribed pressure (static or total coherently with flow type) at the boundary. If a
+            string is set, a variable name or a number with the unit is expected. If a float is set,
+            the unit ``'kg_per_s'`` is automatically added. Also, a dictionary containing the keys
+            ``'Function'`` and ``'Values'`` can be passed to set a transient behaviour. The acceptable
+            values associated with those keys can be found in the Icepak documentation.
+            Default is ``"0kg_per_s"``.
+        inflow : bool, optional
+            Prescribe if the imposed mass flow is an inflow or an outflow. Default is ``"True"``,
+            in which case an inflow is prescribed.
+        direction_vector : list, optional
+            Prescribe the direction of the massflow. Default is ``"None"``, in which case a
+            massflow normal to the boundary is prescribed.
+
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+        oModule.AssignOpeningBoundary
+
+        Examples
+        ----------
+        >>> import pyaedt
+        >>> icepak = pyaedt.Icepak()
+        >>> f_id = icepak.modeler["Region"].faces[0].id
+        >>> icepak.assign_mass_flow_free_opening(f_id)
+        """
+        return self.assign_free_opening(
+            assignment,
+            boundary_name=boundary_name,
+            temperature=temperature,
+            radiation_temperature=radiation_temperature,
+            flow_type="Mass Flow",
+            pressure=pressure,
+            mass_flow_rate=mass_flow_rate,
+            inflow=inflow,
+            direction_vector=direction_vector,
+        )
+
+    @pyaedt_function_handler()
+    def assign_symmetry_wall(
+        self,
+        geometry,
+        boundary_name=None,
+    ):
+        """Assign symmetry wall boundary condition.
+
+        Parameters
+        ----------
+        geometry : str or int or list
+            Surface object name or face ID. A list of surface object names
+            or face IDs is also acceptable.
+        boundary_name : str, optional
+            Name of the boundary condition. The default is ``None``.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+
+        >>> oModule.AssignSymmetryWallBoundary
+        """
+        if not boundary_name:
+            boundary_name = generate_unique_name("SymmetryWall")
+        if isinstance(geometry, (str, int)):
+            geometry = [geometry]
+
+        props = {}
+        if isinstance(geometry[0], int):
+            props["Faces"] = geometry
+        else:
+            props["Objects"] = geometry
+
+        bound = BoundaryObject(self, boundary_name, props, "Symmetry Wall")
+        try:
+            if bound.create():
+                self.boundaries.append(bound)
+                return bound
+            else:  # pragma : no cover
+                raise SystemExit
+        except SystemExit:
+            return None
```

### Comparing `pyaedt-0.6.81/pyaedt/maxwell.py` & `pyaedt-0.6.82/pyaedt/maxwell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1578,14 +1578,98 @@
                 "CaculateForceType:=",
                 calculate_force + " Force",
             ]
         )
         return True
 
     @pyaedt_function_handler()
+    def enable_harmonic_force_on_layout_component(
+        self,
+        layout_component_name,
+        nets,
+        force_type=0,
+        window_function="Rectangular",
+        use_number_of_last_cycles=True,
+        last_cycles_number=1,
+        calculate_force="Harmonic",
+        start_time="0s",
+        stop_time="2ms",
+        use_number_of_cycles_for_stop_time=True,
+        number_of_cycles_for_stop_time=1,
+    ):
+        """Enable the harmonic force calculation for the transient analysis.
+
+        Parameters
+        ----------
+        layout_component_name : str
+            Name of layout component to apply harmonic forces.
+        nets : dict
+            Dictionary containing nets and layers on which enable harmonic forces.
+        force_type : int, optional
+            Force Type. ``0`` for Objects, ``1`` for Surface, ``2`` for volumetric.
+        window_function : str, optional
+            Windowing function. Default is ``"Rectangular"``.
+            Available options are: ``"Rectangular"``, ``"Tri"``, ``"Van Hann"``, ``"Hamming"``,
+            ``"Blackman"``, ``"Lanczos"``, ``"Welch"``.
+        use_number_of_last_cycles : bool, optional
+            Use number Of last cycles for force calculations. Default is ``True``.
+        last_cycles_number : int, optional
+            Defines the number of cycles to compute if `use_number_of_last_cycle` is ``True``.
+        calculate_force : sr, optional
+            How to calculate force. The default is ``"Harmonic"``.
+            Options are ``"Harmonic"`` and ``"Transient"``.
+
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        """
+        if self.solution_type != "TransientAPhiFormulation":
+            self.logger.error("This methods work only with Maxwell TransientAPhiFormulation Analysis.")
+            return False
+        args = [
+            "ForceType:=",
+            force_type,
+            "WindowFunctionType:=",
+            window_function,
+            "UseNumberOfLastCycles:=",
+            use_number_of_last_cycles,
+            "NumberOfLastCycles:=",
+            last_cycles_number,
+            "StartTime:=",
+            start_time,
+            "UseNumberOfCyclesForStopTime:=",
+            use_number_of_cycles_for_stop_time,
+            "NumberOfCyclesForStopTime:=",
+            number_of_cycles_for_stop_time,
+            "StopTime:=",
+            stop_time,
+            "OutputFreqRangeType:=",
+            "Use All",
+            "CaculateForceType:=",
+            calculate_force + " Force",
+        ]
+        args2 = [
+            "NAME:NetsAndLayersChoices",
+            [
+                "NAME:" + layout_component_name,
+                [
+                    "NAME:NetLayerSetMap",
+                ],
+            ],
+        ]
+        for net, layers in nets.items():
+            args2[1][1].append(["Name:" + net, "LayerSet:=", ["<no-layer>"] + layers])
+        args.append(args2)
+        self.odesign.EnableHarmonicForceCalculation(args)
+        return True
+
+    @pyaedt_function_handler()
     def export_element_based_harmonic_force(
         self,
         output_directory=None,
         setup_name=None,
         start_frequency=None,
         stop_frequency=None,
         number_of_frequency=None,
@@ -1606,15 +1690,15 @@
             When a number is entered, the number of frequencies approach is used.
 
         Returns
         -------
         str
             Path to the export directory.
         """
-        if self.solution_type != "Transient":
+        if self.solution_type != "Transient" and self.solution_type != "TransientAPhiFormulation":
             self.logger.error("This methods work only with Maxwell Transient Analysis.")
             return False
         if not output_directory:
             output_directory = self.working_directory
         if not setup_name:
             setup_name = self.setups[0].name
         freq_option = 1
@@ -2561,15 +2645,15 @@
         for sel in objects_list:
             props["Faces"].append(sel)
 
         return self._create_boundary(flux_name, props, "FluxTangential")
 
     @pyaedt_function_handler
     def assign_layout_force(self, nets_layers_mapping, component_name, reference_cs="Global", force_name=None):
-        # type : (dict, str, str, str) -> bool
+        # type: (dict, str, str, str) -> bool
         """Assign the layout force to a component in a Transient A-Phi solver.
         To access layout component features the Beta option has to be enabled first.
 
         Parameters
         ----------
         nets_layers_mapping : dict
             Each <layer, net> pair represents the object(s) in the intersection of corresponding layer and net.
@@ -2612,25 +2696,26 @@
         if component_name not in self.modeler.user_defined_component_names:
             self.logger.error("Provided component name doesn't exist in current design.")
             return False
 
         if not force_name:
             force_name = generate_unique_name("Layout_Force")
 
-        nets_layers_props = []
-        for key in nets_layers_mapping.keys():
-            vArg5 = ["NAME:" + key]
-            vArg5.append("LayerSet:="), vArg5.append(nets_layers_mapping[key])
-            nets_layers_props.append(vArg5)
+        nets_layers_props = None
+        for key, valy in nets_layers_mapping.items():
+            if nets_layers_props:
+                nets_layers_props.append(OrderedDict({key: OrderedDict({"LayerSet": valy})}))
+            else:
+                nets_layers_props = [OrderedDict({key: OrderedDict({"LayerSet": valy})})]
 
         props = OrderedDict(
             {
-                "Coordinate System": reference_cs,
+                "Reference CS": reference_cs,
                 "NetsAndLayersChoices": OrderedDict(
-                    {component_name: OrderedDict({"NetLayerSetMap": nets_layers_mapping})}
+                    {component_name: OrderedDict({"NetLayerSetMap": nets_layers_props})}
                 ),
             }
         )
         bound = MaxwellParameters(self, force_name, props, "LayoutForce")
         if bound.create():
             self.boundaries.append(bound)
             return bound
```

### Comparing `pyaedt-0.6.81/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.82/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/mechanical.py` & `pyaedt-0.6.82/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/Console.py_build` & `pyaedt-0.6.82/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.82/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.82/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.82/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/amat.xml` & `pyaedt-0.6.82/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/console_setup.py` & `pyaedt-0.6.82/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.82/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.82/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.82/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.82/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/misc.py` & `pyaedt-0.6.82/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.82/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.82/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.82/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.82/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/misc/template.acf` & `pyaedt-0.6.82/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/Modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1261,16 +1261,14 @@
         Inherited parent object.
     is3d : bool, optional
         Whether the model is 3D. The default is ``True``.
     """
 
     def __init__(self, app, is3d=True):
         self._app = app
-        self._odefinition_manager = self._app.odefinition_manager
-        self._omaterial_manager = self._app.omaterial_manager
         Modeler.__init__(self, app)
         # TODO Refactor this as a dictionary with names as key
         self._coordinate_systems = []
         self._user_lists = []
         self._planes = []
         self._is3d = is3d
         self._solids = []
@@ -1280,14 +1278,22 @@
         self._unclassified = []
         self._all_object_names = []
         self.objects = {}
         self.user_defined_components = {}
         self._object_names_to_ids = {}
 
     @property
+    def _odefinition_manager(self):
+        return self._app.odefinition_manager
+
+    @property
+    def _omaterial_manager(self):
+        return self._app.omaterial_manager
+
+    @property
     def coordinate_systems(self):
         """Coordinate Systems."""
         if settings.aedt_version > "2022.2":
             cs_names = [i for i in self.oeditor.GetChildNames("CoordinateSystems") if i != "Global"]
             for cs_name in cs_names:
                 props = {}
                 local_names = [i.name for i in self._coordinate_systems]
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/Primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -2761,48 +2761,60 @@
         if self._app._design_type == "HFSS":
             return defaultmatname, self._app.materials.material_keys[defaultmatname].is_dielectric()
         else:
             return defaultmatname, True
 
     @pyaedt_function_handler()
     def _refresh_solids(self):
-        test = list(self.oeditor.GetObjectsInGroup("Solids"))
+        try:
+            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Solids")
+        except TypeError:
+            test = []
         if test is None or test is False:
             assert False, "Get Solids is failing"
         elif test is True:
             self._solids = []  # In IronPython True is returned when no sheets are present
         else:
             self._solids = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
 
     @pyaedt_function_handler()
     def _refresh_sheets(self):
-        test = list(self.oeditor.GetObjectsInGroup("Sheets"))
+        try:
+            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Sheets")
+        except TypeError:
+            test = []
         if test is None or test is False:
             assert False, "Get Sheets is failing"
         elif test is True:
             self._sheets = []  # In IronPython True is returned when no sheets are present
         else:
             self._sheets = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
 
     @pyaedt_function_handler()
     def _refresh_lines(self):
-        test = list(self.oeditor.GetObjectsInGroup("Lines"))
+        try:
+            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Lines")
+        except TypeError:
+            test = []
         if test is None or test is False:
             assert False, "Get Lines is failing"
         elif test is True:
             self._lines = []  # In IronPython True is returned when no lines are present
         else:
             self._lines = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
 
     @pyaedt_function_handler()
     def _refresh_points(self):
-        test = list(self.oeditor.GetPoints())
+        try:
+            test = _retry_ntimes(10, self.oeditor.GetPoints)
+        except TypeError:
+            test = []
         if test is None or test is False:
             assert False, "Get Points is failing"
         elif test is True:
             self._points = []  # In IronPython True is returned when no points are present
         else:
             self._points = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
@@ -2817,15 +2829,18 @@
             }
         except TypeError:
             self._planes = {}
         self._all_object_names = self._solids + self._sheets + self._lines + self._points + list(self._planes.keys())
 
     @pyaedt_function_handler()
     def _refresh_unclassified(self):
-        test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Unclassified")
+        try:
+            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Unclassified")
+        except TypeError:
+            test = []
         if test is None or test is False:
             self._unclassified = []
             self.logger.debug("Unclassified is failing")
         elif test is True:
             self._unclassified = []  # In IronPython True is returned when no unclassified are present
         else:
             self._unclassified = list(test)
@@ -3167,15 +3182,15 @@
                         native_comp_entry = [native_comp_entry]
                     for data in native_comp_entry:
                         native_comp_name = data["SubmodelDefinitionName"]
                         if native_comp_name == component_name:
                             native_comp_properties = data
                             break
             except:
-                self.logger.info("Native component properties were not retrieved from the AEDT file.")
+                return native_comp_properties
 
         return native_comp_properties
 
     @pyaedt_function_handler
     def _get_object_dict_by_material(self, material):
         obj_dict = {}
         for mat in material:
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,30 +451,34 @@
         beta=5,
         bond_type=0,
         diameter=0.025,
         facets=6,
         name=None,
         matname=None,
     ):
+        # type : (list, list, float|str=0.2, float|str=0, float=80, float=5, int=0, float|str=0.025, int=6, str=None,
+        # str=None) -> Object3d
         """Create a bondwire.
 
         Parameters
         ----------
         start_position : list
             List of ``[x, y, z]`` coordinates for the starting
             position of the bond pad.
         end_position :  list
             List of ``[x, y, z]`` coordinates for the ending position
             of the bond pad.
-        h1 : float, optional
+        h1 : float|str optional
             Height between the IC die I/O pad and the top of the bondwire.
+            If the height is provided as a parameter, its value has to be provided as value + unit.
             The default is ``0.2``.
-        h2 : float, optional
-            Height of the IC die I/O pad above the lead frame. The default
-            is ``0``. A negative value indicates that the I/O pad is below
+        h2 : float|str optional
+            Height of the IC die I/O pad above the lead frame.
+            If the height is provided as a parameter, its value has to be provided as value + unit.
+            The default is ``0``. A negative value indicates that the I/O pad is below
             the lead frame.
         alpha : float, optional
             Angle in degrees between the xy plane and the wire bond at the
             IC die I/O pad. The default is ``80``.
         beta : float, optional
             Angle in degrees between the xy plane and the wire bond at the
             lead frame. The default is ``5``.
@@ -482,15 +486,15 @@
             Type of the boundwire, which indicates its shape. Options are:
 
             * ''0'' for JEDEC 5-point
             * ``1`` for JEDEC 4-point
             * ''2`` for Low
 
             The default is ''0``.
-        diameter : float, optional
+        diameter : float|str optional
             Diameter of the wire. The default is ``0.025``.
         facets : int, optional
             Number of wire facets. The default is ``6``.
         name : str, optional
             Name of the bondwire. The default is ``None``, in which case
             the default name is assigned.
         matname : str, optional
@@ -510,21 +514,41 @@
         Examples
         --------
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> origin = [0,0,0]
         >>> endpos = [10,5,20]
         >>> #Material and name are not mandatory fields
-        >>> object_id = hfss.modeler.primivites.create_bondwire(origin, endpos,h1=0.5, h2=0.1, alpha=75, beta=4,
-        ...                                                     bond_type=0, name="mybox", matname="copper")
+        >>> object_id = hfss.modeler.create_bondwire(origin, endpos,h1=0.5, h2=0.1, alpha=75, beta=4,
+        ...                                          bond_type=0, name="mybox", matname="copper")
         """
         x_position, y_position, z_position = self._pos_with_arg(start_position)
+        x_position_end, y_position_end, z_position_end = self._pos_with_arg(end_position)
+
         if x_position is None or y_position is None or z_position is None:
             raise AttributeError("Position Argument must be a valid 3 Element List")
-        x_length, y_length, z_length = self._pos_with_arg([n - m for m, n in zip(start_position, end_position)])
+
+        cont = 0
+        x_length = None
+        y_length = None
+        z_length = None
+
+        for m, n in zip(start_position, end_position):
+            if not isinstance(m, str):
+                m = self._arg_with_dim(m)
+            if not isinstance(n, str):
+                n = self._arg_with_dim(n)
+            if cont == 0:
+                x_length = "(" + str(n) + ") - (" + str(m) + ")"
+            elif cont == 1:
+                y_length = "(" + str(n) + ") - (" + str(m) + ")"
+            elif cont == 2:
+                z_length = "(" + str(n) + ") - (" + str(m) + ")"
+            cont += 1
+
         if x_length is None or y_length is None or z_length is None:
             raise AttributeError("Dimension Argument must be a valid 3 Element List")
         if bond_type == 0:
             bondwire = "JEDEC_5Points"
         elif bond_type == 1:
             bondwire = "JEDEC_4Points"
         elif bond_type == 2:
@@ -538,17 +562,32 @@
         first_argument.append("NumSides:="), first_argument.append(str(facets))
         first_argument.append("XPadPos:="), first_argument.append(x_position)
         first_argument.append("YPadPos:="), first_argument.append(y_position)
         first_argument.append("ZPadPos:="), first_argument.append(z_position)
         first_argument.append("XDir:="), first_argument.append(x_length)
         first_argument.append("YDir:="), first_argument.append(y_length)
         first_argument.append("ZDir:="), first_argument.append(z_length)
-        first_argument.append("Distance:="), first_argument.append(
-            self._arg_with_dim(GeometryOperators.points_distance(start_position, end_position))
+        distance = (
+            "sqrt(("
+            + str(x_position_end)
+            + "-("
+            + str(x_position)
+            + ")) ** 2 + ("
+            + str(y_position_end)
+            + "-("
+            + str(y_position)
+            + ")) ** 2 + ( "
+            + str(z_position_end)
+            + "-("
+            + str(z_position)
+            + ")) ** 2) meter"
         )
+
+        first_argument.append("Distance:="), first_argument.append(distance)
+
         first_argument.append("h1:="), first_argument.append(self._arg_with_dim(h1))
         first_argument.append("h2:="), first_argument.append(self._arg_with_dim(h2))
         first_argument.append("alpha:="), first_argument.append(self._arg_with_dim(alpha, "deg"))
         first_argument.append("beta:="), first_argument.append(self._arg_with_dim(beta, "deg"))
         first_argument.append("WhichAxis:="), first_argument.append("Z")
         first_argument.append("ReverseDirection:="), first_argument.append(False)
         second_argument = self._default_object_attributes(name=name, matname=matname)
@@ -1521,15 +1560,16 @@
         parameters = {}
         for param in component_obj.design_variables:
             parameters[param] = [param + "_" + name, component_obj.design_variables[param].value_string]
             if parameter_mapping:
                 self._app[param + "_" + name] = component_obj.design_variables[param].value_string
 
         # Get coordinate systems
-        component_cs = list(component_obj.components.components.keys())
+        component_cs = list(component_obj.components.instances.keys())
+
         component_obj.close_edb()
 
         vArg1 = ["NAME:InsertNativeComponentData"]
         vArg1.append("TargetCS:=")
         vArg1.append(coordinate_system)
         vArg1.append("SubmodelDefinitionName:=")
         vArg1.append("LC")
@@ -1652,16 +1692,18 @@
             udm_obj = False
             if new_object_name:
                 obj_list = list(self.oeditor.Get3DComponentPartNames(new_object_name))
                 for new_name in obj_list:
                     self._create_object(new_name)
 
                 udm_obj = self._create_user_defined_component(new_object_name)
+
                 if name:
                     udm_obj.name = name
+
         except Exception:  # pragma: no cover
             udm_obj = False
         return udm_obj
 
     @pyaedt_function_handler()
     def get_3d_component_object_list(self, componentname):
         """Retrieve all objects belonging to a 3D component.
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/components_3d.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import absolute_import
 
 from collections import OrderedDict
+import os
 import random
 import re
 import warnings
 
 # from pyaedt import property
+from pyaedt import Edb
 from pyaedt import pyaedt_function_handler
+from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.modeler.cad.elements3d import BinaryTreeNode
 from pyaedt.modeler.cad.elements3d import _dict2arg
 
 
 class UserDefinedComponentParameters(dict):
     def __setitem__(self, key, value):
@@ -99,16 +102,15 @@
             "Date",
             "Purpose",
             "Version",
         ]
         self._group_name = None
         self._is3dcomponent = None
         self._mesh_assembly = None
-        self._show_layout = None
-        self._fast_transformation = None
+
         if name:
             self._m_name = name
         else:
             self._m_name = _uname()
         self._parameters = {}
         self._parts = None
         self._primitives = primitives
@@ -163,14 +165,38 @@
                 ),
             )
             if props:
                 self._update_props(self._props["NativeComponentDefinitionProvider"], props)
             self.native_properties = self._props["NativeComponentDefinitionProvider"]
             self.auto_update = True
 
+        self._layout_component = None
+
+    @property
+    def layout_component(self):
+        """Layout component object.
+
+        Returns
+        -------
+        :class:`LayoutComponent`
+            Layout Component.
+
+        References
+        ----------
+
+        >>> oEditor.GetPropertyValue
+        >>> oEditor.ChangeProperty
+
+        """
+        if not self._layout_component and "Show Layout" in self._primitives._app.get_oo_properties(
+            self._primitives.oeditor, self.name
+        ):
+            self._layout_component = LayoutComponent(self)
+        return self._layout_component
+
     @pyaedt_function_handler()
     def history(self):
         """Component history.
 
         Returns
         -------
             :class:`pyaedt.modeler.cad.elements3d.BinaryTree` when successful,
@@ -300,74 +326,14 @@
             and isinstance(ma, bool)
             and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames()
         ):
             self._primitives.oeditor.GetChildObject(self.name).SetPropValue(key, ma)
             self._mesh_assembly = ma
 
     @property
-    def show_layout(self):
-        """Show layout flag.
-
-        Returns
-        -------
-        bool
-           ``True`` if show layout is checked and if the component is a Layout Component,
-           ``None`` if other cases.
-
-        """
-        key = "Show Layout"
-        if self.is3dcomponent and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames():
-            show_layout = self._primitives.oeditor.GetChildObject(self.name).GetPropValue(key)
-            self._show_layout = show_layout
-            return show_layout
-        else:
-            return None
-
-    @show_layout.setter
-    def show_layout(self, show_layout):
-        key = "Show Layout"
-        if (
-            self.is3dcomponent
-            and isinstance(show_layout, bool)
-            and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames()
-        ):
-            self._primitives.oeditor.GetChildObject(self.name).SetPropValue(key, show_layout)
-            self._show_layout = show_layout
-
-    @property
-    def fast_transformation(self):
-        """Show layout flag.
-
-        Returns
-        -------
-        bool
-           ``True`` if fast transformation is checked and if the component is a Layout Component,
-           ``None`` if other cases.
-
-        """
-        key = "Fast Transformation"
-        if self.is3dcomponent and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames():
-            fast_transformation = self._primitives.oeditor.GetChildObject(self.name).GetPropValue(key)
-            self._fast_transformation = fast_transformation
-            return fast_transformation
-        else:
-            return None
-
-    @fast_transformation.setter
-    def fast_transformation(self, fast_transformation):
-        key = "Fast Transformation"
-        if (
-            self.is3dcomponent
-            and isinstance(fast_transformation, bool)
-            and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames()
-        ):
-            self._primitives.oeditor.GetChildObject(self.name).SetPropValue(key, fast_transformation)
-            self._fast_transformation = fast_transformation
-
-    @property
     def name(self):
         """Name of the object.
 
         Returns
         -------
         str
            Name of the object.
@@ -873,7 +839,249 @@
             project_name = project.GetName()
             if is_linux:
                 design_name = project.GetDesigns()[0].GetName()
             else:
                 design_name = project.GetActiveDesign().GetName()
             return get_pyaedt_app(project_name, design_name)
         return False
+
+
+class LayoutComponent(object):
+    """Manages object attributes for Layout components.
+
+    Parameters
+    ----------
+    primitives : :class:`pyaedt.modeler.Primitives3D.Primitives3D`
+        Inherited parent object.
+    name : str, optional
+        Name of the component. The default value is ``None``.
+
+    """
+
+    def __init__(self, component):
+        self._primitives = component._primitives
+        self._name = component.name
+        self._component = component
+        self._edb_definition = None
+        self._show_layout = None
+        self._fast_transformation = None
+        self._show_dielectric = None
+        self._display_mode = None
+        self.layers = {}
+        self.nets = {}
+        self.objects = {}
+        if self.edb_definition:
+            self._get_edb_info()
+
+    @property
+    def edb_definition(self):
+        """Edb definition.
+
+        Returns
+        -------
+        str
+           EDB definition.
+
+        """
+        key = "EDB Definition"
+        if key in self._primitives._app.get_oo_properties(self._primitives.oeditor, self._component.definition_name):
+            edb_definition = self._primitives._app.get_oo_property_value(
+                self._primitives.oeditor, self._component.definition_name, key
+            )
+            self._edb_definition = edb_definition
+            return edb_definition
+        else:
+            return None
+
+    @property
+    def show_layout(self):
+        """Show layout flag.
+
+        Returns
+        -------
+        bool
+           `Show layout check box.
+
+        """
+        key = "Show Layout"
+        if key in self._primitives._app.get_oo_properties(self._primitives.oeditor, self._name):
+            show_layout = self._primitives._app.get_oo_property_value(self._primitives.oeditor, self._name, key)
+            self._show_layout = show_layout
+            return show_layout
+        else:  # pragma: no cover
+            return None
+
+    @show_layout.setter
+    def show_layout(self, show_layout):
+        key = "Show Layout"
+        if isinstance(show_layout, bool) and key in self._primitives._app.get_oo_properties(
+            self._primitives.oeditor, self._name
+        ):
+            self._primitives.oeditor.GetChildObject(self._name).SetPropValue(key, show_layout)
+            self._show_layout = show_layout
+
+    @property
+    def fast_transformation(self):
+        """Show layout flag.
+
+        Returns
+        -------
+        bool
+           Fast transformation check box.
+
+        """
+        key = "Fast Transformation"
+        if key in self._primitives._app.get_oo_properties(self._primitives.oeditor, self._name):
+            fast_transformation = self._primitives._app.get_oo_property_value(self._primitives.oeditor, self._name, key)
+            self._fast_transformation = fast_transformation
+            return fast_transformation
+        else:  # pragma: no cover
+            return None
+
+    @fast_transformation.setter
+    def fast_transformation(self, fast_transformation):
+        key = "Fast Transformation"
+        if isinstance(fast_transformation, bool) and key in self._primitives._app.get_oo_properties(
+            self._primitives.oeditor, self._name
+        ):
+            self._primitives.oeditor.GetChildObject(self._name).SetPropValue(key, fast_transformation)
+            self._fast_transformation = fast_transformation
+
+    @property
+    def show_dielectric(self):
+        """Show dielectric flag.
+
+        Returns
+        -------
+        bool
+           Show dielectric check box.
+
+        """
+        key = "Object Attributes/ShowDielectric"
+
+        if key in self._primitives._app.get_oo_properties(self._primitives.oeditor, self._name):
+            show_dielectric = self._primitives._app.get_oo_property_value(self._primitives.oeditor, self._name, key)
+            self._show_dielectric = show_dielectric
+            return show_dielectric
+        else:  # pragma: no cover
+            return None
+
+    @show_dielectric.setter
+    def show_dielectric(self, show_dielectric):
+        key = "Object Attributes/ShowDielectric"
+        if isinstance(show_dielectric, bool) and key in self._primitives._app.get_oo_properties(
+            self._primitives.oeditor, self._name
+        ):
+            self._primitives.oeditor.GetChildObject(self._name).SetPropValue(key, show_dielectric)
+            self._show_dielectric = show_dielectric
+
+    @property
+    def display_mode(self):
+        """Show layout flag.
+
+        Returns
+        -------
+        int
+           Layout display mode. Available modes are:
+            * 0 : Layer.
+            * 1 : Net.
+            * 2 : Object.
+
+        """
+        key = "Object Attributes/DisplayMode"
+
+        if key in self._primitives._app.get_oo_properties(self._primitives.oeditor, self._name):
+            display_mode = self._primitives._app.get_oo_property_value(self._primitives.oeditor, self._name, key)
+            self._display_mode = display_mode
+            return display_mode
+        else:  # pragma: no cover
+            return None
+
+    @display_mode.setter
+    def display_mode(self, display_mode):
+        key = "Object Attributes/DisplayMode"
+        if isinstance(display_mode, int) and key in self._primitives._app.get_oo_properties(
+            self._primitives.oeditor, self._name
+        ):
+            self._primitives.oeditor.GetChildObject(self._name).SetPropValue(key, display_mode)
+            self._display_mode = display_mode
+
+    @pyaedt_function_handler()
+    def _get_edb_info(self):
+        """Get Edb information."""
+
+        # Open Layout component and get information
+        aedb_component_path = os.path.join(
+            self._primitives._app.project_file[:-1] + "b",
+            "LayoutComponents",
+            self._edb_definition,
+            self._edb_definition + ".aedb",
+        )
+
+        if not os.path.exists(aedb_component_path):  # pragma: no cover
+            return False
+
+        component_obj = Edb(
+            edbpath=aedb_component_path,
+            isreadonly=True,
+            edbversion=self._primitives._app._aedt_version,
+            student_version=self._primitives._app.student_version,
+        )
+
+        # Get objects, nets and layers
+        self.nets = {key: [True, False, 60] for key in component_obj.nets.netlist}
+        self.layers = {key: [True, False, 60] for key in list(component_obj.stackup.stackup_layers.keys())}
+        self.objects = {key: [True, False, 60] for key in list(component_obj.components.instances.keys())}
+
+        component_obj.close_edb()
+
+        return True
+
+    @pyaedt_function_handler()
+    def update_visibility(self):
+        """Update layer visibility.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        References
+        ----------
+
+        >>> oEditor.ChangeProperty
+        """
+
+        vPropChange = [
+            "NAME:Object Attributes",
+            "ShowDielectric:=",
+            self.show_dielectric,
+            "DisplayMode:=",
+            self.display_mode,
+        ]
+
+        if self.layers:
+            layer_mode = ["NAME:ObjectAttributesInLayerMode"]
+            for layer in self.layers:
+                layer_mode.append(layer + ":=")
+                layer_mode.append(self.layers[layer])
+            vPropChange.append(layer_mode)
+        if self.nets:
+            net_mode = ["NAME:ObjectAttributesInNetMode"]
+            for net in self.nets:
+                net_mode.append(layer + ":=")
+                net_mode.append(self.nets[net])
+            vPropChange.append(net_mode)
+        if self.objects:
+            objects_mode = ["NAME:ObjectAttributesInObjectMode"]
+            for objects in self.objects:
+                objects_mode.append(objects + ":=")
+                objects_mode.append(self.objects[objects])
+            vPropChange.append(objects_mode)
+
+        vChangedProps = ["NAME:ChangedProps", vPropChange]
+        vPropServers = ["NAME:PropServers", self._name]
+        vGeo3d = ["NAME:Visualization", vPropServers, vChangedProps]
+        vOut = ["NAME:AllTabs", vGeo3d]
+        _retry_ntimes(10, self._primitives.oeditor.ChangeProperty, vOut)
+
+        return True
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.82/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/calculators.py` & `pyaedt-0.6.82/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import os
 import random
 import re
 import warnings
 
 from pyaedt.application.Variables import decompose_variable_value
-from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
+from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
@@ -1854,15 +1854,16 @@
         :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
             Circuit Component Object.
         """
         assert os.path.exists(model_path), "Project file doesn't exist"
         comp_name = os.path.splitext(os.path.basename(model_path))[0]
         results_path = model_path + "averesults"
         solution = os.path.join(results_path, comp_name + ".asol")
-        out = load_entire_aedt_file(solution)
+        # out = load_entire_aedt_file(solution)
+        out = load_keyword_in_aedt_file(solution, "Solutions")
         if not solution_name:
             solution_name = list(out["Solutions"]["SYZSolutions"].keys())[0]
         results_folder = os.path.join(
             results_path,
             out["Solutions"]["SYZSolutions"][solution_name]["DiskName"],
             out["Solutions"]["SYZSolutions"][solution_name]["DiskName"] + ".syzinfo",
         )
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.82/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,20 +537,19 @@
         """
         if self._pins:
             return self._pins
         self._pins = []
 
         try:
             pins = _retry_ntimes(10, self._oeditor.GetComponentPins, self.composed_name)
-
-            if not pins:
-                return []
-            elif pins is True:
+            if "Port@" in self.composed_name and pins == []:
                 self._pins.append(CircuitPins(self, self.composed_name))
                 return self._pins
+            elif not pins:
+                return []
             for pin in pins:
                 if self._circuit_components._app.design_type != "Twin Builder":
                     self._pins.append(CircuitPins(self, pin))
                 elif pin not in list(self.parameters.keys()):
                     self._pins.append(CircuitPins(self, pin))
         except AttributeError:
             self._pins.append(CircuitPins(self, self.composed_name))
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.82/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.82/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.82/pyaedt/modeler/modeler3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.82/pyaedt/modeler/modelerpcb.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,18 +44,22 @@
         self.logger.info("Modeler loaded.")
         self.logger.info("EDB loaded.")
         self.layers = Layers(self, roughnessunits="um")
         self.logger.info("Layers loaded.")
         Primitives3DLayout.__init__(self, app)
         self._primitives = self
         self.logger.info("Primitives loaded.")
-        self.o_def_manager = self._app.odefinition_manager
         self.rigid_flex = None
 
     @property
+    def o_def_manager(self):
+        """AEDT Definition manager."""
+        return self._app.odefinition_manager
+
+    @property
     def stackup(self):
         """Get the Stackup class and its methods.
 
         Returns
         -------
         :class:`pyaedt.modules.LayerStackup.Layers`
         """
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.82/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.82/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,37 +317,50 @@
                     locs.append(i)
             return locs
         else:
             return None
 
     @location.setter
     def location(self, position):
+        if self.prim_type in ["component", "pin", "via"]:
+            props = [
+                "NAME:Location",
+                "X:=",
+                self._primitives.number_with_units(position[0]),
+                "Y:=",
+                self._primitives.number_with_units(position[1]),
+            ]
+            self.change_property(props)
         if self.prim_type == "component":
             info = self._oeditor.GetComponentInfo(self.name)
             bbllx = bblly = bburx = bbury = 0
             for i in info:
                 if "BBoxLLx" in i:
                     bbllx = float(i.split("=")[1])
                 elif "BBoxLLy" in i:
                     bblly = float(i.split("=")[1])
                 elif "BBoxURx" in i:
                     bburx = float(i.split("=")[1])
                 elif "BBoxURy" in i:
                     bbury = float(i.split("=")[1])
-            position[0] -= unit_converter((bburx + bbllx) / 2, output_units=self._primitives.model_units)
-            position[1] -= unit_converter((bbury + bblly) / 2, output_units=self._primitives.model_units)
-        if self.prim_type in ["component", "pin", "via"]:
-            props = [
-                "NAME:Location",
-                "X:=",
-                self._primitives.number_with_units(position[0]),
-                "Y:=",
-                self._primitives.number_with_units(position[1]),
-            ]
-            self.change_property(props)
+            position[0] -= self.location[0] - unit_converter(
+                (bburx + bbllx) / 2, output_units=self._primitives.model_units
+            )
+            position[1] -= self.location[1] - unit_converter(
+                (bbury + bblly) / 2, output_units=self._primitives.model_units
+            )
+            if abs(position[0]) > 1e-12 or abs(position[1]) > 1e-12:
+                props = [
+                    "NAME:Location",
+                    "X:=",
+                    self._primitives.number_with_units(position[0]),
+                    "Y:=",
+                    self._primitives.number_with_units(position[1]),
+                ]
+                self.change_property(props)
 
     @property
     def lock_position(self):
         """Get/Set the lock position.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.81/pyaedt/modeler/schematic.py` & `pyaedt-0.6.82/pyaedt/modeler/schematic.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,23 @@
     >>> app = Circuit()
     >>> my_modeler = app.modeler
     """
 
     def __init__(self, app):
         self._app = app
         self._schematic_units = "meter"
-        self.o_def_manager = self._app.odefinition_manager
         Modeler.__init__(self, app)
         self.wire = Wire(self)
 
     @property
+    def o_def_manager(self):
+        """AEDT Definition manager."""
+        return self._app.odefinition_manager
+
+    @property
     def schematic_units(self):
         """Schematic units.
 
         Options are ``"mm"``, ``"mil"``, ``"cm"`` and all other metric and imperial units.
         The default is ``"meter"``.
         """
         return self._schematic_units
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.82/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/Boundary.py` & `pyaedt-0.6.82/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.82/pyaedt/modules/CableModeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1404,10 +1404,11 @@
             except ValueError as e:
                 self._app.logger.error(str(e))
 
     def _cable_properties_parser(self, omodule, working_dir):
         file_path_export = os.path.join(working_dir, "export_cable_library_test.txt")
         omodule.ExportCableLibrary(file_path_export)
         file_path_export_as_json = os.path.join(working_dir, "export_cable_library_as_json_test.json")
+        data = load_entire_aedt_file(file_path_export)
         with open(file_path_export_as_json, "w") as f:
-            json.dump(load_entire_aedt_file(file_path_export), f)
-        return load_entire_aedt_file(file_path_export)
+            json.dump(data, f)
+        return data
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.82/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.82/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.82/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/Material.py` & `pyaedt-0.6.82/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.82/pyaedt/modules/MaterialLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,27 +42,35 @@
     >>> app = Hfss()
     >>> materials = app.materials
     """
 
     def __init__(self, app):
         self._app = app
         self._color_id = 0
-        self.odefinition_manager = self._app.odefinition_manager
-        self.omaterial_manager = self._app.omaterial_manager
         self._mats = []
         self._mats_lower = []
         self._desktop = self._app.odesktop
         self._oproject = self._app.oproject
         self.logger = self._app.logger
         self.logger.info("Successfully loaded project materials !")
         # self.material_keys = self._get_materials()
         self.material_keys = {}
         self._surface_material_keys = {}
         self._load_from_project()
 
+    @property
+    def odefinition_manager(self):
+        """Definition Manager from AEDT."""
+        return self._app.odefinition_manager
+
+    @property
+    def omaterial_manager(self):
+        """Material Manager from AEDT."""
+        return self._app.omaterial_manager
+
     def __len__(self):
         return len(self.material_keys)
 
     def __iter__(self):
         return iter(self.material_keys.values()) if sys.version_info.major > 2 else self.material_keys.itervalues()
 
     def __getitem__(self, item):
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/Mesh.py` & `pyaedt-0.6.82/pyaedt/modules/Mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from collections import OrderedDict
 import os
 import shutil
 
 from pyaedt.application.design_solutions import model_names
 from pyaedt.generic.DataHandlers import _dict2arg
-from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
+from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import MethodNotSupportedError
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
@@ -185,22 +185,26 @@
         >>> oModule.EditLengthOp
         >>> oModule.EditApplyCurvlinearElementsOp
         >>> oModule.EditRotationalLayerOp
         >>> oModule.EditDensityControlOp
         >>> oModule.EditMeshOperation
         >>> oModule.EditSBRCurvatureExtractionOp
         """
-        if key_name and settings.aedt_version > "2022.2":
-            mesh_obj = self._mesh._app.odesign.GetChildObject("Mesh").GetChildObject(self.name)
-            if key_name in mesh_props.keys():
-                if key_name == "SurfaceRepPriority":
-                    value = "Normal" if value == 0 else "High"
-                key_name = mesh_props[key_name]
-            mesh_obj.SetPropValue(key_name, value)
-            return True
+        mesh_names = self._mesh._app.odesign.GetChildObject("Mesh").GetChildNames()
+        if key_name and settings.aedt_version > "2022.2" and self.name in mesh_names:
+            try:
+                mesh_obj = self._mesh._app.odesign.GetChildObject("Mesh").GetChildObject(self.name)
+                if key_name in mesh_props.keys():
+                    if key_name == "SurfaceRepPriority":
+                        value = "Normal" if value == 0 else "High"
+                    key_name = mesh_props[key_name]
+                mesh_obj.SetPropValue(key_name, value)
+                return True
+            except:
+                self._app.logger.info("Failed to use Child Object. Trying with legacy update.")
 
         if self.type == "SurfApproxBased":
             self._mesh.omeshmodule.EditTrueSurfOp(self.name, self._get_args())
         elif self.type == "DefeatureBased":
             self._mesh.omeshmodule.EditModelResolutionOp(self.name, self._get_args())
         elif self.type == "SurfaceRepPriority":
             self._mesh.omeshmodule.EditSurfPriorityForTauOp(self.name, self._get_args())
@@ -214,15 +218,15 @@
             self._mesh.omeshmodule.EditRotationalLayerOp(self.name, self._get_args())
         elif self.type == "DensityControlBased":
             self._mesh.omeshmodule.EditDensityControlOp(self.name, self._get_args())
         elif self.type == "Icepak":
             self._mesh.omeshmodule.EditMeshOperation(self.name, self._get_args())
         elif self.type == "CurvatureExtraction":
             self._mesh.omeshmodule.EditSBRCurvatureExtractionOp(self.name, self._get_args())
-        elif self.type == "InitialMeshSettings":
+        elif self.type in ["InitialMeshSettings", "MeshSettings"]:
             self._mesh.omeshmodule.InitialMeshSettings(self._get_args())
         elif self.type == "CylindricalGap":
             self._mesh.omeshmodule.EditCylindricalGapOp(self.name, self._get_args())
         else:
             return False
         return True
 
@@ -464,15 +468,16 @@
             elif self._app.solution_type == "Terminal":
                 sol = "HFSS Terminal Network"
             else:
                 sol = self._app.solution_type
             oproject_target.InsertDesign(self._app.design_type, temp_name, sol, "")
             oproject_target.SaveAs(temp_proj, True)
             self._app.odesktop.CloseProject(temp_name)
-            _project_dictionary = load_entire_aedt_file(temp_proj)
+            # _project_dictionary = load_entire_aedt_file(temp_proj)
+            _project_dictionary = load_keyword_in_aedt_file(temp_proj, "AnsoftProject")
             try:
                 props = _project_dictionary["AnsoftProject"][model_names[self._app.design_type]]["MeshSetup"][
                     "MeshSettings"
                 ]
             except:
                 pass
             if os.path.exists(temp_proj):
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.82/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.82/pyaedt/modules/MeshIcepak.py`

 * *Files 3% similar despite different names*

```diff
@@ -281,18 +281,25 @@
             else:
                 args = ["NAME:" + self.name, "Enable:=", self.Enable]
             if self.UserSpecifiedSettings:
                 args += self.manualsettings
             else:
                 args += self.autosettings
             if self.name == "Settings":
-                self.meshmodule.EditGlobalMeshRegion(args)
+                try:
+                    self.meshmodule.EditGlobalMeshRegion(args)
+                    return True
+                except Exception:  # pragma : no cover
+                    return False
             else:
-                self.meshmodule.EditMeshRegion(self.name, args)
-            return True
+                try:
+                    self.meshmodule.EditMeshRegion(self.name, args)
+                    return True
+                except Exception:  # pragma : no cover
+                    return False
 
         @pyaedt_function_handler()
         def create(self):
             """Create a new mesh region.
 
             Returns
             -------
@@ -311,14 +318,32 @@
                 args += self.manualsettings
             else:
                 args += self.autosettings
             if self.virtual_region and self._app.check_beta_option_enabled("S544753_ICEPAK_VIRTUALMESHREGION_PARADIGM"):
                 self.meshmodule.AssignVirtualMeshRegion(args)
             else:
                 self.meshmodule.AssignMeshRegion(args)
+            self._app.mesh.meshregions.append(self)
+            return True
+
+        @pyaedt_function_handler()
+        def delete(self):
+            """Delete mesh region.
+
+            Returns
+            -------
+            bool
+                ``True`` when successful, ``False`` when failed.
+
+            References
+            ----------
+
+            >>> oModule.DeleteMeshRegions()
+            """
+            self.meshmodule.DeleteMeshRegions([self.name])
             return True
 
     @property
     def boundingdimension(self):
         """Bounding dimension."""
         return self.modeler.get_bounding_dimension()
 
@@ -639,43 +664,52 @@
         if not objectlist:
             objectlist = [i for i in self.modeler.object_names]
         if is_submodel:
             meshregion.SubModels = objectlist
         else:
             meshregion.Objects = objectlist
         all_objs = [i for i in self.modeler.object_names]
-        meshregion.create()
-        objectlist2 = self.modeler.object_names
-        added_obj = [i for i in objectlist2 if i not in all_objs]
-        if not added_obj:
-            added_obj = [i for i in objectlist2 if i not in all_objs or i in objectlist]
-        meshregion.Objects = added_obj
-        meshregion.SubModels = None
-        self.meshregions.append(meshregion)
-        return meshregion
+        try:
+            meshregion.create()
+            created = True
+        except Exception:  # pragma : no cover
+            created = False
+        if created:
+            objectlist2 = self.modeler.object_names
+            added_obj = [i for i in objectlist2 if i not in all_objs]
+            if not added_obj:
+                added_obj = [i for i in objectlist2 if i not in all_objs or i in objectlist]
+            meshregion.Objects = added_obj
+            meshregion.SubModels = None
+            meshregion.update()
+            return meshregion
+        else:
+            return False
 
     @pyaedt_function_handler()
-    def generate_mesh(self, name):
+    def generate_mesh(self, name=None):
         """Generate the mesh for a given setup name.
 
         Parameters
         ----------
-        name : str
-            Name of the design to mesh.
+        name : str, optional
+            Name of the design to mesh. Default is ``None`` in which case the first available setup will be selected.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oDesign.GenerateMesh
         """
+        if name is None:
+            name = []
         return self._odesign.GenerateMesh(name) == 0
 
     @pyaedt_function_handler()
     def assign_mesh_level_to_group(
         self,
         mesh_level,
         groupName,
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.82/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.82/pyaedt/modules/PostProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -2596,15 +2596,15 @@
             ]
         ]
         self.ofieldsreporter.SetPlotFolderSettings(plot_name, args)
         return True
 
     @pyaedt_function_handler()
     def _create_fieldplot(self, objlist, quantityName, setup_name, intrinsics, listtype, plot_name=None):
-        if not listtype.startswith("Layer"):
+        if not listtype.startswith("Layer") and self._app.design_type != "HFSS 3D Layout Design":
             objlist = self._app.modeler.convert_to_selections(objlist, True)
         if not setup_name:
             setup_name = self._app.existing_analysis_sweeps[0]
         if not intrinsics:
             for i in self._app.setups:
                 if i.name == setup_name.split(" : ")[0]:
                     intrinsics = i.default_intrinsics
@@ -2897,22 +2897,34 @@
             Plot object.
 
         References
         ----------
 
         >>> oModule.CreateFieldPlot
         """
-        if not ("APhi" in self.post_solution_type and settings.aedt_version >= "2023.2"):
+        if not (
+            "APhi" in self.post_solution_type and settings.aedt_version >= "2023.2"
+        ) and not self._app.design_type in ["HFSS", "HFSS 3D Layout Design"]:
             self.logger.error("This method requires AEDT 2023 R2 and Maxwell 3D Transient APhi Formulation.")
             return False
         if intrinsics is None:
             intrinsics = {}
         if plot_name and plot_name in list(self.field_plots.keys()):
             self.logger.info("Plot {} exists. returning the object.".format(plot_name))
             return self.field_plots[plot_name]
+        if self._app.design_type == "HFSS 3D Layout Design":
+            if not setup_name:
+                setup_name = self._app.existing_analysis_sweeps[0]
+            lst = []
+            for layer in layers_nets:
+                for el in layer[1:]:
+                    get_ids = self._odesign.GetGeometryIdsForNetLayerCombination(el, layer[0], setup_name)
+                    if isinstance(get_ids, (tuple, list)) and len(get_ids) > 2:
+                        lst.extend([int(i) for i in get_ids[2:]])
+            return self._create_fieldplot(lst, quantity_name, setup_name, intrinsics, "FacesList", plot_name)
         if plot_on_surface:
             plot_type = "LayerNetsExtFace"
         else:
             plot_type = "LayerNets"
         return self._create_fieldplot(layers_nets, quantity_name, setup_name, intrinsics, plot_type, plot_name)
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.82/pyaedt/modules/SetupTemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1588,15 +1588,15 @@
 
 list_modules = dir()
 
 
 class SetupKeys:
     """Provides setup keys."""
 
-    SetupNames = [  # TODO: HFSSDriven appears twice. Is this correct?
+    SetupNames = [
         "HFSSDrivenAuto",
         "HFSSDriven",
         "HFSSEigen",
         "HFSSTransient",
         "HFSSDriven",
         "Transient",
         "Magnetostatic",
@@ -1645,14 +1645,15 @@
         "PMDC",
         "SRM",
         "LSSM",
         "UNIM",
         "DCM",
         "CPSM",
         "NSSM",
+        "TransientAPhiFormulation",
     ]
 
     SetupTemplates = {
         0: HFSSDrivenAuto,
         1: HFSSDrivenDefault,
         2: HFSSEigen,
         3: HFSSTransient,
@@ -1704,14 +1705,15 @@
         49: PMDC,
         50: SRM,
         51: LSSM,
         52: UNIM,
         53: DCM,
         54: CPSM,
         55: NSSM,
+        56: MaxwellTransient,
     }
 
     SetupTemplates_231 = {
         29: HFSS3DLayout_v231,
     }
     SetupTemplates_232 = {}
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.82/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.82/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.82/pyaedt/modules/monitor_icepak.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,48 @@
 from pyaedt.generic.constants import SI_UNITS
 from pyaedt.generic.constants import unit_system
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
+quantities_dict = {  # pragma: no cover
+    8: "Speed",
+    9: "Pressure",
+    10: "TKE",
+    11: "Epsilon",
+    12: "ViscosityRatio",
+    16: "MassFlow",
+    17: "VolumeFlow",
+    18: "WallYPlus",
+    19: "Temperature",
+    20: "K_X",
+    21: "K_Y",
+    22: "K_Z",
+    29: "HeatFlux",
+    31: "HeatFlowRate",
+}
+
+quantities_type_dict = {  # pragma: no cover
+    "Speed": ["Point"],
+    "Pressure": ["Point"],
+    "TKE": ["Point"],
+    "Epsilon": ["Point"],
+    "ViscosityRatio": ["Point"],
+    "MassFlow": ["Face"],
+    "VolumeFlow": ["Face"],
+    "WallYPlus": ["Point"],
+    "Temperature": ["Point", "Face"],
+    "K_X": ["Point"],
+    "K_Y": ["Point"],
+    "K_Z": ["Point"],
+    "HeatFlux": ["Point"],
+    "HeatFlowRate": ["Face"],
+}
+
 
 class Monitor:
     """Provides Icepak monitor methods."""
 
     def __init__(self, p_app):
         self._face_monitors = {}
         self._point_monitors = {}
@@ -29,16 +63,24 @@
         for point in self._app.oeditor.GetPoints():
             point_pos = self._app.oeditor.GetChildObject(point).GetPropValue("Position")
             if all(point_pos[2 * i + 1] == position[i] for i in range(3)):
                 return point
         return None
 
     @pyaedt_function_handler
+    def _check_quantities(self, quantities):
+        if all(q in quantities_dict.values() for q in quantities):
+            return [monitor_type for q in quantities for monitor_type in quantities_type_dict[q]]
+        else:
+            self._app.logger.error("Invalid quantities selected.")
+            return []
+
+    @pyaedt_function_handler
     def _generate_monitor_names(self, name, n):
-        """Create list of names for monitor objects following Icepak naming rules.
+        """Create a list of names for monitor objects following Icepak naming rules.
 
         Parameters
         ----------
         name : str
             Name for the first monitor object
         n : int
             Number of names to be generated
@@ -67,30 +109,14 @@
                     names.append(candidate_name)
                     n_names_left -= 1
                 n += 1
             return names
 
     @pyaedt_function_handler
     def _load_monitor_objects(self, aedtfile_monitor_dict):
-        quantities_dict = {  # pragma: no cover
-            8: "Speed",
-            9: "Pressure",
-            10: "TKE",
-            11: "Epsilon",
-            12: "ViscosityRatio",
-            16: "MassFlow",
-            17: "VolumeFlow",
-            18: "WallYPlus",
-            19: "Temperature",
-            20: "K_X",
-            21: "K_Y",
-            22: "K_Z",
-            29: "HeatFlux",
-            31: "HeatFlowRate",
-        }
         for monitor_name, monitor_prop in aedtfile_monitor_dict.items():
             if "Faces" in monitor_prop.keys():
                 self._face_monitors[monitor_name] = FaceMonitor(
                     monitor_name,
                     "Face",
                     monitor_prop["Faces"][0],
                     [quantities_dict[i] for i in monitor_prop["Quantities"]],
@@ -144,15 +170,15 @@
         -------
         oEditor COM Object
         """
         return self._app.odesign.GetChildObject("Monitor").GetChildObject(monitor_name)
 
     @property
     def face_monitors(self):
-        """Get face monitor objects.
+        """Get point monitor objects.
 
         Returns
         -------
         dict
             Face monitor objects dictionary.
 
         """
@@ -227,44 +253,47 @@
         else:
             point_names = []
             if not isinstance(point_position[0], list):
                 point_position = [point_position]
 
         if not isinstance(monitor_quantity, list):
             monitor_quantity = [monitor_quantity]
-        for p_p in point_position:
-            point_name = generate_unique_name("Point")
-            self._app.modeler.oeditor.CreatePoint(
-                [
-                    "NAME:PointParameters",
-                    "PointX:=",
-                    self._app.modeler._arg_with_dim(p_p[0]),
-                    "PointY:=",
-                    self._app.modeler._arg_with_dim(p_p[1]),
-                    "PointZ:=",
-                    self._app.modeler._arg_with_dim(p_p[2]),
-                ],
-                ["NAME:Attributes", "Name:=", point_name, "Color:=", "(143 175 143)"],
+        if "Point" in self._check_quantities(monitor_quantity):
+            for p_p in point_position:
+                point_name = generate_unique_name("Point")
+                self._app.modeler.oeditor.CreatePoint(
+                    [
+                        "NAME:PointParameters",
+                        "PointX:=",
+                        self._app.modeler._arg_with_dim(p_p[0]),
+                        "PointY:=",
+                        self._app.modeler._arg_with_dim(p_p[1]),
+                        "PointZ:=",
+                        self._app.modeler._arg_with_dim(p_p[2]),
+                    ],
+                    ["NAME:Attributes", "Name:=", point_name, "Color:=", "(143 175 143)"],
+                )
+                point_names.append(point_name)
+            if not monitor_name:
+                monitor_name = generate_unique_name("Monitor")
+            self._omonitor.AssignPointMonitor(
+                ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Points:=", point_names]
             )
-            point_names.append(point_name)
-        if not monitor_name:
-            monitor_name = generate_unique_name("Monitor")
-        self._omonitor.AssignPointMonitor(
-            ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Points:=", point_names]
-        )
-        try:
-            monitor_names = self._generate_monitor_names(monitor_name, len(point_names))
-            for i, mn in enumerate(monitor_names):
-                self._point_monitors[mn] = PointMonitor(mn, "Point", point_names[i], monitor_quantity, self._app)
-        except:  # pragma: no cover
-            return False
-        if len(monitor_names) == 1:
-            return monitor_names[0]
+            try:
+                monitor_names = self._generate_monitor_names(monitor_name, len(point_names))
+                for i, mn in enumerate(monitor_names):
+                    self._point_monitors[mn] = PointMonitor(mn, "Point", point_names[i], monitor_quantity, self._app)
+            except:  # pragma: no cover
+                return False
+            if len(monitor_names) == 1:
+                return monitor_names[0]
+            else:
+                return monitor_names
         else:
-            return monitor_names
+            return False
 
     @pyaedt_function_handler()
     def assign_point_monitor_to_vertex(self, vertex_id, monitor_quantity="Temperature", monitor_name=None):
         """Create and assign a point monitor to a vertex.
 
         Parameters
         ----------
@@ -289,27 +318,29 @@
         """
         if isinstance(vertex_id, int):
             vertex_id = [vertex_id]
         if isinstance(monitor_quantity, str):
             monitor_quantity = [monitor_quantity]
         if not monitor_name:
             monitor_name = generate_unique_name("Monitor")
-        self._omonitor.AssignPointMonitor(
-            ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Vertices:=", vertex_id]
-        )
-        try:
-            monitor_names = self._generate_monitor_names(monitor_name, len(vertex_id))
-            for i, mn in enumerate(monitor_names):
-                self._point_monitors[mn] = PointMonitor(mn, "Vertex", vertex_id[i], monitor_quantity, self._app)
-        except:  # pragma: no cover
-            return False
-        if len(monitor_names) == 1:
-            return monitor_names[0]
-        else:
-            return monitor_names
+        if "Point" in self._check_quantities(monitor_quantity):
+            self._omonitor.AssignPointMonitor(
+                ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Vertices:=", vertex_id]
+            )
+            try:
+                monitor_names = self._generate_monitor_names(monitor_name, len(vertex_id))
+                for i, mn in enumerate(monitor_names):
+                    self._point_monitors[mn] = PointMonitor(mn, "Vertex", vertex_id[i], monitor_quantity, self._app)
+            except:  # pragma: no cover
+                return False
+            if len(monitor_names) == 1:
+                return monitor_names[0]
+            else:
+                return monitor_names
+        return False
 
     @pyaedt_function_handler()
     def assign_surface_monitor(self, surface_name, monitor_quantity="Temperature", monitor_name=None):
         """Assign a surface monitor.
 
         Parameters
         ----------
@@ -343,27 +374,30 @@
         """
         if isinstance(surface_name, str):
             surface_name = [surface_name]
         if isinstance(monitor_quantity, str):
             monitor_quantity = [monitor_quantity]
         if not monitor_name:
             monitor_name = generate_unique_name("Monitor")
-        self._omonitor.AssignFaceMonitor(
-            ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Objects:=", surface_name]
-        )
-        try:
-            monitor_names = self._generate_monitor_names(monitor_name, len(surface_name))
-            for i, mn in enumerate(monitor_names):
-                self._face_monitors[mn] = FaceMonitor(mn, "Surface", surface_name[i], monitor_quantity, self._app)
-        except:  # pragma: no cover
-            return False
-        if len(monitor_names) == 1:
-            return monitor_names[0]
+        if "Face" in self._check_quantities(monitor_quantity):
+            self._omonitor.AssignFaceMonitor(
+                ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Objects:=", surface_name]
+            )
+            try:
+                monitor_names = self._generate_monitor_names(monitor_name, len(surface_name))
+                for i, mn in enumerate(monitor_names):
+                    self._face_monitors[mn] = FaceMonitor(mn, "Surface", surface_name[i], monitor_quantity, self._app)
+            except:  # pragma: no cover
+                return False
+            if len(monitor_names) == 1:
+                return monitor_names[0]
+            else:
+                return monitor_names
         else:
-            return monitor_names
+            return False
 
     @pyaedt_function_handler()
     def assign_face_monitor(self, face_id, monitor_quantity="Temperature", monitor_name=None):
         """Assign a face monitor.
 
         Parameters
         ----------
@@ -387,25 +421,30 @@
         """
         if isinstance(face_id, int):
             face_id = [face_id]
         if isinstance(monitor_quantity, str):
             monitor_quantity = [monitor_quantity]
         if not monitor_name:
             monitor_name = generate_unique_name("Monitor")
-        self._omonitor.AssignFaceMonitor(["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Faces:=", face_id])
-        try:
-            monitor_names = self._generate_monitor_names(monitor_name, len(face_id))
-            for i, mn in enumerate(monitor_names):
-                self._face_monitors[mn] = FaceMonitor(mn, "Face", face_id[i], monitor_quantity, self._app)
-        except:  # pragma: no cover
-            return False
-        if len(monitor_names) == 1:
-            return monitor_names[0]
+        if "Face" in self._check_quantities(monitor_quantity):
+            self._omonitor.AssignFaceMonitor(
+                ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Faces:=", face_id]
+            )
+            try:
+                monitor_names = self._generate_monitor_names(monitor_name, len(face_id))
+                for i, mn in enumerate(monitor_names):
+                    self._face_monitors[mn] = FaceMonitor(mn, "Face", face_id[i], monitor_quantity, self._app)
+            except:  # pragma: no cover
+                return False
+            if len(monitor_names) == 1:
+                return monitor_names[0]
+            else:
+                return monitor_names
         else:
-            return monitor_names
+            return False
 
     @pyaedt_function_handler()
     def assign_point_monitor_in_object(self, name, monitor_quantity="Temperature", monitor_name=None):
         """Assign a point monitor in the centroid of a specific object.
 
         Parameters
         ----------
@@ -442,32 +481,37 @@
             monitor_quantity = [monitor_quantity]
         name_sel = self._app.modeler.convert_to_selections(name, True)
         original_monitors = list(self._app.odesign.GetChildObject("Monitor").GetChildNames())
         if not monitor_name:
             monitor_name = generate_unique_name("Monitor")
         elif monitor_name in original_monitors:
             monitor_name = generate_unique_name(monitor_name)
-        existing_names = list(set(name_sel).intersection(self._app.modeler.object_names))
-        if existing_names:
-            self._omonitor.AssignPointMonitor(
-                ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Objects:=", existing_names]
-            )
+        if "Point" in self._check_quantities(monitor_quantity):
+            existing_names = list(set(name_sel).intersection(self._app.modeler.object_names))
+            if existing_names:
+                self._omonitor.AssignPointMonitor(
+                    ["NAME:" + monitor_name, "Quantities:=", monitor_quantity, "Objects:=", existing_names]
+                )
+            else:
+                self._app.logger.error("Object is not present in the design")
+                return False
+            try:
+                monitor_names = self._generate_monitor_names(monitor_name, len(existing_names))
+                for i, mn in enumerate(monitor_names):
+                    self._point_monitors[mn] = PointMonitor(
+                        mn, "Object", existing_names[i], monitor_quantity, self._app
+                    )
+            except:  # pragma: no cover
+                return False
+            if len(monitor_names) == 1:
+                return monitor_names[0]
+            else:
+                return monitor_names
         else:
-            self._app.logger.error("Object is not present in the design")
             return False
-        try:
-            monitor_names = self._generate_monitor_names(monitor_name, len(existing_names))
-            for i, mn in enumerate(monitor_names):
-                self._point_monitors[mn] = PointMonitor(mn, "Object", existing_names[i], monitor_quantity, self._app)
-        except:  # pragma: no cover
-            return False
-        if len(monitor_names) == 1:
-            return monitor_names[0]
-        else:
-            return monitor_names
 
     @pyaedt_function_handler()
     def delete_monitor(self, monitor_name):
         """Delete monitor object.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.81/pyaedt/modules/report_templates.py` & `pyaedt-0.6.82/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/modules/solutions.py` & `pyaedt-0.6.82/pyaedt/modules/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2588,26 +2588,29 @@
             info.append("ObjList")
             info.append(len(self.volume_indexes))
             for index in self.volume_indexes:
                 info.append(str(index))
         if self.surfaces_indexes:
             model_faces = []
             nonmodel_faces = []
-            models = self._postprocessor.modeler.model_objects
-            for index in self.surfaces_indexes:
-                try:
-                    if isinstance(index, FacePrimitive):
-                        index = index.id
-                    oname = self._postprocessor.modeler.oeditor.GetObjectNameByFaceID(index)
-                    if oname in models:
-                        model_faces.append(str(index))
-                    else:
-                        nonmodel_faces.append(str(index))
-                except:
-                    pass
+            if self._postprocessor._app.design_type == "HFSS 3D Layout Design":
+                model_faces = [str(i) for i in self.surfaces_indexes]
+            else:
+                models = self._postprocessor.modeler.model_objects
+                for index in self.surfaces_indexes:
+                    try:
+                        if isinstance(index, FacePrimitive):
+                            index = index.id
+                        oname = self._postprocessor.modeler.oeditor.GetObjectNameByFaceID(index)
+                        if oname in models:
+                            model_faces.append(str(index))
+                        else:
+                            nonmodel_faces.append(str(index))
+                    except:
+                        pass
             info.append("Surface")
             if model_faces:
                 info.append("FacesList")
                 info.append(len(model_faces))
                 for index in model_faces:
                     info.append(index)
             if nonmodel_faces:
```

### Comparing `pyaedt-0.6.81/pyaedt/q3d.py` & `pyaedt-0.6.82/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/rmxprt.py` & `pyaedt-0.6.82/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.82/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.82/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.82/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.82/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.82/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/siwave.py` & `pyaedt-0.6.82/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyaedt/twinbuilder.py` & `pyaedt-0.6.82/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.81/pyproject.toml` & `pyaedt-0.6.82/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -31,58 +31,60 @@
     "rpyc==5.3.1",
     "psutil",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "ipython==8.13.0",
+    "ipython==8.13.0; python_version < '3.9'",
+    "ipython==8.14.0; python_version >= '3.9'",
     "imageio==2.31.1",
-    "joblib==1.2.0",
+    "joblib==1.3.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
     "numpy==1.25.0; python_version > '3.9'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.2; python_version > '3.7'",
-    "pytest==7.3.2",
+    "pytest==7.4.0",
     "pytest-cov==4.1.0",
     "pytest-xdist==3.3.1",
     "pyvista==0.39.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
     "imageio==2.31.1",
     "imageio-ffmpeg==0.4.8",
-    "ipython==8.13.0",
+    "ipython==8.13.0; python_version < '3.9'",
+    "ipython==8.14.0; python_version >= '3.9'",
     "ipywidgets==8.0.6",
-    "joblib==1.2.0",
+    "joblib==1.3.0",
     "jupyterlab==4.0.2",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pyvista==0.39.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "recommonmark==0.7.1",
     "scikit-learn==1.2.2",
     "Sphinx==7.0.1",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==1.23.2",
+    "sphinx-autodoc-typehints==1.23.3",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
     "utm",
     "scikit-rf",
```

### Comparing `pyaedt-0.6.81/PKG-INFO` & `pyaedt-0.6.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.81
+Version: 0.6.82
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -34,32 +34,33 @@
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: imageio==2.31.1 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
-Requires-Dist: ipython==8.13.0 ; extra == "doc"
+Requires-Dist: ipython==8.13.0 ; extra == "doc" and ( python_version < '3.9')
+Requires-Dist: ipython==8.14.0 ; extra == "doc" and ( python_version >= '3.9')
 Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
-Requires-Dist: joblib==1.2.0 ; extra == "doc"
+Requires-Dist: joblib==1.3.0 ; extra == "doc"
 Requires-Dist: jupyterlab==4.0.2 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pyvista==0.39.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "doc"
 Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.23.2 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.3 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
@@ -74,26 +75,27 @@
 Requires-Dist: osmnx ; extra == "full"
 Requires-Dist: pyvista==0.39.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
-Requires-Dist: ipython==8.13.0 ; extra == "tests"
+Requires-Dist: ipython==8.13.0 ; extra == "tests" and ( python_version < '3.9')
+Requires-Dist: ipython==8.14.0 ; extra == "tests" and ( python_version >= '3.9')
 Requires-Dist: imageio==2.31.1 ; extra == "tests"
-Requires-Dist: joblib==1.2.0 ; extra == "tests"
+Requires-Dist: joblib==1.3.0 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.9')
 Requires-Dist: numpy==1.25.0 ; extra == "tests" and ( python_version > '3.9')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.2 ; extra == "tests" and ( python_version > '3.7')
-Requires-Dist: pytest==7.3.2 ; extra == "tests"
+Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
 Requires-Dist: pyvista==0.39.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
```

