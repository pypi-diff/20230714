# Comparing `tmp/cloudgenix_config-1.9.0b2.tar.gz` & `tmp/cloudgenix_config-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudgenix_config-1.9.0b2.tar", last modified: Thu Jan 26 23:10:52 2023, max compression
+gzip compressed data, was "cloudgenix_config-2.0.0b1.tar", last modified: Fri Jul 14 20:11:42 2023, max compression
```

## Comparing `cloudgenix_config-1.9.0b2.tar` & `cloudgenix_config-2.0.0b1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)        0 2023-01-26 23:10:52.608710 cloudgenix_config-1.9.0b2/
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)     1066 2023-01-26 23:10:38.000000 cloudgenix_config-1.9.0b2/LICENSE
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)    10215 2023-01-26 23:10:52.608862 cloudgenix_config-1.9.0b2/PKG-INFO
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)     9468 2023-01-26 23:10:38.000000 cloudgenix_config-1.9.0b2/README.md
-drwxr-xr-x   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)        0 2023-01-26 23:10:52.602839 cloudgenix_config-1.9.0b2/cloudgenix_config/
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)    29144 2023-01-26 23:10:38.000000 cloudgenix_config-1.9.0b2/cloudgenix_config/__init__.py
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)    88641 2023-01-26 23:10:38.000000 cloudgenix_config-1.9.0b2/cloudgenix_config/default_interfaces.py
--rwxr-xr-x   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)   573091 2023-01-26 23:10:38.000000 cloudgenix_config-1.9.0b2/cloudgenix_config/do.py
--rwxr-xr-x   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)   104296 2023-01-26 23:10:38.000000 cloudgenix_config-1.9.0b2/cloudgenix_config/pull.py
-drwxr-xr-x   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)        0 2023-01-26 23:10:52.608110 cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)    10215 2023-01-26 23:10:51.000000 cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/PKG-INFO
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)      404 2023-01-26 23:10:52.000000 cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/SOURCES.txt
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)        1 2023-01-26 23:10:51.000000 cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/dependency_links.txt
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)       90 2023-01-26 23:10:51.000000 cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/entry_points.txt
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)       41 2023-01-26 23:10:52.000000 cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/requires.txt
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)       18 2023-01-26 23:10:52.000000 cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/top_level.txt
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)      358 2023-01-26 23:10:52.610031 cloudgenix_config-1.9.0b2/setup.cfg
--rw-r--r--   0 tkamath  (1953533316) PALOALTONETWORK\Domain Users (192360288)     1324 2023-01-26 23:10:38.000000 cloudgenix_config-1.9.0b2/setup.py
+drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-07-14 20:11:42.336189 cloudgenix_config-2.0.0b1/
+-rw-r--r--   0 tkamath  (1953533316) 192360288     1066 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/LICENSE
+-rw-r--r--   0 tkamath  (1953533316) 192360288    10303 2023-07-14 20:11:42.336323 cloudgenix_config-2.0.0b1/PKG-INFO
+-rw-r--r--   0 tkamath  (1953533316) 192360288     9556 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/README.md
+drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-07-14 20:11:42.332246 cloudgenix_config-2.0.0b1/cloudgenix_config/
+-rw-r--r--   0 tkamath  (1953533316) 192360288    29548 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/__init__.py
+-rw-r--r--   0 tkamath  (1953533316) 192360288   172697 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/default_interfaces.py
+-rwxr-xr-x   0 tkamath  (1953533316) 192360288   580626 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/do.py
+-rwxr-xr-x   0 tkamath  (1953533316) 192360288   105950 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/cloudgenix_config/pull.py
+drwxr-xr-x   0 tkamath  (1953533316) 192360288        0 2023-07-14 20:11:42.335781 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/
+-rw-r--r--   0 tkamath  (1953533316) 192360288    10303 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/PKG-INFO
+-rw-r--r--   0 tkamath  (1953533316) 192360288      404 2023-07-14 20:11:42.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/SOURCES.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288        1 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/dependency_links.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288       90 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/entry_points.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288       41 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/requires.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288       18 2023-07-14 20:11:41.000000 cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/top_level.txt
+-rw-r--r--   0 tkamath  (1953533316) 192360288      358 2023-07-14 20:11:42.336827 cloudgenix_config-2.0.0b1/setup.cfg
+-rw-r--r--   0 tkamath  (1953533316) 192360288     1324 2023-07-14 19:59:43.000000 cloudgenix_config-2.0.0b1/setup.py
```

### Comparing `cloudgenix_config-1.9.0b2/LICENSE` & `cloudgenix_config-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudgenix_config-1.9.0b2/PKG-INFO` & `cloudgenix_config-2.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix_config
-Version: 1.9.0b2
+Version: 2.0.0b1
 Summary: Configuration exporting and Continuous Integration (CI) capable configuration importing for the CloudGenix Cloud Controller.
 Home-page: https://github.com/CloudGenix/cloudgenix_config
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix_config.svg)](https://pypi.org/project/cloudgenix_config/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix_config.svg)](https://pypi.org/project/cloudgenix_config/)
 [![Downloads](https://pepy.tech/badge/cloudgenix-config)](https://pepy.tech/project/cloudgenix-config)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix_config.svg?color=brightgreen)](https://pypi.org/project/cloudgenix_config/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/cloudgenix_config.svg)](https://github.com/CloudGenix/cloudgenix_config/issues)
-# CloudGenix Config (Preview)
+# CloudGenix Config 
 Configuration exporting and Continuous Integration (CI) capable configuration importing for the CloudGenix Cloud Controller.
 
 #### Synopsis
 Enables export and import of configurations and templates from the CloudGenix Cloud Controller. Also, the Import of 
 configuration is designed to be run on file change, to maintain configuration state on the Cloud Controller.
 
 #### Features
@@ -124,14 +124,15 @@
  - For ION 9000, if trying to configure a bypasspair and the port with the same name (12,13,14,15,16), configuration pushes via do_site have to be done in the following two steps:
      - Include only interface configuration of type port and use the do_site utility to push this configuration first.
      - Update the YAML file to remove the interface configuration of type port, include interface configuration of type bypasspair and use the do_site utiltiy to push the bypasspair configuration.
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **2.0.0** | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
 | **1.9.0** | **b2** | Bug fixes - CGCBL-1251, CGCBL-1578|
 |           | **b1** | Support for Cloudgenix SDK 6.1.1b1, bug fixes|
 | **1.8.0** | **b1** | Support for Cloudgenix SDK 6.0.2b1, Fix for CGCBL-1399, CGCBL-1347|
 | **1.7.0** | **b3** | Bug fixes|
 |           | **b2** | Fix for CGCBL-336, #73, #74 and CGESC-700|
 |           | **b1** | Support for CloudGenix SDK 6.0.1b1, bug fixes|
 | **1.6.0** | **b2** | Minor bug fixes |
```

### Comparing `cloudgenix_config-1.9.0b2/README.md` & `cloudgenix_config-2.0.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix_config.svg)](https://pypi.org/project/cloudgenix_config/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix_config.svg)](https://pypi.org/project/cloudgenix_config/)
 [![Downloads](https://pepy.tech/badge/cloudgenix-config)](https://pepy.tech/project/cloudgenix-config)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix_config.svg?color=brightgreen)](https://pypi.org/project/cloudgenix_config/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/cloudgenix_config.svg)](https://github.com/CloudGenix/cloudgenix_config/issues)
-# CloudGenix Config (Preview)
+# CloudGenix Config 
 Configuration exporting and Continuous Integration (CI) capable configuration importing for the CloudGenix Cloud Controller.
 
 #### Synopsis
 Enables export and import of configurations and templates from the CloudGenix Cloud Controller. Also, the Import of 
 configuration is designed to be run on file change, to maintain configuration state on the Cloud Controller.
 
 #### Features
@@ -106,14 +106,15 @@
  - For ION 9000, if trying to configure a bypasspair and the port with the same name (12,13,14,15,16), configuration pushes via do_site have to be done in the following two steps:
      - Include only interface configuration of type port and use the do_site utility to push this configuration first.
      - Update the YAML file to remove the interface configuration of type port, include interface configuration of type bypasspair and use the do_site utiltiy to push the bypasspair configuration.
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **2.0.0** | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
 | **1.9.0** | **b2** | Bug fixes - CGCBL-1251, CGCBL-1578|
 |           | **b1** | Support for Cloudgenix SDK 6.1.1b1, bug fixes|
 | **1.8.0** | **b1** | Support for Cloudgenix SDK 6.0.2b1, Fix for CGCBL-1399, CGCBL-1347|
 | **1.7.0** | **b3** | Bug fixes|
 |           | **b2** | Fix for CGCBL-336, #73, #74 and CGESC-700|
 |           | **b1** | Support for CloudGenix SDK 6.0.1b1, bug fixes|
 | **1.6.0** | **b2** | Minor bug fixes |
```

### Comparing `cloudgenix_config-1.9.0b2/cloudgenix_config/__init__.py` & `cloudgenix_config-2.0.0b1/cloudgenix_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Configuration IMPORT/EXPORT common functions
 
-**Version:** 1.9.0b2
+**Version:** 2.0.0b1
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017, 2018 CloudGenix, Inc
 
 **License:** MIT
 
@@ -45,15 +45,15 @@
     binary_type = str
 else:
     text_type = str
     binary_type = bytes
 
 
 # Version for reference
-__version__ = "1.9.0b2"
+__version__ = "2.0.0b1"
 version = __version__
 
 __author__ = "CloudGenix Developer Support <developers@cloudgenix.com>"
 __email__ = "developers@cloudgenix.com"
 __copyright__ = "Copyright (c) 2017, 2018 CloudGenix, Inc"
 __license__ = """
     MIT License
@@ -329,14 +329,24 @@
         return yaml.safe_load(ion_1200_c_na)
     elif model_string == "ion 1200-c5g-ww":
         return yaml.safe_load(ion_1200_c5g_ww)
     elif model_string == "ion 1200-s-c5g-ww":
         return yaml.safe_load(ion_1200_s_c5g_ww)
     elif model_string == "ion 1200-s-c-na":
         return yaml.safe_load(ion_1200_s_c_na)
+    elif model_string == "ion 1200-s-c-row":
+        return yaml.safe_load(ion_1200_s_c_row)
+    elif model_string == "ion 1200-s":
+        return yaml.safe_load(ion_1200s)
+    elif model_string == "ion 5200":
+        return yaml.safe_load(ion_5200)
+    elif model_string == "ion 3200":
+        return yaml.safe_load(ion_3200)
+    elif model_string == "ion 9200":
+        return yaml.safe_load(ion_9200)
     else:
         # model not found, return empty dict
         return {}
 
 
 def get_member_default_config():
     """
```

### Comparing `cloudgenix_config-1.9.0b2/cloudgenix_config/do.py` & `cloudgenix_config-2.0.0b1/cloudgenix_config/do.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Configuration IMPORT worker/script
 
-**Version:** 1.9.0b2
+**Version:** 2.0.0b1
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017, 2018 CloudGenix, Inc
 
 **License:** MIT
 
@@ -216,29 +216,31 @@
     "4\.7\..*" : "5.0.3", ### 4.7.xyz -> 5.0.3
     "5\.0\..*" : "5.2.7", ### 5.0.xyz -> 5.2.7
     "5\.1\..*" : "5.2.7", ### 5.1.xyz -> 5.2.7
     "5\.2\..*" : ["5.5..*", "5.4..*", "5.3..*"], ### 5.2.xyz -> 5.5.3 # Fix for CGCBL-566
     "5\.3\..*" : ["5.5..*", "5.4..*"], ### 5.3.xyz -> 5.5.3
     "5\.4\..*" : ["5.6..*", "5.5..*"], ### 5.4.xyz -> 5.6.1
     "5\.5\..*" : ["6.0..*", "5.6..*"], ### 5.5.xyz -> 5.6.1
-    "5\.6\..*" : ["6.0..*", "6.1..*"],
-    "6\.0\..*" : ["6.1..*"],
+    "5\.6\..*" : ["6.1..*", "6.0..*"],
+    "6\.0\..*" : ["6.2..*", "6.1..*"],
+    "6\.1\..*" : ["6.2..*"]
 }
 
 downgrade_path_regex = {
     "4\.7\..*" : "4.5.3", ### 4.7.xyz -> 4.5.3
     "5\.0\..*" : "4.7.1", ### 5.0 to 4.7.1
     "5\.1\..*" : "4.7.1", ### 5.1 to 4.7.1
     "5\.2\..*" : "5.0.3", ### 5.2 to 5.0.3
     "5\.3\..*" : "5.2.7", ### 5.3 to 5.2.7
     "5\.4\..*" : ["5.2..*", "5.3..*"], ### 5.4 to 5.2.7 # Fix for CGCBL-566
     "5\.5\..*" : ["5.2..*", "5.3..*", "5.4..*"], ### 5.5 to 5.2.7
     "5\.6\..*" : ["5.4..*", "5.5..*"], ### 5.6 to 5.4.1
     "6\.0\..*" : ["5.5..*", "5.6..*"],
     "6\.1\..*" : ["5.6..*", "6.0..*"],
+    "6\.2\..*" : ["6.0..*", "6.1..*"],
 }
 
 # Global Config Cache holders
 sites_cache = []
 elements_cache = []
 machines_cache = []
 policysets_cache = []
@@ -895,18 +897,20 @@
                                                                 sdk.put.site_natlocalprefixes, default=[])
     config_site_ipfix_localprefixes, _ = config_lower_version_get(config_site, 'site_ipfix_localprefixes',
                                                                 sdk.put.site_ipfixlocalprefixes, default=[])
     config_multicastsourcesiteconfigs, _ = config_lower_version_get(config_site, 'multicastsourcesiteconfigs',
                                                                 sdk.put.multicastsourcesiteconfigs, default=[])
     config_hubclusters, _ = config_lower_version_get(config_site, 'hubclusters',
                                                                     sdk.put.hubclusters, default={})
+    config_deviceidconfigs, _ = config_lower_version_get(config_site, 'deviceidconfigs',
+                                                                    sdk.put.deviceidconfigs, default=[])
 
     return config_waninterfaces, config_lannetworks, config_elements, config_dhcpservers, config_site_extensions, \
         config_site_security_zones, config_spokeclusters, config_site_nat_localprefixes, \
-        config_site_ipfix_localprefixes, config_multicastsourcesiteconfigs, config_hubclusters
+        config_site_ipfix_localprefixes, config_multicastsourcesiteconfigs, config_hubclusters, config_deviceidconfigs
 
 
 def parse_element_config(config_element):
     """
     Parse Element level configuration
     :param config_element: Element config dict
     :return: Tuple of Interface config, Routing config, Syslog config, NTP config, SNMP config, Toolkit config and
@@ -1252,15 +1256,15 @@
     Get the full version string matching the version from the available images
     :param version: Upgrade/Downgrade version
     :param image_dict: Available images dict
     :return: Image version
     """
 
     for image_version in image_dict.keys():
-        if re.search(str(version), image_version):
+        if re.match(str(version), image_version):
             return image_version
     return None
 
 
 def upgrade_downgrade_element(element_id, image_id, images_id2n, element_descriptive_text, wait_upgrade_timeout=DEFAULT_WAIT_MAX_TIME, pause_for_upgrade=True, wait_interval=DEFAULT_WAIT_INTERVAL):
     """
     :param element_id: Matching element id
@@ -1526,15 +1530,16 @@
     staged_upgrade_downgrade_element(matching_element, config_element, wait_upgrade_timeout=wait_upgrade_timeout,
                     pause_for_upgrade=pause_for_upgrade,
                     wait_interval=wait_interval)
 
     return
 
 
-def handle_element_spoke_ha(matching_element, site_id, config_element, interfaces_n2id, spokecluster_n2id, hubclusters_n2id, version=None):
+def handle_element_spoke_ha(matching_element, site_id, config_element, interfaces_n2id, spokecluster_n2id,
+                            hubclusters_n2id, waninterfaces_n2id, reset_spoke_ha=0, version=None):
     """
     Since Spoke HA config is part of the element object, we need to handle it separately.
     :param matching_element: Element object (containing ID) to work on
     :param site_id: Site ID to work on
     :param config_element: Element config struct
     :param interfaces_n2id: Intertfaces Name -> ID map.
     :param spokecluster_n2id: Spoke Cluster Name -> ID map.
@@ -1594,14 +1599,25 @@
                 for spoke_ha_config_track_interfaces_entry in spoke_ha_config_track_interfaces:
                     spoke_ha_config_track_interfaces_entry_template = \
                         copy.deepcopy(spoke_ha_config_track_interfaces_entry)
                     name_lookup_in_template(spoke_ha_config_track_interfaces_entry_template,
                                             'interface_id', interfaces_n2id)
                     spoke_ha_config_track_interfaces_template.append(spoke_ha_config_track_interfaces_entry_template)
                 spoke_ha_config_track_template['interfaces'] = spoke_ha_config_track_interfaces_template
+            spoke_ha_config_track_waninterfaces = spoke_ha_config_track.get("waninterfaces")
+            if spoke_ha_config_track_waninterfaces:
+                spoke_ha_config_track_waninterfaces_template = []
+                for spoke_ha_config_track_waninterfaces_entry in spoke_ha_config_track_waninterfaces:
+                    spoke_ha_config_track_waninterfaces_entry_template = \
+                        copy.deepcopy(spoke_ha_config_track_waninterfaces_entry)
+                    name_lookup_in_template(spoke_ha_config_track_waninterfaces_entry_template,
+                                            'wan_interface_id', waninterfaces_n2id)
+                    spoke_ha_config_track_waninterfaces_template.append(
+                        spoke_ha_config_track_waninterfaces_entry_template)
+                spoke_ha_config_track_template['waninterfaces'] = spoke_ha_config_track_waninterfaces_template
             spoke_ha_config_template['track'] = spoke_ha_config_track_template
         config_element_copy['spoke_ha_config'] = spoke_ha_config_template
     else:
         config_element_copy['spoke_ha_config'] = None
 
     # Create a copy of the cleaned element template for update check
     element_change_check = copy.deepcopy(elem_template)
@@ -1609,15 +1625,24 @@
     # Update element template with config changes from cleaned copy
     elem_template.update(config_element_copy)
 
     if elem_template.get('cluster_id'):
         elem_template['cluster_id'] = hubclusters_n2id.get(elem_template['cluster_id'])
 
     # Check for changes in cleaned config copy and cleaned template (will finally detect spoke HA changes here):
-    if not force_update and elem_template == element_change_check:
+    if spoke_ha_config and reset_spoke_ha and element_change_check.get('spoke_ha_config'):
+        if elem_template.get('spoke_ha_config', {}).get('source_interface') != \
+                element_change_check.get('spoke_ha_config', {}).get('source_interface') or \
+                elem_template.get('spoke_ha_config', {}).get('track', {}) != \
+                element_change_check.get('spoke_ha_config', {}).get('track', {}):
+            output_message("   Resetting Spoke HA in element {0}.".format(element_descriptive_text))
+            elem_template['spoke_ha_config'] = None
+        else:
+            return 1
+    elif not force_update and elem_template == element_change_check:
         # no change in config, pass.
         output_message("   No Change for Spoke HA in Element {0}.".format(element_descriptive_text))
         return
 
     if debuglevel >= 3:
         local_debug("ELEMENT SPOKEHA DIFF: {0}".format(find_diff(element_change_check, elem_template)))
 
@@ -2006,15 +2031,15 @@
             # clear out any Spoke HA configurations
             elem_template['spoke_ha_config'] = None
 
             # create a temp element object to flush the configs.
             matching_element = {"id": element_item_id}
 
             # use the temp fake element to flush the Spoke HA configuration prior to unbind.
-            handle_element_spoke_ha(matching_element, site_id, elem_template, {}, {}, {}, version=version)
+            handle_element_spoke_ha(matching_element, site_id, elem_template, {}, {}, {}, {}, version=version)
 
             # refresh the element
             element_resp = sdk.get.elements(element_item_id)
 
             if not element_resp.cgx_status:
                 throw_warning('Could not refresh element after Spoke HA flush: ', element_resp)
 
@@ -2108,14 +2133,15 @@
     site_template = fuzzy_pop(site_template, 'hubclusters')
     site_template = fuzzy_pop(site_template, 'site_extensions')
     site_template = fuzzy_pop(site_template, 'site_security_zones')
     site_template = fuzzy_pop(site_template, 'spokeclusters')
     site_template = fuzzy_pop(site_template, 'site_nat_localprefixes')
     site_template = fuzzy_pop(site_template, 'site_ipfix_localprefixes')
     site_template = fuzzy_pop(site_template, 'multicastsourcesiteconfigs')
+    site_template = fuzzy_pop(site_template, 'deviceidconfigs')
 
     # perform name -> ID lookups
     name_lookup_in_template(site_template, 'policy_set_id', policysets_n2id)
     name_lookup_in_template(site_template, 'security_policyset_id', security_policysets_n2id)
     name_lookup_in_template(site_template, 'security_policysetstack_id', ngfw_security_policysetstack_n2id)
     name_lookup_in_template(site_template, 'network_policysetstack_id', network_policysetstack_n2id)
     name_lookup_in_template(site_template, 'priority_policysetstack_id', priority_policysetstack_n2id)
@@ -2166,14 +2192,15 @@
     site_template = fuzzy_pop(site_template, 'hubclusters')
     site_template = fuzzy_pop(site_template, 'site_extensions')
     site_template = fuzzy_pop(site_template, 'site_security_zones')
     site_template = fuzzy_pop(site_template, 'spokeclusters')
     site_template = fuzzy_pop(site_template, 'site_nat_localprefixes')
     site_template = fuzzy_pop(site_template, 'site_ipfix_localprefixes')
     site_template = fuzzy_pop(site_template, 'multicastsourcesiteconfigs')
+    site_template = fuzzy_pop(site_template, 'deviceidconfigs')
 
     # perform name -> ID lookups
     name_lookup_in_template(site_template, 'policy_set_id', policysets_n2id)
     name_lookup_in_template(site_template, 'security_policyset_id', security_policysets_n2id)
     name_lookup_in_template(site_template, 'security_policysetstack_id', ngfw_security_policysetstack_n2id)
     name_lookup_in_template(site_template, 'network_policysetstack_id', network_policysetstack_n2id)
     name_lookup_in_template(site_template, 'priority_policysetstack_id', priority_policysetstack_n2id)
@@ -2206,15 +2233,15 @@
     if site_config.get("multicast_peer_group_id") != site_change_check.get("multicast_peer_group_id"):
         if site_config.get("multicast_peer_group_id") == None:
 
             site_id = site_change_check.get('id')
             site_name = site_change_check.get('name')
             config_waninterfaces, config_lannetworks, config_elements, config_dhcpservers, config_site_extensions, \
             config_site_security_zones, config_spokeclusters, config_site_nat_localprefixes, config_site_ipfix_localprefixes, \
-            config_multicastsourcesiteconfigs, config_hubclusters = parse_site_config(config_site)
+            config_multicastsourcesiteconfigs, config_hubclusters, config_deviceidconfigs = parse_site_config(config_site)
 
             if not config_multicastsourcesiteconfigs:
                 output_message(" Resetting Multicast Source Site Config for the Site {0}.".format(site_name))
                 multicastsourcesiteconfigs_resp = sdk.get.multicastsourcesiteconfigs(site_id)
                 multicastsourcesiteconfigs_cache, leftover_multicastsourcesiteconfigs = extract_items(
                     multicastsourcesiteconfigs_resp, 'multicastsourcesiteconfigs')
 
@@ -3805,14 +3832,73 @@
         if not site_ipfix_localprefix_del_resp.cgx_status:
             throw_error("Could not delete Site IPFIX Localprefix mapping for Localprefix {0}: "
                         "".format(silp_name),
                         site_ipfix_localprefix_del_resp)
     return
 
 
+def modify_deviceidconfigs(config_deviceidconfigs, deviceidconfigs_id, site_id, version=None):
+    """
+    Modify deviceidconfigs
+    :param config_deviceidconfigss: deviceidconfigs config dict
+    :param deviceidconfigs_id: deviceidconfigs ID
+    :param site_id: Site ID to use
+    :param element_id: Element ID to use
+    :return: Modified deviceidconfigs ID
+    """
+    deviceidconfigs_config = {}
+    # make a copy of deviceidconfigs to modify
+    deviceidconfigs_template = copy.deepcopy(config_deviceidconfigs)
+
+    # get current deviceidconfigs
+    deviceidconfigs_resp = sdk.get.deviceidconfigs(site_id, deviceidconfigs_id)
+    if deviceidconfigs_resp.cgx_status:
+        deviceidconfigs_config = deviceidconfigs_resp.cgx_content
+    else:
+        throw_error("Unable to retrieve Device ID Config: ", deviceidconfigs_resp)
+
+    # extract prev_revision
+    prev_revision = deviceidconfigs_config.get("_etag")
+
+    # Check for changes:
+    deviceidconfigs_change_check = copy.deepcopy(deviceidconfigs_config)
+    deviceidconfigs_config.update(deviceidconfigs_template)
+    if not force_update and deviceidconfigs_config == deviceidconfigs_change_check:
+        # no change in config, pass.
+        deviceidconfigs_id = deviceidconfigs_change_check.get('id')
+        deviceidconfigs_name = deviceidconfigs_change_check.get('name', deviceidconfigs_id)
+        output_message(" No Change for Device ID Config {0}.".format(deviceidconfigs_name))
+        return deviceidconfigs_id
+
+    if debuglevel >= 3:
+        local_debug("Device ID Config DIFF: {0}".format(
+            find_diff(deviceidconfigs_change_check, deviceidconfigs_config)))
+
+    # Update deviceidconfigs.
+    deviceidconfigs_resp2 = sdk.put.deviceidconfigs(site_id, deviceidconfigs_id, deviceidconfigs_config,
+                                                     api_version=version)
+
+    if not deviceidconfigs_resp2.cgx_status:
+        throw_error(" Device ID Config update failed: ", deviceidconfigs_resp2)
+
+    deviceidconfigs_id = deviceidconfigs_resp.cgx_content.get('id')
+    deviceidconfigs_name = deviceidconfigs_resp.cgx_content.get('name', deviceidconfigs_id)
+
+    # extract current_revision
+    current_revision = deviceidconfigs_resp2.cgx_content.get("_etag")
+
+    if not deviceidconfigs_id:
+        throw_error("Unable to determine Device ID Config attributes (ID {0})..".format(deviceidconfigs_id))
+
+    output_message(" Updated Device ID Config {0} (Etag {1} -> {2}).".format(deviceidconfigs_name, prev_revision,
+                                                                           current_revision))
+
+    return deviceidconfigs_id
+
+
 def create_interface(config_interface, interfaces_n2id, waninterfaces_n2id, lannetworks_n2id, site_id, element_id,
                      api_interfaces_cache=None, interfaces_funny_n2id=None, version=None):
     """
     Create a new Interface
     :param config_interface: Interface config dict
     :param interfaces_n2id: Interfaces Name to ID dict
     :param waninterfaces_n2id: WAN Interfaces Name to ID dict
@@ -4357,19 +4443,19 @@
     else:
         throw_error("Unable to retrieve interface: ", interface_resp)
 
     # extract prev_revision
     prev_revision = interface_config.get("_etag")
 
     config = {}
-    if interface_config.get('bypass_pair'):
+    if interface_config.get('bypass_pair') and not interface_template.get('bypass_pair'):
         config['bypass_pair'] = interface_config['bypass_pair']
-    if interface_config.get('sub_interface'):
+    if interface_config.get('sub_interface') and not interface_template.get('sub_interface'):
         config['sub_interface'] = interface_config['sub_interface']
-    if interface_config.get('pppoe_config'):
+    if interface_config.get('pppoe_config') and not interface_template.get('pppoe_config'):
         config['pppoe_config'] = interface_config['pppoe_config']
     if interface_config.get('parent'):
         config['parent'] = interface_config['parent']
     if interface_config.get('type') == 'subinterface' or interface_config.get('type') == 'pppoe':
         config['mtu'] = 0
         config['used_for'] = interface_config.get('used_for')
         config['type'] = interface_config.get('type')
@@ -4387,14 +4473,15 @@
         if interface_config != interface_change_check:
             output_message("   Resetting the vlan interface id for Switch port {0}.".format(interface_change_check.get("name")))
             if interface_config.get("switch_port_config"):
                 interface_config["switch_port_config"]["access_vlan_id"] = None
                 interface_config["switch_port_config"]["native_vlan_id"] = None
                 interface_config["switch_port_config"]["voice_vlan_id"] = None
                 interface_config["switch_port_config"]["trunk_vlans"] = None
+                interface_config["switch_port_config"]["vlan_mode"] = "access"
         else:
             return 1
     elif reset_ipfix_collector_filter_context:
         if interface_config != interface_change_check:
             output_message(
                 "   Resetting the IPFIXCOLLECTORCONTEXT for Interface {0}.".format(interface_change_check.get("name")))
             if interface_config.get("ipfixcollectorcontext_id"):
@@ -6161,15 +6248,15 @@
         throw_error("Unable to determine syslog attributes (ID {0})..".format(syslog_id))
 
     output_message("   Created syslog {0}.".format(syslog_name))
 
     return syslog_id
 
 
-def modify_syslog(config_syslog, syslog_id, interfaces_n2id, syslogserverprofiles_n2id, site_id, element_id, version=None):
+def modify_syslog(config_syslog, syslog_id, interfaces_n2id, syslogserverprofiles_n2id, site_id, element_id, reset_syslog=0, version=None):
     """
     Modify an existing Syslog
     :param config_syslog: Syslog config dict
     :param syslog_id: Existing syslog ID
     :param interfaces_n2id: Interfaces Name to ID dict
     :param site_id: Site ID to use
     :param element_id: Element ID to use
@@ -6197,15 +6284,21 @@
 
     # extract prev_revision
     prev_revision = syslog_config.get("_etag")
 
     # Check for changes:
     syslog_change_check = copy.deepcopy(syslog_config)
     syslog_config.update(syslog_template)
-    if not force_update and syslog_config == syslog_change_check:
+    if reset_syslog:
+        if syslog_config != syslog_change_check:
+            output_message("   Resetting source interface ids for syslog {0}.".format(syslog_change_check.get('name')))
+            syslog_config['source_interface'] = None
+        else:
+            return 1
+    elif not force_update and syslog_config == syslog_change_check:
         # no change in config, pass.
         syslog_id = syslog_change_check.get('id')
         syslog_name = syslog_change_check.get('name')
         output_message("   No Change for Syslog {0}.".format(syslog_name))
         return syslog_id
 
     if debuglevel >= 3:
@@ -6507,15 +6600,15 @@
 
     output_message("   Created Snmp trap {0}.".format(snmp_trap_id))
 
     return snmp_trap_id
 
 
 def modify_snmp_trap(config_snmp_trap, snmp_trap_id, interfaces_n2id,
-                     site_id, element_id, version=None):
+                     site_id, element_id, reset_snmp=0, version=None):
     """
     Modify Existing SNMP Trap
     :param config_snmp_trap: SNMP Trap config dict
     :param snmp_trap_id: Existing SNMP Trap ID
     :param interfaces_n2id: Interfaces Name to ID dict
     :param site_id: Site ID to use
     :param element_id: Element ID to use
@@ -6543,15 +6636,21 @@
 
     # extract prev_revision
     prev_revision = snmp_trap_config.get("_etag")
 
     # Check for changes:
     snmp_trap_change_check = copy.deepcopy(snmp_trap_config)
     snmp_trap_config.update(snmp_trap_template)
-    if not force_update and snmp_trap_config == snmp_trap_change_check:
+    if reset_snmp:
+        if snmp_trap_config != snmp_trap_change_check:
+            output_message("   Resetting source interface ids for SNMP Trap {0}.".format(snmp_trap_id))
+            snmp_trap_config['source_interface'] = None
+        else:
+            return 1
+    elif not force_update and snmp_trap_config == snmp_trap_change_check:
         # no change in config, pass.
         snmp_trap_id = snmp_trap_change_check.get('id')
         output_message("   No Change for Snmp_trap {0}.".format(snmp_trap_id))
         return snmp_trap_id
 
     if debuglevel >= 3:
         local_debug("SNMP_TRAP DIFF: {0}".format(find_diff(snmp_trap_change_check, snmp_trap_config)))
@@ -7713,15 +7812,15 @@
             # recombine site object
             new_site_id = None
             config_site = recombine_named_key_value(config_site_name, config_site_value, name_key='name')
 
             # parse site config
             config_waninterfaces, config_lannetworks, config_elements, config_dhcpservers, config_site_extensions, \
                 config_site_security_zones, config_spokeclusters, config_site_nat_localprefixes, config_site_ipfix_localprefixes, \
-                config_multicastsourcesiteconfigs, config_hubclusters\
+                config_multicastsourcesiteconfigs, config_hubclusters, config_deviceidconfigs \
                 = parse_site_config(config_site)
 
             # Getting version for site resourcesinput apiversion
             waninterfaces_version = use_sdk_yaml_version(config_site, 'waninterfaces', sdk.put.waninterfaces,
                                                                default={}, sdk_or_yaml=apiversion)
             lannetworks_version = use_sdk_yaml_version(config_site, 'lannetworks', sdk.put.lannetworks,
                                                              default={}, sdk_or_yaml=apiversion)
@@ -7739,14 +7838,17 @@
             site_ipfix_localprefixes_version = use_sdk_yaml_version(config_site, 'site_ipfix_localprefixes',
                                                                           sdk.put.site_ipfixlocalprefixes, default=[], sdk_or_yaml=apiversion)
             multicastsourcesiteconfigs_version = use_sdk_yaml_version(config_site, 'multicastsourcesiteconfigs',
                                                                           sdk.put.multicastsourcesiteconfigs, default=[], sdk_or_yaml=apiversion)
             hubclusters_version = use_sdk_yaml_version(config_site, 'hubclusters',
                                                                       sdk.put.hubclusters, default=[],
                                                                       sdk_or_yaml=apiversion)
+            deviceidconfigs_version = use_sdk_yaml_version(config_site, 'deviceidconfigs',
+                                                       sdk.put.deviceidconfigs, default=[],
+                                                       sdk_or_yaml=apiversion)
 
             if "multicast_peer_group_id" in config_site and config_site["multicast_peer_group_id"]:
                 mpg_id = multicastpeergroups_n2id.get(config_site["multicast_peer_group_id"])
                 if mpg_id:
                     config_site["multicast_peer_group_id"] = mpg_id
                 else:
                     throw_error(f"Invalid Multicast Peer Group: {config_site['multicast_peer_group_id']}")
@@ -8371,14 +8473,33 @@
 
                 # remove from delete queue
                 leftover_site_ipfix_localprefixes = [entry for entry in leftover_site_ipfix_localprefixes
                                                      if entry != site_ipfix_localprefix_id]
 
             # -- End Site_ipfix_localprefixes
 
+            deviceidconfigs_resp = sdk.get.deviceidconfigs(site_id)
+            deviceidconfigs_cache, leftover_deviceidconfigs = extract_items(
+                deviceidconfigs_resp, 'deviceidconfigs')
+
+            # iterate configs (list)
+            for config_deviceidconfigs_entry in config_deviceidconfigs:
+
+                config_deviceidconfigs_record = copy.deepcopy(config_deviceidconfigs_entry)
+                deviceidconfigs_id = None
+                if deviceidconfigs_cache:
+                    deviceidconfigs_id = deviceidconfigs_cache[0].get('id')
+
+                # Create or modify deviceidconfigs.
+                if deviceidconfigs_id is not None:
+                    # deviceidconfigs exists, modify.
+                    deviceidconfigs_id = modify_deviceidconfigs(config_deviceidconfigs_record,
+                                                                deviceidconfigs_id, site_id,
+                                                                version=deviceidconfigs_version)
+
             # -- Start Elements - Iterate loop.
             # Get all elements assigned to this site from the global element cache.
             leftover_elements = [entry.get('id') for entry in elements_cache if entry.get('site_id') == site_id]
 
             for config_element_name, config_element_value in config_elements.items():
                 # recombine element object
                 config_element = recombine_named_key_value(config_element_name, config_element_value, name_key='name')
@@ -8908,14 +9029,19 @@
                         # look up ID by name on existing interfaces.
                         syslog_id = name_syslog_id
 
                     else:
                         # no syslog object.
                         syslog_id = None
 
+                    if syslog_id is not None:
+                        # Syslog exists, modify.
+                        syslog_id = modify_syslog(config_syslog_record, syslog_id, interfaces_n2id, syslogserverprofiles_n2id, site_id,
+                                                  element_id, reset_syslog=1, version=syslog_version)
+
                     # remove from delete queue
                     leftover_syslogs = [entry for entry in leftover_syslogs if entry != syslog_id]
 
                 # delete remaining syslog configs
                 syslogs_id2n = build_lookup_dict(syslogs_cache, key_val='id', value_val='name')
                 delete_syslogs(leftover_syslogs, site_id, element_id, id2n=syslogs_id2n)
 
@@ -8954,14 +9080,19 @@
                         # look up ID on existing agent.
                         snmp_trap_id = server_version_snmp_trap_id
 
                     else:
                         # no snmp_trap object.
                         snmp_trap_id = None
 
+                    if snmp_trap_id is not None:
+                        # Snmp_trap exists, modify.
+                        snmp_trap_id = modify_snmp_trap(config_snmp_trap, snmp_trap_id, interfaces_n2id,
+                                                        site_id, element_id, reset_snmp=1, version=snmp_traps_version)
+
                     # remove from delete queue
                     leftover_snmp_traps = [entry for entry in leftover_snmp_traps if entry != snmp_trap_id]
 
                 # delete remaining snmp agent configs
                 delete_snmp_traps(leftover_snmp_traps, site_id, element_id)
 
                 # -- Start NTP config
@@ -8973,23 +9104,22 @@
 
                 # START Aplication Probe
                 # We cannot delete application probe. So checking if app probe is modified in config
                 # If modified, we will reset the source interface id and later update it again
                 if config_app_probe:
                     application_probe_id = modify_application_probe(config_app_probe, site_id, element_id, interfaces_n2id, reset_app_probe=1, version=app_probe_version)
 
+                handle_element_spoke_ha(matching_element, site_id, config_element, interfaces_n2id, spokeclusters_n2id,
+                                        hubclusters_n2id, waninterfaces_n2id, reset_spoke_ha=1, version=elements_version)
                 # END Aplication Probe
 
 
                 # Now we will delete the leftover interfaces for all interfaces type
                 # This will ensure any unused interfaces can be reused or reconfigured
 
-                handle_element_spoke_ha(matching_element, site_id, config_element, interfaces_n2id, spokeclusters_n2id,
-                                        hubclusters_n2id, version=elements_version)
-
                 # START SERVICELINK
 
                 # extend interfaces_n2id with the funny_name cache, Make sure API interfaces trump funny names
                 current_interfaces_n2id_holder = interfaces_n2id
                 interfaces_n2id = copy.deepcopy(interfaces_funny_n2id)
                 interfaces_n2id.update(current_interfaces_n2id_holder)
 
@@ -10249,15 +10379,16 @@
 
                 # -- Start Element Spoke HA config
                 # Since for some reason, Spoke HA config is tied into element object, we can't configure it
                 # at the same time as the element configuration operation is performed. This requires us to do
                 # a second element operation AFTER the interfaces are enumerated and at the correct state (here).
 
                 # assign and configure element
-                handle_element_spoke_ha(matching_element, site_id, config_element, interfaces_n2id, spokeclusters_n2id, hubclusters_n2id, version=elements_version)
+                handle_element_spoke_ha(matching_element, site_id, config_element, interfaces_n2id, spokeclusters_n2id,
+                                        hubclusters_n2id, waninterfaces_n2id, version=elements_version)
 
                 # update element and machine cache before moving on.
                 update_element_machine_cache()
                 config_serial, matching_element, matching_machine, matching_model = detect_elements(config_element)
 
                 # final element ID and model for this element:
                 element_id = matching_element.get('id')
@@ -11502,18 +11633,18 @@
     # Allow Controller modification and debug level sets.
     controller_group = parser.add_argument_group('API', 'These options change how this program connects to the API.')
     controller_group.add_argument("--controller", "-C",
                                   help="Controller URI, ex. https://api.elcapitan.cloudgenix.com",
                                   default=None)
 
     login_group = parser.add_argument_group('Login', 'These options allow skipping of interactive login')
-    login_group.add_argument("--email", "-E", help="Use this email as User Name instead of cloudgenix_settings.py "
+    login_group.add_argument("--email", "-E", help="Use this email as User Name instead of cloudgenix_settings.py.example "
                                                    "or prompting",
                              default=None)
-    login_group.add_argument("--password", "-PW", help="Use this Password instead of cloudgenix_settings.py "
+    login_group.add_argument("--password", "-PW", help="Use this Password instead of cloudgenix_settings.py.example "
                                                        "or prompting",
                              default=None)
     login_group.add_argument("--insecure", "-I", help="Do not verify SSL certificate",
                              action='store_true',
                              default=False)
     login_group.add_argument("--noregion", "-NR", help="Ignore Region-based redirection.",
                              dest='ignore_region', action='store_true', default=False)
```

### Comparing `cloudgenix_config-1.9.0b2/cloudgenix_config/pull.py` & `cloudgenix_config-2.0.0b1/cloudgenix_config/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Configuration EXPORT worker/script
 
-**Version:** 1.9.0b2
+**Version:** 2.0.0b1
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017, 2018 CloudGenix, Inc
 
 **License:** MIT
 
@@ -164,14 +164,15 @@
 MULTICASTRPS_STR = "multicastrps"
 CELLULAR_MODULES_SIM_SECURITY_STR = "cellular_modules_sim_security"
 ELEMENT_CELLULAR_MODULES_STR = "element_cellular_modules"
 ELEMENT_CELLULAR_MODULES_FIRMWARE_STR = "element_cellular_modules_firmware"
 RADII_STR = "radii"
 MULTICASTSOURCESITECONFIGS_STR = "multicastsourcesiteconfigs"
 # MULTICASTPEERGROUPS_STR = "multicastpeergroups"
+DEVICE_ID_CONFIGS_STR = "deviceidconfigs"
 
 # Global Config Cache holders
 sites_cache = []
 elements_cache = []
 machines_cache = []
 policysets_cache = []
 security_policysets_cache = []
@@ -615,14 +616,15 @@
     global MULTICASTGLOBALCONFIGS_STR
     global MULTICASTRPS_STR
     global CELLULAR_MODULES_SIM_SECURITY_STR
     global ELEMENT_CELLULAR_MODULES_STR
     global ELEMENT_CELLULAR_MODULES_FIRMWARE_STR
     global RADII_STR
     global MULTICASTSOURCESITECONFIGS_STR
+    global DEVICE_ID_CONFIGS_STR
 
     if not STRIP_VERSIONS:
         # Config container strings
         SITES_STR = add_version_to_object(sdk.get.sites, "sites")
         ELEMENTS_STR = add_version_to_object(sdk.get.elements, "elements")
         WANINTERFACES_STR = add_version_to_object(sdk.get.waninterfaces, "waninterfaces")
         LANNETWORKS_STR = add_version_to_object(sdk.get.lannetworks, "lannetworks")
@@ -655,15 +657,16 @@
         SITE_IPFIXLOCALPREFIXES_STR = add_version_to_object(sdk.get.site_ipfixlocalprefixes, "site_ipfix_localprefixes")
         MULTICASTGLOBALCONFIGS_STR = add_version_to_object(sdk.get.multicastglobalconfigs, "multicastglobalconfigs")
         MULTICASTRPS_STR = add_version_to_object(sdk.get.multicastrps, "multicastrps")
         CELLULAR_MODULES_SIM_SECURITY_STR = add_version_to_object(sdk.get.cellular_modules_sim_security, "cellular_modules_sim_security")
         ELEMENT_CELLULAR_MODULES_STR = add_version_to_object(sdk.get.element_cellular_modules, "element_cellular_modules")
         ELEMENT_FIRMWARE_CELLULAR_MODULES_STR = add_version_to_object(sdk.get.element_cellular_modules_firmware, "element_cellular_modules_firmware")
         RADII_STR = add_version_to_object(sdk.get.radii, "radii")
-        MULTICASTSOURCESITECONFIGS_STR = add_version_to_object(sdk.get.radii, "multicastsourcesiteconfigs")
+        MULTICASTSOURCESITECONFIGS_STR = add_version_to_object(sdk.get.multicastsourcesiteconfigs, "multicastsourcesiteconfigs")
+        DEVICE_ID_CONFIGS_STR = add_version_to_object(sdk.get.deviceidconfigs, "deviceidconfigs")
 
 def strip_meta_attributes(obj, leave_name=False, report_id=None):
     """
     Strip meta attributes and names
     :param obj: CloudGenix config item dict.
     :param leave_name: Bool, Leave 'name' field in dict
     :param report_id: Bool or None, Leave 'id' field in dict. If None, uses global REPORT_ID
@@ -977,14 +980,26 @@
     for multicastsourcesiteconfigs in multicastsourcesiteconfigs_items:
         multicastsourcesiteconfigs_template = copy.deepcopy(multicastsourcesiteconfigs)
         strip_meta_attributes(multicastsourcesiteconfigs_template)
         site[MULTICASTSOURCESITECONFIGS_STR].append(multicastsourcesiteconfigs_template)
 
     delete_if_empty(site, MULTICASTSOURCESITECONFIGS_STR)
 
+    site[DEVICE_ID_CONFIGS_STR] = []
+    response = sdk.get.deviceidconfigs(site['id'])
+    if not response.cgx_status:
+        throw_error("Device ID Config Fetch Failed: ", response)
+    deviceidconfigs_items = response.cgx_content['items']
+    for device_config in deviceidconfigs_items:
+        device_config_template = copy.deepcopy(device_config)
+        strip_meta_attributes(device_config_template)
+        site[DEVICE_ID_CONFIGS_STR].append(device_config_template)
+
+    delete_if_empty(site, DEVICE_ID_CONFIGS_STR)
+
     # Get Elements
     site[ELEMENTS_STR] = {}
     dup_name_dict_elements = {}
     for element in ELEMENTS:
         if element['site_id'] != site['id']:
             continue
 
@@ -1774,14 +1789,24 @@
                     for spoke_ha_config_track_interfaces_entry in spoke_ha_config_track_interfaces:
                         spoke_ha_config_track_interfaces_entry_template = \
                             copy.deepcopy(spoke_ha_config_track_interfaces_entry)
                         name_lookup_in_template(spoke_ha_config_track_interfaces_entry_template,
                                                 'interface_id', id_name_cache)
                         spoke_ha_config_track_interfaces_template.append(spoke_ha_config_track_interfaces_entry_template)
                     spoke_ha_config_track_template['interfaces'] = spoke_ha_config_track_interfaces_template
+                spoke_ha_config_track_waninterfaces = spoke_ha_config_track.get("waninterfaces")
+                if spoke_ha_config_track_waninterfaces:
+                    spoke_ha_config_track_waninterfaces_template = []
+                    for spoke_ha_config_track_waninterfaces_entry in spoke_ha_config_track_waninterfaces:
+                        spoke_ha_config_track_waninterfaces_entry_template = \
+                            copy.deepcopy(spoke_ha_config_track_waninterfaces_entry)
+                        name_lookup_in_template(spoke_ha_config_track_waninterfaces_entry_template,
+                                                'wan_interface_id', id_name_cache)
+                        spoke_ha_config_track_waninterfaces_template.append(spoke_ha_config_track_waninterfaces_entry_template)
+                    spoke_ha_config_track_template['waninterfaces'] = spoke_ha_config_track_waninterfaces_template
                 spoke_ha_config_template['track'] = spoke_ha_config_track_template
             element_template['spoke_ha_config'] = spoke_ha_config_template
 
         # check for duplicate names
         checked_element_name = check_name(element['name'], dup_name_dict_elements, 'Element',
                                           error_site_txt="{0}({1})".format(error_site_name,
                                                                            site_id))
@@ -2076,18 +2101,18 @@
     # Allow Controller modification and debug level sets.
     controller_group = parser.add_argument_group('API', 'These options change how this program connects to the API.')
     controller_group.add_argument("--controller", "-C",
                                   help="Controller URI, ex. https://api.elcapitan.cloudgenix.com",
                                   default=None)
 
     login_group = parser.add_argument_group('Login', 'These options allow skipping of interactive login')
-    login_group.add_argument("--email", "-E", help="Use this email as User Name instead of cloudgenix_settings.py "
+    login_group.add_argument("--email", "-E", help="Use this email as User Name instead of cloudgenix_settings.py.example "
                                                    "or prompting",
                              default=None)
-    login_group.add_argument("--password", "-PW", help="Use this Password instead of cloudgenix_settings.py "
+    login_group.add_argument("--password", "-PW", help="Use this Password instead of cloudgenix_settings.py.example "
                                                        "or prompting",
                              default=None)
     login_group.add_argument("--insecure", "-I", help="Do not verify SSL certificate",
                              action='store_true',
                              default=False)
     login_group.add_argument("--noregion", "-NR", help="Ignore Region-based redirection.",
                              dest='ignore_region', action='store_true', default=False)
```

### Comparing `cloudgenix_config-1.9.0b2/cloudgenix_config.egg-info/PKG-INFO` & `cloudgenix_config-2.0.0b1/cloudgenix_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix-config
-Version: 1.9.0b2
+Version: 2.0.0b1
 Summary: Configuration exporting and Continuous Integration (CI) capable configuration importing for the CloudGenix Cloud Controller.
 Home-page: https://github.com/CloudGenix/cloudgenix_config
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix_config.svg)](https://pypi.org/project/cloudgenix_config/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix_config.svg)](https://pypi.org/project/cloudgenix_config/)
 [![Downloads](https://pepy.tech/badge/cloudgenix-config)](https://pepy.tech/project/cloudgenix-config)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix_config.svg?color=brightgreen)](https://pypi.org/project/cloudgenix_config/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/cloudgenix_config.svg)](https://github.com/CloudGenix/cloudgenix_config/issues)
-# CloudGenix Config (Preview)
+# CloudGenix Config 
 Configuration exporting and Continuous Integration (CI) capable configuration importing for the CloudGenix Cloud Controller.
 
 #### Synopsis
 Enables export and import of configurations and templates from the CloudGenix Cloud Controller. Also, the Import of 
 configuration is designed to be run on file change, to maintain configuration state on the Cloud Controller.
 
 #### Features
@@ -124,14 +124,15 @@
  - For ION 9000, if trying to configure a bypasspair and the port with the same name (12,13,14,15,16), configuration pushes via do_site have to be done in the following two steps:
      - Include only interface configuration of type port and use the do_site utility to push this configuration first.
      - Update the YAML file to remove the interface configuration of type port, include interface configuration of type bypasspair and use the do_site utiltiy to push the bypasspair configuration.
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **2.0.0** | **b1** | Support for Cloudgenix SDK 6.2.1b1, Bug fixes - CGSDW-12214, CGSDW-11898|
 | **1.9.0** | **b2** | Bug fixes - CGCBL-1251, CGCBL-1578|
 |           | **b1** | Support for Cloudgenix SDK 6.1.1b1, bug fixes|
 | **1.8.0** | **b1** | Support for Cloudgenix SDK 6.0.2b1, Fix for CGCBL-1399, CGCBL-1347|
 | **1.7.0** | **b3** | Bug fixes|
 |           | **b2** | Fix for CGCBL-336, #73, #74 and CGESC-700|
 |           | **b1** | Support for CloudGenix SDK 6.0.1b1, bug fixes|
 | **1.6.0** | **b2** | Minor bug fixes |
```

### Comparing `cloudgenix_config-1.9.0b2/setup.py` & `cloudgenix_config-2.0.0b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='cloudgenix_config',
-      version='1.9.0b2',
+      version='2.0.0b1',
       description='Configuration exporting and Continuous Integration (CI) capable configuration importing for the '
                   'CloudGenix Cloud Controller.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/CloudGenix/cloudgenix_config',
       author='CloudGenix Developer Support',
       author_email='developers@cloudgenix.com',
       license='MIT',
       install_requires=[
-            'cloudgenix >= 6.1.1b1, < 6.1.3b1',
+            'cloudgenix >= 6.2.1b1, < 6.3.1b1',
             'PyYAML >= 5.3'
       ],
       packages=['cloudgenix_config'],
       entry_points={
             'console_scripts': [
                   'do_site = cloudgenix_config.do:go',
                   'pull_site = cloudgenix_config.pull:go',
```

