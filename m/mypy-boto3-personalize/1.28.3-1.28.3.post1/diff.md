# Comparing `tmp/mypy-boto3-personalize-1.28.3.tar.gz` & `tmp/mypy-boto3-personalize-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
```

## Comparing `mypy-boto3-personalize-1.28.3.tar` & `mypy-boto3-personalize-1.28.3.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.177303 mypy-boto3-personalize-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-13 19:49:15.173303 mypy-boto3-personalize-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.169303 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51525 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51435 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18725 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62479 2023-07-13 19:48:22.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62446 2023-07-13 19:48:21.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.173303 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.177303 mypy-boto3-personalize-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.999730 mypy-boto3-personalize-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-14 16:18:02.995730 mypy-boto3-personalize-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23266 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.983729 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52241 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52151 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66438 2023-07-14 16:16:56.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66405 2023-07-14 16:16:55.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.995730 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:02.999730 mypy-boto3-personalize-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-14 16:16:52.000000 mypy-boto3-personalize-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-personalize-1.28.3/LICENSE` & `mypy-boto3-personalize-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3/PKG-INFO` & `mypy-boto3-personalize-1.28.3.post1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-personalize
-Version: 1.28.3
-Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.6
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 personalize type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-personalize"></a>
 
 # mypy-boto3-personalize
 
 [![PyPI - mypy-boto3-personalize](https://img.shields.io/pypi/v/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,54 +357,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize.type_defs import (
-    AlgorithmImageTypeDef,
+    AlgorithmImageOutputTypeDef,
+    AutoMLConfigOutputTypeDef,
     AutoMLConfigTypeDef,
-    AutoMLResultTypeDef,
+    AutoMLResultOutputTypeDef,
     BatchInferenceJobConfigTypeDef,
     S3DataConfigTypeDef,
-    BatchInferenceJobSummaryTypeDef,
-    BatchSegmentJobSummaryTypeDef,
+    BatchInferenceJobSummaryOutputTypeDef,
+    BatchSegmentJobSummaryOutputTypeDef,
+    CampaignConfigOutputTypeDef,
     CampaignConfigTypeDef,
-    CampaignSummaryTypeDef,
+    CampaignSummaryOutputTypeDef,
+    CategoricalHyperParameterRangeOutputTypeDef,
     CategoricalHyperParameterRangeTypeDef,
+    ContinuousHyperParameterRangeOutputTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
+    CreateBatchInferenceJobResponseOutputTypeDef,
+    CreateBatchSegmentJobResponseOutputTypeDef,
+    CreateCampaignResponseOutputTypeDef,
+    CreateDatasetExportJobResponseOutputTypeDef,
+    CreateDatasetGroupResponseOutputTypeDef,
     DataSourceTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
+    CreateDatasetImportJobResponseOutputTypeDef,
+    CreateDatasetResponseOutputTypeDef,
+    CreateEventTrackerResponseOutputTypeDef,
+    CreateFilterResponseOutputTypeDef,
     MetricAttributeTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
+    CreateMetricAttributionResponseOutputTypeDef,
+    CreateRecommenderResponseOutputTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
-    DatasetExportJobSummaryTypeDef,
-    DatasetGroupSummaryTypeDef,
-    DatasetGroupTypeDef,
-    DatasetImportJobSummaryTypeDef,
-    DatasetSchemaSummaryTypeDef,
-    DatasetSchemaTypeDef,
-    DatasetSummaryTypeDef,
-    DatasetUpdateSummaryTypeDef,
-    DefaultCategoricalHyperParameterRangeTypeDef,
-    DefaultContinuousHyperParameterRangeTypeDef,
-    DefaultIntegerHyperParameterRangeTypeDef,
+    CreateSchemaResponseOutputTypeDef,
+    CreateSolutionResponseOutputTypeDef,
+    CreateSolutionVersionResponseOutputTypeDef,
+    DataSourceOutputTypeDef,
+    DatasetExportJobSummaryOutputTypeDef,
+    DatasetGroupOutputTypeDef,
+    DatasetGroupSummaryOutputTypeDef,
+    DatasetImportJobSummaryOutputTypeDef,
+    DatasetUpdateSummaryOutputTypeDef,
+    DatasetSchemaOutputTypeDef,
+    DatasetSchemaSummaryOutputTypeDef,
+    DatasetSummaryOutputTypeDef,
+    DefaultCategoricalHyperParameterRangeOutputTypeDef,
+    DefaultContinuousHyperParameterRangeOutputTypeDef,
+    DefaultIntegerHyperParameterRangeOutputTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteMetricAttributionRequestRequestTypeDef,
     DeleteRecommenderRequestRequestTypeDef,
@@ -447,33 +420,36 @@
     DescribeBatchSegmentJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DescribeDatasetExportJobRequestRequestTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeEventTrackerRequestRequestTypeDef,
-    EventTrackerTypeDef,
+    EventTrackerOutputTypeDef,
     DescribeFeatureTransformationRequestRequestTypeDef,
-    FeatureTransformationTypeDef,
+    FeatureTransformationOutputTypeDef,
     DescribeFilterRequestRequestTypeDef,
-    FilterTypeDef,
+    FilterOutputTypeDef,
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
-    RecipeTypeDef,
+    RecipeOutputTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventTrackerSummaryTypeDef,
-    FilterSummaryTypeDef,
+    EventTrackerSummaryOutputTypeDef,
+    FilterSummaryOutputTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
-    GetSolutionMetricsResponseTypeDef,
+    GetSolutionMetricsResponseOutputTypeDef,
+    HPOObjectiveOutputTypeDef,
+    HPOResourceConfigOutputTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
+    IntegerHyperParameterRangeOutputTypeDef,
     IntegerHyperParameterRangeTypeDef,
     ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
     ListBatchInferenceJobsRequestRequestTypeDef,
     ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
     ListBatchSegmentJobsRequestRequestTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
@@ -487,127 +463,131 @@
     ListDatasetsRequestRequestTypeDef,
     ListEventTrackersRequestListEventTrackersPaginateTypeDef,
     ListEventTrackersRequestRequestTypeDef,
     ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
+    MetricAttributeOutputTypeDef,
     ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
-    MetricAttributionSummaryTypeDef,
+    MetricAttributionSummaryOutputTypeDef,
     ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    RecipeSummaryTypeDef,
+    RecipeSummaryOutputTypeDef,
     ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
-    SolutionVersionSummaryTypeDef,
+    SolutionVersionSummaryOutputTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
-    SolutionSummaryTypeDef,
+    SolutionSummaryOutputTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OptimizationObjectiveOutputTypeDef,
     OptimizationObjectiveTypeDef,
     PaginatorConfigTypeDef,
+    TrainingDataConfigOutputTypeDef,
     TrainingDataConfigTypeDef,
     ResponseMetadataTypeDef,
-    TunedHPOParamsTypeDef,
+    TunedHPOParamsOutputTypeDef,
     StartRecommenderRequestRequestTypeDef,
-    StartRecommenderResponseTypeDef,
+    StartRecommenderResponseOutputTypeDef,
     StopRecommenderRequestRequestTypeDef,
-    StopRecommenderResponseTypeDef,
+    StopRecommenderResponseOutputTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCampaignResponseTypeDef,
+    UpdateCampaignResponseOutputTypeDef,
     UpdateDatasetRequestRequestTypeDef,
-    UpdateDatasetResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    UpdateDatasetResponseOutputTypeDef,
+    UpdateMetricAttributionResponseOutputTypeDef,
+    UpdateRecommenderResponseOutputTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    CampaignUpdateSummaryTypeDef,
+    ListBatchInferenceJobsResponseOutputTypeDef,
+    ListBatchSegmentJobsResponseOutputTypeDef,
+    CampaignUpdateSummaryOutputTypeDef,
     UpdateCampaignRequestRequestTypeDef,
-    ListCampaignsResponseTypeDef,
+    ListCampaignsResponseOutputTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
-    DatasetImportJobTypeDef,
-    ListMetricAttributionMetricsResponseTypeDef,
-    ListDatasetExportJobsResponseTypeDef,
-    ListDatasetGroupsResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    ListDatasetImportJobsResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    DatasetTypeDef,
-    DefaultHyperParameterRangesTypeDef,
-    DescribeEventTrackerResponseTypeDef,
-    DescribeFeatureTransformationResponseTypeDef,
-    DescribeFilterResponseTypeDef,
-    DescribeRecipeResponseTypeDef,
-    ListEventTrackersResponseTypeDef,
-    ListFiltersResponseTypeDef,
+    DatasetImportJobOutputTypeDef,
+    ListDatasetExportJobsResponseOutputTypeDef,
+    DescribeDatasetGroupResponseOutputTypeDef,
+    ListDatasetGroupsResponseOutputTypeDef,
+    ListDatasetImportJobsResponseOutputTypeDef,
+    DatasetOutputTypeDef,
+    DescribeSchemaResponseOutputTypeDef,
+    ListSchemasResponseOutputTypeDef,
+    ListDatasetsResponseOutputTypeDef,
+    DefaultHyperParameterRangesOutputTypeDef,
+    DescribeEventTrackerResponseOutputTypeDef,
+    DescribeFeatureTransformationResponseOutputTypeDef,
+    DescribeFilterResponseOutputTypeDef,
+    DescribeRecipeResponseOutputTypeDef,
+    ListEventTrackersResponseOutputTypeDef,
+    ListFiltersResponseOutputTypeDef,
+    HyperParameterRangesOutputTypeDef,
     HyperParameterRangesTypeDef,
-    ListMetricAttributionsResponseTypeDef,
-    ListRecipesResponseTypeDef,
-    ListSolutionVersionsResponseTypeDef,
-    ListSolutionsResponseTypeDef,
+    ListMetricAttributionMetricsResponseOutputTypeDef,
+    ListMetricAttributionsResponseOutputTypeDef,
+    ListRecipesResponseOutputTypeDef,
+    ListSolutionVersionsResponseOutputTypeDef,
+    ListSolutionsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    RecommenderConfigOutputTypeDef,
     RecommenderConfigTypeDef,
-    BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
-    BatchSegmentJobTypeDef,
+    DescribeBatchInferenceJobResponseOutputTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
+    DescribeBatchSegmentJobResponseOutputTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
-    DatasetExportJobTypeDef,
+    DescribeDatasetExportJobResponseOutputTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
-    MetricAttributionTypeDef,
+    DescribeMetricAttributionResponseOutputTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
-    CampaignTypeDef,
-    DescribeDatasetImportJobResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    AlgorithmTypeDef,
+    CampaignOutputTypeDef,
+    DescribeDatasetImportJobResponseOutputTypeDef,
+    DescribeDatasetResponseOutputTypeDef,
+    AlgorithmOutputTypeDef,
+    HPOConfigOutputTypeDef,
     HPOConfigTypeDef,
+    RecommenderSummaryOutputTypeDef,
+    RecommenderUpdateSummaryOutputTypeDef,
     CreateRecommenderRequestRequestTypeDef,
-    RecommenderSummaryTypeDef,
-    RecommenderUpdateSummaryTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
-    DescribeBatchInferenceJobResponseTypeDef,
-    DescribeBatchSegmentJobResponseTypeDef,
-    DescribeDatasetExportJobResponseTypeDef,
-    DescribeMetricAttributionResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-    DescribeAlgorithmResponseTypeDef,
+    DescribeCampaignResponseOutputTypeDef,
+    DescribeAlgorithmResponseOutputTypeDef,
+    SolutionConfigOutputTypeDef,
     SolutionConfigTypeDef,
-    ListRecommendersResponseTypeDef,
-    RecommenderTypeDef,
+    ListRecommendersResponseOutputTypeDef,
+    RecommenderOutputTypeDef,
+    SolutionOutputTypeDef,
+    SolutionVersionOutputTypeDef,
     CreateSolutionRequestRequestTypeDef,
-    SolutionTypeDef,
-    SolutionVersionTypeDef,
-    DescribeRecommenderResponseTypeDef,
-    DescribeSolutionResponseTypeDef,
-    DescribeSolutionVersionResponseTypeDef,
+    DescribeRecommenderResponseOutputTypeDef,
+    DescribeSolutionResponseOutputTypeDef,
+    DescribeSolutionVersionResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AlgorithmImageTypeDef:
+def get_structure() -> AlgorithmImageOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-1.28.3/README.md` & `mypy-boto3-personalize-1.28.3.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-personalize
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 personalize type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-personalize"></a>
 
 # mypy-boto3-personalize
 
 [![PyPI - mypy-boto3-personalize](https://img.shields.io/pypi/v/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,54 +389,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize.type_defs import (
-    AlgorithmImageTypeDef,
+    AlgorithmImageOutputTypeDef,
+    AutoMLConfigOutputTypeDef,
     AutoMLConfigTypeDef,
-    AutoMLResultTypeDef,
+    AutoMLResultOutputTypeDef,
     BatchInferenceJobConfigTypeDef,
     S3DataConfigTypeDef,
-    BatchInferenceJobSummaryTypeDef,
-    BatchSegmentJobSummaryTypeDef,
+    BatchInferenceJobSummaryOutputTypeDef,
+    BatchSegmentJobSummaryOutputTypeDef,
+    CampaignConfigOutputTypeDef,
     CampaignConfigTypeDef,
-    CampaignSummaryTypeDef,
+    CampaignSummaryOutputTypeDef,
+    CategoricalHyperParameterRangeOutputTypeDef,
     CategoricalHyperParameterRangeTypeDef,
+    ContinuousHyperParameterRangeOutputTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
+    CreateBatchInferenceJobResponseOutputTypeDef,
+    CreateBatchSegmentJobResponseOutputTypeDef,
+    CreateCampaignResponseOutputTypeDef,
+    CreateDatasetExportJobResponseOutputTypeDef,
+    CreateDatasetGroupResponseOutputTypeDef,
     DataSourceTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
+    CreateDatasetImportJobResponseOutputTypeDef,
+    CreateDatasetResponseOutputTypeDef,
+    CreateEventTrackerResponseOutputTypeDef,
+    CreateFilterResponseOutputTypeDef,
     MetricAttributeTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
+    CreateMetricAttributionResponseOutputTypeDef,
+    CreateRecommenderResponseOutputTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
-    DatasetExportJobSummaryTypeDef,
-    DatasetGroupSummaryTypeDef,
-    DatasetGroupTypeDef,
-    DatasetImportJobSummaryTypeDef,
-    DatasetSchemaSummaryTypeDef,
-    DatasetSchemaTypeDef,
-    DatasetSummaryTypeDef,
-    DatasetUpdateSummaryTypeDef,
-    DefaultCategoricalHyperParameterRangeTypeDef,
-    DefaultContinuousHyperParameterRangeTypeDef,
-    DefaultIntegerHyperParameterRangeTypeDef,
+    CreateSchemaResponseOutputTypeDef,
+    CreateSolutionResponseOutputTypeDef,
+    CreateSolutionVersionResponseOutputTypeDef,
+    DataSourceOutputTypeDef,
+    DatasetExportJobSummaryOutputTypeDef,
+    DatasetGroupOutputTypeDef,
+    DatasetGroupSummaryOutputTypeDef,
+    DatasetImportJobSummaryOutputTypeDef,
+    DatasetUpdateSummaryOutputTypeDef,
+    DatasetSchemaOutputTypeDef,
+    DatasetSchemaSummaryOutputTypeDef,
+    DatasetSummaryOutputTypeDef,
+    DefaultCategoricalHyperParameterRangeOutputTypeDef,
+    DefaultContinuousHyperParameterRangeOutputTypeDef,
+    DefaultIntegerHyperParameterRangeOutputTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteMetricAttributionRequestRequestTypeDef,
     DeleteRecommenderRequestRequestTypeDef,
@@ -415,33 +452,36 @@
     DescribeBatchSegmentJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DescribeDatasetExportJobRequestRequestTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeEventTrackerRequestRequestTypeDef,
-    EventTrackerTypeDef,
+    EventTrackerOutputTypeDef,
     DescribeFeatureTransformationRequestRequestTypeDef,
-    FeatureTransformationTypeDef,
+    FeatureTransformationOutputTypeDef,
     DescribeFilterRequestRequestTypeDef,
-    FilterTypeDef,
+    FilterOutputTypeDef,
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
-    RecipeTypeDef,
+    RecipeOutputTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventTrackerSummaryTypeDef,
-    FilterSummaryTypeDef,
+    EventTrackerSummaryOutputTypeDef,
+    FilterSummaryOutputTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
-    GetSolutionMetricsResponseTypeDef,
+    GetSolutionMetricsResponseOutputTypeDef,
+    HPOObjectiveOutputTypeDef,
+    HPOResourceConfigOutputTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
+    IntegerHyperParameterRangeOutputTypeDef,
     IntegerHyperParameterRangeTypeDef,
     ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
     ListBatchInferenceJobsRequestRequestTypeDef,
     ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
     ListBatchSegmentJobsRequestRequestTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
@@ -455,127 +495,131 @@
     ListDatasetsRequestRequestTypeDef,
     ListEventTrackersRequestListEventTrackersPaginateTypeDef,
     ListEventTrackersRequestRequestTypeDef,
     ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
+    MetricAttributeOutputTypeDef,
     ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
-    MetricAttributionSummaryTypeDef,
+    MetricAttributionSummaryOutputTypeDef,
     ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    RecipeSummaryTypeDef,
+    RecipeSummaryOutputTypeDef,
     ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
-    SolutionVersionSummaryTypeDef,
+    SolutionVersionSummaryOutputTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
-    SolutionSummaryTypeDef,
+    SolutionSummaryOutputTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OptimizationObjectiveOutputTypeDef,
     OptimizationObjectiveTypeDef,
     PaginatorConfigTypeDef,
+    TrainingDataConfigOutputTypeDef,
     TrainingDataConfigTypeDef,
     ResponseMetadataTypeDef,
-    TunedHPOParamsTypeDef,
+    TunedHPOParamsOutputTypeDef,
     StartRecommenderRequestRequestTypeDef,
-    StartRecommenderResponseTypeDef,
+    StartRecommenderResponseOutputTypeDef,
     StopRecommenderRequestRequestTypeDef,
-    StopRecommenderResponseTypeDef,
+    StopRecommenderResponseOutputTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCampaignResponseTypeDef,
+    UpdateCampaignResponseOutputTypeDef,
     UpdateDatasetRequestRequestTypeDef,
-    UpdateDatasetResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    UpdateDatasetResponseOutputTypeDef,
+    UpdateMetricAttributionResponseOutputTypeDef,
+    UpdateRecommenderResponseOutputTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    CampaignUpdateSummaryTypeDef,
+    ListBatchInferenceJobsResponseOutputTypeDef,
+    ListBatchSegmentJobsResponseOutputTypeDef,
+    CampaignUpdateSummaryOutputTypeDef,
     UpdateCampaignRequestRequestTypeDef,
-    ListCampaignsResponseTypeDef,
+    ListCampaignsResponseOutputTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
-    DatasetImportJobTypeDef,
-    ListMetricAttributionMetricsResponseTypeDef,
-    ListDatasetExportJobsResponseTypeDef,
-    ListDatasetGroupsResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    ListDatasetImportJobsResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    DatasetTypeDef,
-    DefaultHyperParameterRangesTypeDef,
-    DescribeEventTrackerResponseTypeDef,
-    DescribeFeatureTransformationResponseTypeDef,
-    DescribeFilterResponseTypeDef,
-    DescribeRecipeResponseTypeDef,
-    ListEventTrackersResponseTypeDef,
-    ListFiltersResponseTypeDef,
+    DatasetImportJobOutputTypeDef,
+    ListDatasetExportJobsResponseOutputTypeDef,
+    DescribeDatasetGroupResponseOutputTypeDef,
+    ListDatasetGroupsResponseOutputTypeDef,
+    ListDatasetImportJobsResponseOutputTypeDef,
+    DatasetOutputTypeDef,
+    DescribeSchemaResponseOutputTypeDef,
+    ListSchemasResponseOutputTypeDef,
+    ListDatasetsResponseOutputTypeDef,
+    DefaultHyperParameterRangesOutputTypeDef,
+    DescribeEventTrackerResponseOutputTypeDef,
+    DescribeFeatureTransformationResponseOutputTypeDef,
+    DescribeFilterResponseOutputTypeDef,
+    DescribeRecipeResponseOutputTypeDef,
+    ListEventTrackersResponseOutputTypeDef,
+    ListFiltersResponseOutputTypeDef,
+    HyperParameterRangesOutputTypeDef,
     HyperParameterRangesTypeDef,
-    ListMetricAttributionsResponseTypeDef,
-    ListRecipesResponseTypeDef,
-    ListSolutionVersionsResponseTypeDef,
-    ListSolutionsResponseTypeDef,
+    ListMetricAttributionMetricsResponseOutputTypeDef,
+    ListMetricAttributionsResponseOutputTypeDef,
+    ListRecipesResponseOutputTypeDef,
+    ListSolutionVersionsResponseOutputTypeDef,
+    ListSolutionsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    RecommenderConfigOutputTypeDef,
     RecommenderConfigTypeDef,
-    BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
-    BatchSegmentJobTypeDef,
+    DescribeBatchInferenceJobResponseOutputTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
+    DescribeBatchSegmentJobResponseOutputTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
-    DatasetExportJobTypeDef,
+    DescribeDatasetExportJobResponseOutputTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
-    MetricAttributionTypeDef,
+    DescribeMetricAttributionResponseOutputTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
-    CampaignTypeDef,
-    DescribeDatasetImportJobResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    AlgorithmTypeDef,
+    CampaignOutputTypeDef,
+    DescribeDatasetImportJobResponseOutputTypeDef,
+    DescribeDatasetResponseOutputTypeDef,
+    AlgorithmOutputTypeDef,
+    HPOConfigOutputTypeDef,
     HPOConfigTypeDef,
+    RecommenderSummaryOutputTypeDef,
+    RecommenderUpdateSummaryOutputTypeDef,
     CreateRecommenderRequestRequestTypeDef,
-    RecommenderSummaryTypeDef,
-    RecommenderUpdateSummaryTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
-    DescribeBatchInferenceJobResponseTypeDef,
-    DescribeBatchSegmentJobResponseTypeDef,
-    DescribeDatasetExportJobResponseTypeDef,
-    DescribeMetricAttributionResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-    DescribeAlgorithmResponseTypeDef,
+    DescribeCampaignResponseOutputTypeDef,
+    DescribeAlgorithmResponseOutputTypeDef,
+    SolutionConfigOutputTypeDef,
     SolutionConfigTypeDef,
-    ListRecommendersResponseTypeDef,
-    RecommenderTypeDef,
+    ListRecommendersResponseOutputTypeDef,
+    RecommenderOutputTypeDef,
+    SolutionOutputTypeDef,
+    SolutionVersionOutputTypeDef,
     CreateSolutionRequestRequestTypeDef,
-    SolutionTypeDef,
-    SolutionVersionTypeDef,
-    DescribeRecommenderResponseTypeDef,
-    DescribeSolutionResponseTypeDef,
-    DescribeSolutionVersionResponseTypeDef,
+    DescribeRecommenderResponseOutputTypeDef,
+    DescribeSolutionResponseOutputTypeDef,
+    DescribeSolutionVersionResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AlgorithmImageTypeDef:
+def get_structure() -> AlgorithmImageOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.py` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.pyi` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__main__.py` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Personalize 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.Personalize 1.28.3\nVersion:         1.28.3.post1\nBuilder"
+        " version: 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
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

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.py` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,77 +40,77 @@
 from .type_defs import (
     BatchInferenceJobConfigTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     CampaignConfigTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
+    CreateBatchInferenceJobResponseOutputTypeDef,
+    CreateBatchSegmentJobResponseOutputTypeDef,
+    CreateCampaignResponseOutputTypeDef,
+    CreateDatasetExportJobResponseOutputTypeDef,
+    CreateDatasetGroupResponseOutputTypeDef,
+    CreateDatasetImportJobResponseOutputTypeDef,
+    CreateDatasetResponseOutputTypeDef,
+    CreateEventTrackerResponseOutputTypeDef,
+    CreateFilterResponseOutputTypeDef,
+    CreateMetricAttributionResponseOutputTypeDef,
+    CreateRecommenderResponseOutputTypeDef,
+    CreateSchemaResponseOutputTypeDef,
+    CreateSolutionResponseOutputTypeDef,
+    CreateSolutionVersionResponseOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     DataSourceTypeDef,
-    DescribeAlgorithmResponseTypeDef,
-    DescribeBatchInferenceJobResponseTypeDef,
-    DescribeBatchSegmentJobResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-    DescribeDatasetExportJobResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    DescribeDatasetImportJobResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    DescribeEventTrackerResponseTypeDef,
-    DescribeFeatureTransformationResponseTypeDef,
-    DescribeFilterResponseTypeDef,
-    DescribeMetricAttributionResponseTypeDef,
-    DescribeRecipeResponseTypeDef,
-    DescribeRecommenderResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    DescribeSolutionResponseTypeDef,
-    DescribeSolutionVersionResponseTypeDef,
+    DescribeAlgorithmResponseOutputTypeDef,
+    DescribeBatchInferenceJobResponseOutputTypeDef,
+    DescribeBatchSegmentJobResponseOutputTypeDef,
+    DescribeCampaignResponseOutputTypeDef,
+    DescribeDatasetExportJobResponseOutputTypeDef,
+    DescribeDatasetGroupResponseOutputTypeDef,
+    DescribeDatasetImportJobResponseOutputTypeDef,
+    DescribeDatasetResponseOutputTypeDef,
+    DescribeEventTrackerResponseOutputTypeDef,
+    DescribeFeatureTransformationResponseOutputTypeDef,
+    DescribeFilterResponseOutputTypeDef,
+    DescribeMetricAttributionResponseOutputTypeDef,
+    DescribeRecipeResponseOutputTypeDef,
+    DescribeRecommenderResponseOutputTypeDef,
+    DescribeSchemaResponseOutputTypeDef,
+    DescribeSolutionResponseOutputTypeDef,
+    DescribeSolutionVersionResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetSolutionMetricsResponseTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    ListCampaignsResponseTypeDef,
-    ListDatasetExportJobsResponseTypeDef,
-    ListDatasetGroupsResponseTypeDef,
-    ListDatasetImportJobsResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    ListEventTrackersResponseTypeDef,
-    ListFiltersResponseTypeDef,
-    ListMetricAttributionMetricsResponseTypeDef,
-    ListMetricAttributionsResponseTypeDef,
-    ListRecipesResponseTypeDef,
-    ListRecommendersResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    ListSolutionsResponseTypeDef,
-    ListSolutionVersionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    GetSolutionMetricsResponseOutputTypeDef,
+    ListBatchInferenceJobsResponseOutputTypeDef,
+    ListBatchSegmentJobsResponseOutputTypeDef,
+    ListCampaignsResponseOutputTypeDef,
+    ListDatasetExportJobsResponseOutputTypeDef,
+    ListDatasetGroupsResponseOutputTypeDef,
+    ListDatasetImportJobsResponseOutputTypeDef,
+    ListDatasetsResponseOutputTypeDef,
+    ListEventTrackersResponseOutputTypeDef,
+    ListFiltersResponseOutputTypeDef,
+    ListMetricAttributionMetricsResponseOutputTypeDef,
+    ListMetricAttributionsResponseOutputTypeDef,
+    ListRecipesResponseOutputTypeDef,
+    ListRecommendersResponseOutputTypeDef,
+    ListSchemasResponseOutputTypeDef,
+    ListSolutionsResponseOutputTypeDef,
+    ListSolutionVersionsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
     RecommenderConfigTypeDef,
     SolutionConfigTypeDef,
-    StartRecommenderResponseTypeDef,
-    StopRecommenderResponseTypeDef,
+    StartRecommenderResponseOutputTypeDef,
+    StopRecommenderResponseOutputTypeDef,
     TagTypeDef,
-    UpdateCampaignResponseTypeDef,
-    UpdateDatasetResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    UpdateCampaignResponseOutputTypeDef,
+    UpdateDatasetResponseOutputTypeDef,
+    UpdateMetricAttributionResponseOutputTypeDef,
+    UpdateRecommenderResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -179,15 +179,15 @@
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchInferenceJobResponseTypeDef:
+    ) -> CreateBatchInferenceJobResponseOutputTypeDef:
         """
         Creates a batch inference job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_inference_job)
         """
 
@@ -198,15 +198,15 @@
         solutionVersionArn: str,
         jobInput: BatchSegmentJobInputTypeDef,
         jobOutput: BatchSegmentJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchSegmentJobResponseTypeDef:
+    ) -> CreateBatchSegmentJobResponseOutputTypeDef:
         """
         Creates a batch segment job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_segment_job)
         """
 
@@ -214,15 +214,15 @@
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateCampaignResponseTypeDef:
+    ) -> CreateCampaignResponseOutputTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
 
@@ -230,15 +230,15 @@
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetResponseTypeDef:
+    ) -> CreateDatasetResponseOutputTypeDef:
         """
         Creates an empty dataset and adds it to the specified dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset)
         """
 
@@ -247,15 +247,15 @@
         *,
         jobName: str,
         datasetArn: str,
         roleArn: str,
         jobOutput: DatasetExportJobOutputTypeDef,
         ingestionMode: IngestionModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetExportJobResponseTypeDef:
+    ) -> CreateDatasetExportJobResponseOutputTypeDef:
         """
         Creates a job that exports data from your dataset to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_export_job)
         """
 
@@ -263,15 +263,15 @@
         self,
         *,
         name: str,
         roleArn: str = ...,
         kmsKeyArn: str = ...,
         domain: DomainType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetGroupResponseTypeDef:
+    ) -> CreateDatasetGroupResponseOutputTypeDef:
         """
         Creates an empty dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_group)
         """
 
@@ -281,26 +281,26 @@
         jobName: str,
         datasetArn: str,
         dataSource: DataSourceTypeDef,
         roleArn: str,
         tags: Sequence[TagTypeDef] = ...,
         importMode: ImportModeType = ...,
         publishAttributionMetricsToS3: bool = ...
-    ) -> CreateDatasetImportJobResponseTypeDef:
+    ) -> CreateDatasetImportJobResponseOutputTypeDef:
         """
         Creates a job that imports training data from your data source (an Amazon S3
         bucket) to an Amazon Personalize dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_import_job)
         """
 
     def create_event_tracker(
         self, *, name: str, datasetGroupArn: str, tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventTrackerResponseTypeDef:
+    ) -> CreateEventTrackerResponseOutputTypeDef:
         """
         Creates an event tracker that you use when adding event data to a specified
         dataset group using the
         [PutEvents](https://docs.aws.amazon.com/personalize/latest/dg/API_UBS_PutEvents.html)_
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_event_tracker)
@@ -310,30 +310,30 @@
     def create_filter(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         filterExpression: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateFilterResponseTypeDef:
+    ) -> CreateFilterResponseOutputTypeDef:
         """
         Creates a recommendation filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_filter)
         """
 
     def create_metric_attribution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         metrics: Sequence[MetricAttributeTypeDef],
         metricsOutputConfig: MetricAttributionOutputTypeDef
-    ) -> CreateMetricAttributionResponseTypeDef:
+    ) -> CreateMetricAttributionResponseOutputTypeDef:
         """
         Creates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_metric_attribution)
         """
 
@@ -341,26 +341,26 @@
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
         recommenderConfig: RecommenderConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRecommenderResponseTypeDef:
+    ) -> CreateRecommenderResponseOutputTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_recommender)
         """
 
     def create_schema(
         self, *, name: str, schema: str, domain: DomainType = ...
-    ) -> CreateSchemaResponseTypeDef:
+    ) -> CreateSchemaResponseOutputTypeDef:
         """
         Creates an Amazon Personalize schema from the specified schema string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_schema)
         """
 
@@ -371,30 +371,30 @@
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionResponseTypeDef:
+    ) -> CreateSolutionResponseOutputTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
         """
 
     def create_solution_version(
         self,
         *,
         solutionArn: str,
         name: str = ...,
         trainingMode: TrainingModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionVersionResponseTypeDef:
+    ) -> CreateSolutionVersionResponseOutputTypeDef:
         """
         Trains or retrains an active solution in a Custom dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution_version)
         """
 
@@ -468,169 +468,171 @@
         """
         Deletes all versions of a solution and the `Solution` object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#delete_solution)
         """
 
-    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseTypeDef:
+    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseOutputTypeDef:
         """
         Describes the given algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_algorithm)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_algorithm)
         """
 
     def describe_batch_inference_job(
         self, *, batchInferenceJobArn: str
-    ) -> DescribeBatchInferenceJobResponseTypeDef:
+    ) -> DescribeBatchInferenceJobResponseOutputTypeDef:
         """
         Gets the properties of a batch inference job including name, Amazon Resource
         Name (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate the recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_inference_job)
         """
 
     def describe_batch_segment_job(
         self, *, batchSegmentJobArn: str
-    ) -> DescribeBatchSegmentJobResponseTypeDef:
+    ) -> DescribeBatchSegmentJobResponseOutputTypeDef:
         """
         Gets the properties of a batch segment job including name, Amazon Resource Name
         (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate segments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_segment_job)
         """
 
-    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseTypeDef:
+    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseOutputTypeDef:
         """
         Describes the given campaign, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_campaign)
         """
 
-    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseTypeDef:
+    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseOutputTypeDef:
         """
         Describes the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset)
         """
 
     def describe_dataset_export_job(
         self, *, datasetExportJobArn: str
-    ) -> DescribeDatasetExportJobResponseTypeDef:
+    ) -> DescribeDatasetExportJobResponseOutputTypeDef:
         """
         Describes the dataset export job created by
         [CreateDatasetExportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetExportJob.html)_,
         including the export job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_export_job)
         """
 
     def describe_dataset_group(
         self, *, datasetGroupArn: str
-    ) -> DescribeDatasetGroupResponseTypeDef:
+    ) -> DescribeDatasetGroupResponseOutputTypeDef:
         """
         Describes the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_group)
         """
 
     def describe_dataset_import_job(
         self, *, datasetImportJobArn: str
-    ) -> DescribeDatasetImportJobResponseTypeDef:
+    ) -> DescribeDatasetImportJobResponseOutputTypeDef:
         """
         Describes the dataset import job created by
         [CreateDatasetImportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetImportJob.html)_,
         including the import job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_import_job)
         """
 
     def describe_event_tracker(
         self, *, eventTrackerArn: str
-    ) -> DescribeEventTrackerResponseTypeDef:
+    ) -> DescribeEventTrackerResponseOutputTypeDef:
         """
         Describes an event tracker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_event_tracker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_event_tracker)
         """
 
     def describe_feature_transformation(
         self, *, featureTransformationArn: str
-    ) -> DescribeFeatureTransformationResponseTypeDef:
+    ) -> DescribeFeatureTransformationResponseOutputTypeDef:
         """
         Describes the given feature transformation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_feature_transformation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_feature_transformation)
         """
 
-    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseTypeDef:
+    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseOutputTypeDef:
         """
         Describes a filter's properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_filter)
         """
 
     def describe_metric_attribution(
         self, *, metricAttributionArn: str
-    ) -> DescribeMetricAttributionResponseTypeDef:
+    ) -> DescribeMetricAttributionResponseOutputTypeDef:
         """
         Describes a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_metric_attribution)
         """
 
-    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseTypeDef:
+    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseOutputTypeDef:
         """
         Describes a recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recipe)
         """
 
-    def describe_recommender(self, *, recommenderArn: str) -> DescribeRecommenderResponseTypeDef:
+    def describe_recommender(
+        self, *, recommenderArn: str
+    ) -> DescribeRecommenderResponseOutputTypeDef:
         """
         Describes the given recommender, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recommender)
         """
 
-    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseTypeDef:
+    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseOutputTypeDef:
         """
         Describes a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_schema)
         """
 
-    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseTypeDef:
+    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseOutputTypeDef:
         """
         Describes a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution)
         """
 
     def describe_solution_version(
         self, *, solutionVersionArn: str
-    ) -> DescribeSolutionVersionResponseTypeDef:
+    ) -> DescribeSolutionVersionResponseOutputTypeDef:
         """
         Describes a specific version of a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution_version)
         """
 
@@ -644,207 +646,211 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#generate_presigned_url)
         """
 
-    def get_solution_metrics(self, *, solutionVersionArn: str) -> GetSolutionMetricsResponseTypeDef:
+    def get_solution_metrics(
+        self, *, solutionVersionArn: str
+    ) -> GetSolutionMetricsResponseOutputTypeDef:
         """
         Gets the metrics for the specified solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.get_solution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#get_solution_metrics)
         """
 
     def list_batch_inference_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchInferenceJobsResponseTypeDef:
+    ) -> ListBatchInferenceJobsResponseOutputTypeDef:
         """
         Gets a list of the batch inference jobs that have been performed off of a
         solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_inference_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_inference_jobs)
         """
 
     def list_batch_segment_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchSegmentJobsResponseTypeDef:
+    ) -> ListBatchSegmentJobsResponseOutputTypeDef:
         """
         Gets a list of the batch segment jobs that have been performed off of a solution
         version that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_segment_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_segment_jobs)
         """
 
     def list_campaigns(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListCampaignsResponseTypeDef:
+    ) -> ListCampaignsResponseOutputTypeDef:
         """
         Returns a list of campaigns that use the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_campaigns)
         """
 
     def list_dataset_export_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetExportJobsResponseTypeDef:
+    ) -> ListDatasetExportJobsResponseOutputTypeDef:
         """
         Returns a list of dataset export jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_export_jobs)
         """
 
     def list_dataset_groups(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetGroupsResponseTypeDef:
+    ) -> ListDatasetGroupsResponseOutputTypeDef:
         """
         Returns a list of dataset groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_groups)
         """
 
     def list_dataset_import_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetImportJobsResponseTypeDef:
+    ) -> ListDatasetImportJobsResponseOutputTypeDef:
         """
         Returns a list of dataset import jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_import_jobs)
         """
 
     def list_datasets(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetsResponseTypeDef:
+    ) -> ListDatasetsResponseOutputTypeDef:
         """
         Returns the list of datasets contained in the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_datasets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_datasets)
         """
 
     def list_event_trackers(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListEventTrackersResponseTypeDef:
+    ) -> ListEventTrackersResponseOutputTypeDef:
         """
         Returns the list of event trackers associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_event_trackers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_event_trackers)
         """
 
     def list_filters(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListFiltersResponseTypeDef:
+    ) -> ListFiltersResponseOutputTypeDef:
         """
         Lists all filters that belong to a given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_filters)
         """
 
     def list_metric_attribution_metrics(
         self, *, metricAttributionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionMetricsResponseTypeDef:
+    ) -> ListMetricAttributionMetricsResponseOutputTypeDef:
         """
         Lists the metrics for the metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attribution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attribution_metrics)
         """
 
     def list_metric_attributions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionsResponseTypeDef:
+    ) -> ListMetricAttributionsResponseOutputTypeDef:
         """
         Lists metric attributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attributions)
         """
 
     def list_recipes(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         domain: DomainType = ...
-    ) -> ListRecipesResponseTypeDef:
+    ) -> ListRecipesResponseOutputTypeDef:
         """
         Returns a list of available recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recipes)
         """
 
     def list_recommenders(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListRecommendersResponseTypeDef:
+    ) -> ListRecommendersResponseOutputTypeDef:
         """
         Returns a list of recommenders in a given Domain dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recommenders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recommenders)
         """
 
     def list_schemas(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListSchemasResponseTypeDef:
+    ) -> ListSchemasResponseOutputTypeDef:
         """
         Returns the list of schemas associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_schemas)
         """
 
     def list_solution_versions(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionVersionsResponseTypeDef:
+    ) -> ListSolutionVersionsResponseOutputTypeDef:
         """
         Returns a list of solution versions for the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solution_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solution_versions)
         """
 
     def list_solutions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionsResponseTypeDef:
+    ) -> ListSolutionsResponseOutputTypeDef:
         """
         Returns a list of solutions that use the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
 
-    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, resourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_tags_for_resource)
         """
 
-    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseTypeDef:
+    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseOutputTypeDef:
         """
         Starts a recommender that is INACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.start_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#start_recommender)
         """
 
-    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseTypeDef:
+    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseOutputTypeDef:
         """
         Stops a recommender that is ACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.stop_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#stop_recommender)
         """
 
@@ -879,49 +885,51 @@
     def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...
-    ) -> UpdateCampaignResponseTypeDef:
+    ) -> UpdateCampaignResponseOutputTypeDef:
         """
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
 
-    def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
+    def update_dataset(
+        self, *, datasetArn: str, schemaArn: str
+    ) -> UpdateDatasetResponseOutputTypeDef:
         """
         Update a dataset to replace its schema with a new or existing one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_dataset)
         """
 
     def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
-    ) -> UpdateMetricAttributionResponseTypeDef:
+    ) -> UpdateMetricAttributionResponseOutputTypeDef:
         """
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_metric_attribution)
         """
 
     def update_recommender(
         self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
-    ) -> UpdateRecommenderResponseTypeDef:
+    ) -> UpdateRecommenderResponseOutputTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_recommender)
         """
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.pyi` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -40,77 +40,77 @@
 from .type_defs import (
     BatchInferenceJobConfigTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     CampaignConfigTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
+    CreateBatchInferenceJobResponseOutputTypeDef,
+    CreateBatchSegmentJobResponseOutputTypeDef,
+    CreateCampaignResponseOutputTypeDef,
+    CreateDatasetExportJobResponseOutputTypeDef,
+    CreateDatasetGroupResponseOutputTypeDef,
+    CreateDatasetImportJobResponseOutputTypeDef,
+    CreateDatasetResponseOutputTypeDef,
+    CreateEventTrackerResponseOutputTypeDef,
+    CreateFilterResponseOutputTypeDef,
+    CreateMetricAttributionResponseOutputTypeDef,
+    CreateRecommenderResponseOutputTypeDef,
+    CreateSchemaResponseOutputTypeDef,
+    CreateSolutionResponseOutputTypeDef,
+    CreateSolutionVersionResponseOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     DataSourceTypeDef,
-    DescribeAlgorithmResponseTypeDef,
-    DescribeBatchInferenceJobResponseTypeDef,
-    DescribeBatchSegmentJobResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-    DescribeDatasetExportJobResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    DescribeDatasetImportJobResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    DescribeEventTrackerResponseTypeDef,
-    DescribeFeatureTransformationResponseTypeDef,
-    DescribeFilterResponseTypeDef,
-    DescribeMetricAttributionResponseTypeDef,
-    DescribeRecipeResponseTypeDef,
-    DescribeRecommenderResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    DescribeSolutionResponseTypeDef,
-    DescribeSolutionVersionResponseTypeDef,
+    DescribeAlgorithmResponseOutputTypeDef,
+    DescribeBatchInferenceJobResponseOutputTypeDef,
+    DescribeBatchSegmentJobResponseOutputTypeDef,
+    DescribeCampaignResponseOutputTypeDef,
+    DescribeDatasetExportJobResponseOutputTypeDef,
+    DescribeDatasetGroupResponseOutputTypeDef,
+    DescribeDatasetImportJobResponseOutputTypeDef,
+    DescribeDatasetResponseOutputTypeDef,
+    DescribeEventTrackerResponseOutputTypeDef,
+    DescribeFeatureTransformationResponseOutputTypeDef,
+    DescribeFilterResponseOutputTypeDef,
+    DescribeMetricAttributionResponseOutputTypeDef,
+    DescribeRecipeResponseOutputTypeDef,
+    DescribeRecommenderResponseOutputTypeDef,
+    DescribeSchemaResponseOutputTypeDef,
+    DescribeSolutionResponseOutputTypeDef,
+    DescribeSolutionVersionResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetSolutionMetricsResponseTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    ListCampaignsResponseTypeDef,
-    ListDatasetExportJobsResponseTypeDef,
-    ListDatasetGroupsResponseTypeDef,
-    ListDatasetImportJobsResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    ListEventTrackersResponseTypeDef,
-    ListFiltersResponseTypeDef,
-    ListMetricAttributionMetricsResponseTypeDef,
-    ListMetricAttributionsResponseTypeDef,
-    ListRecipesResponseTypeDef,
-    ListRecommendersResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    ListSolutionsResponseTypeDef,
-    ListSolutionVersionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    GetSolutionMetricsResponseOutputTypeDef,
+    ListBatchInferenceJobsResponseOutputTypeDef,
+    ListBatchSegmentJobsResponseOutputTypeDef,
+    ListCampaignsResponseOutputTypeDef,
+    ListDatasetExportJobsResponseOutputTypeDef,
+    ListDatasetGroupsResponseOutputTypeDef,
+    ListDatasetImportJobsResponseOutputTypeDef,
+    ListDatasetsResponseOutputTypeDef,
+    ListEventTrackersResponseOutputTypeDef,
+    ListFiltersResponseOutputTypeDef,
+    ListMetricAttributionMetricsResponseOutputTypeDef,
+    ListMetricAttributionsResponseOutputTypeDef,
+    ListRecipesResponseOutputTypeDef,
+    ListRecommendersResponseOutputTypeDef,
+    ListSchemasResponseOutputTypeDef,
+    ListSolutionsResponseOutputTypeDef,
+    ListSolutionVersionsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
     RecommenderConfigTypeDef,
     SolutionConfigTypeDef,
-    StartRecommenderResponseTypeDef,
-    StopRecommenderResponseTypeDef,
+    StartRecommenderResponseOutputTypeDef,
+    StopRecommenderResponseOutputTypeDef,
     TagTypeDef,
-    UpdateCampaignResponseTypeDef,
-    UpdateDatasetResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    UpdateCampaignResponseOutputTypeDef,
+    UpdateDatasetResponseOutputTypeDef,
+    UpdateMetricAttributionResponseOutputTypeDef,
+    UpdateRecommenderResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -172,15 +172,15 @@
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchInferenceJobResponseTypeDef:
+    ) -> CreateBatchInferenceJobResponseOutputTypeDef:
         """
         Creates a batch inference job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_inference_job)
         """
     def create_batch_segment_job(
@@ -190,45 +190,45 @@
         solutionVersionArn: str,
         jobInput: BatchSegmentJobInputTypeDef,
         jobOutput: BatchSegmentJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchSegmentJobResponseTypeDef:
+    ) -> CreateBatchSegmentJobResponseOutputTypeDef:
         """
         Creates a batch segment job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_segment_job)
         """
     def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateCampaignResponseTypeDef:
+    ) -> CreateCampaignResponseOutputTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
     def create_dataset(
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetResponseTypeDef:
+    ) -> CreateDatasetResponseOutputTypeDef:
         """
         Creates an empty dataset and adds it to the specified dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset)
         """
     def create_dataset_export_job(
@@ -236,30 +236,30 @@
         *,
         jobName: str,
         datasetArn: str,
         roleArn: str,
         jobOutput: DatasetExportJobOutputTypeDef,
         ingestionMode: IngestionModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetExportJobResponseTypeDef:
+    ) -> CreateDatasetExportJobResponseOutputTypeDef:
         """
         Creates a job that exports data from your dataset to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_export_job)
         """
     def create_dataset_group(
         self,
         *,
         name: str,
         roleArn: str = ...,
         kmsKeyArn: str = ...,
         domain: DomainType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetGroupResponseTypeDef:
+    ) -> CreateDatasetGroupResponseOutputTypeDef:
         """
         Creates an empty dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_group)
         """
     def create_dataset_import_job(
@@ -268,25 +268,25 @@
         jobName: str,
         datasetArn: str,
         dataSource: DataSourceTypeDef,
         roleArn: str,
         tags: Sequence[TagTypeDef] = ...,
         importMode: ImportModeType = ...,
         publishAttributionMetricsToS3: bool = ...
-    ) -> CreateDatasetImportJobResponseTypeDef:
+    ) -> CreateDatasetImportJobResponseOutputTypeDef:
         """
         Creates a job that imports training data from your data source (an Amazon S3
         bucket) to an Amazon Personalize dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_import_job)
         """
     def create_event_tracker(
         self, *, name: str, datasetGroupArn: str, tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventTrackerResponseTypeDef:
+    ) -> CreateEventTrackerResponseOutputTypeDef:
         """
         Creates an event tracker that you use when adding event data to a specified
         dataset group using the
         [PutEvents](https://docs.aws.amazon.com/personalize/latest/dg/API_UBS_PutEvents.html)_
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_event_tracker)
@@ -295,54 +295,54 @@
     def create_filter(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         filterExpression: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateFilterResponseTypeDef:
+    ) -> CreateFilterResponseOutputTypeDef:
         """
         Creates a recommendation filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_filter)
         """
     def create_metric_attribution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         metrics: Sequence[MetricAttributeTypeDef],
         metricsOutputConfig: MetricAttributionOutputTypeDef
-    ) -> CreateMetricAttributionResponseTypeDef:
+    ) -> CreateMetricAttributionResponseOutputTypeDef:
         """
         Creates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_metric_attribution)
         """
     def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
         recommenderConfig: RecommenderConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRecommenderResponseTypeDef:
+    ) -> CreateRecommenderResponseOutputTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_recommender)
         """
     def create_schema(
         self, *, name: str, schema: str, domain: DomainType = ...
-    ) -> CreateSchemaResponseTypeDef:
+    ) -> CreateSchemaResponseOutputTypeDef:
         """
         Creates an Amazon Personalize schema from the specified schema string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_schema)
         """
     def create_solution(
@@ -352,29 +352,29 @@
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionResponseTypeDef:
+    ) -> CreateSolutionResponseOutputTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
         """
     def create_solution_version(
         self,
         *,
         solutionArn: str,
         name: str = ...,
         trainingMode: TrainingModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionVersionResponseTypeDef:
+    ) -> CreateSolutionVersionResponseOutputTypeDef:
         """
         Trains or retrains an active solution in a Custom dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution_version)
         """
     def delete_campaign(self, *, campaignArn: str) -> EmptyResponseMetadataTypeDef:
@@ -438,153 +438,155 @@
     def delete_solution(self, *, solutionArn: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes all versions of a solution and the `Solution` object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#delete_solution)
         """
-    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseTypeDef:
+    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseOutputTypeDef:
         """
         Describes the given algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_algorithm)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_algorithm)
         """
     def describe_batch_inference_job(
         self, *, batchInferenceJobArn: str
-    ) -> DescribeBatchInferenceJobResponseTypeDef:
+    ) -> DescribeBatchInferenceJobResponseOutputTypeDef:
         """
         Gets the properties of a batch inference job including name, Amazon Resource
         Name (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate the recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_inference_job)
         """
     def describe_batch_segment_job(
         self, *, batchSegmentJobArn: str
-    ) -> DescribeBatchSegmentJobResponseTypeDef:
+    ) -> DescribeBatchSegmentJobResponseOutputTypeDef:
         """
         Gets the properties of a batch segment job including name, Amazon Resource Name
         (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate segments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_segment_job)
         """
-    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseTypeDef:
+    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseOutputTypeDef:
         """
         Describes the given campaign, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_campaign)
         """
-    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseTypeDef:
+    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseOutputTypeDef:
         """
         Describes the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset)
         """
     def describe_dataset_export_job(
         self, *, datasetExportJobArn: str
-    ) -> DescribeDatasetExportJobResponseTypeDef:
+    ) -> DescribeDatasetExportJobResponseOutputTypeDef:
         """
         Describes the dataset export job created by
         [CreateDatasetExportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetExportJob.html)_,
         including the export job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_export_job)
         """
     def describe_dataset_group(
         self, *, datasetGroupArn: str
-    ) -> DescribeDatasetGroupResponseTypeDef:
+    ) -> DescribeDatasetGroupResponseOutputTypeDef:
         """
         Describes the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_group)
         """
     def describe_dataset_import_job(
         self, *, datasetImportJobArn: str
-    ) -> DescribeDatasetImportJobResponseTypeDef:
+    ) -> DescribeDatasetImportJobResponseOutputTypeDef:
         """
         Describes the dataset import job created by
         [CreateDatasetImportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetImportJob.html)_,
         including the import job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_import_job)
         """
     def describe_event_tracker(
         self, *, eventTrackerArn: str
-    ) -> DescribeEventTrackerResponseTypeDef:
+    ) -> DescribeEventTrackerResponseOutputTypeDef:
         """
         Describes an event tracker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_event_tracker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_event_tracker)
         """
     def describe_feature_transformation(
         self, *, featureTransformationArn: str
-    ) -> DescribeFeatureTransformationResponseTypeDef:
+    ) -> DescribeFeatureTransformationResponseOutputTypeDef:
         """
         Describes the given feature transformation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_feature_transformation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_feature_transformation)
         """
-    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseTypeDef:
+    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseOutputTypeDef:
         """
         Describes a filter's properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_filter)
         """
     def describe_metric_attribution(
         self, *, metricAttributionArn: str
-    ) -> DescribeMetricAttributionResponseTypeDef:
+    ) -> DescribeMetricAttributionResponseOutputTypeDef:
         """
         Describes a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_metric_attribution)
         """
-    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseTypeDef:
+    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseOutputTypeDef:
         """
         Describes a recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recipe)
         """
-    def describe_recommender(self, *, recommenderArn: str) -> DescribeRecommenderResponseTypeDef:
+    def describe_recommender(
+        self, *, recommenderArn: str
+    ) -> DescribeRecommenderResponseOutputTypeDef:
         """
         Describes the given recommender, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recommender)
         """
-    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseTypeDef:
+    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseOutputTypeDef:
         """
         Describes a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_schema)
         """
-    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseTypeDef:
+    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseOutputTypeDef:
         """
         Describes a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution)
         """
     def describe_solution_version(
         self, *, solutionVersionArn: str
-    ) -> DescribeSolutionVersionResponseTypeDef:
+    ) -> DescribeSolutionVersionResponseOutputTypeDef:
         """
         Describes a specific version of a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution_version)
         """
     def generate_presigned_url(
@@ -596,188 +598,192 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#generate_presigned_url)
         """
-    def get_solution_metrics(self, *, solutionVersionArn: str) -> GetSolutionMetricsResponseTypeDef:
+    def get_solution_metrics(
+        self, *, solutionVersionArn: str
+    ) -> GetSolutionMetricsResponseOutputTypeDef:
         """
         Gets the metrics for the specified solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.get_solution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#get_solution_metrics)
         """
     def list_batch_inference_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchInferenceJobsResponseTypeDef:
+    ) -> ListBatchInferenceJobsResponseOutputTypeDef:
         """
         Gets a list of the batch inference jobs that have been performed off of a
         solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_inference_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_inference_jobs)
         """
     def list_batch_segment_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchSegmentJobsResponseTypeDef:
+    ) -> ListBatchSegmentJobsResponseOutputTypeDef:
         """
         Gets a list of the batch segment jobs that have been performed off of a solution
         version that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_segment_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_segment_jobs)
         """
     def list_campaigns(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListCampaignsResponseTypeDef:
+    ) -> ListCampaignsResponseOutputTypeDef:
         """
         Returns a list of campaigns that use the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_campaigns)
         """
     def list_dataset_export_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetExportJobsResponseTypeDef:
+    ) -> ListDatasetExportJobsResponseOutputTypeDef:
         """
         Returns a list of dataset export jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_export_jobs)
         """
     def list_dataset_groups(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetGroupsResponseTypeDef:
+    ) -> ListDatasetGroupsResponseOutputTypeDef:
         """
         Returns a list of dataset groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_groups)
         """
     def list_dataset_import_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetImportJobsResponseTypeDef:
+    ) -> ListDatasetImportJobsResponseOutputTypeDef:
         """
         Returns a list of dataset import jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_import_jobs)
         """
     def list_datasets(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetsResponseTypeDef:
+    ) -> ListDatasetsResponseOutputTypeDef:
         """
         Returns the list of datasets contained in the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_datasets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_datasets)
         """
     def list_event_trackers(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListEventTrackersResponseTypeDef:
+    ) -> ListEventTrackersResponseOutputTypeDef:
         """
         Returns the list of event trackers associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_event_trackers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_event_trackers)
         """
     def list_filters(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListFiltersResponseTypeDef:
+    ) -> ListFiltersResponseOutputTypeDef:
         """
         Lists all filters that belong to a given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_filters)
         """
     def list_metric_attribution_metrics(
         self, *, metricAttributionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionMetricsResponseTypeDef:
+    ) -> ListMetricAttributionMetricsResponseOutputTypeDef:
         """
         Lists the metrics for the metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attribution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attribution_metrics)
         """
     def list_metric_attributions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionsResponseTypeDef:
+    ) -> ListMetricAttributionsResponseOutputTypeDef:
         """
         Lists metric attributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attributions)
         """
     def list_recipes(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         domain: DomainType = ...
-    ) -> ListRecipesResponseTypeDef:
+    ) -> ListRecipesResponseOutputTypeDef:
         """
         Returns a list of available recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recipes)
         """
     def list_recommenders(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListRecommendersResponseTypeDef:
+    ) -> ListRecommendersResponseOutputTypeDef:
         """
         Returns a list of recommenders in a given Domain dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recommenders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recommenders)
         """
     def list_schemas(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListSchemasResponseTypeDef:
+    ) -> ListSchemasResponseOutputTypeDef:
         """
         Returns the list of schemas associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_schemas)
         """
     def list_solution_versions(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionVersionsResponseTypeDef:
+    ) -> ListSolutionVersionsResponseOutputTypeDef:
         """
         Returns a list of solution versions for the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solution_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solution_versions)
         """
     def list_solutions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionsResponseTypeDef:
+    ) -> ListSolutionsResponseOutputTypeDef:
         """
         Returns a list of solutions that use the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
-    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, resourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_tags_for_resource)
         """
-    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseTypeDef:
+    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseOutputTypeDef:
         """
         Starts a recommender that is INACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.start_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#start_recommender)
         """
-    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseTypeDef:
+    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseOutputTypeDef:
         """
         Stops a recommender that is ACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.stop_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#stop_recommender)
         """
     def stop_solution_version_creation(
@@ -808,46 +814,48 @@
     def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...
-    ) -> UpdateCampaignResponseTypeDef:
+    ) -> UpdateCampaignResponseOutputTypeDef:
         """
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
-    def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
+    def update_dataset(
+        self, *, datasetArn: str, schemaArn: str
+    ) -> UpdateDatasetResponseOutputTypeDef:
         """
         Update a dataset to replace its schema with a new or existing one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_dataset)
         """
     def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
-    ) -> UpdateMetricAttributionResponseTypeDef:
+    ) -> UpdateMetricAttributionResponseOutputTypeDef:
         """
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_metric_attribution)
         """
     def update_recommender(
         self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
-    ) -> UpdateRecommenderResponseTypeDef:
+    ) -> UpdateRecommenderResponseOutputTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_recommender)
         """
     @overload
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.py` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.pyi` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.py` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,30 +52,30 @@
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DomainType
 from .type_defs import (
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    ListCampaignsResponseTypeDef,
-    ListDatasetExportJobsResponseTypeDef,
-    ListDatasetGroupsResponseTypeDef,
-    ListDatasetImportJobsResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    ListEventTrackersResponseTypeDef,
-    ListFiltersResponseTypeDef,
-    ListMetricAttributionMetricsResponseTypeDef,
-    ListMetricAttributionsResponseTypeDef,
-    ListRecipesResponseTypeDef,
-    ListRecommendersResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    ListSolutionsResponseTypeDef,
-    ListSolutionVersionsResponseTypeDef,
+    ListBatchInferenceJobsResponseOutputTypeDef,
+    ListBatchSegmentJobsResponseOutputTypeDef,
+    ListCampaignsResponseOutputTypeDef,
+    ListDatasetExportJobsResponseOutputTypeDef,
+    ListDatasetGroupsResponseOutputTypeDef,
+    ListDatasetImportJobsResponseOutputTypeDef,
+    ListDatasetsResponseOutputTypeDef,
+    ListEventTrackersResponseOutputTypeDef,
+    ListFiltersResponseOutputTypeDef,
+    ListMetricAttributionMetricsResponseOutputTypeDef,
+    ListMetricAttributionsResponseOutputTypeDef,
+    ListRecipesResponseOutputTypeDef,
+    ListRecommendersResponseOutputTypeDef,
+    ListSchemasResponseOutputTypeDef,
+    ListSolutionsResponseOutputTypeDef,
+    ListSolutionVersionsResponseOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -115,165 +115,165 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchInferenceJobsResponseTypeDef]:
+    ) -> _PageIterator[ListBatchInferenceJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
         """
 
 
 class ListBatchSegmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchSegmentJobsResponseTypeDef]:
+    ) -> _PageIterator[ListBatchSegmentJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
         """
 
 
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListCampaignsResponseTypeDef]:
+    ) -> _PageIterator[ListCampaignsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
         """
 
 
 class ListDatasetExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetExportJobsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetExportJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
         """
 
 
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
         """
 
 
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetImportJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
         """
 
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
         """
 
 
 class ListEventTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEventTrackersResponseTypeDef]:
+    ) -> _PageIterator[ListEventTrackersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
         """
 
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListFiltersResponseTypeDef]:
+    ) -> _PageIterator[ListFiltersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
         """
 
 
 class ListMetricAttributionMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
     """
 
     def paginate(
         self, *, metricAttributionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionMetricsResponseTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionMetricsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
         """
 
 
 class ListMetricAttributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionsResponseTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
         """
 
 
 class ListRecipesPaginator(Paginator):
@@ -284,72 +284,72 @@
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecipesResponseTypeDef]:
+    ) -> _PageIterator[ListRecipesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecipespaginator)
         """
 
 
 class ListRecommendersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecommendersResponseTypeDef]:
+    ) -> _PageIterator[ListRecommendersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSchemasResponseTypeDef]:
+    ) -> _PageIterator[ListSchemasResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
         """
 
 
 class ListSolutionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionVersionsResponseTypeDef]:
+    ) -> _PageIterator[ListSolutionVersionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
         """
 
 
 class ListSolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionsResponseTypeDef]:
+    ) -> _PageIterator[ListSolutionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
         """
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.pyi` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -52,30 +52,30 @@
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DomainType
 from .type_defs import (
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    ListCampaignsResponseTypeDef,
-    ListDatasetExportJobsResponseTypeDef,
-    ListDatasetGroupsResponseTypeDef,
-    ListDatasetImportJobsResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    ListEventTrackersResponseTypeDef,
-    ListFiltersResponseTypeDef,
-    ListMetricAttributionMetricsResponseTypeDef,
-    ListMetricAttributionsResponseTypeDef,
-    ListRecipesResponseTypeDef,
-    ListRecommendersResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    ListSolutionsResponseTypeDef,
-    ListSolutionVersionsResponseTypeDef,
+    ListBatchInferenceJobsResponseOutputTypeDef,
+    ListBatchSegmentJobsResponseOutputTypeDef,
+    ListCampaignsResponseOutputTypeDef,
+    ListDatasetExportJobsResponseOutputTypeDef,
+    ListDatasetGroupsResponseOutputTypeDef,
+    ListDatasetImportJobsResponseOutputTypeDef,
+    ListDatasetsResponseOutputTypeDef,
+    ListEventTrackersResponseOutputTypeDef,
+    ListFiltersResponseOutputTypeDef,
+    ListMetricAttributionMetricsResponseOutputTypeDef,
+    ListMetricAttributionsResponseOutputTypeDef,
+    ListRecipesResponseOutputTypeDef,
+    ListRecommendersResponseOutputTypeDef,
+    ListSchemasResponseOutputTypeDef,
+    ListSolutionsResponseOutputTypeDef,
+    ListSolutionVersionsResponseOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -111,155 +111,155 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchInferenceJobsResponseTypeDef]:
+    ) -> _PageIterator[ListBatchInferenceJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
         """
 
 class ListBatchSegmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchSegmentJobsResponseTypeDef]:
+    ) -> _PageIterator[ListBatchSegmentJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
         """
 
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListCampaignsResponseTypeDef]:
+    ) -> _PageIterator[ListCampaignsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
         """
 
 class ListDatasetExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetExportJobsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetExportJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
         """
 
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
         """
 
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetImportJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
         """
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetsResponseTypeDef]:
+    ) -> _PageIterator[ListDatasetsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
         """
 
 class ListEventTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEventTrackersResponseTypeDef]:
+    ) -> _PageIterator[ListEventTrackersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
         """
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListFiltersResponseTypeDef]:
+    ) -> _PageIterator[ListFiltersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
         """
 
 class ListMetricAttributionMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
     """
 
     def paginate(
         self, *, metricAttributionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionMetricsResponseTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionMetricsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
         """
 
 class ListMetricAttributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionsResponseTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
         """
 
 class ListRecipesPaginator(Paginator):
     """
@@ -269,68 +269,68 @@
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecipesResponseTypeDef]:
+    ) -> _PageIterator[ListRecipesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecipespaginator)
         """
 
 class ListRecommendersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecommendersResponseTypeDef]:
+    ) -> _PageIterator[ListRecommendersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSchemasResponseTypeDef]:
+    ) -> _PageIterator[ListSchemasResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
         """
 
 class ListSolutionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionVersionsResponseTypeDef]:
+    ) -> _PageIterator[ListSolutionVersionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
         """
 
 class ListSolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionsResponseTypeDef]:
+    ) -> _PageIterator[ListSolutionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
         """
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.py` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for personalize service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize.type_defs import AlgorithmImageTypeDef
+    from mypy_boto3_personalize.type_defs import AlgorithmImageOutputTypeDef
 
-    data: AlgorithmImageTypeDef = {...}
+    data: AlgorithmImageOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -30,54 +30,59 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AlgorithmImageTypeDef",
+    "AlgorithmImageOutputTypeDef",
+    "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
-    "AutoMLResultTypeDef",
+    "AutoMLResultOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
-    "BatchInferenceJobSummaryTypeDef",
-    "BatchSegmentJobSummaryTypeDef",
+    "BatchInferenceJobSummaryOutputTypeDef",
+    "BatchSegmentJobSummaryOutputTypeDef",
+    "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
-    "CampaignSummaryTypeDef",
+    "CampaignSummaryOutputTypeDef",
+    "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
+    "ContinuousHyperParameterRangeOutputTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
-    "CreateBatchInferenceJobResponseTypeDef",
-    "CreateBatchSegmentJobResponseTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDatasetExportJobResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
+    "CreateBatchInferenceJobResponseOutputTypeDef",
+    "CreateBatchSegmentJobResponseOutputTypeDef",
+    "CreateCampaignResponseOutputTypeDef",
+    "CreateDatasetExportJobResponseOutputTypeDef",
+    "CreateDatasetGroupResponseOutputTypeDef",
     "DataSourceTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateEventTrackerResponseTypeDef",
-    "CreateFilterResponseTypeDef",
+    "CreateDatasetImportJobResponseOutputTypeDef",
+    "CreateDatasetResponseOutputTypeDef",
+    "CreateEventTrackerResponseOutputTypeDef",
+    "CreateFilterResponseOutputTypeDef",
     "MetricAttributeTypeDef",
-    "CreateMetricAttributionResponseTypeDef",
-    "CreateRecommenderResponseTypeDef",
+    "CreateMetricAttributionResponseOutputTypeDef",
+    "CreateRecommenderResponseOutputTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "CreateSolutionResponseTypeDef",
-    "CreateSolutionVersionResponseTypeDef",
-    "DatasetExportJobSummaryTypeDef",
-    "DatasetGroupSummaryTypeDef",
-    "DatasetGroupTypeDef",
-    "DatasetImportJobSummaryTypeDef",
-    "DatasetSchemaSummaryTypeDef",
-    "DatasetSchemaTypeDef",
-    "DatasetSummaryTypeDef",
-    "DatasetUpdateSummaryTypeDef",
-    "DefaultCategoricalHyperParameterRangeTypeDef",
-    "DefaultContinuousHyperParameterRangeTypeDef",
-    "DefaultIntegerHyperParameterRangeTypeDef",
+    "CreateSchemaResponseOutputTypeDef",
+    "CreateSolutionResponseOutputTypeDef",
+    "CreateSolutionVersionResponseOutputTypeDef",
+    "DataSourceOutputTypeDef",
+    "DatasetExportJobSummaryOutputTypeDef",
+    "DatasetGroupOutputTypeDef",
+    "DatasetGroupSummaryOutputTypeDef",
+    "DatasetImportJobSummaryOutputTypeDef",
+    "DatasetUpdateSummaryOutputTypeDef",
+    "DatasetSchemaOutputTypeDef",
+    "DatasetSchemaSummaryOutputTypeDef",
+    "DatasetSummaryOutputTypeDef",
+    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
+    "DefaultContinuousHyperParameterRangeOutputTypeDef",
+    "DefaultIntegerHyperParameterRangeOutputTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteMetricAttributionRequestRequestTypeDef",
     "DeleteRecommenderRequestRequestTypeDef",
@@ -88,33 +93,36 @@
     "DescribeBatchSegmentJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DescribeDatasetExportJobRequestRequestTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeEventTrackerRequestRequestTypeDef",
-    "EventTrackerTypeDef",
+    "EventTrackerOutputTypeDef",
     "DescribeFeatureTransformationRequestRequestTypeDef",
-    "FeatureTransformationTypeDef",
+    "FeatureTransformationOutputTypeDef",
     "DescribeFilterRequestRequestTypeDef",
-    "FilterTypeDef",
+    "FilterOutputTypeDef",
     "DescribeMetricAttributionRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
-    "RecipeTypeDef",
+    "RecipeOutputTypeDef",
     "DescribeRecommenderRequestRequestTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
     "DescribeSolutionRequestRequestTypeDef",
     "DescribeSolutionVersionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "EventTrackerSummaryTypeDef",
-    "FilterSummaryTypeDef",
+    "EventTrackerSummaryOutputTypeDef",
+    "FilterSummaryOutputTypeDef",
     "GetSolutionMetricsRequestRequestTypeDef",
-    "GetSolutionMetricsResponseTypeDef",
+    "GetSolutionMetricsResponseOutputTypeDef",
+    "HPOObjectiveOutputTypeDef",
+    "HPOResourceConfigOutputTypeDef",
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
+    "IntegerHyperParameterRangeOutputTypeDef",
     "IntegerHyperParameterRangeTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchInferenceJobsRequestRequestTypeDef",
     "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestRequestTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
@@ -128,144 +136,156 @@
     "ListDatasetsRequestRequestTypeDef",
     "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
     "ListEventTrackersRequestRequestTypeDef",
     "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
+    "MetricAttributeOutputTypeDef",
     "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     "ListMetricAttributionsRequestRequestTypeDef",
-    "MetricAttributionSummaryTypeDef",
+    "MetricAttributionSummaryOutputTypeDef",
     "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
-    "RecipeSummaryTypeDef",
+    "RecipeSummaryOutputTypeDef",
     "ListRecommendersRequestListRecommendersPaginateTypeDef",
     "ListRecommendersRequestRequestTypeDef",
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
-    "SolutionVersionSummaryTypeDef",
+    "SolutionVersionSummaryOutputTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListSolutionsRequestRequestTypeDef",
-    "SolutionSummaryTypeDef",
+    "SolutionSummaryOutputTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "OptimizationObjectiveOutputTypeDef",
     "OptimizationObjectiveTypeDef",
     "PaginatorConfigTypeDef",
+    "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "ResponseMetadataTypeDef",
-    "TunedHPOParamsTypeDef",
+    "TunedHPOParamsOutputTypeDef",
     "StartRecommenderRequestRequestTypeDef",
-    "StartRecommenderResponseTypeDef",
+    "StartRecommenderResponseOutputTypeDef",
     "StopRecommenderRequestRequestTypeDef",
-    "StopRecommenderResponseTypeDef",
+    "StopRecommenderResponseOutputTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCampaignResponseTypeDef",
+    "UpdateCampaignResponseOutputTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
-    "UpdateDatasetResponseTypeDef",
-    "UpdateMetricAttributionResponseTypeDef",
-    "UpdateRecommenderResponseTypeDef",
+    "UpdateDatasetResponseOutputTypeDef",
+    "UpdateMetricAttributionResponseOutputTypeDef",
+    "UpdateRecommenderResponseOutputTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
-    "ListBatchInferenceJobsResponseTypeDef",
-    "ListBatchSegmentJobsResponseTypeDef",
-    "CampaignUpdateSummaryTypeDef",
+    "ListBatchInferenceJobsResponseOutputTypeDef",
+    "ListBatchSegmentJobsResponseOutputTypeDef",
+    "CampaignUpdateSummaryOutputTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
-    "ListCampaignsResponseTypeDef",
+    "ListCampaignsResponseOutputTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
-    "DatasetImportJobTypeDef",
-    "ListMetricAttributionMetricsResponseTypeDef",
-    "ListDatasetExportJobsResponseTypeDef",
-    "ListDatasetGroupsResponseTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
-    "ListDatasetImportJobsResponseTypeDef",
-    "ListSchemasResponseTypeDef",
-    "DescribeSchemaResponseTypeDef",
-    "ListDatasetsResponseTypeDef",
-    "DatasetTypeDef",
-    "DefaultHyperParameterRangesTypeDef",
-    "DescribeEventTrackerResponseTypeDef",
-    "DescribeFeatureTransformationResponseTypeDef",
-    "DescribeFilterResponseTypeDef",
-    "DescribeRecipeResponseTypeDef",
-    "ListEventTrackersResponseTypeDef",
-    "ListFiltersResponseTypeDef",
+    "DatasetImportJobOutputTypeDef",
+    "ListDatasetExportJobsResponseOutputTypeDef",
+    "DescribeDatasetGroupResponseOutputTypeDef",
+    "ListDatasetGroupsResponseOutputTypeDef",
+    "ListDatasetImportJobsResponseOutputTypeDef",
+    "DatasetOutputTypeDef",
+    "DescribeSchemaResponseOutputTypeDef",
+    "ListSchemasResponseOutputTypeDef",
+    "ListDatasetsResponseOutputTypeDef",
+    "DefaultHyperParameterRangesOutputTypeDef",
+    "DescribeEventTrackerResponseOutputTypeDef",
+    "DescribeFeatureTransformationResponseOutputTypeDef",
+    "DescribeFilterResponseOutputTypeDef",
+    "DescribeRecipeResponseOutputTypeDef",
+    "ListEventTrackersResponseOutputTypeDef",
+    "ListFiltersResponseOutputTypeDef",
+    "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
-    "ListMetricAttributionsResponseTypeDef",
-    "ListRecipesResponseTypeDef",
-    "ListSolutionVersionsResponseTypeDef",
-    "ListSolutionsResponseTypeDef",
+    "ListMetricAttributionMetricsResponseOutputTypeDef",
+    "ListMetricAttributionsResponseOutputTypeDef",
+    "ListRecipesResponseOutputTypeDef",
+    "ListSolutionVersionsResponseOutputTypeDef",
+    "ListSolutionsResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
-    "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
-    "BatchSegmentJobTypeDef",
+    "DescribeBatchInferenceJobResponseOutputTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
+    "DescribeBatchSegmentJobResponseOutputTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
-    "DatasetExportJobTypeDef",
+    "DescribeDatasetExportJobResponseOutputTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
-    "MetricAttributionTypeDef",
+    "DescribeMetricAttributionResponseOutputTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
-    "CampaignTypeDef",
-    "DescribeDatasetImportJobResponseTypeDef",
-    "DescribeDatasetResponseTypeDef",
-    "AlgorithmTypeDef",
+    "CampaignOutputTypeDef",
+    "DescribeDatasetImportJobResponseOutputTypeDef",
+    "DescribeDatasetResponseOutputTypeDef",
+    "AlgorithmOutputTypeDef",
+    "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
+    "RecommenderSummaryOutputTypeDef",
+    "RecommenderUpdateSummaryOutputTypeDef",
     "CreateRecommenderRequestRequestTypeDef",
-    "RecommenderSummaryTypeDef",
-    "RecommenderUpdateSummaryTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
-    "DescribeBatchInferenceJobResponseTypeDef",
-    "DescribeBatchSegmentJobResponseTypeDef",
-    "DescribeDatasetExportJobResponseTypeDef",
-    "DescribeMetricAttributionResponseTypeDef",
-    "DescribeCampaignResponseTypeDef",
-    "DescribeAlgorithmResponseTypeDef",
+    "DescribeCampaignResponseOutputTypeDef",
+    "DescribeAlgorithmResponseOutputTypeDef",
+    "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
-    "ListRecommendersResponseTypeDef",
-    "RecommenderTypeDef",
+    "ListRecommendersResponseOutputTypeDef",
+    "RecommenderOutputTypeDef",
+    "SolutionOutputTypeDef",
+    "SolutionVersionOutputTypeDef",
     "CreateSolutionRequestRequestTypeDef",
-    "SolutionTypeDef",
-    "SolutionVersionTypeDef",
-    "DescribeRecommenderResponseTypeDef",
-    "DescribeSolutionResponseTypeDef",
-    "DescribeSolutionVersionResponseTypeDef",
+    "DescribeRecommenderResponseOutputTypeDef",
+    "DescribeSolutionResponseOutputTypeDef",
+    "DescribeSolutionVersionResponseOutputTypeDef",
 )
 
-AlgorithmImageTypeDef = TypedDict(
-    "AlgorithmImageTypeDef",
+AlgorithmImageOutputTypeDef = TypedDict(
+    "AlgorithmImageOutputTypeDef",
     {
         "name": str,
         "dockerURI": str,
     },
 )
 
+AutoMLConfigOutputTypeDef = TypedDict(
+    "AutoMLConfigOutputTypeDef",
+    {
+        "metricName": str,
+        "recipeList": List[str],
+    },
+)
+
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
 )
 
-AutoMLResultTypeDef = TypedDict(
-    "AutoMLResultTypeDef",
+AutoMLResultOutputTypeDef = TypedDict(
+    "AutoMLResultOutputTypeDef",
     {
         "bestRecipeArn": str,
     },
 )
 
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
@@ -290,69 +310,93 @@
 )
 
 
 class S3DataConfigTypeDef(_RequiredS3DataConfigTypeDef, _OptionalS3DataConfigTypeDef):
     pass
 
 
-BatchInferenceJobSummaryTypeDef = TypedDict(
-    "BatchInferenceJobSummaryTypeDef",
+BatchInferenceJobSummaryOutputTypeDef = TypedDict(
+    "BatchInferenceJobSummaryOutputTypeDef",
     {
         "batchInferenceJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
 )
 
-BatchSegmentJobSummaryTypeDef = TypedDict(
-    "BatchSegmentJobSummaryTypeDef",
+BatchSegmentJobSummaryOutputTypeDef = TypedDict(
+    "BatchSegmentJobSummaryOutputTypeDef",
     {
         "batchSegmentJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
 )
 
+CampaignConfigOutputTypeDef = TypedDict(
+    "CampaignConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": Dict[str, str],
+    },
+)
+
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
 
-CampaignSummaryTypeDef = TypedDict(
-    "CampaignSummaryTypeDef",
+CampaignSummaryOutputTypeDef = TypedDict(
+    "CampaignSummaryOutputTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
 )
 
+CategoricalHyperParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalHyperParameterRangeOutputTypeDef",
+    {
+        "name": str,
+        "values": List[str],
+    },
+)
+
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
+ContinuousHyperParameterRangeOutputTypeDef = TypedDict(
+    "ContinuousHyperParameterRangeOutputTypeDef",
+    {
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+    },
+)
+
 ContinuousHyperParameterRangeTypeDef = TypedDict(
     "ContinuousHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
     },
@@ -363,48 +407,48 @@
     "TagTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
     },
 )
 
-CreateBatchInferenceJobResponseTypeDef = TypedDict(
-    "CreateBatchInferenceJobResponseTypeDef",
+CreateBatchInferenceJobResponseOutputTypeDef = TypedDict(
+    "CreateBatchInferenceJobResponseOutputTypeDef",
     {
         "batchInferenceJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBatchSegmentJobResponseTypeDef = TypedDict(
-    "CreateBatchSegmentJobResponseTypeDef",
+CreateBatchSegmentJobResponseOutputTypeDef = TypedDict(
+    "CreateBatchSegmentJobResponseOutputTypeDef",
     {
         "batchSegmentJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
+CreateCampaignResponseOutputTypeDef = TypedDict(
+    "CreateCampaignResponseOutputTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetExportJobResponseTypeDef = TypedDict(
-    "CreateDatasetExportJobResponseTypeDef",
+CreateDatasetExportJobResponseOutputTypeDef = TypedDict(
+    "CreateDatasetExportJobResponseOutputTypeDef",
     {
         "datasetExportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
+CreateDatasetGroupResponseOutputTypeDef = TypedDict(
+    "CreateDatasetGroupResponseOutputTypeDef",
     {
         "datasetGroupArn": str,
         "domain": DomainType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -412,41 +456,41 @@
     "DataSourceTypeDef",
     {
         "dataLocation": str,
     },
     total=False,
 )
 
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
+CreateDatasetImportJobResponseOutputTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseOutputTypeDef",
     {
         "datasetImportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
+CreateDatasetResponseOutputTypeDef = TypedDict(
+    "CreateDatasetResponseOutputTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEventTrackerResponseTypeDef = TypedDict(
-    "CreateEventTrackerResponseTypeDef",
+CreateEventTrackerResponseOutputTypeDef = TypedDict(
+    "CreateEventTrackerResponseOutputTypeDef",
     {
         "eventTrackerArn": str,
         "trackingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
+CreateFilterResponseOutputTypeDef = TypedDict(
+    "CreateFilterResponseOutputTypeDef",
     {
         "filterArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricAttributeTypeDef = TypedDict(
@@ -454,24 +498,24 @@
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
-CreateMetricAttributionResponseTypeDef = TypedDict(
-    "CreateMetricAttributionResponseTypeDef",
+CreateMetricAttributionResponseOutputTypeDef = TypedDict(
+    "CreateMetricAttributionResponseOutputTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRecommenderResponseTypeDef = TypedDict(
-    "CreateRecommenderResponseTypeDef",
+CreateRecommenderResponseOutputTypeDef = TypedDict(
+    "CreateRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
@@ -492,158 +536,165 @@
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
+CreateSchemaResponseOutputTypeDef = TypedDict(
+    "CreateSchemaResponseOutputTypeDef",
     {
         "schemaArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionResponseTypeDef = TypedDict(
-    "CreateSolutionResponseTypeDef",
+CreateSolutionResponseOutputTypeDef = TypedDict(
+    "CreateSolutionResponseOutputTypeDef",
     {
         "solutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionVersionResponseTypeDef = TypedDict(
-    "CreateSolutionVersionResponseTypeDef",
+CreateSolutionVersionResponseOutputTypeDef = TypedDict(
+    "CreateSolutionVersionResponseOutputTypeDef",
     {
         "solutionVersionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetExportJobSummaryTypeDef = TypedDict(
-    "DatasetExportJobSummaryTypeDef",
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "dataLocation": str,
+    },
+)
+
+DatasetExportJobSummaryOutputTypeDef = TypedDict(
+    "DatasetExportJobSummaryOutputTypeDef",
     {
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
 )
 
-DatasetGroupSummaryTypeDef = TypedDict(
-    "DatasetGroupSummaryTypeDef",
+DatasetGroupOutputTypeDef = TypedDict(
+    "DatasetGroupOutputTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
+        "roleArn": str,
+        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetGroupTypeDef = TypedDict(
-    "DatasetGroupTypeDef",
+DatasetGroupSummaryOutputTypeDef = TypedDict(
+    "DatasetGroupSummaryOutputTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
-        "roleArn": str,
-        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetImportJobSummaryTypeDef = TypedDict(
-    "DatasetImportJobSummaryTypeDef",
+DatasetImportJobSummaryOutputTypeDef = TypedDict(
+    "DatasetImportJobSummaryOutputTypeDef",
     {
         "datasetImportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
     },
 )
 
-DatasetSchemaSummaryTypeDef = TypedDict(
-    "DatasetSchemaSummaryTypeDef",
+DatasetUpdateSummaryOutputTypeDef = TypedDict(
+    "DatasetUpdateSummaryOutputTypeDef",
     {
-        "name": str,
         "schemaArn": str,
+        "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "domain": DomainType,
     },
 )
 
-DatasetSchemaTypeDef = TypedDict(
-    "DatasetSchemaTypeDef",
+DatasetSchemaOutputTypeDef = TypedDict(
+    "DatasetSchemaOutputTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "schema": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
 )
 
-DatasetSummaryTypeDef = TypedDict(
-    "DatasetSummaryTypeDef",
+DatasetSchemaSummaryOutputTypeDef = TypedDict(
+    "DatasetSchemaSummaryOutputTypeDef",
     {
         "name": str,
-        "datasetArn": str,
-        "datasetType": str,
-        "status": str,
+        "schemaArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
+        "domain": DomainType,
     },
 )
 
-DatasetUpdateSummaryTypeDef = TypedDict(
-    "DatasetUpdateSummaryTypeDef",
+DatasetSummaryOutputTypeDef = TypedDict(
+    "DatasetSummaryOutputTypeDef",
     {
-        "schemaArn": str,
+        "name": str,
+        "datasetArn": str,
+        "datasetType": str,
         "status": str,
-        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
-    "DefaultCategoricalHyperParameterRangeTypeDef",
+DefaultCategoricalHyperParameterRangeOutputTypeDef = TypedDict(
+    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
     {
         "name": str,
         "values": List[str],
         "isTunable": bool,
     },
 )
 
-DefaultContinuousHyperParameterRangeTypeDef = TypedDict(
-    "DefaultContinuousHyperParameterRangeTypeDef",
+DefaultContinuousHyperParameterRangeOutputTypeDef = TypedDict(
+    "DefaultContinuousHyperParameterRangeOutputTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
         "isTunable": bool,
     },
 )
 
-DefaultIntegerHyperParameterRangeTypeDef = TypedDict(
-    "DefaultIntegerHyperParameterRangeTypeDef",
+DefaultIntegerHyperParameterRangeOutputTypeDef = TypedDict(
+    "DefaultIntegerHyperParameterRangeOutputTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
         "isTunable": bool,
     },
 )
@@ -770,16 +821,16 @@
 DescribeEventTrackerRequestRequestTypeDef = TypedDict(
     "DescribeEventTrackerRequestRequestTypeDef",
     {
         "eventTrackerArn": str,
     },
 )
 
-EventTrackerTypeDef = TypedDict(
-    "EventTrackerTypeDef",
+EventTrackerOutputTypeDef = TypedDict(
+    "EventTrackerOutputTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "accountId": str,
         "trackingId": str,
         "datasetGroupArn": str,
         "status": str,
@@ -791,16 +842,16 @@
 DescribeFeatureTransformationRequestRequestTypeDef = TypedDict(
     "DescribeFeatureTransformationRequestRequestTypeDef",
     {
         "featureTransformationArn": str,
     },
 )
 
-FeatureTransformationTypeDef = TypedDict(
-    "FeatureTransformationTypeDef",
+FeatureTransformationOutputTypeDef = TypedDict(
+    "FeatureTransformationOutputTypeDef",
     {
         "name": str,
         "featureTransformationArn": str,
         "defaultParameters": Dict[str, str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
@@ -810,16 +861,16 @@
 DescribeFilterRequestRequestTypeDef = TypedDict(
     "DescribeFilterRequestRequestTypeDef",
     {
         "filterArn": str,
     },
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -838,16 +889,16 @@
 DescribeRecipeRequestRequestTypeDef = TypedDict(
     "DescribeRecipeRequestRequestTypeDef",
     {
         "recipeArn": str,
     },
 )
 
-RecipeTypeDef = TypedDict(
-    "RecipeTypeDef",
+RecipeOutputTypeDef = TypedDict(
+    "RecipeOutputTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "algorithmArn": str,
         "featureTransformationArn": str,
         "status": str,
         "description": str,
@@ -888,27 +939,27 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EventTrackerSummaryTypeDef = TypedDict(
-    "EventTrackerSummaryTypeDef",
+EventTrackerSummaryOutputTypeDef = TypedDict(
+    "EventTrackerSummaryOutputTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-FilterSummaryTypeDef = TypedDict(
-    "FilterSummaryTypeDef",
+FilterSummaryOutputTypeDef = TypedDict(
+    "FilterSummaryOutputTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -919,23 +970,40 @@
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
-GetSolutionMetricsResponseTypeDef = TypedDict(
-    "GetSolutionMetricsResponseTypeDef",
+GetSolutionMetricsResponseOutputTypeDef = TypedDict(
+    "GetSolutionMetricsResponseOutputTypeDef",
     {
         "solutionVersionArn": str,
         "metrics": Dict[str, float],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+HPOObjectiveOutputTypeDef = TypedDict(
+    "HPOObjectiveOutputTypeDef",
+    {
+        "type": str,
+        "metricName": str,
+        "metricRegex": str,
+    },
+)
+
+HPOResourceConfigOutputTypeDef = TypedDict(
+    "HPOResourceConfigOutputTypeDef",
+    {
+        "maxNumberOfTrainingJobs": str,
+        "maxParallelTrainingJobs": str,
+    },
+)
+
 HPOObjectiveTypeDef = TypedDict(
     "HPOObjectiveTypeDef",
     {
         "type": str,
         "metricName": str,
         "metricRegex": str,
     },
@@ -947,14 +1015,23 @@
     {
         "maxNumberOfTrainingJobs": str,
         "maxParallelTrainingJobs": str,
     },
     total=False,
 )
 
+IntegerHyperParameterRangeOutputTypeDef = TypedDict(
+    "IntegerHyperParameterRangeOutputTypeDef",
+    {
+        "name": str,
+        "minValue": int,
+        "maxValue": int,
+    },
+)
+
 IntegerHyperParameterRangeTypeDef = TypedDict(
     "IntegerHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
     },
@@ -1145,14 +1222,23 @@
         "metricAttributionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+MetricAttributeOutputTypeDef = TypedDict(
+    "MetricAttributeOutputTypeDef",
+    {
+        "eventType": str,
+        "metricName": str,
+        "expression": str,
+    },
+)
+
 ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef = TypedDict(
     "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     {
         "datasetGroupArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1164,16 +1250,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-MetricAttributionSummaryTypeDef = TypedDict(
-    "MetricAttributionSummaryTypeDef",
+MetricAttributionSummaryOutputTypeDef = TypedDict(
+    "MetricAttributionSummaryOutputTypeDef",
     {
         "name": str,
         "metricAttributionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -1197,16 +1283,16 @@
         "nextToken": str,
         "maxResults": int,
         "domain": DomainType,
     },
     total=False,
 )
 
-RecipeSummaryTypeDef = TypedDict(
-    "RecipeSummaryTypeDef",
+RecipeSummaryOutputTypeDef = TypedDict(
+    "RecipeSummaryOutputTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
@@ -1264,16 +1350,16 @@
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionVersionSummaryTypeDef = TypedDict(
-    "SolutionVersionSummaryTypeDef",
+SolutionVersionSummaryOutputTypeDef = TypedDict(
+    "SolutionVersionSummaryOutputTypeDef",
     {
         "solutionVersionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
@@ -1294,16 +1380,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionSummaryTypeDef = TypedDict(
-    "SolutionSummaryTypeDef",
+SolutionSummaryOutputTypeDef = TypedDict(
+    "SolutionSummaryOutputTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recipeArn": str,
@@ -1313,14 +1399,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "tagKey": str,
+        "tagValue": str,
+    },
+)
+
+OptimizationObjectiveOutputTypeDef = TypedDict(
+    "OptimizationObjectiveOutputTypeDef",
+    {
+        "itemAttribute": str,
+        "objectiveSensitivity": ObjectiveSensitivityType,
+    },
+)
+
 OptimizationObjectiveTypeDef = TypedDict(
     "OptimizationObjectiveTypeDef",
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
     },
     total=False,
@@ -1332,14 +1434,21 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+TrainingDataConfigOutputTypeDef = TypedDict(
+    "TrainingDataConfigOutputTypeDef",
+    {
+        "excludedDatasetColumns": Dict[str, List[str]],
+    },
+)
+
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
         "excludedDatasetColumns": Mapping[str, Sequence[str]],
     },
     total=False,
 )
@@ -1351,45 +1460,45 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TunedHPOParamsTypeDef = TypedDict(
-    "TunedHPOParamsTypeDef",
+TunedHPOParamsOutputTypeDef = TypedDict(
+    "TunedHPOParamsOutputTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
 )
 
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StartRecommenderResponseTypeDef = TypedDict(
-    "StartRecommenderResponseTypeDef",
+StartRecommenderResponseOutputTypeDef = TypedDict(
+    "StartRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRecommenderRequestRequestTypeDef = TypedDict(
     "StopRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StopRecommenderResponseTypeDef = TypedDict(
-    "StopRecommenderResponseTypeDef",
+StopRecommenderResponseOutputTypeDef = TypedDict(
+    "StopRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopSolutionVersionCreationRequestRequestTypeDef = TypedDict(
@@ -1403,48 +1512,48 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
+UpdateCampaignResponseOutputTypeDef = TypedDict(
+    "UpdateCampaignResponseOutputTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDatasetRequestRequestTypeDef = TypedDict(
     "UpdateDatasetRequestRequestTypeDef",
     {
         "datasetArn": str,
         "schemaArn": str,
     },
 )
 
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
+UpdateDatasetResponseOutputTypeDef = TypedDict(
+    "UpdateDatasetResponseOutputTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateMetricAttributionResponseTypeDef = TypedDict(
-    "UpdateMetricAttributionResponseTypeDef",
+UpdateMetricAttributionResponseOutputTypeDef = TypedDict(
+    "UpdateMetricAttributionResponseOutputTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRecommenderResponseTypeDef = TypedDict(
-    "UpdateRecommenderResponseTypeDef",
+UpdateRecommenderResponseOutputTypeDef = TypedDict(
+    "UpdateRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchInferenceJobInputTypeDef = TypedDict(
@@ -1499,38 +1608,38 @@
 
 class MetricAttributionOutputTypeDef(
     _RequiredMetricAttributionOutputTypeDef, _OptionalMetricAttributionOutputTypeDef
 ):
     pass
 
 
-ListBatchInferenceJobsResponseTypeDef = TypedDict(
-    "ListBatchInferenceJobsResponseTypeDef",
+ListBatchInferenceJobsResponseOutputTypeDef = TypedDict(
+    "ListBatchInferenceJobsResponseOutputTypeDef",
     {
-        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
+        "batchInferenceJobs": List[BatchInferenceJobSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBatchSegmentJobsResponseTypeDef = TypedDict(
-    "ListBatchSegmentJobsResponseTypeDef",
+ListBatchSegmentJobsResponseOutputTypeDef = TypedDict(
+    "ListBatchSegmentJobsResponseOutputTypeDef",
     {
-        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
+        "batchSegmentJobs": List[BatchSegmentJobSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CampaignUpdateSummaryTypeDef = TypedDict(
-    "CampaignUpdateSummaryTypeDef",
+CampaignUpdateSummaryOutputTypeDef = TypedDict(
+    "CampaignUpdateSummaryOutputTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigTypeDef,
+        "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
@@ -1553,18 +1662,18 @@
 
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
 
-ListCampaignsResponseTypeDef = TypedDict(
-    "ListCampaignsResponseTypeDef",
+ListCampaignsResponseOutputTypeDef = TypedDict(
+    "ListCampaignsResponseOutputTypeDef",
     {
-        "campaigns": List[CampaignSummaryTypeDef],
+        "campaigns": List[CampaignSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
@@ -1705,22 +1814,14 @@
 class CreateSolutionVersionRequestRequestTypeDef(
     _RequiredCreateSolutionVersionRequestRequestTypeDef,
     _OptionalCreateSolutionVersionRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1748,250 +1849,257 @@
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
 
-DatasetImportJobTypeDef = TypedDict(
-    "DatasetImportJobTypeDef",
+DatasetImportJobOutputTypeDef = TypedDict(
+    "DatasetImportJobOutputTypeDef",
     {
         "jobName": str,
         "datasetImportJobArn": str,
         "datasetArn": str,
-        "dataSource": DataSourceTypeDef,
+        "dataSource": DataSourceOutputTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
 )
 
-ListMetricAttributionMetricsResponseTypeDef = TypedDict(
-    "ListMetricAttributionMetricsResponseTypeDef",
+ListDatasetExportJobsResponseOutputTypeDef = TypedDict(
+    "ListDatasetExportJobsResponseOutputTypeDef",
     {
-        "metrics": List[MetricAttributeTypeDef],
+        "datasetExportJobs": List[DatasetExportJobSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetExportJobsResponseTypeDef = TypedDict(
-    "ListDatasetExportJobsResponseTypeDef",
+DescribeDatasetGroupResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseOutputTypeDef",
     {
-        "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
-        "nextToken": str,
+        "datasetGroup": DatasetGroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetGroupsResponseTypeDef = TypedDict(
-    "ListDatasetGroupsResponseTypeDef",
+ListDatasetGroupsResponseOutputTypeDef = TypedDict(
+    "ListDatasetGroupsResponseOutputTypeDef",
     {
-        "datasetGroups": List[DatasetGroupSummaryTypeDef],
+        "datasetGroups": List[DatasetGroupSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
+ListDatasetImportJobsResponseOutputTypeDef = TypedDict(
+    "ListDatasetImportJobsResponseOutputTypeDef",
     {
-        "datasetGroup": DatasetGroupTypeDef,
+        "datasetImportJobs": List[DatasetImportJobSummaryOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetImportJobsResponseTypeDef = TypedDict(
-    "ListDatasetImportJobsResponseTypeDef",
+DatasetOutputTypeDef = TypedDict(
+    "DatasetOutputTypeDef",
     {
-        "datasetImportJobs": List[DatasetImportJobSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryOutputTypeDef,
     },
 )
 
-ListSchemasResponseTypeDef = TypedDict(
-    "ListSchemasResponseTypeDef",
+DescribeSchemaResponseOutputTypeDef = TypedDict(
+    "DescribeSchemaResponseOutputTypeDef",
     {
-        "schemas": List[DatasetSchemaSummaryTypeDef],
-        "nextToken": str,
+        "schema": DatasetSchemaOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
+ListSchemasResponseOutputTypeDef = TypedDict(
+    "ListSchemasResponseOutputTypeDef",
     {
-        "schema": DatasetSchemaTypeDef,
+        "schemas": List[DatasetSchemaSummaryOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetsResponseTypeDef = TypedDict(
-    "ListDatasetsResponseTypeDef",
+ListDatasetsResponseOutputTypeDef = TypedDict(
+    "ListDatasetsResponseOutputTypeDef",
     {
-        "datasets": List[DatasetSummaryTypeDef],
+        "datasets": List[DatasetSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
+DefaultHyperParameterRangesOutputTypeDef = TypedDict(
+    "DefaultHyperParameterRangesOutputTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
-        "schemaArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
+        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeOutputTypeDef],
+        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeOutputTypeDef],
+        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeOutputTypeDef],
     },
 )
 
-DefaultHyperParameterRangesTypeDef = TypedDict(
-    "DefaultHyperParameterRangesTypeDef",
+DescribeEventTrackerResponseOutputTypeDef = TypedDict(
+    "DescribeEventTrackerResponseOutputTypeDef",
     {
-        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
-        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
-        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeTypeDef],
+        "eventTracker": EventTrackerOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventTrackerResponseTypeDef = TypedDict(
-    "DescribeEventTrackerResponseTypeDef",
+DescribeFeatureTransformationResponseOutputTypeDef = TypedDict(
+    "DescribeFeatureTransformationResponseOutputTypeDef",
     {
-        "eventTracker": EventTrackerTypeDef,
+        "featureTransformation": FeatureTransformationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFeatureTransformationResponseTypeDef = TypedDict(
-    "DescribeFeatureTransformationResponseTypeDef",
+DescribeFilterResponseOutputTypeDef = TypedDict(
+    "DescribeFilterResponseOutputTypeDef",
     {
-        "featureTransformation": FeatureTransformationTypeDef,
+        "filter": FilterOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFilterResponseTypeDef = TypedDict(
-    "DescribeFilterResponseTypeDef",
+DescribeRecipeResponseOutputTypeDef = TypedDict(
+    "DescribeRecipeResponseOutputTypeDef",
     {
-        "filter": FilterTypeDef,
+        "recipe": RecipeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecipeResponseTypeDef = TypedDict(
-    "DescribeRecipeResponseTypeDef",
+ListEventTrackersResponseOutputTypeDef = TypedDict(
+    "ListEventTrackersResponseOutputTypeDef",
     {
-        "recipe": RecipeTypeDef,
+        "eventTrackers": List[EventTrackerSummaryOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEventTrackersResponseTypeDef = TypedDict(
-    "ListEventTrackersResponseTypeDef",
+ListFiltersResponseOutputTypeDef = TypedDict(
+    "ListFiltersResponseOutputTypeDef",
     {
-        "eventTrackers": List[EventTrackerSummaryTypeDef],
+        "Filters": List[FilterSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
+HyperParameterRangesOutputTypeDef = TypedDict(
+    "HyperParameterRangesOutputTypeDef",
     {
-        "Filters": List[FilterSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "integerHyperParameterRanges": List[IntegerHyperParameterRangeOutputTypeDef],
+        "continuousHyperParameterRanges": List[ContinuousHyperParameterRangeOutputTypeDef],
+        "categoricalHyperParameterRanges": List[CategoricalHyperParameterRangeOutputTypeDef],
     },
 )
 
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMetricAttributionsResponseTypeDef = TypedDict(
-    "ListMetricAttributionsResponseTypeDef",
+ListMetricAttributionMetricsResponseOutputTypeDef = TypedDict(
+    "ListMetricAttributionMetricsResponseOutputTypeDef",
+    {
+        "metrics": List[MetricAttributeOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMetricAttributionsResponseOutputTypeDef = TypedDict(
+    "ListMetricAttributionsResponseOutputTypeDef",
     {
-        "metricAttributions": List[MetricAttributionSummaryTypeDef],
+        "metricAttributions": List[MetricAttributionSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRecipesResponseTypeDef = TypedDict(
-    "ListRecipesResponseTypeDef",
+ListRecipesResponseOutputTypeDef = TypedDict(
+    "ListRecipesResponseOutputTypeDef",
     {
-        "recipes": List[RecipeSummaryTypeDef],
+        "recipes": List[RecipeSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionVersionsResponseTypeDef = TypedDict(
-    "ListSolutionVersionsResponseTypeDef",
+ListSolutionVersionsResponseOutputTypeDef = TypedDict(
+    "ListSolutionVersionsResponseOutputTypeDef",
     {
-        "solutionVersions": List[SolutionVersionSummaryTypeDef],
+        "solutionVersions": List[SolutionVersionSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionsResponseTypeDef = TypedDict(
-    "ListSolutionsResponseTypeDef",
+ListSolutionsResponseOutputTypeDef = TypedDict(
+    "ListSolutionsResponseOutputTypeDef",
     {
-        "solutions": List[SolutionSummaryTypeDef],
+        "solutions": List[SolutionSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RecommenderConfigOutputTypeDef = TypedDict(
+    "RecommenderConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": Dict[str, str],
+        "minRecommendationRequestsPerSecond": int,
+        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
+    },
+)
+
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
         "minRecommendationRequestsPerSecond": int,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
-BatchInferenceJobTypeDef = TypedDict(
-    "BatchInferenceJobTypeDef",
-    {
-        "jobName": str,
-        "batchInferenceJobArn": str,
-        "filterArn": str,
-        "failureReason": str,
-        "solutionVersionArn": str,
-        "numResults": int,
-        "jobInput": BatchInferenceJobInputTypeDef,
-        "jobOutput": BatchInferenceJobOutputTypeDef,
-        "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
-        "roleArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-    },
-)
-
 _RequiredCreateBatchInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchInferenceJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
         "jobInput": BatchInferenceJobInputTypeDef,
         "jobOutput": BatchInferenceJobOutputTypeDef,
@@ -2013,29 +2121,19 @@
 class CreateBatchInferenceJobRequestRequestTypeDef(
     _RequiredCreateBatchInferenceJobRequestRequestTypeDef,
     _OptionalCreateBatchInferenceJobRequestRequestTypeDef,
 ):
     pass
 
 
-BatchSegmentJobTypeDef = TypedDict(
-    "BatchSegmentJobTypeDef",
+DescribeBatchInferenceJobResponseOutputTypeDef = TypedDict(
+    "DescribeBatchInferenceJobResponseOutputTypeDef",
     {
-        "jobName": str,
-        "batchSegmentJobArn": str,
-        "filterArn": str,
-        "failureReason": str,
-        "solutionVersionArn": str,
-        "numResults": int,
-        "jobInput": BatchSegmentJobInputTypeDef,
-        "jobOutput": BatchSegmentJobOutputTypeDef,
-        "roleArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+        "batchInferenceJob": BatchInferenceJobOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBatchSegmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchSegmentJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -2059,14 +2157,22 @@
 class CreateBatchSegmentJobRequestRequestTypeDef(
     _RequiredCreateBatchSegmentJobRequestRequestTypeDef,
     _OptionalCreateBatchSegmentJobRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeBatchSegmentJobResponseOutputTypeDef = TypedDict(
+    "DescribeBatchSegmentJobResponseOutputTypeDef",
+    {
+        "batchSegmentJob": BatchSegmentJobOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDatasetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetExportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "roleArn": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
@@ -2085,123 +2191,143 @@
 class CreateDatasetExportJobRequestRequestTypeDef(
     _RequiredCreateDatasetExportJobRequestRequestTypeDef,
     _OptionalCreateDatasetExportJobRequestRequestTypeDef,
 ):
     pass
 
 
-DatasetExportJobTypeDef = TypedDict(
-    "DatasetExportJobTypeDef",
+DescribeDatasetExportJobResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetExportJobResponseOutputTypeDef",
     {
-        "jobName": str,
-        "datasetExportJobArn": str,
-        "datasetArn": str,
-        "ingestionMode": IngestionModeType,
-        "roleArn": str,
-        "status": str,
-        "jobOutput": DatasetExportJobOutputTypeDef,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "failureReason": str,
+        "datasetExportJob": DatasetExportJobOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMetricAttributionRequestRequestTypeDef = TypedDict(
     "CreateMetricAttributionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "metrics": Sequence[MetricAttributeTypeDef],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
     },
 )
 
-MetricAttributionTypeDef = TypedDict(
-    "MetricAttributionTypeDef",
+DescribeMetricAttributionResponseOutputTypeDef = TypedDict(
+    "DescribeMetricAttributionResponseOutputTypeDef",
     {
-        "name": str,
-        "metricAttributionArn": str,
-        "datasetGroupArn": str,
-        "metricsOutputConfig": MetricAttributionOutputTypeDef,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "failureReason": str,
+        "metricAttribution": MetricAttributionOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMetricAttributionRequestRequestTypeDef = TypedDict(
     "UpdateMetricAttributionRequestRequestTypeDef",
     {
         "addMetrics": Sequence[MetricAttributeTypeDef],
         "removeMetrics": Sequence[str],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
         "metricAttributionArn": str,
     },
     total=False,
 )
 
-CampaignTypeDef = TypedDict(
-    "CampaignTypeDef",
+CampaignOutputTypeDef = TypedDict(
+    "CampaignOutputTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigTypeDef,
+        "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
+        "latestCampaignUpdate": CampaignUpdateSummaryOutputTypeDef,
     },
 )
 
-DescribeDatasetImportJobResponseTypeDef = TypedDict(
-    "DescribeDatasetImportJobResponseTypeDef",
+DescribeDatasetImportJobResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetImportJobResponseOutputTypeDef",
     {
-        "datasetImportJob": DatasetImportJobTypeDef,
+        "datasetImportJob": DatasetImportJobOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
+DescribeDatasetResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetResponseOutputTypeDef",
     {
-        "dataset": DatasetTypeDef,
+        "dataset": DatasetOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AlgorithmTypeDef = TypedDict(
-    "AlgorithmTypeDef",
+AlgorithmOutputTypeDef = TypedDict(
+    "AlgorithmOutputTypeDef",
     {
         "name": str,
         "algorithmArn": str,
-        "algorithmImage": AlgorithmImageTypeDef,
+        "algorithmImage": AlgorithmImageOutputTypeDef,
         "defaultHyperParameters": Dict[str, str],
-        "defaultHyperParameterRanges": DefaultHyperParameterRangesTypeDef,
+        "defaultHyperParameterRanges": DefaultHyperParameterRangesOutputTypeDef,
         "defaultResourceConfig": Dict[str, str],
         "trainingInputMode": str,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
+HPOConfigOutputTypeDef = TypedDict(
+    "HPOConfigOutputTypeDef",
+    {
+        "hpoObjective": HPOObjectiveOutputTypeDef,
+        "hpoResourceConfig": HPOResourceConfigOutputTypeDef,
+        "algorithmHyperParameterRanges": HyperParameterRangesOutputTypeDef,
+    },
+)
+
 HPOConfigTypeDef = TypedDict(
     "HPOConfigTypeDef",
     {
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
         "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
+RecommenderSummaryOutputTypeDef = TypedDict(
+    "RecommenderSummaryOutputTypeDef",
+    {
+        "name": str,
+        "recommenderArn": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+    },
+)
+
+RecommenderUpdateSummaryOutputTypeDef = TypedDict(
+    "RecommenderUpdateSummaryOutputTypeDef",
+    {
+        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "status": str,
+        "failureReason": str,
+    },
+)
+
 _RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecommenderRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "recipeArn": str,
     },
@@ -2218,92 +2344,48 @@
 
 class CreateRecommenderRequestRequestTypeDef(
     _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
 ):
     pass
 
 
-RecommenderSummaryTypeDef = TypedDict(
-    "RecommenderSummaryTypeDef",
-    {
-        "name": str,
-        "recommenderArn": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-    },
-)
-
-RecommenderUpdateSummaryTypeDef = TypedDict(
-    "RecommenderUpdateSummaryTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "status": str,
-        "failureReason": str,
-    },
-)
-
 UpdateRecommenderRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
 
-DescribeBatchInferenceJobResponseTypeDef = TypedDict(
-    "DescribeBatchInferenceJobResponseTypeDef",
-    {
-        "batchInferenceJob": BatchInferenceJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBatchSegmentJobResponseTypeDef = TypedDict(
-    "DescribeBatchSegmentJobResponseTypeDef",
-    {
-        "batchSegmentJob": BatchSegmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeDatasetExportJobResponseTypeDef = TypedDict(
-    "DescribeDatasetExportJobResponseTypeDef",
-    {
-        "datasetExportJob": DatasetExportJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeMetricAttributionResponseTypeDef = TypedDict(
-    "DescribeMetricAttributionResponseTypeDef",
+DescribeCampaignResponseOutputTypeDef = TypedDict(
+    "DescribeCampaignResponseOutputTypeDef",
     {
-        "metricAttribution": MetricAttributionTypeDef,
+        "campaign": CampaignOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCampaignResponseTypeDef = TypedDict(
-    "DescribeCampaignResponseTypeDef",
+DescribeAlgorithmResponseOutputTypeDef = TypedDict(
+    "DescribeAlgorithmResponseOutputTypeDef",
     {
-        "campaign": CampaignTypeDef,
+        "algorithm": AlgorithmOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAlgorithmResponseTypeDef = TypedDict(
-    "DescribeAlgorithmResponseTypeDef",
+SolutionConfigOutputTypeDef = TypedDict(
+    "SolutionConfigOutputTypeDef",
     {
-        "algorithm": AlgorithmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eventValueThreshold": str,
+        "hpoConfig": HPOConfigOutputTypeDef,
+        "algorithmHyperParameters": Dict[str, str],
+        "featureTransformationParameters": Dict[str, str],
+        "autoMLConfig": AutoMLConfigOutputTypeDef,
+        "optimizationObjective": OptimizationObjectiveOutputTypeDef,
+        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
     },
 )
 
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": str,
@@ -2313,124 +2395,124 @@
         "autoMLConfig": AutoMLConfigTypeDef,
         "optimizationObjective": OptimizationObjectiveTypeDef,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
-ListRecommendersResponseTypeDef = TypedDict(
-    "ListRecommendersResponseTypeDef",
+ListRecommendersResponseOutputTypeDef = TypedDict(
+    "ListRecommendersResponseOutputTypeDef",
     {
-        "recommenders": List[RecommenderSummaryTypeDef],
+        "recommenders": List[RecommenderSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommenderTypeDef = TypedDict(
-    "RecommenderTypeDef",
+RecommenderOutputTypeDef = TypedDict(
+    "RecommenderOutputTypeDef",
     {
         "recommenderArn": str,
         "datasetGroupArn": str,
         "name": str,
         "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
+        "recommenderConfig": RecommenderConfigOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
-        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
+        "latestRecommenderUpdate": RecommenderUpdateSummaryOutputTypeDef,
         "modelMetrics": Dict[str, float],
     },
 )
 
-_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSolutionRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-    },
-)
-_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSolutionRequestRequestTypeDef",
-    {
-        "performHPO": bool,
-        "performAutoML": bool,
-        "recipeArn": str,
-        "eventType": str,
-        "solutionConfig": SolutionConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSolutionRequestRequestTypeDef(
-    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
-):
-    pass
-
-
-SolutionTypeDef = TypedDict(
-    "SolutionTypeDef",
+SolutionOutputTypeDef = TypedDict(
+    "SolutionOutputTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "datasetGroupArn": str,
         "eventType": str,
-        "solutionConfig": SolutionConfigTypeDef,
-        "autoMLResult": AutoMLResultTypeDef,
+        "solutionConfig": SolutionConfigOutputTypeDef,
+        "autoMLResult": AutoMLResultOutputTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestSolutionVersion": SolutionVersionSummaryTypeDef,
+        "latestSolutionVersion": SolutionVersionSummaryOutputTypeDef,
     },
 )
 
-SolutionVersionTypeDef = TypedDict(
-    "SolutionVersionTypeDef",
+SolutionVersionOutputTypeDef = TypedDict(
+    "SolutionVersionOutputTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "eventType": str,
         "datasetGroupArn": str,
-        "solutionConfig": SolutionConfigTypeDef,
+        "solutionConfig": SolutionConfigOutputTypeDef,
         "trainingHours": float,
         "trainingMode": TrainingModeType,
-        "tunedHPOParams": TunedHPOParamsTypeDef,
+        "tunedHPOParams": TunedHPOParamsOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-DescribeRecommenderResponseTypeDef = TypedDict(
-    "DescribeRecommenderResponseTypeDef",
+_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSolutionRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+    },
+)
+_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSolutionRequestRequestTypeDef",
+    {
+        "performHPO": bool,
+        "performAutoML": bool,
+        "recipeArn": str,
+        "eventType": str,
+        "solutionConfig": SolutionConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSolutionRequestRequestTypeDef(
+    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
+):
+    pass
+
+
+DescribeRecommenderResponseOutputTypeDef = TypedDict(
+    "DescribeRecommenderResponseOutputTypeDef",
     {
-        "recommender": RecommenderTypeDef,
+        "recommender": RecommenderOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionResponseTypeDef = TypedDict(
-    "DescribeSolutionResponseTypeDef",
+DescribeSolutionResponseOutputTypeDef = TypedDict(
+    "DescribeSolutionResponseOutputTypeDef",
     {
-        "solution": SolutionTypeDef,
+        "solution": SolutionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionVersionResponseTypeDef = TypedDict(
-    "DescribeSolutionVersionResponseTypeDef",
+DescribeSolutionVersionResponseOutputTypeDef = TypedDict(
+    "DescribeSolutionVersionResponseOutputTypeDef",
     {
-        "solutionVersion": SolutionVersionTypeDef,
+        "solutionVersion": SolutionVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.pyi` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for personalize service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize.type_defs import AlgorithmImageTypeDef
+    from mypy_boto3_personalize.type_defs import AlgorithmImageOutputTypeDef
 
-    data: AlgorithmImageTypeDef = {...}
+    data: AlgorithmImageOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -29,54 +29,59 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AlgorithmImageTypeDef",
+    "AlgorithmImageOutputTypeDef",
+    "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
-    "AutoMLResultTypeDef",
+    "AutoMLResultOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
-    "BatchInferenceJobSummaryTypeDef",
-    "BatchSegmentJobSummaryTypeDef",
+    "BatchInferenceJobSummaryOutputTypeDef",
+    "BatchSegmentJobSummaryOutputTypeDef",
+    "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
-    "CampaignSummaryTypeDef",
+    "CampaignSummaryOutputTypeDef",
+    "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
+    "ContinuousHyperParameterRangeOutputTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
-    "CreateBatchInferenceJobResponseTypeDef",
-    "CreateBatchSegmentJobResponseTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDatasetExportJobResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
+    "CreateBatchInferenceJobResponseOutputTypeDef",
+    "CreateBatchSegmentJobResponseOutputTypeDef",
+    "CreateCampaignResponseOutputTypeDef",
+    "CreateDatasetExportJobResponseOutputTypeDef",
+    "CreateDatasetGroupResponseOutputTypeDef",
     "DataSourceTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateEventTrackerResponseTypeDef",
-    "CreateFilterResponseTypeDef",
+    "CreateDatasetImportJobResponseOutputTypeDef",
+    "CreateDatasetResponseOutputTypeDef",
+    "CreateEventTrackerResponseOutputTypeDef",
+    "CreateFilterResponseOutputTypeDef",
     "MetricAttributeTypeDef",
-    "CreateMetricAttributionResponseTypeDef",
-    "CreateRecommenderResponseTypeDef",
+    "CreateMetricAttributionResponseOutputTypeDef",
+    "CreateRecommenderResponseOutputTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "CreateSolutionResponseTypeDef",
-    "CreateSolutionVersionResponseTypeDef",
-    "DatasetExportJobSummaryTypeDef",
-    "DatasetGroupSummaryTypeDef",
-    "DatasetGroupTypeDef",
-    "DatasetImportJobSummaryTypeDef",
-    "DatasetSchemaSummaryTypeDef",
-    "DatasetSchemaTypeDef",
-    "DatasetSummaryTypeDef",
-    "DatasetUpdateSummaryTypeDef",
-    "DefaultCategoricalHyperParameterRangeTypeDef",
-    "DefaultContinuousHyperParameterRangeTypeDef",
-    "DefaultIntegerHyperParameterRangeTypeDef",
+    "CreateSchemaResponseOutputTypeDef",
+    "CreateSolutionResponseOutputTypeDef",
+    "CreateSolutionVersionResponseOutputTypeDef",
+    "DataSourceOutputTypeDef",
+    "DatasetExportJobSummaryOutputTypeDef",
+    "DatasetGroupOutputTypeDef",
+    "DatasetGroupSummaryOutputTypeDef",
+    "DatasetImportJobSummaryOutputTypeDef",
+    "DatasetUpdateSummaryOutputTypeDef",
+    "DatasetSchemaOutputTypeDef",
+    "DatasetSchemaSummaryOutputTypeDef",
+    "DatasetSummaryOutputTypeDef",
+    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
+    "DefaultContinuousHyperParameterRangeOutputTypeDef",
+    "DefaultIntegerHyperParameterRangeOutputTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteMetricAttributionRequestRequestTypeDef",
     "DeleteRecommenderRequestRequestTypeDef",
@@ -87,33 +92,36 @@
     "DescribeBatchSegmentJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DescribeDatasetExportJobRequestRequestTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeEventTrackerRequestRequestTypeDef",
-    "EventTrackerTypeDef",
+    "EventTrackerOutputTypeDef",
     "DescribeFeatureTransformationRequestRequestTypeDef",
-    "FeatureTransformationTypeDef",
+    "FeatureTransformationOutputTypeDef",
     "DescribeFilterRequestRequestTypeDef",
-    "FilterTypeDef",
+    "FilterOutputTypeDef",
     "DescribeMetricAttributionRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
-    "RecipeTypeDef",
+    "RecipeOutputTypeDef",
     "DescribeRecommenderRequestRequestTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
     "DescribeSolutionRequestRequestTypeDef",
     "DescribeSolutionVersionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "EventTrackerSummaryTypeDef",
-    "FilterSummaryTypeDef",
+    "EventTrackerSummaryOutputTypeDef",
+    "FilterSummaryOutputTypeDef",
     "GetSolutionMetricsRequestRequestTypeDef",
-    "GetSolutionMetricsResponseTypeDef",
+    "GetSolutionMetricsResponseOutputTypeDef",
+    "HPOObjectiveOutputTypeDef",
+    "HPOResourceConfigOutputTypeDef",
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
+    "IntegerHyperParameterRangeOutputTypeDef",
     "IntegerHyperParameterRangeTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchInferenceJobsRequestRequestTypeDef",
     "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestRequestTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
@@ -127,144 +135,156 @@
     "ListDatasetsRequestRequestTypeDef",
     "ListEventTrackersRequestListEventTrackersPaginateTypeDef",
     "ListEventTrackersRequestRequestTypeDef",
     "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
+    "MetricAttributeOutputTypeDef",
     "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     "ListMetricAttributionsRequestRequestTypeDef",
-    "MetricAttributionSummaryTypeDef",
+    "MetricAttributionSummaryOutputTypeDef",
     "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
-    "RecipeSummaryTypeDef",
+    "RecipeSummaryOutputTypeDef",
     "ListRecommendersRequestListRecommendersPaginateTypeDef",
     "ListRecommendersRequestRequestTypeDef",
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
-    "SolutionVersionSummaryTypeDef",
+    "SolutionVersionSummaryOutputTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListSolutionsRequestRequestTypeDef",
-    "SolutionSummaryTypeDef",
+    "SolutionSummaryOutputTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "OptimizationObjectiveOutputTypeDef",
     "OptimizationObjectiveTypeDef",
     "PaginatorConfigTypeDef",
+    "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "ResponseMetadataTypeDef",
-    "TunedHPOParamsTypeDef",
+    "TunedHPOParamsOutputTypeDef",
     "StartRecommenderRequestRequestTypeDef",
-    "StartRecommenderResponseTypeDef",
+    "StartRecommenderResponseOutputTypeDef",
     "StopRecommenderRequestRequestTypeDef",
-    "StopRecommenderResponseTypeDef",
+    "StopRecommenderResponseOutputTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCampaignResponseTypeDef",
+    "UpdateCampaignResponseOutputTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
-    "UpdateDatasetResponseTypeDef",
-    "UpdateMetricAttributionResponseTypeDef",
-    "UpdateRecommenderResponseTypeDef",
+    "UpdateDatasetResponseOutputTypeDef",
+    "UpdateMetricAttributionResponseOutputTypeDef",
+    "UpdateRecommenderResponseOutputTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
-    "ListBatchInferenceJobsResponseTypeDef",
-    "ListBatchSegmentJobsResponseTypeDef",
-    "CampaignUpdateSummaryTypeDef",
+    "ListBatchInferenceJobsResponseOutputTypeDef",
+    "ListBatchSegmentJobsResponseOutputTypeDef",
+    "CampaignUpdateSummaryOutputTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
-    "ListCampaignsResponseTypeDef",
+    "ListCampaignsResponseOutputTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
-    "DatasetImportJobTypeDef",
-    "ListMetricAttributionMetricsResponseTypeDef",
-    "ListDatasetExportJobsResponseTypeDef",
-    "ListDatasetGroupsResponseTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
-    "ListDatasetImportJobsResponseTypeDef",
-    "ListSchemasResponseTypeDef",
-    "DescribeSchemaResponseTypeDef",
-    "ListDatasetsResponseTypeDef",
-    "DatasetTypeDef",
-    "DefaultHyperParameterRangesTypeDef",
-    "DescribeEventTrackerResponseTypeDef",
-    "DescribeFeatureTransformationResponseTypeDef",
-    "DescribeFilterResponseTypeDef",
-    "DescribeRecipeResponseTypeDef",
-    "ListEventTrackersResponseTypeDef",
-    "ListFiltersResponseTypeDef",
+    "DatasetImportJobOutputTypeDef",
+    "ListDatasetExportJobsResponseOutputTypeDef",
+    "DescribeDatasetGroupResponseOutputTypeDef",
+    "ListDatasetGroupsResponseOutputTypeDef",
+    "ListDatasetImportJobsResponseOutputTypeDef",
+    "DatasetOutputTypeDef",
+    "DescribeSchemaResponseOutputTypeDef",
+    "ListSchemasResponseOutputTypeDef",
+    "ListDatasetsResponseOutputTypeDef",
+    "DefaultHyperParameterRangesOutputTypeDef",
+    "DescribeEventTrackerResponseOutputTypeDef",
+    "DescribeFeatureTransformationResponseOutputTypeDef",
+    "DescribeFilterResponseOutputTypeDef",
+    "DescribeRecipeResponseOutputTypeDef",
+    "ListEventTrackersResponseOutputTypeDef",
+    "ListFiltersResponseOutputTypeDef",
+    "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
-    "ListMetricAttributionsResponseTypeDef",
-    "ListRecipesResponseTypeDef",
-    "ListSolutionVersionsResponseTypeDef",
-    "ListSolutionsResponseTypeDef",
+    "ListMetricAttributionMetricsResponseOutputTypeDef",
+    "ListMetricAttributionsResponseOutputTypeDef",
+    "ListRecipesResponseOutputTypeDef",
+    "ListSolutionVersionsResponseOutputTypeDef",
+    "ListSolutionsResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
-    "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
-    "BatchSegmentJobTypeDef",
+    "DescribeBatchInferenceJobResponseOutputTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
+    "DescribeBatchSegmentJobResponseOutputTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
-    "DatasetExportJobTypeDef",
+    "DescribeDatasetExportJobResponseOutputTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
-    "MetricAttributionTypeDef",
+    "DescribeMetricAttributionResponseOutputTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
-    "CampaignTypeDef",
-    "DescribeDatasetImportJobResponseTypeDef",
-    "DescribeDatasetResponseTypeDef",
-    "AlgorithmTypeDef",
+    "CampaignOutputTypeDef",
+    "DescribeDatasetImportJobResponseOutputTypeDef",
+    "DescribeDatasetResponseOutputTypeDef",
+    "AlgorithmOutputTypeDef",
+    "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
+    "RecommenderSummaryOutputTypeDef",
+    "RecommenderUpdateSummaryOutputTypeDef",
     "CreateRecommenderRequestRequestTypeDef",
-    "RecommenderSummaryTypeDef",
-    "RecommenderUpdateSummaryTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
-    "DescribeBatchInferenceJobResponseTypeDef",
-    "DescribeBatchSegmentJobResponseTypeDef",
-    "DescribeDatasetExportJobResponseTypeDef",
-    "DescribeMetricAttributionResponseTypeDef",
-    "DescribeCampaignResponseTypeDef",
-    "DescribeAlgorithmResponseTypeDef",
+    "DescribeCampaignResponseOutputTypeDef",
+    "DescribeAlgorithmResponseOutputTypeDef",
+    "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
-    "ListRecommendersResponseTypeDef",
-    "RecommenderTypeDef",
+    "ListRecommendersResponseOutputTypeDef",
+    "RecommenderOutputTypeDef",
+    "SolutionOutputTypeDef",
+    "SolutionVersionOutputTypeDef",
     "CreateSolutionRequestRequestTypeDef",
-    "SolutionTypeDef",
-    "SolutionVersionTypeDef",
-    "DescribeRecommenderResponseTypeDef",
-    "DescribeSolutionResponseTypeDef",
-    "DescribeSolutionVersionResponseTypeDef",
+    "DescribeRecommenderResponseOutputTypeDef",
+    "DescribeSolutionResponseOutputTypeDef",
+    "DescribeSolutionVersionResponseOutputTypeDef",
 )
 
-AlgorithmImageTypeDef = TypedDict(
-    "AlgorithmImageTypeDef",
+AlgorithmImageOutputTypeDef = TypedDict(
+    "AlgorithmImageOutputTypeDef",
     {
         "name": str,
         "dockerURI": str,
     },
 )
 
+AutoMLConfigOutputTypeDef = TypedDict(
+    "AutoMLConfigOutputTypeDef",
+    {
+        "metricName": str,
+        "recipeList": List[str],
+    },
+)
+
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
 )
 
-AutoMLResultTypeDef = TypedDict(
-    "AutoMLResultTypeDef",
+AutoMLResultOutputTypeDef = TypedDict(
+    "AutoMLResultOutputTypeDef",
     {
         "bestRecipeArn": str,
     },
 )
 
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
@@ -287,69 +307,93 @@
     },
     total=False,
 )
 
 class S3DataConfigTypeDef(_RequiredS3DataConfigTypeDef, _OptionalS3DataConfigTypeDef):
     pass
 
-BatchInferenceJobSummaryTypeDef = TypedDict(
-    "BatchInferenceJobSummaryTypeDef",
+BatchInferenceJobSummaryOutputTypeDef = TypedDict(
+    "BatchInferenceJobSummaryOutputTypeDef",
     {
         "batchInferenceJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
 )
 
-BatchSegmentJobSummaryTypeDef = TypedDict(
-    "BatchSegmentJobSummaryTypeDef",
+BatchSegmentJobSummaryOutputTypeDef = TypedDict(
+    "BatchSegmentJobSummaryOutputTypeDef",
     {
         "batchSegmentJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
 )
 
+CampaignConfigOutputTypeDef = TypedDict(
+    "CampaignConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": Dict[str, str],
+    },
+)
+
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
 
-CampaignSummaryTypeDef = TypedDict(
-    "CampaignSummaryTypeDef",
+CampaignSummaryOutputTypeDef = TypedDict(
+    "CampaignSummaryOutputTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
 )
 
+CategoricalHyperParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalHyperParameterRangeOutputTypeDef",
+    {
+        "name": str,
+        "values": List[str],
+    },
+)
+
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
+ContinuousHyperParameterRangeOutputTypeDef = TypedDict(
+    "ContinuousHyperParameterRangeOutputTypeDef",
+    {
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+    },
+)
+
 ContinuousHyperParameterRangeTypeDef = TypedDict(
     "ContinuousHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
     },
@@ -360,48 +404,48 @@
     "TagTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
     },
 )
 
-CreateBatchInferenceJobResponseTypeDef = TypedDict(
-    "CreateBatchInferenceJobResponseTypeDef",
+CreateBatchInferenceJobResponseOutputTypeDef = TypedDict(
+    "CreateBatchInferenceJobResponseOutputTypeDef",
     {
         "batchInferenceJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBatchSegmentJobResponseTypeDef = TypedDict(
-    "CreateBatchSegmentJobResponseTypeDef",
+CreateBatchSegmentJobResponseOutputTypeDef = TypedDict(
+    "CreateBatchSegmentJobResponseOutputTypeDef",
     {
         "batchSegmentJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
+CreateCampaignResponseOutputTypeDef = TypedDict(
+    "CreateCampaignResponseOutputTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetExportJobResponseTypeDef = TypedDict(
-    "CreateDatasetExportJobResponseTypeDef",
+CreateDatasetExportJobResponseOutputTypeDef = TypedDict(
+    "CreateDatasetExportJobResponseOutputTypeDef",
     {
         "datasetExportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
+CreateDatasetGroupResponseOutputTypeDef = TypedDict(
+    "CreateDatasetGroupResponseOutputTypeDef",
     {
         "datasetGroupArn": str,
         "domain": DomainType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -409,41 +453,41 @@
     "DataSourceTypeDef",
     {
         "dataLocation": str,
     },
     total=False,
 )
 
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
+CreateDatasetImportJobResponseOutputTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseOutputTypeDef",
     {
         "datasetImportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
+CreateDatasetResponseOutputTypeDef = TypedDict(
+    "CreateDatasetResponseOutputTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEventTrackerResponseTypeDef = TypedDict(
-    "CreateEventTrackerResponseTypeDef",
+CreateEventTrackerResponseOutputTypeDef = TypedDict(
+    "CreateEventTrackerResponseOutputTypeDef",
     {
         "eventTrackerArn": str,
         "trackingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
+CreateFilterResponseOutputTypeDef = TypedDict(
+    "CreateFilterResponseOutputTypeDef",
     {
         "filterArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricAttributeTypeDef = TypedDict(
@@ -451,24 +495,24 @@
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
-CreateMetricAttributionResponseTypeDef = TypedDict(
-    "CreateMetricAttributionResponseTypeDef",
+CreateMetricAttributionResponseOutputTypeDef = TypedDict(
+    "CreateMetricAttributionResponseOutputTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRecommenderResponseTypeDef = TypedDict(
-    "CreateRecommenderResponseTypeDef",
+CreateRecommenderResponseOutputTypeDef = TypedDict(
+    "CreateRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
@@ -487,158 +531,165 @@
 )
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
+CreateSchemaResponseOutputTypeDef = TypedDict(
+    "CreateSchemaResponseOutputTypeDef",
     {
         "schemaArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionResponseTypeDef = TypedDict(
-    "CreateSolutionResponseTypeDef",
+CreateSolutionResponseOutputTypeDef = TypedDict(
+    "CreateSolutionResponseOutputTypeDef",
     {
         "solutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionVersionResponseTypeDef = TypedDict(
-    "CreateSolutionVersionResponseTypeDef",
+CreateSolutionVersionResponseOutputTypeDef = TypedDict(
+    "CreateSolutionVersionResponseOutputTypeDef",
     {
         "solutionVersionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetExportJobSummaryTypeDef = TypedDict(
-    "DatasetExportJobSummaryTypeDef",
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "dataLocation": str,
+    },
+)
+
+DatasetExportJobSummaryOutputTypeDef = TypedDict(
+    "DatasetExportJobSummaryOutputTypeDef",
     {
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
 )
 
-DatasetGroupSummaryTypeDef = TypedDict(
-    "DatasetGroupSummaryTypeDef",
+DatasetGroupOutputTypeDef = TypedDict(
+    "DatasetGroupOutputTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
+        "roleArn": str,
+        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetGroupTypeDef = TypedDict(
-    "DatasetGroupTypeDef",
+DatasetGroupSummaryOutputTypeDef = TypedDict(
+    "DatasetGroupSummaryOutputTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
-        "roleArn": str,
-        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetImportJobSummaryTypeDef = TypedDict(
-    "DatasetImportJobSummaryTypeDef",
+DatasetImportJobSummaryOutputTypeDef = TypedDict(
+    "DatasetImportJobSummaryOutputTypeDef",
     {
         "datasetImportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
     },
 )
 
-DatasetSchemaSummaryTypeDef = TypedDict(
-    "DatasetSchemaSummaryTypeDef",
+DatasetUpdateSummaryOutputTypeDef = TypedDict(
+    "DatasetUpdateSummaryOutputTypeDef",
     {
-        "name": str,
         "schemaArn": str,
+        "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "domain": DomainType,
     },
 )
 
-DatasetSchemaTypeDef = TypedDict(
-    "DatasetSchemaTypeDef",
+DatasetSchemaOutputTypeDef = TypedDict(
+    "DatasetSchemaOutputTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "schema": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
 )
 
-DatasetSummaryTypeDef = TypedDict(
-    "DatasetSummaryTypeDef",
+DatasetSchemaSummaryOutputTypeDef = TypedDict(
+    "DatasetSchemaSummaryOutputTypeDef",
     {
         "name": str,
-        "datasetArn": str,
-        "datasetType": str,
-        "status": str,
+        "schemaArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
+        "domain": DomainType,
     },
 )
 
-DatasetUpdateSummaryTypeDef = TypedDict(
-    "DatasetUpdateSummaryTypeDef",
+DatasetSummaryOutputTypeDef = TypedDict(
+    "DatasetSummaryOutputTypeDef",
     {
-        "schemaArn": str,
+        "name": str,
+        "datasetArn": str,
+        "datasetType": str,
         "status": str,
-        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
-    "DefaultCategoricalHyperParameterRangeTypeDef",
+DefaultCategoricalHyperParameterRangeOutputTypeDef = TypedDict(
+    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
     {
         "name": str,
         "values": List[str],
         "isTunable": bool,
     },
 )
 
-DefaultContinuousHyperParameterRangeTypeDef = TypedDict(
-    "DefaultContinuousHyperParameterRangeTypeDef",
+DefaultContinuousHyperParameterRangeOutputTypeDef = TypedDict(
+    "DefaultContinuousHyperParameterRangeOutputTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
         "isTunable": bool,
     },
 )
 
-DefaultIntegerHyperParameterRangeTypeDef = TypedDict(
-    "DefaultIntegerHyperParameterRangeTypeDef",
+DefaultIntegerHyperParameterRangeOutputTypeDef = TypedDict(
+    "DefaultIntegerHyperParameterRangeOutputTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
         "isTunable": bool,
     },
 )
@@ -765,16 +816,16 @@
 DescribeEventTrackerRequestRequestTypeDef = TypedDict(
     "DescribeEventTrackerRequestRequestTypeDef",
     {
         "eventTrackerArn": str,
     },
 )
 
-EventTrackerTypeDef = TypedDict(
-    "EventTrackerTypeDef",
+EventTrackerOutputTypeDef = TypedDict(
+    "EventTrackerOutputTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "accountId": str,
         "trackingId": str,
         "datasetGroupArn": str,
         "status": str,
@@ -786,16 +837,16 @@
 DescribeFeatureTransformationRequestRequestTypeDef = TypedDict(
     "DescribeFeatureTransformationRequestRequestTypeDef",
     {
         "featureTransformationArn": str,
     },
 )
 
-FeatureTransformationTypeDef = TypedDict(
-    "FeatureTransformationTypeDef",
+FeatureTransformationOutputTypeDef = TypedDict(
+    "FeatureTransformationOutputTypeDef",
     {
         "name": str,
         "featureTransformationArn": str,
         "defaultParameters": Dict[str, str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
@@ -805,16 +856,16 @@
 DescribeFilterRequestRequestTypeDef = TypedDict(
     "DescribeFilterRequestRequestTypeDef",
     {
         "filterArn": str,
     },
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -833,16 +884,16 @@
 DescribeRecipeRequestRequestTypeDef = TypedDict(
     "DescribeRecipeRequestRequestTypeDef",
     {
         "recipeArn": str,
     },
 )
 
-RecipeTypeDef = TypedDict(
-    "RecipeTypeDef",
+RecipeOutputTypeDef = TypedDict(
+    "RecipeOutputTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "algorithmArn": str,
         "featureTransformationArn": str,
         "status": str,
         "description": str,
@@ -883,27 +934,27 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EventTrackerSummaryTypeDef = TypedDict(
-    "EventTrackerSummaryTypeDef",
+EventTrackerSummaryOutputTypeDef = TypedDict(
+    "EventTrackerSummaryOutputTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-FilterSummaryTypeDef = TypedDict(
-    "FilterSummaryTypeDef",
+FilterSummaryOutputTypeDef = TypedDict(
+    "FilterSummaryOutputTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -914,23 +965,40 @@
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
-GetSolutionMetricsResponseTypeDef = TypedDict(
-    "GetSolutionMetricsResponseTypeDef",
+GetSolutionMetricsResponseOutputTypeDef = TypedDict(
+    "GetSolutionMetricsResponseOutputTypeDef",
     {
         "solutionVersionArn": str,
         "metrics": Dict[str, float],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+HPOObjectiveOutputTypeDef = TypedDict(
+    "HPOObjectiveOutputTypeDef",
+    {
+        "type": str,
+        "metricName": str,
+        "metricRegex": str,
+    },
+)
+
+HPOResourceConfigOutputTypeDef = TypedDict(
+    "HPOResourceConfigOutputTypeDef",
+    {
+        "maxNumberOfTrainingJobs": str,
+        "maxParallelTrainingJobs": str,
+    },
+)
+
 HPOObjectiveTypeDef = TypedDict(
     "HPOObjectiveTypeDef",
     {
         "type": str,
         "metricName": str,
         "metricRegex": str,
     },
@@ -942,14 +1010,23 @@
     {
         "maxNumberOfTrainingJobs": str,
         "maxParallelTrainingJobs": str,
     },
     total=False,
 )
 
+IntegerHyperParameterRangeOutputTypeDef = TypedDict(
+    "IntegerHyperParameterRangeOutputTypeDef",
+    {
+        "name": str,
+        "minValue": int,
+        "maxValue": int,
+    },
+)
+
 IntegerHyperParameterRangeTypeDef = TypedDict(
     "IntegerHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
     },
@@ -1140,14 +1217,23 @@
         "metricAttributionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+MetricAttributeOutputTypeDef = TypedDict(
+    "MetricAttributeOutputTypeDef",
+    {
+        "eventType": str,
+        "metricName": str,
+        "expression": str,
+    },
+)
+
 ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef = TypedDict(
     "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     {
         "datasetGroupArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1159,16 +1245,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-MetricAttributionSummaryTypeDef = TypedDict(
-    "MetricAttributionSummaryTypeDef",
+MetricAttributionSummaryOutputTypeDef = TypedDict(
+    "MetricAttributionSummaryOutputTypeDef",
     {
         "name": str,
         "metricAttributionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -1192,16 +1278,16 @@
         "nextToken": str,
         "maxResults": int,
         "domain": DomainType,
     },
     total=False,
 )
 
-RecipeSummaryTypeDef = TypedDict(
-    "RecipeSummaryTypeDef",
+RecipeSummaryOutputTypeDef = TypedDict(
+    "RecipeSummaryOutputTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
@@ -1259,16 +1345,16 @@
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionVersionSummaryTypeDef = TypedDict(
-    "SolutionVersionSummaryTypeDef",
+SolutionVersionSummaryOutputTypeDef = TypedDict(
+    "SolutionVersionSummaryOutputTypeDef",
     {
         "solutionVersionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
@@ -1289,16 +1375,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionSummaryTypeDef = TypedDict(
-    "SolutionSummaryTypeDef",
+SolutionSummaryOutputTypeDef = TypedDict(
+    "SolutionSummaryOutputTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recipeArn": str,
@@ -1308,14 +1394,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "tagKey": str,
+        "tagValue": str,
+    },
+)
+
+OptimizationObjectiveOutputTypeDef = TypedDict(
+    "OptimizationObjectiveOutputTypeDef",
+    {
+        "itemAttribute": str,
+        "objectiveSensitivity": ObjectiveSensitivityType,
+    },
+)
+
 OptimizationObjectiveTypeDef = TypedDict(
     "OptimizationObjectiveTypeDef",
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
     },
     total=False,
@@ -1327,14 +1429,21 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+TrainingDataConfigOutputTypeDef = TypedDict(
+    "TrainingDataConfigOutputTypeDef",
+    {
+        "excludedDatasetColumns": Dict[str, List[str]],
+    },
+)
+
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
         "excludedDatasetColumns": Mapping[str, Sequence[str]],
     },
     total=False,
 )
@@ -1346,45 +1455,45 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TunedHPOParamsTypeDef = TypedDict(
-    "TunedHPOParamsTypeDef",
+TunedHPOParamsOutputTypeDef = TypedDict(
+    "TunedHPOParamsOutputTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
 )
 
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StartRecommenderResponseTypeDef = TypedDict(
-    "StartRecommenderResponseTypeDef",
+StartRecommenderResponseOutputTypeDef = TypedDict(
+    "StartRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRecommenderRequestRequestTypeDef = TypedDict(
     "StopRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StopRecommenderResponseTypeDef = TypedDict(
-    "StopRecommenderResponseTypeDef",
+StopRecommenderResponseOutputTypeDef = TypedDict(
+    "StopRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopSolutionVersionCreationRequestRequestTypeDef = TypedDict(
@@ -1398,48 +1507,48 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
+UpdateCampaignResponseOutputTypeDef = TypedDict(
+    "UpdateCampaignResponseOutputTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDatasetRequestRequestTypeDef = TypedDict(
     "UpdateDatasetRequestRequestTypeDef",
     {
         "datasetArn": str,
         "schemaArn": str,
     },
 )
 
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
+UpdateDatasetResponseOutputTypeDef = TypedDict(
+    "UpdateDatasetResponseOutputTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateMetricAttributionResponseTypeDef = TypedDict(
-    "UpdateMetricAttributionResponseTypeDef",
+UpdateMetricAttributionResponseOutputTypeDef = TypedDict(
+    "UpdateMetricAttributionResponseOutputTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRecommenderResponseTypeDef = TypedDict(
-    "UpdateRecommenderResponseTypeDef",
+UpdateRecommenderResponseOutputTypeDef = TypedDict(
+    "UpdateRecommenderResponseOutputTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchInferenceJobInputTypeDef = TypedDict(
@@ -1492,38 +1601,38 @@
 )
 
 class MetricAttributionOutputTypeDef(
     _RequiredMetricAttributionOutputTypeDef, _OptionalMetricAttributionOutputTypeDef
 ):
     pass
 
-ListBatchInferenceJobsResponseTypeDef = TypedDict(
-    "ListBatchInferenceJobsResponseTypeDef",
+ListBatchInferenceJobsResponseOutputTypeDef = TypedDict(
+    "ListBatchInferenceJobsResponseOutputTypeDef",
     {
-        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
+        "batchInferenceJobs": List[BatchInferenceJobSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBatchSegmentJobsResponseTypeDef = TypedDict(
-    "ListBatchSegmentJobsResponseTypeDef",
+ListBatchSegmentJobsResponseOutputTypeDef = TypedDict(
+    "ListBatchSegmentJobsResponseOutputTypeDef",
     {
-        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
+        "batchSegmentJobs": List[BatchSegmentJobSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CampaignUpdateSummaryTypeDef = TypedDict(
-    "CampaignUpdateSummaryTypeDef",
+CampaignUpdateSummaryOutputTypeDef = TypedDict(
+    "CampaignUpdateSummaryOutputTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigTypeDef,
+        "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
@@ -1544,18 +1653,18 @@
 )
 
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
-ListCampaignsResponseTypeDef = TypedDict(
-    "ListCampaignsResponseTypeDef",
+ListCampaignsResponseOutputTypeDef = TypedDict(
+    "ListCampaignsResponseOutputTypeDef",
     {
-        "campaigns": List[CampaignSummaryTypeDef],
+        "campaigns": List[CampaignSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
@@ -1684,22 +1793,14 @@
 
 class CreateSolutionVersionRequestRequestTypeDef(
     _RequiredCreateSolutionVersionRequestRequestTypeDef,
     _OptionalCreateSolutionVersionRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1725,250 +1826,257 @@
 
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
-DatasetImportJobTypeDef = TypedDict(
-    "DatasetImportJobTypeDef",
+DatasetImportJobOutputTypeDef = TypedDict(
+    "DatasetImportJobOutputTypeDef",
     {
         "jobName": str,
         "datasetImportJobArn": str,
         "datasetArn": str,
-        "dataSource": DataSourceTypeDef,
+        "dataSource": DataSourceOutputTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
 )
 
-ListMetricAttributionMetricsResponseTypeDef = TypedDict(
-    "ListMetricAttributionMetricsResponseTypeDef",
+ListDatasetExportJobsResponseOutputTypeDef = TypedDict(
+    "ListDatasetExportJobsResponseOutputTypeDef",
     {
-        "metrics": List[MetricAttributeTypeDef],
+        "datasetExportJobs": List[DatasetExportJobSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetExportJobsResponseTypeDef = TypedDict(
-    "ListDatasetExportJobsResponseTypeDef",
+DescribeDatasetGroupResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseOutputTypeDef",
     {
-        "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
-        "nextToken": str,
+        "datasetGroup": DatasetGroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetGroupsResponseTypeDef = TypedDict(
-    "ListDatasetGroupsResponseTypeDef",
+ListDatasetGroupsResponseOutputTypeDef = TypedDict(
+    "ListDatasetGroupsResponseOutputTypeDef",
     {
-        "datasetGroups": List[DatasetGroupSummaryTypeDef],
+        "datasetGroups": List[DatasetGroupSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
+ListDatasetImportJobsResponseOutputTypeDef = TypedDict(
+    "ListDatasetImportJobsResponseOutputTypeDef",
     {
-        "datasetGroup": DatasetGroupTypeDef,
+        "datasetImportJobs": List[DatasetImportJobSummaryOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetImportJobsResponseTypeDef = TypedDict(
-    "ListDatasetImportJobsResponseTypeDef",
+DatasetOutputTypeDef = TypedDict(
+    "DatasetOutputTypeDef",
     {
-        "datasetImportJobs": List[DatasetImportJobSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryOutputTypeDef,
     },
 )
 
-ListSchemasResponseTypeDef = TypedDict(
-    "ListSchemasResponseTypeDef",
+DescribeSchemaResponseOutputTypeDef = TypedDict(
+    "DescribeSchemaResponseOutputTypeDef",
     {
-        "schemas": List[DatasetSchemaSummaryTypeDef],
-        "nextToken": str,
+        "schema": DatasetSchemaOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
+ListSchemasResponseOutputTypeDef = TypedDict(
+    "ListSchemasResponseOutputTypeDef",
     {
-        "schema": DatasetSchemaTypeDef,
+        "schemas": List[DatasetSchemaSummaryOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetsResponseTypeDef = TypedDict(
-    "ListDatasetsResponseTypeDef",
+ListDatasetsResponseOutputTypeDef = TypedDict(
+    "ListDatasetsResponseOutputTypeDef",
     {
-        "datasets": List[DatasetSummaryTypeDef],
+        "datasets": List[DatasetSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
+DefaultHyperParameterRangesOutputTypeDef = TypedDict(
+    "DefaultHyperParameterRangesOutputTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
-        "schemaArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
+        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeOutputTypeDef],
+        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeOutputTypeDef],
+        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeOutputTypeDef],
     },
 )
 
-DefaultHyperParameterRangesTypeDef = TypedDict(
-    "DefaultHyperParameterRangesTypeDef",
+DescribeEventTrackerResponseOutputTypeDef = TypedDict(
+    "DescribeEventTrackerResponseOutputTypeDef",
     {
-        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
-        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
-        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeTypeDef],
+        "eventTracker": EventTrackerOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventTrackerResponseTypeDef = TypedDict(
-    "DescribeEventTrackerResponseTypeDef",
+DescribeFeatureTransformationResponseOutputTypeDef = TypedDict(
+    "DescribeFeatureTransformationResponseOutputTypeDef",
     {
-        "eventTracker": EventTrackerTypeDef,
+        "featureTransformation": FeatureTransformationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFeatureTransformationResponseTypeDef = TypedDict(
-    "DescribeFeatureTransformationResponseTypeDef",
+DescribeFilterResponseOutputTypeDef = TypedDict(
+    "DescribeFilterResponseOutputTypeDef",
     {
-        "featureTransformation": FeatureTransformationTypeDef,
+        "filter": FilterOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFilterResponseTypeDef = TypedDict(
-    "DescribeFilterResponseTypeDef",
+DescribeRecipeResponseOutputTypeDef = TypedDict(
+    "DescribeRecipeResponseOutputTypeDef",
     {
-        "filter": FilterTypeDef,
+        "recipe": RecipeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecipeResponseTypeDef = TypedDict(
-    "DescribeRecipeResponseTypeDef",
+ListEventTrackersResponseOutputTypeDef = TypedDict(
+    "ListEventTrackersResponseOutputTypeDef",
     {
-        "recipe": RecipeTypeDef,
+        "eventTrackers": List[EventTrackerSummaryOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEventTrackersResponseTypeDef = TypedDict(
-    "ListEventTrackersResponseTypeDef",
+ListFiltersResponseOutputTypeDef = TypedDict(
+    "ListFiltersResponseOutputTypeDef",
     {
-        "eventTrackers": List[EventTrackerSummaryTypeDef],
+        "Filters": List[FilterSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
+HyperParameterRangesOutputTypeDef = TypedDict(
+    "HyperParameterRangesOutputTypeDef",
     {
-        "Filters": List[FilterSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "integerHyperParameterRanges": List[IntegerHyperParameterRangeOutputTypeDef],
+        "continuousHyperParameterRanges": List[ContinuousHyperParameterRangeOutputTypeDef],
+        "categoricalHyperParameterRanges": List[CategoricalHyperParameterRangeOutputTypeDef],
     },
 )
 
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMetricAttributionsResponseTypeDef = TypedDict(
-    "ListMetricAttributionsResponseTypeDef",
+ListMetricAttributionMetricsResponseOutputTypeDef = TypedDict(
+    "ListMetricAttributionMetricsResponseOutputTypeDef",
     {
-        "metricAttributions": List[MetricAttributionSummaryTypeDef],
+        "metrics": List[MetricAttributeOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRecipesResponseTypeDef = TypedDict(
-    "ListRecipesResponseTypeDef",
+ListMetricAttributionsResponseOutputTypeDef = TypedDict(
+    "ListMetricAttributionsResponseOutputTypeDef",
     {
-        "recipes": List[RecipeSummaryTypeDef],
+        "metricAttributions": List[MetricAttributionSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionVersionsResponseTypeDef = TypedDict(
-    "ListSolutionVersionsResponseTypeDef",
+ListRecipesResponseOutputTypeDef = TypedDict(
+    "ListRecipesResponseOutputTypeDef",
     {
-        "solutionVersions": List[SolutionVersionSummaryTypeDef],
+        "recipes": List[RecipeSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionsResponseTypeDef = TypedDict(
-    "ListSolutionsResponseTypeDef",
+ListSolutionVersionsResponseOutputTypeDef = TypedDict(
+    "ListSolutionVersionsResponseOutputTypeDef",
     {
-        "solutions": List[SolutionSummaryTypeDef],
+        "solutionVersions": List[SolutionVersionSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListSolutionsResponseOutputTypeDef = TypedDict(
+    "ListSolutionsResponseOutputTypeDef",
+    {
+        "solutions": List[SolutionSummaryOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RecommenderConfigOutputTypeDef = TypedDict(
+    "RecommenderConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": Dict[str, str],
+        "minRecommendationRequestsPerSecond": int,
+        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
+    },
+)
+
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
         "minRecommendationRequestsPerSecond": int,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
-BatchInferenceJobTypeDef = TypedDict(
-    "BatchInferenceJobTypeDef",
-    {
-        "jobName": str,
-        "batchInferenceJobArn": str,
-        "filterArn": str,
-        "failureReason": str,
-        "solutionVersionArn": str,
-        "numResults": int,
-        "jobInput": BatchInferenceJobInputTypeDef,
-        "jobOutput": BatchInferenceJobOutputTypeDef,
-        "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
-        "roleArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-    },
-)
-
 _RequiredCreateBatchInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchInferenceJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
         "jobInput": BatchInferenceJobInputTypeDef,
         "jobOutput": BatchInferenceJobOutputTypeDef,
@@ -1988,29 +2096,19 @@
 
 class CreateBatchInferenceJobRequestRequestTypeDef(
     _RequiredCreateBatchInferenceJobRequestRequestTypeDef,
     _OptionalCreateBatchInferenceJobRequestRequestTypeDef,
 ):
     pass
 
-BatchSegmentJobTypeDef = TypedDict(
-    "BatchSegmentJobTypeDef",
+DescribeBatchInferenceJobResponseOutputTypeDef = TypedDict(
+    "DescribeBatchInferenceJobResponseOutputTypeDef",
     {
-        "jobName": str,
-        "batchSegmentJobArn": str,
-        "filterArn": str,
-        "failureReason": str,
-        "solutionVersionArn": str,
-        "numResults": int,
-        "jobInput": BatchSegmentJobInputTypeDef,
-        "jobOutput": BatchSegmentJobOutputTypeDef,
-        "roleArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+        "batchInferenceJob": BatchInferenceJobOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBatchSegmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchSegmentJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -2032,14 +2130,22 @@
 
 class CreateBatchSegmentJobRequestRequestTypeDef(
     _RequiredCreateBatchSegmentJobRequestRequestTypeDef,
     _OptionalCreateBatchSegmentJobRequestRequestTypeDef,
 ):
     pass
 
+DescribeBatchSegmentJobResponseOutputTypeDef = TypedDict(
+    "DescribeBatchSegmentJobResponseOutputTypeDef",
+    {
+        "batchSegmentJob": BatchSegmentJobOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDatasetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetExportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "roleArn": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
@@ -2056,223 +2162,199 @@
 
 class CreateDatasetExportJobRequestRequestTypeDef(
     _RequiredCreateDatasetExportJobRequestRequestTypeDef,
     _OptionalCreateDatasetExportJobRequestRequestTypeDef,
 ):
     pass
 
-DatasetExportJobTypeDef = TypedDict(
-    "DatasetExportJobTypeDef",
+DescribeDatasetExportJobResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetExportJobResponseOutputTypeDef",
     {
-        "jobName": str,
-        "datasetExportJobArn": str,
-        "datasetArn": str,
-        "ingestionMode": IngestionModeType,
-        "roleArn": str,
-        "status": str,
-        "jobOutput": DatasetExportJobOutputTypeDef,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "failureReason": str,
+        "datasetExportJob": DatasetExportJobOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMetricAttributionRequestRequestTypeDef = TypedDict(
     "CreateMetricAttributionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "metrics": Sequence[MetricAttributeTypeDef],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
     },
 )
 
-MetricAttributionTypeDef = TypedDict(
-    "MetricAttributionTypeDef",
+DescribeMetricAttributionResponseOutputTypeDef = TypedDict(
+    "DescribeMetricAttributionResponseOutputTypeDef",
     {
-        "name": str,
-        "metricAttributionArn": str,
-        "datasetGroupArn": str,
-        "metricsOutputConfig": MetricAttributionOutputTypeDef,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "failureReason": str,
+        "metricAttribution": MetricAttributionOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMetricAttributionRequestRequestTypeDef = TypedDict(
     "UpdateMetricAttributionRequestRequestTypeDef",
     {
         "addMetrics": Sequence[MetricAttributeTypeDef],
         "removeMetrics": Sequence[str],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
         "metricAttributionArn": str,
     },
     total=False,
 )
 
-CampaignTypeDef = TypedDict(
-    "CampaignTypeDef",
+CampaignOutputTypeDef = TypedDict(
+    "CampaignOutputTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigTypeDef,
+        "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
+        "latestCampaignUpdate": CampaignUpdateSummaryOutputTypeDef,
     },
 )
 
-DescribeDatasetImportJobResponseTypeDef = TypedDict(
-    "DescribeDatasetImportJobResponseTypeDef",
+DescribeDatasetImportJobResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetImportJobResponseOutputTypeDef",
     {
-        "datasetImportJob": DatasetImportJobTypeDef,
+        "datasetImportJob": DatasetImportJobOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
+DescribeDatasetResponseOutputTypeDef = TypedDict(
+    "DescribeDatasetResponseOutputTypeDef",
     {
-        "dataset": DatasetTypeDef,
+        "dataset": DatasetOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AlgorithmTypeDef = TypedDict(
-    "AlgorithmTypeDef",
+AlgorithmOutputTypeDef = TypedDict(
+    "AlgorithmOutputTypeDef",
     {
         "name": str,
         "algorithmArn": str,
-        "algorithmImage": AlgorithmImageTypeDef,
+        "algorithmImage": AlgorithmImageOutputTypeDef,
         "defaultHyperParameters": Dict[str, str],
-        "defaultHyperParameterRanges": DefaultHyperParameterRangesTypeDef,
+        "defaultHyperParameterRanges": DefaultHyperParameterRangesOutputTypeDef,
         "defaultResourceConfig": Dict[str, str],
         "trainingInputMode": str,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
+HPOConfigOutputTypeDef = TypedDict(
+    "HPOConfigOutputTypeDef",
+    {
+        "hpoObjective": HPOObjectiveOutputTypeDef,
+        "hpoResourceConfig": HPOResourceConfigOutputTypeDef,
+        "algorithmHyperParameterRanges": HyperParameterRangesOutputTypeDef,
+    },
+)
+
 HPOConfigTypeDef = TypedDict(
     "HPOConfigTypeDef",
     {
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
         "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecommenderRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-    },
-)
-_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecommenderRequestRequestTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateRecommenderRequestRequestTypeDef(
-    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
-):
-    pass
-
-RecommenderSummaryTypeDef = TypedDict(
-    "RecommenderSummaryTypeDef",
+RecommenderSummaryOutputTypeDef = TypedDict(
+    "RecommenderSummaryOutputTypeDef",
     {
         "name": str,
         "recommenderArn": str,
         "datasetGroupArn": str,
         "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
+        "recommenderConfig": RecommenderConfigOutputTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-RecommenderUpdateSummaryTypeDef = TypedDict(
-    "RecommenderUpdateSummaryTypeDef",
+RecommenderUpdateSummaryOutputTypeDef = TypedDict(
+    "RecommenderUpdateSummaryOutputTypeDef",
     {
-        "recommenderConfig": RecommenderConfigTypeDef,
+        "recommenderConfig": RecommenderConfigOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
     },
 )
 
-UpdateRecommenderRequestRequestTypeDef = TypedDict(
-    "UpdateRecommenderRequestRequestTypeDef",
+_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecommenderRequestRequestTypeDef",
     {
-        "recommenderArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
+        "name": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
     },
 )
-
-DescribeBatchInferenceJobResponseTypeDef = TypedDict(
-    "DescribeBatchInferenceJobResponseTypeDef",
+_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecommenderRequestRequestTypeDef",
     {
-        "batchInferenceJob": BatchInferenceJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-DescribeBatchSegmentJobResponseTypeDef = TypedDict(
-    "DescribeBatchSegmentJobResponseTypeDef",
-    {
-        "batchSegmentJob": BatchSegmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class CreateRecommenderRequestRequestTypeDef(
+    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
+):
+    pass
 
-DescribeDatasetExportJobResponseTypeDef = TypedDict(
-    "DescribeDatasetExportJobResponseTypeDef",
+UpdateRecommenderRequestRequestTypeDef = TypedDict(
+    "UpdateRecommenderRequestRequestTypeDef",
     {
-        "datasetExportJob": DatasetExportJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "recommenderArn": str,
+        "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
 
-DescribeMetricAttributionResponseTypeDef = TypedDict(
-    "DescribeMetricAttributionResponseTypeDef",
+DescribeCampaignResponseOutputTypeDef = TypedDict(
+    "DescribeCampaignResponseOutputTypeDef",
     {
-        "metricAttribution": MetricAttributionTypeDef,
+        "campaign": CampaignOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCampaignResponseTypeDef = TypedDict(
-    "DescribeCampaignResponseTypeDef",
+DescribeAlgorithmResponseOutputTypeDef = TypedDict(
+    "DescribeAlgorithmResponseOutputTypeDef",
     {
-        "campaign": CampaignTypeDef,
+        "algorithm": AlgorithmOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAlgorithmResponseTypeDef = TypedDict(
-    "DescribeAlgorithmResponseTypeDef",
+SolutionConfigOutputTypeDef = TypedDict(
+    "SolutionConfigOutputTypeDef",
     {
-        "algorithm": AlgorithmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eventValueThreshold": str,
+        "hpoConfig": HPOConfigOutputTypeDef,
+        "algorithmHyperParameters": Dict[str, str],
+        "featureTransformationParameters": Dict[str, str],
+        "autoMLConfig": AutoMLConfigOutputTypeDef,
+        "optimizationObjective": OptimizationObjectiveOutputTypeDef,
+        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
     },
 )
 
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": str,
@@ -2282,122 +2364,122 @@
         "autoMLConfig": AutoMLConfigTypeDef,
         "optimizationObjective": OptimizationObjectiveTypeDef,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
-ListRecommendersResponseTypeDef = TypedDict(
-    "ListRecommendersResponseTypeDef",
+ListRecommendersResponseOutputTypeDef = TypedDict(
+    "ListRecommendersResponseOutputTypeDef",
     {
-        "recommenders": List[RecommenderSummaryTypeDef],
+        "recommenders": List[RecommenderSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommenderTypeDef = TypedDict(
-    "RecommenderTypeDef",
+RecommenderOutputTypeDef = TypedDict(
+    "RecommenderOutputTypeDef",
     {
         "recommenderArn": str,
         "datasetGroupArn": str,
         "name": str,
         "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
+        "recommenderConfig": RecommenderConfigOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
-        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
+        "latestRecommenderUpdate": RecommenderUpdateSummaryOutputTypeDef,
         "modelMetrics": Dict[str, float],
     },
 )
 
-_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSolutionRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-    },
-)
-_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSolutionRequestRequestTypeDef",
-    {
-        "performHPO": bool,
-        "performAutoML": bool,
-        "recipeArn": str,
-        "eventType": str,
-        "solutionConfig": SolutionConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSolutionRequestRequestTypeDef(
-    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
-):
-    pass
-
-SolutionTypeDef = TypedDict(
-    "SolutionTypeDef",
+SolutionOutputTypeDef = TypedDict(
+    "SolutionOutputTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "datasetGroupArn": str,
         "eventType": str,
-        "solutionConfig": SolutionConfigTypeDef,
-        "autoMLResult": AutoMLResultTypeDef,
+        "solutionConfig": SolutionConfigOutputTypeDef,
+        "autoMLResult": AutoMLResultOutputTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestSolutionVersion": SolutionVersionSummaryTypeDef,
+        "latestSolutionVersion": SolutionVersionSummaryOutputTypeDef,
     },
 )
 
-SolutionVersionTypeDef = TypedDict(
-    "SolutionVersionTypeDef",
+SolutionVersionOutputTypeDef = TypedDict(
+    "SolutionVersionOutputTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "eventType": str,
         "datasetGroupArn": str,
-        "solutionConfig": SolutionConfigTypeDef,
+        "solutionConfig": SolutionConfigOutputTypeDef,
         "trainingHours": float,
         "trainingMode": TrainingModeType,
-        "tunedHPOParams": TunedHPOParamsTypeDef,
+        "tunedHPOParams": TunedHPOParamsOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-DescribeRecommenderResponseTypeDef = TypedDict(
-    "DescribeRecommenderResponseTypeDef",
+_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSolutionRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+    },
+)
+_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSolutionRequestRequestTypeDef",
+    {
+        "performHPO": bool,
+        "performAutoML": bool,
+        "recipeArn": str,
+        "eventType": str,
+        "solutionConfig": SolutionConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSolutionRequestRequestTypeDef(
+    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
+):
+    pass
+
+DescribeRecommenderResponseOutputTypeDef = TypedDict(
+    "DescribeRecommenderResponseOutputTypeDef",
     {
-        "recommender": RecommenderTypeDef,
+        "recommender": RecommenderOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionResponseTypeDef = TypedDict(
-    "DescribeSolutionResponseTypeDef",
+DescribeSolutionResponseOutputTypeDef = TypedDict(
+    "DescribeSolutionResponseOutputTypeDef",
     {
-        "solution": SolutionTypeDef,
+        "solution": SolutionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionVersionResponseTypeDef = TypedDict(
-    "DescribeSolutionVersionResponseTypeDef",
+DescribeSolutionVersionResponseOutputTypeDef = TypedDict(
+    "DescribeSolutionVersionResponseOutputTypeDef",
     {
-        "solutionVersion": SolutionVersionTypeDef,
+        "solutionVersion": SolutionVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/PKG-INFO` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.28.3
-Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,54 +389,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize.type_defs import (
-    AlgorithmImageTypeDef,
+    AlgorithmImageOutputTypeDef,
+    AutoMLConfigOutputTypeDef,
     AutoMLConfigTypeDef,
-    AutoMLResultTypeDef,
+    AutoMLResultOutputTypeDef,
     BatchInferenceJobConfigTypeDef,
     S3DataConfigTypeDef,
-    BatchInferenceJobSummaryTypeDef,
-    BatchSegmentJobSummaryTypeDef,
+    BatchInferenceJobSummaryOutputTypeDef,
+    BatchSegmentJobSummaryOutputTypeDef,
+    CampaignConfigOutputTypeDef,
     CampaignConfigTypeDef,
-    CampaignSummaryTypeDef,
+    CampaignSummaryOutputTypeDef,
+    CategoricalHyperParameterRangeOutputTypeDef,
     CategoricalHyperParameterRangeTypeDef,
+    ContinuousHyperParameterRangeOutputTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    CreateBatchInferenceJobResponseTypeDef,
-    CreateBatchSegmentJobResponseTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDatasetExportJobResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
+    CreateBatchInferenceJobResponseOutputTypeDef,
+    CreateBatchSegmentJobResponseOutputTypeDef,
+    CreateCampaignResponseOutputTypeDef,
+    CreateDatasetExportJobResponseOutputTypeDef,
+    CreateDatasetGroupResponseOutputTypeDef,
     DataSourceTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateEventTrackerResponseTypeDef,
-    CreateFilterResponseTypeDef,
+    CreateDatasetImportJobResponseOutputTypeDef,
+    CreateDatasetResponseOutputTypeDef,
+    CreateEventTrackerResponseOutputTypeDef,
+    CreateFilterResponseOutputTypeDef,
     MetricAttributeTypeDef,
-    CreateMetricAttributionResponseTypeDef,
-    CreateRecommenderResponseTypeDef,
+    CreateMetricAttributionResponseOutputTypeDef,
+    CreateRecommenderResponseOutputTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateSolutionResponseTypeDef,
-    CreateSolutionVersionResponseTypeDef,
-    DatasetExportJobSummaryTypeDef,
-    DatasetGroupSummaryTypeDef,
-    DatasetGroupTypeDef,
-    DatasetImportJobSummaryTypeDef,
-    DatasetSchemaSummaryTypeDef,
-    DatasetSchemaTypeDef,
-    DatasetSummaryTypeDef,
-    DatasetUpdateSummaryTypeDef,
-    DefaultCategoricalHyperParameterRangeTypeDef,
-    DefaultContinuousHyperParameterRangeTypeDef,
-    DefaultIntegerHyperParameterRangeTypeDef,
+    CreateSchemaResponseOutputTypeDef,
+    CreateSolutionResponseOutputTypeDef,
+    CreateSolutionVersionResponseOutputTypeDef,
+    DataSourceOutputTypeDef,
+    DatasetExportJobSummaryOutputTypeDef,
+    DatasetGroupOutputTypeDef,
+    DatasetGroupSummaryOutputTypeDef,
+    DatasetImportJobSummaryOutputTypeDef,
+    DatasetUpdateSummaryOutputTypeDef,
+    DatasetSchemaOutputTypeDef,
+    DatasetSchemaSummaryOutputTypeDef,
+    DatasetSummaryOutputTypeDef,
+    DefaultCategoricalHyperParameterRangeOutputTypeDef,
+    DefaultContinuousHyperParameterRangeOutputTypeDef,
+    DefaultIntegerHyperParameterRangeOutputTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteMetricAttributionRequestRequestTypeDef,
     DeleteRecommenderRequestRequestTypeDef,
@@ -447,33 +452,36 @@
     DescribeBatchSegmentJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DescribeDatasetExportJobRequestRequestTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeEventTrackerRequestRequestTypeDef,
-    EventTrackerTypeDef,
+    EventTrackerOutputTypeDef,
     DescribeFeatureTransformationRequestRequestTypeDef,
-    FeatureTransformationTypeDef,
+    FeatureTransformationOutputTypeDef,
     DescribeFilterRequestRequestTypeDef,
-    FilterTypeDef,
+    FilterOutputTypeDef,
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
-    RecipeTypeDef,
+    RecipeOutputTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventTrackerSummaryTypeDef,
-    FilterSummaryTypeDef,
+    EventTrackerSummaryOutputTypeDef,
+    FilterSummaryOutputTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
-    GetSolutionMetricsResponseTypeDef,
+    GetSolutionMetricsResponseOutputTypeDef,
+    HPOObjectiveOutputTypeDef,
+    HPOResourceConfigOutputTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
+    IntegerHyperParameterRangeOutputTypeDef,
     IntegerHyperParameterRangeTypeDef,
     ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
     ListBatchInferenceJobsRequestRequestTypeDef,
     ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef,
     ListBatchSegmentJobsRequestRequestTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
@@ -487,127 +495,131 @@
     ListDatasetsRequestRequestTypeDef,
     ListEventTrackersRequestListEventTrackersPaginateTypeDef,
     ListEventTrackersRequestRequestTypeDef,
     ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
+    MetricAttributeOutputTypeDef,
     ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
-    MetricAttributionSummaryTypeDef,
+    MetricAttributionSummaryOutputTypeDef,
     ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    RecipeSummaryTypeDef,
+    RecipeSummaryOutputTypeDef,
     ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
-    SolutionVersionSummaryTypeDef,
+    SolutionVersionSummaryOutputTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
-    SolutionSummaryTypeDef,
+    SolutionSummaryOutputTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OptimizationObjectiveOutputTypeDef,
     OptimizationObjectiveTypeDef,
     PaginatorConfigTypeDef,
+    TrainingDataConfigOutputTypeDef,
     TrainingDataConfigTypeDef,
     ResponseMetadataTypeDef,
-    TunedHPOParamsTypeDef,
+    TunedHPOParamsOutputTypeDef,
     StartRecommenderRequestRequestTypeDef,
-    StartRecommenderResponseTypeDef,
+    StartRecommenderResponseOutputTypeDef,
     StopRecommenderRequestRequestTypeDef,
-    StopRecommenderResponseTypeDef,
+    StopRecommenderResponseOutputTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCampaignResponseTypeDef,
+    UpdateCampaignResponseOutputTypeDef,
     UpdateDatasetRequestRequestTypeDef,
-    UpdateDatasetResponseTypeDef,
-    UpdateMetricAttributionResponseTypeDef,
-    UpdateRecommenderResponseTypeDef,
+    UpdateDatasetResponseOutputTypeDef,
+    UpdateMetricAttributionResponseOutputTypeDef,
+    UpdateRecommenderResponseOutputTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
-    ListBatchInferenceJobsResponseTypeDef,
-    ListBatchSegmentJobsResponseTypeDef,
-    CampaignUpdateSummaryTypeDef,
+    ListBatchInferenceJobsResponseOutputTypeDef,
+    ListBatchSegmentJobsResponseOutputTypeDef,
+    CampaignUpdateSummaryOutputTypeDef,
     UpdateCampaignRequestRequestTypeDef,
-    ListCampaignsResponseTypeDef,
+    ListCampaignsResponseOutputTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
-    DatasetImportJobTypeDef,
-    ListMetricAttributionMetricsResponseTypeDef,
-    ListDatasetExportJobsResponseTypeDef,
-    ListDatasetGroupsResponseTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
-    ListDatasetImportJobsResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    DatasetTypeDef,
-    DefaultHyperParameterRangesTypeDef,
-    DescribeEventTrackerResponseTypeDef,
-    DescribeFeatureTransformationResponseTypeDef,
-    DescribeFilterResponseTypeDef,
-    DescribeRecipeResponseTypeDef,
-    ListEventTrackersResponseTypeDef,
-    ListFiltersResponseTypeDef,
+    DatasetImportJobOutputTypeDef,
+    ListDatasetExportJobsResponseOutputTypeDef,
+    DescribeDatasetGroupResponseOutputTypeDef,
+    ListDatasetGroupsResponseOutputTypeDef,
+    ListDatasetImportJobsResponseOutputTypeDef,
+    DatasetOutputTypeDef,
+    DescribeSchemaResponseOutputTypeDef,
+    ListSchemasResponseOutputTypeDef,
+    ListDatasetsResponseOutputTypeDef,
+    DefaultHyperParameterRangesOutputTypeDef,
+    DescribeEventTrackerResponseOutputTypeDef,
+    DescribeFeatureTransformationResponseOutputTypeDef,
+    DescribeFilterResponseOutputTypeDef,
+    DescribeRecipeResponseOutputTypeDef,
+    ListEventTrackersResponseOutputTypeDef,
+    ListFiltersResponseOutputTypeDef,
+    HyperParameterRangesOutputTypeDef,
     HyperParameterRangesTypeDef,
-    ListMetricAttributionsResponseTypeDef,
-    ListRecipesResponseTypeDef,
-    ListSolutionVersionsResponseTypeDef,
-    ListSolutionsResponseTypeDef,
+    ListMetricAttributionMetricsResponseOutputTypeDef,
+    ListMetricAttributionsResponseOutputTypeDef,
+    ListRecipesResponseOutputTypeDef,
+    ListSolutionVersionsResponseOutputTypeDef,
+    ListSolutionsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    RecommenderConfigOutputTypeDef,
     RecommenderConfigTypeDef,
-    BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
-    BatchSegmentJobTypeDef,
+    DescribeBatchInferenceJobResponseOutputTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
+    DescribeBatchSegmentJobResponseOutputTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
-    DatasetExportJobTypeDef,
+    DescribeDatasetExportJobResponseOutputTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
-    MetricAttributionTypeDef,
+    DescribeMetricAttributionResponseOutputTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
-    CampaignTypeDef,
-    DescribeDatasetImportJobResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    AlgorithmTypeDef,
+    CampaignOutputTypeDef,
+    DescribeDatasetImportJobResponseOutputTypeDef,
+    DescribeDatasetResponseOutputTypeDef,
+    AlgorithmOutputTypeDef,
+    HPOConfigOutputTypeDef,
     HPOConfigTypeDef,
+    RecommenderSummaryOutputTypeDef,
+    RecommenderUpdateSummaryOutputTypeDef,
     CreateRecommenderRequestRequestTypeDef,
-    RecommenderSummaryTypeDef,
-    RecommenderUpdateSummaryTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
-    DescribeBatchInferenceJobResponseTypeDef,
-    DescribeBatchSegmentJobResponseTypeDef,
-    DescribeDatasetExportJobResponseTypeDef,
-    DescribeMetricAttributionResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-    DescribeAlgorithmResponseTypeDef,
+    DescribeCampaignResponseOutputTypeDef,
+    DescribeAlgorithmResponseOutputTypeDef,
+    SolutionConfigOutputTypeDef,
     SolutionConfigTypeDef,
-    ListRecommendersResponseTypeDef,
-    RecommenderTypeDef,
+    ListRecommendersResponseOutputTypeDef,
+    RecommenderOutputTypeDef,
+    SolutionOutputTypeDef,
+    SolutionVersionOutputTypeDef,
     CreateSolutionRequestRequestTypeDef,
-    SolutionTypeDef,
-    SolutionVersionTypeDef,
-    DescribeRecommenderResponseTypeDef,
-    DescribeSolutionResponseTypeDef,
-    DescribeSolutionVersionResponseTypeDef,
+    DescribeRecommenderResponseOutputTypeDef,
+    DescribeSolutionResponseOutputTypeDef,
+    DescribeSolutionVersionResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AlgorithmImageTypeDef:
+def get_structure() -> AlgorithmImageOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/SOURCES.txt` & `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3/setup.py` & `mypy-boto3-personalize-1.28.3.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder"
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

