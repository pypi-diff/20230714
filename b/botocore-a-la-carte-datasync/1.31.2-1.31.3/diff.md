# Comparing `tmp/botocore-a-la-carte-datasync-1.31.2.tar.gz` & `tmp/botocore-a-la-carte-datasync-1.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-datasync-1.31.2.tar", last modified: Wed Jul 12 01:44:28 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-datasync-1.31.3.tar", last modified: Fri Jul 14 01:46:04 2023, max compression
```

## Comparing `botocore-a-la-carte-datasync-1.31.2.tar` & `botocore-a-la-carte-datasync-1.31.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 01:44:28.000000 botocore-a-la-carte-datasync-1.31.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-12 01:44:12.000000 botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 01:44:12.000000 botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-12 01:44:12.000000 botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   220762 2023-07-12 01:44:12.000000 botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/botocore_a_la_carte_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-12 01:44:28.000000 botocore-a-la-carte-datasync-1.31.2/botocore_a_la_carte_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-12 01:44:28.000000 botocore-a-la-carte-datasync-1.31.2/botocore_a_la_carte_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:28.000000 botocore-a-la-carte-datasync-1.31.2/botocore_a_la_carte_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:44:28.000000 botocore-a-la-carte-datasync-1.31.2/botocore_a_la_carte_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:44:28.463161 botocore-a-la-carte-datasync-1.31.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-12 01:44:28.000000 botocore-a-la-carte-datasync-1.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:04.000000 botocore-a-la-carte-datasync-1.31.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-14 01:45:45.000000 botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:45.000000 botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-14 01:45:45.000000 botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220116 2023-07-14 01:45:45.000000 botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/botocore_a_la_carte_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-14 01:46:04.000000 botocore-a-la-carte-datasync-1.31.3/botocore_a_la_carte_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-14 01:46:04.000000 botocore-a-la-carte-datasync-1.31.3/botocore_a_la_carte_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:04.000000 botocore-a-la-carte-datasync-1.31.3/botocore_a_la_carte_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:04.000000 botocore-a-la-carte-datasync-1.31.3/botocore_a_la_carte_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:04.502598 botocore-a-la-carte-datasync-1.31.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-14 01:46:04.000000 botocore-a-la-carte-datasync-1.31.3/setup.py
```

### Comparing `botocore-a-la-carte-datasync-1.31.2/LICENSE.txt` & `botocore-a-la-carte-datasync-1.31.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-datasync-1.31.2/PKG-INFO` & `botocore-a-la-carte-datasync-1.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-datasync
-Version: 1.31.2
+Version: 1.31.3
 Summary: datasync data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json` & `botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/paginators-1.json` & `botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-datasync-1.31.2/botocore/data/datasync/2018-11-09/service-2.json` & `botocore-a-la-carte-datasync-1.31.3/botocore/data/datasync/2018-11-09/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899913475034651%*

 * *Differences: {"'documentation'": "'<fullname>DataSync</fullname> <p>DataSync is an online data movement and "*

 * *                    'discovery service that simplifies data migration and helps you quickly, '*

 * *                    'easily, and securely transfer your file or object data to, from, and between '*

 * *                    'Amazon Web Services storage services.</p> <p>This API interface reference '*

 * *                    'includes documentation for using DataSync programmatically. For complete '*

 * *                    'inform […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<fullname>DataSync</fullname> <p>DataSync is a managed data transfer service that makes it simpler for you to automate moving data between on-premises storage and Amazon Web Services storage services. You also can use DataSync to transfer data between other cloud providers and Amazon Web Services storage services.</p> <p>This API interface reference includes documentation for using DataSync programmatically. For complete information, see the <i> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/what-is-datasync.html\">DataSync User Guide</a> </i>.</p>",
+    "documentation": "<fullname>DataSync</fullname> <p>DataSync is an online data movement and discovery service that simplifies data migration and helps you quickly, easily, and securely transfer your file or object data to, from, and between Amazon Web Services storage services.</p> <p>This API interface reference includes documentation for using DataSync programmatically. For complete information, see the <i> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/what-is-datasync.html\">DataSync User Guide</a> </i>.</p>",
     "metadata": {
         "apiVersion": "2018-11-09",
         "endpointPrefix": "datasync",
         "jsonVersion": "1.1",
         "protocol": "json",
         "serviceAbbreviation": "DataSync",
         "serviceFullName": "AWS DataSync",
@@ -58,15 +58,15 @@
             },
             "name": "CancelTaskExecution",
             "output": {
                 "shape": "CancelTaskExecutionResponse"
             }
         },
         "CreateAgent": {
-            "documentation": "<p>Activates an DataSync agent that you have deployed in your storage environment. The activation process associates your agent with your account. In the activation process, you specify information such as the Amazon Web Services Region that you want to activate the agent in. You activate the agent in the Amazon Web Services Region where your target locations (in Amazon S3 or Amazon EFS) reside. Your tasks are created in this Amazon Web Services Region.</p> <p>You can activate the agent in a VPC (virtual private cloud) or provide the agent access to a VPC endpoint so you can run tasks without going over the public internet.</p> <p>You can use an agent for more than one location. If a task uses multiple agents, all of them need to have status AVAILABLE for the task to run. If you use multiple agents for a source location, the status of all the agents must be AVAILABLE for the task to run. </p> <p>Agents are automatically updated by Amazon Web Services on a regular basis, using a mechanism that ensures minimal interruption to your tasks.</p>",
+            "documentation": "<p>Activates an DataSync agent that you've deployed in your storage environment. The activation process associates the agent with your Amazon Web Services account.</p> <p>If you haven't deployed an agent yet, see the following topics to learn more:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/agent-requirements.html\">Agent requirements</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/configure-agent.html\">Create an agent</a> </p> </li> </ul> <note> <p>If you're transferring between Amazon Web Services storage services, you don't need a DataSync agent. </p> </note>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalException"
                 }
@@ -1466,48 +1466,48 @@
             "min": 60,
             "type": "integer"
         },
         "CreateAgentRequest": {
             "documentation": "<p>CreateAgentRequest</p>",
             "members": {
                 "ActivationKey": {
-                    "documentation": "<p>Your agent activation key. You can get the activation key either by sending an HTTP GET request with redirects that enable you to get the agent IP address (port 80). Alternatively, you can get it from the DataSync console.</p> <p>The redirect URL returned in the response provides you the activation key for your agent in the query string parameter <code>activationKey</code>. It might also include other activation-related parameters; however, these are merely defaults. The arguments you pass to this API call determine the actual configuration of your agent.</p> <p>For more information, see Activating an Agent in the <i>DataSync User Guide.</i> </p>",
+                    "documentation": "<p>Specifies your DataSync agent's activation key. If you don't have an activation key, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/activate-agent.html\">Activate your agent</a>.</p>",
                     "shape": "ActivationKey"
                 },
                 "AgentName": {
-                    "documentation": "<p>The name you configured for your agent. This value is a text reference that is used to identify the agent in the console.</p>",
+                    "documentation": "<p>Specifies a name for your agent. You can see this name in the DataSync console.</p>",
                     "shape": "TagValue"
                 },
                 "SecurityGroupArns": {
-                    "documentation": "<p>The ARNs of the security groups used to protect your data transfer task subnets. See <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_Ec2Config.html#DataSync-Type-Ec2Config-SecurityGroupArns\">SecurityGroupArns</a>.</p>",
+                    "documentation": "<p>Specifies the Amazon Resource Name (ARN) of the security group that protects your task's <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/datasync-network.html#required-network-interfaces\">network interfaces</a> when <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/choose-service-endpoint.html#choose-service-endpoint-vpc\">using a virtual private cloud (VPC) endpoint</a>.</p>",
                     "shape": "PLSecurityGroupArnList"
                 },
                 "SubnetArns": {
-                    "documentation": "<p>The Amazon Resource Names (ARNs) of the subnets in which DataSync will create elastic network interfaces for each data transfer task. The agent that runs a task must be private. When you start a task that is associated with an agent created in a VPC, or one that has access to an IP address in a VPC, then the task is also private. In this case, DataSync creates four network interfaces for each task in your subnet. For a data transfer to work, the agent must be able to route to all these four network interfaces.</p>",
+                    "documentation": "<p>Specifies the ARN of the subnet where you want to run your DataSync task when using a VPC endpoint. This is the subnet where DataSync creates and manages the <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/datasync-network.html#required-network-interfaces\">network interfaces</a> for your transfer.</p>",
                     "shape": "PLSubnetArnList"
                 },
                 "Tags": {
-                    "documentation": "<p>The key-value pair that represents the tag that you want to associate with the agent. The value can be an empty string. This value helps you manage, filter, and search for your agents.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. </p> </note>",
+                    "documentation": "<p>Specifies labels that help you categorize, filter, and search for your Amazon Web Services resources. We recommend creating at least one tag for your agent.</p>",
                     "shape": "InputTagList"
                 },
                 "VpcEndpointId": {
-                    "documentation": "<p>The ID of the VPC (virtual private cloud) endpoint that the agent has access to. This is the client-side VPC endpoint, also called a PrivateLink. If you don't have a PrivateLink VPC endpoint, see <a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/endpoint-service.html#create-endpoint-service\">Creating a VPC Endpoint Service Configuration</a> in the Amazon VPC User Guide.</p> <p>VPC endpoint ID looks like this: <code>vpce-01234d5aff67890e1</code>.</p>",
+                    "documentation": "<p>Specifies the ID of the VPC endpoint that you want your agent to connect to. For example, a VPC endpoint ID looks like <code>vpce-01234d5aff67890e1</code>.</p> <important> <p>The VPC endpoint you use must include the DataSync service name (for example, <code>com.amazonaws.us-east-2.datasync</code>).</p> </important>",
                     "shape": "VpcEndpointId"
                 }
             },
             "required": [
                 "ActivationKey"
             ],
             "type": "structure"
         },
         "CreateAgentResponse": {
             "documentation": "<p>CreateAgentResponse</p>",
             "members": {
                 "AgentArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the agent. Use the <code>ListAgents</code> operation to return a list of agents for your account and Amazon Web Services Region.</p>",
+                    "documentation": "<p>The ARN of the agent that you just activated. Use the <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/API_ListAgents.html\">ListAgents</a> operation to return a list of agents in your Amazon Web Services account and Amazon Web Services Region.</p>",
                     "shape": "AgentArn"
                 }
             },
             "type": "structure"
         },
         "CreateLocationEfsRequest": {
             "documentation": "<p>CreateLocationEfsRequest</p>",
@@ -1691,15 +1691,15 @@
                     "shape": "FsxWindowsSubdirectory"
                 },
                 "Tags": {
                     "documentation": "<p>Specifies labels that help you categorize, filter, and search for your Amazon Web Services resources. We recommend creating at least a name tag for your location.</p>",
                     "shape": "InputTagList"
                 },
                 "User": {
-                    "documentation": "<p>Specifies the user who has the permissions to access files and folders in the file system.</p> <p>For information about choosing a user name that ensures sufficient permissions to files, folders, and metadata, see <a href=\"create-fsx-location.html#FSxWuser\">user</a>.</p>",
+                    "documentation": "<p>Specifies the user who has the permissions to access files, folders, and metadata in your file system.</p> <p>For information about choosing a user with sufficient permissions, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/create-fsx-location.html#create-fsx-windows-location-permissions\">Required permissions</a>.</p>",
                     "shape": "SmbUser"
                 }
             },
             "required": [
                 "FsxFilesystemArn",
                 "SecurityGroupArns",
                 "User",
@@ -1844,15 +1844,15 @@
                     "shape": "ObjectStorageBucketName"
                 },
                 "SecretKey": {
                     "documentation": "<p>Specifies the secret key (for example, a password) if credentials are required to authenticate with the object storage server.</p>",
                     "shape": "ObjectStorageSecretKey"
                 },
                 "ServerCertificate": {
-                    "documentation": "<p>Specifies a certificate to authenticate with an object storage system that uses a private or self-signed certificate authority (CA). You must specify a Base64-encoded <code>.pem</code> file (for example, <code>file:///home/user/.ssh/storage_sys_certificate.pem</code>). The certificate can be up to 32768 bytes (before Base64 encoding).</p> <p>To use this parameter, configure <code>ServerProtocol</code> to <code>HTTPS</code>.</p>",
+                    "documentation": "<p>Specifies a file with the certificates that are used to sign the object storage server's certificate (for example, <code>file:///home/user/.ssh/storage_sys_certificate.pem</code>). The file you specify must include the following:</p> <ul> <li> <p>The certificate of the signing certificate authority (CA)</p> </li> <li> <p>Any intermediate certificates</p> </li> <li> <p>base64 encoding</p> </li> <li> <p>A <code>.pem</code> extension</p> </li> </ul> <p>The file can be up to 32768 bytes (before base64 encoding).</p> <p>To use this parameter, configure <code>ServerProtocol</code> to <code>HTTPS</code>.</p>",
                     "shape": "ObjectStorageCertificate"
                 },
                 "ServerHostname": {
                     "documentation": "<p>Specifies the domain name or IP address of the object storage server. A DataSync agent uses this hostname to mount the object storage server in a network.</p>",
                     "shape": "ServerHostname"
                 },
                 "ServerPort": {
@@ -3887,14 +3887,18 @@
                     "documentation": "<p>The storage space that's being used in a cluster.</p>",
                     "shape": "NonNegativeLong"
                 },
                 "ClusterName": {
                     "documentation": "<p>The name of the cluster.</p>",
                     "shape": "PtolemyString"
                 },
+                "LunCount": {
+                    "documentation": "<p>The number of LUNs (logical unit numbers) in the cluster.</p>",
+                    "shape": "NonNegativeLong"
+                },
                 "MaxP95Performance": {
                     "documentation": "<p>The performance data that DataSync Discovery collects about the cluster.</p>",
                     "shape": "MaxP95Performance"
                 },
                 "NfsExportedVolumes": {
                     "documentation": "<p>The number of NFS volumes in the cluster.</p>",
                     "shape": "NonNegativeLong"
@@ -3931,14 +3935,18 @@
                     "documentation": "<p>The universally unique identifier (UUID) of the cluster associated with the SVM.</p>",
                     "shape": "PtolemyUUID"
                 },
                 "EnabledProtocols": {
                     "documentation": "<p>The data transfer protocols (such as NFS) configured for the SVM.</p>",
                     "shape": "EnabledProtocols"
                 },
+                "LunCount": {
+                    "documentation": "<p>The number of LUNs (logical unit numbers) in the SVM.</p>",
+                    "shape": "NonNegativeLong"
+                },
                 "MaxP95Performance": {
                     "documentation": "<p>The performance data that DataSync Discovery collects about the SVM.</p>",
                     "shape": "MaxP95Performance"
                 },
                 "NfsExportedVolumes": {
                     "documentation": "<p>The number of NFS volumes in the SVM.</p>",
                     "shape": "NonNegativeLong"
@@ -3999,14 +4007,18 @@
                     "documentation": "<p>The number of CIFS shares in the volume.</p>",
                     "shape": "NonNegativeLong"
                 },
                 "LogicalCapacityUsed": {
                     "documentation": "<p>The storage space that's being used in the volume without accounting for compression or deduplication.</p>",
                     "shape": "NonNegativeLong"
                 },
+                "LunCount": {
+                    "documentation": "<p>The number of LUNs (logical unit numbers) in the volume.</p>",
+                    "shape": "NonNegativeLong"
+                },
                 "MaxP95Performance": {
                     "documentation": "<p>The performance data that DataSync Discovery collects about the volume.</p>",
                     "shape": "MaxP95Performance"
                 },
                 "NfsExported": {
                     "documentation": "<p>The number of NFS volumes in the volume.</p>",
                     "shape": "PtolemyBoolean"
@@ -4211,15 +4223,15 @@
                     "shape": "PreserveDevices"
                 },
                 "SecurityDescriptorCopyFlags": {
                     "documentation": "<p>Specifies which components of the SMB security descriptor are copied from source to destination objects. </p> <p>This value is only used for transfers between SMB and Amazon FSx for Windows File Server locations or between two FSx for Windows File Server locations. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/special-files.html\">how DataSync handles metadata</a>.</p> <p>Default value: <code>OWNER_DACL</code> </p> <p> <code>OWNER_DACL</code>: For each copied object, DataSync copies the following metadata:</p> <ul> <li> <p>The object owner.</p> </li> <li> <p>NTFS discretionary access control lists (DACLs), which determine whether to grant access to an object.</p> <p>DataSync won't copy NTFS system access control lists (SACLs) with this option.</p> </li> </ul> <p> <code>OWNER_DACL_SACL</code>: For each copied object, DataSync copies the following metadata:</p> <ul> <li> <p>The object owner.</p> </li> <li> <p>NTFS discretionary access control lists (DACLs), which determine whether to grant access to an object.</p> </li> <li> <p>SACLs, which are used by administrators to log attempts to access a secured object.</p> <p>Copying SACLs requires granting additional permissions to the Windows user that DataSync uses to access your SMB location. For information about choosing a user that ensures sufficient permissions to files, folders, and metadata, see <a href=\"create-smb-location.html#SMBuser\">user</a>.</p> </li> </ul> <p> <code>NONE</code>: None of the SMB security descriptor components are copied. Destination objects are owned by the user that was provided for accessing the destination location. DACLs and SACLs are set based on the destination server\u2019s configuration. </p>",
                     "shape": "SmbSecurityDescriptorCopyFlags"
                 },
                 "TaskQueueing": {
-                    "documentation": "<p>Specifies whether tasks should be queued before executing the tasks. The default is <code>ENABLED</code>, which means the tasks will be queued.</p> <p>If you use the same agent to run multiple tasks, you can enable the tasks to run in series. For more information, see <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/run-task.html#queue-task-execution\">Queueing task executions</a>.</p>",
+                    "documentation": "<p>Specifies whether your transfer tasks should be put into a queue during certain scenarios when <a href=\"https://docs.aws.amazon.com/datasync/latest/userguide/run-task.html#running-multiple-tasks\">running multiple tasks</a>. This is <code>ENABLED</code> by default.</p>",
                     "shape": "TaskQueueing"
                 },
                 "TransferMode": {
                     "documentation": "<p>Determines whether DataSync transfers only the data and metadata that differ between the source and the destination location or transfers all the content from the source (without comparing what's in the destination).</p> <p> <code>CHANGED</code>: DataSync copies only data or metadata that is new or different content from the source location to the destination location.</p> <p> <code>ALL</code>: DataSync copies all source location content to the destination (without comparing what's in the destination).</p>",
                     "shape": "TransferMode"
                 },
                 "Uid": {
```

### Comparing `botocore-a-la-carte-datasync-1.31.2/botocore_a_la_carte_datasync.egg-info/PKG-INFO` & `botocore-a-la-carte-datasync-1.31.3/botocore_a_la_carte_datasync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-datasync
-Version: 1.31.2
+Version: 1.31.3
 Summary: datasync data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-datasync-1.31.2/setup.py` & `botocore-a-la-carte-datasync-1.31.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-datasync',
-    version="1.31.2",
+    version="1.31.3",
     description='datasync data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/datasync/*/*.json'],
```

