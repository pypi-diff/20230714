# Comparing `tmp/ogsapi-0.7.2.tar.gz` & `tmp/ogsapi-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.7.2.tar", last modified: Thu Jul  6 23:44:44 2023, max compression
+gzip compressed data, was "ogsapi-0.7.3.tar", last modified: Fri Jul 14 05:31:21 2023, max compression
```

## Comparing `ogsapi-0.7.2.tar` & `ogsapi-0.7.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.831642 ogsapi-0.7.2/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-07-06 23:44:33.000000 ogsapi-0.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 23:44:44.831642 ogsapi-0.7.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5123 2023-07-06 23:44:33.000000 ogsapi-0.7.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-06 23:44:33.000000 ogsapi-0.7.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 23:44:44.831642 ogsapi-0.7.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.828642 ogsapi-0.7.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.830642 ogsapi-0.7.2/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22383 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/ogs_api_exception.py
--rw-rw-rw-   0 root         (0) root         (0)    14931 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/ogsgame.py
--rw-rw-rw-   0 root         (0) root         (0)     6726 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/ogssocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.831642 ogsapi-0.7.2/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.831642 ogsapi-0.7.2/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)      879 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.215380 ogsapi-0.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-07-14 05:31:08.000000 ogsapi-0.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-14 05:31:21.215380 ogsapi-0.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-07-14 05:31:08.000000 ogsapi-0.7.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-14 05:31:08.000000 ogsapi-0.7.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 05:31:21.215380 ogsapi-0.7.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.212380 ogsapi-0.7.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.214380 ogsapi-0.7.3/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18160 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogs_api_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogscredentials.py
+-rw-rw-rw-   0 root         (0) root         (0)    14974 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogsgame.py
+-rw-rw-rw-   0 root         (0) root         (0)     4088 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogsrestapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6395 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogssocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.214380 ogsapi-0.7.3/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.215380 ogsapi-0.7.3/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/tests/test.py
```

### Comparing `ogsapi-0.7.2/LICENSE` & `ogsapi-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.2/PKG-INFO` & `ogsapi-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.7.2
+Version: 0.7.3
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.7.2/README.md` & `ogsapi-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.2/pyproject.toml` & `ogsapi-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.7.2/src/ogsapi/client.py` & `ogsapi-0.7.3/src/ogsapi/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import requests
+from .ogscredentials import OGSCredentials
 from .ogssocket import OGSSocket
+from .ogsrestapi import OGSRestAPI
 from .ogs_api_exception import OGSApiException
 
 
 # TODO: This will eventually need to be moved to `termination-api` instead of `/api/v1/`
 # TODO: Should probably implement a user class that contains all user info and functions
 # TODO: Break REST API functions into their own class, leaving the OGSClient class to be the interface for the user client
 
@@ -26,202 +27,56 @@
         client_id (str): Client ID from OGS
         client_secret (str): Client Secret from OGS
         username (str): Username of OGS account
         password (str): Password of OGS account
         debug (bool, optional): Enable debug logging. Defaults to False.        
 
     Attributes:
-        client_id (str): Client ID from OGS
-        client_secret (str): Client Secret from OGS
-        username (str): Username of OGS account
-        password (str): Password of OGS account
-        access_token (str): Access Token from OGS
-        refresh_token (str): Refresh Token from OGS
-        user_id (int): User ID from OGS
-        base_url (str): Base URL for OGS API
-        api_ver (str): API version for OGS API
+        credentials (OGSCredentials): Credentials object containing all credentials
+        api (OGSRestAPI): REST API connection to OGS
         sock (OGSSocket): SocketIO connection to OGS
 
     """
-    def __init__(self, client_id, client_secret, username, password, debug: bool = False):
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.username = username
-        self.password = password
-        self.access_token = None
-        # TODO:  Implement refresh token
-        self.refresh_token = None
-        self.user_id = None
-        self.base_url = "https://online-go.com"
-        self.api_ver = "v1"
-
-        # Attempt authentication once everything is defined
-        # TODO: Maybe implement some form of token caching, so we arent making new tokens every time the script runs
-        self.authenticate()
+    def __init__(self, client_id, client_secret, username, password, debug: bool = False, dev: bool = False):
 
-        self.sock = OGSSocket(self.access_token)
+        self.credentials = OGSCredentials(client_id=client_id, client_secret=client_secret,
+                                          username=username, password=password)
+        self.api = OGSRestAPI(self.credentials,dev=dev)
+        self.sock = OGSSocket(self.credentials, debug=debug)
         self.sock.connect()
 
+        self.credentials.user_id = self.user_vitals()
+
     def __del__(self):
         # Disconnect the OGSSocket instance if it exists
         if hasattr(self, 'sock') and self.sock is not None:
             self.sock.disconnect()
 
-    # TODO: All these internal functions should be moved into private functions
-    def authenticate(self):
-        """Authenticate with the OGS API and save the access token and user ID."""
-
-        endpoint = f'{self.base_url}/oauth2/token/'
-        try:
-            response = requests.post(endpoint, data={
-                'client_id': self.client_id,
-                'grant_type': 'password',
-                'username': self.username,
-                'password': self.password
-            }, headers={'Content-Type': 'application/x-www-form-urlencoded'})
-        except requests.exceptions.RequestException as e:
-            raise OGSApiException("Authentication Failed") from e
-
-        if 299 >= response.status_code >= 200:
-            # Save Access Token, Refresh Token, and User ID
-            # TODO: This should probably be made into a user object that has token and ID info
-            self.access_token = response.json()['access_token']
-            self.refresh_token = response.json()['refresh_token']
-            self.user_id = self.user_vitals()['id']
-        else:
-            raise OGSApiException(f"{response.status_code}: {response.reason}")
-
-    # TODO: The GET POST and PUT functions can be refactored into its own class, because DRY
-    def get_rest_endpoint(self, endpoint: str, params: dict = None):
-        """Make a GET request to the OGS REST API.
-        
-        Args:
-            endpoint (str): Endpoint to make request to
-            params (dict, optional): Parameters to pass to the endpoint. Defaults to None.
-            
-        Returns:
-            response (dict): JSON response from the endpoint
-        """
-
-        url = f'{self.base_url}/api/{self.api_ver}{endpoint}'
-        headers = {
-            'Authorization' : f'Bearer {self.access_token}'
-        }
-        try:
-            response = requests.get(url, headers=headers, params=params)
-        except requests.exceptions.RequestException as e:
-            raise OGSApiException("GET Failed") from e
-
-        if 299 >= response.status_code >= 200:
-            return response.json()
-        else:
-            raise OGSApiException(f"{response.status_code}: {response.reason}")
-
-    def post_rest_endpoint(self, endpoint: str, payload: dict, params: dict = None):
-        """Make a POST request to the OGS REST API.
-        
-        Args:
-            endpoint (str): Endpoint to make request to
-            payload (dict): Payload to pass to the endpoint
-            params (dict, optional): Parameters to pass to the endpoint. Defaults to None.
-        
-        Returns:
-            response (dict): JSON response from the endpoint
-        """
-        url = f'{self.base_url}/api/{self.api_ver}{endpoint}'
-        headers = {
-            'Authorization' : f'Bearer {self.access_token}',
-            'Content-Type': 'application/json'
-        }
-        try:
-            response = requests.post(url, headers=headers, json=payload, params=params)
-        except requests.exceptions.RequestException as e:
-            raise OGSApiException("POST Failed") from e
-
-        if 299 >= response.status_code >= 200:
-            return response.json()
-        else:
-            raise OGSApiException(f"{response.status_code}: {response.reason}")
-
-    def put_rest_endpoint(self, endpoint: str, payload: dict, params: dict = None):
-        """Make a PUT request to the OGS REST API.
-        
-        Args:
-            endpoint (str): Endpoint to make request to
-            payload (dict): Payload to pass to the endpoint
-            params (dict, optional): Parameters to pass to the endpoint. Defaults to None.
-            
-        Returns:
-            response (dict): JSON response from the endpoint
-        """
-
-        url = f'{self.base_url}/api/{self.api_ver}{endpoint}'
-        headers = {
-            'Authorization' : f'Bearer {self.access_token}',
-            'Content-Type': 'application/json'
-        }
-        try:
-            response = requests.put(url, headers=headers, json=payload, params=params)
-        except requests.exceptions.RequestException as e:
-            raise OGSApiException("PUT Failed") from e
-
-        if 299 >= response.status_code >= 200:
-            return response.json()
-        else:
-            raise OGSApiException(f"{response.status_code}: {response.reason}")
-
-    def delete_rest_endpoint(self, endpoint: str, payload: dict, params: dict = None):
-        """Make a DELETE request to the OGS REST API.
-        
-        Args:
-            endpoint (str): Endpoint to make request to
-            payload (dict): Payload to pass to the endpoint
-            params (dict, optional): Parameters to pass to the endpoint. Defaults to None.
-        
-        Returns:
-            response (dict): JSON response from the endpoint
-        """
-
-        url = f'{self.base_url}/api/{self.api_ver}{endpoint}'
-        headers = {
-            'Authorization' : f'Bearer {self.access_token}',
-            'Content-Type': 'application/json'
-        }
-        try:
-            response = requests.delete(url, headers=headers, json=payload, params=params)
-        except requests.exceptions.RequestException as e:
-            raise OGSApiException("DELETE Failed") from e
-
-        if 299 >= response.status_code >= 200:
-            return response.json()
-        else:
-            raise OGSApiException(f"{response.status_code}: {response.reason}")
-
     # User Specific Resources: /me
 
     def user_vitals(self):
         """Get the user's vitals.
         
         Returns:
             response (dict): JSON response from the endpoint
         """
 
         endpoint = '/me'
-        return self.get_rest_endpoint(endpoint)
-    
+        return self.api.call_rest_endpoint('GET', endpoint=endpoint).json()
+
     def user_settings(self):
         """Get the user's settings.
         
         Returns:
             response (dict): JSON response from the endpoint
         """
 
         endpoint = '/me/settings/'
-        return self.get_rest_endpoint(endpoint=endpoint)
-    
+        return self.api.call_rest_endpoint('GET', endpoint=endpoint).json()
+
     def update_user_settings(
             self, username: str = None, 
             first_name: str = None, 
             last_name: str = None, 
             private_name: bool = None, 
             country: str = None, 
             website: str = None,
@@ -255,40 +110,40 @@
         if country is not None:
             payload['country'] = country
         if website is not None:
             payload['website'] = website
         if about is not None:
             payload['about'] = about
 
-        endpoint = f'/players/{self.user_id}'
+        endpoint = f'/players/{self.credentials.user_id}'
         # Add the inputs to a payload, only if they are not None
-        return self.put_rest_endpoint(endpoint=endpoint, payload=payload)
+        return self.api.call_rest_endpoint('PUT', endpoint=endpoint, payload=payload).json()
 
     def user_games(self):
         """Get the user's games.
         
         Returns:
             response (dict): JSON response from the endpoint
         """
 
         endpoint = '/me/games'
-        return self.get_rest_endpoint(endpoint)
+        return self.api.call_rest_endpoint('GET', endpoint=endpoint).json()
 
     def user_friends(self, username: str = None):
         """Get the user's friends.
         
         Args:
             username (str, optional): Username of the user to get friends of. Defaults to None.
             
         Returns:
             response (dict): JSON response from the endpoint
         """
 
         endpoint = '/me/friends'
-        return self.get_rest_endpoint(endpoint=endpoint, params={'username' : username})
+        return self.api.call_rest_endpoint('GET', endpoint=endpoint, params={'username' : username}).json()
 
     def send_friend_request(self, username: str):
         """Send a friend request to a user.
         
         Args:
             username (str): Username of the user to send a friend request to.
             
@@ -297,15 +152,15 @@
         """
 
         endpoint = '/me/friends'
         player_id = self.get_player(username)['id']
         payload = {
             "player_id" : player_id
         }
-        return self.post_rest_endpoint(endpoint=endpoint, payload=payload)
+        return self.api.call_rest_endpoint('POST', endpoint=endpoint, payload=payload).json()
 
     def remove_friend(self, username: str):
         """Remove a friend.
         
         Args:
             username (str): Username of the user to remove as a friend.
         
@@ -315,30 +170,30 @@
 
         endpoint = '/me/friends/'
         player_id = self.get_player(username)['id']
         payload = {
             "delete": True,
             "player_id" : player_id
         }
-        return self.post_rest_endpoint(endpoint=endpoint, payload=payload)
+        return self.api.call_rest_endpoint('POST', endpoint=endpoint, payload=payload).json()
 
     # Players: /players
 
     def get_player(self, player_username):
         """Get a player by username.
         
         Args:
             player_username (str): Username of the player to get.
         
         Returns:
             player_data (dict): Player data returned from the endpoint
         """
 
-        endpoint = f'/players/'
-        return self.get_rest_endpoint(endpoint=endpoint, params={'username' : player_username})['results'][0]
+        endpoint = '/players/'
+        return self.api.call_rest_endpoint('GET', endpoint=endpoint, params={'username' : player_username}).json()['results'][0]
 
     # TODO: Need to make these customizable 
     def create_challenge(self, player_username: str = None, **game_settings):
         """Create either an open challenge or a challenge to a specific player.
         The time control settings are built depending on which time control is used.
         Make sure that you pass the correct time control settings for the time control you want to use.
         The other time control settings will be ignored.
@@ -457,19 +312,19 @@
             'invite_only' : game_settings.get('invite_only', False),
         }
 
         if player_username is not None:
             player_id = self.get_player(player_username)['id']
             print(f"Challenging player: {player_username} - {player_id}")
             endpoint = f'/players/{player_id}/challenge/'
-            response = self.post_rest_endpoint(endpoint, challenge)
+            response = self.api.call_rest_endpoint('POST', endpoint, challenge).json()
         else:
             endpoint = '/challenges/'
             print("Creating open challenge")
-            response = self.post_rest_endpoint(endpoint, challenge)
+            response = self.api.call_rest_endpoint('POST', endpoint, challenge).json()
 
         challenge_id = response['challenge']
         game_id = response['game']
         return challenge_id, game_id
 
     # Challenges
 
@@ -479,70 +334,114 @@
         
         Returns:
             challenges (dict): JSON response from the endpoint
         """
 
         endpoint = '/me/challenges/'
         received_challenges = []
-        all_challenges = self.get_rest_endpoint(endpoint)['results']
+        all_challenges = self.api.call_rest_endpoint('GET', endpoint).json()['results']
         for challenge in all_challenges:
-            if challenge['challenger']['id'] != self.user_id:
+            if challenge['challenger']['id'] != self.credentials.user_id:
                 received_challenges.append(challenge)
         return received_challenges
 
     # TODO: Same as above
     def sent_challenges(self):
         """Get all sent challenges.
         
         Returns:
             challenges (dict): JSON response from the endpoint
         """
         endpoint = '/me/challenges'
         sent_challenges = []
-        all_challenges = self.get_rest_endpoint(endpoint)['results']
+        all_challenges = self.api.call_rest_endpoint('GET', endpoint).json()['results']
         for challenge in all_challenges:
-            if challenge['challenger']['id'] == self.user_id:
+            if challenge['challenger']['id'] == self.credentials.user_id:
                 sent_challenges.append(challenge)
         return sent_challenges
-    
+
     def accept_challenge(self, challenge_id):
         """Accept a challenge.
         
         Args:
             challenge_id (str): ID of the challenge to accept.
             
         Returns:
             response (dict): JSON response from the endpoint
         """
 
         endpoint = f'/me/challenges/{challenge_id}/accept'
-        return self.post_rest_endpoint(endpoint=endpoint,payload={})
+        return self.api.call_rest_endpoint('POST', endpoint=endpoint,payload={}).json()
     
     def decline_challenge(self, challenge_id):
         """Decline a challenge.
         
         Args:
             challenge_id (str): ID of the challenge to decline.
         
         Returns:
             response (dict): JSON response from the endpoint
         """
 
         endpoint = f'/me/challenges/{challenge_id}/'
-        return self.delete_rest_endpoint(endpoint=endpoint, payload={})
+        return self.api.call_rest_endpoint('DELETE', endpoint=endpoint, payload={}).json()
 
     def challenge_details(self, challenge_id):
         """Get details of a challenge.
         
         Args:
             challenge_id (str): ID of the challenge to get details of.
             
         Returns:
             response (dict): JSON response from the endpoint
         """
 
         endpoint = f'/me/challenges/{challenge_id}'
-        return self.get_rest_endpoint(endpoint=endpoint)
+        return self.api.call_rest_endpoint('GET', endpoint=endpoint).json()
 
     def game_details(self, game_id):
+        """Get details of a game.
+        
+        Args:
+            game_id (str): ID of the game to get details of.
+            
+        Returns:
+            response (dict): JSON response from the endpoint
+        """
         endpoint = f'/games/{game_id}'
-        return self.get_rest_endpoint(endpoint)
+        return self.api.call_rest_endpoint('GET', endpoint).json()
+
+    def game_reviews(self, game_id):
+        """Get reviews of a game.
+        
+        Args:
+            game_id (str): ID of the game to get reviews of.
+            
+        Returns:
+            response (dict): JSON response from the endpoint
+        """
+        endpoint = f'/games/{game_id}/reviews'
+        return self.api.call_rest_endpoint('GET', endpoint).json()
+
+    def game_png(self, game_id):
+        """Get PNG of a game.
+        
+        Args:
+            game_id (str): ID of the game to get PNG of.
+        
+        Returns:
+            response (bytes): PNG image of the game
+        """
+        endpoint = f'/games/{game_id}/png'
+        return self.api.call_rest_endpoint('GET', endpoint).content
+
+    def game_sgf(self, game_id):
+        """Get SGF of a game.
+        
+        Args:  
+            game_id (str): ID of the game to get SGF of.
+        
+        Returns:
+            response (str): SGF of the game
+        """
+        endpoint = f'/games/{game_id}/sgf'
+        return self.api.call_rest_endpoint('GET', endpoint).text
```

### Comparing `ogsapi-0.7.2/src/ogsapi/ogsgame.py` & `ogsapi-0.7.3/src/ogsapi/ogsgame.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .ogs_api_exception import OGSApiException
 from typing import Callable
+from .ogs_api_exception import OGSApiException
+from .ogscredentials import OGSCredentials
 
 class OGSGame:
     """OGSGame class for handling games connected via the OGSSocket.
     
     Args:
         game_socket (OGSSocket): OGSSocket object to connect to the game.
         game_id (str): ID of the game to connect to.
@@ -35,21 +36,20 @@
         callback_func (dict): Dictionary containing the callback functions.
 
     """
     # Class for handling each OGSGame connected via the OGSSocket
     # To receive data from the game, use the callback function to register functions to be called when data is received.
     # on_move and on_clock are required for the game to function properly, on_undo is only for handling undo requests
     
-    def __init__(self, game_socket, game_id, auth_data, user_data):
+    def __init__(self, game_socket: Callable, credentials: OGSCredentials, game_id):
         self.socket = game_socket
         self.game_id = game_id
-        self.user_data = user_data
-        self.auth_data = auth_data
         # Define callback functions from the API
         self._game_call_backs()
+        self.credentials = credentials
         # Connect to the game
         self.connect()
 
         # Define relevant game data
         self.name: str = None
         self.private: bool = None
         self.white_player: dict = {
@@ -243,15 +243,15 @@
             except TypeError as e:
                 raise OGSApiException("Callback function 'on_undo_canceled' must be Type Callable") from e
     
     # Send functions
     def connect(self):
         """Connect to the game"""
         print(f"Connecting to game {self.game_id}")
-        self.socket.emit(event="game/connect", data={'game_id': self.game_id, 'player_id': self.user_data['id'], 'chat': False})
+        self.socket.emit(event="game/connect", data={'game_id': self.game_id, 'player_id': self.credentials.user_id, 'chat': False})
 
     def disconnect(self):
         """Disconnect from the game"""
         print(f"Disconnecting game {self.game_id}")
         self.socket.emit(event="game/disconnect", data={'game_id': self.game_id})
 
     def pause(self):
@@ -271,71 +271,71 @@
             move (str): The move to submit to the game. Accepts GTP format.
             
         Examples:
             >>> game.move('B2')
         """
 
         print(f"Submitting move {move} to game {self.game_id}")
-        self.socket.emit(event="game/move", data={'auth': self.auth_data['chat_auth'], 'player_id': self.user_data['id'], 'game_id': self.game_id, 'move': move})
+        self.socket.emit(event="game/move", data={'auth': self.credentials.chat_auth, 'player_id': self.credentials.user_id, 'game_id': self.game_id, 'move': move})
 
     def resign(self):
         """Resign the game"""
         print(f"Resigning game {self.game_id}")
-        self.socket.emit(event="game/resign", data={'auth': self.auth_data['chat_auth'], 'game_id': self.game_id})  
+        self.socket.emit(event="game/resign", data={'auth': self.credentials.chat_auth, 'game_id': self.game_id})  
     
     def cancel(self):
         """Cancel the game if within the first few moves"""
         print(f"Canceling game {self.game_id}")
-        self.socket.emit(event="game/cancel", data={'auth': self.auth_data['chat_auth'], 'game_id': self.game_id})
+        self.socket.emit(event="game/cancel", data={'auth': self.credentials.chat_auth, 'game_id': self.game_id})
 
     def undo(self, move: int):
         """Request an undo on the game
 
         Args:
             move (int): The move number to accept the undo at.        
         """
         print(f"Requesting undo on game {self.game_id}")
-        self.socket.emit(event="game/undo/request", data={'auth': self.auth_data['chat_auth'], 'game_id': self.game_id, 'move_number': move})
+        self.socket.emit(event="game/undo/request", data={'auth': self.credentials.chat_auth, 'game_id': self.game_id, 'move_number': move})
 
     def cancel_undo(self, move: int):
         """Cancel an undo request on the game
         
         Args:
             move (int): The move number to accept the undo at.        
         """
         print(f"Canceling undo on game {self.game_id}")
-        self.socket.emit(event="game/undo/cancel", data={'auth': self.auth_data['chat_auth'], 'game_id': self.game_id, 'move_number': move})
+        self.socket.emit(event="game/undo/cancel", data={'auth': self.credentials.chat_auth, 'game_id': self.game_id, 'move_number': move})
 
     def accept_undo(self, move: int):
         """Accept an undo request on the game
 
         Args:
             move (int): The move number to accept the undo at.
         """
         print(f"Accepting undo on game {self.game_id}")
-        self.socket.emit(event="game/undo/accept", data={'auth': self.auth_data['chat_auth'], 'game_id': self.game_id, 'move_number': move})
+        self.socket.emit(event="game/undo/accept", data={'auth': self.credentials.chat_auth, 'game_id': self.game_id, 'move_number': move})
 
     def pass_turn(self):
         """Pass the turn in the game"""
         print(f'Submitting move pass to game {self.game_id}')
-        self.socket.emit(event="game/move", data={'auth': self.auth_data['chat_auth'], 'player_id': self.user_data['id'], 'game_id': self.game_id, 'move': '..'})
+        self.socket.emit(event="game/move", data={'auth': self.credentials.chat_auth, 'player_id': self.credentials.user_id, 'game_id': self.game_id, 'move': '..'})
     
-    def send_chat(self, message: str, type: str, move: int):
+    def send_chat(self, message: str, chat_type: str, move: int):
         """Send a chat message to the game
         
         Args:
             message (str): The message to send to the game.
             type (str): The type of message to send. Accepts 'main', 'malkovich', 'hidden', or 'personal'
             move (int): The move number to send the message at.
             
         Examples:
             >>> game.send_chat('Hello World', 'game')
         """
         print(f'Sending chat message to game {self.game_id}')
-        self.socket.emit(event="game/chat", data={'auth': self.auth_data['chat_auth'], 'game_id': self.game_id, 'body': message, 'type': type, 'move_number': move})
+        self.socket.emit(event="game/chat", data={'auth': self.credentials.chat_auth, 'game_id': self.game_id, 'body': message, 'type': chat_type, 'move_number': move})
 
     # Pass game attributes as a dict
     def asdict(self):
         """Return the game as a dict
         
         Returns:
             data (dict): The game as a dict
```

### Comparing `ogsapi-0.7.2/src/ogsapi/ogssocket.py` & `ogsapi-0.7.3/src/ogsapi/ogssocket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,85 @@
-import socketio
-import requests
 from typing import Callable
-from .ogs_api_exception import OGSApiException
 from time import sleep, time
+import socketio
+from .ogs_api_exception import OGSApiException
+from .ogscredentials import OGSCredentials
 from .ogsgame import OGSGame
 
 class OGSSocket:
     """OGS Socket Class for handling SocketIO connections to OGS
     
     Args:
         bearer_token (str): The bearer token to use for authentication
         debug (bool, optional): Enable debug logging. Defaults to False.
     
     Attributes:
         clock_drift (float): The clock drift of the socket
         clock_latency (float): The clock latency of the socket
         last_ping (int): The last ping time of the socket
         last_issued_ping (int): The last time a ping was issued
-        games (dict): A dict of connected game objects
+        games (dict[OGSGame]): A dict of connected game objects
         bearer_token (str): The bearer token used for authentication
         client_callbacks (dict): A dict of socket level callbacks
         auth_data (dict): The auth data returned from the OGS API
         user_data (dict): The user data returned from the OGS API
         socket (socketio.Client): The socketio client object
         
     """
 
-    def __init__(self, bearer_token: str, debug: bool = False):
+    def __init__(self, credentials: OGSCredentials, debug: bool = False):
         # Clock Settings
         self.clock_drift = 0.0
         self.clock_latency = 0.0
         self.last_ping = 0
         self.last_issued_ping = 0
         # Dict of connected game objects
         self.games = {}
-        self.bearer_token = bearer_token
         # Socket level callbacks
         self.client_callbacks = {
             'notification': None,
             'error': None,
         }
+        self.credentials = credentials
         self.socket = socketio.Client(logger=debug, engineio_logger=False)
-        try:
-            self.auth_data = requests.get('https://online-go.com/api/v1/ui/config', headers={'Authorization': f'Bearer {bearer_token}'}).json()
-        except requests.exceptions.RequestException as e:
-            raise OGSApiException("Failed to get auth_data") from e
-        
-        # Grab user data as its own variable for ease of use
-        self.user_data = self.auth_data['user']
 
     def __del__(self):
         self.disconnect()
 
     def connect(self):
         """Connect to the socket"""
         self.socket_callbacks()
         print("Connecting to Websocket")
         try:
-            self.socket.connect('https://online-go.com/socket.io/?EIO=4', transports='websocket', headers={"Authorization" : f"Bearer {self.bearer_token}"})
-        except:
-            raise OGSApiException("Failed to connect to OGS Websocket")
+            self.socket.connect('https://online-go.com/socket.io/?EIO=4', transports='websocket', headers={"Authorization" : f"Bearer {self.credentials.access_token}"})
+        except Exception as e:
+            raise OGSApiException("Failed to connect to OGS Websocket") from e
 
     def register_callback(self, event: str, callback: Callable):
         """Register a callback function for receiving data from the API.
         
         Args:
             event (str): Event to register the callback function for.
                 Accepted events are:
                     - notification
                     - chat
                     - error
             callback (Callable): Callback function to register.   
         """
-        self.client_callbacks[event] = callback
+        self.client_callbacks[event]: OGSGame = callback
 
     # Listens to events received from the socket via the decorators, and calls the appropriate function
     def socket_callbacks(self):
         """Set the callback functions for the socket"""
 
         @self.socket.on('connect')
         def authenticate():
             """Authenticate to the socket"""
             print("Connected to socket, authenticating")
-            self.socket.emit(event="authenticate", data={"auth": self.auth_data['chat_auth'], "player_id": self.user_data['id'], "username": self.user_data['username'], "jwt": self.auth_data['user_jwt']})
+            self.socket.emit(event="authenticate", data={"auth": self.credentials.chat_auth, "player_id": self.credentials.user_id, "username": self.credentials.username, "jwt": self.credentials.user_jwt})
             sleep(1)
         
         @self.socket.on('hostinfo')
         def on_hostinfo(data):
             """Called when hostinfo is received on the socket"""
             print(f"Got: {data}")
         
@@ -133,31 +126,31 @@
     
     def ping(self):
         """Ping the socket"""
         self.socket.emit(event="net/ping", data={"client": int(time() * 1000), "drift": self.clock_drift, "latency": self.clock_latency})
     
     def notification_connect(self):
         """Connect to the notification socket"""
-        self.socket.emit(event="notification/connect", data={"auth": self.auth_data['notification_auth'], "player_id": self.user_data['id'], "username": self.user_data['username']})
+        self.socket.emit(event="notification/connect", data={"auth": self.credentials.notification_auth, "player_id": self.credentials.user_id, "username": self.credentials.username})
     
     def chat_connect(self):
         """Connect to the chat socket"""
-        self.socket.emit(event="chat/connect", data={"auth": self.auth_data['chat_auth'], "player_id": self.user_data['id'], "username": self.user_data['username']})
+        self.socket.emit(event="chat/connect", data={"auth": self.credentials.chat_auth, "player_id": self.credentials.user_id, "username": self.credentials.username})
 
     def game_connect(self, game_id: int):
         """Connect to a game
         
         Args:
             game_id (int): The id of the game to connect to
             
         Returns:
             OGSGame (OGSGame): The game object
         """
 
-        self.games[game_id] = OGSGame(game_socket=self.socket, game_id=game_id, auth_data=self.auth_data, user_data=self.user_data)
+        self.games[game_id] = OGSGame(game_socket=self.socket, game_id=game_id, credentials=self.credentials)
 
         return self.games[game_id]
 
     def game_disconnect(self, game_id: int):
         """Disconnect from a game
         
         Args:
```

### Comparing `ogsapi-0.7.2/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.7.3/src/ogsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.7.2
+Version: 0.7.3
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.7.2/src/tests/test.py` & `ogsapi-0.7.3/src/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,12 +17,12 @@
         try:
             from src.ogsapi.client import OGSClient
         except ImportError:
             self.fail("Failed to import OGSClient")
 
     def test_authentication(self):
         self.client = OGSClient(self.client_id, self.client_secret, self.username, self.password)
-        self.assertIsNotNone(self.client.access_token)
-        self.assertIsNotNone(self.client.refresh_token)
+        self.assertIsNotNone(self.client.credentials.access_token)
+        self.assertIsNotNone(self.client.credentials.refresh_token)
 
 if __name__ == '__main__':
     unittest.main()
```

