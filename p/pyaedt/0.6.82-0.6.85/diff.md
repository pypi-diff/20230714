# Comparing `tmp/pyaedt-0.6.82.tar.gz` & `tmp/pyaedt-0.6.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.82.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.85.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.82.tar` & `pyaedt-0.6.85.tar`

### file list

```diff
@@ -1,255 +1,258 @@
--rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.82/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.82/README.md
--rw-r--r--   0        0        0     2691 2023-06-30 08:45:32.173961 pyaedt-0.6.82/pyaedt/__init__.py
--rw-r--r--   0        0        0    26639 2023-06-15 12:39:09.822780 pyaedt-0.6.82/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88301 2023-06-21 14:18:52.796067 pyaedt-0.6.82/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    50849 2023-06-20 08:45:57.577348 pyaedt-0.6.82/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17066 2023-05-29 06:50:01.462409 pyaedt-0.6.82/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19852 2023-05-29 06:50:01.462409 pyaedt-0.6.82/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4431 2023-05-29 06:50:01.462409 pyaedt-0.6.82/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4596 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   129864 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75524 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.82/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36750 2023-06-29 10:10:15.395808 pyaedt-0.6.82/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62954 2023-05-26 06:18:30.544561 pyaedt-0.6.82/pyaedt/circuit.py
--rw-r--r--   0        0        0    10247 2023-06-05 09:37:00.357207 pyaedt-0.6.82/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    65852 2023-06-29 13:44:57.328647 pyaedt-0.6.82/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1086 2023-06-29 10:10:15.395808 pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23390 2023-06-14 08:55:18.804330 pyaedt-0.6.82/pyaedt/downloads.py
--rw-r--r--   0        0        0   137623 2023-06-29 16:42:04.115357 pyaedt-0.6.82/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    93329 2023-06-29 16:42:04.115357 pyaedt-0.6.82/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    31497 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     7909 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48210 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    33195 2023-06-12 08:03:15.118737 pyaedt-0.6.82/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40100 2023-05-29 06:50:01.477983 pyaedt-0.6.82/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.82/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      867 2023-05-26 06:18:30.544561 pyaedt-0.6.82/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12243 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65661 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20386 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     6856 2023-06-21 10:09:02.405348 pyaedt-0.6.82/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61171 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32590 2023-06-29 17:19:42.860399 pyaedt-0.6.82/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0   102298 2023-06-14 08:55:18.804330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36324 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    34575 2023-06-19 09:51:41.631657 pyaedt-0.6.82/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     3923 2023-06-05 14:55:02.766448 pyaedt-0.6.82/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2432 2023-06-05 09:10:35.931330 pyaedt-0.6.82/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    68725 2023-06-29 10:33:27.694259 pyaedt-0.6.82/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2850 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7763 2023-05-29 06:50:01.493602 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4703 2023-05-29 06:50:01.493602 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11390 2023-05-29 06:50:01.493602 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21800 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.82/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    47176 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33310 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    44030 2023-06-05 14:55:02.766448 pyaedt-0.6.82/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    48356 2023-06-29 12:57:01.275697 pyaedt-0.6.82/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    58809 2023-06-19 09:51:41.631657 pyaedt-0.6.82/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   109207 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11500 2023-06-14 05:38:07.853286 pyaedt-0.6.82/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     2813 2023-06-14 05:38:07.853286 pyaedt-0.6.82/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     1621 2023-06-14 05:38:07.853286 pyaedt-0.6.82/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-19 05:07:06.470308 pyaedt-0.6.82/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    13412 2023-06-17 11:56:24.503714 pyaedt-0.6.82/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    12252 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-26 11:30:35.579837 pyaedt-0.6.82/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83444 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-26 06:18:30.560187 pyaedt-0.6.82/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3395 2023-05-19 12:41:50.180833 pyaedt-0.6.82/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    69462 2023-06-29 10:10:15.395808 pyaedt-0.6.82/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.82/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62327 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11405 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3536 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60412 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   253082 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/hfss.py
--rw-r--r--   0        0        0    83113 2023-06-14 08:55:18.804330 pyaedt-0.6.82/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   199927 2023-06-29 13:44:57.328647 pyaedt-0.6.82/pyaedt/icepak.py
--rw-r--r--   0        0        0   126473 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24316 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.82/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3818 2023-05-19 06:53:58.810568 pyaedt-0.6.82/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.82/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14107 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20051 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16840 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120888 2023-05-29 06:50:01.509226 pyaedt-0.6.82/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   198276 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116971 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11387 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   129118 2023-06-29 17:19:42.860399 pyaedt-0.6.82/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.82/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    38399 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49138 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59754 2023-06-19 10:57:25.606048 pyaedt-0.6.82/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53131 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12645 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42629 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32781 2023-06-29 21:55:15.328018 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8212 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63170 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15149 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    32043 2023-06-29 19:22:14.082088 pyaedt-0.6.82/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6952 2023-05-29 06:50:01.524910 pyaedt-0.6.82/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    59936 2023-05-30 06:01:38.290945 pyaedt-0.6.82/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    32895 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    50072 2023-06-16 13:14:31.523832 pyaedt-0.6.82/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    66136 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23762 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   150771 2023-06-22 08:12:52.117360 pyaedt-0.6.82/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71535 2023-06-21 10:09:54.048412 pyaedt-0.6.82/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.82/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51967 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40465 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82903 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28517 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53616 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11976 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    27635 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   180536 2023-06-23 13:22:55.453306 pyaedt-0.6.82/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64120 2023-06-29 10:10:15.411431 pyaedt-0.6.82/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   121445 2023-06-15 11:58:34.060146 pyaedt-0.6.82/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33257 2023-05-29 06:50:01.540477 pyaedt-0.6.82/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    30706 2023-06-29 10:10:15.427058 pyaedt-0.6.82/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103333 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   126124 2023-06-23 13:22:55.453306 pyaedt-0.6.82/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95908 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/q3d.py
--rw-r--r--   0        0        0    10581 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.82/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7632 2023-05-29 06:50:01.556103 pyaedt-0.6.82/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10410 2023-06-05 09:10:35.946956 pyaedt-0.6.82/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.82/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4556 2023-06-30 08:45:32.173961 pyaedt-0.6.82/pyproject.toml
--rw-r--r--   0        0        0    15772 1970-01-01 00:00:00.000000 pyaedt-0.6.82/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.85/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.85/README.md
+-rw-r--r--   0        0        0     2691 2023-07-14 12:25:57.045581 pyaedt-0.6.85/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26756 2023-07-06 12:41:13.683251 pyaedt-0.6.85/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88917 2023-07-05 10:16:58.951877 pyaedt-0.6.85/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    50696 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17066 2023-05-29 06:50:01.462409 pyaedt-0.6.85/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19857 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-29 06:50:01.462409 pyaedt-0.6.85/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-29 06:50:01.477983 pyaedt-0.6.85/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   135985 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75595 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-29 06:50:01.477983 pyaedt-0.6.85/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36750 2023-06-29 10:10:15.395808 pyaedt-0.6.85/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62949 2023-07-12 14:57:59.361294 pyaedt-0.6.85/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10247 2023-06-05 09:37:00.357207 pyaedt-0.6.85/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    84902 2023-07-14 12:25:57.045581 pyaedt-0.6.85/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1086 2023-06-29 10:10:15.395808 pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    24039 2023-07-14 08:27:52.560421 pyaedt-0.6.85/pyaedt/downloads.py
+-rw-r--r--   0        0        0   137623 2023-06-29 16:42:04.115357 pyaedt-0.6.85/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    98675 2023-07-12 14:57:59.361294 pyaedt-0.6.85/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    31497 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     7909 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48210 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    33195 2023-06-12 08:03:15.118737 pyaedt-0.6.85/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40100 2023-05-29 06:50:01.477983 pyaedt-0.6.85/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      867 2023-05-26 06:18:30.544561 pyaedt-0.6.85/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12243 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65661 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20386 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     6880 2023-07-14 09:29:55.878674 pyaedt-0.6.85/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61171 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32590 2023-06-29 17:19:42.860399 pyaedt-0.6.85/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0   102298 2023-06-14 08:55:18.804330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36324 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    34944 2023-07-07 09:29:33.858435 pyaedt-0.6.85/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     3923 2023-06-05 14:55:02.766448 pyaedt-0.6.85/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2432 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    68725 2023-06-29 10:33:27.694259 pyaedt-0.6.85/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2850 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-29 06:50:01.493602 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-29 06:50:01.493602 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-29 06:50:01.493602 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21800 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47176 2023-06-22 08:12:52.117360 pyaedt-0.6.85/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33310 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    44030 2023-06-05 14:55:02.766448 pyaedt-0.6.85/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    49394 2023-07-07 09:29:33.858435 pyaedt-0.6.85/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    58809 2023-06-19 09:51:41.631657 pyaedt-0.6.85/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   109207 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11500 2023-07-05 14:41:01.487654 pyaedt-0.6.85/pyaedt/emit.py
+-rw-r--r--   0        0        0     6100 2023-07-05 14:41:01.487654 pyaedt-0.6.85/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     2813 2023-06-14 05:38:07.853286 pyaedt-0.6.85/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     1621 2023-06-14 05:38:07.853286 pyaedt-0.6.85/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-07-05 14:41:01.487654 pyaedt-0.6.85/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    13896 2023-07-05 14:41:01.503279 pyaedt-0.6.85/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    12252 2023-06-21 10:09:54.048412 pyaedt-0.6.85/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-26 11:30:35.579837 pyaedt-0.6.85/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83444 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-26 06:18:30.560187 pyaedt-0.6.85/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3442 2023-07-12 15:53:29.956835 pyaedt-0.6.85/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    70821 2023-07-14 12:25:57.045581 pyaedt-0.6.85/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0     9417 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/generic/grpc_plugin.py
+-rw-r--r--   0        0        0     3043 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/generic/grpc_plugin_dll.py
+-rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     7029 2023-07-12 14:57:59.361294 pyaedt-0.6.85/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11405 2023-06-22 08:12:52.117360 pyaedt-0.6.85/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3536 2023-06-21 10:09:54.048412 pyaedt-0.6.85/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   255506 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/hfss.py
+-rw-r--r--   0        0        0    84753 2023-07-06 12:04:15.245225 pyaedt-0.6.85/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   200124 2023-07-14 08:52:47.315413 pyaedt-0.6.85/pyaedt/icepak.py
+-rw-r--r--   0        0        0   127831 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24372 2023-07-06 12:04:15.245225 pyaedt-0.6.85/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3972 2023-07-07 09:29:33.874017 pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     3311 2023-07-07 09:29:33.874017 pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2620 2023-07-05 06:36:05.694306 pyaedt-0.6.85/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     5611 2023-07-07 09:29:33.874017 pyaedt-0.6.85/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120896 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   198119 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116735 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11407 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   129702 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    38322 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49140 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59316 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53078 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12645 2023-05-29 06:50:01.524910 pyaedt-0.6.85/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    43135 2023-07-14 12:06:38.284859 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    33551 2023-07-05 14:41:01.503279 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8236 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63132 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15185 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31781 2023-07-14 10:51:56.427377 pyaedt-0.6.85/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6956 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    64961 2023-07-14 12:06:38.284859 pyaedt-0.6.85/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    32782 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    50049 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65191 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23687 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    34537 2023-07-12 21:05:43.799165 pyaedt-0.6.85/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   159807 2023-07-06 12:04:15.260849 pyaedt-0.6.85/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71535 2023-06-21 10:09:54.048412 pyaedt-0.6.85/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28440 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53543 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11976 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    27635 2023-06-29 10:10:15.411431 pyaedt-0.6.85/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   181969 2023-07-11 09:19:45.845452 pyaedt-0.6.85/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64120 2023-06-29 10:10:15.411431 pyaedt-0.6.85/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   121445 2023-06-15 11:58:34.060146 pyaedt-0.6.85/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    30706 2023-06-29 10:10:15.427058 pyaedt-0.6.85/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-29 06:50:01.556103 pyaedt-0.6.85/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   126124 2023-06-23 13:22:55.453306 pyaedt-0.6.85/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95976 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-05-29 06:50:01.556103 pyaedt-0.6.85/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-29 06:50:01.556103 pyaedt-0.6.85/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10410 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4556 2023-07-14 07:11:37.571749 pyaedt-0.6.85/pyproject.toml
+-rw-r--r--   0        0        0    15772 1970-01-01 00:00:00.000000 pyaedt-0.6.85/PKG-INFO
```

### Comparing `pyaedt-0.6.82/LICENSE` & `pyaedt-0.6.85/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/README.md` & `pyaedt-0.6.85/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/__init__.py` & `pyaedt-0.6.85/pyaedt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.82"
+__version__ = "0.6.85"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
```

### Comparing `pyaedt-0.6.82/pyaedt/aedt_logger.py` & `pyaedt-0.6.85/pyaedt/aedt_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,32 +140,33 @@
 
         self._std_out_handler = None
         if settings.formatter:
             self.formatter = settings.formatter
         else:
             self.formatter = logging.Formatter(settings.logger_formatter, datefmt=settings.logger_datefmt)
         global_handler = False
-        for handler in self._global.handlers:
-            if settings.global_log_file_name in str(handler):
-                global_handler = True
-                break
-        log_file = os.path.join(tempfile.gettempdir(), settings.global_log_file_name)
-        my_handler = RotatingFileHandler(
-            log_file,
-            mode="a",
-            maxBytes=float(settings.global_log_file_size) * 1024 * 1024,
-            backupCount=2,
-            encoding=None,
-            delay=0,
-        )
-        my_handler.setFormatter(self.formatter)
-        my_handler.setLevel(self.level)
-        if not global_handler and settings.global_log_file_name:
-            self._global.addHandler(my_handler)
-        self._files_handlers.append(my_handler)
+        if settings.enable_global_log_file:
+            for handler in self._global.handlers:
+                if settings.global_log_file_name in str(handler):
+                    global_handler = True
+                    break
+            log_file = os.path.join(tempfile.gettempdir(), settings.global_log_file_name)
+            my_handler = RotatingFileHandler(
+                log_file,
+                mode="a",
+                maxBytes=float(settings.global_log_file_size) * 1024 * 1024,
+                backupCount=2,
+                encoding=None,
+                delay=0,
+            )
+            my_handler.setFormatter(self.formatter)
+            my_handler.setLevel(self.level)
+            if not global_handler and settings.global_log_file_name:
+                self._global.addHandler(my_handler)
+            self._files_handlers.append(my_handler)
         if self.filename and os.path.exists(self.filename):
             shutil.rmtree(self.filename, ignore_errors=True)
         if self.filename and settings.enable_local_log_file:
             self.add_file_logger(self.filename, "Global", level)
 
         if to_stdout:
             settings.enable_screen_logs = True
```

### Comparing `pyaedt-0.6.82/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.85/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/application/Analysis.py` & `pyaedt-0.6.85/pyaedt/application/Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,59 +433,70 @@
     def get_traces_for_plot(
         self,
         get_self_terms=True,
         get_mutual_terms=True,
         first_element_filter=None,
         second_element_filter=None,
         category="dB(S",
+        differential_pairs=[],
     ):
+        # type: (bool, bool, str, str, str, list) -> list
         """Retrieve a list of traces of specified designs ready to use in plot reports.
 
         Parameters
         ----------
         get_self_terms : bool, optional
             Whether to return self terms. The default is ``True``.
         get_mutual_terms : bool, optional
             Whether to return mutual terms. The default is ``True``.
         first_element_filter : str, optional
             Filter to apply to the first element of the equation.
             This parameter accepts ``*`` and ``?`` as special characters. The default is ``None``.
         second_element_filter : str, optional
             Filter to apply to the second element of the equation.
             This parameter accepts ``*`` and ``?`` as special characters. The default is ``None``.
-        category : str
+        category : str, optional
             Plot category name as in the report (including operator).
             The default is ``"dB(S"``,  which is the plot category name for capacitance.
+        differential_pairs : list, optional
+            Differential pairs defined. The default is ``[]``.
 
         Returns
         -------
         list
             List of traces of specified designs ready to use in plot reports.
 
         Examples
         --------
-        >>> from pyaedt import Q3d
-        >>> hfss = hfss(project_path)
+        >>> from pyaedt import Hfss3dLayout
+        >>> hfss = Hfss3dLayout(project_path)
         >>> hfss.get_traces_for_plot(first_element_filter="Bo?1",
-        ...                           second_element_filter="GND*", category="dB(S")
+        ...                          second_element_filter="GND*", category="dB(S")
+        >>> hfss.get_traces_for_plot(differential_pairs=['Diff_U0_data0','Diff_U1_data0','Diff_U1_data1'],
+        ...                          first_element_filter="*_U1_data?",
+        ...                          second_element_filter="*_U0_*", category="dB(S")
         """
         if not first_element_filter:
             first_element_filter = "*"
         if not second_element_filter:
             second_element_filter = "*"
         list_output = []
         end_str = ")" * (category.count("(") + 1)
+        if differential_pairs:
+            excitations = differential_pairs
+        else:
+            excitations = self.excitations
         if get_self_terms:
-            for el in self.excitations:
+            for el in excitations:
                 value = "{}({},{}{}".format(category, el, el, end_str)
                 if filter_tuple(value, first_element_filter, second_element_filter):
                     list_output.append(value)
         if get_mutual_terms:
-            for el1 in self.excitations:
-                for el2 in self.excitations:
+            for el1 in excitations:
+                for el2 in excitations:
                     if el1 != el2:
                         value = "{}({},{}{}".format(category, el1, el2, end_str)
                         if filter_tuple(value, first_element_filter, second_element_filter):
                             list_output.append(value)
         return list_output
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.82/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.85/pyaedt/application/Analysis3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import warnings
 
 from pyaedt import settings
 from pyaedt.application.Analysis import Analysis
 from pyaedt.generic.configurations import Configurations
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class FieldAnalysis3D(Analysis, object):
@@ -365,36 +364,36 @@
             "HFSS": ["HfssTab", "MeshSetupTab"],
             "Icepak": ["Icepak"],
             "Q3D": ["Q3D", "General"],
             "Maxwell3D": ["Maxwell3D", "General"],
         }
         if type == "Boundary":
             propserv = boundary[self._design_type]
-            val = _retry_ntimes(10, self.odesign.GetPropertyValue, propserv, objectname, property)
+            val = self.odesign.GetPropertyValue(propserv, objectname, property)
             return val
         elif type == "Setup":
             propserv = setup[self._design_type]
-            val = _retry_ntimes(10, self.odesign.GetPropertyValue, propserv, objectname, property)
+            val = self.odesign.GetPropertyValue(propserv, objectname, property)
             return val
 
         elif type == "Excitation":
             propserv = excitation[self._design_type]
-            val = _retry_ntimes(10, self.odesign.GetPropertyValue, propserv, objectname, property)
+            val = self.odesign.GetPropertyValue(propserv, objectname, property)
             return val
 
         elif type == "Mesh":
             propserv = mesh[self._design_type]
-            val = _retry_ntimes(10, self.odesign.GetPropertyValue, propserv, objectname, property)
+            val = self.odesign.GetPropertyValue(propserv, objectname, property)
             return val
         else:
             propservs = all[self._design_type]
             for propserv in propservs:
                 properties = list(self.odesign.GetProperties(propserv, objectname))
                 if property in properties:
-                    val = _retry_ntimes(10, self.odesign.GetPropertyValue, propserv, objectname, property)
+                    val = self.odesign.GetPropertyValue(propserv, objectname, property)
                     return val
         return None
 
     @pyaedt_function_handler()
     def copy_solid_bodies_from(self, design, object_list=None, no_vacuum=True, no_pec=True, include_sheets=False):
         """Copy a list of objects and user defined models from one design to the active design.
         If user defined models are selected, the project will be saved automatically.
```

### Comparing `pyaedt-0.6.82/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.85/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.85/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.85/pyaedt/application/AnalysisNexxim.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     @pyaedt_function_handler()
     def push_down(self, component_name):
         """Push-down to the child component and reinitialize the Circuit object.
 
         Parameters
         ----------
-        component_name : str or :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        component_name : str or :class:`pyaedt.modeler.cad.object3d.circuit.CircuitComponent`
             Component to initialize.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
```

### Comparing `pyaedt-0.6.82/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.85/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.85/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/application/Design.py` & `pyaedt-0.6.85/pyaedt/application/Design.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 from pyaedt.desktop import release_desktop
 from pyaedt.generic.DataHandlers import variation_string_to_dict
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import unit_system
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import check_and_download_file
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_project_locked
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
@@ -183,15 +182,15 @@
         self._init_variables()
         self._design_type = design_type
         self.last_run_log = ""
         self.last_run_job = ""
         self._design_dictionary = None
         # Get Desktop from global Desktop Environment
         self._project_dictionary = OrderedDict()
-        self._boundaries = []
+        self._boundaries = {}
         self._project_datasets = {}
         self._design_datasets = {}
         main_module = sys.modules["__main__"]
         self.close_on_exit = close_on_exit
         self._global_logger = pyaedt_logger
         self._logger = pyaedt_logger
         self._desktop_class = None
@@ -293,17 +292,150 @@
     def boundaries(self):
         """Design boundaries and excitations.
 
         Returns
         -------
         List of :class:`pyaedt.modules.Boundary.BoundaryObject`
         """
-        if not self._boundaries:
-            self._boundaries = self._get_boundaries_data()
-        return self._boundaries
+        bb = []
+
+        if "GetBoundaries" in self.oboundary.__dir__():
+            bb = list(self.oboundary.GetBoundaries())
+        elif "Boundaries" in self.get_oo_name(self.odesign):
+            bb = self.get_oo_name(self.odesign, "Boundaries")
+
+        # Parameters and Motion definitions
+        if self.design_type in ["Maxwell 3D", "Maxwell 2D"]:
+            maxwell_parameters = list(self.get_oo_name(self.odesign, "Parameters"))
+            for parameter in maxwell_parameters:
+                bb.append(parameter)
+                bb.append("MaxwellParameters")
+            if "Model" in list(self.get_oo_name(self.odesign)):
+                maxwell_model = list(self.get_oo_name(self.odesign, "Model"))
+                for parameter in maxwell_model:
+                    if self.get_oo_property_value(self.odesign, "Model\\{}".format(parameter), "Type") == "Band":
+                        bb.append(parameter)
+                        bb.append("MotionSetup")
+
+        # Icepak definition
+        elif self.design_type == "Icepak":
+            othermal = self.get_oo_object(self.odesign, "Thermal")
+            thermal_definitions = list(self.get_oo_name(othermal))
+            for thermal in thermal_definitions:
+                bb.append(thermal)
+                bb.append(self.get_oo_property_value(othermal, thermal, "Type"))
+
+            if self.modeler.user_defined_components:
+                for component in self.modeler.user_defined_components:
+                    thermal_properties = self.get_oo_properties(self.oeditor, component)
+                    if thermal_properties and "Type" not in thermal_properties and thermal_properties[-1] != "Icepak":
+                        thermal_boundaries = self.design_properties["BoundarySetup"]["Boundaries"]
+                        for component_boundary in thermal_boundaries:
+                            if component_boundary not in bb and isinstance(
+                                thermal_boundaries[component_boundary], dict
+                            ):
+                                boundarytype = thermal_boundaries[component_boundary]["BoundType"]
+                                bb.append(component_boundary)
+                                bb.append(boundarytype)
+
+        current_boundaries = bb[::2]
+        current_types = bb[1::2]
+
+        for boundary, boundarytype in zip(current_boundaries, current_types):
+            if boundary in self._boundaries:
+                continue
+            if boundarytype == "MaxwellParameters":
+                maxwell_parameter_type = self.get_oo_property_value(
+                    self.odesign, "Parameters\\{}".format(boundary), "Type"
+                )
+
+                self._boundaries[boundary] = MaxwellParameters(self, boundary, boundarytype=maxwell_parameter_type)
+            elif boundarytype == "MotionSetup":
+                maxwell_motion_type = self.get_oo_property_value(self.odesign, "Model\\{}".format(boundary), "Type")
+
+                self._boundaries[boundary] = BoundaryObject(self, boundary, boundarytype=maxwell_motion_type)
+            elif boundarytype == "Network":
+                self._boundaries[boundary] = NetworkObject(self, boundary)
+            else:
+                self._boundaries[boundary] = BoundaryObject(self, boundary, boundarytype=boundarytype)
+
+        return list(self._boundaries.values()) + self.design_excitations
+
+    @property
+    def boundaries_by_type(self):
+        """Design boundaries by type.
+
+        Returns
+        -------
+        Dictionary of boundaries.
+        """
+        _dict_out = {}
+        for bound in self.boundaries:
+            if bound.type in _dict_out:
+                _dict_out[bound.type].append(bound)
+            else:
+                _dict_out[bound.type] = [bound]
+        return _dict_out
+
+    @property
+    def excitations_by_type(self):
+        """Design excitations by tupe.
+
+        Returns
+        -------
+        dict
+            Dictionary of excitations.
+        """
+        _dict_out = {}
+        for bound in self._excitations:
+            if bound.type in _dict_out:
+                _dict_out[bound.type].append(bound)
+            else:
+                _dict_out[bound.type] = [bound]
+        return _dict_out
+
+    @property
+    def design_excitations(self):
+        """Design excitations.
+
+        Returns
+        -------
+        list
+            List of :class:`pyaedt.modules.Boundary.BoundaryObject`.
+        """
+        design_excitations = {}
+
+        if "GetExcitations" in self.oboundary.__dir__():
+            ee = list(self.oboundary.GetExcitations())
+            current_boundaries = [i.split(":")[0] for i in ee[::2]]
+            current_types = ee[1::2]
+            for i in set(current_types):
+                new_port = []
+                if "GetExcitationsOfType" in self.oboundary.__dir__():
+                    new_port = list(self.oboundary.GetExcitationsOfType(i))
+                if new_port:
+                    current_boundaries = current_boundaries + new_port
+                    current_types = current_types + [i] * len(new_port)
+            for boundary, boundarytype in zip(current_boundaries, current_types):
+                if boundary in self._boundaries:
+                    continue
+                design_excitations[boundary] = BoundaryObject(self, boundary, boundarytype=boundarytype)
+
+        elif "GetAllPortsList" in self.oboundary.__dir__() and self.design_type in ["HFSS 3D Layout Design"]:
+            for port in self.oboundary.GetAllPortsList():
+                if port in self._boundaries:
+                    continue
+                bound = self._update_port_info(port)
+                if bound:
+                    design_excitations[port] = bound
+
+        if design_excitations:
+            return list(design_excitations.values())
+
+        return []
 
     @property
     def odesktop(self):
         """AEDT instance containing all projects and designs.
 
         Examples
         --------
@@ -2073,14 +2205,30 @@
             for port in self.oboundary.GetAllPortsList():
                 bound = self._update_port_info(port)
                 if bound:
                     boundaries.append(bound)
         return boundaries
 
     @pyaedt_function_handler()
+    def _get_boundaries_object(self):
+        """Retrieve boundary objects.
+
+        Returns
+        -------
+        list
+            Boundary objects.
+        """
+        boundaries = []
+        boundaries_names = list(self.get_oo_name(self.odesign, "Boundaries"))
+        if boundaries_names:
+            boundaries = self.get_oo_object(self.odesign, "Boundaries")
+
+        return boundaries
+
+    @pyaedt_function_handler()
     def _get_ds_data(self, name, datas):
         """
 
         Parameters
         ----------
         name :
 
@@ -3082,15 +3230,15 @@
             if design_type == "HFSS" and self._aedt_version < "2021.2":
                 new_design = self._oproject.InsertDesign(design_type, unique_design_name, "DrivenModal", "")
             else:
                 new_design = self._oproject.InsertDesign(
                     design_type, unique_design_name, self.default_solution_type, ""
                 )
         self.logger.info("Added design '%s' of type %s.", unique_design_name, design_type)
-        name = _retry_ntimes(10, new_design.GetName)
+        name = new_design.GetName()
         self._odesign = new_design
         return name
 
     @pyaedt_function_handler()
     def _generate_unique_design_name(self, design_name):
         """Generate an unique design name.
 
@@ -3153,15 +3301,15 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oDesign.RenameDesignInstance
         """
-        _retry_ntimes(10, self._odesign.RenameDesignInstance, self.design_name, new_name)
+        self._odesign.RenameDesignInstance(self.design_name, new_name)
         if save_after_duplicate:
             self.oproject.Save()
             self._project_dictionary = None
         return True
 
     @pyaedt_function_handler()
     def copy_design_from(self, project_fullname, design_name, save_project=True, set_active_design=True):
@@ -3249,16 +3397,16 @@
 
         >>> oProject.CopyDesign
         >>> oProject.Paste
         """
 
         active_design = self.design_name
         design_list = self.design_list
-        _retry_ntimes(10, self._oproject.CopyDesign, active_design)
-        _retry_ntimes(10, self._oproject.Paste)
+        self._oproject.CopyDesign(active_design)
+        self._oproject.Paste()
         newname = label
         ind = 1
         while newname in self.design_list:
             newname = label + "_" + str(ind)
             ind += 1
         actual_name = [i for i in self.design_list if i not in design_list]
         self.odesign = actual_name[0]
@@ -3553,15 +3701,15 @@
                 if variable_name in self.get_oo_name(app, "Instance:{}".format(self._odesign.GetName())):
                     var_obj = self.get_oo_object(app, "Instance:{}/{}".format(self._odesign.GetName(), variable_name))
                 elif variable_name in self.get_oo_object(app, "DefinitionParameters").GetPropNames():
                     val = self.get_oo_object(app, "DefinitionParameters").GetPropEvaluatedValue(variable_name)
             else:
                 var_obj = self.get_oo_object(app, "Variables/{}".format(variable_name))
         if var_obj:
-            val = _retry_ntimes(10, var_obj.GetPropValue, "SIValue")
+            val = var_obj.GetPropValue("SIValue")
         elif not val:
             try:
                 variation_string = self._odesign.GetNominalVariation()
                 val = self._odesign.GetVariationVariableValue(variation_string, variable_name)  # pragma: no cover
             except:
                 val_units = app.GetVariableValue(variable_name)
                 val, original_units = decompose_variable_value(val_units)
```

### Comparing `pyaedt-0.6.82/pyaedt/application/JobManager.py` & `pyaedt-0.6.85/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/application/Variables.py` & `pyaedt-0.6.85/pyaedt/application/Variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 # from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SI_UNITS
 from pyaedt.generic.constants import _resolve_unit_system
 from pyaedt.generic.constants import unit_system
+from pyaedt.generic.general_methods import GrpcApiError
 from pyaedt.generic.general_methods import is_array
 from pyaedt.generic.general_methods import is_number
 from pyaedt.generic.general_methods import open_file
 
 
 class CSVDataset:
     """Reads in a CSV file and extracts data, which can be augmented with constant values.
@@ -1604,15 +1605,15 @@
     @property
     def units(self):
         """Units."""
         try:
             var_obj = self._aedt_obj.GetChildObject("Variables").GetChildObject(self._variable_name)
             _, self._units = decompose_variable_value(var_obj.GetPropEvaluatedValue("EvaluatedValue"))
             return self._units
-        except (TypeError, AttributeError):
+        except (TypeError, AttributeError, GrpcApiError):
             pass
         return self._units
 
     @property
     def value(self):
         """Value."""
```

### Comparing `pyaedt-0.6.82/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.85/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/application/design_solutions.py` & `pyaedt-0.6.85/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/circuit.py` & `pyaedt-0.6.85/pyaedt/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 """This module contains the ``Circuit`` class."""
 
 from __future__ import absolute_import  # noreorder
 
-import glob
 import io
 import math
 import os
 import re
 import shutil
 
 from pyaedt import Hfss3dLayout
 from pyaedt.application.AnalysisNexxim import FieldAnalysisCircuit
 from pyaedt.generic import ibis_reader
 from pyaedt.generic.DataHandlers import from_rkm_to_aedt
+from pyaedt.generic.filesystem import search_files
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Boundary import CurrentSinSource
 from pyaedt.modules.Boundary import PowerIQSource
 from pyaedt.modules.Boundary import PowerSinSource
 from pyaedt.modules.Boundary import Sources
@@ -1533,21 +1533,21 @@
             if not os.path.exists(filepath):
                 os.mkdir(filepath)
 
         results_path = os.path.join(os.path.normpath(self.results_directory), self.design_name)
         results_temp_path = os.path.join(results_path, "temp")
 
         # Check if .log exist in temp folder
-        if os.path.exists(results_temp_path) and glob.glob(os.path.join(results_temp_path, "*.log")):
+        if os.path.exists(results_temp_path) and search_files(results_temp_path, "*.log"):
             # Check the most recent
-            files = glob.glob(os.path.join(results_temp_path, "*.log"))
+            files = search_files(results_temp_path, "*.log")
             latest_file = max(files, key=os.path.getctime)
-        elif os.path.exists(results_path) and glob.glob(os.path.join(results_path, "*.log")):
+        elif os.path.exists(results_path) and search_files(results_path, "*.log"):
             # Check the most recent
-            files = glob.glob(os.path.join(results_path, "*.log"))
+            files = search_files(results_path, "*.log")
             latest_file = max(files, key=os.path.getctime)
         else:
             self.logger.error("Design not solved")
             return None
 
         shutil.copy(latest_file, filepath)
         filename = os.path.basename(latest_file)
```

### Comparing `pyaedt-0.6.82/pyaedt/common_rpc.py` & `pyaedt-0.6.85/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/desktop.py` & `pyaedt-0.6.85/pyaedt/generic/general_methods.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1787 +1,2261 @@
-"""
-This module contains the ``Desktop`` class.
-This module is used to initialize AEDT and the message manager for managing AEDT.
-You can initialize this module before launching an app or
-have the app automatically initialize it to the latest installed AEDT version.
-"""
-
-from __future__ import absolute_import  # noreorder
+# -*- coding: utf-8 -*-
+from __future__ import absolute_import
 
+import ast
+import codecs
+from collections import OrderedDict
+import csv
 import datetime
-import gc
+import difflib
+import fnmatch
+from functools import update_wrapper
+import inspect
+import itertools
+import json
 import logging
+import math
 import os
-import pkgutil
+import random
 import re
-import shutil
-import socket
+import string
 import sys
 import tempfile
-import threading
 import time
 import traceback
-import warnings
 
-from pyaedt import is_ironpython
-from pyaedt import is_linux
-from pyaedt import is_windows
-from pyaedt import pyaedt_logger
-
-if is_linux:
-    os.environ["ANS_NODEPCHECK"] = str(1)
-
-if is_linux and is_ironpython:
-    import subprocessdotnet as subprocess
-else:
-    import subprocess
-
-# from pyaedt import property
-from pyaedt import __version__
-from pyaedt import pyaedt_function_handler
-from pyaedt import settings
-from pyaedt.generic.general_methods import _pythonver
-from pyaedt.generic.general_methods import active_sessions
-from pyaedt.generic.general_methods import com_active_sessions
-from pyaedt.generic.general_methods import grpc_active_sessions
-from pyaedt.generic.general_methods import inside_desktop
-from pyaedt.generic.general_methods import is_ironpython
-from pyaedt.generic.general_methods import open_file
-from pyaedt.misc import list_installed_ansysem
-
-pathname = os.path.dirname(__file__)
-
-pyaedtversion = __version__
-
-modules = [tup[1] for tup in pkgutil.iter_modules()]
-
-if is_ironpython:
-    _com = "ironpython"
-elif is_windows and "pythonnet" in modules:
-    _com = "pythonnet_v3"
-else:
-    _com = "gprc_v3"
-    settings.use_grpc_api = True
+from pyaedt.generic.constants import CSS4_COLORS
 
+is_ironpython = "IronPython" in sys.version or ".NETFramework" in sys.version
+is_linux = os.name == "posix"
+is_windows = not is_linux
+_pythonver = sys.version_info[0]
+inside_desktop = True if is_ironpython and "4.0.30319.42000" in sys.version else False
 
-@pyaedt_function_handler()
-def launch_aedt(full_path, non_graphical, port, first_run=True):
-    """Launch AEDT in gRPC mode."""
-
-    def launch_desktop_on_port():
-        command = [full_path, "-grpcsrv", str(port)]
-        if non_graphical:
-            command.append("-ng")
-        my_env = os.environ.copy()
-        for env, val in settings.aedt_environment_variables.items():
-            my_env[env] = val
-        if is_linux:  # pragma: no cover
-            with subprocess.Popen(command, env=my_env, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL) as p:
-                p.wait()
-        else:
-            with subprocess.Popen(
-                " ".join(command), env=my_env, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
-            ) as p:
-                p.wait()
-
-    _aedt_process_thread = threading.Thread(target=launch_desktop_on_port)
-    _aedt_process_thread.daemon = True
-    _aedt_process_thread.start()
-    timeout = settings.desktop_launch_timeout
-    k = 0
-    while not _check_grpc_port(port):
-        if k > timeout:  # pragma: no cover
-            active_s = active_sessions(student_version=settings.is_student)
-            for p in active_s:
-                if port == p[1]:
-                    try:
-                        os.kill(p[0], 9)
-                    except (OSError, PermissionError):
-                        pass
-            if first_run:
-                port = _find_free_port()
-                return launch_aedt(full_path, non_graphical, port, first_run=False)
-            return False, _find_free_port()
-        time.sleep(1)
-        k += 1
-    return True, port
-
-
-def launch_aedt_in_lsf(non_graphical, port):  # pragma: no cover
-    """Launch AEDT in LSF in GRPC mode."""
-    if settings.lsf_queue:
-        command = [
-            "bsub",
-            "-n",
-            str(settings.lsf_num_cores),
-            "-R",
-            '"rusage[mem={}]"'.format(settings.lsf_ram),
-            "-queue {}".format(settings.lsf_queue),
-            "-Is",
-            settings.lsf_aedt_command,
-            "-grpcsrv",
-            str(port),
-        ]
-    else:
-        command = [
-            "bsub",
-            "-n",
-            str(settings.lsf_num_cores),
-            "-R",
-            '"rusage[mem={}]"'.format(settings.lsf_ram),
-            "-Is",
-            settings.lsf_aedt_command,
-            "-grpcsrv",
-            str(port),
-        ]
-    if non_graphical:
-        command.append("-ng")
-    print(command)
-    p = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-    timeout = settings.lsf_timeout
-    i = 0
-    while i < timeout:
-        err = p.stderr.readline().strip().decode("utf-8", "replace")
-        m = re.search(r"<<Starting on (.+?)>>", err)
-        if m:
-            aedt_startup_timeout = 120
-            k = 0
-            while not _check_grpc_port(port, machine_name=m.group(1)):
-                if k > aedt_startup_timeout:
-                    return False, err
-                time.sleep(1)
-                k += 1
-            return True, m.group(1)
-        i += 1
-        time.sleep(1)
-    return False, err
+if not is_ironpython:
+    import psutil
 
+try:
+    import xml.etree.cElementTree as ET
+
+    ET.VERSION
+except ImportError:
+    ET = None
 
-def _check_grpc_port(port, machine_name=""):
-    s = socket.socket()
-    try:
-        if not machine_name:
-            machine_name = "127.0.0.1"
-        s.connect((machine_name, port))
-    except socket.error:
-        success = False
-    else:
-        success = True
-    finally:
-        s.close()
-    return success
 
+class GrpcApiError(Exception):
+    """ """
 
-def _find_free_port():
-    from contextlib import closing
+    pass
 
-    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
-        s.bind(("127.0.0.1", 0))
-        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        return s.getsockname()[1]
 
+class MethodNotSupportedError(Exception):
+    """ """
 
-def exception_to_desktop(ex_value, tb_data):  # pragma: no cover
-    """Writes the trace stack to AEDT when a Python error occurs.
+    pass
 
-    The message is added to the AEDT global logger and to the log file (if present).
+
+def _write_mes(mes_text):
+    mes_text = str(mes_text)
+    parts = [mes_text[i : i + 250] for i in range(0, len(mes_text), 250)]
+    for el in parts:
+        settings.logger.error(el)
+
+
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
+def _exception(ex_info, func, args, kwargs, message="Type Error"):
+    """Write the trace stack to the desktop when a Python error occurs.
 
     Parameters
     ----------
-    ex_value : str
-        Type of the exception.
-    tb_data : str
-        Traceback data.
+    ex_info :
 
-    """
-    tb_trace = traceback.format_tb(tb_data)
-    tblist = tb_trace[0].split("\n")
-    pyaedt_logger.error(str(ex_value))
-    for el in tblist:
-        pyaedt_logger.error(el)
+    func :
 
+    args :
 
-def _delete_objects():
-    settings._non_graphical = False
-    settings._aedt_version = None
-    settings.remote_api = False
-    settings._use_grpc_api = None
-    settings.machine = ""
-    settings.port = 0
-    module = sys.modules["__main__"]
-    try:
-        del module.COMUtil
-    except AttributeError:
-        pass
-    pyaedt_logger.remove_all_project_file_logger()
-    try:
-        del module.oDesktop
-    except AttributeError:
-        pass
-    try:
-        del module.pyaedt_initialized
-    except AttributeError:
-        pass
-    try:
-        del module.oAnsoftApplication
-    except AttributeError:
-        pass
-    try:
-        del module.desktop
-    except AttributeError:
-        pass
-    try:
-        del module.sDesktopinstallDirectory
-    except AttributeError:
-        pass
-    try:
-        del module.isoutsideDesktop
-    except AttributeError:
-        pass
-    try:
-        del module.AEDTVersion
-    except AttributeError:
-        pass
+    kwargs :
+
+    message :
+         (Default value = "Type Error")
+
+    Returns
+    -------
+
+    """
+
+    tb_data = ex_info[2]
+    tb_trace = traceback.format_tb(tb_data)
+    _write_mes("{} on {}".format(message.upper(), func.__name__))
     try:
-        del sys.modules["PyDesktopPluginDll"]
-    except:
+        _write_mes(ex_info[1].args[0])
+    except (IndexError, AttributeError):
         pass
+    for trace in traceback.format_stack():
+        if func.__name__ in trace:
+            for el in trace.split("\n"):
+                _write_mes(el)
+    for trace in tb_trace:
+        tblist = trace.split("\n")
+        for el in tblist:
+            if func.__name__ in el:
+                _write_mes(el)
+
+    message_to_print = ""
+    messages = ""
     try:
-        del sys.modules["PyDesktopPlugin"]
-    except:
+        messages = list(sys.modules["__main__"].oDesktop.GetMessages("", "", 2))[-1].lower()
+    except (GrpcApiError, AttributeError, TypeError, IndexError):
         pass
+    if "error" in messages:
+        message_to_print = messages[messages.index("[error]") :]
+    # _write_mes("{} - {} -  {}.".format(ex_info[1], func.__name__, message.upper()))
+
+    if message_to_print:
+        _write_mes("Last Electronics Desktop Message - " + message_to_print)
+
+    args_name = []
     try:
-        del sys.modules["ScriptEnv"]
+        args_dict = _get_args_dicts(func, args, kwargs)
+        first_time_log = True
+
+        for el in args_dict:
+            if el != "self" and args_dict[el]:
+                if first_time_log:
+                    _write_mes("Method arguments: ")
+                    first_time_log = False
+                _write_mes("    {} = {} ".format(el, args_dict[el]))
     except:
         pass
-    keys = [k for k in sys.modules.keys()]
-    for i in keys:
-        if "Ansys.Ansoft" in i:
-            del sys.modules[i]
-    for p in sys.path[::-1]:
-        if "AnsysEM" in p:
-            del sys.path[sys.path.index(p)]
-    gc.collect()
+    args = [func.__name__] + [i for i in args_name if i not in ["self"]]
+    if not func.__name__.startswith("_"):
+        _write_mes(
+            "Check Online documentation on: https://aedt.docs.pyansys.com/version/stable/search.html?q={}".format(
+                "+".join(args)
+            )
+        )
 
 
-@pyaedt_function_handler()
-def release_desktop(close_projects=True, close_desktop=True):
-    """Release the AEDT API.
+def normalize_path(path_in, sep=None):
+    """Normalize path separators.
 
     Parameters
     ----------
-    close_projects : bool, optional
-        Whether to close the AEDT projects open in the session. The default is ``True``.
-    close_desktop : bool, optional
-        Whether to close the active AEDT session. The default is ``True``.
+    path_in : str
+        Path to normalize.
+    sep : str, optional
+        Separator.
 
     Returns
     -------
-    bool
-        ``True`` when successful, ``False`` when failed.
+    str
+        Path normalized to new separator.
+    """
+    if sep is None:
+        sep = os.sep
+    return path_in.replace("\\", sep).replace("/", sep)
+
+
+def _check_types(arg):
+    if "netref.builtins.list" in str(type(arg)):
+        return "list"
+    elif "netref.builtins.dict" in str(type(arg)):
+        return "dict"
+    elif "netref.__builtin__.list" in str(type(arg)):
+        return "list"
+    elif "netref.__builtin__.dict" in str(type(arg)):
+        return "dict"
+    return ""
+
+
+def _function_handler_wrapper(user_function):
+    def wrapper(*args, **kwargs):
+        if not settings.enable_error_handler:
+            result = user_function(*args, **kwargs)
+            return result
+        else:
+            try:
+                settings.time_tick = time.time()
+                out = user_function(*args, **kwargs)
+                if settings.enable_debug_logger or settings.enable_debug_edb_logger:
+                    _log_method(user_function, args, kwargs)
+                return out
+            except TypeError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "Type Error")
+                return False
+            except ValueError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "Value Error")
+                return False
+            except AttributeError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "Attribute Error")
+                return False
+            except KeyError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "Key Error")
+                return False
+            except IndexError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "Index Error")
+                return False
+            except AssertionError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "Assertion Error")
+                return False
+            except NameError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "Name Error")
+                return False
+            except IOError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "IO Error")
+                return False
+            except MethodNotSupportedError:
+                message = "This Method is not supported in current AEDT Design Type."
+                if settings.enable_screen_logs:
+                    print("**************************************************************")
+                    print("pyaedt error on Method {}:  {}. Please Check again".format(user_function.__name__, message))
+                    print("**************************************************************")
+                    print("")
+                if settings.enable_file_logs:
+                    settings.logger.error(message)
+                return False
+            except GrpcApiError:
+                _exception(sys.exc_info(), user_function, args, kwargs, "AEDT grpc API call Error")
+                return False
+            except BaseException:
+                _exception(sys.exc_info(), user_function, args, kwargs, "General or AEDT Error")
+                return False
+
+    return wrapper
+
+
+def pyaedt_function_handler(direct_func=None):
+    """Provides an exception handler, logging mechanism, and argument converter for client-server
+    communications.
+
+    This method returns the function itself if correctly executed. Otherwise, it returns ``False``
+    and displays errors.
 
     """
+    if callable(direct_func):
+        user_function = direct_func
+        wrapper = _function_handler_wrapper(user_function)
+        return update_wrapper(wrapper, user_function)
+    elif direct_func is not None:
+        raise TypeError("Expected first argument to be a callable, or None")
+
+    def decorating_function(user_function):
+        wrapper = _function_handler_wrapper(user_function)
+        return update_wrapper(wrapper, user_function)
 
-    _main = sys.modules["__main__"]
-    try:
-        desktop = _main.oDesktop
-        if close_projects:
-            projects = desktop.GetProjectList()
-            for project in projects:
-                desktop.CloseProject(project)
-        pid = _main.oDesktop.GetProcessID()
-        if settings.remote_rpc_session or (
-            settings.aedt_version >= "2022.2" and settings.use_grpc_api and not is_ironpython
-        ):
-            try:
-                import ScriptEnv
+    return decorating_function
 
-                if close_desktop:
-                    ScriptEnv.Shutdown()
-                else:
-                    ScriptEnv.Release()
-            except:
-                pass
-            _delete_objects()
-            return True
-        elif not inside_desktop:
-            i = 0
-            scopeID = 5
-            while i <= scopeID:
-                _main.COMUtil.ReleaseCOMObjectScope(_main.COMUtil.PInvokeProxyAPI, i)
-                i += 1
-        if close_desktop:
-            try:
-                os.kill(pid, 9)
-                _delete_objects()
-                return True
-            except Exception:  # pragma: no cover
-                warnings.warn("Something went wrong in closing AEDT.")
-                return False
-        _delete_objects()
-        return True
-    except AttributeError:
-        _delete_objects()
-        return False
 
+@pyaedt_function_handler()
+def check_numeric_equivalence(a, b, relative_tolerance=1e-7):
+    """Check if two numeric values are equivalent to within a relative tolerance.
 
-def force_close_desktop():
-    """Forcibly close all AEDT projects and shut down AEDT.
+    Paraemters
+    ----------
+    a : int, float
+        Reference value to compare to.
+    b : int, float
+        Secondary value for the comparison.
+    relative_tolerance : float, optional
+        Relative tolerance for the equivalence test. The difference is relative to the first value.
+        The default is ``1E-7``.
 
     Returns
     -------
     bool
-        ``True`` when successful, ``False`` when failed.
+        ``True`` if the two passed values are equivalent.
     """
-    Module = sys.modules["__main__"]
-    pid = Module.oDesktop.GetProcessID()
-    logger = logging.getLogger(__name__)
+    if abs(a) > 0.0:
+        reldiff = abs(a - b) / a
+    else:
+        reldiff = abs(b)
+    return True if reldiff < relative_tolerance else False
 
-    if pid > 0:
-        try:
-            projects = Module.oDesktop.GetProjectList()
-            for project in projects:
-                Module.oDesktop.CloseProject(project)
-        except:
-            logger.warning("No projects are open. Closing the AEDT connection.")
-        try:
-            i = 0
-            scopeID = 5
-            while i <= scopeID:
-                Module.COMUtil.ReleaseCOMObjectScope(Module.COMUtil.PInvokeProxyAPI, 0)
-                i += 1
-        except:
-            logger.warning("No COM UTIL. Closing AEDT....")
-        try:
-            del Module.pyaedt_initialized
-        except:
-            pass
-        try:
-            os.kill(pid, 9)
-            del Module.oDesktop
-            successfully_closed = True
-        except:
-            pyaedt_logger.error("Something went wrong in closing AEDT.")
-            successfully_closed = False
-        finally:
-            log = logging.getLogger("Global")
-            handlers = log.handlers[:]
-            for handler in handlers:
-                handler.close()
-                log.removeHandler(handler)
-            return successfully_closed
 
+@pyaedt_function_handler()
+def check_and_download_file(local_path, remote_path, overwrite=True):
+    """Check if a file is remote and either download it or return the path.
 
-def run_process(command, bufsize=None):
-    """Run a process with a subprocess.
+    Parameters
+    ----------
+    local_path : str
+        Local path to save the file to.
+    remote_path : str
+        Path to the remote file.
+    overwrite : bool
+        Whether to overwrite the file if it already exits locally.
+        The default is ``True``.
+
+    Returns
+    -------
+    str
+    """
+    if settings.remote_rpc_session:
+        remote_path = remote_path.replace("\\", "/") if remote_path[0] != "\\" else remote_path
+        settings.remote_rpc_session.filemanager.download_file(remote_path, local_path, overwrite=overwrite)
+        return local_path
+    return remote_path
+
+
+def check_if_path_exists(path):
+    """Check whether a path exists or not local or remote machine (for remote sessions only).
 
     Parameters
     ----------
-    command : str
-        Command to execute.
-    bufsize : int, optional
-        Buffer size. The default is ``None``.
+    path : str
+        Local or remote path to check.
 
+    Returns
+    -------
+    bool
     """
-    if bufsize:
-        return subprocess.call(command, bufsize=bufsize)
-    else:
-        return subprocess.call(command)
+    if settings.remote_rpc_session:
+        return settings.remote_rpc_session.filemanager.pathexists(path)
+    return os.path.exists(path)
 
 
-def get_version_env_variable(version_id):
-    """Get the environment variable for the AEDT version.
+@pyaedt_function_handler()
+def check_and_download_folder(local_path, remote_path, overwrite=True):
+    """Check if a folder is remote and either download it or return the path.
 
     Parameters
     ----------
-    version_id : str
-        Full AEDT version number. For example, ``"2021.2"``.
+    local_path : str
+        Local path to save the folder to.
+    remote_path : str
+        Path to the remote folder.
+    overwrite : bool
+        Whether to overwrite the folder if it already exits locally.
+        The default is ``True``.
 
     Returns
     -------
     str
-        Environment variable for the version.
+    """
+    if settings.remote_rpc_session:
+        remote_path = remote_path.replace("\\", "/") if remote_path[0] != "\\" else remote_path
+        settings.remote_rpc_session.filemanager.download_folder(remote_path, local_path, overwrite=overwrite)
+        return local_path
+    return remote_path
 
-    Examples
-    --------
-    >>> from pyaedt import desktop
-    >>> desktop.get_version_env_variable("2021.2")
-    'ANSYSEM_ROOT212'
 
+def open_file(file_path, file_options="r"):
+    """Open a file and return the object.
+
+    Parameters
+    ----------
+    file_path : str
+        Full absolute path to the file (either local or remote).
+    file_options : str, optional
+        Options for opening the file.
+
+    Returns
+    -------
+    object
+        Opened file.
     """
-    version_env_var = "ANSYSEM_ROOT"
-    values = version_id.split(".")
-    version = int(values[0][2:])
-    release = int(values[1])
+    file_path = file_path.replace("\\", "/") if file_path[0] != "\\" else file_path
+    dir_name = os.path.dirname(file_path)
+    if "r" in file_options:
+        if os.path.exists(file_path):
+            return open(file_path, file_options)
+        elif settings.remote_rpc_session and settings.remote_rpc_session.filemanager.pathexists(
+            file_path
+        ):  # pragma: no cover
+            local_file = os.path.join(tempfile.gettempdir(), os.path.split(file_path)[-1])
+            settings.remote_rpc_session.filemanager.download_file(file_path, local_file)
+            return open(local_file, file_options)
+    elif os.path.exists(dir_name):
+        return open(file_path, file_options)
+    else:
+        settings.logger.error("The file or folder %s does not exist", dir_name)
+
+
+def _log_method(func, new_args, new_kwargs):
+    if not settings.enable_debug_internal_methods_logger and str(func.__name__)[0] == "_":
+        return
+    if not settings.enable_debug_geometry_operator_logger and "GeometryOperators" in str(func):
+        return
+    if (
+        not settings.enable_debug_edb_logger
+        and "Edb" in str(func) + str(new_args)
+        or "edb_core" in str(func) + str(new_args)
+    ):
+        return
+    line_begin = "ARGUMENTS: "
+    message = []
+    delta = time.time() - settings.time_tick
+    m, s = divmod(delta, 60)
+    h, m = divmod(m, 60)
+    d, h = divmod(h, 24)
+    msec = (s - int(s)) * 1000
+    if d > 0:
+        time_msg = " {}days {}h {}m {}sec.".format(d, h, m, int(s))
+    elif h > 0:
+        time_msg = " {}h {}m {}sec.".format(h, m, int(s))
+    else:
+        time_msg = "  {}m {}sec {}msec.".format(m, int(s), int(msec))
+    if settings.enable_debug_methods_argument_logger:
+        args_dict = _get_args_dicts(func, new_args, new_kwargs)
+        id = 0
+        if new_args:
+            object_name = str([new_args[0]])[1:-1]
+            id = object_name.find(" object at ")
+        if id > 0:
+            object_name = object_name[1:id]
+            message.append("'{}' was run in {}".format(object_name + "." + str(func.__name__), time_msg))
+        else:
+            message.append("'{}' was run in {}".format(str(func.__name__), time_msg))
+        message.append(line_begin)
+        for k, v in args_dict.items():
+            if k != "self":
+                message.append("    {} = {}".format(k, v))
+    for m in message:
+        settings.logger.debug(m)
+
+
+@pyaedt_function_handler()
+def get_version_and_release(input_version):
+    version = int(input_version[2:4])
+    release = int(input_version[5])
     if version < 20:
         if release < 3:
-            version += 1
+            version -= 1
         else:
-            release += 2
-    version_env_var += str(version) + str(release)
-    return version_env_var
+            release -= 2
+    return (version, release)
 
 
-def is_student_version(oDesktop):
-    edt_root = os.path.normpath(oDesktop.GetExeDir())
-    if is_windows and os.path.isdir(edt_root):
-        if any("ansysedtsv" in fn.lower() for fn in os.listdir(edt_root)):
-            return True
-    return False
+@pyaedt_function_handler()
+def env_path(input_version):
+    """Get the path of the version environment variable for an AEDT version.
 
+    Parameters
+    ----------
+    input_version : str
+        AEDT version.
 
-class Desktop(object):
-    """Provides the Ansys Electronics Desktop (AEDT) interface.
+    Returns
+    -------
+    str
+        Path for the version environment variable.
+
+    Examples
+    --------
+    >>> env_path_student("2021.2")
+    "C:/Program Files/ANSYSEM/ANSYSEM2021.2/Win64"
+    """
+    return os.getenv(
+        "ANSYSEM_ROOT{0}{1}".format(
+            get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
+        ),
+        "",
+    )
+
+
+@pyaedt_function_handler()
+def env_value(input_version):
+    """Get the name of the version environment variable for an AEDT version.
 
     Parameters
     ----------
-    specified_version : str, optional
-        Version of AEDT to use. The default is ``None``, in which case the
-        active setup or latest installed version is used.
-    non_graphical : bool, optional
-        Whether to launch AEDT in non-graphical mode. The default
-        is ``False``, in which case AEDT is launched in graphical mode.
-        This parameter is ignored when a script is launched within AEDT.
-    new_desktop_session : bool, optional
-        Whether to launch an instance of AEDT in a new thread, even if
-        another instance of the ``specified_version`` is active on the machine.
-        The default is ``True``.
-    close_on_exit : bool, optional
-        Whether to close AEDT on exit. The default is ``True``.
-    student_version : bool, optional
-        Whether to open the AEDT student version. The default is
-        ``False``.
-    machine : str, optional
-        Machine name to connect the oDesktop session to. This parameters works only in 2022 R2
-        and later. The remote server must be up and running with the command
-        `"ansysedt.exe -grpcsrv portnum"`. If the machine is `"localhost"`, the server also
-        starts if not present.
-    port : int, optional
-        Port number on which to start the oDesktop communication on the already existing server.
-        This parameter is ignored when creating a new server. It works only in 2022 R2 and
-        later. The remote server must be up and running with the command `"ansysedt.exe -grpcsrv portnum"`.
-    aedt_process_id : int, optional
-        Process ID for the instance of AEDT to point PyAEDT at. The default is
-        ``None``. This parameter is only used when ``new_desktop_session = False``.
+    input_version : str
+        AEDT version.
+
+    Returns
+    -------
+    str
+        Name for the version environment variable.
 
     Examples
     --------
-    Launch AEDT 2021 R1 in non-graphical mode and initialize HFSS.
+    >>> env_value("2021.2")
+    "ANSYSEM_ROOT211"
+    """
+    return "ANSYSEM_ROOT{0}{1}".format(
+        get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
+    )
 
-    >>> import pyaedt
-    >>> desktop = pyaedt.Desktop("2021.2", non_graphical=True)
-    PyAEDT INFO: pyaedt v...
-    PyAEDT INFO: Python version ...
-    >>> hfss = pyaedt.Hfss(designname="HFSSDesign1")
-    PyAEDT INFO: Project...
-    PyAEDT INFO: Added design 'HFSSDesign1' of type HFSS.
-
-    Launch AEDT 2021 R1 in graphical mode and initialize HFSS.
-
-    >>> desktop = Desktop("2021.2")
-    PyAEDT INFO: pyaedt v...
-    PyAEDT INFO: Python version ...
-    >>> hfss = pyaedt.Hfss(designname="HFSSDesign1")
-    PyAEDT INFO: No project is defined. Project...
-    """
-
-    def __init__(
-        self,
-        specified_version=None,
-        non_graphical=False,
-        new_desktop_session=True,
-        close_on_exit=True,
-        student_version=False,
-        machine="",
-        port=0,
-        aedt_process_id=None,
-    ):
-        """Initialize desktop."""
-        if os.getenv("PYAEDT_NON_GRAPHICAL", "False").lower() in ("true", "1", "t"):
-            non_graphical = os.getenv("PYAEDT_NON_GRAPHICAL", "False").lower() in ("true", "1", "t")
-
-        self._main = sys.modules["__main__"]
-        self._main.interpreter = _com
-        self.release_on_exit = close_on_exit
-        self.close_on_exit = close_on_exit
-        self._main.pyaedt_version = pyaedtversion
-        self._main.interpreter_ver = _pythonver
-        self._main.student_version = student_version
-        self.machine = machine
-        self.port = port
-        self.aedt_process_id = aedt_process_id
-        if is_ironpython:
-            self._main.isoutsideDesktop = False
-        else:
-            self._main.isoutsideDesktop = True
-        self.release_on_exit = True
-        self.logfile = None
-
-        self._logger = pyaedt_logger
-        if settings.enable_screen_logs:
-            self._logger.enable_stdout_log()
-        else:
-            self._logger.disable_stdout_log()
-        self._logger.info("using existing logger.")
 
-        if "oDesktop" in dir():  # pragma: no cover
-            self.release_on_exit = False
-            self._main.oDesktop = oDesktop
-            try:
-                settings.non_graphical = oDesktop.GetIsNonGraphical()
-            except:
-                settings.non_graphical = non_graphical
-            settings.aedt_version = self._main.oDesktop.GetVersion()[0:6]
-            settings.is_student = is_student_version(self._main.oDesktop)
-        elif "oDesktop" in dir(self._main) and self._main.oDesktop is not None:  # pragma: no cover
-            self.release_on_exit = False
-            try:
-                settings.non_graphical = self._main.oDesktop.GetIsNonGraphical()
-            except:
-                settings.non_graphical = non_graphical
-            settings.aedt_version = self._main.oDesktop.GetVersion()[0:6]
-            settings.is_student = is_student_version(self._main.oDesktop)
-        else:
-            settings.non_graphical = non_graphical
+@pyaedt_function_handler()
+def env_path_student(input_version):
+    """Get the path of the version environment variable for an AEDT student version.
 
-            if "oDesktop" in dir(self._main):
-                del self._main.oDesktop
-            self._main.student_version, version_key, version = self._set_version(specified_version, student_version)
-            settings.aedt_version = version_key
-            settings.is_student = self._main.student_version
-            if not new_desktop_session and not is_ironpython:  # pragma: no cover
-                sessions = active_sessions(
-                    version=version_key, student_version=student_version, non_graphical=non_graphical
-                )
-                if aedt_process_id:
-                    for session in sessions:
-                        if session[0] == aedt_process_id and session[1] != -1:
-                            self.port = session[1]
-                            settings.use_grpc_api = True
-                            break
-                        elif session[0] == aedt_process_id:
-                            settings.use_grpc_api = False
-                            break
-
-            if version_key < "2022.2":
-                settings.use_grpc_api = False
-            elif (
-                version_key.startswith("2022.2")
-                and not self.port
-                and not self.machine
-                and settings.use_grpc_api is None
-                and _com != "gprc_v3"
-            ):
-                settings.use_grpc_api = False
-            elif settings.use_grpc_api is None or _com == "gprc_v3":
-                settings.use_grpc_api = True
-            if _com == "ironpython":  # pragma: no cover
-                self._logger.info("Launching PyAEDT outside AEDT with IronPython.")
-                self._init_ironpython(non_graphical, new_desktop_session, version)
-            elif settings.use_grpc_api:
-                settings.use_grpc_api = True
-                self._init_cpython_new(
-                    non_graphical, new_desktop_session, version, self._main.student_version, version_key
-                )
-            elif _com == "pythonnet_v3":
-                self._logger.info("Launching PyAEDT outside AEDT with CPython and PythonNET.")
-                self._init_cpython(
-                    non_graphical,
-                    new_desktop_session,
-                    version,
-                    self._main.student_version,
-                    version_key,
-                    aedt_process_id,
-                )
-            else:
-                from pyaedt.generic.clr_module import win32_client
+    Parameters
+    ----------
+    input_version : str
+       AEDT student version.
 
-                oAnsoftApp = win32_client.Dispatch(version)
-                self._main.oDesktop = oAnsoftApp.GetAppDesktop()
-                self._main.isoutsideDesktop = True
-        self._set_logger_file()
-        self._init_desktop(non_graphical)
-        self._logger.info("pyaedt v%s", self._main.pyaedt_version)
-        if not settings.remote_api:
-            self._logger.info("Python version %s", sys.version)
-        self.odesktop = self._main.oDesktop
-        settings.machine = self.machine
-        settings.port = self.port
-        self.aedt_process_id = self.odesktop.GetProcessID()  # bit of cleanup for consistency if used in future
-        settings.aedt_process_id = self.aedt_process_id
-        settings.is_student = student_version
-        self._logger.info("AEDT %s Build Date %s", self.odesktop.GetVersion(), self.odesktop.GetBuildDateTimeString())
-
-        if _com == "ironpython":
-            sys.path.append(
-                os.path.join(self._main.sDesktopinstallDirectory, "common", "commonfiles", "IronPython", "DLLs")
-            )
+    Returns
+    -------
+    str
+        Path for the student version environment variable.
 
-    def __enter__(self):
-        return self
+    Examples
+    --------
+    >>> env_path_student("2021.2")
+    "C:/Program Files/ANSYSEM/ANSYSEM2021.2/Win64"
+    """
+    return os.getenv(
+        "ANSYSEMSV_ROOT{0}{1}".format(
+            get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
+        ),
+        "",
+    )
 
-    def __exit__(self, ex_type, ex_value, ex_traceback):
-        # Write the trace stack to the log file if an exception occurred in the main script.
-        if ex_type:
-            err = self._exception(ex_value, ex_traceback)
-        if self.close_on_exit or not is_ironpython:
-            self.release_desktop(close_projects=self.close_on_exit, close_on_exit=self.close_on_exit)
 
-    @pyaedt_function_handler()
-    def __getitem__(self, project_design_name):
-        """Get the application interface object (Hfss, Icepak, Maxwell3D...) for a given project name and design name.
+@pyaedt_function_handler()
+def env_value_student(input_version):
+    """Get the name of the version environment variable for an AEDT student version.
 
-        Parameters
-        ----------
-        project_design_name : list
-            Project and design name.
+    Parameters
+    ----------
+    input_version : str
+        AEDT student version.
 
-        Returns
-        -------
-        :class:Application interface
-            Returns None if project and design name are not found.
+    Returns
+    -------
+    str
+         Name for the student version environment variable.
 
-        """
-        from pyaedt import get_pyaedt_app
+    Examples
+    --------
+    >>> env_value_student("2021.2")
+    "ANSYSEMSV_ROOT211"
+    """
+    return "ANSYSEMSV_ROOT{0}{1}".format(
+        get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
+    )
 
-        if len(project_design_name) != 2:
-            return None
-        if isinstance(project_design_name[0], int) and project_design_name[0] < len(self.project_list()):
-            projectname = self.project_list()[project_design_name[0]]
-        elif isinstance(project_design_name[0], str) and project_design_name[0] in self.project_list():
-            projectname = project_design_name[0]
-        else:
-            return None
 
-        initial_oproject = self.odesktop.GetActiveProject()
-        if initial_oproject.GetName() != projectname:
-            self.odesktop.SetActiveProject(projectname)
-
-        if isinstance(project_design_name[1], int) and project_design_name[1] < len(self.design_list()):
-            designname = self.design_list()[project_design_name[1]]
-        elif isinstance(project_design_name[1], str) and project_design_name[1] in self.design_list():
-            designname = project_design_name[1]
-        else:
-            return None
+@pyaedt_function_handler()
+def get_filename_without_extension(path):
+    """Get the filename without its extension.
 
-        return get_pyaedt_app(projectname, designname)
+    Parameters
+    ----------
+    path : str
+        Path for the file.
 
-    @property
-    def install_path(self):
-        """Installation path for AEDT."""
-        version_key = self._main.AEDTVersion
-        root = self._version_ids[version_key]
-        return os.environ[root]
 
-    @property
-    def version_keys(self):
-        """Version keys for AEDT."""
+    Returns
+    -------
+    str
+       Name for the file, excluding its extension.
 
-        self._version_keys = []
-        self._version_ids = {}
-        version_list = list_installed_ansysem()
-        for version_env_var in version_list:
-            if "ANSYSEMSV_ROOT" in version_env_var:
-                current_version_id = version_env_var.replace("ANSYSEMSV_ROOT", "")
-                student = True
-            else:
-                current_version_id = version_env_var.replace("ANSYSEM_ROOT", "")
-                student = False
-            try:
-                version = int(current_version_id[0:2])
-                release = int(current_version_id[2])
-                if version < 20:
-                    if release < 3:
-                        version -= 1
-                    else:
-                        release -= 2
-                if student:
-                    v_key = "20{0}.{1}SV".format(version, release)
-                    self._version_keys.append(v_key)
-                    self._version_ids[v_key] = version_env_var
-                else:
-                    v_key = "20{0}.{1}".format(version, release)
-                    self._version_keys.append(v_key)
-                    self._version_ids[v_key] = version_env_var
-            except:
-                pass
-        return self._version_keys
+    """
+    return os.path.splitext(os.path.split(path)[1])[0]
 
-    @property
-    def current_version(self):
-        """Current AEDT version."""
-        try:
-            return self.version_keys[0]
-        except (NameError, IndexError):
-            return ""
-
-    @property
-    def current_version_student(self):
-        """Current student AEDT version."""
-        for version_key in self.version_keys:
-            if "SV" in version_key:
-                return version_key
-        return ""
-
-    def _init_desktop(self, non_graphical):
-        self._main.AEDTVersion = self._main.oDesktop.GetVersion()[0:6]
-        self._main.oDesktop.RestoreWindow()
-        self._main.sDesktopinstallDirectory = self._main.oDesktop.GetExeDir()
-        self._main.pyaedt_initialized = True
-        if non_graphical or self._main.oDesktop.GetIsNonGraphical():
-            try:
-                settings.enable_desktop_logs = not self._main.oDesktop.GetIsNonGraphical()
-            except AttributeError:
-                settings.enable_desktop_logs = not non_graphical
 
-    def _set_version(self, specified_version, student_version):
-        student_version_flag = False
-        if specified_version:
-            if float(specified_version) < 2021:
-                if float(specified_version) < 2019:
-                    raise ValueError("PyAEDT supports AEDT version 2021 R1 and later.")
-                else:
-                    warnings.warn(
-                        """PyAEDT has limited capabilities when used with an AEDT version earlier than 2021 R1.
-                        PyAEDT officially supports AEDT version 2021 R1 and later."""
-                    )
-            if student_version:
-                specified_version += "SV"
-                student_version_flag = True
-            assert specified_version in self.version_keys, "Specified version {} is not known".format(specified_version)
-            version_key = specified_version
+@pyaedt_function_handler()
+def generate_unique_name(rootname, suffix="", n=6):
+    """Generate a new name given a root name and optional suffix.
+
+    Parameters
+    ----------
+    rootname :
+        Root name to add random characters to.
+    suffix : string
+        Suffix to add. The default is ``''``.
+    n : int
+        Number of random characters to add to the name. The default value is ``6``.
+
+    Returns
+    -------
+    str
+        Newly generated name.
+
+    """
+    char_set = string.ascii_uppercase + string.digits
+    uName = "".join(random.choice(char_set) for _ in range(n))
+    unique_name = rootname + "_" + uName
+    if suffix:
+        unique_name += "_" + suffix
+    return unique_name
+
+
+@pyaedt_function_handler()
+def generate_unique_folder_name(rootname=None, folder_name=None):
+    """Generate a new AEDT folder name given a rootname.
+
+    Parameters
+    ----------
+    rootname : str, optional
+        Root name for the new folder. The default is ``None``.
+    folder_name : str, optional
+        Name for the new AEDT folder if one must be created.
+
+    Returns
+    -------
+    str
+    """
+    if not rootname:
+        if settings.remote_rpc_session:
+            rootname = settings.remote_rpc_session_temp_folder
+        else:
+            rootname = tempfile.gettempdir()
+    if folder_name is None:
+        folder_name = generate_unique_name("pyaedt_prj", n=3)
+    temp_folder = os.path.join(rootname, folder_name)
+    if settings.remote_rpc_session and not settings.remote_rpc_session.filemanager.pathexists(temp_folder):
+        settings.remote_rpc_session.filemanager.makedirs(temp_folder)
+    elif not os.path.exists(temp_folder):
+        os.makedirs(temp_folder)
+
+    return temp_folder
+
+
+@pyaedt_function_handler()
+def generate_unique_project_name(rootname=None, folder_name=None, project_name=None, project_format="aedt"):
+    """Generate a new AEDT project name given a rootname.
+
+    Parameters
+    ----------
+    rootname : str, optional
+        Root name where the new project is to be created.
+    folder_name : str, optional
+        Name of the folder to create. The default is ``None``, in which case a random folder
+        is created. Use ``""`` if you do not want to create a subfolder.
+    project_name : str, optional
+        Name for the project. The default is ``None``, in which case a random project is
+        created. If a project with this name already exists, a new suffix is added.
+    project_format : str, optional
+        Project format. The default is ``"aedt"``. Options are ``"aedt"`` and ``"aedb"``.
+
+    Returns
+    -------
+    str
+    """
+    if not project_name:
+        project_name = generate_unique_name("Project", n=3)
+    name_with_ext = project_name + "." + project_format
+    folder_path = generate_unique_folder_name(rootname, folder_name=folder_name)
+    prj = os.path.join(folder_path, name_with_ext)
+    if check_if_path_exists(prj):
+        name_with_ext = generate_unique_name(project_name, n=3) + "." + project_format
+        prj = os.path.join(folder_path, name_with_ext)
+    return prj
+
+
+def _retry_ntimes(n, function, *args, **kwargs):
+    """
+
+    Parameters
+    ----------
+    n :
+
+    function :
+
+    *args :
+
+    **kwargs :
+
+
+    Returns
+    -------
+
+    """
+    retry = 0
+    ret_val = None
+    while retry < n:
+        try:
+            ret_val = function(*args, **kwargs)
+            # if ret_val is None:
+            # if not ret_val and type(ret_val) not in [float, int, str, tuple, list]:
+            #    ret_val = True
+        except:
+            retry += 1
+            time.sleep(0.1)
         else:
-            if student_version and self.current_version_student:
-                version_key = self.current_version_student
-                student_version_flag = True
-            else:
-                version_key = self.current_version
-                student_version_flag = False
-        if student_version and student_version_flag:
-            version = "Ansoft.ElectronicsDesktop." + version_key[:-2]
+            break
+    if retry == n:
+        if "__name__" in dir(function):
+            raise AttributeError("Error in Executing Method {}.".format(function.__name__))
         else:
-            version = "Ansoft.ElectronicsDesktop." + version_key
-        self._main.sDesktopinstallDirectory = os.getenv(self._version_ids[version_key])
-        return student_version_flag, version_key, version
-
-    def _init_ironpython(self, non_graphical, new_aedt_session, version):
-        from pyaedt.generic.clr_module import _clr
-
-        base_path = self._main.sDesktopinstallDirectory
-        sys.path.append(base_path)
-        sys.path.append(os.path.join(base_path, "PythonFiles", "DesktopPlugin"))
-        _clr.AddReference("Ansys.Ansoft.CoreCOMScripting")
-        AnsoftCOMUtil = __import__("Ansys.Ansoft.CoreCOMScripting")
-        self.COMUtil = AnsoftCOMUtil.Ansoft.CoreCOMScripting.Util.COMUtil
-        self._main.COMUtil = self.COMUtil
-        StandalonePyScriptWrapper = AnsoftCOMUtil.Ansoft.CoreCOMScripting.COM.StandalonePyScriptWrapper
-        if non_graphical or new_aedt_session:
-            # forcing new thread to start in non-graphical
-            oAnsoftApp = StandalonePyScriptWrapper.CreateObjectNew(non_graphical)
+            raise AttributeError("Error in Executing Method.")
+
+    return ret_val
+
+
+def time_fn(fn, *args, **kwargs):
+    start = datetime.datetime.now()
+    results = fn(*args, **kwargs)
+    end = datetime.datetime.now()
+    fn_name = fn.__module__ + "." + fn.__name__
+    delta = (end - start).microseconds * 1e-6
+    print(fn_name + ": " + str(delta) + "s")
+    return results
+
+
+def isclose(a, b, rel_tol=1e-9, abs_tol=0.0):
+    return abs(a - b) <= max(rel_tol * max(abs(a), abs(b)), abs_tol)
+
+
+def is_number(a):
+    if isinstance(a, float) or isinstance(a, int):
+        return True
+    elif isinstance(a, str):
+        try:
+            float(a)
+            return True
+        except ValueError:
+            return False
+    else:
+        return False
+
+
+def is_array(a):
+    try:
+        v = list(ast.literal_eval(a))
+    except (ValueError, TypeError, NameError, SyntaxError):
+        return False
+    else:
+        if type(v) is list:
+            return True
         else:
-            oAnsoftApp = StandalonePyScriptWrapper.CreateObject(version)
-        self._main.oDesktop = oAnsoftApp.GetAppDesktop()
-        self._main.isoutsideDesktop = True
-        sys.path.append(os.path.join(base_path, "common", "commonfiles", "IronPython", "DLLs"))
+            return False
+
+
+def is_project_locked(project_path):
+    """Check if an AEDT project lock file exists.
+
+    Parameters
+    ----------
+    project_path : str
+        Path for the AEDT project.
+
+    Returns
+    -------
+    bool
+        ``True`` when successful, ``False`` when failed.
+    """
+    return check_if_path_exists(project_path + ".lock")
+
+
+@pyaedt_function_handler()
+def remove_project_lock(project_path):
+    """Check if an AEDT project exists and try to remove the lock file.
+
+    .. note::
+       This operation is risky because the file could be opened in another AEDT instance.
+
+    Parameters
+    ----------
+    project_path : str
+        Path for the AEDT project.
 
+    Returns
+    -------
+    bool
+        ``True`` when successful, ``False`` when failed.
+    """
+    if os.path.exists(project_path + ".lock"):
+        os.remove(project_path + ".lock")
+    return True
+
+
+@pyaedt_function_handler()
+def read_csv(filename, encoding="utf-8"):
+    """Read information from a CSV file and return a list.
+
+    Parameters
+    ----------
+    filename : str
+            Full path and name for the CSV file.
+    encoding : str, optional
+            File encoding for the CSV file. The default is ``"utf-8"``.
+
+    Returns
+    -------
+    list
+
+    """
+
+    lines = []
+    with codecs.open(filename, "rb", encoding) as csvfile:
+        reader = csv.reader(csvfile, delimiter=",")
+        for row in reader:
+            lines.append(row)
+    return lines
+
+
+@pyaedt_function_handler()
+def read_csv_pandas(filename, encoding="utf-8"):
+    """Read information from a CSV file and return a list.
+
+    Parameters
+    ----------
+    filename : str
+            Full path and name for the CSV file.
+    encoding : str, optional
+            File encoding for the CSV file. The default is ``"utf-8"``.
+
+    Returns
+    -------
+    :class:`pandas.DataFrame`
+
+    """
+    try:
+        import pandas as pd
+
+        return pd.read_csv(filename, encoding=encoding, header=0, na_values=".")
+    except ImportError:
+        logging.error("Pandas is not available. Install it.")
+        return None
+
+
+@pyaedt_function_handler()
+def read_tab(filename):
+    """Read information from a TAB file and return a list.
+
+    Parameters
+    ----------
+    filename : str
+            Full path and name for the TAB file.
+
+    Returns
+    -------
+    list
+
+    """
+    with open(filename) as my_file:
+        lines = my_file.readlines()
+    return lines
+
+
+@pyaedt_function_handler()
+def read_xlsx(filename):
+    """Read information from an XLSX file and return a list.
+
+    Parameters
+    ----------
+    filename : str
+            Full path and name for the XLSX file.
+
+    Returns
+    -------
+    list
+
+    """
+    try:
+        import pandas as pd
+
+        lines = pd.read_excel(filename)
+        return lines
+    except ImportError:
+        lines = []
+        return lines
+
+
+@pyaedt_function_handler()
+def write_csv(output, list_data, delimiter=",", quotechar="|", quoting=csv.QUOTE_MINIMAL):
+    if is_ironpython:
+        f = open(output, "wb")
+    else:
+        f = open(output, "w", newline="")
+    writer = csv.writer(f, delimiter=delimiter, quotechar=quotechar, quoting=quoting)
+    for data in list_data:
+        writer.writerow(data)
+    f.close()
+    return True
+
+
+@pyaedt_function_handler()
+def filter_tuple(value, search_key1, search_key2):
+    """Filter a tuple of two elements with two search keywords."""
+    ignore_case = True
+
+    def _create_pattern(k1, k2):
+        k1a = re.sub(r"\?", r".", k1)
+        k1b = re.sub(r"\*", r".*?", k1a)
+        k2a = re.sub(r"\?", r".", k2)
+        k2b = re.sub(r"\*", r".*?", k2a)
+        pattern = r".*\({},{}\)".format(k1b, k2b)
+        return pattern
+
+    if ignore_case:
+        compiled_re = re.compile(_create_pattern(search_key1, search_key2), re.IGNORECASE)
+    else:
+        compiled_re = re.compile(_create_pattern(search_key1, search_key2))
+
+    m = compiled_re.search(value)
+    if m:
         return True
+    return False
 
-    def _run_student(self):
-        DETACHED_PROCESS = 0x00000008
-        pid = subprocess.Popen(
-            [os.path.join(self._main.sDesktopinstallDirectory, "ansysedtsv.exe")], creationflags=DETACHED_PROCESS
-        ).pid
-        time.sleep(5)
-
-    def _dispatch_win32(self, version):
-        from pyaedt.generic.clr_module import win32_client
-
-        o_ansoft_app = win32_client.Dispatch(version)
-        self._main.oDesktop = o_ansoft_app.GetAppDesktop()
-        self._main.isoutsideDesktop = True
-
-    def _init_cpython(
-        self,
-        non_graphical,
-        new_aedt_session,
-        version,
-        student_version,
-        version_key,
-        aedt_process_id=None,
-    ):  # pragma: no cover
-        import pythoncom
 
-        from pyaedt.generic.clr_module import _clr
+@pyaedt_function_handler()
+def filter_string(value, search_key1):
+    """Filter a string"""
+    ignore_case = True
+
+    def _create_pattern(k1):
+        k1a = re.sub(r"\?", r".", k1.replace("\\", "\\\\"))
+        k1b = re.sub(r"\*", r".*?", k1a)
+        pattern = r"^{}$".format(k1b)
+        return pattern
 
-        if is_linux:
-            raise Exception(
-                "PyAEDT supports COM initialization in Windows only. To use in Linux, upgrade to AEDT 2022 R2 or later."
-            )
-        base_path = self._main.sDesktopinstallDirectory
-        sys.path.insert(0, base_path)
-        sys.path.insert(0, os.path.join(base_path, "PythonFiles", "DesktopPlugin"))
-        launch_msg = "AEDT installation Path {}.".format(base_path)
-        self.logger.info(launch_msg)
-        _clr.AddReference("Ansys.Ansoft.CoreCOMScripting")
-        AnsoftCOMUtil = __import__("Ansys.Ansoft.CoreCOMScripting")
-        self.COMUtil = AnsoftCOMUtil.Ansoft.CoreCOMScripting.Util.COMUtil
-        self._main.COMUtil = self.COMUtil
-        StandalonePyScriptWrapper = AnsoftCOMUtil.Ansoft.CoreCOMScripting.COM.StandalonePyScriptWrapper
-        self.logger.info("Launching AEDT with module PythonNET.")
-        processID = []
-        if is_windows:
-            processID = com_active_sessions(version, student_version, non_graphical)
-        if student_version and not processID:  # Opens an instance if processID is an empty list
-            self._run_student()
-        elif non_graphical or new_aedt_session or not processID:
-            # Force new object if no non-graphical instance is running or if there is not an already existing process.
-            StandalonePyScriptWrapper.CreateObjectNew(non_graphical)
-        else:
-            StandalonePyScriptWrapper.CreateObject(version)
-        processID2 = []
-        if is_windows:
-            processID2 = com_active_sessions(version, student_version, non_graphical)
-        proc = [i for i in processID2 if i not in processID]  # Looking for the "new" process
-        if (
-            not proc and (not new_aedt_session) and aedt_process_id
-        ):  # if it isn't a new aedt session and a process ID is given
-            proc = [aedt_process_id]
-        elif not proc:
-            proc = processID2
-        if proc == processID2 and len(processID2) > 1:
-            self._dispatch_win32(version)
-        elif version_key >= "2021.2":
-            if student_version:
-                self.logger.info("AEDT {} Student version started with process ID {}.".format(version_key, proc[0]))
-            else:
-                self.logger.info("AEDT {} Started with process ID {}.".format(version_key, proc[0]))
-            context = pythoncom.CreateBindCtx(0)
-            running_coms = pythoncom.GetRunningObjectTable()
-            monikiers = running_coms.EnumRunning()
-            for monikier in monikiers:
-                m = re.search(version[10:] + r"\.\d:" + str(proc[0]), monikier.GetDisplayName(context, monikier))
-                if m:
-                    obj = running_coms.GetObject(monikier)
-                    self._main.isoutsideDesktop = True
-                    from pyaedt.generic.clr_module import win32_client
+    if ignore_case:
+        compiled_re = re.compile(_create_pattern(search_key1), re.IGNORECASE)
+    else:
+        compiled_re = re.compile(_create_pattern(search_key1))  # pragma: no cover
 
-                    self._main.oDesktop = win32_client.Dispatch(obj.QueryInterface(pythoncom.IID_IDispatch))
-                    break
-        else:
-            self.logger.warning(
-                "PyAEDT is not supported in AEDT versions earlier than 2021 R2. Trying to launch PyAEDT with PyWin32."
-            )
-            self._dispatch_win32(version)
+    m = compiled_re.search(value)
+    if m:
+        return True
+    return False
 
-    def _init_cpython_new(self, non_graphical, new_aedt_session, version, student_version, version_key):
-        base_path = self._main.sDesktopinstallDirectory
-        sys.path.insert(0, base_path)
-        sys.path.insert(0, os.path.join(base_path, "PythonFiles", "DesktopPlugin"))
-        if is_linux:
-            if os.environ.get("LD_LIBRARY_PATH"):
-                os.environ["LD_LIBRARY_PATH"] = (
-                    os.path.join(base_path, "defer") + os.pathsep + os.environ["LD_LIBRARY_PATH"]
-                )
-            else:
-                os.environ["LD_LIBRARY_PATH"] = os.path.join(base_path, "defer")
-            pyaedt_path = os.path.realpath(os.path.join(os.path.dirname(os.path.realpath(__file__)), ".."))
-            os.environ["PATH"] = pyaedt_path + os.pathsep + os.environ["PATH"]
-
-        import ScriptEnv
-
-        launch_msg = "AEDT installation Path {}".format(base_path)
-        self.logger.info(launch_msg)
-        self.logger.info("Launching AEDT with the gRPC plugin.")
-        if not self.machine or self.machine in [
-            "localhost",
-            "127.0.0.1",
-            socket.getfqdn(),
-            socket.getfqdn().split(".")[0],
-        ]:
-            self.machine = ""
-        else:
-            settings.remote_api = True
 
-        if not self.port:
-            if self.machine:
-                self.logger.error("New Session of AEDT cannot be started on remote machine from Desktop Class.")
-                self.logger.error("Either use port argument or start an rpc session to start AEDT on remote machine.")
-                self.logger.error("Use client = pyaedt.common_rpc.client(machinename) to start a remote session.")
-                self.logger.error("Use client.aedt(port) to start aedt on remote machine before connecting.")
-            elif new_aedt_session:
-                self.port = _find_free_port()
-                self.logger.info("New AEDT session is starting on gRPC port %s", self.port)
-            else:
-                sessions = grpc_active_sessions(
-                    version=version, student_version=student_version, non_graphical=non_graphical
-                )
-                if sessions:
-                    self.port = sessions[0]
-                    if len(sessions):
-                        self.logger.info("Found active AEDT gRPC session on port %s", self.port)
-                    else:
-                        self.logger.warning(
-                            "Multiple AEDT gRPC sessions are found. Setting the active session on port %s", self.port
-                        )
-                else:
-                    if is_windows:  # pragma: no cover
-                        if com_active_sessions(
-                            version=version, student_version=student_version, non_graphical=non_graphical
-                        ):
-                            settings.use_grpc_api = False
-                            self.logger.info("No AEDT gRPC found. Found active COM Sessions.")
-                            return self._init_cpython(
-                                non_graphical, new_aedt_session, version, student_version, version_key
+@pyaedt_function_handler()
+def recursive_glob(startpath, filepattern):
+    """Get a list of files matching a pattern, searching recursively from a start path.
+
+    Keyword Arguments:
+    startpath -- starting path (directory)
+    filepattern -- fnmatch-style filename pattern
+    """
+    if settings.remote_rpc_session:
+        files = []
+        for i in settings.remote_rpc_session.filemanager.listdir(startpath):
+            if settings.remote_rpc_session.filemanager.isdir(os.path.join(startpath, i)):
+                files.extend(recursive_glob(os.path.join(startpath, i), filepattern))
+            elif fnmatch.fnmatch(i, filepattern):
+                files.append(os.path.join(startpath, i))
+        return files
+    else:
+        return [
+            os.path.join(dirpath, filename)
+            for dirpath, _, filenames in os.walk(startpath)
+            for filename in filenames
+            if fnmatch.fnmatch(filename, filepattern)
+        ]
+
+
+@pyaedt_function_handler()
+def number_aware_string_key(s):
+    """Get a key for sorting strings that treats embedded digit sequences as integers.
+
+    Parameters
+    ----------
+    s : str
+        String to calculate the key from.
+
+    Returns
+    -------
+    tuple
+        Tuple of key entries.
+    """
+
+    def is_digit(c):
+        return "0" <= c and c <= "9"
+
+    result = []
+    i = 0
+    while i < len(s):
+        if is_digit(s[i]):
+            j = i + 1
+            while j < len(s) and is_digit(s[j]):
+                j += 1
+            key = int(s[i:j])
+            result.append(key)
+            i = j
+        else:
+            j = i + 1
+            while j < len(s) and not is_digit(s[j]):
+                j += 1
+            key = s[i:j]
+            result.append(key)
+            i = j
+    return tuple(result)
+
+
+@pyaedt_function_handler()
+def _create_json_file(json_dict, full_json_path):
+    if not is_ironpython:
+        with open(full_json_path, "w") as fp:
+            json.dump(json_dict, fp, indent=4)
+    else:
+        temp_path = full_json_path.replace(".json", "_temp.json")
+        with open(temp_path, "w") as fp:
+            json.dump(json_dict, fp, indent=4)
+        with open(temp_path, "r") as file:
+            filedata = file.read()
+        filedata = filedata.replace("True", "true")
+        filedata = filedata.replace("False", "false")
+        with open(full_json_path, "w") as file:
+            file.write(filedata)
+        os.remove(temp_path)
+    return True
+
+
+@pyaedt_function_handler()
+def com_active_sessions(version=None, student_version=False, non_graphical=False):
+    """Get information for the active COM AEDT sessions.
+
+    Parameters
+    ----------
+    version : str, optional
+        Version to check. The default is ``None``, in which case all versions are checked.
+        When specifying a version, you can use a three-digit format like ``"222"`` or a
+        five-digit format like ``"2022.2"``.
+    student_version : bool, optional
+        Whether to check for student version sessions. The default is ``False``.
+    non_graphical : bool, optional
+        Whether to check only for active non-graphical sessions. The default is ``False``.
+
+    Returns
+    -------
+    list
+        List of AEDT PIDs.
+    """
+    if student_version:
+        keys = ["ansysedtsv.exe"]
+    else:
+        keys = ["ansysedt.exe"]
+    long_version = None
+    if len(version) > 6:
+        version = version[-6:]
+    if version and "." in version:
+        long_version = version
+        version = version[-4:].replace(".", "")
+    if version < "221":
+        version = version[:2] + "." + version[2]
+        long_version = "20{}".format(version)
+    sessions = []
+    for p in psutil.process_iter():
+        try:
+            if p.name() in keys:
+                if long_version and _check_installed_version(os.path.dirname(p.exe()), long_version):
+                    sessions.append(p.pid)
+                    continue
+                cmd = p.cmdline()
+                if non_graphical and "-ng" in cmd or not non_graphical:
+                    if not version or (version and version in cmd[0]):
+                        sessions.append(p.pid)
+        except:
+            pass
+    return sessions
+
+
+@pyaedt_function_handler()
+def grpc_active_sessions(version=None, student_version=False, non_graphical=False):
+    """Get information for the active gRPC AEDT sessions.
+
+    Parameters
+    ----------
+    version : str, optional
+        Version to check. The default is ``None``, in which case all versions are checked.
+        When specififying a version, you can use a three-digit format like ``"222"`` or a
+        five-digit format like ``"2022.2"``.
+    student_version : bool, optional
+        Whether to check for student version sessions. The default is ``False``.
+    non_graphical : bool, optional
+        Whether to check only for active non-graphical sessions. The default is ``False``.
+
+    Returns
+    -------
+    list
+        List of gRPC ports.
+    """
+    if student_version:
+        keys = ["ansysedtsv.exe", "ansysedtsv"]
+    else:
+        keys = ["ansysedt.exe", "ansysedt"]
+    if version and "." in version:
+        version = version[-4:].replace(".", "")
+    sessions = []
+    for p in psutil.process_iter():
+        try:
+            if p.name() in keys:
+                cmd = p.cmdline()
+                if "-grpcsrv" in cmd:
+                    if non_graphical and "-ng" in cmd or not non_graphical:
+                        if not version or (version and version in cmd[0]):
+                            try:
+                                sessions.append(
+                                    int(cmd[cmd.index("-grpcsrv") + 1]),
+                                )
+                            except (IndexError, ValueError):
+                                # default desktop grpc port.
+                                sessions.append(50051)
+        except:
+            pass
+    return sessions
+
+
+def active_sessions(version=None, student_version=False, non_graphical=False):
+    """Get information for the active COM AEDT sessions.
+
+    Parameters
+    ----------
+    version : str, optional
+        Version to check. The default is ``None``, in which case all versions are checked.
+        When specifying a version, you can use a three-digit format like ``"222"`` or a
+        five-digit format like ``"2022.2"``.
+    student_version : bool, optional
+    non_graphical : bool, optional
+
+
+    Returns
+    -------
+    list
+        List of AEDT PIDs.
+    """
+    if student_version:
+        keys = ["ansysedtsv.exe", "ansysedtsv"]
+    else:
+        keys = ["ansysedt.exe", "ansysedt"]
+    if version and "." in version:
+        version = version[-4:].replace(".", "")
+    if version and version < "222":
+        version = version[:2] + "." + version[2]
+    sessions = []
+    for p in psutil.process_iter():
+        try:
+            if p.name() in keys:
+                cmd = p.cmdline()
+                if non_graphical and "-ng" in cmd or not non_graphical:
+                    if not version or (version and version in cmd[0]):
+                        if "-grpcsrv" in cmd:
+                            if not version or (version and version in cmd[0]):
+                                try:
+                                    sessions.append(
+                                        [
+                                            p.pid,
+                                            int(cmd[cmd.index("-grpcsrv") + 1]),
+                                        ]
+                                    )
+                                except (IndexError, ValueError):
+                                    # default desktop grpc port.
+                                    sessions.append(
+                                        [
+                                            p.pid,
+                                            50051,
+                                        ]
+                                    )
+                        else:
+                            sessions.append(
+                                [
+                                    p.pid,
+                                    -1,
+                                ]
                             )
-                    self.port = _find_free_port()
-                    self.logger.info("New AEDT session is starting on gRPC port %s", self.port)
-                    new_aedt_session = True
-        elif new_aedt_session and not _check_grpc_port(self.port, self.machine):
-            self.logger.info("New AEDT session is starting on gRPC port %s", self.port)
-        elif new_aedt_session:
-            self.logger.warning("New Session of AEDT cannot be started on specified port because occupied.")
-            self.port = _find_free_port()
-            self.logger.info("New AEDT session is starting on gRPC port %s", self.port)
-        elif _check_grpc_port(self.port, self.machine):
-            self.logger.info("Connecting to AEDT session on gRPC port %s", self.port)
-        else:
-            self.logger.info("AEDT session is starting on gRPC port %s", self.port)
-            new_aedt_session = True
+        except:
+            pass
+    return sessions
 
-        if new_aedt_session and settings.use_lsf_scheduler and is_linux:  # pragma: no cover
-            out, self.machine = launch_aedt_in_lsf(non_graphical, self.port)
-            if out:
-                ScriptEnv._doInitialize(version, None, False, non_graphical, self.machine, self.port)
-            else:
-                self.logger.error("Failed to start LSF job on machine: %s.", self.machine)
-                return
-        elif new_aedt_session:
-            installer = os.path.join(base_path, "ansysedt")
-            if not is_linux:
-                installer = os.path.join(base_path, "ansysedt.exe")
-            out, self.port = launch_aedt(installer, non_graphical, self.port)
-            ScriptEnv._doInitialize(version, None, not out, non_graphical, self.machine, self.port)
-        else:
-            ScriptEnv._doInitialize(version, None, new_aedt_session, non_graphical, self.machine, self.port)
-        if "oAnsoftApplication" in dir(self._main):
-            self._main.isoutsideDesktop = True
-            self._main.oDesktop = self._main.oAnsoftApplication.GetAppDesktop()
-            _proc = self._main.oDesktop.GetProcessID()
-            if new_aedt_session:
-                message = "{} {} version started with process ID {}.".format(
-                    version, "Student" if student_version else "", _proc
-                )
-                self.logger.info(message)
 
-        else:
-            self.logger.error("Failed to connect to AEDT using gRPC plugin.")
-            self.logger.error("Check installation, license and environment variables.")
+@pyaedt_function_handler()
+def compute_fft(time_vals, value):  # pragma: no cover
+    """Compute FFT of input transient data.
 
-    def _set_logger_file(self):
-        # Set up the log file in the AEDT project directory
-        if settings.remote_api:
-            project_dir = tempfile.gettempdir()
-        elif "oDesktop" in dir(self._main):
-            project_dir = self._main.oDesktop.GetProjectDirectory()
-        else:
-            project_dir = tempfile.gettempdir()
-        if settings.logger_file_path:
-            self.logfile = settings.logger_file_path
-        else:
-            if not project_dir:
-                project_dir = tempfile.gettempdir()
-            self.logfile = os.path.join(
-                project_dir, "pyaedt{}.log".format(datetime.datetime.now().strftime("%Y%m%d_%H%M%S"))
-            )
+    Parameters
+    ----------
+    time_vals : `pandas.Series`
+    value : `pandas.Series`
 
-        return True
+    Returns
+    -------
+    tuple
+        Frequency and Values.
+    """
+    try:
+        import numpy as np
+    except ImportError:
+        logging.error("NumPy is not available. Install it.")
+        return False
 
-    @property
-    def messenger(self):
-        """Messenger manager for the AEDT logger."""
-        return pyaedt_logger
+    deltaT = time_vals[-1] - time_vals[0]
+    num_points = len(time_vals)
+    valueFFT = np.fft.fft(value, num_points)
+    Npoints = int(len(valueFFT) / 2)
+    valueFFT = valueFFT[1 : Npoints + 1]
+    valueFFT = valueFFT / len(valueFFT)
+    n = np.arange(num_points)
+    freq = n / deltaT
+    return freq, valueFFT
+
+
+def parse_excitation_file(
+    file_name,
+    is_time_domain=True,
+    x_scale=1,
+    y_scale=1,
+    impedance=50,
+    data_format="Power",
+    encoding="utf-8",
+    out_mag="Voltage",
+):
+    """Parse a csv file and convert data in list that can be applied to Hfss and Hfss3dLayout sources.
 
-    @property
-    def logger(self):
-        """AEDT logger."""
-        return self._logger
+    Parameters
+    ----------
+    file_name : str
+        Full name of the input file.
+    is_time_domain : bool, optional
+        Either if the input data is Time based or Frequency Based. Frequency based data are Mag/Phase (deg).
+    x_scale : float, optional
+        Scaling factor for x axis.
+    y_scale : float, optional
+        Scaling factor for y axis.
+    data_format : str, optional
+        Either `"Power"`, `"Current"` or `"Voltage"`.
+    impedance : float, optional
+        Excitation impedance. Default is `50`.
+    encoding : str, optional
+        Csv file encoding.
+    out_mag : str, optional
+        Output magnitude format. It can be `"Voltage"` or `"Power"` depending on Hfss solution.
 
-    @pyaedt_function_handler()
-    def project_list(self):
-        """Get a list of projects.
+    Returns
+    -------
+    tuple
+        Frequency, magnitude and phase.
+    """
+    try:
+        import numpy as np
+    except ImportError:
+        logging.error("NumPy is not available. Install it.")
+        return False
+    df = read_csv_pandas(file_name, encoding=encoding)
+    if is_time_domain:
+        time = df[df.keys()[0]].values * x_scale
+        val = df[df.keys()[1]].values * y_scale
+        freq, fval = compute_fft(time, val)
+
+        if data_format.lower() == "current":
+            if out_mag == "Voltage":
+                fval = fval * impedance
+            else:
+                fval = fval * fval * impedance
+        elif data_format.lower() == "voltage":
+            if out_mag == "Power":
+                fval = fval * fval / impedance
+        else:
+            if out_mag == "Voltage":
+                fval = np.sqrt(fval * impedance)
+        mag = list(np.abs(fval))
+        phase = [math.atan2(j, i) * 180 / math.pi for i, j in zip(list(fval.real), list(fval.imag))]
 
-        Returns
-        -------
-        list
-            List of projects.
+    else:
+        freq = list(df[df.keys()[0]].values * x_scale)
+        if data_format.lower() == "current":
+            mag = df[df.keys()[1]].values * df[df.keys()[1]].values * impedance * y_scale * y_scale
+        elif data_format.lower() == "voltage":
+            mag = df[df.keys()[1]].values * df[df.keys()[1]].values / impedance * y_scale * y_scale
+        else:
+            mag = df[df.keys()[1]].values * y_scale
+        mag = list(mag)
+        phase = list(df[df.keys()[2]].values)
+    return freq, mag, phase
 
+
+def tech_to_control_file(tech_path, unit="nm", control_path=None):
+    """Convert a TECH file to an XML file for use in a GDS or DXF import.
+
+    Parameters
+    ----------
+    tech_path : str
+        Full path to the TECH file.
+    unit : str, optional
+        Tech units. If specified in tech file this parameter will not be used. Default is ``"nm"``.
+    control_path : str, optional
+        Path for outputting the XML file.
+
+    Returns
+    -------
+    str
+        Out xml file.
+    """
+    result = []
+    with open(tech_path) as f:
+        vals = list(CSS4_COLORS.values())
+        id_layer = 0
+        for line in f:
+            line_split = line.split()
+            if len(line_split) == 5:
+                layerID, layer_name, _, elevation, layer_height = line.split()
+                x = '      <Layer Color="{}" GDSIIVia="{}" Name="{}" TargetLayer="{}" Thickness="{}"'.format(
+                    vals[id_layer],
+                    "true" if layer_name.lower().startswith("v") else "false",
+                    layerID,
+                    layer_name,
+                    layer_height,
+                )
+                x += ' Type="conductor"/>'
+                result.append(x)
+                id_layer += 1
+            elif len(line_split) > 1 and "UNIT" in line_split[0]:
+                unit = line_split[1]
+    if not control_path:
+        control_path = os.path.splitext(tech_path)[0] + ".xml"
+    with open(control_path, "w") as f:
+        f.write('<?xml version="1.0" encoding="UTF-8" standalone="no" ?>\n')
+        f.write('    <c:Control xmlns:c="http://www.ansys.com/control" schemaVersion="1.0">\n')
+        f.write("\n")
+        f.write('      <Stackup schemaVersion="1.0">\n')
+        f.write('        <Layers LengthUnit="{}">\n'.format(unit))
+        for res in result:
+            f.write(res + "\n")
+
+        f.write("    </Layers>\n")
+        f.write("  </Stackup>\n")
+        f.write("\n")
+        f.write('  <ImportOptions Flatten="true" GDSIIConvertPolygonToCircles="false" ImportDummyNet="true"/>\n')
+        f.write("\n")
+        f.write("</c:Control>\n")
+
+    return control_path
+
+
+class PropsManager(object):
+    def __getitem__(self, item):
+        """Get the `self.props` key value.
+
+        Parameters
+        ----------
+        item : str
+            Key to search
         """
-        return list(self.odesktop.GetProjectList())
+        item_split = item.split("/")
+        if len(item_split) == 1:
+            item_split = item_split[0].split("__")
+        props = self.props
+        found_el = []
+        matching_percentage = 1
+        while matching_percentage >= 0.4:
+            for item_value in item_split:
+                found_el = self._recursive_search(props, item_value, matching_percentage)
+                # found_el = difflib.get_close_matches(item_value, list(props.keys()), 1, matching_percentage)
+                if found_el:
+                    props = found_el[1][found_el[2]]
+                    # props = props[found_el[0]]
+            if found_el:
+                return props
+            else:
+                matching_percentage -= 0.02
+        self._app.logger.warning("Key %s not found.Check one of available keys in self.available_properties", item)
+        return None
 
-    @pyaedt_function_handler()
-    def analyze_all(self, project=None, design=None):
-        """Analyze all setups in a project.
+    def __setitem__(self, key, value):
+        """Set the `self.props` key value.
 
         Parameters
         ----------
-        project : str, optional
-            Project name. The default is ``None``, in which case the active project
-            is used.
-        design : str, optional
-            Design name. The default is ``None``, in which case all designs in
-            the project are analyzed.
+        key : str
+            Key to apply.
+        value : int, float, bool, str, dict
+            Value to apply.
+        """
+        item_split = key.split("/")
+        if len(item_split) == 1:
+            item_split = item_split[0].split("__")
+        found_el = []
+        props = self.props
+        matching_percentage = 1
+        key_path = []
+        while matching_percentage >= 0.4:
+            for item_value in item_split:
+                found_el = self._recursive_search(props, item_value, matching_percentage)
+                if found_el:
+                    props = found_el[1][found_el[2]]
+                    key_path.append(found_el[2])
+            if found_el:
+                if matching_percentage < 1:
+                    self._app.logger.info(
+                        "Key %s matched internal key '%s' with confidence of %s.",
+                        key,
+                        "/".join(key_path),
+                        round(matching_percentage * 100),
+                    )
+                matching_percentage = 0
 
-        Returns
-        -------
-        bool
-            ``True`` when successful, ``False`` when failed.
-        """
-        if not project:
-            oproject = self.odesktop.GetActiveProject()
-        else:
-            oproject = self.odesktop.SetActiveProject(project)
-        if oproject:
-            if not design:
-                oproject.AnalyzeAll()
             else:
-                odesign = oproject.SetActiveDesign(design)
-                if odesign:
-                    odesign.AnalyzeAll()
-        return True
+                matching_percentage -= 0.02
+        if found_el:
+            found_el[1][found_el[2]] = value
+            self.update()
+        else:
+            props[key] = value
+            self.update()
+            self._app.logger.warning("Key %s not found. Trying to applying new key ", key)
 
     @pyaedt_function_handler()
-    def clear_messages(self):
-        """Clear all AEDT messages.
+    def _recursive_search(self, dict_in, key="", matching_percentage=0.8):
+        f = difflib.get_close_matches(key, list(dict_in.keys()), 1, matching_percentage)
+        if f:
+            return True, dict_in, f[0]
+        else:
+            for v in list(dict_in.values()):
+                if isinstance(v, (dict, OrderedDict)):
+                    out_val = self._recursive_search(v, key, matching_percentage)
+                    if out_val:
+                        return out_val
+                elif isinstance(v, list) and isinstance(v[0], (dict, OrderedDict)):
+                    for val in v:
+                        out_val = self._recursive_search(val, key, matching_percentage)
+                        if out_val:
+                            return out_val
+        return False
+
+    @pyaedt_function_handler()
+    def _recursive_list(self, dict_in, prefix=""):
+        available_list = []
+        for k, v in dict_in.items():
+            if prefix:
+                name = prefix + "/" + k
+            else:
+                name = k
+            available_list.append(name)
+            if isinstance(v, (dict, OrderedDict)):
+                available_list.extend(self._recursive_list(v, name))
+        return available_list
+
+    @property
+    def available_properties(self):
+        """Available properties.
 
         Returns
         -------
-        bool
-            ``True`` when successful, ``False`` when failed.
+        list
         """
-        self.odesktop.ClearMessages("", "", 3)
-        return True
+        if self.props:
+            return self._recursive_list(self.props)
+        return []
 
     @pyaedt_function_handler()
-    def save_project(self, project_name=None, project_path=None):
-        """Save the project.
+    def update(self):
+        """Update method."""
+        pass
 
-        Parameters
-        ----------
-        project_name : str, optional
-            Project name. The default is ``None``, in which case the active project
-            is used.
-        project_path : str, optional
-            Full path to the project. The default is ``None``. If a path is
-            provided, ``save as`` is used.
 
-        Returns
-        -------
-        bool
-            ``True`` when successful, ``False`` when failed.
-        """
-        if not project_name:
-            oproject = self.odesktop.GetActiveProject()
+clamp = lambda n, minn, maxn: max(min(maxn, n), minn)
+rgb_color_codes = {
+    "Black": (0, 0, 0),
+    "Green": (0, 128, 0),
+    "White": (255, 255, 255),
+    "Red": (255, 0, 0),
+    "Lime": (0, 255, 0),
+    "Blue": (0, 0, 255),
+    "Yellow": (255, 255, 0),
+    "Cyan": (0, 255, 255),
+    "Magenta": (255, 0, 255),
+    "Silver": (192, 192, 192),
+    "Gray": (128, 128, 128),
+    "Maroon": (128, 0, 0),
+    "Olive": (128, 128, 0),
+    "Purple": (128, 0, 128),
+    "Teal": (0, 128, 128),
+    "Navy": (0, 0, 128),
+    "copper": (184, 115, 51),
+    "stainless steel": (224, 223, 219),
+}
+
+
+@pyaedt_function_handler()
+def _arg2dict(arg, dict_out):
+    if arg[0] == "NAME:DimUnits" or "NAME:Point" in arg[0]:
+        if arg[0][5:] in dict_out:
+            if isinstance(dict_out[arg[0][5:]][0], (list, tuple)):
+                dict_out[arg[0][5:]].append(list(arg[1:]))
+            else:
+                dict_out[arg[0][5:]] = [dict_out[arg[0][5:]]]
+                dict_out[arg[0][5:]].append(list(arg[1:]))
         else:
-            oproject = self.odesktop.SetActiveProject(project_name)
-        if project_path:
-            oproject.SaveAs(project_path, True)
+            dict_out[arg[0][5:]] = list(arg[1:])
+    elif arg[0][:5] == "NAME:":
+        top_key = arg[0][5:]
+        dict_in = OrderedDict()
+        i = 1
+        while i < len(arg):
+            if arg[i][0][:5] == "NAME:" and (
+                isinstance(arg[i], (list, tuple)) or str(type(arg[i])) == r"<type 'List'>"
+            ):
+                _arg2dict(list(arg[i]), dict_in)
+                i += 1
+            elif arg[i][-2:] == ":=":
+                if str(type(arg[i + 1])) == r"<type 'List'>":
+                    if arg[i][:-2] in dict_in:
+                        dict_in[arg[i][:-2]].append(list(arg[i + 1]))
+                    else:
+                        dict_in[arg[i][:-2]] = list(arg[i + 1])
+                else:
+                    if arg[i][:-2] in dict_in:
+                        if isinstance(dict_in[arg[i][:-2]], list):
+                            dict_in[arg[i][:-2]].append(arg[i + 1])
+                        else:
+                            dict_in[arg[i][:-2]] = [dict_in[arg[i][:-2]]]
+                            dict_in[arg[i][:-2]].append(arg[i + 1])
+                    else:
+                        dict_in[arg[i][:-2]] = arg[i + 1]
+
+                i += 2
+            else:
+                raise ValueError("Incorrect data argument format")
+        if top_key in dict_out:
+            if isinstance(dict_out[top_key], list):
+                dict_out[top_key].append(dict_in)
+            else:
+                dict_out[top_key] = [dict_out[top_key], dict_in]
         else:
-            oproject.Save()
-        return True
+            dict_out[top_key] = dict_in
+    else:
+        raise ValueError("Incorrect data argument format")
 
-    @pyaedt_function_handler()
-    def copy_design(self, project_name=None, design_name=None, target_project=None):
-        """Copy a design and paste it in an existing project or new project.
 
-        .. deprecated:: 0.6.31
-           Use :func:`copy_design_from` instead.
+def _uname(name=None):
+    """Append a 6-digit hash code to a specified name.
 
-        Parameters
-        ----------
-        project_name : str, optional
-            Project name. The default is ``None``, in which case the active project
-            is used.
-        design_name : str, optional
-            Design name. The default is ``None``.
-        target_project : str, optional
-            Target project. The default is ``None``.
+    Parameters
+    ----------
+    name : str
+        Name to append the hash code to. The default is ``"NewObject_"``.
 
-        Returns
-        -------
-        bool
-            ``True`` when successful, ``False`` when failed.
-        """
-        if not project_name:  # pragma: no cover
-            oproject = self.odesktop.GetActiveProject()
-        else:  # pragma: no cover
-            oproject = self.odesktop.SetActiveProject(project_name)
-        if oproject:  # pragma: no cover
-            if not design_name:
-                odesign = oproject.GetActiveDesign()
-            else:
-                odesign = oproject.SetActiveDesign(design_name)
-            if odesign:
-                oproject.CopyDesign(design_name)
-                if not target_project:
-                    oproject.Paste()
+    Returns
+    -------
+    str
+
+    """
+    char_set = string.ascii_uppercase + string.digits
+    unique_name = "".join(random.sample(char_set, 6))
+    if name:
+        return name + unique_name
+    else:
+        return "NewObject_" + unique_name
+
+
+@pyaedt_function_handler()
+def _to_boolean(val):
+    """Retrieve the Boolean value of the provided input.
+
+        If the value is a Boolean, return the value.
+        Otherwise check to see if the value is in
+        ["false", "f", "no", "n", "none", "0", "[]", "{}", "" ]
+        and return True if the value is not in the list.
+
+    Parameters
+    ----------
+    val : bool or str
+        Input value to test for True/False condition.
+
+    Returns
+    -------
+    bool
+
+    """
+
+    if val is True or val is False:
+        return val
+
+    false_items = ["false", "f", "no", "n", "none", "0", "[]", "{}", ""]
+
+    return not str(val).strip().lower() in false_items
+
+
+@pyaedt_function_handler()
+def _dim_arg(value, units):
+    """Concatenate a specified units string to a numerical input.
+
+    Parameters
+    ----------
+    value : str or number
+        Valid expression string in the AEDT modeler. For example, ``"5mm"``.
+    units : str
+        Valid units string in the AEDT modeler. For example, ``"mm"``.
+
+    Returns
+    -------
+    str
+
+    """
+    try:
+        val = float(value)
+        if isinstance(value, int):
+            val = value
+        return str(val) + units
+    except:
+        return value
+
+
+@pyaedt_function_handler()
+def _check_installed_version(install_path, long_version):
+    """Check installation folder to determine if it is for specified Ansys EM version.
+
+    Parameters
+    ----------
+    install_path: str
+        Installation folder to check.  For example, ``"C:\\Program Files\\AnsysEM\\v231\\Win64"``.
+    long_version: str
+        Long form of version number.  For example, ``"2023.1"``.
+
+    Returns
+    -------
+    bool
+
+    """
+    product_list_path = os.path.join(install_path, "config", "ProductList.txt")
+    if os.path.isfile(product_list_path):
+        try:
+            with open(product_list_path, "r") as f:
+                install_version = f.readline().strip()[-6:]
+                if install_version == long_version:
                     return True
-                else:
-                    oproject_target = self.odesktop.SetActiveProject(target_project)
-                    if not oproject_target:
-                        oproject_target = self.odesktop.NewProject(target_project)
-                        oproject_target.Paste()
-                        return True
-        return False
+        except:
+            pass
+    return False
 
-    @pyaedt_function_handler()
-    def project_path(self, project_name=None):
-        """Get the path to the project.
 
-        Parameters
-        ----------
-        project_name : str, optional
-            Project name. The default is ``None``, in which case the active
-            project is used.
+def install_with_pip(package_name, package_path=None, upgrade=False, uninstall=False):  # pragma: no cover
+    """Install a new package using pip.
+    This method is useful for installing a package from the AEDT Console without launching the Python environment.
 
-        Returns
-        -------
-        str
-            Path to the project.
+    Parameters
+    ----------
+    package_name : str
+        Name of the package to install.
+    package_path : str, optional
+        Path for the GitHub package to download and install. For example, ``git+https://.....``.
+    upgrade : bool, optional
+        Whether to upgrade the package. The default is ``False``.
+    uninstall : bool, optional
+        Whether to install the package or uninstall the package.
+    """
+    if is_linux and is_ironpython:
+        import subprocessdotnet as subprocess
+    else:
+        import subprocess
+    executable = '"{}"'.format(sys.executable) if is_windows else sys.executable
 
-        """
-        if not project_name:
-            oproject = self.odesktop.GetActiveProject()
+    commands = []
+    if uninstall:
+        commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
+    else:
+        if package_path and upgrade:
+            commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
+            command = [executable, "-m", "pip", "install", package_path]
+        else:
+            command = [executable, "-m", "pip", "install", package_name]
+        if upgrade:
+            command.append("-U")
+
+        commands.append(command)
+    for command in commands:
+        if is_linux:
+            p = subprocess.Popen(command)
         else:
-            oproject = self.odesktop.SetActiveProject(project_name)
-        if oproject:
-            return oproject.GetPath()
-        return None
+            p = subprocess.Popen(" ".join(command))
+        p.wait()
 
-    @pyaedt_function_handler()
-    def design_list(self, project=None):
-        """Get a list of the designs.
 
-        Parameters
-        ----------
-        project : str, optional
-            Project name. The default is ``None``, in which case the active
-            project is used.
+class Help:  # pragma: no cover
+    def __init__(self):
+        self._base_path = "https://aedt.docs.pyansys.com/version/stable"
+        self.browser = "default"
 
-        Returns
-        -------
-        list
-            List of the designs.
-        """
+    def _launch_ur(self, url):
+        import webbrowser
 
-        updateddeslist = []
-        if not project:
-            oproject = self.odesktop.GetActiveProject()
+        if self.browser != "default":
+            webbrowser.get(self.browser).open_new_tab(url)
         else:
-            oproject = self.odesktop.SetActiveProject(project)
-        if oproject:
-            deslist = list(oproject.GetTopDesignList())
-            for el in deslist:
-                m = re.search(r"[^;]+$", el)
-                updateddeslist.append(m.group(0))
-        return updateddeslist
+            webbrowser.open_new_tab(url)
 
-    @pyaedt_function_handler()
-    def design_type(self, project_name=None, design_name=None):
-        """Get the type of a design.
+    def search(self, keywords, app_name=None, search_in_examples_only=False):
+        """Search for one or more keywords.
 
         Parameters
         ----------
-        project_name : str, optional
-            Project name. The default is ``None``, in which case the active
-            project is used.
-        design_name : str, optional
-            Design name. The default is ``None``, in which case the active
-            design is used.
+        keywords : str or list
+        app_name : str, optional
+            Name of a PyAEDT app. For example, ``"Hfss"``, ``"Circuit"``, ``"Icepak"``, or any other available app.
+        search_in_examples_only : bool, optional
+            Whether to search for the one or more keywords only in the PyAEDT examples.
+            The default is ``False``.
+        """
+        if isinstance(keywords, str):
+            keywords = [keywords]
+        if search_in_examples_only:
+            keywords.append("This example")
+        if app_name:
+            keywords.append(app_name)
+        url = self._base_path + "/search.html?q={}".format("+".join(keywords))
+        self._launch_ur(url)
+
+    def getting_started(self):
+        """Open the PyAEDT User guide page."""
+        url = self._base_path + "/User_guide/index.html"
+        self._launch_ur(url)
+
+    def examples(self):
+        """Open the PyAEDT Examples page."""
+        url = self._base_path + "/examples/index.html"
+        self._launch_ur(url)
+
+    def github(self):
+        """Open the PyAEDT GitHub page."""
+        url = "https://github.com/pyansys/pyaedt"
+        self._launch_ur(url)
 
-        Returns
-        -------
-        str
-            Design type.
+    def changelog(self, release=None):
+        """Open the PyAEDT GitHub Changelog for a given release.
+
+        Parameters
+        ----------
+        release : str, optional
+            Release to get the changelog for. For example, ``"0.6.70"``.
         """
-        if not project_name:
-            oproject = self.odesktop.GetActiveProject()
-        else:
-            oproject = self.odesktop.SetActiveProject(project_name)
-        if not oproject:
-            return ""
-        if not design_name:
-            odesign = oproject.GetActiveDesign()
-        else:
-            odesign = oproject.SetActiveDesign(design_name)
-        if odesign:
-            return odesign.GetDesignType()
-        return ""
+        if release is None:
+            from pyaedt import __version__ as release
+        url = "https://github.com/pyansys/pyaedt/releases/tag/v" + release
+        self._launch_ur(url)
+
+    def issues(self):
+        """Open the PyAEDT GitHub Issues page."""
+        url = "https://github.com/pyansys/pyaedt/issues"
+        self._launch_ur(url)
+
+    def ansys_forum(self):
+        """Open the PyAEDT GitHub Issues page."""
+        url = "https://discuss.ansys.com/discussions/tagged/pyaedt"
+        self._launch_ur(url)
+
+    def developer_forum(self):
+        """Open the Discussions page on the Ansys Developer site."""
+        url = "https://developer.ansys.com/"
+        self._launch_ur(url)
+
+
+# class Property(property):
+#
+#     @pyaedt_function_handler()
+#     def getter(self, fget):
+#         """Property getter."""
+#         return self.__class__.__base__(fget, self.fset, self.fdel, self.__doc__)
+#
+#     @pyaedt_function_handler()
+#     def setter(self, fset):
+#         """Property setter."""
+#         return self.__class__.__base__(self.fget, fset, self.fdel, self.__doc__)
+#
+#     @pyaedt_function_handler()
+#     def deleter(self, fdel):
+#         """Property deleter."""
+#         return self.__class__.__base__(self.fget, self.fset, fdel, self.__doc__)
+
+
+class Settings(object):
+    """Manages all PyAEDT environment variables and global settings."""
+
+    def __init__(self):
+        self._enable_logger = True
+        self._enable_desktop_logs = True
+        self._enable_screen_logs = True
+        self._enable_file_logs = True
+        self.pyaedt_server_path = ""
+        self._logger_file_path = None
+        self._logger_formatter = "%(asctime)s:%(destination)s:%(extra)s%(levelname)-8s:%(message)s"
+        self._logger_datefmt = "%Y/%m/%d %H.%M.%S"
+        self._enable_debug_edb_logger = False
+        self._enable_debug_grpc_api_logger = False
+        self._enable_debug_methods_argument_logger = False
+        self._enable_debug_geometry_operator_logger = False
+        self._enable_debug_internal_methods_logger = False
+        self._enable_debug_logger = False
+        self._enable_error_handler = True
+        self._non_graphical = False
+        self._aedt_version = None
+        self.remote_api = False
+        self._use_grpc_api = None
+        self.machine = ""
+        self.port = 0
+        self.formatter = None
+        self.remote_rpc_session = None
+        self.remote_rpc_session_temp_folder = ""
+        self.remote_rpc_service_manager_port = 17878
+        self._project_properties = {}
+        self._project_time_stamp = 0
+        self._disable_bounding_box_sat = False
+        self._force_error_on_missing_project = False
+        self._enable_pandas_output = False
+        self.time_tick = time.time()
+        self._global_log_file_name = "pyaedt_{}.log".format(os.path.split(os.path.expanduser("~"))[-1])
+        self._enable_global_log_file = True
+        self._enable_local_log_file = False
+        self._global_log_file_size = 10
+        self._edb_dll_path = None
+        self._lsf_num_cores = 2
+        self._lsf_ram = 1000
+        self._use_lsf_scheduler = False
+        self._lsf_aedt_command = "ansysedt"
+        self._lsf_timeout = 3600
+        self._lsf_queue = None
+        self._aedt_environment_variables = {
+            "ANS_MESHER_PROC_DUMP_PREPOST_BEND_SM3": "1",
+            "ANSYSEM_FEATURE_SF6694_NON_GRAPHICAL_COMMAND_EXECUTION_ENABLE": "1",
+            "ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE": "1",
+            "ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE": "1",
+            "ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE": "1",
+            "ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE": "1",
+            "ANSYSEM_FEATURE_F545177_ECAD_INTEGRATION_WITH_APHI_ENABLE": "1",
+            "ANSYSEM_FEATURE_F650636_MECH_LAYOUT_COMPONENT_ENABLE": "1",
+        }
+        if is_linux:
+            self._aedt_environment_variables["ANS_NODEPCHECK"] = "1"
+        self._desktop_launch_timeout = 90
+        self._aedt_process_id = None
+        self._is_student = False
+        self._number_of_grpc_api_retries = 3
 
     @property
-    def personallib(self):
-        """PersonalLib directory.
+    def number_of_grpc_api_retries(self):
+        """Number of Grpc API retries. Default is 3.
 
         Returns
         -------
-        str
-            Full absolute path for the ``PersonalLib`` directory.
-
+        int
         """
-        return self.odesktop.GetPersonalLibDirectory()
+        return self._number_of_grpc_api_retries
+
+    @number_of_grpc_api_retries.setter
+    def number_of_grpc_api_retries(self, value):
+        self._number_of_grpc_api_retries = int(value)
 
     @property
-    def userlib(self):
-        """UserLib directory.
+    def aedt_process_id(self):
+        """ID of the desktop process. The default is ``None``.
 
         Returns
         -------
-        str
-            Full absolute path for the ``UserLib`` directory.
-
+        int
         """
-        return self.odesktop.GetUserLibDirectory()
+        return self._aedt_process_id
+
+    @aedt_process_id.setter
+    def aedt_process_id(self, value):
+        self._aedt_process_id = int(value)
 
     @property
-    def syslib(self):
-        """SysLib directory.
+    def is_student(self):
+        """Whether the desktop process is set to the student version. The
+        default is ``False``.
 
         Returns
         -------
-        str
-            Full absolute path for the ``SysLib`` directory.
-
+        bool
         """
-        return self.odesktop.GetLibraryDirectory()
+        return self._is_student
+
+    @is_student.setter
+    def is_student(self, value):
+        self._is_student = value
 
     @property
-    def aedt_version_id(self):
-        """AEDT version.
+    def desktop_launch_timeout(self):
+        """Set the desktop launcher max timeout. Default is ``90`` seconds.
 
         Returns
         -------
-        str
-            Version of AEDT.
-
+        int
         """
-        version = self.odesktop.GetVersion().split(".")
-        v = ".".join([version[0], version[1]])
-        return v
+        return self._desktop_launch_timeout
+
+    @desktop_launch_timeout.setter
+    def desktop_launch_timeout(self, value):
+        self._desktop_launch_timeout = int(value)
 
     @property
-    def src_dir(self):
-        """Python source directory.
+    def aedt_environment_variables(self):
+        """Set environment variables to be set before launching a new aedt session.
+        This includes beta features enablemement.
 
         Returns
         -------
-        str
-            Full absolute path for the ``python`` directory.
-
+        dict
         """
-        return os.path.dirname(os.path.realpath(__file__))
+        return self._aedt_environment_variables
+
+    @aedt_environment_variables.setter
+    def aedt_environment_variables(self, value):
+        self._aedt_environment_variables = value
 
     @property
-    def pyaedt_dir(self):
-        """PyAEDT directory.
+    def lsf_queue(self):
+        """LSF queue name. This attribute is valid only on Linux
+        systems running LSF Scheduler."""
+        return self._lsf_queue
+
+    @lsf_queue.setter
+    def lsf_queue(self, value):
+        self._lsf_queue = value
 
-        Returns
-        -------
-        str
-           Full absolute path for the ``pyaedt`` directory.
+    @property
+    def use_lsf_scheduler(self):
+        """Whether to use LSF Scheduler. This attribute is valid only on Linux
+        systems running LSF Scheduler."""
+        return self._use_lsf_scheduler
+
+    @use_lsf_scheduler.setter
+    def use_lsf_scheduler(self, value):
+        self._use_lsf_scheduler = value
 
-        """
-        return os.path.realpath(os.path.join(self.src_dir, ".."))
+    @property
+    def lsf_aedt_command(self):
+        """Get or set the ``ansysedt`` command to launch. The default is ``"ansysedt"``.
+        This attribute is valid only on Linux systems running LSF Scheduler."""
+        return self._lsf_aedt_command
+
+    @lsf_aedt_command.setter
+    def lsf_aedt_command(self, value):
+        self._lsf_aedt_command = value
 
-    def _exception(self, ex_value, tb_data):
-        """Write the trace stack to AEDT when a Python error occurs.
+    @property
+    def lsf_num_cores(self):
+        """Get or set the number of LSF cores. This attribute is valid only
+        on Linux systems running LSF Scheduler."""
+        return self._lsf_num_cores
+
+    @lsf_num_cores.setter
+    def lsf_num_cores(self, value):
+        self._lsf_num_cores = int(value)
 
-        Parameters
-        ----------
-        ex_value : str
-            Type of the exception.
-        tb_data : str
-            Traceback data.
+    @property
+    def lsf_ram(self):
+        """Get or set the RAM allocated for the LSF job. This attribute is valid
+        only on Linux systems running LSF Scheduler."""
+        return self._lsf_ram
+
+    @lsf_ram.setter
+    def lsf_ram(self, value):
+        self._lsf_ram = int(value)
+
+    @property
+    def lsf_timeout(self):
+        """Get or set the timeout for starting the interactive session. The default is ``3600`` seconds."""
+        return self._lsf_timeout
+
+    @lsf_timeout.setter
+    def lsf_timeout(self, value):
+        self._lsf_timeout = int(value)
+
+    @property
+    def aedt_version(self):
+        """Get and set the aedt version.
+        It disables the sat bounding box for AEDT version > 2022.2.
 
         Returns
         -------
         str
-            Type of the exception.
-
+            Aedt version in the form ``"2023.x"``.
         """
-        tb_trace = traceback.format_tb(tb_data)
-        tblist = tb_trace[0].split("\n")
-        self.logger.error(str(ex_value))
-        for el in tblist:
-            self.logger.error(el)
-
-        return str(ex_value)
+        return self._aedt_version
 
-    @pyaedt_function_handler()
-    def release_desktop(self, close_projects=True, close_on_exit=True):
-        """Release AEDT.
+    @aedt_version.setter
+    def aedt_version(self, value):
+        self._aedt_version = value
+        if self._aedt_version >= "2023.1":
+            self.disable_bounding_box_sat = True
 
-        Parameters
-        ----------
-        close_projects : bool, optional
-            Whether to close the AEDT projects that are open in the session.
-            The default is ``True``.
-        close_on_exit : bool, optional
-            Whether to close the active AEDT session on exiting AEDT.
-            The default is ``True``.
+    @property
+    def edb_dll_path(self):
+        """Get/Set an optional path for Edb Dll.
 
         Returns
         -------
         bool
-            ``True`` when successful, ``False`` when failed.
+        """
+        return self._edb_dll_path
 
-        Examples
-        --------
-        >>> import pyaedt
-        >>> desktop = pyaedt.Desktop("2021.2")
-        PyAEDT INFO: pyaedt v...
-        PyAEDT INFO: Python version ...
-        >>> desktop.release_desktop(close_projects=False, close_on_exit=False) # doctest: +SKIP
-
-        """
-        result = release_desktop(close_projects, close_on_exit)
-        props = [a for a in dir(self) if not a.startswith("__")]
-        for a in props:
-            self.__dict__.pop(a, None)
-        dicts = [self, sys.modules["__main__"]]
-        for dict_to_clean in dicts:
-            props = [a for a in dir(dict_to_clean) if "win32com" in str(type(dict_to_clean.__dict__.get(a, None)))]
-            for a in props:
-                dict_to_clean.__dict__[a] = None
-
-        gc.collect()
-        self.odesktop = None
-        return result
+    @edb_dll_path.setter
+    def edb_dll_path(self, value):
+        if os.path.exists(value):
+            self._edb_dll_path = value
 
-    def close_desktop(self):
-        """Close all projects and shut down AEDT.
+    @property
+    def global_log_file_size(self):
+        """Get/Set the global pyaedt log file size in Mbytes. The default value is ``10``.
 
         Returns
         -------
         bool
-            ``True`` when successful, ``False`` when failed.
-
-        Examples
-        --------
-        >>> import pyaedt
-        >>> desktop = pyaedt.Desktop("2021.2")
-        PyAEDT INFO: pyaedt v...
-        PyAEDT INFO: Python version ...
-        >>> desktop.close_desktop() # doctest: +SKIP
-
         """
-        return self.release_desktop(close_projects=True, close_on_exit=True)
+        return self._global_log_file_size
 
-    def enable_autosave(self):
-        """Enable the autosave option.
+    @global_log_file_size.setter
+    def global_log_file_size(self, value):
+        self._global_log_file_size = value
 
-        Examples
-        --------
-        >>> import pyaedt
-        >>> desktop = pyaedt.Desktop("2021.2")
-        PyAEDT INFO: pyaedt v...
-        PyAEDT INFO: Python version ...
-        >>> desktop.enable_autosave()
+    @property
+    def enable_global_log_file(self):
+        """Enable/Disable the global pyaedt log file logging in global temp folder. Default is `True`.
 
+        Returns
+        -------
+        bool
         """
-        self._main.oDesktop.EnableAutoSave(True)
+        return self._enable_global_log_file
 
-    def disable_autosave(self):
-        """Disable the autosave option.
+    @enable_global_log_file.setter
+    def enable_global_log_file(self, value):
+        self._enable_global_log_file = value
 
-        Examples
-        --------
-        >>> import pyaedt
-        >>> desktop = pyaedt.Desktop("2021.2")
-        PyAEDT INFO: pyaedt v...
-        PyAEDT INFO: Python version ...
-        >>> desktop.disable_autosave()
+    @property
+    def enable_local_log_file(self):
+        """Enable/Disable the local pyaedt log file logging in projectname.pyaedt project folder. Default is `True`.
 
+        Returns
+        -------
+        bool
         """
-        self._main.oDesktop.EnableAutoSave(False)
+        return self._enable_local_log_file
 
-    def change_license_type(self, license_type="Pool"):
-        """Change the license type.
+    @enable_local_log_file.setter
+    def enable_local_log_file(self, value):
+        self._enable_local_log_file = value
 
-        Parameters
-        ----------
-        license_type : str, optional
-            Type of the license. The options are ``"Pack"`` and ``"Pool"``.
-            The default is ``"Pool"``.
+    @property
+    def global_log_file_name(self):
+        """Get/Set the global pyaedt log file path. Default is pyaedt_username.log.
 
         Returns
         -------
-        bool
-           ``True``.
-
-            .. note::
-               Because of an API limitation, this method returns ``True`` even when the key is wrong.
-
+        str
         """
-        try:
-            self._main.oDesktop.SetRegistryString("Desktop/Settings/ProjectOptions/HPCLicenseType", license_type)
-            return True
-        except:
-            return False
+        return self._global_log_file_name
 
-    def change_registry_key(self, key_full_name, key_value):
-        """Change an AEDT registry key to a new value.
+    @global_log_file_name.setter
+    def global_log_file_name(self, value):
+        self._global_log_file_name = value
 
-        Parameters
-        ----------
-        key_full_name : str
-            Full name of the AEDT registry key.
-        key_value : str, int
-            Value for the AEDT registry key.
+    @property
+    def enable_pandas_output(self):
+        """
+        Set/Get a flag to use Pandas to export dict and lists. This applies to Solution data output.
+        If ``True`` the property or method will return a pandas object in CPython environment.
+        Default is ``False``.
 
         Returns
         -------
         bool
-            ``True`` when successful, ``False`` when failed.
         """
-        if isinstance(key_value, str):
-            try:
-                self._main.oDesktop.SetRegistryString(key_full_name, key_value)
-                self.logger.info("Key %s correctly changed.", key_full_name)
-                return True
-            except:
-                self.logger.warning("Error setting up Key %s.", key_full_name)
-                return False
-        elif isinstance(key_value, int):
-            try:
-                self._main.oDesktop.SetRegistryInt(key_full_name, key_value)
-                self.logger.info("Key %s correctly changed.", key_full_name)
-                return True
-            except:
-                self.logger.warning("Error setting up Key %s.", key_full_name)
-                return False
-        else:
-            self.logger.warning("Key value must be an integer or string.")
-            return False
+        return self._enable_pandas_output
 
-    def change_active_dso_config_name(self, product_name="HFSS", config_name="Local"):
-        """Change a specific registry key to a new value.
+    @enable_pandas_output.setter
+    def enable_pandas_output(self, val):
+        self._enable_pandas_output = val
 
-        Parameters
-        ----------
-        product_name : str, optional
-            Name of the tool to apply the active configuration to. The default is
-            ``"HFSS"``.
-        config_name : str, optional
-            Name of the configuration to apply. The default is ``"Local"``.
+    @property
+    def enable_debug_methods_argument_logger(self):
+        """
+        Set/Get a flag to plot methods argument in debug logger.
+        Default is ``False``.
 
         Returns
         -------
         bool
-            ``True`` when successful, ``False`` when failed.
-
         """
-        try:
-            self.change_registry_key("Desktop/ActiveDSOConfigurations/{}".format(product_name), config_name)
-            self.logger.info("Configuration Changed correctly to %s for %s.", config_name, product_name)
-            return True
-        except:
-            self.logger.warning("Error Setting Up Configuration %s for %s.", config_name, product_name)
-            return False
-
-    def change_registry_from_file(self, registry_file, make_active=True):
-        """Apply desktop registry settings from an ACF file.
+        return self._enable_debug_methods_argument_logger
 
-        One way to get an ACF file is to export a configuration from the AEDT UI and then edit and reuse it.
+    @enable_debug_methods_argument_logger.setter
+    def enable_debug_methods_argument_logger(self, val):
+        self._enable_debug_methods_argument_logger = val
 
-        Parameters
-        ----------
-        registry_file : str
-            Full path to the ACF file.
-        make_active : bool, optional
-            Whether to set the imported configuration as active. The default is ``True``.
+    @property
+    def force_error_on_missing_project(self):
+        """Set/Get a flag to check project path.
+        If ``True`` when passing a project path, the project has to exist otherwise it will raise an error.
+        Default is ``False``.
 
         Returns
         -------
         bool
-            ``True`` when successful, ``False`` when failed.
         """
-        try:
-            self._main.oDesktop.SetRegistryFromFile(registry_file)
-            if make_active:
-                with open(registry_file, "r") as f:
-                    for line in f:
-                        stripped_line = line.strip()
-                        if "ConfigName" in stripped_line:
-                            config_name = stripped_line.split("=")
-                        elif "DesignType" in stripped_line:
-                            design_type = stripped_line.split("=")
-                            break
-                    if design_type and config_name:
-                        self.change_registry_key(design_type[1], config_name[1])
-            return True
-        except:
-            return False
+        return self._force_error_on_missing_project
 
-    @pyaedt_function_handler()
-    def get_available_toolkits(self):
-        """Get toolkit ready for installation.
+    @force_error_on_missing_project.setter
+    def force_error_on_missing_project(self, val):
+        self._force_error_on_missing_project = val
+
+    @property
+    def disable_bounding_box_sat(self):
+        """Set/Get Bounding Box Sat enablement.
 
         Returns
         -------
-        list
-            List of toolkit names.
+        bool
         """
-        from pyaedt.misc.install_extra_toolkits import available_toolkits
-
-        return list(available_toolkits.keys())
+        return self._disable_bounding_box_sat
 
-    @pyaedt_function_handler()
-    def add_custom_toolkit(self, toolkit_name):  # pragma: no cover
-        """Add toolkit to AEDT Automation Tab.
+    @disable_bounding_box_sat.setter
+    def disable_bounding_box_sat(self, val):
+        self._disable_bounding_box_sat = val
 
-        Parameters
-        ----------
-        toolkit_name : str
-            Name of toolkit to add.
+    @property
+    def use_grpc_api(self):
+        """Set/Get 20222R2 GPRC API usage or Legacy COM Objectr.
 
         Returns
         -------
         bool
         """
-        from pyaedt.misc.install_extra_toolkits import available_toolkits
-        from pyaedt.misc.install_extra_toolkits import write_toolkit_config
-
-        toolkit = available_toolkits[toolkit_name]
-        toolkit_name = toolkit_name.replace("_", "")
-
-        def install(package_path, package_name=None):
-            executable = '"{}"'.format(sys.executable) if is_windows else sys.executable
-
-            commands = []
-            if package_path.startswith("git") and package_name:
-                commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
-
-            commands.append([executable, "-m", "pip", "install", "--upgrade", package_path])
-
-            if self.aedt_version_id == "2023.1" and is_windows and "AnsysEM" in sys.base_prefix:
-                commands.append([executable, "-m", "pip", "uninstall", "--yes", "pywin32"])
+        return self._use_grpc_api
 
-            for command in commands:
-                if is_linux:
-                    p = subprocess.Popen(command)
-                else:
-                    p = subprocess.Popen(" ".join(command))
-                p.wait()
-
-        install(toolkit["pip"], toolkit.get("package_name", None))
-        import site
-
-        packages = site.getsitepackages()
-        full_path = None
-        for pkg in packages:
-            if os.path.exists(os.path.join(pkg, toolkit["toolkit_script"])):
-                full_path = os.path.join(pkg, toolkit["toolkit_script"])
-                break
-        if not full_path:
-            raise FileNotFoundError("Error finding the package.")
-        product = toolkit["installation_path"]
-        toolkit_dir = os.path.join(self.personallib, "Toolkits")
-        aedt_version = self.aedt_version_id
-        tool_dir = os.path.join(toolkit_dir, product, toolkit_name)
-        lib_dir = os.path.join(tool_dir, "Lib")
-        toolkit_rel_lib_dir = os.path.relpath(lib_dir, tool_dir)
-        if is_linux and aedt_version <= "2023.1":
-            toolkit_rel_lib_dir = os.path.join("Lib", toolkit_name)
-            lib_dir = os.path.join(toolkit_dir, toolkit_rel_lib_dir)
-            toolkit_rel_lib_dir = "../../" + toolkit_rel_lib_dir
-        os.makedirs(lib_dir, exist_ok=True)
-        os.makedirs(tool_dir, exist_ok=True)
-        files_to_copy = ["Run_PyAEDT_Toolkit_Script"]
-        executable_version_agnostic = sys.executable
-        for file_name in files_to_copy:
-            src = os.path.join(pathname, "misc", file_name + ".py_build")
-            dst = os.path.join(tool_dir, file_name.replace("_", " ") + ".py")
-            if not os.path.isfile(src):
-                raise FileNotFoundError("File not found: {}".format(src))
-            with open(src, "r") as build_file:
-                with open(dst, "w") as out_file:
-                    self.logger.info("Building to " + dst)
-                    build_file_data = build_file.read()
-                    build_file_data = (
-                        build_file_data.replace("##TOOLKIT_REL_LIB_DIR##", toolkit_rel_lib_dir)
-                        .replace("##PYTHON_EXE##", executable_version_agnostic)
-                        .replace("##PYTHON_SCRIPT##", full_path)
-                    )
-                    build_file_data = build_file_data.replace(" % version", "")
-                    out_file.write(build_file_data)
-        if aedt_version >= "2023.2":
-            write_toolkit_config(os.path.join(toolkit_dir, product), lib_dir, toolkit_name, toolkit=toolkit)
-        self.logger.info("{} toolkit installed.".format(toolkit_name))
+    @use_grpc_api.setter
+    def use_grpc_api(self, val):
+        """Set/Get 20222R2 GPRC API usage or Legacy COM Objectr."""
+        self._use_grpc_api = val
 
-    @pyaedt_function_handler()
-    def submit_job(
-        self,
-        project_file,
-        clustername,
-        aedt_full_exe_path=None,
-        numnodes=1,
-        numcores=32,
-        wait_for_license=True,
-        setting_file=None,
-    ):  # pragma: no cover
-        """Submit a job to be solved on a cluster.
+    @property
+    def logger(self):
+        """Get the active logger."""
+        try:
+            return logging.getLogger("Global")
+        except:
+            return logging.getLogger(__name__)
 
-        Parameters
-        ----------
-        project : str
-            Full path to the project.
-        clustername : str
-            Name of the cluster to submit the job to.
-        aedt_full_exe_path : str, optional
-            Full path to the AEDT executable file. The default is ``None``, in which
-            case ``"/clustername/AnsysEM/AnsysEM2x.x/Win64/ansysedt.exe"`` is used.
-        numnodes : int, optional
-            Number of nodes. The default is ``1``.
-        numcores : int, optional
-            Number of cores. The default is ``32``.
-        wait_for_license : bool, optional
-             Whether to wait for the license to be validated. The default is ``True``.
-        setting_file : str, optional
-            Name of the file to use as a template. The default value is ``None``.
+    @property
+    def non_graphical(self):
+        """Get the value for the non-graphical flag."""
+        return self._non_graphical
+
+    @non_graphical.setter
+    def non_graphical(self, val):
+        self._non_graphical = val
 
-        Returns
-        -------
-        int
-            ID of the job.
+    @property
+    def enable_error_handler(self):
+        """Return the content for the environment variable."""
+        return self._enable_error_handler
+
+    @enable_error_handler.setter
+    def enable_error_handler(self, val):
+        self._enable_error_handler = val
 
-        References
-        ----------
+    @property
+    def enable_desktop_logs(self):
+        """Get the content for the environment variable."""
+        return False if self.non_graphical else self._enable_desktop_logs
+
+    @enable_desktop_logs.setter
+    def enable_desktop_logs(self, val):
+        self._enable_desktop_logs = val
 
-        >>> oDesktop.SubmitJob
-        """
+    @property
+    def enable_screen_logs(self):
+        """Get the content for the environment variable."""
+        return self._enable_screen_logs
+
+    @enable_screen_logs.setter
+    def enable_screen_logs(self, val):
+        self._enable_screen_logs = val
 
-        project_path = os.path.dirname(project_file)
-        project_name = os.path.basename(project_file).split(".")[0]
-        if not aedt_full_exe_path:
-            version = self.odesktop.GetVersion()[2:6]
-            if version >= "22.2":
-                version_name = "v" + version.replace(".", "")
-            else:
-                version_name = "AnsysEM" + version
-            if os.path.exists(r"\\" + clustername + r"\AnsysEM\{}\Win64\ansysedt.exe".format(version_name)):
-                aedt_full_exe_path = (
-                    r"\\\\\\\\" + clustername + r"\\\\AnsysEM\\\\{}\\\\Win64\\\\ansysedt.exe".format(version_name)
-                )
-            elif os.path.exists(r"\\" + clustername + r"\AnsysEM\{}\Linux64\ansysedt".format(version_name)):
-                aedt_full_exe_path = (
-                    r"\\\\\\\\" + clustername + r"\\\\AnsysEM\\\\{}\\\\Linux64\\\\ansysedt".format(version_name)
-                )
-            else:
-                self.logger.error("AEDT shared path does not exist. Provide a full path.")
-                return False
-        else:
-            if not os.path.exists(aedt_full_exe_path):
-                self.logger.error("AEDT shared path does not exist. Provide a full path.")
-                return False
-            aedt_full_exe_path.replace("\\", "\\\\")
-        if project_name in self.project_list:
-            self.odesktop.CloseProject(project_name)
-        path_file = os.path.dirname(__file__)
-        destination_reg = os.path.join(project_path, "Job_settings.areg")
-        if not setting_file:
-            setting_file = os.path.join(path_file, "misc", "Job_Settings.areg")
-        shutil.copy(setting_file, destination_reg)
-
-        f1 = open_file(destination_reg, "w")
-        with open_file(setting_file) as f:
-            lines = f.readlines()
-            for line in lines:
-                if "\\	$begin" == line[:8]:
-                    lin = "\\	$begin \\'{}\\'\\\n".format(clustername)
-                    f1.write(lin)
-                elif "\\	$end" == line[:6]:
-                    lin = "\\	$end \\'{}\\'\\\n".format(clustername)
-                    f1.write(lin)
-                elif "NumCores" in line:
-                    lin = "\\	\\	\\	\\	NumCores={}\\\n".format(numcores)
-                    f1.write(lin)
-                elif "NumNodes=1" in line:
-                    lin = "\\	\\	\\	\\	NumNodes={}\\\n".format(numnodes)
-                    f1.write(lin)
-                elif "ProductPath" in line:
-                    lin = "\\	\\	ProductPath =\\'{}\\'\\\n".format(aedt_full_exe_path)
-                    f1.write(lin)
-                elif "WaitForLicense" in line:
-                    lin = "\\	\\	WaitForLicense={}\\\n".format(str(wait_for_license).lower())
-                    f1.write(lin)
-                else:
-                    f1.write(line)
-        f1.close()
-        return self.odesktop.SubmitJob(os.path.join(project_path, "Job_settings.areg"), project_file)
+    @property
+    def pyaedt_server_path(self):
+        """Get the content for the environment variable."""
+        return os.getenv("PYAEDT_SERVER_AEDT_PATH", "")
+
+    @pyaedt_server_path.setter
+    def pyaedt_server_path(self, val):
+        os.environ["PYAEDT_SERVER_AEDT_PATH"] = str(val)
 
     @property
-    def are_there_simulations_running(self):
-        """Check if there are simulation running.
+    def enable_file_logs(self):
+        """Get the content for the environment variable."""
+        return self._enable_file_logs
+
+    @enable_file_logs.setter
+    def enable_file_logs(self, val):
+        self._enable_file_logs = val
 
-        .. note::
-           It works only for AEDT >= ``"2023.2"``.
+    @property
+    def enable_logger(self):
+        """Return the Environment Variable Content."""
+        return self._enable_logger
+
+    @enable_logger.setter
+    def enable_logger(self, val):
+        self._enable_logger = val
 
-        Returns
-        -------
-        float
+    @property
+    def logger_file_path(self):
+        """Return the Environment Variable Content."""
+        return self._logger_file_path
+
+    @logger_file_path.setter
+    def logger_file_path(self, val):
+        self._logger_file_path = val
 
-        """
-        if self.aedt_version_id > "2023.1":
-            return self.odesktop.AreThereSimulationsRunning()
-        else:
-            self.logger.error("It works only for AEDT >= `2023.2`.")
-        return False
+    @property
+    def logger_formatter(self):
+        """Return the Environment Variable Content."""
+        return self._logger_formatter
+
+    @logger_formatter.setter
+    def logger_formatter(self, val):
+        self._logger_formatter = val
 
-    @pyaedt_function_handler()
-    def get_monitor_data(self):
-        """Check and get monitor data of an existing analysis.
+    @property
+    def logger_datefmt(self):
+        """Return the Environment Variable Content."""
+        return self._logger_datefmt
+
+    @logger_datefmt.setter
+    def logger_datefmt(self, val):
+        self._logger_datefmt = val
 
-        .. note::
-           It works only for AEDT >= ``"2023.2"``.
+    @property
+    def enable_debug_edb_logger(self):
+        """Enable or disable Logger for any EDB API method."""
+        return self._enable_debug_edb_logger
 
-        Returns
-        -------
-        dict
+    @property
+    def enable_debug_grpc_api_logger(self):
+        """Enable or disable Logger for any grpc API method."""
+        return self._enable_debug_grpc_api_logger
+
+    @enable_debug_grpc_api_logger.setter
+    def enable_debug_grpc_api_logger(self, val):
+        self._enable_debug_grpc_api_logger = val
+
+    @enable_debug_edb_logger.setter
+    def enable_debug_edb_logger(self, val):
+        self._enable_debug_edb_logger = val
 
-        """
-        counts = {"profile": 0, "convergence": 0, "sweptvar": 0, "progress": 0, "variations": 0, "displaytype": 0}
-        if self.are_there_simulations_running:
-            reqstr = " ".join(["%s %d 0" % (t, counts[t]) for t in counts])
-            data = self.odesktop.GetMonitorData(reqstr)
-            all_lines = (line.strip() for line in data.split("\n"))
-            for line in all_lines:
-                if line.startswith("$begin"):
-                    btype = line.split()[1].strip("'")
-                    if btype == "MonitoringProfileMsg":
-                        counts["profile"] += 1
-                    elif btype == "MonConvData":
-                        counts["convergence"] += 1
-                    elif btype == "MonGenericVariations":
-                        pass
-                    elif btype == "MapMonGraphicalProgMsg":
-                        pass
-                    elif btype == "MonitoringSweptVariableMsg":
-                        counts["sweptvar"] += 1
-            return counts
-        return counts
+    @property
+    def enable_debug_geometry_operator_logger(self):
+        """Return the Environment Variable Content."""
+        return self._enable_debug_geometry_operator_logger
+
+    @enable_debug_geometry_operator_logger.setter
+    def enable_debug_geometry_operator_logger(self, val):
+        self._enable_debug_geometry_operator_logger = val
 
-    @pyaedt_function_handler()
-    def stop_simulations(self, clean_stop=True):
-        """Check if there are simulation running and stops them.
+    @property
+    def enable_debug_internal_methods_logger(self):
+        """Return the Environment Variable Content."""
+        return self._enable_debug_internal_methods_logger
+
+    @enable_debug_internal_methods_logger.setter
+    def enable_debug_internal_methods_logger(self, val):
+        self._enable_debug_internal_methods_logger = val
 
-        .. note::
-           It works only for AEDT >= ``"2023.2"``.
+    @property
+    def enable_debug_logger(self):
+        """Return the Environment Variable Content."""
+        return self._enable_debug_logger
+
+    @enable_debug_logger.setter
+    def enable_debug_logger(self, val):
+        self._enable_debug_logger = val
 
-        Returns
-        -------
-        str
 
-        """
-        if self.aedt_version_id > "2023.1":
-            return self.odesktop.StopSimulations(clean_stop)
-        else:
-            self.logger.error("It works only for AEDT >= `2023.2`.")
-        return False
+# property = Property
+settings = Settings()
+online_help = Help()
```

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/downloads.py` & `pyaedt-0.6.85/pyaedt/downloads.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Download example datasets from https://github.com/pyansys/example-data"""
-import ast
 import os
 import shutil
 import tempfile
 import zipfile
 
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
@@ -12,15 +11,15 @@
 
 if is_ironpython:
     import urllib
 else:
     import urllib.request
 
 tmpfold = tempfile.gettempdir()
-EXAMPLE_REPO = "https://github.com/pyansys/example-data/raw/master/pyaedt/"
+EXAMPLE_REPO = "https://github.com/ansys/example-data/raw/master/"
 EXAMPLES_PATH = os.path.join(tmpfold, "PyAEDTExamples")
 
 
 def delete_downloads():
     """Delete all downloaded examples to free space or update the files."""
     shutil.rmtree(EXAMPLES_PATH, ignore_errors=True)
 
@@ -28,23 +27,23 @@
 def _get_file_url(directory, filename=None):
     if not filename:
         return EXAMPLE_REPO + "/".join([directory])
     else:
         return EXAMPLE_REPO + "/".join([directory, filename])
 
 
-def _retrieve_file(url, filename, directory, destination=None):
+def _retrieve_file(url, filename, directory, destination=None, local_paths=[]):
     """Download a file from a url"""
     # First check if file has already been downloaded
     if not destination:
         destination = EXAMPLES_PATH
     local_path = os.path.join(destination, directory, os.path.basename(filename))
     local_path_no_zip = local_path.replace(".zip", "")
     if os.path.isfile(local_path_no_zip) or os.path.isdir(local_path_no_zip):
-        return local_path_no_zip
+        local_paths.append(local_path_no_zip)
 
     # grab the correct url retriever
     if not is_ironpython:
         urlretrieve = urllib.request.urlretrieve
     destination_dir = os.path.join(destination, directory)
     if not os.path.isdir(destination_dir):
         os.makedirs(destination_dir)
@@ -79,65 +78,75 @@
                 f.write('url = r"{}"\n'.format(url))
                 f.write('local_path = r"{}"\n'.format(local_path))
                 f.write("urlretrieve(url, local_path)\n")
             print(command)
             os.system(command)
     else:
         _, resp = urlretrieve(url, local_path)
-    return local_path
+    local_paths.append(local_path)
 
 
-def _retrieve_folder(url, directory, destination=None):
+def _retrieve_folder(url, directory, destination=None, local_paths=[]):
     """Download a folder from a url"""
     # First check if folder exists
+    import json
+    import re
+
     if not destination:
         destination = EXAMPLES_PATH
-    local_path = os.path.join(destination, directory)
-    # if os.path.isdir(local_path):
-    #     return local_path
+    if directory.startswith("pyaedt/"):
+        local_path = os.path.join(destination, directory[7:])
+    else:
+        local_path = os.path.join(destination, directory)
 
     if is_ironpython:
         return False
-
-    with urllib.request.urlopen(url) as response:  # nosec
+    _get_dir = _get_file_url(directory)
+    with urllib.request.urlopen(_get_dir) as response:  # nosec
         data = response.read().decode("utf-8").split("\n")
 
-    if not os.path.isdir(destination):
+    if not os.path.isdir(local_path):
         try:
-            os.mkdir(destination)
+            os.mkdir(local_path)
         except FileNotFoundError:
             os.makedirs(local_path)
 
-    for line in data:
-        if "js-navigation-open Link--primary" in line:
-            name = line[line.find("title=") + len("title=") : line.rfind(" data-pjax")]
-            if "data-turbo-frame" in name:
-                name = line[line.find("title=") + len("title=") : line.rfind(" data-turbo-frame")]
-            filename = ast.literal_eval(name)
-            if ".aedb" in filename:
-                _download_file(directory + "/" + filename, "edb.def", destination)
+    try:
+        tree = [i for i in data if '"payload"' in i][0]
+        b = re.search(r'>({"payload".+)</script>', tree)
+        itemsfromjson = json.loads(b.group(1))
+        items = itemsfromjson["payload"]["tree"]["items"]
+        for item in items:
+            if item["contentType"] == "directory":
+                _retrieve_folder(url, item["path"], destination, local_paths)
             else:
-                _download_file(directory, filename, destination)
-    return local_path
+                dir_folder = os.path.split(item["path"])
+                _download_file(dir_folder[0], dir_folder[1], destination, local_paths)
+    except:
+        return False
 
 
-def _download_file(directory, filename=None, destination=None):
+def _download_file(directory, filename=None, destination=None, local_paths=[]):
     if not filename:
-        url = _get_file_url(directory)
-        local_path = _retrieve_folder(url, directory, destination)
+        if not directory.startswith("pyaedt/"):
+            directory = "pyaedt/" + directory
+        _retrieve_folder(EXAMPLE_REPO, directory, destination, local_paths)
     else:
-        url = _get_file_url(directory, filename)
-        local_path = _retrieve_file(url, filename, directory, destination)
+        if directory.startswith("pyaedt/"):
+            url = _get_file_url(directory, filename)
+            directory = directory[7:]
+        else:
+            url = _get_file_url("pyaedt/" + directory, filename)
+        _retrieve_file(url, filename, directory, destination, local_paths)
     if settings.remote_rpc_session:
-        remote_path = os.path.join(settings.remote_rpc_session_temp_folder, os.path.split(local_path)[-1])
+        remote_path = os.path.join(settings.remote_rpc_session_temp_folder, os.path.split(local_paths[-1])[-1])
         if not settings.remote_rpc_session.filemanager.pathexists(settings.remote_rpc_session_temp_folder):
             settings.remote_rpc_session.filemanager.makedirs(settings.remote_rpc_session_temp_folder)
-        settings.remote_rpc_session.filemanager.upload(local_path, remote_path)
-        return remote_path
-    return local_path
+        settings.remote_rpc_session.filemanager.upload(local_paths[-1], remote_path)
+        local_paths[-1] = remote_path
 
 
 ###############################################################################
 # front-facing functions
 
 
 def download_aedb(destination=None):
@@ -160,17 +169,18 @@
     --------
     Download an example result file and return the path of the file.
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_aedb()
     >>> path
     'C:/Users/user/AppData/local/temp/Galileo.aedb'
     """
-    _download_file("edb/Galileo.aedb", "GRM32ER72A225KA35_25C_0V.sp", destination)
-
-    return _download_file("edb/Galileo.aedb", "edb.def", destination)
+    local_paths = []
+    _download_file("pyaedt/edb/Galileo.aedb", "GRM32ER72A225KA35_25C_0V.sp", destination, local_paths)
+    _download_file("pyaedt/edb/Galileo.aedb", "edb.def", destination, local_paths)
+    return local_paths
 
 
 def download_edb_merge_utility(force_download=False, destination=None):
     """Download an example of WPF Project which allows to merge 2aedb files.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -197,19 +207,21 @@
     """
     if not destination:
         destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, "wpf_edb_merge")
         if os.path.exists(local_path):
             shutil.rmtree(local_path, ignore_errors=True)
-    _download_file("wpf_edb_merge/board.aedb", "edb.def", destination)
-    _download_file("wpf_edb_merge/package.aedb", "edb.def", destination)
-    _download_file("wpf_edb_merge", "merge_wizard_settings.json", destination)
+    local_paths = []
+    _download_file("pyaedt/wpf_edb_merge/board.aedb", "edb.def", destination, local_paths)
+    _download_file("pyaedt/wpf_edb_merge/package.aedb", "edb.def", destination, local_paths)
+    _download_file("pyaedt/wpf_edb_merge", "merge_wizard_settings.json", destination, local_paths)
 
-    return _download_file("wpf_edb_merge", "merge_wizard.py", destination)
+    _download_file("pyaedt/wpf_edb_merge", "merge_wizard.py", destination, local_paths)
+    return local_paths[0]
 
 
 def download_netlist(destination=None):
     """Download an example of netlist File and return the def path.
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
 
@@ -228,16 +240,17 @@
     Download an example result file and return the path of the file.
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_netlist()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/netlist_small.cir'
     """
-
-    return _download_file("netlist", "netlist_small.cir", destination)
+    local_paths = []
+    _download_file("pyaedt/netlist", "netlist_small.cir", destination, local_paths)
+    return local_paths[0]
 
 
 def download_antenna_array(destination=None):
     """Download an example of Antenna Array and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -259,15 +272,17 @@
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_antenna_array()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/FiniteArray_Radome_77GHz_3D_CADDM.aedt'
     """
 
-    return _download_file("array_antenna", "FiniteArray_Radome_77GHz_3D_CADDM.aedt", destination)
+    local_paths = []
+    _download_file("pyaedt/array_antenna", "FiniteArray_Radome_77GHz_3D_CADDM.aedt", destination, local_paths)
+    return local_paths[0]
 
 
 def download_sbr(destination=None):
     """Download an example of SBR+ Array and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -288,15 +303,17 @@
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_antenna_array()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/FiniteArray_Radome_77GHz_3D_CADDM.aedt'
     """
 
-    return _download_file("sbr", "Cassegrain.aedt", destination)
+    local_paths = []
+    _download_file("pyaedt/sbr", "Cassegrain.aedt", destination, local_paths)
+    return local_paths[0]
 
 
 def download_sbr_time(destination=None):
     """Download an example of SBR+ Time domain animation and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -317,15 +334,15 @@
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_sbr_time()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/sbr/poc_scat_small.aedt'
     """
 
-    return _download_file("sbr", "poc_scat_small.aedt", destination)
+    return _download_file("pyaedt/sbr", "poc_scat_small.aedt", destination)
 
 
 def download_icepak(destination=None):
     """Download an example of Icepak Array and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -346,15 +363,15 @@
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_icepak()
     >>> pathavoid
     'C:/Users/user/AppData/local/temp/pyaedtexamples/Graphic_Card.aedt'
     """
 
-    return _download_file("icepak", "Graphics_card.aedt", destination)
+    return _download_file("pyaedt/icepak", "Graphics_card.aedt", destination)
 
 
 def download_icepak_3d_component(destination=None):  # pragma: no cover
     """Download an example of Icepak Array and return the def pathsw.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -376,18 +393,19 @@
     Download an example result file and return the path of the file.
 
     >>> import pyaedt
     >>> path1, path2 = pyaedt.downloads.download_icepak_3d_component()
     >>> path1
     'C:/Users/user/AppData/local/temp/pyaedtexamples/PCBAssembly.aedt',
     """
-    _download_file("icepak_3dcomp//PCBAssembly.aedb", destination=destination)
-    return _download_file("icepak_3dcomp", "PCBAssembly.aedt", destination), _download_file(
-        "icepak_3dcomp", "QFP2.aedt", destination
-    )
+    local_paths = []
+    _download_file("pyaedt/icepak_3dcomp//PCBAssembly.aedb", destination=destination)
+    _download_file("pyaedt/icepak_3dcomp", "PCBAssembly.aedt", destination, local_paths)
+    _download_file("icepak_3dcomp", "QFP2.aedt", destination, local_paths)
+    return local_paths
 
 
 def download_via_wizard(destination=None):
     """Download an example of Hfss Via Wizard and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -408,15 +426,15 @@
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_via_wizard()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/Graphic_Card.aedt'
     """
 
-    return _download_file("via_wizard", "viawizard_vacuum_FR4.aedt", destination)
+    return _download_file("pyaedt/via_wizard", "viawizard_vacuum_FR4.aedt", destination)
 
 
 def download_touchstone(destination=None):
     """Download an example of touchstone File and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -435,15 +453,17 @@
     --------
     Download an example result file and return the path of the file.
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_touchstone()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/ssn_ssn.s6p'
     """
-    return _download_file("touchstone", "SSN_ssn.s6p", destination)
+    local_paths = []
+    _download_file("pyaedt/touchstone", "SSN_ssn.s6p", destination, local_paths)
+    return local_paths
 
 
 def download_sherlock(destination=None):
     """Download an example of sherlock needed files and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -465,19 +485,20 @@
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_sherlock()
     >>> path
     'C:/Users/user/AppData/local/temp/Galileo.aedb'
     """
     if not destination:
         destination = EXAMPLES_PATH
-    _download_file("sherlock", "MaterialExport.csv", destination)
-    _download_file("sherlock", "TutorialBoardPartsList.csv", destination)
-    _download_file("sherlock", "SherlockTutorial.aedt", destination)
-    _download_file("sherlock", "TutorialBoard.stp", destination)
-    _download_file("sherlock/SherlockTutorial.aedb", "edb.def", destination)
+    local_paths = []
+    _download_file("pyaedt/sherlock", "MaterialExport.csv", destination, local_paths)
+    _download_file("pyaedt/sherlock", "TutorialBoardPartsList.csv", destination, local_paths)
+    _download_file("pyaedt/sherlock", "SherlockTutorial.aedt", destination, local_paths)
+    _download_file("pyaedt/sherlock", "TutorialBoard.stp", destination, local_paths)
+    _download_file("pyaedt/sherlock/SherlockTutorial.aedb", "edb.def", destination, local_paths)
 
     return os.path.join(destination, "sherlock")
 
 
 def download_leaf(destination=None):
     """Download an example of Nissan leaf files and return the def path.
 
@@ -501,18 +522,19 @@
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_leaf(r"c:\temp")
     >>> path
     ('C:/temp/BH_Arnold_Magnetics_N30UH_80C.tab', 'C:/temp/BH_Arnold_Magnetics_N30UH_80C.tab')
     """
     if not destination:
         destination = EXAMPLES_PATH
-    file1 = _download_file("nissan", "30DH_20C_smooth.tab", destination)
-    file2 = _download_file("nissan", "BH_Arnold_Magnetics_N30UH_80C.tab", destination)
+    local_paths = []
+    _download_file("pyaedt/nissan", "30DH_20C_smooth.tab", destination, local_paths)
+    _download_file("pyaedt/nissan", "BH_Arnold_Magnetics_N30UH_80C.tab", destination, local_paths)
 
-    return file1, file2
+    return local_paths
 
 
 def download_custom_reports(force_download=False, destination=None):
     """Download an example of CISPR25 with customer reports json template files.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -533,27 +555,22 @@
     --------
     Download an example result file and return the path of the file.
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_custom_reports(force_download=True)
     >>> path
     'C:/Users/user/AppData/local/temp/custom_reports'
     """
-    if not destination:
-        destination = EXAMPLES_PATH
+
     if force_download:
         local_path = os.path.join(destination, "custom_reports")
         if os.path.exists(local_path):
             shutil.rmtree(local_path, ignore_errors=True)
-    _download_file("custom_reports", "CISPR25_Radiated_Emissions_Example22R1.aedtz", destination)
-    _download_file("custom_reports", "EyeDiagram_CISPR_Basic.json", destination)
-    _download_file("custom_reports", "EyeDiagram_CISPR_Custom.json", destination)
-    _download_file("custom_reports", "Spectrum_CISPR_Basic.json", destination)
-    _download_file("custom_reports", "Spectrum_CISPR_Custom.json", destination)
-    _download_file("custom_reports", "Transient_CISPR_Basic.json", destination)
-    _download_file("custom_reports", "Transient_CISPR_Custom.json", destination)
+    download_file("pyaedt/custom_reports")
+    if not destination:
+        destination = EXAMPLES_PATH
     return os.path.join(destination, "custom_reports")
 
 
 def download_3dcomponent(force_download=False, destination=None):
     """Download an example of 3d component array with json template files.
 
     Examples files are downloaded to a persistent cache to avoid
@@ -581,17 +598,15 @@
     """
     if not destination:
         destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, "array_3d_component")
         if os.path.exists(local_path):
             shutil.rmtree(local_path, ignore_errors=True)
-    _download_file("array_3d_component", "Circ_Patch_5GHz.a3dcomp", destination)
-    _download_file("array_3d_component", "Circ_Patch_5GHz_hex.a3dcomp", destination)
-    _download_file("array_3d_component", "array_simple.json", destination)
+    download_file("pyaedt/array_3d_component", destination=destination)
     return os.path.join(destination, "array_3d_component")
 
 
 def download_multiparts(destination=None):
     """Download an example of 3DComponents Multiparts.
 
     Examples files are downloaded to a persistent cache to avoid
@@ -617,15 +632,15 @@
     'C:/Users/user/AppData/local/temp/multiparts/library'
     """
     if not destination:
         destination = EXAMPLES_PATH
     dest_folder = os.path.join(destination, "multiparts")
     if os.path.exists(os.path.join(dest_folder, "library")):
         shutil.rmtree(os.path.join(dest_folder, "library"), ignore_errors=True)
-    _download_file("multiparts", "library.zip", destination)
+    _download_file("pyaedt/multiparts", "library.zip", destination)
     if os.path.exists(os.path.join(destination, "multiparts", "library.zip")):
         unzip(os.path.join(destination, "multiparts", "library.zip"), dest_folder)
     return os.path.join(dest_folder, "library")
 
 
 def download_twin_builder_data(file_name, force_download=False, destination=None):
     """Download a Twin Builder example data file.
@@ -657,15 +672,15 @@
     """
     if not destination:
         destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, os.path.join("twin_builder", file_name))
         if os.path.exists(local_path):
             os.unlink(local_path)
-    _download_file("twin_builder", file_name, destination)
+    _download_file("pyaedt/twin_builder", file_name, destination)
     return os.path.join(destination, "twin_builder")
 
 
 def download_file(directory, filename=None, destination=None):
     """
     Download file from directory.
 
@@ -690,15 +705,21 @@
     Download an example result file and return the path of the file.
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_file("motorcad", "IPM_Vweb_Hairpin.mot")
     >>> path
     'C:/Users/user/AppData/local/temp/PyAEDTExamples/motorcad'
     """
-    local_path = _download_file(directory, filename, destination)
-
-    return local_path
+    local_paths = []
+    _download_file(directory, filename, destination, local_paths)
+    if filename:
+        return list(set(local_paths))[0]
+    else:
+        if not destination:
+            destination = EXAMPLES_PATH
+        destination_dir = os.path.join(destination, directory)
+        return destination_dir
 
 
 def unzip(source_filename, dest_dir):
     with zipfile.ZipFile(source_filename) as zf:
         zf.extractall(dest_dir)
```

### Comparing `pyaedt-0.6.82/pyaedt/edb.py` & `pyaedt-0.6.85/pyaedt/edb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/components.py` & `pyaedt-0.6.85/pyaedt/edb_core/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -799,22 +799,17 @@
         term.SetReferenceTerminal(ref_term)
         if term:
             return term
         return False
 
     @pyaedt_function_handler()
     def create_port_on_component(
-        self,
-        component,
-        net_list,
-        port_type=SourceType.CoaxPort,
-        do_pingroup=True,
-        reference_net="gnd",
+        self, component, net_list, port_type=SourceType.CoaxPort, do_pingroup=True, reference_net="gnd", port_name=None
     ):
-        """Create ports on given component.
+        """Create ports on a component.
 
         Parameters
         ----------
         component : str or  self._pedb.component
             EDB component or str component name.
         net_list : str or list of string.
             List of nets where ports must be created on the component.
@@ -823,14 +818,20 @@
             Type of port to create. ``CoaxPort`` generates solder balls.
             ``CircuitPort`` generates circuit ports on pins belonging to the net list.
         do_pingroup : bool
             True activate pingroup during port creation (only used with combination of CoaxPort),
             False will take the closest reference pin and generate one port per signal pin.
         refnet : string or list of string.
             list of the reference net.
+        port_name : string
+            Port name for overwriting the default port-naming convention,
+            which is ``[component][net][pin]``. The port name must be unique.
+            If a port with the specified name already exists, the
+            default naming convention is used so that port creation does
+            not fail.
 
         Returns
         -------
         double, bool
             Salder ball height vale, ``False`` when failed.
 
         Examples
@@ -876,15 +877,15 @@
                 solder_ball_height = sball_diam / 2
             else:
                 bbox = pad_params[1]
                 sball_diam = min([abs(bbox[2] - bbox[0]), abs(bbox[3] - bbox[1])]) * 0.8
                 solder_ball_height = sball_diam / 2
             self.set_solder_ball(component, solder_ball_height, sball_diam)
             for pin in cmp_pins:
-                self._padstack.create_coax_port(pin)
+                self._padstack.create_coax_port(padstackinstance=pin, name=port_name)
 
         elif port_type == SourceType.CircPort:  # pragma no cover
             ref_pins = [
                 p
                 for p in list(component.LayoutObjs)
                 if int(p.GetObjType()) == 1 and p.GetNet().GetName() in reference_net
             ]
@@ -992,14 +993,56 @@
             temp_distance = pin_position.Distance(ref_pin_position)
             if temp_distance < distance:
                 distance = temp_distance
                 closest_pin = ref_pin
         return closest_pin
 
     @pyaedt_function_handler()
+    def replace_rlc_by_gap_boundaries(self, component=None):
+        """Replace RLC component by RLC gap boundaries. These boundary types are compatible with 3D modeler export.
+        Only 2 pins RLC components are supported in this command.
+
+        Parameters
+        ----------
+        component : str
+            Reference designator of the RLC component.
+
+        Returns
+        -------
+        bool
+        ``True`` when succeed, ``False`` if it failed.
+
+        Examples
+        --------
+        >>> from pyaedt import Edb
+        >>> edb = Edb(edb_file)
+        >>>  for refdes, cmp in edb.components.capacitors.items():
+        >>>     edb.components.replace_rlc_by_gap_boundaries(refdes)
+        >>> edb.save_edb()
+        >>> edb.close_edb()
+        """
+        if not component:  # pragma no cover
+            return False
+        if isinstance(component, str):
+            component = self.instances[component]
+            if not component:  # pragma  no cover
+                self._logger.error("component %s not found.", component)
+                return False
+        component_type = component.edbcomponent.GetComponentType()
+        if (
+            component_type == self._edb.definition.ComponentType.Other
+            or component_type == self._edb.definition.ComponentType.IC
+            or component_type == self._edb.definition.ComponentType.IO
+        ):
+            self._logger.info("Component %s passed to deactivate is not an RLC.", component.refdes)
+            return False
+        component.is_enabled = False
+        return self.add_rlc_boundary(component.refdes, False)
+
+    @pyaedt_function_handler()
     def deactivate_rlc_component(self, component=None, create_circuit_port=False):
         """Deactivate RLC component with a possibility to convert to a circuit port.
 
         Parameters
         ----------
         component : str
             Reference designator of the RLC component.
@@ -1096,14 +1139,88 @@
             neg_pin_term.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.PortBoundary)
             neg_pin_term.SetIsCircuitPort(True)
             pos_pin_term.SetReferenceTerminal(neg_pin_term)
             self._logger.info("Component {} has been replaced by port".format(component.refdes))
             return True
 
     @pyaedt_function_handler()
+    def add_rlc_boundary(self, component=None, circuit_type=True):
+        """Add RLC gap boundary on component and replace it with a circuit port.
+        The circuit port supports only 2-pin components.
+
+        Parameters
+        ----------
+        component : str
+            Reference designator of the RLC component.
+        circuit_type : bool
+            When ``True`` circuit type are defined, if ``False`` gap type will be used instead (compatible with HFSS 3D
+            modeler). Default value is ``True``.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+        """
+        if isinstance(component, str):  # pragma: no cover
+            component = self.instances[component]
+        if not isinstance(component, EDBComponent):  # pragma: no cover
+            return False
+        self.set_component_rlc(component.refdes)
+        pins = self.get_pin_from_component(component.refdes)
+        if len(pins) == 2:  # pragma: no cover
+            pin_layer = self._padstack._get_pin_layer_range(pins[0])[0]
+            pos_pin_term = self._pedb.edb_api.cell.terminal.PadstackInstanceTerminal.Create(
+                self._active_layout,
+                pins[0].GetNet(),
+                "{}_{}".format(component.refdes, pins[0].GetName()),
+                pins[0],
+                pin_layer,
+                False,
+            )
+            if not pos_pin_term:  # pragma: no cover
+                return False
+            neg_pin_term = self._pedb.edb_api.cell.terminal.PadstackInstanceTerminal.Create(
+                self._active_layout,
+                pins[1].GetNet(),
+                "{}_{}_ref".format(component.refdes, pins[1].GetName()),
+                pins[1],
+                pin_layer,
+                True,
+            )
+            if not neg_pin_term:  # pragma: no cover
+                return False
+            pos_pin_term.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.RlcBoundary)
+            if not circuit_type:
+                pos_pin_term.SetIsCircuitPort(False)
+            else:
+                pos_pin_term.SetIsCircuitPort(True)
+            pos_pin_term.SetName(component.refdes)
+            neg_pin_term.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.RlcBoundary)
+            if not circuit_type:
+                neg_pin_term.SetIsCircuitPort(False)
+            else:
+                neg_pin_term.SetIsCircuitPort(True)
+            pos_pin_term.SetReferenceTerminal(neg_pin_term)
+            rlc_values = component.rlc_values
+            rlc = self._edb.utility.Rlc()
+            if rlc_values[0]:
+                rlc.REnabled = True
+                rlc.R = self._edb.utility.value(rlc_values[0])
+            if rlc_values[1]:
+                rlc.LEnabled = True
+                rlc.L = self._edb.utility.value(rlc_values[1])
+            if rlc_values[2]:
+                rlc.CEnabled = True
+                rlc.C = self._edb.utility.value(rlc_values[2])
+            rlc.is_parallel = component.is_parallel_rlc
+            pos_pin_term.SetRlcBoundaryParameters(rlc)
+            self._logger.info("Component {} has been replaced by port".format(component.refdes))
+            return True
+
+    @pyaedt_function_handler()
     def _create_pin_group_terminal(self, pingroup, isref=False):
         """Creates an EDB pin group terminal from a given EDB pin group.
 
         Parameters
         ----------
         pingroup : Edb pin group.
```

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/dotnet/database.py` & `pyaedt-0.6.85/pyaedt/edb_core/dotnet/database.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/dotnet/layout.py` & `pyaedt-0.6.85/pyaedt/edb_core/dotnet/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/dotnet/primitive.py` & `pyaedt-0.6.85/pyaedt/edb_core/dotnet/primitive.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,19 +165,19 @@
             edb_net = all_nets[net_name]
             for refdes, val in edb_net.components.items():
                 if not val.is_enabled:
                     continue
 
                 if refdes in exception_list:
                     pass
-                elif val.type == "Inductor" and val.value < inductor_below and val.is_enabled:
+                elif val.type == "Inductor" and val.rlc_values[1] < inductor_below and val.is_enabled:
                     pass
-                elif val.type == "Resistor" and val.value < resistor_below and val.is_enabled:
+                elif val.type == "Resistor" and val.rlc_values[0] < resistor_below and val.is_enabled:
                     pass
-                elif val.type == "Capacitor" and val.value > capacitor_above and val.is_enabled:
+                elif val.type == "Capacitor" and val.rlc_values[2] > capacitor_above and val.is_enabled:
                     pass
                 else:
                     _comp[refdes] = val
                     continue
 
                 _rlc_serial[refdes] = val
                 for net in val.nets:
```

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,17 +506,25 @@
 
         Returns
         -------
         str
         """
         return self._edb_terminal.GetName()
 
+    @name.setter
+    def name(self, value):
+        if isinstance(value, str):
+            if not any(port for port in list(self._pedb.excitations.keys()) if port == value):
+                self._edb_terminal.SetName(value)
+            else:
+                self._pedb.logger.warning("An existing port already has this same name. A port name must be unique.")
+
     @property
     def net_name(self):
-        """Net Name.
+        """Net name.
 
         Returns
         -------
         str
         """
         return self._edb_terminal.GetNet().GetName()
```

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.85/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/general.py` & `pyaedt-0.6.85/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.85/pyaedt/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/layout.py` & `pyaedt-0.6.85/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/materials.py` & `pyaedt-0.6.85/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/nets.py` & `pyaedt-0.6.85/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.85/pyaedt/edb_core/padstack.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,64 +458,80 @@
         if sball_layer is not None:
             padstackInst.SetSolderBallLayer(sball_layer)
             return True
 
         return False
 
     @pyaedt_function_handler()
-    def create_coax_port(self, padstackinstance, use_dot_separator=True):
+    def create_coax_port(self, padstackinstance, use_dot_separator=True, name=None):
         """Create HFSS 3Dlayout coaxial lumped port on a pastack
         Requires to have solder ball defined before calling this method.
 
         Parameters
         ----------
         padstackinstance : `Edb.Cell.Primitive.PadstackInstance` or int
             Padstack instance object.
+        use_dot_separator : bool, optional
+            Whether to use ``.`` as the separator for the naming convention, which
+            is ``[component][net][pin]``. The default is ``True``. If ``False``, ``_`` is
+            used as the separator instead.
+        name : str
+            Port name for overwriting the default port-naming convention,
+            which is ``[component][net][pin]``. The port name must be unique.
+            If a port with the specified name already exists, the
+            default naming convention is used so that port creation does
+            not fail.
 
         Returns
         -------
         str
             Terminal name.
 
         """
         if isinstance(padstackinstance, int):
             padstackinstance = self.instances[padstackinstance]._edb_padstackinstance
         elif isinstance(padstackinstance, EDBPadstackInstance):
             padstackinstance = padstackinstance._edb_padstackinstance
         cmp_name = padstackinstance.GetComponent().GetName()
         if cmp_name == "":
             cmp_name = "no_comp"
-
         net_name = padstackinstance.GetNet().GetName()
         if net_name == "":
             net_name = "no_net"
-
         pin_name = padstackinstance.GetName()
         if pin_name == "":
             pin_name = "no_pin_name"
         if use_dot_separator:
             port_name = "{0}.{1}.{2}".format(cmp_name, pin_name, net_name)
         else:
             port_name = "{0}_{1}_{2}".format(cmp_name, pin_name, net_name)
         if not padstackinstance.IsLayoutPin():
             padstackinstance.SetIsLayoutPin(True)
-
         res = padstackinstance.GetLayerRange()
+        if name:
+            port_name = name
+        if self._port_exist(port_name):
+            port_name = generate_unique_name(port_name, n=2)
+            self._logger.info("An existing port already has this same name. Renaming to {}.".format(port_name))
         self._edb.cell.terminal.PadstackInstanceTerminal.Create(
             self._active_layout,
             padstackinstance.GetNet(),
             port_name,
             padstackinstance,
             res[2],
         )
         if res[0]:
             return port_name
         return ""
 
     @pyaedt_function_handler()
+    def _port_exist(self, port_name):
+        return any(port for port in list(self._pedb.excitations.keys()) if port == port_name)
+
+    @pyaedt_function_handler()
     def get_pinlist_from_component_and_net(self, refdes=None, netname=None):
         """Retrieve pins given a component's reference designator and net name.
 
         Parameters
         ----------
         refdes : str, optional
             Reference designator of the component. The default is ``None``.
```

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.85/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.85/pyaedt/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/emit.py` & `pyaedt-0.6.85/pyaedt/emit.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.schematic import ModelerEmit
 
 
 class Emit(Design, object):
-    """Provides the Emit application interface.
+    """Provides the EMIT application interface.
 
     Parameters
     ----------
     projectname : str, optional
         Name of the project to select or the full path to the project
         or AEDTZ archive to open.  The default is ``None``, in which case
         an attempt is made to get an active project. If no projects are
@@ -123,15 +123,15 @@
         if projectname is None:
             projectname = generate_unique_project_name()
         self.__emit_api_enabled = False
         self.results = None
         """Constructor for the ``FieldAnalysisEmit`` class"""
 
         self._units = {}
-        """Default Emit units."""
+        """Default EMIT units."""
 
         Design.__init__(
             self,
             "EMIT",
             projectname,
             designname,
             solution_type,
@@ -144,15 +144,15 @@
             port=port,
             aedt_process_id=aedt_process_id,
         )
         self._modeler = ModelerEmit(self)
         self._couplings = CouplingsEmit(self)
         if self._aedt_version > "2023.1":
             # the next 2 lines of code are needed to point
-            # the Emit object to the correct EmiApiPython
+            # the EMIT object to the correct EmiApiPython
             # module for the current AEDT version
             emit_core._set_api(self.aedt_version_id)
             self._emit_api = emit_core.emit_api_python().EmitApi()
             """Instance of the EMIT API."""
 
             self.results = Results(self)
             """''Result'' object for the selected design."""
@@ -174,15 +174,15 @@
         pyaedt.modeler.schematic.ModelerEmit
             Design oModeler
         """
         return self._modeler
 
     @property
     def couplings(self):
-        """Emit Couplings.
+        """EMIT Couplings.
 
         Returns
         -------
         pyaedt.emit_core.Couplings.CouplingsEmit
             Couplings within the EMIT Design
         """
         return self._couplings
```

### Comparing `pyaedt-0.6.82/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.85/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.6.85/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.85/pyaedt/emit_core/results/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 class Results:
     """
     Provides the ``Results`` object.
 
     Parameters
     ----------
     emit_obj : emit_obj object
-        Emit object used to create the result.
+        EMIT object used to create the result.
 
     Examples
     --------
     Create an instance of the ``Result`` object.
 
     >>> aedtapp.results = Results()
     >>> revision = aedtapp.results.analyze()
     >>> receivers = revision.get_receiver_names()
     """
 
     def __init__(self, emit_obj):
         self.emit_project = emit_obj
-        """Emit project."""
+        """EMIT project."""
 
         self.current_revision = None
         """Current active Revision."""
 
         self.revisions = []
         """List of all result revisions. Only one loaded at a time"""
 
         self.design = emit_obj.odesktop.GetActiveProject().GetActiveDesign()
-        """Active design for the Emit project."""
+        """Active design for the EMIT project."""
 
     @pyaedt_function_handler()
     def _add_revision(self, name=None):
         """Add a new revision or get the current revision if it already exists.
 
         Parameters
         ----------
@@ -102,15 +102,15 @@
         --------
         >>> domain = Emit.results.InteractionDomain()
 
         """
         try:
             domain = emit_core.emit_api_python().InteractionDomain()
         except NameError:
-            raise ValueError("An Emit object must be initialized before any static member of the Results.")
+            raise ValueError("An EMIT object must be initialized before any static member of the Results.")
         return domain
 
     @pyaedt_function_handler
     def _unload_revisions(self):
         """Convenience function to set all revisions
         as ``unloaded``
```

### Comparing `pyaedt-0.6.82/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.85/pyaedt/emit_core/results/revision.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,23 +48,23 @@
         self.name = name
         """Name of the revision."""
 
         self.path = full
         """Full path of the revision."""
 
         self.emit_project = emit_obj
-        """Emit project."""
+        """EMIT project."""
 
         raw_props = emit_obj.odesign.GetResultProperties(name)
         key = lambda s: s.split("=", 1)[0]
         val = lambda s: s.split("=", 1)[1]
         props = {key(s): val(s) for s in raw_props}
 
         self.revision_number = int(props["Revision"])
-        """Unique revision number from the Emit design"""
+        """Unique revision number from the EMIT design"""
 
         self.timestamp = props["Timestamp"]
         """Unique timestamp for the revision"""
 
         self.parent_results = parent_results
         """Parent Results object"""
 
@@ -91,16 +91,20 @@
     @staticmethod
     def result_mode_error():
         """
         Print the function mode error message.
 
         Returns
         -------
+        err_msg : str
+            Error/warning message that the specified revision is not accessible.
         """
-        print("This function is inaccessible when the revision is not loaded.")
+        err_msg = "This function is inaccessible when the revision is not loaded."
+        print(err_msg)
+        return err_msg
 
     @pyaedt_function_handler()
     def get_interaction(self, domain):
         """
         Creates a new interaction for a domain.
 
         Parameters
@@ -222,15 +226,17 @@
         ----------
         >>> rxs = aedtapp.results.current_revision.get_reciver_names()
         """
         if self.revision_loaded:
             radios = self.emit_project._emit_api.get_radio_names(TxRxMode.RX, InterfererType.TRANSMITTERS_AND_EMITTERS)
         else:
             radios = None
-            self.result_mode_error()
+            err_msg = self.result_mode_error()
+            warnings.warn(err_msg)
+            return radios
         if len(radios) == 0:
             warnings.warn("No valid receivers in the project.")
         return radios
 
     @pyaedt_function_handler()
     def get_interferer_names(self, interferer_type=None):
         """
@@ -258,15 +264,17 @@
         """
         if interferer_type is None:
             interferer_type = InterfererType.TRANSMITTERS_AND_EMITTERS
         if self.revision_loaded:
             radios = self.emit_project._emit_api.get_radio_names(TxRxMode.TX, interferer_type)
         else:
             radios = None
-            self.result_mode_error()
+            err_msg = self.result_mode_error()
+            warnings.warn(err_msg)
+            return radios
         if len(radios) == 0:
             warnings.warn("No valid radios or emitters in the project.")
             return None
         return radios
 
     @pyaedt_function_handler()
     def get_band_names(self, radio_name, tx_rx_mode=None):
@@ -295,14 +303,17 @@
         if tx_rx_mode is None:
             tx_rx_mode = TxRxMode.BOTH
         if self.revision_loaded:
             bands = self.emit_project._emit_api.get_band_names(radio_name, tx_rx_mode)
         else:
             bands = None
             self.result_mode_error()
+            err_msg = self.result_mode_error()
+            warnings.warn(err_msg)
+            return bands
         return bands
 
     @pyaedt_function_handler()
     def get_active_frequencies(self, radio_name, band_name, tx_rx_mode, units=""):
         """
         Get a list of active frequencies for a ``tx`` or ``rx`` band in a radio/emitter.
 
@@ -330,15 +341,17 @@
         """
         if tx_rx_mode is None or tx_rx_mode == TxRxMode.BOTH:
             raise ValueError("The mode type must be specified as either Tx or Rx.")
         if self.revision_loaded:
             freqs = self.emit_project._emit_api.get_active_frequencies(radio_name, band_name, tx_rx_mode, units)
         else:
             freqs = None
-            self.result_mode_error()
+            err_msg = self.result_mode_error()
+            warnings.warn(err_msg)
+            return freqs
         return freqs
 
     @property
     def notes(self):
         """
         Add notes to the revision.
```

### Comparing `pyaedt-0.6.82/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.85/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.85/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/clr_module.py` & `pyaedt-0.6.85/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/configurations.py` & `pyaedt-0.6.85/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/constants.py` & `pyaedt-0.6.85/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/design_types.py` & `pyaedt-0.6.85/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/filesystem.py` & `pyaedt-0.6.85/pyaedt/generic/filesystem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from glob import glob
 import os
 import random
 import shutil
 import string
 
 
-def my_location():
-    """ """
-    return os.path.normpath(os.path.dirname(__file__))
-
-
-def files_in_directory(path=".", ext=""):
-    """
+def search_files(dirname, pattern="*"):
+    """Search for files inside a directory given a specific pattern.
 
     Parameters
     ----------
-    path :
-         (Default value = '.')
-    ext :
-         (Default value = '')
+    dirname : str
+    pattern :str, optional
 
     Returns
     -------
-
+    list
     """
-    result = []
-    if os.path.exists(path):
-        for dir in os.listdir(path):
-            bd = os.path.join(path, dir)
-            if os.path.isfile(bd) and dir.endswith("." + ext):
-                result.append(bd)
-    return result
+    from pyaedt.generic.general_methods import is_ironpython
+
+    if is_ironpython:
+        import glob
+
+        return list(glob.glob(os.path.join(dirname, pattern)))
+    else:
+        import pathlib
+
+        return [os.path.abspath(i) for i in pathlib.Path(dirname).glob(pattern)]
+
+
+def my_location():
+    """ """
+    return os.path.normpath(os.path.dirname(__file__))
 
 
 class Scratch:
     """ """
 
     @property
     def path(self):
@@ -137,8 +137,8 @@
     ----------
     start_folder, str
         Path to the folder where the json files are located.
 
     Returns
     -------
     """
-    return [y for x in os.walk(start_folder) for y in glob(os.path.join(x[0], "*.json"))]
+    return [y for x in os.walk(start_folder) for y in search_files(x[0], "*.json")]
```

### Comparing `pyaedt-0.6.82/pyaedt/generic/general_methods.py` & `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,2217 +1,1884 @@
 # -*- coding: utf-8 -*-
-from __future__ import absolute_import
-
-import ast
-import codecs
-from collections import OrderedDict
-import csv
-import datetime
-import difflib
-import fnmatch
-from functools import update_wrapper
-import inspect
-import itertools
-import json
-import logging
-import math
 import os
 import random
 import re
-import string
-import sys
-import tempfile
-import time
-import traceback
-
-from pyaedt.generic.constants import CSS4_COLORS
-
-is_ironpython = "IronPython" in sys.version or ".NETFramework" in sys.version
-is_linux = os.name == "posix"
-is_windows = not is_linux
-_pythonver = sys.version_info[0]
-inside_desktop = True if is_ironpython and "4.0.30319.42000" in sys.version else False
-
-if not is_ironpython:
-    import psutil
-
-try:
-    import xml.etree.cElementTree as ET
-
-    ET.VERSION
-except ImportError:
-    ET = None
-
-
-class MethodNotSupportedError(Exception):
-    """ """
-
-    pass
-
-
-def _write_mes(mes_text):
-    mes_text = str(mes_text)
-    parts = [mes_text[i : i + 250] for i in range(0, len(mes_text), 250)]
-    for el in parts:
-        settings.logger.error(el)
-
-
-def _get_args_dicts(func, args, kwargs):
-    if int(sys.version[0]) > 2:
-        args_name = list(OrderedDict.fromkeys(inspect.getfullargspec(func)[0] + list(kwargs.keys())))
-        args_dict = OrderedDict(list(itertools.zip_longest(args_name, args)) + list(kwargs.items()))
-    else:
-        args_name = list(OrderedDict.fromkeys(inspect.getargspec(func)[0] + list(kwargs.keys())))
-        args_dict = OrderedDict(list(itertools.izip(args_name, args)) + list(kwargs.iteritems()))
-    return args_dict
-
-
-def _exception(ex_info, func, args, kwargs, message="Type Error"):
-    """Write the trace stack to the desktop when a Python error occurs.
-
-    Parameters
-    ----------
-    ex_info :
+import warnings
 
-    func :
+from pyaedt.application.Variables import decompose_variable_value
+from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
+from pyaedt.generic.constants import AEDT_UNITS
 
-    args :
+# from pyaedt.generic.general_methods import property
+from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import pyaedt_function_handler
+from pyaedt.modeler.circuits.PrimitivesCircuit import CircuitComponents
+from pyaedt.modeler.circuits.PrimitivesCircuit import ComponentCatalog
+from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
+from pyaedt.modules.Boundary import Excitations
 
-    kwargs :
 
-    message :
-         (Default value = "Type Error")
-
-    Returns
-    -------
-
-    """
-    tb_data = ex_info[2]
-    tb_trace = traceback.format_tb(tb_data)
-    if len(tb_trace) > 1:
-        tblist = tb_trace[1].split("\n")
-    else:
-        tblist = tb_trace[0].split("\n")
-
-    message_to_print = ""
-    try:
-        messages = list(sys.modules["__main__"].oDesktop.GetMessages("", "", 2))
-    except AttributeError:
-        messages = []
-    except TypeError:
-        messages = []
-    if messages and "error" in messages[-1].lower():
-        message_to_print = messages[-1]
-    # _write_mes("{} - {} -  {}.".format(ex_info[1], func.__name__, message.upper()))
-
-    if message_to_print:
-        _write_mes("API Message - " + message_to_print)
-    for el in tblist:
-        if func.__name__ in el:
-            _write_mes("{}, {}".format(el, message.upper()))
-    args_name = []
-    try:
-        args_dict = _get_args_dicts(func, args, kwargs)
-        first_time_log = True
-
-        for el in args_dict:
-            if el != "self" and args_dict[el]:
-                if first_time_log:
-                    _write_mes("Method arguments: ")
-                    first_time_log = False
-                _write_mes("    {} = {} ".format(el, args_dict[el]))
-    except:
-        pass
-    args = [func.__name__] + [i for i in args_name if i not in ["self"]]
-    if not func.__name__.startswith("_"):
-        _write_mes(
-            "Check Online documentation on: https://aedt.docs.pyansys.com/version/stable/search.html?q={}".format(
-                "+".join(args)
-            )
-        )
-
-
-def normalize_path(path_in, sep=None):
-    """Normalize path separators.
+class NexximComponents(CircuitComponents):
+    """Manages circuit components for Nexxim.
 
     Parameters
     ----------
-    path_in : str
-        Path to normalize.
-    sep : str, optional
-        Separator.
-
-    Returns
-    -------
-    str
-        Path normalized to new separator.
-    """
-    if sep is None:
-        sep = os.sep
-    return path_in.replace("\\", sep).replace("/", sep)
-
-
-def _check_types(arg):
-    if "netref.builtins.list" in str(type(arg)):
-        return "list"
-    elif "netref.builtins.dict" in str(type(arg)):
-        return "dict"
-    elif "netref.__builtin__.list" in str(type(arg)):
-        return "list"
-    elif "netref.__builtin__.dict" in str(type(arg)):
-        return "dict"
-    return ""
-
-
-def _function_handler_wrapper(user_function):
-    def wrapper(*args, **kwargs):
-        if not settings.enable_error_handler:
-            result = user_function(*args, **kwargs)
-            return result
-        else:
-            try:
-                settings.time_tick = time.time()
-                out = user_function(*args, **kwargs)
-                if settings.enable_debug_logger or settings.enable_debug_edb_logger:
-                    _log_method(user_function, args, kwargs)
-                return out
-            except TypeError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "Type Error")
-                return False
-            except ValueError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "Value Error")
-                return False
-            except AttributeError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "Attribute Error")
-                return False
-            except KeyError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "Key Error")
-                return False
-            except IndexError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "Index Error")
-                return False
-            except AssertionError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "Assertion Error")
-                return False
-            except NameError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "Name Error")
-                return False
-            except IOError:
-                _exception(sys.exc_info(), user_function, args, kwargs, "IO Error")
-                return False
-            except MethodNotSupportedError:
-                message = "This Method is not supported in current AEDT Design Type."
-                if settings.enable_screen_logs:
-                    print("**************************************************************")
-                    print("pyaedt error on Method {}:  {}. Please Check again".format(user_function.__name__, message))
-                    print("**************************************************************")
-                    print("")
-                if settings.enable_file_logs:
-                    settings.logger.error(message)
-                return False
-            except BaseException:
-                _exception(sys.exc_info(), user_function, args, kwargs, "General or AEDT Error")
-                return False
-
-    return wrapper
-
-
-def pyaedt_function_handler(direct_func=None):
-    """Provides an exception handler, logging mechanism, and argument converter for client-server
-    communications.
-
-    This method returns the function itself if correctly executed. Otherwise, it returns ``False``
-    and displays errors.
+    modeler : :class:`pyaedt.modeler.schematic.ModelerNexxim`
+        Inherited parent object.
+    Examples
+    --------
 
+    >>> from pyaedt import Circuit
+    >>> aedtapp = Circuit()
+    >>> prim = aedtapp.modeler.schematic
     """
-    if callable(direct_func):
-        user_function = direct_func
-        wrapper = _function_handler_wrapper(user_function)
-        return update_wrapper(wrapper, user_function)
-    elif direct_func is not None:
-        raise TypeError("Expected first argument to be a callable, or None")
 
-    def decorating_function(user_function):
-        wrapper = _function_handler_wrapper(user_function)
-        return update_wrapper(wrapper, user_function)
+    @property
+    def design_libray(self):
+        """Design library."""
+        return "Nexxim Circuit Elements"
 
-    return decorating_function
+    @property
+    def tab_name(self):
+        """Tab name."""
+        return "PassedParameterTab"
 
+    @pyaedt_function_handler()
+    def __getitem__(self, partname):
+        """Get the object ID if the part name is an integer or the object name if it is a string.
+        Parameters
+        ----------
+        partname : int or str
+            Part ID or object name.
 
-@pyaedt_function_handler()
-def check_numeric_equivalence(a, b, relative_tolerance=1e-7):
-    """Check if two numeric values are equivalent to within a relative tolerance.
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
+        """
+        if type(partname) is int:
+            return self.components[partname]
+        for el in self.components:
+            if self.components[el].name == partname or self.components[el].composed_name == partname or el == partname:
+                return self.components[el]
 
-    Paraemters
-    ----------
-    a : int, float
-        Reference value to compare to.
-    b : int, float
-        Secondary value for the comparison.
-    relative_tolerance : float, optional
-        Relative tolerance for the equivalence test. The difference is relative to the first value.
-        The default is ``1E-7``.
-
-    Returns
-    -------
-    bool
-        ``True`` if the two passed values are equivalent.
-    """
-    if abs(a) > 0.0:
-        reldiff = abs(a - b) / a
-    else:
-        reldiff = abs(b)
-    return True if reldiff < relative_tolerance else False
+        return None
 
+    @property
+    def _logger(self):
+        return self._app.logger
 
-@pyaedt_function_handler()
-def check_and_download_file(local_path, remote_path, overwrite=True):
-    """Check if a file is remote and either download it or return the path.
+    def __init__(self, modeler):
+        CircuitComponents.__init__(self, modeler)
+        self._app = modeler._app
+        self._modeler = modeler
+        self._currentId = 0
+        self._components_catalog = None
 
-    Parameters
-    ----------
-    local_path : str
-        Local path to save the file to.
-    remote_path : str
-        Path to the remote file.
-    overwrite : bool
-        Whether to overwrite the file if it already exits locally.
-        The default is ``True``.
-
-    Returns
-    -------
-    str
-    """
-    if settings.remote_rpc_session:
-        remote_path = remote_path.replace("\\", "/") if remote_path[0] != "\\" else remote_path
-        settings.remote_rpc_session.filemanager.download_file(remote_path, local_path, overwrite=overwrite)
-        return local_path
-    return remote_path
+    @property
+    def components_catalog(self):
+        """Return the syslib component catalog with all info.
 
+        Returns
+        -------
+        :class:`pyaedt.modeler.PrimitivesCircuit.ComponentCatalog`
+        """
+        if not self._components_catalog:
+            self._components_catalog = ComponentCatalog(self)
+        return self._components_catalog
 
-def check_if_path_exists(path):
-    """Check whether a path exists or not local or remote machine (for remote sessions only).
+    @pyaedt_function_handler()
+    def create_subcircuit(self, location=None, angle=None, name=None, nested_subcircuit_id=None):
+        """Add a new Circuit subcircuit to the design.
 
-    Parameters
-    ----------
-    path : str
-        Local or remote path to check.
+        Parameters
+        ----------
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``None``.
+        name : str, optional
+            Name of the design. The default is ``None``, in which case
+            a unique name is generated.
+        nested_subcircuit_id : str, optional
+            ID of the nested subcircuit.
+            Example `"U1"`.
 
-    Returns
-    -------
-    bool
-    """
-    if settings.remote_rpc_session:
-        return settings.remote_rpc_session.filemanager.pathexists(path)
-    return os.path.exists(path)
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object when successful or ``False`` when failed.
 
+        Examples
+        --------
+        >>> from pyaedt import Circuit
+        >>> cir = Circuit()
+        """
+        if not name:
+            name = generate_unique_name("Circuit")
+
+        if nested_subcircuit_id:
+            parent_name = "{}:{}:{}".format(
+                self._app.design_name.split("/")[0], nested_subcircuit_id, random.randint(1, 10000)
+            )
+        else:
+            parent_name = "{}:{}".format(self._app.design_name.split("/")[0], ":U" + str(random.randint(1, 10000)))
 
-@pyaedt_function_handler()
-def check_and_download_folder(local_path, remote_path, overwrite=True):
-    """Check if a folder is remote and either download it or return the path.
+        self._app.odesign.InsertDesign("Circuit Design", name, "", parent_name)
+        if nested_subcircuit_id:
+            pname = "{}:{}".format(self._app.design_name.split("/")[0], nested_subcircuit_id)
+            odes = self._app.oproject.SetActiveDesign(pname)
+            oed = odes.SetActiveEditor("SchematicEditor")
+            objs = oed.GetAllElements()
+            match = [i for i in objs if name in i]
+            o = CircuitComponent(self, tabname=self.tab_name, custom_editor=oed)
+            name = match[0].split(";")
+            o.name = name[0]
+            o.schematic_id = name[2]
+            o.id = int(name[1])
+            return o
+        self.refresh_all_ids()
+        for el in self.components:
+            if name in self.components[el].composed_name:
+                if location:
+                    self.components[el].location = [
+                        i / AEDT_UNITS["Length"][self.schematic_units] for i in self._get_location(location)
+                    ]
+                if angle is not None:
+                    self.components[el].angle = self.number_with_units(angle, "°")
+                return self.components[el]
+        return False
 
-    Parameters
-    ----------
-    local_path : str
-        Local path to save the folder to.
-    remote_path : str
-        Path to the remote folder.
-    overwrite : bool
-        Whether to overwrite the folder if it already exits locally.
-        The default is ``True``.
-
-    Returns
-    -------
-    str
-    """
-    if settings.remote_rpc_session:
-        remote_path = remote_path.replace("\\", "/") if remote_path[0] != "\\" else remote_path
-        settings.remote_rpc_session.filemanager.download_folder(remote_path, local_path, overwrite=overwrite)
-        return local_path
-    return remote_path
+    @pyaedt_function_handler()
+    def duplicate(self, component, location=None, angle=0, flip=False):  # pragma: no cover
+        """Add a new subcircuit to the design.
 
+        .. note::
+            This works only in graphical mode.
 
-def open_file(file_path, file_options="r"):
-    """Open a file and return the object.
+        Parameters
+        ----------
+        component : class:`pyaedt.modeler.Object3d.CircuitComponent` Circuit Component Object
+            Component to duplicate.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        flip : bool, optional
+            Whether the component should be flipped. The default value is ``False``.
 
-    Parameters
-    ----------
-    file_path : str
-        Full absolute path to the file (either local or remote).
-    file_options : str, optional
-        Options for opening the file.
-
-    Returns
-    -------
-    object
-        Opened file.
-    """
-    file_path = file_path.replace("\\", "/") if file_path[0] != "\\" else file_path
-    dir_name = os.path.dirname(file_path)
-    if "r" in file_options:
-        if os.path.exists(file_path):
-            return open(file_path, file_options)
-        elif settings.remote_rpc_session and settings.remote_rpc_session.filemanager.pathexists(
-            file_path
-        ):  # pragma: no cover
-            local_file = os.path.join(tempfile.gettempdir(), os.path.split(file_path)[-1])
-            settings.remote_rpc_session.filemanager.download_file(file_path, local_file)
-            return open(local_file, file_options)
-    elif os.path.exists(dir_name):
-        return open(file_path, file_options)
-    else:
-        settings.logger.error("The file or folder %s does not exist", dir_name)
-
-
-def _log_method(func, new_args, new_kwargs):
-    if not settings.enable_debug_internal_methods_logger and str(func.__name__)[0] == "_":
-        return
-    if not settings.enable_debug_geometry_operator_logger and "GeometryOperators" in str(func):
-        return
-    if (
-        not settings.enable_debug_edb_logger
-        and "Edb" in str(func) + str(new_args)
-        or "edb_core" in str(func) + str(new_args)
-    ):
-        return
-    line_begin = "ARGUMENTS: "
-    message = []
-    delta = time.time() - settings.time_tick
-    m, s = divmod(delta, 60)
-    h, m = divmod(m, 60)
-    d, h = divmod(h, 24)
-    msec = (s - int(s)) * 1000
-    if d > 0:
-        time_msg = " {}days {}h {}m {}sec.".format(d, h, m, int(s))
-    elif h > 0:
-        time_msg = " {}h {}m {}sec.".format(h, m, int(s))
-    else:
-        time_msg = "  {}m {}sec {}msec.".format(m, int(s), int(msec))
-    if settings.enable_debug_methods_argument_logger:
-        args_dict = _get_args_dicts(func, new_args, new_kwargs)
-        id = 0
-        if new_args:
-            object_name = str([new_args[0]])[1:-1]
-            id = object_name.find(" object at ")
-        if id > 0:
-            object_name = object_name[1:id]
-            message.append("'{}' was run in {}".format(object_name + "." + str(func.__name__), time_msg))
-        else:
-            message.append("'{}' was run in {}".format(str(func.__name__), time_msg))
-        message.append(line_begin)
-        for k, v in args_dict.items():
-            if k != "self":
-                message.append("    {} = {}".format(k, v))
-    for m in message:
-        settings.logger.debug(m)
-
-
-@pyaedt_function_handler()
-def get_version_and_release(input_version):
-    version = int(input_version[2:4])
-    release = int(input_version[5])
-    if version < 20:
-        if release < 3:
-            version -= 1
+        Returns
+        -------
+        :class:`pyaedt.modeler.Object3d.CircuitComponent` Circuit Component Object
+        when successful or ``False`` when failed.
+        """
+        comp_names = []
+        if isinstance(component, CircuitComponent):
+            comp_names.append(component.composed_name)
         else:
-            release -= 2
-    return (version, release)
-
-
-@pyaedt_function_handler()
-def env_path(input_version):
-    """Get the path of the version environment variable for an AEDT version.
+            comp_names.append(component)
+        self._modeler.oeditor.Copy(["NAME:Selections", "Selections:=", comp_names])
+        location = self._get_location(location)
+        self._modeler.oeditor.Paste(
+            ["NAME:Attributes", "Page:=", 1, "X:=", location[0], "Y:=", location[1], "Angle:=", angle, "Flip:=", flip]
+        )
+        ids = [id for id in list(self.components.keys())]
+        self.refresh_all_ids()
+        new_ids = [id for id in list(self.components.keys()) if id not in ids]
+        if new_ids:
+            return self.components[new_ids[0]]
+        return False
 
-    Parameters
-    ----------
-    input_version : str
-        AEDT version.
+    @pyaedt_function_handler()
+    def connect_components_in_series(self, components_to_connect, use_wire=True):
+        """Connect schematic components in series.
 
-    Returns
-    -------
-    str
-        Path for the version environment variable.
+        Parameters
+        ----------
+        components_to_connect : list of :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+           List of Components to connect. It can be a list of objects or component names.
+        use_wire : bool, optional
+            Whether to use wires or a page port to connect the pins.
+            The default is ``True``, in which case wires are used. Note
+            that if wires are not well placed, shorts can result.
 
-    Examples
-    --------
-    >>> env_path_student("2021.2")
-    "C:/Program Files/ANSYSEM/ANSYSEM2021.2/Win64"
-    """
-    return os.getenv(
-        "ANSYSEM_ROOT{0}{1}".format(
-            get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
-        ),
-        "",
-    )
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
 
+        Examples
+        --------
+        >>> from pyaedt import Circuit
+        >>> circuit = Circuit()
+        >>> circuit.modeler.schematic_units = "mil"
+        >>> myind = circuit.modeler.schematic.create_inductor(compname="L100", value=1e-9, location=[0,0])
+        >>> myres = circuit.modeler.schematic.create_resistor(compname="R100", value=50, location=[100, 2000])
+        >>> circuit.modeler.schematic.connect_components_in_series([myind, myres])
+        """
+        comps = []
+        for component in components_to_connect:
+            if isinstance(component, (CircuitComponent, Excitations)):
+                comps.append(component)
+            else:
+                for id, cmp in self.components.items():
+                    if component in [cmp.id, cmp.name, cmp.composed_name]:
+                        comps.append(cmp)
+                        break
+        i = 0
+        assert len(comps) > 1, "At least two components have to be passed."
+        while i < (len(comps) - 1):
+            comps[i].pins[-1].connect_to_component(comps[i + 1].pins[0], use_wire=use_wire)
+            i += 1
+        return True
 
-@pyaedt_function_handler()
-def env_value(input_version):
-    """Get the name of the version environment variable for an AEDT version.
+    @pyaedt_function_handler()
+    def connect_components_in_parallel(self, components_to_connect):
+        """Connect schematic components in parallel.
 
-    Parameters
-    ----------
-    input_version : str
-        AEDT version.
+        Parameters
+        ----------
+        components_to_connect : list of :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+           List of Components to connect. It can be a list of objects or component names.
 
-    Returns
-    -------
-    str
-        Name for the version environment variable.
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
 
-    Examples
-    --------
-    >>> env_value("2021.2")
-    "ANSYSEM_ROOT211"
-    """
-    return "ANSYSEM_ROOT{0}{1}".format(
-        get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
-    )
+        Examples
+        --------
+        >>> from pyaedt import Circuit
+        >>> circuit = Circuit()
+        >>> myind = circuit.modeler.schematic.create_inductor("L100", 1e-9)
+        >>> myres = circuit.modeler.schematic.create_resistor("R100", 50)
+        >>> circuit.modeler.schematic.connect_components_in_parallel([myind, myres.composed_name])
+        """
+        comps = []
+        for component in components_to_connect:
+            if isinstance(component, CircuitComponent):
+                comps.append(component)
+            else:
+                for id, cmp in self.components.items():
+                    if component in [cmp.id, cmp.name, cmp.composed_name]:
+                        comps.append(cmp)
+                        break
+        assert len(comps) > 1, "At least two components have to be passed."
+        comps[0].pins[0].connect_to_component([i.pins[0] for i in comps[1:]])
+        terminal_to_connect = [cmp for cmp in comps if len(cmp.pins) >= 2]
+        if len(terminal_to_connect) > 1:
+            terminal_to_connect[0].pins[1].connect_to_component([i.pins[1] for i in terminal_to_connect[1:]])
+        return True
 
+    @pyaedt_function_handler()
+    def add_subcircuit_3dlayout(self, sourcename):
+        """Add a subcircuit from a HFSS 3DLayout.
 
-@pyaedt_function_handler()
-def env_path_student(input_version):
-    """Get the path of the version environment variable for an AEDT student version.
+        Parameters
+        ----------
+        sourcename : str
+            Name of the source design.
 
-    Parameters
-    ----------
-    input_version : str
-       AEDT student version.
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    Returns
-    -------
-    str
-        Path for the student version environment variable.
+        References
+        ----------
 
-    Examples
-    --------
-    >>> env_path_student("2021.2")
-    "C:/Program Files/ANSYSEM/ANSYSEM2021.2/Win64"
-    """
-    return os.getenv(
-        "ANSYSEMSV_ROOT{0}{1}".format(
-            get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
-        ),
-        "",
-    )
+        >>> oProject.CopyDesign
+        >>> oEditor.PasteDesign
+        """
+        self._app._oproject.CopyDesign(sourcename)
+        self.oeditor.PasteDesign(
+            0,
+            ["NAME:Attributes", "Page:=", 1, "X:=", 0, "Y:=", 0, "Angle:=", 0, "Flip:=", False],
+        )
+        self.refresh_all_ids()
+        for el in self.components:
+            if sourcename in self.components[el].composed_name:
+                return self.components[el]
+        return False
 
+    @pyaedt_function_handler()
+    def create_field_model(self, design_name, solution_name, pin_names, model_type="hfss"):
+        """Create a field model.
 
-@pyaedt_function_handler()
-def env_value_student(input_version):
-    """Get the name of the version environment variable for an AEDT student version.
+        Parameters
+        ----------
+        design_name : str
+            Name of the design.
+        solution_name : str
+            Name  of the solution.
+        pin_names : list
+            List of the pin names.
+        model_type : str, optional
+            Type of the model. The default is ``"hfss"``.
 
-    Parameters
-    ----------
-    input_version : str
-        AEDT student version.
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
 
-    Returns
-    -------
-    str
-         Name for the student version environment variable.
+        References
+        ----------
 
-    Examples
-    --------
-    >>> env_value_student("2021.2")
-    "ANSYSEMSV_ROOT211"
-    """
-    return "ANSYSEMSV_ROOT{0}{1}".format(
-        get_version_and_release(input_version)[0], get_version_and_release(input_version)[1]
-    )
+        >>> oModelManager.Add
+        >>> oComponentManager.Add
+        """
+        id = self.create_unique_id()
+        component_name = design_name + "_" + str(id)
+        arg = [
+            "NAME: " + component_name,
+            "Name:=",
+            component_name,
+            "ModTime:=",
+            1589868932,
+            "Library:=",
+            "",
+            "LibLocation:=",
+            "Project",
+            "ModelType:=",
+            model_type,
+            "Description:=",
+            "",
+            "ImageFile:=",
+            "",
+            "SymbolPinConfiguration:=",
+            0,
+            ["NAME:PortInfoBlk"],
+            ["NAME:PortOrderBlk"],
+            "DesignName:=",
+            design_name,
+            "SolutionName:=",
+            solution_name,
+            "NewToOldMap:=",
+            [],
+            "OldToNewMap:=",
+            [],
+            "PinNames:=",
+            pin_names,
+            [
+                "NAME:DesignerCustomization",
+                "DCOption:=",
+                0,
+                "InterpOption:=",
+                0,
+                "ExtrapOption:=",
+                1,
+                "Convolution:=",
+                0,
+                "Passivity:=",
+                0,
+                "Reciprocal:=",
+                False,
+                "ModelOption:=",
+                "",
+                "DataType:=",
+                1,
+            ],
+            [
+                "NAME:NexximCustomization",
+                "DCOption:=",
+                3,
+                "InterpOption:=",
+                1,
+                "ExtrapOption:=",
+                3,
+                "Convolution:=",
+                0,
+                "Passivity:=",
+                0,
+                "Reciprocal:=",
+                False,
+                "ModelOption:=",
+                "",
+                "DataType:=",
+                2,
+            ],
+            [
+                "NAME:HSpiceCustomization",
+                "DCOption:=",
+                1,
+                "InterpOption:=",
+                2,
+                "ExtrapOption:=",
+                3,
+                "Convolution:=",
+                0,
+                "Passivity:=",
+                0,
+                "Reciprocal:=",
+                False,
+                "ModelOption:=",
+                "",
+                "DataType:=",
+                3,
+            ],
+            "NoiseModelOption:=",
+            "External",
+            "WB_SystemID:=",
+            design_name,
+            "IsWBModel:=",
+            False,
+            "filename:=",
+            "",
+            "numberofports:=",
+            len(pin_names),
+            "Simulate:=",
+            False,
+            "CloseProject:=",
+            False,
+            "SaveProject:=",
+            True,
+            "InterpY:=",
+            True,
+            "InterpAlg:=",
+            "auto",
+            "IgnoreDepVars:=",
+            False,
+            "Renormalize:=",
+            False,
+            "RenormImpedance:=",
+            50,
+        ]
+        self.o_model_manager.Add(arg)
+        arg = [
+            "NAME:" + component_name,
+            "Info:=",
+            [
+                "Type:=",
+                8,
+                "NumTerminals:=",
+                len(pin_names),
+                "DataSource:=",
+                "",
+                "ModifiedOn:=",
+                1589868933,
+                "Manufacturer:=",
+                "",
+                "Symbol:=",
+                "",
+                "ModelNames:=",
+                "",
+                "Footprint:=",
+                "",
+                "Description:=",
+                "",
+                "InfoTopic:=",
+                "",
+                "InfoHelpFile:=",
+                "",
+                "IconFile:=",
+                "",
+                "Library:=",
+                "",
+                "OriginalLocation:=",
+                "Project",
+                "IEEE:=",
+                "",
+                "Author:=",
+                "",
+                "OriginalAuthor:=",
+                "",
+                "CreationDate:=",
+                1589868933,
+                "ExampleFile:=",
+                "",
+                "HiddenComponent:=",
+                0,
+                "CircuitEnv:=",
+                0,
+                "GroupID:=",
+                0,
+            ],
+            "CircuitEnv:=",
+            0,
+            "Refbase:=",
+            "S",
+            "NumParts:=",
+            1,
+            "ModSinceLib:=",
+            False,
+        ]
+        id = 2
+        for pn in pin_names:
+            arg.append("Terminal:=")
+            arg.append([pn, pn, "A", False, id, 1, "", "Electrical", "0"])
+            id += 1
+        arg.append(["NAME:Properties", "TextProp:=", ["Owner", "RD", "", model_type.upper()]])
+        arg.append("CompExtID:="), arg.append(5)
+        arg.append(
+            [
+                "NAME:Parameters",
+                "TextProp:=",
+                ["ModelName", "RD", "", "FieldSolver"],
+                "MenuProp:=",
+                ["CoSimulator", "SD", "", "Default", 0],
+                "ButtonProp:=",
+                ["CosimDefinition", "SD", "", "Edit", "Edit", 40501, "ButtonPropClientData:=", []],
+            ]
+        )
+        arg.append(
+            [
+                "NAME:CosimDefinitions",
+                [
+                    "NAME:CosimDefinition",
+                    "CosimulatorType:=",
+                    103,
+                    "CosimDefName:=",
+                    "Default",
+                    "IsDefinition:=",
+                    True,
+                    "Connect:=",
+                    True,
+                    "ModelDefinitionName:=",
+                    component_name,
+                    "ShowRefPin2:=",
+                    2,
+                    "LenPropName:=",
+                    "",
+                ],
+                "DefaultCosim:=",
+                "Default",
+            ]
+        )
 
+        self.o_component_manager.Add(arg)
+        self._app._odesign.AddCompInstance(component_name)
+        self.refresh_all_ids()
+        for el in self.components:
+            if component_name in self.components[el].composed_name:
+                return el, self.components[el].composed_name
+        return False
 
-@pyaedt_function_handler()
-def get_filename_without_extension(path):
-    """Get the filename without its extension.
+    @pyaedt_function_handler()
+    def create_resistor(self, compname=None, value=50, location=[], angle=0, use_instance_id_netlist=False):
+        """Create a resistor.
 
-    Parameters
-    ----------
-    path : str
-        Path for the file.
+        Parameters
+        ----------
+        compname : str, optional
+            Name of the resistor. The default is ``None``.
+        value : float, optional
+            Resistance in ohms. The default is ``50``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    Returns
-    -------
-    str
-       Name for the file, excluding its extension.
+        References
+        ----------
 
-    """
-    return os.path.splitext(os.path.split(path)[1])[0]
+        >>> oEditor.CreateComponent
+        """
+        cmpid = self.create_component(
+            compname, location=location, angle=angle, use_instance_id_netlist=use_instance_id_netlist
+        )
 
+        cmpid.set_property("R", value)
+        return cmpid
 
-@pyaedt_function_handler()
-def generate_unique_name(rootname, suffix="", n=6):
-    """Generate a new name given a root name and optional suffix.
+    @pyaedt_function_handler()
+    def create_inductor(self, compname=None, value=50, location=[], angle=0, use_instance_id_netlist=False):
+        """Create an inductor.
 
-    Parameters
-    ----------
-    rootname :
-        Root name to add random characters to.
-    suffix : string
-        Suffix to add. The default is ``''``.
-    n : int
-        Number of random characters to add to the name. The default value is ``6``.
-
-    Returns
-    -------
-    str
-        Newly generated name.
+        Parameters
+        ----------
+        compname : str, optional
+            Name of the inductor. The default is ``None``.
+        value : float, optional
+            Inductance value. The default is ``50``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    """
-    char_set = string.ascii_uppercase + string.digits
-    uName = "".join(random.choice(char_set) for _ in range(n))
-    unique_name = rootname + "_" + uName
-    if suffix:
-        unique_name += "_" + suffix
-    return unique_name
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
+        References
+        ----------
 
-@pyaedt_function_handler()
-def generate_unique_folder_name(rootname=None, folder_name=None):
-    """Generate a new AEDT folder name given a rootname.
+        >>> oEditor.CreateComponent
+        """
+        cmpid = self.create_component(
+            compname,
+            component_library="Inductors",
+            component_name="IND_",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
-    Parameters
-    ----------
-    rootname : str, optional
-        Root name for the new folder. The default is ``None``.
-    folder_name : str, optional
-        Name for the new AEDT folder if one must be created.
-
-    Returns
-    -------
-    str
-    """
-    if not rootname:
-        if settings.remote_rpc_session:
-            rootname = settings.remote_rpc_session_temp_folder
-        else:
-            rootname = tempfile.gettempdir()
-    if folder_name is None:
-        folder_name = generate_unique_name("pyaedt_prj", n=3)
-    temp_folder = os.path.join(rootname, folder_name)
-    if settings.remote_rpc_session and not settings.remote_rpc_session.filemanager.pathexists(temp_folder):
-        settings.remote_rpc_session.filemanager.makedirs(temp_folder)
-    elif not os.path.exists(temp_folder):
-        os.makedirs(temp_folder)
-
-    return temp_folder
+        cmpid.set_property("L", value)
 
+        return cmpid
 
-@pyaedt_function_handler()
-def generate_unique_project_name(rootname=None, folder_name=None, project_name=None, project_format="aedt"):
-    """Generate a new AEDT project name given a rootname.
+    @pyaedt_function_handler()
+    def create_capacitor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+        """Create a capacitor.
 
-    Parameters
-    ----------
-    rootname : str, optional
-        Root name where the new project is to be created.
-    folder_name : str, optional
-        Name of the folder to create. The default is ``None``, in which case a random folder
-        is created. Use ``""`` if you do not want to create a subfolder.
-    project_name : str, optional
-        Name for the project. The default is ``None``, in which case a random project is
-        created. If a project with this name already exists, a new suffix is added.
-    project_format : str, optional
-        Project format. The default is ``"aedt"``. Options are ``"aedt"`` and ``"aedb"``.
-
-    Returns
-    -------
-    str
-    """
-    if not project_name:
-        project_name = generate_unique_name("Project", n=3)
-    name_with_ext = project_name + "." + project_format
-    folder_path = generate_unique_folder_name(rootname, folder_name=folder_name)
-    prj = os.path.join(folder_path, name_with_ext)
-    if check_if_path_exists(prj):
-        name_with_ext = generate_unique_name(project_name, n=3) + "." + project_format
-        prj = os.path.join(folder_path, name_with_ext)
-    return prj
+        Parameters
+        ----------
+        compname : str, optional
+            Name of the capacitor. The default is ``None``.
+        value : float, optional
+            Capacitor value. The default is ``50``.
+        location : list of float, optional
+            Position on the X axis and Y axis. The default is ``None``.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-def _retry_ntimes(n, function, *args, **kwargs):
-    """
+        References
+        ----------
 
-    Parameters
-    ----------
-    n :
+        >>> oEditor.CreateComponent
+        """
 
-    function :
+        if location == None:
+            location = []
 
-    *args :
+        cmpid = self.create_component(
+            compname,
+            component_library="Capacitors",
+            component_name="CAP_",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
-    **kwargs :
+        cmpid.set_property("C", value)
+        return cmpid
 
+    @pyaedt_function_handler()
+    def create_voltage_dc(self, compname=None, value=1, location=None, angle=0, use_instance_id_netlist=False):
+        """Create a voltage DC source.
 
-    Returns
-    -------
+        Parameters
+        ----------
+        compname : str, optional
+            Name of the voltage DC source. The default is ``None``.
+        value : float, optional
+            Voltage value. The default is ``50``.
+        location : list of float, optional
+            Position on the X axis and Y axis. The default is ``None``.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    """
-    retry = 0
-    ret_val = None
-    while retry < n:
-        try:
-            ret_val = function(*args, **kwargs)
-            if ret_val is None:
-                # if not ret_val and type(ret_val) not in [float, int, str, tuple, list]:
-                ret_val = True
-        except:
-            retry += 1
-            time.sleep(0.5)
-        else:
-            break
-    if retry == n:
-        if "__name__" in dir(function):
-            raise AttributeError("Error in Executing Method {}.".format(function.__name__))
-        else:
-            raise AttributeError("Error in Executing Method.")
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    return ret_val
+        References
+        ----------
 
+        >>> oEditor.CreateComponent
+        """
+        if location == None:
+            location = []
 
-def time_fn(fn, *args, **kwargs):
-    start = datetime.datetime.now()
-    results = fn(*args, **kwargs)
-    end = datetime.datetime.now()
-    fn_name = fn.__module__ + "." + fn.__name__
-    delta = (end - start).microseconds * 1e-6
-    print(fn_name + ": " + str(delta) + "s")
-    return results
+        cmpid = self.create_component(
+            compname,
+            component_library="Independent Sources",
+            component_name="V_DC",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
+        cmpid.set_property("DC", value)
+        return cmpid
 
-def isclose(a, b, rel_tol=1e-9, abs_tol=0.0):
-    return abs(a - b) <= max(rel_tol * max(abs(a), abs(b)), abs_tol)
+    @pyaedt_function_handler()
+    def create_voltage_probe(self, probe_name=None, location=None, angle=0, use_instance_id_netlist=False):
+        """Create a voltage probe.
 
+        Parameters
+        ----------
+        probe_name :
+            Name of the voltage probe. The default is ``None``.
+        location : list of float, optional
+            Position on the X axis and Y axis. The default is ``None``.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-def is_number(a):
-    if isinstance(a, float) or isinstance(a, int):
-        return True
-    elif isinstance(a, str):
-        try:
-            float(a)
-            return True
-        except ValueError:
-            return False
-    else:
-        return False
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
+        References
+        ----------
 
-def is_array(a):
-    try:
-        v = list(ast.literal_eval(a))
-    except (ValueError, TypeError, NameError, SyntaxError):
-        return False
-    else:
-        if type(v) is list:
-            return True
+        >>> oEditor.CreateComponent
+        """
+        if location is None:
+            location = []
         else:
-            return False
+            location = [location[0] + 0.2 * 24.4 / 1000, location[1] + 0.2 * 24.4 / 1000]
 
+        cmpid = self.create_component(
+            None,
+            component_library="Probes",
+            component_name="VPROBE",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
-def is_project_locked(project_path):
-    """Check if an AEDT project lock file exists.
-
-    Parameters
-    ----------
-    project_path : str
-        Path for the AEDT project.
-
-    Returns
-    -------
-    bool
-        ``True`` when successful, ``False`` when failed.
-    """
-    return check_if_path_exists(project_path + ".lock")
+        cmpid.set_property("Name", probe_name)
+        return cmpid
 
+    @pyaedt_function_handler()
+    def create_current_pulse(self, compname=None, value_lists=[], location=[], angle=0, use_instance_id_netlist=False):
+        """Create a current pulse.
 
-@pyaedt_function_handler()
-def remove_project_lock(project_path):
-    """Check if an AEDT project exists and try to remove the lock file.
+        Parameters
+        ----------
+        compname : str, optional
+            Name of the current pulse. The default is ``None``.
+        value_lists : list, optional
+            List of values for the current pulse. The default is ``[]``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    .. note::
-       This operation is risky because the file could be opened in another AEDT instance.
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    Parameters
-    ----------
-    project_path : str
-        Path for the AEDT project.
+        References
+        ----------
 
-    Returns
-    -------
-    bool
-        ``True`` when successful, ``False`` when failed.
-    """
-    if os.path.exists(project_path + ".lock"):
-        os.remove(project_path + ".lock")
-    return True
+        >>> oEditor.CreateComponent
+        """
+        cmpid = self.create_component(
+            compname,
+            component_library="Independent Sources",
+            component_name="I_PULSE",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
+        if len(value_lists) > 0:
+            cmpid.set_property("I1", value_lists[0])
+        if len(value_lists) > 1:
+            cmpid.set_property("I2", value_lists[1])
+        if len(value_lists) > 2:
+            cmpid.set_property("TD", value_lists[2])
+        if len(value_lists) > 3:
+            cmpid.set_property("TR", value_lists[3])
+        if len(value_lists) > 4:
+            cmpid.set_property("TF", value_lists[4])
+        if len(value_lists) > 5:
+            cmpid.set_property("PW", value_lists[5])
+        if len(value_lists) > 6:
+            cmpid.set_property("PER", value_lists[6])
 
-@pyaedt_function_handler()
-def read_csv(filename, encoding="utf-8"):
-    """Read information from a CSV file and return a list.
+        return cmpid
 
-    Parameters
-    ----------
-    filename : str
-            Full path and name for the CSV file.
-    encoding : str, optional
-            File encoding for the CSV file. The default is ``"utf-8"``.
-
-    Returns
-    -------
-    list
+    @pyaedt_function_handler()
+    def create_voltage_pulse(self, compname=None, value_lists=[], location=[], angle=0, use_instance_id_netlist=False):
+        """Create a voltage pulse.
 
-    """
+        Parameters
+        ----------
+        compname : str, optional
+            Name of the voltage pulse. The default is ``None``.
+        value_lists : list, optional
+            List of values for the voltage pulse. The default is ``[]``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    lines = []
-    with codecs.open(filename, "rb", encoding) as csvfile:
-        reader = csv.reader(csvfile, delimiter=",")
-        for row in reader:
-            lines.append(row)
-    return lines
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
+        References
+        ----------
 
-@pyaedt_function_handler()
-def read_csv_pandas(filename, encoding="utf-8"):
-    """Read information from a CSV file and return a list.
+        >>> oEditor.CreateComponent
+        """
+        cmpid = self.create_component(
+            compname,
+            component_library="Independent Sources",
+            component_name="V_PULSE",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
-    Parameters
-    ----------
-    filename : str
-            Full path and name for the CSV file.
-    encoding : str, optional
-            File encoding for the CSV file. The default is ``"utf-8"``.
-
-    Returns
-    -------
-    :class:`pandas.DataFrame`
+        if len(value_lists) > 0:
+            cmpid.set_property("V1", value_lists[0])
+        if len(value_lists) > 1:
+            cmpid.set_property("V2", value_lists[1])
+        if len(value_lists) > 2:
+            cmpid.set_property("TD", value_lists[2])
+        if len(value_lists) > 3:
+            cmpid.set_property("TR", value_lists[3])
+        if len(value_lists) > 4:
+            cmpid.set_property("TF", value_lists[4])
+        if len(value_lists) > 5:
+            cmpid.set_property("PW", value_lists[5])
+        if len(value_lists) > 6:
+            cmpid.set_property("PER", value_lists[6])
 
-    """
-    try:
-        import pandas as pd
+        return cmpid
 
-        return pd.read_csv(filename, encoding=encoding, header=0, na_values=".")
-    except ImportError:
-        logging.error("Pandas is not available. Install it.")
-        return None
+    @pyaedt_function_handler()
+    def create_current_dc(self, compname=None, value=1, location=[], angle=0, use_instance_id_netlist=False):
+        """Create a current DC source.
 
+        Parameters
+        ----------
+        compname : str, optional
+            Name of the current DC source. The default is ``None``.
+        value : float, optional
+            Current value. The default is ``1``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-@pyaedt_function_handler()
-def read_tab(filename):
-    """Read information from a TAB file and return a list.
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    Parameters
-    ----------
-    filename : str
-            Full path and name for the TAB file.
+        References
+        ----------
 
-    Returns
-    -------
-    list
+        >>> oEditor.CreateComponent
+        """
+        cmpid = self.create_component(
+            compname,
+            component_library="Independent Sources",
+            component_name="I_DC",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
-    """
-    with open(filename) as my_file:
-        lines = my_file.readlines()
-    return lines
+        cmpid.set_property("DC", value)
+        return cmpid
 
+    def create_coupling_inductors(
+        self, compname, l1, l2, value=1, location=None, angle=0, use_instance_id_netlist=False
+    ):
+        """Create a coupling inductor.
 
-@pyaedt_function_handler()
-def read_xlsx(filename):
-    """Read information from an XLSX file and return a list.
+        Parameters
+        ----------
+        compname : str
+            Name of the coupling inductor.
+        l1 : float, optional
+            Value for the first inductor.
+        l2 : float, optional
+            Value for the second inductor.
+        value : float, optional
+            Value for the coupling inductor. The default is ``1``.
+        location : list of float, optional
+            Position on the X axis and Y axis. The default is ``None``.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    Parameters
-    ----------
-    filename : str
-            Full path and name for the XLSX file.
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    Returns
-    -------
-    list
+        References
+        ----------
 
-    """
-    try:
-        import pandas as pd
+        >>> oEditor.CreateComponent
+        """
+        if location == None:
+            location = []
 
-        lines = pd.read_excel(filename)
-        return lines
-    except ImportError:
-        lines = []
-        return lines
-
-
-@pyaedt_function_handler()
-def write_csv(output, list_data, delimiter=",", quotechar="|", quoting=csv.QUOTE_MINIMAL):
-    if is_ironpython:
-        f = open(output, "wb")
-    else:
-        f = open(output, "w", newline="")
-    writer = csv.writer(f, delimiter=delimiter, quotechar=quotechar, quoting=quoting)
-    for data in list_data:
-        writer.writerow(data)
-    f.close()
-    return True
-
-
-@pyaedt_function_handler()
-def filter_tuple(value, search_key1, search_key2):
-    """Filter a tuple of two elements with two search keywords."""
-    ignore_case = True
-
-    def _create_pattern(k1, k2):
-        k1a = re.sub(r"\?", r".", k1)
-        k1b = re.sub(r"\*", r".*?", k1a)
-        k2a = re.sub(r"\?", r".", k2)
-        k2b = re.sub(r"\*", r".*?", k2a)
-        pattern = r".*\({},{}\)".format(k1b, k2b)
-        return pattern
-
-    if ignore_case:
-        compiled_re = re.compile(_create_pattern(search_key1, search_key2), re.IGNORECASE)
-    else:
-        compiled_re = re.compile(_create_pattern(search_key1, search_key2))
+        cmpid = self.create_component(
+            compname,
+            component_library="Inductors",
+            component_name="K_IND",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
-    m = compiled_re.search(value)
-    if m:
-        return True
-    return False
+        cmpid.set_property("Inductor1", l1)
+        cmpid.set_property("Inductor2", l2)
+        cmpid.set_property("CouplingFactor", value)
+        return cmpid
 
+    @pyaedt_function_handler()
+    def create_diode(self, compname=None, model_name="required", location=[], angle=0, use_instance_id_netlist=False):
+        """Create a diode.
 
-@pyaedt_function_handler()
-def filter_string(value, search_key1):
-    """Filter a string"""
-    ignore_case = True
-
-    def _create_pattern(k1):
-        k1a = re.sub(r"\?", r".", k1.replace("\\", "\\\\"))
-        k1b = re.sub(r"\*", r".*?", k1a)
-        pattern = r"^{}$".format(k1b)
-        return pattern
-
-    if ignore_case:
-        compiled_re = re.compile(_create_pattern(search_key1), re.IGNORECASE)
-    else:
-        compiled_re = re.compile(_create_pattern(search_key1))  # pragma: no cover
+        Parameters
+        ----------
+        compname : str
+            Name of the diode. The default is ``None``.
+        model_name : str, optional
+            Name of the model. The default is ``"required"``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    m = compiled_re.search(value)
-    if m:
-        return True
-    return False
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
+        References
+        ----------
 
-@pyaedt_function_handler()
-def recursive_glob(startpath, filepattern):
-    """Get a list of files matching a pattern, searching recursively from a start path.
+        >>> oEditor.CreateComponent
+        """
+        cmpid = self.create_component(
+            compname,
+            component_library="Diodes",
+            component_name="DIODE_Level1",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
 
-    Keyword Arguments:
-    startpath -- starting path (directory)
-    filepattern -- fnmatch-style filename pattern
-    """
-    if settings.remote_rpc_session:
-        files = []
-        for i in settings.remote_rpc_session.filemanager.listdir(startpath):
-            if settings.remote_rpc_session.filemanager.isdir(os.path.join(startpath, i)):
-                files.extend(recursive_glob(os.path.join(startpath, i), filepattern))
-            elif fnmatch.fnmatch(i, filepattern):
-                files.append(os.path.join(startpath, i))
-        return files
-    else:
-        return [
-            os.path.join(dirpath, filename)
-            for dirpath, _, filenames in os.walk(startpath)
-            for filename in filenames
-            if fnmatch.fnmatch(filename, filepattern)
-        ]
+        cmpid.set_property("MOD", model_name)
+        return cmpid
 
+    @pyaedt_function_handler()
+    def create_npn(self, compname=None, value=None, location=[], angle=0, use_instance_id_netlist=False):
+        """Create an NPN transistor.
 
-@pyaedt_function_handler()
-def number_aware_string_key(s):
-    """Get a key for sorting strings that treats embedded digit sequences as integers.
+        Parameters
+        ----------
+        compname : str
+            Name of the NPN transistor. The default is ``None``.
+        value : float, optional
+            Value for the NPN transistor. The default is ``None``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    Parameters
-    ----------
-    s : str
-        String to calculate the key from.
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    Returns
-    -------
-    tuple
-        Tuple of key entries.
-    """
+        References
+        ----------
 
-    def is_digit(c):
-        return "0" <= c and c <= "9"
+        >>> oEditor.CreateComponent
+        """
+        id = self.create_component(
+            compname,
+            component_library="BJTs",
+            component_name="Level01_NPN",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
+        if value:
+            id.set_property("MOD", value)
+        return id
 
-    result = []
-    i = 0
-    while i < len(s):
-        if is_digit(s[i]):
-            j = i + 1
-            while j < len(s) and is_digit(s[j]):
-                j += 1
-            key = int(s[i:j])
-            result.append(key)
-            i = j
-        else:
-            j = i + 1
-            while j < len(s) and not is_digit(s[j]):
-                j += 1
-            key = s[i:j]
-            result.append(key)
-            i = j
-    return tuple(result)
-
-
-@pyaedt_function_handler()
-def _create_json_file(json_dict, full_json_path):
-    if not is_ironpython:
-        with open(full_json_path, "w") as fp:
-            json.dump(json_dict, fp, indent=4)
-    else:
-        temp_path = full_json_path.replace(".json", "_temp.json")
-        with open(temp_path, "w") as fp:
-            json.dump(json_dict, fp, indent=4)
-        with open(temp_path, "r") as file:
-            filedata = file.read()
-        filedata = filedata.replace("True", "true")
-        filedata = filedata.replace("False", "false")
-        with open(full_json_path, "w") as file:
-            file.write(filedata)
-        os.remove(temp_path)
-    return True
-
-
-@pyaedt_function_handler()
-def com_active_sessions(version=None, student_version=False, non_graphical=False):
-    """Get information for the active COM AEDT sessions.
+    @pyaedt_function_handler()
+    def create_pnp(self, compname=None, value=50, location=[], angle=0, use_instance_id_netlist=False):
+        """Create a PNP transistor.
 
-    Parameters
-    ----------
-    version : str, optional
-        Version to check. The default is ``None``, in which case all versions are checked.
-        When specifying a version, you can use a three-digit format like ``"222"`` or a
-        five-digit format like ``"2022.2"``.
-    student_version : bool, optional
-        Whether to check for student version sessions. The default is ``False``.
-    non_graphical : bool, optional
-        Whether to check only for active non-graphical sessions. The default is ``False``.
-
-    Returns
-    -------
-    list
-        List of AEDT PIDs.
-    """
-    if student_version:
-        keys = ["ansysedtsv.exe"]
-    else:
-        keys = ["ansysedt.exe"]
-    long_version = None
-    if len(version) > 6:
-        version = version[-6:]
-    if version and "." in version:
-        long_version = version
-        version = version[-4:].replace(".", "")
-    if version < "221":
-        version = version[:2] + "." + version[2]
-        long_version = "20{}".format(version)
-    sessions = []
-    for p in psutil.process_iter():
-        try:
-            if p.name() in keys:
-                if long_version and _check_installed_version(os.path.dirname(p.exe()), long_version):
-                    sessions.append(p.pid)
-                    continue
-                cmd = p.cmdline()
-                if non_graphical and "-ng" in cmd or not non_graphical:
-                    if not version or (version and version in cmd[0]):
-                        sessions.append(p.pid)
-        except:
-            pass
-    return sessions
-
-
-@pyaedt_function_handler()
-def grpc_active_sessions(version=None, student_version=False, non_graphical=False):
-    """Get information for the active gRPC AEDT sessions.
+        Parameters
+        ----------
+        compname : str
+            Name of the PNP transistor. The default is ``None``.
+        value : float, optional
+            Value for the PNP transistor. The default is ``None``.
+        location : list of float, optional
+            Position on the X axis and Y axis.
+        angle : float, optional
+            Angle rotation in degrees. The default is ``0``.
+        use_instance_id_netlist : bool, optional
+            Whether to use the instance ID in the net list.
+            The default is ``False``.
 
-    Parameters
-    ----------
-    version : str, optional
-        Version to check. The default is ``None``, in which case all versions are checked.
-        When specififying a version, you can use a three-digit format like ``"222"`` or a
-        five-digit format like ``"2022.2"``.
-    student_version : bool, optional
-        Whether to check for student version sessions. The default is ``False``.
-    non_graphical : bool, optional
-        Whether to check only for active non-graphical sessions. The default is ``False``.
-
-    Returns
-    -------
-    list
-        List of gRPC ports.
-    """
-    if student_version:
-        keys = ["ansysedtsv.exe", "ansysedtsv"]
-    else:
-        keys = ["ansysedt.exe", "ansysedt"]
-    if version and "." in version:
-        version = version[-4:].replace(".", "")
-    sessions = []
-    for p in psutil.process_iter():
-        try:
-            if p.name() in keys:
-                cmd = p.cmdline()
-                if "-grpcsrv" in cmd:
-                    if non_graphical and "-ng" in cmd or not non_graphical:
-                        if not version or (version and version in cmd[0]):
-                            try:
-                                sessions.append(
-                                    int(cmd[cmd.index("-grpcsrv") + 1]),
-                                )
-                            except (IndexError, ValueError):
-                                # default desktop grpc port.
-                                sessions.append(50051)
-        except:
-            pass
-    return sessions
+        Returns
+        -------
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
+        References
+        ----------
 
-def active_sessions(version=None, student_version=False, non_graphical=False):
-    """Get information for the active COM AEDT sessions.
+        >>> oEditor.CreateComponent
+        """
+        id = self.create_component(
+            compname,
+            component_library="BJTs",
+            component_name="Level01_PNP",
+            location=location,
+            angle=angle,
+            use_instance_id_netlist=use_instance_id_netlist,
+        )
+        if value:
+            id.set_property("MOD", value)
 
-    Parameters
-    ----------
-    version : str, optional
-        Version to check. The default is ``None``, in which case all versions are checked.
-        When specifying a version, you can use a three-digit format like ``"222"`` or a
-        five-digit format like ``"2022.2"``.
-    student_version : bool, optional
-    non_graphical : bool, optional
+        return id
 
+    @pyaedt_function_handler()
+    def create_new_component_from_symbol(
+        self,
+        symbol_name,
+        pin_lists,
+        time_stamp=1591858313,
+        description="",
+        refbase="x",
+        parameter_list=[],
+        parameter_value=[],
+        gref="",
+    ):
+        """Create a component from a symbol.
 
-    Returns
-    -------
-    list
-        List of AEDT PIDs.
-    """
-    if student_version:
-        keys = ["ansysedtsv.exe", "ansysedtsv"]
-    else:
-        keys = ["ansysedt.exe", "ansysedt"]
-    if version and "." in version:
-        version = version[-4:].replace(".", "")
-    if version and version < "222":
-        version = version[:2] + "." + version[2]
-    sessions = []
-    for p in psutil.process_iter():
-        try:
-            if p.name() in keys:
-                cmd = p.cmdline()
-                if non_graphical and "-ng" in cmd or not non_graphical:
-                    if not version or (version and version in cmd[0]):
-                        if "-grpcsrv" in cmd:
-                            if not version or (version and version in cmd[0]):
-                                try:
-                                    sessions.append(
-                                        [
-                                            p.pid,
-                                            int(cmd[cmd.index("-grpcsrv") + 1]),
-                                        ]
-                                    )
-                                except (IndexError, ValueError):
-                                    # default desktop grpc port.
-                                    sessions.append(
-                                        [
-                                            p.pid,
-                                            50051,
-                                        ]
-                                    )
-                        else:
-                            sessions.append(
-                                [
-                                    p.pid,
-                                    -1,
-                                ]
-                            )
-        except:
-            pass
-    return sessions
-
-
-@pyaedt_function_handler()
-def compute_fft(time_vals, value):  # pragma: no cover
-    """Compute FFT of input transient data.
+        Parameters
+        ----------
+        symbol_name : str
+            Name of the symbol.
+        pin_lists : list
+            List of pin names.
+        time_stamp : int, optional
+            UTC time stamp.
+        description : str, optional
+            Component description.
+        refbase : str, optional
+            Reference base. The default is ``"U"``.
+        parameter_list : list
+            List of parameters. The default is ``[]``.
+        parameter_value : list
+            List of parameter values. The default is ``[]``.
+        gref : str, optional
+            Global Reference
 
-    Parameters
-    ----------
-    time_vals : `pandas.Series`
-    value : `pandas.Series`
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
 
-    Returns
-    -------
-    tuple
-        Frequency and Values.
-    """
-    try:
-        import numpy as np
-    except ImportError:
-        logging.error("NumPy is not available. Install it.")
-        return False
+        References
+        ----------
 
-    deltaT = time_vals[-1] - time_vals[0]
-    num_points = len(time_vals)
-    valueFFT = np.fft.fft(value, num_points)
-    Npoints = int(len(valueFFT) / 2)
-    valueFFT = valueFFT[1 : Npoints + 1]
-    valueFFT = valueFFT / len(valueFFT)
-    n = np.arange(num_points)
-    freq = n / deltaT
-    return freq, valueFFT
-
-
-def parse_excitation_file(
-    file_name,
-    is_time_domain=True,
-    x_scale=1,
-    y_scale=1,
-    impedance=50,
-    data_format="Power",
-    encoding="utf-8",
-    out_mag="Voltage",
-):
-    """Parse a csv file and convert data in list that can be applied to Hfss and Hfss3dLayout sources.
+        >>> oModelManager.Add
+        >>> oComponentManager.Add
+        """
+        arg = [
+            "NAME:" + symbol_name,
+            "Info:=",
+            [
+                "Type:=",
+                0,
+                "NumTerminals:=",
+                len(pin_lists),
+                "DataSource:=",
+                "",
+                "ModifiedOn:=",
+                time_stamp,
+                "Manufacturer:=",
+                "",
+                "Symbol:=",
+                symbol_name,
+                "ModelNames:=",
+                "",
+                "Footprint:=",
+                "",
+                "Description:=",
+                description,
+                "InfoTopic:=",
+                "",
+                "InfoHelpFile:=",
+                "",
+                "IconFile:=",
+                "",
+                "Library:=",
+                "",
+                "OriginalLocation:=",
+                "Project",
+                "IEEE:=",
+                "",
+                "Author:=",
+                "",
+                "OriginalAuthor:=",
+                "",
+                "CreationDate:=",
+                time_stamp,
+                "ExampleFile:=",
+                "",
+                "HiddenComponent:=",
+                0,
+                "CircuitEnv:=",
+                0,
+                "GroupID:=",
+                0,
+            ],
+            "CircuitEnv:=",
+            0,
+            "Refbase:=",
+            refbase,
+            "NumParts:=",
+            1,
+            "ModSinceLib:=",
+            True,
+        ]
 
-    Parameters
-    ----------
-    file_name : str
-        Full name of the input file.
-    is_time_domain : bool, optional
-        Either if the input data is Time based or Frequency Based. Frequency based data are Mag/Phase (deg).
-    x_scale : float, optional
-        Scaling factor for x axis.
-    y_scale : float, optional
-        Scaling factor for y axis.
-    data_format : str, optional
-        Either `"Power"`, `"Current"` or `"Voltage"`.
-    impedance : float, optional
-        Excitation impedance. Default is `50`.
-    encoding : str, optional
-        Csv file encoding.
-    out_mag : str, optional
-        Output magnitude format. It can be `"Voltage"` or `"Power"` depending on Hfss solution.
-
-    Returns
-    -------
-    tuple
-        Frequency, magnitude and phase.
-    """
-    try:
-        import numpy as np
-    except ImportError:
-        logging.error("NumPy is not available. Install it.")
-        return False
-    df = read_csv_pandas(file_name, encoding=encoding)
-    if is_time_domain:
-        time = df[df.keys()[0]].values * x_scale
-        val = df[df.keys()[1]].values * y_scale
-        freq, fval = compute_fft(time, val)
-
-        if data_format.lower() == "current":
-            if out_mag == "Voltage":
-                fval = fval * impedance
+        for pin in pin_lists:
+            arg.append("Terminal:=")
+            arg.append([pin, pin, "A", False, 0, 1, "", "Electrical", "0"])
+        arg.append("CompExtID:=")
+        arg.append(1)
+        arg2 = ["NAME:Parameters"]
+
+        for el, val in zip(parameter_list, parameter_value):
+            if "MOD" in el:
+                arg2.append("TextValueProp:=")
+                arg2.append([el, "D", "", val])
             else:
-                fval = fval * fval * impedance
-        elif data_format.lower() == "voltage":
-            if out_mag == "Power":
-                fval = fval * fval / impedance
-        else:
-            if out_mag == "Voltage":
-                fval = np.sqrt(fval * impedance)
-        mag = list(np.abs(fval))
-        phase = [math.atan2(j, i) * 180 / math.pi for i, j in zip(list(fval.real), list(fval.imag))]
-
-    else:
-        freq = list(df[df.keys()[0]].values * x_scale)
-        if data_format.lower() == "current":
-            mag = df[df.keys()[1]].values * df[df.keys()[1]].values * impedance * y_scale * y_scale
-        elif data_format.lower() == "voltage":
-            mag = df[df.keys()[1]].values * df[df.keys()[1]].values / impedance * y_scale * y_scale
-        else:
-            mag = df[df.keys()[1]].values * y_scale
-        mag = list(mag)
-        phase = list(df[df.keys()[2]].values)
-    return freq, mag, phase
-
+                arg2.append("ValuePropNU:=")
+                arg2.append([el, "D", "", str(val), 0, ""])
 
-def tech_to_control_file(tech_path, unit="nm", control_path=None):
-    """Convert a TECH file to an XML file for use in a GDS or DXF import.
+        arg2.append("ButtonProp:=")
+        arg2.append(["CosimDefinition", "D", "", "Edit", "Edit", 40501, "ButtonPropClientData:=", []])
+        arg2.append("MenuProp:=")
+        arg2.append(["CoSimulator", "D", "", "DefaultNetlist", 0])
 
-    Parameters
-    ----------
-    tech_path : str
-        Full path to the TECH file.
-    unit : str, optional
-        Tech units. If specified in tech file this parameter will not be used. Default is ``"nm"``.
-    control_path : str, optional
-        Path for outputting the XML file.
-
-    Returns
-    -------
-    str
-        Out xml file.
-    """
-    result = []
-    with open(tech_path) as f:
-        vals = list(CSS4_COLORS.values())
-        id_layer = 0
-        for line in f:
-            line_split = line.split()
-            if len(line_split) == 5:
-                layerID, layer_name, _, elevation, layer_height = line.split()
-                x = '      <Layer Color="{}" GDSIIVia="{}" Name="{}" TargetLayer="{}" Thickness="{}"'.format(
-                    vals[id_layer],
-                    "true" if layer_name.lower().startswith("v") else "false",
-                    layerID,
-                    layer_name,
-                    layer_height,
-                )
-                x += ' Type="conductor"/>'
-                result.append(x)
-                id_layer += 1
-            elif len(line_split) > 1 and "UNIT" in line_split[0]:
-                unit = line_split[1]
-    if not control_path:
-        control_path = os.path.splitext(tech_path)[0] + ".xml"
-    with open(control_path, "w") as f:
-        f.write('<?xml version="1.0" encoding="UTF-8" standalone="no" ?>\n')
-        f.write('    <c:Control xmlns:c="http://www.ansys.com/control" schemaVersion="1.0">\n')
-        f.write("\n")
-        f.write('      <Stackup schemaVersion="1.0">\n')
-        f.write('        <Layers LengthUnit="{}">\n'.format(unit))
-        for res in result:
-            f.write(res + "\n")
-
-        f.write("    </Layers>\n")
-        f.write("  </Stackup>\n")
-        f.write("\n")
-        f.write('  <ImportOptions Flatten="true" GDSIIConvertPolygonToCircles="false" ImportDummyNet="true"/>\n')
-        f.write("\n")
-        f.write("</c:Control>\n")
-
-    return control_path
-
-
-class PropsManager(object):
-    def __getitem__(self, item):
-        """Get the `self.props` key value.
-
-        Parameters
-        ----------
-        item : str
-            Key to search
-        """
-        item_split = item.split("/")
-        if len(item_split) == 1:
-            item_split = item_split[0].split("__")
-        props = self.props
-        found_el = []
-        matching_percentage = 1
-        while matching_percentage >= 0.4:
-            for item_value in item_split:
-                found_el = self._recursive_search(props, item_value, matching_percentage)
-                # found_el = difflib.get_close_matches(item_value, list(props.keys()), 1, matching_percentage)
-                if found_el:
-                    props = found_el[1][found_el[2]]
-                    # props = props[found_el[0]]
-            if found_el:
-                return props
+        arg.append(arg2)
+        spicesintax = refbase + "@ID "
+        id = 0
+        while id < len(pin_lists):
+            spicesintax += "%" + str(id) + " "
+            id += 1
+            spicesintax += symbol_name + " "
+        for el, val in zip(parameter_list, parameter_value):
+            if "MOD" in el:
+                spicesintax += "@{} ".format(el)
             else:
-                matching_percentage -= 0.02
-        self._app.logger.warning("Key %s not found.Check one of available keys in self.available_properties", item)
-        return None
-
-    def __setitem__(self, key, value):
-        """Set the `self.props` key value.
-
-        Parameters
-        ----------
-        key : str
-            Key to apply.
-        value : int, float, bool, str, dict
-            Value to apply.
-        """
-        item_split = key.split("/")
-        if len(item_split) == 1:
-            item_split = item_split[0].split("__")
-        found_el = []
-        props = self.props
-        matching_percentage = 1
-        key_path = []
-        while matching_percentage >= 0.4:
-            for item_value in item_split:
-                found_el = self._recursive_search(props, item_value, matching_percentage)
-                if found_el:
-                    props = found_el[1][found_el[2]]
-                    key_path.append(found_el[2])
-            if found_el:
-                if matching_percentage < 1:
-                    self._app.logger.info(
-                        "Key %s matched internal key '%s' with confidence of %s.",
-                        key,
-                        "/".join(key_path),
-                        round(matching_percentage * 100),
-                    )
-                matching_percentage = 0
+                spicesintax += "{}=@{} ".format(el, el)
 
-            else:
-                matching_percentage -= 0.02
-        if found_el:
-            found_el[1][found_el[2]] = value
-            self.update()
-        else:
-            props[key] = value
-            self.update()
-            self._app.logger.warning("Key %s not found. Trying to applying new key ", key)
+        arg3 = [
+            "NAME:CosimDefinitions",
+            [
+                "NAME:CosimDefinition",
+                "CosimulatorType:=",
+                4,
+                "CosimDefName:=",
+                "DefaultNetlist",
+                "IsDefinition:=",
+                True,
+                "Connect:=",
+                True,
+                "Data:=",
+                ["Nexxim Circuit:=", spicesintax],
+                "GRef:=",
+                ["Nexxim Circuit:=", gref],
+            ],
+            "DefaultCosim:=",
+            "DefaultNetlist",
+        ]
+        arg.append(arg3)
+        print(arg)
+        self.o_component_manager.Add(arg)
+        return True
 
     @pyaedt_function_handler()
-    def _recursive_search(self, dict_in, key="", matching_percentage=0.8):
-        f = difflib.get_close_matches(key, list(dict_in.keys()), 1, matching_percentage)
-        if f:
-            return True, dict_in, f[0]
-        else:
-            for v in list(dict_in.values()):
-                if isinstance(v, (dict, OrderedDict)):
-                    out_val = self._recursive_search(v, key, matching_percentage)
-                    if out_val:
-                        return out_val
-                elif isinstance(v, list) and isinstance(v[0], (dict, OrderedDict)):
-                    for val in v:
-                        out_val = self._recursive_search(val, key, matching_percentage)
-                        if out_val:
-                            return out_val
-        return False
+    def get_comp_custom_settings(
+        self, toolNum, dc=0, interp=0, extrap=1, conv=0, passivity=0, reciprocal="False", opt="", data_type=1
+    ):
+        """Retrieve custom settings for a resistor.
 
-    @pyaedt_function_handler()
-    def _recursive_list(self, dict_in, prefix=""):
-        available_list = []
-        for k, v in dict_in.items():
-            if prefix:
-                name = prefix + "/" + k
-            else:
-                name = k
-            available_list.append(name)
-            if isinstance(v, (dict, OrderedDict)):
-                available_list.extend(self._recursive_list(v, name))
-        return available_list
+        Parameters
+        ----------
+        toolNum :
 
-    @property
-    def available_properties(self):
-        """Available properties.
+        dc :
+            The default is ``0``.
+        interp :
+            The default is ``0``.
+        extrap :
+            The default is ``1``.
+        conv :
+            The default is ``0``.
+        passivity : optional
+            The default is ``0``.
+        reciprocal : bool, optional
+            The default is ``False``.
+        opt : str, optional
+            The default is ``""``.
+        data_type : optional
+            Type of the data. The default is ``1``.
 
         Returns
         -------
         list
-        """
-        return self._recursive_list(self.props)
-
-    @pyaedt_function_handler()
-    def update(self):
-        """Update method."""
-        pass
-
-
-clamp = lambda n, minn, maxn: max(min(maxn, n), minn)
-rgb_color_codes = {
-    "Black": (0, 0, 0),
-    "Green": (0, 128, 0),
-    "White": (255, 255, 255),
-    "Red": (255, 0, 0),
-    "Lime": (0, 255, 0),
-    "Blue": (0, 0, 255),
-    "Yellow": (255, 255, 0),
-    "Cyan": (0, 255, 255),
-    "Magenta": (255, 0, 255),
-    "Silver": (192, 192, 192),
-    "Gray": (128, 128, 128),
-    "Maroon": (128, 0, 0),
-    "Olive": (128, 128, 0),
-    "Purple": (128, 0, 128),
-    "Teal": (0, 128, 128),
-    "Navy": (0, 0, 128),
-    "copper": (184, 115, 51),
-    "stainless steel": (224, 223, 219),
-}
-
-
-@pyaedt_function_handler()
-def _arg2dict(arg, dict_out):
-    if arg[0] == "NAME:DimUnits" or "NAME:Point" in arg[0]:
-        if arg[0][5:] in dict_out:
-            if isinstance(dict_out[arg[0][5:]][0], (list, tuple)):
-                dict_out[arg[0][5:]].append(list(arg[1:]))
-            else:
-                dict_out[arg[0][5:]] = [dict_out[arg[0][5:]]]
-                dict_out[arg[0][5:]].append(list(arg[1:]))
-        else:
-            dict_out[arg[0][5:]] = list(arg[1:])
-    elif arg[0][:5] == "NAME:":
-        top_key = arg[0][5:]
-        dict_in = OrderedDict()
-        i = 1
-        while i < len(arg):
-            if arg[i][0][:5] == "NAME:" and (
-                isinstance(arg[i], (list, tuple)) or str(type(arg[i])) == r"<type 'List'>"
-            ):
-                _arg2dict(list(arg[i]), dict_in)
-                i += 1
-            elif arg[i][-2:] == ":=":
-                if str(type(arg[i + 1])) == r"<type 'List'>":
-                    if arg[i][:-2] in dict_in:
-                        dict_in[arg[i][:-2]].append(list(arg[i + 1]))
-                    else:
-                        dict_in[arg[i][:-2]] = list(arg[i + 1])
-                else:
-                    if arg[i][:-2] in dict_in:
-                        if isinstance(dict_in[arg[i][:-2]], list):
-                            dict_in[arg[i][:-2]].append(arg[i + 1])
-                        else:
-                            dict_in[arg[i][:-2]] = [dict_in[arg[i][:-2]]]
-                            dict_in[arg[i][:-2]].append(arg[i + 1])
-                    else:
-                        dict_in[arg[i][:-2]] = arg[i + 1]
-
-                i += 2
-            else:
-                raise ValueError("Incorrect data argument format")
-        if top_key in dict_out:
-            if isinstance(dict_out[top_key], list):
-                dict_out[top_key].append(dict_in)
-            else:
-                dict_out[top_key] = [dict_out[top_key], dict_in]
-        else:
-            dict_out[top_key] = dict_in
-    else:
-        raise ValueError("Incorrect data argument format")
-
-
-def _uname(name=None):
-    """Append a 6-digit hash code to a specified name.
-
-    Parameters
-    ----------
-    name : str
-        Name to append the hash code to. The default is ``"NewObject_"``.
-
-    Returns
-    -------
-    str
-
-    """
-    char_set = string.ascii_uppercase + string.digits
-    unique_name = "".join(random.sample(char_set, 6))
-    if name:
-        return name + unique_name
-    else:
-        return "NewObject_" + unique_name
-
-
-@pyaedt_function_handler()
-def _to_boolean(val):
-    """Retrieve the Boolean value of the provided input.
-
-        If the value is a Boolean, return the value.
-        Otherwise check to see if the value is in
-        ["false", "f", "no", "n", "none", "0", "[]", "{}", "" ]
-        and return True if the value is not in the list.
-
-    Parameters
-    ----------
-    val : bool or str
-        Input value to test for True/False condition.
-
-    Returns
-    -------
-    bool
-
-    """
-
-    if val is True or val is False:
-        return val
-
-    false_items = ["false", "f", "no", "n", "none", "0", "[]", "{}", ""]
-
-    return not str(val).strip().lower() in false_items
-
-
-@pyaedt_function_handler()
-def _dim_arg(value, units):
-    """Concatenate a specified units string to a numerical input.
-
-    Parameters
-    ----------
-    value : str or number
-        Valid expression string in the AEDT modeler. For example, ``"5mm"``.
-    units : str
-        Valid units string in the AEDT modeler. For example, ``"mm"``.
-
-    Returns
-    -------
-    str
-
-    """
-    try:
-        val = float(value)
-        if isinstance(value, int):
-            val = value
-        return str(val) + units
-    except:
-        return value
-
+            List of the custom settings for the resistor.
 
-@pyaedt_function_handler()
-def _check_installed_version(install_path, long_version):
-    """Check installation folder to determine if it is for specified Ansys EM version.
-
-    Parameters
-    ----------
-    install_path: str
-        Installation folder to check.  For example, ``"C:\\Program Files\\AnsysEM\\v231\\Win64"``.
-    long_version: str
-        Long form of version number.  For example, ``"2023.1"``.
-
-    Returns
-    -------
-    bool
-
-    """
-    product_list_path = os.path.join(install_path, "config", "ProductList.txt")
-    if os.path.isfile(product_list_path):
-        try:
-            with open(product_list_path, "r") as f:
-                install_version = f.readline().strip()[-6:]
-                if install_version == long_version:
-                    return True
-        except:
-            pass
-    return False
-
-
-def install_with_pip(package_name, package_path=None, upgrade=False, uninstall=False):  # pragma: no cover
-    """Install a new package using pip.
-    This method is useful for installing a package from the AEDT Console without launching the Python environment.
-
-    Parameters
-    ----------
-    package_name : str
-        Name of the package to install.
-    package_path : str, optional
-        Path for the GitHub package to download and install. For example, ``git+https://.....``.
-    upgrade : bool, optional
-        Whether to upgrade the package. The default is ``False``.
-    uninstall : bool, optional
-        Whether to install the package or uninstall the package.
-    """
-    if is_linux and is_ironpython:
-        import subprocessdotnet as subprocess
-    else:
-        import subprocess
-    executable = '"{}"'.format(sys.executable) if is_windows else sys.executable
-
-    commands = []
-    if uninstall:
-        commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
-    else:
-        if package_path and upgrade:
-            commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
-            command = [executable, "-m", "pip", "install", package_path]
-        else:
-            command = [executable, "-m", "pip", "install", package_name]
-        if upgrade:
-            command.append("-U")
-
-        commands.append(command)
-    for command in commands:
-        if is_linux:
-            p = subprocess.Popen(command)
+        """
+        if toolNum == 1:
+            custom = "NAME:DesignerCustomization"
+        elif toolNum == 2:
+            custom = "NAME:NexximCustomization"
         else:
-            p = subprocess.Popen(" ".join(command))
-        p.wait()
-
+            custom = "NAME:HSpiceCustomization"
 
-class Help:  # pragma: no cover
-    def __init__(self):
-        self._base_path = "https://aedt.docs.pyansys.com/version/stable"
-        self.browser = "default"
-
-    def _launch_ur(self, url):
-        import webbrowser
+        res = [
+            custom,
+            "DCOption:=",
+            dc,
+            "InterpOption:=",
+            interp,
+            "ExtrapOption:=",
+            extrap,
+            "Convolution:=",
+            conv,
+            "Passivity:=",
+            passivity,
+            "Reciprocal:=",
+            reciprocal,
+            "ModelOption:=",
+            opt,
+            "DataType:=",
+            data_type,
+        ]
 
-        if self.browser != "default":
-            webbrowser.get(self.browser).open_new_tab(url)
-        else:
-            webbrowser.open_new_tab(url)
+        return res
 
-    def search(self, keywords, app_name=None, search_in_examples_only=False):
-        """Search for one or more keywords.
+    @pyaedt_function_handler()
+    def add_subcircuit_dynamic_link(
+        self,
+        pyaedt_app=None,
+        solution_name=None,
+        extrusion_length=None,
+        enable_cable_modeling=True,
+        default_matrix="Original",
+        tline_port="",
+        comp_name=None,
+    ):
+        """Add a subcircuit from `HFSS`, `Q3d` or `2D Extractor` in circuit design.
 
         Parameters
         ----------
-        keywords : str or list
-        app_name : str, optional
-            Name of a PyAEDT app. For example, ``"Hfss"``, ``"Circuit"``, ``"Icepak"``, or any other available app.
-        search_in_examples_only : bool, optional
-            Whether to search for the one or more keywords only in the PyAEDT examples.
-            The default is ``False``.
-        """
-        if isinstance(keywords, str):
-            keywords = [keywords]
-        if search_in_examples_only:
-            keywords.append("This example")
-        if app_name:
-            keywords.append(app_name)
-        url = self._base_path + "/search.html?q={}".format("+".join(keywords))
-        self._launch_ur(url)
-
-    def getting_started(self):
-        """Open the PyAEDT User guide page."""
-        url = self._base_path + "/User_guide/index.html"
-        self._launch_ur(url)
-
-    def examples(self):
-        """Open the PyAEDT Examples page."""
-        url = self._base_path + "/examples/index.html"
-        self._launch_ur(url)
-
-    def github(self):
-        """Open the PyAEDT GitHub page."""
-        url = "https://github.com/pyansys/pyaedt"
-        self._launch_ur(url)
-
-    def changelog(self, release=None):
-        """Open the PyAEDT GitHub Changelog for a given release.
-
-        Parameters
-        ----------
-        release : str, optional
-            Release to get the changelog for. For example, ``"0.6.70"``.
-        """
-        if release is None:
-            from pyaedt import __version__ as release
-        url = "https://github.com/pyansys/pyaedt/releases/tag/v" + release
-        self._launch_ur(url)
-
-    def issues(self):
-        """Open the PyAEDT GitHub Issues page."""
-        url = "https://github.com/pyansys/pyaedt/issues"
-        self._launch_ur(url)
-
-    def ansys_forum(self):
-        """Open the PyAEDT GitHub Issues page."""
-        url = "https://discuss.ansys.com/discussions/tagged/pyaedt"
-        self._launch_ur(url)
-
-    def developer_forum(self):
-        """Open the Discussions page on the Ansys Developer site."""
-        url = "https://developer.ansys.com/"
-        self._launch_ur(url)
-
-
-# class Property(property):
-#
-#     @pyaedt_function_handler()
-#     def getter(self, fget):
-#         """Property getter."""
-#         return self.__class__.__base__(fget, self.fset, self.fdel, self.__doc__)
-#
-#     @pyaedt_function_handler()
-#     def setter(self, fset):
-#         """Property setter."""
-#         return self.__class__.__base__(self.fget, fset, self.fdel, self.__doc__)
-#
-#     @pyaedt_function_handler()
-#     def deleter(self, fdel):
-#         """Property deleter."""
-#         return self.__class__.__base__(self.fget, self.fset, fdel, self.__doc__)
-
-
-class Settings(object):
-    """Manages all PyAEDT environment variables and global settings."""
-
-    def __init__(self):
-        self._enable_logger = True
-        self._enable_desktop_logs = True
-        self._enable_screen_logs = True
-        self._enable_file_logs = True
-        self.pyaedt_server_path = ""
-        self._logger_file_path = None
-        self._logger_formatter = "%(asctime)s:%(destination)s:%(extra)s%(levelname)-8s:%(message)s"
-        self._logger_datefmt = "%Y/%m/%d %H.%M.%S"
-        self._enable_debug_edb_logger = False
-        self._enable_debug_methods_argument_logger = False
-        self._enable_debug_geometry_operator_logger = False
-        self._enable_debug_internal_methods_logger = False
-        self._enable_debug_logger = False
-        self._enable_error_handler = True
-        self._non_graphical = False
-        self._aedt_version = None
-        self.remote_api = False
-        self._use_grpc_api = None
-        self.machine = ""
-        self.port = 0
-        self.formatter = None
-        self.remote_rpc_session = None
-        self.remote_rpc_session_temp_folder = ""
-        self.remote_rpc_service_manager_port = 17878
-        self._project_properties = {}
-        self._project_time_stamp = 0
-        self._disable_bounding_box_sat = False
-        self._force_error_on_missing_project = False
-        self._enable_pandas_output = False
-        self.time_tick = time.time()
-        self._global_log_file_name = "pyaedt_{}.log".format(os.path.split(os.path.expanduser("~"))[-1])
-        self._enable_global_log_file = True
-        self._enable_local_log_file = False
-        self._global_log_file_size = 10
-        self._edb_dll_path = None
-        self._lsf_num_cores = 2
-        self._lsf_ram = 1000
-        self._use_lsf_scheduler = False
-        self._lsf_aedt_command = "ansysedt"
-        self._lsf_timeout = 3600
-        self._lsf_queue = None
-        self._aedt_environment_variables = {
-            "ANS_MESHER_PROC_DUMP_PREPOST_BEND_SM3": "1",
-            "ANSYSEM_FEATURE_SF6694_NON_GRAPHICAL_COMMAND_EXECUTION_ENABLE": "1",
-            "ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE": "1",
-            "ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE": "1",
-            "ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE": "1",
-            "ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE": "1",
-            "ANSYSEM_FEATURE_F545177_ECAD_INTEGRATION_WITH_APHI_ENABLE": "1",
-            "ANSYSEM_FEATURE_F650636_MECH_LAYOUT_COMPONENT_ENABLE": "1",
-        }
-        if is_linux:
-            self._aedt_environment_variables["ANS_NODEPCHECK"] = "1"
-        self._desktop_launch_timeout = 90
-        self._aedt_process_id = None
-        self._is_student = False
-
-    @property
-    def aedt_process_id(self):
-        """ID of the desktop process. The default is ``None``.
+        pyaedt_app : :class:`pyaedt.q3d.Q3d` or :class:`pyaedt.q3d.Q2d` or :class:`pyaedt.q3d.Hfss`.
+            pyaedt application object to include. It could be an Hfss object, a Q3d object or a Q2d.
+        solution_name : str, optional
+            Name of the solution and sweep. The default is ``"Setup1 : Sweep"``.
+        extrusion_length : float, str, optional
+            Extrusion length for 2D Models (q2d or Hfss) in model units. Default is `None`.
+        enable_cable_modeling : bool, optional
+            Either if the Hfss Cable modeling has to be enabled for 2D subcircuits.
+        default_matrix : str, optional
+            Matrix to link to the subcircuit. Default to `"Original"`. It only applies to 2D Extractor and Q3D.
+        tline_port : str, optional
+            Port to be used for tramsission line. Only applies to Hfss.
+        comp_name : str, optional
+            Component name.
 
         Returns
         -------
-        int
-        """
-        return self._aedt_process_id
-
-    @aedt_process_id.setter
-    def aedt_process_id(self, value):
-        self._aedt_process_id = int(value)
-
-    @property
-    def is_student(self):
-        """Whether the desktop process is set to the student version. The
-        default is ``False``.
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-        Returns
-        -------
-        bool
-        """
-        return self._is_student
-
-    @is_student.setter
-    def is_student(self, value):
-        self._is_student = value
-
-    @property
-    def desktop_launch_timeout(self):
-        """Set the desktop launcher max timeout. Default is ``90`` seconds.
+        References
+        ----------
 
-        Returns
-        -------
-        int
-        """
-        return self._desktop_launch_timeout
+        >>> oModelManager.Add
+        >>> oComponentManager.Add
+        >>> oDesign.AddCompInstance
+        >>> oDesign.AddDynamicLink
+        """
+        if not comp_name:
+            comp_name = generate_unique_name(pyaedt_app.design_name)
+        source_project_path = pyaedt_app.project_file
+        source_design_name = pyaedt_app.design_name
+        if not solution_name:
+            solution_name = pyaedt_app.nominal_sweep
+        self._app.odesign.AddDynamicLink(
+            source_design_name,
+            source_project_path,
+            comp_name,
+            solution_name,
+            tline_port,
+            default_matrix,
+            enable_cable_modeling,
+            "Pyaedt Dynamic Link",
+        )
+        self.refresh_all_ids()
+        for el in self.components:
+            if comp_name in self.components[el].composed_name:
+                if extrusion_length:
+                    _, units = decompose_variable_value(self.components[el].parameters["Length"])
+                    self.components[el].set_property("Length", self.number_with_units(extrusion_length, units))
+                if tline_port and extrusion_length:
+                    _, units = decompose_variable_value(self.components[el].parameters["TLineLength"])
+                    self.components[el].set_property("TLineLength", self.number_with_units(extrusion_length, units))
+                return self.components[el]
+        return False
 
-    @desktop_launch_timeout.setter
-    def desktop_launch_timeout(self, value):
-        self._desktop_launch_timeout = int(value)
+    @pyaedt_function_handler()
+    def _add_subcircuit_link(
+        self,
+        comp_name,
+        pin_names,
+        source_project_path,
+        source_design_name,
+        solution_name="Setup1 : Sweep",
+        image_subcircuit_path=None,
+        model_type="hfss",
+        variables=None,
+        extrusion_length_q2d=10,
+        matrix=None,
+        enable_cable_modeling=False,
+        default_matrix="Original",
+        simulate_solutions=False,
+    ):
+        """Add a subcircuit HFSS link.
 
-    @property
-    def aedt_environment_variables(self):
-        """Set environment variables to be set before launching a new aedt session.
-        This includes beta features enablemement.
+        Parameters
+        ----------
+        comp_name : str
+            Name of the subcircuit HFSS link.
+        pin_names : list
+            List of the pin names.
+        source_project_path : str
+            Path to the source project.
+        source_design_name : str
+            Name of the design.
+        solution_name : str, optional
+            Name of the solution and sweep. The
+            default is ``"Setup1 : Sweep"``.
+        image_subcircuit_path : str, optional
+            Path of the Picture used in Circuit.
+            Default is an HFSS Picture exported automatically.
+        model_type : str, optional
+            Dynamick Link type. Options are `Hfss`, `Q3d`, `Q2d`.
+        variables : dict, optional
+            Dictionary of variables and default values of original design, if exists.
+        extrusion_length_q2d : str, float optional
+            Extrusion length for 2D Models. Default is 10 (in model units).
+        matrix : list, optional
+        simulate_solutions : bool, optional
+            Either if simulate or interpolate solutions.
 
         Returns
         -------
-        dict
-        """
-        return self._aedt_environment_variables
-
-    @aedt_environment_variables.setter
-    def aedt_environment_variables(self, value):
-        self._aedt_environment_variables = value
-
-    @property
-    def lsf_queue(self):
-        """LSF queue name. This attribute is valid only on Linux
-        systems running LSF Scheduler."""
-        return self._lsf_queue
-
-    @lsf_queue.setter
-    def lsf_queue(self, value):
-        self._lsf_queue = value
-
-    @property
-    def use_lsf_scheduler(self):
-        """Whether to use LSF Scheduler. This attribute is valid only on Linux
-        systems running LSF Scheduler."""
-        return self._use_lsf_scheduler
-
-    @use_lsf_scheduler.setter
-    def use_lsf_scheduler(self, value):
-        self._use_lsf_scheduler = value
-
-    @property
-    def lsf_aedt_command(self):
-        """Get or set the ``ansysedt`` command to launch. The default is ``"ansysedt"``.
-        This attribute is valid only on Linux systems running LSF Scheduler."""
-        return self._lsf_aedt_command
-
-    @lsf_aedt_command.setter
-    def lsf_aedt_command(self, value):
-        self._lsf_aedt_command = value
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
 
-    @property
-    def lsf_num_cores(self):
-        """Get or set the number of LSF cores. This attribute is valid only
-        on Linux systems running LSF Scheduler."""
-        return self._lsf_num_cores
-
-    @lsf_num_cores.setter
-    def lsf_num_cores(self, value):
-        self._lsf_num_cores = int(value)
+        References
+        ----------
 
-    @property
-    def lsf_ram(self):
-        """Get or set the RAM allocated for the LSF job. This attribute is valid
-        only on Linux systems running LSF Scheduler."""
-        return self._lsf_ram
-
-    @lsf_ram.setter
-    def lsf_ram(self, value):
-        self._lsf_ram = int(value)
+        >>> oModelManager.Add
+        >>> oComponentManager.Add
+        >>> oDesign.AddCompInstance
+        """
+        model = "hfss"
+        owner = "HFSS"
+        icon_file = "hfss.bmp"
+        if model_type.lower() == "q3d extractor":
+            model = "q3d"
+            owner = "Q3D"
+            icon_file = "q3d.bmp"
+
+        elif model_type.lower() == "2d extractor":
+            model = "2dext"
+            owner = "2DExtractor"
+            icon_file = "2dextractor.bmp"
+        elif model_type.lower() == "siwave":
+            model = "siwave"
+            owner = "Siwave"
+            icon_file = ""
+        designer_customization = self.get_comp_custom_settings(1, 0, 0, 1, 0, 0, "False", "", 1)
+        nexxim_customization = self.get_comp_custom_settings(2, 3, 1, 3, 0, 0, "False", "", 2)
+        hspice_customization = self.get_comp_custom_settings(3, 1, 2, 3, 0, 0, "False", "", 3)
+
+        if image_subcircuit_path:
+            _, file_extension = os.path.splitext(image_subcircuit_path)
+            if file_extension != ".gif" or file_extension != ".bmp" or file_extension != ".jpg":
+                image_subcircuit_path = None
+                warnings.warn("Image extension is not valid. Use default image instead.")
+        if not image_subcircuit_path:
+            image_subcircuit_path = os.path.normpath(
+                os.path.join(self._modeler._app.desktop_install_dir, "syslib", "Bitmaps", icon_file)
+            )
+        filename = ""
+        comp_name_aux = generate_unique_name(source_design_name)
+        WB_SystemID = source_design_name
+        if not self._app.project_file == source_project_path:
+            filename = source_project_path
+            comp_name_aux = comp_name
+            WB_SystemID = ""
+
+        compInfo = [
+            "NAME:" + str(comp_name_aux),
+            "Name:=",
+            comp_name_aux,
+            "ModTime:=",
+            1591855779,
+            "Library:=",
+            "",
+            "LibLocation:=",
+            "Project",
+            "ModelType:=",
+            model,
+            "Description:=",
+            "",
+            "ImageFile:=",
+            image_subcircuit_path,
+            "SymbolPinConfiguration:=",
+            0,
+            ["NAME:PortInfoBlk"],
+            ["NAME:PortOrderBlk"],
+            "DesignName:=",
+            source_design_name,
+            "SolutionName:=",
+            solution_name,
+            "NewToOldMap:=",
+            [],
+            "OldToNewMap:=",
+            [],
+            "PinNames:=",
+            pin_names,
+            designer_customization,
+            nexxim_customization,
+            hspice_customization,
+            "NoiseModelOption:=",
+            "External",
+            "WB_SystemID:=",
+            WB_SystemID,
+            "IsWBModel:=",
+            False,
+            "filename:=",
+            filename,
+            "numberofports:=",
+            len(pin_names),
+            "Simulate:=",
+            simulate_solutions,
+            "CloseProject:=",
+            model_type.lower() == "siwave",
+            "SaveProject:=",
+            True,
+            "InterpY:=",
+            True,
+            "InterpAlg:=",
+            "auto",
+            "IgnoreDepVars:=",
+            False,
+        ]
+        if owner in ["HFSS", "Siwave"]:
+            compInfo.extend(
+                [
+                    "Renormalize:=",
+                    False,
+                    "RenormImpedance:=",
+                    50,
+                ]
+            )
+        elif owner == "Q3D":
+            compInfo.extend(
+                [
+                    "Renormalize:=",
+                    False,
+                    "RenormImpedance:=",
+                    50,
+                ]
+            )
+            if not matrix:
+                matrix = ["NAME:Reduce Matrix Choices", default_matrix]
+            compInfo.extend(["Reduce Matrix:=", "Original", matrix])
+        else:
+            if not matrix:
+                matrix = ["NAME:Reduce Matrix Choices", "Original"]
+            compInfo.extend(["Reduce Matrix:=", default_matrix, matrix, "EnableCableModeling:=", enable_cable_modeling])
+
+        self.o_model_manager.Add(compInfo)
+
+        info = [
+            "Type:=",
+            8,
+            "NumTerminals:=",
+            len(pin_names),
+            "DataSource:=",
+            "",
+            "ModifiedOn:=",
+            1591855894,
+            "Manufacturer:=",
+            "",
+            "Symbol:=",
+            "",
+            "ModelNames:=",
+            "",
+            "Footprint:=",
+            "",
+            "Description:=",
+            "",
+            "InfoTopic:=",
+            "",
+            "InfoHelpFile:=",
+            "",
+            "IconFile:=",
+            icon_file,
+            "Library:=",
+            "",
+            "OriginalLocation:=",
+            "Project",
+            "IEEE:=",
+            "",
+            "Author:=",
+            "",
+            "OriginalAuthor:=",
+            "",
+            "CreationDate:=",
+            1591855894,
+            "ExampleFile:=",
+            "",
+            "HiddenComponent:=",
+            0,
+            "CircuitEnv:=",
+            0,
+            "GroupID:=",
+            0,
+        ]
 
-    @property
-    def lsf_timeout(self):
-        """Get or set the timeout for starting the interactive session. The default is ``3600`` seconds."""
-        return self._lsf_timeout
-
-    @lsf_timeout.setter
-    def lsf_timeout(self, value):
-        self._lsf_timeout = int(value)
+        compInfo2 = [
+            "NAME:" + str(comp_name),
+            "Info:=",
+            info,
+            "CircuitEnv:=",
+            0,
+            "Refbase:=",
+            "S",
+            "NumParts:=",
+            1,
+            "ModSinceLib:=",
+            False,
+        ]
 
-    @property
-    def aedt_version(self):
-        """Get and set the aedt version.
-        It disables the sat bounding box for AEDT version > 2022.2.
+        id = 0
+        for pin in pin_names:
+            compInfo2.append("Terminal:=")
+            compInfo2.append([pin, pin, "A", False, id, 1, "", "Electrical", "0"])
+            id += 1
+
+        compInfo2.append(["NAME:Properties", "TextProp:=", ["Owner", "RD", "", owner]])
+        compInfo2.append("CompExtID:=")
+        compInfo2.append(5)
+        variable_args = [
+            "NAME:Parameters",
+            "TextProp:=",
+            ["ModelName", "RD", "", "FieldSolver"],
+        ]
+        if owner == "2DExtractor":
+            variable_args.append("VariableProp:=")
+            variable_args.append(["Length", "D", "", self.number_with_units(extrusion_length_q2d)])
+        if variables:
+            for k, v in variables.items():
+                variable_args.append("VariableProp:=")
+                variable_args.append([k, "D", "", str(v)])
+        variable_args.append("MenuProp:=")
+        variable_args.append(["CoSimulator", "SD", "", "Default", 0])
+        variable_args.append("ButtonProp:=")
+        variable_args.append(["CosimDefinition", "SD", "", "Edit", "Edit", 40501, "ButtonPropClientData:=", []])
+
+        compInfo2.append(variable_args)
+        compInfo2.append(
+            [
+                "NAME:CosimDefinitions",
+                [
+                    "NAME:CosimDefinition",
+                    "CosimulatorType:=",
+                    103,
+                    "CosimDefName:=",
+                    "Default",
+                    "IsDefinition:=",
+                    True,
+                    "Connect:=",
+                    True,
+                    "ModelDefinitionName:=",
+                    comp_name_aux,
+                    "ShowRefPin2:=",
+                    2,
+                    "LenPropName:=",
+                    "",
+                ],
+                "DefaultCosim:=",
+                "Default",
+            ]
+        )
 
-        Returns
-        -------
-        str
-            Aedt version in the form ``"2023.x"``.
-        """
-        return self._aedt_version
+        self.o_component_manager.Add(compInfo2)
+        self._app._odesign.AddCompInstance(comp_name)
+        self.refresh_all_ids()
+        for el in self.components:
+            item = comp_name
+            item2 = self.components[el].composed_name
+            if comp_name in self.components[el].composed_name:
+                return self.components[el]
+        return False
 
-    @aedt_version.setter
-    def aedt_version(self, value):
-        self._aedt_version = value
-        if self._aedt_version >= "2023.1":
-            self.disable_bounding_box_sat = True
+    @pyaedt_function_handler()
+    def set_sim_option_on_hfss_subcircuit(self, component, option="simulate"):
+        """Set the simulation option on the HFSS subscircuit.
 
-    @property
-    def edb_dll_path(self):
-        """Get/Set an optional path for Edb Dll.
+        Parameters
+        ----------
+        component : str
+            Address of the component instance. For example, ``"Inst@Galileo_cutout3;87;1"``.
+        option : str
+            Set the simulation strategy. Options are ``"simulate"`` and ``"interpolate"``. The default
+            is ``"simulate"``.
 
         Returns
         -------
         bool
-        """
-        return self._edb_dll_path
+            ``True`` when successful, ``False`` when failed.
 
-    @edb_dll_path.setter
-    def edb_dll_path(self, value):
-        if os.path.exists(value):
-            self._edb_dll_path = value
-
-    @property
-    def global_log_file_size(self):
-        """Get/Set the global pyaedt log file size in Mbytes. The default value is ``10``.
+        References
+        ----------
 
-        Returns
-        -------
-        bool
+        >>> oProject.ChangeProperty
         """
-        return self._global_log_file_size
+        if option == "simulate":
+            setting = "Simulate missing solutions"
+        elif option == "interpolate":
+            setting = "Interpolate existing solutions"
+        else:
+            return False
+        arg = ["NAME:Simulation option", "Value:=", setting]
+        return self._edit_link_definition_hfss_subcircuit(component, arg)
 
-    @global_log_file_size.setter
-    def global_log_file_size(self, value):
-        self._global_log_file_size = value
+    @pyaedt_function_handler()
+    def set_sim_solution_on_hfss_subcircuit(self, component, solution_name="Setup1 : Sweep"):
+        """Set the simulation solution on the HFSS subcircuit.
 
-    @property
-    def enable_global_log_file(self):
-        """Enable/Disable the global pyaedt log file logging in global temp folder. Default is `True`.
+        Parameters
+        ----------
+        component : str
+            Address of the component instance. For example, ``"Inst@Galileo_cutout3;87;1"``.
+        solution_name : str, optional
+            Name of the solution and sweep. The default is ``"Setup1 : Sweep"``.
 
         Returns
         -------
         bool
-        """
-        return self._enable_global_log_file
-
-    @enable_global_log_file.setter
-    def enable_global_log_file(self, value):
-        self._enable_global_log_file = value
+            ``True`` when successful, ``False`` when failed.
 
-    @property
-    def enable_local_log_file(self):
-        """Enable/Disable the local pyaedt log file logging in projectname.pyaedt project folder. Default is `True`.
+        References
+        ----------
 
-        Returns
-        -------
-        bool
+        >>> oProject.ChangeProperty
         """
-        return self._enable_local_log_file
-
-    @enable_local_log_file.setter
-    def enable_local_log_file(self, value):
-        self._enable_local_log_file = value
+        arg = ["NAME:Solution", "Value:=", solution_name]
+        return self._edit_link_definition_hfss_subcircuit(component, arg)
 
-    @property
-    def global_log_file_name(self):
-        """Get/Set the global pyaedt log file path. Default is pyaedt_username.log.
+    @pyaedt_function_handler()
+    def _edit_link_definition_hfss_subcircuit(self, component, edited_prop):
+        """Generic function to set the link definition for an hfss subcircuit."""
+        if isinstance(component, str):
+            complist = component.split(";")
+        elif isinstance(component, CircuitComponent):
+            complist = component.composed_name.split(";")
+        elif isinstance(component, int):
+            complist = self.components[component].composed_name.split(";")
+        else:
+            raise AttributeError("Wrong Component Input")
+        complist2 = complist[0].split("@")
+        arg = ["NAME:AllTabs"]
+        arg1 = ["NAME:Model"]
+        arg2 = ["NAME:PropServers", "Component@" + str(complist2[1])]
+        arg3 = ["NAME:ChangedProps", edited_prop]
+
+        arg1.append(arg2)
+        arg1.append(arg3)
+        arg.append(arg1)
 
-        Returns
-        -------
-        str
-        """
-        return self._global_log_file_name
+        self._app._oproject.ChangeProperty(arg)
+        return True
 
-    @global_log_file_name.setter
-    def global_log_file_name(self, value):
-        self._global_log_file_name = value
+    @pyaedt_function_handler()
+    def refresh_dynamic_link(self, component_name):
+        """Refresh a dynamic link component.
 
-    @property
-    def enable_pandas_output(self):
-        """
-        Set/Get a flag to use Pandas to export dict and lists. This applies to Solution data output.
-        If ``True`` the property or method will return a pandas object in CPython environment.
-        Default is ``False``.
+        Parameters
+        ----------
+        component_name : str
+            Name of the dynamic link component.
 
         Returns
         -------
         bool
-        """
-        return self._enable_pandas_output
+            ``True`` when successful, ``False`` when failed.
 
-    @enable_pandas_output.setter
-    def enable_pandas_output(self, val):
-        self._enable_pandas_output = val
-
-    @property
-    def enable_debug_methods_argument_logger(self):
-        """
-        Set/Get a flag to plot methods argument in debug logger.
-        Default is ``False``.
+        References
+        ----------
 
-        Returns
-        -------
-        bool
+        >>> oComponentManager.UpdateDynamicLink
         """
-        return self._enable_debug_methods_argument_logger
-
-    @enable_debug_methods_argument_logger.setter
-    def enable_debug_methods_argument_logger(self, val):
-        self._enable_debug_methods_argument_logger = val
-
-    @property
-    def force_error_on_missing_project(self):
-        """Set/Get a flag to check project path.
-        If ``True`` when passing a project path, the project has to exist otherwise it will raise an error.
-        Default is ``False``.
+        if "@" in component_name:
+            component_name = component_name.split("@")[1]
+        component_name = component_name.split(";")[0]
+        self.o_component_manager.UpdateDynamicLink(component_name)
+        return True
 
-        Returns
-        -------
-        bool
-        """
-        return self._force_error_on_missing_project
+    @pyaedt_function_handler()
+    def _parse_spice_model(self, model_path):
+        models = []
+        with open_file(model_path, "r") as f:
+            for line in f:
+                if ".subckt" in line.lower():
+                    pinNames = [i.strip() for i in re.split(" |\t", line) if i]
+                    models.append(pinNames[1])
+        return models
 
-    @force_error_on_missing_project.setter
-    def force_error_on_missing_project(self, val):
-        self._force_error_on_missing_project = val
+    @pyaedt_function_handler()
+    def create_component_from_spicemodel(self, model_path, model_name=None, create_component=True, location=None):
+        """Create and place a new component based on a spice .lib file.
 
-    @property
-    def disable_bounding_box_sat(self):
-        """Set/Get Bounding Box Sat enablement.
+        Parameters
+        ----------
+        model_path : str
+            Path to .lib file.
+        model_name : str, optional
+            Model name to import. If `None` the first subckt in the lib file will be placed.
+        create_component : bool, optional
+            If set to ``True``, create a spice model component. Otherwise, only import the spice model.
+        location : list, optional
+            Position in the schematic of the new component.
 
         Returns
         -------
-        bool
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
         """
-        return self._disable_bounding_box_sat
+        models = self._parse_spice_model(model_path)
+        if not model_name and models:
+            model_name = models[0]
+        elif model_name not in models:
+            return False
+        arg = ["NAME:Options", "Mode:=", 2, "Overwrite:=", False, "SupportsSimModels:=", False, "LoadOnly:=", False]
+        arg2 = ["NAME:Models"]
+        for el in models:
+            arg2.append(el + ":=")
+            if el == model_name:
+                arg2.append([True, "", "", False])
+            else:
+                arg2.append([False, "", "", False])
+        arg.append(arg2)
+        self.o_component_manager.ImportModelsFromFile(model_path.replace("\\", "/"), arg)
+
+        if create_component:
+            return self.create_component(
+                None,
+                component_library=None,
+                component_name=model_name,
+                location=location,
+            )
+        else:
+            return True
 
-    @disable_bounding_box_sat.setter
-    def disable_bounding_box_sat(self, val):
-        self._disable_bounding_box_sat = val
+    @pyaedt_function_handler()
+    def add_siwave_dynamic_link(self, model_path, solution_name=None, simulate_solutions=False):
+        """Add a siwave dinamyc link object.
 
-    @property
-    def use_grpc_api(self):
-        """Set/Get 20222R2 GPRC API usage or Legacy COM Objectr.
+        Parameters
+        ----------
+        model_path : str
+            Full path to the .siw file.
+        solution_name : str, optional
+            Solution name.
+        simulate_solutions : bool, optional
+            Either if simulate or interpolate existing solutions.
 
         Returns
         -------
-        bool
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+            Circuit Component Object.
         """
-        return self._use_grpc_api
-
-    @use_grpc_api.setter
-    def use_grpc_api(self, val):
-        """Set/Get 20222R2 GPRC API usage or Legacy COM Objectr."""
-        self._use_grpc_api = val
-
-    @property
-    def logger(self):
-        """Get the active logger."""
-        try:
-            return logging.getLogger("Global")
-        except:
-            return logging.getLogger(__name__)
-
-    @property
-    def non_graphical(self):
-        """Get the value for the non-graphical flag."""
-        return self._non_graphical
-
-    @non_graphical.setter
-    def non_graphical(self, val):
-        self._non_graphical = val
-
-    @property
-    def enable_error_handler(self):
-        """Return the content for the environment variable."""
-        return self._enable_error_handler
-
-    @enable_error_handler.setter
-    def enable_error_handler(self, val):
-        self._enable_error_handler = val
-
-    @property
-    def enable_desktop_logs(self):
-        """Get the content for the environment variable."""
-        return False if self.non_graphical else self._enable_desktop_logs
-
-    @enable_desktop_logs.setter
-    def enable_desktop_logs(self, val):
-        self._enable_desktop_logs = val
-
-    @property
-    def enable_screen_logs(self):
-        """Get the content for the environment variable."""
-        return self._enable_screen_logs
-
-    @enable_screen_logs.setter
-    def enable_screen_logs(self, val):
-        self._enable_screen_logs = val
-
-    @property
-    def pyaedt_server_path(self):
-        """Get the content for the environment variable."""
-        return os.getenv("PYAEDT_SERVER_AEDT_PATH", "")
-
-    @pyaedt_server_path.setter
-    def pyaedt_server_path(self, val):
-        os.environ["PYAEDT_SERVER_AEDT_PATH"] = str(val)
-
-    @property
-    def enable_file_logs(self):
-        """Get the content for the environment variable."""
-        return self._enable_file_logs
-
-    @enable_file_logs.setter
-    def enable_file_logs(self, val):
-        self._enable_file_logs = val
-
-    @property
-    def enable_logger(self):
-        """Return the Environment Variable Content."""
-        return self._enable_logger
-
-    @enable_logger.setter
-    def enable_logger(self, val):
-        self._enable_logger = val
-
-    @property
-    def logger_file_path(self):
-        """Return the Environment Variable Content."""
-        return self._logger_file_path
-
-    @logger_file_path.setter
-    def logger_file_path(self, val):
-        self._logger_file_path = val
-
-    @property
-    def logger_formatter(self):
-        """Return the Environment Variable Content."""
-        return self._logger_formatter
-
-    @logger_formatter.setter
-    def logger_formatter(self, val):
-        self._logger_formatter = val
-
-    @property
-    def logger_datefmt(self):
-        """Return the Environment Variable Content."""
-        return self._logger_datefmt
-
-    @logger_datefmt.setter
-    def logger_datefmt(self, val):
-        self._logger_datefmt = val
-
-    @property
-    def enable_debug_edb_logger(self):
-        """Return the Environment Variable Content."""
-        return self._enable_debug_edb_logger
-
-    @enable_debug_edb_logger.setter
-    def enable_debug_edb_logger(self, val):
-        self._enable_debug_edb_logger = val
-
-    @property
-    def enable_debug_geometry_operator_logger(self):
-        """Return the Environment Variable Content."""
-        return self._enable_debug_geometry_operator_logger
-
-    @enable_debug_geometry_operator_logger.setter
-    def enable_debug_geometry_operator_logger(self, val):
-        self._enable_debug_geometry_operator_logger = val
-
-    @property
-    def enable_debug_internal_methods_logger(self):
-        """Return the Environment Variable Content."""
-        return self._enable_debug_internal_methods_logger
-
-    @enable_debug_internal_methods_logger.setter
-    def enable_debug_internal_methods_logger(self, val):
-        self._enable_debug_internal_methods_logger = val
-
-    @property
-    def enable_debug_logger(self):
-        """Return the Environment Variable Content."""
-        return self._enable_debug_logger
-
-    @enable_debug_logger.setter
-    def enable_debug_logger(self, val):
-        self._enable_debug_logger = val
-
+        assert os.path.exists(model_path), "Project file doesn't exist"
+        comp_name = os.path.splitext(os.path.basename(model_path))[0]
+        results_path = model_path + "averesults"
+        solution = os.path.join(results_path, comp_name + ".asol")
+        # out = load_entire_aedt_file(solution)
+        out = load_keyword_in_aedt_file(solution, "Solutions")
+        if not solution_name:
+            solution_name = list(out["Solutions"]["SYZSolutions"].keys())[0]
+        results_folder = os.path.join(
+            results_path,
+            out["Solutions"]["SYZSolutions"][solution_name]["DiskName"],
+            out["Solutions"]["SYZSolutions"][solution_name]["DiskName"] + ".syzinfo",
+        )
 
-# property = Property
-settings = Settings()
-online_help = Help()
+        pin_names = []
+        with open_file(results_folder, "r") as f:
+            lines = f.read().splitlines()
+            for line in lines:
+                if line[:4] == "PORT":
+                    line_spit = line.split(" ")
+                    pin_names.append(line_spit[1].strip('"'))
+
+        return self._add_subcircuit_link(
+            comp_name,
+            pin_names,
+            model_path,
+            comp_name,
+            solution_name=solution_name,
+            model_type="siwave",
+            simulate_solutions=simulate_solutions,
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyaedt-0.6.82/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.85/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.85/pyaedt/generic/near_field_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import csv
-import glob
 import os
 import re
 
+from pyaedt.generic.filesystem import search_files
 from pyaedt.generic.general_methods import open_file
 
 
 class BoxFacePointsAndFields(object):
     """Data model class containing field component and coordinates."""
 
     def __init__(self):
@@ -70,15 +70,15 @@
         "ymin": BoxFacePointsAndFields(),
         "zmin": BoxFacePointsAndFields(),
         "xmax": BoxFacePointsAndFields(),
         "ymax": BoxFacePointsAndFields(),
         "zmax": BoxFacePointsAndFields(),
     }
 
-    file_names = glob.glob(dat_folder + "/*.dat")
+    file_names = search_files(dat_folder, "*.dat")
     for data_file in file_names:
         match = re.search(r"data_(\S+)_(\S+).dat", os.path.basename(data_file))
         field_component = match.group(1)
         face = match.group(2)
 
         if not os.path.exists(data_file):
             continue
```

### Comparing `pyaedt-0.6.82/pyaedt/generic/pdf.py` & `pyaedt-0.6.85/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/plot.py` & `pyaedt-0.6.85/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/process.py` & `pyaedt-0.6.85/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.85/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.85/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/toolkit.py` & `pyaedt-0.6.85/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.85/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/hfss.py` & `pyaedt-0.6.85/pyaedt/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             Boundary object.
 
         """
 
         bound = BoundaryObject(self, name, props, boundary_type)
         result = bound.create()
         if result:
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("Boundary %s %s has been correctly created.", boundary_type, name)
             return bound
         self.logger.error("Error in boundary creation for %s %s.", boundary_type, name)
 
         return result
 
     @pyaedt_function_handler()
@@ -398,15 +398,21 @@
         props["RenormalizeModes"] = True
         ports = list(self.oboundary.GetExcitationsOfType("Terminal"))
         boundary = self._create_boundary(portname, props, "AutoIdentify")
         if boundary:
             new_ports = list(self.oboundary.GetExcitationsOfType("Terminal"))
             terminals = [i for i in new_ports if i not in ports]
             for count, terminal in enumerate(terminals, start=1):
+                props_terminal = OrderedDict()
+                props_terminal["TerminalResistance"] = "50ohm"
+                props_terminal["ParentBndID"] = boundary.name
+                terminal_name = terminal
+
                 if impedance:
+                    props_terminal["TerminalResistance"] = str(impedance) + "ohm"
                     properties = [
                         "NAME:AllTabs",
                         [
                             "NAME:HfssTab",
                             ["NAME:PropServers", "BoundarySetup:" + terminal],
                             [
                                 "NAME:ChangedProps",
@@ -432,26 +438,29 @@
                     ]
                     try:
                         self.odesign.ChangeProperty(properties)
                     except:  # pragma: no cover
                         self.logger.warning("Failed to change normalization.")
                 if terminals_rename:
                     new_name = portname + "_T" + str(count)
+                    terminal_name = new_name
                     properties = [
                         "NAME:AllTabs",
                         [
                             "NAME:HfssTab",
                             ["NAME:PropServers", "BoundarySetup:" + terminal],
                             ["NAME:ChangedProps", ["NAME:Name", "Value:=", new_name]],
                         ],
                     ]
                     try:
                         self.odesign.ChangeProperty(properties)
                     except:  # pragma: no cover
                         self.logger.warning("Failed to rename terminal {}.".format(terminal))
+                bound = BoundaryObject(self, terminal_name, props_terminal, "Terminal")
+                self._boundaries[terminal_name] = bound
 
             if iswaveport:
                 boundary.type = "Wave Port"
             else:
                 boundary.type = "Lumped Port"
             props["Faces"] = [objectname]
             if iswaveport:
@@ -464,16 +473,19 @@
             else:
                 props["DoDeembed"] = True
                 if iswaveport:
                     props["DeembedDist"] = self.modeler._arg_with_dim(deembed)
             props["RenormalizeAllTerminals"] = renorm
             props["ShowReporterFilter"] = False
             props["UseAnalyticAlignment"] = False
-            boundary.props = props
+            boundary.auto_update = False
+            boundary.props.update(props)
+            boundary.auto_update = True
             boundary.update()
+
         return boundary
 
     @pyaedt_function_handler()
     def _create_circuit_port(self, edgelist, impedance, name, renorm, deemb, renorm_impedance=""):
         edgelist = self.modeler.convert_to_selections(edgelist, True)
         props = OrderedDict(
             {
@@ -1718,18 +1730,18 @@
 
         The two objects must have two adjacent, parallel, and identical faces.
         The faces must be a polygon (not a circle).
         The closest faces must be aligned with the main planes of the reference system.
 
         Parameters
         ----------
-        start_object : str or int or :class:`pyaedt.modeler.object3d.Object3d`
+        start_object : str or int or :class:`pyaedt.modeler.cad.object3d.Object3d`
             First solid connected to the spiral port.
 
-        end_object : str or int or :class:`pyaedt.modeler.object3d.Object3d`
+        end_object : str or int or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Second object connected to the spiral port.
 
         port_width : float, optional
             Width of the spiral port.
             If not specified the width will be calculated based on the object dimensions.
             The default is ``None``.
 
@@ -3067,15 +3079,15 @@
         """Create a waveport on sheet objects created starting from sheets.
 
         .. deprecated:: 0.6.62
             `create_wave_port_from_sheet` is deprecated. Use `wave_port` property instead.
 
         Parameters
         ----------
-        sheet : str or int or list or :class:`pyaedt.modeler.object3d.Object3d`
+        sheet : str or int or list or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Name of the sheet.
         deemb : float, optional
             Deembedding value distance in model units. The default is ``0``.
         axisdir : int or :class:`pyaedt.application.Analysis.Analysis.AxisDir`, optional
             Position of the port. It is used to auto evaluate the integration line.
             If set to ``None`` the integration line is not defined.
             It should be one of the values for ``Application.AxisDir``,
@@ -4389,15 +4401,15 @@
 
     @pyaedt_function_handler()
     def assign_radiation_boundary_to_objects(self, obj_names, boundary_name=""):
         """Assign a radiation boundary to one or more objects (usually airbox objects).
 
         Parameters
         ----------
-        obj_names : str or list or int or :class:`pyaedt.modeler.object3d.Object3d`
+        obj_names : str or list or int or :class:`pyaedt.modeler.cad.object3d.Object3d`
             One or more object names or IDs.
         boundary_name : str, optional
             Name of the boundary. The default is ``""``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
@@ -4430,15 +4442,15 @@
 
     @pyaedt_function_handler()
     def assign_hybrid_region(self, obj_names, boundary_name="", hybrid_region="SBR+"):
         """Assign a hybrid region to one or more objects.
 
         Parameters
         ----------
-        obj_names : str or list or int or :class:`pyaedt.modeler.object3d.Object3d`
+        obj_names : str or list or int or :class:`pyaedt.modeler.cad.object3d.Object3d`
             One or more object names or IDs.
         boundary_name : str, optional
             Name of the boundary. The default is ``""``.
         hybrid_region : str, optional
             Hybrid region to assign. Options are ``"SBR+"``, ``"IE"``, ``"PO"``. The default is `"SBR+"``.
 
         Returns
@@ -5776,14 +5788,55 @@
 
             props = OrderedDict({"Name": symmetry_name, "Faces": entity_list, "IsPerfectE": is_perfect_e})
             return self._create_boundary(symmetry_name, props, "Symmetry")
         except:
             return False
 
     @pyaedt_function_handler()
+    def set_impedance_multiplier(self, impedance):
+        # type: (float) -> bool
+        """Set impedance multiplier.
+
+        Parameters
+        ----------
+        impedance : float
+            Impedance.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        References
+        ----------
+
+        >>> oModule.ChangeImpedanceMult
+
+        Examples
+        --------
+
+        Create a box. Select the faces of this box and assign a symmetry.
+
+        >>> symmetry_box = hfss.modeler.create_box([0 , -100, 0], [200, 200, 200],
+        ...                                         name="SymmetryForFaces")
+        >>> ids = [i.id for i in hfss.modeler["SymmetryForFaces"].faces]
+        >>> symmetry = hfss.assign_symmetry(ids)
+        >>> hfss.set_impedance_multiplier(2.0)
+
+        """
+        try:
+            if self.solution_type not in ["Modal"]:
+                self.logger.error("Symmetry is only available with 'Modal' solution type.")
+                return False
+            self.oboundary.ChangeImpedanceMult(impedance)
+            return True
+        except:
+            return False
+
+    @pyaedt_function_handler()
     def get_touchstone_data(self, setup_name, sweep_name=None, variation_dict=None):
         """
         Return a Touchstone data plot.
 
         Parameters
         ----------
         setup_name : list
@@ -5881,18 +5934,18 @@
     ):
         """Create a circuit port from two objects.
 
         The integration line is from edge 2 to edge 1.
 
         Parameters
         ----------
-        signal : int or :class:`pyaedt.modeler.object3d.Object3d` or
+        signal : int or :class:`pyaedt.modeler.cad.object3d.Object3d` or
          :class:`pyaedt.modeler.cad.FacePrimitive`or :class:`pyaedt.modeler.cad.EdgePrimitive`
             Signal object.
-        reference : int or :class:`pyaedt.modeler.object3d.Object3d` or
+        reference : int or :class:`pyaedt.modeler.cad.object3d.Object3d` or
          :class:`pyaedt.modeler.cad.FacePrimitive`or :class:`pyaedt.modeler.cad.EdgePrimitive`
             Reference object.
         port_location : int or :class:`pyaedt.application.Analysis.Analysis.AxisDir`, optional
             Position of the port when an object different from an edge is provided.
             It should be one of the values for ``Application.AxisDir``,
             which are: ``XNeg``, ``YNeg``, ``ZNeg``, ``XPos``, ``YPos``, and ``ZPos``.
             The default is ``Application.AxisDir.XNeg``.
@@ -5970,18 +6023,18 @@
         deembed=False,
         terminals_rename=True,
     ):
         """Create a waveport taking the closest edges of two objects.
 
         Parameters
         ----------
-        signal : str, int, list, :class:`pyaedt.modeler.object3d.Object3d` or
+        signal : str, int, list, :class:`pyaedt.modeler.cad.object3d.Object3d` or
          :class:`pyaedt.modeler.elements3d.FacePrimitive`
             Main object for port creation or starting object for the integration line.
-        reference : int, list or :class:`pyaedt.modeler.object3d.Object3d`
+        reference : int, list or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Ending object for the integration line or reference for Terminal solution. Can be multiple objects.
         create_port_sheet : bool, optional
             Whether to create a port sheet or use given start_object as port shee.
         integration_line : int or :class:`pyaedt.application.Analysis.Analysis.AxisDir`, optional
             Position of the port. It should be one of the values for ``Application.AxisDir``,
             which are: ``XNeg``, ``YNeg``, ``ZNeg``, ``XPos``, ``YPos``, and ``ZPos``.
             The default is ``Application.AxisDir.XNeg``.
@@ -6094,18 +6147,18 @@
         hfactor=5,
         terminals_rename=True,
     ):
         """Create a waveport from a sheet (``start_object``) or taking the closest edges of two objects.
 
         Parameters
         ----------
-        signal : int, str, :class:`pyaedt.modeler.object3d.Object3d` or
+        signal : int, str, :class:`pyaedt.modeler.cad.object3d.Object3d` or
          :class:`pyaedt.modeler.elements3d.FacePrimitive`
             Main object for port creation or starting object for the integration line.
-        reference : int, str, list or :class:`pyaedt.modeler.object3d.Object3d`
+        reference : int, str, list or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Ending object for the integration line or reference for Terminal solution. Can be multiple objects.
         create_port_sheet : bool, optional
             Whether to create a port sheet or use given start_object as port shee.
         create_pec_cap : bool, False
             Whether to create a port cap or not.
         integration_line : list or int or :class:`pyaedt.application.Analysis.Analysis.AxisDir`, optional
             Position of the integration. It should be one of the values for ``Application.AxisDir``,
@@ -6248,7 +6301,23 @@
                     impedance=impedance,
                     terminals_rename=terminals_rename,
                 )
             else:
                 self.logger.error("Reference conductors are missing.")
                 return False
         return False
+
+    @pyaedt_function_handler()
+    def set_radiated_power_calc_method(self, method="Auto"):
+        """Set the radiated power calculation method in Hfss.
+
+        method : str, optional
+            Radiated power calculation method.
+            The options are ``"Auto"``, ``"Radiation Surface Integral"`` and ``"Far Field Integral"``.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+        """
+        self.oradfield.EditRadiatedPowerCalculationMethod(method)
+        return True
```

### Comparing `pyaedt-0.6.82/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.85/pyaedt/hfss3dlayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,16 +247,16 @@
                     property_object="Excitations:{}".format(a[0]),
                     property_name="PEC Launch Width",
                     property_value=str(wave_launcher),
                     property_tab="EM Design",
                 )
             bound = self._update_port_info(a[0])
             if bound:
-                self.boundaries.append(bound)
-                return self.boundaries[-1]
+                self._boundaries[bound.name] = bound
+                return bound
             else:
                 return False
         else:
             return False
 
     @pyaedt_function_handler()
     def create_wave_port(
@@ -399,15 +399,15 @@
         listnew = self.port_list
         a = [i for i in listnew if i not in listp]
         ports = []
         if len(a) > 0:
             for port in a:
                 bound = self._update_port_info(port)
                 if bound:
-                    self.boundaries.append(bound)
+                    self._boundaries[bound.name] = bound
                     ports.append(bound)
         return ports
 
     @pyaedt_function_handler()
     def create_differential_port(self, via_signal, via_reference, port_name, deembed=True):
         """Create a new differential port.
 
@@ -498,16 +498,16 @@
                 self.modeler.change_property(
                     a[0],
                     "Pad Port Layer",
                     layer,
                 )
             bound = self._update_port_info(a[0])
             if bound:
-                self.boundaries.append(bound)
-                return self.boundaries[-1]
+                self._boundaries[bound.name] = bound
+                return bound
             else:
                 return False
         else:
             return False
 
     @pyaedt_function_handler()
     def create_pin_port(self, name, xpos=0, ypos=0, rotation=0, top_layer=None, bot_layer=None):
@@ -566,16 +566,16 @@
                 top_layer,
                 "lowest_layer:=",
                 bot_layer,
             ]
         )
         bound = self._update_port_info(name)
         if bound:
-            self.boundaries.append(bound)
-            return self.boundaries[-1]
+            self._boundaries[bound.name] = bound
+            return bound
         else:
             return False
 
     @pyaedt_function_handler()
     def delete_port(self, portname):
         """Delete a port.
 
@@ -1652,15 +1652,55 @@
         try:
             self.oexcitation.SetDiffPairs(arg)
         except:  # pragma: no cover
             return False
         return True
 
     @pyaedt_function_handler()
+    def get_differential_pairs(self):
+        # type: () -> list
+        """Get the list defined differential pairs.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        list
+            List of differential pairs.
+
+        Examples
+        --------
+        >>> from pyaedt import Hfss3dLayout
+        >>> hfss = Hfss3dLayout()
+        >>> hfss.get_defined_diff_pairs()
+        """
+
+        list_output = []
+        if len(self.excitations) != 0:
+            tmpfile1 = os.path.join(self.working_directory, generate_unique_name("tmp"))
+            file_flag = self.save_diff_pairs_to_file(tmpfile1)
+            if file_flag and os.stat(tmpfile1).st_size != 0:
+                with open_file(tmpfile1, "r") as fi:
+                    fi_lst = fi.readlines()
+                list_output = [line.split(",")[4] for line in fi_lst]
+            else:
+                self.logger.warning("ERROR: No differential pairs defined under Excitations > Differential Pairs...")
+
+            try:
+                os.remove(tmpfile1)
+            except:  # pragma: no cover
+                self.logger.warning("ERROR: Cannot remove temp files.")
+
+        return list_output
+
+    @pyaedt_function_handler()
     def load_diff_pairs_from_file(self, filename):
+        # type: (str) -> bool
         """Load differtential pairs definition from file.
 
         You can use the ``save_diff_pairs_to_file`` method to obtain the file format.
         The ``File End Of Line`` must be UNIX (LF).
         New definitions are added only if compatible with the existing definition already defined in the project.
 
         Parameters
@@ -1692,17 +1732,18 @@
             os.remove(new_file)
         except:  # pragma: no cover
             return False
         return True
 
     @pyaedt_function_handler()
     def save_diff_pairs_to_file(self, filename):
+        # type: (str) -> bool
         """Save differtential pairs definition to a file.
 
-        If a filee with the specified name already exists, it is overwritten.
+        If a file with the specified name already exists, it is overwritten.
 
         Parameters
         ----------
         filename : str
             Fully qualified name of the file containing the differential pairs definition.
 
         Returns
@@ -1771,14 +1812,15 @@
         diel_extent_horizontal_padding=None,
         diel_honor_primitives_on_diel_layers="keep",
         air_extent_type=None,
         air_truncate_model_at_ground_layer="keep",
         air_vertical_positive_padding=None,
         air_vertical_negative_padding=None,
         airbox_values_as_dim=True,
+        air_horizontal_padding=None,
     ):
         """Edit HFSS 3D Layout extents.
 
         Parameters
         ----------
         diel_extent_type : str, optional
             Dielectric extent type. The default is ``None``. Options are ``"BboxExtent"``,
@@ -1794,14 +1836,17 @@
             Whether to set airbox truncate model at ground layer. The default is ``None``.
         air_vertical_positive_padding : str, optional
             Airbox vertical positive padding. The default is ``None``.
         air_vertical_negative_padding : str, optional
             Airbox vertical negative padding. The default is ``None``.
         airbox_values_as_dim : bool, optional
             Either if inputs are dims or not. Default is `True`.
+        air_horizontal_padding : float, optional
+            Airbox horizontal padding. The default is ``None``.
+
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         arg = ["NAME:HfssExportInfo"]
@@ -1816,14 +1861,17 @@
             arg.append(diel_honor_primitives_on_diel_layers)
         if air_extent_type:
             arg.append("ExtentType:=")
             arg.append(air_extent_type)
         if not air_truncate_model_at_ground_layer == "keep":
             arg.append("TruncAtGnd:=")
             arg.append(air_truncate_model_at_ground_layer)
+        if air_horizontal_padding:
+            arg.append("AirHorExt:=")
+            arg.append(["Ext:=", str(air_horizontal_padding), "Dim:=", airbox_values_as_dim])
         if air_vertical_positive_padding:
             arg.append("AirPosZExt:=")
             arg.append(["Ext:=", air_vertical_positive_padding, "Dim:=", airbox_values_as_dim])
         if air_vertical_negative_padding:
             arg.append("AirNegZExt:=")
             arg.append(["Ext:=", air_vertical_negative_padding, "Dim:=", airbox_values_as_dim])
         arg.append("UseStackupForZExtFact:=")
```

### Comparing `pyaedt-0.6.82/pyaedt/icepak.py` & `pyaedt-0.6.85/pyaedt/icepak.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import csv
 import math
 import os
 import warnings
 
 from pyaedt import is_ironpython
 from pyaedt import is_linux
+from pyaedt.generic.general_methods import GrpcApiError
 from pyaedt.modules.SetupTemplates import SetupKeys
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
     import subprocess
 
@@ -278,15 +279,15 @@
             props["External Rad. Temperature"] = external_temp
             props["External Total Pressure"] = expternal_pressure
 
         props["X"] = x_curve
         props["Y"] = y_curve
         bound = BoundaryObject(self, boundary_name, props, "Grille")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("Grille Assigned")
             return bound
         return None
 
     @pyaedt_function_handler()
     def assign_openings(self, air_faces):
         """Assign openings to a list of faces.
@@ -325,15 +326,15 @@
         props["Faces"] = air_faces
         props["Temperature"] = "AmbientTemp"
         props["External Rad. Temperature"] = "AmbientRadTemp"
         props["Inlet Type"] = "Pressure"
         props["Total Pressure"] = "AmbientPressure"
         bound = BoundaryObject(self, boundary_name, props, "Opening")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("Opening Assigned")
             return bound
         return None
 
     @pyaedt_function_handler()
     def assign_2way_coupling(
         self, setup_name=None, number_of_iterations=2, continue_ipk_iterations=True, ipk_iterations_per_coupling=20
@@ -510,15 +511,15 @@
         if use_object_for_name:
             boundary_name = object_name[0]
         else:
             boundary_name = generate_unique_name("Block")
 
         bound = BoundaryObject(self, boundary_name, props, "Block")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("Block on {} with {} power created correctly.".format(object_name, input_power))
             return bound
         return None
 
     @pyaedt_function_handler()
     def create_conduting_plate(
         self,
@@ -621,19 +622,19 @@
                     "Variation Value": '["1W", "pwl({},Temp)"]'.format(thermal_dependent_dataset),
                 }
             )
         props["Shell Conduction"] = shell_conduction
         bound = BoundaryObject(self, bc_name, props, "Conducting Plate")
         try:
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
             else:  # pragma : no cover
                 raise SystemExit
-        except SystemExit:
+        except (GrpcApiError, SystemExit):
             return None
 
     @pyaedt_function_handler()
     def create_source_power(
         self,
         face_id,
         thermal_dependent_dataset=None,
@@ -718,19 +719,19 @@
             )
         props["Surface Heat"] = surface_heat
         props["Temperature"] = temperature
         props["Radiation"] = OrderedDict({"Radiate": radiate})
         bound = BoundaryObject(self, source_name, props, "SourceIcepak")
         try:
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
             else:  # pragma : no cover
                 raise SystemExit
-        except SystemExit:
+        except (GrpcApiError, SystemExit):
             return None
 
     @pyaedt_function_handler()
     def create_network_block(
         self,
         object_name,
         power,
@@ -833,15 +834,15 @@
                     "Link1": ["Face" + str(fcrjc), "Internal", "R", str(rjc) + "cel_per_w"],
                     "Link2": ["Face" + str(fcrjb), "Internal", "R", str(rjb) + "cel_per_w"],
                 }
             )
             props["SchematicData"] = OrderedDict({})
             bound = BoundaryObject(self, boundary_name, props, "Network")
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 self.modeler[object_name].solve_inside = False
                 return bound
             return None
 
     @pyaedt_function_handler()
     def create_network_blocks(
         self, input_list, gravity_dir, top, assign_material=True, default_material="Ceramic_material"
@@ -1569,15 +1570,15 @@
         )
         props["Intrinsics"] = intr
         props["SurfaceOnly"] = surfaces
 
         name = generate_unique_name("EMLoss")
         bound = BoundaryObject(self, name, props, "EMLoss")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("EM losses mapped from design: %s.", designname)
             return bound
         return False
 
     @pyaedt_function_handler()
     def eval_surface_quantity_from_field_summary(
         self,
@@ -3106,15 +3107,15 @@
             ),
             "SchematicData": ({}),
         }
 
         self.modeler.primitives[object_name].material_name = "Ceramic_material"
         boundary = BoundaryObject(self, object_name, props, "Network")
         if boundary.create():
-            self.boundaries.append(boundary)
+            self._boundaries[boundary.name] = boundary
             self.modeler.primitives[object_name].solve_inside = False
             return boundary
         return None
 
     @pyaedt_function_handler()
     def assign_stationary_wall(
         self,
@@ -3323,19 +3324,19 @@
         props["External Surface Radiation"] = ext_surf_rad
         props["External Material"] = ext_surf_rad_material
         props["External Radiation Reference Temperature"] = ext_surf_rad_ref_temp
         props["External Radiation View Factor"] = ext_surf_rad_view_factor
         bound = BoundaryObject(self, name, props, "Stationary Wall")
         try:
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
             else:  # pragma : no cover
                 raise SystemExit
-        except SystemExit:
+        except (GrpcApiError, SystemExit):
             return None
 
     @pyaedt_function_handler()
     def assign_stationary_wall_with_heat_flux(
         self,
         geometry,
         name=None,
@@ -3797,15 +3798,15 @@
                 else:
                     props[quantity] = voltage_current_value
             else:
                 props[quantity] = value
 
         bound = BoundaryObject(self, boundary_name, props, "SourceIcepak")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         else:
             return None
 
     @pyaedt_function_handler()
     def create_network_object(self, name=None, props=None, create=False):
         """Create a thermal network.
@@ -3837,15 +3838,16 @@
         --------
 
         >>> from pyaedt import Icepak
         >>> app = Icepak()
         >>> network = app.create_network_object()
         """
         bound = NetworkObject(self, name, props, create)
-        self.boundaries.append(bound)
+        if create:
+            self._boundaries[bound.name] = bound
         return bound
 
     @pyaedt_function_handler()
     def create_resistor_network_from_matrix(self, sources_power, faces_ids, matrix, network_name=None, node_names=None):
         """Create a thermal network.
 
         Parameters
@@ -3906,14 +3908,15 @@
             second = net.add_face_node(id, name=node_name)
             all_nodes.append(second.name)
         for i in range(len(matrix)):
             for j in range(len(matrix[0])):
                 if matrix[i][j] > 0:
                     net.add_link(all_nodes[i], all_nodes[j], matrix[i][j], "Link_" + all_nodes[i] + "_" + all_nodes[j])
         if net.create():
+            self._boundaries[net.name] = net
             return net
         else:  # pragma: no cover
             return None
 
     @pyaedt_function_handler
     def assign_solid_block(
         self, object_name, power_assignment, boundary_name=None, htc=None, ext_temperature="AmbientTemp"
@@ -3926,29 +3929,26 @@
         object_name : str or list
             Object name or a list of object names.
         power_assignment : str or dict
             String with the value and units of the power assignment or with
             ``"Joule Heating"``. For a temperature-dependent or transient
             assignment, a dictionary can be used. The dictionary should contain three keys:
             ``"Type"``, ``"Function"``, and ``"Values"``.
-
             - For the ``"Type"`` key, accepted values are ``"Temp Dep"`` and ``"Transient"``.
             - For the ``"Function"`` key, acceptable values depend on the ``"Type"`` key
-              selection. When the ``"Type"`` key is set to ``"Temp Dep"``, the only
-              accepted value is ````"Piecewise Linear"`` . When the ``"Type"`` key is
-              set to ``"Transient"``, acceptable values are `"Exponential"``, `"Linear"``,
-              ```"Piecewise Linear"``, ``"Power Law"``, ``"Sinusoidal"``, and ``"Square
-               Wave"``.
+            selection. When the ``"Type"`` key is set to ``"Temp Dep"``, the only
+            accepted value is ``"Piecewise Linear"``. When the ``"Type"`` key is
+            set to ``"Transient"``, acceptable values are `"Exponential"``, `"Linear"``,
+            ``"Piecewise Linear"``, ``"Power Law"``, ``"Sinusoidal"``, and ``"SquareWave"``.
             - For the ``"Values"`` key, a list of strings contain the parameters required by
-              the ``"Function"`` key selection. For example, whn``"Linear"`` is set as the
-              ``"Function"`` key, two parameters are required: the value of the variable
-              at t=0 and the slope of the line. For the parameters required by each
-              ``"Function"`` key selection, see the Icepak documentation. The parameters
-              must contain the units where needed.
-
+            the ``"Function"`` key selection. For example, whn``"Linear"`` is set as the
+            ``"Function"`` key, two parameters are required: the value of the variable
+            at t=0 and the slope of the line. For the parameters required by each
+            ``"Function"`` key selection, see the Icepak documentation. The parameters
+            must contain the units where needed.
         boundary_name : str, optional
             Name of the source boundary. The default is ``None``, in which case the
             boundary name is automatically generated.
         htc : float, str, or dict, optional
             String with the value and units of the heat transfer coefficient for the
             external conditions. If a float is provided, the ``"w_per_m2kel"`` unit is used.
             For a temperature-dependent or transient
@@ -3959,15 +3959,14 @@
             String with the value and units of temperature for the external conditions.
             If a float is provided, the ``"cel"`` unit is used.
             For a transient assignment, a dictionary can be used. For more information,
             see the description for the preceding ``power_assignment`` parameter. The
             default is ``"AmbientTemp"``, which is used if the ``htc`` parameter is not
             set to ``None``.
 
-
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object when successful or ``None`` when failed.
 
         References
         ----------
@@ -3978,14 +3977,15 @@
         --------
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
         >>> ipk.solution_type = "Transient"
         >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox3", "copper")
         >>> power_dict = {"Type": "Transient", "Function": "Sinusoidal", "Values": ["0W", 1, 1, "1s"]}
         >>> block = ipk.assign_solid_block("BlockBox3", power_dict)
+
         """
         if ext_temperature != "AmbientTemp" and ext_temperature is not None and not htc:
             self.logger.add_error_message("Set an argument for ``htc`` or remove the ``ext_temperature`` argument.")
             return None
         if isinstance(ext_temperature, dict) and ext_temperature["Type"] == "Temp Dep":
             self.logger.add_error_message(
                 'It is not possible to use a "Temp Dep" assignment for ' "temperature assignment."
@@ -4038,68 +4038,60 @@
 
         if not boundary_name:
             boundary_name = generate_unique_name("Block")
 
         bound = BoundaryObject(self, boundary_name, props, "Block")
         try:
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
             else:  # pragma : no cover
                 raise SystemExit
-        except SystemExit:
+        except (GrpcApiError, SystemExit):
             return None
 
     @pyaedt_function_handler
     def assign_hollow_block(
         self, object_name, assignment_type, assignment_value, boundary_name=None, external_temperature="AmbientTemp"
     ):
-        """
-        Assign block boundary for hollow objects.
+        """Assign block boundary for hollow objects.
 
         Parameters
         ----------
         object_name : str or list
             Object name or a list of object names.
         assignment_type : str
             Type of the boundary assignment. Options are ``"Heat Transfer Coefficient"``,
             ``"Heat Flux"``, ``"Temperature"``, and ``"Total Power"``.
         assignment_value : str or dict
             String with value and units of the assignment. If ``"Total Power"`` is
             the assignment type, ``"Joule Heating"`` can be used.
             For a temperature-dependent or transient assignment, a dictionary can be used.
-            The dictionary should contain three keys:
-            ``"Type"``, ``"Function"``, and ``"Values"``.
-
+            The dictionary should contain three keys: ``"Type"``, ``"Function"``, and ``"Values"``.
             - For the ``"Type"`` key, accepted values are ``"Temp Dep"`` and ``"Transient"``.
-            - For the ``"Function"`` key, acceptable values depend on the ``"Type"`` key
-              selection. When the ``"Type"`` key is set to ``"Temp Dep"``, the only
-              accepted value is ````"Piecewise Linear"`` . When the ``"Type"`` key is
-              set to ``"Transient"``, acceptable values are `"Exponential"``, `"Linear"``,
-              ```"Piecewise Linear"``, ``"Power Law"``, ``"Sinusoidal"``, and ``"Square
-               Wave"``.
-            - For the ``"Values"`` key, a list of strings contain the parameters required by
-              the ``"Function"`` key selection. For example, whn``"Linear"`` is set as the
-              ``"Function"`` key, two parameters are required: the value of the variable
-              at t=0 and the slope of the line. For the parameters required by each
-              ``"Function"`` key selection, see the Icepak documentation. The parameters
-              must contain the units where needed.
-
+            - For the ``"Function"`` key, acceptable values depend on the ``"Type"`` key selection. When the ``"Type"``
+            key is set to ``"Temp Dep"``, the only accepted value is ``"Piecewise Linear"``.
+            When the ``"Type"`` key is set to ``"Transient"``, acceptable values are `"Exponential"``, `"Linear"``,
+            ``"Piecewise Linear"``, ``"Power Law"``, ``"Sinusoidal"``, and ``"Square Wave"``.
+            - For the ``"Values"`` key, a list of strings contain the parameters required by the ``"Function"``
+            key selection. For example, whn``"Linear"`` is set as the ``"Function"`` key, two parameters are required:
+            the value of the variable at t=0 and the slope of the line.
+            For the parameters required by each ``"Function"`` key selection, see the Icepak documentation.
+            The parameters must contain the units where needed.
         boundary_name : str, optional
             Name of the source boundary. The default is ``None``, in which case the
             boundary is automatically generated.
         external_temperature : str, dict or float, optional
             String with the value and unit of the temperature for the heat transfer
             coefficient. If a float value is specified, the ``"cel"`` unit is automatically
             added.
             For a transient assignment, a dictionary can be used as described for the
-            ``assignment_value argument``. Temperature dependent assignment is not supported.
+            ``assignment_value`` argument. Temperature dependent assignment is not supported.
             The default is ``"AmbientTemp"``.
 
-
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object when successful or ``None`` when failed.
 
         References
         ----------
@@ -4111,14 +4103,15 @@
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
         >>> ipk.solution_type = "Transient"
         >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox5", "copper")
         >>> box.solve_inside = False
         >>> temp_dict = {"Type": "Transient", "Function": "Square Wave", "Values": ["1cel", "0s", "1s", "0.5s", "0cel"]}
         >>> block = ipk.assign_hollow_block("BlockBox5", "Heat Transfer Coefficient", "1w_per_m2kel", "Test", temp_dict)
+
         """
         if assignment_value == "Joule Heating" and assignment_type != "Total Power":
             self.logger.add_error_message(
                 '``"Joule Heating"`` assignment is supported only if ``assignment_type``' 'is ``"Total Power"``.'
             )
             return None
 
@@ -4180,19 +4173,19 @@
 
         if not boundary_name:
             boundary_name = generate_unique_name("Block")
 
         bound = BoundaryObject(self, boundary_name, props, "Block")
         try:
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
             else:  # pragma : no cover
                 raise SystemExit
-        except SystemExit:
+        except (GrpcApiError, SystemExit):
             return None
 
     @pyaedt_function_handler()
     def get_fans_operating_point(self, export_file=None, setup_name=None, timestep=None, design_variation=None):
         """
         Get operating point of the fans in the design.
 
@@ -4344,15 +4337,14 @@
         inflow : bool, optional
             Prescribe if the imposed mass flow is an inflow or an outflow. Default is ``"True"``,
             in which case an inflow is prescribed.
         direction_vector : list, optional
             Prescribe the direction of the massflow. Default is ``"None"``, in which case a
             massflow normal to the boundary is prescribed.
 
-
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object when successful or ``None`` when failed.
 
         References
         ----------
@@ -4360,14 +4352,15 @@
 
         Examples
         ----------
         >>> import pyaedt
         >>> icepak = pyaedt.Icepak()
         >>> f_id = icepak.modeler["Region"].faces[0].id
         >>> icepak.assign_free_opening(f_id)
+
         """
         # Sanitize input
         for i in range(len(velocity)):
             if not isinstance(velocity[i], str) and not isinstance(velocity[i], dict):
                 velocity[i] = str(velocity[i]) + "m_per_sec"
         if not isinstance(mass_flow_rate, str) and not isinstance(mass_flow_rate, dict):
             mass_flow_rate = str(mass_flow_rate) + "kg_per_s"
@@ -4434,15 +4427,15 @@
                 props[quantity] = assignment
 
         if not boundary_name:
             boundary_name = generate_unique_name("Opening")
 
         bound = BoundaryObject(self, boundary_name, props, "Opening")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         else:
             return None
 
     @pyaedt_function_handler()
     def assign_pressure_free_opening(
         self,
@@ -4709,13 +4702,13 @@
             props["Faces"] = geometry
         else:
             props["Objects"] = geometry
 
         bound = BoundaryObject(self, boundary_name, props, "Symmetry Wall")
         try:
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
             else:  # pragma : no cover
                 raise SystemExit
-        except SystemExit:
+        except (GrpcApiError, SystemExit):
             return None
```

### Comparing `pyaedt-0.6.82/pyaedt/maxwell.py` & `pyaedt-0.6.85/pyaedt/maxwell.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                             {"GroupName": element, "NumberOfBranches": branches[cont], "Sources": source_list}
                         )
                         props["MatrixGroup"]["MatrixGroup"].append(prop)
                         cont += 1
 
             bound = MaxwellParameters(self, matrix_name, props, "Matrix")
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
         else:
             self.logger.error("Solution type does not have matrix parameters")
             return False
 
     @pyaedt_function_handler()
     def setup_ctrlprog(
@@ -640,15 +640,15 @@
             if type(object_list[0]) is str:
                 props = OrderedDict({"Objects": object_list, "Current": amplitude, "IsPositive": swap_direction})
             else:
                 self.logger.warning("Input must be a 2D object.")
                 return False
         bound = BoundaryObject(self, name, props, "Current")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_translate_motion(
         self,
         band_object,
@@ -740,15 +740,15 @@
                 "Damping": str(damping),
                 "Load Force": self._arg_with_units(load_force, "newton"),
                 "Objects": object_list,
             }
         )
         bound = BoundaryObject(self, motion_name, props, "Band")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_rotate_motion(
         self,
         band_object,
@@ -838,15 +838,15 @@
                 "Damping": str(damping),
                 "Load Torque": self._arg_with_units(load_torque, "NewtonMeter"),
                 "Objects": object_list,
             }
         )
         bound = BoundaryObject(self, motion_name, props, "Band")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_voltage(self, face_list, amplitude=1, name=None):
         """Assign a voltage source to a list of faces in Maxwell 3D or a list of Objects in Maxwell 2D.
 
@@ -879,15 +879,15 @@
 
         if self.design_type == "Maxwell 2D":
             props = OrderedDict({"Objects": face_list, "Value": amplitude})
         else:
             props = OrderedDict({"Faces": face_list, "Voltage": amplitude})
         bound = BoundaryObject(self, name, props, "Voltage")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_voltage_drop(self, face_list, amplitude=1, swap_direction=False, name=None):
         """Assign a voltage drop across a list of faces to a specific value.
 
@@ -921,15 +921,15 @@
         if not name:
             name = generate_unique_name("VoltageDrop")
         face_list = self.modeler.convert_to_selections(face_list, True)
 
         props = OrderedDict({"Faces": face_list, "Voltage Drop": amplitude, "Point out of terminal": swap_direction})
         bound = BoundaryObject(self, name, props, "VoltageDrop")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_winding(
         self,
         coil_terminals=None,
@@ -992,15 +992,15 @@
                 "Inductance": self.modeler._arg_with_dim(ind, "H"),
                 "Voltage": self.modeler._arg_with_dim(voltage, "V"),
                 "ParallelBranchesNum": str(parallel_branches),
             }
         )
         bound = BoundaryObject(self, name, props, "Winding")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             if coil_terminals is None:
                 coil_terminals = []
             if type(coil_terminals) is not list:
                 coil_terminals = [coil_terminals]
             coil_names = []
             for coil in coil_terminals:
                 c = self.assign_coil(coil)
@@ -1098,15 +1098,15 @@
                 )
                 bound = BoundaryObject(self, name, props2, "CoilTerminal")
 
             else:
                 self.logger.warning("Face Selection is not allowed in Maxwell 2D. Provide a 2D object.")
                 return False
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_force(self, input_object, reference_cs="Global", is_virtual=True, force_name=None):
         """Assign a force to one or more objects.
 
@@ -1158,15 +1158,15 @@
                         "Reference CS": reference_cs,
                         "Objects": input_object,
                     }
                 )
 
             bound = MaxwellParameters(self, force_name, prop, "Force")
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
         else:
             self.logger.error("Solution Type has not Matrix Parameter")
             return False
 
     @pyaedt_function_handler()
     def assign_torque(
@@ -1231,15 +1231,15 @@
                         "Is Positive": is_positive,
                         "Objects": input_object,
                     }
                 )
 
             bound = MaxwellParameters(self, torque_name, prop, "Torque")
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
         else:
             self.logger.error("Solution Type has not Matrix Parameter")
             return False
 
     @pyaedt_function_handler()
     def solve_inside(self, name, activate=True):
@@ -1366,15 +1366,15 @@
                     prop = OrderedDict({"Name": symmetry_name, "Faces": entity_list, "IsOdd": is_odd})
             else:
                 msg = "At least one edge must be provided."
                 ValueError(msg)
 
             bound = BoundaryObject(self, symmetry_name, prop, "Symmetry")
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
             return True
         except:
             return False
 
     @pyaedt_function_handler()
     def assign_current_density(
@@ -1498,15 +1498,15 @@
                                 "Value": current_density_2d,
                                 "CoordinateSystem": "",
                             }
                         )
                         bound = BoundaryObject(self, current_density_name, props, "CurrentDensity")
 
                 if bound.create():
-                    self.boundaries.append(bound)
+                    self._boundaries[bound.name] = bound
                     return bound
                 return True
             except:
                 self.logger.error("Couldn't assign current density to desired list of objects.")
                 return False
         else:
             self.logger.error("Current density can only be applied to Eddy current or magnetostatic solution types.")
@@ -1591,15 +1591,17 @@
         use_number_of_last_cycles=True,
         last_cycles_number=1,
         calculate_force="Harmonic",
         start_time="0s",
         stop_time="2ms",
         use_number_of_cycles_for_stop_time=True,
         number_of_cycles_for_stop_time=1,
+        include_no_layer=True,
     ):
+        # type: (str, dict, int, str,bool, int, str, str, str, bool, int, bool) -> bool
         """Enable the harmonic force calculation for the transient analysis.
 
         Parameters
         ----------
         layout_component_name : str
             Name of layout component to apply harmonic forces.
         nets : dict
@@ -1610,17 +1612,27 @@
             Windowing function. Default is ``"Rectangular"``.
             Available options are: ``"Rectangular"``, ``"Tri"``, ``"Van Hann"``, ``"Hamming"``,
             ``"Blackman"``, ``"Lanczos"``, ``"Welch"``.
         use_number_of_last_cycles : bool, optional
             Use number Of last cycles for force calculations. Default is ``True``.
         last_cycles_number : int, optional
             Defines the number of cycles to compute if `use_number_of_last_cycle` is ``True``.
-        calculate_force : sr, optional
+        calculate_force : str, optional
             How to calculate force. The default is ``"Harmonic"``.
             Options are ``"Harmonic"`` and ``"Transient"``.
+        start_time : str, optional
+            Harmonic Force Start Time. Default is ``"0s"``.
+        stop_time : str, optional
+            Harmonic Force Stop Time. Default is ``"2ms"``.
+        use_number_of_cycles_for_stop_time : bool, optional
+            Use number of cycles for force stop time calculations. Default is ``True``.
+        number_of_cycles_for_stop_time : int, optional
+            Number of cycles for force stop time calculations. Default is ``1``.
+        include_no_layer : bool, optional
+            Whether to include ``"<no-layer>"`` layer or not (used for vias). Default is ``True``.
 
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -1656,15 +1668,18 @@
                 "NAME:" + layout_component_name,
                 [
                     "NAME:NetLayerSetMap",
                 ],
             ],
         ]
         for net, layers in nets.items():
-            args2[1][1].append(["Name:" + net, "LayerSet:=", ["<no-layer>"] + layers])
+            if include_no_layer:
+                args2[1][1].append(["Name:" + net, "LayerSet:=", ["<no-layer>"] + layers])
+            else:
+                args2[1][1].append(["Name:" + net, "LayerSet:=", layers])
         args.append(args2)
         self.odesign.EnableHarmonicForceCalculation(args)
         return True
 
     @pyaedt_function_handler()
     def export_element_based_harmonic_force(
         self,
@@ -2413,19 +2428,19 @@
                     props[current_density_group_names[0]] = OrderedDict({"Objects": objects_list})
                     bound = BoundaryObject(self, current_density_group_names[0], props, "CurrentDensityTerminalGroup")
                 else:
                     props = OrderedDict({"Objects": objects_list})
                     bound = BoundaryObject(self, current_density_name, props, "CurrentDensityTerminal")
 
                 if bound.create():
-                    self.boundaries.append(bound)
+                    self._boundaries[bound.name] = bound
                     return bound
-                return True
+                return False
             except:
-                pass
+                return False
         else:
             self.logger.error("Current density can only be applied to Eddy current or magnetostatic solution types.")
             return False
 
     @pyaedt_function_handler()
     def _create_boundary(self, name, props, boundary_type):
         """Create a boundary.
@@ -2445,15 +2460,15 @@
             Boundary object.
 
         """
 
         bound = BoundaryObject(self, name, props, boundary_type)
         result = bound.create()
         if result:
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("Boundary %s %s has been correctly created.", boundary_type, name)
             return bound
 
         self.logger.error("Error in boundary creation for %s %s.", boundary_type, name)
         return result
 
     @pyaedt_function_handler()
@@ -2567,15 +2582,15 @@
                 }
             )
             props2 = OrderedDict(
                 {"Faces": master_entity, "CoordSysVector": u_master_vector_coordinates, "ReverseV": reverse_master}
             )
             bound = BoundaryObject(self, bound_name_m, props2, "Independent")
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
 
                 u_slave_vector_coordinates = OrderedDict(
                     {
                         "Coordinate System": "Global",
                         "Origin": u_vector_origin_coordinates_slave,
                         "UPos": u_vector_pos_coordinates_slave,
                     }
@@ -2588,15 +2603,15 @@
                         "ReverseU": reverse_slave,
                         "Independent": bound_name_m,
                         "RelationIsSame": same_as_master,
                     }
                 )
                 bound2 = BoundaryObject(self, bound_name_s, props2, "Dependent")
                 if bound2.create():
-                    self.boundaries.append(bound2)
+                    self._boundaries[bound2.name] = bound2
                     return bound, bound2
                 else:
                     return bound, False
         except:
             return False, False
 
     @pyaedt_function_handler
@@ -2644,16 +2659,18 @@
         props = {"NAME": flux_name, "Faces": []}
         for sel in objects_list:
             props["Faces"].append(sel)
 
         return self._create_boundary(flux_name, props, "FluxTangential")
 
     @pyaedt_function_handler
-    def assign_layout_force(self, nets_layers_mapping, component_name, reference_cs="Global", force_name=None):
-        # type: (dict, str, str, str) -> bool
+    def assign_layout_force(
+        self, nets_layers_mapping, component_name, reference_cs="Global", force_name=None, include_no_layer=True
+    ):
+        # type: (dict, str, str, str, bool) -> bool
         """Assign the layout force to a component in a Transient A-Phi solver.
         To access layout component features the Beta option has to be enabled first.
 
         Parameters
         ----------
         nets_layers_mapping : dict
             Each <layer, net> pair represents the object(s) in the intersection of corresponding layer and net.
@@ -2662,14 +2679,16 @@
             Name of the 3d component to assign the layout force to.
         reference_cs : str, optional
             Reference coordinate system.
             If not provided the global one will be set.
         force_name : str, optional
             Name of the layout force.
             If not provided a random name will be generated.
+        include_no_layer : bool, optional
+            Whether to include ``"<no-layer>"`` layer or not (used for vias). Default is ``True``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
@@ -2685,43 +2704,47 @@
         >>> nets_layers["<no-net>"] = ["PWR","TOP","UNNAMED_000","UNNAMED_002"]
         >>> nets_layers["GND"] = ["LYR_1","LYR_2","UNNAMED_006"]
 
         Assign layout force to a component.
         >>> m3d = Maxwell3d()
         >>> m3d.assign_layout_force(nets_layers_mapping=nets_layers, component_name="LC1_1")
         """
+
         for key in nets_layers_mapping.keys():
             if not isinstance(nets_layers_mapping[key], list):
                 nets_layers_mapping[key] = list(nets_layers_mapping[key])
 
         if component_name not in self.modeler.user_defined_component_names:
             self.logger.error("Provided component name doesn't exist in current design.")
             return False
 
         if not force_name:
             force_name = generate_unique_name("Layout_Force")
 
         nets_layers_props = None
         for key, valy in nets_layers_mapping.items():
+            layers = valy[:]
+            if include_no_layer:
+                layers = layers[:] + ["<no-layer>"]
             if nets_layers_props:
-                nets_layers_props.append(OrderedDict({key: OrderedDict({"LayerSet": valy})}))
+                nets_layers_props.append(OrderedDict({key: OrderedDict({"LayerSet": layers})}))
             else:
-                nets_layers_props = [OrderedDict({key: OrderedDict({"LayerSet": valy})})]
+                nets_layers_props = [OrderedDict({key: OrderedDict({"LayerSet": layers})})]
 
         props = OrderedDict(
             {
                 "Reference CS": reference_cs,
                 "NetsAndLayersChoices": OrderedDict(
                     {component_name: OrderedDict({"NetLayerSetMap": nets_layers_props})}
                 ),
             }
         )
         bound = MaxwellParameters(self, force_name, props, "LayoutForce")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
 
 
 class Maxwell2d(Maxwell, FieldAnalysis3D, object):
     """Provides the Maxwell 2D app interface.
 
     This class allows you to connect to an existing Maxwell 2D design or create a
@@ -2972,15 +2995,15 @@
         if not bound_name:
             bound_name = generate_unique_name("Balloon")
 
         props2 = OrderedDict({"Edges": edge_list})
         bound = BoundaryObject(self, bound_name, props2, "Balloon")
 
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_vector_potential(self, input_edge, vectorvalue=0, bound_name=None):
         """Assign a vector potential boundary condition to specified edges.
 
@@ -3013,15 +3036,15 @@
         if type(input_edge[0]) is str:
             props2 = OrderedDict({"Objects": input_edge, "Value": str(vectorvalue), "CoordinateSystem": ""})
         else:
             props2 = OrderedDict({"Edges": input_edge, "Value": str(vectorvalue), "CoordinateSystem": ""})
         bound = BoundaryObject(self, bound_name, props2, "Vector Potential")
 
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_master_slave(
         self, master_edge, slave_edge, reverse_master=False, reverse_slave=False, same_as_master=True, bound_name=None
     ):
@@ -3060,39 +3083,39 @@
             bound_name_s = generate_unique_name("Dependent")
         else:
             bound_name_m = bound_name
             bound_name_s = bound_name + "_dep"
         props2 = OrderedDict({"Edges": master_edge, "ReverseV": reverse_master})
         bound = BoundaryObject(self, bound_name_m, props2, "Independent")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
 
             props2 = OrderedDict(
                 {
                     "Edges": slave_edge,
                     "ReverseU": reverse_slave,
                     "Independent": bound_name_m,
                     "SameAsMaster": same_as_master,
                 }
             )
             bound2 = BoundaryObject(self, bound_name_s, props2, "Dependent")
             if bound2.create():
-                self.boundaries.append(bound2)
+                self._boundaries[bound2.name] = bound2
                 return bound, bound2
             else:
                 return bound, False
         return False, False
 
     @pyaedt_function_handler()
     def assign_end_connection(self, objects, resistance=0, inductance=0, bound_name=None):
         """Assign an end connection to a list of objects.
 
         Parameters
         ----------
-        objects : list of int or str or :class:`pyaedt.modeler.object3d.Object3d`
+        objects : list of int or str or :class:`pyaedt.modeler.cad.object3d.Object3d`
             List of objects to assign an end connection to.
         resistance : float or str, optional
             Resistance value. If float is provided, the units are assumed to be ohms.
             The default value is ``0``,
         inductance : float or str, optional
             Inductance value. If a float is provided, the units are assumed to Henry (H).
             The default value is ``0``.
@@ -3125,10 +3148,10 @@
                 "Objects": objects,
                 "ResistanceValue": self.modeler._arg_with_dim(resistance, "ohm"),
                 "InductanceValue": self.modeler._arg_with_dim(inductance, "H"),
             }
         )
         bound = BoundaryObject(self, bound_name, props, "EndConnection")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
```

### Comparing `pyaedt-0.6.82/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.85/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/mechanical.py` & `pyaedt-0.6.85/pyaedt/mechanical.py`

 * *Files 8% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         if intr:
             props["Intrinsics"] = intr
             props["SurfaceOnly"] = surfaces
 
         name = generate_unique_name("EMLoss")
         bound = BoundaryObject(self, name, props, "EMLoss")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("EM losses mapped from design %s.", designname)
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_thermal_map(
         self,
@@ -317,15 +317,15 @@
                 "PathRelativeTo": "TargetProject",
             }
         )
 
         name = generate_unique_name("ThermalLink")
         bound = BoundaryObject(self, name, props, "ThermalCondition")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             self.logger.info("Thermal conditions are mapped from design %s.", designname)
             return bound
 
         return True
 
     @pyaedt_function_handler()
     def assign_uniform_convection(
@@ -372,15 +372,15 @@
         props["Uniform"] = True
         props["FilmCoeff"] = str(convection_value) + convection_unit
 
         if not boundary_name:
             boundary_name = generate_unique_name("Convection")
         bound = BoundaryObject(self, boundary_name, props, "Convection")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_uniform_temperature(self, objects_list, temperature="AmbientTemp", boundary_name=""):
         """Assign a uniform temperature boundary.
 
@@ -419,15 +419,15 @@
 
         props["Temperature"] = temperature
 
         if not boundary_name:
             boundary_name = generate_unique_name("Temp")
         bound = BoundaryObject(self, boundary_name, props, "Temperature")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_frictionless_support(self, objects_list, boundary_name=""):
         """Assign a Mechanical frictionless support.
 
@@ -465,15 +465,15 @@
             else:
                 props["Faces"] = objects_list
 
         if not boundary_name:
             boundary_name = generate_unique_name("Temp")
         bound = BoundaryObject(self, boundary_name, props, "Frictionless")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_fixed_support(self, objects_list, boundary_name=""):
         """Assign a Mechanical fixed support.
 
@@ -507,15 +507,15 @@
         if type(objects_list) is list:
             props["Faces"] = objects_list
 
         if not boundary_name:
             boundary_name = generate_unique_name("Temp")
         bound = BoundaryObject(self, boundary_name, props, "FixedSupport")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @property
     def existing_analysis_sweeps(self):
         """Existing analysis sweeps in the design.
 
@@ -577,15 +577,15 @@
             props["SurfaceFlux"] = value
 
         if not boundary_name:
             boundary_name = generate_unique_name("HeatFlux")
 
         bound = BoundaryObject(self, boundary_name, props, "HeatFlux")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_heat_generation(self, objects_list, value, boundary_name=""):
         """Assign a heat generation boundary condition to an object list.
 
@@ -619,15 +619,15 @@
         props["TotalPower"] = value
 
         if not boundary_name:
             boundary_name = generate_unique_name("HeatGeneration")
 
         bound = BoundaryObject(self, boundary_name, props, "HeatGeneration")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def create_setup(self, setupname="MySetupAuto", setuptype=None, **kwargs):
         """Create an analysis setup for Mechanical.
```

### Comparing `pyaedt-0.6.82/pyaedt/misc/Console.py_build` & `pyaedt-0.6.85/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.85/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.85/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         if ret == ret.OK:
             # launch file
             version = oDesktop.GetVersion()[2:6].replace(".", "")
             python_exe = r"##PYTHON_EXE##" % version
             pyaedt_script = file_dialog.FileName
             check_file(python_exe)
             check_file(pyaedt_script)
+            os.environ["PYAEDT_SCRIPT_PROCESS_ID"] = str(oDesktop.GetProcessID())
+            os.environ["PYAEDT_SCRIPT_VERSION"] = str(oDesktop.GetVersion()[:6])
             if is_linux:
                 edt_root = os.path.normpath(oDesktop.GetExeDir())
                 os.environ["ANSYSEM_ROOT{}".format(version)] = edt_root
                 ld_library_path_dirs_to_add = [
                     "{}/commonfiles/CPython/3_7/linx64/Release/python/lib".format(edt_root),
                     "{}/commonfiles/CPython/3_10/linx64/Release/python/lib".format(edt_root),
                     "{}/common/mono/Linux64/lib64".format(edt_root),
@@ -61,23 +63,25 @@
                     "LD_LIBRARY_PATH", "")
                 command = [
                     python_exe,
                     pyaedt_script,
                     str(oDesktop.GetProcessID()),
                     str(oDesktop.GetVersion()[:6]),
                 ]
-                subprocess.Popen(command)
+                my_env = os.environ.copy()
+                subprocess.Popen(command, env=my_env)
             else:
                 command = [
                     '"{}"'.format(python_exe),
                     '"{}"'.format(pyaedt_script),
                     str(oDesktop.GetProcessID()),
                     str(oDesktop.GetVersion()[:6]),
                 ]
-                subprocess.Popen(" ".join(command))
+                my_env = os.environ.copy()
+                subprocess.Popen(" ".join(command), env=my_env)
         else:
             debug("ret didn't pass the equivalence. ret:" + repr(ret))
     except Exception as e:
         show_error(str(e))
 
 
 def check_file(file_path):
```

### Comparing `pyaedt-0.6.82/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files 19% similar despite different names*

```diff
@@ -32,31 +32,46 @@
     try:
         # launch file
         version = oDesktop.GetVersion()[2:6].replace(".", "")
         python_exe = r"##PYTHON_EXE##" % version
         pyaedt_script = r"##PYTHON_SCRIPT##"
         check_file(python_exe)
         check_file(pyaedt_script)
+        os.environ["PYAEDT_SCRIPT_PROCESS_ID"] = str(oDesktop.GetProcessID())
+        os.environ["PYAEDT_SCRIPT_VERSION"] = str(oDesktop.GetVersion()[:6])
         if is_linux:
+            edt_root = os.path.normpath(oDesktop.GetExeDir())
+            os.environ["ANSYSEM_ROOT{}".format(version)] = edt_root
+            ld_library_path_dirs_to_add = [
+                "{}/commonfiles/CPython/3_7/linx64/Release/python/lib".format(edt_root),
+                "{}/commonfiles/CPython/3_10/linx64/Release/python/lib".format(edt_root),
+                "{}/common/mono/Linux64/lib64".format(edt_root),
+                "{}/Delcross".format(edt_root),
+                "{}".format(edt_root),
+            ]
+            os.environ["LD_LIBRARY_PATH"] = ":".join(ld_library_path_dirs_to_add) + ":" + os.getenv(
+                "LD_LIBRARY_PATH", "")
             command = [
                 python_exe,
                 pyaedt_script,
                 str(oDesktop.GetProcessID()),
                 str(oDesktop.GetVersion()[:6]),
             ]
-            subprocess.Popen(command)
+            my_env = os.environ.copy()
+            subprocess.Popen(command, env=my_env)
         else:
             CREATE_NO_WINDOW = 0x08000000
             command = [
                 '"{}"'.format(python_exe),
                 '"{}"'.format(pyaedt_script),
                 str(oDesktop.GetProcessID()),
                 str(oDesktop.GetVersion()[:6]),
             ]
-            subprocess.Popen(" ".join(command), creationflags=CREATE_NO_WINDOW)
+            my_env = os.environ.copy()
+            subprocess.Popen(" ".join(command), env=my_env, creationflags=CREATE_NO_WINDOW)
     except Exception as e:
         show_error(str(e))
 
 
 def check_file(file_path):
     if not os.path.isfile(file_path):
         show_error('"{}" does not exist. Please click on the "Install PyAEDT" button in the Automation ribbon.'.format(
```

### Comparing `pyaedt-0.6.82/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.85/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/amat.xml` & `pyaedt-0.6.85/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/console_setup.py` & `pyaedt-0.6.85/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.85/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.85/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.85/pyaedt/misc/install_extra_toolkits.py`

 * *Files 23% similar despite different names*

```diff
@@ -64,28 +64,69 @@
     buttons = panel.findall("./button")
     if buttons:
         button_names = [button.attrib["label"] for button in buttons]
         if toolkitname in button_names:
             # Remove previously existing PyAEDT panel and update with newer one.
             b = [button for button in buttons if button.attrib["label"] == toolkitname][0]
             panel.remove(b)
-
+    if isinstance(toolkit, str) and os.path.exists(toolkit):
+        image_name = os.path.split(toolkit)[-1]
+    else:
+        image_name = toolkit["image"]
+    image_abs_path = image_rel_path + "images/large/{}".format(image_name)
     ET.SubElement(
         panel,
         "button",
         label=toolkitname,
         isLarge="1",
-        image=image_rel_path + "images/large/{}".format(toolkit["image"]),
+        image=image_abs_path,
         script="{}/Run PyAEDT Toolkit Script".format(toolkitname),
     )
 
     # Backup any existing file if present
     if os.path.isfile(tab_config_file_path):
         shutil.copy(tab_config_file_path, tab_config_file_path + ".orig")
 
     write_pretty_xml(root, tab_config_file_path)
 
-    files_to_copy = ["images/large/{}".format(toolkit["image"])]
+    files_to_copy = ["images/large/{}".format(image_name)]
     for file_name in files_to_copy:
         dest_file = os.path.normpath(os.path.join(pyaedt_lib_dir, file_name))
         os.makedirs(os.path.dirname(dest_file), exist_ok=True)
-        shutil.copy(os.path.normpath(os.path.join(current_dir, file_name)), dest_file)
+        if isinstance(toolkit, str):
+            shutil.copy(toolkit, dest_file)
+        else:
+            shutil.copy(os.path.normpath(os.path.join(current_dir, file_name)), dest_file)
+
+
+def remove_toolkit_config(product_toolkit_dir, toolkitname):
+    """Remove a toolkit configuration file and, if needed a button in Automation menu."""
+    tab_config_file_path = os.path.join(product_toolkit_dir, "TabConfig.xml")
+    if not os.path.isfile(tab_config_file_path):
+        return True
+    try:
+        tree = ET.parse(tab_config_file_path)
+    except ParseError as e:
+        warnings.warn("Unable to parse %s\nError received = %s" % (tab_config_file_path, str(e)))
+        return
+    root = tree.getroot()
+
+    panels = root.findall("./panel")
+    if panels:
+        panel_names = [panel.attrib["label"] for panel in panels]
+        if "Panel_PyAEDT_Toolkits" in panel_names:
+            # Remove previously existing PyAEDT panel and update with newer one.
+            panel = [panel for panel in panels if panel.attrib["label"] == "Panel_PyAEDT_Toolkits"][0]
+        else:
+            panel = ET.SubElement(root, "panel", label="Panel_PyAEDT_Toolkits")
+    else:
+        panel = ET.SubElement(root, "panel", label="Panel_PyAEDT_Toolkits")
+
+    buttons = panel.findall("./button")
+    if buttons:
+        button_names = [button.attrib["label"] for button in buttons]
+        if toolkitname in button_names:
+            # Remove previously existing PyAEDT panel and update with newer one.
+            b = [button for button in buttons if button.attrib["label"] == toolkitname][0]
+            panel.remove(b)
+
+    write_pretty_xml(root, tab_config_file_path)
```

### Comparing `pyaedt-0.6.82/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.85/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/misc.py` & `pyaedt-0.6.85/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.85/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.85/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.85/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.85/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/misc/template.acf` & `pyaedt-0.6.85/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1131,15 +1131,15 @@
             Via name. The default is ``None``.
         reference_system : str, optional
             Whether to use an existing reference system or create a new one. The default
             is ``None``, in which case a new reference system is created.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             Object created.
         """
         if not instance_name:
             instance_name = generate_unique_name("{}_".format(self.name), n=3)
             if reference_system:
                 self._app.modeler.set_working_coordinate_system(reference_system)
                 self._reference_system = reference_system
@@ -1878,15 +1878,15 @@
 
     @property
     def aedt_object(self):
         """PyAEDT object 3D.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
         """
         return self._aedt_object
 
     @property
     def layer_name(self):
         """Layer name.
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/Modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import warnings
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 from pyaedt.modeler.cad.object3d import Object3d
@@ -186,15 +185,15 @@
         Returns
         -------
         list
             List of changed properties of the coordinate system.
 
         """
         arguments = ["NAME:AllTabs", ["NAME:Geometry3DCSTab", ["NAME:PropServers", name], arg]]
-        _retry_ntimes(10, self._modeler.oeditor.ChangeProperty, arguments)
+        self._modeler.oeditor.ChangeProperty(arguments)
 
     @pyaedt_function_handler()
     def rename(self, newname):
         """Rename the coordinate system.
 
         Parameters
         ----------
@@ -1518,15 +1517,15 @@
 
         References
         ----------
 
         >>> oEditor.GetModelUnits
         >>> oEditor.SetModelUnits
         """
-        return _retry_ntimes(10, self.oeditor.GetModelUnits)
+        return self.oeditor.GetModelUnits()
 
     @model_units.setter
     def model_units(self, units):
         assert units in AEDT_UNITS["Length"], "Invalid units string {0}.".format(units)
         self.oeditor.SetModelUnits(["NAME:Units Parameter", "Units:=", units, "Rescale:=", False])
 
     @property
@@ -2635,15 +2634,15 @@
         sides : str
             Which side to keep. Options are ``"Both"``, ``"PositiveOnly"``,
             and ``"NegativeOnly"``. The default is ``"Both"``, in which case
             all objects are kept after the split.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.Object3d`
+        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
             List of split objects.
 
         References
         ----------
 
         >>> oEditor.Split
         """
@@ -2756,15 +2755,15 @@
             vArg2.append("DuplicateMirrorBaseZ:="), vArg2.append(Zpos)
             vArg2.append("DuplicateMirrorNormalX:="), vArg2.append(Xnorm)
             vArg2.append("DuplicateMirrorNormalY:="), vArg2.append(Ynorm)
             vArg2.append("DuplicateMirrorNormalZ:="), vArg2.append(Znorm)
             vArg3 = ["NAME:Options", "DuplicateAssignments:=", duplicate_assignment]
             if is_3d_comp:
                 orig_3d = [i for i in self.user_defined_component_names]
-            added_objs = _retry_ntimes(10, self.oeditor.DuplicateMirror, vArg1, vArg2, vArg3)
+            added_objs = self.oeditor.DuplicateMirror(vArg1, vArg2, vArg3)
             self.add_new_objects()
             if is_3d_comp:
                 added_3d_comps = [i for i in self.user_defined_component_names if i not in orig_3d]
                 if added_3d_comps:
                     self.logger.info("Found 3D Components Duplication")
                     return added_3d_comps
             return added_objs
@@ -2935,15 +2934,15 @@
         vArg2 = ["NAME:DuplicateToAlongLineParameters"]
         vArg2.append("CreateNewObjects:="), vArg2.append(not attachObject)
         vArg2.append("XComponent:="), vArg2.append(Xpos)
         vArg2.append("YComponent:="), vArg2.append(Ypos)
         vArg2.append("ZComponent:="), vArg2.append(Zpos)
         vArg2.append("Numclones:="), vArg2.append(str(nclones))
         vArg3 = ["NAME:Options", "DuplicateAssignments:=", duplicate_assignment]
-        _retry_ntimes(10, self.oeditor.DuplicateAlongLine, vArg1, vArg2, vArg3)
+        self.oeditor.DuplicateAlongLine(vArg1, vArg2, vArg3)
         if is_3d_comp:
             return self._duplicate_added_components_tuple()
         if attachObject:
             return True, []
         return self._duplicate_added_objects_tuple()
 
     @pyaedt_function_handler()
@@ -2957,15 +2956,15 @@
         thickness : float, str
             Amount to thicken the sheet by.
         bBothSides : bool, optional
             Whether to thicken the sheet on both side. The default is ``False``.
 
         Returns
         -------
-        pyaedt.modeler.object3d.Object3d
+        pyaedt.modeler.cad.object3d.Object3d
 
         References
         ----------
 
         >>> oEditor.ThickenSheet
         """
         selections = self.convert_to_selections(objid)
@@ -2995,15 +2994,15 @@
         face_id : int
             Face to sweep.
         sweep_value : float, optional
             Sweep value. The default is ``0.1``.
 
         Returns
         -------
-        pyaedt.modeler.object3d.Object3d
+        pyaedt.modeler.cad.object3d.Object3d
 
         References
         ----------
 
         >>> oEditor.SweepFacesAlongNormal
         """
         selections = self.convert_to_selections(obj_name)
@@ -3472,15 +3471,16 @@
 
         >>> oEditor.PurgeHistory
         """
         szList = self.convert_to_selections(theList)
 
         vArg1 = ["NAME:Selections", "Selections:=", szList, "NewPartsModelFlag:=", "Model"]
 
-        return _retry_ntimes(10, self.oeditor.PurgeHistory, vArg1)
+        self.oeditor.PurgeHistory(vArg1)
+        return True
 
     @pyaedt_function_handler()
     def get_model_bounding_box(self):
         """Retrieve the model bounding box.
 
 
         Returns
@@ -3570,16 +3570,16 @@
         ----------
 
         >>> oEditor.Copy
         >>> oEditor.Paste
         """
         szSelections = self.convert_to_selections(objid)
         vArg1 = ["NAME:Selections", "Selections:=", szSelections]
-        _retry_ntimes(10, self.oeditor.Copy, vArg1)
-        _retry_ntimes(10, self.oeditor.Paste)
+        self.oeditor.Copy(vArg1)
+        self.oeditor.Paste()
         new_objects = self.add_new_objects()
         return True, new_objects
 
     @pyaedt_function_handler()
     def intersect(self, theList, keep_originals=False, **kwargs):
         """Intersect objects from a list.
 
@@ -3918,15 +3918,15 @@
             If str, padding with units in the -Z direction.
             The default is ``0``.
         is_percentage : bool, optional
             Region definition in percentage or absolute value. The default is `True``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateRegion
         """
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/Primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import time
 
 from pyaedt.application.Variables import Variable
 from pyaedt.application.Variables import decompose_variable_value
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _dim_arg
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import is_number
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import Plane
 from pyaedt.modeler.cad.elements3d import Point
@@ -71,74 +70,74 @@
 
     @property
     def solid_objects(self):
         """List of all solid objects.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.Object3d`
+        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         """
         self._refresh_solids()
         return [self[name] for name in self.solid_names if self[name]]
 
     @property
     def sheet_objects(self):
         """List of all sheet objects.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.Object3d`
+        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         """
         self._refresh_sheets()
         return [self[name] for name in self.sheet_names if self[name]]
 
     @property
     def line_objects(self):
         """List of all line objects.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.Object3d`
+        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         """
         self._refresh_lines()
         return [self[name] for name in self.line_names if self[name]]
 
     @property
     def point_objects(self):
         """List of points objects.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.Object3d`
+        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         """
         return [v for v in list(self.points.values())]
 
     @property
     def unclassified_objects(self):
         """List of all unclassified objects.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.Object3d`
+        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         """
         self._refresh_unclassified()
         return [self[name] for name in self._unclassified if name is not None]
 
     @property
     def object_list(self):
         """List of all objects.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.Object3d`
+        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         """
         self._refresh_object_types()
         return [self[name] for name in self._all_object_names if name is not None]
 
     @property
     def solid_names(self):
@@ -365,15 +364,15 @@
         parameters.append("PointY:="), parameters.append(y_position)
         parameters.append("PointZ:="), parameters.append(z_position)
 
         attributes = ["NAME:Attributes"]
         attributes.append("Name:="), attributes.append(name)
         attributes.append("Color:="), attributes.append(color)
 
-        _retry_ntimes(10, self.oeditor.CreatePoint, parameters, attributes)
+        self.oeditor.CreatePoint(parameters, attributes)
         self._refresh_points()
         return self._create_object(name)
 
     @pyaedt_function_handler()
     def create_plane(
         self,
         name=None,
@@ -440,15 +439,15 @@
         parameters.append("PlaneNormalY:="), parameters.append(plane_normal_y)
         parameters.append("PlaneNormalZ:="), parameters.append(plane_normal_z)
 
         attributes = ["NAME:Attributes"]
         attributes.append("Name:="), attributes.append(name)
         attributes.append("Color:="), attributes.append(color)
 
-        _retry_ntimes(10, self.oeditor.CreateCutplane, parameters, attributes)
+        self.oeditor.CreateCutplane(parameters, attributes)
         # self._refresh_planes()
         self.planes[name] = None
         plane = self._create_object(name)
         self.planes[name] = plane
         return plane
 
     @pyaedt_function_handler()
@@ -456,55 +455,55 @@
         names = self._app.modeler.convert_to_selections(names_list, True)
         vChangedProps = ["NAME:ChangedProps", vPropChange]
         vPropServers = ["NAME:PropServers"]
         for el in names:
             vPropServers.append(el)
         vGeo3d = ["NAME:General", vPropServers, vChangedProps]
         vOut = ["NAME:AllTabs", vGeo3d]
-        _retry_ntimes(10, self.oeditor.ChangeProperty, vOut)
+        self.oeditor.ChangeProperty(vOut)
         return True
 
     @pyaedt_function_handler()
     def _change_geometry_property(self, vPropChange, names_list):
         names = self._app.modeler.convert_to_selections(names_list, True)
         vChangedProps = ["NAME:ChangedProps", vPropChange]
         vPropServers = ["NAME:PropServers"]
         for el in names:
             vPropServers.append(el)
         vGeo3d = ["NAME:Geometry3DAttributeTab", vPropServers, vChangedProps]
         vOut = ["NAME:AllTabs", vGeo3d]
-        _retry_ntimes(10, self.oeditor.ChangeProperty, vOut)
+        self.oeditor.ChangeProperty(vOut)
         if "NAME:Name" in vPropChange:
             self.cleanup_objects()
         return True
 
     @pyaedt_function_handler()
     def _change_point_property(self, vPropChange, names_list):
         names = self._app.modeler.convert_to_selections(names_list, True)
         vChangedProps = ["NAME:ChangedProps", vPropChange]
         vPropServers = ["NAME:PropServers"]
         for el in names:
             vPropServers.append(el)
         vGeo3d = ["NAME:Geometry3DPointTab", vPropServers, vChangedProps]
         vOut = ["NAME:AllTabs", vGeo3d]
-        _retry_ntimes(10, self.oeditor.ChangeProperty, vOut)
+        self.oeditor.ChangeProperty(vOut)
         if "NAME:Name" in vPropChange:
             self.cleanup_objects()
         return True
 
     @pyaedt_function_handler()
     def _change_plane_property(self, vPropChange, names_list):
         names = self._app.modeler.convert_to_selections(names_list, True)
         vChangedProps = ["NAME:ChangedProps", vPropChange]
         vPropServers = ["NAME:PropServers"]
         for el in names:
             vPropServers.append(el)
         vGeo3d = ["NAME:Geometry3DPlaneTab", vPropServers, vChangedProps]
         vOut = ["NAME:AllTabs", vGeo3d]
-        _retry_ntimes(10, self.oeditor.ChangeProperty, vOut)
+        self.oeditor.ChangeProperty(vOut)
         if "NAME:Name" in vPropChange:
             self.cleanup_objects()
         return True
 
     @pyaedt_function_handler()
     def update_object(self, obj):
         """Update any :class:`pyaedt.modeler.Object3d.Object3d` derivatives
@@ -513,15 +512,15 @@
         Parameters
         ----------
         obj : int, str, or :class:`pyaedt.modeler.Object3d.Object3d`
             Object to be updated after a modeler operation.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
            Updated 3D object.
 
         """
         o = self._resolve_object(obj)
         name = o.name
 
         del self.objects[self._object_names_to_ids[name]]
@@ -605,15 +604,15 @@
             Same padding is applied if not a list. The default is ``300``.
             If a list of floats or str, interpret as adding for ``["+X", "+Y", "+Z", "-X", "-Y", "-Z"]``.
         is_percentage : bool, optional
             Region definition in percentage or absolute value. The default is `True``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             Region object.
 
         References
         ----------
 
         >>> oEditor.CreateRegion
         """
@@ -1058,15 +1057,15 @@
 
     @pyaedt_function_handler()
     def get_existing_polyline(self, object):
         """Retrieve a polyline object to manipulate it.
 
         Parameters
         ----------
-        src_object : :class:`pyaedt.modeler.object3d.Object3d`
+        src_object : :class:`pyaedt.modeler.cad.object3d.Object3d`
             An existing polyline object in the 3D Modeler.
 
         Returns
         -------
         Polyline
         """
         return Polyline(self, src_object=object)
@@ -1085,15 +1084,15 @@
         upd_library : str, optional
             Name of the UDP library. The default is ``"syslib"``.
         name : str, optional
             Name of the component. The default is ``None``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             UDP object created.
 
         References
         ----------
 
         >>> oEditor.CreateUserDefinedPart
 
@@ -1318,15 +1317,15 @@
         Parameters
         ----------
         objname : str
             Name of the object.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object returned.
 
         """
         if objname in self._object_names_to_ids:
             object_id = self.get_obj_id(objname)
             return self.objects[object_id]
 
@@ -2762,62 +2761,62 @@
             return defaultmatname, self._app.materials.material_keys[defaultmatname].is_dielectric()
         else:
             return defaultmatname, True
 
     @pyaedt_function_handler()
     def _refresh_solids(self):
         try:
-            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Solids")
+            test = self.oeditor.GetObjectsInGroup("Solids")
         except TypeError:
             test = []
-        if test is None or test is False:
+        if test is False:
             assert False, "Get Solids is failing"
-        elif test is True:
+        elif test is True or test is None:
             self._solids = []  # In IronPython True is returned when no sheets are present
         else:
             self._solids = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
 
     @pyaedt_function_handler()
     def _refresh_sheets(self):
         try:
-            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Sheets")
+            test = self.oeditor.GetObjectsInGroup("Sheets")
         except TypeError:
             test = []
-        if test is None or test is False:
+        if test is False:
             assert False, "Get Sheets is failing"
-        elif test is True:
+        elif test is True or test is None:
             self._sheets = []  # In IronPython True is returned when no sheets are present
         else:
             self._sheets = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
 
     @pyaedt_function_handler()
     def _refresh_lines(self):
         try:
-            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Lines")
+            test = self.oeditor.GetObjectsInGroup("Lines")
         except TypeError:
             test = []
-        if test is None or test is False:
+        if test is False:
             assert False, "Get Lines is failing"
-        elif test is True:
+        elif test is True or test is None:
             self._lines = []  # In IronPython True is returned when no lines are present
         else:
             self._lines = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
 
     @pyaedt_function_handler()
     def _refresh_points(self):
         try:
-            test = _retry_ntimes(10, self.oeditor.GetPoints)
+            test = self.oeditor.GetPoints()
         except TypeError:
             test = []
-        if test is None or test is False:
+        if test is False:
             assert False, "Get Points is failing"
-        elif test is True:
+        elif test is True or test is None:
             self._points = []  # In IronPython True is returned when no points are present
         else:
             self._points = list(test)
         self._all_object_names = self._solids + self._sheets + self._lines + self._points
 
     @pyaedt_function_handler()
     def _refresh_planes(self):
@@ -2830,15 +2829,15 @@
         except TypeError:
             self._planes = {}
         self._all_object_names = self._solids + self._sheets + self._lines + self._points + list(self._planes.keys())
 
     @pyaedt_function_handler()
     def _refresh_unclassified(self):
         try:
-            test = _retry_ntimes(10, self.oeditor.GetObjectsInGroup, "Unclassified")
+            test = self.oeditor.GetObjectsInGroup("Unclassified")
         except TypeError:
             test = []
         if test is None or test is False:
             self._unclassified = []
             self.logger.debug("Unclassified is failing")
         elif test is True:
             self._unclassified = []  # In IronPython True is returned when no unclassified are present
@@ -3130,15 +3129,15 @@
         objListSheets = self.sheet_names
         if len(objListSheets) > 0:
             objList.extend(objListSheets)
         objListSolids = self.solid_names
         if len(objListSolids) > 0:
             objList.extend(objListSolids)
         for obj in objList:
-            val = _retry_ntimes(10, self.oeditor.GetEdgeIDsFromObject, obj)
+            val = self.oeditor.GetEdgeIDsFromObject(obj)
             if not (isinstance(val, bool)) and str(lval) in list(val):
                 return obj
         return None
 
     @pyaedt_function_handler()
     def _find_object_from_face_id(self, lval):
         if self.oeditor is not None:
@@ -3217,15 +3216,15 @@
         Parameters
         ----------
         partId : int or str
             Object ID or object name from the 3D modeler.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             Returns None if the part ID or the object name is not found.
 
         """
         if isinstance(partId, int):
             if partId in self.objects:
                 return self.objects[partId]
         elif partId in self._object_names_to_ids:
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/Primitives2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             a unique name ``"NewObject_xxxxxx"`` will be assigned)
         matname : str, optional
             Name of the material. The default is ``None``. If ``None``,
             the default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateCircle
 
@@ -106,15 +106,15 @@
             a unique name NewObject_xxxxxx will be assigned)
         matname : str, default=None
              Name of the material. The default is ``None``. If ``None``,
              the default material is assigned.
 
         Returns
         -------
-        pyaedt.modeler.object3d.Object3d
+        pyaedt.modeler.cad.object3d.Object3d
             Object 3d.
 
         References
         ----------
 
         >>> oEditor.CreateEllipse
 
@@ -157,15 +157,15 @@
             a unique name NewObject_xxxxxx will be assigned)
         matname : str, default=None
              Name of the material. The default is ``None``. If ``None``,
              the default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
 
         References
         ----------
 
         >>> oEditor.CreateRectangle
 
         Examples
@@ -213,15 +213,15 @@
             a unique name NewObject_xxxxxx will be assigned)
         matname : str, default=None
              Name of the material. The default is ``None``. If ``None``,
              the default material is assigned.
 
         Returns
         -------
-        pyaedt.modeler.object3d.Object3d
+        pyaedt.modeler.cad.object3d.Object3d
 
         References
         ----------
 
         >>> oEditor.CreateRegularPolygon
 
         Examples
@@ -263,15 +263,15 @@
             Same padding is applied if not a list. The default is ``300``.
             If a list of floats or str, interpret as adding for ``["+X", "+Y", "-X", "-Y"]``.
         is_percentage : bool, optional
             Region definition in percentage or absolute value. The default is `True``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             Region object.
 
         References
         ----------
 
         >>> oEditor.CreateRegion
         """
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from math import sqrt
 from math import tan
 import os
 
 from pyaedt import Edb
 from pyaedt import Icepak
 from pyaedt.generic import LoadAEDTFile
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import normalize_path
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.advanced_cad.actors import Bird
 from pyaedt.modeler.advanced_cad.actors import Person
 from pyaedt.modeler.advanced_cad.actors import Vehicle
@@ -69,15 +68,15 @@
         matname : str, optional
             Name of the material.  The default is ``None``, in which case the
             default material is assigned. If the material name supplied is
             invalid, the default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateBox
 
@@ -100,15 +99,15 @@
         vArg1.append("XPosition:="), vArg1.append(XPosition)
         vArg1.append("YPosition:="), vArg1.append(YPosition)
         vArg1.append("ZPosition:="), vArg1.append(ZPosition)
         vArg1.append("XSize:="), vArg1.append(XSize)
         vArg1.append("YSize:="), vArg1.append(YSize)
         vArg1.append("ZSize:="), vArg1.append(ZSize)
         vArg2 = self._default_object_attributes(name=name, matname=matname)
-        new_object_name = _retry_ntimes(10, self.oeditor.CreateBox, vArg1, vArg2)
+        new_object_name = self.oeditor.CreateBox(vArg1, vArg2)
         return self._create_object(new_object_name)
 
     @pyaedt_function_handler()
     def create_cylinder(self, cs_axis, position, radius, height, numSides=0, name=None, matname=None):
         """Create a cylinder.
 
         Parameters
@@ -130,15 +129,15 @@
             the default name is assigned.
         matname : str, optional
             Name of the material. The default is ''None``, in which case the
             default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateCylinder
 
@@ -205,15 +204,15 @@
             default name is assigned.
         matname : str, optional
             Name of the material. The default is ``None``, in which the
             default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateRegularPolyhedron
 
@@ -270,15 +269,15 @@
             the default name is assigned.
         matname : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateCone
 
@@ -334,15 +333,15 @@
             the default name is assigned.
         matname : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateSphere
 
@@ -393,15 +392,15 @@
         material_name : str, optional
             Name of the material.  The default is ``None``, in which case the
             default material is assigned. If the material name supplied is
             invalid, the default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateTorus
 
@@ -433,15 +432,15 @@
         first_argument.append("XCenter:="), first_argument.append(x_center)
         first_argument.append("YCenter:="), first_argument.append(y_center)
         first_argument.append("ZCenter:="), first_argument.append(z_center)
         first_argument.append("MajorRadius:="), first_argument.append(major_radius)
         first_argument.append("MinorRadius:="), first_argument.append(minor_radius)
         first_argument.append("WhichAxis:="), first_argument.append(axis)
         second_argument = self._default_object_attributes(name=name, matname=material_name)
-        new_object_name = _retry_ntimes(10, self.oeditor.CreateTorus, first_argument, second_argument)
+        new_object_name = self.oeditor.CreateTorus(first_argument, second_argument)
         return self._create_object(new_object_name)
 
     @pyaedt_function_handler()
     def create_bondwire(
         self,
         start_position,
         end_position,
@@ -450,14 +449,15 @@
         alpha=80,
         beta=5,
         bond_type=0,
         diameter=0.025,
         facets=6,
         name=None,
         matname=None,
+        cs_axis="Z",
     ):
         # type : (list, list, float|str=0.2, float|str=0, float=80, float=5, int=0, float|str=0.025, int=6, str=None,
         # str=None) -> Object3d
         """Create a bondwire.
 
         Parameters
         ----------
@@ -496,18 +496,20 @@
             Number of wire facets. The default is ``6``.
         name : str, optional
             Name of the bondwire. The default is ``None``, in which case
             the default name is assigned.
         matname : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
+        cs_axis : str, optional
+            Coordinate system axis. The default is ``"Z"``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateBondwire
 
@@ -584,15 +586,15 @@
 
         first_argument.append("Distance:="), first_argument.append(distance)
 
         first_argument.append("h1:="), first_argument.append(self._arg_with_dim(h1))
         first_argument.append("h2:="), first_argument.append(self._arg_with_dim(h2))
         first_argument.append("alpha:="), first_argument.append(self._arg_with_dim(alpha, "deg"))
         first_argument.append("beta:="), first_argument.append(self._arg_with_dim(beta, "deg"))
-        first_argument.append("WhichAxis:="), first_argument.append("Z")
+        first_argument.append("WhichAxis:="), first_argument.append(GeometryOperators.cs_axis_str(cs_axis))
         first_argument.append("ReverseDirection:="), first_argument.append(False)
         second_argument = self._default_object_attributes(name=name, matname=matname)
         new_object_name = self.oeditor.CreateBondwire(first_argument, second_argument)
         return self._create_object(new_object_name)
 
     @pyaedt_function_handler()
     def create_rectangle(self, csPlane, position, dimension_list, name=None, matname=None, is_covered=True):
@@ -615,15 +617,15 @@
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
         is_covered : bool, optional
             Whether the rectangle is covered. The default is ``True``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateRectangle
 
@@ -670,15 +672,15 @@
             Name of the material. The default is ``None``, in which case the
             default material is assigned.
         non_model : bool, optional
              Either if create the new object as model or non-model. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateCircle
 
@@ -725,15 +727,15 @@
             default name is assigned.
         matname : str, optional
             Name of the material. The default is ``None``, in which case the
             default material is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateEllipse
 
@@ -818,15 +820,15 @@
         xsection_bend_type : str, optional
             Type of the bend for the cross-section. The default is ``None``, in which
             case the bend type is set to ``"Corner"``. For the type ``"Circle"``, the
             bend type should be set to ``"Curved"``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateEquationCurve
 
@@ -898,15 +900,15 @@
             Whether the helix turning direction is right hand. The default value is ``True``.
         radius_increment : float, optional
             Radius change per turn. The default value is ``0.0``.
         thread : float
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateHelix
 
@@ -956,15 +958,15 @@
         Parameters
         ----------
         object_name : int, str, or Object3d
             Specified for the object.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
 
@@ -1469,27 +1471,30 @@
     @pyaedt_function_handler()
     def insert_layout_component(
         self,
         comp_file,
         coordinate_system="Global",
         name=None,
         parameter_mapping=False,
+        layout_coordinate_systems=[],
     ):
         """Insert a new layout component.
 
         Parameters
         ----------
         comp_file : str
             Path of the component file. Either ``".aedb"`` and ``".aedbcomp"`` are allowed.
         coordinate_system : str, optional
             Target coordinate system. The default is ``"Global"``.
         name : str, optional
             3D component name. The default is ``None``.
         parameter_mapping : bool, optional
             Map the layout parameters in the target HFSS design. The default is ``False``.
+        layout_coordinate_systems : list, optional
+            Coordinate system to import. The default is all available coordinate systems.
 
         Returns
         -------
         :class:`pyaedt.modeler.components_3d.UserDefinedComponent`
             User defined component object.
 
         References
@@ -1595,15 +1600,15 @@
             "",
             "Help URL:=",
             "",
             "Version:=",
             "1.0",
             "Notes:=",
             "",
-            "IconTypeL:=",
+            "IconType:=",
             "Layout Component",
         ]
         vArg1.append(varg4)
         varg5 = [
             "NAME:GeometryDefinitionParameters",
         ]
         if parameters and parameter_mapping:
@@ -1658,19 +1663,25 @@
             aedt_component_name,
             varg8,
             "ReferenceCS:=",
             "Global",
             "CSToImport:=",
         ]
 
-        if component_cs:
+        if component_cs and not layout_coordinate_systems:  # pragma: no cover
             varg10 = component_cs
             varg10.append("Global")
+        elif component_cs and layout_coordinate_systems:  # pragma: no cover
+            varg10 = ["Global"]
+            for cs in layout_coordinate_systems:
+                if cs in component_cs:
+                    varg10.append(cs)
         else:
             varg10 = ["Global"]
+
         varg9.append(varg10)
         vArg1.append(varg9)
 
         varg11 = ["NAME:InstanceParameters"]
         varg11.append("GeometryParameters:=")
 
         if parameters and parameter_mapping:
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/components_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import random
 import re
 import warnings
 
 # from pyaedt import property
 from pyaedt import Edb
 from pyaedt import pyaedt_function_handler
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.modeler.cad.elements3d import BinaryTreeNode
 from pyaedt.modeler.cad.elements3d import _dict2arg
 
 
 class UserDefinedComponentParameters(dict):
     def __setitem__(self, key, value):
@@ -1078,10 +1077,10 @@
                 objects_mode.append(self.objects[objects])
             vPropChange.append(objects_mode)
 
         vChangedProps = ["NAME:ChangedProps", vPropChange]
         vPropServers = ["NAME:PropServers", self._name]
         vGeo3d = ["NAME:Visualization", vPropServers, vChangedProps]
         vOut = ["NAME:AllTabs", vGeo3d]
-        _retry_ntimes(10, self._primitives.oeditor.ChangeProperty, vOut)
+        self._primitives.oeditor.ChangeProperty(vOut)
 
         return True
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/elements3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import absolute_import
 
 from collections import OrderedDict
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _dim_arg
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import clamp
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import rgb_color_codes
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
@@ -191,15 +190,15 @@
 
 
 class VertexPrimitive(EdgeTypePrimitive, object):
     """Contains the vertex object within the AEDT Desktop Modeler.
 
     Parameters
     ----------
-    object3d : :class:`pyaedt.modeler.object3d.Object3d`
+    object3d : :class:`pyaedt.modeler.cad.object3d.Object3d`
         Pointer to the calling object that provides additional functionality.
     objid : int
         Object ID as determined by the parent object.
 
     """
 
     def __init__(self, object3d, objid, position=None):
@@ -241,15 +240,15 @@
 
 
 class EdgePrimitive(EdgeTypePrimitive, object):
     """Contains the edge object within the AEDT Desktop Modeler.
 
     Parameters
     ----------
-    object3d : :class:`pyaedt.modeler.object3d.Object3d`
+    object3d : :class:`pyaedt.modeler.cad.object3d.Object3d`
         Pointer to the calling object that provides additional functionality.
     edge_id : int
         Object ID as determined by the parent object.
 
     """
 
     def __init__(self, object3d, edge_id):
@@ -301,15 +300,15 @@
 
     @property
     def vertices(self):
         """Vertices list.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.VertexPrimitive`
+        list of :class:`pyaedt.modeler.cad.object3d.VertexPrimitive`
             List of vertices.
 
         References
         ----------
 
         >>> oEditor.GetVertexIDsFromEdge
 
@@ -379,15 +378,15 @@
 
     @pyaedt_function_handler()
     def create_object(self, non_model=False):
         """Return a new object from the selected edge.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         non_model : bool, optional
             Either if create the new object as model or non-model. The default is `False`.
 
         References
         ----------
 
@@ -432,15 +431,15 @@
         return "FaceId " + str(self.id)
 
     def __init__(self, object3d, obj_id):
         """
 
         Parameters
         ----------
-        object3d : :class:`pyaedt.modeler.object3d.Object3d`
+        object3d : :class:`pyaedt.modeler.cad.object3d.Object3d`
         obj_id : int
         """
         self._id = obj_id
         self._object3d = object3d
 
     @property
     def oeditor(self):
@@ -486,15 +485,15 @@
 
     @property
     def edges(self):
         """Edges lists.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.EdgePrimitive`
+        list of :class:`pyaedt.modeler.cad.object3d.EdgePrimitive`
             List of Edges.
 
         References
         ----------
 
         >>> oEditor.GetEdgeIDsFromFace
 
@@ -506,15 +505,15 @@
 
     @property
     def vertices(self):
         """Vertices lists.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d.VertexPrimitive`
+        list of :class:`pyaedt.modeler.cad.object3d.VertexPrimitive`
             List of Vertices.
 
         References
         ----------
 
         >>> oEditor.GetVertexIDsFromFace
 
@@ -600,15 +599,19 @@
             return [float(i) for i in self.oeditor.GetFaceCenter(self.id)]
         except:  # pragma: no cover
             vtx = self.vertices
             if len(vtx) > 1:
                 return GeometryOperators.get_polygon_centroid([pos.position for pos in vtx])
             elif len(vtx) <= 1:
                 eval_points = 4
-                edge = self.edges[0]
+                try:
+                    edge = self.edges[0]
+                except IndexError:
+                    self.logger.error("At least one edge is needed to compute face center.")
+                    return
                 centroid = GeometryOperators.get_polygon_centroid(
                     [
                         [
                             float(i)
                             for i in self.oeditor.GetEdgePositionAtNormalizedParameter(
                                 edge.id, float(pos) / eval_points
                             )
@@ -638,15 +641,15 @@
 
     @property
     def top_edge_z(self):
         """Top edge in the Z direction of the object. Midpoint is used as criteria to find the edge.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.EdgePrimitive`
+        :class:`pyaedt.modeler.cad.object3d.EdgePrimitive`
 
         References
         ----------
 
         >>> oEditor.FaceCenter
 
         """
@@ -659,15 +662,15 @@
 
     @property
     def bottom_edge_z(self):
         """Bottom edge in the Z direction of the object. Midpoint is used as criteria to find the edge.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.EdgePrimitive`
+        :class:`pyaedt.modeler.cad.object3d.EdgePrimitive`
 
         """
         try:
             result = [(float(edge.midpoint[2]), edge) for edge in self.edges]
             result = sorted(result, key=lambda tup: tup[0])
             return result[0][1]
         except:
@@ -675,15 +678,15 @@
 
     @property
     def top_edge_x(self):
         """Top edge in the X direction of the object. Midpoint is used as criteria to find the edge.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.EdgePrimitive`
+        :class:`pyaedt.modeler.cad.object3d.EdgePrimitive`
 
         """
         try:
             result = [(float(edge.midpoint[0]), edge) for edge in self.edges]
             result = sorted(result, key=lambda tup: tup[0])
             return result[-1][1]
         except:
@@ -691,15 +694,15 @@
 
     @property
     def bottom_edge_x(self):
         """Bottom edge in the X direction of the object. Midpoint is used as criteria to find the edge.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.EdgePrimitive`
+        :class:`pyaedt.modeler.cad.object3d.EdgePrimitive`
 
         """
         try:
             result = [(float(edge.midpoint[0]), edge) for edge in self.edges]
             result = sorted(result, key=lambda tup: tup[0])
             return result[0][1]
         except:
@@ -707,15 +710,15 @@
 
     @property
     def top_edge_y(self):
         """Top edge in the Y direction of the object. Midpoint is used as criteria to find the edge.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.EdgePrimitive`
+        :class:`pyaedt.modeler.cad.object3d.EdgePrimitive`
 
         """
         try:
             result = [(float(edge.midpoint[1]), edge) for edge in self.edges]
             result = sorted(result, key=lambda tup: tup[0])
             return result[-1][1]
         except:
@@ -723,15 +726,15 @@
 
     @property
     def bottom_edge_y(self):
         """Bottom edge in the X direction of the object. Midpoint is used as criteria to find the edge.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.EdgePrimitive`
+        :class:`pyaedt.modeler.cad.object3d.EdgePrimitive`
 
         """
         try:
             result = [(float(edge.midpoint[1]), edge) for edge in self.edges]
             result = sorted(result, key=lambda tup: tup[0])
             return result[0][1]
         except:
@@ -914,15 +917,15 @@
 
     @pyaedt_function_handler()
     def create_object(self, non_model=False):
         """Return a new object from the selected face.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
         non_model : bool, optional
             Either if create the new object as model or non-model. Default is `False`.
 
         References
         ----------
 
@@ -1008,15 +1011,15 @@
                 name_property.append("Value:=")
                 name_property.append(point_name)
                 changed_property = ["NAME:ChangedProps", name_property]
                 property_servers = ["NAME:PropServers"]
                 property_servers.append(self._name)
                 point_tab = ["NAME:Geometry3DPointTab", property_servers, changed_property]
                 all_tabs = ["NAME:AllTabs", point_tab]
-                _retry_ntimes(10, self._primitives.oeditor.ChangeProperty, all_tabs)
+                self._primitives.oeditor.ChangeProperty(all_tabs)
                 self._name = point_name
                 self._primitives.cleanup_objects()
         else:
             self.logger.warning("A point named '%s' already exists.", point_name)
 
     @property
     def valid_properties(self):
@@ -1024,21 +1027,20 @@
 
         References
         ----------
 
         >>> oEditor.GetProperties
         """
         if not self._all_props:
-            self._all_props = _retry_ntimes(10, self._oeditor.GetProperties, "Geometry3DPointTab", self._name)
+            self._all_props = self._oeditor.GetProperties("Geometry3DPointTab", self._name)
         return self._all_props
 
     # Note: We currently cannot get the color property value because
     # when we try to access it, we only get access to the 'edit' button.
     # Following is the line that we would use but it currently returns 'edit'.
-    # color = _retry_ntimes(10, self._oeditor.GetPropertyValue, "Geometry3DPointTab", self._name, "Color")
     def set_color(self, color_value):
         """Set symbol color.
 
         Parameters
         ----------
         color_value : string
             String exposing the new color of the point in the format of "(001 255 255)".
@@ -1097,16 +1099,16 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._point_coordinate_system is not None:
             return self._point_coordinate_system
         if "Orientation" in self.valid_properties:
-            self._point_coordinate_system = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DPointTab", self._name, "Orientation"
+            self._point_coordinate_system = self._oeditor.GetPropertyValue(
+                "Geometry3DPointTab", self._name, "Orientation"
             )
             return self._point_coordinate_system
 
     @coordinate_system.setter
     def coordinate_system(self, new_coordinate_system):
         coordinate_system = ["NAME:Orientation", "Value:=", new_coordinate_system]
         self._change_property(coordinate_system)
@@ -1211,15 +1213,15 @@
                 name_property.append("Value:=")
                 name_property.append(plane_name)
                 changed_property = ["NAME:ChangedProps", name_property]
                 property_servers = ["NAME:PropServers"]
                 property_servers.append(self._name)
                 plane_tab = ["NAME:Geometry3DPlaneTab", property_servers, changed_property]
                 all_tabs = ["NAME:AllTabs", plane_tab]
-                _retry_ntimes(10, self._primitives.oeditor.ChangeProperty, all_tabs)
+                self._primitives.oeditor.ChangeProperty(all_tabs)
                 self._name = plane_name
                 # TO BE DELETED self._primitives.cleanup_objects()
                 # Update the name of the plane in the ``planes`` dictionary listing all existing planes.
                 self._primitives.planes[plane_name] = self._primitives.planes.pop(plane_old_name)
         else:
             self.logger.warning("A plane named '%s' already exists.", plane_name)
 
@@ -1229,21 +1231,20 @@
 
         References
         ----------
 
         >>> oEditor.GetProperties
         """
         if not self._all_props:
-            self._all_props = _retry_ntimes(10, self._oeditor.GetProperties, "Geometry3DPlaneTab", self._name)
+            self._all_props = self._oeditor.GetProperties("Geometry3DPlaneTab", self._name)
         return self._all_props
 
     # Note: You currently cannot get the color property value because
     # when you try to access it, you only get access to the 'edit' button.
     # Following is the line that you would use, but it currently returns 'edit'.
-    # color = _retry_ntimes(10, self._oeditor.GetPropertyValue, "Geometry3DPlaneTab", self._name, "Color")
     @pyaedt_function_handler()
     def set_color(self, color_value):
         """Set symbol color.
 
         Parameters
         ----------
         color_value : string
@@ -1303,16 +1304,16 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._plane_coordinate_system is not None:
             return self._plane_coordinate_system
         if "Orientation" in self.valid_properties:
-            self._plane_coordinate_system = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DPlaneTab", self._name, "Orientation"
+            self._plane_coordinate_system = self._oeditor.GetPropertyValue(
+                "Geometry3DPlaneTab", self._name, "Orientation"
             )
             return self._plane_coordinate_system
 
     @coordinate_system.setter
     def coordinate_system(self, new_coordinate_system):
         coordinate_system = ["NAME:Orientation", "Value:=", new_coordinate_system]
         self._change_property(coordinate_system)
@@ -1357,14 +1358,16 @@
         OrderedDict.__setitem__(self, key, value)
 
 
 class BinaryTreeNode:
     """Manages an object's history structure."""
 
     def __init__(self, node, child_object, first_level=False, get_child_obj_arg=None, root_name=None):
+        if not root_name:
+            root_name = node
         saved_root_name = node if first_level else root_name
         self.node = node
         self.child_object = child_object
         self.children = {}
         self.auto_update = True
         name = None
         if get_child_obj_arg is None:
@@ -1391,15 +1394,18 @@
             self.props = self.children[name].props
             if name == "CreatePolyline:1":
                 self.segments = self.children[name].children
             del self.children[name]
         else:
             self.props = {}
             for p in self.child_object.GetPropNames():
-                self.props[p] = self.child_object.GetPropValue(p)
+                try:
+                    self.props[p] = self.child_object.GetPropValue(p)
+                except:
+                    self.props[p] = None
             self.props = HistoryProps(self, self.props)
         self.command = self.props.get("Command", "")
 
     def update_property(self, prop_name, prop_value):
         """Update the property of the binary tree node.
 
         Parameters
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/object3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import os
 import re
 
 from pyaedt.generic.constants import AEDT_UNITS
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _to_boolean
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import clamp
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import rgb_color_codes
@@ -789,16 +788,16 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._surface_material is not None:
             return self._surface_material
         if "Surface Material" in self.valid_properties and self.model:
-            self._surface_material = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Surface Material"
+            self._surface_material = self._oeditor.GetPropertyValue(
+                "Geometry3DAttributeTab", self._m_name, "Surface Material"
             )
             return self._surface_material.strip('"')
 
     @property
     def group_name(self):
         """Group the object belongs to.
 
@@ -813,17 +812,15 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._m_groupName is not None:
             return self._m_groupName
         if "Group" in self.valid_properties:
-            self._m_groupName = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Group"
-            )
+            self._m_groupName = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Group")
             return self._m_groupName
 
     @group_name.setter
     def group_name(self, name):
         """Assign Object to a specific group. it creates a new group if the group doesn't exist.
 
         Parameters
@@ -854,17 +851,15 @@
                     self._m_name,
                     "SubmodelInstances:=",
                     "",
                     "Groups:=",
                     "",
                 ]
             )
-            groupName = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Group"
-            )
+            groupName = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Group")
             self._oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:Attributes",
                         ["NAME:PropServers", groupName],
                         ["NAME:ChangedProps", ["NAME:Name", "Value:=", name]],
@@ -899,15 +894,15 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._material_name is not None:
             return self._material_name
         if "Material" in self.valid_properties and self.model:
-            mat = _retry_ntimes(10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Material")
+            mat = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Material")
             self._material_name = ""
             if mat:
                 self._material_name = mat.strip('"').lower()
             return self._material_name
         return ""
 
     @material_name.setter
@@ -1081,15 +1076,15 @@
                 vName.append("Value:=")
                 vName.append(obj_name)
                 vChangedProps = ["NAME:ChangedProps", vName]
                 vPropServers = ["NAME:PropServers"]
                 vPropServers.append(self._m_name)
                 vGeo3d = ["NAME:Geometry3DAttributeTab", vPropServers, vChangedProps]
                 vOut = ["NAME:AllTabs", vGeo3d]
-                _retry_ntimes(10, self._primitives.oeditor.ChangeProperty, vOut)
+                self._primitives.oeditor.ChangeProperty(vOut)
                 self._m_name = obj_name
                 self._primitives.add_new_objects()
                 self._primitives.cleanup_objects()
         else:
             pass
 
     @property
@@ -1098,15 +1093,15 @@
 
         References
         ----------
 
         >>> oEditor.GetProperties
         """
         if not self._all_props:
-            self._all_props = _retry_ntimes(10, self._oeditor.GetProperties, "Geometry3DAttributeTab", self._m_name)
+            self._all_props = self._oeditor.GetProperties("Geometry3DAttributeTab", self._m_name)
         return self._all_props
 
     @property
     def color(self):
         """Part color as a tuple of integer values for `(Red, Green, Blue)` color values.
 
         If the integer values are outside the range 0-255, then limit the values. Invalid inputs are ignored.
@@ -1121,15 +1116,15 @@
         --------
         >>> part.color = (255,255,0)
 
         """
         if self._color is not None:
             return self._color
         if "Color" in self.valid_properties:
-            color = _retry_ntimes(10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Color")
+            color = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Color")
             if color:
                 b = (int(color) >> 16) & 255
                 g = (int(color) >> 8) & 255
                 r = int(color) & 255
                 self._color = (r, g, b)
             else:
                 self._color = (0, 195, 255)
@@ -1189,17 +1184,15 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._transparency is not None:
             return self._transparency
         if "Transparent" in self.valid_properties:
-            transp = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Transparent"
-            )
+            transp = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Transparent")
             try:
                 self._transparency = float(transp)
             except:
                 self._transparency = 0.3
             return self._transparency
 
     @transparency.setter
@@ -1238,16 +1231,16 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._part_coordinate_system is not None and not isinstance(self._part_coordinate_system, int):
             return self._part_coordinate_system
         if "Orientation" in self.valid_properties:
-            self._part_coordinate_system = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Orientation"
+            self._part_coordinate_system = self._oeditor.GetPropertyValue(
+                "Geometry3DAttributeTab", self._m_name, "Orientation"
             )
             return self._part_coordinate_system
 
     @part_coordinate_system.setter
     def part_coordinate_system(self, sCS):
         pcs = ["NAME:Orientation", "Value:=", sCS]
         self._change_property(pcs)
@@ -1269,17 +1262,15 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._solve_inside is not None:
             return self._solve_inside
         if "Solve Inside" in self.valid_properties and self.model:
-            solveinside = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Solve Inside"
-            )
+            solveinside = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Solve Inside")
             if solveinside == "false" or solveinside == "False":
                 self._solve_inside = False
             else:
                 self._solve_inside = True
             return self._solve_inside
         return None
 
@@ -1311,17 +1302,15 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._wireframe is not None:
             return self._wireframe
         if "Display Wireframe" in self.valid_properties:
-            wireframe = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Display Wireframe"
-            )
+            wireframe = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Display Wireframe")
             if wireframe == "true" or wireframe == "True":
                 self._wireframe = True
             else:
                 self._wireframe = False
             return self._wireframe
 
     @display_wireframe.setter
@@ -1364,15 +1353,15 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
 
         """
         if self._model is not None:
             return self._model
         if "Model" in self.valid_properties:
-            mod = _retry_ntimes(10, self._oeditor.GetPropertyValue, "Geometry3DAttributeTab", self._m_name, "Model")
+            mod = self._oeditor.GetPropertyValue("Geometry3DAttributeTab", self._m_name, "Model")
             if mod == "false" or mod == "False":
                 self._model = False
             else:
                 self._model = True
             return self._model
 
     @model.setter
@@ -1384,15 +1373,15 @@
 
     @pyaedt_function_handler()
     def unite(self, object_list):
         """Unite a list of objects with this object.
 
         Parameters
         ----------
-        object_list : list of str or list of pyaedt.modeler.object3d.Object3d
+        object_list : list of str or list of pyaedt.modeler.cad.object3d.Object3d
             List of objects.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
            Object 3D object.
 
@@ -1629,15 +1618,15 @@
     def sweep_along_path(
         self, sweep_object, draft_angle=0, draft_type="Round", is_check_face_intersection=False, twist_angle=0
     ):
         """Sweep the selection along a vector.
 
         Parameters
         ----------
-        sweep_object : :class:`pyaedt.modeler.object3d.Object3d`
+        sweep_object : :class:`pyaedt.modeler.cad.object3d.Object3d`
             Application.Position object.
         draft_angle : float, optional
             Angle of the draft in degrees. The default is ``0``.
         draft_type : str
             Type of the draft. Options are ``"Extended"``, ``"Round"``,
             and ``"Natural"``. The default is ``"Round``.
         is_check_face_intersection : bool, optional
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.85/pyaedt/modeler/cad/polylines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import absolute_import
 
 import math
 import warnings
 
 # from pyaedt import property
-from pyaedt import _retry_ntimes
 from pyaedt import pyaedt_function_handler
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import PLANE
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.cad.object3d import Object3d
 from pyaedt.modeler.geometry_operators import GeometryOperators
@@ -321,15 +320,15 @@
             varg1 = self._point_segment_string_array()
             if non_model:
                 flag = "NonModel#"
             else:
                 flag = ""
             varg2 = self._primitives._default_object_attributes(name=name, matname=matname, flags=flag)
 
-            new_object_name = _retry_ntimes(10, self._oeditor.CreatePolyline, varg1, varg2)
+            new_object_name = self._oeditor.CreatePolyline(varg1, varg2)
             Object3d.__init__(self, primitives, name=new_object_name)
             self._primitives._create_object(self.name)
 
     @property
     def start_point(self):
         """List of the ``[x, y, z]`` coordinates for the starting point in the polyline
         object in the object's coordinate system.
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/calculators.py` & `pyaedt-0.6.85/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import warnings
 
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import filter_string
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import recursive_glob
 from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
 from pyaedt.modeler.circuits.object3dcircuit import Wire
@@ -288,15 +287,15 @@
         location : list, optional
             Position on the X and Y axis. The default is ``None``.
         angle : optional
             Angle rotation in degrees. The default is ``0``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreatePagePort
         """
@@ -321,15 +320,15 @@
         location : list, optional
             Position on the X and Y axis. The default is ``None``.
         angle : optional
             Angle rotation in degrees. The default is ``0``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
         >>> oEditor.CreateGround
         """
         xpos, ypos = self._get_location(location)
@@ -343,23 +342,26 @@
         self.add_id_to_component(id)
         # return id, self.components[id].composed_name
         for el in self.components:
             if name in self.components[el].composed_name:
                 return self.components[el]
 
     @pyaedt_function_handler()
-    def create_model_from_touchstone(self, touchstone_full_path, model_name=None):
+    def create_model_from_touchstone(self, touchstone_full_path, model_name=None, show_bitmap=True):
         """Create a model from a Touchstone file.
 
         Parameters
         ----------
         touchstone_full_path : str
             Full path to the Touchstone file.
         model_name : str, optional
             Name of the model. The default is ``None``.
+        show_bitmap : bool, optional
+            Show bitmap image of schematic component.
+            The default value is ``True``.
 
         Returns
         -------
         str
             Model name when successfully created. ``False`` if something went wrong.
 
         References
@@ -400,15 +402,21 @@
         if not model_name:
             model_name = os.path.splitext(os.path.basename(touchstone_full_path))[0]
         if model_name in list(self.o_model_manager.GetNames()):
             model_name = generate_unique_name(model_name, n=2)
         num_terminal = int(os.path.splitext(touchstone_full_path)[1].lower().strip(".sp"))
         with open_file(touchstone_full_path, "r") as f:
             port_names = _parse_ports_name(f, num_terminal)
-        image_subcircuit_path = os.path.join(self._modeler._app.desktop_install_dir, "syslib", "Bitmaps", "nport.bmp")
+        image_subcircuit_path = ""
+        bmp_file_name = ""
+        if show_bitmap:
+            image_subcircuit_path = os.path.join(
+                self._modeler._app.desktop_install_dir, "syslib", "Bitmaps", "nport.bmp"
+            )
+            bmp_file_name = os.path.basename(image_subcircuit_path)
 
         if not port_names:
             port_names = ["Port" + str(i + 1) for i in range(num_terminal)]
         arg = [
             "NAME:" + model_name,
             "Name:=",
             model_name,
@@ -534,15 +542,15 @@
                 "Description:=",
                 "",
                 "InfoTopic:=",
                 "",
                 "InfoHelpFile:=",
                 "",
                 "IconFile:=",
-                "nport.bmp",
+                bmp_file_name,
                 "Library:=",
                 "",
                 "OriginalLocation:=",
                 "Project",
                 "IEEE:=",
                 "",
                 "Author:=",
@@ -613,46 +621,59 @@
 
     @pyaedt_function_handler()
     def create_touchsthone_component(
         self,
         model_name,
         location=[],
         angle=0,
+        show_bitmap=True,
     ):
         """Create a component from a Touchstone model.
 
         Parameters
         ----------
         model_name : str
             Name of the Touchstone model or full path to touchstone file.
             If full touchstone is provided then, new model will be created.
         location : list of float, optional
             Position on the X  and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
+        show_bitmap : bool, optional
+            Show bitmap image of schematic component.
+            The default value is ``True``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oModelManager.Add
         >>> oComponentManager.Add
         >>> oEditor.CreateComponent
+
+        Examples
+        --------
+
+        >>> from pyaedt import Circuit
+        >>> cir = Circuit()
+        >>> comps = cir.modeler.components
+        >>> s_parameter_path = os.path.join("your_path", "s_param_file_name.s4p")
+        >>> circuit_comp = comps.create_touchsthone_component(s_parameter_path, location=[0.0, 0.0], show_bitmap=False)
         """
         xpos, ypos = self._get_location(location)
         id = self.create_unique_id()
         if os.path.exists(model_name):
-            model_name = self.create_model_from_touchstone(model_name)
+            model_name = self.create_model_from_touchstone(model_name, show_bitmap=show_bitmap)
         arg1 = ["NAME:ComponentProps", "Name:=", model_name, "Id:=", str(id)]
         arg2 = ["NAME:Attributes", "Page:=", 1, "X:=", xpos, "Y:=", ypos, "Angle:=", angle, "Flip:=", False]
-        id = _retry_ntimes(10, self.oeditor.CreateComponent, arg1, arg2)
+        id = self.oeditor.CreateComponent(arg1, arg2)
         id = int(id.split(";")[1])
         self.add_id_to_component(id)
         return self.components[id]
 
     @pyaedt_function_handler()
     def create_component(
         self,
@@ -682,15 +703,15 @@
             Whether to enable the instance ID in the net list.
             The default is ``False``.
         global_netlist_list : list, optional
             The default is``[]``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -699,15 +720,15 @@
             name = self.design_libray + "\\" + component_library + ":" + component_name
         else:
             name = component_name
         arg1 = ["NAME:ComponentProps", "Name:=", name, "Id:=", str(id)]
         xpos, ypos = self._get_location(location)
 
         arg2 = ["NAME:Attributes", "Page:=", 1, "X:=", xpos, "Y:=", ypos, "Angle:=", angle, "Flip:=", False]
-        id = _retry_ntimes(10, self.oeditor.CreateComponent, arg1, arg2)
+        id = self.oeditor.CreateComponent(arg1, arg2)
         id = int(id.split(";")[1])
         # self.refresh_all_ids()
         self.add_id_to_component(id)
         if inst_name:
             self.components[id].set_property("InstanceName", inst_name)
         if use_instance_id_netlist:
             self.enable_use_instance_name(component_library, component_name)
@@ -781,17 +802,15 @@
         if len(properties) > 0:
             nexxim = list(properties[len(properties) - 1][1])
             for el in nexxim:
                 if el == "GRef:=":
                     nexxim_data = list(nexxim[nexxim.index(el) + 1])
                     nexxim_data[1] = "\n".join(global_netlist_list).replace("\\", "/")
                     nexxim[nexxim.index(el) + 1] = nexxim_data
-        _retry_ntimes(
-            10,
-            self.o_component_manager.Edit,
+        self.o_component_manager.Edit(
             name,
             ["Name:" + component_name, ["NAME:CosimDefinitions", nexxim, "DefaultCosim:=", "DefaultNetlist"]],
         )
         return True
 
     @pyaedt_function_handler()
     def create_symbol(self, symbol_name, pin_lists):
@@ -910,17 +929,15 @@
                     if "@InstanceName" not in netlist[:15]:
                         newnetlist = "@InstanceName" + netlist[4:]
                         nexxim_data[1] = newnetlist
                     nexxim[nexxim.index(el) + 1] = nexxim_data
                 elif el == "GRef:=":
                     nexxim_data = list(nexxim[nexxim.index(el) + 1])
                     nexxim[nexxim.index(el) + 1] = nexxim_data
-        _retry_ntimes(
-            10,
-            self.o_component_manager.Edit,
+        self.o_component_manager.Edit(
             name,
             ["Name:" + component_name, ["NAME:CosimDefinitions", nexxim, "DefaultCosim:=", "DefaultNetlist"]],
         )
         return True
 
     @pyaedt_function_handler()
     def refresh_all_ids(self):
@@ -962,15 +979,15 @@
 
         Returns
         -------
         int
             Number of components.
 
         """
-        obj = _retry_ntimes(10, self.oeditor.GetAllElements)
+        obj = self.oeditor.GetAllElements()
         for el in obj:
             name = el.split(";")
             if len(name) > 1 and str(id) == name[1]:
                 o = CircuitComponent(self, tabname=self.tab_name)
                 o.name = name[0]
                 if len(name) > 2:
                     o.id = int(name[1])
@@ -1019,20 +1036,20 @@
 
         References
         ----------
 
         >>> oEditor.GetComponentPins
         """
         if isinstance(partid, CircuitComponent):
-            pins = _retry_ntimes(10, self.oeditor.GetComponentPins, partid.composed_name)
+            pins = self.oeditor.GetComponentPins(partid.composed_name)
         elif isinstance(partid, str):
-            pins = _retry_ntimes(10, self.oeditor.GetComponentPins, partid)
+            pins = self.oeditor.GetComponentPins(partid)
             # pins = self.oeditor.GetComponentPins(partid)
         else:
-            pins = _retry_ntimes(10, self.oeditor.GetComponentPins, self.components[partid].composed_name)
+            pins = self.oeditor.GetComponentPins(self.components[partid].composed_name)
             # pins = self.oeditor.GetComponentPins(self.components[partid].composed_name)
         return list(pins)
 
     @pyaedt_function_handler()
     def get_pin_location(self, partid, pinname):
         """Retrieve the location of a pin.
 
@@ -1051,23 +1068,19 @@
         References
         ----------
 
         >>> oEditor.GetComponentPinLocation
 
         """
         if isinstance(partid, str):
-            x = _retry_ntimes(30, self.oeditor.GetComponentPinLocation, partid, pinname, True)
-            y = _retry_ntimes(30, self.oeditor.GetComponentPinLocation, partid, pinname, False)
+            x = self.oeditor.GetComponentPinLocation(partid, pinname, True)
+            y = self.oeditor.GetComponentPinLocation(partid, pinname, False)
         else:
-            x = _retry_ntimes(
-                30, self.oeditor.GetComponentPinLocation, self.components[partid].composed_name, pinname, True
-            )
-            y = _retry_ntimes(
-                30, self.oeditor.GetComponentPinLocation, self.components[partid].composed_name, pinname, False
-            )
+            x = self.oeditor.GetComponentPinLocation(self.components[partid].composed_name, pinname, True)
+            y = self.oeditor.GetComponentPinLocation(self.components[partid].composed_name, pinname, False)
         return self._convert_point_to_units([x, y])
 
     @pyaedt_function_handler()
     def arg_with_dim(self, Value, sUnits=None):
         """Format an argument with dimensions.
 
         .. deprecated:: 0.6.56
@@ -1119,15 +1132,15 @@
         color : string or 3 item list, optional
             Color or the line. The default is ``"0"``.
         line_width : float, optional
             Width of the line. The default is ``0``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.Line`
+        :class:`pyaedt.modeler.cad.object3dcircuit.Line`
             Line Object.
 
         >>> oEditor.CreateLine
         """
         points = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
         id = self.create_unique_id()
         return self.oeditor.CreateLine(
@@ -1145,28 +1158,28 @@
             A nested list of point coordinates. For example,
             ``[[x1, y1], [x2, y2], ...]``.
         wire_name : str, optional
             Name of the wire. Default value is ``""``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.Wire`
+        :class:`pyaedt.modeler.cad.object3dcircuit.Wire`
             Wire Object.
 
         References
         ----------
 
         >>> oEditor.CreateWire
         """
         points = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
         wire_id = self.create_unique_id()
         arg1 = ["NAME:WireData", "Name:=", wire_name, "Id:=", wire_id, "Points:=", points]
         arg2 = ["NAME:Attributes", "Page:=", 1]
         try:
-            wire_id = _retry_ntimes(10, self.oeditor.CreateWire, arg1, arg2)
+            wire_id = self.oeditor.CreateWire(arg1, arg2)
             w = Wire(self._modeler)
             for segment in self._app.oeditor.GetWireSegments(wire_id):
                 key = "SegmentID_{}".format(segment.split(" ")[3])
                 point1 = [float(x) for x in segment.split(" ")[1].split(",")]
                 point2 = [float(x) for x in segment.split(" ")[2].split(",")]
                 w.points_in_segment[key] = [point1, point2]
             if ":" in wire_id.split(";")[1]:
@@ -1214,15 +1227,15 @@
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to enable the instance ID in the net list.
             The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,14 +221,26 @@
         Dict : radio_name : EmitRadioComponents
             Dict of all the radio_name and EmitRadioComponents in the
             design.
         """
         return {k: v for k, v in self.components.items() if v.get_type() == "RadioNode"}
 
     @pyaedt_function_handler()
+    def get_antennas(self):
+        """Get all antennas in the design.
+
+        Returns
+        -------
+        Dict : antenna_name : EmitAntennaComponents
+            Dict of all the antenna_name and EmitAntennaComponents in the
+            design.
+        """
+        return {k: v for k, v in self.components.items() if v.get_type() == "AntennaNode"}
+
+    @pyaedt_function_handler()
     def refresh_all_ids(self):
         """Refresh all IDs and return the number of components."""
         all_comps = self.oeditor.GetAllComponents()
         for comp_name in all_comps:
             if not self.get_obj_id(comp_name):
                 o = EmitComponent.create(self, comp_name)
                 o_update = self.update_object_properties(o)
@@ -289,15 +301,15 @@
             cls.subclasses[root_node_type] = subclass
             return subclass
 
         return decorator
 
     @classmethod
     def create(cls, components, component_name):
-        """Create an Emit component.
+        """Create an EMIT component.
 
         Parameters
         ----------
         components : list
             List of components in the design.
         component_name : str
             Name of the component.
@@ -463,45 +475,14 @@
         if node is not None:
             node_name = root_node + "-*-" + "-*-".join(node.split("/")[1:])
         props_list = self.odesign.GetComponentNodeProperties(self.name, node_name)
         props = dict(p.split("=", 1) for p in props_list)
         return props
 
     @pyaedt_function_handler()
-    def set_property(self, property_name, property_value):
-        """Set part property
-
-        Parameters
-        ----------
-        property_name : str
-            property name
-        property_value : str
-            property value
-
-        Returns
-        -------
-        bool
-
-        References
-        ----------
-
-        >>> oEditor.ChangeProperty
-        """
-        if type(property_name) is list:
-            for p, v in zip(property_name, property_value):
-                v_prop = ["NAME:" + p, "Value:=", v]
-                self.change_property(v_prop)
-                self.__dict__[p] = v
-        else:
-            v_prop = ["NAME:" + property_name, "Value:=", property_value]
-            self.change_property(v_prop)
-            self.__dict__[property_name] = property_value
-        return True
-
-    @pyaedt_function_handler()
     def _add_property(self, property_name, property_value):
         """Add a property or update existing property value.
 
         Parameters
         ----------
         property_name : str
             Name of property.
@@ -659,15 +640,15 @@
 
         if position_string is None:
             return None
 
         # Build a tuple of the position
         parts = position_string.split()
 
-        # Check the units specified are a valid Emit length
+        # Check the units specified are a valid EMIT length
         if not units or units not in emit_consts.EMIT_VALID_UNITS["Length"]:
             units = self.units["Length"]
         position = (
             consts.unit_converter(float(parts[0]), "Length", "meter", units),
             consts.unit_converter(float(parts[1]), "Length", "meter", units),
             consts.unit_converter(float(parts[2]), "Length", "meter", units),
         )
@@ -743,14 +724,48 @@
         -------
         Float
             Start frequency of the band node."""
         if not units or units not in emit_consts.EMIT_VALID_UNITS["Frequency"]:
             units = self.units["Frequency"]
         return consts.unit_converter(float(band_node.props["StartFrequency"]), "Freq", "Hz", units)
 
+    def band_stop_frequency(self, band_node, units=""):
+        """Get the stop frequency of the band node.
+
+        Parameters
+        ----------
+        band_node : Instance of the band node.
+        units : str, optional
+            If ``None`` specified, global units are used.
+
+        Returns
+        -------
+        Float
+            Stop frequency of the band node."""
+        if not units or units not in emit_consts.EMIT_VALID_UNITS["Frequency"]:
+            units = self.units["Frequency"]
+        return consts.unit_converter(float(band_node.props["StopFrequency"]), "Freq", "Hz", units)
+
+    def band_channel_bandwidth(self, band_node, units=""):
+        """Get the channel bandwidth of the band node.
+
+        Parameters
+        ----------
+        band_node : Instance of the band node.
+        units : str, optional
+            If ``None`` specified, global units are used.
+
+        Returns
+        -------
+        Float
+            Channel bandwidth of the band node."""
+        if not units or units not in emit_consts.EMIT_VALID_UNITS["Frequency"]:
+            units = self.units["Frequency"]
+        return consts.unit_converter(float(band_node.props["ChannelBandwidth"]), "Freq", "Hz", units)
+
     def band_tx_power(self, band_node, units=""):
         """Get the transmit power of the band node.
 
         Parameters
         ----------
         band_node : Instance of the band node.
         units : str
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Parameters
         ----------
         partname : int or str
             ID or name of the object.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         """
         if isinstance(partname, int):
             return self.components[partname]
         for el in self.components:
             if self.components[el].name == partname or self.components[el].composed_name == partname or el == partname:
@@ -71,15 +71,15 @@
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list or not. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -114,15 +114,15 @@
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list or not. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -156,15 +156,15 @@
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list or not. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -193,15 +193,15 @@
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -231,15 +231,15 @@
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Parameters
         ----------
         partname : int or str
             ID or name of the object.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         """
         if isinstance(partname, int):
             return self.components[partname]
         for el in self.components:
             if self.components[el].name == partname or self.components[el].composed_name == partname or el == partname:
@@ -95,15 +95,15 @@
         angle : float, optional
             Angle rotation in degrees. The default value is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default value is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -138,15 +138,15 @@
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -180,15 +180,15 @@
         angle : float, optional
             Angle rotation in degrees. The default value is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default value is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -229,15 +229,15 @@
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list or not. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -278,15 +278,15 @@
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -316,15 +316,15 @@
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -354,15 +354,15 @@
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
@@ -418,15 +418,15 @@
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list or not. The default is ``False``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
+        :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.85/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 
 from collections import OrderedDict
 import math
 
 # from pyaedt import property
-from pyaedt import _retry_ntimes
 from pyaedt import pyaedt_function_handler
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _arg2dict
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.cad.elements3d import _dict2arg
@@ -35,41 +34,35 @@
 
         References
         ----------
 
         >>> oPadstackManager.GetComponentPinLocation
         """
         if "Port" in self._circuit_comp.composed_name:
-            pos1 = _retry_ntimes(
-                30,
-                self._oeditor.GetPropertyValue,
+            pos1 = self._oeditor.GetPropertyValue(
                 "BaseElementTab",
                 self._circuit_comp.composed_name,
                 "Component Location",
             )
             if isinstance(pos1, str):
                 pos1 = pos1.split(", ")
                 pos1 = [float(i.strip()[:-3]) * 0.0000254 for i in pos1]
                 if "GPort" in self._circuit_comp.composed_name:
                     pos1[1] += 0.00254
                 pos1 = [round(i / AEDT_UNITS["Length"][self.units], 8) for i in pos1]
                 return pos1
             return []
         return [
             round(
-                _retry_ntimes(
-                    30, self._oeditor.GetComponentPinLocation, self._circuit_comp.composed_name, self.name, True
-                )
+                self._oeditor.GetComponentPinLocation(self._circuit_comp.composed_name, self.name, True)
                 / AEDT_UNITS["Length"][self.units],
                 8,
             ),
             round(
-                _retry_ntimes(
-                    30, self._oeditor.GetComponentPinLocation, self._circuit_comp.composed_name, self.name, False
-                )
+                self._oeditor.GetComponentPinLocation(self._circuit_comp.composed_name, self.name, False)
                 / AEDT_UNITS["Length"][self.units],
                 8,
             ),
         ]
 
     @property
     def net(self):
@@ -468,15 +461,15 @@
             tab = "Quantities"
         try:
             proparray = self._oeditor.GetProperties(tab, self.composed_name)
         except:
             proparray = []
 
         for j in proparray:
-            propval = _retry_ntimes(10, self._oeditor.GetPropertyValue, tab, self.composed_name, j)
+            propval = self._oeditor.GetPropertyValue(tab, self.composed_name, j)
             _parameters[j] = propval
         self._parameters = ComponentParameters(self, tab, _parameters)
         return self._parameters
 
     @property
     def component_info(self):
         """Component parameters.
@@ -490,15 +483,15 @@
         if self._component_info or self._circuit_components._app.design_type != "Circuit Design":
             return self._component_info
         _component_info = {}
         tab = "Component"
         proparray = self._oeditor.GetProperties(tab, self.composed_name)
 
         for j in proparray:
-            propval = _retry_ntimes(10, self._oeditor.GetPropertyValue, tab, self.composed_name, j)
+            propval = self._oeditor.GetPropertyValue(tab, self.composed_name, j)
             _component_info[j] = propval
         self._component_info = ComponentParameters(self, tab, _component_info)
         return self._component_info
 
     @property
     def bounding_box(self):
         """Component bounding box."""
@@ -536,15 +529,15 @@
 
         """
         if self._pins:
             return self._pins
         self._pins = []
 
         try:
-            pins = _retry_ntimes(10, self._oeditor.GetComponentPins, self.composed_name)
+            pins = list(self._oeditor.GetComponentPins(self.composed_name))
             if "Port@" in self.composed_name and pins == []:
                 self._pins.append(CircuitPins(self, self.composed_name))
                 return self._pins
             elif not pins:
                 return []
             for pin in pins:
                 if self._circuit_components._app.design_type != "Twin Builder":
@@ -563,17 +556,15 @@
         ----------
 
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
         """
         self._location = []
         try:
-            loc = _retry_ntimes(
-                10, self._oeditor.GetPropertyValue, "BaseElementTab", self.composed_name, "Component Location"
-            )
+            loc = self._oeditor.GetPropertyValue("BaseElementTab", self.composed_name, "Component Location")
             loc = [loc.split(",")[0].strip(), loc.split(",")[1].strip()]
             loc = [decompose_variable_value(i) for i in loc]
 
             self._location = [
                 round(i[0] * AEDT_UNITS["Length"][i[1]] / AEDT_UNITS["Length"][self.units], 10) for i in loc
             ]
         except:
@@ -642,18 +633,15 @@
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
         """
         if self._mirror is not None:
             return self._mirror
         try:
             self._mirror = (
-                _retry_ntimes(
-                    10, self._oeditor.GetPropertyValue, "BaseElementTab", self.composed_name, "Component Mirror"
-                )
-                == "true"
+                self._oeditor.GetPropertyValue("BaseElementTab", self.composed_name, "Component Mirror") == "true"
             )
         except:
             self._mirror = False
         return self._mirror
 
     @mirror.setter
     def mirror(self, mirror_value=True):
@@ -753,14 +741,18 @@
                 else:
                     self.__dict__[p] = v
         else:
             v_prop = ["NAME:" + property_name, "Value:=", property_value]
             self.change_property(v_prop)
             if self.__dict__.get("_parameters", None) and property_name in self.__dict__["_parameters"]:
                 self.__dict__["_parameters"][property_name] = property_value
+            elif self.__dict__.get("_component_info", None) and property_name in self.__dict__.get(
+                "_component_info", None
+            ):
+                self.__dict__["_component_info"][property_name] = property_value
             else:
                 self.__dict__[property_name] = property_value
         return True
 
     @pyaedt_function_handler()
     def _add_property(self, property_name, property_value):
         """Add a property.
@@ -807,28 +799,26 @@
         if names_list:
             vPropServers = ["NAME:PropServers"]
             for el in names_list:
                 vPropServers.append(el)
         else:
             vPropServers = ["NAME:PropServers", self.composed_name]
         tabname = None
-        if vPropChange[0][5:] in _retry_ntimes(10, self._oeditor.GetProperties, self.tabname, self.composed_name):
+        if vPropChange[0][5:] in self._oeditor.GetProperties(self.tabname, self.composed_name):
             tabname = self.tabname
-        elif vPropChange[0][5:] in _retry_ntimes(
-            10, self._oeditor.GetProperties, "PassedParameterTab", self.composed_name
-        ):
+        elif vPropChange[0][5:] in self._oeditor.GetProperties("PassedParameterTab", self.composed_name):
             tabname = "PassedParameterTab"
-        elif vPropChange[0][5:] in _retry_ntimes(10, self._oeditor.GetProperties, "BaseElementTab", self.composed_name):
+        elif vPropChange[0][5:] in self._oeditor.GetProperties("BaseElementTab", self.composed_name):
             tabname = "BaseElementTab"
         if tabname:
             vGeo3dlayout = ["NAME:" + tabname, vPropServers, vChangedProps]
             vOut = ["NAME:AllTabs", vGeo3dlayout]
             if "NAME:Component Location" in str(vChangedProps) and "PagePort" not in self.composed_name:
-                _retry_ntimes(10, self._oeditor.ChangeProperty, vOut)
-            return _retry_ntimes(10, self._oeditor.ChangeProperty, vOut)
+                self._oeditor.ChangeProperty(vOut)
+            return self._oeditor.ChangeProperty(vOut)
         return False
 
 
 class Wire(object):
     """Creates and manipulates a wire."""
 
     def __init__(self, modeler):
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.85/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.85/pyaedt/modeler/modeler2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         check_lines : bool, optional
             Whether to check line objects. The default is ``True``.
         check_sheets : bool, optional
             Whether to check sheet objects. The default is ``True``.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d`
+        list of :class:`pyaedt.modeler.cad.object3d`
         """
         if len(bounding_box) != 4 and len(bounding_box) != 6:
             raise ValueError("Bounding box must be a list of 4 or 6 elements.")
 
         if len(bounding_box) == 4:
             if self._app.design_type == "2D Extractor" or self._app.xy_plane:
                 bounding_box = [bounding_box[0], bounding_box[1], 0, bounding_box[2], bounding_box[3], 0]
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.85/pyaedt/modeler/modeler3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import datetime
 import json
 import os.path
 import warnings
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
+from pyaedt.generic.general_methods import GrpcApiError
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import GeometryModeler
 from pyaedt.modeler.cad.Primitives3D import Primitives3D
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
@@ -360,15 +360,16 @@
                                 cs_set.add(cs)
                 out_dict["coordinatesystems"] = copy.deepcopy(config_dict["coordinatesystems"])
                 for cs in list(out_dict["coordinatesystems"]):
                     if cs not in cs_set:
                         del out_dict["coordinatesystems"][cs]
             with open(auxiliary_dict, "w") as outfile:
                 json.dump(out_dict, outfile)
-        return _retry_ntimes(10, self.oeditor.Create3DComponent, arg, arg2, component_file, arg3)
+        self.oeditor.Create3DComponent(arg, arg2, component_file, arg3)
+        return True
 
     @pyaedt_function_handler()
     def replace_3dcomponent(
         self,
         component_name=None,
         variables_to_include=None,
         object_list=None,
@@ -529,15 +530,15 @@
                 if all(included_obj in objs for included_obj in mesh_comp):
                     used_mesh_ops.append(self._app.mesh.meshoperations[mesh].name)
             arg2.append("MeshOperations:="), arg2.append(used_mesh_ops)
         else:
             arg2.append("MeshOperations:="), arg2.append(meshops)
         arg3 = ["NAME:ImageFile", "ImageFile:=", ""]
         old_components = self.user_defined_component_names
-        _retry_ntimes(10, self.oeditor.ReplaceWith3DComponent, arg, arg2, arg3)
+        self.oeditor.ReplaceWith3DComponent(arg, arg2, arg3)
         self.refresh_all_ids()
         new_name = list(set(self.user_defined_component_names) - set(old_components))
         return self.user_defined_components[new_name[0]]
 
     @pyaedt_function_handler()
     def create_coaxial(
         self,
@@ -809,15 +810,15 @@
         check_lines : bool, optional
             Check line objects.
         check_sheets : bool, optional
             Check sheet objects.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.object3d`
+        list of :class:`pyaedt.modeler.cad.object3d`
         """
         if len(bounding_box) != 6:
             raise ValueError("Bounding box list must have dimension 6.")
 
         objects = []
         if check_solids:
             for obj in self.solid_objects:
@@ -1330,18 +1331,19 @@
 
         objects_list = self.convert_to_selections(objects_list, True)
 
         segment_sheets = {}
         segment_objects = {}
         for obj_name in objects_list:
             obj = self[obj_name]
+            obj_axial_length = GeometryOperators.points_distance(obj.top_face_z.center, obj.bottom_face_z.center)
             if segments_number:
-                segmentation_thickness = obj.top_edge_y.length / segments_number
+                segmentation_thickness = obj_axial_length / segments_number
             elif segmentation_thickness:
-                segments_number = round(obj.top_edge_y.length / segmentation_thickness)
+                segments_number = round(obj_axial_length / segmentation_thickness)
             face_object = self.modeler.create_object_from_face(obj.bottom_face_z)
             # segment sheets
             segment_sheets[obj.name] = face_object.duplicate_along_line(
                 ["0", "0", segmentation_thickness], segments_number
             )
             segment_objects[obj.name] = []
             for value in segment_sheets[obj.name]:
@@ -1353,11 +1355,133 @@
                 self.move(face_object, [0, 0, segmentation_thickness / 4])
                 mesh_sheets[obj.name] = face_object.duplicate_along_line(
                     [0, 0, (segmentation_thickness * 2.0) / 4.0], segments_number * 2
                 )
                 mesh_objects[obj.name] = []
                 for value in mesh_sheets[obj.name]:
                     mesh_objects[obj.name].append([x for x in self.sheet_objects if x.name == value][0])
+        face_object.delete()
         if apply_mesh_sheets:
             return segment_objects, mesh_objects
         else:
             return segment_objects
+
+    @pyaedt_function_handler
+    def change_region_padding(self, padding_data, padding_type, direction=None, region_name="Region"):
+        """
+        Change region padding settings.
+
+        Parameters
+        ----------
+        padding_data : str or list of str
+            Padding value (with unit if necessary). A list of padding values must have corresponding
+            elements in ``padding_type`` and ``direction`` arguments.
+        padding_type : str or list of str
+            Padding type. Available options are ``"Percentage Offset"``, ``"Transverse Percentage Offset"``,
+            ``"Absolute Offset"``, ``"Absolute Position"``.
+        direction : str or list of str, optional
+            Direction to which apply the padding settings. A direction can be ``"+X"``, ``"-X"``,
+            `"+Y"``, ``"-Y"``, ``"+Z"`` or ``"-Z"``. Default is ``None``, in which case all the
+            directions are used (in the order written in the previous sentence).
+        region_name : str optional
+            Region name. Default is ``Region``.
+
+        Returns
+        -------
+        bool
+            ``True`` if successful, else ``None``.
+
+        Examples
+        ----------
+        >>> import pyaedt
+        >>> app = pyaedt.Icepak()
+        >>> app.modeler.change_region_padding("10mm", padding_type="Absolute Offset", direction="-X")
+        """
+        available_directions = ["+X", "-X", "+Y", "-Y", "+Z", "-Z"]
+        available_paddings = [
+            "Percentage Offset",
+            "Transverse Percentage Offset",
+            "Absolute Offset",
+            "Absolute Position",
+        ]
+        if not isinstance(padding_data, list):
+            padding_data = [padding_data]
+        if not isinstance(padding_type, list):
+            padding_type = [padding_type]
+        if direction is None:
+            direction = available_directions
+        else:
+            if not isinstance(direction, list):
+                direction = [direction]
+            if not all(dire in available_directions for dire in direction):
+                raise Exception("Check ``axes`` input.")
+        if not all(pad in available_paddings for pad in padding_type):
+            raise Exception("Check ``padding_type`` input.")
+
+        modify_props = []
+        for i in range(len(padding_data)):
+            modify_props.append(["NAME:" + direction[i] + " Padding Type", "Value:=", padding_type[i]])
+            modify_props.append(["NAME:" + direction[i] + " Padding Data", "Value:=", padding_data[i]])
+
+        try:
+            create_region_name = self.modeler.oeditor.GetChildObject(region_name).GetChildNames()[0]
+            self.modeler.oeditor.ChangeProperty(
+                list(
+                    [
+                        "NAME:AllTabs",
+                        list(
+                            [
+                                "NAME:Geometry3DCmdTab",
+                                list(["NAME:PropServers", region_name + ":" + create_region_name]),
+                                list(["NAME:ChangedProps"] + modify_props),
+                            ]
+                        ),
+                    ]
+                )
+            )
+            return True
+        except (GrpcApiError, SystemExit):
+            return False
+
+    @pyaedt_function_handler
+    def change_region_coordinate_system(self, region_cs="Global", region_name="Region"):
+        """
+        Change region coordinate system.
+
+        Parameters
+        ----------
+        region_cs : str, optional
+            Region coordinate system. Default is ``Global``.
+        region_name : str optional
+            Region name. Default is ``Region``.
+
+        Returns
+        -------
+        bool
+            ``True`` if successful, else ``None``.
+
+        Examples
+        ----------
+        >>> import pyaedt
+        >>> app = pyaedt.Icepak()
+        >>> app.modeler.create_coordinate_system(origin=[1, 1, 1], name="NewCS")
+        >>> app.modeler.change_region_coordinate_system(region_cs="NewCS")
+        """
+        try:
+            create_region_name = self.modeler.oeditor.GetChildObject(region_name).GetChildNames()[0]
+            self.modeler.oeditor.ChangeProperty(
+                list(
+                    [
+                        "NAME:AllTabs",
+                        list(
+                            [
+                                "NAME:Geometry3DCmdTab",
+                                list(["NAME:PropServers", region_name + ":" + create_region_name]),
+                                list(["NAME:ChangedProps", list(["NAME:Coordinate System", "Value:=", region_cs])]),
+                            ]
+                        ),
+                    ]
+                )
+            )
+            return True
+        except (GrpcApiError, SystemExit):
+            return False
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.85/pyaedt/modeler/modelerpcb.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from warnings import warn
 
 from pyaedt import settings
 from pyaedt.edb import Edb
 from pyaedt.generic.constants import AEDT_UNITS
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import get_filename_without_extension
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.pcb.Primitives3DLayout import Primitives3DLayout
@@ -156,15 +155,15 @@
 
         References
         ----------
 
         >>> oEditor.GetActiveUnits
         >>> oEditor.SetActivelUnits
         """
-        return _retry_ntimes(10, self.oeditor.GetActiveUnits)
+        return self.oeditor.GetActiveUnits()
 
     @model_units.setter
     def model_units(self, units):
         assert units in AEDT_UNITS["Length"], "Invalid units string {0}.".format(units)
         """Set the model units as a string (for example, "mm")."""
         self.oeditor.SetActiveUnits(["NAME:Units Parameter", "Units:=", units, "Rescale:=", False])
 
@@ -328,15 +327,15 @@
         """
         des_name = merged_design.design_name
         merged_design.oproject.CopyDesign(des_name)
         self._app.odesign.PasteDesign(1)
         comp_name = ""
         for i in range(100, 0, -1):
             try:
-                cmp_info = _retry_ntimes(10, self.oeditor.GetComponentInfo, str(i))
+                cmp_info = self.oeditor.GetComponentInfo(str(i))
                 if cmp_info and des_name in cmp_info[0]:
                     comp_name = str(i)
                     break
             except:
                 continue
         if not comp_name:
             return False
@@ -463,15 +462,15 @@
         >>> out1 = h3d.modeler.expand("line_3")
         >>> print(out1)
         line_4
 
         """
         object_to_expand = self.convert_to_selections(object_to_expand)
         self.cleanup_objects()
-        layer = _retry_ntimes(10, self.oeditor.GetPropertyValue, "BaseElementTab", object_to_expand, "PlacementLayer")
+        layer = self.oeditor.GetPropertyValue("BaseElementTab", object_to_expand, "PlacementLayer")
         poly = self.oeditor.GetPolygonDef(object_to_expand).GetPoints()
         pos = [poly[0].GetX(), poly[0].GetY()]
         geom_names = self.oeditor.FindObjectsByPoint(self.oeditor.Point().Set(pos[0], pos[1]), layer)
         self.oeditor.Expand(
             self.number_with_units(size), expand_type, replace_original, ["NAME:elements", object_to_expand]
         )
         self.cleanup_objects()
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.85/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import sys
 import warnings
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Primitives import default_materials
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modeler.pcb.object3dlayout import Circle3dLayout
 from pyaedt.modeler.pcb.object3dlayout import Components3DLayout
@@ -107,15 +106,15 @@
 
     @property
     def components(self):
         """Components.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Components3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Components3DLayout`]
             Components objects.
 
         """
         if self._components:
             return self._components
         objs = self.modeler.oeditor.FindObjects("Type", "component")
         for obj in objs:
@@ -394,30 +393,30 @@
 
     @property
     def polygons(self):
         """Polygons.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Polygons3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Polygons3DLayout`]
             Pyaedt Objects.
         """
         if self._polygons:
             return self._polygons
         for obj in self.polygon_names:
             self._polygons[obj] = Polygons3DLayout(self, obj, "poly", False)
         return self._polygons
 
     @property
     def lines(self):
         """Lines.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Line3dLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Line3dLayout`]
             Pyaedt Objects.
         """
 
         if self._lines:
             return self._lines
 
         for obj in self.line_names:
@@ -426,60 +425,60 @@
 
     @property
     def circles(self):
         """Circles.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Circle3dLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Circle3dLayout`]
             Pyaedt Objects.
         """
         if self._circles:
             return self._circles
         for obj in self.circle_names:
             self._circles[obj] = Circle3dLayout(self, obj, False)
         return self._circles
 
     @property
     def rectangles(self):
         """Rectangles.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Rect3dLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Rect3dLayout`]
             Pyaedt Objects.
         """
         if self._rectangles:
             return self._rectangles
         for obj in self.rectangle_names:
             self._rectangles[obj] = Rect3dLayout(self, obj, False)
         return self._rectangles
 
     @property
     def polygons_voids(self):
         """Void Polygons.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Polygons3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Polygons3DLayout`]
             Pyaedt Objects.
         """
         if self._polygons_voids:
             return self._polygons_voids
         for obj in self.polygon_voids_names:
             self._polygons_voids[obj] = Polygons3DLayout(self, obj, "poly", True)
         return self._polygons_voids
 
     @property
     def lines_voids(self):
         """Void Lines.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Line3dLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Line3dLayout`]
             Pyaedt Objects.
         """
 
         if self._lines:
             return self._lines
         for obj in self.line_voids_names:
             self._lines[obj] = Line3dLayout(self, obj, True)
@@ -487,45 +486,45 @@
 
     @property
     def circles_voids(self):
         """Void Circles.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Circle3dLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Circle3dLayout`]
             Pyaedt Objects.
         """
         if self._circles:
             return self._circles
         for obj in self.circle_voids_names:
             self._circles[obj] = Circle3dLayout(self, obj, True)
         return self._circles
 
     @property
     def rectangles_voids(self):
         """Void Rectangles.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Rect3dLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Rect3dLayout`]
             Pyaedt Objects.
         """
         if self._rectangles:
             return self._rectangles
         for obj in self.rectangle_void_names:
             self._rectangles[obj] = Rect3dLayout(self, obj, True)
         return self._rectangles
 
     @property
     def components_3d(self):
         """Components.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Components3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Components3DLayout`]
             Pyaedt Objects.
         """
         if not self._components3d:
             for i in range(1, 1000):
                 cmp_info = self.oeditor.GetComponentInfo(str(i))
                 if cmp_info and "ComponentName" in cmp_info[0]:
                     self._components3d[str(i)] = Components3DLayout(self, str(i))
@@ -558,45 +557,45 @@
 
     @property
     def pins(self):
         """Pins.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Pins3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Pins3DLayout`]
             Pins Dictionary.
 
         """
         if self._pins or len(self._get_names(["pin"])) == len(self._pins):
             return self._pins
         self._cleanup_vias(True)
         return self._pins
 
     @property
     def vias(self):
         """Vias.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Pins3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Pins3DLayout`]
             Vias Dictionary.
         """
         if self._vias or len(self._get_names(["via"])) == len(self._vias):
             return self._vias
         self._cleanup_vias(False)
 
         return self._vias
 
     @property
     def nets(self):
         """Nets.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Nets3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Nets3DLayout`]
             Nets Dictionary.
 
         """
         n = {}
         for k, v in self.power_nets.items():
             n[k] = v
         for k, v in self.signal_nets.items():
@@ -607,15 +606,15 @@
 
     @property
     def power_nets(self):
         """Nets.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Nets3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Nets3DLayout`]
             Power Nets Dictionary.
 
         """
         if self._power_nets:
             return self._power_nets
 
         objs = self.modeler.oeditor.GetNetClassNets("<Power/Ground>")
@@ -625,15 +624,15 @@
 
     @property
     def signal_nets(self):
         """Nets.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Nets3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Nets3DLayout`]
             Signal Nets Dictionary.
 
         """
         if self._signal_nets:
             return self._signal_nets
 
         objs = self.modeler.oeditor.GetNetClassNets("Non Power/Ground")
@@ -643,15 +642,15 @@
 
     @property
     def no_nets(self):
         """Nets without class type.
 
         Returns
         -------
-        dict[str, :class:`pyaedt.modeler.object3dlayout.Nets3DLayout`]
+        dict[str, :class:`pyaedt.modeler.cad.object3dlayout.Nets3DLayout`]
             No Nets Dictionary.
 
         """
         if self._no_nets:
             return self._no_nets
 
         objs = self.modeler.oeditor.GetNetClassNets("<All>")
@@ -711,15 +710,15 @@
         Parameters
         ----------
         name : str, optional
             Name of the padstack. The default is ``"Padstack"``.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Padstack`
+        :class:`pyaedt.modeler.cad.object3dlayout.Padstack`
             Padstack object if a padstack with this name does not already exist.
 
         """
         if name in self.padstacks:
             return None
         else:
             self.padstacks[name] = Padstack(name, self.opadstackmanager, self.model_units)
@@ -905,15 +904,15 @@
             Name of the via. If ``None`` a random name is generated.
         netname : str, optional
             Name of the net. The default is ``None``, in which case no
             name is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Pins3DLayout` or bool
+        :class:`pyaedt.modeler.cad.object3dlayout.Pins3DLayout` or bool
             Object via created when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CreateVia
         """
@@ -943,15 +942,15 @@
                 arg.append("overrides hole:="), arg.append(False)
                 arg.append("hole diameter:="), arg.append([self.number_with_units(1)])
 
             arg.append("Pin:="), arg.append(False)
             arg.append("highest_layer:="), arg.append(top_layer)
             arg.append("lowest_layer:="), arg.append(bot_layer)
 
-            _retry_ntimes(10, self.oeditor.CreateVia, arg)
+            self.oeditor.CreateVia(arg)
             if netname:
                 self.oeditor.ChangeProperty(
                     [
                         "NAME:AllTabs",
                         [
                             "NAME:BaseElementTab",
                             ["NAME:PropServers", name],
@@ -984,15 +983,15 @@
             default name is assigned.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Circle3dLayout`
+        :class:`pyaedt.modeler.cad.object3dlayout.Circle3dLayout`
             Objects of the circle created when successful.
 
         References
         ----------
 
         >>> oEditor.CreateCircle
         """
@@ -1049,15 +1048,15 @@
             default name is assigned.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Rect3dLayout`
+        :class:`pyaedt.modeler.cad.object3dlayout.Rect3dLayout`
             Name of the rectangle created when successful.
 
         References
         ----------
 
         >>> oEditor.CreateRectangle
         """
@@ -1117,15 +1116,15 @@
             default name is assigned.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Polygons3DLayout`
+        :class:`pyaedt.modeler.cad.object3dlayout.Polygons3DLayout`
             Object of the rectangle created when successful.
 
         References
         ----------
 
         >>> oEditor.CreatePolygon
         """
@@ -1172,15 +1171,15 @@
             Polygon units. Default is modeler units.
         name : str, optional
             Name of the rectangle. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Polygons3DLayout`
+        :class:`pyaedt.modeler.cad.object3dlayout.Polygons3DLayout`
             Object of the rectangle created when successful.
 
         References
         ----------
 
         >>> oEditor.CreatePolygon
         """
@@ -1242,15 +1241,15 @@
             default name is assigned.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Line3dLayout`
+        :class:`pyaedt.modeler.cad.object3dlayout.Line3dLayout`
             Object of the line created when successful.
 
         References
         ----------
 
         >>> oEditor.CreateLine
         """
@@ -1444,15 +1443,15 @@
         args.append("ModSinceLib:=")
         args.append(True)
         args.append("CompExtID:=")
         args.append(8)
         args.append("3DCompSourceFileName:=")
         args.append(component_path)
 
-        _retry_ntimes(10, self.modeler.o_component_manager.Add, args)
+        self.modeler.o_component_manager.Add(args)
         stack_layers = ["0:{}".format(i.name) for i in self.modeler.layers.stackup_layers]
         drawing = ["{}:{}".format(i.name, i.name) for i in self.modeler.layers.drawing_layers]
         arg_x = self.modeler._arg_with_dim(pos_x)
         arg_y = self.modeler._arg_with_dim(pos_y)
         args = [
             "NAME:Contents",
             "definition_name:=",
@@ -1468,15 +1467,15 @@
             "rect_width:=",
             0.01,
             "StackupLayers:=",
             stack_layers,
             "DrawLayers:=",
             drawing,
         ]
-        comp_name = _retry_ntimes(10, self.modeler.oeditor.CreateComponent, args)
+        comp_name = self.modeler.oeditor.CreateComponent(args)
         comp = ComponentsSubCircuit3DLayout(self, comp_name.split(";")[-1])
         self.components_3d[comp_name.split(";")[-1]] = comp
         if create_ports:
             self.oeditor.CreatePortsOnComponentsByNet(["NAME:Components", comp.name], [], "Port", "0", "0", "0")
         return comp  #
 
     def create_text(self, text, position, angle=0, font_size=12):
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.85/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 """
 from __future__ import absolute_import  # noreorder
 
 import math
 import re
 
 # from pyaedt import property
-from pyaedt import _retry_ntimes
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Objec3DLayout(object):
@@ -111,15 +110,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if self.prim_type in ["component", "pin", "via"]:
-            return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Angle")
+            return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Angle")
 
     @angle.setter
     def angle(self, value):
         if self.prim_type in ["component", "pin", "via"]:
             vMaterial = ["NAME:Angle", "Value:=", value]
             self.change_property(vMaterial)
 
@@ -168,15 +167,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if self.prim_type not in ["component"]:
-            return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Net")
+            return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Net")
 
     @net_name.setter
     def net_name(self, netname=""):
         if self.prim_type not in ["component"]:
             vMaterial = ["NAME:Net", "Value:=", netname]
             self.change_property(vMaterial)
 
@@ -191,15 +190,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if self.prim_type not in ["pin", "via"]:
-            return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "PlacementLayer")
+            return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "PlacementLayer")
 
     @placement_layer.setter
     def placement_layer(self, layer_name):
         if self.prim_type not in ["pin", "via"]:
             vMaterial = ["NAME:PlacementLayer", "Value:=", layer_name]
             self.change_property(vMaterial)
 
@@ -302,17 +301,15 @@
                     bbury = float(i.split("=")[1])
             loc_x = (bburx + bbllx) / 2
             loc_y = (bbury + bblly) / 2
             loc_x = round(unit_converter(loc_x, output_units=self._primitives.model_units), 9)
             loc_y = round(unit_converter(loc_y, output_units=self._primitives.model_units), 9)
             return [loc_x, loc_y]
         elif self.prim_type in ["pin", "via"]:
-            location = _retry_ntimes(
-                self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Location"
-            ).split(",")
+            location = self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Location").split(",")
             locs = []
             for i in location:
                 try:
                     locs.append(float(i))
                 except ValueError:  # pragma: no cover
                     locs.append(i)
             return locs
@@ -374,16 +371,15 @@
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
         return (
             True
-            if _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "LockPosition")
-            in [True, "true"]
+            if self._oeditor.GetPropertyValue("BaseElementTab", self.name, "LockPosition") in [True, "true"]
             else False
         )
 
     @lock_position.setter
     def lock_position(self, lock_position=True):
         vMaterial = ["NAME:LockPosition", "Value:=", lock_position]
         self.change_property(vMaterial)
@@ -392,15 +388,15 @@
 class ModelInfoRlc(object):
     def __init__(self, component, name):
         self._comp = component
         self._name = name
 
     @property
     def rlc_model_type(self):
-        props = _retry_ntimes(self._comp._n, self._comp._oeditor.GetComponentInfo, self._name)
+        props = self._comp._oeditor.GetComponentInfo(self._name)
         model = ""
         for p in props:
             if "ComponentProp=" in p:
                 model = p
                 break
         s = r".+rlc\(r='(.+?)', re=(.+?), l='(.+?)', le=(.+?), c='(.+?)', ce=(.+?), p=(.+?), lyr=(.+?)"
         m = re.search(s, model)
@@ -454,15 +450,15 @@
             Component part.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Part")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Part")
 
     @property
     def part_type(self):
         """Retrieve the component part type.
 
         Returns
         -------
@@ -470,15 +466,15 @@
             Component part type.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Part Type")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Part Type")
 
     @property
     def _part_type_id(self):
         parts = {"Other": 0, "Resistor": 1, "Inductor": 2, "Capacitor": 3, "IC": 4, "IO": 5}
         if self.part_type in parts:
             return parts[self.part_type]
         return -1
@@ -661,15 +657,15 @@
         """
         if self._part_type_id not in [0, 4, 5]:
             return False
         if self._part_type_id == 4:
             prop_name = "ICProp:="
             if not self.die_enabled:
                 self.set_die_type()
-            props = _retry_ntimes(10, self._oeditor.GetComponentInfo, self.name)
+            props = self._oeditor.GetComponentInfo(self.name)
             model = ""
             for p in props:
                 if "PortProp(" in p:
                     model = p
                     break
             s = r".+PortProp\(rh='(.+?)', rsa=(.+?), rsx='(.+?)', rsy='(.+?)'\)"
             m = re.search(s, model)
@@ -761,15 +757,15 @@
 
     @property
     def model(self):
         """RLC model if available.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.ModelInfoRlc`
+        :class:`pyaedt.modeler.cad.object3dlayout.ModelInfoRlc`
         """
         if self._part_type_id in [1, 2, 3]:
             return ModelInfoRlc(self, self.name)
 
 
 class Nets3DLayout(object):
     """Contains Nets in HFSS 3D Layout."""
@@ -782,15 +778,15 @@
 
     @property
     def components(self):
         """Components that belongs to the Nets.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3dlayout.Components3DLayout`
+        :class:`pyaedt.modeler.cad.object3dlayout.Components3DLayout`
         """
         comps = {}
         for c in self._oeditor.FilterObjectList("Type", "component", self._oeditor.FindObjects("Net", self.name)):
             comps[c] = self._primitives.components[c]
         return comps
 
 
@@ -813,15 +809,15 @@
             Name of the starting layer of the pin.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Start Layer")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Start Layer")
 
     @property
     def stop_layer(self):
         """Retrieve the starting layer of the pin.
 
         Returns
         -------
@@ -829,15 +825,15 @@
             Name of the stopping layer of the pin.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Stop Layer")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Stop Layer")
 
     @property
     def holediam(self):
         """Retrieve the hole diameter of the pin.
 
         Returns
         -------
@@ -845,15 +841,15 @@
            Hole diameter of the pin.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "HoleDiameter")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "HoleDiameter")
 
 
 class Geometries3DLayout(Objec3DLayout, object):
     """Contains geometries in HFSS 3D Layout."""
 
     def __init__(self, primitives, name, prim_type="poly", is_void=False):
         Objec3DLayout.__init__(self, primitives, prim_type)
@@ -888,15 +884,15 @@
 
     @property
     def points(self):
         """Provide the polygon points. For Lines it returns the center line.
 
         Returns
         -------
-        List of :class:`pyaedt.modeler.object3dlayout.Points3dLayout`
+        List of :class:`pyaedt.modeler.cad.object3dlayout.Points3dLayout`
         """
         if self._points:
             return self._points
         self._points = []
         obj = self._oeditor.GetPolygon(self.name)
         for oo in obj.GetPoints():
             self._points.append(Points3dLayout(self._primitives, oo))
@@ -1031,15 +1027,15 @@
             Value of the property.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, propertyname)
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, propertyname)
 
     @property
     def negative(self):
         """Get/Set the negative.
 
         Parameters
         ----------
@@ -1054,18 +1050,15 @@
         ----------
 
         >>> oEditor.ChangeProperty
         """
         if self.is_void:
             return False
         return (
-            True
-            if _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Negative")
-            in [True, "true"]
-            else False
+            True if self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Negative") in [True, "true"] else False
         )
 
     @negative.setter
     def negative(self, negative=False):
         if not self.is_void:
             vMaterial = ["NAME:Negative", "Value:=", negative]
             self.change_property(vMaterial)
@@ -1083,15 +1076,15 @@
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if self.is_void:
             return None
         if self.prim_type not in ["component"]:
-            return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Net")
+            return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Net")
 
     @net_name.setter
     def net_name(self, netname=""):
         if not self.is_void and self.prim_type not in ["component"]:
             vMaterial = ["NAME:Net", "Value:=", netname]
             self.change_property(vMaterial)
 
@@ -1146,15 +1139,15 @@
             placement layer.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        cent = _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Center")
+        cent = self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Center")
         if cent:
             return cent.split(",")
 
     @center.setter
     def center(self, position):
         vMaterial = ["NAME:Center", "Value:=", position]
         self.change_property(vMaterial)
@@ -1169,15 +1162,15 @@
             placement layer.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Radius")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Radius")
 
     @radius.setter
     def radius(self, value):
         vMaterial = ["NAME:Radius", "Value:=", value]
         self.change_property(vMaterial)
 
 
@@ -1197,15 +1190,15 @@
             placement layer.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "CornerRadius")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "CornerRadius")
 
     @corner_radius.setter
     def corner_radius(self, value):
         vMaterial = ["NAME:CornerRadius", "Value:=", value]
         self.change_property(vMaterial)
 
     @property
@@ -1220,16 +1213,15 @@
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         return (
             True
-            if _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "2 pt Description")
-            in [True, "true"]
+            if self._oeditor.GetPropertyValue("BaseElementTab", self.name, "2 pt Description") in [True, "true"]
             else False
         )
 
     @two_point_description.setter
     def two_point_description(self, value):
         vMaterial = ["NAME:2 pt Description", "Value:=", value]
         self.change_property(vMaterial)
@@ -1245,15 +1237,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if not self.two_point_description:
-            cent = _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Center")
+            cent = self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Center")
             if cent:
                 return cent.split(",")
 
     @center.setter
     def center(self, value):
         if not self.two_point_description:
             vMaterial = ["NAME:Center", "X:=", value[0], "Y:=", value[1]]
@@ -1270,15 +1262,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if not self.two_point_description:
-            return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Width")
+            return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Width")
 
     @width.setter
     def width(self, value):
         if not self.two_point_description:
             vMaterial = ["NAME:Width", "Value:=", value]
             self.change_property(vMaterial)
 
@@ -1293,15 +1285,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if not self.two_point_description:
-            return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Height")
+            return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Height")
 
     @height.setter
     def height(self, value):
         if not self.two_point_description:
             vMaterial = ["NAME:Height", "Value:=", value]
             self.change_property(vMaterial)
 
@@ -1316,15 +1308,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if self.two_point_description:
-            pa = _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Pt A")
+            pa = self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Pt A")
             if pa:
                 return pa.split(",")
 
     @point_a.setter
     def point_a(self, value):
         if self.two_point_description:
             vMaterial = ["NAME:Pt A", "X:=", value[0], "Y:=", value[1]]
@@ -1341,15 +1333,15 @@
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
         if self.two_point_description:
-            pa = _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Pt B")
+            pa = self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Pt B")
             if pa:
                 return pa.split(",")
 
     @point_b.setter
     def point_b(self, value):
         if self.two_point_description:
             vMaterial = ["NAME:Pt B", "X:=", value[0], "Y:=", value[1]]
@@ -1374,15 +1366,15 @@
             Bend Type.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "BendType")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "BendType")
 
     @bend_type.setter
     def bend_type(self, value):
         vMaterial = ["NAME:BendType", "Value:=", value]
         self.change_property(vMaterial)
 
     @property
@@ -1395,15 +1387,15 @@
             Start Cap Type.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "StartCapType")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "StartCapType")
 
     @start_cap_type.setter
     def start_cap_type(self, value):
         vMaterial = ["NAME:StartCap Type", "Value:=", value]
         self.change_property(vMaterial)
 
     @property
@@ -1416,15 +1408,15 @@
             End Cap Type.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "EndCapType")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "EndCapType")
 
     @end_cap_type.setter
     def end_cap_type(self, value):
         vMaterial = ["NAME:EndCap Type", "Value:=", value]
         self.change_property(vMaterial)
 
     @property
@@ -1437,15 +1429,15 @@
             Line Width.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "LineWidth")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "LineWidth")
 
     @width.setter
     def width(self, value):
         vMaterial = ["NAME:LineWidth", "Value:=", value]
         self.change_property(vMaterial)
 
     @property
@@ -1458,33 +1450,30 @@
             Line length.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "TotalLength")
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "TotalLength")
 
     @property
     def center_line(self):
         """Get the center line points.
 
         Returns
         -------
         dict
             Points.
         """
         props = [i for i in list(self._oeditor.GetProperties("BaseElementTab", self.name)) if i.startswith("Pt")]
         self._center_line = {}
         for i in props:
             self._center_line[i] = [
-                i.strip()
-                for i in _retry_ntimes(self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, i).split(
-                    ","
-                )
+                i.strip() for i in self._oeditor.GetPropertyValue("BaseElementTab", self.name, i).split(",")
             ]
         return self._center_line
 
     @center_line.setter
     def center_line(self, points):
         u = self._primitives.model_units
         for point_name, value in points.items():
@@ -1793,17 +1782,15 @@
            List of ``(x, y)`` coordinates for the component location.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        location = _retry_ntimes(
-            self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Location"
-        ).split(",")
+        location = self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Location").split(",")
         locs = []
         for i in location:
             try:
                 locs.append(float(i))
             except ValueError:  # pragma: no cover
                 locs.append(i)
         return locs
```

### Comparing `pyaedt-0.6.82/pyaedt/modeler/schematic.py` & `pyaedt-0.6.85/pyaedt/modeler/schematic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 import random
 import re
 
 from pyaedt.generic.constants import AEDT_UNITS
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.circuits.PrimitivesEmit import EmitComponent
 from pyaedt.modeler.circuits.PrimitivesEmit import EmitComponents
 from pyaedt.modeler.circuits.PrimitivesMaxwellCircuit import MaxwellCircuitComponents
 from pyaedt.modeler.circuits.PrimitivesNexxim import NexximComponents
 from pyaedt.modeler.circuits.PrimitivesTwinBuilder import TwinBuilderComponents
@@ -538,15 +537,15 @@
 
         References
         ----------
 
         >>> oEditor.GetActiveUnits
         >>> oEditor.SetActiveUnits
         """
-        return _retry_ntimes(10, self.layouteditor.GetActiveUnits)
+        return self.layouteditor.GetActiveUnits()
 
     @property
     def layout(self):
         """Primitives.
 
         Returns
         -------
```

### Comparing `pyaedt-0.6.82/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.85/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -480,20 +480,134 @@
             log_scale,
         )
         if not keep_plot_after_generation:
             plotf.delete()
         return model
 
     @pyaedt_function_handler()
+    def plot_animated_field(
+        self,
+        quantity,
+        object_list,
+        plot_type="Surface",
+        setup_name=None,
+        intrinsics=None,
+        variation_variable="Phi",
+        variation_list=["0deg"],
+        view="isometric",
+        plot_label=None,
+        show=True,
+        scale_min=None,
+        scale_max=None,
+        plot_cad_objs=True,
+        log_scale=True,
+        zoom=None,
+        export_gif=False,
+        export_path="",
+        force_opacity_value=0.1,
+    ):
+        """Create an animated field plot using Python PyVista and export to a gif file.
+
+        .. note::
+           The PyVista module rebuilds the mesh and the overlap fields on the mesh.
+
+        Parameters
+        ----------
+        quantity : str
+            Quantity to plot (e.g. ``"Mag_E"``).
+        object_list : list, str
+            List of objects or faces to which apply the Field Plot.
+        plot_type  : str, optional
+            Plot type. Options are ``"Surface"``, ``"Volume"``, ``"CutPlane"``.
+        setup_name : str, optional
+            Setup and sweep name on which create the field plot. Default is None for nominal setup usage.
+        intrinsics : dict, optional.
+            Intrinsic dictionary that is needed for the export.
+            The default is ``None`` which try to retrieve intrinsics from setup.
+        variation_variable : str, optional
+            Variable to vary. The default is ``"Phi"``.
+        variation_list : list, optional
+            List of variation values with units. The default is
+            ``["0deg"]``.
+        view : str, optional
+           View to export. Options are ``"isometric"``, ``"xy"``, ``"xz"``, ``"yz"``.
+        show : bool, optional
+            Export Image without plotting on UI.
+        scale_min : float, optional
+            Fix the Scale Minimum value.
+        scale_max : float, optional
+            Fix the Scale Maximum value.
+        plot_cad_objs : bool, optional
+            Whether to include objects in the plot. The default is ``True``.
+        log_scale : bool, optional
+            Whether to plot fields in log scale. The default is ``True``.
+        zoom : float, optional
+            Zoom factor.
+        export_gif : bool, optional
+             Whether to export an animated gif or not. The default is ``False``.
+        export_path : str, optional
+            Image export path. Default is ``None`` to not ``working_directory`` will be used to save the image.
+        force_opacity_value : float, optional
+            Opacity value between 0 and 1 to be applied to all model.
+            If `None` aedt opacity will be applied to each object.
+
+        Returns
+        -------
+        :class:`pyaedt.generic.plot.ModelPlotter`
+            Model Object.
+        """
+        if not export_path:
+            export_path = self._app.working_directory
+
+        v = 0
+        fields_to_add = []
+        for el in variation_list:
+            intrinsics[variation_variable] = el
+            if plot_type == "Surface":
+                plotf = self.create_fieldplot_surface(object_list, quantity, setup_name, intrinsics)
+            elif plot_type == "Volume":
+                plotf = self.create_fieldplot_volume(object_list, quantity, setup_name, intrinsics)
+            else:
+                plotf = self.create_fieldplot_cutplane(object_list, quantity, setup_name, intrinsics)
+            if plotf:
+                file_to_add = self.export_field_plot(plotf.name, export_path, plotf.name + str(v))
+                if file_to_add:
+                    fields_to_add.append(file_to_add)
+                plotf.delete()
+            v += 1
+        model = self.get_model_plotter_geometries(
+            generate_mesh=False, get_objects_from_aedt=plot_cad_objs, force_opacity_value=force_opacity_value
+        )
+        model.off_screen = not show
+
+        if fields_to_add:
+            model.add_frames_from_file(fields_to_add, log_scale=log_scale)
+        if export_gif:
+            model.gif_file = os.path.join(self._app.working_directory, self._app.project_name + ".gif")
+        if view != "isometric" and view in ["xy", "xz", "yz"]:
+            model.camera_position = view
+        elif view != "isometric":
+            self.logger.warning("Wrong view setup. It has to be one of xy, xz, yz, isometric.")
+
+        if scale_min and scale_max:
+            model.range_min = scale_min
+            model.range_max = scale_max
+        if zoom:
+            model.zoom = zoom
+        if show or export_gif:
+            model.animate()
+        return model
+
+    @pyaedt_function_handler()
     def animate_fields_from_aedtplt(
         self,
         plotname,
         plot_folder=None,
         meshplot=False,
-        variation_variable="Phi",
+        variation_variable="Phase",
         variation_list=["0deg"],
         project_path="",
         export_gif=False,
         show=True,
     ):
         """Generate a field plot to an image file (JPG or PNG) using PyVista.
 
@@ -504,15 +618,15 @@
         ----------
         plotname : str
             Name of the plot or the name of the object.
         plot_folder : str, optional
             Name of the folder in which the plot resides. The default
             is ``None``.
         variation_variable : str, optional
-            Variable to vary. The default is ``"Phi"``.
+            Variable to vary. The default is ``"Phase"``.
         variation_list : list, optional
             List of variation values with units. The default is
             ``["0deg"]``.
         project_path : str, optional
             Path for the export. The default is ``""`` which export file in working_directory.
         meshplot : bool, optional
              The default is ``False``. Valid from Version 2021.2.
@@ -532,24 +646,28 @@
         else:
             self.ofieldsreporter.UpdateQuantityFieldsPlots(plot_folder)
 
         fields_to_add = []
         if not project_path:
             project_path = self._app.working_directory
         for el in variation_list:
-            self._app._odesign.ChangeProperty(
-                [
-                    "NAME:AllTabs",
+            if plotname in self.field_plots and variation_variable in self.field_plots[plotname].intrinsincList:
+                self.field_plots[plotname].intrinsincList[variation_variable] = el
+                self.field_plots[plotname].update()
+            else:
+                self._app._odesign.ChangeProperty(
                     [
-                        "NAME:FieldsPostProcessorTab",
-                        ["NAME:PropServers", "FieldsReporter:" + plotname],
-                        ["NAME:ChangedProps", ["NAME:" + variation_variable, "Value:=", el]],
-                    ],
-                ]
-            )
+                        "NAME:AllTabs",
+                        [
+                            "NAME:FieldsPostProcessorTab",
+                            ["NAME:PropServers", "FieldsReporter:" + plotname],
+                            ["NAME:ChangedProps", ["NAME:" + variation_variable, "Value:=", el]],
+                        ],
+                    ]
+                )
             fields_to_add.append(
                 self.export_field_plot(plotname, project_path, plotname + variation_variable + str(el))
             )
 
         model = self.get_model_plotter_geometries(generate_mesh=False)
         model.off_screen = not show
 
@@ -577,14 +695,17 @@
         export_gif=False,
         show=True,
         zoom=None,
         log_scale=False,
     ):
         """Generate a field plot to an animated gif file using PyVista.
 
+        .. deprecated:: 0.6.83
+            No need to use primitives anymore. You can instantiate primitives methods directly from modeler instead.
+
          .. note::
             The PyVista module rebuilds the mesh and the overlap fields on the mesh.
 
         This method creates the plot and exports it.
         It is an alternative to the method :func:`animate_fields_from_aedtplt`,
         which uses an existing plot.
 
@@ -623,45 +744,33 @@
             Whether to plot fields in log scale. The default is ``True``.
 
         Returns
         -------
         :class:`pyaedt.generic.plot.ModelPlotter`
             Model Object.
         """
-        if not project_path:
-            project_path = self._app.working_directory
-
-        v = 0
-        fields_to_add = []
-        for el in variation_list:
-            intrinsic_dict[variation_variable] = el
-            if plottype == "Surface":
-                plotf = self.create_fieldplot_surface(object_list, quantityname, setup_name, intrinsic_dict)
-            elif plottype == "Volume":
-                plotf = self.create_fieldplot_volume(object_list, quantityname, setup_name, intrinsic_dict)
-            else:
-                plotf = self.create_fieldplot_cutplane(object_list, quantityname, setup_name, intrinsic_dict)
-            if plotf:
-                file_to_add = self.export_field_plot(plotf.name, project_path, plotf.name + str(v))
-                if file_to_add:
-                    fields_to_add.append(file_to_add)
-                plotf.delete()
-            v += 1
-        model = self.get_model_plotter_geometries(generate_mesh=False)
-        model.off_screen = not show
+        warnings.warn(
+            "`animate_fields_from_aedtplt_2` is deprecated. Use `plot_animated_field` property instead.",
+            DeprecationWarning,
+        )
 
-        if fields_to_add:
-            model.add_frames_from_file(fields_to_add, log_scale=log_scale)
-        if export_gif:
-            model.gif_file = os.path.join(self._app.working_directory, self._app.project_name + ".gif")
-        if zoom:
-            model.zoom = zoom
-        if show or export_gif:
-            model.animate()
-        return model
+        return self.plot_animated_field(
+            quantity=quantityname,
+            object_list=object_list,
+            plot_type=plottype,
+            setup_name=setup_name,
+            intrinsics=intrinsic_dict,
+            variation_variable=variation_variable,
+            variation_list=variation_list,
+            export_path=project_path,
+            log_scale=log_scale,
+            show=show,
+            export_gif=export_gif,
+            zoom=zoom,
+        )
 
     @pyaedt_function_handler()
     def create_3d_plot(
         self, solution_data, nominal_sweep=None, nominal_value=None, primary_sweep="Theta", secondary_sweep="Phi"
     ):
         """Create a 3D plot using Matplotlib.
```

### Comparing `pyaedt-0.6.82/pyaedt/modules/Boundary.py` & `pyaedt-0.6.85/pyaedt/modules/Boundary.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,63 @@
         else:
             self._app.oboundary.DeleteBoundaries([self.name])
         for el in self._app.boundaries:
             if el.name == self.name:
                 self._app.boundaries.remove(el)
         return True
 
+    def _get_boundary_data(self):
+        dict_out = {}
+        if self._app.design_properties and "BoundarySetup" in self._app.design_properties:
+            for ds in self._app.design_properties["BoundarySetup"]["Boundaries"]:
+                try:
+                    if isinstance(self._app.design_properties["BoundarySetup"]["Boundaries"][ds], (OrderedDict, dict)):
+                        if (
+                            self._app.design_properties["BoundarySetup"]["Boundaries"][ds]["BoundType"] == "Network"
+                            and self._app.design_type == "Icepak"
+                        ):
+                            dict_out[ds] = [self._app.design_properties["BoundarySetup"]["Boundaries"][ds], ""]
+                        else:
+                            dict_out[ds] = [
+                                self._app.design_properties["BoundarySetup"]["Boundaries"][ds],
+                                self._app.design_properties["BoundarySetup"]["Boundaries"][ds]["BoundType"],
+                            ]
+
+                except:
+                    pass
+        if self._app.design_properties and "MaxwellParameterSetup" in self._app.design_properties:
+            for ds in self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"]:
+                try:
+                    param = "MaxwellParameters"
+                    setup = "MaxwellParameterSetup"
+                    if isinstance(self._app.design_properties[setup][param][ds], (OrderedDict, dict)):
+                        dict_out[ds] = [
+                            self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds],
+                            self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds][
+                                "MaxwellParameterType"
+                            ],
+                        ]
+                except:
+                    pass
+        if self._app.design_properties and "ModelSetup" in self._app.design_properties:
+            if "MotionSetupList" in self._app.design_properties["ModelSetup"]:
+                for ds in self._app.design_properties["ModelSetup"]["MotionSetupList"]:
+                    try:
+                        motion_list = "MotionSetupList"
+                        setup = "ModelSetup"
+                        # check moving part
+                        if isinstance(self._app.design_properties[setup][motion_list][ds], (OrderedDict, dict)):
+                            dict_out[ds] = [
+                                self._app.design_properties["ModelSetup"]["MotionSetupList"][ds],
+                                self._app.design_properties["ModelSetup"]["MotionSetupList"][ds]["MotionType"],
+                            ]
+                    except:
+                        pass
+        return dict_out
+
 
 class NativeComponentObject(BoundaryCommon, object):
     """Manages Native Component data and execution.
 
     Parameters
     ----------
     app : object
@@ -128,14 +177,15 @@
     """
 
     def __init__(self, app, component_type, component_name, props):
         self.auto_update = False
         self._app = app
         self.name = "InsertNativeComponentData"
         self.component_name = component_name
+
         self.props = BoundaryProps(
             self,
             OrderedDict(
                 {
                     "TargetCS": "Global",
                     "SubmodelDefinitionName": self.component_name,
                     "ComponentPriorityLists": OrderedDict({}),
@@ -292,17 +342,17 @@
 
     Parameters
     ----------
     app : object
         An AEDT application from ``pyaedt.application``.
     name : str
         Name of the boundary.
-    props : dict
+    props : dict, optional
         Properties of the boundary.
-    boundarytype : str
+    boundarytype : str, optional
         Type of the boundary.
 
     Examples
     --------
 
     Create a cylinder at the XY working plane and assign a copper coating of 0.2 mm to it. The Coating is a boundary
     operation and coat will return a ``pyaedt.modules.Boundary.BoundaryObject``
@@ -311,32 +361,108 @@
     >>> hfss =Hfss()
     >>> origin = hfss.modeler.Position(0, 0, 0)
     >>> inner = hfss.modeler.create_cylinder(hfss.PLANE.XY, origin, 3, 200, 0, "inner")
     >>> inner_id = hfss.modeler.get_obj_id("inner")
     >>> coat = hfss.assign_coating([inner_id], "copper", usethickness=True, thickness="0.2mm")
     """
 
-    def __init__(self, app, name, props, boundarytype, auto_update=True):
+    def __init__(self, app, name, props=None, boundarytype=None, auto_update=True):
         self.auto_update = False
         self._app = app
         self._name = name
-        self.props = BoundaryProps(self, OrderedDict(props))
+        self._props = None
+        if props:
+            self._props = BoundaryProps(self, OrderedDict(props))
         self._type = boundarytype
         self._boundary_name = self.name
         self.auto_update = auto_update
 
     @property
+    def object_properties(self):
+        """Object-oriented properties.
+
+        Returns
+        -------
+        class:`pyaedt.modeler.cad.elements3d.BinaryTreeNode`
+
+        """
+        from pyaedt.modeler.cad.elements3d import BinaryTreeNode
+
+        child_object = None
+        design_childs = self._app.get_oo_name(self._app.odesign)
+
+        if "Thermal" in design_childs:
+            cc = self._app.get_oo_object(self._app.odesign, "Thermal")
+            cc_names = self._app.get_oo_name(cc)
+            if self.name in cc_names:
+                child_object = cc_names
+            if child_object:
+                return BinaryTreeNode(self.name, child_object, False)
+        elif "Boundaries" in design_childs:
+            cc = self._app.get_oo_object(self._app.odesign, "Boundaries")
+            if self.name in cc.GetChildNames():
+                child_object = cc.GetChildObject(self.name)
+            elif "Excitations" in design_childs and self.name in self._app.get_oo_name(
+                self._app.odesign, "Excitations"
+            ):
+                child_object = self._app.get_oo_object(self._app.odesign, "Excitations").GetChildObject(self.name)
+            elif self._app.design_type in ["Maxwell 3D", "Maxwell 2D"] and "Model" in design_childs:
+                model = self._app.get_oo_object(self._app.odesign, "Model")
+                if self.name in model.GetChildNames():
+                    child_object = model.GetChildObject(self.name)
+            elif "Excitations" in design_childs and self._app.get_oo_name(self._app.odesign, "Excitations"):
+                for port in self._app.get_oo_name(self._app.odesign, "Excitations"):
+                    terminals = self._app.get_oo_name(self._app.odesign, "Excitations\\{}".format(port))
+                    if self.name in terminals:
+                        child_object = self._app.get_oo_object(
+                            self._app.odesign, "Excitations\\{}\\{}".format(port, self.name)
+                        )
+            elif "Conductors" in design_childs and self._app.get_oo_name(self._app.odesign, "Conductors"):
+                for port in self._app.get_oo_name(self._app.odesign, "Conductors"):
+                    if self.name == port:
+                        child_object = self._app.get_oo_object(self._app.odesign, "Conductors\\{}".format(port))
+
+        if child_object:
+            return BinaryTreeNode(self.name, child_object, False)
+
+        return False
+
+    @property
+    def props(self):
+        """Boundary data.
+
+        Returns
+        -------
+        :class:BoundaryProps
+        """
+        props = self._get_boundary_data()
+
+        if self.name in props and not self._props:
+            self._props = BoundaryProps(self, OrderedDict(props[self.name][0]))
+            self._type = props[self.name][1]
+        return self._props
+
+    @property
     def type(self):
         """Boundary type.
 
         Returns
         -------
         str
-            Returns Type of the boundary
+            Returns the type of the boundary.
         """
+        if not self._type:
+            if self.available_properties:
+                if "Type" in self.available_properties:
+                    self._type = self.props["Type"]
+                elif "BoundType" in self.available_properties:
+                    self._type = self.props["BoundType"]
+            elif self.object_properties and self.object_properties.props["Type"]:
+                self._type = self.object_properties.props["Type"]
+
         if self._app.design_type == "Icepak" and self._type == "Source":
             return "SourceIcepak"
         else:
             return self._type
 
     @type.setter
     def type(self, value):
@@ -379,163 +505,164 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        if self.type == "Perfect E":
+        bound_type = self.type
+        if bound_type == "Perfect E":
             self._app.oboundary.AssignPerfectE(self._get_args())
-        elif self.type == "Perfect H":
+        elif bound_type == "Perfect H":
             self._app.oboundary.AssignPerfectH(self._get_args())
-        elif self.type == "Aperture":
+        elif bound_type == "Aperture":
             self._app.oboundary.AssignAperture(self._get_args())
-        elif self.type == "Radiation":
+        elif bound_type == "Radiation":
             self._app.oboundary.AssignRadiation(self._get_args())
-        elif self.type == "Finite Conductivity":
+        elif bound_type == "Finite Conductivity":
             self._app.oboundary.AssignFiniteCond(self._get_args())
-        elif self.type == "Lumped RLC":
+        elif bound_type == "Lumped RLC":
             self._app.oboundary.AssignLumpedRLC(self._get_args())
-        elif self.type == "Impedance":
+        elif bound_type == "Impedance":
             self._app.oboundary.AssignImpedance(self._get_args())
-        elif self.type == "Layered Impedance":
+        elif bound_type == "Layered Impedance":
             self._app.oboundary.AssignLayeredImp(self._get_args())
-        elif self.type == "Anisotropic Impedance":
+        elif bound_type == "Anisotropic Impedance":
             self._app.oboundary.AssignAnisotropicImpedance(self._get_args())
-        elif self.type == "Primary":
+        elif bound_type == "Primary":
             self._app.oboundary.AssignPrimary(self._get_args())
-        elif self.type == "Secondary":
+        elif bound_type == "Secondary":
             self._app.oboundary.AssignSecondary(self._get_args())
-        elif self.type == "Lattice Pair":
+        elif bound_type == "Lattice Pair":
             self._app.oboundary.AssignLatticePair(self._get_args())
-        elif self.type == "HalfSpace":
+        elif bound_type == "HalfSpace":
             self._app.oboundary.AssignHalfSpace(self._get_args())
-        elif self.type == "Multipaction SEE":
+        elif bound_type == "Multipaction SEE":
             self._app.oboundary.AssignMultipactionSEE(self._get_args())
-        elif self.type == "Fresnel":
+        elif bound_type == "Fresnel":
             self._app.oboundary.AssignFresnel(self._get_args())
-        elif self.type == "Symmetry":
+        elif bound_type == "Symmetry":
             self._app.oboundary.AssignSymmetry(self._get_args())
-        elif self.type == "Zero Tangential H Field":
+        elif bound_type == "Zero Tangential H Field":
             self._app.oboundary.AssignZeroTangentialHField(self._get_args())
-        elif self.type == "Zero Integrated Tangential H Field":
+        elif bound_type == "Zero Integrated Tangential H Field":
             self._app.oboundary.AssignIntegratedZeroTangentialHField(self._get_args())
-        elif self.type == "Tangential H Field":
+        elif bound_type == "Tangential H Field":
             self._app.oboundary.AssignTangentialHField(self._get_args())
-        elif self.type == "Insulating":
+        elif bound_type == "Insulating":
             self._app.oboundary.AssignInsulating(self._get_args())
-        elif self.type == "Independent":
+        elif bound_type == "Independent":
             self._app.oboundary.AssignIndependent(self._get_args())
-        elif self.type == "Dependent":
+        elif bound_type == "Dependent":
             self._app.oboundary.AssignDependent(self._get_args())
-        elif self.type == "Band":
+        elif bound_type == "Band":
             self._app.omodelsetup.AssignBand(self._get_args())
-        elif self.type == "InfiniteGround":
+        elif bound_type == "InfiniteGround":
             self._app.oboundary.AssignInfiniteGround(self._get_args())
-        elif self.type == "ThinConductor":
+        elif bound_type == "ThinConductor":
             self._app.oboundary.AssignThinConductor(self._get_args())
-        elif self.type == "Stationary Wall":
+        elif bound_type == "Stationary Wall":
             self._app.oboundary.AssignStationaryWallBoundary(self._get_args())
-        elif self.type == "Symmetry Wall":
+        elif bound_type == "Symmetry Wall":
             self._app.oboundary.AssignSymmetryWallBoundary(self._get_args())
-        elif self.type == "Resistance":
+        elif bound_type == "Resistance":
             self._app.oboundary.AssignResistanceBoundary(self._get_args())
-        elif self.type == "Conducting Plate":
+        elif bound_type == "Conducting Plate":
             self._app.oboundary.AssignConductingPlateBoundary(self._get_args())
-        elif self.type == "Adiabatic Plate":
+        elif bound_type == "Adiabatic Plate":
             self._app.oboundary.AssignAdiabaticPlateBoundary(self._get_args())
-        elif self.type == "Network":
+        elif bound_type == "Network":
             self._app.oboundary.AssignNetworkBoundary(self._get_args())
-        elif self.type == "Grille":
+        elif bound_type == "Grille":
             self._app.oboundary.AssignGrilleBoundary(self._get_args())
-        elif self.type == "Block":
+        elif bound_type == "Block":
             self._app.oboundary.AssignBlockBoundary(self._get_args())
-        elif self.type == "SourceIcepak":
+        elif bound_type == "SourceIcepak":
             self._app.oboundary.AssignSourceBoundary(self._get_args())
-        elif self.type == "Opening":
+        elif bound_type == "Opening":
             self._app.oboundary.AssignOpeningBoundary(self._get_args())
-        elif self.type == "EMLoss":
+        elif bound_type == "EMLoss":
             self._app.oboundary.AssignEMLoss(self._get_args())
-        elif self.type == "ThermalCondition":
+        elif bound_type == "ThermalCondition":
             self._app.oboundary.AssignThermalCondition(self._get_args())
-        elif self.type == "Convection":
+        elif bound_type == "Convection":
             self._app.oboundary.AssignConvection(self._get_args())
-        elif self.type == "HeatFlux":
+        elif bound_type == "HeatFlux":
             self._app.oboundary.AssignHeatFlux(self._get_args())
-        elif self.type == "HeatGeneration":
+        elif bound_type == "HeatGeneration":
             self._app.oboundary.AssignHeatGeneration(self._get_args())
-        elif self.type == "Temperature":
+        elif bound_type == "Temperature":
             self._app.oboundary.AssignTemperature(self._get_args())
-        elif self.type == "RotatingFluid":
+        elif bound_type == "RotatingFluid":
             self._app.oboundary.AssignRotatingFluid(self._get_args())
-        elif self.type == "Frictionless":
+        elif bound_type == "Frictionless":
             self._app.oboundary.AssignFrictionlessSupport(self._get_args())
-        elif self.type == "FixedSupport":
+        elif bound_type == "FixedSupport":
             self._app.oboundary.AssignFixedSupport(self._get_args())
-        elif self.type == "Voltage":
+        elif bound_type == "Voltage":
             self._app.oboundary.AssignVoltage(self._get_args())
-        elif self.type == "VoltageDrop":
+        elif bound_type == "VoltageDrop":
             self._app.oboundary.AssignVoltageDrop(self._get_args())
-        elif self.type == "Current":
+        elif bound_type == "Current":
             self._app.oboundary.AssignCurrent(self._get_args())
-        elif self.type == "CurrentDensity":
+        elif bound_type == "CurrentDensity":
             self._app.oboundary.AssignCurrentDensity(self._get_args())
-        elif self.type == "CurrentDensityGroup":
+        elif bound_type == "CurrentDensityGroup":
             self._app.oboundary.AssignCurrentDensityGroup(self._get_args()[2], self._get_args()[3])
-        elif self.type == "CurrentDensityTerminal":
+        elif bound_type == "CurrentDensityTerminal":
             self._app.oboundary.AssignCurrentDensityTerminal(self._get_args())
-        elif self.type == "CurrentDensityTerminalGroup":
+        elif bound_type == "CurrentDensityTerminalGroup":
             self._app.oboundary.AssignCurrentDensityTerminalGroup(self._get_args()[2], self._get_args()[3])
-        elif self.type == "Balloon":
+        elif bound_type == "Balloon":
             self._app.oboundary.AssignBalloon(self._get_args())
-        elif self.type == "Winding" or self.type == "Winding Group":
+        elif bound_type == "Winding" or bound_type == "Winding Group":
             self._app.oboundary.AssignWindingGroup(self._get_args())
-        elif self.type == "Vector Potential":
+        elif bound_type == "Vector Potential":
             self._app.oboundary.AssignVectorPotential(self._get_args())
-        elif self.type == "CoilTerminal" or self.type == "Coil Terminal":
+        elif bound_type == "CoilTerminal" or bound_type == "Coil Terminal":
             self._app.oboundary.AssignCoilTerminal(self._get_args())
-        elif self.type == "Coil":
+        elif bound_type == "Coil":
             self._app.oboundary.AssignCoil(self._get_args())
-        elif self.type == "Source":
+        elif bound_type == "Source":
             self._app.oboundary.AssignSource(self._get_args())
-        elif self.type == "Sink":
+        elif bound_type == "Sink":
             self._app.oboundary.AssignSink(self._get_args())
-        elif self.type == "SignalNet":
+        elif bound_type == "SignalNet":
             self._app.oboundary.AssignSignalNet(self._get_args())
-        elif self.type == "GroundNet":
+        elif bound_type == "GroundNet":
             self._app.oboundary.AssignGroundNet(self._get_args())
-        elif self.type == "FloatingNet":
+        elif bound_type == "FloatingNet":
             self._app.oboundary.AssignFloatingNet(self._get_args())
-        elif self.type == "SignalLine":
+        elif bound_type == "SignalLine":
             self._app.oboundary.AssignSingleSignalLine(self._get_args())
-        elif self.type == "ReferenceGround":
+        elif bound_type == "ReferenceGround":
             self._app.oboundary.AssignSingleReferenceGround(self._get_args())
-        elif self.type == "Circuit Port":
+        elif bound_type == "Circuit Port":
             self._app.oboundary.AssignCircuitPort(self._get_args())
-        elif self.type == "Lumped Port":
+        elif bound_type == "Lumped Port":
             self._app.oboundary.AssignLumpedPort(self._get_args())
-        elif self.type == "Wave Port":
+        elif bound_type == "Wave Port":
             self._app.oboundary.AssignWavePort(self._get_args())
-        elif self.type == "Floquet Port":
+        elif bound_type == "Floquet Port":
             self._app.oboundary.AssignFloquetPort(self._get_args())
-        elif self.type == "AutoIdentify":
+        elif bound_type == "AutoIdentify":
             self._app.oboundary.AutoIdentifyPorts(
                 ["NAME:Faces", self.props["Faces"]],
                 self.props["IsWavePort"],
                 ["NAME:ReferenceConductors"] + self.props["ReferenceConductors"],
                 self.name,
                 self.props["RenormalizeModes"],
             )
-        elif self.type == "SBRTxRxSettings":
+        elif bound_type == "SBRTxRxSettings":
             self._app.oboundary.SetSBRTxRxSettings(self._get_args())
-        elif self.type == "EndConnection":
+        elif bound_type == "EndConnection":
             self._app.oboundary.AssignEndConnection(self._get_args())
-        elif self.type == "Hybrid":
+        elif bound_type == "Hybrid":
             self._app.oboundary.AssignHybridRegion(self._get_args())
-        elif self.type == "FluxTangential":
+        elif bound_type == "FluxTangential":
             self._app.oboundary.AssignFluxTangential(self._get_args())
         else:
             return False
         return True
 
     @pyaedt_function_handler()
     def update(self):
@@ -543,141 +670,145 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        if self.type == "Perfect E":
+        bound_type = self.type
+        if bound_type == "Perfect E":
             self._app.oboundary.EditPerfectE(self._boundary_name, self._get_args())
-        elif self.type == "Perfect H":
+        elif bound_type == "Perfect H":
             self._app.oboundary.EditPerfectH(self._boundary_name, self._get_args())
-        elif self.type == "Aperture":
+        elif bound_type == "Aperture":
             self._app.oboundary.EditAperture(self._boundary_name, self._get_args())
-        elif self.type == "Radiation":
+        elif bound_type == "Radiation":
             self._app.oboundary.EditRadiation(self._boundary_name, self._get_args())
-        elif self.type == "Finite Conductivity":
+        elif bound_type == "Finite Conductivity":
             self._app.oboundary.EditFiniteCond(self._boundary_name, self._get_args())
-        elif self.type == "Lumped RLC":
+        elif bound_type == "Lumped RLC":
             self._app.oboundary.EditLumpedRLC(self._boundary_name, self._get_args())
-        elif self.type == "Impedance":
+        elif bound_type == "Impedance":
             self._app.oboundary.EditImpedance(self._boundary_name, self._get_args())
-        elif self.type == "Layered Impedance":
+        elif bound_type == "Layered Impedance":
             self._app.oboundary.EditLayeredImpedance(self._boundary_name, self._get_args())
-        elif self.type == "Anisotropic Impedance":
+        elif bound_type == "Anisotropic Impedance":
             self._app.oboundary.EditAssignAnisotropicImpedance(
                 self._boundary_name, self._get_args()
             )  # pragma: no cover
-        elif self.type == "Primary":
+        elif bound_type == "Primary":
             self._app.oboundary.EditPrimary(self._boundary_name, self._get_args())
-        elif self.type == "Secondary":
+        elif bound_type == "Secondary":
             self._app.oboundary.EditSecondary(self._boundary_name, self._get_args())
-        elif self.type == "Lattice Pair":
+        elif bound_type == "Lattice Pair":
             self._app.oboundary.EditLatticePair(self._boundary_name, self._get_args())
-        elif self.type == "HalfSpace":
+        elif bound_type == "HalfSpace":
             self._app.oboundary.EditHalfSpace(self._boundary_name, self._get_args())
-        elif self.type == "Multipaction SEE":
+        elif bound_type == "Multipaction SEE":
             self._app.oboundary.EditMultipactionSEE(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Fresnel":
+        elif bound_type == "Fresnel":
             self._app.oboundary.EditFresnel(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Symmetry":
+        elif bound_type == "Symmetry":
             self._app.oboundary.EditSymmetry(self._boundary_name, self._get_args())
-        elif self.type == "Zero Tangential H Field":
+        elif bound_type == "Zero Tangential H Field":
             self._app.oboundary.EditZeroTangentialHField(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Zero Integrated Tangential H Field":
+        elif bound_type == "Zero Integrated Tangential H Field":
             self._app.oboundary.EditIntegratedZeroTangentialHField(
                 self._boundary_name, self._get_args()
             )  # pragma: no cover
-        elif self.type == "Tangential H Field":
+        elif bound_type == "Tangential H Field":
             self._app.oboundary.EditTangentialHField(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Insulating":
+        elif bound_type == "Insulating":
             self._app.oboundary.EditInsulating(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Independent":
+        elif bound_type == "Independent":
             self._app.oboundary.EditIndependent(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Dependent":
+        elif bound_type == "Dependent":
             self._app.oboundary.EditDependent(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Band":
+        elif bound_type == "Band":
             self._app.omodelsetup.EditMotionSetup(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "InfiniteGround":
+        elif bound_type == "InfiniteGround":
             self._app.oboundary.EditInfiniteGround(self._boundary_name, self._get_args())
-        elif self.type == "ThinConductor":
+        elif bound_type == "ThinConductor":
             self._app.oboundary.EditThinConductor(self._boundary_name, self._get_args())
-        elif self.type == "Stationary Wall":
+        elif bound_type == "Stationary Wall":
             self._app.oboundary.EditStationaryWallBoundary(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Symmetry Wall":
+        elif bound_type == "Symmetry Wall":
             self._app.oboundary.EditSymmetryWallBoundary(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Resistance":
+        elif bound_type == "Resistance":
             self._app.oboundary.EditResistanceBoundary(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Conducting Plate":
+        elif bound_type == "Conducting Plate":
             self._app.oboundary.EditConductingPlateBoundary(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Adiabatic Plate":
+        elif bound_type == "Adiabatic Plate":
             self._app.oboundary.EditAdiabaticPlateBoundary(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Network":
+        elif bound_type == "Network":
             self._app.oboundary.EditNetworkBoundary(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Grille":
+        elif bound_type == "Grille":
             self._app.oboundary.EditGrilleBoundary(self._boundary_name, self._get_args())
-        elif self.type == "Opening":
+        elif bound_type == "Opening":
             self._app.oboundary.EditOpeningBoundary(self._boundary_name, self._get_args())
-        elif self.type == "EMLoss":
+        elif bound_type == "EMLoss":
             self._app.oboundary.EditEMLoss(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Block":
+        elif bound_type == "Block":
             self._app.oboundary.EditBlockBoundary(self._boundary_name, self._get_args())
-        elif self.type == "SourceIcepak":
+        elif bound_type == "SourceIcepak":
             self._app.oboundary.EditSourceBoundary(self._boundary_name, self._get_args())
-        elif self.type == "HeatFlux":
+        elif bound_type == "HeatFlux":
             self._app.oboundary.EditHeatFlux(self._boundary_name, self._get_args())
-        elif self.type == "HeatGeneration":
+        elif bound_type == "HeatGeneration":
             self._app.oboundary.EditHeatGeneration(self._boundary_name, self._get_args())
-        elif self.type == "Voltage":
+        elif bound_type == "Voltage":
             self._app.oboundary.EditVoltage(self._boundary_name, self._get_args())
-        elif self.type == "VoltageDrop":
+        elif bound_type == "VoltageDrop":
             self._app.oboundary.EditVoltageDrop(self._boundary_name, self._get_args())
-        elif self.type == "Current":
+        elif bound_type == "Current":
             self._app.oboundary.EditCurrent(self._boundary_name, self._get_args())
-        elif self.type == "CurrentDensity":
+        elif bound_type == "CurrentDensity":
             self._app.oboundary.AssignCurrentDensity(self._get_args())
-        elif self.type == "CurrentDensityGroup":
+        elif bound_type == "CurrentDensityGroup":
             self._app.oboundary.AssignCurrentDensityGroup(self._get_args()[2], self._get_args()[3])
-        elif self.type == "CurrentDensityTerminal":
+        elif bound_type == "CurrentDensityTerminal":
             self._app.oboundary.AssignCurrentDensityTerminal(self._get_args())
-        elif self.type == "CurrentDensityTerminalGroup":
+        elif bound_type == "CurrentDensityTerminalGroup":
             self._app.oboundary.AssignCurrentDensityTerminalGroup(self._get_args()[2], self._get_args()[3])
-        elif self.type == "Winding" or self.type == "Winding Group":
+        elif bound_type == "Winding" or bound_type == "Winding Group":
             self._app.oboundary.EditWindingGroup(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Vector Potential":
+        elif bound_type == "Vector Potential":
             self._app.oboundary.EditVectorPotential(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "CoilTerminal" or self.type == "Coil Terminal":
+        elif bound_type == "CoilTerminal" or bound_type == "Coil Terminal":
             self._app.oboundary.EditCoilTerminal(self._boundary_name, self._get_args())
-        elif self.type == "Coil":
+        elif bound_type == "Coil":
             self._app.oboundary.EditCoil(self._boundary_name, self._get_args())
-        elif self.type == "Source":
+        elif bound_type == "Source":
             self._app.oboundary.EditTerminal(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "Sink":
+        elif bound_type == "Sink":
             self._app.oboundary.EditTerminal(self._boundary_name, self._get_args())
-        elif self.type == "SignalNet" or self.type == "GroundNet" or self.type == "FloatingNet":
+        elif bound_type == "SignalNet" or bound_type == "GroundNet" or bound_type == "FloatingNet":
             self._app.oboundary.EditTerminal(self._boundary_name, self._get_args())
-        elif self.type in "Circuit Port":
+        elif bound_type in "Circuit Port":
             self._app.oboundary.EditCircuitPort(self._boundary_name, self._get_args())
-        elif self.type in "Lumped Port":
+        elif bound_type in "Lumped Port":
             self._app.oboundary.EditLumpedPort(self._boundary_name, self._get_args())
-        elif self.type in "Wave Port":
+        elif bound_type in "Wave Port":
             self._app.oboundary.EditWavePort(self._boundary_name, self._get_args())
-        elif self.type == "SetSBRTxRxSettings":
+        elif bound_type == "SetSBRTxRxSettings":
             self._app.oboundary.SetSBRTxRxSettings(self._get_args())  # pragma: no cover
-        elif self.type == "Floquet Port":
+        elif bound_type == "Floquet Port":
             self._app.oboundary.EditFloquetPort(self._boundary_name, self._get_args())  # pragma: no cover
-        elif self.type == "End Connection":
+        elif bound_type == "End Connection":
             self._app.oboundary.EditEndConnection(self._boundary_name, self._get_args())
-        elif self.type == "Hybrid":
+        elif bound_type == "Hybrid":
             self._app.oboundary.EditHybridRegion(self._boundary_name, self._get_args())
-        elif self.type == "Terminal":
+        elif bound_type == "Terminal":
             self._app.oboundary.EditTerminal(self._boundary_name, self._get_args())
         else:
             return False  # pragma: no cover
+
+        self._app._boundaries[self.name] = self._app._boundaries.pop(self._boundary_name)
         self._boundary_name = self.name
+
         return True
 
     @pyaedt_function_handler()
     def update_assignment(self):
         """Update the boundary assignment.
 
         Returns
@@ -723,43 +854,82 @@
 
     Parameters
     ----------
     app : :class:`pyaedt.maxwell.Maxwell3d`, :class:`pyaedt.maxwell.Maxwell2d`
         Either ``Maxwell3d`` or ``Maxwell2d`` application.
     name : str
         Name of the boundary.
-    props : dict
+    props : dict, optional
         Properties of the boundary.
-    boundarytype : str
+    boundarytype : str, optional
         Type of the boundary.
 
     Examples
     --------
 
     Create a matrix in Maxwell3D return a ``pyaedt.modules.Boundary.BoundaryObject``
 
     >>> from pyaedt import Maxwell2d
     >>> maxwell_2d = Maxwell2d()
     >>> coil1 = maxwell_2d.modeler.create_rectangle([8.5,1.5, 0], [8, 3], True, "Coil_1", "vacuum")
     >>> coil2 = maxwell_2d.modeler.create_rectangle([8.5,1.5, 0], [8, 3], True, "Coil_2", "vacuum")
     >>> maxwell_2d.assign_matrix(["Coil_1", "Coil_2"])
     """
 
-    def __init__(self, app, name, props, boundarytype):
+    def __init__(self, app, name, props=None, boundarytype=None):
         self.auto_update = False
         self._app = app
         self._name = name
-        self.props = BoundaryProps(self, OrderedDict(props))
+        self._props = None
+        if props:
+            self._props = BoundaryProps(self, OrderedDict(props))
         self.type = boundarytype
         self._boundary_name = self.name
         self.auto_update = True
 
     @property
+    def object_properties(self):
+        """Object-oriented properties.
+
+        Returns
+        -------
+        class:`pyaedt.modeler.cad.elements3d.BinaryTreeNode`
+
+        """
+
+        from pyaedt.modeler.cad.elements3d import BinaryTreeNode
+
+        cc = self._app.odesign.GetChildObject("Parameters")
+        child_object = None
+        if self.name in cc.GetChildNames():
+            child_object = self._app.odesign.GetChildObject("Parameters").GetChildObject(self.name)
+        elif self.name in self._app.odesign.GetChildObject("Parameters").GetChildNames():
+            child_object = self._app.odesign.GetChildObject("Parameters").GetChildObject(self.name)
+        if child_object:
+            return BinaryTreeNode(self.name, child_object, False)
+        return False
+
+    @property
+    def props(self):
+        """Maxwell parameter data.
+
+        Returns
+        -------
+        :class:BoundaryProps
+        """
+        props = self._get_boundary_data()
+
+        if self.name in props:
+            self._props = BoundaryProps(self, OrderedDict(props[self.name][0]))
+            self._type = props[self.name][1]
+        return self._props
+
+    @property
     def name(self):
-        """Boundary Name."""
+        """Boundary name."""
         return self._name
 
     @name.setter
     def name(self, value):
         self._name = value
         self.update()
 
@@ -1612,33 +1782,71 @@
         Type of the boundary.
     """
 
     def __init__(self, app, name, props, boundarytype):
         self.auto_update = False
         self._app = app
         self._name = name
-        self.props = BoundaryProps(self, OrderedDict(props))
+        self._props = None
+        if props:
+            self._props = BoundaryProps(self, OrderedDict(props))
         self.type = boundarytype
         self._boundary_name = self.name
         self.auto_update = True
 
     @property
+    def object_properties(self):
+        """Object-oriented properties.
+
+        Returns
+        -------
+        class:`pyaedt.modeler.cad.elements3d.BinaryTreeNode`
+
+        """
+        from pyaedt.modeler.cad.elements3d import BinaryTreeNode
+
+        cc = self._app.odesign.GetChildObject("Excitations")
+        child_object = None
+        if self.name in cc.GetChildNames():
+            child_object = self._app.odesign.GetChildObject("Excitations").GetChildObject(self.name)
+        elif self.name in self._app.odesign.GetChildObject("Excitations").GetChildNames():
+            child_object = self._app.odesign.GetChildObject("Excitations").GetChildObject(self.name)
+        if child_object:
+            return BinaryTreeNode(self.name, child_object, False)
+        return False
+
+    @property
     def name(self):
         """Boundary Name."""
         return self._name
 
     @name.setter
     def name(self, value):
         if "Port" in self.props:
             self.auto_update = False
             self.props["Port"] = value
             self.auto_update = True
         self.update()
         self._name = value
 
+    @property
+    def props(self):
+        """Excitation data.
+
+        Returns
+        -------
+        :class:BoundaryProps
+        """
+        props = self._get_boundary_data()
+
+        if self.name in props:
+            self._props = BoundaryProps(self, OrderedDict(props[self.name][0]))
+            self._type = props[self.name][1]
+        return self._props
+
     @pyaedt_function_handler()
     def _get_args(self, props=None):
         """Retrieve arguments.
 
         Parameters
         ----------
         props :
@@ -1659,15 +1867,15 @@
     @pyaedt_function_handler()
     def _refresh_properties(self):
         if len(self._app.oeditor.GetProperties("EM Design", "Excitations:{}".format(self.name))) != len(self.props):
             propnames = self._app.oeditor.GetProperties("EM Design", "Excitations:{}".format(self.name))
             props = OrderedDict()
             for prop in propnames:
                 props[prop] = self._app.oeditor.GetPropertyValue("EM Design", "Excitations:{}".format(self.name), prop)
-            self.props = BoundaryProps(self, props)
+            self._props = BoundaryProps(self, props)
 
     @pyaedt_function_handler()
     def update(self):
         """Update the boundary.
 
         Returns
         -------
@@ -3363,20 +3571,17 @@
     def __init__(self, app, name=None, props=None, create=False):
         if not app.design_type == "Icepak":  # pragma: no cover
             raise NotImplementedError("Networks object works only with Icepak projects ")
         if name is None:
             self._name = generate_unique_name("Network")
         else:
             self._name = name
-        if props is None:
-            props_arg = OrderedDict({})
-        else:
-            props_arg = props
-        # super().__init__(app, self._name, props_arg, "Network", False)
-        super(NetworkObject, self).__init__(app, self._name, props_arg, "Network", False)
+        super(NetworkObject, self).__init__(app, self._name, props, "Network", False)
+        if self.props is None:
+            self._props = {}
         self._nodes = []
         self._links = []
         self._schematic_data = OrderedDict({})
         self._update_from_props()
         if create:
             self.create()
```

### Comparing `pyaedt-0.6.82/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.85/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.85/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.85/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.85/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/Material.py` & `pyaedt-0.6.85/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.85/pyaedt/modules/MaterialLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from pyaedt import is_ironpython
 from pyaedt import settings
 from pyaedt.generic.DataHandlers import _arg2dict
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _create_json_file
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Material import MatProperties
 from pyaedt.modules.Material import Material
 from pyaedt.modules.Material import OrderedDict
 from pyaedt.modules.Material import SurfaceMaterial
@@ -637,15 +636,15 @@
         Returns
         -------
         :class:`pyaedt.modules.Material.Material`
         """
         if matname not in self.odefinition_manager.GetProjectMaterialNames() and not settings.remote_api:
             matname = self._get_aedt_case_name(matname)
         props = {}
-        _arg2dict(list(_retry_ntimes(20, self.omaterial_manager.GetData, matname)), props)
+        _arg2dict(list(self.omaterial_manager.GetData(matname)), props)
         values_view = props.values()
         value_iterator = iter(values_view)
         first_value = next(value_iterator)
         newmat = Material(self, matname, first_value)
         self.material_keys[matname.lower()] = newmat
         return self.material_keys[matname.lower()]
```

### Comparing `pyaedt-0.6.82/pyaedt/modules/Mesh.py` & `pyaedt-0.6.85/pyaedt/modules/Mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from pyaedt.application.design_solutions import model_names
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import MethodNotSupportedError
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 
@@ -286,15 +285,15 @@
         Returns
         -------
         list
             List of changed properties of the mesh operation.
 
         """
         arguments = ["NAME:AllTabs", ["NAME:MeshSetupTab", ["NAME:PropServers", "MeshSetup:{}".format(name)], arg]]
-        _retry_ntimes(10, self._mesh._app.odesign.ChangeProperty, arguments)
+        self._mesh._app.odesign.ChangeProperty(arguments)
 
     @pyaedt_function_handler()
     def delete(self):
         """Delete the mesh.
 
         Returns
         -------
@@ -1352,15 +1351,15 @@
         moving_side_layers=1,
         static_side_layers=1,
     ):
         """Assign a cylindrical gap for a 2D or 3D design to enable a clone mesh and associated band mapping angle.
 
         Parameters
         ----------
-        obj : int or str or :class:`pyaedt.modeler.object3d.Object3d`
+        obj : int or str or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Object to assign cylindrical gap to.
         meshop_name : str, optional
             Name of the mesh. The default is ``None``, in which
             case the default name is used.
         clone_mesh : bool, optional
             Whether to clone the mesh. This parameter is valid only for 3D design.
             The default is ``False``. If ``True``, the solid bodies adjacent to the band
```

### Comparing `pyaedt-0.6.82/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.85/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.85/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.85/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.85/pyaedt/modules/PostProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from pyaedt import is_ironpython
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.generic.constants import unit_converter
 
 # from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import check_and_download_file
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 import pyaedt.modules.report_templates as rt
 from pyaedt.modules.solutions import FieldPlot
 from pyaedt.modules.solutions import SolutionData
@@ -1876,15 +1875,15 @@
         """Model units.
 
         Returns
         -------
         str
            Model units, such as ``"mm"``.
         """
-        return _retry_ntimes(10, self.oeditor.GetModelUnits)
+        return self.oeditor.GetModelUnits()
 
     @property
     def post_osolution(self):
         """Solution.
 
         Returns
         -------
@@ -2468,33 +2467,29 @@
                 variation_dict.append(intrinsics)
                 variation_dict.append("Phase:=")
                 if phase:
                     variation_dict.append(phase)
                 else:
                     variation_dict.append("0deg")
         if not sample_points_file and not sample_points_lists:
-            _retry_ntimes(10, self.ofieldsreporter.CalculatorWrite, filename, ["Solution:=", solution], variation_dict)
+            self.ofieldsreporter.CalculatorWrite(filename, ["Solution:=", solution], variation_dict)
         elif sample_points_file:
-            _retry_ntimes(
-                10,
-                self.ofieldsreporter.ExportToFile,
+            self.ofieldsreporter.ExportToFile(
                 filename,
                 sample_points_file,
                 solution,
                 variation_dict,
                 export_with_sample_points,
             )
         else:
             sample_points_file = os.path.join(self._app.working_directory, "temp_points.pts")
             with open_file(sample_points_file, "w") as f:
                 for point in sample_points_lists:
                     f.write(" ".join([str(i) for i in point]) + "\n")
-            _retry_ntimes(
-                10,
-                self.ofieldsreporter.ExportToFile,
+            self.ofieldsreporter.ExportToFile(
                 filename,
                 sample_points_file,
                 solution,
                 variation_dict,
                 export_with_sample_points,
             )
 
@@ -3052,33 +3047,53 @@
         fileName,
         plotName,
         foldername,
         orientation="isometric",
         width=1920,
         height=1080,
         display_wireframe=True,
+        selections=None,
+        show_axis=True,
+        show_grid=True,
+        show_ruler=True,
+        show_region="Default",
     ):
         """Export a field plot and coordinate system to a JPG file.
 
         Parameters
         ----------
         fileName : str
             Full path and name to save the JPG file to.
         plotName : str
             Name of the plot.
         foldername : str
             Name of the folder plot.
-        orientation : str
-            Name of the orientation to apply.
-        width : int
-            Plot Width.
-        height : int
-            Plot Height.
-        display_wireframe : bool
-            Display wireframe.
+        orientation : str, optional
+            Name of the orientation to apply. The default is ``"isometric"``.
+        width : int, optional
+            Plot Width. The default is ``1920``.
+        height : int, optional
+            Plot Height. The default is ``1080``.
+        display_wireframe : bool, optional
+            Display wireframe. The default is ``True``.
+        selections : list, optional
+            List of objects to include in the plot.
+             Supported in 3D Field Plots only starting from 23R1.
+        show_axis : bool, optional
+            Whether to show the axes. The default is ``True``.
+            Supported in 3D Field Plots only starting from 23R1.
+        show_grid : bool, optional
+            Whether to show the grid. The default is ``True``.
+            Supported in 3D Field Plots only starting from 23R1.
+        show_ruler : bool, optional
+            Whether to show the ruler. The default is ``True``.
+            Supported in 3D Field Plots only starting from 23R1.
+        show_region : bool, optional
+            Whether to show the region or not. The default is ``Default``.
+            Supported in 3D Field Plots only starting from 23R1.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
@@ -3104,15 +3119,24 @@
                 ]
                 view = orientation_to_view.get(orientation, "iso")
                 cs = self.modeler.create_coordinate_system(origin=center, mode="view", view=view)
                 self.ofieldsreporter.ExportPlotImageToFile(fileName, foldername, plotName, cs.name)
                 cs.delete()
             else:
                 self.export_model_picture(
-                    full_name=fileName, width=width, height=height, orientation=orientation, field_selections=plotName
+                    full_name=fileName,
+                    width=width,
+                    height=height,
+                    orientation=orientation,
+                    field_selections=plotName,
+                    selections=selections,
+                    show_axis=show_axis,
+                    show_grid=show_grid,
+                    show_ruler=show_ruler,
+                    show_region=show_region,
                 )
 
             for solid in wireframes:
                 self._primitives[solid].display_wireframe = False
         else:
             self.ofieldsreporter.ExportPlotImageWithViewToFile(
                 fileName, foldername, plotName, width, height, orientation
@@ -3206,18 +3230,24 @@
             selections = self.modeler.convert_to_selections(selections, False)
         else:
             selections = ""
         if not full_name:
             full_name = os.path.join(self._app.working_directory, generate_unique_name(self._app.design_name) + ".jpg")
 
         # open the 3D modeler and remove the selection on other objects
-        if self._app.design_type not in ["HFSS 3D Layout Design", "Circuit Design", "Maxwell Circuit", "Twin Builder"]:
-            self.oeditor.ShowWindow()
-            self.steal_focus_oneditor()
-        self.modeler.fit_all()
+        if not settings.non_graphical:
+            if self._app.design_type not in [
+                "HFSS 3D Layout Design",
+                "Circuit Design",
+                "Maxwell Circuit",
+                "Twin Builder",
+            ]:
+                self.oeditor.ShowWindow()
+                self.steal_focus_oneditor()
+            self.modeler.fit_all()
         # export the image
         if field_selections:
             if isinstance(field_selections, str):
                 if field_selections.lower() == "all":
                     field_selections = [""]
                 else:
                     field_selections = [field_selections]
@@ -3508,15 +3538,15 @@
             expression = expression.split(",")[0].split("(")[1]
             return value, expression
 
         if not available_bcs:
             self.logger.warning("No boundaries defined")
             return True
         for bc_obj in available_bcs:
-            if bc_obj.type == "Block":
+            if bc_obj.type == "Solid Block" or bc_obj.type == "Block":
                 n = len(bc_obj.props["Objects"])
                 if "Total Power Variation Data" not in bc_obj.props:
                     mult = 1
                     power_value = list(decompose_variable_value(bc_obj.props["Total Power"]))
                     power_value = unit_converter(
                         power_value[0], unit_system="Power", input_units=power_value[1], output_units=units
                     )
@@ -3770,21 +3800,21 @@
 
         if output_type == "boundary":
             for comp in power_dict.keys():
                 self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict[comp], 3)), units))
             self.logger.info("The total power is {} {}".format(str(round(sum(power_dict.values()), 3)), units))
             return power_dict, sum(power_dict.values())
 
-        elif output_type == "component":
+        elif output_type == "component":  # pragma: no cover
             for comp in power_dict_obj.keys():
                 self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict_obj[comp], 3)), units))
             self.logger.info("The total power is {} {}".format(str(round(sum(power_dict_obj.values()), 3)), units))
             return power_dict_obj, sum(power_dict_obj.values())
 
-        else:
+        else:  # pragma: no cover
             for comp in power_dict.keys():
                 self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict[comp], 3)), units))
             self.logger.info("The total power is {} {}".format(str(round(sum(power_dict.values()), 3)), units))
             for comp in power_dict_obj.keys():
                 self.logger.info("The power of {} is {} {}".format(comp, str(round(power_dict_obj[comp], 3)), units))
             self.logger.info("The total power is {} {}".format(str(round(sum(power_dict_obj.values()), 3)), units))
             return power_dict_obj, sum(power_dict_obj.values()), power_dict, sum(power_dict.values())
```

### Comparing `pyaedt-0.6.82/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.85/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.85/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.85/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.85/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/report_templates.py` & `pyaedt-0.6.85/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/modules/solutions.py` & `pyaedt-0.6.85/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/q3d.py` & `pyaedt-0.6.85/pyaedt/q3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1444,15 +1444,15 @@
         new_nets = [i for i in self.nets if i not in original_nets]
         for net in new_nets:
             objects = self.modeler.convert_to_selections(
                 [int(i) for i in list(self.oboundary.GetExcitationAssignment(net))], True
             )
             props = OrderedDict({"Objects": objects})
             bound = BoundaryObject(self, net, props, "SignalNet")
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
         if new_nets:
             self.logger.info("{} Nets have been identified: {}".format(len(new_nets), ", ".join(new_nets)))
         else:
             self.logger.info("No new nets identified")
         return True
 
     @pyaedt_function_handler()
@@ -1497,27 +1497,27 @@
         type_bound = "SignalNet"
         if net_type.lower() == "ground":
             type_bound = "GroundNet"
         elif net_type.lower() == "floating":
             type_bound = "FloatingNet"
         bound = BoundaryObject(self, net_name, props, type_bound)
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def source(self, objects=None, axisdir=0, name=None, net_name=None, terminal_type="voltage"):
         """Generate a source on a face of an object or a group of faces or face ids.
         The face ID is selected based on the axis direction. It is the face that
         has the maximum/minimum in this axis direction.
 
         Parameters
         ----------
-        objects : str, int or list or :class:`pyaedt.modeler.object3d.Object3d`
+        objects : str, int or list or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Name of the object or face ID or face ID list.
         axisdir : int, optional
             Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
         name : str, optional
             Name of the source. The default is ``None``.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
@@ -1541,15 +1541,15 @@
         """Generate a sink on a face of an object or a group of faces or face ids.
 
         The face ID is selected based on the axis direction. It is the face that
         has the maximum/minimum in this axis direction.
 
         Parameters
         ----------
-        objects : str, int or list or :class:`pyaedt.modeler.object3d.Object3d`
+        objects : str, int or list or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Name of the object or face ID or face ID list.
         axisdir : int, optional
             Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
         name : str, optional
             Name of the source. The default is ``None``.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
@@ -1599,15 +1599,15 @@
             terminal_str = "ConstantVoltage"
 
         props["TerminalType"] = terminal_str
         if net_name:
             props["Net"] = net_name
         bound = BoundaryObject(self, name, props, exc_type)
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_source_to_objectface(self, object_name, axisdir=0, source_name=None, net_name=None):
         """Generate a source on a face of an object.
 
@@ -1716,15 +1716,15 @@
             net_name = object_name
         if a:
             props = OrderedDict(
                 {"Faces": [a], "ParentBndID": object_name, "TerminalType": "ConstantVoltage", "Net": net_name}
             )
             bound = BoundaryObject(self, sink_name, props, "Sink")
             if bound.create():
-                self.boundaries.append(bound)
+                self._boundaries[bound.name] = bound
                 return bound
         return False
 
     @pyaedt_function_handler()
     def assign_sink_to_sheet(self, sheetname, objectname=None, netname=None, sinkname=None, terminal_type="voltage"):
         """Generate a sink on a sheet.
 
@@ -1769,15 +1769,15 @@
         props["TerminalType"] = terminal_str
 
         if netname:
             props["Net"] = netname
 
         bound = BoundaryObject(self, sinkname, props, "Sink")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def create_frequency_sweep(self, setupname, units, freqstart, freqstop, freqstep=None, sweepname=None):
         """Create a frequency sweep.
 
@@ -2129,15 +2129,15 @@
             the default name is assigned.
         matname : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is used.
 
         Returns
         -------
-        :class:`pyaedt.modeler.object3d.Object3d`
+        :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateRectangle
         """
@@ -2237,15 +2237,15 @@
                 t_list.append(t_obj.faces[0].area / perimeter)
             thickness = sum(t_list) / len(t_list)
 
         props = OrderedDict({"Objects": obj_names, "SolveOption": solve_option, "Thickness": str(thickness) + unit})
 
         bound = BoundaryObject(self, name, props, conductor_type)
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_huray_finitecond_to_edges(self, edges, radius, ratio, unit="um", name=""):
         """
         Assign the Huray surface roughness model to edges.
@@ -2280,15 +2280,15 @@
 
         a = self.modeler.convert_to_selections(edges, True)
 
         props = OrderedDict({"Edges": a, "UseCoating": False, "Radius": ra, "Ratio": str(ratio)})
 
         bound = BoundaryObject(self, name, props, "Finite Conductivity")
         if bound.create():
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def auto_assign_conductors(self):
         """Automatically assign conductors to signal lines.
 
@@ -2303,15 +2303,15 @@
         i = 0
         while i < len(new_nets):
             objects = self.modeler.convert_to_selections(
                 [int(k) for k in list(self.oboundary.GetExcitationAssignment(new_nets[i]))], True
             )
             props = OrderedDict({"Objects": objects})
             bound = BoundaryObject(self, new_nets[i], props, new_nets[i + 1])
-            self.boundaries.append(bound)
+            self._boundaries[bound.name] = bound
             i += 2
         if new_nets:
             self.logger.info("{} Nets have been identified: {}".format(len(new_nets), ", ".join(new_nets)))
         else:
             self.logger.info("No new nets identified")
         return True
```

### Comparing `pyaedt-0.6.82/pyaedt/rmxprt.py` & `pyaedt-0.6.85/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.85/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.85/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.85/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.85/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.85/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/siwave.py` & `pyaedt-0.6.85/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyaedt/twinbuilder.py` & `pyaedt-0.6.85/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.82/pyproject.toml` & `pyaedt-0.6.85/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,54 +34,54 @@
 ]
 
 [project.optional-dependencies]
 tests = [
     "ipython==8.13.0; python_version < '3.9'",
     "ipython==8.14.0; python_version >= '3.9'",
     "imageio==2.31.1",
-    "joblib==1.3.0",
+    "joblib==1.3.1",
     "matplotlib==3.5.3; python_version <= '3.7'",
-    "matplotlib==3.7.1; python_version > '3.7'",
+    "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
-    "numpy==1.25.0; python_version > '3.9'",
+    "numpy==1.25.1; python_version > '3.9'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==2.0.2; python_version > '3.7'",
+    "pandas==2.0.3; python_version > '3.7'",
     "pytest==7.4.0",
     "pytest-cov==4.1.0",
     "pytest-xdist==3.3.1",
-    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.40.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
-    "scikit-learn==1.2.2",
+    "scikit-learn==1.3.0",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
     "imageio==2.31.1",
     "imageio-ffmpeg==0.4.8",
     "ipython==8.13.0; python_version < '3.9'",
     "ipython==8.14.0; python_version >= '3.9'",
-    "ipywidgets==8.0.6",
-    "joblib==1.3.0",
-    "jupyterlab==4.0.2",
+    "ipywidgets==8.0.7",
+    "joblib==1.3.1",
+    "jupyterlab==4.0.3",
     "matplotlib==3.5.3; python_version <= '3.7'",
-    "matplotlib==3.7.1; python_version > '3.7'",
+    "matplotlib==3.7.2; python_version > '3.7'",
     "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.40.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "recommonmark==0.7.1",
-    "scikit-learn==1.2.2",
+    "scikit-learn==1.3.0",
     "Sphinx==7.0.1",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.3",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
@@ -89,37 +89,37 @@
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 full = [
     "imageio",
     "matplotlib==3.5.3; python_version <= '3.7'",
-    "matplotlib==3.7.1; python_version > '3.7'",
+    "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
-    "numpy==1.25.0; python_version > '3.9'",
+    "numpy==1.25.1; python_version > '3.9'",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==2.0.2; python_version > '3.7'",
+    "pandas==2.0.3; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.40.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
     "imageio",
     "matplotlib==3.5.3; python_version <= '3.7'",
-    "matplotlib==3.7.1; python_version > '3.7'",
+    "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
-    "numpy==1.25.0; python_version > '3.9'",
+    "numpy==1.25.1; python_version > '3.9'",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==2.0.2; python_version > '3.7'",
+    "pandas==2.0.3; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.40.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
```

### Comparing `pyaedt-0.6.82/PKG-INFO` & `pyaedt-0.6.85/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.82
+Version: 0.6.85
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -19,88 +19,88 @@
 Requires-Dist: pywin32 >= 303;platform_system=='Windows'
 Requires-Dist: pythonnet == 3.0.1
 Requires-Dist: rpyc==5.3.1
 Requires-Dist: psutil
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
 Requires-Dist: imageio ; extra == "all"
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
-Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: matplotlib==3.7.2 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.9')
-Requires-Dist: numpy==1.25.0 ; extra == "all" and ( python_version > '3.9')
+Requires-Dist: numpy==1.25.1 ; extra == "all" and ( python_version > '3.9')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
-Requires-Dist: pandas==2.0.2 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
-Requires-Dist: pyvista==0.39.1 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: imageio==2.31.1 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: ipython==8.13.0 ; extra == "doc" and ( python_version < '3.9')
 Requires-Dist: ipython==8.14.0 ; extra == "doc" and ( python_version >= '3.9')
-Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
-Requires-Dist: joblib==1.3.0 ; extra == "doc"
-Requires-Dist: jupyterlab==4.0.2 ; extra == "doc"
+Requires-Dist: ipywidgets==8.0.7 ; extra == "doc"
+Requires-Dist: joblib==1.3.1 ; extra == "doc"
+Requires-Dist: jupyterlab==4.0.3 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
-Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
+Requires-Dist: matplotlib==3.7.2 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.39.1 ; extra == "doc" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
-Requires-Dist: scikit-learn==1.2.2 ; extra == "doc"
+Requires-Dist: scikit-learn==1.3.0 ; extra == "doc"
 Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.3 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
 Requires-Dist: openpyxl==3.1.2 ; extra == "doc"
 Requires-Dist: imageio ; extra == "full"
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
-Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: matplotlib==3.7.2 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.9')
-Requires-Dist: numpy==1.25.0 ; extra == "full" and ( python_version > '3.9')
+Requires-Dist: numpy==1.25.1 ; extra == "full" and ( python_version > '3.9')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
-Requires-Dist: pandas==2.0.2 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
-Requires-Dist: pyvista==0.39.1 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests" and ( python_version < '3.9')
 Requires-Dist: ipython==8.14.0 ; extra == "tests" and ( python_version >= '3.9')
 Requires-Dist: imageio==2.31.1 ; extra == "tests"
-Requires-Dist: joblib==1.3.0 ; extra == "tests"
+Requires-Dist: joblib==1.3.1 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
-Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: matplotlib==3.7.2 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.9')
-Requires-Dist: numpy==1.25.0 ; extra == "tests" and ( python_version > '3.9')
+Requires-Dist: numpy==1.25.1 ; extra == "tests" and ( python_version > '3.9')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
-Requires-Dist: pandas==2.0.2 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
-Requires-Dist: pyvista==0.39.1 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
-Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
+Requires-Dist: scikit-learn==1.3.0 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
 Project-URL: Documentation, https://aedt.docs.pyansys.com
 Project-URL: Source Code, https://github.com/pyansys/pyaedt
 Provides-Extra: all
```

