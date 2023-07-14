# Comparing `tmp/types_usd-23.5.2.tar.gz` & `tmp/types_usd-23.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_usd-23.5.2.tar", max compression
+gzip compressed data, was "types_usd-23.5.3.tar", max compression
```

## Comparing `types_usd-23.5.2.tar` & `types_usd-23.5.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0     1377 2023-06-30 00:47:23.745223 types_usd-23.5.2/README.md
--rw-r--r--   0        0        0      920 2023-07-11 12:57:51.208750 types_usd-23.5.2/pyproject.toml
--rw-r--r--   0        0        0       49 2023-07-03 21:00:08.032287 types_usd-23.5.2/stubs/Boost-stubs/Python.pyi
--rw-r--r--   0        0        0        0 2023-07-03 21:00:08.027458 types_usd-23.5.2/stubs/Boost-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-07-11 17:00:39.585766 types_usd-23.5.2/stubs/Boost-stubs/py.typed
--rw-r--r--   0        0        0     6613 2023-07-11 17:00:15.168485 types_usd-23.5.2/stubs/pxr-stubs/Ar/__init__.pyi
--rw-r--r--   0        0        0     2619 2023-07-11 17:00:15.186085 types_usd-23.5.2/stubs/pxr-stubs/CameraUtil/__init__.pyi
--rw-r--r--   0        0        0      534 2023-07-11 17:00:15.191499 types_usd-23.5.2/stubs/pxr-stubs/Garch/__init__.pyi
--rw-r--r--   0        0        0     2456 2023-07-11 17:00:15.210352 types_usd-23.5.2/stubs/pxr-stubs/GeomUtil/__init__.pyi
--rw-r--r--   0        0        0   144855 2023-07-11 17:00:16.324020 types_usd-23.5.2/stubs/pxr-stubs/Gf/__init__.pyi
--rw-r--r--   0        0        0     2697 2023-07-11 17:00:16.345219 types_usd-23.5.2/stubs/pxr-stubs/Glf/__init__.pyi
--rw-r--r--   0        0        0     1128 2023-07-11 17:00:16.352405 types_usd-23.5.2/stubs/pxr-stubs/Kind/__init__.pyi
--rw-r--r--   0        0        0     9877 2023-07-11 17:00:16.430920 types_usd-23.5.2/stubs/pxr-stubs/Ndr/__init__.pyi
--rw-r--r--   0        0        0    16622 2023-07-11 17:00:16.535266 types_usd-23.5.2/stubs/pxr-stubs/Pcp/__init__.pyi
--rw-r--r--   0        0        0     4652 2023-07-11 17:00:16.571590 types_usd-23.5.2/stubs/pxr-stubs/Plug/__init__.pyi
--rw-r--r--   0        0        0     6559 2023-07-11 17:00:16.610438 types_usd-23.5.2/stubs/pxr-stubs/PxOsd/__init__.pyi
--rw-r--r--   0        0        0   107489 2023-07-11 17:00:17.325923 types_usd-23.5.2/stubs/pxr-stubs/Sdf/__init__.pyi
--rw-r--r--   0        0        0     7489 2023-07-11 17:00:17.369849 types_usd-23.5.2/stubs/pxr-stubs/Sdr/__init__.pyi
--rw-r--r--   0        0        0      450 2023-07-11 17:00:17.381338 types_usd-23.5.2/stubs/pxr-stubs/Sdr/shaderParserTestUtils.pyi
--rw-r--r--   0        0        0       55 2023-07-11 17:00:17.388826 types_usd-23.5.2/stubs/pxr-stubs/SdrGlslfx/__init__.pyi
--rw-r--r--   0        0        0    22462 2023-07-11 17:00:17.638202 types_usd-23.5.2/stubs/pxr-stubs/Tf/__init__.pyi
--rw-r--r--   0        0        0      393 2023-07-11 17:00:17.647646 types_usd-23.5.2/stubs/pxr-stubs/Tf/testenv/testTfPyInvoke_callees.pyi
--rw-r--r--   0        0        0       75 2023-07-11 17:00:17.649456 types_usd-23.5.2/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_DepLoadsAll.pyi
--rw-r--r--   0        0        0       75 2023-07-11 17:00:17.650920 types_usd-23.5.2/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsAll.pyi
--rw-r--r--   0        0        0      166 2023-07-11 17:00:17.655976 types_usd-23.5.2/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsUnknown.pyi
--rw-r--r--   0        0        0       75 2023-07-11 17:00:17.657271 types_usd-23.5.2/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Other.pyi
--rw-r--r--   0        0        0       55 2023-07-11 17:00:17.658420 types_usd-23.5.2/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Test.pyi
--rw-r--r--   0        0        0       75 2023-07-11 17:00:17.659096 types_usd-23.5.2/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Unknown.pyi
--rw-r--r--   0        0        0     2966 2023-07-11 17:00:17.694203 types_usd-23.5.2/stubs/pxr-stubs/Trace/__init__.pyi
--rw-r--r--   0        0        0    85508 2023-07-11 17:00:18.351855 types_usd-23.5.2/stubs/pxr-stubs/Usd/__init__.pyi
--rw-r--r--   0        0        0     1271 2023-07-11 17:00:18.361098 types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/__init__.pyi
--rw-r--r--   0        0        0      188 2023-07-11 17:00:18.362348 types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/cameraArgs.pyi
--rw-r--r--   0        0        0      140 2023-07-11 17:00:18.363430 types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/colorArgs.pyi
--rw-r--r--   0        0        0     1051 2023-07-11 17:00:18.367325 types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi
--rw-r--r--   0        0        0      727 2023-07-11 17:00:18.380343 types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi
--rw-r--r--   0        0        0      197 2023-07-11 17:00:18.381992 types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/rendererArgs.pyi
--rw-r--r--   0        0        0      390 2023-07-11 17:00:18.395859 types_usd-23.5.2/stubs/pxr-stubs/UsdBakeMtlx/__init__.pyi
--rw-r--r--   0        0        0    82312 2023-07-11 17:00:18.995949 types_usd-23.5.2/stubs/pxr-stubs/UsdGeom/__init__.pyi
--rw-r--r--   0        0        0     3413 2023-07-11 17:00:19.015987 types_usd-23.5.2/stubs/pxr-stubs/UsdHydra/__init__.pyi
--rw-r--r--   0        0        0     6025 2023-07-11 17:00:19.068652 types_usd-23.5.2/stubs/pxr-stubs/UsdImagingGL/__init__.pyi
--rw-r--r--   0        0        0    34853 2023-07-11 17:00:19.389513 types_usd-23.5.2/stubs/pxr-stubs/UsdLux/__init__.pyi
--rw-r--r--   0        0        0     5140 2023-07-11 17:00:19.462084 types_usd-23.5.2/stubs/pxr-stubs/UsdMedia/__init__.pyi
--rw-r--r--   0        0        0      257 2023-07-11 17:00:19.465744 types_usd-23.5.2/stubs/pxr-stubs/UsdMtlx/__init__.pyi
--rw-r--r--   0        0        0    29548 2023-07-11 17:00:19.702256 types_usd-23.5.2/stubs/pxr-stubs/UsdPhysics/__init__.pyi
--rw-r--r--   0        0        0     1325 2023-07-11 17:00:19.710870 types_usd-23.5.2/stubs/pxr-stubs/UsdProc/__init__.pyi
--rw-r--r--   0        0        0    10754 2023-07-11 17:00:19.782344 types_usd-23.5.2/stubs/pxr-stubs/UsdRender/__init__.pyi
--rw-r--r--   0        0        0      430 2023-07-11 17:00:19.793044 types_usd-23.5.2/stubs/pxr-stubs/UsdResolverExample/__init__.pyi
--rw-r--r--   0        0        0     8982 2023-07-11 17:00:19.854371 types_usd-23.5.2/stubs/pxr-stubs/UsdRi/__init__.pyi
--rw-r--r--   0        0        0     4020 2023-07-11 17:00:19.918881 types_usd-23.5.2/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi
--rw-r--r--   0        0        0    35536 2023-07-11 17:00:20.159478 types_usd-23.5.2/stubs/pxr-stubs/UsdShade/__init__.pyi
--rw-r--r--   0        0        0       55 2023-07-11 17:00:20.160311 types_usd-23.5.2/stubs/pxr-stubs/UsdShaders/__init__.pyi
--rw-r--r--   0        0        0    35473 2023-07-11 17:00:20.405443 types_usd-23.5.2/stubs/pxr-stubs/UsdSkel/__init__.pyi
--rw-r--r--   0        0        0     5304 2023-07-11 17:00:20.445081 types_usd-23.5.2/stubs/pxr-stubs/UsdUI/__init__.pyi
--rw-r--r--   0        0        0    11757 2023-07-11 17:00:20.511505 types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/__init__.pyi
--rw-r--r--   0        0        0     6341 2023-07-11 17:00:20.523130 types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi
--rw-r--r--   0        0        0      439 2023-07-11 17:00:20.526053 types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/constantsGroup.pyi
--rw-r--r--   0        0        0      353 2023-07-11 17:00:20.529337 types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/fixBrokenPixarSchemas.pyi
--rw-r--r--   0        0        0       84 2023-07-11 17:00:20.531065 types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/toolPaths.pyi
--rw-r--r--   0        0        0     2181 2023-07-11 17:00:20.542606 types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi
--rw-r--r--   0        0        0      698 2023-07-11 17:00:20.546712 types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi
--rw-r--r--   0        0        0     7462 2023-07-11 17:00:20.599621 types_usd-23.5.2/stubs/pxr-stubs/UsdVol/__init__.pyi
--rw-r--r--   0        0        0     6690 2023-07-11 17:00:20.638969 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/__init__.pyi
--rw-r--r--   0        0        0      621 2023-07-11 17:00:20.640551 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi
--rw-r--r--   0        0        0      193 2023-07-11 17:00:20.642109 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterialUI.pyi
--rw-r--r--   0        0        0     1041 2023-07-11 17:00:20.646923 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi
--rw-r--r--   0        0        0      178 2023-07-11 17:00:20.647905 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/adjustFreeCameraUI.pyi
--rw-r--r--   0        0        0    18577 2023-07-11 17:00:20.694571 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/appController.pyi
--rw-r--r--   0        0        0      666 2023-07-11 17:00:20.696792 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi
--rw-r--r--   0        0        0     2109 2023-07-11 17:00:20.702295 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi
--rw-r--r--   0        0        0      837 2023-07-11 17:00:20.703608 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi
--rw-r--r--   0        0        0      190 2023-07-11 17:00:20.705146 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/attributeValueEditorUI.pyi
--rw-r--r--   0        0        0     2005 2023-07-11 17:00:20.710095 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi
--rw-r--r--   0        0        0     8714 2023-07-11 17:00:20.738500 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/common.pyi
--rw-r--r--   0        0        0      303 2023-07-11 17:00:20.739915 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/configController.pyi
--rw-r--r--   0        0        0     1688 2023-07-11 17:00:20.743922 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/customAttributes.pyi
--rw-r--r--   0        0        0      645 2023-07-11 17:00:20.745728 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi
--rw-r--r--   0        0        0      540 2023-07-11 17:00:20.747629 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/frameSlider.pyi
--rw-r--r--   0        0        0     1878 2023-07-11 17:00:20.758564 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/freeCamera.pyi
--rw-r--r--   0        0        0      763 2023-07-11 17:00:20.761830 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi
--rw-r--r--   0        0        0     6226 2023-07-11 17:00:20.778171 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi
--rw-r--r--   0        0        0     1569 2023-07-11 17:00:20.781447 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi
--rw-r--r--   0        0        0      182 2023-07-11 17:00:20.782081 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/legendUtil.pyi
--rw-r--r--   0        0        0      523 2023-07-11 17:00:20.783357 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/mainWindowUI.pyi
--rw-r--r--   0        0        0      430 2023-07-11 17:00:20.785324 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/overridableLineEdit.pyi
--rw-r--r--   0        0        0     1468 2023-07-11 17:00:20.793590 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/plugin.pyi
--rw-r--r--   0        0        0      566 2023-07-11 17:00:20.794699 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/preferences.pyi
--rw-r--r--   0        0        0      163 2023-07-11 17:00:20.795700 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/preferencesUI.pyi
--rw-r--r--   0        0        0      117 2023-07-11 17:00:20.796714 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/prettyPrint.pyi
--rw-r--r--   0        0        0      392 2023-07-11 17:00:20.797621 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primContextMenu.pyi
--rw-r--r--   0        0        0     2652 2023-07-11 17:00:20.803052 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi
--rw-r--r--   0        0        0      662 2023-07-11 17:00:20.804669 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primLegend.pyi
--rw-r--r--   0        0        0      160 2023-07-11 17:00:20.806300 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primLegendUI.pyi
--rw-r--r--   0        0        0     3597 2023-07-11 17:00:20.814572 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi
--rw-r--r--   0        0        0     2130 2023-07-11 17:00:20.822966 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primViewItem.pyi
--rw-r--r--   0        0        0      694 2023-07-11 17:00:20.825066 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi
--rw-r--r--   0        0        0      172 2023-07-11 17:00:20.826689 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/propertyLegendUI.pyi
--rw-r--r--   0        0        0     3397 2023-07-11 17:00:20.835860 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi
--rw-r--r--   0        0        0      254 2023-07-11 17:00:20.837047 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/qt.pyi
--rw-r--r--   0        0        0     1331 2023-07-11 17:00:20.841213 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi
--rw-r--r--   0        0        0      266 2023-07-11 17:00:20.843009 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/scalarTypes.pyi
--rw-r--r--   0        0        0     5307 2023-07-11 17:00:20.879224 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi
--rw-r--r--   0        0        0     1389 2023-07-11 17:00:20.887548 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/settings.pyi
--rw-r--r--   0        0        0     7856 2023-07-11 17:00:20.908641 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/stageView.pyi
--rw-r--r--   0        0        0     1742 2023-07-11 17:00:20.914272 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi
--rw-r--r--   0        0        0      112 2023-07-11 17:00:20.916191 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/usdviewContextMenuItem.pyi
--rw-r--r--   0        0        0      421 2023-07-11 17:00:20.917906 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/variantComboBox.pyi
--rw-r--r--   0        0        0     3823 2023-07-11 17:00:20.930822 types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi
--rw-r--r--   0        0        0   275783 2023-07-11 17:00:22.980820 types_usd-23.5.2/stubs/pxr-stubs/Vt/__init__.pyi
--rw-r--r--   0        0        0      353 2023-07-11 17:00:22.984232 types_usd-23.5.2/stubs/pxr-stubs/Work/__init__.pyi
--rw-r--r--   0        0        0      684 2023-07-11 17:00:15.109426 types_usd-23.5.2/stubs/pxr-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-07-11 17:00:39.585678 types_usd-23.5.2/stubs/pxr-stubs/py.typed
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 types_usd-23.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1377 2023-06-30 00:47:23.745223 types_usd-23.5.3/README.md
+-rw-r--r--   0        0        0      920 2023-07-14 18:43:39.888953 types_usd-23.5.3/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-07-03 21:00:08.032287 types_usd-23.5.3/stubs/Boost-stubs/Python.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 21:00:08.027458 types_usd-23.5.3/stubs/Boost-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-14 16:35:26.124668 types_usd-23.5.3/stubs/Boost-stubs/py.typed
+-rw-r--r--   0        0        0     6613 2023-07-14 16:35:02.266845 types_usd-23.5.3/stubs/pxr-stubs/Ar/__init__.pyi
+-rw-r--r--   0        0        0     2619 2023-07-14 16:35:02.287079 types_usd-23.5.3/stubs/pxr-stubs/CameraUtil/__init__.pyi
+-rw-r--r--   0        0        0      534 2023-07-14 16:35:02.298597 types_usd-23.5.3/stubs/pxr-stubs/Garch/__init__.pyi
+-rw-r--r--   0        0        0     2456 2023-07-14 16:35:02.326763 types_usd-23.5.3/stubs/pxr-stubs/GeomUtil/__init__.pyi
+-rw-r--r--   0        0        0   144855 2023-07-14 16:35:03.347396 types_usd-23.5.3/stubs/pxr-stubs/Gf/__init__.pyi
+-rw-r--r--   0        0        0     2697 2023-07-14 16:35:03.367076 types_usd-23.5.3/stubs/pxr-stubs/Glf/__init__.pyi
+-rw-r--r--   0        0        0     1128 2023-07-14 16:35:03.373897 types_usd-23.5.3/stubs/pxr-stubs/Kind/__init__.pyi
+-rw-r--r--   0        0        0     9907 2023-07-14 16:35:03.443257 types_usd-23.5.3/stubs/pxr-stubs/Ndr/__init__.pyi
+-rw-r--r--   0        0        0    16670 2023-07-14 16:35:03.538694 types_usd-23.5.3/stubs/pxr-stubs/Pcp/__init__.pyi
+-rw-r--r--   0        0        0     4652 2023-07-14 16:35:03.570500 types_usd-23.5.3/stubs/pxr-stubs/Plug/__init__.pyi
+-rw-r--r--   0        0        0     6559 2023-07-14 16:35:03.604362 types_usd-23.5.3/stubs/pxr-stubs/PxOsd/__init__.pyi
+-rw-r--r--   0        0        0   107567 2023-07-14 16:35:04.188582 types_usd-23.5.3/stubs/pxr-stubs/Sdf/__init__.pyi
+-rw-r--r--   0        0        0     7530 2023-07-14 16:35:04.230095 types_usd-23.5.3/stubs/pxr-stubs/Sdr/__init__.pyi
+-rw-r--r--   0        0        0      450 2023-07-14 16:35:04.233532 types_usd-23.5.3/stubs/pxr-stubs/Sdr/shaderParserTestUtils.pyi
+-rw-r--r--   0        0        0       55 2023-07-14 16:35:04.234322 types_usd-23.5.3/stubs/pxr-stubs/SdrGlslfx/__init__.pyi
+-rw-r--r--   0        0        0    22450 2023-07-14 16:35:04.639939 types_usd-23.5.3/stubs/pxr-stubs/Tf/__init__.pyi
+-rw-r--r--   0        0        0      393 2023-07-14 16:35:04.643127 types_usd-23.5.3/stubs/pxr-stubs/Tf/testenv/testTfPyInvoke_callees.pyi
+-rw-r--r--   0        0        0       75 2023-07-14 16:35:04.644921 types_usd-23.5.3/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_DepLoadsAll.pyi
+-rw-r--r--   0        0        0       75 2023-07-14 16:35:04.646583 types_usd-23.5.3/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsAll.pyi
+-rw-r--r--   0        0        0      166 2023-07-14 16:35:04.649463 types_usd-23.5.3/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_LoadsUnknown.pyi
+-rw-r--r--   0        0        0       75 2023-07-14 16:35:04.650573 types_usd-23.5.3/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Other.pyi
+-rw-r--r--   0        0        0       55 2023-07-14 16:35:04.652208 types_usd-23.5.3/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Test.pyi
+-rw-r--r--   0        0        0       75 2023-07-14 16:35:04.652950 types_usd-23.5.3/stubs/pxr-stubs/Tf/testenv/testTfScriptModuleLoader_Unknown.pyi
+-rw-r--r--   0        0        0     2966 2023-07-14 16:35:04.686948 types_usd-23.5.3/stubs/pxr-stubs/Trace/__init__.pyi
+-rw-r--r--   0        0        0    85498 2023-07-14 16:35:05.458130 types_usd-23.5.3/stubs/pxr-stubs/Usd/__init__.pyi
+-rw-r--r--   0        0        0     1271 2023-07-14 16:35:05.467224 types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/__init__.pyi
+-rw-r--r--   0        0        0      188 2023-07-14 16:35:05.468502 types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/cameraArgs.pyi
+-rw-r--r--   0        0        0      140 2023-07-14 16:35:05.470156 types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/colorArgs.pyi
+-rw-r--r--   0        0        0     1051 2023-07-14 16:35:05.473715 types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi
+-rw-r--r--   0        0        0      727 2023-07-14 16:35:05.482450 types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi
+-rw-r--r--   0        0        0      197 2023-07-14 16:35:05.484118 types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/rendererArgs.pyi
+-rw-r--r--   0        0        0      390 2023-07-14 16:35:05.501035 types_usd-23.5.3/stubs/pxr-stubs/UsdBakeMtlx/__init__.pyi
+-rw-r--r--   0        0        0    82293 2023-07-14 16:35:06.088691 types_usd-23.5.3/stubs/pxr-stubs/UsdGeom/__init__.pyi
+-rw-r--r--   0        0        0     3413 2023-07-14 16:35:06.104966 types_usd-23.5.3/stubs/pxr-stubs/UsdHydra/__init__.pyi
+-rw-r--r--   0        0        0     6044 2023-07-14 16:35:06.142315 types_usd-23.5.3/stubs/pxr-stubs/UsdImagingGL/__init__.pyi
+-rw-r--r--   0        0        0    34853 2023-07-14 16:35:06.372321 types_usd-23.5.3/stubs/pxr-stubs/UsdLux/__init__.pyi
+-rw-r--r--   0        0        0     5140 2023-07-14 16:35:06.401589 types_usd-23.5.3/stubs/pxr-stubs/UsdMedia/__init__.pyi
+-rw-r--r--   0        0        0      257 2023-07-14 16:35:06.403254 types_usd-23.5.3/stubs/pxr-stubs/UsdMtlx/__init__.pyi
+-rw-r--r--   0        0        0    29548 2023-07-14 16:35:06.656534 types_usd-23.5.3/stubs/pxr-stubs/UsdPhysics/__init__.pyi
+-rw-r--r--   0        0        0     1325 2023-07-14 16:35:06.665256 types_usd-23.5.3/stubs/pxr-stubs/UsdProc/__init__.pyi
+-rw-r--r--   0        0        0    10754 2023-07-14 16:35:06.735895 types_usd-23.5.3/stubs/pxr-stubs/UsdRender/__init__.pyi
+-rw-r--r--   0        0        0      430 2023-07-14 16:35:06.745325 types_usd-23.5.3/stubs/pxr-stubs/UsdResolverExample/__init__.pyi
+-rw-r--r--   0        0        0     8982 2023-07-14 16:35:06.811375 types_usd-23.5.3/stubs/pxr-stubs/UsdRi/__init__.pyi
+-rw-r--r--   0        0        0     4020 2023-07-14 16:35:06.858371 types_usd-23.5.3/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi
+-rw-r--r--   0        0        0    35556 2023-07-14 16:35:07.082639 types_usd-23.5.3/stubs/pxr-stubs/UsdShade/__init__.pyi
+-rw-r--r--   0        0        0       55 2023-07-14 16:35:07.083364 types_usd-23.5.3/stubs/pxr-stubs/UsdShaders/__init__.pyi
+-rw-r--r--   0        0        0    35473 2023-07-14 16:35:07.304785 types_usd-23.5.3/stubs/pxr-stubs/UsdSkel/__init__.pyi
+-rw-r--r--   0        0        0     5304 2023-07-14 16:35:07.338657 types_usd-23.5.3/stubs/pxr-stubs/UsdUI/__init__.pyi
+-rw-r--r--   0        0        0    11767 2023-07-14 16:35:07.404153 types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/__init__.pyi
+-rw-r--r--   0        0        0     6341 2023-07-14 16:35:07.414052 types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi
+-rw-r--r--   0        0        0      439 2023-07-14 16:35:07.415842 types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/constantsGroup.pyi
+-rw-r--r--   0        0        0      353 2023-07-14 16:35:07.418761 types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/fixBrokenPixarSchemas.pyi
+-rw-r--r--   0        0        0       84 2023-07-14 16:35:07.420317 types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/toolPaths.pyi
+-rw-r--r--   0        0        0     2181 2023-07-14 16:35:07.429727 types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi
+-rw-r--r--   0        0        0      698 2023-07-14 16:35:07.433501 types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi
+-rw-r--r--   0        0        0     7462 2023-07-14 16:35:07.477401 types_usd-23.5.3/stubs/pxr-stubs/UsdVol/__init__.pyi
+-rw-r--r--   0        0        0     6690 2023-07-14 16:35:07.509229 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/__init__.pyi
+-rw-r--r--   0        0        0      621 2023-07-14 16:35:07.510412 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi
+-rw-r--r--   0        0        0      193 2023-07-14 16:35:07.511356 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterialUI.pyi
+-rw-r--r--   0        0        0     1041 2023-07-14 16:35:07.516015 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi
+-rw-r--r--   0        0        0      178 2023-07-14 16:35:07.517217 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/adjustFreeCameraUI.pyi
+-rw-r--r--   0        0        0    18577 2023-07-14 16:35:07.558364 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/appController.pyi
+-rw-r--r--   0        0        0      666 2023-07-14 16:35:07.560760 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi
+-rw-r--r--   0        0        0     2109 2023-07-14 16:35:07.565377 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi
+-rw-r--r--   0        0        0      837 2023-07-14 16:35:07.566765 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi
+-rw-r--r--   0        0        0      190 2023-07-14 16:35:07.567645 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/attributeValueEditorUI.pyi
+-rw-r--r--   0        0        0     2005 2023-07-14 16:35:07.570882 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi
+-rw-r--r--   0        0        0     8714 2023-07-14 16:35:07.593512 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/common.pyi
+-rw-r--r--   0        0        0      303 2023-07-14 16:35:07.594684 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/configController.pyi
+-rw-r--r--   0        0        0     1688 2023-07-14 16:35:07.598868 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/customAttributes.pyi
+-rw-r--r--   0        0        0      645 2023-07-14 16:35:07.600550 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi
+-rw-r--r--   0        0        0      540 2023-07-14 16:35:07.602138 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/frameSlider.pyi
+-rw-r--r--   0        0        0     1878 2023-07-14 16:35:07.609656 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/freeCamera.pyi
+-rw-r--r--   0        0        0      763 2023-07-14 16:35:07.611292 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi
+-rw-r--r--   0        0        0     6226 2023-07-14 16:35:07.622648 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi
+-rw-r--r--   0        0        0     1569 2023-07-14 16:35:07.625984 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi
+-rw-r--r--   0        0        0      182 2023-07-14 16:35:07.626683 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/legendUtil.pyi
+-rw-r--r--   0        0        0      523 2023-07-14 16:35:07.627882 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/mainWindowUI.pyi
+-rw-r--r--   0        0        0      430 2023-07-14 16:35:07.629739 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/overridableLineEdit.pyi
+-rw-r--r--   0        0        0     1468 2023-07-14 16:35:07.639821 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/plugin.pyi
+-rw-r--r--   0        0        0      566 2023-07-14 16:35:07.641508 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/preferences.pyi
+-rw-r--r--   0        0        0      163 2023-07-14 16:35:07.642881 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/preferencesUI.pyi
+-rw-r--r--   0        0        0      117 2023-07-14 16:35:07.644486 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/prettyPrint.pyi
+-rw-r--r--   0        0        0      392 2023-07-14 16:35:07.646136 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primContextMenu.pyi
+-rw-r--r--   0        0        0     2652 2023-07-14 16:35:07.653657 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi
+-rw-r--r--   0        0        0      662 2023-07-14 16:35:07.655076 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primLegend.pyi
+-rw-r--r--   0        0        0      160 2023-07-14 16:35:07.656597 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primLegendUI.pyi
+-rw-r--r--   0        0        0     3597 2023-07-14 16:35:07.666151 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi
+-rw-r--r--   0        0        0     2130 2023-07-14 16:35:07.670564 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primViewItem.pyi
+-rw-r--r--   0        0        0      694 2023-07-14 16:35:07.671809 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi
+-rw-r--r--   0        0        0      172 2023-07-14 16:35:07.672887 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/propertyLegendUI.pyi
+-rw-r--r--   0        0        0     3397 2023-07-14 16:35:07.681881 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi
+-rw-r--r--   0        0        0      254 2023-07-14 16:35:07.683865 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/qt.pyi
+-rw-r--r--   0        0        0     1331 2023-07-14 16:35:07.690284 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi
+-rw-r--r--   0        0        0      266 2023-07-14 16:35:07.693041 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/scalarTypes.pyi
+-rw-r--r--   0        0        0     5307 2023-07-14 16:35:07.725103 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi
+-rw-r--r--   0        0        0     1389 2023-07-14 16:35:07.734329 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/settings.pyi
+-rw-r--r--   0        0        0     7856 2023-07-14 16:35:07.760194 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/stageView.pyi
+-rw-r--r--   0        0        0     1742 2023-07-14 16:35:07.765419 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi
+-rw-r--r--   0        0        0      112 2023-07-14 16:35:07.766494 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/usdviewContextMenuItem.pyi
+-rw-r--r--   0        0        0      421 2023-07-14 16:35:07.767628 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/variantComboBox.pyi
+-rw-r--r--   0        0        0     3823 2023-07-14 16:35:07.776717 types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi
+-rw-r--r--   0        0        0   275783 2023-07-14 16:35:09.770154 types_usd-23.5.3/stubs/pxr-stubs/Vt/__init__.pyi
+-rw-r--r--   0        0        0      353 2023-07-14 16:35:09.772979 types_usd-23.5.3/stubs/pxr-stubs/Work/__init__.pyi
+-rw-r--r--   0        0        0      684 2023-07-14 16:35:02.195909 types_usd-23.5.3/stubs/pxr-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-14 16:35:26.124561 types_usd-23.5.3/stubs/pxr-stubs/py.typed
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 types_usd-23.5.3/PKG-INFO
```

### Comparing `types_usd-23.5.2/README.md` & `types_usd-23.5.3/README.md`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/pyproject.toml` & `types_usd-23.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "types-usd"
-version = "23.05.2"
+version = "23.05.3"
 
 readme = "README.md"
 authors = ["Chad Dombrova"]
 description = "Unofficial python stubs for Pixar's Universal Scene Description (USD)"
 license = "MIT"
 
 classifiers = [
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Ar/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Ar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/CameraUtil/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/CameraUtil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Garch/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Garch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/GeomUtil/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/GeomUtil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Gf/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Gf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Glf/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Glf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Kind/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Kind/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Ndr/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Ndr/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -135,17 +135,17 @@
     def IsConnectable(self) -> bool: ...
     def IsDynamicArray(self) -> bool: ...
     def IsOutput(self) -> bool: ...
 
 class Registry(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
     def GetAllNodeSourceTypes(self) -> list[str]: ...
-    def GetNodeByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ...) -> Node: ...
+    def GetNodeByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath, typePriority: typing.Iterable[str | pxr.Ar.ResolvedPath] = ...) -> Node: ...
     def GetNodeByIdentifierAndType(self, identifier: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath) -> Node: ...
-    def GetNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ..., filter: VersionFilter = ...) -> Node: ...
+    def GetNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: typing.Iterable[str | pxr.Ar.ResolvedPath] = ..., filter: VersionFilter = ...) -> Node: ...
     def GetNodeByNameAndType(self, name: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath, filter: VersionFilter = ...) -> Node: ...
     def GetNodeFromAsset(self, asset: pxr.Sdf.AssetPath | str, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ..., subIdentifier: str | pxr.Ar.ResolvedPath = ..., sourceType: str | pxr.Ar.ResolvedPath = ...) -> Node: ...
     def GetNodeFromSourceCode(self, sourceCode: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ...) -> Node: ...
     def GetNodeIdentifiers(self, family: str | pxr.Ar.ResolvedPath = ..., filter: VersionFilter = ...) -> list[str]: ...
     def GetNodeNames(self, family: str | pxr.Ar.ResolvedPath = ...) -> list[str]: ...
     def GetNodesByFamily(self, family: str | pxr.Ar.ResolvedPath = ..., filter: VersionFilter = ...) -> NodeList: ...
     def GetNodesByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath) -> NodeList: ...
@@ -212,11 +212,11 @@
     def __bool__(self) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
     def __lt__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     @property
     def expired(self) -> Any: ...
 
-def FsHelpersDiscoverFiles(searchPaths: list[str] | list[pxr.Ar.ResolvedPath], allowedExtensions: list[str] | list[pxr.Ar.ResolvedPath], followSymlinks: bool = ...) -> list: ...
-def FsHelpersDiscoverNodes(searchPaths: list[str] | list[pxr.Ar.ResolvedPath], allowedExtensions: list[str] | list[pxr.Ar.ResolvedPath], followSymlinks: bool = ..., context: DiscoveryPluginContext = ...) -> tuple[NodeDiscoveryResultVec, DiscoveryPluginContext]: ...
+def FsHelpersDiscoverFiles(searchPaths: typing.Iterable[str | pxr.Ar.ResolvedPath], allowedExtensions: typing.Iterable[str | pxr.Ar.ResolvedPath], followSymlinks: bool = ...) -> list: ...
+def FsHelpersDiscoverNodes(searchPaths: typing.Iterable[str | pxr.Ar.ResolvedPath], allowedExtensions: typing.Iterable[str | pxr.Ar.ResolvedPath], followSymlinks: bool = ..., context: DiscoveryPluginContext = ...) -> tuple[NodeDiscoveryResultVec, DiscoveryPluginContext]: ...
 def FsHelpersSplitShaderIdentifier(identifier: str | pxr.Ar.ResolvedPath) -> tuple[str, str, Version]: ...
 def _ValidateProperty(arg1: Node, arg2: Property) -> _AnnotatedBool: ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Pcp/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Pcp/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -215,33 +215,33 @@
     def __lt__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     @property
     def expired(self) -> Any: ...
     @property
     def identifier(self) -> LayerStackIdentifier: ...
     @property
-    def incrementalRelocatesSourceToTarget(self) -> pxr.Sdf.RelocatesMap: ...
+    def incrementalRelocatesSourceToTarget(self) -> dict[pxr.Sdf.Path, pxr.Sdf.Path]: ...
     @property
-    def incrementalRelocatesTargetToSource(self) -> pxr.Sdf.RelocatesMap: ...
+    def incrementalRelocatesTargetToSource(self) -> dict[pxr.Sdf.Path, pxr.Sdf.Path]: ...
     @property
     def layerOffsets(self) -> Any: ...
     @property
     def layerTree(self) -> pxr.Sdf.LayerTree: ...
     @property
     def layers(self) -> list[pxr.Sdf.Layer]: ...
     @property
     def localErrors(self) -> list[Error]: ...
     @property
     def mutedLayers(self) -> list[str]: ...
     @property
     def pathsToPrimsWithRelocates(self) -> list[pxr.Sdf.Path]: ...
     @property
-    def relocatesSourceToTarget(self) -> pxr.Sdf.RelocatesMap: ...
+    def relocatesSourceToTarget(self) -> dict[pxr.Sdf.Path, pxr.Sdf.Path]: ...
     @property
-    def relocatesTargetToSource(self) -> pxr.Sdf.RelocatesMap: ...
+    def relocatesTargetToSource(self) -> dict[pxr.Sdf.Path, pxr.Sdf.Path]: ...
 
 class LayerStackIdentifier(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
     @overload
     def __init__(self, rootLayer: pxr.Sdf.Layer, sessionLayer: pxr.Sdf.Layer = ..., pathResolverContext: pxr.Ar.ResolverContext = ...) -> None: ...
     @overload
     def __init__(self) -> None: ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Plug/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Plug/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/PxOsd/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/PxOsd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Sdf/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Sdf/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
     @classmethod
     def FindAllFileFormatExtensions(cls) -> list[str]: ...
     @overload
     @classmethod
     def FindByExtension(cls, extension: str | pxr.Ar.ResolvedPath, target: str | pxr.Ar.ResolvedPath = ...) -> FileFormat: ...
     @overload
     @classmethod
-    def FindByExtension(cls, extension: str | pxr.Ar.ResolvedPath, args: FileFormatArguments) -> FileFormat: ...
+    def FindByExtension(cls, extension: str | pxr.Ar.ResolvedPath, args: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath]) -> FileFormat: ...
     @classmethod
     def FindById(cls, arg1: str | pxr.Ar.ResolvedPath) -> FileFormat: ...
     @classmethod
     def FormatSupportsEditing(cls, extension: str | pxr.Ar.ResolvedPath, target: str | pxr.Ar.ResolvedPath = ...) -> bool: ...
     @classmethod
     def FormatSupportsReading(cls, extension: str | pxr.Ar.ResolvedPath, target: str | pxr.Ar.ResolvedPath = ...) -> bool: ...
     @classmethod
@@ -593,15 +593,15 @@
     @overload
     @classmethod
     def CreateAnonymous(cls, tag: str | pxr.Ar.ResolvedPath, format: FileFormat, args: dict = ...) -> Layer: ...
     @overload
     @classmethod
     def CreateAnonymous(cls, tag: str | pxr.Ar.ResolvedPath = ..., args: dict = ...) -> Layer: ...
     @classmethod
-    def CreateIdentifier(cls, arg1: str | pxr.Ar.ResolvedPath, arg2: FileFormatArguments) -> str: ...
+    def CreateIdentifier(cls, arg1: str | pxr.Ar.ResolvedPath, arg2: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath]) -> str: ...
     @classmethod
     def CreateNew(cls, identifier: object, args: dict = ...) -> Layer: ...
     @classmethod
     def DumpLayerInfo(cls) -> None: ...
     def EraseTimeSample(self, arg2: Path | str, arg3: float) -> None: ...
     def Export(self, filename: str | pxr.Ar.ResolvedPath, comment: str | pxr.Ar.ResolvedPath = ..., args: dict = ...) -> bool: ...
     def ExportToString(self) -> str: ...
@@ -627,15 +627,15 @@
     def GetDetachedLayerRules(cls) -> Layer.DetachedLayerRules: ...
     def GetDisplayName(self) -> str: ...
     @classmethod
     def GetDisplayNameFromIdentifier(cls, arg1: str | pxr.Ar.ResolvedPath) -> str: ...
     def GetExternalAssetDependencies(self) -> list[str]: ...
     def GetExternalReferences(self) -> tuple: ...
     def GetFileFormat(self) -> FileFormat: ...
-    def GetFileFormatArguments(self) -> FileFormatArguments: ...
+    def GetFileFormatArguments(self) -> dict[str, str]: ...
     @classmethod
     def GetLoadedLayers(cls) -> list[Layer]: ...
     @classmethod
     def GetMutedLayers(cls) -> list[str]: ...
     def GetNumTimeSamplesForPath(self, arg2: Path | str) -> int: ...
     def GetObjectAtPath(self, arg2: Path | str) -> Spec: ...
     def GetPrimAtPath(self, arg2: Path | str) -> PrimSpec: ...
@@ -1411,15 +1411,15 @@
     @classmethod
     def FindPrefixedRange(cls, arg2: Path | str) -> Any: ...
     def GetAbsoluteRootOrPrimPath(self) -> Path: ...
     def GetAllTargetPathsRecursively(self) -> list: ...
     def GetAncestorsRange(self) -> AncestorsRange: ...
     def GetCommonPrefix(self, arg2: Path | str) -> Path: ...
     @classmethod
-    def GetConciseRelativePaths(cls, arg1: list[Path] | list[str]) -> list[Path]: ...
+    def GetConciseRelativePaths(cls, arg1: typing.Iterable[Path | str]) -> list[Path]: ...
     def GetParentPath(self) -> Path: ...
     def GetPrefixes(self) -> list: ...
     def GetPrimOrPrimVariantSelectionPath(self) -> Path: ...
     def GetPrimPath(self) -> Path: ...
     def GetVariantSelection(self) -> tuple: ...
     def HasPrefix(self, arg2: Path | str) -> bool: ...
     def IsAbsolutePath(self) -> bool: ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Sdr/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Sdr/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # mypy: disable-error-code="misc, override, no-redef"
 
 import Boost.Python
 import pxr.Ar
 import pxr.Ndr
 import pxr.Sdf
+import typing
 from typing import Any, ClassVar
 
 __MFB_FULL_PACKAGE_NAME: str
 
 class NodeContext(Boost.Python.instance):
     Displacement: ClassVar[str] = ...  # read-only
     Light: ClassVar[str] = ...  # read-only
@@ -81,17 +82,17 @@
     Unknown: ClassVar[str] = ...  # read-only
     Vector: ClassVar[str] = ...  # read-only
     Vstruct: ClassVar[str] = ...  # read-only
     def __init__(self, *args, **kwargs) -> None: ...
 
 class Registry(pxr.Ndr.Registry):
     def __init__(self) -> None: ...
-    def GetShaderNodeByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ...) -> ShaderNode: ...
+    def GetShaderNodeByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath, typePriority: typing.Iterable[str | pxr.Ar.ResolvedPath] = ...) -> ShaderNode: ...
     def GetShaderNodeByIdentifierAndType(self, identifier: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath) -> ShaderNode: ...
-    def GetShaderNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: list[str] | list[pxr.Ar.ResolvedPath] = ..., filter: pxr.Ndr.VersionFilter = ...) -> ShaderNode: ...
+    def GetShaderNodeByName(self, name: str | pxr.Ar.ResolvedPath, typePriority: typing.Iterable[str | pxr.Ar.ResolvedPath] = ..., filter: pxr.Ndr.VersionFilter = ...) -> ShaderNode: ...
     def GetShaderNodeByNameAndType(self, name: str | pxr.Ar.ResolvedPath, nodeType: str | pxr.Ar.ResolvedPath, filter: pxr.Ndr.VersionFilter = ...) -> ShaderNode: ...
     def GetShaderNodeFromAsset(self, shaderAsset: pxr.Sdf.AssetPath | str, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ..., subIdentifier: str | pxr.Ar.ResolvedPath = ..., sourceType: str | pxr.Ar.ResolvedPath = ...) -> ShaderNode: ...
     def GetShaderNodeFromSourceCode(self, sourceCode: str | pxr.Ar.ResolvedPath, sourceType: str | pxr.Ar.ResolvedPath, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath] = ...) -> ShaderNode: ...
     def GetShaderNodesByFamily(self, family: str | pxr.Ar.ResolvedPath = ..., filter: pxr.Ndr.VersionFilter = ...) -> ShaderNodeList: ...
     def GetShaderNodesByIdentifier(self, identifier: str | pxr.Ar.ResolvedPath) -> ShaderNodeList: ...
     def GetShaderNodesByName(self, name: str | pxr.Ar.ResolvedPath, filter: pxr.Ndr.VersionFilter = ...) -> ShaderNodeList: ...
     def __bool__(self) -> bool: ...
@@ -134,15 +135,15 @@
 class ShaderProperty(pxr.Ndr.Property):
     def __init__(self, *args, **kwargs) -> None: ...
     def GetDefaultValueAsSdfType(self) -> Any: ...
     def GetHelp(self) -> str: ...
     def GetHints(self) -> dict: ...
     def GetImplementationName(self) -> str: ...
     def GetLabel(self) -> str: ...
-    def GetOptions(self) -> list: ...
+    def GetOptions(self) -> list[tuple[str, str]]: ...
     def GetPage(self) -> str: ...
     def GetVStructConditionalExpr(self) -> str: ...
     def GetVStructMemberName(self) -> str: ...
     def GetVStructMemberOf(self) -> str: ...
     def GetValidConnectionTypes(self) -> list[str]: ...
     def GetWidget(self) -> str: ...
     def IsAssetIdentifier(self) -> bool: ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Tf/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Tf/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -214,19 +214,19 @@
     __instance_size__: ClassVar[int] = ...
     def __init__(self) -> None: ...
     def AddFrom(self, arg2: Stopwatch) -> None: ...
     def Reset(self) -> None: ...
     def Start(self) -> None: ...
     def Stop(self) -> None: ...
     @property
-    def microseconds(self) -> int64_t: ...
+    def microseconds(self) -> int: ...
     @property
-    def milliseconds(self) -> int64_t: ...
+    def milliseconds(self) -> int: ...
     @property
-    def nanoseconds(self) -> int64_t: ...
+    def nanoseconds(self) -> int: ...
     @property
     def sampleCount(self) -> int: ...
     @property
     def seconds(self) -> float: ...
 
 class TemplateString(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Trace/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Trace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usd/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usd/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def HasAuthoredValueOpinion(self) -> bool: ...
     def HasColorSpace(self) -> bool: ...
     def HasFallbackValue(self) -> bool: ...
     def HasValue(self) -> bool: ...
     def RemoveConnection(self, source: pxr.Sdf.Path | str) -> bool: ...
     def Set(self, value: object, time: TimeCode | float | pxr.Sdf.TimeCode = ...) -> bool: ...
     def SetColorSpace(self, arg2: str | pxr.Ar.ResolvedPath) -> None: ...
-    def SetConnections(self, sources: list[pxr.Sdf.Path] | list[str]) -> bool: ...
+    def SetConnections(self, sources: typing.Iterable[pxr.Sdf.Path | str]) -> bool: ...
     def SetTypeName(self, typeName: pxr.Sdf.ValueTypeName) -> bool: ...
     def SetVariability(self, variability: pxr.Sdf.Variability) -> bool: ...
     def ValueMightBeTimeVarying(self) -> bool: ...
 
 class AttributeQuery(Boost.Python.instance):
     @overload
     def __init__(self, prim: Prim, attributeName: object) -> None: ...
@@ -388,15 +388,15 @@
 class Inherits(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
     def AddInherit(self, primPath: pxr.Sdf.Path | str, position: ListPosition = ...) -> bool: ...
     def ClearInherits(self) -> bool: ...
     def GetAllDirectInherits(self) -> list[pxr.Sdf.Path]: ...
     def GetPrim(self) -> Prim: ...
     def RemoveInherit(self, primPath: pxr.Sdf.Path | str) -> bool: ...
-    def SetInherits(self, arg2: list[pxr.Sdf.Path] | list[str]) -> bool: ...
+    def SetInherits(self, arg2: typing.Iterable[pxr.Sdf.Path | str]) -> bool: ...
     def __bool__(self) -> bool: ...
 
 class InterpolationType(pxr.Tf.Tf_PyEnumWrapper):
     _baseName: ClassVar[str] = ...
     allValues: ClassVar[tuple] = ...
     def __init__(self, *args, **kwargs) -> None: ...
     def GetValueFromName(self, name: object) -> Any: ...
@@ -655,18 +655,18 @@
     def GetRelationships(self) -> list[Relationship]: ...
     def GetSpecializes(self) -> Specializes: ...
     def GetSpecifier(self) -> pxr.Sdf.Specifier: ...
     def GetTypeName(self) -> str: ...
     def GetVariantSet(self, arg2: str | pxr.Ar.ResolvedPath) -> VariantSet: ...
     def GetVariantSets(self) -> VariantSets: ...
     @overload
-    def GetVersionIfHasAPIInFamily(self, arg2: str | pxr.Ar.ResolvedPath, arg3: str | pxr.Ar.ResolvedPath) -> SchemaVersion: ...
+    def GetVersionIfHasAPIInFamily(self, arg2: str | pxr.Ar.ResolvedPath, arg3: str | pxr.Ar.ResolvedPath) -> int: ...
     @overload
-    def GetVersionIfHasAPIInFamily(self, arg2: str | pxr.Ar.ResolvedPath) -> SchemaVersion: ...
-    def GetVersionIfIsInFamily(self, arg2: str | pxr.Ar.ResolvedPath) -> SchemaVersion: ...
+    def GetVersionIfHasAPIInFamily(self, arg2: str | pxr.Ar.ResolvedPath) -> int: ...
+    def GetVersionIfIsInFamily(self, arg2: str | pxr.Ar.ResolvedPath) -> int: ...
     @overload
     def HasAPI(self, schemaFamily: object, schemaVersion: int, instanceName: object) -> bool: ...
     @overload
     def HasAPI(self, schemaType: pxr.Tf.Type, instanceName: object) -> bool: ...
     @overload
     def HasAPI(self, schemaIdentifier: object, instanceName: object) -> bool: ...
     @overload
@@ -948,15 +948,15 @@
     def __init__(self) -> None: ...
     def AddTarget(self, target: pxr.Sdf.Path | str, position: ListPosition = ...) -> bool: ...
     def ClearTargets(self, removeSpec: bool) -> bool: ...
     def GetForwardedTargets(self) -> list[pxr.Sdf.Path]: ...
     def GetTargets(self) -> list[pxr.Sdf.Path]: ...
     def HasAuthoredTargets(self) -> bool: ...
     def RemoveTarget(self, target: pxr.Sdf.Path | str) -> bool: ...
-    def SetTargets(self, targets: list[pxr.Sdf.Path] | list[str]) -> bool: ...
+    def SetTargets(self, targets: typing.Iterable[pxr.Sdf.Path | str]) -> bool: ...
 
 class ResolveInfo(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
     def __init__(self) -> None: ...
     def GetNode(self) -> pxr.Pcp.NodeRef: ...
     def GetSource(self) -> ResolveInfoSource: ...
     def ValueIsBlocked(self) -> bool: ...
@@ -1135,15 +1135,15 @@
 
 class Specializes(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
     def AddSpecialize(self, primPath: pxr.Sdf.Path | str, position: ListPosition = ...) -> bool: ...
     def ClearSpecializes(self) -> bool: ...
     def GetPrim(self) -> Prim: ...
     def RemoveSpecialize(self, primPath: pxr.Sdf.Path | str) -> bool: ...
-    def SetSpecializes(self, arg2: list[pxr.Sdf.Path] | list[str]) -> bool: ...
+    def SetSpecializes(self, arg2: typing.Iterable[pxr.Sdf.Path | str]) -> bool: ...
     def __bool__(self) -> bool: ...
 
 class Stage(Boost.Python.instance):
     class InitialLoadSet(pxr.Tf.Tf_PyEnumWrapper):
         _baseName: ClassVar[str] = ...
         allValues: ClassVar[tuple] = ...
         def __init__(self, *args, **kwargs) -> None: ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/complexityArgs.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdAppUtils/framesArgs.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdGeom/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdGeom/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 class BBoxCache(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
     def __init__(self, time: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode, includedPurposes: object, useExtentsHint: bool = ..., ignoreVisibility: bool = ...) -> None: ...
     def Clear(self) -> None: ...
     def ClearBaseTime(self) -> None: ...
     def ComputeLocalBound(self, prim: pxr.Usd.Prim) -> pxr.Gf.BBox3d: ...
     def ComputePointInstanceLocalBound(self, instancer: PointInstancer, instanceId: int) -> pxr.Gf.BBox3d: ...
-    def ComputePointInstanceLocalBounds(self, instancer: PointInstancer, instanceIds: int) -> tuple[int64_t, pxr.Gf.BBox3d]: ...
+    def ComputePointInstanceLocalBounds(self, instancer: PointInstancer, instanceIds: int) -> tuple[int, pxr.Gf.BBox3d]: ...
     def ComputePointInstanceRelativeBound(self, instancer: PointInstancer, instanceId: int, relativeToAncestorPrim: pxr.Usd.Prim) -> pxr.Gf.BBox3d: ...
-    def ComputePointInstanceRelativeBounds(self, instancer: PointInstancer, instanceIds: int, relativeToAncestorPrim: pxr.Usd.Prim) -> tuple[int64_t, pxr.Gf.BBox3d]: ...
+    def ComputePointInstanceRelativeBounds(self, instancer: PointInstancer, instanceIds: int, relativeToAncestorPrim: pxr.Usd.Prim) -> tuple[int, pxr.Gf.BBox3d]: ...
     def ComputePointInstanceUntransformedBound(self, instancer: PointInstancer, instanceId: int) -> pxr.Gf.BBox3d: ...
-    def ComputePointInstanceUntransformedBounds(self, instancer: PointInstancer, instanceIds: int) -> tuple[int64_t, pxr.Gf.BBox3d]: ...
+    def ComputePointInstanceUntransformedBounds(self, instancer: PointInstancer, instanceIds: int) -> tuple[int, pxr.Gf.BBox3d]: ...
     def ComputePointInstanceWorldBound(self, instancer: PointInstancer, instanceId: int) -> pxr.Gf.BBox3d: ...
-    def ComputePointInstanceWorldBounds(self, instancer: PointInstancer, instanceIds: int) -> tuple[int64_t, pxr.Gf.BBox3d]: ...
+    def ComputePointInstanceWorldBounds(self, instancer: PointInstancer, instanceIds: int) -> tuple[int, pxr.Gf.BBox3d]: ...
     def ComputeRelativeBound(self, prim: pxr.Usd.Prim, relativeRootPrim: pxr.Usd.Prim) -> pxr.Gf.BBox3d: ...
     @overload
     def ComputeUntransformedBound(self, prim: pxr.Usd.Prim, pathsToSkip: typing.Iterable[pxr.Sdf.Path | str], ctmOverrides: pxr.Tf.HashMap[pxr.Sdf.Path | str, pxr.Gf.Matrix4d, pxr.Sdf.Path.Hash]) -> pxr.Gf.BBox3d: ...
     @overload
     def ComputeUntransformedBound(self, prim: pxr.Usd.Prim) -> pxr.Gf.BBox3d: ...
     def ComputeWorldBound(self, prim: pxr.Usd.Prim) -> pxr.Gf.BBox3d: ...
     def ComputeWorldBoundWithOverrides(self, prim: pxr.Usd.Prim, pathsToSkip: typing.Iterable[pxr.Sdf.Path | str], primOverride: pxr.Gf.Matrix4d, ctmOverrides: pxr.Tf.HashMap[pxr.Sdf.Path | str, pxr.Gf.Matrix4d, pxr.Sdf.Path.Hash]) -> pxr.Gf.BBox3d: ...
@@ -47,15 +47,15 @@
     __instance_size__: ClassVar[int] = ...
     @overload
     def __init__(self, schemaObj: pxr.Usd.SchemaBase) -> None: ...
     @overload
     def __init__(self, prim: pxr.Usd.Prim) -> None: ...
     @overload
     def __init__(self) -> None: ...
-    def ComputeInterpolationForSize(self, arg2: int, arg3: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode) -> tuple[str, ComputeInterpolationInfo]: ...
+    def ComputeInterpolationForSize(self, arg2: int, arg3: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode) -> tuple[str, list[tuple[str, int]]]: ...
     def ComputeUniformDataSize(self, arg2: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode) -> int: ...
     def ComputeVaryingDataSize(self, arg2: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode) -> int: ...
     def ComputeVertexDataSize(self, arg2: pxr.Usd.TimeCode | float | pxr.Sdf.TimeCode) -> int: ...
     def CreateBasisAttr(self, defaultValue: Any = ..., writeSparsely: bool = ...) -> pxr.Usd.Attribute: ...
     def CreateTypeAttr(self, defaultValue: Any = ..., writeSparsely: bool = ...) -> pxr.Usd.Attribute: ...
     def CreateWrapAttr(self, defaultValue: Any = ..., writeSparsely: bool = ...) -> pxr.Usd.Attribute: ...
     @classmethod
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdHydra/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdHydra/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdImagingGL/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdImagingGL/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import Boost.Python
 import pxr.Ar
 import pxr.CameraUtil
 import pxr.Gf
 import pxr.Glf
 import pxr.Sdf
 import pxr.Usd
+import typing
 from typing import Any, ClassVar, overload
 
 ALL_INSTANCES: int
 __MFB_FULL_PACKAGE_NAME: str
 
 class CullStyle(Boost.Python.enum):
     CULL_STYLE_BACK: ClassVar[CullStyle] = ...
@@ -69,15 +70,15 @@
     def SetLightingState(self, arg2: object, arg3: pxr.Glf.SimpleMaterial, arg4: pxr.Gf.Vec4f | list[float] | tuple[float, float, float, float]) -> None: ...
     def SetOverrideWindowPolicy(self, arg2: tuple[bool, pxr.CameraUtil.ConformWindowPolicy]) -> None: ...
     def SetRenderBufferSize(self, arg2: pxr.Gf.Vec2i | list[int] | pxr.Gf.Size2 | tuple[int, int]) -> None: ...
     def SetRenderViewport(self, arg2: pxr.Gf.Vec4d | list[float] | tuple[float, float, float, float]) -> None: ...
     def SetRendererAov(self, arg2: str | pxr.Ar.ResolvedPath) -> bool: ...
     def SetRendererPlugin(self, arg2: str | pxr.Ar.ResolvedPath) -> bool: ...
     def SetRendererSetting(self, arg2: str | pxr.Ar.ResolvedPath, arg3: Any) -> None: ...
-    def SetSelected(self, arg2: list[pxr.Sdf.Path] | list[str]) -> None: ...
+    def SetSelected(self, arg2: typing.Iterable[pxr.Sdf.Path | str]) -> None: ...
     def SetSelectionColor(self, arg2: pxr.Gf.Vec4f | list[float] | tuple[float, float, float, float]) -> None: ...
     def SetWindowPolicy(self, arg2: pxr.CameraUtil.ConformWindowPolicy) -> None: ...
     def StopRenderer(self) -> bool: ...
     def TestIntersection(self, arg2: pxr.Gf.Matrix4d, arg3: pxr.Gf.Matrix4d, arg4: pxr.Usd.Prim, arg5: RenderParams) -> tuple: ...
 
 class RenderParams(Boost.Python.instance):
     __instance_size__: ClassVar[int] = ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdLux/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdLux/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdMedia/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdMedia/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdPhysics/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdPhysics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdProc/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdProc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdRender/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdRender/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdRi/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdRi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdSchemaExamples/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdShade/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdShade/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 class ShaderDefUtils(Boost.Python.instance):
     def __init__(self, *args, **kwargs) -> None: ...
     @classmethod
     def GetNodeDiscoveryResults(cls, shaderDef: Shader, sourceUri: str | pxr.Ar.ResolvedPath) -> list: ...
     @classmethod
     def GetPrimvarNamesMetadataString(cls, metadata: dict[str | pxr.Ar.ResolvedPath, str | pxr.Ar.ResolvedPath], shaderDef: ConnectableAPI) -> str: ...
     @classmethod
-    def GetShaderProperties(cls, shaderDef: ConnectableAPI) -> list: ...
+    def GetShaderProperties(cls, shaderDef: ConnectableAPI) -> list[[pxr.Ndr.Property]]: ...
 
 class Tokens(Boost.Python.instance):
     ConnectableAPI: ClassVar[str] = ...  # read-only
     CoordSysAPI: ClassVar[str] = ...  # read-only
     Material: ClassVar[str] = ...  # read-only
     MaterialBindingAPI: ClassVar[str] = ...  # read-only
     NodeDefAPI: ClassVar[str] = ...  # read-only
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdSkel/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdSkel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdUI/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdUI/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     pureOverCount: ClassVar[str] = ...  # read-only
     totalInstanceCount: ClassVar[str] = ...  # read-only
     totalPrimCount: ClassVar[str] = ...  # read-only
     untyped: ClassVar[str] = ...  # read-only
     usedLayerCount: ClassVar[str] = ...  # read-only
     def __init__(self, *args, **kwargs) -> None: ...
 
-def AuthorCollection(collectionName: str | pxr.Ar.ResolvedPath, usdPrim: pxr.Usd.Prim, pathsToInclude: list[pxr.Sdf.Path] | list[str], pathsToExclude: list[pxr.Sdf.Path] | list[str] = ...) -> pxr.Usd.CollectionAPI: ...
+def AuthorCollection(collectionName: str | pxr.Ar.ResolvedPath, usdPrim: pxr.Usd.Prim, pathsToInclude: typing.Iterable[pxr.Sdf.Path | str], pathsToExclude: typing.Iterable[pxr.Sdf.Path | str] = ...) -> pxr.Usd.CollectionAPI: ...
 def ComputeAllDependencies(assetPath: pxr.Sdf.AssetPath | str) -> tuple: ...
 def ComputeCollectionIncludesAndExcludes(includedRootPaths: typing.Iterable[pxr.Sdf.Path | str], usdStage: pxr.Usd.Stage, minInclusionRatio: float = ..., maxNumExcludesBelowInclude: int = ..., minIncludeExcludeCollectionSize: int = ..., pathsToIgnore: PathHashSet = ...) -> tuple[list[pxr.Sdf.Path], list[pxr.Sdf.Path]]: ...
 @overload
 def ComputeUsdStageStats(arg1: str | pxr.Ar.ResolvedPath) -> tuple[pxr.Usd.Stage, dict]: ...
 @overload
 def ComputeUsdStageStats(arg1: pxr.Usd.Stage) -> tuple[int, dict]: ...
 def CopyLayerMetadata(source: pxr.Sdf.Layer, destination: pxr.Sdf.Layer, skipSublayers: bool = ..., bakeUnauthoredFallbacks: bool = ...) -> bool: ...
```

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/complianceChecker.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/updateSchemaWithSdrNode.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdUtils/usdzUtils.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/UsdVol/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/UsdVol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/adjustDefaultMaterial.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/adjustFreeCamera.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/appController.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/appController.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/appEventFilter.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/arrayAttributeView.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/attributeValueEditor.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/attributeViewContextMenu.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/common.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/common.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/customAttributes.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/customAttributes.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/debugFlagsWidget.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/frameSlider.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/frameSlider.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/freeCamera.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/freeCamera.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/headerContextMenu.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/hydraSceneBrowser.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/layerStackContextMenu.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/mainWindowUI.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/mainWindowUI.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/plugin.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/preferences.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/preferences.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primContextMenuItems.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primLegend.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primLegend.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primTreeWidget.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/primViewItem.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/primViewItem.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/propertyLegend.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/pythonInterpreter.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/rootDataModel.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/selectionDataModel.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/settings.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/settings.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/stageView.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/stageView.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/usdviewApi.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Usdviewq/viewSettingsDataModel.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/Vt/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/Vt/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/stubs/pxr-stubs/__init__.pyi` & `types_usd-23.5.3/stubs/pxr-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_usd-23.5.2/PKG-INFO` & `types_usd-23.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-usd
-Version: 23.5.2
+Version: 23.5.3
 Summary: Unofficial python stubs for Pixar's Universal Scene Description (USD)
 Home-page: https://github.com/LumaPictures/cg-stubs
 License: MIT
 Keywords: 3d,graphics,games,VFX,CG,animation
 Author: Chad Dombrova
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

