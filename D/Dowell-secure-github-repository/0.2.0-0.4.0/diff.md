# Comparing `tmp/Dowell secure github repository-0.2.0.tar.gz` & `tmp/Dowell secure github repository-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dowell secure github repository-0.2.0.tar", last modified: Fri Jul 14 16:32:03 2023, max compression
+gzip compressed data, was "Dowell secure github repository-0.4.0.tar", last modified: Fri Jul 14 16:51:40 2023, max compression
```

## Comparing `Dowell secure github repository-0.2.0.tar` & `Dowell secure github repository-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:32:03.975653 Dowell secure github repository-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:32:03.969438 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/
--rw-rw-rw-   0        0        0     5379 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5379 2023-07-14 16:32:03.974231 Dowell secure github repository-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5062 2023-07-14 15:56:02.000000 Dowell secure github repository-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 16:32:03.971453 Dowell secure github repository-0.2.0/doWell_secure_github_repository/
--rw-rw-rw-   0        0        0       64 2023-07-14 15:53:03.000000 Dowell secure github repository-0.2.0/doWell_secure_github_repository/__init__.py
--rw-rw-rw-   0        0        0     3299 2023-07-14 15:53:20.000000 Dowell secure github repository-0.2.0/doWell_secure_github_repository/doWell_secure_github_repository.py
--rw-rw-rw-   0        0        0       42 2023-07-14 16:32:03.975653 Dowell secure github repository-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      756 2023-07-14 16:30:08.000000 Dowell secure github repository-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:51:40.970025 Dowell secure github repository-0.4.0/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:51:40.965368 Dowell secure github repository-0.4.0/Dowell_secure_github_repository.egg-info/
+-rw-rw-rw-   0        0        0     4826 2023-07-14 16:51:40.000000 Dowell secure github repository-0.4.0/Dowell_secure_github_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-14 16:51:40.000000 Dowell secure github repository-0.4.0/Dowell_secure_github_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:51:40.000000 Dowell secure github repository-0.4.0/Dowell_secure_github_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 16:51:40.000000 Dowell secure github repository-0.4.0/Dowell_secure_github_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 16:51:40.000000 Dowell secure github repository-0.4.0/Dowell_secure_github_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4826 2023-07-14 16:51:40.970025 Dowell secure github repository-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4515 2023-07-14 16:51:30.000000 Dowell secure github repository-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 16:51:40.967521 Dowell secure github repository-0.4.0/doWell_secure_github_repository/
+-rw-rw-rw-   0        0        0       64 2023-07-14 15:53:03.000000 Dowell secure github repository-0.4.0/doWell_secure_github_repository/__init__.py
+-rw-rw-rw-   0        0        0     3299 2023-07-14 15:53:20.000000 Dowell secure github repository-0.4.0/doWell_secure_github_repository/doWell_secure_github_repository.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 16:51:40.970025 Dowell secure github repository-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-07-14 16:51:26.000000 Dowell secure github repository-0.4.0/setup.py
```

### Comparing `Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/PKG-INFO` & `Dowell secure github repository-0.4.0/Dowell_secure_github_repository.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,93 @@
 Metadata-Version: 2.1
 Name: Dowell-secure-github-repository
-Version: 0.2.0
+Version: 0.4.0
 Summary: Dowell secure github repository from DoWell
 Author: uxlivinglab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
-# Version: 1.0.0
+# Version: 0.4.0
 # Description:
     
-    This API seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The API offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository API ensures the integrity and availability of your code backups.
-    
-    The Secure Repository API offers a range of powerful features to enhance code backup:
-    
-    - Repository Clone: The API enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
-    - Webhooks Integration: With seamless integration with Github's webhooks, the API automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the API captures these changes in real-time, ensuring that your backups are always up to date.
-    - Backup Reports: The Secure Repository API generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
-    - Repository Reports: In addition to backup reports, the API also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
+This API seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The API offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository API ensures the integrity and availability of your code backups.
+
+The Secure Repository API offers a range of powerful features to enhance code backup:
+
+- Repository Clone: The API enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
+- Webhooks Integration: With seamless integration with Github's webhooks, the API automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the API captures these changes in real-time, ensuring that your backups are always up to date.
+- Backup Reports: The Secure Repository API generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
+- Repository Reports: In addition to backup reports, the API also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
 # Installation:
-    - Install the package using pip:
-        
-        ```
-        pip install doWell_secure_github_repository
-        
-        ```
+- Install the package using pip: 
+    
+    `pip install doWell_secure_github_repository`
         
 # Usage:
-    - Import the package and create an instance of the `SecureRepositoryAPI` class:
-        
-        ```
-        from dowell_secure_repository_api import SecureRepositoryAPI
-        
-        api = SecureRepositoryAPI(api_key)
-        
-        ```
+- Import the package and create an instance of the `SecureRepositoryAPI` class:
+    
+    `from dowell_secure_repository_api import SecureRepositoryAPI`
+    
+    `api = SecureRepositoryAPI(api_key)`
+    
         
-    - Available methods:
-        - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
-        - `get_backup_reports()`: Retrieves backup reports.
-        - `get_repository_reports()`: Retrieves repository reports.
-        - `__init__(self, api_key)`
-            
-            Description: Initializes an instance of the SecureRepositoryAPI class.
-            
-            Parameters:
-            
-            - `api_key` (str): The API key required for authentication with the Secure Repository API.
-        - `clone_repository(self, repository_url)`
-            
-            Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
-            
-            Parameters:
-            
-            - `repository_url` (str): The URL of the GitHub repository to clone.
-            
-            Returns: The response from the API as a JSON object.
-            
-        - `get_backup_reports(self)`
-            
-            Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
-            
-            Returns: The response from the API as a JSON object.
-            
-        - `get_repository_reports(self)`
-            
-            Description: Retrieves repository reports from the Secure Repository API by making a GET request.
-            
-            Returns: The response from the API as a JSON object.
-            
-        1. Package Name: DoWell-Secure-Repository-API
-# Example:
+- Available methods:
+- `clone_repository(repository_url)`: Clones a GitHub repository for backup.
+- `get_backup_reports()`: Retrieves backup reports.
+- `get_repository_reports()`: Retrieves repository reports.
+- `__init__(self, api_key)`
+    
+    Description: Initializes an instance of the SecureRepositoryAPI class.
+    
+    Parameters:
+    
+    `api_key` (str): The API key required for authentication with the Secure Repository API.
+- `clone_repository(self, repository_url)`
+    
+    Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
     
-    ```
-    from dowell_secure_repository_api import SecureRepositoryAPI
+    Parameters:
     
-    api = SecureRepositoryAPI(api_key)
-    api.clone_repository(repository_url)
-    api.get_backup_reports()
-    api.get_repository_reports()
+    `repository_url` (str): The URL of the GitHub repository to clone.
+    
+    Returns: The response from the API as a JSON object.
+    
+- `get_backup_reports(self)`
+    
+    Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
+    
+    Returns: The response from the API as a JSON object.
+    
+- `get_repository_reports(self)`
+    
+    Description: Retrieves repository reports from the Secure Repository API by making a GET request.
+    
+    Returns: The response from the API as a JSON object.
+            
+# Example:
     
-    ```
+```python
+from dowell_secure_repository_api import SecureRepositoryAPI
+
+api = SecureRepositoryAPI(api_key)
+api.clone_repository(repository_url)
+api.get_backup_reports()
+api.get_repository_reports()
+
+```
     
 # API Reference:
-    - `SecureRepositoryAPI` class:
-        - `__init__(api_key)`: Initializes the `SecureRepositoryAPI` object with the API key.
-        - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
-        - `get_backup_reports()`: Retrieves backup reports.
-        - `get_repository_reports()`: Retrieves repository reports.
+- `SecureRepositoryAPI` class:
+    - `__init__(api_key)`: Initializes the `SecureRepositoryAPI` object with the API key.
+    - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
+    - `get_backup_reports()`: Retrieves backup reports.
+    - `get_repository_reports()`: Retrieves repository reports.
 # Configuration:
-    - The package requires a valid API key for authentication.
+- The package requires a valid API key for authentication.
 # Dependencies:
-    - requests: Required for making HTTP requests.
-    - json: Required for parsing JSON data.
+- requests: Required for making HTTP requests.
+- json: Required for parsing JSON data.
 # Support:
-    - For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
-    - If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
+- For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
+- If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
 # License:
-    - Specify the license under which your package is released.
+- Apache License 2.0
```

### Comparing `Dowell secure github repository-0.2.0/PKG-INFO` & `Dowell secure github repository-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,99 +1,93 @@
 Metadata-Version: 2.1
 Name: Dowell secure github repository
-Version: 0.2.0
+Version: 0.4.0
 Summary: Dowell secure github repository from DoWell
 Author: uxlivinglab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
-# Version: 1.0.0
+# Version: 0.4.0
 # Description:
     
-    This API seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The API offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository API ensures the integrity and availability of your code backups.
-    
-    The Secure Repository API offers a range of powerful features to enhance code backup:
-    
-    - Repository Clone: The API enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
-    - Webhooks Integration: With seamless integration with Github's webhooks, the API automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the API captures these changes in real-time, ensuring that your backups are always up to date.
-    - Backup Reports: The Secure Repository API generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
-    - Repository Reports: In addition to backup reports, the API also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
+This API seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The API offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository API ensures the integrity and availability of your code backups.
+
+The Secure Repository API offers a range of powerful features to enhance code backup:
+
+- Repository Clone: The API enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
+- Webhooks Integration: With seamless integration with Github's webhooks, the API automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the API captures these changes in real-time, ensuring that your backups are always up to date.
+- Backup Reports: The Secure Repository API generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
+- Repository Reports: In addition to backup reports, the API also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
 # Installation:
-    - Install the package using pip:
-        
-        ```
-        pip install doWell_secure_github_repository
-        
-        ```
+- Install the package using pip: 
+    
+    `pip install doWell_secure_github_repository`
         
 # Usage:
-    - Import the package and create an instance of the `SecureRepositoryAPI` class:
-        
-        ```
-        from dowell_secure_repository_api import SecureRepositoryAPI
-        
-        api = SecureRepositoryAPI(api_key)
-        
-        ```
+- Import the package and create an instance of the `SecureRepositoryAPI` class:
+    
+    `from dowell_secure_repository_api import SecureRepositoryAPI`
+    
+    `api = SecureRepositoryAPI(api_key)`
+    
         
-    - Available methods:
-        - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
-        - `get_backup_reports()`: Retrieves backup reports.
-        - `get_repository_reports()`: Retrieves repository reports.
-        - `__init__(self, api_key)`
-            
-            Description: Initializes an instance of the SecureRepositoryAPI class.
-            
-            Parameters:
-            
-            - `api_key` (str): The API key required for authentication with the Secure Repository API.
-        - `clone_repository(self, repository_url)`
-            
-            Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
-            
-            Parameters:
-            
-            - `repository_url` (str): The URL of the GitHub repository to clone.
-            
-            Returns: The response from the API as a JSON object.
-            
-        - `get_backup_reports(self)`
-            
-            Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
-            
-            Returns: The response from the API as a JSON object.
-            
-        - `get_repository_reports(self)`
-            
-            Description: Retrieves repository reports from the Secure Repository API by making a GET request.
-            
-            Returns: The response from the API as a JSON object.
-            
-        1. Package Name: DoWell-Secure-Repository-API
-# Example:
+- Available methods:
+- `clone_repository(repository_url)`: Clones a GitHub repository for backup.
+- `get_backup_reports()`: Retrieves backup reports.
+- `get_repository_reports()`: Retrieves repository reports.
+- `__init__(self, api_key)`
+    
+    Description: Initializes an instance of the SecureRepositoryAPI class.
+    
+    Parameters:
+    
+    `api_key` (str): The API key required for authentication with the Secure Repository API.
+- `clone_repository(self, repository_url)`
+    
+    Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
     
-    ```
-    from dowell_secure_repository_api import SecureRepositoryAPI
+    Parameters:
     
-    api = SecureRepositoryAPI(api_key)
-    api.clone_repository(repository_url)
-    api.get_backup_reports()
-    api.get_repository_reports()
+    `repository_url` (str): The URL of the GitHub repository to clone.
+    
+    Returns: The response from the API as a JSON object.
+    
+- `get_backup_reports(self)`
+    
+    Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
+    
+    Returns: The response from the API as a JSON object.
+    
+- `get_repository_reports(self)`
+    
+    Description: Retrieves repository reports from the Secure Repository API by making a GET request.
+    
+    Returns: The response from the API as a JSON object.
+            
+# Example:
     
-    ```
+```python
+from dowell_secure_repository_api import SecureRepositoryAPI
+
+api = SecureRepositoryAPI(api_key)
+api.clone_repository(repository_url)
+api.get_backup_reports()
+api.get_repository_reports()
+
+```
     
 # API Reference:
-    - `SecureRepositoryAPI` class:
-        - `__init__(api_key)`: Initializes the `SecureRepositoryAPI` object with the API key.
-        - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
-        - `get_backup_reports()`: Retrieves backup reports.
-        - `get_repository_reports()`: Retrieves repository reports.
+- `SecureRepositoryAPI` class:
+    - `__init__(api_key)`: Initializes the `SecureRepositoryAPI` object with the API key.
+    - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
+    - `get_backup_reports()`: Retrieves backup reports.
+    - `get_repository_reports()`: Retrieves repository reports.
 # Configuration:
-    - The package requires a valid API key for authentication.
+- The package requires a valid API key for authentication.
 # Dependencies:
-    - requests: Required for making HTTP requests.
-    - json: Required for parsing JSON data.
+- requests: Required for making HTTP requests.
+- json: Required for parsing JSON data.
 # Support:
-    - For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
-    - If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
+- For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
+- If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
 # License:
-    - Specify the license under which your package is released.
+- Apache License 2.0
```

### Comparing `Dowell secure github repository-0.2.0/README.md` & `Dowell secure github repository-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,85 @@
-# Version: 1.0.0
+# Version: 0.4.0
 # Description:
     
-    This API seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The API offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository API ensures the integrity and availability of your code backups.
-    
-    The Secure Repository API offers a range of powerful features to enhance code backup:
-    
-    - Repository Clone: The API enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
-    - Webhooks Integration: With seamless integration with Github's webhooks, the API automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the API captures these changes in real-time, ensuring that your backups are always up to date.
-    - Backup Reports: The Secure Repository API generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
-    - Repository Reports: In addition to backup reports, the API also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
+This API seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The API offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository API ensures the integrity and availability of your code backups.
+
+The Secure Repository API offers a range of powerful features to enhance code backup:
+
+- Repository Clone: The API enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
+- Webhooks Integration: With seamless integration with Github's webhooks, the API automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the API captures these changes in real-time, ensuring that your backups are always up to date.
+- Backup Reports: The Secure Repository API generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
+- Repository Reports: In addition to backup reports, the API also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
 # Installation:
-    - Install the package using pip:
-        
-        ```
-        pip install doWell_secure_github_repository
-        
-        ```
+- Install the package using pip: 
+    
+    `pip install doWell_secure_github_repository`
         
 # Usage:
-    - Import the package and create an instance of the `SecureRepositoryAPI` class:
-        
-        ```
-        from dowell_secure_repository_api import SecureRepositoryAPI
-        
-        api = SecureRepositoryAPI(api_key)
-        
-        ```
+- Import the package and create an instance of the `SecureRepositoryAPI` class:
+    
+    `from dowell_secure_repository_api import SecureRepositoryAPI`
+    
+    `api = SecureRepositoryAPI(api_key)`
+    
         
-    - Available methods:
-        - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
-        - `get_backup_reports()`: Retrieves backup reports.
-        - `get_repository_reports()`: Retrieves repository reports.
-        - `__init__(self, api_key)`
-            
-            Description: Initializes an instance of the SecureRepositoryAPI class.
-            
-            Parameters:
-            
-            - `api_key` (str): The API key required for authentication with the Secure Repository API.
-        - `clone_repository(self, repository_url)`
-            
-            Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
-            
-            Parameters:
-            
-            - `repository_url` (str): The URL of the GitHub repository to clone.
-            
-            Returns: The response from the API as a JSON object.
-            
-        - `get_backup_reports(self)`
-            
-            Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
-            
-            Returns: The response from the API as a JSON object.
-            
-        - `get_repository_reports(self)`
-            
-            Description: Retrieves repository reports from the Secure Repository API by making a GET request.
-            
-            Returns: The response from the API as a JSON object.
-            
-        1. Package Name: DoWell-Secure-Repository-API
-# Example:
+- Available methods:
+- `clone_repository(repository_url)`: Clones a GitHub repository for backup.
+- `get_backup_reports()`: Retrieves backup reports.
+- `get_repository_reports()`: Retrieves repository reports.
+- `__init__(self, api_key)`
+    
+    Description: Initializes an instance of the SecureRepositoryAPI class.
+    
+    Parameters:
+    
+    `api_key` (str): The API key required for authentication with the Secure Repository API.
+- `clone_repository(self, repository_url)`
+    
+    Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
     
-    ```
-    from dowell_secure_repository_api import SecureRepositoryAPI
+    Parameters:
     
-    api = SecureRepositoryAPI(api_key)
-    api.clone_repository(repository_url)
-    api.get_backup_reports()
-    api.get_repository_reports()
+    `repository_url` (str): The URL of the GitHub repository to clone.
+    
+    Returns: The response from the API as a JSON object.
+    
+- `get_backup_reports(self)`
+    
+    Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
+    
+    Returns: The response from the API as a JSON object.
+    
+- `get_repository_reports(self)`
+    
+    Description: Retrieves repository reports from the Secure Repository API by making a GET request.
+    
+    Returns: The response from the API as a JSON object.
+            
+# Example:
     
-    ```
+```python
+from dowell_secure_repository_api import SecureRepositoryAPI
+
+api = SecureRepositoryAPI(api_key)
+api.clone_repository(repository_url)
+api.get_backup_reports()
+api.get_repository_reports()
+
+```
     
 # API Reference:
-    - `SecureRepositoryAPI` class:
-        - `__init__(api_key)`: Initializes the `SecureRepositoryAPI` object with the API key.
-        - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
-        - `get_backup_reports()`: Retrieves backup reports.
-        - `get_repository_reports()`: Retrieves repository reports.
+- `SecureRepositoryAPI` class:
+    - `__init__(api_key)`: Initializes the `SecureRepositoryAPI` object with the API key.
+    - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
+    - `get_backup_reports()`: Retrieves backup reports.
+    - `get_repository_reports()`: Retrieves repository reports.
 # Configuration:
-    - The package requires a valid API key for authentication.
+- The package requires a valid API key for authentication.
 # Dependencies:
-    - requests: Required for making HTTP requests.
-    - json: Required for parsing JSON data.
+- requests: Required for making HTTP requests.
+- json: Required for parsing JSON data.
 # Support:
-    - For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
-    - If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
+- For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
+- If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
 # License:
-    - Specify the license under which your package is released.
+- Apache License 2.0
```

### Comparing `Dowell secure github repository-0.2.0/doWell_secure_github_repository/doWell_secure_github_repository.py` & `Dowell secure github repository-0.4.0/doWell_secure_github_repository/doWell_secure_github_repository.py`

 * *Files identical despite different names*

### Comparing `Dowell secure github repository-0.2.0/setup.py` & `Dowell secure github repository-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name="Dowell secure github repository",
-    version="0.2.0",
+    version="0.4.0",
     description="Dowell secure github repository from DoWell",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='uxlivinglab',
     license="Apache License 2.0",
     packages=["doWell_secure_github_repository"],
     include_package_data=True,
```

