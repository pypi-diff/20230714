# Comparing `tmp/spark_rapids_user_tools-23.6.1-153_dcfbc66-py3-none-any.whl.zip` & `tmp/spark_rapids_user_tools-23.6.2-156_f44974b-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,67 +1,70 @@
-Zip file size: 158956 bytes, number of entries: 65
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-03 18:44 spark_rapids_pytools/__init__.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jul-03 18:44 spark_rapids_pytools/build.py
--rw-r--r--  2.0 unx     1324 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrapper.py
--rw-r--r--  2.0 unx      646 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/__init__.py
--rw-r--r--  2.0 unx     8507 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/azurestorage.py
--rw-r--r--  2.0 unx    12837 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_aws.py
--rw-r--r--  2.0 unx     1268 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_aws_job.py
--rw-r--r--  2.0 unx    16418 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_azure.py
--rw-r--r--  2.0 unx     2428 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_azure_job.py
--rw-r--r--  2.0 unx    24930 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/dataproc.py
--rw-r--r--  2.0 unx     1426 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/dataproc_job.py
--rw-r--r--  2.0 unx    22142 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/emr.py
--rw-r--r--  2.0 unx    11269 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/emr_job.py
--rw-r--r--  2.0 unx     4939 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/gstorage.py
--rw-r--r--  2.0 unx    13541 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/onprem.py
--rw-r--r--  2.0 unx     4055 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/s3storage.py
--rw-r--r--  2.0 unx    51283 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/sp_types.py
--rw-r--r--  2.0 unx      658 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/__init__.py
--rw-r--r--  2.0 unx      978 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/exceptions.py
--rw-r--r--  2.0 unx     5432 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/prop_manager.py
--rw-r--r--  2.0 unx    14712 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/sys_storage.py
--rw-r--r--  2.0 unx    14006 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/utilities.py
--rw-r--r--  2.0 unx      659 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/__init__.py
--rw-r--r--  2.0 unx     3429 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/databricks_azure_pricing.py
--rw-r--r--  2.0 unx     3522 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/databricks_pricing.py
--rw-r--r--  2.0 unx     4247 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/dataproc_pricing.py
--rw-r--r--  2.0 unx     4717 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/emr_pricing.py
--rw-r--r--  2.0 unx     6400 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/price_provider.py
--rw-r--r--  2.0 unx      666 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/__init__.py
--rw-r--r--  2.0 unx     8830 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/bootstrap.py
--rw-r--r--  2.0 unx     6546 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/diagnostic.py
--rw-r--r--  2.0 unx    13489 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/profiling.py
--rw-r--r--  2.0 unx    43658 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/qualification.py
--rw-r--r--  2.0 unx     6864 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/rapids_job.py
--rw-r--r--  2.0 unx    33590 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/rapids_tool.py
--rw-r--r--  2.0 unx     6576 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/tool_ctxt.py
--rw-r--r--  2.0 unx     1390 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/bootstrap-conf.yaml
--rwxr-xr-x  2.0 unx     4453 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/collect.sh
--rw-r--r--  2.0 unx    30566 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/databricks-premium-catalog.json
--rw-r--r--  2.0 unx    10448 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/databricks_aws-configs.json
--rw-r--r--  2.0 unx    10017 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/databricks_azure-configs.json
--rw-r--r--  2.0 unx     8047 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/dataproc-configs.json
--rw-r--r--  2.0 unx       30 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/diagnostic-conf.yaml
--rw-r--r--  2.0 unx     8994 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/emr-configs.json
--rw-r--r--  2.0 unx     4727 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/onprem-configs.json
--rw-r--r--  2.0 unx    38903 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json
--rw-r--r--  2.0 unx     1460 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/profiling-conf.yaml
--rw-r--r--  2.0 unx     4273 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/qualification-conf.yaml
--rw-r--r--  2.0 unx     2195 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py
--rw-r--r--  2.0 unx      671 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms
--rw-r--r--  2.0 unx      855 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
--rw-r--r--  2.0 unx      537 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms
--rw-r--r--  2.0 unx      630 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/__init__.py
--rw-r--r--  2.0 unx    13207 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
--rw-r--r--  2.0 unx     7985 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py
--rw-r--r--  2.0 unx    16647 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/dataproc_wrapper.py
--rw-r--r--  2.0 unx    18151 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/emr_wrapper.py
--rw-r--r--  2.0 unx     4480 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/onprem_wrapper.py
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2927 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       78 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6768 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/RECORD
-65 files, 577890 bytes uncompressed, 147760 bytes compressed:  74.4%
+Zip file size: 159564 bytes, number of entries: 68
+-rw-r--r--  2.0 unx      750 b- defN 23-Jul-14 02:43 spark_rapids_pytools/__init__.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jul-14 02:43 spark_rapids_pytools/build.py
+-rw-r--r--  2.0 unx     1324 b- defN 23-Jul-14 02:43 spark_rapids_pytools/wrapper.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-14 02:43 spark_rapids_pytools/ascli_cli/__init__.py
+-rw-r--r--  2.0 unx     8270 b- defN 23-Jul-14 02:43 spark_rapids_pytools/ascli_cli/ascli.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/__init__.py
+-rw-r--r--  2.0 unx     8507 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/azurestorage.py
+-rw-r--r--  2.0 unx    12662 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/databricks_aws.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/databricks_aws_job.py
+-rw-r--r--  2.0 unx    16308 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/databricks_azure.py
+-rw-r--r--  2.0 unx     2428 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/databricks_azure_job.py
+-rw-r--r--  2.0 unx    24674 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/dataproc.py
+-rw-r--r--  2.0 unx      922 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/dataproc_job.py
+-rw-r--r--  2.0 unx    21033 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/emr.py
+-rw-r--r--  2.0 unx     1252 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/emr_job.py
+-rw-r--r--  2.0 unx     4939 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/gstorage.py
+-rw-r--r--  2.0 unx    13387 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/onprem.py
+-rw-r--r--  2.0 unx     4055 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/s3storage.py
+-rw-r--r--  2.0 unx    51024 b- defN 23-Jul-14 02:43 spark_rapids_pytools/cloud_api/sp_types.py
+-rw-r--r--  2.0 unx      658 b- defN 23-Jul-14 02:43 spark_rapids_pytools/common/__init__.py
+-rw-r--r--  2.0 unx      978 b- defN 23-Jul-14 02:43 spark_rapids_pytools/common/exceptions.py
+-rw-r--r--  2.0 unx     5432 b- defN 23-Jul-14 02:43 spark_rapids_pytools/common/prop_manager.py
+-rw-r--r--  2.0 unx    14712 b- defN 23-Jul-14 02:43 spark_rapids_pytools/common/sys_storage.py
+-rw-r--r--  2.0 unx    14006 b- defN 23-Jul-14 02:43 spark_rapids_pytools/common/utilities.py
+-rw-r--r--  2.0 unx      659 b- defN 23-Jul-14 02:43 spark_rapids_pytools/pricing/__init__.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-Jul-14 02:43 spark_rapids_pytools/pricing/databricks_azure_pricing.py
+-rw-r--r--  2.0 unx     3522 b- defN 23-Jul-14 02:43 spark_rapids_pytools/pricing/databricks_pricing.py
+-rw-r--r--  2.0 unx     4247 b- defN 23-Jul-14 02:43 spark_rapids_pytools/pricing/dataproc_pricing.py
+-rw-r--r--  2.0 unx     4717 b- defN 23-Jul-14 02:43 spark_rapids_pytools/pricing/emr_pricing.py
+-rw-r--r--  2.0 unx     6400 b- defN 23-Jul-14 02:43 spark_rapids_pytools/pricing/price_provider.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/__init__.py
+-rw-r--r--  2.0 unx     8830 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/bootstrap.py
+-rw-r--r--  2.0 unx     6546 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/diagnostic.py
+-rw-r--r--  2.0 unx    14549 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/profiling.py
+-rw-r--r--  2.0 unx    38670 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/qualification.py
+-rw-r--r--  2.0 unx     5739 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/rapids_job.py
+-rw-r--r--  2.0 unx    33598 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/rapids_tool.py
+-rw-r--r--  2.0 unx     6576 b- defN 23-Jul-14 02:43 spark_rapids_pytools/rapids/tool_ctxt.py
+-rw-r--r--  2.0 unx     1390 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/bootstrap-conf.yaml
+-rwxr-xr-x  2.0 unx     4453 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/collect.sh
+-rw-r--r--  2.0 unx    30566 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/databricks-premium-catalog.json
+-rw-r--r--  2.0 unx    10448 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/databricks_aws-configs.json
+-rw-r--r--  2.0 unx    10017 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/databricks_azure-configs.json
+-rw-r--r--  2.0 unx     8047 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/dataproc-configs.json
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/diagnostic-conf.yaml
+-rw-r--r--  2.0 unx     8994 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/emr-configs.json
+-rw-r--r--  2.0 unx     4727 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/onprem-configs.json
+-rw-r--r--  2.0 unx    38903 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json
+-rw-r--r--  2.0 unx     1524 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/profiling-conf.yaml
+-rw-r--r--  2.0 unx     4273 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/qualification-conf.yaml
+-rw-r--r--  2.0 unx     2195 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py
+-rw-r--r--  2.0 unx      671 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms
+-rw-r--r--  2.0 unx      518 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms
+-rw-r--r--  2.0 unx      855 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
+-rw-r--r--  2.0 unx      537 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms
+-rw-r--r--  2.0 unx      424 b- defN 23-Jul-14 02:43 spark_rapids_pytools/resources/templates/info_recommendations_disabled.ms
+-rw-r--r--  2.0 unx      630 b- defN 23-Jul-14 02:43 spark_rapids_pytools/wrappers/__init__.py
+-rw-r--r--  2.0 unx    13207 b- defN 23-Jul-14 02:43 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
+-rw-r--r--  2.0 unx    12960 b- defN 23-Jul-14 02:43 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py
+-rw-r--r--  2.0 unx    15910 b- defN 23-Jul-14 02:43 spark_rapids_pytools/wrappers/dataproc_wrapper.py
+-rw-r--r--  2.0 unx    12086 b- defN 23-Jul-14 02:43 spark_rapids_pytools/wrappers/emr_wrapper.py
+-rw-r--r--  2.0 unx     9829 b- defN 23-Jul-14 02:43 spark_rapids_pytools/wrappers/onprem_wrapper.py
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jul-14 02:43 spark_rapids_user_tools-23.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2927 b- defN 23-Jul-14 02:43 spark_rapids_user_tools-23.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 02:43 spark_rapids_user_tools-23.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      128 b- defN 23-Jul-14 02:43 spark_rapids_user_tools-23.6.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-14 02:43 spark_rapids_user_tools-23.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7091 b- defN 23-Jul-14 02:43 spark_rapids_user_tools-23.6.2.dist-info/RECORD
+68 files, 573541 bytes uncompressed, 147832 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -3,14 +3,20 @@
 
 Filename: spark_rapids_pytools/build.py
 Comment: 
 
 Filename: spark_rapids_pytools/wrapper.py
 Comment: 
 
+Filename: spark_rapids_pytools/ascli_cli/__init__.py
+Comment: 
+
+Filename: spark_rapids_pytools/ascli_cli/ascli.py
+Comment: 
+
 Filename: spark_rapids_pytools/cloud_api/__init__.py
 Comment: 
 
 Filename: spark_rapids_pytools/cloud_api/azurestorage.py
 Comment: 
 
 Filename: spark_rapids_pytools/cloud_api/databricks_aws.py
@@ -153,14 +159,17 @@
 
 Filename: spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
 Comment: 
 
 Filename: spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms
 Comment: 
 
+Filename: spark_rapids_pytools/resources/templates/info_recommendations_disabled.ms
+Comment: 
+
 Filename: spark_rapids_pytools/wrappers/__init__.py
 Comment: 
 
 Filename: spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
 Comment: 
 
 Filename: spark_rapids_pytools/wrappers/databricks_azure_wrapper.py
@@ -171,26 +180,26 @@
 
 Filename: spark_rapids_pytools/wrappers/emr_wrapper.py
 Comment: 
 
 Filename: spark_rapids_pytools/wrappers/onprem_wrapper.py
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.1.dist-info/LICENSE
+Filename: spark_rapids_user_tools-23.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.1.dist-info/METADATA
+Filename: spark_rapids_user_tools-23.6.2.dist-info/METADATA
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.1.dist-info/WHEEL
+Filename: spark_rapids_user_tools-23.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.1.dist-info/entry_points.txt
+Filename: spark_rapids_user_tools-23.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.1.dist-info/top_level.txt
+Filename: spark_rapids_user_tools-23.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.1.dist-info/RECORD
+Filename: spark_rapids_user_tools-23.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_rapids_pytools/__init__.py

```diff
@@ -12,9 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """init file of the spark_rapids_pytools package."""
 
 from spark_rapids_pytools.build import get_version
 
-VERSION = '23.06.1'
+VERSION = '23.06.2'
 __version__ = get_version(VERSION)
```

## spark_rapids_pytools/cloud_api/databricks_aws.py

```diff
@@ -76,26 +76,20 @@
         databricks_price_provider = DatabricksPriceProvider(region=self.cli.get_region(),
                                                             pricing_configs={'databricks': pricing_config})
         saving_estimator = DBAWSSavingsEstimator(price_provider=databricks_price_provider,
                                                  reshaped_cluster=reshaped_cluster,
                                                  source_cluster=source_cluster)
         return saving_estimator
 
-    def create_submission_job(self, job_prop, ctxt) -> Any:
-        pass
-
     def create_local_submission_job(self, job_prop, ctxt) -> Any:
         return DBAWSLocalRapidsJob(prop_container=job_prop, exec_ctxt=ctxt)
 
     def validate_job_submission_args(self, submission_args: dict) -> dict:
         pass
 
-    def create_spark_submission_job(self, job_prop, ctxt) -> Any:
-        raise NotImplementedError
-
 
 @dataclass
 class DBAWSCMDDriver(CMDDriverBase):
     """Represents the command interface that will be used by DATABRICKS_AWS"""
 
     def _list_inconsistent_configurations(self) -> list:
         incorrect_envs = super()._list_inconsistent_configurations()
```

## spark_rapids_pytools/cloud_api/databricks_azure.py

```diff
@@ -19,15 +19,15 @@
 import os
 from dataclasses import dataclass, field
 from typing import Any, List
 
 from spark_rapids_pytools.cloud_api.azurestorage import AzureStorageDriver
 from spark_rapids_pytools.cloud_api.databricks_azure_job import DBAzureLocalRapidsJob
 from spark_rapids_pytools.cloud_api.sp_types import CloudPlatform, CMDDriverBase, ClusterBase, ClusterNode, \
-    PlatformBase, SysInfo, GpuHWInfo, ClusterState, SparkNodeType, ClusterGetAccessor, NodeHWInfo
+    PlatformBase, SysInfo, GpuHWInfo, ClusterState, SparkNodeType, ClusterGetAccessor, NodeHWInfo, GpuDevice
 from spark_rapids_pytools.common.prop_manager import JSONPropertiesContainer
 from spark_rapids_pytools.common.sys_storage import FSUtil
 from spark_rapids_pytools.common.utilities import Utils
 from spark_rapids_pytools.pricing.databricks_azure_pricing import DatabricksAzurePriceProvider
 from spark_rapids_pytools.pricing.price_provider import SavingsEstimator
 
 
@@ -77,26 +77,20 @@
         db_azure_price_provider = DatabricksAzurePriceProvider(region=self.cli.get_region(),
                                                                pricing_configs={'databricks-azure': pricing_config})
         saving_estimator = DBAzureSavingsEstimator(price_provider=db_azure_price_provider,
                                                    reshaped_cluster=reshaped_cluster,
                                                    source_cluster=source_cluster)
         return saving_estimator
 
-    def create_submission_job(self, job_prop, ctxt) -> Any:
-        pass
-
     def create_local_submission_job(self, job_prop, ctxt) -> Any:
         return DBAzureLocalRapidsJob(prop_container=job_prop, exec_ctxt=ctxt)
 
     def validate_job_submission_args(self, submission_args: dict) -> dict:
         pass
 
-    def create_spark_submission_job(self, job_prop, ctxt) -> Any:
-        raise NotImplementedError
-
     def get_supported_gpus(self) -> dict:
         gpus_from_configs = self.configs.get_value('gpuConfigs', 'user-tools', 'supportedGpuInstances')
         gpu_scopes = {}
         for mc_prof, mc_info in gpus_from_configs.items():
             hw_info_json = mc_info['SysInfo']
             hw_info_ob = SysInfo(num_cpus=hw_info_json['num_cpus'], cpu_mem=hw_info_json['cpu_mem'])
             gpu_info_json = mc_info['GpuInfo']['GPUs'][0]
@@ -217,16 +211,17 @@
     def _pull_gpu_hw_info(self, cli=None) -> GpuHWInfo or None:
         gpu_info = cli.configs.get_value('gpuConfigs', 'user-tools', 'supportedGpuInstances')
         if gpu_info is None:
             return None
         if self.instance_type not in gpu_info:
             return None
         gpu_instance = gpu_info[self.instance_type]['GpuInfo']['GPUs'][0]
+        gpu_device = GpuDevice.fromstring(gpu_instance['Name'])
         return GpuHWInfo(num_gpus=gpu_instance['Count'],
-                         gpu_device=gpu_instance['Name'],
+                         gpu_device=gpu_device,
                          gpu_mem=gpu_instance['MemoryInfo']['SizeInMiB'])
 
 
 @dataclass
 class DatabricksAzureCluster(ClusterBase):
     """
     Represents an instance of running cluster on Databricks.
```

## spark_rapids_pytools/cloud_api/dataproc.py

```diff
@@ -15,15 +15,15 @@
 
 """Implementation specific to Dataproc"""
 
 import json
 from dataclasses import dataclass, field
 from typing import Any, List
 
-from spark_rapids_pytools.cloud_api.dataproc_job import DataprocLocalRapidsJob, DataprocSubmitSparkRapidsJob
+from spark_rapids_pytools.cloud_api.dataproc_job import DataprocLocalRapidsJob
 from spark_rapids_pytools.cloud_api.gstorage import GStorageDriver
 from spark_rapids_pytools.cloud_api.sp_types import PlatformBase, CMDDriverBase, CloudPlatform, \
     ClusterBase, ClusterNode, SysInfo, GpuHWInfo, SparkNodeType, ClusterState, GpuDevice, \
     NodeHWInfo, ClusterGetAccessor
 from spark_rapids_pytools.common.prop_manager import JSONPropertiesContainer
 from spark_rapids_pytools.common.sys_storage import FSUtil
 from spark_rapids_pytools.common.utilities import SysCmd, Utils
@@ -108,23 +108,17 @@
         pricing_provider = DataprocPriceProvider(region=self.cli.get_region(),
                                                  pricing_configs={'gcloud': pricing_config})
         saving_estimator = DataprocSavingsEstimator(price_provider=pricing_provider,
                                                     reshaped_cluster=reshaped_cluster,
                                                     source_cluster=source_cluster)
         return saving_estimator
 
-    def create_submission_job(self, job_prop, ctxt) -> Any:
-        pass
-
     def create_local_submission_job(self, job_prop, ctxt) -> Any:
         return DataprocLocalRapidsJob(prop_container=job_prop, exec_ctxt=ctxt)
 
-    def create_spark_submission_job(self, job_prop, ctxt) -> Any:
-        return DataprocSubmitSparkRapidsJob(prop_container=job_prop, exec_ctxt=ctxt)
-
     def validate_job_submission_args(self, submission_args: dict) -> dict:
         pass
 
     def get_supported_gpus(self) -> dict:
         def calc_num_gpus(gpus_criteria_conf: List[dict], num_cores: int) -> int:
             if gpus_criteria_conf:
                 for c_conf in gpus_criteria_conf:
```

## spark_rapids_pytools/cloud_api/dataproc_job.py

```diff
@@ -12,37 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implementation of Job submissions on GCloud Dataproc"""
 
 from dataclasses import dataclass
 
-from spark_rapids_pytools.rapids.rapids_job import RapidsJob, RapidsLocalJob, RapidsSubmitSparkJob
+from spark_rapids_pytools.rapids.rapids_job import RapidsLocalJob
 
 
 @dataclass
 class DataprocLocalRapidsJob(RapidsLocalJob):
     """
     Implementation of a RAPIDS job that runs on a local machine.
     """
     job_label = 'dataprocLocal'
-
-
-@dataclass
-class DataprocSubmitSparkRapidsJob(RapidsSubmitSparkJob):
-    """
-    Implementation of a RAPIDS job that runs on a remote .
-    """
-    job_label = 'dataprocRemoteSparkJobSubmission'
-
-
-@dataclass
-class DataprocServerlessRapidsJob(RapidsJob):
-    """
-    An implementation that uses Dataproc-Serverless to run RAPIDS accelerator tool.
-    """
-
-    def _build_submission_cmd(self):
-        pass
-
-    def _submit_job(self, cmd_args: list) -> str:
-        pass
```

## spark_rapids_pytools/cloud_api/emr.py

```diff
@@ -15,25 +15,24 @@
 """Implementation specific to EMR"""
 
 import json
 import os
 from dataclasses import field, dataclass
 from typing import Any, List
 
-from spark_rapids_pytools.cloud_api.emr_job import EmrServerlessRapidsJob, EmrLocalRapidsJob
+from spark_rapids_pytools.cloud_api.emr_job import EmrLocalRapidsJob
 from spark_rapids_pytools.cloud_api.s3storage import S3StorageDriver
 from spark_rapids_pytools.cloud_api.sp_types import PlatformBase, ClusterBase, CMDDriverBase, \
     CloudPlatform, ClusterState, SparkNodeType, ClusterNode, GpuHWInfo, SysInfo, GpuDevice, \
     ClusterGetAccessor
 from spark_rapids_pytools.common.prop_manager import JSONPropertiesContainer, \
     AbstractPropertiesContainer
 from spark_rapids_pytools.common.utilities import Utils
 from spark_rapids_pytools.pricing.emr_pricing import EMREc2PriceProvider
 from spark_rapids_pytools.pricing.price_provider import SavingsEstimator
-from spark_rapids_pytools.rapids.rapids_job import RapidsJobPropContainer, RapidsJob
 
 
 @dataclass
 class EMRPlatform(PlatformBase):
     """
     Represents the interface and utilities required by AWS EMR.
     Prerequisites:
@@ -87,23 +86,14 @@
     def validate_job_submission_args(self, submission_args: dict) -> dict:
         """
         process the job submission and return the final arguments to be used for the execution.
         :param submission_args: dictionary containing the job submission arguments
         :return: a dictionary with the processed arguments.
         """
         # TODO: verify that all arguments are valid
-        valid_keys = ['execution-role-arn', 'application-id']
-        for submit_arg in submission_args:
-            if submit_arg not in valid_keys:
-                raise RuntimeError(f'Invalid submission argument [{submit_arg}]. Accepted arguments: {valid_keys}.')
-            if submit_arg == 'application-id' and submission_args.get(submit_arg) is None:
-                # show a message that the appID is not passed
-                self.cli.logger.warning('The EMR-Serverless application-ID is not set. '
-                                        'Note that it is recommended to use a pre-existing SPARK EMR-Serverless '
-                                        'application-id to reduce the overhead of initializing the job.')
         return submission_args
 
     def create_saving_estimator(self,
                                 source_cluster: ClusterGetAccessor,
                                 reshaped_cluster: ClusterGetAccessor):
         raw_pricing_config = self.configs.get_value_silent('pricing')
         if raw_pricing_config:
@@ -113,23 +103,17 @@
         emr_price_provider = EMREc2PriceProvider(region=self.cli.get_region(),
                                                  pricing_configs={'emr': pricing_config})
         saving_estimator = EmrSavingsEstimator(price_provider=emr_price_provider,
                                                reshaped_cluster=reshaped_cluster,
                                                source_cluster=source_cluster)
         return saving_estimator
 
-    def create_submission_job(self, job_prop: RapidsJobPropContainer, ctxt) -> RapidsJob:
-        return EmrServerlessRapidsJob(prop_container=job_prop, exec_ctxt=ctxt)
-
     def create_local_submission_job(self, job_prop, ctxt) -> Any:
         return EmrLocalRapidsJob(prop_container=job_prop, exec_ctxt=ctxt)
 
-    def create_spark_submission_job(self, job_prop, ctxt) -> Any:
-        raise NotImplementedError
-
 
 @dataclass
 class EMRCMDDriver(CMDDriverBase):
     """Represents the command interface that will be used by EMR"""
 
     def _list_inconsistent_configurations(self) -> list:
         incorrect_envs = super()._list_inconsistent_configurations()
```

## spark_rapids_pytools/cloud_api/emr_job.py

```diff
@@ -10,270 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implementation of Job submissions on EMR"""
 
-import json
-import time
-from dataclasses import field, dataclass
-from logging import Logger
-
-from spark_rapids_pytools.cloud_api.sp_types import EnumeratedType
-from spark_rapids_pytools.common.prop_manager import JSONPropertiesContainer
-from spark_rapids_pytools.common.utilities import ToolLogging, Utils
-from spark_rapids_pytools.rapids.rapids_job import RapidsJob, RapidsLocalJob
-from spark_rapids_pytools.rapids.tool_ctxt import ToolContext
-
-
-class EMRJobState(EnumeratedType):
-    """
-    Standard states for an EMR job.
-    """
-    SUBMITTED = 'submitted'
-    PENDING = 'Pending'
-    SCHEDULED = 'Scheduled'
-    RUNNING = 'Running'
-    FAILED = 'Failed'
-    SUCCESS = 'Success'
-    CANCELLING = 'Cancelling'
-    CANCELLED = 'Cancelled'
-    UNKNOWN = 'Unknown'
-
-
-class EMRAppState(EnumeratedType):
-    """
-    Standard states for a EMR application.
-    Creating 	The application is being prepared and isn't ready to use yet.
-    Created 	The application has been created but hasn't provisioned capacity yet.
-                 You can modify the application to change its initial capacity configuration.
-    Starting 	The application is starting and is provisioning capacity.
-    Started 	The application is ready to accept new jobs. The application only accepts jobs when
-                it's in this state.
-    Stopping 	All jobs have completed and the application is releasing its capacity.
-    Stopped 	The application is stopped and no resources are running on the application.
-                You can modify the application to change its initial capacity configuration.
-    Terminated 	The application has been terminated and doesn't appear on your application list.
-    """
-    CREATING = 'Creating'
-    CREATED = 'Created'
-    STARTING = 'Starting'
-    STARTED = 'Started'
-    STOPPING = 'Stopping'
-    STOPPED = 'Stopped'
-    TERMINATED = 'Terminated'
-
-
-class EMRAppType(EnumeratedType):
-    """
-    Standard types for EMR application types.
-    """
-    SPARK = 'SPARK'
-
-
-@dataclass
-class EMRServerlessApplication:
-    """
-    A wrapper that encapsulates an EMR-serverless application created to host the submitted
-    RAPIDS tool job through EMR-serverless.
-    """
-    app_name: None
-    id: str = None
-    exec_ctxt: ToolContext = None
-    app_type: EMRAppType = EMRAppType.SPARK
-    state: EMRAppState = field(default_factory=dict, init=False)
-    details: JSONPropertiesContainer = field(default=None, init=False)
-    outlive_submission: bool = field(default=False, init=False)
-    logger: Logger = field(default=None, init=False)
-
-    def __post_init__(self):
-        # when debug is set to true set it in the environment.
-        self.logger = ToolLogging.get_and_setup_logger('rapids.tools.submit.app')
-        if self.id is not None:
-            self.outlive_submission = True
-            self._update_status()
-        else:
-            # if name is none auto generate a new one:
-            if self.app_name is None:
-                self.app_name = f'rapids-tools-{Utils.gen_random_string(8)}'
-            self.outlive_submission = False
-            self._create_as_new()
-
-    def _update_status(self):
-        cmd_args = [
-            'aws',
-            'emr-serverless',
-            'get-application',
-            '--application-id',
-            self.id
-        ]
-        std_out = self.exec_ctxt.platform.cli.run_sys_cmd(cmd_args)
-        self.details = JSONPropertiesContainer(prop_arg=std_out, file_load=False)
-        self.state = EMRAppState.fromstring(self.details.get_value('application', 'state'))
-        self.app_name = self.details.get_value('application', 'name')
-
-    def _create_as_new(self):
-        cmd_args = [
-            'aws',
-            'emr-serverless',
-            'create-application',
-            '--release-label',
-            'emr-6.9.0',
-            '--type',
-            f'\"{EMRAppType.tostring(self.app_type)}\"',
-            '--name',
-            self.app_name
-        ]
-        self.logger.info('Creating new EMR-serverless application')
-        std_out = self.exec_ctxt.platform.cli.run_sys_cmd(cmd_args)
-        json_value = json.loads(std_out)
-        self.id = json_value['applicationId']
-        self._update_status()
-        return self
-
-    def _wait_for_states(self, *states):
-        self.logger.debug('Waiting for application to reach state: %s', states)
-        while self.state not in states:
-            time.sleep(5)
-            self._update_status()
-        self.logger.debug('Done waiting for application to reach state: %s', states)
-
-    def app_is_terminated(self):
-        return self.state in [EMRAppState.TERMINATED, EMRAppState.STOPPED]
-
-    def wait_for_app_ready(self):
-        if self.app_is_terminated():
-            raise RuntimeError(f'EMR Application {self.id} is not active. '
-                               f'Current state is {self.state}.')
-        self._wait_for_states(EMRAppState.STARTED, EMRAppState.STARTING, EMRAppState.CREATED)
-
-    def stop_app(self):
-        self.logger.info('Start stopping application %s. Current state %s', self.id, self.state)
-        if self.state not in [EMRAppState.STOPPING, EMRAppState.STOPPED, EMRAppState.TERMINATED]:
-            cmd_args = [
-                'aws', 'emr-serverless', 'stop-application', '--application-id', self.id
-            ]
-            std_out = self.exec_ctxt.platform.cli.run_sys_cmd(cmd_args)
-            self.logger.info('Application %s has stopped: %s', self.id, std_out)
-        else:
-            self.logger.info('Application %s. was already stopped %s', self.id, self.state)
-        self._wait_for_states(EMRAppState.TERMINATED, EMRAppState.STOPPED)
-
-    def delete_app(self):
-        # stop app first
-        self.stop_app()
-        # now delete teh app
-        cmd_args = [
-            'aws', 'emr-serverless', 'delete-application', '--application-id', self.id
-        ]
-        std_out = self.exec_ctxt.platform.cli.run_sys_cmd(cmd_args)
-        self.logger.info('the emr-serverless application was deleted. %s', std_out)
-
-    def terminate_app(self):
-        if self.outlive_submission:
-            self.logger.info('Skipping termination of Emr-serverless app %s. The app outlives the '
-                             'execution.',
-                             self.id)
-        else:
-            self.logger.info('Deleting the temporary app %s with current state %s', self.id, self.state)
-            self.delete_app()
-
-
-@dataclass
-class EmrServerlessRapidsJob(RapidsJob):
-    """
-    An implementation that uses EMR-Serverless to run RAPIDS accelerator tool.
-    """
-    job_label = 'emrServerless'
-    job_state: EMRJobState = field(default=None, init=False)
-    emr_app: EMRServerlessApplication = field(default=None, init=False)
-
-    def is_finished(self):
-        if self.job_state is None:
-            return False
-        return self.job_state in [EMRJobState.FAILED, EMRJobState.SUCCESS, EMRJobState.CANCELLED]
-
-    def _init_fields(self):
-        super()._init_fields()
-        app_id = self.prop_container.get_value_silent('platformArgs', 'application-id')
-        self.emr_app = EMRServerlessApplication(id=app_id,
-                                                app_name=self.__generate_app_name(),
-                                                exec_ctxt=self.exec_ctxt)
-        self.emr_app.wait_for_app_ready()
-
-    def __generate_app_name(self) -> str:
-        return self.exec_ctxt.get_ctxt('execFullName')
-
-    def __get_role_arn(self):
-        return self.prop_container.get_value('platformArgs', 'execution-role-arn')
-
-    def __generate_job_name(self):
-        # use the same name as the output folder
-        return f'{self.emr_app.app_name}-{Utils.gen_random_string(4)}'
-
-    def __build_driver(self) -> str:
-        spark_job_configs = self.prop_container.get_value('sparkConfArgs', 'properties')
-        spark_params = ['--class', self.prop_container.get_jar_main_class()]
-        for conf_k, conf_val in spark_job_configs.items():
-            conf_arg = ['--conf', f'{conf_k}={conf_val}']
-            spark_params.extend(conf_arg)
-        submit_params = {
-            'entryPoint': self.prop_container.get_jar_file(),
-            'entryPointArguments': self._build_rapids_args(),
-            'sparkSubmitParameters': Utils.gen_joined_str(' ', spark_params)
-        }
-        res = {
-            'sparkSubmit': submit_params
-        }
-        return json.dumps(res)
-
-    def _build_submission_cmd(self):
-        cmd_args = ['aws',
-                    'emr-serverless',
-                    'start-job-run']
-        # add application_id
-        cmd_args.extend(['--application-id', self.emr_app.id])
-        # add job_role_arn
-        cmd_args.extend(['--execution-role-arn', self.__get_role_arn()])
-        # add job_name
-        cmd_args.extend(['--name', self.__generate_job_name()])
-        # add job_driver
-        cmd_args.extend(['--job-driver', f"\'{self.__build_driver()}\'"])
-        return cmd_args
-
-    def __get_job_details(self, job_id: str, app_id: str) -> dict:
-        cmd_args = [
-            'aws',
-            'emr-serverless',
-            'get-job-run',
-            '--application-id',
-            app_id,
-            '--job-run-id',
-            job_id]
-        std_out = self.exec_ctxt.platform.cli.run_sys_cmd(cmd_args)
-        return json.loads(std_out)
-
-    def _submit_job(self, cmd_args: list) -> str:
-        std_out = self.exec_ctxt.platform.cli.run_sys_cmd(cmd_args)
-        self.logger.debug('Output of job submission is %s', std_out)
-        # get the job_id
-        json_out = json.loads(std_out)
-        job_id = json_out['jobRunId']
-        self.logger.info('Submitted JOB ID is %s', job_id)
-        # wait while the job is still running
-        while not self.is_finished():
-            time.sleep(10)
-            job_details = self.__get_job_details(job_id, self.emr_app.id)
-            self.job_state = EMRJobState.fromstring(job_details['jobRun']['state'])
-            self.logger.info('Job state: %s', self.job_state)
-        self.logger.info('Done waiting for the job to finish.')
-        # Cleanup the emr application if necessary
-        self.emr_app.terminate_app()
-        return std_out
+from dataclasses import dataclass
+from spark_rapids_pytools.rapids.rapids_job import RapidsLocalJob
 
 
 @dataclass
 class EmrLocalRapidsJob(RapidsLocalJob):
     """
     Implementation of a RAPIDS job that runs local on a local machine.
     """
```

## spark_rapids_pytools/cloud_api/onprem.py

```diff
@@ -77,17 +77,14 @@
         else:
             self_id = self.type_id
         return CloudPlatform.pretty_print(self_id)
 
     def get_footer_message(self) -> str:
         return 'To support acceleration with T4 GPUs, please use these worker node instance types.'
 
-    def create_submission_job(self, job_prop, ctxt) -> Any:
-        pass
-
     def create_saving_estimator(self,
                                 source_cluster: ClusterGetAccessor,
                                 reshaped_cluster: ClusterGetAccessor):
         if self.platform == 'dataproc':
             region = 'us-central1'
             raw_pricing_config = self.configs.get_value_silent('csp_pricing')
             if raw_pricing_config:
@@ -98,17 +95,14 @@
             pricing_provider = DataprocPriceProvider(region=region,
                                                      pricing_configs={'gcloud': pricing_config})
             saving_estimator = OnpremSavingsEstimator(price_provider=pricing_provider,
                                                       reshaped_cluster=reshaped_cluster,
                                                       source_cluster=source_cluster)
         return saving_estimator
 
-    def create_spark_submission_job(self, job_prop, ctxt) -> Any:
-        pass
-
     def set_offline_cluster(self, cluster_args: dict = None):
         pass
 
     def validate_job_submission_args(self, submission_args: dict) -> dict:
         pass
 
     def get_supported_gpus(self) -> dict:
```

## spark_rapids_pytools/cloud_api/sp_types.py

```diff
@@ -60,23 +60,21 @@
         """
         value = cast(Enum, value)
         return str(value._value_)  # pylint: disable=protected-access
 
 
 class DeployMode(EnumeratedType):
     """List of tools deployment methods"""
-    # The rapids job runs by submitting a spinning serverless job
-    SERVERLESS = 'serverless'
     # The rapids job is running on local node
     LOCAL = 'local'
     # The rapids job is submitted on a remote cluster
     REMOTE_CLUSTER = 'remote'
 
     def requires_remote_storage(self) -> bool:
-        return self.value in [self.SERVERLESS, self.REMOTE_CLUSTER]
+        return self.value in [self.REMOTE_CLUSTER]
 
 
 class GpuDevice(EnumeratedType):
     """List of supported GPU devices"""
     T4 = 't4'
     V100 = 'v100'
     K80 = 'k80'
@@ -121,17 +119,20 @@
 class CloudPlatform(EnumeratedType):
     """symbolic names (members) bound to supported cloud platforms."""
     DATABRICKS_AWS = 'databricks_aws'
     DATABRICKS_AZURE = 'databricks_azure'
     DATAPROC = 'dataproc'
     EMR = 'emr'
     ONPREM = 'onprem'
-    LOCAL = 'local'
     NONE = 'NONE'
 
+    @classmethod
+    def get_default(cls):
+        return cls.ONPREM
+
 
 class TargetPlatform(EnumeratedType):
     """Determine CostSavings for target platform based on OnPrem cluster configuration"""
     DATAPROC = 'dataproc'
     NONE = None
 
 
@@ -846,23 +847,17 @@
         raise NotImplementedError
 
     def create_saving_estimator(self,
                                 source_cluster: ClusterGetAccessor,
                                 reshaped_cluster: ClusterGetAccessor):
         raise NotImplementedError
 
-    def create_submission_job(self, job_prop, ctxt) -> Any:
-        raise NotImplementedError
-
     def create_local_submission_job(self, job_prop, ctxt) -> Any:
         raise NotImplementedError
 
-    def create_spark_submission_job(self, job_prop, ctxt) -> Any:
-        raise NotImplementedError
-
     def load_platform_configs(self):
         config_file_name = f'{CloudPlatform.tostring(self.type_id).lower()}-configs.json'
         config_path = Utils.resource_path(config_file_name)
         self.configs = JSONPropertiesContainer(prop_arg=config_path)
 
     def get_supported_gpus(self) -> dict:
         gpus_from_configs = self.configs.get_value('gpuConfigs', 'user-tools', 'supportedGpuInstances')
```

## spark_rapids_pytools/rapids/profiling.py

```diff
@@ -21,15 +21,15 @@
 from typing import List
 
 import yaml
 from tabulate import tabulate
 
 from spark_rapids_pytools.cloud_api.sp_types import ClusterBase
 from spark_rapids_pytools.common.sys_storage import FSUtil
-from spark_rapids_pytools.common.utilities import Utils
+from spark_rapids_pytools.common.utilities import Utils, TemplateGenerator
 from spark_rapids_pytools.rapids.rapids_tool import RapidsJarTool
 
 
 @dataclass
 class Profiling(RapidsJarTool):
     """
     Wrapper layer around Profiling Tool.
@@ -62,32 +62,35 @@
             self._process_offline_cluster_args()
         else:
             self.logger.info('Skipping building of GPU_CLUSTER because WorkerInfo is defined')
         self._process_eventlogs_args()
 
     def _process_offline_cluster_args(self):
         offline_cluster_opts = self.wrapper_options.get('migrationClustersProps', {})
-        self._process_gpu_cluster_args(offline_cluster_opts)
-        self._generate_autotuner_input()
+        if self._process_gpu_cluster_args(offline_cluster_opts):
+            # only if we succeed to get the GPU cluster, we can generate auto-tuner-input
+            self._generate_autotuner_input()
+
+    def __load_disabled_recommendation_report(self) -> str:
+        template_file_name = self.ctxt.get_value('toolOutput', 'recommendations', 'disabledInfoMsgTemplate')
+        template_path = Utils.resource_path(f'templates/{template_file_name}')
+        return TemplateGenerator.render_template_file(template_path, {'CLUSTER_ARG': 'cluster'})
 
     def _process_gpu_cluster_args(self, offline_cluster_opts: dict = None):
         gpu_cluster_arg = offline_cluster_opts.get('gpuCluster')
         if gpu_cluster_arg:
             gpu_cluster_obj = self._create_migration_cluster('GPU', gpu_cluster_arg)
             self.ctxt.set_ctxt('gpuClusterProxy', gpu_cluster_obj)
-        else:
-            # If we are here, we know that the workerInfoPath was not set as well.
-            # Then we should fail
-            self.logger.error('The gpuCluster argument was not set. '
-                              'Please make sure to set the arguments properly by either:\n'
-                              '  1. Setting <gpu_cluster> argument and optional set <eventlogs> if '
-                              'the path is not defined by the cluster properties ; or\n'
-                              '  2. Setting both <worker_info> and <eventlogs>')
-            raise RuntimeError('Invalid Arguments: The <gpu_cluster> and <worker_info> arguments are '
-                               'not defined. Aborting Execution.')
+            return True
+        # If we are here, we know that the workerInfoPath was not set as well.
+        # Then we can remind the user that recommendations won't be calculated
+        disabled_recommendations_msg = self.__load_disabled_recommendation_report()
+        self.ctxt.set_ctxt('disabledRecommendationsMsg', disabled_recommendations_msg)
+        self.logger.info(disabled_recommendations_msg)
+        return False
 
     def _generate_autotuner_file_for_cluster(self, file_path: str, cluster_ob: ClusterBase):
         """
         Given file path and the cluster object, it will generate the formatted input file in yaml
         that can be used by the autotuner to run the profiling tool.
         :param file_path: local path whether the file should be stored
         :param cluster_ob: the object representing the cluster proxy.
@@ -128,19 +131,19 @@
         autotuner_input_path = FSUtil.build_path(self.ctxt.get_local_work_dir(), 'worker_info.yaml')
         self._generate_autotuner_file_for_cluster(file_path=autotuner_input_path,
                                                   cluster_ob=gpu_cluster_obj)
         self.logger.info('Generated autotuner worker info: %s', autotuner_input_path)
         self.ctxt.set_ctxt('autoTunerFilePath', autotuner_input_path)
 
     def _create_autotuner_rapids_args(self) -> list:
-        # add the autotuner argument
-        autotuner_args = ['--auto-tuner',
-                          '--worker-info',
-                          self.ctxt.get_ctxt('autoTunerFilePath')]
-        return autotuner_args
+        # Add the autotuner argument if the autotunerPath exists
+        autotuner_path = self.ctxt.get_ctxt('autoTunerFilePath')
+        if autotuner_path is None:
+            return []
+        return ['--auto-tuner', '--worker-info', autotuner_path]
 
     def __read_single_app_output(self, file_path: str) -> (str, List[str], List[str]):
         def split_list_str_by_pattern(input_seq: List[str], pattern: str) -> int:
             ind = 0
             while ind < len(input_seq):
                 if input_seq[ind].find(pattern) != -1:
                     return ind
@@ -202,17 +205,23 @@
         props_list.sort()
         return app_name, props_list, comments_list
 
     def _write_summary(self):
         print(Utils.gen_multiline_str(self._report_tool_full_location(),
                                       self.ctxt.get_ctxt('wrapperOutputContent')))
 
-    def _process_output(self):
-        if not self._evaluate_rapids_jar_tool_output_exist():
-            return
+    def __generate_report_no_recommendations(self):
+        prof_app_dirs = FSUtil.get_subdirectories(self.ctxt.get_rapids_output_folder())
+        wrapper_content = [Utils.gen_report_sec_header('Recommendations'),
+                           self.ctxt.get_ctxt('disabledRecommendationsMsg'),
+                           Utils.gen_report_sec_header('Profiling status'),
+                           f'Total application profiled: {len(prof_app_dirs)}']
+        self.ctxt.set_ctxt('wrapperOutputContent', wrapper_content)
+
+    def __generate_report_with_recommendations(self):
         prof_app_dirs = FSUtil.get_subdirectories(self.ctxt.get_rapids_output_folder())
         profiling_log = self.ctxt.get_value('toolOutput', 'recommendations', 'fileName')
         recommendations_table = []
         log_lines = []
 
         header_str = '### Recommended configurations ###'
         sec_props_head = ['\tSpark Properties:']
@@ -244,14 +253,25 @@
         # wrapper STDOUT report contains both tabular and plain text format of recommendations
         wrapper_content = [Utils.gen_report_sec_header('Recommendations'),
                            log_file_lines_str,
                            '### Recommendations Table Summary ###',
                            tabulate(recommendations_table, headers, tablefmt='grid')]
         self.ctxt.set_ctxt('wrapperOutputContent', wrapper_content)
 
+    def _process_output(self):
+        if not self._evaluate_rapids_jar_tool_output_exist():
+            return
+
+        if self.ctxt.get_ctxt('autoTunerFilePath'):
+            # if autotuner is enabled, generate full recommendations summary
+            self.__generate_report_with_recommendations()
+        else:
+            # generate a brief summary
+            self.__generate_report_no_recommendations()
+
     def _init_rapids_arg_list(self) -> List[str]:
         return self._create_autotuner_rapids_args()
 
 
 @dataclass
 class ProfilingAsLocal(Profiling):
     """
```

## spark_rapids_pytools/rapids/qualification.py

```diff
@@ -18,19 +18,18 @@
 from dataclasses import dataclass, field
 from math import ceil
 from typing import Any, List, Callable
 
 import pandas as pd
 from tabulate import tabulate
 
-from spark_rapids_pytools.cloud_api.sp_types import EnumeratedType, ClusterReshape, DeployMode
+from spark_rapids_pytools.cloud_api.sp_types import EnumeratedType, ClusterReshape
 from spark_rapids_pytools.common.sys_storage import FSUtil
 from spark_rapids_pytools.common.utilities import Utils, TemplateGenerator
 from spark_rapids_pytools.pricing.price_provider import SavingsEstimator
-from spark_rapids_pytools.rapids.rapids_job import RapidsJobPropContainer
 from spark_rapids_pytools.rapids.rapids_tool import RapidsJarTool
 
 
 class QualFilterApp(EnumeratedType):
     """Values used to filter out the applications in the qualification report"""
     SAVINGS = 'savings'
     SPEEDUPS = 'speedups'
@@ -204,24 +203,25 @@
     def _process_cpu_cluster_args(self, offline_cluster_opts: dict = None):
         # get the name of the cpu_cluster
         cpu_cluster_arg = offline_cluster_opts.get('cpuCluster')
         if cpu_cluster_arg is not None:
             cpu_cluster_obj = self._create_migration_cluster('CPU', cpu_cluster_arg)
             self.ctxt.set_ctxt('cpuClusterProxy', cpu_cluster_obj)
 
-    def _process_gpu_cluster_args(self, offline_cluster_opts: dict = None):
+    def _process_gpu_cluster_args(self, offline_cluster_opts: dict = None) -> bool:
         gpu_cluster_arg = offline_cluster_opts.get('gpuCluster')
         if gpu_cluster_arg is None:
             self.logger.info('Creating GPU cluster by converting the CPU cluster instances to GPU supported types')
             # Convert the CPU instances to support gpu
             orig_cluster = self.ctxt.get_ctxt('cpuClusterProxy')
             gpu_cluster_obj = self.ctxt.platform.migrate_cluster_to_gpu(orig_cluster)
         else:
             gpu_cluster_obj = self._create_migration_cluster('GPU', gpu_cluster_arg)
         self.ctxt.set_ctxt('gpuClusterProxy', gpu_cluster_obj)
+        return True
 
     def _process_offline_cluster_args(self):
         offline_cluster_opts = self.wrapper_options.get('migrationClustersProps', {})
         self._process_cpu_cluster_args(offline_cluster_opts)
         self._process_gpu_cluster_args(offline_cluster_opts)
 
     def __process_gpu_cluster_recommendation(self, arg_val: str):
@@ -299,85 +299,14 @@
         self.__process_filter_args(self.wrapper_options.get('filterApps'))
 
         self._process_offline_cluster_args()
         self._process_eventlogs_args()
         # This is noise to dump everything
         # self.logger.debug('%s custom arguments = %s', self.pretty_name(), self.ctxt.props['wrapperCtx'])
 
-    def _process_job_submission_args(self):
-        job_args = {}
-        submission_args = self.wrapper_options.get('jobSubmissionProps')
-        # get the root remote folder and make sure it exists
-        job_args.update(self._set_remote_folder_for_submission(self.requires_remote_folder()))
-        platform_args = submission_args.get('platformArgs')
-        if platform_args is not None:
-            processed_platform_args = self.ctxt.platform.validate_job_submission_args(platform_args)
-            job_args['platformArgs'] = processed_platform_args
-        self.ctxt.update_job_args(job_args)
-
-    def _copy_dependencies_to_remote(self):
-        self.logger.info('Preparing remote dependency folder')
-        remote_work_dir = self.ctxt.get_remote('workDir')
-        local_folder = self.ctxt.get_local('outputFolder')
-        cp_res = self.ctxt.platform.storage.upload_resource(local_folder, remote_work_dir)
-        self.logger.debug('Executed command of copying %s', cp_res)
-
-    def _prepare_job_arguments(self):
-        job_args = self.ctxt.get_ctxt('jobArgs')
-        remote_folder = job_args.get('outputDirectory')
-        if remote_folder is None:
-            # for dataproc we can get the tmp gs storage
-            self.logger.info('The remote directory to archive the job results is not set')
-        else:
-            # check the remote_folder exists
-            if not self.ctxt.platform.storage.resource_exists(remote_folder):
-                raise RuntimeError(f'Remote folder [{remote_folder}] does not exist.')
-        # now we can create the job object
-        # Todo: For dataproc, this can be autogenerated from cluster name
-        rapids_arg_list = self._init_rapids_arg_list()
-        ctxt_rapids_args = self.ctxt.get_ctxt('rapidsArgs')
-        jar_file_name = ctxt_rapids_args.get('jarFileName')
-        rapids_opts = ctxt_rapids_args.get('rapidsOpts')
-        if rapids_opts is not None:
-            rapids_arg_list.extend(rapids_opts)
-        # add the eventlogs at the end of all the tool options
-        rapids_arg_list.extend(self.ctxt.get_ctxt('eventLogs'))
-        class_name = self.ctxt.get_value('sparkRapids', 'mainClass')
-        remote_jar = FSUtil.build_url_from_parts(self.ctxt.get_remote('depFolder'), jar_file_name)
-        rapids_arg_obj = {
-            'jarFile': remote_jar,
-            'jarArgs': rapids_arg_list,
-            'className': class_name
-        }
-        # EMR specific things
-        platform_args = job_args.get('platformArgs')
-        spark_conf_args = {
-            'properties': {
-                'spark.executor.cores': '4',
-                'spark.executor.memory': '20g',
-                'spark.driver.cores': '4',
-                'spark.driver.memory': '8g',
-                'spark.executor.instances': '1'
-            }
-        }
-        job_properties_json = {
-            'outputDirectory': remote_folder,
-            'rapidsArgs': rapids_arg_obj,
-            'sparkConfArgs': spark_conf_args,
-            'platformArgs': platform_args
-        }
-        job_properties = RapidsJobPropContainer(prop_arg=job_properties_json,
-                                                file_load=False)
-        if self.ctxt.get_deploy_mode() == DeployMode.REMOTE_CLUSTER:
-            job_obj = self.ctxt.platform.create_spark_submission_job(job_prop=job_properties,
-                                                                     ctxt=self.ctxt)
-        else:
-            job_obj = self.ctxt.platform.create_submission_job(job_prop=job_properties, ctxt=self.ctxt)
-        job_obj.run_job()
-
     def __get_recommended_apps(self, all_rows, selected_cols=None) -> pd.DataFrame:
         speed_up_col = self.ctxt.get_value('toolOutput', 'csv', 'summaryReport',
                                            'recommendations', 'speedUp', 'columnName')
         recommended_vals = self.ctxt.get_value('toolOutput', 'csv', 'summaryReport',
                                                'recommendations', 'speedUp', 'selectedRecommendations')
         mask = all_rows[speed_up_col].isin(recommended_vals)
         if selected_cols is None:
@@ -737,28 +666,14 @@
         self.ctxt.set_ctxt('wrapperOutputContent', summary_report)
 
     def _write_summary(self):
         wrapper_out_content = self.ctxt.get_ctxt('wrapperOutputContent')
         if wrapper_out_content is not None:
             print(Utils.gen_multiline_str(wrapper_out_content))
 
-    def _archive_results(self):
-        archive_enabled = self.ctxt.get_ctxt('archiveToRemote')
-        if archive_enabled:
-            # we should only archive when the remote_folder is being set
-            remote_work_dir = self.ctxt.get_remote('workDir')
-            if remote_work_dir and self._rapids_jar_tool_has_output():
-                local_folder = self.ctxt.get_output_folder()
-                # TODO make sure it worth issuing the command
-                rapids_subfolder = self.ctxt.get_value_silent('toolOutput', 'subFolder')
-                exclude_folder = rapids_subfolder
-                self.ctxt.platform.storage.upload_resource(local_folder,
-                                                           remote_work_dir,
-                                                           exclude_pattern=exclude_folder)
-
     def _init_rapids_arg_list(self) -> List[str]:
         # TODO: Make sure we add this argument only for jar versions 23.02+
         return ['--platform', self.ctxt.platform.get_platform_name().replace('_', '-')]
 
     def _generate_section_lines(self, sec_conf: dict) -> List[str]:
         if sec_conf.get('sectionID') == 'initializationScript':
             # format the initialization scripts
@@ -790,27 +705,14 @@
             script_content = gpu_cluster.generate_bootstrap_script(overridden_args=override_args)
             highlighted_code = TemplateGenerator.highlight_bash_code(script_content)
             return ['```bash', highlighted_code, '```', '']
         return super()._generate_section_content(sec_conf)
 
 
 @dataclass
-class QualificationAsRemote(Qualification):
-    """
-    Qualification tool running on Remote cluster development.
-    """
-    description: str = 'This is the Remote Spark Qualification implementation'
-
-    def _handle_non_running_exec_cluster(self, err_msg: str) -> None:
-        # For remote cluster mode, the execution cluster must be running
-        raise RuntimeError(f'Exception verifying remote cluster: {err_msg}. \n\t'
-                           'Make sure the execution cluster passed to the CLI is currently active')
-
-
-@dataclass
 class QualificationAsLocal(Qualification):
     """
     Qualification tool running on local development.
     """
     description: str = 'This is the localQualification'
 
     def _copy_dependencies_to_remote(self):
```

## spark_rapids_pytools/rapids/rapids_job.py

```diff
@@ -14,15 +14,14 @@
 
 """Abstract representation of a wrapper Job"""
 
 from dataclasses import dataclass, field
 from logging import Logger
 from typing import List
 
-from spark_rapids_pytools.cloud_api.sp_types import ClusterGetAccessor
 from spark_rapids_pytools.common.prop_manager import JSONPropertiesContainer
 from spark_rapids_pytools.common.utilities import ToolLogging, Utils
 from spark_rapids_pytools.rapids.tool_ctxt import ToolContext
 
 
 @dataclass
 class RapidsJobPropContainer(JSONPropertiesContainer):
@@ -148,33 +147,7 @@
         return cmd_arg
 
     def _submit_job(self, cmd_args: list) -> str:
         env_args = self.prop_container.get_value_silent('platformArgs', 'envArgs')
         out_std = self.exec_ctxt.platform.cli.run_sys_cmd(cmd=cmd_args,
                                                           env_vars=env_args)
         return out_std
-
-
-@dataclass
-class RapidsSubmitSparkJob(RapidsJob):
-    """
-    Class to submit a spark job to remote Cluster
-    """
-
-    def _submit_job(self, cmd_args: list) -> str:
-        env_args = self.prop_container.get_value_silent('platformArgs', 'envArgs')
-        out_std = self.exec_ctxt.platform.cli.run_sys_cmd(cmd=cmd_args,
-                                                          env_vars=env_args)
-        return out_std
-
-    def _build_submission_cmd(self) -> List[str]:
-        submit_args = {
-            'jarArgs': self._build_rapids_args(),
-            'platformSparkJobArgs': {
-                'jars': self.prop_container.get_jar_file(),
-                'class': self.prop_container.get_jar_main_class()
-            },
-        }
-        exec_cluster: ClusterGetAccessor = self.exec_ctxt.get_ctxt('execCluster')
-        cluster_name = exec_cluster.get_name()
-        return self.exec_ctxt.platform.cli.get_submit_spark_job_cmd_for_cluster(cluster_name,
-                                                                                submit_args)
```

## spark_rapids_pytools/rapids/rapids_tool.py

```diff
@@ -503,15 +503,15 @@
         self._process_jar_arg()
         self._process_dependencies()
         self._process_tool_args()
 
     def _process_offline_cluster_args(self):
         pass
 
-    def _process_gpu_cluster_args(self, offline_cluster_opts: dict = None):
+    def _process_gpu_cluster_args(self, offline_cluster_opts: dict = None) -> bool:
         pass
 
     def _copy_dependencies_to_remote(self):
         self.logger.info('Skipping preparing remote dependency folder')
 
     def _prepare_job_arguments(self):
         self._prepare_local_job_arguments()
```

## spark_rapids_pytools/resources/profiling-conf.yaml

```diff
@@ -1,11 +1,12 @@
 toolOutput:
   subFolder: rapids_4_spark_profile
   recommendations:
     fileName: profile.log
+    disabledInfoMsgTemplate: 'info_recommendations_disabled.ms'
     headers:
       section: '### D. Recommended Configuration ###'
       sparkProperties: 'Spark Properties:'
       comments: 'Comments:'
 sparkRapids:
   mvnUrl: 'https://repo1.maven.org/maven2/com/nvidia/rapids-4-spark-tools_2.12'
   repoUrl: '{}/{}/rapids-4-spark-tools_2.12-{}.jar'
```

## spark_rapids_pytools/wrappers/databricks_azure_wrapper.py

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 
 """Wrapper class to run tools associated with RAPIDS Accelerator for Apache Spark plugin on DATABRICKS_AZURE."""
 
 from spark_rapids_pytools.cloud_api.sp_types import DeployMode, CloudPlatform
 from spark_rapids_pytools.common.utilities import ToolLogging
+from spark_rapids_pytools.rapids.profiling import ProfilingAsLocal
 from spark_rapids_pytools.rapids.qualification import QualFilterApp, QualificationAsLocal, QualGpuClusterReshapeType
 
 
 class CliDBAzureLocalMode:  # pylint: disable=too-few-public-methods
     """
     A wrapper that runs the RAPIDS Accelerator tools locally on the dev machine for DATABRICKS_AZURE.
     """
@@ -119,15 +120,93 @@
         }
         QualificationAsLocal(platform_type=CloudPlatform.DATABRICKS_AZURE,
                              cluster=None,
                              output_folder=local_folder,
                              wrapper_options=wrapper_qual_options,
                              rapids_options=rapids_options).launch()
 
+    @staticmethod
+    def profiling(gpu_cluster: str = None,
+                  worker_info: str = None,
+                  eventlogs: str = None,
+                  profile: str = None,
+                  local_folder: str = None,
+                  remote_folder: str = None,
+                  tools_jar: str = None,
+                  credentials_file: str = None,
+                  jvm_heap_size: int = 24,
+                  verbose: bool = False,
+                  **rapids_options) -> None:
+        """
+        The Profiling tool analyzes both CPU or GPU generated event logs and generates information
+        which can be used for debugging and profiling Apache Spark applications.
+        :param  gpu_cluster: The Databricks-cluster on which the Spark applications were executed. The argument
+                can be a Databricks-cluster or a valid path to the cluster's properties file (json format)
+                generated by the databricks-CLI. If missing, then the argument worker_info has to be provided.
+        :param  worker_info: A path pointing to a yaml file containing the system information of a
+                worker node. It is assumed that all workers are homogenous.
+                If missing, the wrapper pulls the worker info from the "gpu_cluster".
+        :param  eventlogs: Event log filenames or ABFS (Azure Blob File System) storage directories
+                containing event logs (comma separated). If missing, the wrapper reads the Spark's
+                property `spark.eventLog.dir` defined in `gpu_cluster`. This property should be included
+                in the output of `databricks clusters get [--cluster-id CLUSTER_ID| --cluster-name CLUSTER_NAME]`.
+                Note that the wrapper will raise an exception if the property is not set.
+        :param profile: A named Databricks profile to get the settings/credentials of the Databricks CLI.
+        :param local_folder: Local work-directory path to store the output and to be used as root
+                directory for temporary folders/files. The final output will go into a subdirectory called
+                ${local_folder}/prof-${EXEC_ID} where exec_id is an auto-generated unique identifier of the
+                execution. If the argument is NONE, the default value is the env variable
+                RAPIDS_USER_TOOLS_OUTPUT_DIRECTORY if any; or the current working directory.
+        :param remote_folder: An ABFS (Azure Blob File System) folder where the output is uploaded at the end
+                of execution. If no value is provided, the output will be only available on local disk.
+        :param tools_jar: Path to a bundled jar including Rapids tool. The path is a local filesystem,
+                or remote S3 url. If missing, the wrapper downloads the latest rapids-4-spark-tools_*.jar
+                from maven repo.
+        :param credentials_file: The local path of JSON file that contains the application credentials.
+               If missing, the wrapper looks for "DATABRICKS_CONFIG_FILE" environment variable
+               to provide the location of a credential file. The default credentials file exists as
+               "~/.databrickscfg" on Unix, Linux, or macOS.
+        :param verbose: True or False to enable verbosity to the wrapper script.
+        :param jvm_heap_size: The maximum heap size of the JVM in gigabytes.
+        :param rapids_options: A list of valid Profiling tool options.
+                Note that the wrapper ignores ["output-directory", "worker-info"] flags, and it does not support
+                multiple "spark-property" arguments.
+                For more details on Profiling tool options, please visit
+                https://nvidia.github.io/spark-rapids/docs/spark-profiling-tool.html#profiling-tool-options
+        """
+        if verbose:
+            # when debug is set to true set it in the environment.
+            ToolLogging.enable_debug_mode()
+        wrapper_prof_options = {
+            'platformOpts': {
+                # the databricks profile
+                'profile': profile,
+                'credentialFile': credentials_file,
+                'deployMode': DeployMode.LOCAL,
+            },
+            'migrationClustersProps': {
+                'gpuCluster': gpu_cluster
+            },
+            'jobSubmissionProps': {
+                'remoteFolder': remote_folder,
+                'platformArgs': {
+                    'jvmMaxHeapSize': jvm_heap_size
+                }
+            },
+            'eventlogs': eventlogs,
+            'toolsJar': tools_jar,
+            'autoTunerFileInput': worker_info
+        }
+        ProfilingAsLocal(platform_type=CloudPlatform.DATABRICKS_AZURE,
+                         output_folder=local_folder,
+                         wrapper_options=wrapper_prof_options,
+                         rapids_options=rapids_options).launch()
+
 
 class DBAzureWrapper:  # pylint: disable=too-few-public-methods
     """
     A wrapper script to run RAPIDS Accelerator tools (Qualification, Profiling, and Bootstrap) on Databricks_Azure.
     """
 
     def __init__(self):
         self.qualification = CliDBAzureLocalMode.qualification
+        self.profiling = CliDBAzureLocalMode.profiling
```

## spark_rapids_pytools/wrappers/dataproc_wrapper.py

```diff
@@ -16,26 +16,24 @@
 """Wrapper class to run tools associated with RAPIDS Accelerator for Apache Spark plugin on Dataproc."""
 
 from spark_rapids_pytools.cloud_api.sp_types import DeployMode, CloudPlatform
 from spark_rapids_pytools.common.utilities import ToolLogging
 from spark_rapids_pytools.rapids.bootstrap import Bootstrap
 from spark_rapids_pytools.rapids.diagnostic import Diagnostic
 from spark_rapids_pytools.rapids.profiling import ProfilingAsLocal
-from spark_rapids_pytools.rapids.qualification import QualFilterApp, QualificationAsLocal, QualGpuClusterReshapeType, \
-    QualificationAsRemote
+from spark_rapids_pytools.rapids.qualification import QualFilterApp, QualificationAsLocal, QualGpuClusterReshapeType
 
 
 class CliDataprocLocalMode:  # pylint: disable=too-few-public-methods
     """
     A wrapper that runs the RAPIDS Accelerator tools locally on the dev machine for Dataproc.
     """
 
     @staticmethod
     def qualification(cpu_cluster: str,
-                      execution_cluster: str = None,
                       eventlogs: str = None,
                       local_folder: str = None,
                       remote_folder: str = None,
                       gpu_cluster: str = None,
                       tools_jar: str = None,
                       credentials_file: str = None,
                       filter_apps: str = QualFilterApp.tostring(QualFilterApp.SAVINGS),
@@ -48,33 +46,32 @@
         The Qualification tool analyzes Spark events generated from CPU based Spark applications to
         help quantify the expected acceleration and costs savings of migrating a Spark application
         or query to GPU. The wrapper downloads dependencies and executes the analysis on the local
         dev machine
         :param cpu_cluster: The Dataproc-cluster on which the Spark applications were executed. The argument
                 can be a Dataproc-cluster or a valid path to the cluster's properties file (json format)
                 generated by the gcloud-CLI.
-        :param execution_cluster: the cluster on which the Rapids tool will be running.
-        :param  eventlogs: Event log filenames or S3 storage directories
+        :param  eventlogs: Event log filenames or gcs storage directories
                 containing event logs (comma separated). If missing, the wrapper Reads the Spark's
                 property `spark.eventLog.dir` defined in `cpu_cluster`. This property should be included
                 in the output of `gcloud dataproc clusters describe`
                 Note that the wrapper will raise an exception if the property is not set
         :param local_folder: Local work-directory path to store the output and to be used as root
                 directory for temporary folders/files. The final output will go into a subdirectory called
                 ${local_folder}/qual-${EXEC_ID} where exec_id is an auto-generated unique identifier of the
                 execution. If the argument is NONE, the default value is the env variable
                 RAPIDS_USER_TOOLS_OUTPUT_DIRECTORY if any; or the current working directory
-        :param remote_folder: An S3 folder where the output is uploaded at the end of execution.
+        :param remote_folder: A gcs folder where the output is uploaded at the end of execution.
                 If no value is provided, the output will be only available on local disk
         :param gpu_cluster: The Dataproc-cluster on which the Spark applications is planned to be migrated.
                 The argument can be a Dataproc-cluster or a valid path to the cluster's properties file
                 (json format) generated by the gcloud-CLI. If missing, the wrapper maps the dataproc machine
                 instances of the original cluster into dataproc instances that support GPU acceleration
         :param tools_jar: Path to a bundled jar including Rapids tool. The path is a local filesystem,
-                or remote S3 url. If missing, the wrapper downloads the latest rapids-4-spark-tools_*.jar
+                or remote gcs url. If missing, the wrapper downloads the latest rapids-4-spark-tools_*.jar
                 from maven repo
         :param credentials_file: The local path of JSON file that contains the application credentials.
                If missing, the wrapper looks for "GOOGLE_APPLICATION_CREDENTIALS" environment variable
                to provide the location of a credential JSON file. The default credentials file exists as
                "$HOME/.config/gcloud/application_default_credentials.json"
         :param filter_apps: filtering criteria of the applications listed in the final STDOUT table
                 is one of the following (NONE, SPEEDUPS, savings).
@@ -98,15 +95,15 @@
         """
         if verbose:
             # when debug is set to true set it in the environment.
             ToolLogging.enable_debug_mode()
         wrapper_qual_options = {
             'platformOpts': {
                 'credentialFile': credentials_file,
-                'deployMode': DeployMode.REMOTE_CLUSTER if execution_cluster else DeployMode.LOCAL,
+                'deployMode': DeployMode.LOCAL,
             },
             'migrationClustersProps': {
                 'cpuCluster': cpu_cluster,
                 'gpuCluster': gpu_cluster
             },
             'jobSubmissionProps': {
                 'remoteFolder': remote_folder,
@@ -115,26 +112,19 @@
                 }
             },
             'eventlogs': eventlogs,
             'filterApps': filter_apps,
             'toolsJar': tools_jar,
             'gpuClusterRecommendation': gpu_cluster_recommendation
         }
-        if execution_cluster:
-            tool_obj = QualificationAsRemote(platform_type=CloudPlatform.DATAPROC,
-                                             cluster=execution_cluster,
-                                             output_folder=local_folder,
-                                             wrapper_options=wrapper_qual_options,
-                                             rapids_options=rapids_options)
-        else:
-            tool_obj = QualificationAsLocal(platform_type=CloudPlatform.DATAPROC,
-                                            cluster=execution_cluster,
-                                            output_folder=local_folder,
-                                            wrapper_options=wrapper_qual_options,
-                                            rapids_options=rapids_options)
+
+        tool_obj = QualificationAsLocal(platform_type=CloudPlatform.DATAPROC,
+                                        output_folder=local_folder,
+                                        wrapper_options=wrapper_qual_options,
+                                        rapids_options=rapids_options)
         tool_obj.launch()
 
     @staticmethod
     def profiling(gpu_cluster: str = None,
                   worker_info: str = None,
                   eventlogs: str = None,
                   local_folder: str = None,
```

## spark_rapids_pytools/wrappers/emr_wrapper.py

```diff
@@ -16,15 +16,15 @@
 """Wrapper class to run tools associated with RAPIDS Accelerator for Apache Spark plugin on AWS-EMR."""
 
 from spark_rapids_pytools.cloud_api.sp_types import DeployMode, CloudPlatform
 from spark_rapids_pytools.common.utilities import ToolLogging
 from spark_rapids_pytools.rapids.bootstrap import Bootstrap
 from spark_rapids_pytools.rapids.diagnostic import Diagnostic
 from spark_rapids_pytools.rapids.qualification import QualFilterApp, QualificationAsLocal, \
-    Qualification, QualGpuClusterReshapeType
+    QualGpuClusterReshapeType
 
 
 class CliEmrLocalMode:  # pylint: disable=too-few-public-methods
     """
     A wrapper that runs the RAPIDS Accelerator tools locally on the dev machine.
     """
 
@@ -200,117 +200,16 @@
         diag_tool = Diagnostic(platform_type=CloudPlatform.EMR,
                                cluster=cluster,
                                output_folder=output_folder,
                                wrapper_options=wrapper_diag_options)
         diag_tool.launch()
 
 
-class CliEmrServerlessMode:  # pylint: disable=too-few-public-methods
-    """
-    A wrapper that runs the logic as an EMR-serverless application.
-    """
-
-    @staticmethod
-    def qualification(cpu_cluster: str,
-                      remote_folder: str,
-                      job_arn: str,
-                      eventlogs: str = None,
-                      profile: str = None,
-                      app_id: str = None,
-                      gpu_cluster: str = None,
-                      local_folder: str = None,
-                      tools_jar: str = None,
-                      filter_apps: str = QualFilterApp.tostring(QualFilterApp.SAVINGS),
-                      verbose: bool = False,
-                      **rapids_options) -> None:
-        """
-        The Qualification tool analyzes Spark events generated from CPU based Spark applications to
-        help quantify the expected acceleration and costs savings of migrating a Spark application
-        or query to GPU. The wrapper submits Spark EMR-Serverless job to run the RAPIDS accelerator.
-
-        :param cpu_cluster: The EMR-cluster on which the Spark applications were executed. The argument
-               can be an EMR-cluster or a valid path to the cluster's properties file (json format)
-               generated by the AWS CLI.
-        :param eventlogs: Event log filenames or S3 storage directories
-               containing event logs (comma separated). If missing, the wrapper Reads the Spark's
-               property `spark.eventLog.dir` defined in `cpu_cluster`. This property should be included
-               in the output of `emr describe-cluster`. Note that the wrapper will raise an exception
-               if the property is not set.
-        :param remote_folder: The S3 folder where the output is archived.
-        :param job_arn: The execution role ARN for the job run.
-        :param app_id: The ID of the EMR-serverless application on which to run the job.
-                If missing, the wrapper creates an EMR-serverless application that gets deleted at
-                the end of the execution. Note that creating an EMR-serverless application takes a few
-                minutes.
-        :param gpu_cluster: The EMR-cluster on which the Spark applications is planned to be migrated.
-                The argument can be an EMR-cluster or a valid path to the cluster's properties file
-                (json format) generated by the AWS CLI. If missing, the wrapper maps the EC2 machine
-                instances of the original cluster into EC2 instances that support GPU acceleration.
-        :param local_folder: Local work-directory path to store the output and to be used as root
-                directory for temporary folders/files. If the argument is NONE,
-               the default value is the env variable RAPIDS_USER_TOOLS_OUTPUT_DIRECTORY if any;
-               or the current working directory.
-        :param profile: A named AWS profile that you can specify to get the settings/credentials of the AWS account.
-        :param tools_jar: Path to a bundled jar including RAPIDS tool. The path is a local filesystem,
-                or remote S3 url. If missing, the wrapper downloads the latest rapids-4-spark-tools_*.jar
-                from maven repo.
-        :param filter_apps: filtering criteria of the applications listed in the final STDOUT table
-                is one of the following (NONE, SPEEDUPS, savings). Default is "SAVINGS".
-                Note that this filter does not affect the CSV report.
-                "NONE" means no filter applied. "SPEEDUPS" lists all the apps that are either
-                'Recommended', or 'Strongly Recommended' based on speedups. "SAVINGS"
-                lists all the apps that have positive estimated GPU savings except for the apps that
-                are "Not Applicable".
-        :param verbose: True or False to enable verbosity to the wrapper script.
-        :param rapids_options: A list of valid Qualification tool options.
-            Note that the wrapper ignores ["output-directory", "platform"] flags, and it does not support
-            multiple “spark-property“ arguments.
-            For more details on Qualification tool options, please visit
-            https://nvidia.github.io/spark-rapids/docs/spark-qualification-tool.html#qualification-tool-options
-        """
-        if verbose:
-            # when debug is set to true set it in the environment.
-            ToolLogging.enable_debug_mode()
-        wrapper_qual_options = {
-            'platformOpts': {
-                'profile': profile,
-                'deployMode': DeployMode.SERVERLESS,
-            },
-            'migrationClustersProps': {
-                'cpuCluster': cpu_cluster,
-                'gpuCluster': gpu_cluster
-            },
-            'jobSubmissionProps': {
-                'remoteFolder': remote_folder,
-                'platformArgs': {
-                    'application-id': app_id,
-                    'execution-role-arn': job_arn,
-                }
-            },
-            'eventlogs': eventlogs,
-            'filterApps': filter_apps,
-            'toolsJar': tools_jar,
-        }
-        Qualification(platform_type=CloudPlatform.EMR,
-                      cluster=None,
-                      output_folder=local_folder,
-                      wrapper_options=wrapper_qual_options,
-                      rapids_options=rapids_options).launch()
-
-
 class EMRWrapper:  # pylint: disable=too-few-public-methods
     """
     A wrapper script to run RAPIDS Accelerator tools (Qualification, Profiling, and Bootstrap) on Amazon EMR.
-    :param mode: The deployment mode of the tool command from RAPIDS Accelerator for Apache Spark. Accepted options
-                are <local|serverless>. local means that the tool runs locally on the development machine.
-                "serverless" means that the wrapper will trigger an Amazon EMR cluster to submit a new job.
     """
 
-    def __init__(self, mode: str = DeployMode.pretty_print(DeployMode.LOCAL)):
-        self.mode = mode
-        if DeployMode.fromstring(self.mode) == DeployMode.SERVERLESS:
-            self.qualification = CliEmrServerlessMode.qualification
-            self.bootstrap = CliEmrLocalMode.bootstrap
-        else:
-            self.qualification = CliEmrLocalMode.qualification
-            self.bootstrap = CliEmrLocalMode.bootstrap
-            self.diagnostic = CliEmrLocalMode.diagnostic
+    def __init__(self):
+        self.qualification = CliEmrLocalMode.qualification
+        self.bootstrap = CliEmrLocalMode.bootstrap
+        self.diagnostic = CliEmrLocalMode.diagnostic
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## spark_rapids_pytools/wrappers/onprem_wrapper.py

```diff
@@ -13,39 +13,68 @@
 # limitations under the License.
 
 
 """Wrapper class to run tools associated with RAPIDS Accelerator for Apache Spark plugin on On-Prem cluster."""
 
 from spark_rapids_pytools.cloud_api.sp_types import DeployMode, CloudPlatform
 from spark_rapids_pytools.common.utilities import ToolLogging
+from spark_rapids_pytools.rapids.profiling import ProfilingAsLocal
 from spark_rapids_pytools.rapids.qualification import QualFilterApp, QualificationAsLocal, QualGpuClusterReshapeType
 
 
 class CliOnpremLocalMode:  # pylint: disable=too-few-public-methods
     """
     A wrapper that runs the RAPIDS Accelerator tools locally on the dev machine for OnPrem
     platform. Apps are qualified based on speedup.
     """
 
     @staticmethod
     def qualification(cpu_cluster: str = None,
-                      execution_cluster: str = None,
                       eventlogs: str = None,
                       local_folder: str = None,
-                      remote_folder: str = None,
-                      gpu_cluster: str = None,
                       tools_jar: str = None,
-                      credentials_file: str = None,
                       filter_apps: str = QualFilterApp.tostring(QualFilterApp.SPEEDUPS),
                       target_platform: str = None,
                       gpu_cluster_recommendation: str = QualGpuClusterReshapeType.tostring(
                           QualGpuClusterReshapeType.get_default()),
                       jvm_heap_size: int = 24,
                       verbose: bool = False,
                       **rapids_options) -> None:
+        """
+        The Qualification tool analyzes Spark events generated from CPU based Spark applications to
+        help quantify the expected acceleration and costs savings of migrating a Spark application
+        or query to GPU. The wrapper downloads dependencies and executes the analysis on the local
+        dev machine
+        :param cpu_cluster: The on-premises cluster on which the Apache Spark applications were executed.
+                Accepted value is valid path to the cluster properties file (json format).
+        :param eventlogs: A comma separated list of urls pointing to event logs in local directory.
+        :param local_folder: Local work-directory path to store the output and to be used as root
+                directory for temporary folders/files. The final output will go into a subdirectory
+                named `qual-${EXEC_ID}` where `exec_id` is an auto-generated unique identifier of the execution.
+        :param tools_jar: Path to a bundled jar including RAPIDS tool. The path is a local filesystem path
+        :param filter_apps:  Filtering criteria of the applications listed in the final STDOUT table is one of
+                the following (`NONE`, `SPEEDUPS`). "`NONE`" means no filter applied. "`SPEEDUPS`" lists all the
+                apps that are either '_Recommended_', or '_Strongly Recommended_' based on speedups.
+        :param target_platform: Cost savings and speedup recommendation for comparable cluster in target_platform
+                based on on-premises cluster configuration. Currently only `dataproc` is supported for
+                target_platform.If not provided, the final report will be limited to GPU speedups only
+                without cost-savings.
+        :param gpu_cluster_recommendation: The type of GPU cluster recommendation to generate.
+               It accepts one of the following ("CLUSTER", "JOB" and the default value "MATCH").
+                "MATCH": keep GPU cluster same number of nodes as CPU cluster;
+                "CLUSTER": recommend optimal GPU cluster by cost for entire cluster;
+                "JOB": recommend optimal GPU cluster by cost per job
+        :param jvm_heap_size: The maximum heap size of the JVM in gigabytes
+        :param verbose: True or False to enable verbosity to the wrapper script
+        :param rapids_options: A list of valid Qualification tool options.
+                Note that the wrapper ignores ["output-directory", "platform"] flags, and it does not support
+                multiple "spark-property" arguments.
+                For more details on Qualification tool options, please visit
+                https://nvidia.github.io/spark-rapids/docs/spark-qualification-tool.html#qualification-tool-options
+        """
         if verbose:
             # when debug is set to true set it in the environment.
             ToolLogging.enable_debug_mode()
         # if target_platform is specified, check if it's valid supported platform and filter the
         # apps based on savings
         if target_platform is not None:
             if CliOnpremLocalMode.is_target_platform_supported(target_platform):
@@ -55,45 +84,96 @@
                 filter_apps: str = QualFilterApp.tostring(QualFilterApp.SAVINGS)
             else:
                 raise RuntimeError(target_platform + ' platform is currently not supported to calculate savings'
                                    ' from OnPrem cluster')
 
         wrapper_qual_options = {
             'platformOpts': {
-                'credentialFile': credentials_file,
                 'deployMode': DeployMode.LOCAL,
                 'targetPlatform': target_platform
             },
             'migrationClustersProps': {
-                'cpuCluster': cpu_cluster,
-                'gpuCluster': gpu_cluster
+                'cpuCluster': cpu_cluster
             },
             'jobSubmissionProps': {
-                'remoteFolder': remote_folder,
                 'platformArgs': {
                     'jvmMaxHeapSize': jvm_heap_size
                 }
             },
             'eventlogs': eventlogs,
             'filterApps': filter_apps,
             'toolsJar': tools_jar,
             'gpuClusterRecommendation': gpu_cluster_recommendation,
             'target_platform': target_platform
         }
         tool_obj = QualificationAsLocal(platform_type=CloudPlatform.ONPREM,
-                                        cluster=execution_cluster,
                                         output_folder=local_folder,
                                         wrapper_options=wrapper_qual_options,
                                         rapids_options=rapids_options)
         tool_obj.launch()
 
     @staticmethod
     def is_target_platform_supported(target_platform: str):
         return target_platform == 'dataproc'
 
+    @staticmethod
+    def profiling(worker_info: str = None,
+                  eventlogs: str = None,
+                  local_folder: str = None,
+                  tools_jar: str = None,
+                  jvm_heap_size: int = 24,
+                  verbose: bool = False,
+                  **rapids_options) -> None:
+        """
+        The Profiling tool analyzes both CPU or GPU generated event logs and generates information
+        which can be used for debugging and profiling Apache Spark applications.
+
+        :param  worker_info: A path pointing to a yaml file containing the system information of a
+        worker node. It is assumed that all workers are homogenous.
+        If missing, it throws an error.
+        :param  eventlogs: Event log filenames or directories containing event logs (comma separated).
+        :param local_folder: Local work-directory path to store the output and to be used as root
+        directory for temporary folders/files. The final output will go into a subdirectory called
+        ${local_folder}/prof-${EXEC_ID} where exec_id is an auto-generated unique identifier of the
+        execution. If the argument is NONE, the default value is the env variable
+        RAPIDS_USER_TOOLS_OUTPUT_DIRECTORY if any; or the current working directory.
+        :param tools_jar: Path to a bundled jar including Rapids tool. The path is a local filesystem.
+        If missing, the wrapper downloads the latest rapids-4-spark-tools_*.jar from maven repo
+        :param verbose: True or False to enable verbosity to the wrapper script
+        :param jvm_heap_size: The maximum heap size of the JVM in gigabytes
+        :param rapids_options: A list of valid Profiling tool options.
+        Note that the wrapper ignores ["output-directory", "worker-info"] flags, and it does not support
+        multiple "spark-property" arguments.
+        For more details on Profiling tool options, please visit
+        https://nvidia.github.io/spark-rapids/docs/spark-profiling-tool.html#profiling-tool-options
+        """
+
+        if verbose:
+            # when debug is set to true set it in the environment.
+            ToolLogging.enable_debug_mode()
+        wrapper_prof_options = {
+            'platformOpts': {
+                'deployMode': DeployMode.LOCAL,
+                'targetPlatform': CloudPlatform.ONPREM
+            },
+            'jobSubmissionProps': {
+                'platformArgs': {
+                     'jvmMaxHeapSize': jvm_heap_size
+                }
+            },
+            'eventlogs': eventlogs,
+            'toolsJar': tools_jar,
+            'autoTunerFileInput': worker_info
+        }
+        ProfilingAsLocal(platform_type=CloudPlatform.ONPREM,
+                         output_folder=local_folder,
+                         wrapper_options=wrapper_prof_options,
+                         rapids_options=rapids_options).launch()
+
 
 class OnPremWrapper:  # pylint: disable=too-few-public-methods
     """
-    A wrapper script to run RAPIDS Accelerator tools (Qualification) on On-prem cluster.
+    A wrapper script to run RAPIDS Accelerator tools (Qualification, Profiling) on On-prem cluster.
     """
     def __init__(self):
         self.qualification = CliOnpremLocalMode.qualification
+        self.profiling = CliOnpremLocalMode.profiling
```

## Comparing `spark_rapids_user_tools-23.6.1.dist-info/LICENSE` & `spark_rapids_user_tools-23.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `spark_rapids_user_tools-23.6.1.dist-info/METADATA` & `spark_rapids_user_tools-23.6.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: spark-rapids-user-tools
-Version: 23.6.1
+Version: 23.6.2
 Summary: A simple wrapper process around cloud service providers to run tools for the RAPIDS Accelerator for Apache Spark.
 Author-email: NVIDIA Corporation <spark-rapids-support@nvidia.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chevron (==0.14.0)
 Requires-Dist: fastprogress (==1.0.3)
 Requires-Dist: fastcore (==1.5.29)
-Requires-Dist: fire (==0.4.0)
+Requires-Dist: fire (>=0.5.0)
 Requires-Dist: pandas (==1.4.3)
 Requires-Dist: pyYAML (==6.0)
 Requires-Dist: tabulate (==0.8.10)
 Requires-Dist: importlib-resources (==5.10.2)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: packaging (==23.0)
 Requires-Dist: certifi (==2022.12.7)
```

## Comparing `spark_rapids_user_tools-23.6.1.dist-info/RECORD` & `spark_rapids_user_tools-23.6.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,68 @@
-spark_rapids_pytools/__init__.py,sha256=0swyb0tOSpVwpEU_yt3yo-AIZiPAiNZP-aZHixOPJhA,750
+spark_rapids_pytools/__init__.py,sha256=v4w4dPmBMO2Koe_vJ0T3X8-SDijhkEnnLRiPmH3eJKI,750
 spark_rapids_pytools/build.py,sha256=Ej4Pc2jPIyeVUUOyC67ZMc6Tj90NKj0DrXyniJc0FnY,992
 spark_rapids_pytools/wrapper.py,sha256=mKTxIpK3V_OKJ4ua3TSjasC5mITs_TRHU5dRfCqcde0,1324
+spark_rapids_pytools/ascli_cli/__init__.py,sha256=i0t3LTjoAuxT5vp9ikODfXK3OnvCNYjFymqk5KMDMf4,627
+spark_rapids_pytools/ascli_cli/ascli.py,sha256=Y397MBIGTTPWiPLRrEb-5XJLNrtd17cYZDcChF7W5xE,8270
 spark_rapids_pytools/cloud_api/__init__.py,sha256=NQSbmxhLzvnZrf4ltpgCLMjCEERPv5QoYo62LEdDBs8,646
 spark_rapids_pytools/cloud_api/azurestorage.py,sha256=yuFk7H5Y8aY0H5dOmeJBS03uhgS2nah5v0Kw2GJzDnE,8507
-spark_rapids_pytools/cloud_api/databricks_aws.py,sha256=g0XXBVeQwtVAjsm6Po3R3dUA-7CUqaRp9W7iFqkuU4I,12837
+spark_rapids_pytools/cloud_api/databricks_aws.py,sha256=W0qOOwfTzzW2MK-fL5V7mXvpz17-DbmllIlCD-cViG4,12662
 spark_rapids_pytools/cloud_api/databricks_aws_job.py,sha256=ZNYM2pa8fObRhc9c9VcqCT6HxGJNfHeFhdoVYNek51E,1268
-spark_rapids_pytools/cloud_api/databricks_azure.py,sha256=D5FcZ-wo0lNf3NOMI6sXQGk8ur7RsYG1sBj1kys_kM0,16418
+spark_rapids_pytools/cloud_api/databricks_azure.py,sha256=QcOoVpkp9waGsgELqkDW1dj73PruZN-vD2d4EK7u--Y,16308
 spark_rapids_pytools/cloud_api/databricks_azure_job.py,sha256=u-wOcJXRyFCuEsXQypW8O09O5YQ2pt_gNcOlQjwpXYE,2428
-spark_rapids_pytools/cloud_api/dataproc.py,sha256=i4yoDrZ5D5vghN1KXq1HRXiNzefbRGi7GdpC40SCb84,24930
-spark_rapids_pytools/cloud_api/dataproc_job.py,sha256=gwqDpa_pmwKB5TAFCJqWs8mOFENcMhwfgCJwOh3TMVg,1426
-spark_rapids_pytools/cloud_api/emr.py,sha256=pZZqaVjEqHmIMvABoHvVW8v9l7k0C1ommqzGSQM2Sok,22142
-spark_rapids_pytools/cloud_api/emr_job.py,sha256=EoVrjwSL9pYTJk6QDfokQOudla8KLwGAbR0AAZhk2bA,11269
+spark_rapids_pytools/cloud_api/dataproc.py,sha256=iQZvIyu__ge2Wf_fRKpjBVKWfOkI4DENxO8ZLy1lsqs,24674
+spark_rapids_pytools/cloud_api/dataproc_job.py,sha256=VMBbFjUfzF7ZZtwWI5dsc8exiZwkARHQIeWIcY3wZNs,922
+spark_rapids_pytools/cloud_api/emr.py,sha256=qZtOUIR7UpSDAOn292lwlMO5sx5-UjEdSTHS8sT5LPk,21033
+spark_rapids_pytools/cloud_api/emr_job.py,sha256=-6VA4HV34BVm_CoxaSh13pDb1pyeYHoRbzWVQFfuT0o,1252
 spark_rapids_pytools/cloud_api/gstorage.py,sha256=88IzLWOzEphCETGQaVN3_U7wUD0M2doDy759WQmNoJI,4939
-spark_rapids_pytools/cloud_api/onprem.py,sha256=fagH-UiD8DgK2AMTmEcUoNYq34dGWfXT2cSp39RR4Tw,13541
+spark_rapids_pytools/cloud_api/onprem.py,sha256=hrsUe0KUa6qEMYiXgse5myDtllE25K1C3AikEJvXrkU,13387
 spark_rapids_pytools/cloud_api/s3storage.py,sha256=cFqZETxWt_3Yagk3UlQt65pM4A0qb6idpbi8kUOK5pE,4055
-spark_rapids_pytools/cloud_api/sp_types.py,sha256=HcykohkS7asOhNPu5PD2PLEuphzA13CSt0vNe7zoqx4,51283
+spark_rapids_pytools/cloud_api/sp_types.py,sha256=3FSnFir4jP9VvHcM1bWd3DifT4XduhYp47BlhJEZQLM,51024
 spark_rapids_pytools/common/__init__.py,sha256=A8h0t211p8t_aATYiwCLWTwTy564kCcZp-HTWKiO4u8,658
 spark_rapids_pytools/common/exceptions.py,sha256=CK9PF75hSrRh6qaz0aKoiNqaU78E8OfiNydZ4i6WgoM,978
 spark_rapids_pytools/common/prop_manager.py,sha256=ijCqsnrLHn8Ntb1dCEDHqITrxjb3LoEP8Eqhqsb0PS8,5432
 spark_rapids_pytools/common/sys_storage.py,sha256=-La2Oc5EemnRH2x5B24MHlrtEZh6nL2FjqAyrV953Os,14712
 spark_rapids_pytools/common/utilities.py,sha256=VtS0shH3GhOTGpHHZNYdH4p1ziKKY1h14Q_qfRi7XQk,14006
 spark_rapids_pytools/pricing/__init__.py,sha256=Y_IWTtiKulkkoC84SLS8LkRWTi393zeUGHaNogZfOSg,659
 spark_rapids_pytools/pricing/databricks_azure_pricing.py,sha256=HLto1Dbv61Awfo4icJiRiCkx3G8KDRfUBiTjloEy1WM,3429
 spark_rapids_pytools/pricing/databricks_pricing.py,sha256=q7pRBs2YGJAJnxItBUDYB00f3hdWsFKgK4sXZocjMC4,3522
 spark_rapids_pytools/pricing/dataproc_pricing.py,sha256=4-RuYxW9V0K0mqj2mqCJsKEUbvxPXHCwF4AsK1z6UXE,4247
 spark_rapids_pytools/pricing/emr_pricing.py,sha256=vat14Df8_1By-McNl2ot_75RAwjJkyTfXA24-iefrM4,4717
 spark_rapids_pytools/pricing/price_provider.py,sha256=zZt2ay-BN1vM0cZXkiEzY5kpnYx1brRCJcyfotU71lo,6400
 spark_rapids_pytools/rapids/__init__.py,sha256=xiYk9b76AV_v3fEELcYzXCUPvXQhCD687eJ5RCYQW7M,666
 spark_rapids_pytools/rapids/bootstrap.py,sha256=KEeF1Ux0mfqCW-6oyQOoImSuCm_MmoITm_t6qg9yB4s,8830
 spark_rapids_pytools/rapids/diagnostic.py,sha256=pShr5Ndi8kxZXTbZ7fOkbWVk2opF1UYP0q4AJETGHGc,6546
-spark_rapids_pytools/rapids/profiling.py,sha256=n0l6-WKweQPBg_7g9rNb9YqIpsZcPVT3YosFZ3bmglQ,13489
-spark_rapids_pytools/rapids/qualification.py,sha256=5zKCPacUyWdVKhAupMncw6_4UgnDRt7kqQ8_kq0RfJ0,43658
-spark_rapids_pytools/rapids/rapids_job.py,sha256=w7D5jZPCsyb7PqupPfQ02bNnOYAwld7RLMHXqoovUTs,6864
-spark_rapids_pytools/rapids/rapids_tool.py,sha256=3USqFAQRUDKDtsBHUqQSP-EQHp-71USzcYKlmciZh3w,33590
+spark_rapids_pytools/rapids/profiling.py,sha256=ufyIUOxRXeZGPBRQ2jH3d0-qQ4vzUe2HNrKtmYkZzgs,14549
+spark_rapids_pytools/rapids/qualification.py,sha256=kiYkjgTrUPH5z6RenxJJt1w26khHfYy-nzUCIzh7vjQ,38670
+spark_rapids_pytools/rapids/rapids_job.py,sha256=HId6wvfXwsPVb26meKGn_C1PcS68NGT41uNgZZx6vTY,5739
+spark_rapids_pytools/rapids/rapids_tool.py,sha256=SX8GpcHRQB3v4hJgKD2dJNz8rjcZMyf2wwdcRKTGEHs,33598
 spark_rapids_pytools/rapids/tool_ctxt.py,sha256=8bWqooTKcIH5ShxTFrXPuSr1KEJeHXU5LdDq8F6ienU,6576
 spark_rapids_pytools/resources/bootstrap-conf.yaml,sha256=xATXdInBA2NFR2Le9uqioRwyqYB7TnFBYvoaT8NEDZQ,1390
 spark_rapids_pytools/resources/collect.sh,sha256=EdbNF90ZQUgaERPYY1p3fYdf3qvmU9f2WGD7RzYoLOE,4453
 spark_rapids_pytools/resources/databricks-premium-catalog.json,sha256=XBptMDeu7Abbrv6xC4C1oDuMuEIqnrGEqwrhJFutLJM,30566
 spark_rapids_pytools/resources/databricks_aws-configs.json,sha256=I_VqLdvavbQGUqCNcUqMpNrH5aF0xBZDdN7kuncNKQk,10448
 spark_rapids_pytools/resources/databricks_azure-configs.json,sha256=TSo17t28bRfeAjSWDZR4KqMhEUKoLzoqO5YknfiokYA,10017
 spark_rapids_pytools/resources/dataproc-configs.json,sha256=9rEXtuCKsLUMyoRsKAeW2OWckM1AXYsE3JuNjFAYmWA,8047
 spark_rapids_pytools/resources/diagnostic-conf.yaml,sha256=vS32UyRhj5ox2MZ8-6EgMjXEWlGeaw9izYiAdAoWpfE,30
 spark_rapids_pytools/resources/emr-configs.json,sha256=_F5XxM5kFen_iCAWW5Z_jdD6G626h4hH_Uf2dq2Dn6U,8994
 spark_rapids_pytools/resources/onprem-configs.json,sha256=TWqp95Ildys0-eGOrWNL-KpUqTTLVHLqzW4u48eNmhM,4727
 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json,sha256=KGxUoiNPVTVzQaR3SN_FV9PH80fEnp6JnMhnv2YFOBY,38903
-spark_rapids_pytools/resources/profiling-conf.yaml,sha256=s7TR1agVORA4g28bYYK7jSMpgMT6s-awMySK0jT4kaA,1460
+spark_rapids_pytools/resources/profiling-conf.yaml,sha256=jdJy6I_alouAk_Ff39r0a3D8EAByaKK2r979bAjPTrQ,1524
 spark_rapids_pytools/resources/qualification-conf.yaml,sha256=FwQGa9cFXQbEutN9aGb9IEzgRFdHTC7fP_QYTrFWmyc,4273
 spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py,sha256=lmXGoTdrwdrhh8UO7DSL-kgbLOJP1X0kgJPq6cJfF3U,2195
 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms,sha256=pigL0kAsg1VaP9Jn9-5oNblJRj0IbeZLh1T5Op8CQqA,671
 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms,sha256=lmnyouNCpbytpRVZ_YbQ6d6hCl3XaYxqzNomxSJwSSk,518
 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms,sha256=UIlW0GcYn2fovtcDNYPUmg99h0zKy-DxXGO-1Lr_xQs,855
 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms,sha256=7xqXBMIu5Tg02KCq_YN9oLLiE3c8jgWl8BUvFQZODhs,537
+spark_rapids_pytools/resources/templates/info_recommendations_disabled.ms,sha256=YwNa8iY9MhoDFWU_KfgPIO1hdfHssWXZw51dYXbM9T8,424
 spark_rapids_pytools/wrappers/__init__.py,sha256=CQ7Mf-YyBFNl6xmQGsPARv1w5GU3jGliByn5IHCcLkE,630
 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py,sha256=-axS_C8sb3RvlOByfk6ZqYQvOSJ36GJwk4zwqiZ-t-c,13207
-spark_rapids_pytools/wrappers/databricks_azure_wrapper.py,sha256=5NElNnmmGg7v8WuFgraCAR1qX6X7w3N-NPwe7ypXi3o,7985
-spark_rapids_pytools/wrappers/dataproc_wrapper.py,sha256=96wdNER9NZVv8N0-YElje6pYuNUt2Oz_WpJ4fdLKnoE,16647
-spark_rapids_pytools/wrappers/emr_wrapper.py,sha256=v8bw3qDWc5vzrW8s6MWCl3uHv4H2423H8E-3G2x7dPI,18151
-spark_rapids_pytools/wrappers/onprem_wrapper.py,sha256=KFZrSMjk4xTLWC8lEhnD1ms1bZ75Sch0yLRL9swKULM,4480
-spark_rapids_user_tools-23.6.1.dist-info/LICENSE,sha256=RnI8IUCDrXfGVHFfYTsT8OKEuaOtkMGDQOn8foh7D00,21086
-spark_rapids_user_tools-23.6.1.dist-info/METADATA,sha256=LwgOAl_HA7lfnvfMBhFCuvxxfEGp4inf9aP4Wq3nygE,2927
-spark_rapids_user_tools-23.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spark_rapids_user_tools-23.6.1.dist-info/entry_points.txt,sha256=GyaV1NES81c2p204FZjglRxwrzsI2yVmCtL5cUI4rZc,78
-spark_rapids_user_tools-23.6.1.dist-info/top_level.txt,sha256=47ZJrA6QPYYeI7JxABL1bTLJ7H9haiGWrN-6jVLYOXU,21
-spark_rapids_user_tools-23.6.1.dist-info/RECORD,,
+spark_rapids_pytools/wrappers/databricks_azure_wrapper.py,sha256=fd77N19GhREtG8P4rTQu4w64BB0on37b9iT5p6PPmEo,12960
+spark_rapids_pytools/wrappers/dataproc_wrapper.py,sha256=EXpizTdx6gve5kYY5vxAONITRehxhu3E_oooqUffvEY,15910
+spark_rapids_pytools/wrappers/emr_wrapper.py,sha256=kbhlIdfnNbur6voSG6X0rDxzeFB9AB11TQYT482K6lo,12086
+spark_rapids_pytools/wrappers/onprem_wrapper.py,sha256=DOWHGDKToGHMiu9uDfgjnRgY7wWuVZsffvjeSwp-lXw,9829
+spark_rapids_user_tools-23.6.2.dist-info/LICENSE,sha256=RnI8IUCDrXfGVHFfYTsT8OKEuaOtkMGDQOn8foh7D00,21086
+spark_rapids_user_tools-23.6.2.dist-info/METADATA,sha256=-zFTDwYLAfOTOE7oWSqPTLxIf7AoMRa38CN9ZwiLzJg,2927
+spark_rapids_user_tools-23.6.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spark_rapids_user_tools-23.6.2.dist-info/entry_points.txt,sha256=xiWYwYIymak3h07eV4KehH9gksbSubHnVFaKhfanJqk,128
+spark_rapids_user_tools-23.6.2.dist-info/top_level.txt,sha256=47ZJrA6QPYYeI7JxABL1bTLJ7H9haiGWrN-6jVLYOXU,21
+spark_rapids_user_tools-23.6.2.dist-info/RECORD,,
```

