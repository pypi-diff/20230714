# Comparing `tmp/azure-mgmt-paloaltonetworksngfw-1.0.0b1.zip` & `tmp/azure-mgmt-paloaltonetworksngfw-1.0.0b2.zip`

## zipinfo {}

```diff
@@ -1,73 +1,75 @@
-Zip file size: 182231 bytes, number of entries: 71
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/
--rw-rw-r--  2.0 unx     3200 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/PKG-INFO
--rw-rw-r--  2.0 unx       62 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx      226 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     2854 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/setup.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/LICENSE
--rw-rw-r--  2.0 unx     2223 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/README.md
--rw-rw-r--  2.0 unx       38 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/setup.cfg
--rw-rw-r--  2.0 unx      640 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/_meta.json
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/
--rw-rw-r--  2.0 unx       65 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/
--rw-rw-r--  2.0 unx       26 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/py.typed
--rw-rw-r--  2.0 unx     8419 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_palo_alto_networks_ngfw_mgmt_client.py
--rw-rw-r--  2.0 unx     1302 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_vendor.py
--rw-rw-r--  2.0 unx      488 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_version.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_patch.py
--rw-rw-r--  2.0 unx      933 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/__init__.py
--rw-rw-r--  2.0 unx    78836 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_serialization.py
--rw-rw-r--  2.0 unx     3535 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_configuration.py
--rw-rw-r--  2.0 unx    33768 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_local_rulestack_operations.py
--rw-rw-r--  2.0 unx    30118 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_global_rulestack_operations.py
--rw-rw-r--  2.0 unx    94726 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_local_rulestacks_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_patch.py
--rw-rw-r--  2.0 unx    41469 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_post_rules_operations.py
--rw-rw-r--  2.0 unx    29654 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_global_rulestack_operations.py
--rw-rw-r--  2.0 unx    47628 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_local_rules_operations.py
--rw-rw-r--  2.0 unx    73022 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_global_rulestack_operations.py
--rw-rw-r--  2.0 unx     2113 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/__init__.py
--rw-rw-r--  2.0 unx    29806 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_global_rulestack_operations.py
--rw-rw-r--  2.0 unx    63882 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_firewalls_operations.py
--rw-rw-r--  2.0 unx    33359 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_local_rulestack_operations.py
--rw-rw-r--  2.0 unx    41405 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_pre_rules_operations.py
--rw-rw-r--  2.0 unx    32907 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_local_rulestack_operations.py
--rw-rw-r--  2.0 unx     6504 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/
--rw-rw-r--  2.0 unx     8603 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_palo_alto_networks_ngfw_mgmt_client.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_patch.py
--rw-rw-r--  2.0 unx      880 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/__init__.py
--rw-rw-r--  2.0 unx     3583 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_configuration.py
--rw-rw-r--  2.0 unx    27997 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_local_rulestack_operations.py
--rw-rw-r--  2.0 unx    25805 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_global_rulestack_operations.py
--rw-rw-r--  2.0 unx    70608 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rulestacks_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    33105 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_post_rules_operations.py
--rw-rw-r--  2.0 unx    25399 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_global_rulestack_operations.py
--rw-rw-r--  2.0 unx    36661 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rules_operations.py
--rw-rw-r--  2.0 unx    57032 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_global_rulestack_operations.py
--rw-rw-r--  2.0 unx     2113 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    25518 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_global_rulestack_operations.py
--rw-rw-r--  2.0 unx    50257 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewalls_operations.py
--rw-rw-r--  2.0 unx    27591 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_local_rulestack_operations.py
--rw-rw-r--  2.0 unx    33047 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_pre_rules_operations.py
--rw-rw-r--  2.0 unx    27169 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_local_rulestack_operations.py
--rw-rw-r--  2.0 unx     5788 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     5216 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_palo_alto_networks_ngfw_mgmt_client_enums.py
--rw-rw-r--  2.0 unx   195860 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_models_py3.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_patch.py
--rw-rw-r--  2.0 unx     9156 b- defN 23-May-04 03:58 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/__init__.py
--rw-rw-r--  2.0 unx     3200 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx      124 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     3580 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-04 04:00 azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/dependency_links.txt
-71 files, 1346017 bytes uncompressed, 163547 bytes compressed:  87.8%
+Zip file size: 188826 bytes, number of entries: 73
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/
+-rw-rw-r--  2.0 unx     2223 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/setup.cfg
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/MANIFEST.in
+-rw-rw-r--  2.0 unx      640 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/_meta.json
+-rw-rw-r--  2.0 unx     3354 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx      216 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/LICENSE
+-rw-rw-r--  2.0 unx     2854 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/setup.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/py.typed
+-rw-rw-r--  2.0 unx    78836 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_serialization.py
+-rw-rw-r--  2.0 unx     8782 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_palo_alto_networks_ngfw_mgmt_client.py
+-rw-rw-r--  2.0 unx     3539 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_version.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_patch.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_vendor.py
+-rw-rw-r--  2.0 unx    41445 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_pre_rules_operations.py
+-rw-rw-r--  2.0 unx    29686 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx    30159 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx    63958 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_firewalls_operations.py
+-rw-rw-r--  2.0 unx    33391 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_local_rulestack_operations.py
+-rw-rw-r--  2.0 unx    29838 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx    12133 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_firewall_status_operations.py
+-rw-rw-r--  2.0 unx    41536 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_post_rules_operations.py
+-rw-rw-r--  2.0 unx    73176 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx    32975 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_local_rulestack_operations.py
+-rw-rw-r--  2.0 unx    33800 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_local_rulestack_operations.py
+-rw-rw-r--  2.0 unx    47704 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_local_rules_operations.py
+-rw-rw-r--  2.0 unx    94888 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_local_rulestacks_operations.py
+-rw-rw-r--  2.0 unx     2211 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_patch.py
+-rw-rw-r--  2.0 unx     6512 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_operations.py
+-rw-rw-r--  2.0 unx   202545 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_models_py3.py
+-rw-rw-r--  2.0 unx     5808 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_palo_alto_networks_ngfw_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx     9687 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/
+-rw-rw-r--  2.0 unx     8985 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_palo_alto_networks_ngfw_mgmt_client.py
+-rw-rw-r--  2.0 unx     3587 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_configuration.py
+-rw-rw-r--  2.0 unx      880 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_patch.py
+-rw-rw-r--  2.0 unx    33087 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_pre_rules_operations.py
+-rw-rw-r--  2.0 unx    25431 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx    25846 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx    50333 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewalls_operations.py
+-rw-rw-r--  2.0 unx    27623 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_local_rulestack_operations.py
+-rw-rw-r--  2.0 unx    25550 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx     9428 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewall_status_operations.py
+-rw-rw-r--  2.0 unx    33145 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_post_rules_operations.py
+-rw-rw-r--  2.0 unx    57120 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_global_rulestack_operations.py
+-rw-rw-r--  2.0 unx    27201 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_local_rulestack_operations.py
+-rw-rw-r--  2.0 unx    28029 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_local_rulestack_operations.py
+-rw-rw-r--  2.0 unx    36701 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rules_operations.py
+-rw-rw-r--  2.0 unx    70704 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rulestacks_operations.py
+-rw-rw-r--  2.0 unx     2211 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     5805 b- defN 23-May-05 06:19 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     3732 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx     3354 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx      124 b- defN 23-May-05 06:20 azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/requires.txt
+73 files, 1378367 bytes uncompressed, 169530 bytes compressed:  87.7%
```

## zipnote {}

```diff
@@ -1,214 +1,220 @@
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/PKG-INFO
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/README.md
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/CHANGELOG.md
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/MANIFEST.in
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/setup.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/_meta.json
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/LICENSE
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/README.md
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/setup.cfg
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/LICENSE
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/_meta.json
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/setup.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/__init__.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/__init__.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/py.typed
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/py.typed
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_palo_alto_networks_ngfw_mgmt_client.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_vendor.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_palo_alto_networks_ngfw_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_version.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_patch.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_version.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/__init__.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/__init__.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_serialization.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_patch.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_configuration.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_local_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_pre_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_local_rulestacks_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_patch.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_firewalls_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_post_rules_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_local_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_local_rules_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_firewall_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_post_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/__init__.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_local_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_firewalls_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_local_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_local_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_local_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_pre_rules_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_local_rulestacks_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_local_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_palo_alto_networks_ngfw_mgmt_client.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_patch.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_palo_alto_networks_ngfw_mgmt_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/__init__.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_configuration.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_local_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_palo_alto_networks_ngfw_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rulestacks_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_patch.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_post_rules_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_pre_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rules_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/__init__.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewalls_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_global_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_local_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewalls_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_local_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewall_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_pre_rules_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_post_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_local_rulestack_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_global_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_operations.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_local_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_palo_alto_networks_ngfw_mgmt_client_enums.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_local_rulestack_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_models_py3.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_patch.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rulestacks_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/__init__.py
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/PKG-INFO
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/requires.txt
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/not-zip-safe
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/top_level.txt
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/SOURCES.txt
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/dependency_links.txt
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/PKG-INFO
+Comment: 
+
+Filename: azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/requires.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/PKG-INFO` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-paloaltonetworksngfw
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Microsoft Azure Paloaltonetworksngfw Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -85,10 +85,20 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-paloaltonetworksngfw%2FREADME.png)
 
 
 # Release History
 
+## 1.0.0b2 (2023-05-05)
+
+### Features Added
+
+  - Added operation group FirewallStatusOperations
+
+### Other Changes
+
+  - Fixed annotation about namespace
+
 ## 1.0.0b1 (2023-05-04)
 
 * Initial Release
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/setup.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/LICENSE` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/README.md` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/_meta.json` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/_meta.json`

 * *Files 27% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/paloaltonetworks/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.4.8 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'b2fe1573f29f056930d79b1b8abf2611b98fa81a'",*

 * * "'use'":  […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/paloaltonetworks/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.6 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "2bd9b148ec4232e878641ccbb2bdde671e575add",
+    "autorest_command": "autorest specification/paloaltonetworks/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.8 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "b2fe1573f29f056930d79b1b8abf2611b98fa81a",
     "readme": "specification/paloaltonetworks/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.4.6",
+        "@autorest/python@6.4.8",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_palo_alto_networks_ngfw_mgmt_client.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_palo_alto_networks_ngfw_mgmt_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, TYPE_CHECKING
+from typing import Any, Awaitable, TYPE_CHECKING
 
-from azure.core.rest import HttpRequest, HttpResponse
-from azure.mgmt.core import ARMPipelineClient
+from azure.core.rest import AsyncHttpResponse, HttpRequest
+from azure.mgmt.core import AsyncARMPipelineClient
 
-from . import models as _models
+from .. import models as _models
+from .._serialization import Deserializer, Serializer
 from ._configuration import PaloAltoNetworksNgfwMgmtClientConfiguration
-from ._serialization import Deserializer, Serializer
 from .operations import (
     CertificateObjectGlobalRulestackOperations,
     CertificateObjectLocalRulestackOperations,
+    FirewallStatusOperations,
     FirewallsOperations,
     FqdnListGlobalRulestackOperations,
     FqdnListLocalRulestackOperations,
     GlobalRulestackOperations,
     LocalRulesOperations,
     LocalRulestacksOperations,
     Operations,
@@ -29,77 +30,82 @@
     PreRulesOperations,
     PrefixListGlobalRulestackOperations,
     PrefixListLocalRulestackOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class PaloAltoNetworksNgfwMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """PaloAltoNetworksNgfwMgmtClient.
 
     :ivar global_rulestack: GlobalRulestackOperations operations
-    :vartype global_rulestack: azure.mgmt.paloaltonetworks.operations.GlobalRulestackOperations
+    :vartype global_rulestack:
+     azure.mgmt.paloaltonetworksngfw.aio.operations.GlobalRulestackOperations
     :ivar certificate_object_global_rulestack: CertificateObjectGlobalRulestackOperations
      operations
     :vartype certificate_object_global_rulestack:
-     azure.mgmt.paloaltonetworks.operations.CertificateObjectGlobalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.aio.operations.CertificateObjectGlobalRulestackOperations
     :ivar fqdn_list_global_rulestack: FqdnListGlobalRulestackOperations operations
     :vartype fqdn_list_global_rulestack:
-     azure.mgmt.paloaltonetworks.operations.FqdnListGlobalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.aio.operations.FqdnListGlobalRulestackOperations
     :ivar post_rules: PostRulesOperations operations
-    :vartype post_rules: azure.mgmt.paloaltonetworks.operations.PostRulesOperations
+    :vartype post_rules: azure.mgmt.paloaltonetworksngfw.aio.operations.PostRulesOperations
     :ivar prefix_list_global_rulestack: PrefixListGlobalRulestackOperations operations
     :vartype prefix_list_global_rulestack:
-     azure.mgmt.paloaltonetworks.operations.PrefixListGlobalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.aio.operations.PrefixListGlobalRulestackOperations
     :ivar pre_rules: PreRulesOperations operations
-    :vartype pre_rules: azure.mgmt.paloaltonetworks.operations.PreRulesOperations
+    :vartype pre_rules: azure.mgmt.paloaltonetworksngfw.aio.operations.PreRulesOperations
     :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.paloaltonetworks.operations.Operations
+    :vartype operations: azure.mgmt.paloaltonetworksngfw.aio.operations.Operations
     :ivar firewalls: FirewallsOperations operations
-    :vartype firewalls: azure.mgmt.paloaltonetworks.operations.FirewallsOperations
+    :vartype firewalls: azure.mgmt.paloaltonetworksngfw.aio.operations.FirewallsOperations
     :ivar local_rulestacks: LocalRulestacksOperations operations
-    :vartype local_rulestacks: azure.mgmt.paloaltonetworks.operations.LocalRulestacksOperations
+    :vartype local_rulestacks:
+     azure.mgmt.paloaltonetworksngfw.aio.operations.LocalRulestacksOperations
+    :ivar firewall_status: FirewallStatusOperations operations
+    :vartype firewall_status:
+     azure.mgmt.paloaltonetworksngfw.aio.operations.FirewallStatusOperations
     :ivar certificate_object_local_rulestack: CertificateObjectLocalRulestackOperations operations
     :vartype certificate_object_local_rulestack:
-     azure.mgmt.paloaltonetworks.operations.CertificateObjectLocalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.aio.operations.CertificateObjectLocalRulestackOperations
     :ivar fqdn_list_local_rulestack: FqdnListLocalRulestackOperations operations
     :vartype fqdn_list_local_rulestack:
-     azure.mgmt.paloaltonetworks.operations.FqdnListLocalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.aio.operations.FqdnListLocalRulestackOperations
     :ivar local_rules: LocalRulesOperations operations
-    :vartype local_rules: azure.mgmt.paloaltonetworks.operations.LocalRulesOperations
+    :vartype local_rules: azure.mgmt.paloaltonetworksngfw.aio.operations.LocalRulesOperations
     :ivar prefix_list_local_rulestack: PrefixListLocalRulestackOperations operations
     :vartype prefix_list_local_rulestack:
-     azure.mgmt.paloaltonetworks.operations.PrefixListLocalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.aio.operations.PrefixListLocalRulestackOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
     :keyword api_version: Api Version. Default value is "2022-08-29-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
-        credential: "TokenCredential",
+        credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = PaloAltoNetworksNgfwMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.global_rulestack = GlobalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -116,49 +122,50 @@
         )
         self.pre_rules = PreRulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.firewalls = FirewallsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.local_rulestacks = LocalRulestacksOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.firewall_status = FirewallStatusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.certificate_object_local_rulestack = CertificateObjectLocalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.fqdn_list_local_rulestack = FqdnListLocalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.local_rules = LocalRulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.prefix_list_local_rulestack = PrefixListLocalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = client._send_request(request)
-        <HttpResponse: 200 OK>
+        >>> response = await client._send_request(request)
+        <AsyncHttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.HttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self) -> None:
-        self._client.close()
+    async def close(self) -> None:
+        await self._client.close()
 
-    def __enter__(self) -> "PaloAltoNetworksNgfwMgmtClient":
-        self._client.__enter__()
+    async def __aenter__(self) -> "PaloAltoNetworksNgfwMgmtClient":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details: Any) -> None:
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details: Any) -> None:
+        await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_vendor.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_patch.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/__init__.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_serialization.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/_configuration.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
-        kwargs.setdefault("sdk_moniker", "mgmt-paloaltonetworks/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "mgmt-paloaltonetworksngfw/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_local_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_local_rulestack_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
 class CertificateObjectLocalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`certificate_object_local_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -206,15 +206,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either CertificateObjectLocalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateObjectLocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -300,15 +300,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CertificateObjectLocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -448,30 +448,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either CertificateObjectLocalRulestackResource
          or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -503,15 +503,15 @@
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either CertificateObjectLocalRulestackResource
          or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -527,31 +527,31 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a
          CertificateObjectLocalRulestackResource type or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource or
-         IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource
+         or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either CertificateObjectLocalRulestackResource
          or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_global_rulestack_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 class CertificateObjectGlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`certificate_object_global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -178,15 +178,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either CertificateObjectGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateObjectGlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -265,15 +265,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CertificateObjectGlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -404,30 +404,31 @@
         """Create a CertificateObjectGlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource
+        :type resource:
+         ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either CertificateObjectGlobalRulestackResource
          or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -455,15 +456,15 @@
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either CertificateObjectGlobalRulestackResource
          or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -475,31 +476,31 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a
          CertificateObjectGlobalRulestackResource type or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource or
-         IO
+        :type resource:
+         ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either CertificateObjectGlobalRulestackResource
          or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_local_rulestacks_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_local_rulestacks_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_advanced_security_objects_request(
+def build_list_advanced_security_objects_request(  # pylint: disable=name-too-long
     resource_group_name: str,
     local_rulestack_name: str,
     subscription_id: str,
     *,
     type: Union[str, _models.AdvSecurityObjectTypeEnum],
     skip: Optional[str] = None,
     top: Optional[int] = None,
@@ -504,15 +504,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_predefined_url_categories_request(
+def build_list_predefined_url_categories_request(  # pylint: disable=name-too-long
     resource_group_name: str,
     local_rulestack_name: str,
     subscription_id: str,
     *,
     skip: Optional[str] = None,
     top: Optional[int] = None,
     **kwargs: Any
@@ -631,15 +631,15 @@
 
 class LocalRulestacksOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`local_rulestacks` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -652,15 +652,15 @@
     def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.LocalRulestackResource"]:
         """List LocalRulestackResource resources by subscription ID.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either LocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.LocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -742,15 +742,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either LocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.LocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -831,15 +831,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -973,30 +973,30 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either LocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -1025,15 +1025,15 @@
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either LocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -1046,30 +1046,30 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param resource: Resource create parameters. Is either a LocalRulestackResource type or a IO
          type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either LocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -1132,21 +1132,21 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param properties: The resource properties to be updated. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResourceUpdate
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResourceUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         resource_group_name: str,
@@ -1166,15 +1166,15 @@
         :param properties: The resource properties to be updated. Required.
         :type properties: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         resource_group_name: str,
@@ -1187,21 +1187,21 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param properties: The resource properties to be updated. Is either a
          LocalRulestackResourceUpdate type or a IO type. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResourceUpdate or IO
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResourceUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1496,15 +1496,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Changelog or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.Changelog
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.Changelog
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1563,15 +1563,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param email: email address on behalf of which this API called. Default value is None.
         :type email: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SupportInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SupportInfo
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SupportInfo
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1634,22 +1634,22 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param type: Known values are: "urlCustom" and "feeds". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AdvSecurityObjectListResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectListResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectListResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1724,15 +1724,15 @@
         :type app_prefix: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListAppIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListAppIdResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListAppIdResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1802,15 +1802,15 @@
         :type local_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CountriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CountriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CountriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1869,15 +1869,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListFirewallsResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListFirewallsResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListFirewallsResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1943,15 +1943,15 @@
         :type local_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PredefinedUrlCategoriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PredefinedUrlCategoriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PredefinedUrlCategoriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -2016,22 +2016,22 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param type: Known values are: "antiSpyware", "antiVirus", "ipsVulnerability", "urlFiltering",
          "fileBlocking", and "dnsSubscription". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.SecurityServicesTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SecurityServicesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SecurityServicesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_patch.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_post_rules_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_post_rules_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
 class PostRulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`post_rules` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -270,15 +270,15 @@
     def list(self, global_rulestack_name: str, **kwargs: Any) -> Iterable["_models.PostRulesResource"]:
         """List PostRulesResource resources by Tenant.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PostRulesResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PostRulesResourceListResult] = kwargs.pop("cls", None)
@@ -355,15 +355,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PostRulesResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PostRulesResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -490,29 +490,30 @@
         """Create a PostRulesResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PostRulesResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PostRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -539,15 +540,16 @@
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PostRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self, global_rulestack_name: str, priority: str, resource: Union[_models.PostRulesResource, IO], **kwargs: Any
     ) -> LROPoller[_models.PostRulesResource]:
@@ -555,29 +557,30 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Is either a PostRulesResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PostRulesResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PostRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -748,15 +751,15 @@
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounter or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounter
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounter
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -876,15 +879,15 @@
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounterReset or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounterReset
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounterReset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_global_rulestack_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
 class FqdnListGlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`fqdn_list_global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -173,15 +173,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FqdnListGlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FqdnListGlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -258,15 +258,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FqdnListGlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -397,30 +397,30 @@
         """Create a FqdnListGlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FqdnListGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -448,15 +448,15 @@
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FqdnListGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -468,30 +468,30 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a FqdnListGlobalRulestackResource type
          or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FqdnListGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_local_rules_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_local_rules_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 
 class LocalRulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`local_rules` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -330,15 +330,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either LocalRulesResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.LocalRulesResourceListResult] = kwargs.pop("cls", None)
@@ -424,15 +425,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulesResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulesResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -572,29 +573,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulesResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either LocalRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -625,15 +627,16 @@
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either LocalRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -649,29 +652,30 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Is either a LocalRulesResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulesResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either LocalRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -859,15 +863,15 @@
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounter or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounter
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounter
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1007,15 +1011,15 @@
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounterReset or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounterReset
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounterReset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_global_rulestack_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_advanced_security_objects_request(
+def build_list_advanced_security_objects_request(  # pylint: disable=name-too-long
     global_rulestack_name: str,
     *,
     type: Union[str, _models.AdvSecurityObjectTypeEnum],
     skip: Optional[str] = None,
     top: Optional[int] = None,
     **kwargs: Any
 ) -> HttpRequest:
@@ -346,15 +346,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_predefined_url_categories_request(
+def build_list_predefined_url_categories_request(  # pylint: disable=name-too-long
     global_rulestack_name: str, *, skip: Optional[str] = None, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-08-29-preview"))
     accept = _headers.pop("Accept", "application/json")
@@ -450,15 +450,15 @@
 
 class GlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -471,15 +471,15 @@
     def list(self, **kwargs: Any) -> Iterable["_models.GlobalRulestackResource"]:
         """List GlobalRulestackResource resources by Tenant.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either GlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.GlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -553,15 +553,15 @@
     def get(self, global_rulestack_name: str, **kwargs: Any) -> _models.GlobalRulestackResource:
         """Get a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -681,30 +681,30 @@
         **kwargs: Any
     ) -> LROPoller[_models.GlobalRulestackResource]:
         """Create a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either GlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self, global_rulestack_name: str, resource: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> LROPoller[_models.GlobalRulestackResource]:
@@ -724,44 +724,44 @@
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either GlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self, global_rulestack_name: str, resource: Union[_models.GlobalRulestackResource, IO], **kwargs: Any
     ) -> LROPoller[_models.GlobalRulestackResource]:
         """Create a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param resource: Resource create parameters. Is either a GlobalRulestackResource type or a IO
          type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either GlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -819,21 +819,21 @@
         **kwargs: Any
     ) -> _models.GlobalRulestackResource:
         """Update a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param properties: The resource properties to be updated. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResourceUpdate
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResourceUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self, global_rulestack_name: str, properties: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.GlobalRulestackResource:
@@ -844,35 +844,35 @@
         :param properties: The resource properties to be updated. Required.
         :type properties: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self, global_rulestack_name: str, properties: Union[_models.GlobalRulestackResourceUpdate, IO], **kwargs: Any
     ) -> _models.GlobalRulestackResource:
         """Update a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param properties: The resource properties to be updated. Is either a
          GlobalRulestackResourceUpdate type or a IO type. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResourceUpdate or IO
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResourceUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1144,15 +1144,15 @@
     def get_change_log(self, global_rulestack_name: str, **kwargs: Any) -> _models.Changelog:
         """Get changelog.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Changelog or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.Changelog
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.Changelog
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1208,22 +1208,22 @@
         **kwargs: Any
     ) -> _models.AdvSecurityObjectListResponse:
         """Get the list of advanced security objects.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param type: Known values are: "urlCustom" and "feeds". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AdvSecurityObjectListResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectListResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectListResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1292,15 +1292,15 @@
         :type app_prefix: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListAppIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListAppIdResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListAppIdResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1360,15 +1360,15 @@
         :type global_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CountriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CountriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CountriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1420,15 +1420,15 @@
     def list_firewalls(self, global_rulestack_name: str, **kwargs: Any) -> _models.ListFirewallsResponse:
         """List of Firewalls associated with Rulestack.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListFirewallsResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListFirewallsResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListFirewallsResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1484,15 +1484,15 @@
         :type global_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PredefinedUrlCategoriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PredefinedUrlCategoriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PredefinedUrlCategoriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1551,22 +1551,22 @@
     ) -> _models.SecurityServicesResponse:
         """List the security services for rulestack.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param type: Known values are: "antiSpyware", "antiVirus", "ipsVulnerability", "urlFiltering",
          "fileBlocking", and "dnsSubscription". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.SecurityServicesTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SecurityServicesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SecurityServicesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/__init__.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ._fqdn_list_global_rulestack_operations import FqdnListGlobalRulestackOperations
 from ._post_rules_operations import PostRulesOperations
 from ._prefix_list_global_rulestack_operations import PrefixListGlobalRulestackOperations
 from ._pre_rules_operations import PreRulesOperations
 from ._operations import Operations
 from ._firewalls_operations import FirewallsOperations
 from ._local_rulestacks_operations import LocalRulestacksOperations
+from ._firewall_status_operations import FirewallStatusOperations
 from ._certificate_object_local_rulestack_operations import CertificateObjectLocalRulestackOperations
 from ._fqdn_list_local_rulestack_operations import FqdnListLocalRulestackOperations
 from ._local_rules_operations import LocalRulesOperations
 from ._prefix_list_local_rulestack_operations import PrefixListLocalRulestackOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
@@ -30,14 +31,15 @@
     "FqdnListGlobalRulestackOperations",
     "PostRulesOperations",
     "PrefixListGlobalRulestackOperations",
     "PreRulesOperations",
     "Operations",
     "FirewallsOperations",
     "LocalRulestacksOperations",
+    "FirewallStatusOperations",
     "CertificateObjectLocalRulestackOperations",
     "FqdnListLocalRulestackOperations",
     "LocalRulesOperations",
     "PrefixListLocalRulestackOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_global_rulestack_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 class PrefixListGlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`prefix_list_global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -176,15 +176,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrefixListGlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrefixListGlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -261,15 +261,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrefixListGlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -400,30 +400,30 @@
         """Create a PrefixListGlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrefixListGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -451,15 +451,15 @@
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrefixListGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -471,30 +471,30 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a PrefixListGlobalRulestackResource type
          or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrefixListGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_firewalls_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_firewalls_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
 class FirewallsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`firewalls` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -386,15 +386,15 @@
 
     @distributed_trace
     def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.FirewallResource"]:
         """List FirewallResource resources by subscription ID.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FirewallResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FirewallResourceListResult] = kwargs.pop("cls", None)
@@ -472,15 +472,15 @@
         """List FirewallResource resources by resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FirewallResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FirewallResourceListResult] = kwargs.pop("cls", None)
@@ -561,15 +561,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -699,29 +699,29 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FirewallResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -749,15 +749,15 @@
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FirewallResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self, resource_group_name: str, firewall_name: str, resource: Union[_models.FirewallResource, IO], **kwargs: Any
     ) -> LROPoller[_models.FirewallResource]:
@@ -766,29 +766,29 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param resource: Resource create parameters. Is either a FirewallResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FirewallResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FirewallResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -851,21 +851,21 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param properties: The resource properties to be updated. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.FirewallResourceUpdate
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResourceUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         resource_group_name: str,
@@ -885,15 +885,15 @@
         :param properties: The resource properties to be updated. Required.
         :type properties: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         resource_group_name: str,
@@ -906,21 +906,21 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param properties: The resource properties to be updated. Is either a FirewallResourceUpdate
          type or a IO type. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.FirewallResourceUpdate or IO
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResourceUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1103,15 +1103,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackInfo
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackInfo
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1166,15 +1166,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LogSettings or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LogSettings
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LogSettings
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1233,15 +1233,15 @@
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param email: email address on behalf of which this API called. Default value is None.
         :type email: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SupportInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SupportInfo
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SupportInfo
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1304,15 +1304,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param log_settings: Default value is None.
-        :type log_settings: ~azure.mgmt.paloaltonetworks.models.LogSettings
+        :type log_settings: ~azure.mgmt.paloaltonetworksngfw.models.LogSettings
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1358,15 +1358,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param log_settings: Is either a LogSettings type or a IO type. Default value is None.
-        :type log_settings: ~azure.mgmt.paloaltonetworks.models.LogSettings or IO
+        :type log_settings: ~azure.mgmt.paloaltonetworksngfw.models.LogSettings or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_local_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_local_rulestack_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
 class FqdnListLocalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`fqdn_list_local_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -206,15 +206,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FqdnListLocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FqdnListLocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -300,15 +300,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FqdnListLocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -448,30 +448,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FqdnListLocalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -503,15 +503,15 @@
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FqdnListLocalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -527,30 +527,30 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a FqdnListLocalRulestackResource type or
          a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either FqdnListLocalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_pre_rules_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_pre_rules_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
 class PreRulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`pre_rules` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -270,15 +270,15 @@
     def list(self, global_rulestack_name: str, **kwargs: Any) -> Iterable["_models.PreRulesResource"]:
         """List PreRulesResource resources by Tenant.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PreRulesResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PreRulesResourceListResult] = kwargs.pop("cls", None)
@@ -355,15 +355,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PreRulesResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PreRulesResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -490,29 +490,29 @@
         """Create a PreRulesResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PreRulesResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PreRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -539,15 +539,15 @@
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PreRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self, global_rulestack_name: str, priority: str, resource: Union[_models.PreRulesResource, IO], **kwargs: Any
     ) -> LROPoller[_models.PreRulesResource]:
@@ -555,29 +555,29 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Is either a PreRulesResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PreRulesResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PreRulesResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -748,15 +748,15 @@
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounter or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounter
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounter
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -876,15 +876,15 @@
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounterReset or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounterReset
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounterReset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_local_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_prefix_list_local_rulestack_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
 class PrefixListLocalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`prefix_list_local_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -204,15 +204,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrefixListResource or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrefixListResourceListResult] = kwargs.pop("cls", None)
@@ -298,15 +299,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrefixListResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PrefixListResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -446,29 +447,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrefixListResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -499,15 +501,16 @@
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrefixListResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -523,29 +526,30 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a PrefixListResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrefixListResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/operations/_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -76,15 +76,15 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
         """List the operations for the provider.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworks.models.Operation]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.paloaltonetworksngfw.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_palo_alto_networks_ngfw_mgmt_client.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/_palo_alto_networks_ngfw_mgmt_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, Awaitable, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING
 
-from azure.core.rest import AsyncHttpResponse, HttpRequest
-from azure.mgmt.core import AsyncARMPipelineClient
+from azure.core.rest import HttpRequest, HttpResponse
+from azure.mgmt.core import ARMPipelineClient
 
-from .. import models as _models
-from .._serialization import Deserializer, Serializer
+from . import models as _models
 from ._configuration import PaloAltoNetworksNgfwMgmtClientConfiguration
+from ._serialization import Deserializer, Serializer
 from .operations import (
     CertificateObjectGlobalRulestackOperations,
     CertificateObjectLocalRulestackOperations,
+    FirewallStatusOperations,
     FirewallsOperations,
     FqdnListGlobalRulestackOperations,
     FqdnListLocalRulestackOperations,
     GlobalRulestackOperations,
     LocalRulesOperations,
     LocalRulestacksOperations,
     Operations,
@@ -29,77 +30,79 @@
     PreRulesOperations,
     PrefixListGlobalRulestackOperations,
     PrefixListLocalRulestackOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class PaloAltoNetworksNgfwMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """PaloAltoNetworksNgfwMgmtClient.
 
     :ivar global_rulestack: GlobalRulestackOperations operations
-    :vartype global_rulestack: azure.mgmt.paloaltonetworks.aio.operations.GlobalRulestackOperations
+    :vartype global_rulestack: azure.mgmt.paloaltonetworksngfw.operations.GlobalRulestackOperations
     :ivar certificate_object_global_rulestack: CertificateObjectGlobalRulestackOperations
      operations
     :vartype certificate_object_global_rulestack:
-     azure.mgmt.paloaltonetworks.aio.operations.CertificateObjectGlobalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.operations.CertificateObjectGlobalRulestackOperations
     :ivar fqdn_list_global_rulestack: FqdnListGlobalRulestackOperations operations
     :vartype fqdn_list_global_rulestack:
-     azure.mgmt.paloaltonetworks.aio.operations.FqdnListGlobalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.operations.FqdnListGlobalRulestackOperations
     :ivar post_rules: PostRulesOperations operations
-    :vartype post_rules: azure.mgmt.paloaltonetworks.aio.operations.PostRulesOperations
+    :vartype post_rules: azure.mgmt.paloaltonetworksngfw.operations.PostRulesOperations
     :ivar prefix_list_global_rulestack: PrefixListGlobalRulestackOperations operations
     :vartype prefix_list_global_rulestack:
-     azure.mgmt.paloaltonetworks.aio.operations.PrefixListGlobalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.operations.PrefixListGlobalRulestackOperations
     :ivar pre_rules: PreRulesOperations operations
-    :vartype pre_rules: azure.mgmt.paloaltonetworks.aio.operations.PreRulesOperations
+    :vartype pre_rules: azure.mgmt.paloaltonetworksngfw.operations.PreRulesOperations
     :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.paloaltonetworks.aio.operations.Operations
+    :vartype operations: azure.mgmt.paloaltonetworksngfw.operations.Operations
     :ivar firewalls: FirewallsOperations operations
-    :vartype firewalls: azure.mgmt.paloaltonetworks.aio.operations.FirewallsOperations
+    :vartype firewalls: azure.mgmt.paloaltonetworksngfw.operations.FirewallsOperations
     :ivar local_rulestacks: LocalRulestacksOperations operations
-    :vartype local_rulestacks: azure.mgmt.paloaltonetworks.aio.operations.LocalRulestacksOperations
+    :vartype local_rulestacks: azure.mgmt.paloaltonetworksngfw.operations.LocalRulestacksOperations
+    :ivar firewall_status: FirewallStatusOperations operations
+    :vartype firewall_status: azure.mgmt.paloaltonetworksngfw.operations.FirewallStatusOperations
     :ivar certificate_object_local_rulestack: CertificateObjectLocalRulestackOperations operations
     :vartype certificate_object_local_rulestack:
-     azure.mgmt.paloaltonetworks.aio.operations.CertificateObjectLocalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.operations.CertificateObjectLocalRulestackOperations
     :ivar fqdn_list_local_rulestack: FqdnListLocalRulestackOperations operations
     :vartype fqdn_list_local_rulestack:
-     azure.mgmt.paloaltonetworks.aio.operations.FqdnListLocalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.operations.FqdnListLocalRulestackOperations
     :ivar local_rules: LocalRulesOperations operations
-    :vartype local_rules: azure.mgmt.paloaltonetworks.aio.operations.LocalRulesOperations
+    :vartype local_rules: azure.mgmt.paloaltonetworksngfw.operations.LocalRulesOperations
     :ivar prefix_list_local_rulestack: PrefixListLocalRulestackOperations operations
     :vartype prefix_list_local_rulestack:
-     azure.mgmt.paloaltonetworks.aio.operations.PrefixListLocalRulestackOperations
+     azure.mgmt.paloaltonetworksngfw.operations.PrefixListLocalRulestackOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
     :keyword api_version: Api Version. Default value is "2022-08-29-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
-        credential: "AsyncTokenCredential",
+        credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = PaloAltoNetworksNgfwMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.global_rulestack = GlobalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -116,49 +119,50 @@
         )
         self.pre_rules = PreRulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.firewalls = FirewallsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.local_rulestacks = LocalRulestacksOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.firewall_status = FirewallStatusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.certificate_object_local_rulestack = CertificateObjectLocalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.fqdn_list_local_rulestack = FqdnListLocalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.local_rules = LocalRulesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.prefix_list_local_rulestack = PrefixListLocalRulestackOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = await client._send_request(request)
-        <AsyncHttpResponse: 200 OK>
+        >>> response = client._send_request(request)
+        <HttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.AsyncHttpResponse
+        :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
-    async def close(self) -> None:
-        await self._client.close()
+    def close(self) -> None:
+        self._client.close()
 
-    async def __aenter__(self) -> "PaloAltoNetworksNgfwMgmtClient":
-        await self._client.__aenter__()
+    def __enter__(self) -> "PaloAltoNetworksNgfwMgmtClient":
+        self._client.__enter__()
         return self
 
-    async def __aexit__(self, *exc_details: Any) -> None:
-        await self._client.__aexit__(*exc_details)
+    def __exit__(self, *exc_details: Any) -> None:
+        self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_patch.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/__init__.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/_configuration.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
-        kwargs.setdefault("sdk_moniker", "mgmt-paloaltonetworks/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "mgmt-paloaltonetworksngfw/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_local_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_local_rulestack_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class CertificateObjectLocalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`certificate_object_local_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -71,15 +71,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either CertificateObjectLocalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateObjectLocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -165,15 +165,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CertificateObjectLocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -313,30 +313,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either
          CertificateObjectLocalRulestackResource or the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -368,15 +368,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either
          CertificateObjectLocalRulestackResource or the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -392,31 +392,31 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a
          CertificateObjectLocalRulestackResource type or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource or
-         IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource
+         or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either
          CertificateObjectLocalRulestackResource or the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_global_rulestack_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class CertificateObjectGlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`certificate_object_global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -68,15 +68,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either CertificateObjectGlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CertificateObjectGlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -155,15 +155,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CertificateObjectGlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -294,30 +294,31 @@
         """Create a CertificateObjectGlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource
+        :type resource:
+         ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either
          CertificateObjectGlobalRulestackResource or the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -345,15 +346,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either
          CertificateObjectGlobalRulestackResource or the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -365,31 +366,31 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: certificate name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a
          CertificateObjectGlobalRulestackResource type or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource or
-         IO
+        :type resource:
+         ~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either
          CertificateObjectGlobalRulestackResource or the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rulestacks_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rulestacks_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 class LocalRulestacksOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`local_rulestacks` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -76,15 +76,15 @@
     def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.LocalRulestackResource"]:
         """List LocalRulestackResource resources by subscription ID.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either LocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.LocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -166,15 +166,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either LocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.LocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -257,15 +257,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -399,30 +399,30 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either LocalRulestackResource or the result
          of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -451,15 +451,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either LocalRulestackResource or the result
          of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -472,30 +472,30 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param resource: Resource create parameters. Is either a LocalRulestackResource type or a IO
          type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either LocalRulestackResource or the result
          of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -559,21 +559,21 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param properties: The resource properties to be updated. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResourceUpdate
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResourceUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update(
         self,
         resource_group_name: str,
@@ -593,15 +593,15 @@
         :param properties: The resource properties to be updated. Required.
         :type properties: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update(
         self,
         resource_group_name: str,
@@ -614,21 +614,21 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param properties: The resource properties to be updated. Is either a
          LocalRulestackResourceUpdate type or a IO type. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResourceUpdate or IO
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResourceUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -930,15 +930,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Changelog or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.Changelog
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.Changelog
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -997,15 +997,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param email: email address on behalf of which this API called. Default value is None.
         :type email: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SupportInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SupportInfo
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SupportInfo
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1068,22 +1068,22 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param type: Known values are: "urlCustom" and "feeds". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AdvSecurityObjectListResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectListResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectListResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1158,15 +1158,15 @@
         :type app_prefix: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListAppIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListAppIdResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListAppIdResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1236,15 +1236,15 @@
         :type local_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CountriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CountriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CountriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1303,15 +1303,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListFirewallsResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListFirewallsResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListFirewallsResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1377,15 +1377,15 @@
         :type local_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PredefinedUrlCategoriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PredefinedUrlCategoriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PredefinedUrlCategoriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1450,22 +1450,22 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param type: Known values are: "antiSpyware", "antiVirus", "ipsVulnerability", "urlFiltering",
          "fileBlocking", and "dnsSubscription". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.SecurityServicesTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SecurityServicesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SecurityServicesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_patch.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_post_rules_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_post_rules_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 class PostRulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`post_rules` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -68,15 +68,15 @@
         """List PostRulesResource resources by Tenant.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PostRulesResource or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PostRulesResourceListResult] = kwargs.pop("cls", None)
@@ -153,15 +153,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PostRulesResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PostRulesResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -288,30 +288,30 @@
         """Create a PostRulesResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PostRulesResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PostRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -339,15 +339,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PostRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self, global_rulestack_name: str, priority: str, resource: Union[_models.PostRulesResource, IO], **kwargs: Any
     ) -> AsyncLROPoller[_models.PostRulesResource]:
@@ -355,30 +355,30 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Is either a PostRulesResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PostRulesResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PostRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -551,15 +551,15 @@
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounter or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounter
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounter
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -679,15 +679,15 @@
         :type global_rulestack_name: str
         :param priority: Post Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounterReset or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounterReset
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounterReset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_global_rulestack_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class FqdnListGlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`fqdn_list_global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -68,15 +68,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FqdnListGlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FqdnListGlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -155,15 +155,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FqdnListGlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -294,30 +294,30 @@
         """Create a FqdnListGlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FqdnListGlobalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -345,15 +345,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FqdnListGlobalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -365,30 +365,30 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a FqdnListGlobalRulestackResource type
          or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FqdnListGlobalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rules_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rules_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 class LocalRulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`local_rules` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -73,15 +73,15 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either LocalRulesResource or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.LocalRulesResourceListResult] = kwargs.pop("cls", None)
@@ -167,15 +167,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LocalRulesResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LocalRulesResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -315,30 +315,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulesResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either LocalRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -370,15 +370,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either LocalRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -394,30 +394,30 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Is either a LocalRulesResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.LocalRulesResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either LocalRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -607,15 +607,15 @@
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounter or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounter
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounter
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -755,15 +755,15 @@
         :type local_rulestack_name: str
         :param priority: Local Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounterReset or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounterReset
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounterReset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_global_rulestack_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 class GlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -74,15 +74,15 @@
     def list(self, **kwargs: Any) -> AsyncIterable["_models.GlobalRulestackResource"]:
         """List GlobalRulestackResource resources by Tenant.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either GlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.GlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -156,15 +156,15 @@
     async def get(self, global_rulestack_name: str, **kwargs: Any) -> _models.GlobalRulestackResource:
         """Get a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -284,30 +284,30 @@
         **kwargs: Any
     ) -> AsyncLROPoller[_models.GlobalRulestackResource]:
         """Create a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either GlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self, global_rulestack_name: str, resource: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> AsyncLROPoller[_models.GlobalRulestackResource]:
@@ -327,44 +327,44 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either GlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self, global_rulestack_name: str, resource: Union[_models.GlobalRulestackResource, IO], **kwargs: Any
     ) -> AsyncLROPoller[_models.GlobalRulestackResource]:
         """Create a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param resource: Resource create parameters. Is either a GlobalRulestackResource type or a IO
          type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either GlobalRulestackResource or the
          result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -423,21 +423,21 @@
         **kwargs: Any
     ) -> _models.GlobalRulestackResource:
         """Update a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param properties: The resource properties to be updated. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResourceUpdate
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResourceUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update(
         self, global_rulestack_name: str, properties: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.GlobalRulestackResource:
@@ -448,35 +448,35 @@
         :param properties: The resource properties to be updated. Required.
         :type properties: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update(
         self, global_rulestack_name: str, properties: Union[_models.GlobalRulestackResourceUpdate, IO], **kwargs: Any
     ) -> _models.GlobalRulestackResource:
         """Update a GlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param properties: The resource properties to be updated. Is either a
          GlobalRulestackResourceUpdate type or a IO type. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResourceUpdate or IO
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResourceUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -749,15 +749,15 @@
     async def get_change_log(self, global_rulestack_name: str, **kwargs: Any) -> _models.Changelog:
         """Get changelog.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Changelog or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.Changelog
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.Changelog
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -813,22 +813,22 @@
         **kwargs: Any
     ) -> _models.AdvSecurityObjectListResponse:
         """Get the list of advanced security objects.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param type: Known values are: "urlCustom" and "feeds". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AdvSecurityObjectListResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectListResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectListResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -897,15 +897,15 @@
         :type app_prefix: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListAppIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListAppIdResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListAppIdResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -965,15 +965,15 @@
         :type global_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CountriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.CountriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.CountriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1025,15 +1025,15 @@
     async def list_firewalls(self, global_rulestack_name: str, **kwargs: Any) -> _models.ListFirewallsResponse:
         """List of Firewalls associated with Rulestack.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ListFirewallsResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.ListFirewallsResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.ListFirewallsResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1089,15 +1089,15 @@
         :type global_rulestack_name: str
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PredefinedUrlCategoriesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PredefinedUrlCategoriesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PredefinedUrlCategoriesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1156,22 +1156,22 @@
     ) -> _models.SecurityServicesResponse:
         """List the security services for rulestack.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param type: Known values are: "antiSpyware", "antiVirus", "ipsVulnerability", "urlFiltering",
          "fileBlocking", and "dnsSubscription". Required.
-        :type type: str or ~azure.mgmt.paloaltonetworks.models.SecurityServicesTypeEnum
+        :type type: str or ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesTypeEnum
         :param skip: Default value is None.
         :type skip: str
         :param top: Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SecurityServicesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SecurityServicesResponse
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/__init__.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ._fqdn_list_global_rulestack_operations import FqdnListGlobalRulestackOperations
 from ._post_rules_operations import PostRulesOperations
 from ._prefix_list_global_rulestack_operations import PrefixListGlobalRulestackOperations
 from ._pre_rules_operations import PreRulesOperations
 from ._operations import Operations
 from ._firewalls_operations import FirewallsOperations
 from ._local_rulestacks_operations import LocalRulestacksOperations
+from ._firewall_status_operations import FirewallStatusOperations
 from ._certificate_object_local_rulestack_operations import CertificateObjectLocalRulestackOperations
 from ._fqdn_list_local_rulestack_operations import FqdnListLocalRulestackOperations
 from ._local_rules_operations import LocalRulesOperations
 from ._prefix_list_local_rulestack_operations import PrefixListLocalRulestackOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
@@ -30,14 +31,15 @@
     "FqdnListGlobalRulestackOperations",
     "PostRulesOperations",
     "PrefixListGlobalRulestackOperations",
     "PreRulesOperations",
     "Operations",
     "FirewallsOperations",
     "LocalRulestacksOperations",
+    "FirewallStatusOperations",
     "CertificateObjectLocalRulestackOperations",
     "FqdnListLocalRulestackOperations",
     "LocalRulesOperations",
     "PrefixListLocalRulestackOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_global_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_global_rulestack_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class PrefixListGlobalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`prefix_list_global_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -68,15 +68,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrefixListGlobalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrefixListGlobalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -155,15 +155,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrefixListGlobalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -294,30 +294,30 @@
         """Create a PrefixListGlobalRulestackResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrefixListGlobalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -345,15 +345,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrefixListGlobalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -365,30 +365,30 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a PrefixListGlobalRulestackResource type
          or a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrefixListGlobalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewalls_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_firewalls_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 class FirewallsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`firewalls` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -69,15 +69,15 @@
     @distributed_trace
     def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.FirewallResource"]:
         """List FirewallResource resources by subscription ID.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FirewallResource or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FirewallResourceListResult] = kwargs.pop("cls", None)
@@ -158,15 +158,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FirewallResource or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FirewallResourceListResult] = kwargs.pop("cls", None)
@@ -247,15 +247,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -385,30 +385,30 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FirewallResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -437,15 +437,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FirewallResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self, resource_group_name: str, firewall_name: str, resource: Union[_models.FirewallResource, IO], **kwargs: Any
     ) -> AsyncLROPoller[_models.FirewallResource]:
@@ -454,30 +454,30 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param resource: Resource create parameters. Is either a FirewallResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FirewallResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FirewallResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -541,21 +541,21 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param properties: The resource properties to be updated. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.FirewallResourceUpdate
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResourceUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update(
         self,
         resource_group_name: str,
@@ -575,15 +575,15 @@
         :param properties: The resource properties to be updated. Required.
         :type properties: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update(
         self,
         resource_group_name: str,
@@ -596,21 +596,21 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param properties: The resource properties to be updated. Is either a FirewallResourceUpdate
          type or a IO type. Required.
-        :type properties: ~azure.mgmt.paloaltonetworks.models.FirewallResourceUpdate or IO
+        :type properties: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResourceUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FirewallResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FirewallResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -794,15 +794,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: GlobalRulestackInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.GlobalRulestackInfo
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackInfo
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -857,15 +857,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: LogSettings or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.LogSettings
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.LogSettings
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -924,15 +924,15 @@
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param email: email address on behalf of which this API called. Default value is None.
         :type email: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SupportInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.SupportInfo
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.SupportInfo
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -995,15 +995,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param log_settings: Default value is None.
-        :type log_settings: ~azure.mgmt.paloaltonetworks.models.LogSettings
+        :type log_settings: ~azure.mgmt.paloaltonetworksngfw.models.LogSettings
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1049,15 +1049,15 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param firewall_name: Firewall resource name. Required.
         :type firewall_name: str
         :param log_settings: Is either a LogSettings type or a IO type. Default value is None.
-        :type log_settings: ~azure.mgmt.paloaltonetworks.models.LogSettings or IO
+        :type log_settings: ~azure.mgmt.paloaltonetworksngfw.models.LogSettings or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_local_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_local_rulestack_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class FqdnListLocalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`fqdn_list_local_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -71,15 +71,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FqdnListLocalRulestackResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FqdnListLocalRulestackResourceListResult] = kwargs.pop("cls", None)
@@ -165,15 +165,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FqdnListLocalRulestackResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -313,30 +313,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FqdnListLocalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -368,15 +368,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FqdnListLocalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -392,30 +392,30 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: fqdn list name. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a FqdnListLocalRulestackResource type or
          a IO type. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FqdnListLocalRulestackResource or
          the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_pre_rules_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_pre_rules_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 class PreRulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`pre_rules` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -68,15 +68,15 @@
         """List PreRulesResource resources by Tenant.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PreRulesResource or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PreRulesResourceListResult] = kwargs.pop("cls", None)
@@ -153,15 +153,15 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PreRulesResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PreRulesResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -288,30 +288,30 @@
         """Create a PreRulesResource.
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PreRulesResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PreRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         global_rulestack_name: str,
@@ -339,15 +339,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PreRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self, global_rulestack_name: str, priority: str, resource: Union[_models.PreRulesResource, IO], **kwargs: Any
     ) -> AsyncLROPoller[_models.PreRulesResource]:
@@ -355,30 +355,30 @@
 
         :param global_rulestack_name: GlobalRulestack resource name. Required.
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param resource: Resource create parameters. Is either a PreRulesResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PreRulesResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PreRulesResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
@@ -551,15 +551,15 @@
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounter or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounter
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounter
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -679,15 +679,15 @@
         :type global_rulestack_name: str
         :param priority: Pre Rule priority. Required.
         :type priority: str
         :param firewall_name: Default value is None.
         :type firewall_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RuleCounterReset or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.RuleCounterReset
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.RuleCounterReset
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_local_rulestack_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_prefix_list_local_rulestack_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class PrefixListLocalRulestackOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`prefix_list_local_rulestack` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -70,15 +70,15 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrefixListResource or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrefixListResourceListResult] = kwargs.pop("cls", None)
@@ -164,15 +164,15 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrefixListResource or the result of cls(response)
-        :rtype: ~azure.mgmt.paloaltonetworks.models.PrefixListResource
+        :rtype: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -312,30 +312,30 @@
          Required.
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListResource
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrefixListResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -367,15 +367,15 @@
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrefixListResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
@@ -391,30 +391,30 @@
         :type resource_group_name: str
         :param local_rulestack_name: LocalRulestack resource name. Required.
         :type local_rulestack_name: str
         :param name: Local Rule priority. Required.
         :type name: str
         :param resource: Resource create parameters. Is either a PrefixListResource type or a IO type.
          Required.
-        :type resource: ~azure.mgmt.paloaltonetworks.models.PrefixListResource or IO
+        :type resource: ~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrefixListResource or the result of
          cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/aio/operations/_operations.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.paloaltonetworks.aio.PaloAltoNetworksNgfwMgmtClient`'s
+        :class:`~azure.mgmt.paloaltonetworksngfw.aio.PaloAltoNetworksNgfwMgmtClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -54,15 +54,16 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
         """List the operations for the provider.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworks.models.Operation]
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.paloaltonetworksngfw.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_palo_alto_networks_ngfw_mgmt_client_enums.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_palo_alto_networks_ngfw_mgmt_client_enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,23 @@
 class EnabledDNSType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Enabled DNS type values."""
 
     CUSTOM = "CUSTOM"
     AZURE = "AZURE"
 
 
+class HealthStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Status Codes for the Firewall."""
+
+    GREEN = "GREEN"
+    YELLOW = "YELLOW"
+    RED = "RED"
+    INITIALIZING = "INITIALIZING"
+
+
 class LogOption(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Log options possible."""
 
     SAME_DESTINATION = "SAME_DESTINATION"
     INDIVIDUAL_DESTINATION = "INDIVIDUAL_DESTINATION"
 
 
@@ -164,32 +173,48 @@
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     CANCELED = "Canceled"
     DELETED = "Deleted"
     NOT_SPECIFIED = "NotSpecified"
 
 
+class ReadOnlyProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Provisioning state of the firewall resource."""
+
+    SUCCEEDED = "Succeeded"
+    FAILED = "Failed"
+    DELETED = "Deleted"
+
+
 class ScopeType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Rulestack Type."""
 
     LOCAL = "LOCAL"
     GLOBAL = "GLOBAL"
+    GLOBAL_ENUM = "GLOBAL"
 
 
 class SecurityServicesTypeEnum(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """SecurityServicesTypeEnum."""
 
     ANTI_SPYWARE = "antiSpyware"
     ANTI_VIRUS = "antiVirus"
     IPS_VULNERABILITY = "ipsVulnerability"
     URL_FILTERING = "urlFiltering"
     FILE_BLOCKING = "fileBlocking"
     DNS_SUBSCRIPTION = "dnsSubscription"
 
 
+class ServerStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Connectivity Status for Panorama Server."""
+
+    UP = "UP"
+    DOWN = "DOWN"
+
+
 class StateEnum(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Enabled or Disabled Enum."""
 
     DISABLED = "DISABLED"
     ENABLED = "ENABLED"
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_models_py3.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/_models_py3.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class AdvSecurityObjectListResponse(_serialization.Model):
     """advanced security object.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: response value. Required.
-    :vartype value: ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectModel
+    :vartype value: ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectModel
     :ivar next_link: next link.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -38,15 +38,15 @@
     }
 
     def __init__(
         self, *, value: "_models.AdvSecurityObjectModel", next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: response value. Required.
-        :paramtype value: ~azure.mgmt.paloaltonetworks.models.AdvSecurityObjectModel
+        :paramtype value: ~azure.mgmt.paloaltonetworksngfw.models.AdvSecurityObjectModel
         :keyword next_link: next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -55,15 +55,15 @@
     """List of custom and predefined url category.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: type of object.
     :vartype type: str
     :ivar entry: URL entry. Required.
-    :vartype entry: list[~azure.mgmt.paloaltonetworks.models.NameDescriptionObject]
+    :vartype entry: list[~azure.mgmt.paloaltonetworksngfw.models.NameDescriptionObject]
     """
 
     _validation = {
         "entry": {"required": True},
     }
 
     _attribute_map = {
@@ -74,15 +74,15 @@
     def __init__(
         self, *, entry: List["_models.NameDescriptionObject"], type: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword type: type of object.
         :paramtype type: str
         :keyword entry: URL entry. Required.
-        :paramtype entry: list[~azure.mgmt.paloaltonetworks.models.NameDescriptionObject]
+        :paramtype entry: list[~azure.mgmt.paloaltonetworksngfw.models.NameDescriptionObject]
         """
         super().__init__(**kwargs)
         self.type = type
         self.entry = entry
 
 
 class ApplicationInsights(_serialization.Model):
@@ -117,15 +117,15 @@
     """Data Type for App Seen.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar count: number of rows. Required.
     :vartype count: int
     :ivar app_seen_list: array of appSeen. Required.
-    :vartype app_seen_list: list[~azure.mgmt.paloaltonetworks.models.AppSeenInfo]
+    :vartype app_seen_list: list[~azure.mgmt.paloaltonetworksngfw.models.AppSeenInfo]
     """
 
     _validation = {
         "count": {"required": True},
         "app_seen_list": {"required": True},
     }
 
@@ -135,15 +135,15 @@
     }
 
     def __init__(self, *, count: int, app_seen_list: List["_models.AppSeenInfo"], **kwargs: Any) -> None:
         """
         :keyword count: number of rows. Required.
         :paramtype count: int
         :keyword app_seen_list: array of appSeen. Required.
-        :paramtype app_seen_list: list[~azure.mgmt.paloaltonetworks.models.AppSeenInfo]
+        :paramtype app_seen_list: list[~azure.mgmt.paloaltonetworksngfw.models.AppSeenInfo]
         """
         super().__init__(**kwargs)
         self.count = count
         self.app_seen_list = app_seen_list
 
 
 class AppSeenInfo(_serialization.Model):
@@ -234,18 +234,18 @@
 
     :ivar tenant_id: The Active Directory tenant id of the principal.
     :vartype tenant_id: str
     :ivar principal_id: The active directory identifier of this principal.
     :vartype principal_id: str
     :ivar type: The type of managed identity assigned to this resource. Required. Known values are:
      "None", "SystemAssigned", "UserAssigned", and "SystemAssigned,UserAssigned".
-    :vartype type: str or ~azure.mgmt.paloaltonetworks.models.ManagedIdentityType
+    :vartype type: str or ~azure.mgmt.paloaltonetworksngfw.models.ManagedIdentityType
     :ivar user_assigned_identities: The identities assigned to this resource by the user.
     :vartype user_assigned_identities: dict[str,
-     ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerUserAssignedIdentity]
+     ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerUserAssignedIdentity]
     """
 
     _validation = {
         "tenant_id": {"readonly": True},
         "principal_id": {"readonly": True},
         "type": {"required": True},
     }
@@ -266,18 +266,18 @@
         type: Union[str, "_models.ManagedIdentityType"],
         user_assigned_identities: Optional[Dict[str, "_models.AzureResourceManagerUserAssignedIdentity"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword type: The type of managed identity assigned to this resource. Required. Known values
          are: "None", "SystemAssigned", "UserAssigned", and "SystemAssigned,UserAssigned".
-        :paramtype type: str or ~azure.mgmt.paloaltonetworks.models.ManagedIdentityType
+        :paramtype type: str or ~azure.mgmt.paloaltonetworksngfw.models.ManagedIdentityType
         :keyword user_assigned_identities: The identities assigned to this resource by the user.
         :paramtype user_assigned_identities: dict[str,
-         ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerUserAssignedIdentity]
+         ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerUserAssignedIdentity]
         """
         super().__init__(**kwargs)
         self.tenant_id = None
         self.principal_id = None
         self.type = type
         self.user_assigned_identities = user_assigned_identities
 
@@ -352,15 +352,15 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -394,15 +394,15 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -433,31 +433,31 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar certificate_signer_resource_id: Resource Id of certificate signer, to be populated only
      when certificateSelfSigned is false.
     :vartype certificate_signer_resource_id: str
     :ivar certificate_self_signed: use certificate self signed. Required. Known values are: "TRUE"
      and "FALSE".
-    :vartype certificate_self_signed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype certificate_self_signed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar audit_comment: comment for this object.
     :vartype audit_comment: str
     :ivar description: user description for this object.
     :vartype description: str
     :ivar etag: read only string representing last create or update.
     :vartype etag: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -490,15 +490,15 @@
     ) -> None:
         """
         :keyword certificate_signer_resource_id: Resource Id of certificate signer, to be populated
          only when certificateSelfSigned is false.
         :paramtype certificate_signer_resource_id: str
         :keyword certificate_self_signed: use certificate self signed. Required. Known values are:
          "TRUE" and "FALSE".
-        :paramtype certificate_self_signed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype certificate_self_signed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword audit_comment: comment for this object.
         :paramtype audit_comment: str
         :keyword description: user description for this object.
         :paramtype description: str
         :keyword etag: read only string representing last create or update.
         :paramtype etag: str
         """
@@ -514,15 +514,15 @@
 class CertificateObjectGlobalRulestackResourceListResult(_serialization.Model):
     """The response of a CertificateObjectGlobalRulestackResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
     :vartype value:
-     list[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+     list[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -538,15 +538,15 @@
         value: List["_models.CertificateObjectGlobalRulestackResource"],
         next_link: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
         :paramtype value:
-         list[~azure.mgmt.paloaltonetworks.models.CertificateObjectGlobalRulestackResource]
+         list[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectGlobalRulestackResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -564,31 +564,31 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar certificate_signer_resource_id: Resource Id of certificate signer, to be populated only
      when certificateSelfSigned is false.
     :vartype certificate_signer_resource_id: str
     :ivar certificate_self_signed: use certificate self signed. Required. Known values are: "TRUE"
      and "FALSE".
-    :vartype certificate_self_signed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype certificate_self_signed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar audit_comment: comment for this object.
     :vartype audit_comment: str
     :ivar description: user description for this object.
     :vartype description: str
     :ivar etag: read only string representing last create or update.
     :vartype etag: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -621,15 +621,15 @@
     ) -> None:
         """
         :keyword certificate_signer_resource_id: Resource Id of certificate signer, to be populated
          only when certificateSelfSigned is false.
         :paramtype certificate_signer_resource_id: str
         :keyword certificate_self_signed: use certificate self signed. Required. Known values are:
          "TRUE" and "FALSE".
-        :paramtype certificate_self_signed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype certificate_self_signed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword audit_comment: comment for this object.
         :paramtype audit_comment: str
         :keyword description: user description for this object.
         :paramtype description: str
         :keyword etag: read only string representing last create or update.
         :paramtype etag: str
         """
@@ -645,15 +645,15 @@
 class CertificateObjectLocalRulestackResourceListResult(_serialization.Model):
     """The response of a CertificateObjectLocalRulestackResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
     :vartype value:
-     list[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+     list[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -669,15 +669,15 @@
         value: List["_models.CertificateObjectLocalRulestackResource"],
         next_link: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
         :paramtype value:
-         list[~azure.mgmt.paloaltonetworks.models.CertificateObjectLocalRulestackResource]
+         list[~azure.mgmt.paloaltonetworksngfw.models.CertificateObjectLocalRulestackResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -729,15 +729,15 @@
 
 class CountriesResponse(_serialization.Model):
     """Countries Response Object.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: List of countries. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.Country]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.Country]
     :ivar next_link: next link.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -746,15 +746,15 @@
         "value": {"key": "value", "type": "[Country]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(self, *, value: List["_models.Country"], next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: List of countries. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.Country]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.Country]
         :keyword next_link: next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -845,20 +845,20 @@
 
 
 class DNSSettings(_serialization.Model):
     """DNS Proxy settings for Firewall.
 
     :ivar enable_dns_proxy: Enable DNS proxy, disabled by default. Known values are: "DISABLED" and
      "ENABLED".
-    :vartype enable_dns_proxy: str or ~azure.mgmt.paloaltonetworks.models.DNSProxy
+    :vartype enable_dns_proxy: str or ~azure.mgmt.paloaltonetworksngfw.models.DNSProxy
     :ivar enabled_dns_type: Enabled DNS proxy type, disabled by default. Known values are: "CUSTOM"
      and "AZURE".
-    :vartype enabled_dns_type: str or ~azure.mgmt.paloaltonetworks.models.EnabledDNSType
+    :vartype enabled_dns_type: str or ~azure.mgmt.paloaltonetworksngfw.models.EnabledDNSType
     :ivar dns_servers: List of IPs associated with the Firewall.
-    :vartype dns_servers: list[~azure.mgmt.paloaltonetworks.models.IPAddress]
+    :vartype dns_servers: list[~azure.mgmt.paloaltonetworksngfw.models.IPAddress]
     """
 
     _attribute_map = {
         "enable_dns_proxy": {"key": "enableDnsProxy", "type": "str"},
         "enabled_dns_type": {"key": "enabledDnsType", "type": "str"},
         "dns_servers": {"key": "dnsServers", "type": "[IPAddress]"},
     }
@@ -870,20 +870,20 @@
         enabled_dns_type: Optional[Union[str, "_models.EnabledDNSType"]] = None,
         dns_servers: Optional[List["_models.IPAddress"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword enable_dns_proxy: Enable DNS proxy, disabled by default. Known values are: "DISABLED"
          and "ENABLED".
-        :paramtype enable_dns_proxy: str or ~azure.mgmt.paloaltonetworks.models.DNSProxy
+        :paramtype enable_dns_proxy: str or ~azure.mgmt.paloaltonetworksngfw.models.DNSProxy
         :keyword enabled_dns_type: Enabled DNS proxy type, disabled by default. Known values are:
          "CUSTOM" and "AZURE".
-        :paramtype enabled_dns_type: str or ~azure.mgmt.paloaltonetworks.models.EnabledDNSType
+        :paramtype enabled_dns_type: str or ~azure.mgmt.paloaltonetworksngfw.models.EnabledDNSType
         :keyword dns_servers: List of IPs associated with the Firewall.
-        :paramtype dns_servers: list[~azure.mgmt.paloaltonetworks.models.IPAddress]
+        :paramtype dns_servers: list[~azure.mgmt.paloaltonetworksngfw.models.IPAddress]
         """
         super().__init__(**kwargs)
         self.enable_dns_proxy = enable_dns_proxy
         self.enabled_dns_type = enabled_dns_type
         self.dns_servers = dns_servers
 
 
@@ -891,15 +891,15 @@
     """Endpoint Configuration for frontend and backend.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar port: port ID. Required.
     :vartype port: str
     :ivar address: Address Space. Required.
-    :vartype address: ~azure.mgmt.paloaltonetworks.models.IPAddress
+    :vartype address: ~azure.mgmt.paloaltonetworksngfw.models.IPAddress
     """
 
     _validation = {
         "port": {"required": True},
         "address": {"required": True},
     }
 
@@ -909,15 +909,15 @@
     }
 
     def __init__(self, *, port: str, address: "_models.IPAddress", **kwargs: Any) -> None:
         """
         :keyword port: port ID. Required.
         :paramtype port: str
         :keyword address: Address Space. Required.
-        :paramtype address: ~azure.mgmt.paloaltonetworks.models.IPAddress
+        :paramtype address: ~azure.mgmt.paloaltonetworksngfw.models.IPAddress
         """
         super().__init__(**kwargs)
         self.port = port
         self.address = address
 
 
 class ErrorAdditionalInfo(_serialization.Model):
@@ -956,17 +956,17 @@
     :ivar code: The error code.
     :vartype code: str
     :ivar message: The error message.
     :vartype message: str
     :ivar target: The error target.
     :vartype target: str
     :ivar details: The error details.
-    :vartype details: list[~azure.mgmt.paloaltonetworks.models.ErrorDetail]
+    :vartype details: list[~azure.mgmt.paloaltonetworksngfw.models.ErrorDetail]
     :ivar additional_info: The error additional info.
-    :vartype additional_info: list[~azure.mgmt.paloaltonetworks.models.ErrorAdditionalInfo]
+    :vartype additional_info: list[~azure.mgmt.paloaltonetworksngfw.models.ErrorAdditionalInfo]
     """
 
     _validation = {
         "code": {"readonly": True},
         "message": {"readonly": True},
         "target": {"readonly": True},
         "details": {"readonly": True},
@@ -992,25 +992,25 @@
 
 
 class ErrorResponse(_serialization.Model):
     """Common error response for all Azure Resource Manager APIs to return error details for failed
     operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
-    :vartype error: ~azure.mgmt.paloaltonetworks.models.ErrorDetail
+    :vartype error: ~azure.mgmt.paloaltonetworksngfw.models.ErrorDetail
     """
 
     _attribute_map = {
         "error": {"key": "error", "type": "ErrorDetail"},
     }
 
     def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
         """
         :keyword error: The error object.
-        :paramtype error: ~azure.mgmt.paloaltonetworks.models.ErrorDetail
+        :paramtype error: ~azure.mgmt.paloaltonetworksngfw.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
 
 class EventHub(_serialization.Model):
     """EventHub configurations.
@@ -1079,15 +1079,15 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     """
 
     _validation = {
@@ -1132,45 +1132,45 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     :ivar identity: The managed service identities assigned to this resource.
     :vartype identity:
-     ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+     ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
     :ivar pan_etag: panEtag info.
     :vartype pan_etag: str
     :ivar network_profile: Network settings. Required.
-    :vartype network_profile: ~azure.mgmt.paloaltonetworks.models.NetworkProfile
+    :vartype network_profile: ~azure.mgmt.paloaltonetworksngfw.models.NetworkProfile
     :ivar is_panorama_managed: Panorama Managed: Default is False. Default will be CloudSec
      managed. Known values are: "TRUE" and "FALSE".
-    :vartype is_panorama_managed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype is_panorama_managed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar panorama_config: Panorama Configuration.
-    :vartype panorama_config: ~azure.mgmt.paloaltonetworks.models.PanoramaConfig
+    :vartype panorama_config: ~azure.mgmt.paloaltonetworksngfw.models.PanoramaConfig
     :ivar associated_rulestack: Associated Rulestack.
-    :vartype associated_rulestack: ~azure.mgmt.paloaltonetworks.models.RulestackDetails
+    :vartype associated_rulestack: ~azure.mgmt.paloaltonetworksngfw.models.RulestackDetails
     :ivar dns_settings: DNS settings for Firewall. Required.
-    :vartype dns_settings: ~azure.mgmt.paloaltonetworks.models.DNSSettings
+    :vartype dns_settings: ~azure.mgmt.paloaltonetworksngfw.models.DNSSettings
     :ivar front_end_settings: Frontend settings for Firewall.
-    :vartype front_end_settings: list[~azure.mgmt.paloaltonetworks.models.FrontendSetting]
+    :vartype front_end_settings: list[~azure.mgmt.paloaltonetworksngfw.models.FrontendSetting]
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     :ivar plan_data: Billing plan information. Required.
-    :vartype plan_data: ~azure.mgmt.paloaltonetworks.models.PlanData
+    :vartype plan_data: ~azure.mgmt.paloaltonetworksngfw.models.PlanData
     :ivar marketplace_details: Marketplace details. Required.
-    :vartype marketplace_details: ~azure.mgmt.paloaltonetworks.models.MarketplaceDetails
+    :vartype marketplace_details: ~azure.mgmt.paloaltonetworksngfw.models.MarketplaceDetails
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1222,34 +1222,34 @@
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword identity: The managed service identities assigned to this resource.
         :paramtype identity:
-         ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
         :keyword pan_etag: panEtag info.
         :paramtype pan_etag: str
         :keyword network_profile: Network settings. Required.
-        :paramtype network_profile: ~azure.mgmt.paloaltonetworks.models.NetworkProfile
+        :paramtype network_profile: ~azure.mgmt.paloaltonetworksngfw.models.NetworkProfile
         :keyword is_panorama_managed: Panorama Managed: Default is False. Default will be CloudSec
          managed. Known values are: "TRUE" and "FALSE".
-        :paramtype is_panorama_managed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype is_panorama_managed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword panorama_config: Panorama Configuration.
-        :paramtype panorama_config: ~azure.mgmt.paloaltonetworks.models.PanoramaConfig
+        :paramtype panorama_config: ~azure.mgmt.paloaltonetworksngfw.models.PanoramaConfig
         :keyword associated_rulestack: Associated Rulestack.
-        :paramtype associated_rulestack: ~azure.mgmt.paloaltonetworks.models.RulestackDetails
+        :paramtype associated_rulestack: ~azure.mgmt.paloaltonetworksngfw.models.RulestackDetails
         :keyword dns_settings: DNS settings for Firewall. Required.
-        :paramtype dns_settings: ~azure.mgmt.paloaltonetworks.models.DNSSettings
+        :paramtype dns_settings: ~azure.mgmt.paloaltonetworksngfw.models.DNSSettings
         :keyword front_end_settings: Frontend settings for Firewall.
-        :paramtype front_end_settings: list[~azure.mgmt.paloaltonetworks.models.FrontendSetting]
+        :paramtype front_end_settings: list[~azure.mgmt.paloaltonetworksngfw.models.FrontendSetting]
         :keyword plan_data: Billing plan information. Required.
-        :paramtype plan_data: ~azure.mgmt.paloaltonetworks.models.PlanData
+        :paramtype plan_data: ~azure.mgmt.paloaltonetworksngfw.models.PlanData
         :keyword marketplace_details: Marketplace details. Required.
-        :paramtype marketplace_details: ~azure.mgmt.paloaltonetworks.models.MarketplaceDetails
+        :paramtype marketplace_details: ~azure.mgmt.paloaltonetworksngfw.models.MarketplaceDetails
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.identity = identity
         self.pan_etag = pan_etag
         self.network_profile = network_profile
         self.is_panorama_managed = is_panorama_managed
         self.panorama_config = panorama_config
@@ -1263,15 +1263,15 @@
 
 class FirewallResourceListResult(_serialization.Model):
     """The response of a FirewallResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -1282,33 +1282,33 @@
     }
 
     def __init__(
         self, *, value: List["_models.FirewallResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.FirewallResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.FirewallResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class FirewallResourceUpdate(_serialization.Model):
     """The type used for update operations of the FirewallResource.
 
     :ivar identity: The managed service identities assigned to this resource.
     :vartype identity:
-     ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+     ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar properties: The updatable properties of the FirewallResource.
-    :vartype properties: ~azure.mgmt.paloaltonetworks.models.FirewallResourceUpdateProperties
+    :vartype properties: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResourceUpdateProperties
     """
 
     _attribute_map = {
         "identity": {"key": "identity", "type": "AzureResourceManagerManagedIdentityProperties"},
         "tags": {"key": "tags", "type": "{str}"},
         "properties": {"key": "properties", "type": "FirewallResourceUpdateProperties"},
     }
@@ -1320,48 +1320,48 @@
         tags: Optional[Dict[str, str]] = None,
         properties: Optional["_models.FirewallResourceUpdateProperties"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword identity: The managed service identities assigned to this resource.
         :paramtype identity:
-         ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword properties: The updatable properties of the FirewallResource.
-        :paramtype properties: ~azure.mgmt.paloaltonetworks.models.FirewallResourceUpdateProperties
+        :paramtype properties: ~azure.mgmt.paloaltonetworksngfw.models.FirewallResourceUpdateProperties
         """
         super().__init__(**kwargs)
         self.identity = identity
         self.tags = tags
         self.properties = properties
 
 
 class FirewallResourceUpdateProperties(_serialization.Model):
     """The updatable properties of the FirewallResource.
 
     :ivar pan_etag: panEtag info.
     :vartype pan_etag: str
     :ivar network_profile: Network settings.
-    :vartype network_profile: ~azure.mgmt.paloaltonetworks.models.NetworkProfile
+    :vartype network_profile: ~azure.mgmt.paloaltonetworksngfw.models.NetworkProfile
     :ivar is_panorama_managed: Panorama Managed: Default is False. Default will be CloudSec
      managed. Known values are: "TRUE" and "FALSE".
-    :vartype is_panorama_managed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype is_panorama_managed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar panorama_config: Panorama Configuration.
-    :vartype panorama_config: ~azure.mgmt.paloaltonetworks.models.PanoramaConfig
+    :vartype panorama_config: ~azure.mgmt.paloaltonetworksngfw.models.PanoramaConfig
     :ivar associated_rulestack: Associated Rulestack.
-    :vartype associated_rulestack: ~azure.mgmt.paloaltonetworks.models.RulestackDetails
+    :vartype associated_rulestack: ~azure.mgmt.paloaltonetworksngfw.models.RulestackDetails
     :ivar dns_settings: DNS settings for Firewall.
-    :vartype dns_settings: ~azure.mgmt.paloaltonetworks.models.DNSSettings
+    :vartype dns_settings: ~azure.mgmt.paloaltonetworksngfw.models.DNSSettings
     :ivar front_end_settings: Frontend settings for Firewall.
-    :vartype front_end_settings: list[~azure.mgmt.paloaltonetworks.models.FrontendSetting]
+    :vartype front_end_settings: list[~azure.mgmt.paloaltonetworksngfw.models.FrontendSetting]
     :ivar plan_data: Billing plan information.
-    :vartype plan_data: ~azure.mgmt.paloaltonetworks.models.PlanData
+    :vartype plan_data: ~azure.mgmt.paloaltonetworksngfw.models.PlanData
     :ivar marketplace_details: Marketplace details.
-    :vartype marketplace_details: ~azure.mgmt.paloaltonetworks.models.MarketplaceDetails
+    :vartype marketplace_details: ~azure.mgmt.paloaltonetworksngfw.models.MarketplaceDetails
     """
 
     _attribute_map = {
         "pan_etag": {"key": "panEtag", "type": "str"},
         "network_profile": {"key": "networkProfile", "type": "NetworkProfile"},
         "is_panorama_managed": {"key": "isPanoramaManaged", "type": "str"},
         "panorama_config": {"key": "panoramaConfig", "type": "PanoramaConfig"},
@@ -1386,43 +1386,143 @@
         marketplace_details: Optional["_models.MarketplaceDetails"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword pan_etag: panEtag info.
         :paramtype pan_etag: str
         :keyword network_profile: Network settings.
-        :paramtype network_profile: ~azure.mgmt.paloaltonetworks.models.NetworkProfile
+        :paramtype network_profile: ~azure.mgmt.paloaltonetworksngfw.models.NetworkProfile
         :keyword is_panorama_managed: Panorama Managed: Default is False. Default will be CloudSec
          managed. Known values are: "TRUE" and "FALSE".
-        :paramtype is_panorama_managed: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype is_panorama_managed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword panorama_config: Panorama Configuration.
-        :paramtype panorama_config: ~azure.mgmt.paloaltonetworks.models.PanoramaConfig
+        :paramtype panorama_config: ~azure.mgmt.paloaltonetworksngfw.models.PanoramaConfig
         :keyword associated_rulestack: Associated Rulestack.
-        :paramtype associated_rulestack: ~azure.mgmt.paloaltonetworks.models.RulestackDetails
+        :paramtype associated_rulestack: ~azure.mgmt.paloaltonetworksngfw.models.RulestackDetails
         :keyword dns_settings: DNS settings for Firewall.
-        :paramtype dns_settings: ~azure.mgmt.paloaltonetworks.models.DNSSettings
+        :paramtype dns_settings: ~azure.mgmt.paloaltonetworksngfw.models.DNSSettings
         :keyword front_end_settings: Frontend settings for Firewall.
-        :paramtype front_end_settings: list[~azure.mgmt.paloaltonetworks.models.FrontendSetting]
+        :paramtype front_end_settings: list[~azure.mgmt.paloaltonetworksngfw.models.FrontendSetting]
         :keyword plan_data: Billing plan information.
-        :paramtype plan_data: ~azure.mgmt.paloaltonetworks.models.PlanData
+        :paramtype plan_data: ~azure.mgmt.paloaltonetworksngfw.models.PlanData
         :keyword marketplace_details: Marketplace details.
-        :paramtype marketplace_details: ~azure.mgmt.paloaltonetworks.models.MarketplaceDetails
+        :paramtype marketplace_details: ~azure.mgmt.paloaltonetworksngfw.models.MarketplaceDetails
         """
         super().__init__(**kwargs)
         self.pan_etag = pan_etag
         self.network_profile = network_profile
         self.is_panorama_managed = is_panorama_managed
         self.panorama_config = panorama_config
         self.associated_rulestack = associated_rulestack
         self.dns_settings = dns_settings
         self.front_end_settings = front_end_settings
         self.plan_data = plan_data
         self.marketplace_details = marketplace_details
 
 
+class FirewallStatusResource(ProxyResource):
+    """Firewall Status.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
+    :ivar is_panorama_managed: Panorama Managed: Default is False. Default will be CloudSec
+     managed. Known values are: "TRUE" and "FALSE".
+    :vartype is_panorama_managed: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
+    :ivar health_status: Current status of the Firewall. Known values are: "GREEN", "YELLOW",
+     "RED", and "INITIALIZING".
+    :vartype health_status: str or ~azure.mgmt.paloaltonetworksngfw.models.HealthStatus
+    :ivar health_reason: Detail description of current health of the Firewall.
+    :vartype health_reason: str
+    :ivar panorama_status: Panorama Status.
+    :vartype panorama_status: ~azure.mgmt.paloaltonetworksngfw.models.PanoramaStatus
+    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Succeeded",
+     "Failed", and "Deleted".
+    :vartype provisioning_state: str or
+     ~azure.mgmt.paloaltonetworksngfw.models.ReadOnlyProvisioningState
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "is_panorama_managed": {"readonly": True},
+        "health_status": {"readonly": True},
+        "health_reason": {"readonly": True},
+        "panorama_status": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "is_panorama_managed": {"key": "properties.isPanoramaManaged", "type": "str"},
+        "health_status": {"key": "properties.healthStatus", "type": "str"},
+        "health_reason": {"key": "properties.healthReason", "type": "str"},
+        "panorama_status": {"key": "properties.panoramaStatus", "type": "PanoramaStatus"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.is_panorama_managed = None
+        self.health_status = None
+        self.health_reason = None
+        self.panorama_status = None
+        self.provisioning_state = None
+
+
+class FirewallStatusResourceListResult(_serialization.Model):
+    """The response of a FirewallStatusResource list operation.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar value: The items on this page. Required.
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.FirewallStatusResource]
+    :ivar next_link: The link to the next page of items.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[FirewallStatusResource]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(
+        self, *, value: List["_models.FirewallStatusResource"], next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword value: The items on this page. Required.
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.FirewallStatusResource]
+        :keyword next_link: The link to the next page of items.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
+
+
 class FqdnListGlobalRulestackResource(ProxyResource):
     """GlobalRulestack fqdnList.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -1432,27 +1532,27 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar description: fqdn object description.
     :vartype description: str
     :ivar fqdn_list: fqdn list. Required.
     :vartype fqdn_list: list[str]
     :ivar etag: etag info.
     :vartype etag: str
     :ivar audit_comment: comment for this object.
     :vartype audit_comment: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1501,15 +1601,15 @@
 
 class FqdnListGlobalRulestackResourceListResult(_serialization.Model):
     """The response of a FqdnListGlobalRulestackResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -1520,15 +1620,15 @@
     }
 
     def __init__(
         self, *, value: List["_models.FqdnListGlobalRulestackResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.FqdnListGlobalRulestackResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.FqdnListGlobalRulestackResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -1546,27 +1646,27 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar description: fqdn object description.
     :vartype description: str
     :ivar fqdn_list: fqdn list. Required.
     :vartype fqdn_list: list[str]
     :ivar etag: etag info.
     :vartype etag: str
     :ivar audit_comment: comment for this object.
     :vartype audit_comment: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1615,15 +1715,15 @@
 
 class FqdnListLocalRulestackResourceListResult(_serialization.Model):
     """The response of a FqdnListLocalRulestackResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -1634,15 +1734,15 @@
     }
 
     def __init__(
         self, *, value: List["_models.FqdnListLocalRulestackResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.FqdnListLocalRulestackResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.FqdnListLocalRulestackResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -1651,19 +1751,19 @@
     """Frontend setting for Firewall.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar name: Settings name. Required.
     :vartype name: str
     :ivar protocol: Protocol Type. Required. Known values are: "TCP" and "UDP".
-    :vartype protocol: str or ~azure.mgmt.paloaltonetworks.models.ProtocolType
+    :vartype protocol: str or ~azure.mgmt.paloaltonetworksngfw.models.ProtocolType
     :ivar frontend_configuration: Frontend configurations. Required.
-    :vartype frontend_configuration: ~azure.mgmt.paloaltonetworks.models.EndpointConfiguration
+    :vartype frontend_configuration: ~azure.mgmt.paloaltonetworksngfw.models.EndpointConfiguration
     :ivar backend_configuration: Backend configurations. Required.
-    :vartype backend_configuration: ~azure.mgmt.paloaltonetworks.models.EndpointConfiguration
+    :vartype backend_configuration: ~azure.mgmt.paloaltonetworksngfw.models.EndpointConfiguration
     """
 
     _validation = {
         "name": {"required": True},
         "protocol": {"required": True},
         "frontend_configuration": {"required": True},
         "backend_configuration": {"required": True},
@@ -1685,19 +1785,20 @@
         backend_configuration: "_models.EndpointConfiguration",
         **kwargs: Any
     ) -> None:
         """
         :keyword name: Settings name. Required.
         :paramtype name: str
         :keyword protocol: Protocol Type. Required. Known values are: "TCP" and "UDP".
-        :paramtype protocol: str or ~azure.mgmt.paloaltonetworks.models.ProtocolType
+        :paramtype protocol: str or ~azure.mgmt.paloaltonetworksngfw.models.ProtocolType
         :keyword frontend_configuration: Frontend configurations. Required.
-        :paramtype frontend_configuration: ~azure.mgmt.paloaltonetworks.models.EndpointConfiguration
+        :paramtype frontend_configuration:
+         ~azure.mgmt.paloaltonetworksngfw.models.EndpointConfiguration
         :keyword backend_configuration: Backend configurations. Required.
-        :paramtype backend_configuration: ~azure.mgmt.paloaltonetworks.models.EndpointConfiguration
+        :paramtype backend_configuration: ~azure.mgmt.paloaltonetworksngfw.models.EndpointConfiguration
         """
         super().__init__(**kwargs)
         self.name = name
         self.protocol = protocol
         self.frontend_configuration = frontend_configuration
         self.backend_configuration = backend_configuration
 
@@ -1741,41 +1842,41 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar location: Global Location. Required.
     :vartype location: str
     :ivar identity: The managed service identities assigned to this resource.
     :vartype identity:
-     ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+     ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
     :ivar pan_etag: PanEtag info.
     :vartype pan_etag: str
     :ivar pan_location: Rulestack Location, Required for GlobalRulestacks, Not for LocalRulestacks.
     :vartype pan_location: str
-    :ivar scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-    :vartype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+    :ivar scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+    :vartype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
     :ivar associated_subscriptions: subscription scope of global rulestack.
     :vartype associated_subscriptions: list[str]
     :ivar description: rulestack description.
     :vartype description: str
     :ivar default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL", and
      "NONE".
-    :vartype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+    :vartype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
     :ivar min_app_id_version: minimum version.
     :vartype min_app_id_version: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     :ivar security_services: Security Profile.
-    :vartype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+    :vartype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1817,33 +1918,33 @@
         **kwargs: Any
     ) -> None:
         """
         :keyword location: Global Location. Required.
         :paramtype location: str
         :keyword identity: The managed service identities assigned to this resource.
         :paramtype identity:
-         ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
         :keyword pan_etag: PanEtag info.
         :paramtype pan_etag: str
         :keyword pan_location: Rulestack Location, Required for GlobalRulestacks, Not for
          LocalRulestacks.
         :paramtype pan_location: str
-        :keyword scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-        :paramtype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+        :keyword scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+        :paramtype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
         :keyword associated_subscriptions: subscription scope of global rulestack.
         :paramtype associated_subscriptions: list[str]
         :keyword description: rulestack description.
         :paramtype description: str
         :keyword default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL",
          and "NONE".
-        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
         :keyword min_app_id_version: minimum version.
         :paramtype min_app_id_version: str
         :keyword security_services: Security Profile.
-        :paramtype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+        :paramtype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
         """
         super().__init__(**kwargs)
         self.location = location
         self.identity = identity
         self.pan_etag = pan_etag
         self.pan_location = pan_location
         self.scope = scope
@@ -1857,15 +1958,15 @@
 
 class GlobalRulestackResourceListResult(_serialization.Model):
     """The response of a GlobalRulestackResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -1876,15 +1977,15 @@
     }
 
     def __init__(
         self, *, value: List["_models.GlobalRulestackResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.GlobalRulestackResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -1892,18 +1993,18 @@
 class GlobalRulestackResourceUpdate(_serialization.Model):
     """The type used for update operations of the GlobalRulestackResource.
 
     :ivar location: Global Location.
     :vartype location: str
     :ivar identity: The managed service identities assigned to this resource.
     :vartype identity:
-     ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+     ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
     :ivar properties: The updatable properties of the GlobalRulestackResource.
     :vartype properties:
-     ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResourceUpdateProperties
+     ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResourceUpdateProperties
     """
 
     _attribute_map = {
         "location": {"key": "location", "type": "str"},
         "identity": {"key": "identity", "type": "AzureResourceManagerManagedIdentityProperties"},
         "properties": {"key": "properties", "type": "GlobalRulestackResourceUpdateProperties"},
     }
@@ -1917,45 +2018,45 @@
         **kwargs: Any
     ) -> None:
         """
         :keyword location: Global Location.
         :paramtype location: str
         :keyword identity: The managed service identities assigned to this resource.
         :paramtype identity:
-         ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
         :keyword properties: The updatable properties of the GlobalRulestackResource.
         :paramtype properties:
-         ~azure.mgmt.paloaltonetworks.models.GlobalRulestackResourceUpdateProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.GlobalRulestackResourceUpdateProperties
         """
         super().__init__(**kwargs)
         self.location = location
         self.identity = identity
         self.properties = properties
 
 
 class GlobalRulestackResourceUpdateProperties(_serialization.Model):
     """The updatable properties of the GlobalRulestackResource.
 
     :ivar pan_etag: PanEtag info.
     :vartype pan_etag: str
     :ivar pan_location: Rulestack Location, Required for GlobalRulestacks, Not for LocalRulestacks.
     :vartype pan_location: str
-    :ivar scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-    :vartype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+    :ivar scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+    :vartype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
     :ivar associated_subscriptions: subscription scope of global rulestack.
     :vartype associated_subscriptions: list[str]
     :ivar description: rulestack description.
     :vartype description: str
     :ivar default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL", and
      "NONE".
-    :vartype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+    :vartype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
     :ivar min_app_id_version: minimum version.
     :vartype min_app_id_version: str
     :ivar security_services: Security Profile.
-    :vartype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+    :vartype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
     """
 
     _attribute_map = {
         "pan_etag": {"key": "panEtag", "type": "str"},
         "pan_location": {"key": "panLocation", "type": "str"},
         "scope": {"key": "scope", "type": "str"},
         "associated_subscriptions": {"key": "associatedSubscriptions", "type": "[str]"},
@@ -1980,27 +2081,27 @@
     ) -> None:
         """
         :keyword pan_etag: PanEtag info.
         :paramtype pan_etag: str
         :keyword pan_location: Rulestack Location, Required for GlobalRulestacks, Not for
          LocalRulestacks.
         :paramtype pan_location: str
-        :keyword scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-        :paramtype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+        :keyword scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+        :paramtype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
         :keyword associated_subscriptions: subscription scope of global rulestack.
         :paramtype associated_subscriptions: list[str]
         :keyword description: rulestack description.
         :paramtype description: str
         :keyword default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL",
          and "NONE".
-        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
         :keyword min_app_id_version: minimum version.
         :paramtype min_app_id_version: str
         :keyword security_services: Security Profile.
-        :paramtype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+        :paramtype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
         """
         super().__init__(**kwargs)
         self.pan_etag = pan_etag
         self.pan_location = pan_location
         self.scope = scope
         self.associated_subscriptions = associated_subscriptions
         self.description = description
@@ -2140,60 +2241,60 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar etag: etag info.
     :vartype etag: str
     :ivar rule_name: rule name. Required.
     :vartype rule_name: str
     :ivar priority:
     :vartype priority: int
     :ivar description: rule description.
     :vartype description: str
     :ivar rule_state: state of this rule. Known values are: "DISABLED" and "ENABLED".
-    :vartype rule_state: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+    :vartype rule_state: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
     :ivar source: source address.
-    :vartype source: ~azure.mgmt.paloaltonetworks.models.SourceAddr
+    :vartype source: ~azure.mgmt.paloaltonetworksngfw.models.SourceAddr
     :ivar negate_source: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-    :vartype negate_source: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype negate_source: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar destination: destination address.
-    :vartype destination: ~azure.mgmt.paloaltonetworks.models.DestinationAddr
+    :vartype destination: ~azure.mgmt.paloaltonetworksngfw.models.DestinationAddr
     :ivar negate_destination: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-    :vartype negate_destination: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype negate_destination: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar applications: array of rule applications.
     :vartype applications: list[str]
     :ivar category: rule category.
-    :vartype category: ~azure.mgmt.paloaltonetworks.models.Category
+    :vartype category: ~azure.mgmt.paloaltonetworksngfw.models.Category
     :ivar protocol: any, application-default, TCP:number, UDP:number.
     :vartype protocol: str
     :ivar protocol_port_list: prot port list.
     :vartype protocol_port_list: list[str]
     :ivar inbound_inspection_certificate: inbound Inspection Certificate.
     :vartype inbound_inspection_certificate: str
     :ivar audit_comment: rule comment.
     :vartype audit_comment: str
     :ivar action_type: rule action. Known values are: "Allow", "DenySilent", "DenyResetServer", and
      "DenyResetBoth".
-    :vartype action_type: str or ~azure.mgmt.paloaltonetworks.models.ActionEnum
+    :vartype action_type: str or ~azure.mgmt.paloaltonetworksngfw.models.ActionEnum
     :ivar enable_logging: enable or disable logging. Known values are: "DISABLED" and "ENABLED".
-    :vartype enable_logging: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+    :vartype enable_logging: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
     :ivar decryption_rule_type: enable or disable decryption. Known values are:
      "SSLOutboundInspection", "SSLInboundInspection", and "None".
     :vartype decryption_rule_type: str or
-     ~azure.mgmt.paloaltonetworks.models.DecryptionRuleTypeEnum
+     ~azure.mgmt.paloaltonetworksngfw.models.DecryptionRuleTypeEnum
     :ivar tags: tag for rule.
-    :vartype tags: list[~azure.mgmt.paloaltonetworks.models.TagInfo]
+    :vartype tags: list[~azure.mgmt.paloaltonetworksngfw.models.TagInfo]
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -2256,46 +2357,46 @@
         :keyword etag: etag info.
         :paramtype etag: str
         :keyword rule_name: rule name. Required.
         :paramtype rule_name: str
         :keyword description: rule description.
         :paramtype description: str
         :keyword rule_state: state of this rule. Known values are: "DISABLED" and "ENABLED".
-        :paramtype rule_state: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+        :paramtype rule_state: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
         :keyword source: source address.
-        :paramtype source: ~azure.mgmt.paloaltonetworks.models.SourceAddr
+        :paramtype source: ~azure.mgmt.paloaltonetworksngfw.models.SourceAddr
         :keyword negate_source: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-        :paramtype negate_source: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype negate_source: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword destination: destination address.
-        :paramtype destination: ~azure.mgmt.paloaltonetworks.models.DestinationAddr
+        :paramtype destination: ~azure.mgmt.paloaltonetworksngfw.models.DestinationAddr
         :keyword negate_destination: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-        :paramtype negate_destination: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype negate_destination: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword applications: array of rule applications.
         :paramtype applications: list[str]
         :keyword category: rule category.
-        :paramtype category: ~azure.mgmt.paloaltonetworks.models.Category
+        :paramtype category: ~azure.mgmt.paloaltonetworksngfw.models.Category
         :keyword protocol: any, application-default, TCP:number, UDP:number.
         :paramtype protocol: str
         :keyword protocol_port_list: prot port list.
         :paramtype protocol_port_list: list[str]
         :keyword inbound_inspection_certificate: inbound Inspection Certificate.
         :paramtype inbound_inspection_certificate: str
         :keyword audit_comment: rule comment.
         :paramtype audit_comment: str
         :keyword action_type: rule action. Known values are: "Allow", "DenySilent", "DenyResetServer",
          and "DenyResetBoth".
-        :paramtype action_type: str or ~azure.mgmt.paloaltonetworks.models.ActionEnum
+        :paramtype action_type: str or ~azure.mgmt.paloaltonetworksngfw.models.ActionEnum
         :keyword enable_logging: enable or disable logging. Known values are: "DISABLED" and "ENABLED".
-        :paramtype enable_logging: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+        :paramtype enable_logging: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
         :keyword decryption_rule_type: enable or disable decryption. Known values are:
          "SSLOutboundInspection", "SSLInboundInspection", and "None".
         :paramtype decryption_rule_type: str or
-         ~azure.mgmt.paloaltonetworks.models.DecryptionRuleTypeEnum
+         ~azure.mgmt.paloaltonetworksngfw.models.DecryptionRuleTypeEnum
         :keyword tags: tag for rule.
-        :paramtype tags: list[~azure.mgmt.paloaltonetworks.models.TagInfo]
+        :paramtype tags: list[~azure.mgmt.paloaltonetworksngfw.models.TagInfo]
         """
         super().__init__(**kwargs)
         self.etag = etag
         self.rule_name = rule_name
         self.priority = None
         self.description = description
         self.rule_state = rule_state
@@ -2318,15 +2419,15 @@
 
 class LocalRulesResourceListResult(_serialization.Model):
     """The response of a LocalRulesResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -2337,15 +2438,15 @@
     }
 
     def __init__(
         self, *, value: List["_models.LocalRulesResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.LocalRulesResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.LocalRulesResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -2363,43 +2464,43 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     :ivar identity: The managed service identities assigned to this resource.
     :vartype identity:
-     ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+     ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
     :ivar pan_etag: PanEtag info.
     :vartype pan_etag: str
     :ivar pan_location: Rulestack Location, Required for GlobalRulestacks, Not for LocalRulestacks.
     :vartype pan_location: str
-    :ivar scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-    :vartype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+    :ivar scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+    :vartype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
     :ivar associated_subscriptions: subscription scope of global rulestack.
     :vartype associated_subscriptions: list[str]
     :ivar description: rulestack description.
     :vartype description: str
     :ivar default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL", and
      "NONE".
-    :vartype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+    :vartype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
     :ivar min_app_id_version: minimum version.
     :vartype min_app_id_version: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     :ivar security_services: Security Profile.
-    :vartype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+    :vartype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -2445,33 +2546,33 @@
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword identity: The managed service identities assigned to this resource.
         :paramtype identity:
-         ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
         :keyword pan_etag: PanEtag info.
         :paramtype pan_etag: str
         :keyword pan_location: Rulestack Location, Required for GlobalRulestacks, Not for
          LocalRulestacks.
         :paramtype pan_location: str
-        :keyword scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-        :paramtype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+        :keyword scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+        :paramtype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
         :keyword associated_subscriptions: subscription scope of global rulestack.
         :paramtype associated_subscriptions: list[str]
         :keyword description: rulestack description.
         :paramtype description: str
         :keyword default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL",
          and "NONE".
-        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
         :keyword min_app_id_version: minimum version.
         :paramtype min_app_id_version: str
         :keyword security_services: Security Profile.
-        :paramtype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+        :paramtype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.identity = identity
         self.pan_etag = pan_etag
         self.pan_location = pan_location
         self.scope = scope
         self.associated_subscriptions = associated_subscriptions
@@ -2484,15 +2585,15 @@
 
 class LocalRulestackResourceListResult(_serialization.Model):
     """The response of a LocalRulestackResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -2503,33 +2604,34 @@
     }
 
     def __init__(
         self, *, value: List["_models.LocalRulestackResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.LocalRulestackResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class LocalRulestackResourceUpdate(_serialization.Model):
     """The type used for update operations of the LocalRulestackResource.
 
     :ivar identity: The managed service identities assigned to this resource.
     :vartype identity:
-     ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+     ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar properties: The updatable properties of the LocalRulestackResource.
-    :vartype properties: ~azure.mgmt.paloaltonetworks.models.LocalRulestackResourceUpdateProperties
+    :vartype properties:
+     ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResourceUpdateProperties
     """
 
     _attribute_map = {
         "identity": {"key": "identity", "type": "AzureResourceManagerManagedIdentityProperties"},
         "tags": {"key": "tags", "type": "{str}"},
         "properties": {"key": "properties", "type": "LocalRulestackResourceUpdateProperties"},
     }
@@ -2541,47 +2643,47 @@
         tags: Optional[Dict[str, str]] = None,
         properties: Optional["_models.LocalRulestackResourceUpdateProperties"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword identity: The managed service identities assigned to this resource.
         :paramtype identity:
-         ~azure.mgmt.paloaltonetworks.models.AzureResourceManagerManagedIdentityProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.AzureResourceManagerManagedIdentityProperties
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword properties: The updatable properties of the LocalRulestackResource.
         :paramtype properties:
-         ~azure.mgmt.paloaltonetworks.models.LocalRulestackResourceUpdateProperties
+         ~azure.mgmt.paloaltonetworksngfw.models.LocalRulestackResourceUpdateProperties
         """
         super().__init__(**kwargs)
         self.identity = identity
         self.tags = tags
         self.properties = properties
 
 
 class LocalRulestackResourceUpdateProperties(_serialization.Model):
     """The updatable properties of the LocalRulestackResource.
 
     :ivar pan_etag: PanEtag info.
     :vartype pan_etag: str
     :ivar pan_location: Rulestack Location, Required for GlobalRulestacks, Not for LocalRulestacks.
     :vartype pan_location: str
-    :ivar scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-    :vartype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+    :ivar scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+    :vartype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
     :ivar associated_subscriptions: subscription scope of global rulestack.
     :vartype associated_subscriptions: list[str]
     :ivar description: rulestack description.
     :vartype description: str
     :ivar default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL", and
      "NONE".
-    :vartype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+    :vartype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
     :ivar min_app_id_version: minimum version.
     :vartype min_app_id_version: str
     :ivar security_services: Security Profile.
-    :vartype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+    :vartype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
     """
 
     _attribute_map = {
         "pan_etag": {"key": "panEtag", "type": "str"},
         "pan_location": {"key": "panLocation", "type": "str"},
         "scope": {"key": "scope", "type": "str"},
         "associated_subscriptions": {"key": "associatedSubscriptions", "type": "[str]"},
@@ -2606,27 +2708,27 @@
     ) -> None:
         """
         :keyword pan_etag: PanEtag info.
         :paramtype pan_etag: str
         :keyword pan_location: Rulestack Location, Required for GlobalRulestacks, Not for
          LocalRulestacks.
         :paramtype pan_location: str
-        :keyword scope: Rulestack Type. Known values are: "LOCAL" and "GLOBAL".
-        :paramtype scope: str or ~azure.mgmt.paloaltonetworks.models.ScopeType
+        :keyword scope: Rulestack Type. Known values are: "LOCAL", "GLOBAL", and "GLOBAL".
+        :paramtype scope: str or ~azure.mgmt.paloaltonetworksngfw.models.ScopeType
         :keyword associated_subscriptions: subscription scope of global rulestack.
         :paramtype associated_subscriptions: list[str]
         :keyword description: rulestack description.
         :paramtype description: str
         :keyword default_mode: Mode for default rules creation. Known values are: "IPS", "FIREWALL",
          and "NONE".
-        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworks.models.DefaultMode
+        :paramtype default_mode: str or ~azure.mgmt.paloaltonetworksngfw.models.DefaultMode
         :keyword min_app_id_version: minimum version.
         :paramtype min_app_id_version: str
         :keyword security_services: Security Profile.
-        :paramtype security_services: ~azure.mgmt.paloaltonetworks.models.SecurityServices
+        :paramtype security_services: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServices
         """
         super().__init__(**kwargs)
         self.pan_etag = pan_etag
         self.pan_location = pan_location
         self.scope = scope
         self.associated_subscriptions = associated_subscriptions
         self.description = description
@@ -2635,19 +2737,19 @@
         self.security_services = security_services
 
 
 class LogDestination(_serialization.Model):
     """Log Destination.
 
     :ivar storage_configurations: Storage account configurations.
-    :vartype storage_configurations: ~azure.mgmt.paloaltonetworks.models.StorageAccount
+    :vartype storage_configurations: ~azure.mgmt.paloaltonetworksngfw.models.StorageAccount
     :ivar event_hub_configurations: Event Hub configurations.
-    :vartype event_hub_configurations: ~azure.mgmt.paloaltonetworks.models.EventHub
+    :vartype event_hub_configurations: ~azure.mgmt.paloaltonetworksngfw.models.EventHub
     :ivar monitor_configurations: Monitor Log configurations.
-    :vartype monitor_configurations: ~azure.mgmt.paloaltonetworks.models.MonitorLog
+    :vartype monitor_configurations: ~azure.mgmt.paloaltonetworksngfw.models.MonitorLog
     """
 
     _attribute_map = {
         "storage_configurations": {"key": "storageConfigurations", "type": "StorageAccount"},
         "event_hub_configurations": {"key": "eventHubConfigurations", "type": "EventHub"},
         "monitor_configurations": {"key": "monitorConfigurations", "type": "MonitorLog"},
     }
@@ -2658,45 +2760,45 @@
         storage_configurations: Optional["_models.StorageAccount"] = None,
         event_hub_configurations: Optional["_models.EventHub"] = None,
         monitor_configurations: Optional["_models.MonitorLog"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword storage_configurations: Storage account configurations.
-        :paramtype storage_configurations: ~azure.mgmt.paloaltonetworks.models.StorageAccount
+        :paramtype storage_configurations: ~azure.mgmt.paloaltonetworksngfw.models.StorageAccount
         :keyword event_hub_configurations: Event Hub configurations.
-        :paramtype event_hub_configurations: ~azure.mgmt.paloaltonetworks.models.EventHub
+        :paramtype event_hub_configurations: ~azure.mgmt.paloaltonetworksngfw.models.EventHub
         :keyword monitor_configurations: Monitor Log configurations.
-        :paramtype monitor_configurations: ~azure.mgmt.paloaltonetworks.models.MonitorLog
+        :paramtype monitor_configurations: ~azure.mgmt.paloaltonetworksngfw.models.MonitorLog
         """
         super().__init__(**kwargs)
         self.storage_configurations = storage_configurations
         self.event_hub_configurations = event_hub_configurations
         self.monitor_configurations = monitor_configurations
 
 
 class LogSettings(_serialization.Model):
     """Log Settings for Firewall.
 
     :ivar log_type: One of possible log type. Known values are: "TRAFFIC", "THREAT", "DECRYPTION",
      "WILDFIRE", "DLP", and "AUDIT".
-    :vartype log_type: str or ~azure.mgmt.paloaltonetworks.models.LogType
+    :vartype log_type: str or ~azure.mgmt.paloaltonetworksngfw.models.LogType
     :ivar log_option: Log option SAME/INDIVIDUAL. Known values are: "SAME_DESTINATION" and
      "INDIVIDUAL_DESTINATION".
-    :vartype log_option: str or ~azure.mgmt.paloaltonetworks.models.LogOption
+    :vartype log_option: str or ~azure.mgmt.paloaltonetworksngfw.models.LogOption
     :ivar application_insights: Application Insight details.
-    :vartype application_insights: ~azure.mgmt.paloaltonetworks.models.ApplicationInsights
+    :vartype application_insights: ~azure.mgmt.paloaltonetworksngfw.models.ApplicationInsights
     :ivar common_destination: Common destination configurations.
-    :vartype common_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+    :vartype common_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
     :ivar traffic_log_destination: Traffic destination configurations.
-    :vartype traffic_log_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+    :vartype traffic_log_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
     :ivar threat_log_destination: Threat destination configurations.
-    :vartype threat_log_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+    :vartype threat_log_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
     :ivar decrypt_log_destination: Decrypt destination configurations.
-    :vartype decrypt_log_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+    :vartype decrypt_log_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
     """
 
     _attribute_map = {
         "log_type": {"key": "logType", "type": "str"},
         "log_option": {"key": "logOption", "type": "str"},
         "application_insights": {"key": "applicationInsights", "type": "ApplicationInsights"},
         "common_destination": {"key": "commonDestination", "type": "LogDestination"},
@@ -2716,28 +2818,28 @@
         threat_log_destination: Optional["_models.LogDestination"] = None,
         decrypt_log_destination: Optional["_models.LogDestination"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword log_type: One of possible log type. Known values are: "TRAFFIC", "THREAT",
          "DECRYPTION", "WILDFIRE", "DLP", and "AUDIT".
-        :paramtype log_type: str or ~azure.mgmt.paloaltonetworks.models.LogType
+        :paramtype log_type: str or ~azure.mgmt.paloaltonetworksngfw.models.LogType
         :keyword log_option: Log option SAME/INDIVIDUAL. Known values are: "SAME_DESTINATION" and
          "INDIVIDUAL_DESTINATION".
-        :paramtype log_option: str or ~azure.mgmt.paloaltonetworks.models.LogOption
+        :paramtype log_option: str or ~azure.mgmt.paloaltonetworksngfw.models.LogOption
         :keyword application_insights: Application Insight details.
-        :paramtype application_insights: ~azure.mgmt.paloaltonetworks.models.ApplicationInsights
+        :paramtype application_insights: ~azure.mgmt.paloaltonetworksngfw.models.ApplicationInsights
         :keyword common_destination: Common destination configurations.
-        :paramtype common_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+        :paramtype common_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
         :keyword traffic_log_destination: Traffic destination configurations.
-        :paramtype traffic_log_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+        :paramtype traffic_log_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
         :keyword threat_log_destination: Threat destination configurations.
-        :paramtype threat_log_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+        :paramtype threat_log_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
         :keyword decrypt_log_destination: Decrypt destination configurations.
-        :paramtype decrypt_log_destination: ~azure.mgmt.paloaltonetworks.models.LogDestination
+        :paramtype decrypt_log_destination: ~azure.mgmt.paloaltonetworksngfw.models.LogDestination
         """
         super().__init__(**kwargs)
         self.log_type = log_type
         self.log_option = log_option
         self.application_insights = application_insights
         self.common_destination = common_destination
         self.traffic_log_destination = traffic_log_destination
@@ -2758,15 +2860,15 @@
     :vartype offer_id: str
     :ivar publisher_id: Publisher Id. Required.
     :vartype publisher_id: str
     :ivar marketplace_subscription_status: Marketplace Subscription Status. Known values are:
      "PendingFulfillmentStart", "Subscribed", "Suspended", "Unsubscribed", "NotStarted", and
      "FulfillmentRequested".
     :vartype marketplace_subscription_status: str or
-     ~azure.mgmt.paloaltonetworks.models.MarketplaceSubscriptionStatus
+     ~azure.mgmt.paloaltonetworksngfw.models.MarketplaceSubscriptionStatus
     """
 
     _validation = {
         "marketplace_subscription_id": {"readonly": True},
         "offer_id": {"required": True},
         "publisher_id": {"required": True},
     }
@@ -2791,15 +2893,15 @@
         :paramtype offer_id: str
         :keyword publisher_id: Publisher Id. Required.
         :paramtype publisher_id: str
         :keyword marketplace_subscription_status: Marketplace Subscription Status. Known values are:
          "PendingFulfillmentStart", "Subscribed", "Suspended", "Unsubscribed", "NotStarted", and
          "FulfillmentRequested".
         :paramtype marketplace_subscription_status: str or
-         ~azure.mgmt.paloaltonetworks.models.MarketplaceSubscriptionStatus
+         ~azure.mgmt.paloaltonetworksngfw.models.MarketplaceSubscriptionStatus
         """
         super().__init__(**kwargs)
         self.marketplace_subscription_id = None
         self.offer_id = offer_id
         self.publisher_id = publisher_id
         self.marketplace_subscription_status = marketplace_subscription_status
 
@@ -2891,27 +2993,27 @@
 
 class NetworkProfile(_serialization.Model):
     """Network settings for Firewall.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar vnet_configuration: Vnet configurations.
-    :vartype vnet_configuration: ~azure.mgmt.paloaltonetworks.models.VnetConfiguration
+    :vartype vnet_configuration: ~azure.mgmt.paloaltonetworksngfw.models.VnetConfiguration
     :ivar vwan_configuration: Vwan configurations.
-    :vartype vwan_configuration: ~azure.mgmt.paloaltonetworks.models.VwanConfiguration
+    :vartype vwan_configuration: ~azure.mgmt.paloaltonetworksngfw.models.VwanConfiguration
     :ivar network_type: vnet or vwan, cannot be updated. Required. Known values are: "VNET" and
      "VWAN".
-    :vartype network_type: str or ~azure.mgmt.paloaltonetworks.models.NetworkType
+    :vartype network_type: str or ~azure.mgmt.paloaltonetworksngfw.models.NetworkType
     :ivar public_ips: List of IPs associated with the Firewall. Required.
-    :vartype public_ips: list[~azure.mgmt.paloaltonetworks.models.IPAddress]
+    :vartype public_ips: list[~azure.mgmt.paloaltonetworksngfw.models.IPAddress]
     :ivar enable_egress_nat: Enable egress NAT, enabled by default. Required. Known values are:
      "DISABLED" and "ENABLED".
-    :vartype enable_egress_nat: str or ~azure.mgmt.paloaltonetworks.models.EgressNat
+    :vartype enable_egress_nat: str or ~azure.mgmt.paloaltonetworksngfw.models.EgressNat
     :ivar egress_nat_ip: Egress nat IP to use.
-    :vartype egress_nat_ip: list[~azure.mgmt.paloaltonetworks.models.IPAddress]
+    :vartype egress_nat_ip: list[~azure.mgmt.paloaltonetworksngfw.models.IPAddress]
     """
 
     _validation = {
         "network_type": {"required": True},
         "public_ips": {"required": True},
         "enable_egress_nat": {"required": True},
     }
@@ -2934,27 +3036,27 @@
         vnet_configuration: Optional["_models.VnetConfiguration"] = None,
         vwan_configuration: Optional["_models.VwanConfiguration"] = None,
         egress_nat_ip: Optional[List["_models.IPAddress"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword vnet_configuration: Vnet configurations.
-        :paramtype vnet_configuration: ~azure.mgmt.paloaltonetworks.models.VnetConfiguration
+        :paramtype vnet_configuration: ~azure.mgmt.paloaltonetworksngfw.models.VnetConfiguration
         :keyword vwan_configuration: Vwan configurations.
-        :paramtype vwan_configuration: ~azure.mgmt.paloaltonetworks.models.VwanConfiguration
+        :paramtype vwan_configuration: ~azure.mgmt.paloaltonetworksngfw.models.VwanConfiguration
         :keyword network_type: vnet or vwan, cannot be updated. Required. Known values are: "VNET" and
          "VWAN".
-        :paramtype network_type: str or ~azure.mgmt.paloaltonetworks.models.NetworkType
+        :paramtype network_type: str or ~azure.mgmt.paloaltonetworksngfw.models.NetworkType
         :keyword public_ips: List of IPs associated with the Firewall. Required.
-        :paramtype public_ips: list[~azure.mgmt.paloaltonetworks.models.IPAddress]
+        :paramtype public_ips: list[~azure.mgmt.paloaltonetworksngfw.models.IPAddress]
         :keyword enable_egress_nat: Enable egress NAT, enabled by default. Required. Known values are:
          "DISABLED" and "ENABLED".
-        :paramtype enable_egress_nat: str or ~azure.mgmt.paloaltonetworks.models.EgressNat
+        :paramtype enable_egress_nat: str or ~azure.mgmt.paloaltonetworksngfw.models.EgressNat
         :keyword egress_nat_ip: Egress nat IP to use.
-        :paramtype egress_nat_ip: list[~azure.mgmt.paloaltonetworks.models.IPAddress]
+        :paramtype egress_nat_ip: list[~azure.mgmt.paloaltonetworksngfw.models.IPAddress]
         """
         super().__init__(**kwargs)
         self.vnet_configuration = vnet_configuration
         self.vwan_configuration = vwan_configuration
         self.network_type = network_type
         self.public_ips = public_ips
         self.enable_egress_nat = enable_egress_nat
@@ -2969,22 +3071,22 @@
     :ivar name: The name of the operation, as per Resource-Based Access Control (RBAC). Examples:
      "Microsoft.Compute/virtualMachines/write", "Microsoft.Compute/virtualMachines/capture/action".
     :vartype name: str
     :ivar is_data_action: Whether the operation applies to data-plane. This is "true" for
      data-plane operations and "false" for ARM/control-plane operations.
     :vartype is_data_action: bool
     :ivar display: Localized display information for this particular operation.
-    :vartype display: ~azure.mgmt.paloaltonetworks.models.OperationDisplay
+    :vartype display: ~azure.mgmt.paloaltonetworksngfw.models.OperationDisplay
     :ivar origin: The intended executor of the operation; as in Resource Based Access Control
      (RBAC) and audit logs UX. Default value is "user,system". Known values are: "user", "system",
      and "user,system".
-    :vartype origin: str or ~azure.mgmt.paloaltonetworks.models.Origin
+    :vartype origin: str or ~azure.mgmt.paloaltonetworksngfw.models.Origin
     :ivar action_type: Enum. Indicates the action type. "Internal" refers to actions that are for
      internal only APIs. "Internal"
-    :vartype action_type: str or ~azure.mgmt.paloaltonetworks.models.ActionType
+    :vartype action_type: str or ~azure.mgmt.paloaltonetworksngfw.models.ActionType
     """
 
     _validation = {
         "name": {"readonly": True},
         "is_data_action": {"readonly": True},
         "origin": {"readonly": True},
         "action_type": {"readonly": True},
@@ -2997,15 +3099,15 @@
         "origin": {"key": "origin", "type": "str"},
         "action_type": {"key": "actionType", "type": "str"},
     }
 
     def __init__(self, *, display: Optional["_models.OperationDisplay"] = None, **kwargs: Any) -> None:
         """
         :keyword display: Localized display information for this particular operation.
-        :paramtype display: ~azure.mgmt.paloaltonetworks.models.OperationDisplay
+        :paramtype display: ~azure.mgmt.paloaltonetworksngfw.models.OperationDisplay
         """
         super().__init__(**kwargs)
         self.name = None
         self.is_data_action = None
         self.display = display
         self.origin = None
         self.action_type = None
@@ -3056,15 +3158,15 @@
 class OperationListResult(_serialization.Model):
     """A list of REST API operations supported by an Azure Resource Provider. It contains an URL link
     to get the next set of results.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: List of operations supported by the resource provider.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.Operation]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.Operation]
     :ivar next_link: URL to get the next set of operation list results (if there are any).
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"readonly": True},
         "next_link": {"readonly": True},
@@ -3145,27 +3247,57 @@
         self.panorama_server2 = None
         self.dg_name = None
         self.tpl_name = None
         self.cg_name = None
         self.host_name = None
 
 
+class PanoramaStatus(_serialization.Model):
+    """Panorama connectivity information.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar panorama_server_status: Primary Panorama connection status. Known values are: "UP" and
+     "DOWN".
+    :vartype panorama_server_status: str or ~azure.mgmt.paloaltonetworksngfw.models.ServerStatus
+    :ivar panorama_server2_status: Secondary Panorama connection status. Known values are: "UP" and
+     "DOWN".
+    :vartype panorama_server2_status: str or ~azure.mgmt.paloaltonetworksngfw.models.ServerStatus
+    """
+
+    _validation = {
+        "panorama_server_status": {"readonly": True},
+        "panorama_server2_status": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "panorama_server_status": {"key": "panoramaServerStatus", "type": "str"},
+        "panorama_server2_status": {"key": "panoramaServer2Status", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.panorama_server_status = None
+        self.panorama_server2_status = None
+
+
 class PlanData(_serialization.Model):
     """Billing plan information.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar usage_type: different usage type like PAYG/COMMITTED. Known values are: "PAYG" and
      "COMMITTED".
-    :vartype usage_type: str or ~azure.mgmt.paloaltonetworks.models.UsageType
+    :vartype usage_type: str or ~azure.mgmt.paloaltonetworksngfw.models.UsageType
     :ivar billing_cycle: different billing cycles like MONTHLY/WEEKLY. Required. Known values are:
      "WEEKLY" and "MONTHLY".
-    :vartype billing_cycle: str or ~azure.mgmt.paloaltonetworks.models.BillingCycle
+    :vartype billing_cycle: str or ~azure.mgmt.paloaltonetworksngfw.models.BillingCycle
     :ivar plan_id: plan id as published by Liftr.PAN. Required.
     :vartype plan_id: str
     :ivar effective_date: date when plan was applied.
     :vartype effective_date: ~datetime.datetime
     """
 
     _validation = {
@@ -3188,18 +3320,18 @@
         plan_id: str,
         usage_type: Optional[Union[str, "_models.UsageType"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword usage_type: different usage type like PAYG/COMMITTED. Known values are: "PAYG" and
          "COMMITTED".
-        :paramtype usage_type: str or ~azure.mgmt.paloaltonetworks.models.UsageType
+        :paramtype usage_type: str or ~azure.mgmt.paloaltonetworksngfw.models.UsageType
         :keyword billing_cycle: different billing cycles like MONTHLY/WEEKLY. Required. Known values
          are: "WEEKLY" and "MONTHLY".
-        :paramtype billing_cycle: str or ~azure.mgmt.paloaltonetworks.models.BillingCycle
+        :paramtype billing_cycle: str or ~azure.mgmt.paloaltonetworksngfw.models.BillingCycle
         :keyword plan_id: plan id as published by Liftr.PAN. Required.
         :paramtype plan_id: str
         """
         super().__init__(**kwargs)
         self.usage_type = usage_type
         self.billing_cycle = billing_cycle
         self.plan_id = plan_id
@@ -3219,60 +3351,60 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar etag: etag info.
     :vartype etag: str
     :ivar rule_name: rule name. Required.
     :vartype rule_name: str
     :ivar priority:
     :vartype priority: int
     :ivar description: rule description.
     :vartype description: str
     :ivar rule_state: state of this rule. Known values are: "DISABLED" and "ENABLED".
-    :vartype rule_state: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+    :vartype rule_state: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
     :ivar source: source address.
-    :vartype source: ~azure.mgmt.paloaltonetworks.models.SourceAddr
+    :vartype source: ~azure.mgmt.paloaltonetworksngfw.models.SourceAddr
     :ivar negate_source: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-    :vartype negate_source: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype negate_source: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar destination: destination address.
-    :vartype destination: ~azure.mgmt.paloaltonetworks.models.DestinationAddr
+    :vartype destination: ~azure.mgmt.paloaltonetworksngfw.models.DestinationAddr
     :ivar negate_destination: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-    :vartype negate_destination: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype negate_destination: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar applications: array of rule applications.
     :vartype applications: list[str]
     :ivar category: rule category.
-    :vartype category: ~azure.mgmt.paloaltonetworks.models.Category
+    :vartype category: ~azure.mgmt.paloaltonetworksngfw.models.Category
     :ivar protocol: any, application-default, TCP:number, UDP:number.
     :vartype protocol: str
     :ivar protocol_port_list: prot port list.
     :vartype protocol_port_list: list[str]
     :ivar inbound_inspection_certificate: inbound Inspection Certificate.
     :vartype inbound_inspection_certificate: str
     :ivar audit_comment: rule comment.
     :vartype audit_comment: str
     :ivar action_type: rule action. Known values are: "Allow", "DenySilent", "DenyResetServer", and
      "DenyResetBoth".
-    :vartype action_type: str or ~azure.mgmt.paloaltonetworks.models.ActionEnum
+    :vartype action_type: str or ~azure.mgmt.paloaltonetworksngfw.models.ActionEnum
     :ivar enable_logging: enable or disable logging. Known values are: "DISABLED" and "ENABLED".
-    :vartype enable_logging: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+    :vartype enable_logging: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
     :ivar decryption_rule_type: enable or disable decryption. Known values are:
      "SSLOutboundInspection", "SSLInboundInspection", and "None".
     :vartype decryption_rule_type: str or
-     ~azure.mgmt.paloaltonetworks.models.DecryptionRuleTypeEnum
+     ~azure.mgmt.paloaltonetworksngfw.models.DecryptionRuleTypeEnum
     :ivar tags: tag for rule.
-    :vartype tags: list[~azure.mgmt.paloaltonetworks.models.TagInfo]
+    :vartype tags: list[~azure.mgmt.paloaltonetworksngfw.models.TagInfo]
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -3335,46 +3467,46 @@
         :keyword etag: etag info.
         :paramtype etag: str
         :keyword rule_name: rule name. Required.
         :paramtype rule_name: str
         :keyword description: rule description.
         :paramtype description: str
         :keyword rule_state: state of this rule. Known values are: "DISABLED" and "ENABLED".
-        :paramtype rule_state: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+        :paramtype rule_state: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
         :keyword source: source address.
-        :paramtype source: ~azure.mgmt.paloaltonetworks.models.SourceAddr
+        :paramtype source: ~azure.mgmt.paloaltonetworksngfw.models.SourceAddr
         :keyword negate_source: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-        :paramtype negate_source: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype negate_source: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword destination: destination address.
-        :paramtype destination: ~azure.mgmt.paloaltonetworks.models.DestinationAddr
+        :paramtype destination: ~azure.mgmt.paloaltonetworksngfw.models.DestinationAddr
         :keyword negate_destination: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-        :paramtype negate_destination: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype negate_destination: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword applications: array of rule applications.
         :paramtype applications: list[str]
         :keyword category: rule category.
-        :paramtype category: ~azure.mgmt.paloaltonetworks.models.Category
+        :paramtype category: ~azure.mgmt.paloaltonetworksngfw.models.Category
         :keyword protocol: any, application-default, TCP:number, UDP:number.
         :paramtype protocol: str
         :keyword protocol_port_list: prot port list.
         :paramtype protocol_port_list: list[str]
         :keyword inbound_inspection_certificate: inbound Inspection Certificate.
         :paramtype inbound_inspection_certificate: str
         :keyword audit_comment: rule comment.
         :paramtype audit_comment: str
         :keyword action_type: rule action. Known values are: "Allow", "DenySilent", "DenyResetServer",
          and "DenyResetBoth".
-        :paramtype action_type: str or ~azure.mgmt.paloaltonetworks.models.ActionEnum
+        :paramtype action_type: str or ~azure.mgmt.paloaltonetworksngfw.models.ActionEnum
         :keyword enable_logging: enable or disable logging. Known values are: "DISABLED" and "ENABLED".
-        :paramtype enable_logging: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+        :paramtype enable_logging: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
         :keyword decryption_rule_type: enable or disable decryption. Known values are:
          "SSLOutboundInspection", "SSLInboundInspection", and "None".
         :paramtype decryption_rule_type: str or
-         ~azure.mgmt.paloaltonetworks.models.DecryptionRuleTypeEnum
+         ~azure.mgmt.paloaltonetworksngfw.models.DecryptionRuleTypeEnum
         :keyword tags: tag for rule.
-        :paramtype tags: list[~azure.mgmt.paloaltonetworks.models.TagInfo]
+        :paramtype tags: list[~azure.mgmt.paloaltonetworksngfw.models.TagInfo]
         """
         super().__init__(**kwargs)
         self.etag = etag
         self.rule_name = rule_name
         self.priority = None
         self.description = description
         self.rule_state = rule_state
@@ -3397,15 +3529,15 @@
 
 class PostRulesResourceListResult(_serialization.Model):
     """The response of a PostRulesResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -3416,30 +3548,30 @@
     }
 
     def __init__(
         self, *, value: List["_models.PostRulesResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.PostRulesResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.PostRulesResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class PredefinedUrlCategoriesResponse(_serialization.Model):
     """predefined url categories response.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: predefined url categories. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.PredefinedUrlCategory]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.PredefinedUrlCategory]
     :ivar next_link: next link.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -3450,15 +3582,15 @@
     }
 
     def __init__(
         self, *, value: List["_models.PredefinedUrlCategory"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: predefined url categories. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.PredefinedUrlCategory]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.PredefinedUrlCategory]
         :keyword next_link: next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -3509,27 +3641,27 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar description: prefix description.
     :vartype description: str
     :ivar prefix_list: prefix list. Required.
     :vartype prefix_list: list[str]
     :ivar etag: etag info.
     :vartype etag: str
     :ivar audit_comment: comment for this object.
     :vartype audit_comment: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -3578,15 +3710,15 @@
 
 class PrefixListGlobalRulestackResourceListResult(_serialization.Model):
     """The response of a PrefixListGlobalRulestackResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -3601,15 +3733,16 @@
         *,
         value: List["_models.PrefixListGlobalRulestackResource"],
         next_link: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.PrefixListGlobalRulestackResource]
+        :paramtype value:
+         list[~azure.mgmt.paloaltonetworksngfw.models.PrefixListGlobalRulestackResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -3627,27 +3760,27 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar description: prefix description.
     :vartype description: str
     :ivar prefix_list: prefix list. Required.
     :vartype prefix_list: list[str]
     :ivar etag: etag info.
     :vartype etag: str
     :ivar audit_comment: comment for this object.
     :vartype audit_comment: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -3696,15 +3829,15 @@
 
 class PrefixListResourceListResult(_serialization.Model):
     """The response of a PrefixListResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -3715,15 +3848,15 @@
     }
 
     def __init__(
         self, *, value: List["_models.PrefixListResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.PrefixListResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.PrefixListResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -3741,60 +3874,60 @@
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
-    :vartype system_data: ~azure.mgmt.paloaltonetworks.models.SystemData
+    :vartype system_data: ~azure.mgmt.paloaltonetworksngfw.models.SystemData
     :ivar etag: etag info.
     :vartype etag: str
     :ivar rule_name: rule name. Required.
     :vartype rule_name: str
     :ivar priority:
     :vartype priority: int
     :ivar description: rule description.
     :vartype description: str
     :ivar rule_state: state of this rule. Known values are: "DISABLED" and "ENABLED".
-    :vartype rule_state: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+    :vartype rule_state: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
     :ivar source: source address.
-    :vartype source: ~azure.mgmt.paloaltonetworks.models.SourceAddr
+    :vartype source: ~azure.mgmt.paloaltonetworksngfw.models.SourceAddr
     :ivar negate_source: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-    :vartype negate_source: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype negate_source: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar destination: destination address.
-    :vartype destination: ~azure.mgmt.paloaltonetworks.models.DestinationAddr
+    :vartype destination: ~azure.mgmt.paloaltonetworksngfw.models.DestinationAddr
     :ivar negate_destination: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-    :vartype negate_destination: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype negate_destination: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar applications: array of rule applications.
     :vartype applications: list[str]
     :ivar category: rule category.
-    :vartype category: ~azure.mgmt.paloaltonetworks.models.Category
+    :vartype category: ~azure.mgmt.paloaltonetworksngfw.models.Category
     :ivar protocol: any, application-default, TCP:number, UDP:number.
     :vartype protocol: str
     :ivar protocol_port_list: prot port list.
     :vartype protocol_port_list: list[str]
     :ivar inbound_inspection_certificate: inbound Inspection Certificate.
     :vartype inbound_inspection_certificate: str
     :ivar audit_comment: rule comment.
     :vartype audit_comment: str
     :ivar action_type: rule action. Known values are: "Allow", "DenySilent", "DenyResetServer", and
      "DenyResetBoth".
-    :vartype action_type: str or ~azure.mgmt.paloaltonetworks.models.ActionEnum
+    :vartype action_type: str or ~azure.mgmt.paloaltonetworksngfw.models.ActionEnum
     :ivar enable_logging: enable or disable logging. Known values are: "DISABLED" and "ENABLED".
-    :vartype enable_logging: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+    :vartype enable_logging: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
     :ivar decryption_rule_type: enable or disable decryption. Known values are:
      "SSLOutboundInspection", "SSLInboundInspection", and "None".
     :vartype decryption_rule_type: str or
-     ~azure.mgmt.paloaltonetworks.models.DecryptionRuleTypeEnum
+     ~azure.mgmt.paloaltonetworksngfw.models.DecryptionRuleTypeEnum
     :ivar tags: tag for rule.
-    :vartype tags: list[~azure.mgmt.paloaltonetworks.models.TagInfo]
+    :vartype tags: list[~azure.mgmt.paloaltonetworksngfw.models.TagInfo]
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
      "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted", and
      "NotSpecified".
-    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworks.models.ProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.paloaltonetworksngfw.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -3857,46 +3990,46 @@
         :keyword etag: etag info.
         :paramtype etag: str
         :keyword rule_name: rule name. Required.
         :paramtype rule_name: str
         :keyword description: rule description.
         :paramtype description: str
         :keyword rule_state: state of this rule. Known values are: "DISABLED" and "ENABLED".
-        :paramtype rule_state: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+        :paramtype rule_state: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
         :keyword source: source address.
-        :paramtype source: ~azure.mgmt.paloaltonetworks.models.SourceAddr
+        :paramtype source: ~azure.mgmt.paloaltonetworksngfw.models.SourceAddr
         :keyword negate_source: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-        :paramtype negate_source: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype negate_source: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword destination: destination address.
-        :paramtype destination: ~azure.mgmt.paloaltonetworks.models.DestinationAddr
+        :paramtype destination: ~azure.mgmt.paloaltonetworksngfw.models.DestinationAddr
         :keyword negate_destination: cidr should not be 'any'. Known values are: "TRUE" and "FALSE".
-        :paramtype negate_destination: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype negate_destination: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword applications: array of rule applications.
         :paramtype applications: list[str]
         :keyword category: rule category.
-        :paramtype category: ~azure.mgmt.paloaltonetworks.models.Category
+        :paramtype category: ~azure.mgmt.paloaltonetworksngfw.models.Category
         :keyword protocol: any, application-default, TCP:number, UDP:number.
         :paramtype protocol: str
         :keyword protocol_port_list: prot port list.
         :paramtype protocol_port_list: list[str]
         :keyword inbound_inspection_certificate: inbound Inspection Certificate.
         :paramtype inbound_inspection_certificate: str
         :keyword audit_comment: rule comment.
         :paramtype audit_comment: str
         :keyword action_type: rule action. Known values are: "Allow", "DenySilent", "DenyResetServer",
          and "DenyResetBoth".
-        :paramtype action_type: str or ~azure.mgmt.paloaltonetworks.models.ActionEnum
+        :paramtype action_type: str or ~azure.mgmt.paloaltonetworksngfw.models.ActionEnum
         :keyword enable_logging: enable or disable logging. Known values are: "DISABLED" and "ENABLED".
-        :paramtype enable_logging: str or ~azure.mgmt.paloaltonetworks.models.StateEnum
+        :paramtype enable_logging: str or ~azure.mgmt.paloaltonetworksngfw.models.StateEnum
         :keyword decryption_rule_type: enable or disable decryption. Known values are:
          "SSLOutboundInspection", "SSLInboundInspection", and "None".
         :paramtype decryption_rule_type: str or
-         ~azure.mgmt.paloaltonetworks.models.DecryptionRuleTypeEnum
+         ~azure.mgmt.paloaltonetworksngfw.models.DecryptionRuleTypeEnum
         :keyword tags: tag for rule.
-        :paramtype tags: list[~azure.mgmt.paloaltonetworks.models.TagInfo]
+        :paramtype tags: list[~azure.mgmt.paloaltonetworksngfw.models.TagInfo]
         """
         super().__init__(**kwargs)
         self.etag = etag
         self.rule_name = rule_name
         self.priority = None
         self.description = description
         self.rule_state = rule_state
@@ -3919,15 +4052,15 @@
 
 class PreRulesResourceListResult(_serialization.Model):
     """The response of a PreRulesResource list operation.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: The items on this page. Required.
-    :vartype value: list[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+    :vartype value: list[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
     :ivar next_link: The link to the next page of items.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -3938,15 +4071,15 @@
     }
 
     def __init__(
         self, *, value: List["_models.PreRulesResource"], next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: The items on this page. Required.
-        :paramtype value: list[~azure.mgmt.paloaltonetworks.models.PreRulesResource]
+        :paramtype value: list[~azure.mgmt.paloaltonetworksngfw.models.PreRulesResource]
         :keyword next_link: The link to the next page of items.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -3965,15 +4098,15 @@
     :ivar firewall_name: firewall name.
     :vartype firewall_name: str
     :ivar rule_name: rule name. Required.
     :vartype rule_name: str
     :ivar hit_count: hit count.
     :vartype hit_count: int
     :ivar app_seen: apps seen.
-    :vartype app_seen: ~azure.mgmt.paloaltonetworks.models.AppSeenData
+    :vartype app_seen: ~azure.mgmt.paloaltonetworksngfw.models.AppSeenData
     :ivar timestamp: timestamp of response.
     :vartype timestamp: ~datetime.datetime
     :ivar request_timestamp: timestamp of request.
     :vartype request_timestamp: ~datetime.datetime
     :ivar last_updated_timestamp: last updated timestamp.
     :vartype last_updated_timestamp: ~datetime.datetime
     """
@@ -4021,15 +4154,15 @@
         :keyword firewall_name: firewall name.
         :paramtype firewall_name: str
         :keyword rule_name: rule name. Required.
         :paramtype rule_name: str
         :keyword hit_count: hit count.
         :paramtype hit_count: int
         :keyword app_seen: apps seen.
-        :paramtype app_seen: ~azure.mgmt.paloaltonetworks.models.AppSeenData
+        :paramtype app_seen: ~azure.mgmt.paloaltonetworksngfw.models.AppSeenData
         :keyword timestamp: timestamp of response.
         :paramtype timestamp: ~datetime.datetime
         :keyword request_timestamp: timestamp of request.
         :paramtype request_timestamp: ~datetime.datetime
         :keyword last_updated_timestamp: last updated timestamp.
         :paramtype last_updated_timestamp: ~datetime.datetime
         """
@@ -4217,15 +4350,15 @@
 
 class SecurityServicesResponse(_serialization.Model):
     """Security services list response.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar value: response value. Required.
-    :vartype value: ~azure.mgmt.paloaltonetworks.models.SecurityServicesTypeList
+    :vartype value: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesTypeList
     :ivar next_link: next link.
     :vartype next_link: str
     """
 
     _validation = {
         "value": {"required": True},
     }
@@ -4236,15 +4369,15 @@
     }
 
     def __init__(
         self, *, value: "_models.SecurityServicesTypeList", next_link: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword value: response value. Required.
-        :paramtype value: ~azure.mgmt.paloaltonetworks.models.SecurityServicesTypeList
+        :paramtype value: ~azure.mgmt.paloaltonetworksngfw.models.SecurityServicesTypeList
         :keyword next_link: next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
@@ -4253,15 +4386,15 @@
     """Security services type list.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: security services type.
     :vartype type: str
     :ivar entry: list. Required.
-    :vartype entry: list[~azure.mgmt.paloaltonetworks.models.NameDescriptionObject]
+    :vartype entry: list[~azure.mgmt.paloaltonetworksngfw.models.NameDescriptionObject]
     """
 
     _validation = {
         "entry": {"required": True},
     }
 
     _attribute_map = {
@@ -4272,15 +4405,15 @@
     def __init__(
         self, *, entry: List["_models.NameDescriptionObject"], type: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
         :keyword type: security services type.
         :paramtype type: str
         :keyword entry: list. Required.
-        :paramtype entry: list[~azure.mgmt.paloaltonetworks.models.NameDescriptionObject]
+        :paramtype entry: list[~azure.mgmt.paloaltonetworksngfw.models.NameDescriptionObject]
         """
         super().__init__(**kwargs)
         self.type = type
         self.entry = entry
 
 
 class SourceAddr(_serialization.Model):
@@ -4373,25 +4506,25 @@
 
     :ivar product_sku: product SKU associated with given resource.
     :vartype product_sku: str
     :ivar product_serial: product Serial associated with given resource.
     :vartype product_serial: str
     :ivar account_registered: account registered in Customer Support Portal. Known values are:
      "TRUE" and "FALSE".
-    :vartype account_registered: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype account_registered: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar account_id: Support account associated with given resource.
     :vartype account_id: str
     :ivar user_domain_supported: user domain is supported in Customer Support Portal. Known values
      are: "TRUE" and "FALSE".
-    :vartype user_domain_supported: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype user_domain_supported: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar user_registered: user registered in Customer Support Portal. Known values are: "TRUE" and
      "FALSE".
-    :vartype user_registered: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype user_registered: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar free_trial: Product usage is in free trial period. Known values are: "TRUE" and "FALSE".
-    :vartype free_trial: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+    :vartype free_trial: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
     :ivar free_trial_days_left: Free trial days remaining.
     :vartype free_trial_days_left: int
     :ivar free_trial_credit_left: Free trial credit remaining.
     :vartype free_trial_credit_left: int
     :ivar help_url: URL for paloaltonetworks live community.
     :vartype help_url: str
     :ivar support_url: URL for paloaltonetworks Customer Service Portal.
@@ -4435,26 +4568,26 @@
         """
         :keyword product_sku: product SKU associated with given resource.
         :paramtype product_sku: str
         :keyword product_serial: product Serial associated with given resource.
         :paramtype product_serial: str
         :keyword account_registered: account registered in Customer Support Portal. Known values are:
          "TRUE" and "FALSE".
-        :paramtype account_registered: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype account_registered: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword account_id: Support account associated with given resource.
         :paramtype account_id: str
         :keyword user_domain_supported: user domain is supported in Customer Support Portal. Known
          values are: "TRUE" and "FALSE".
-        :paramtype user_domain_supported: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype user_domain_supported: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword user_registered: user registered in Customer Support Portal. Known values are: "TRUE"
          and "FALSE".
-        :paramtype user_registered: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype user_registered: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword free_trial: Product usage is in free trial period. Known values are: "TRUE" and
          "FALSE".
-        :paramtype free_trial: str or ~azure.mgmt.paloaltonetworks.models.BooleanEnum
+        :paramtype free_trial: str or ~azure.mgmt.paloaltonetworksngfw.models.BooleanEnum
         :keyword free_trial_days_left: Free trial days remaining.
         :paramtype free_trial_days_left: int
         :keyword free_trial_credit_left: Free trial credit remaining.
         :paramtype free_trial_credit_left: int
         :keyword help_url: URL for paloaltonetworks live community.
         :paramtype help_url: str
         :keyword support_url: URL for paloaltonetworks Customer Service Portal.
@@ -4480,22 +4613,22 @@
 class SystemData(_serialization.Model):
     """Metadata pertaining to creation and last modification of the resource.
 
     :ivar created_by: The identity that created the resource.
     :vartype created_by: str
     :ivar created_by_type: The type of identity that created the resource. Known values are:
      "User", "Application", "ManagedIdentity", and "Key".
-    :vartype created_by_type: str or ~azure.mgmt.paloaltonetworks.models.CreatedByType
+    :vartype created_by_type: str or ~azure.mgmt.paloaltonetworksngfw.models.CreatedByType
     :ivar created_at: The timestamp of resource creation (UTC).
     :vartype created_at: ~datetime.datetime
     :ivar last_modified_by: The identity that last modified the resource.
     :vartype last_modified_by: str
     :ivar last_modified_by_type: The type of identity that last modified the resource. Known values
      are: "User", "Application", "ManagedIdentity", and "Key".
-    :vartype last_modified_by_type: str or ~azure.mgmt.paloaltonetworks.models.CreatedByType
+    :vartype last_modified_by_type: str or ~azure.mgmt.paloaltonetworksngfw.models.CreatedByType
     :ivar last_modified_at: The timestamp of resource last modification (UTC).
     :vartype last_modified_at: ~datetime.datetime
     """
 
     _attribute_map = {
         "created_by": {"key": "createdBy", "type": "str"},
         "created_by_type": {"key": "createdByType", "type": "str"},
@@ -4517,22 +4650,22 @@
         **kwargs: Any
     ) -> None:
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
         :keyword created_by_type: The type of identity that created the resource. Known values are:
          "User", "Application", "ManagedIdentity", and "Key".
-        :paramtype created_by_type: str or ~azure.mgmt.paloaltonetworks.models.CreatedByType
+        :paramtype created_by_type: str or ~azure.mgmt.paloaltonetworksngfw.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: The identity that last modified the resource.
         :paramtype last_modified_by: str
         :keyword last_modified_by_type: The type of identity that last modified the resource. Known
          values are: "User", "Application", "ManagedIdentity", and "Key".
-        :paramtype last_modified_by_type: str or ~azure.mgmt.paloaltonetworks.models.CreatedByType
+        :paramtype last_modified_by_type: str or ~azure.mgmt.paloaltonetworksngfw.models.CreatedByType
         :keyword last_modified_at: The timestamp of resource last modification (UTC).
         :paramtype last_modified_at: ~datetime.datetime
         """
         super().__init__(**kwargs)
         self.created_by = created_by
         self.created_by_type = created_by_type
         self.created_at = created_at
@@ -4576,21 +4709,21 @@
 
 class VnetConfiguration(_serialization.Model):
     """VnetInfo for Firewall Networking.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar vnet: Azure Virtual Network. Required.
-    :vartype vnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+    :vartype vnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
     :ivar trust_subnet: Trust Subnet. Required.
-    :vartype trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+    :vartype trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
     :ivar un_trust_subnet: Untrust Subnet. Required.
-    :vartype un_trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+    :vartype un_trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
     :ivar ip_of_trust_subnet_for_udr: IP of trust subnet for UDR.
-    :vartype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworks.models.IPAddress
+    :vartype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworksngfw.models.IPAddress
     """
 
     _validation = {
         "vnet": {"required": True},
         "trust_subnet": {"required": True},
         "un_trust_subnet": {"required": True},
     }
@@ -4609,21 +4742,21 @@
         trust_subnet: "_models.IPAddressSpace",
         un_trust_subnet: "_models.IPAddressSpace",
         ip_of_trust_subnet_for_udr: Optional["_models.IPAddress"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword vnet: Azure Virtual Network. Required.
-        :paramtype vnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+        :paramtype vnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
         :keyword trust_subnet: Trust Subnet. Required.
-        :paramtype trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+        :paramtype trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
         :keyword un_trust_subnet: Untrust Subnet. Required.
-        :paramtype un_trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+        :paramtype un_trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
         :keyword ip_of_trust_subnet_for_udr: IP of trust subnet for UDR.
-        :paramtype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworks.models.IPAddress
+        :paramtype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworksngfw.models.IPAddress
         """
         super().__init__(**kwargs)
         self.vnet = vnet
         self.trust_subnet = trust_subnet
         self.un_trust_subnet = un_trust_subnet
         self.ip_of_trust_subnet_for_udr = ip_of_trust_subnet_for_udr
 
@@ -4632,21 +4765,21 @@
     """VwanInfo for Firewall Networking.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar network_virtual_appliance_id: Network Virtual Appliance resource ID.
     :vartype network_virtual_appliance_id: str
     :ivar v_hub: vHub Address. Required.
-    :vartype v_hub: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+    :vartype v_hub: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
     :ivar trust_subnet: Trust Subnet.
-    :vartype trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+    :vartype trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
     :ivar un_trust_subnet: Untrust Subnet.
-    :vartype un_trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+    :vartype un_trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
     :ivar ip_of_trust_subnet_for_udr: IP of trust subnet for UDR.
-    :vartype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworks.models.IPAddress
+    :vartype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworksngfw.models.IPAddress
     """
 
     _validation = {
         "v_hub": {"required": True},
     }
 
     _attribute_map = {
@@ -4667,21 +4800,21 @@
         ip_of_trust_subnet_for_udr: Optional["_models.IPAddress"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword network_virtual_appliance_id: Network Virtual Appliance resource ID.
         :paramtype network_virtual_appliance_id: str
         :keyword v_hub: vHub Address. Required.
-        :paramtype v_hub: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+        :paramtype v_hub: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
         :keyword trust_subnet: Trust Subnet.
-        :paramtype trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+        :paramtype trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
         :keyword un_trust_subnet: Untrust Subnet.
-        :paramtype un_trust_subnet: ~azure.mgmt.paloaltonetworks.models.IPAddressSpace
+        :paramtype un_trust_subnet: ~azure.mgmt.paloaltonetworksngfw.models.IPAddressSpace
         :keyword ip_of_trust_subnet_for_udr: IP of trust subnet for UDR.
-        :paramtype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworks.models.IPAddress
+        :paramtype ip_of_trust_subnet_for_udr: ~azure.mgmt.paloaltonetworksngfw.models.IPAddress
         """
         super().__init__(**kwargs)
         self.network_virtual_appliance_id = network_virtual_appliance_id
         self.v_hub = v_hub
         self.trust_subnet = trust_subnet
         self.un_trust_subnet = un_trust_subnet
         self.ip_of_trust_subnet_for_udr = ip_of_trust_subnet_for_udr
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/_patch.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure/mgmt/paloaltonetworksngfw/models/__init__.py` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure/mgmt/paloaltonetworksngfw/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import EventHub
 from ._models_py3 import FirewallResource
 from ._models_py3 import FirewallResourceListResult
 from ._models_py3 import FirewallResourceUpdate
 from ._models_py3 import FirewallResourceUpdateProperties
+from ._models_py3 import FirewallStatusResource
+from ._models_py3 import FirewallStatusResourceListResult
 from ._models_py3 import FqdnListGlobalRulestackResource
 from ._models_py3 import FqdnListGlobalRulestackResourceListResult
 from ._models_py3 import FqdnListLocalRulestackResource
 from ._models_py3 import FqdnListLocalRulestackResourceListResult
 from ._models_py3 import FrontendSetting
 from ._models_py3 import GlobalRulestackInfo
 from ._models_py3 import GlobalRulestackResource
@@ -58,14 +60,15 @@
 from ._models_py3 import MonitorLog
 from ._models_py3 import NameDescriptionObject
 from ._models_py3 import NetworkProfile
 from ._models_py3 import Operation
 from ._models_py3 import OperationDisplay
 from ._models_py3 import OperationListResult
 from ._models_py3 import PanoramaConfig
+from ._models_py3 import PanoramaStatus
 from ._models_py3 import PlanData
 from ._models_py3 import PostRulesResource
 from ._models_py3 import PostRulesResourceListResult
 from ._models_py3 import PreRulesResource
 from ._models_py3 import PreRulesResourceListResult
 from ._models_py3 import PredefinedUrlCategoriesResponse
 from ._models_py3 import PredefinedUrlCategory
@@ -97,24 +100,27 @@
 from ._palo_alto_networks_ngfw_mgmt_client_enums import BooleanEnum
 from ._palo_alto_networks_ngfw_mgmt_client_enums import CreatedByType
 from ._palo_alto_networks_ngfw_mgmt_client_enums import DNSProxy
 from ._palo_alto_networks_ngfw_mgmt_client_enums import DecryptionRuleTypeEnum
 from ._palo_alto_networks_ngfw_mgmt_client_enums import DefaultMode
 from ._palo_alto_networks_ngfw_mgmt_client_enums import EgressNat
 from ._palo_alto_networks_ngfw_mgmt_client_enums import EnabledDNSType
+from ._palo_alto_networks_ngfw_mgmt_client_enums import HealthStatus
 from ._palo_alto_networks_ngfw_mgmt_client_enums import LogOption
 from ._palo_alto_networks_ngfw_mgmt_client_enums import LogType
 from ._palo_alto_networks_ngfw_mgmt_client_enums import ManagedIdentityType
 from ._palo_alto_networks_ngfw_mgmt_client_enums import MarketplaceSubscriptionStatus
 from ._palo_alto_networks_ngfw_mgmt_client_enums import NetworkType
 from ._palo_alto_networks_ngfw_mgmt_client_enums import Origin
 from ._palo_alto_networks_ngfw_mgmt_client_enums import ProtocolType
 from ._palo_alto_networks_ngfw_mgmt_client_enums import ProvisioningState
+from ._palo_alto_networks_ngfw_mgmt_client_enums import ReadOnlyProvisioningState
 from ._palo_alto_networks_ngfw_mgmt_client_enums import ScopeType
 from ._palo_alto_networks_ngfw_mgmt_client_enums import SecurityServicesTypeEnum
+from ._palo_alto_networks_ngfw_mgmt_client_enums import ServerStatus
 from ._palo_alto_networks_ngfw_mgmt_client_enums import StateEnum
 from ._palo_alto_networks_ngfw_mgmt_client_enums import UsageType
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
@@ -140,14 +146,16 @@
     "ErrorDetail",
     "ErrorResponse",
     "EventHub",
     "FirewallResource",
     "FirewallResourceListResult",
     "FirewallResourceUpdate",
     "FirewallResourceUpdateProperties",
+    "FirewallStatusResource",
+    "FirewallStatusResourceListResult",
     "FqdnListGlobalRulestackResource",
     "FqdnListGlobalRulestackResourceListResult",
     "FqdnListLocalRulestackResource",
     "FqdnListLocalRulestackResourceListResult",
     "FrontendSetting",
     "GlobalRulestackInfo",
     "GlobalRulestackResource",
@@ -170,14 +178,15 @@
     "MonitorLog",
     "NameDescriptionObject",
     "NetworkProfile",
     "Operation",
     "OperationDisplay",
     "OperationListResult",
     "PanoramaConfig",
+    "PanoramaStatus",
     "PlanData",
     "PostRulesResource",
     "PostRulesResourceListResult",
     "PreRulesResource",
     "PreRulesResourceListResult",
     "PredefinedUrlCategoriesResponse",
     "PredefinedUrlCategory",
@@ -208,22 +217,25 @@
     "BooleanEnum",
     "CreatedByType",
     "DNSProxy",
     "DecryptionRuleTypeEnum",
     "DefaultMode",
     "EgressNat",
     "EnabledDNSType",
+    "HealthStatus",
     "LogOption",
     "LogType",
     "ManagedIdentityType",
     "MarketplaceSubscriptionStatus",
     "NetworkType",
     "Origin",
     "ProtocolType",
     "ProvisioningState",
+    "ReadOnlyProvisioningState",
     "ScopeType",
     "SecurityServicesTypeEnum",
+    "ServerStatus",
     "StateEnum",
     "UsageType",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/PKG-INFO` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-paloaltonetworksngfw
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Microsoft Azure Paloaltonetworksngfw Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -85,10 +85,20 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-paloaltonetworksngfw%2FREADME.png)
 
 
 # Release History
 
+## 1.0.0b2 (2023-05-05)
+
+### Features Added
+
+  - Added operation group FirewallStatusOperations
+
+### Other Changes
+
+  - Fixed annotation about namespace
+
 ## 1.0.0b1 (2023-05-04)
 
 * Initial Release
```

## Comparing `azure-mgmt-paloaltonetworksngfw-1.0.0b1/azure_mgmt_paloaltonetworksngfw.egg-info/SOURCES.txt` & `azure-mgmt-paloaltonetworksngfw-1.0.0b2/azure_mgmt_paloaltonetworksngfw.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 azure/mgmt/paloaltonetworksngfw/aio/__init__.py
 azure/mgmt/paloaltonetworksngfw/aio/_configuration.py
 azure/mgmt/paloaltonetworksngfw/aio/_palo_alto_networks_ngfw_mgmt_client.py
 azure/mgmt/paloaltonetworksngfw/aio/_patch.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/__init__.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_global_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_certificate_object_local_rulestack_operations.py
+azure/mgmt/paloaltonetworksngfw/aio/operations/_firewall_status_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_firewalls_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_global_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_fqdn_list_local_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_global_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rules_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_local_rulestacks_operations.py
 azure/mgmt/paloaltonetworksngfw/aio/operations/_operations.py
@@ -36,14 +37,15 @@
 azure/mgmt/paloaltonetworksngfw/models/__init__.py
 azure/mgmt/paloaltonetworksngfw/models/_models_py3.py
 azure/mgmt/paloaltonetworksngfw/models/_palo_alto_networks_ngfw_mgmt_client_enums.py
 azure/mgmt/paloaltonetworksngfw/models/_patch.py
 azure/mgmt/paloaltonetworksngfw/operations/__init__.py
 azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_global_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_certificate_object_local_rulestack_operations.py
+azure/mgmt/paloaltonetworksngfw/operations/_firewall_status_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_firewalls_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_global_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_fqdn_list_local_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_global_rulestack_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_local_rules_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_local_rulestacks_operations.py
 azure/mgmt/paloaltonetworksngfw/operations/_operations.py
```

