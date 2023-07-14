# Comparing `tmp/mypy-boto3-mediatailor-1.28.3.tar.gz` & `tmp/mypy-boto3-mediatailor-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediatailor-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
+gzip compressed data, was "mypy-boto3-mediatailor-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:02 2023, max compression
```

## Comparing `mypy-boto3-mediatailor-1.28.3.tar` & `mypy-boto3-mediatailor-1.28.3.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.205304 mypy-boto3-mediatailor-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-13 19:49:15.201304 mypy-boto3-mediatailor-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33557 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33498 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50479 2023-07-13 19:48:19.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50428 2023-07-13 19:48:18.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.201304 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.205304 mypy-boto3-mediatailor-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.967727 mypy-boto3-mediatailor-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20568 2023-07-14 16:18:02.963726 mypy-boto3-mediatailor-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.963726 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33957 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33898 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-14 16:16:51.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57550 2023-07-14 16:16:52.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57500 2023-07-14 16:16:51.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.963726 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20568 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:02.967727 mypy-boto3-mediatailor-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-mediatailor-1.28.3/LICENSE` & `mypy-boto3-mediatailor-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3/PKG-INFO` & `mypy-boto3-mediatailor-1.28.3.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.28.3
-Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,37 +364,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediatailor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediatailor.type_defs import (
+    SecretsManagerAccessTokenConfigurationOutputTypeDef,
     SecretsManagerAccessTokenConfigurationTypeDef,
+    KeyValuePairOutputTypeDef,
+    SlateSourceOutputTypeDef,
+    SpliceInsertMessageOutputTypeDef,
     KeyValuePairTypeDef,
     SlateSourceTypeDef,
     SpliceInsertMessageTypeDef,
+    AdMarkerPassthroughOutputTypeDef,
     AdMarkerPassthroughTypeDef,
-    AlertTypeDef,
+    AlertOutputTypeDef,
+    AvailMatchingCriteriaOutputTypeDef,
     AvailMatchingCriteriaTypeDef,
+    AvailSuppressionOutputTypeDef,
     AvailSuppressionTypeDef,
+    BumperOutputTypeDef,
     BumperTypeDef,
+    CdnConfigurationOutputTypeDef,
     CdnConfigurationTypeDef,
-    LogConfigurationForChannelTypeDef,
+    LogConfigurationForChannelOutputTypeDef,
+    ClipRangeOutputTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
+    ConfigureLogsForChannelResponseOutputTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
     HttpPackageConfigurationTypeDef,
+    HttpPackageConfigurationOutputTypeDef,
     PrefetchRetrievalTypeDef,
+    PrefetchRetrievalOutputTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
+    DefaultSegmentDeliveryConfigurationOutputTypeDef,
+    HttpConfigurationOutputTypeDef,
+    SegmentDeliveryConfigurationOutputTypeDef,
     DashConfigurationForPutTypeDef,
-    DashConfigurationTypeDef,
+    DashConfigurationOutputTypeDef,
+    DashPlaylistSettingsOutputTypeDef,
     DashPlaylistSettingsTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteLiveSourceRequestRequestTypeDef,
     DeletePlaybackConfigurationRequestRequestTypeDef,
     DeletePrefetchScheduleRequestRequestTypeDef,
     DeleteProgramRequestRequestTypeDef,
@@ -403,109 +419,117 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseTypeDef,
+    GetChannelPolicyResponseOutputTypeDef,
     GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
-    HlsConfigurationTypeDef,
-    LivePreRollConfigurationTypeDef,
-    LogConfigurationTypeDef,
+    HlsConfigurationOutputTypeDef,
+    LivePreRollConfigurationOutputTypeDef,
+    LogConfigurationOutputTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
+    HlsPlaylistSettingsOutputTypeDef,
     HlsPlaylistSettingsTypeDef,
     ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     ListLiveSourcesRequestRequestTypeDef,
     ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
     ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
+    LivePreRollConfigurationTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    ScheduleAdBreakTypeDef,
+    ScheduleAdBreakOutputTypeDef,
     TransitionTypeDef,
+    SegmentationDescriptorOutputTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
+    AccessConfigurationOutputTypeDef,
     AccessConfigurationTypeDef,
+    ManifestProcessingRulesOutputTypeDef,
     ManifestProcessingRulesTypeDef,
-    ListAlertsResponseTypeDef,
+    ListAlertsResponseOutputTypeDef,
+    PrefetchConsumptionOutputTypeDef,
     PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
-    CreateLiveSourceResponseTypeDef,
     CreateVodSourceRequestRequestTypeDef,
-    CreateVodSourceResponseTypeDef,
-    DescribeLiveSourceResponseTypeDef,
-    DescribeVodSourceResponseTypeDef,
-    LiveSourceTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
-    UpdateLiveSourceResponseTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
-    UpdateVodSourceResponseTypeDef,
-    VodSourceTypeDef,
+    CreateLiveSourceResponseOutputTypeDef,
+    CreateVodSourceResponseOutputTypeDef,
+    DescribeLiveSourceResponseOutputTypeDef,
+    DescribeVodSourceResponseOutputTypeDef,
+    LiveSourceOutputTypeDef,
+    UpdateLiveSourceResponseOutputTypeDef,
+    UpdateVodSourceResponseOutputTypeDef,
+    VodSourceOutputTypeDef,
+    ResponseOutputItemOutputTypeDef,
     RequestOutputItemTypeDef,
-    ResponseOutputItemTypeDef,
-    ScheduleEntryTypeDef,
+    ScheduleEntryOutputTypeDef,
     ScheduleConfigurationTypeDef,
+    TimeSignalMessageOutputTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
+    CreateSourceLocationResponseOutputTypeDef,
+    DescribeSourceLocationResponseOutputTypeDef,
+    SourceLocationOutputTypeDef,
+    UpdateSourceLocationResponseOutputTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
-    CreateSourceLocationResponseTypeDef,
-    DescribeSourceLocationResponseTypeDef,
-    SourceLocationTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
-    UpdateSourceLocationResponseTypeDef,
-    GetPlaybackConfigurationResponseTypeDef,
-    PlaybackConfigurationTypeDef,
+    GetPlaybackConfigurationResponseOutputTypeDef,
+    PlaybackConfigurationOutputTypeDef,
+    PutPlaybackConfigurationResponseOutputTypeDef,
     PutPlaybackConfigurationRequestRequestTypeDef,
-    PutPlaybackConfigurationResponseTypeDef,
+    CreatePrefetchScheduleResponseOutputTypeDef,
+    GetPrefetchScheduleResponseOutputTypeDef,
+    PrefetchScheduleOutputTypeDef,
     CreatePrefetchScheduleRequestRequestTypeDef,
-    CreatePrefetchScheduleResponseTypeDef,
-    GetPrefetchScheduleResponseTypeDef,
-    PrefetchScheduleTypeDef,
-    ListLiveSourcesResponseTypeDef,
-    ListVodSourcesResponseTypeDef,
+    ListLiveSourcesResponseOutputTypeDef,
+    ListVodSourcesResponseOutputTypeDef,
+    ChannelOutputTypeDef,
+    CreateChannelResponseOutputTypeDef,
+    DescribeChannelResponseOutputTypeDef,
+    UpdateChannelResponseOutputTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    ChannelTypeDef,
-    CreateChannelResponseTypeDef,
-    DescribeChannelResponseTypeDef,
-    UpdateChannelResponseTypeDef,
-    GetChannelScheduleResponseTypeDef,
+    GetChannelScheduleResponseOutputTypeDef,
+    AdBreakOutputTypeDef,
     AdBreakTypeDef,
-    ListSourceLocationsResponseTypeDef,
-    ListPlaybackConfigurationsResponseTypeDef,
-    ListPrefetchSchedulesResponseTypeDef,
-    ListChannelsResponseTypeDef,
+    ListSourceLocationsResponseOutputTypeDef,
+    ListPlaybackConfigurationsResponseOutputTypeDef,
+    ListPrefetchSchedulesResponseOutputTypeDef,
+    ListChannelsResponseOutputTypeDef,
+    CreateProgramResponseOutputTypeDef,
+    DescribeProgramResponseOutputTypeDef,
+    UpdateProgramResponseOutputTypeDef,
     CreateProgramRequestRequestTypeDef,
-    CreateProgramResponseTypeDef,
-    DescribeProgramResponseTypeDef,
     UpdateProgramRequestRequestTypeDef,
-    UpdateProgramResponseTypeDef,
 )
 
 
-def get_structure() -> SecretsManagerAccessTokenConfigurationTypeDef:
+def get_structure() -> SecretsManagerAccessTokenConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediatailor-1.28.3/README.md` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-mediatailor
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 mediatailor type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-mediatailor"></a>
 
 # mypy-boto3-mediatailor
 
 [![PyPI - mypy-boto3-mediatailor](https://img.shields.io/pypi/v/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
@@ -15,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,37 +364,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediatailor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediatailor.type_defs import (
+    SecretsManagerAccessTokenConfigurationOutputTypeDef,
     SecretsManagerAccessTokenConfigurationTypeDef,
+    KeyValuePairOutputTypeDef,
+    SlateSourceOutputTypeDef,
+    SpliceInsertMessageOutputTypeDef,
     KeyValuePairTypeDef,
     SlateSourceTypeDef,
     SpliceInsertMessageTypeDef,
+    AdMarkerPassthroughOutputTypeDef,
     AdMarkerPassthroughTypeDef,
-    AlertTypeDef,
+    AlertOutputTypeDef,
+    AvailMatchingCriteriaOutputTypeDef,
     AvailMatchingCriteriaTypeDef,
+    AvailSuppressionOutputTypeDef,
     AvailSuppressionTypeDef,
+    BumperOutputTypeDef,
     BumperTypeDef,
+    CdnConfigurationOutputTypeDef,
     CdnConfigurationTypeDef,
-    LogConfigurationForChannelTypeDef,
+    LogConfigurationForChannelOutputTypeDef,
+    ClipRangeOutputTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
+    ConfigureLogsForChannelResponseOutputTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
     HttpPackageConfigurationTypeDef,
+    HttpPackageConfigurationOutputTypeDef,
     PrefetchRetrievalTypeDef,
+    PrefetchRetrievalOutputTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
+    DefaultSegmentDeliveryConfigurationOutputTypeDef,
+    HttpConfigurationOutputTypeDef,
+    SegmentDeliveryConfigurationOutputTypeDef,
     DashConfigurationForPutTypeDef,
-    DashConfigurationTypeDef,
+    DashConfigurationOutputTypeDef,
+    DashPlaylistSettingsOutputTypeDef,
     DashPlaylistSettingsTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteLiveSourceRequestRequestTypeDef,
     DeletePlaybackConfigurationRequestRequestTypeDef,
     DeletePrefetchScheduleRequestRequestTypeDef,
     DeleteProgramRequestRequestTypeDef,
@@ -371,109 +419,117 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseTypeDef,
+    GetChannelPolicyResponseOutputTypeDef,
     GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
-    HlsConfigurationTypeDef,
-    LivePreRollConfigurationTypeDef,
-    LogConfigurationTypeDef,
+    HlsConfigurationOutputTypeDef,
+    LivePreRollConfigurationOutputTypeDef,
+    LogConfigurationOutputTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
+    HlsPlaylistSettingsOutputTypeDef,
     HlsPlaylistSettingsTypeDef,
     ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     ListLiveSourcesRequestRequestTypeDef,
     ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
     ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
+    LivePreRollConfigurationTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    ScheduleAdBreakTypeDef,
+    ScheduleAdBreakOutputTypeDef,
     TransitionTypeDef,
+    SegmentationDescriptorOutputTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
+    AccessConfigurationOutputTypeDef,
     AccessConfigurationTypeDef,
+    ManifestProcessingRulesOutputTypeDef,
     ManifestProcessingRulesTypeDef,
-    ListAlertsResponseTypeDef,
+    ListAlertsResponseOutputTypeDef,
+    PrefetchConsumptionOutputTypeDef,
     PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
-    CreateLiveSourceResponseTypeDef,
     CreateVodSourceRequestRequestTypeDef,
-    CreateVodSourceResponseTypeDef,
-    DescribeLiveSourceResponseTypeDef,
-    DescribeVodSourceResponseTypeDef,
-    LiveSourceTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
-    UpdateLiveSourceResponseTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
-    UpdateVodSourceResponseTypeDef,
-    VodSourceTypeDef,
+    CreateLiveSourceResponseOutputTypeDef,
+    CreateVodSourceResponseOutputTypeDef,
+    DescribeLiveSourceResponseOutputTypeDef,
+    DescribeVodSourceResponseOutputTypeDef,
+    LiveSourceOutputTypeDef,
+    UpdateLiveSourceResponseOutputTypeDef,
+    UpdateVodSourceResponseOutputTypeDef,
+    VodSourceOutputTypeDef,
+    ResponseOutputItemOutputTypeDef,
     RequestOutputItemTypeDef,
-    ResponseOutputItemTypeDef,
-    ScheduleEntryTypeDef,
+    ScheduleEntryOutputTypeDef,
     ScheduleConfigurationTypeDef,
+    TimeSignalMessageOutputTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
+    CreateSourceLocationResponseOutputTypeDef,
+    DescribeSourceLocationResponseOutputTypeDef,
+    SourceLocationOutputTypeDef,
+    UpdateSourceLocationResponseOutputTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
-    CreateSourceLocationResponseTypeDef,
-    DescribeSourceLocationResponseTypeDef,
-    SourceLocationTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
-    UpdateSourceLocationResponseTypeDef,
-    GetPlaybackConfigurationResponseTypeDef,
-    PlaybackConfigurationTypeDef,
+    GetPlaybackConfigurationResponseOutputTypeDef,
+    PlaybackConfigurationOutputTypeDef,
+    PutPlaybackConfigurationResponseOutputTypeDef,
     PutPlaybackConfigurationRequestRequestTypeDef,
-    PutPlaybackConfigurationResponseTypeDef,
+    CreatePrefetchScheduleResponseOutputTypeDef,
+    GetPrefetchScheduleResponseOutputTypeDef,
+    PrefetchScheduleOutputTypeDef,
     CreatePrefetchScheduleRequestRequestTypeDef,
-    CreatePrefetchScheduleResponseTypeDef,
-    GetPrefetchScheduleResponseTypeDef,
-    PrefetchScheduleTypeDef,
-    ListLiveSourcesResponseTypeDef,
-    ListVodSourcesResponseTypeDef,
+    ListLiveSourcesResponseOutputTypeDef,
+    ListVodSourcesResponseOutputTypeDef,
+    ChannelOutputTypeDef,
+    CreateChannelResponseOutputTypeDef,
+    DescribeChannelResponseOutputTypeDef,
+    UpdateChannelResponseOutputTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    ChannelTypeDef,
-    CreateChannelResponseTypeDef,
-    DescribeChannelResponseTypeDef,
-    UpdateChannelResponseTypeDef,
-    GetChannelScheduleResponseTypeDef,
+    GetChannelScheduleResponseOutputTypeDef,
+    AdBreakOutputTypeDef,
     AdBreakTypeDef,
-    ListSourceLocationsResponseTypeDef,
-    ListPlaybackConfigurationsResponseTypeDef,
-    ListPrefetchSchedulesResponseTypeDef,
-    ListChannelsResponseTypeDef,
+    ListSourceLocationsResponseOutputTypeDef,
+    ListPlaybackConfigurationsResponseOutputTypeDef,
+    ListPrefetchSchedulesResponseOutputTypeDef,
+    ListChannelsResponseOutputTypeDef,
+    CreateProgramResponseOutputTypeDef,
+    DescribeProgramResponseOutputTypeDef,
+    UpdateProgramResponseOutputTypeDef,
     CreateProgramRequestRequestTypeDef,
-    CreateProgramResponseTypeDef,
-    DescribeProgramResponseTypeDef,
     UpdateProgramRequestRequestTypeDef,
-    UpdateProgramResponseTypeDef,
 )
 
 
-def get_structure() -> SecretsManagerAccessTokenConfigurationTypeDef:
+def get_structure() -> SecretsManagerAccessTokenConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.py` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.pyi` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__main__.py` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaTailor 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.MediaTailor 1.28.3\nVersion:         1.28.3.post1\nBuilder"
+        " version: 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.3")
+    print("1.28.3.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.py` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,59 +31,59 @@
 )
 from .type_defs import (
     AccessConfigurationTypeDef,
     AdBreakTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    CreateLiveSourceResponseTypeDef,
-    CreatePrefetchScheduleResponseTypeDef,
-    CreateProgramResponseTypeDef,
-    CreateSourceLocationResponseTypeDef,
-    CreateVodSourceResponseTypeDef,
+    ConfigureLogsForChannelResponseOutputTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
+    CreateChannelResponseOutputTypeDef,
+    CreateLiveSourceResponseOutputTypeDef,
+    CreatePrefetchScheduleResponseOutputTypeDef,
+    CreateProgramResponseOutputTypeDef,
+    CreateSourceLocationResponseOutputTypeDef,
+    CreateVodSourceResponseOutputTypeDef,
     DashConfigurationForPutTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
-    DescribeChannelResponseTypeDef,
-    DescribeLiveSourceResponseTypeDef,
-    DescribeProgramResponseTypeDef,
-    DescribeSourceLocationResponseTypeDef,
-    DescribeVodSourceResponseTypeDef,
+    DescribeChannelResponseOutputTypeDef,
+    DescribeLiveSourceResponseOutputTypeDef,
+    DescribeProgramResponseOutputTypeDef,
+    DescribeSourceLocationResponseOutputTypeDef,
+    DescribeVodSourceResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetChannelPolicyResponseTypeDef,
-    GetChannelScheduleResponseTypeDef,
-    GetPlaybackConfigurationResponseTypeDef,
-    GetPrefetchScheduleResponseTypeDef,
+    GetChannelPolicyResponseOutputTypeDef,
+    GetChannelScheduleResponseOutputTypeDef,
+    GetPlaybackConfigurationResponseOutputTypeDef,
+    GetPrefetchScheduleResponseOutputTypeDef,
     HttpConfigurationTypeDef,
     HttpPackageConfigurationTypeDef,
-    ListAlertsResponseTypeDef,
-    ListChannelsResponseTypeDef,
-    ListLiveSourcesResponseTypeDef,
-    ListPlaybackConfigurationsResponseTypeDef,
-    ListPrefetchSchedulesResponseTypeDef,
-    ListSourceLocationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVodSourcesResponseTypeDef,
+    ListAlertsResponseOutputTypeDef,
+    ListChannelsResponseOutputTypeDef,
+    ListLiveSourcesResponseOutputTypeDef,
+    ListPlaybackConfigurationsResponseOutputTypeDef,
+    ListPrefetchSchedulesResponseOutputTypeDef,
+    ListSourceLocationsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListVodSourcesResponseOutputTypeDef,
     LivePreRollConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
     PrefetchConsumptionTypeDef,
     PrefetchRetrievalTypeDef,
-    PutPlaybackConfigurationResponseTypeDef,
+    PutPlaybackConfigurationResponseOutputTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
-    UpdateChannelResponseTypeDef,
-    UpdateLiveSourceResponseTypeDef,
-    UpdateProgramResponseTypeDef,
+    UpdateChannelResponseOutputTypeDef,
+    UpdateLiveSourceResponseOutputTypeDef,
+    UpdateProgramResponseOutputTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
-    UpdateSourceLocationResponseTypeDef,
-    UpdateVodSourceResponseTypeDef,
+    UpdateSourceLocationResponseOutputTypeDef,
+    UpdateVodSourceResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -135,25 +135,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#close)
         """
 
     def configure_logs_for_channel(
         self, *, ChannelName: str, LogTypes: Sequence[Literal["AS_RUN"]]
-    ) -> ConfigureLogsForChannelResponseTypeDef:
+    ) -> ConfigureLogsForChannelResponseOutputTypeDef:
         """
         Configures Amazon CloudWatch log settings for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_channel)
         """
 
     def configure_logs_for_playback_configuration(
         self, *, PercentEnabled: int, PlaybackConfigurationName: str
-    ) -> ConfigureLogsForPlaybackConfigurationResponseTypeDef:
+    ) -> ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef:
         """
         Amazon CloudWatch log settings for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_playback_configuration)
         """
 
@@ -162,30 +162,30 @@
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         PlaybackMode: PlaybackModeType,
         FillerSlate: SlateSourceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Tier: TierType = ...
-    ) -> CreateChannelResponseTypeDef:
+    ) -> CreateChannelResponseOutputTypeDef:
         """
         Creates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_channel)
         """
 
     def create_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateLiveSourceResponseTypeDef:
+    ) -> CreateLiveSourceResponseOutputTypeDef:
         """
         The live source configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_live_source)
         """
 
@@ -193,15 +193,15 @@
         self,
         *,
         Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
         Retrieval: PrefetchRetrievalTypeDef,
         StreamId: str = ...
-    ) -> CreatePrefetchScheduleResponseTypeDef:
+    ) -> CreatePrefetchScheduleResponseOutputTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_prefetch_schedule)
         """
 
@@ -211,15 +211,15 @@
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
         AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
         VodSourceName: str = ...
-    ) -> CreateProgramResponseTypeDef:
+    ) -> CreateProgramResponseOutputTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_program)
         """
 
@@ -228,30 +228,30 @@
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateSourceLocationResponseTypeDef:
+    ) -> CreateSourceLocationResponseOutputTypeDef:
         """
         Creates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_source_location)
         """
 
     def create_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVodSourceResponseTypeDef:
+    ) -> CreateVodSourceResponseOutputTypeDef:
         """
         The VOD source configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_vod_source)
         """
 
@@ -317,55 +317,55 @@
         """
         The video on demand (VOD) source to delete.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#delete_vod_source)
         """
 
-    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseTypeDef:
+    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseOutputTypeDef:
         """
         Describes a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_channel)
         """
 
     def describe_live_source(
         self, *, LiveSourceName: str, SourceLocationName: str
-    ) -> DescribeLiveSourceResponseTypeDef:
+    ) -> DescribeLiveSourceResponseOutputTypeDef:
         """
         The live source to describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_live_source)
         """
 
     def describe_program(
         self, *, ChannelName: str, ProgramName: str
-    ) -> DescribeProgramResponseTypeDef:
+    ) -> DescribeProgramResponseOutputTypeDef:
         """
         Describes a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_program)
         """
 
     def describe_source_location(
         self, *, SourceLocationName: str
-    ) -> DescribeSourceLocationResponseTypeDef:
+    ) -> DescribeSourceLocationResponseOutputTypeDef:
         """
         Describes a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_source_location)
         """
 
     def describe_vod_source(
         self, *, SourceLocationName: str, VodSourceName: str
-    ) -> DescribeVodSourceResponseTypeDef:
+    ) -> DescribeVodSourceResponseOutputTypeDef:
         """
         Provides details about a specific video on demand (VOD) source in a specific
         source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_vod_source)
         """
@@ -380,133 +380,137 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#generate_presigned_url)
         """
 
-    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseTypeDef:
+    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseOutputTypeDef:
         """
         Returns the channel's IAM policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_policy)
         """
 
     def get_channel_schedule(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> GetChannelScheduleResponseTypeDef:
+    ) -> GetChannelScheduleResponseOutputTypeDef:
         """
         Retrieves information about your channel's schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_schedule)
         """
 
-    def get_playback_configuration(self, *, Name: str) -> GetPlaybackConfigurationResponseTypeDef:
+    def get_playback_configuration(
+        self, *, Name: str
+    ) -> GetPlaybackConfigurationResponseOutputTypeDef:
         """
         Retrieves a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_playback_configuration)
         """
 
     def get_prefetch_schedule(
         self, *, Name: str, PlaybackConfigurationName: str
-    ) -> GetPrefetchScheduleResponseTypeDef:
+    ) -> GetPrefetchScheduleResponseOutputTypeDef:
         """
         Retrieves a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_prefetch_schedule)
         """
 
     def list_alerts(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAlertsResponseTypeDef:
+    ) -> ListAlertsResponseOutputTypeDef:
         """
         Lists the alerts that are associated with a MediaTailor channel assembly
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_alerts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_alerts)
         """
 
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListChannelsResponseTypeDef:
+    ) -> ListChannelsResponseOutputTypeDef:
         """
         Retrieves information about the channels that are associated with the current
         AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_channels)
         """
 
     def list_live_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListLiveSourcesResponseTypeDef:
+    ) -> ListLiveSourcesResponseOutputTypeDef:
         """
         Lists the live sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_live_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_live_sources)
         """
 
     def list_playback_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListPlaybackConfigurationsResponseTypeDef:
+    ) -> ListPlaybackConfigurationsResponseOutputTypeDef:
         """
         Retrieves existing playback configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_playback_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_playback_configurations)
         """
 
     def list_prefetch_schedules(
         self,
         *,
         PlaybackConfigurationName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         StreamId: str = ...
-    ) -> ListPrefetchSchedulesResponseTypeDef:
+    ) -> ListPrefetchSchedulesResponseOutputTypeDef:
         """
         Lists the prefetch schedules for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_prefetch_schedules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_prefetch_schedules)
         """
 
     def list_source_locations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListSourceLocationsResponseTypeDef:
+    ) -> ListSourceLocationsResponseOutputTypeDef:
         """
         Lists the source locations for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_source_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_source_locations)
         """
 
-    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, ResourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         A list of tags that are associated with this resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_tags_for_resource)
         """
 
     def list_vod_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListVodSourcesResponseTypeDef:
+    ) -> ListVodSourcesResponseOutputTypeDef:
         """
         Lists the VOD sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_vod_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_vod_sources)
         """
 
@@ -531,15 +535,15 @@
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
         VideoContentSourceUrl: str = ...
-    ) -> PutPlaybackConfigurationResponseTypeDef:
+    ) -> PutPlaybackConfigurationResponseOutputTypeDef:
         """
         Creates a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#put_playback_configuration)
         """
 
@@ -581,44 +585,44 @@
 
     def update_channel(
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         FillerSlate: SlateSourceTypeDef = ...
-    ) -> UpdateChannelResponseTypeDef:
+    ) -> UpdateChannelResponseOutputTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_channel)
         """
 
     def update_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str
-    ) -> UpdateLiveSourceResponseTypeDef:
+    ) -> UpdateLiveSourceResponseOutputTypeDef:
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_live_source)
         """
 
     def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
         AdBreaks: Sequence[AdBreakTypeDef] = ...
-    ) -> UpdateProgramResponseTypeDef:
+    ) -> UpdateProgramResponseOutputTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_program)
         """
 
@@ -626,29 +630,29 @@
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...
-    ) -> UpdateSourceLocationResponseTypeDef:
+    ) -> UpdateSourceLocationResponseOutputTypeDef:
         """
         Updates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_source_location)
         """
 
     def update_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str
-    ) -> UpdateVodSourceResponseTypeDef:
+    ) -> UpdateVodSourceResponseOutputTypeDef:
         """
         Updates a VOD source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_vod_source)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.pyi` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -31,59 +31,59 @@
 )
 from .type_defs import (
     AccessConfigurationTypeDef,
     AdBreakTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    CreateLiveSourceResponseTypeDef,
-    CreatePrefetchScheduleResponseTypeDef,
-    CreateProgramResponseTypeDef,
-    CreateSourceLocationResponseTypeDef,
-    CreateVodSourceResponseTypeDef,
+    ConfigureLogsForChannelResponseOutputTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
+    CreateChannelResponseOutputTypeDef,
+    CreateLiveSourceResponseOutputTypeDef,
+    CreatePrefetchScheduleResponseOutputTypeDef,
+    CreateProgramResponseOutputTypeDef,
+    CreateSourceLocationResponseOutputTypeDef,
+    CreateVodSourceResponseOutputTypeDef,
     DashConfigurationForPutTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
-    DescribeChannelResponseTypeDef,
-    DescribeLiveSourceResponseTypeDef,
-    DescribeProgramResponseTypeDef,
-    DescribeSourceLocationResponseTypeDef,
-    DescribeVodSourceResponseTypeDef,
+    DescribeChannelResponseOutputTypeDef,
+    DescribeLiveSourceResponseOutputTypeDef,
+    DescribeProgramResponseOutputTypeDef,
+    DescribeSourceLocationResponseOutputTypeDef,
+    DescribeVodSourceResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetChannelPolicyResponseTypeDef,
-    GetChannelScheduleResponseTypeDef,
-    GetPlaybackConfigurationResponseTypeDef,
-    GetPrefetchScheduleResponseTypeDef,
+    GetChannelPolicyResponseOutputTypeDef,
+    GetChannelScheduleResponseOutputTypeDef,
+    GetPlaybackConfigurationResponseOutputTypeDef,
+    GetPrefetchScheduleResponseOutputTypeDef,
     HttpConfigurationTypeDef,
     HttpPackageConfigurationTypeDef,
-    ListAlertsResponseTypeDef,
-    ListChannelsResponseTypeDef,
-    ListLiveSourcesResponseTypeDef,
-    ListPlaybackConfigurationsResponseTypeDef,
-    ListPrefetchSchedulesResponseTypeDef,
-    ListSourceLocationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVodSourcesResponseTypeDef,
+    ListAlertsResponseOutputTypeDef,
+    ListChannelsResponseOutputTypeDef,
+    ListLiveSourcesResponseOutputTypeDef,
+    ListPlaybackConfigurationsResponseOutputTypeDef,
+    ListPrefetchSchedulesResponseOutputTypeDef,
+    ListSourceLocationsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListVodSourcesResponseOutputTypeDef,
     LivePreRollConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
     PrefetchConsumptionTypeDef,
     PrefetchRetrievalTypeDef,
-    PutPlaybackConfigurationResponseTypeDef,
+    PutPlaybackConfigurationResponseOutputTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
-    UpdateChannelResponseTypeDef,
-    UpdateLiveSourceResponseTypeDef,
-    UpdateProgramResponseTypeDef,
+    UpdateChannelResponseOutputTypeDef,
+    UpdateLiveSourceResponseOutputTypeDef,
+    UpdateProgramResponseOutputTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
-    UpdateSourceLocationResponseTypeDef,
-    UpdateVodSourceResponseTypeDef,
+    UpdateSourceLocationResponseOutputTypeDef,
+    UpdateVodSourceResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -128,24 +128,24 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#close)
         """
     def configure_logs_for_channel(
         self, *, ChannelName: str, LogTypes: Sequence[Literal["AS_RUN"]]
-    ) -> ConfigureLogsForChannelResponseTypeDef:
+    ) -> ConfigureLogsForChannelResponseOutputTypeDef:
         """
         Configures Amazon CloudWatch log settings for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_channel)
         """
     def configure_logs_for_playback_configuration(
         self, *, PercentEnabled: int, PlaybackConfigurationName: str
-    ) -> ConfigureLogsForPlaybackConfigurationResponseTypeDef:
+    ) -> ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef:
         """
         Amazon CloudWatch log settings for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_playback_configuration)
         """
     def create_channel(
@@ -153,44 +153,44 @@
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         PlaybackMode: PlaybackModeType,
         FillerSlate: SlateSourceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Tier: TierType = ...
-    ) -> CreateChannelResponseTypeDef:
+    ) -> CreateChannelResponseOutputTypeDef:
         """
         Creates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_channel)
         """
     def create_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateLiveSourceResponseTypeDef:
+    ) -> CreateLiveSourceResponseOutputTypeDef:
         """
         The live source configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_live_source)
         """
     def create_prefetch_schedule(
         self,
         *,
         Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
         Retrieval: PrefetchRetrievalTypeDef,
         StreamId: str = ...
-    ) -> CreatePrefetchScheduleResponseTypeDef:
+    ) -> CreatePrefetchScheduleResponseOutputTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_prefetch_schedule)
         """
     def create_program(
@@ -199,15 +199,15 @@
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
         AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
         VodSourceName: str = ...
-    ) -> CreateProgramResponseTypeDef:
+    ) -> CreateProgramResponseOutputTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_program)
         """
     def create_source_location(
@@ -215,29 +215,29 @@
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateSourceLocationResponseTypeDef:
+    ) -> CreateSourceLocationResponseOutputTypeDef:
         """
         Creates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_source_location)
         """
     def create_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVodSourceResponseTypeDef:
+    ) -> CreateVodSourceResponseOutputTypeDef:
         """
         The VOD source configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_vod_source)
         """
     def delete_channel(self, *, ChannelName: str) -> Dict[str, Any]:
@@ -294,51 +294,51 @@
     def delete_vod_source(self, *, SourceLocationName: str, VodSourceName: str) -> Dict[str, Any]:
         """
         The video on demand (VOD) source to delete.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#delete_vod_source)
         """
-    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseTypeDef:
+    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseOutputTypeDef:
         """
         Describes a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_channel)
         """
     def describe_live_source(
         self, *, LiveSourceName: str, SourceLocationName: str
-    ) -> DescribeLiveSourceResponseTypeDef:
+    ) -> DescribeLiveSourceResponseOutputTypeDef:
         """
         The live source to describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_live_source)
         """
     def describe_program(
         self, *, ChannelName: str, ProgramName: str
-    ) -> DescribeProgramResponseTypeDef:
+    ) -> DescribeProgramResponseOutputTypeDef:
         """
         Describes a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_program)
         """
     def describe_source_location(
         self, *, SourceLocationName: str
-    ) -> DescribeSourceLocationResponseTypeDef:
+    ) -> DescribeSourceLocationResponseOutputTypeDef:
         """
         Describes a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_source_location)
         """
     def describe_vod_source(
         self, *, SourceLocationName: str, VodSourceName: str
-    ) -> DescribeVodSourceResponseTypeDef:
+    ) -> DescribeVodSourceResponseOutputTypeDef:
         """
         Provides details about a specific video on demand (VOD) source in a specific
         source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_vod_source)
         """
@@ -351,122 +351,126 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#generate_presigned_url)
         """
-    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseTypeDef:
+    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseOutputTypeDef:
         """
         Returns the channel's IAM policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_policy)
         """
     def get_channel_schedule(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> GetChannelScheduleResponseTypeDef:
+    ) -> GetChannelScheduleResponseOutputTypeDef:
         """
         Retrieves information about your channel's schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_schedule)
         """
-    def get_playback_configuration(self, *, Name: str) -> GetPlaybackConfigurationResponseTypeDef:
+    def get_playback_configuration(
+        self, *, Name: str
+    ) -> GetPlaybackConfigurationResponseOutputTypeDef:
         """
         Retrieves a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_playback_configuration)
         """
     def get_prefetch_schedule(
         self, *, Name: str, PlaybackConfigurationName: str
-    ) -> GetPrefetchScheduleResponseTypeDef:
+    ) -> GetPrefetchScheduleResponseOutputTypeDef:
         """
         Retrieves a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_prefetch_schedule)
         """
     def list_alerts(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAlertsResponseTypeDef:
+    ) -> ListAlertsResponseOutputTypeDef:
         """
         Lists the alerts that are associated with a MediaTailor channel assembly
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_alerts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_alerts)
         """
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListChannelsResponseTypeDef:
+    ) -> ListChannelsResponseOutputTypeDef:
         """
         Retrieves information about the channels that are associated with the current
         AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_channels)
         """
     def list_live_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListLiveSourcesResponseTypeDef:
+    ) -> ListLiveSourcesResponseOutputTypeDef:
         """
         Lists the live sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_live_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_live_sources)
         """
     def list_playback_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListPlaybackConfigurationsResponseTypeDef:
+    ) -> ListPlaybackConfigurationsResponseOutputTypeDef:
         """
         Retrieves existing playback configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_playback_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_playback_configurations)
         """
     def list_prefetch_schedules(
         self,
         *,
         PlaybackConfigurationName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         StreamId: str = ...
-    ) -> ListPrefetchSchedulesResponseTypeDef:
+    ) -> ListPrefetchSchedulesResponseOutputTypeDef:
         """
         Lists the prefetch schedules for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_prefetch_schedules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_prefetch_schedules)
         """
     def list_source_locations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListSourceLocationsResponseTypeDef:
+    ) -> ListSourceLocationsResponseOutputTypeDef:
         """
         Lists the source locations for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_source_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_source_locations)
         """
-    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, ResourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         A list of tags that are associated with this resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_tags_for_resource)
         """
     def list_vod_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListVodSourcesResponseTypeDef:
+    ) -> ListVodSourcesResponseOutputTypeDef:
         """
         Lists the VOD sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_vod_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_vod_sources)
         """
     def put_channel_policy(self, *, ChannelName: str, Policy: str) -> Dict[str, Any]:
@@ -489,15 +493,15 @@
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
         VideoContentSourceUrl: str = ...
-    ) -> PutPlaybackConfigurationResponseTypeDef:
+    ) -> PutPlaybackConfigurationResponseOutputTypeDef:
         """
         Creates a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#put_playback_configuration)
         """
     def start_channel(self, *, ChannelName: str) -> Dict[str, Any]:
@@ -534,70 +538,70 @@
         """
     def update_channel(
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         FillerSlate: SlateSourceTypeDef = ...
-    ) -> UpdateChannelResponseTypeDef:
+    ) -> UpdateChannelResponseOutputTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_channel)
         """
     def update_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str
-    ) -> UpdateLiveSourceResponseTypeDef:
+    ) -> UpdateLiveSourceResponseOutputTypeDef:
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_live_source)
         """
     def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
         AdBreaks: Sequence[AdBreakTypeDef] = ...
-    ) -> UpdateProgramResponseTypeDef:
+    ) -> UpdateProgramResponseOutputTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_program)
         """
     def update_source_location(
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...
-    ) -> UpdateSourceLocationResponseTypeDef:
+    ) -> UpdateSourceLocationResponseOutputTypeDef:
         """
         Updates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_source_location)
         """
     def update_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str
-    ) -> UpdateVodSourceResponseTypeDef:
+    ) -> UpdateVodSourceResponseOutputTypeDef:
         """
         Updates a VOD source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_vod_source)
         """
     @overload
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.py` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.pyi` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.py` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    GetChannelScheduleResponseTypeDef,
-    ListAlertsResponseTypeDef,
-    ListChannelsResponseTypeDef,
-    ListLiveSourcesResponseTypeDef,
-    ListPlaybackConfigurationsResponseTypeDef,
-    ListPrefetchSchedulesResponseTypeDef,
-    ListSourceLocationsResponseTypeDef,
-    ListVodSourcesResponseTypeDef,
+    GetChannelScheduleResponseOutputTypeDef,
+    ListAlertsResponseOutputTypeDef,
+    ListChannelsResponseOutputTypeDef,
+    ListLiveSourcesResponseOutputTypeDef,
+    ListPlaybackConfigurationsResponseOutputTypeDef,
+    ListPrefetchSchedulesResponseOutputTypeDef,
+    ListSourceLocationsResponseOutputTypeDef,
+    ListVodSourcesResponseOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "GetChannelSchedulePaginator",
     "ListAlertsPaginator",
     "ListChannelsPaginator",
@@ -79,75 +79,75 @@
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetChannelScheduleResponseTypeDef]:
+    ) -> _PageIterator[GetChannelScheduleResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
 
 class ListAlertsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAlertsResponseTypeDef]:
+    ) -> _PageIterator[ListAlertsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
         """
 
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListChannelsResponseTypeDef]:
+    ) -> _PageIterator[ListChannelsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
         """
 
 
 class ListLiveSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLiveSourcesResponseTypeDef]:
+    ) -> _PageIterator[ListLiveSourcesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
         """
 
 
 class ListPlaybackConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPlaybackConfigurationsResponseTypeDef]:
+    ) -> _PageIterator[ListPlaybackConfigurationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
         """
 
 
 class ListPrefetchSchedulesPaginator(Paginator):
@@ -158,42 +158,42 @@
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPrefetchSchedulesResponseTypeDef]:
+    ) -> _PageIterator[ListPrefetchSchedulesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
         """
 
 
 class ListSourceLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSourceLocationsResponseTypeDef]:
+    ) -> _PageIterator[ListSourceLocationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
         """
 
 
 class ListVodSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVodSourcesResponseTypeDef]:
+    ) -> _PageIterator[ListVodSourcesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.pyi` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    GetChannelScheduleResponseTypeDef,
-    ListAlertsResponseTypeDef,
-    ListChannelsResponseTypeDef,
-    ListLiveSourcesResponseTypeDef,
-    ListPlaybackConfigurationsResponseTypeDef,
-    ListPrefetchSchedulesResponseTypeDef,
-    ListSourceLocationsResponseTypeDef,
-    ListVodSourcesResponseTypeDef,
+    GetChannelScheduleResponseOutputTypeDef,
+    ListAlertsResponseOutputTypeDef,
+    ListChannelsResponseOutputTypeDef,
+    ListLiveSourcesResponseOutputTypeDef,
+    ListPlaybackConfigurationsResponseOutputTypeDef,
+    ListPrefetchSchedulesResponseOutputTypeDef,
+    ListSourceLocationsResponseOutputTypeDef,
+    ListVodSourcesResponseOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "GetChannelSchedulePaginator",
     "ListAlertsPaginator",
     "ListChannelsPaginator",
@@ -76,71 +76,71 @@
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetChannelScheduleResponseTypeDef]:
+    ) -> _PageIterator[GetChannelScheduleResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
 class ListAlertsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAlertsResponseTypeDef]:
+    ) -> _PageIterator[ListAlertsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
         """
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListChannelsResponseTypeDef]:
+    ) -> _PageIterator[ListChannelsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
         """
 
 class ListLiveSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLiveSourcesResponseTypeDef]:
+    ) -> _PageIterator[ListLiveSourcesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
         """
 
 class ListPlaybackConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPlaybackConfigurationsResponseTypeDef]:
+    ) -> _PageIterator[ListPlaybackConfigurationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
         """
 
 class ListPrefetchSchedulesPaginator(Paginator):
     """
@@ -150,40 +150,40 @@
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPrefetchSchedulesResponseTypeDef]:
+    ) -> _PageIterator[ListPrefetchSchedulesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
         """
 
 class ListSourceLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSourceLocationsResponseTypeDef]:
+    ) -> _PageIterator[ListSourceLocationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
         """
 
 class ListVodSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVodSourcesResponseTypeDef]:
+    ) -> _PageIterator[ListVodSourcesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.py` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediatailor service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediatailor.type_defs import SecretsManagerAccessTokenConfigurationTypeDef
+    from mypy_boto3_mediatailor.type_defs import SecretsManagerAccessTokenConfigurationOutputTypeDef
 
-    data: SecretsManagerAccessTokenConfigurationTypeDef = {...}
+    data: SecretsManagerAccessTokenConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -38,37 +38,53 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "SecretsManagerAccessTokenConfigurationOutputTypeDef",
     "SecretsManagerAccessTokenConfigurationTypeDef",
+    "KeyValuePairOutputTypeDef",
+    "SlateSourceOutputTypeDef",
+    "SpliceInsertMessageOutputTypeDef",
     "KeyValuePairTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
+    "AdMarkerPassthroughOutputTypeDef",
     "AdMarkerPassthroughTypeDef",
-    "AlertTypeDef",
+    "AlertOutputTypeDef",
+    "AvailMatchingCriteriaOutputTypeDef",
     "AvailMatchingCriteriaTypeDef",
+    "AvailSuppressionOutputTypeDef",
     "AvailSuppressionTypeDef",
+    "BumperOutputTypeDef",
     "BumperTypeDef",
+    "CdnConfigurationOutputTypeDef",
     "CdnConfigurationTypeDef",
-    "LogConfigurationForChannelTypeDef",
+    "LogConfigurationForChannelOutputTypeDef",
+    "ClipRangeOutputTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
-    "ConfigureLogsForChannelResponseTypeDef",
+    "ConfigureLogsForChannelResponseOutputTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
+    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
     "HttpPackageConfigurationTypeDef",
+    "HttpPackageConfigurationOutputTypeDef",
     "PrefetchRetrievalTypeDef",
+    "PrefetchRetrievalOutputTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
+    "DefaultSegmentDeliveryConfigurationOutputTypeDef",
+    "HttpConfigurationOutputTypeDef",
+    "SegmentDeliveryConfigurationOutputTypeDef",
     "DashConfigurationForPutTypeDef",
-    "DashConfigurationTypeDef",
+    "DashConfigurationOutputTypeDef",
+    "DashPlaylistSettingsOutputTypeDef",
     "DashPlaylistSettingsTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteLiveSourceRequestRequestTypeDef",
     "DeletePlaybackConfigurationRequestRequestTypeDef",
     "DeletePrefetchScheduleRequestRequestTypeDef",
     "DeleteProgramRequestRequestTypeDef",
@@ -77,117 +93,160 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeLiveSourceRequestRequestTypeDef",
     "DescribeProgramRequestRequestTypeDef",
     "DescribeSourceLocationRequestRequestTypeDef",
     "DescribeVodSourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "GetChannelPolicyResponseTypeDef",
+    "GetChannelPolicyResponseOutputTypeDef",
     "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     "GetChannelScheduleRequestRequestTypeDef",
     "GetPlaybackConfigurationRequestRequestTypeDef",
-    "HlsConfigurationTypeDef",
-    "LivePreRollConfigurationTypeDef",
-    "LogConfigurationTypeDef",
+    "HlsConfigurationOutputTypeDef",
+    "LivePreRollConfigurationOutputTypeDef",
+    "LogConfigurationOutputTypeDef",
     "GetPrefetchScheduleRequestRequestTypeDef",
+    "HlsPlaylistSettingsOutputTypeDef",
     "HlsPlaylistSettingsTypeDef",
     "ListAlertsRequestListAlertsPaginateTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     "ListLiveSourcesRequestRequestTypeDef",
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
     "ListPrefetchSchedulesRequestRequestTypeDef",
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListSourceLocationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "ListVodSourcesRequestRequestTypeDef",
+    "LivePreRollConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ScheduleAdBreakTypeDef",
+    "ScheduleAdBreakOutputTypeDef",
     "TransitionTypeDef",
+    "SegmentationDescriptorOutputTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
+    "AccessConfigurationOutputTypeDef",
     "AccessConfigurationTypeDef",
+    "ManifestProcessingRulesOutputTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "ListAlertsResponseTypeDef",
+    "ListAlertsResponseOutputTypeDef",
+    "PrefetchConsumptionOutputTypeDef",
     "PrefetchConsumptionTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
-    "CreateLiveSourceResponseTypeDef",
     "CreateVodSourceRequestRequestTypeDef",
-    "CreateVodSourceResponseTypeDef",
-    "DescribeLiveSourceResponseTypeDef",
-    "DescribeVodSourceResponseTypeDef",
-    "LiveSourceTypeDef",
     "UpdateLiveSourceRequestRequestTypeDef",
-    "UpdateLiveSourceResponseTypeDef",
     "UpdateVodSourceRequestRequestTypeDef",
-    "UpdateVodSourceResponseTypeDef",
-    "VodSourceTypeDef",
+    "CreateLiveSourceResponseOutputTypeDef",
+    "CreateVodSourceResponseOutputTypeDef",
+    "DescribeLiveSourceResponseOutputTypeDef",
+    "DescribeVodSourceResponseOutputTypeDef",
+    "LiveSourceOutputTypeDef",
+    "UpdateLiveSourceResponseOutputTypeDef",
+    "UpdateVodSourceResponseOutputTypeDef",
+    "VodSourceOutputTypeDef",
+    "ResponseOutputItemOutputTypeDef",
     "RequestOutputItemTypeDef",
-    "ResponseOutputItemTypeDef",
-    "ScheduleEntryTypeDef",
+    "ScheduleEntryOutputTypeDef",
     "ScheduleConfigurationTypeDef",
+    "TimeSignalMessageOutputTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
+    "CreateSourceLocationResponseOutputTypeDef",
+    "DescribeSourceLocationResponseOutputTypeDef",
+    "SourceLocationOutputTypeDef",
+    "UpdateSourceLocationResponseOutputTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
-    "CreateSourceLocationResponseTypeDef",
-    "DescribeSourceLocationResponseTypeDef",
-    "SourceLocationTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
-    "UpdateSourceLocationResponseTypeDef",
-    "GetPlaybackConfigurationResponseTypeDef",
-    "PlaybackConfigurationTypeDef",
+    "GetPlaybackConfigurationResponseOutputTypeDef",
+    "PlaybackConfigurationOutputTypeDef",
+    "PutPlaybackConfigurationResponseOutputTypeDef",
     "PutPlaybackConfigurationRequestRequestTypeDef",
-    "PutPlaybackConfigurationResponseTypeDef",
+    "CreatePrefetchScheduleResponseOutputTypeDef",
+    "GetPrefetchScheduleResponseOutputTypeDef",
+    "PrefetchScheduleOutputTypeDef",
     "CreatePrefetchScheduleRequestRequestTypeDef",
-    "CreatePrefetchScheduleResponseTypeDef",
-    "GetPrefetchScheduleResponseTypeDef",
-    "PrefetchScheduleTypeDef",
-    "ListLiveSourcesResponseTypeDef",
-    "ListVodSourcesResponseTypeDef",
+    "ListLiveSourcesResponseOutputTypeDef",
+    "ListVodSourcesResponseOutputTypeDef",
+    "ChannelOutputTypeDef",
+    "CreateChannelResponseOutputTypeDef",
+    "DescribeChannelResponseOutputTypeDef",
+    "UpdateChannelResponseOutputTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "ChannelTypeDef",
-    "CreateChannelResponseTypeDef",
-    "DescribeChannelResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
-    "GetChannelScheduleResponseTypeDef",
+    "GetChannelScheduleResponseOutputTypeDef",
+    "AdBreakOutputTypeDef",
     "AdBreakTypeDef",
-    "ListSourceLocationsResponseTypeDef",
-    "ListPlaybackConfigurationsResponseTypeDef",
-    "ListPrefetchSchedulesResponseTypeDef",
-    "ListChannelsResponseTypeDef",
+    "ListSourceLocationsResponseOutputTypeDef",
+    "ListPlaybackConfigurationsResponseOutputTypeDef",
+    "ListPrefetchSchedulesResponseOutputTypeDef",
+    "ListChannelsResponseOutputTypeDef",
+    "CreateProgramResponseOutputTypeDef",
+    "DescribeProgramResponseOutputTypeDef",
+    "UpdateProgramResponseOutputTypeDef",
     "CreateProgramRequestRequestTypeDef",
-    "CreateProgramResponseTypeDef",
-    "DescribeProgramResponseTypeDef",
     "UpdateProgramRequestRequestTypeDef",
-    "UpdateProgramResponseTypeDef",
+)
+
+SecretsManagerAccessTokenConfigurationOutputTypeDef = TypedDict(
+    "SecretsManagerAccessTokenConfigurationOutputTypeDef",
+    {
+        "HeaderName": str,
+        "SecretArn": str,
+        "SecretStringKey": str,
+    },
 )
 
 SecretsManagerAccessTokenConfigurationTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationTypeDef",
     {
         "HeaderName": str,
         "SecretArn": str,
         "SecretStringKey": str,
     },
     total=False,
 )
 
+KeyValuePairOutputTypeDef = TypedDict(
+    "KeyValuePairOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+SlateSourceOutputTypeDef = TypedDict(
+    "SlateSourceOutputTypeDef",
+    {
+        "SourceLocationName": str,
+        "VodSourceName": str,
+    },
+)
+
+SpliceInsertMessageOutputTypeDef = TypedDict(
+    "SpliceInsertMessageOutputTypeDef",
+    {
+        "AvailNum": int,
+        "AvailsExpected": int,
+        "SpliceEventId": int,
+        "UniqueProgramId": int,
+    },
+)
+
 KeyValuePairTypeDef = TypedDict(
     "KeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -208,73 +267,124 @@
         "AvailsExpected": int,
         "SpliceEventId": int,
         "UniqueProgramId": int,
     },
     total=False,
 )
 
+AdMarkerPassthroughOutputTypeDef = TypedDict(
+    "AdMarkerPassthroughOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+
 AdMarkerPassthroughTypeDef = TypedDict(
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
-AlertTypeDef = TypedDict(
-    "AlertTypeDef",
+AlertOutputTypeDef = TypedDict(
+    "AlertOutputTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
         "Category": AlertCategoryType,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
     },
 )
 
+AvailMatchingCriteriaOutputTypeDef = TypedDict(
+    "AvailMatchingCriteriaOutputTypeDef",
+    {
+        "DynamicVariable": str,
+        "Operator": Literal["EQUALS"],
+    },
+)
+
 AvailMatchingCriteriaTypeDef = TypedDict(
     "AvailMatchingCriteriaTypeDef",
     {
         "DynamicVariable": str,
         "Operator": Literal["EQUALS"],
     },
 )
 
+AvailSuppressionOutputTypeDef = TypedDict(
+    "AvailSuppressionOutputTypeDef",
+    {
+        "FillPolicy": FillPolicyType,
+        "Mode": ModeType,
+        "Value": str,
+    },
+)
+
 AvailSuppressionTypeDef = TypedDict(
     "AvailSuppressionTypeDef",
     {
         "FillPolicy": FillPolicyType,
         "Mode": ModeType,
         "Value": str,
     },
+    total=False,
+)
+
+BumperOutputTypeDef = TypedDict(
+    "BumperOutputTypeDef",
+    {
+        "EndUrl": str,
+        "StartUrl": str,
+    },
 )
 
 BumperTypeDef = TypedDict(
     "BumperTypeDef",
     {
         "EndUrl": str,
         "StartUrl": str,
     },
+    total=False,
+)
+
+CdnConfigurationOutputTypeDef = TypedDict(
+    "CdnConfigurationOutputTypeDef",
+    {
+        "AdSegmentUrlPrefix": str,
+        "ContentSegmentUrlPrefix": str,
+    },
 )
 
 CdnConfigurationTypeDef = TypedDict(
     "CdnConfigurationTypeDef",
     {
         "AdSegmentUrlPrefix": str,
         "ContentSegmentUrlPrefix": str,
     },
+    total=False,
 )
 
-LogConfigurationForChannelTypeDef = TypedDict(
-    "LogConfigurationForChannelTypeDef",
+LogConfigurationForChannelOutputTypeDef = TypedDict(
+    "LogConfigurationForChannelOutputTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
 )
 
+ClipRangeOutputTypeDef = TypedDict(
+    "ClipRangeOutputTypeDef",
+    {
+        "EndOffsetMillis": int,
+    },
+)
+
 ClipRangeTypeDef = TypedDict(
     "ClipRangeTypeDef",
     {
         "EndOffsetMillis": int,
     },
 )
 
@@ -282,16 +392,16 @@
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
 
-ConfigureLogsForChannelResponseTypeDef = TypedDict(
-    "ConfigureLogsForChannelResponseTypeDef",
+ConfigureLogsForChannelResponseOutputTypeDef = TypedDict(
+    "ConfigureLogsForChannelResponseOutputTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -299,16 +409,16 @@
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
     },
 )
 
-ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
+ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef = TypedDict(
+    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -317,14 +427,23 @@
     {
         "Path": str,
         "SourceGroup": str,
         "Type": TypeType,
     },
 )
 
+HttpPackageConfigurationOutputTypeDef = TypedDict(
+    "HttpPackageConfigurationOutputTypeDef",
+    {
+        "Path": str,
+        "SourceGroup": str,
+        "Type": TypeType,
+    },
+)
+
 _RequiredPrefetchRetrievalTypeDef = TypedDict(
     "_RequiredPrefetchRetrievalTypeDef",
     {
         "EndTime": Union[datetime, str],
     },
 )
 _OptionalPrefetchRetrievalTypeDef = TypedDict(
@@ -339,14 +458,23 @@
 
 class PrefetchRetrievalTypeDef(
     _RequiredPrefetchRetrievalTypeDef, _OptionalPrefetchRetrievalTypeDef
 ):
     pass
 
 
+PrefetchRetrievalOutputTypeDef = TypedDict(
+    "PrefetchRetrievalOutputTypeDef",
+    {
+        "DynamicVariables": Dict[str, str],
+        "EndTime": datetime,
+        "StartTime": datetime,
+    },
+)
+
 DefaultSegmentDeliveryConfigurationTypeDef = TypedDict(
     "DefaultSegmentDeliveryConfigurationTypeDef",
     {
         "BaseUrl": str,
     },
     total=False,
 )
@@ -363,32 +491,64 @@
     {
         "BaseUrl": str,
         "Name": str,
     },
     total=False,
 )
 
+DefaultSegmentDeliveryConfigurationOutputTypeDef = TypedDict(
+    "DefaultSegmentDeliveryConfigurationOutputTypeDef",
+    {
+        "BaseUrl": str,
+    },
+)
+
+HttpConfigurationOutputTypeDef = TypedDict(
+    "HttpConfigurationOutputTypeDef",
+    {
+        "BaseUrl": str,
+    },
+)
+
+SegmentDeliveryConfigurationOutputTypeDef = TypedDict(
+    "SegmentDeliveryConfigurationOutputTypeDef",
+    {
+        "BaseUrl": str,
+        "Name": str,
+    },
+)
+
 DashConfigurationForPutTypeDef = TypedDict(
     "DashConfigurationForPutTypeDef",
     {
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
     total=False,
 )
 
-DashConfigurationTypeDef = TypedDict(
-    "DashConfigurationTypeDef",
+DashConfigurationOutputTypeDef = TypedDict(
+    "DashConfigurationOutputTypeDef",
     {
         "ManifestEndpointPrefix": str,
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
 )
 
+DashPlaylistSettingsOutputTypeDef = TypedDict(
+    "DashPlaylistSettingsOutputTypeDef",
+    {
+        "ManifestWindowSeconds": int,
+        "MinBufferTimeSeconds": int,
+        "MinUpdatePeriodSeconds": int,
+        "SuggestedPresentationDelaySeconds": int,
+    },
+)
+
 DashPlaylistSettingsTypeDef = TypedDict(
     "DashPlaylistSettingsTypeDef",
     {
         "ManifestWindowSeconds": int,
         "MinBufferTimeSeconds": int,
         "MinUpdatePeriodSeconds": int,
         "SuggestedPresentationDelaySeconds": int,
@@ -504,16 +664,16 @@
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
+GetChannelPolicyResponseOutputTypeDef = TypedDict(
+    "GetChannelPolicyResponseOutputTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -566,44 +726,52 @@
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-HlsConfigurationTypeDef = TypedDict(
-    "HlsConfigurationTypeDef",
+HlsConfigurationOutputTypeDef = TypedDict(
+    "HlsConfigurationOutputTypeDef",
     {
         "ManifestEndpointPrefix": str,
     },
 )
 
-LivePreRollConfigurationTypeDef = TypedDict(
-    "LivePreRollConfigurationTypeDef",
+LivePreRollConfigurationOutputTypeDef = TypedDict(
+    "LivePreRollConfigurationOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
         "MaxDurationSeconds": int,
     },
 )
 
-LogConfigurationTypeDef = TypedDict(
-    "LogConfigurationTypeDef",
+LogConfigurationOutputTypeDef = TypedDict(
+    "LogConfigurationOutputTypeDef",
     {
         "PercentEnabled": int,
     },
 )
 
 GetPrefetchScheduleRequestRequestTypeDef = TypedDict(
     "GetPrefetchScheduleRequestRequestTypeDef",
     {
         "Name": str,
         "PlaybackConfigurationName": str,
     },
 )
 
+HlsPlaylistSettingsOutputTypeDef = TypedDict(
+    "HlsPlaylistSettingsOutputTypeDef",
+    {
+        "AdMarkupType": List[AdMarkupTypeType],
+        "ManifestWindowSeconds": int,
+    },
+)
+
 HlsPlaylistSettingsTypeDef = TypedDict(
     "HlsPlaylistSettingsTypeDef",
     {
         "AdMarkupType": Sequence[AdMarkupTypeType],
         "ManifestWindowSeconds": int,
     },
     total=False,
@@ -798,16 +966,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
@@ -850,14 +1018,23 @@
 
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
 
+LivePreRollConfigurationTypeDef = TypedDict(
+    "LivePreRollConfigurationTypeDef",
+    {
+        "AdDecisionServerUrl": str,
+        "MaxDurationSeconds": int,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -879,16 +1056,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ScheduleAdBreakTypeDef = TypedDict(
-    "ScheduleAdBreakTypeDef",
+ScheduleAdBreakOutputTypeDef = TypedDict(
+    "ScheduleAdBreakOutputTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
@@ -911,14 +1088,28 @@
 )
 
 
 class TransitionTypeDef(_RequiredTransitionTypeDef, _OptionalTransitionTypeDef):
     pass
 
 
+SegmentationDescriptorOutputTypeDef = TypedDict(
+    "SegmentationDescriptorOutputTypeDef",
+    {
+        "SegmentNum": int,
+        "SegmentationEventId": int,
+        "SegmentationTypeId": int,
+        "SegmentationUpid": str,
+        "SegmentationUpidType": int,
+        "SegmentsExpected": int,
+        "SubSegmentNum": int,
+        "SubSegmentsExpected": int,
+    },
+)
+
 SegmentationDescriptorTypeDef = TypedDict(
     "SegmentationDescriptorTypeDef",
     {
         "SegmentNum": int,
         "SegmentationEventId": int,
         "SegmentationTypeId": int,
         "SegmentationUpid": str,
@@ -965,39 +1156,66 @@
     {
         "DurationMillis": int,
         "ScheduledStartTimeMillis": int,
     },
     total=False,
 )
 
+AccessConfigurationOutputTypeDef = TypedDict(
+    "AccessConfigurationOutputTypeDef",
+    {
+        "AccessType": AccessTypeType,
+        "SecretsManagerAccessTokenConfiguration": (
+            SecretsManagerAccessTokenConfigurationOutputTypeDef
+        ),
+    },
+)
+
 AccessConfigurationTypeDef = TypedDict(
     "AccessConfigurationTypeDef",
     {
         "AccessType": AccessTypeType,
         "SecretsManagerAccessTokenConfiguration": SecretsManagerAccessTokenConfigurationTypeDef,
     },
     total=False,
 )
 
+ManifestProcessingRulesOutputTypeDef = TypedDict(
+    "ManifestProcessingRulesOutputTypeDef",
+    {
+        "AdMarkerPassthrough": AdMarkerPassthroughOutputTypeDef,
+    },
+)
+
 ManifestProcessingRulesTypeDef = TypedDict(
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
+    total=False,
 )
 
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
+ListAlertsResponseOutputTypeDef = TypedDict(
+    "ListAlertsResponseOutputTypeDef",
     {
-        "Items": List[AlertTypeDef],
+        "Items": List[AlertOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PrefetchConsumptionOutputTypeDef = TypedDict(
+    "PrefetchConsumptionOutputTypeDef",
+    {
+        "AvailMatchingCriteria": List[AvailMatchingCriteriaOutputTypeDef],
+        "EndTime": datetime,
+        "StartTime": datetime,
+    },
+)
+
 _RequiredPrefetchConsumptionTypeDef = TypedDict(
     "_RequiredPrefetchConsumptionTypeDef",
     {
         "EndTime": Union[datetime, str],
     },
 )
 _OptionalPrefetchConsumptionTypeDef = TypedDict(
@@ -1035,28 +1253,14 @@
 
 class CreateLiveSourceRequestRequestTypeDef(
     _RequiredCreateLiveSourceRequestRequestTypeDef, _OptionalCreateLiveSourceRequestRequestTypeDef
 ):
     pass
 
 
-CreateLiveSourceResponseTypeDef = TypedDict(
-    "CreateLiveSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
-        "LastModifiedTime": datetime,
-        "LiveSourceName": str,
-        "SourceLocationName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateVodSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVodSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "SourceLocationName": str,
         "VodSourceName": str,
     },
@@ -1072,128 +1276,153 @@
 
 class CreateVodSourceRequestRequestTypeDef(
     _RequiredCreateVodSourceRequestRequestTypeDef, _OptionalCreateVodSourceRequestRequestTypeDef
 ):
     pass
 
 
-CreateVodSourceResponseTypeDef = TypedDict(
-    "CreateVodSourceResponseTypeDef",
+UpdateLiveSourceRequestRequestTypeDef = TypedDict(
+    "UpdateLiveSourceRequestRequestTypeDef",
     {
-        "Arn": str,
-        "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
-        "LastModifiedTime": datetime,
+        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
+        "LiveSourceName": str,
+        "SourceLocationName": str,
+    },
+)
+
+UpdateVodSourceRequestRequestTypeDef = TypedDict(
+    "UpdateVodSourceRequestRequestTypeDef",
+    {
+        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "SourceLocationName": str,
-        "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLiveSourceResponseTypeDef = TypedDict(
-    "DescribeLiveSourceResponseTypeDef",
+CreateLiveSourceResponseOutputTypeDef = TypedDict(
+    "CreateLiveSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVodSourceResponseTypeDef = TypedDict(
-    "DescribeVodSourceResponseTypeDef",
+CreateVodSourceResponseOutputTypeDef = TypedDict(
+    "CreateVodSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-LiveSourceTypeDef = TypedDict(
-    "LiveSourceTypeDef",
+DescribeLiveSourceResponseOutputTypeDef = TypedDict(
+    "DescribeLiveSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateLiveSourceRequestRequestTypeDef = TypedDict(
-    "UpdateLiveSourceRequestRequestTypeDef",
+DescribeVodSourceResponseOutputTypeDef = TypedDict(
+    "DescribeVodSourceResponseOutputTypeDef",
     {
-        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
-        "LiveSourceName": str,
+        "Arn": str,
+        "CreationTime": datetime,
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
+        "LastModifiedTime": datetime,
         "SourceLocationName": str,
+        "Tags": Dict[str, str],
+        "VodSourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateLiveSourceResponseTypeDef = TypedDict(
-    "UpdateLiveSourceResponseTypeDef",
+LiveSourceOutputTypeDef = TypedDict(
+    "LiveSourceOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVodSourceRequestRequestTypeDef = TypedDict(
-    "UpdateVodSourceRequestRequestTypeDef",
+UpdateLiveSourceResponseOutputTypeDef = TypedDict(
+    "UpdateLiveSourceResponseOutputTypeDef",
     {
-        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
+        "Arn": str,
+        "CreationTime": datetime,
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
+        "LastModifiedTime": datetime,
+        "LiveSourceName": str,
         "SourceLocationName": str,
-        "VodSourceName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVodSourceResponseTypeDef = TypedDict(
-    "UpdateVodSourceResponseTypeDef",
+UpdateVodSourceResponseOutputTypeDef = TypedDict(
+    "UpdateVodSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VodSourceTypeDef = TypedDict(
-    "VodSourceTypeDef",
+VodSourceOutputTypeDef = TypedDict(
+    "VodSourceOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
     },
 )
 
+ResponseOutputItemOutputTypeDef = TypedDict(
+    "ResponseOutputItemOutputTypeDef",
+    {
+        "DashPlaylistSettings": DashPlaylistSettingsOutputTypeDef,
+        "HlsPlaylistSettings": HlsPlaylistSettingsOutputTypeDef,
+        "ManifestName": str,
+        "PlaybackUrl": str,
+        "SourceGroup": str,
+    },
+)
+
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
 )
@@ -1209,35 +1438,24 @@
 
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
 
-ResponseOutputItemTypeDef = TypedDict(
-    "ResponseOutputItemTypeDef",
-    {
-        "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
-        "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
-        "ManifestName": str,
-        "PlaybackUrl": str,
-        "SourceGroup": str,
-    },
-)
-
-ScheduleEntryTypeDef = TypedDict(
-    "ScheduleEntryTypeDef",
+ScheduleEntryOutputTypeDef = TypedDict(
+    "ScheduleEntryOutputTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "Arn": str,
         "ChannelName": str,
         "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
+        "ScheduleAdBreaks": List[ScheduleAdBreakOutputTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
 _RequiredScheduleConfigurationTypeDef = TypedDict(
@@ -1257,14 +1475,21 @@
 
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
 
+TimeSignalMessageOutputTypeDef = TypedDict(
+    "TimeSignalMessageOutputTypeDef",
+    {
+        "SegmentationDescriptors": List[SegmentationDescriptorOutputTypeDef],
+    },
+)
+
 TimeSignalMessageTypeDef = TypedDict(
     "TimeSignalMessageTypeDef",
     {
         "SegmentationDescriptors": Sequence[SegmentationDescriptorTypeDef],
     },
     total=False,
 )
@@ -1274,87 +1499,103 @@
     {
         "ClipRange": ClipRangeTypeDef,
         "Transition": UpdateProgramTransitionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateSourceLocationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSourceLocationRequestRequestTypeDef",
+CreateSourceLocationResponseOutputTypeDef = TypedDict(
+    "CreateSourceLocationResponseOutputTypeDef",
     {
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
+        "Arn": str,
+        "CreationTime": datetime,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateSourceLocationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSourceLocationRequestRequestTypeDef",
-    {
-        "AccessConfiguration": AccessConfigurationTypeDef,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateSourceLocationRequestRequestTypeDef(
-    _RequiredCreateSourceLocationRequestRequestTypeDef,
-    _OptionalCreateSourceLocationRequestRequestTypeDef,
-):
-    pass
-
 
-CreateSourceLocationResponseTypeDef = TypedDict(
-    "CreateSourceLocationResponseTypeDef",
+DescribeSourceLocationResponseOutputTypeDef = TypedDict(
+    "DescribeSourceLocationResponseOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSourceLocationResponseTypeDef = TypedDict(
-    "DescribeSourceLocationResponseTypeDef",
+SourceLocationOutputTypeDef = TypedDict(
+    "SourceLocationOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SourceLocationTypeDef = TypedDict(
-    "SourceLocationTypeDef",
+UpdateSourceLocationResponseOutputTypeDef = TypedDict(
+    "UpdateSourceLocationResponseOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateSourceLocationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceLocationRequestRequestTypeDef",
+    {
+        "HttpConfiguration": HttpConfigurationTypeDef,
+        "SourceLocationName": str,
+    },
+)
+_OptionalCreateSourceLocationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceLocationRequestRequestTypeDef",
+    {
+        "AccessConfiguration": AccessConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
+        "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
+
+class CreateSourceLocationRequestRequestTypeDef(
+    _RequiredCreateSourceLocationRequestRequestTypeDef,
+    _OptionalCreateSourceLocationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1372,78 +1613,88 @@
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateSourceLocationResponseTypeDef = TypedDict(
-    "UpdateSourceLocationResponseTypeDef",
+GetPlaybackConfigurationResponseOutputTypeDef = TypedDict(
+    "GetPlaybackConfigurationResponseOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
-        "Arn": str,
-        "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
-        "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
-        "SourceLocationName": str,
+        "AdDecisionServerUrl": str,
+        "AvailSuppression": AvailSuppressionOutputTypeDef,
+        "Bumper": BumperOutputTypeDef,
+        "CdnConfiguration": CdnConfigurationOutputTypeDef,
+        "ConfigurationAliases": Dict[str, Dict[str, str]],
+        "DashConfiguration": DashConfigurationOutputTypeDef,
+        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
+        "Name": str,
+        "PersonalizationThresholdSeconds": int,
+        "PlaybackConfigurationArn": str,
+        "PlaybackEndpointPrefix": str,
+        "SessionInitializationEndpointPrefix": str,
+        "SlateAdUrl": str,
         "Tags": Dict[str, str],
+        "TranscodeProfileName": str,
+        "VideoContentSourceUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPlaybackConfigurationResponseTypeDef = TypedDict(
-    "GetPlaybackConfigurationResponseTypeDef",
+PlaybackConfigurationOutputTypeDef = TypedDict(
+    "PlaybackConfigurationOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
-        "AvailSuppression": AvailSuppressionTypeDef,
-        "Bumper": BumperTypeDef,
-        "CdnConfiguration": CdnConfigurationTypeDef,
+        "AvailSuppression": AvailSuppressionOutputTypeDef,
+        "Bumper": BumperOutputTypeDef,
+        "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationTypeDef,
-        "HlsConfiguration": HlsConfigurationTypeDef,
-        "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
-        "LogConfiguration": LogConfigurationTypeDef,
-        "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
+        "DashConfiguration": DashConfigurationOutputTypeDef,
+        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PlaybackConfigurationTypeDef = TypedDict(
-    "PlaybackConfigurationTypeDef",
+PutPlaybackConfigurationResponseOutputTypeDef = TypedDict(
+    "PutPlaybackConfigurationResponseOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
-        "AvailSuppression": AvailSuppressionTypeDef,
-        "Bumper": BumperTypeDef,
-        "CdnConfiguration": CdnConfigurationTypeDef,
+        "AvailSuppression": AvailSuppressionOutputTypeDef,
+        "Bumper": BumperOutputTypeDef,
+        "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationTypeDef,
-        "HlsConfiguration": HlsConfigurationTypeDef,
-        "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
-        "LogConfiguration": LogConfigurationTypeDef,
-        "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
+        "DashConfiguration": DashConfigurationOutputTypeDef,
+        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
@@ -1473,40 +1724,52 @@
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-PutPlaybackConfigurationResponseTypeDef = TypedDict(
-    "PutPlaybackConfigurationResponseTypeDef",
+CreatePrefetchScheduleResponseOutputTypeDef = TypedDict(
+    "CreatePrefetchScheduleResponseOutputTypeDef",
     {
-        "AdDecisionServerUrl": str,
-        "AvailSuppression": AvailSuppressionTypeDef,
-        "Bumper": BumperTypeDef,
-        "CdnConfiguration": CdnConfigurationTypeDef,
-        "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationTypeDef,
-        "HlsConfiguration": HlsConfigurationTypeDef,
-        "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
-        "LogConfiguration": LogConfigurationTypeDef,
-        "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
+        "Arn": str,
+        "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
-        "PersonalizationThresholdSeconds": int,
-        "PlaybackConfigurationArn": str,
-        "PlaybackEndpointPrefix": str,
-        "SessionInitializationEndpointPrefix": str,
-        "SlateAdUrl": str,
-        "Tags": Dict[str, str],
-        "TranscodeProfileName": str,
-        "VideoContentSourceUrl": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalOutputTypeDef,
+        "StreamId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetPrefetchScheduleResponseOutputTypeDef = TypedDict(
+    "GetPrefetchScheduleResponseOutputTypeDef",
+    {
+        "Arn": str,
+        "Consumption": PrefetchConsumptionOutputTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalOutputTypeDef,
+        "StreamId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PrefetchScheduleOutputTypeDef = TypedDict(
+    "PrefetchScheduleOutputTypeDef",
+    {
+        "Arn": str,
+        "Consumption": PrefetchConsumptionOutputTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalOutputTypeDef,
+        "StreamId": str,
+    },
+)
+
 _RequiredCreatePrefetchScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
@@ -1524,66 +1787,97 @@
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
 
-CreatePrefetchScheduleResponseTypeDef = TypedDict(
-    "CreatePrefetchScheduleResponseTypeDef",
+ListLiveSourcesResponseOutputTypeDef = TypedDict(
+    "ListLiveSourcesResponseOutputTypeDef",
     {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalTypeDef,
-        "StreamId": str,
+        "Items": List[LiveSourceOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPrefetchScheduleResponseTypeDef = TypedDict(
-    "GetPrefetchScheduleResponseTypeDef",
+ListVodSourcesResponseOutputTypeDef = TypedDict(
+    "ListVodSourcesResponseOutputTypeDef",
     {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalTypeDef,
-        "StreamId": str,
+        "Items": List[VodSourceOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PrefetchScheduleTypeDef = TypedDict(
-    "PrefetchScheduleTypeDef",
+ChannelOutputTypeDef = TypedDict(
+    "ChannelOutputTypeDef",
     {
         "Arn": str,
-        "Consumption": PrefetchConsumptionTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalTypeDef,
-        "StreamId": str,
+        "ChannelName": str,
+        "ChannelState": str,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
     },
 )
 
-ListLiveSourcesResponseTypeDef = TypedDict(
-    "ListLiveSourcesResponseTypeDef",
+CreateChannelResponseOutputTypeDef = TypedDict(
+    "CreateChannelResponseOutputTypeDef",
     {
-        "Items": List[LiveSourceTypeDef],
-        "NextToken": str,
+        "Arn": str,
+        "ChannelName": str,
+        "ChannelState": ChannelStateType,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVodSourcesResponseTypeDef = TypedDict(
-    "ListVodSourcesResponseTypeDef",
+DescribeChannelResponseOutputTypeDef = TypedDict(
+    "DescribeChannelResponseOutputTypeDef",
     {
-        "Items": List[VodSourceTypeDef],
-        "NextToken": str,
+        "Arn": str,
+        "ChannelName": str,
+        "ChannelState": ChannelStateType,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateChannelResponseOutputTypeDef = TypedDict(
+    "UpdateChannelResponseOutputTypeDef",
+    {
+        "Arn": str,
+        "ChannelName": str,
+        "ChannelState": ChannelStateType,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
@@ -1627,89 +1921,32 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-ChannelTypeDef = TypedDict(
-    "ChannelTypeDef",
+GetChannelScheduleResponseOutputTypeDef = TypedDict(
+    "GetChannelScheduleResponseOutputTypeDef",
     {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": str,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelTypeDef,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
-    },
-)
-
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": ChannelStateType,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": ChannelStateType,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelTypeDef,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": ChannelStateType,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
+        "Items": List[ScheduleEntryOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetChannelScheduleResponseTypeDef = TypedDict(
-    "GetChannelScheduleResponseTypeDef",
+AdBreakOutputTypeDef = TypedDict(
+    "AdBreakOutputTypeDef",
     {
-        "Items": List[ScheduleEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AdBreakMetadata": List[KeyValuePairOutputTypeDef],
+        "MessageType": MessageTypeType,
+        "OffsetMillis": int,
+        "Slate": SlateSourceOutputTypeDef,
+        "SpliceInsertMessage": SpliceInsertMessageOutputTypeDef,
+        "TimeSignalMessage": TimeSignalMessageOutputTypeDef,
     },
 )
 
 AdBreakTypeDef = TypedDict(
     "AdBreakTypeDef",
     {
         "AdBreakMetadata": Sequence[KeyValuePairTypeDef],
@@ -1718,145 +1955,144 @@
         "Slate": SlateSourceTypeDef,
         "SpliceInsertMessage": SpliceInsertMessageTypeDef,
         "TimeSignalMessage": TimeSignalMessageTypeDef,
     },
     total=False,
 )
 
-ListSourceLocationsResponseTypeDef = TypedDict(
-    "ListSourceLocationsResponseTypeDef",
+ListSourceLocationsResponseOutputTypeDef = TypedDict(
+    "ListSourceLocationsResponseOutputTypeDef",
     {
-        "Items": List[SourceLocationTypeDef],
+        "Items": List[SourceLocationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPlaybackConfigurationsResponseTypeDef = TypedDict(
-    "ListPlaybackConfigurationsResponseTypeDef",
+ListPlaybackConfigurationsResponseOutputTypeDef = TypedDict(
+    "ListPlaybackConfigurationsResponseOutputTypeDef",
     {
-        "Items": List[PlaybackConfigurationTypeDef],
+        "Items": List[PlaybackConfigurationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPrefetchSchedulesResponseTypeDef = TypedDict(
-    "ListPrefetchSchedulesResponseTypeDef",
+ListPrefetchSchedulesResponseOutputTypeDef = TypedDict(
+    "ListPrefetchSchedulesResponseOutputTypeDef",
     {
-        "Items": List[PrefetchScheduleTypeDef],
+        "Items": List[PrefetchScheduleOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListChannelsResponseTypeDef = TypedDict(
-    "ListChannelsResponseTypeDef",
+ListChannelsResponseOutputTypeDef = TypedDict(
+    "ListChannelsResponseOutputTypeDef",
     {
-        "Items": List[ChannelTypeDef],
+        "Items": List[ChannelOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProgramRequestRequestTypeDef",
+CreateProgramResponseOutputTypeDef = TypedDict(
+    "CreateProgramResponseOutputTypeDef",
     {
+        "AdBreaks": List[AdBreakOutputTypeDef],
+        "Arn": str,
         "ChannelName": str,
+        "ClipRange": ClipRangeOutputTypeDef,
+        "CreationTime": datetime,
+        "DurationMillis": int,
+        "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "ScheduledStartTime": datetime,
         "SourceLocationName": str,
-    },
-)
-_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProgramRequestRequestTypeDef",
-    {
-        "AdBreaks": Sequence[AdBreakTypeDef],
-        "LiveSourceName": str,
         "VodSourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class CreateProgramRequestRequestTypeDef(
-    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
-):
-    pass
-
-
-CreateProgramResponseTypeDef = TypedDict(
-    "CreateProgramResponseTypeDef",
+DescribeProgramResponseOutputTypeDef = TypedDict(
+    "DescribeProgramResponseOutputTypeDef",
     {
-        "AdBreaks": List[AdBreakTypeDef],
+        "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
+        "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeProgramResponseTypeDef = TypedDict(
-    "DescribeProgramResponseTypeDef",
+UpdateProgramResponseOutputTypeDef = TypedDict(
+    "UpdateProgramResponseOutputTypeDef",
     {
-        "AdBreaks": List[AdBreakTypeDef],
+        "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
+        "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProgramRequestRequestTypeDef",
+_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
         "ProgramName": str,
-        "ScheduleConfiguration": UpdateProgramScheduleConfigurationTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "SourceLocationName": str,
     },
 )
-_OptionalUpdateProgramRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProgramRequestRequestTypeDef",
+_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProgramRequestRequestTypeDef",
     {
         "AdBreaks": Sequence[AdBreakTypeDef],
+        "LiveSourceName": str,
+        "VodSourceName": str,
     },
     total=False,
 )
 
 
-class UpdateProgramRequestRequestTypeDef(
-    _RequiredUpdateProgramRequestRequestTypeDef, _OptionalUpdateProgramRequestRequestTypeDef
+class CreateProgramRequestRequestTypeDef(
+    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
 ):
     pass
 
 
-UpdateProgramResponseTypeDef = TypedDict(
-    "UpdateProgramResponseTypeDef",
+_RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProgramRequestRequestTypeDef",
     {
-        "AdBreaks": List[AdBreakTypeDef],
-        "Arn": str,
         "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
-        "CreationTime": datetime,
-        "DurationMillis": int,
-        "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduledStartTime": datetime,
-        "SourceLocationName": str,
-        "VodSourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ScheduleConfiguration": UpdateProgramScheduleConfigurationTypeDef,
+    },
+)
+_OptionalUpdateProgramRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProgramRequestRequestTypeDef",
+    {
+        "AdBreaks": Sequence[AdBreakTypeDef],
     },
+    total=False,
 )
+
+
+class UpdateProgramRequestRequestTypeDef(
+    _RequiredUpdateProgramRequestRequestTypeDef, _OptionalUpdateProgramRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.pyi` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediatailor service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediatailor.type_defs import SecretsManagerAccessTokenConfigurationTypeDef
+    from mypy_boto3_mediatailor.type_defs import SecretsManagerAccessTokenConfigurationOutputTypeDef
 
-    data: SecretsManagerAccessTokenConfigurationTypeDef = {...}
+    data: SecretsManagerAccessTokenConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -37,37 +37,53 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "SecretsManagerAccessTokenConfigurationOutputTypeDef",
     "SecretsManagerAccessTokenConfigurationTypeDef",
+    "KeyValuePairOutputTypeDef",
+    "SlateSourceOutputTypeDef",
+    "SpliceInsertMessageOutputTypeDef",
     "KeyValuePairTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
+    "AdMarkerPassthroughOutputTypeDef",
     "AdMarkerPassthroughTypeDef",
-    "AlertTypeDef",
+    "AlertOutputTypeDef",
+    "AvailMatchingCriteriaOutputTypeDef",
     "AvailMatchingCriteriaTypeDef",
+    "AvailSuppressionOutputTypeDef",
     "AvailSuppressionTypeDef",
+    "BumperOutputTypeDef",
     "BumperTypeDef",
+    "CdnConfigurationOutputTypeDef",
     "CdnConfigurationTypeDef",
-    "LogConfigurationForChannelTypeDef",
+    "LogConfigurationForChannelOutputTypeDef",
+    "ClipRangeOutputTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
-    "ConfigureLogsForChannelResponseTypeDef",
+    "ConfigureLogsForChannelResponseOutputTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
+    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
     "HttpPackageConfigurationTypeDef",
+    "HttpPackageConfigurationOutputTypeDef",
     "PrefetchRetrievalTypeDef",
+    "PrefetchRetrievalOutputTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
+    "DefaultSegmentDeliveryConfigurationOutputTypeDef",
+    "HttpConfigurationOutputTypeDef",
+    "SegmentDeliveryConfigurationOutputTypeDef",
     "DashConfigurationForPutTypeDef",
-    "DashConfigurationTypeDef",
+    "DashConfigurationOutputTypeDef",
+    "DashPlaylistSettingsOutputTypeDef",
     "DashPlaylistSettingsTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteLiveSourceRequestRequestTypeDef",
     "DeletePlaybackConfigurationRequestRequestTypeDef",
     "DeletePrefetchScheduleRequestRequestTypeDef",
     "DeleteProgramRequestRequestTypeDef",
@@ -76,117 +92,160 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeLiveSourceRequestRequestTypeDef",
     "DescribeProgramRequestRequestTypeDef",
     "DescribeSourceLocationRequestRequestTypeDef",
     "DescribeVodSourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "GetChannelPolicyResponseTypeDef",
+    "GetChannelPolicyResponseOutputTypeDef",
     "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     "GetChannelScheduleRequestRequestTypeDef",
     "GetPlaybackConfigurationRequestRequestTypeDef",
-    "HlsConfigurationTypeDef",
-    "LivePreRollConfigurationTypeDef",
-    "LogConfigurationTypeDef",
+    "HlsConfigurationOutputTypeDef",
+    "LivePreRollConfigurationOutputTypeDef",
+    "LogConfigurationOutputTypeDef",
     "GetPrefetchScheduleRequestRequestTypeDef",
+    "HlsPlaylistSettingsOutputTypeDef",
     "HlsPlaylistSettingsTypeDef",
     "ListAlertsRequestListAlertsPaginateTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     "ListLiveSourcesRequestRequestTypeDef",
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
     "ListPrefetchSchedulesRequestRequestTypeDef",
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListSourceLocationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "ListVodSourcesRequestRequestTypeDef",
+    "LivePreRollConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ScheduleAdBreakTypeDef",
+    "ScheduleAdBreakOutputTypeDef",
     "TransitionTypeDef",
+    "SegmentationDescriptorOutputTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
+    "AccessConfigurationOutputTypeDef",
     "AccessConfigurationTypeDef",
+    "ManifestProcessingRulesOutputTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "ListAlertsResponseTypeDef",
+    "ListAlertsResponseOutputTypeDef",
+    "PrefetchConsumptionOutputTypeDef",
     "PrefetchConsumptionTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
-    "CreateLiveSourceResponseTypeDef",
     "CreateVodSourceRequestRequestTypeDef",
-    "CreateVodSourceResponseTypeDef",
-    "DescribeLiveSourceResponseTypeDef",
-    "DescribeVodSourceResponseTypeDef",
-    "LiveSourceTypeDef",
     "UpdateLiveSourceRequestRequestTypeDef",
-    "UpdateLiveSourceResponseTypeDef",
     "UpdateVodSourceRequestRequestTypeDef",
-    "UpdateVodSourceResponseTypeDef",
-    "VodSourceTypeDef",
+    "CreateLiveSourceResponseOutputTypeDef",
+    "CreateVodSourceResponseOutputTypeDef",
+    "DescribeLiveSourceResponseOutputTypeDef",
+    "DescribeVodSourceResponseOutputTypeDef",
+    "LiveSourceOutputTypeDef",
+    "UpdateLiveSourceResponseOutputTypeDef",
+    "UpdateVodSourceResponseOutputTypeDef",
+    "VodSourceOutputTypeDef",
+    "ResponseOutputItemOutputTypeDef",
     "RequestOutputItemTypeDef",
-    "ResponseOutputItemTypeDef",
-    "ScheduleEntryTypeDef",
+    "ScheduleEntryOutputTypeDef",
     "ScheduleConfigurationTypeDef",
+    "TimeSignalMessageOutputTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
+    "CreateSourceLocationResponseOutputTypeDef",
+    "DescribeSourceLocationResponseOutputTypeDef",
+    "SourceLocationOutputTypeDef",
+    "UpdateSourceLocationResponseOutputTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
-    "CreateSourceLocationResponseTypeDef",
-    "DescribeSourceLocationResponseTypeDef",
-    "SourceLocationTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
-    "UpdateSourceLocationResponseTypeDef",
-    "GetPlaybackConfigurationResponseTypeDef",
-    "PlaybackConfigurationTypeDef",
+    "GetPlaybackConfigurationResponseOutputTypeDef",
+    "PlaybackConfigurationOutputTypeDef",
+    "PutPlaybackConfigurationResponseOutputTypeDef",
     "PutPlaybackConfigurationRequestRequestTypeDef",
-    "PutPlaybackConfigurationResponseTypeDef",
+    "CreatePrefetchScheduleResponseOutputTypeDef",
+    "GetPrefetchScheduleResponseOutputTypeDef",
+    "PrefetchScheduleOutputTypeDef",
     "CreatePrefetchScheduleRequestRequestTypeDef",
-    "CreatePrefetchScheduleResponseTypeDef",
-    "GetPrefetchScheduleResponseTypeDef",
-    "PrefetchScheduleTypeDef",
-    "ListLiveSourcesResponseTypeDef",
-    "ListVodSourcesResponseTypeDef",
+    "ListLiveSourcesResponseOutputTypeDef",
+    "ListVodSourcesResponseOutputTypeDef",
+    "ChannelOutputTypeDef",
+    "CreateChannelResponseOutputTypeDef",
+    "DescribeChannelResponseOutputTypeDef",
+    "UpdateChannelResponseOutputTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "ChannelTypeDef",
-    "CreateChannelResponseTypeDef",
-    "DescribeChannelResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
-    "GetChannelScheduleResponseTypeDef",
+    "GetChannelScheduleResponseOutputTypeDef",
+    "AdBreakOutputTypeDef",
     "AdBreakTypeDef",
-    "ListSourceLocationsResponseTypeDef",
-    "ListPlaybackConfigurationsResponseTypeDef",
-    "ListPrefetchSchedulesResponseTypeDef",
-    "ListChannelsResponseTypeDef",
+    "ListSourceLocationsResponseOutputTypeDef",
+    "ListPlaybackConfigurationsResponseOutputTypeDef",
+    "ListPrefetchSchedulesResponseOutputTypeDef",
+    "ListChannelsResponseOutputTypeDef",
+    "CreateProgramResponseOutputTypeDef",
+    "DescribeProgramResponseOutputTypeDef",
+    "UpdateProgramResponseOutputTypeDef",
     "CreateProgramRequestRequestTypeDef",
-    "CreateProgramResponseTypeDef",
-    "DescribeProgramResponseTypeDef",
     "UpdateProgramRequestRequestTypeDef",
-    "UpdateProgramResponseTypeDef",
+)
+
+SecretsManagerAccessTokenConfigurationOutputTypeDef = TypedDict(
+    "SecretsManagerAccessTokenConfigurationOutputTypeDef",
+    {
+        "HeaderName": str,
+        "SecretArn": str,
+        "SecretStringKey": str,
+    },
 )
 
 SecretsManagerAccessTokenConfigurationTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationTypeDef",
     {
         "HeaderName": str,
         "SecretArn": str,
         "SecretStringKey": str,
     },
     total=False,
 )
 
+KeyValuePairOutputTypeDef = TypedDict(
+    "KeyValuePairOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+SlateSourceOutputTypeDef = TypedDict(
+    "SlateSourceOutputTypeDef",
+    {
+        "SourceLocationName": str,
+        "VodSourceName": str,
+    },
+)
+
+SpliceInsertMessageOutputTypeDef = TypedDict(
+    "SpliceInsertMessageOutputTypeDef",
+    {
+        "AvailNum": int,
+        "AvailsExpected": int,
+        "SpliceEventId": int,
+        "UniqueProgramId": int,
+    },
+)
+
 KeyValuePairTypeDef = TypedDict(
     "KeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -207,73 +266,124 @@
         "AvailsExpected": int,
         "SpliceEventId": int,
         "UniqueProgramId": int,
     },
     total=False,
 )
 
+AdMarkerPassthroughOutputTypeDef = TypedDict(
+    "AdMarkerPassthroughOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+
 AdMarkerPassthroughTypeDef = TypedDict(
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
-AlertTypeDef = TypedDict(
-    "AlertTypeDef",
+AlertOutputTypeDef = TypedDict(
+    "AlertOutputTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
         "Category": AlertCategoryType,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
     },
 )
 
+AvailMatchingCriteriaOutputTypeDef = TypedDict(
+    "AvailMatchingCriteriaOutputTypeDef",
+    {
+        "DynamicVariable": str,
+        "Operator": Literal["EQUALS"],
+    },
+)
+
 AvailMatchingCriteriaTypeDef = TypedDict(
     "AvailMatchingCriteriaTypeDef",
     {
         "DynamicVariable": str,
         "Operator": Literal["EQUALS"],
     },
 )
 
+AvailSuppressionOutputTypeDef = TypedDict(
+    "AvailSuppressionOutputTypeDef",
+    {
+        "FillPolicy": FillPolicyType,
+        "Mode": ModeType,
+        "Value": str,
+    },
+)
+
 AvailSuppressionTypeDef = TypedDict(
     "AvailSuppressionTypeDef",
     {
         "FillPolicy": FillPolicyType,
         "Mode": ModeType,
         "Value": str,
     },
+    total=False,
+)
+
+BumperOutputTypeDef = TypedDict(
+    "BumperOutputTypeDef",
+    {
+        "EndUrl": str,
+        "StartUrl": str,
+    },
 )
 
 BumperTypeDef = TypedDict(
     "BumperTypeDef",
     {
         "EndUrl": str,
         "StartUrl": str,
     },
+    total=False,
+)
+
+CdnConfigurationOutputTypeDef = TypedDict(
+    "CdnConfigurationOutputTypeDef",
+    {
+        "AdSegmentUrlPrefix": str,
+        "ContentSegmentUrlPrefix": str,
+    },
 )
 
 CdnConfigurationTypeDef = TypedDict(
     "CdnConfigurationTypeDef",
     {
         "AdSegmentUrlPrefix": str,
         "ContentSegmentUrlPrefix": str,
     },
+    total=False,
 )
 
-LogConfigurationForChannelTypeDef = TypedDict(
-    "LogConfigurationForChannelTypeDef",
+LogConfigurationForChannelOutputTypeDef = TypedDict(
+    "LogConfigurationForChannelOutputTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
 )
 
+ClipRangeOutputTypeDef = TypedDict(
+    "ClipRangeOutputTypeDef",
+    {
+        "EndOffsetMillis": int,
+    },
+)
+
 ClipRangeTypeDef = TypedDict(
     "ClipRangeTypeDef",
     {
         "EndOffsetMillis": int,
     },
 )
 
@@ -281,16 +391,16 @@
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
 
-ConfigureLogsForChannelResponseTypeDef = TypedDict(
-    "ConfigureLogsForChannelResponseTypeDef",
+ConfigureLogsForChannelResponseOutputTypeDef = TypedDict(
+    "ConfigureLogsForChannelResponseOutputTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -298,16 +408,16 @@
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
     },
 )
 
-ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
+ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef = TypedDict(
+    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -316,14 +426,23 @@
     {
         "Path": str,
         "SourceGroup": str,
         "Type": TypeType,
     },
 )
 
+HttpPackageConfigurationOutputTypeDef = TypedDict(
+    "HttpPackageConfigurationOutputTypeDef",
+    {
+        "Path": str,
+        "SourceGroup": str,
+        "Type": TypeType,
+    },
+)
+
 _RequiredPrefetchRetrievalTypeDef = TypedDict(
     "_RequiredPrefetchRetrievalTypeDef",
     {
         "EndTime": Union[datetime, str],
     },
 )
 _OptionalPrefetchRetrievalTypeDef = TypedDict(
@@ -336,14 +455,23 @@
 )
 
 class PrefetchRetrievalTypeDef(
     _RequiredPrefetchRetrievalTypeDef, _OptionalPrefetchRetrievalTypeDef
 ):
     pass
 
+PrefetchRetrievalOutputTypeDef = TypedDict(
+    "PrefetchRetrievalOutputTypeDef",
+    {
+        "DynamicVariables": Dict[str, str],
+        "EndTime": datetime,
+        "StartTime": datetime,
+    },
+)
+
 DefaultSegmentDeliveryConfigurationTypeDef = TypedDict(
     "DefaultSegmentDeliveryConfigurationTypeDef",
     {
         "BaseUrl": str,
     },
     total=False,
 )
@@ -360,32 +488,64 @@
     {
         "BaseUrl": str,
         "Name": str,
     },
     total=False,
 )
 
+DefaultSegmentDeliveryConfigurationOutputTypeDef = TypedDict(
+    "DefaultSegmentDeliveryConfigurationOutputTypeDef",
+    {
+        "BaseUrl": str,
+    },
+)
+
+HttpConfigurationOutputTypeDef = TypedDict(
+    "HttpConfigurationOutputTypeDef",
+    {
+        "BaseUrl": str,
+    },
+)
+
+SegmentDeliveryConfigurationOutputTypeDef = TypedDict(
+    "SegmentDeliveryConfigurationOutputTypeDef",
+    {
+        "BaseUrl": str,
+        "Name": str,
+    },
+)
+
 DashConfigurationForPutTypeDef = TypedDict(
     "DashConfigurationForPutTypeDef",
     {
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
     total=False,
 )
 
-DashConfigurationTypeDef = TypedDict(
-    "DashConfigurationTypeDef",
+DashConfigurationOutputTypeDef = TypedDict(
+    "DashConfigurationOutputTypeDef",
     {
         "ManifestEndpointPrefix": str,
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
 )
 
+DashPlaylistSettingsOutputTypeDef = TypedDict(
+    "DashPlaylistSettingsOutputTypeDef",
+    {
+        "ManifestWindowSeconds": int,
+        "MinBufferTimeSeconds": int,
+        "MinUpdatePeriodSeconds": int,
+        "SuggestedPresentationDelaySeconds": int,
+    },
+)
+
 DashPlaylistSettingsTypeDef = TypedDict(
     "DashPlaylistSettingsTypeDef",
     {
         "ManifestWindowSeconds": int,
         "MinBufferTimeSeconds": int,
         "MinUpdatePeriodSeconds": int,
         "SuggestedPresentationDelaySeconds": int,
@@ -501,16 +661,16 @@
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
+GetChannelPolicyResponseOutputTypeDef = TypedDict(
+    "GetChannelPolicyResponseOutputTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -559,44 +719,52 @@
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-HlsConfigurationTypeDef = TypedDict(
-    "HlsConfigurationTypeDef",
+HlsConfigurationOutputTypeDef = TypedDict(
+    "HlsConfigurationOutputTypeDef",
     {
         "ManifestEndpointPrefix": str,
     },
 )
 
-LivePreRollConfigurationTypeDef = TypedDict(
-    "LivePreRollConfigurationTypeDef",
+LivePreRollConfigurationOutputTypeDef = TypedDict(
+    "LivePreRollConfigurationOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
         "MaxDurationSeconds": int,
     },
 )
 
-LogConfigurationTypeDef = TypedDict(
-    "LogConfigurationTypeDef",
+LogConfigurationOutputTypeDef = TypedDict(
+    "LogConfigurationOutputTypeDef",
     {
         "PercentEnabled": int,
     },
 )
 
 GetPrefetchScheduleRequestRequestTypeDef = TypedDict(
     "GetPrefetchScheduleRequestRequestTypeDef",
     {
         "Name": str,
         "PlaybackConfigurationName": str,
     },
 )
 
+HlsPlaylistSettingsOutputTypeDef = TypedDict(
+    "HlsPlaylistSettingsOutputTypeDef",
+    {
+        "AdMarkupType": List[AdMarkupTypeType],
+        "ManifestWindowSeconds": int,
+    },
+)
+
 HlsPlaylistSettingsTypeDef = TypedDict(
     "HlsPlaylistSettingsTypeDef",
     {
         "AdMarkupType": Sequence[AdMarkupTypeType],
         "ManifestWindowSeconds": int,
     },
     total=False,
@@ -779,16 +947,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
@@ -827,14 +995,23 @@
 )
 
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
+LivePreRollConfigurationTypeDef = TypedDict(
+    "LivePreRollConfigurationTypeDef",
+    {
+        "AdDecisionServerUrl": str,
+        "MaxDurationSeconds": int,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -856,16 +1033,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ScheduleAdBreakTypeDef = TypedDict(
-    "ScheduleAdBreakTypeDef",
+ScheduleAdBreakOutputTypeDef = TypedDict(
+    "ScheduleAdBreakOutputTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
@@ -886,14 +1063,28 @@
     },
     total=False,
 )
 
 class TransitionTypeDef(_RequiredTransitionTypeDef, _OptionalTransitionTypeDef):
     pass
 
+SegmentationDescriptorOutputTypeDef = TypedDict(
+    "SegmentationDescriptorOutputTypeDef",
+    {
+        "SegmentNum": int,
+        "SegmentationEventId": int,
+        "SegmentationTypeId": int,
+        "SegmentationUpid": str,
+        "SegmentationUpidType": int,
+        "SegmentsExpected": int,
+        "SubSegmentNum": int,
+        "SubSegmentsExpected": int,
+    },
+)
+
 SegmentationDescriptorTypeDef = TypedDict(
     "SegmentationDescriptorTypeDef",
     {
         "SegmentNum": int,
         "SegmentationEventId": int,
         "SegmentationTypeId": int,
         "SegmentationUpid": str,
@@ -940,39 +1131,66 @@
     {
         "DurationMillis": int,
         "ScheduledStartTimeMillis": int,
     },
     total=False,
 )
 
+AccessConfigurationOutputTypeDef = TypedDict(
+    "AccessConfigurationOutputTypeDef",
+    {
+        "AccessType": AccessTypeType,
+        "SecretsManagerAccessTokenConfiguration": (
+            SecretsManagerAccessTokenConfigurationOutputTypeDef
+        ),
+    },
+)
+
 AccessConfigurationTypeDef = TypedDict(
     "AccessConfigurationTypeDef",
     {
         "AccessType": AccessTypeType,
         "SecretsManagerAccessTokenConfiguration": SecretsManagerAccessTokenConfigurationTypeDef,
     },
     total=False,
 )
 
+ManifestProcessingRulesOutputTypeDef = TypedDict(
+    "ManifestProcessingRulesOutputTypeDef",
+    {
+        "AdMarkerPassthrough": AdMarkerPassthroughOutputTypeDef,
+    },
+)
+
 ManifestProcessingRulesTypeDef = TypedDict(
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
+    total=False,
 )
 
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
+ListAlertsResponseOutputTypeDef = TypedDict(
+    "ListAlertsResponseOutputTypeDef",
     {
-        "Items": List[AlertTypeDef],
+        "Items": List[AlertOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PrefetchConsumptionOutputTypeDef = TypedDict(
+    "PrefetchConsumptionOutputTypeDef",
+    {
+        "AvailMatchingCriteria": List[AvailMatchingCriteriaOutputTypeDef],
+        "EndTime": datetime,
+        "StartTime": datetime,
+    },
+)
+
 _RequiredPrefetchConsumptionTypeDef = TypedDict(
     "_RequiredPrefetchConsumptionTypeDef",
     {
         "EndTime": Union[datetime, str],
     },
 )
 _OptionalPrefetchConsumptionTypeDef = TypedDict(
@@ -1006,28 +1224,14 @@
 )
 
 class CreateLiveSourceRequestRequestTypeDef(
     _RequiredCreateLiveSourceRequestRequestTypeDef, _OptionalCreateLiveSourceRequestRequestTypeDef
 ):
     pass
 
-CreateLiveSourceResponseTypeDef = TypedDict(
-    "CreateLiveSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
-        "LastModifiedTime": datetime,
-        "LiveSourceName": str,
-        "SourceLocationName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateVodSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVodSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "SourceLocationName": str,
         "VodSourceName": str,
     },
@@ -1041,128 +1245,153 @@
 )
 
 class CreateVodSourceRequestRequestTypeDef(
     _RequiredCreateVodSourceRequestRequestTypeDef, _OptionalCreateVodSourceRequestRequestTypeDef
 ):
     pass
 
-CreateVodSourceResponseTypeDef = TypedDict(
-    "CreateVodSourceResponseTypeDef",
+UpdateLiveSourceRequestRequestTypeDef = TypedDict(
+    "UpdateLiveSourceRequestRequestTypeDef",
     {
-        "Arn": str,
-        "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
-        "LastModifiedTime": datetime,
+        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
+        "LiveSourceName": str,
+        "SourceLocationName": str,
+    },
+)
+
+UpdateVodSourceRequestRequestTypeDef = TypedDict(
+    "UpdateVodSourceRequestRequestTypeDef",
+    {
+        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "SourceLocationName": str,
-        "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLiveSourceResponseTypeDef = TypedDict(
-    "DescribeLiveSourceResponseTypeDef",
+CreateLiveSourceResponseOutputTypeDef = TypedDict(
+    "CreateLiveSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVodSourceResponseTypeDef = TypedDict(
-    "DescribeVodSourceResponseTypeDef",
+CreateVodSourceResponseOutputTypeDef = TypedDict(
+    "CreateVodSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-LiveSourceTypeDef = TypedDict(
-    "LiveSourceTypeDef",
+DescribeLiveSourceResponseOutputTypeDef = TypedDict(
+    "DescribeLiveSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateLiveSourceRequestRequestTypeDef = TypedDict(
-    "UpdateLiveSourceRequestRequestTypeDef",
+DescribeVodSourceResponseOutputTypeDef = TypedDict(
+    "DescribeVodSourceResponseOutputTypeDef",
     {
-        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
-        "LiveSourceName": str,
+        "Arn": str,
+        "CreationTime": datetime,
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
+        "LastModifiedTime": datetime,
         "SourceLocationName": str,
+        "Tags": Dict[str, str],
+        "VodSourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateLiveSourceResponseTypeDef = TypedDict(
-    "UpdateLiveSourceResponseTypeDef",
+LiveSourceOutputTypeDef = TypedDict(
+    "LiveSourceOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVodSourceRequestRequestTypeDef = TypedDict(
-    "UpdateVodSourceRequestRequestTypeDef",
+UpdateLiveSourceResponseOutputTypeDef = TypedDict(
+    "UpdateLiveSourceResponseOutputTypeDef",
     {
-        "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
+        "Arn": str,
+        "CreationTime": datetime,
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
+        "LastModifiedTime": datetime,
+        "LiveSourceName": str,
         "SourceLocationName": str,
-        "VodSourceName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVodSourceResponseTypeDef = TypedDict(
-    "UpdateVodSourceResponseTypeDef",
+UpdateVodSourceResponseOutputTypeDef = TypedDict(
+    "UpdateVodSourceResponseOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VodSourceTypeDef = TypedDict(
-    "VodSourceTypeDef",
+VodSourceOutputTypeDef = TypedDict(
+    "VodSourceOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
     },
 )
 
+ResponseOutputItemOutputTypeDef = TypedDict(
+    "ResponseOutputItemOutputTypeDef",
+    {
+        "DashPlaylistSettings": DashPlaylistSettingsOutputTypeDef,
+        "HlsPlaylistSettings": HlsPlaylistSettingsOutputTypeDef,
+        "ManifestName": str,
+        "PlaybackUrl": str,
+        "SourceGroup": str,
+    },
+)
+
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
 )
@@ -1176,35 +1405,24 @@
 )
 
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
-ResponseOutputItemTypeDef = TypedDict(
-    "ResponseOutputItemTypeDef",
-    {
-        "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
-        "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
-        "ManifestName": str,
-        "PlaybackUrl": str,
-        "SourceGroup": str,
-    },
-)
-
-ScheduleEntryTypeDef = TypedDict(
-    "ScheduleEntryTypeDef",
+ScheduleEntryOutputTypeDef = TypedDict(
+    "ScheduleEntryOutputTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "Arn": str,
         "ChannelName": str,
         "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
+        "ScheduleAdBreaks": List[ScheduleAdBreakOutputTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
 _RequiredScheduleConfigurationTypeDef = TypedDict(
@@ -1222,14 +1440,21 @@
 )
 
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
+TimeSignalMessageOutputTypeDef = TypedDict(
+    "TimeSignalMessageOutputTypeDef",
+    {
+        "SegmentationDescriptors": List[SegmentationDescriptorOutputTypeDef],
+    },
+)
+
 TimeSignalMessageTypeDef = TypedDict(
     "TimeSignalMessageTypeDef",
     {
         "SegmentationDescriptors": Sequence[SegmentationDescriptorTypeDef],
     },
     total=False,
 )
@@ -1239,85 +1464,101 @@
     {
         "ClipRange": ClipRangeTypeDef,
         "Transition": UpdateProgramTransitionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateSourceLocationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSourceLocationRequestRequestTypeDef",
+CreateSourceLocationResponseOutputTypeDef = TypedDict(
+    "CreateSourceLocationResponseOutputTypeDef",
     {
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
+        "Arn": str,
+        "CreationTime": datetime,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateSourceLocationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSourceLocationRequestRequestTypeDef",
-    {
-        "AccessConfiguration": AccessConfigurationTypeDef,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
 
-class CreateSourceLocationRequestRequestTypeDef(
-    _RequiredCreateSourceLocationRequestRequestTypeDef,
-    _OptionalCreateSourceLocationRequestRequestTypeDef,
-):
-    pass
-
-CreateSourceLocationResponseTypeDef = TypedDict(
-    "CreateSourceLocationResponseTypeDef",
+DescribeSourceLocationResponseOutputTypeDef = TypedDict(
+    "DescribeSourceLocationResponseOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSourceLocationResponseTypeDef = TypedDict(
-    "DescribeSourceLocationResponseTypeDef",
+SourceLocationOutputTypeDef = TypedDict(
+    "SourceLocationOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SourceLocationTypeDef = TypedDict(
-    "SourceLocationTypeDef",
+UpdateSourceLocationResponseOutputTypeDef = TypedDict(
+    "UpdateSourceLocationResponseOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
+        "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
+        "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateSourceLocationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceLocationRequestRequestTypeDef",
+    {
+        "HttpConfiguration": HttpConfigurationTypeDef,
+        "SourceLocationName": str,
+    },
+)
+_OptionalCreateSourceLocationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceLocationRequestRequestTypeDef",
+    {
+        "AccessConfiguration": AccessConfigurationTypeDef,
+        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
+        "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateSourceLocationRequestRequestTypeDef(
+    _RequiredCreateSourceLocationRequestRequestTypeDef,
+    _OptionalCreateSourceLocationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1333,78 +1574,88 @@
 
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
-UpdateSourceLocationResponseTypeDef = TypedDict(
-    "UpdateSourceLocationResponseTypeDef",
+GetPlaybackConfigurationResponseOutputTypeDef = TypedDict(
+    "GetPlaybackConfigurationResponseOutputTypeDef",
     {
-        "AccessConfiguration": AccessConfigurationTypeDef,
-        "Arn": str,
-        "CreationTime": datetime,
-        "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
-        "HttpConfiguration": HttpConfigurationTypeDef,
-        "LastModifiedTime": datetime,
-        "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
-        "SourceLocationName": str,
+        "AdDecisionServerUrl": str,
+        "AvailSuppression": AvailSuppressionOutputTypeDef,
+        "Bumper": BumperOutputTypeDef,
+        "CdnConfiguration": CdnConfigurationOutputTypeDef,
+        "ConfigurationAliases": Dict[str, Dict[str, str]],
+        "DashConfiguration": DashConfigurationOutputTypeDef,
+        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
+        "Name": str,
+        "PersonalizationThresholdSeconds": int,
+        "PlaybackConfigurationArn": str,
+        "PlaybackEndpointPrefix": str,
+        "SessionInitializationEndpointPrefix": str,
+        "SlateAdUrl": str,
         "Tags": Dict[str, str],
+        "TranscodeProfileName": str,
+        "VideoContentSourceUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPlaybackConfigurationResponseTypeDef = TypedDict(
-    "GetPlaybackConfigurationResponseTypeDef",
+PlaybackConfigurationOutputTypeDef = TypedDict(
+    "PlaybackConfigurationOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
-        "AvailSuppression": AvailSuppressionTypeDef,
-        "Bumper": BumperTypeDef,
-        "CdnConfiguration": CdnConfigurationTypeDef,
+        "AvailSuppression": AvailSuppressionOutputTypeDef,
+        "Bumper": BumperOutputTypeDef,
+        "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationTypeDef,
-        "HlsConfiguration": HlsConfigurationTypeDef,
-        "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
-        "LogConfiguration": LogConfigurationTypeDef,
-        "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
+        "DashConfiguration": DashConfigurationOutputTypeDef,
+        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PlaybackConfigurationTypeDef = TypedDict(
-    "PlaybackConfigurationTypeDef",
+PutPlaybackConfigurationResponseOutputTypeDef = TypedDict(
+    "PutPlaybackConfigurationResponseOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
-        "AvailSuppression": AvailSuppressionTypeDef,
-        "Bumper": BumperTypeDef,
-        "CdnConfiguration": CdnConfigurationTypeDef,
+        "AvailSuppression": AvailSuppressionOutputTypeDef,
+        "Bumper": BumperOutputTypeDef,
+        "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationTypeDef,
-        "HlsConfiguration": HlsConfigurationTypeDef,
-        "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
-        "LogConfiguration": LogConfigurationTypeDef,
-        "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
+        "DashConfiguration": DashConfigurationOutputTypeDef,
+        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
@@ -1432,40 +1683,52 @@
 
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
-PutPlaybackConfigurationResponseTypeDef = TypedDict(
-    "PutPlaybackConfigurationResponseTypeDef",
+CreatePrefetchScheduleResponseOutputTypeDef = TypedDict(
+    "CreatePrefetchScheduleResponseOutputTypeDef",
     {
-        "AdDecisionServerUrl": str,
-        "AvailSuppression": AvailSuppressionTypeDef,
-        "Bumper": BumperTypeDef,
-        "CdnConfiguration": CdnConfigurationTypeDef,
-        "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationTypeDef,
-        "HlsConfiguration": HlsConfigurationTypeDef,
-        "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
-        "LogConfiguration": LogConfigurationTypeDef,
-        "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
+        "Arn": str,
+        "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
-        "PersonalizationThresholdSeconds": int,
-        "PlaybackConfigurationArn": str,
-        "PlaybackEndpointPrefix": str,
-        "SessionInitializationEndpointPrefix": str,
-        "SlateAdUrl": str,
-        "Tags": Dict[str, str],
-        "TranscodeProfileName": str,
-        "VideoContentSourceUrl": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalOutputTypeDef,
+        "StreamId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetPrefetchScheduleResponseOutputTypeDef = TypedDict(
+    "GetPrefetchScheduleResponseOutputTypeDef",
+    {
+        "Arn": str,
+        "Consumption": PrefetchConsumptionOutputTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalOutputTypeDef,
+        "StreamId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PrefetchScheduleOutputTypeDef = TypedDict(
+    "PrefetchScheduleOutputTypeDef",
+    {
+        "Arn": str,
+        "Consumption": PrefetchConsumptionOutputTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalOutputTypeDef,
+        "StreamId": str,
+    },
+)
+
 _RequiredCreatePrefetchScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
@@ -1481,66 +1744,97 @@
 
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
-CreatePrefetchScheduleResponseTypeDef = TypedDict(
-    "CreatePrefetchScheduleResponseTypeDef",
+ListLiveSourcesResponseOutputTypeDef = TypedDict(
+    "ListLiveSourcesResponseOutputTypeDef",
     {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalTypeDef,
-        "StreamId": str,
+        "Items": List[LiveSourceOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPrefetchScheduleResponseTypeDef = TypedDict(
-    "GetPrefetchScheduleResponseTypeDef",
+ListVodSourcesResponseOutputTypeDef = TypedDict(
+    "ListVodSourcesResponseOutputTypeDef",
     {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalTypeDef,
-        "StreamId": str,
+        "Items": List[VodSourceOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PrefetchScheduleTypeDef = TypedDict(
-    "PrefetchScheduleTypeDef",
+ChannelOutputTypeDef = TypedDict(
+    "ChannelOutputTypeDef",
     {
         "Arn": str,
-        "Consumption": PrefetchConsumptionTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalTypeDef,
-        "StreamId": str,
+        "ChannelName": str,
+        "ChannelState": str,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
     },
 )
 
-ListLiveSourcesResponseTypeDef = TypedDict(
-    "ListLiveSourcesResponseTypeDef",
+CreateChannelResponseOutputTypeDef = TypedDict(
+    "CreateChannelResponseOutputTypeDef",
     {
-        "Items": List[LiveSourceTypeDef],
-        "NextToken": str,
+        "Arn": str,
+        "ChannelName": str,
+        "ChannelState": ChannelStateType,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVodSourcesResponseTypeDef = TypedDict(
-    "ListVodSourcesResponseTypeDef",
+DescribeChannelResponseOutputTypeDef = TypedDict(
+    "DescribeChannelResponseOutputTypeDef",
     {
-        "Items": List[VodSourceTypeDef],
-        "NextToken": str,
+        "Arn": str,
+        "ChannelName": str,
+        "ChannelState": ChannelStateType,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateChannelResponseOutputTypeDef = TypedDict(
+    "UpdateChannelResponseOutputTypeDef",
+    {
+        "Arn": str,
+        "ChannelName": str,
+        "ChannelState": ChannelStateType,
+        "CreationTime": datetime,
+        "FillerSlate": SlateSourceOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "PlaybackMode": str,
+        "Tags": Dict[str, str],
+        "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
@@ -1580,89 +1874,32 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-ChannelTypeDef = TypedDict(
-    "ChannelTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": str,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelTypeDef,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
-    },
-)
-
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": ChannelStateType,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": ChannelStateType,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelTypeDef,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
+GetChannelScheduleResponseOutputTypeDef = TypedDict(
+    "GetChannelScheduleResponseOutputTypeDef",
     {
-        "Arn": str,
-        "ChannelName": str,
-        "ChannelState": ChannelStateType,
-        "CreationTime": datetime,
-        "FillerSlate": SlateSourceTypeDef,
-        "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tags": Dict[str, str],
-        "Tier": str,
+        "Items": List[ScheduleEntryOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetChannelScheduleResponseTypeDef = TypedDict(
-    "GetChannelScheduleResponseTypeDef",
+AdBreakOutputTypeDef = TypedDict(
+    "AdBreakOutputTypeDef",
     {
-        "Items": List[ScheduleEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AdBreakMetadata": List[KeyValuePairOutputTypeDef],
+        "MessageType": MessageTypeType,
+        "OffsetMillis": int,
+        "Slate": SlateSourceOutputTypeDef,
+        "SpliceInsertMessage": SpliceInsertMessageOutputTypeDef,
+        "TimeSignalMessage": TimeSignalMessageOutputTypeDef,
     },
 )
 
 AdBreakTypeDef = TypedDict(
     "AdBreakTypeDef",
     {
         "AdBreakMetadata": Sequence[KeyValuePairTypeDef],
@@ -1671,110 +1908,128 @@
         "Slate": SlateSourceTypeDef,
         "SpliceInsertMessage": SpliceInsertMessageTypeDef,
         "TimeSignalMessage": TimeSignalMessageTypeDef,
     },
     total=False,
 )
 
-ListSourceLocationsResponseTypeDef = TypedDict(
-    "ListSourceLocationsResponseTypeDef",
+ListSourceLocationsResponseOutputTypeDef = TypedDict(
+    "ListSourceLocationsResponseOutputTypeDef",
     {
-        "Items": List[SourceLocationTypeDef],
+        "Items": List[SourceLocationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPlaybackConfigurationsResponseTypeDef = TypedDict(
-    "ListPlaybackConfigurationsResponseTypeDef",
+ListPlaybackConfigurationsResponseOutputTypeDef = TypedDict(
+    "ListPlaybackConfigurationsResponseOutputTypeDef",
     {
-        "Items": List[PlaybackConfigurationTypeDef],
+        "Items": List[PlaybackConfigurationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPrefetchSchedulesResponseTypeDef = TypedDict(
-    "ListPrefetchSchedulesResponseTypeDef",
+ListPrefetchSchedulesResponseOutputTypeDef = TypedDict(
+    "ListPrefetchSchedulesResponseOutputTypeDef",
     {
-        "Items": List[PrefetchScheduleTypeDef],
+        "Items": List[PrefetchScheduleOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListChannelsResponseTypeDef = TypedDict(
-    "ListChannelsResponseTypeDef",
+ListChannelsResponseOutputTypeDef = TypedDict(
+    "ListChannelsResponseOutputTypeDef",
     {
-        "Items": List[ChannelTypeDef],
+        "Items": List[ChannelOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProgramRequestRequestTypeDef",
+CreateProgramResponseOutputTypeDef = TypedDict(
+    "CreateProgramResponseOutputTypeDef",
     {
+        "AdBreaks": List[AdBreakOutputTypeDef],
+        "Arn": str,
         "ChannelName": str,
+        "ClipRange": ClipRangeOutputTypeDef,
+        "CreationTime": datetime,
+        "DurationMillis": int,
+        "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "ScheduledStartTime": datetime,
         "SourceLocationName": str,
-    },
-)
-_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProgramRequestRequestTypeDef",
-    {
-        "AdBreaks": Sequence[AdBreakTypeDef],
-        "LiveSourceName": str,
         "VodSourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class CreateProgramRequestRequestTypeDef(
-    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
-):
-    pass
-
-CreateProgramResponseTypeDef = TypedDict(
-    "CreateProgramResponseTypeDef",
+DescribeProgramResponseOutputTypeDef = TypedDict(
+    "DescribeProgramResponseOutputTypeDef",
     {
-        "AdBreaks": List[AdBreakTypeDef],
+        "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
+        "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeProgramResponseTypeDef = TypedDict(
-    "DescribeProgramResponseTypeDef",
+UpdateProgramResponseOutputTypeDef = TypedDict(
+    "UpdateProgramResponseOutputTypeDef",
     {
-        "AdBreaks": List[AdBreakTypeDef],
+        "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
+        "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProgramRequestRequestTypeDef",
+    {
+        "ChannelName": str,
+        "ProgramName": str,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "SourceLocationName": str,
+    },
+)
+_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProgramRequestRequestTypeDef",
+    {
+        "AdBreaks": Sequence[AdBreakTypeDef],
+        "LiveSourceName": str,
+        "VodSourceName": str,
+    },
+    total=False,
+)
+
+class CreateProgramRequestRequestTypeDef(
+    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
         "ProgramName": str,
         "ScheduleConfiguration": UpdateProgramScheduleConfigurationTypeDef,
     },
@@ -1787,25 +2042,7 @@
     total=False,
 )
 
 class UpdateProgramRequestRequestTypeDef(
     _RequiredUpdateProgramRequestRequestTypeDef, _OptionalUpdateProgramRequestRequestTypeDef
 ):
     pass
-
-UpdateProgramResponseTypeDef = TypedDict(
-    "UpdateProgramResponseTypeDef",
-    {
-        "AdBreaks": List[AdBreakTypeDef],
-        "Arn": str,
-        "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
-        "CreationTime": datetime,
-        "DurationMillis": int,
-        "LiveSourceName": str,
-        "ProgramName": str,
-        "ScheduledStartTime": datetime,
-        "SourceLocationName": str,
-        "VodSourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/PKG-INFO` & `mypy-boto3-mediatailor-1.28.3.post1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-mediatailor
-Version: 1.28.3
-Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.6
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediatailor type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-mediatailor"></a>
 
 # mypy-boto3-mediatailor
 
 [![PyPI - mypy-boto3-mediatailor](https://img.shields.io/pypi/v/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
@@ -47,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,37 +332,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediatailor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediatailor.type_defs import (
+    SecretsManagerAccessTokenConfigurationOutputTypeDef,
     SecretsManagerAccessTokenConfigurationTypeDef,
+    KeyValuePairOutputTypeDef,
+    SlateSourceOutputTypeDef,
+    SpliceInsertMessageOutputTypeDef,
     KeyValuePairTypeDef,
     SlateSourceTypeDef,
     SpliceInsertMessageTypeDef,
+    AdMarkerPassthroughOutputTypeDef,
     AdMarkerPassthroughTypeDef,
-    AlertTypeDef,
+    AlertOutputTypeDef,
+    AvailMatchingCriteriaOutputTypeDef,
     AvailMatchingCriteriaTypeDef,
+    AvailSuppressionOutputTypeDef,
     AvailSuppressionTypeDef,
+    BumperOutputTypeDef,
     BumperTypeDef,
+    CdnConfigurationOutputTypeDef,
     CdnConfigurationTypeDef,
-    LogConfigurationForChannelTypeDef,
+    LogConfigurationForChannelOutputTypeDef,
+    ClipRangeOutputTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
+    ConfigureLogsForChannelResponseOutputTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
     HttpPackageConfigurationTypeDef,
+    HttpPackageConfigurationOutputTypeDef,
     PrefetchRetrievalTypeDef,
+    PrefetchRetrievalOutputTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
+    DefaultSegmentDeliveryConfigurationOutputTypeDef,
+    HttpConfigurationOutputTypeDef,
+    SegmentDeliveryConfigurationOutputTypeDef,
     DashConfigurationForPutTypeDef,
-    DashConfigurationTypeDef,
+    DashConfigurationOutputTypeDef,
+    DashPlaylistSettingsOutputTypeDef,
     DashPlaylistSettingsTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteLiveSourceRequestRequestTypeDef,
     DeletePlaybackConfigurationRequestRequestTypeDef,
     DeletePrefetchScheduleRequestRequestTypeDef,
     DeleteProgramRequestRequestTypeDef,
@@ -403,109 +387,117 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseTypeDef,
+    GetChannelPolicyResponseOutputTypeDef,
     GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
-    HlsConfigurationTypeDef,
-    LivePreRollConfigurationTypeDef,
-    LogConfigurationTypeDef,
+    HlsConfigurationOutputTypeDef,
+    LivePreRollConfigurationOutputTypeDef,
+    LogConfigurationOutputTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
+    HlsPlaylistSettingsOutputTypeDef,
     HlsPlaylistSettingsTypeDef,
     ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     ListLiveSourcesRequestRequestTypeDef,
     ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
     ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
+    LivePreRollConfigurationTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    ScheduleAdBreakTypeDef,
+    ScheduleAdBreakOutputTypeDef,
     TransitionTypeDef,
+    SegmentationDescriptorOutputTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
+    AccessConfigurationOutputTypeDef,
     AccessConfigurationTypeDef,
+    ManifestProcessingRulesOutputTypeDef,
     ManifestProcessingRulesTypeDef,
-    ListAlertsResponseTypeDef,
+    ListAlertsResponseOutputTypeDef,
+    PrefetchConsumptionOutputTypeDef,
     PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
-    CreateLiveSourceResponseTypeDef,
     CreateVodSourceRequestRequestTypeDef,
-    CreateVodSourceResponseTypeDef,
-    DescribeLiveSourceResponseTypeDef,
-    DescribeVodSourceResponseTypeDef,
-    LiveSourceTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
-    UpdateLiveSourceResponseTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
-    UpdateVodSourceResponseTypeDef,
-    VodSourceTypeDef,
+    CreateLiveSourceResponseOutputTypeDef,
+    CreateVodSourceResponseOutputTypeDef,
+    DescribeLiveSourceResponseOutputTypeDef,
+    DescribeVodSourceResponseOutputTypeDef,
+    LiveSourceOutputTypeDef,
+    UpdateLiveSourceResponseOutputTypeDef,
+    UpdateVodSourceResponseOutputTypeDef,
+    VodSourceOutputTypeDef,
+    ResponseOutputItemOutputTypeDef,
     RequestOutputItemTypeDef,
-    ResponseOutputItemTypeDef,
-    ScheduleEntryTypeDef,
+    ScheduleEntryOutputTypeDef,
     ScheduleConfigurationTypeDef,
+    TimeSignalMessageOutputTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
+    CreateSourceLocationResponseOutputTypeDef,
+    DescribeSourceLocationResponseOutputTypeDef,
+    SourceLocationOutputTypeDef,
+    UpdateSourceLocationResponseOutputTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
-    CreateSourceLocationResponseTypeDef,
-    DescribeSourceLocationResponseTypeDef,
-    SourceLocationTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
-    UpdateSourceLocationResponseTypeDef,
-    GetPlaybackConfigurationResponseTypeDef,
-    PlaybackConfigurationTypeDef,
+    GetPlaybackConfigurationResponseOutputTypeDef,
+    PlaybackConfigurationOutputTypeDef,
+    PutPlaybackConfigurationResponseOutputTypeDef,
     PutPlaybackConfigurationRequestRequestTypeDef,
-    PutPlaybackConfigurationResponseTypeDef,
+    CreatePrefetchScheduleResponseOutputTypeDef,
+    GetPrefetchScheduleResponseOutputTypeDef,
+    PrefetchScheduleOutputTypeDef,
     CreatePrefetchScheduleRequestRequestTypeDef,
-    CreatePrefetchScheduleResponseTypeDef,
-    GetPrefetchScheduleResponseTypeDef,
-    PrefetchScheduleTypeDef,
-    ListLiveSourcesResponseTypeDef,
-    ListVodSourcesResponseTypeDef,
+    ListLiveSourcesResponseOutputTypeDef,
+    ListVodSourcesResponseOutputTypeDef,
+    ChannelOutputTypeDef,
+    CreateChannelResponseOutputTypeDef,
+    DescribeChannelResponseOutputTypeDef,
+    UpdateChannelResponseOutputTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    ChannelTypeDef,
-    CreateChannelResponseTypeDef,
-    DescribeChannelResponseTypeDef,
-    UpdateChannelResponseTypeDef,
-    GetChannelScheduleResponseTypeDef,
+    GetChannelScheduleResponseOutputTypeDef,
+    AdBreakOutputTypeDef,
     AdBreakTypeDef,
-    ListSourceLocationsResponseTypeDef,
-    ListPlaybackConfigurationsResponseTypeDef,
-    ListPrefetchSchedulesResponseTypeDef,
-    ListChannelsResponseTypeDef,
+    ListSourceLocationsResponseOutputTypeDef,
+    ListPlaybackConfigurationsResponseOutputTypeDef,
+    ListPrefetchSchedulesResponseOutputTypeDef,
+    ListChannelsResponseOutputTypeDef,
+    CreateProgramResponseOutputTypeDef,
+    DescribeProgramResponseOutputTypeDef,
+    UpdateProgramResponseOutputTypeDef,
     CreateProgramRequestRequestTypeDef,
-    CreateProgramResponseTypeDef,
-    DescribeProgramResponseTypeDef,
     UpdateProgramRequestRequestTypeDef,
-    UpdateProgramResponseTypeDef,
 )
 
 
-def get_structure() -> SecretsManagerAccessTokenConfigurationTypeDef:
+def get_structure() -> SecretsManagerAccessTokenConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/SOURCES.txt` & `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3/setup.py` & `mypy-boto3-mediatailor-1.28.3.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediatailor",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_mediatailor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder"
-        " 7.14.6"
+        " 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

