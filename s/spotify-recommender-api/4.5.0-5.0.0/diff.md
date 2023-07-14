# Comparing `tmp/spotify_recommender_api-4.5.0-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-5.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,22 @@
-Zip file size: 42685 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       21 b- defN 23-Jul-01 23:53 spotify_recommender_api/__init__.py
--rw-rw-r--  2.0 unx     1263 b- defN 23-Jul-01 13:50 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    15896 b- defN 23-Jul-01 23:53 spotify_recommender_api/core.py
--rw-rw-r--  2.0 unx     2042 b- defN 23-Jul-01 23:52 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx   121606 b- defN 23-Jul-02 00:01 spotify_recommender_api/recommender.py
--rw-rw-r--  2.0 unx     6217 b- defN 23-Jul-01 23:52 spotify_recommender_api/request_handler.py
--rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
--rw-rw-r--  2.0 unx     6722 b- defN 23-Jul-01 13:51 spotify_recommender_api/server.py
--rw-rw-r--  2.0 unx     9757 b- defN 23-Jul-01 23:53 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    22073 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/RECORD
-13 files, 187006 bytes uncompressed, 40653 bytes compressed:  78.3%
+Zip file size: 33791 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-14 18:41 spotify_recommender_api/__init__.py
+-rw-rw-r--  2.0 unx     2653 b- defN 23-Jul-14 18:41 spotify_recommender_api/error.py
+-rw-rw-r--  2.0 unx    29365 b- defN 23-Jul-14 18:41 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx     5610 b- defN 23-Jul-14 18:41 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx     1186 b- defN 23-Jul-14 18:41 spotify_recommender_api/visualization.py
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jul-14 18:41 spotify_recommender_api/artist/__init__.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-14 18:41 spotify_recommender_api/artist/artist.py
+-rw-rw-r--  2.0 unx       59 b- defN 23-Jul-14 18:41 spotify_recommender_api/server/__init__.py
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jul-14 13:02 spotify_recommender_api/server/sensitive.py
+-rw-rw-r--  2.0 unx     6629 b- defN 23-Jul-14 18:41 spotify_recommender_api/server/server.py
+-rw-rw-r--  2.0 unx       50 b- defN 23-Jul-14 18:41 spotify_recommender_api/song/__init__.py
+-rw-rw-r--  2.0 unx     2706 b- defN 23-Jul-14 18:41 spotify_recommender_api/song/song.py
+-rw-rw-r--  2.0 unx     1480 b- defN 23-Jul-14 18:41 spotify_recommender_api/song/util.py
+-rw-rw-r--  2.0 unx       50 b- defN 23-Jul-14 18:41 spotify_recommender_api/user/__init__.py
+-rw-rw-r--  2.0 unx    11265 b- defN 23-Jul-14 18:41 spotify_recommender_api/user/user.py
+-rw-rw-r--  2.0 unx    36708 b- defN 23-Jul-14 18:41 spotify_recommender_api/user/util.py
+-rw-rw-r--  2.0 unx    23528 b- defN 23-Jul-14 18:43 spotify_recommender_api-5.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-14 18:43 spotify_recommender_api-5.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-Jul-14 18:43 spotify_recommender_api-5.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1872 b- defN 23-Jul-14 18:43 spotify_recommender_api-5.0.0.dist-info/RECORD
+20 files, 124129 bytes uncompressed, 30651 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,40 +1,61 @@
 Filename: spotify_recommender_api/__init__.py
 Comment: 
 
-Filename: spotify_recommender_api/authentication.py
+Filename: spotify_recommender_api/error.py
 Comment: 
 
-Filename: spotify_recommender_api/core.py
+Filename: spotify_recommender_api/recommender.py
 Comment: 
 
-Filename: spotify_recommender_api/error.py
+Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api/recommender.py
+Filename: spotify_recommender_api/visualization.py
 Comment: 
 
-Filename: spotify_recommender_api/request_handler.py
+Filename: spotify_recommender_api/artist/__init__.py
 Comment: 
 
-Filename: spotify_recommender_api/sensitive.py
+Filename: spotify_recommender_api/artist/artist.py
 Comment: 
 
-Filename: spotify_recommender_api/server.py
+Filename: spotify_recommender_api/server/__init__.py
 Comment: 
 
-Filename: spotify_recommender_api/util.py
+Filename: spotify_recommender_api/server/sensitive.py
+Comment: 
+
+Filename: spotify_recommender_api/server/server.py
+Comment: 
+
+Filename: spotify_recommender_api/song/__init__.py
+Comment: 
+
+Filename: spotify_recommender_api/song/song.py
+Comment: 
+
+Filename: spotify_recommender_api/song/util.py
+Comment: 
+
+Filename: spotify_recommender_api/user/__init__.py
+Comment: 
+
+Filename: spotify_recommender_api/user/user.py
+Comment: 
+
+Filename: spotify_recommender_api/user/util.py
 Comment: 
 
-Filename: spotify_recommender_api-4.5.0.dist-info/METADATA
+Filename: spotify_recommender_api-5.0.0.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-4.5.0.dist-info/WHEEL
+Filename: spotify_recommender_api-5.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-4.5.0.dist-info/top_level.txt
+Filename: spotify_recommender_api-5.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-4.5.0.dist-info/RECORD
+Filename: spotify_recommender_api-5.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1,3 @@
-__version__ = '4.5.0'
+from spotify_recommender_api.recommender import start_api
+
+__version__ = '5.0.0'
```

## spotify_recommender_api/error.py

```diff
@@ -21,15 +21,17 @@
             if message is None:
                 message = 'There was an error regarding an HTTP Request'
 
             message += f', on the execution of the {func_name}({arguments}) function'
 
         err_code = f': {err_code}' if err_code else ''
 
-        super().__init__(f'{message}{err_code}')
+        self.message = f'{message}{err_code}'
+
+        super().__init__(self.message)
 
 class TooManyRequestsError(HTTPRequestError):
     """Generic exception for HTTP Request Exceptions
         It can receive the function name and the function arguments, besides the message, to better help debugging the error
     """
     def __init__(self, func_name=None, message=None, *args, **kwargs):
         super().__init__(*args, err_code='429 Too Many Requests', func_name=func_name, message=message, **kwargs)
@@ -43,7 +45,24 @@
     kwargs: 'dict[str, Any]'
 
     def __init__(self, func_name: Union[str, None] = None, func: Union[Callable, None] = None, message: Union[str, None] = None, *args, **kwargs):
         super().__init__(*args, err_code='401 Access Token Expired', func_name=func_name, message=message, **kwargs)
         self.func = func
         self.args = args
         self.kwargs = kwargs
+
+    def __str__(self) -> str:
+        return 'Access Token is not valid'
+
+class EmptyResultError(Exception):
+    """Exception raised when the result from an operation is empty, such as a dataframe when the filter of a specific artist is applied
+
+    """
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+
+class NoPlaylistProvidedError(Exception):
+    """Exception raised when trying to access a playlist action without have provided a playlist beforehand
+
+    """
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
```

## spotify_recommender_api/recommender.py

```diff
@@ -1,1519 +1,390 @@
-import os
-import re
 import logging
-import operator
 import warnings
 import pandas as pd
 import spotify_recommender_api.util as util
-import spotify_recommender_api.core as core
-import spotify_recommender_api.authentication as auth
-import spotify_recommender_api.request_handler as requests
-
-from functools import reduce
-from typing import Any, Union
-from spotify_recommender_api.error import AccessTokenExpiredError
+
+from typing import Union, Any, Callable
+from spotify_recommender_api.user import User
+from spotify_recommender_api.playlist.playlist import Playlist
+from spotify_recommender_api.error import NoPlaylistProvidedError
+from spotify_recommender_api.playlist.liked_songs import LikedSongs
+from spotify_recommender_api.requests.request_handler import RequestHandler
 
 warnings.filterwarnings('error')
 
 
 class SpotifyAPI:
-    """
-    Spotify API is the Class that provides access to the playlists recommendations
-    """
-
-    def __get_playlist_from_csv(self):
-        """
-        Function that creates the playlist variable from a CSV file previously created by this same package
-
-        """
-
-        try:
-            df = pd.read_parquet(f'./.spotify-recommender-util/{self.__base_playlist_name}.parquet')
-        except FileNotFoundError as e:
-            try:
-                df = pd.read_parquet('./.spotify-recommender-util/util.parquet')
-                logging.warning(f'The playlist {self.__base_playlist_name} does not exist in the CSV format, but ever since the version 3.5.0 the csv file and the util file created, have the same name as the playlist, but there is only a generic file on your machine.')
-                response = input('Therefore, do you want to rename the generic files to the new format, and therefore having the playlist name (y/n)? ')
-                while response not in ['y', 'n']:
-                    response = input('Select a valid option.\n Do you want to rename the generic files to the new format, and therefore having the playlist name (y/n)? ')
-
-                if response == 'n':
-                    raise FileNotFoundError(
-                        'The playlist with the specified ID does not exist in the CSV format, try again but selecting the "web" option, as the source for the playlist') from e
-
-                else:
-                    self.__update_created_files = True
-
-            except FileNotFoundError as exc:
-                raise FileNotFoundError(
-                    'The playlist with the specified ID does not exist in the CSV format, try again but selecting the "web" option, as the source for the playlist') from exc
+    """Spotify API is the Class that provides access to the playlists recommendations"""
 
-        self.__artists, self.__songs, self.__all_genres = [eval(arr) if isinstance(arr, str) else arr for arr in [df['artists'][0], df['songs'][0], df['all_genres'][0]]]
-
-        if self.__update_created_files:
-            self.__playlist = pd.read_csv('playlist.csv')
-        else:
-            self.__playlist = pd.read_csv(f'{self.__base_playlist_name}.csv')
-
-    def __get_playlist(self):
-        """
-        General purpose function to get the playlist, either from CSV or web requests
+    def __init__(self, user_id: str, playlist_id: Union[str, None] = None, playlist_url: Union[str, None] = None, liked_songs: bool = False):
+        """Spotify API is the Class that provides access to the playlists recommendations
 
-        """
-        answer = input('Do you want to get the playlist data via CSV saved previously or read from spotify, *which will take a few minutes* depending on the playlist size (csv/web)? ')
-        while answer.lower() not in ['csv', 'web']:  # , 'parquet'
-            answer = input("Please select a valid response: ")
-
-        self.__update_created_files = False
-        if answer.lower() == 'csv':
-            self.__get_playlist_from_csv()
-            return False
+        Note:
+            It will trigger most of the API functions and can take a good while to complete if the playlist is specified, and the "web" option selected to retrieve the playlist items
 
-        return True
-
-    def __get_song_genres(self, song: 'dict[str, Any]') -> 'list[str]':
-        """
-        Function that gets all the genres for a given song
 
         Args:
-          song(dict[str, Any]): the song dictionary
-
-        Returns:
-          list[str]: list of genres for a given song
-        """
-        genres = []
-        song_artists = song["track"]["artists"] if 'track' in list(song.keys()) else song["artists"]
-        for artist in song_artists:
-            artist_id = artist["id"]
-            if artist_id not in self.__artists:
-                artist_genres_res = requests.get_request(url=f'https://api.spotify.com/v1/artists/{artist_id}', headers=self.__headers)
-                try:
-                    artist_genres = artist_genres_res.json()["genres"]
-                    genres += artist_genres
-                    self.__artists[artist["name"]] = artist_genres
-                except Exception as e:
-                    logging.error(f'{e = }')
-                    logging.debug(artist_genres_res.json())
-            else:
-                genres += self.__artists[artist_id]
-
-        return list(set(genres))
+            user_id (str): The user ID, visible in the Spotify profile account settings
+            playlist_id (str, optional): The playlist ID hash in Spotify. Defaults to None.
+            playlist_url (str, optional): The url used while sharing the playlist. Defaults to None.
+            liked_songs (bool, optional): Whether to use the User's Liked Songs as the base playlist, Defaults to False.
 
-    def __get_playlist_items(self):
         """
-        Function that gets the items (songs) inside the playlist
 
-        # Note
-        Ran automatically but can last as long as 2.5 seconds for each song (can be worse depending on the network connection) inside of the playlist, not because it is compute demanding but because it needs to do a up to a handful of http requests per song, which can take a while
+        self.user = User(user_id=user_id)
 
-        """
-        self.__all_genres = []
-        try:
-            total_song_count = util.get_total_song_count(playlist_id=self.__playlist_id, headers=self.__headers)
-            for offset in range(0, total_song_count, 100):
-                logging.info(f'Songs mapped: {offset}/{total_song_count}')
-                all_genres_res = requests.get_request(
-                    headers=self.__headers,
-                    url=f'https://api.spotify.com/v1/playlists/{self.__playlist_id}/tracks?limit=100&{offset=!s}'
-                )
-                for song in all_genres_res.json()["items"]:
-                    (id, name, popularity, artist, added_at), song_genres = util.song_data(song=song), self.__get_song_genres(song)
-                    song['id'] = id
-                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
-                    self.__songs.append({
-                        "id": id,
-                        "name": name,
-                        "artists": artist,
-                        "popularity": popularity,
-                        "genres": song_genres,
-                        "added_at": added_at,
-                        "danceability": danceability,
-                        "loudness": loudness,
-                        "energy": energy,
-                        "instrumentalness": instrumentalness,
-                        "tempo": tempo,
-                        "valence": valence
-                    })
-                    self.__all_genres += song_genres
-
-        except KeyError as e:
-            raise ValueError(
-                'Invalid Auth Token, try again with a valid one') from e
+        if liked_songs or playlist_id is not None or playlist_url is not None:
+            self.select_playlist(
+                liked_songs=liked_songs,
+                playlist_id=playlist_id,
+                playlist_url=playlist_url
+            )
 
         else:
-            self.__all_genres = list(set(self.__all_genres))
-
-    def __get_liked_songs(self):
-        """
-        Function that gets the items (songs) inside the user's liked songs
-
-        # Note
-        Ran automatically but can last as long as 2.5 seconds for each song (can be worse depending on the network connection) inside of the playlist, not because it is compute demanding but because it needs to do a up to a handful of http requests per song, which can take a while
-
-        """
-        self.__all_genres = []
-        for _ in range(2):
-            try:
-                total_song_count = requests.get_request(headers=self.__headers, url='https://api.spotify.com/v1/me/tracks').json()['total']
-
-                for offset in range(0, total_song_count, 50):
-                    logging.info(f'Songs mapped: {offset}/{total_song_count}')
-                    all_genres_res = requests.get_request(
-                        headers=self.__headers,
-                        url=f'https://api.spotify.com/v1/me/tracks?limit=50&{offset=!s}'
-                    )
-                    for song in all_genres_res.json()["items"]:
-                        (id, name, popularity, artist, added_at), song_genres = util.song_data(
-                            song=song), self.__get_song_genres(song)
-                        song['id'] = id
-                        danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                            song=song, headers=self.__headers)
-                        self.__songs.append({
-                            "id": id,
-                            "name": name,
-                            "artists": artist,
-                            "popularity": popularity,
-                            "genres": song_genres,
-                            "added_at": added_at,
-                            "danceability": danceability,
-                            "loudness": loudness,
-                            "energy": energy,
-                            "instrumentalness": instrumentalness,
-                            "tempo": tempo,
-                            "valence": valence
-                        })
-                        self.__all_genres += song_genres
-
-                logging.info(f'Songs mapping complete: {total_song_count}/{total_song_count}')
-
-                self.__all_genres: 'list[str]' = list(set(self.__all_genres))
-
-            except AccessTokenExpiredError as e:
-                logging.warning('Error due to the access token expiration')
-                auth_token = auth.get_auth()
-
-                self.__auth_token = auth_token
-
-                self.__headers['Authorization'] = f'Bearer {auth_token}'
-            else:
-                break
+            logging.info('Class initiated without any playlist. To access any playlist-related functions please use the select_playlist method.\nAll Profile related functions can still be used in any way you prefer')
 
-    def __playlist_adjustments(self):
-        """
-        Function that does a bunch of adjustments to the overall formatting of the playlist, before making it visible
+        logging.info('After version 5.0.0 there has been a full refactoring of the package, so any problems that you may encounter, submit an issue at: https://github.com/nikolas-virionis/spotify-api/issues')
 
-        """
-        try:
-            songs = self.__songs[-util.get_total_song_count(playlist_id=self.__playlist_id, headers=self.__headers):]
-        except KeyError as e:
-            raise AccessTokenExpiredError('Invalid Auth Token, try again with a valid one') from e
-
-        self.__all_artists = list(self.__artists.keys())
-        playlist = pd.DataFrame(data=list(songs))
-
-        playlist["genres_indexed"] = [
-            util.item_list_indexed(
-                all_items=self.__all_genres,
-                items=eval(genre) if isinstance(genre, str) else genre,
-            ) for genre in playlist["genres"]
-        ]
-        playlist["artists_indexed"] = [
-            util.item_list_indexed(
-                all_items=self.__all_artists,
-                items=eval(artist) if isinstance(artist, str) else artist,
-            ) for artist in playlist["artists"]
-        ]
-        playlist['id'] = playlist["id"].astype(str)
-        playlist['name'] = playlist["name"].astype(str)
-        playlist['popularity'] = playlist["popularity"].astype(int)
-        playlist['added_at'] = pd.to_datetime(playlist["added_at"])
-        playlist['danceability'] = playlist["danceability"].astype(float)
-        playlist['energy'] = playlist["energy"].astype(float)
-        playlist['instrumentalness'] = playlist["instrumentalness"].astype(float)
-        playlist['tempo'] = playlist["tempo"].astype(float)
-        playlist['valence'] = playlist["valence"].astype(float)
-        if 'loudness' not in playlist.columns:
-            playlist['loudness'] = 0
-            logging.warning('Since version 4.3.0, there is a new column "loudness" and in order to get it you will need to get the playlist from web and not csv, after that everything will work just as before')
+    def needs_playlist(func: Callable[..., Any]) -> Callable[..., Any]: # type: ignore
+        """Decorator to check if a playlist is provided before accessing a function.
 
-        playlist['loudness'] = playlist["loudness"].astype(float)
-        self.__playlist = playlist
+        Args:
+            func (Callable[..., Any]): The function to be decorated.
 
-    def playlist_to_csv(self):
-        """
-        Function to convert playlist to CSV format
-        Really useful if the package is being used in a .py file since it is not worth it to use it directly through web requests everytime even more when the playlist has not changed since last package usage
+        Returns:
+            Callable[..., Any]: The decorated function.
         """
-        if not os.path.exists('./.spotify-recommender-util'):
-            os.mkdir('./.spotify-recommender-util')
+        def wrapper(self, *args, **kwargs):
+            if getattr(self, 'playlist', None) is None:
+                raise NoPlaylistProvidedError('To access this function, you need to provide a playlist via the select_playlist method')
 
-        df = pd.DataFrame(
-            columns=['artists', 'songs', 'all_genres'],
-            data=[
-                {
-                    'songs': self.__songs,
-                    'artists': self.__artists,
-                    'all_genres': self.__all_genres
-                }
-            ],
-        )
+            return func(self, *args, **kwargs) # type: ignore
 
-        df.to_parquet(
-            f'./.spotify-recommender-util/{self.__base_playlist_name}.parquet')
-
-        playlist = self.__playlist[
-            [
-                'id',
-                'name',
-                'artists',
-                'genres',
-                'popularity',
-                'added_at',
-                'danceability',
-                'loudness',
-                'energy',
-                'instrumentalness',
-                'tempo',
-                'valence'
-            ]
-        ]
-
-        playlist.to_csv(f'{self.__base_playlist_name}.csv')
+        return wrapper
 
     def select_playlist(
             self,
-            user_id: str,
+            liked_songs: bool = False,
             playlist_id: Union[str, None] = None,
             playlist_url: Union[str, None] = None,
-            liked_songs: bool = False,
-            prepare_favorites: bool = False
         ) -> None:
         """Function to select a playlist to be mapped and be available on all the playlist related recommendation functions
 
         Args:
-            user_id (str): Spotify User ID
             playlist_id (str, optional): Playlist ID. Defaults to None.
             playlist_url (str, optional): Playlist Share URL (contains the ID, and it's easier to get). Defaults to None.
             liked_songs (bool, optional): Flag to use the user 'Liked songs' as the playlist. Defaults to False.
-            prepare_favorites (bool, optional): Flag to prepare the deprecated functions for mid-term and short term favorites. Defaults to False.
 
         """
-        self.__artists = {}
-        self.__songs = []
-        self.__deny_favorites = False
         if liked_songs:
-            self.__playlist_id = 'liked_songs'
-
-            self.__base_playlist_name = f'{user_id} Liked Songs'
-
-        else:
-            if playlist_id:
-                self.__playlist_id = playlist_id
-            else:
-                if not playlist_url:
-                    raise ValueError(
-                        'Either the playlist url or its id must be specified')
-                self.__playlist_id = util.playlist_url_to_id(url=playlist_url)
-                self.__playlist_url = playlist_url
+            self.playlist = LikedSongs(user_id=self.user.user_id)
 
-            for _ in range(2):
-                try:
-                    self.__base_playlist_name = util.get_base_playlist_name(
-                        headers=self.__headers,
-                        playlist_id=self.__playlist_id,
-                    )
-                except AccessTokenExpiredError as e:
-                    logging.warning('Error due to the access token expiration')
-                    auth_token = auth.get_auth()
+        elif playlist_id is not None:
+            self.playlist = Playlist(user_id=self.user.user_id, playlist_id=playlist_id)
 
-                    self.__auth_token = auth_token
+        elif playlist_url is not None:
+            playlist_id = util.playlist_url_to_id(url=playlist_url)
 
-                    self.__headers['Authorization'] = f'Bearer {auth_token}'
-                else:
-                    break
-
-
-        logging.info('Mapping playlist items')
-
-        if self.__get_playlist():
-            if liked_songs:
-                self.__get_liked_songs()
-            else:
-                self.__get_playlist_items()
-
-        logging.info('Setting up some operations with the playlist')
-
-        self.__playlist_adjustments()
-
-        self.__song_dict = core.knn_prepared_data(playlist=self.__playlist)
-        if prepare_favorites:
-            self.__prepare_favorites_playlist()
-
-        if self.__update_created_files:
-            self.playlist_to_csv()
-
-        self.__top_genres = self.__top_artists = self.__top_tracks = None
-
-
-
-    def __init__(self, auth_token: str, user_id: str, playlist_id: Union[str, None] = None, playlist_url: Union[str, None] = None, liked_songs: bool = False, prepare_favorites: bool = False):
-        """Spotify API is the Class that provides access to the playlists recommendations
-
-        Note:
-            It will trigger most of the API functions and can take a good while to complete
+            self.playlist = Playlist(user_id=self.user.user_id, playlist_id=playlist_id)
 
+    def get_most_listened(self, time_range: str = 'long_term', number_of_songs: int = 50, build_playlist: bool = False) -> pd.DataFrame:
+        """Function that creates the most-listened songs playlist for a given period of time in the users profile
 
         Args:
-            auth_token (str): The authentication token for the Spotify API, base64 encoded string that allows the use of the API's functionalities
-            user_id (str): The user ID, visible in the Spotify profile account settings
-            playlist_id (str, optional): The playlist ID hash in Spotify. Defaults to None.
-            playlist_url (str, optional): The url used while sharing the playlist. Defaults to None.
+            time_range (str, optional): time range ('long_term', 'medium_term', 'short_term'). Defaults to 'long'.
+            number_of_songs (int, optional): Number of the most listened songs to return. Defaults to 50.
+            build_playlist (bool, optional): Whether to create, or update, a playlist in the user's library. Defaults to False.
 
         Raises:
-            ValueError: auth_token is required
-            ValueError: Either the playlist url or its id must be specified
-        """
-        if not auth_token:
-            raise ValueError('auth_token is required')
-        self.__user_id = user_id
-        self.__auth_token = auth_token
-        self.__headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/json",
-            "Authorization": self.__auth_token
-        }
-
-        self.select_playlist(
-            user_id=user_id,
-            liked_songs=liked_songs,
-            playlist_id=playlist_id,
-            playlist_url=playlist_url,
-            prepare_favorites=prepare_favorites
-        )
+            ValueError: time range does not correspond to a valid time range ('long_term', 'medium_term', 'short_term')
+            ValueError: Value for number_of_songs must be between 1 and 1500
 
-    def __get_neighbors(self, song: int, K: int, song_dict: list, type: Union[str, None] = None) -> list:
-        """Function thats using the distance calculated above, returns the K nearest neighbors for a given song
-
-        Args:
-            song (str): song's index in the songs list
-            K (int): desired number K of neighbors to be returned
-            song_dict (list): the list of songs
-            type (str, optional): Neighbor playlist type. Defaults to None.
 
         Returns:
-            list: list neighbors
+            pd.DataFrame: pandas DataFrame containing the top number_of_songs songs in the time range
         """
-        if type is None:
-            return []
+        if time_range not in ['long_term', 'medium_term', 'short_term']:
+            raise ValueError('time_range must be long_term, medium_term or short_term')
 
-        distances = []
+        if not (1 <= number_of_songs <= 1500):
+            raise ValueError(f'Value for number_of_songs must be between 1 and 1500: {time_range} term most listened')
 
-        for song_index, song_value in enumerate(song_dict):
-            if song_index != song:
-                dist = core.compute_distance(song_a=song_dict[song], song_b=song_value, artist_recommendation='artist' in type)
-                distances.append((song_index, dist))
-
-        distances.sort(key=operator.itemgetter(1))
-        return [[*distances[x]] for x in range(K)]
+        return self.user.get_most_listened(
+            time_range=time_range,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+        )
 
-    def __get_index_for_song(self, song: Union[str, 'list[str]', None]) -> int:
-        """Function that returns the index of a given song in the list of songs
+    def get_profile_recommendation(
+            self,
+            number_of_songs: int = 50,
+            main_criteria: str = 'mixed',
+            save_with_date: bool = False,
+            build_playlist: bool = False,
+            time_range: str = 'short_term'
+        ) -> pd.DataFrame:
+        """Builds a Profile based recommendation
 
         Args:
-            song (str): song name
+            number_of_songs (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
+            main_criteria (str, optional): Main criteria for the recommendations playlist. Can be one of the following: 'mixed', 'artists', 'tracks', 'genres'. Defaults to 'mixed'.
+            save_with_date (bool, optional): Flag to save the recommendations playlist as a Point in Time Snapshot. Defaults to False.
+            build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
+            time_range (str, optional): The time range to get the profile most listened information from. Can be one of the following: 'short_term', 'medium_term', 'long_term'. Defaults to 'short_term'
 
         Raises:
-            ValueError: Playlist does not contain the song
+            ValueError: If number_of_songs is not between 1 and 100.
+            ValueError: If main_criteria is not one of 'mixed', 'artists', 'tracks', 'genres'.
+            ValueError: If time_range is not one of 'short_term', 'medium_term', 'long_term'.
 
         Returns:
-            int: the index for the song
+            pd.DataFrame: Recommendations playlist
         """
-        if song not in self.__playlist['name'].tolist():
-            raise ValueError(f'Playlist does not contain the song {song!r}')
-
-        item = self.__playlist.index[self.__playlist['name'] == song].tolist()
-
-        return item[0]
 
+        return self.user.get_profile_recommendation(
+            time_range=time_range,
+            main_criteria=main_criteria,
+            save_with_date=save_with_date,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+        )
 
-    def __push_songs_to_playlist(self, full_uris: str, playlist_id: Union[str, bool, None]):
-        """Function to push soongs to a specified playlist
+    def get_general_recommendation(
+        self,
+        number_of_songs: int = 50,
+        build_playlist: bool = False,
+        genres_info: Union['list[str]', None] = None,
+        artists_info: Union['list[str]', None] = None,
+        use_main_playlist_audio_features: bool = False,
+        tracks_info: 'Union[list[str], list[tuple[str, str]], list[list[str]], dict[str, str], None]' = None,
+    ) -> pd.DataFrame:
+        """Builds a general recommendation based on up to 5 items spread across artists, genres, and tracks.
 
         Args:
-            full_uris (str): list of song uri's
-            playlist_id (str): playlist id
-        """
-        full_uris_list = full_uris.split(',')
-
-        if len(full_uris_list) <= 100:
-            uris = ','.join(full_uris_list)
-            add_songs_req = requests.post_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}/tracks?{uris=!s}', headers=self.__headers)
-
-        else:
-
-            for offset in range(0, len(full_uris_list), 100):
-
-                uris = ','.join(full_uris_list[offset:offset + min(len(full_uris_list) - offset, 100)])
-                add_songs_req = requests.post_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}/tracks?{uris=!s}', headers=self.__headers)
-
+            number_of_songs (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
+            genres_info (list[str], optional): list of the genre names to be used in the recommendation. Defaults to [].
+            artists_info (list[str], optional): list of the artist names to be used in the recommendation. Defaults to [].
+            build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
+            use_main_playlist_audio_features (bool, optional): Flag to use the audio features of the main playlist to target better recommendations. Defaults to False.
+            tracks_info (list[str] | list[tuple[str]] | list[list[str]] | dict[str, str]], optional): List of the song names to be used in the recommendations. They can be only the song names, but since there are a lot of songs with the same name i recommend using also the artist name in a key-value format using either a tuple, or list, or dict. Examples below. Defaults to [].
 
-    def __build_playlist(self, type: str, uris: str):
-        """Function that builds the contents of a playlist
+        Raises:
+            ValueError: number_of_songs must be between 1 and 100
+            ValueError: At least one of the three args must be provided: genres_info, artists_info, tracks_info
+            ValueError: The sum of the number of items in each of the three args mustn't exceed 5
+            ValueError: The argument tracks_info must be an instance of one of the following 4 types: list[str], list[tuple[str]], list[list[str]], dict[str, str]
 
-        Note:
-            This function will change the user's library by filling the previously created empty playlist
+        Returns:
+            pd.DataFrame: Recommendations playlist
 
-        Args:
-            type (str): the type of the playlist being created
-            uris (str): string containing all song uris in the format the Spotify API expects
+        ## Examples of tracks_info
+        >>> api.get_general_recommendation(tracks_info={'song': 'artist', 'song': 'artist'})
+        # or
+        >>> api.get_general_recommendation(tracks_info=[('song', 'artist'), ('song', 'artist')])
+        # or
+        >>> api.get_general_recommendation(tracks_info=[['song', 'artist'], ['song', 'artist']])
+        # or, but not recommended
+        >>> api.get_general_recommendation(tracks_info=['song', 'song'])
         """
-        if not uris:
-            raise ValueError('Invalid value for the song uris')
+        if use_main_playlist_audio_features:
+            audio_statistics = self.audio_features_statistics()
+        else:
+            audio_statistics = None
 
-        additional_information_by_type = {
-            'song': getattr(self, '_SpotifyAPI__song_name', None),
-            'artist': getattr(self, '_SpotifyAPI__artist_name', None),
-            'mood': [
-                getattr(self, '_SpotifyAPI__mood', None),
-                getattr(self, '_SpotifyAPI__exclude_mostly_instrumental', None),
-            ],
-            'profile-recommendation': [
-                getattr(self, '_SpotifyAPI__profile_recommendation_criteria', None),
-                getattr(self, '_SpotifyAPI__profile_recommendation_date', None),
-                getattr(self, '_SpotifyAPI__profile_recommendation_time_range', None)
-            ],
-            'playlist-recommendation': [
-                getattr(self, '_SpotifyAPI__playlist_recommendation_criteria', None),
-                getattr(self, '_SpotifyAPI__playlist_recommendation_date', None),
-                getattr(self, '_SpotifyAPI__playlist_recommendation_time_range', None)
-            ],
-            'general-recommendation': [
-                getattr(self, '_SpotifyAPI__general_recommendation_description', None),
-                getattr(self, '_SpotifyAPI__general_recommendation_description_types', None)
-            ],
-            'most-listened-recommendation': getattr(self, '_SpotifyAPI__most_listened_recommendation_time_range', None),
-        }
-
-
-        playlist_id = core.create_playlist(
-            type=type,
-            headers=self.__headers,
-            user_id=self.__user_id,
-            base_playlist_name=self.__base_playlist_name,
-            _update_created_playlists=self.__update_created_files,
-            additional_info=additional_information_by_type['artist'] if "artist" in type else additional_information_by_type.get(type)
+        return self.user.get_general_recommendation(
+            genres_info=genres_info,
+            tracks_info=tracks_info,
+            artists_info=artists_info,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+            audio_statistics=audio_statistics,
         )
 
-        self.__push_songs_to_playlist(full_uris=uris, playlist_id=playlist_id)
-
-    def __write_playlist(self, type: str, K: int, additional_info: Union[str, 'list[str]', None] = None):
-        """Function that writes a new playlist with the recommendations for the given type
-        type: the type of the playlist being created ('song', 'short', 'medium'):
-         - 'song': a playlist related to a song
-         - 'short': a playlist related to the short term favorites for that given user
-         - 'medium': a playlist related to the medium term favorites for that given user
-
-        Note:
-            This function will change the user's library by either creating a new plalylist or overriding the existing one
-
-        Args:
-            type (str): the type of the playlist being created
-            K (int): desired number K of neighbors to be returned
-            additional_info (Any, optional): the song name when the type is 'song'. Defaults to None.
-
-        Raises:
-            ValueError: Value for K must be between 1 and 1500
-            ValueError: Invalid type
+    @needs_playlist
+    def playlist_to_csv(self):
+        """
+        Function to convert playlist to CSV format. \n
+        Really useful if the package is being used in a .py file since it is not worth it to use it directly through web requests everytime even more when the playlist has not changed since last package usage, making it possible to store it for easier and quicker access
         """
-        if K > 1500:
-            logging.warning('K limit exceded. Maximum value for K is 1500')
-            K = 1500
-        elif K < 1:
-            raise ValueError(f'Value for K must be between 1 and 1500 on creation of {type} playlist. {additional_info=!r}')
-
-        if type == 'song':
-            index = self.__get_index_for_song(additional_info)
-            uris = f'spotify:track:{self.__song_dict[index]["id"]},'
-
-            uris += ','.join([f'spotify:track:{neighbor}' for neighbor in self.__get_recommendations('song', additional_info, K)['id']])
-
-        elif type in {'medium', 'short'}:
-            ids = self.__medium_fav['id'] if type == 'medium' else self.__short_fav['id']
-
-            uris = ','.join([f'spotify:track:{song}' for song in ids])
-
-        elif any(x in type for x in ['most-listened', 'artist', '-recommendation', 'mood']):
-            ids = additional_info
-            if ids is None: # only because of strict type checking enforncing that if it can be None it souldnt be part of an iteration
-                ids = []
-            uris = ','.join([f'spotify:track:{song}' for song in ids])
 
-        else:
-            uris = ''
-            raise ValueError('Invalid type')
+        playlist = self.get_playlist()
 
-        self.__build_playlist(type=type, uris=uris)
+        playlist.to_csv(f'{self.playlist.playlist_name}.csv')
 
+    @needs_playlist
     def get_recommendations_for_song(
         self,
-        K: int,
-        song: str,
-        generate_csv: bool = False,
+        song_name: str,
+        artist_name: str,
+        number_of_songs: int = 50,
         with_distance: bool = False,
         build_playlist: bool = False,
-        generate_parquet: bool = False,
         print_base_caracteristics: bool = False
-    ) -> Union[pd.DataFrame, None]:
+    ) -> pd.DataFrame:
         """Playlist which centralises the actions for a recommendation made for a given song
 
         Note
             The build_playlist option when set to True will change the user's library
 
 
         Args:
-            K (int): desired number K of neighbors to be returned
-            song (str): The desired song name
-            generate_csv (bool, optional): Whether to generate a CSV file containing the recommended playlist. Defaults to False.
+            song_name (str): The desired song name
+            artist_name (str): The desired song's artist name
+            number_of_songs (int): desired number number_of_songs of neighbors to be returned
             with_distance (bool, optional): Whether to allow the distance column to the DataFrame returned, which will have no actual value for most use cases, since  it does not obey any actual unit, it is just a mathematical value to determine the closet songs. Defaults to False.
             build_playlist (bool, optional): Whether to build the playlist to the user's library. Defaults to False.
-            generate_parquet (bool, optional): Whether to generate a parquet file containing the recommended playlist. Defaults to False.
             print_base_caracteristics (bool, optional): Whether to print the base / informed song information, in order to check why such predictions were made by the algorithm. Defaults to False.
 
         Raises:
-            ValueError: Value for K must be between 1 and 1500
+            ValueError: Value for number_of_songs must be between 1 and 1500
 
         Returns:
             pd.DataFrame: Pandas DataFrame containing the song recommendations
         """
-        try:
-            if not (1 < K <= 1500):
-                raise ValueError(
-                    f'Value for K must be between 1 and 1500 on creation of recommendation for the song {song}')
-
-            self.__song_name = song
-
-            df = self.__get_recommendations('song', song, K)
-            playlist_name = f'{song} Related'
-
-            if print_base_caracteristics:
-                index = self.__get_index_for_song(song)
-                caracteristics = self.__song_dict[index]
-                name, genres, artists, popularity, _, danceability, loudness, energy, instrumentalness, tempo, valence = list(caracteristics.values())[1:11]
-                util.print_base_caracteristics(name, genres, artists, popularity, danceability, loudness, energy, instrumentalness, tempo, valence)
-
-            if generate_csv:
-                df.to_csv(f'{playlist_name}.csv')
-
-            if generate_parquet:
-                df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
-
-            for _ in range(2):
-                try:
-
-                    if build_playlist:
-                        self.__write_playlist('song', K, additional_info=song)
-
-                except AccessTokenExpiredError as e:
-                    logging.warning('Error due to the access token expiration')
-                    auth_token = auth.get_auth()
-
-                    self.__auth_token = auth_token
-
-                    self.__headers['Authorization'] = f'Bearer {auth_token}'
-                else:
-                    break
-
-            return df if with_distance else df.drop(columns=['distance'])
-
-        except ValueError as e:
-            logging.error(e)
-
-    def __get_desired_dict_fields(self, index: int, song_dict: Union['list[dict[str, Any]]', None] = None) -> 'list[str]':
-        """Function that returns the usual fields for a given song
-
-        Args:
-            index (int): The index of the song inside the song list
-            song_dict (list, optional): song dictionary. Defaults to None.
-
-        Returns:
-            list[str]: list of fields of the desired song
-        """
-
-        if song_dict is None:
-            song_dict = self.__song_dict
-
-        desired_song_dict = song_dict[index]
-
-        return [
-            desired_song_dict['id'],
-            desired_song_dict['name'],
-            desired_song_dict['artists'],
-            desired_song_dict['genres'],
-            desired_song_dict['popularity'],
-            desired_song_dict['added_at'],
-            desired_song_dict['danceability'],
-            desired_song_dict['loudness'],
-            desired_song_dict['energy'],
-            desired_song_dict['instrumentalness'],
-            desired_song_dict['tempo'],
-            desired_song_dict['valence']
-        ]
-
-    def __song_list_to_df(self, neighbors: list, song_dict: Union['list[dict[str, Any]]', None] = None) -> pd.DataFrame:
-        """Function that returns DataFrame representation of the list of neighbor songs
-
-        Args:
-            neighbors (list): list of a given song's neighbors
-            song_dict (list, optional): song dictionary. Defaults to None.
-
-        Returns:
-            pd.DataFrame: Song DataFrame
-        """
-        data = [list(self.__get_desired_dict_fields(neighbor[0], song_dict=song_dict) + [neighbor[1]]) for neighbor in neighbors]
-
-        return pd.DataFrame(data=data, columns=['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence', 'distance'])
-
-    def __get_recommendations(self, type: str, info, K: int = 51) -> pd.DataFrame:
-        """General purpose function to get recommendations for any type supported by the package
-
-        Args:
-            info (Any): the changed song_dict list if the type is short or medium or else it is the name of the song to get recommendations from
-            K (int, optional): desired number K of neighbors to be returned. Defaults to 51.
-            type (str): the type of the playlist being created ('song', 'short', 'medium'), meaning:
-
-            --- 'song': a playlist related to a song
-
-            --- 'short': a playlist related to the short term favorites for that given user
-
-            --- 'medium': a playlist related to the medium term favorites for that given user
-
-            --- 'artist-related': a playlist related to a specific artist
-
-
-        Raises:
-            ValueError: Type does not correspond to a valid option
-
-        Returns:
-            pd.DataFrame: song DataFrame
-        """
-        index = 0
-        if type == 'song':
-            index = self.__get_index_for_song(info)
-        elif type in {'long', 'medium', 'short', 'artist-related'}:
-            index = len(info) - 1
-        else:
-            raise ValueError('Type does not correspond to a valid option')
-        song_dict = self.__song_dict if type == 'song' else info
-        neighbors = self.__get_neighbors(song=index, K=K, song_dict=song_dict, type=type)
-        return self.__song_list_to_df(neighbors, song_dict=song_dict)
-
-    def __get_genres(self, genres: 'list[list[str]]') -> 'list[str]':
-        """Function to unite all the genres from different songs into one list of genres
-
-        Args:
-            genres (list[list[str]]): the list of lists of genres from the different songs
-
-        Raises:
-            ValueError: Playlist chosen does not correspond to any of the users favorite songs
-
-        Returns:
-            list[str]: full list of genres
-        """
-        try:
-            all_genres = genres[0][:]
-        except IndexError as e:
-            self.__deny_favorites = True
-            raise ValueError(
-                'Playlist chosen does not correspond to any of the users favorite songs') from e
-
-        for index in range(1, len(genres)):
-            for i in range(len(all_genres)):
-                all_genres[i] = all_genres[i] or genres[index][i]
-
-        return all_genres
-
-    def __get_artists(self, artists: 'list[list[str]]') -> 'list[str]':
-        """Function to unite all the artists from different songs into one list of artists
-
-        Args:
-            artists (list[list[str]]): the list of lists of artists from the different songs
-
-        Raises:
-            ValueError: Playlist chosen does not correspond to any of the users favorite songs
-
-        Returns:
-            list[str]: full list of artists
-        """
-        try:
-            all_artists = artists[0][:]
-        except IndexError as e:
-            raise ValueError(
-                'Playlist chosen does not correspond to any of the users favorite songs') from e
-
-        for index in range(1, len(artists)):
-            for i in range(len(all_artists)):
-                all_artists[i] = all_artists[i] or artists[index][i]
-
-        return all_artists
-
-    def __get_top_5(self, time_range='medium') -> 'list[dict[str, Any]]':
-        """Function that gets and initially formats the top 5 songs in a given time_range
-
-        Args:
-            time_range (str, optional): The time range to get the top 5 songs from ('medium', 'short'). Defaults to 'medium'.
-
-        Raises:
-            ValueError: time_range must be either medium_term or short_term
-
-        Returns:
-            list[dict[str, Any]]: top 5 songs listened
-        """
-        if time_range not in ['medium', 'short']:
-            raise ValueError('time_range must be either medium_term or short_term')
-
-        top_5 = requests.get_request(url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit=5', headers=self.__headers).json()
-
-        return [
-            {
-                'name': song['name'],
-                'genres': self.__get_song_genres(song),
-                'artists': [artist['name'] for artist in song['artists']],
-                'popularity': song['popularity'],
-                'danceability': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['danceability'],
-                'loudness': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['loudness'],
-                'energy': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['energy'],
-                'instrumentalness': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['instrumentalness'],
-                'tempo': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['tempo'],
-                'valence': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['valence']
-            }
-            for song in top_5['items']
-            if song['name'] in self.__playlist['name'].tolist()
-        ]
-
-
-    def __find_recommendations_to_songs(self, base_songs: 'list[dict[str, Any]]', subset_name: str) -> 'dict[str, Any]':
-        """Generates a song format record from a list of songs, with all the information the "song-based" recommendation needs
-
-        Args:
-            base_songs (list[dict[str, Any]]): List of base songs
-            subset_name (str): Name of thihs subset of songs (barely seen, unless the dataframe is printed with this record in it)
-
-        Returns:
-            dict[str, Any]: New song fomat record with the information gathered from the list of base songs
-        """
-        temp_genres = list(reduce(lambda acc, x: acc + list(set(x['genres']) - set(acc)), base_songs, []))
-
-        temp_artists = list(reduce(lambda acc, x: acc + list(set(x['artists']) - set(acc)), base_songs, []))
-
-        latest_fav = {
-            'id': "",
-            'name': subset_name,
-            'genres': temp_genres,
-            'artists': temp_artists,
-            'genres_indexed': self.__get_genres([util.item_list_indexed(song['genres'], all_items=self.__all_genres) for song in base_songs])
-        }
-
-        latest_fav['artists_indexed'] = self.__get_artists([util.item_list_indexed(song['artists'], all_items=self.__all_artists) for song in base_songs])
-
-        latest_fav['popularity'] = int(round(reduce(lambda acc, song: acc + int(song['popularity']), base_songs, 0) / len(base_songs)))
-
-        latest_fav['danceability'] = float(reduce(lambda acc, song: acc + float(song['danceability']), base_songs, 0) / len(base_songs))
-
-        latest_fav['loudness'] = float(reduce(lambda acc, song: acc + float(song['loudness']), base_songs, 0) / len(base_songs))
-
-        latest_fav['energy'] = float(reduce(lambda acc, song: acc + float(song['energy']), base_songs, 0) / len(base_songs))
-
-        latest_fav['instrumentalness'] = float(reduce(lambda acc, song: acc + float(song['instrumentalness']), base_songs, 0) / len(base_songs))
-
-        latest_fav['tempo'] = float(reduce(lambda acc, song: acc + float(song['tempo']), base_songs, 0) / len(base_songs))
-
-        latest_fav['valence'] = float(reduce(lambda acc, song: acc + float(song['valence']), base_songs, 0) / len(base_songs))
-
-        return latest_fav
-
-    def __prepare_fav_data(self, term: str) -> 'dict[str, Any]':
-        """Function that expands on the formatting of the top_5 some time_range favorites
-
-        Args:
-            term (str): The time range to get the top 5 songs from ('medium', 'short')
-
-        Returns:
-            dict[str,]: recommendations for the favorite songs
-        """
-        top_5_songs = self.__get_top_5(term)
-
-        return self.__find_recommendations_to_songs(
-            base_songs=top_5_songs,
-            subset_name="Recent-ish Favorites" if term == 'medium' else "Latest Favorites"
+        return self.playlist.get_recommendations_for_song(
+            song_name=song_name,
+            artist_name=artist_name,
+            with_distance=with_distance,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+            print_base_caracteristics=print_base_caracteristics
         )
 
-    def __end_prepared_fav_data(self, type: str) -> 'list[dict[str, Any]]':
-        """Final preparation for favorite data before getting visible
-
-        Args:
-            type (str): Playlist creation type
-
-        Returns:
-            list[dict[str,]]: song dictionary
-        """
-        song_dict = self.__song_dict[:]
-        fav = self.__prepare_fav_data(type)
-        song_dict.append(fav)
-        return song_dict
-
+    @needs_playlist
     def get_playlist(self) -> pd.DataFrame:
         """Function that returns the playlist as pandas DataFrame with the needed, human readable, columns
 
         Returns:
             pd.DataFrame: Playlist DataFrame
         """
-        return self.__playlist[['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']]
-
-    @util.deprecated
-    def get_short_term_favorites_playlist(
-        self,
-        generate_csv: bool = False,
-        with_distance: bool = False,
-        build_playlist: bool = False,
-        generate_parquet: bool = False,
-    ) -> Union[pd.DataFrame, None]:
-        """###DEPRECATED METHOD###\n
-        Playlist which centralises the actions for a recommendation made for top 5 songs short term
-
-        Note
-            The build_playlist option when set to True will change the user's library
-
-        Args:
-            generate_csv (bool, optional): Whether to generate a CSV file containing the recommended playlist. Defaults to False.
-            with_distance (bool, optional): Whether to allow the distance column to the DataFrame returned, which will have no actual value for most use cases, since  it does not obey any actual unit, it is just a mathematical value to determine the closet songs. Defaults to False.
-            build_playlist (bool, optional): Whether to generate a parquet file containing the recommended playlist. Defaults to False.
-            generate_parquet (bool, optional): Whether to build the playlist to the user's library. Defaults to False.
-
-        Returns:
-            pd.DataFrame: Short term favorites DataFrame
-        """
-        if self.__deny_favorites:
-            logging.error("The chosen playlist does not contain the user's favorite songs")
-            return
-        df = self.__short_fav
-        playlist_name = 'Latest Favorites'
-        if generate_csv:
-            df.to_csv(f'{playlist_name}.csv')
-        if generate_parquet:
-            df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
-
-        if build_playlist:
-            self.__write_playlist('short', 51)
-
-        return df if with_distance else df.drop(columns=['distance'])
-
-    @util.deprecated
-    def get_medium_term_favorites_playlist(
-            self,
-            with_distance: bool = False,
-            generate_csv: bool = False,
-            generate_parquet: bool = False,
-            build_playlist: bool = False
-        ) -> Union[pd.DataFrame, None]:
-        """###DEPRECATED METHOD###\n
-        Playlist which centralises the actions for a recommendation made for top 5 songs medium term
-
-        Note
-            The build_playlist option when set to True will change the user's library
-
-        Args:
-            with_distance (bool, optional): Whether to allow the distance column to the DataFrame returned, which will have no actual value for most use cases, since  it does not obey any actual unit, it is just a mathematical value to determine the closet songs. Defaults to False.
-            generate_csv (bool, optional): Whether to generate a CSV file containing the recommended playlist. Defaults to False.
-            generate_parquet (bool, optional): Whether to generate a parquet file containing the recommended playlist. Defaults to False.
-            build_playlist (bool, optional): Whether to build the playlist to the user's library. Defaults to False.
-
-        Returns:
-            pd.DataFrame: Medium term favorites DataFrame
-        """
-        if self.__deny_favorites:
-            logging.error("The chosen playlist does not contain the user's favorite songs")
-            return
-        df = self.__medium_fav
-        playlist_name = 'Recent-ish Favorites'
-        if generate_csv:
-            df.to_csv(f'{playlist_name}.csv')
-        if generate_parquet:
-            df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
-
-        if build_playlist:
-            self.__write_playlist('medium', 51)
-
-        return df if with_distance else df.drop(columns=['distance'])
-
-    def __prepare_favorites_playlist(self):
-        """###DEPRECATED METHOD###\n
-        Note: Although this method and the whole medium and short term favorite category is deprecated, this method will stil run, since somebody may want to use it. Having that said, I do not recommend it
-
-        Automatic creation of both the favorites related recommendations
-        """
-        try:
-            self.__short_fav = self.__get_recommendations('short',  self.__end_prepared_fav_data('short'))
-            self.__medium_fav = self.__get_recommendations('medium',  self.__end_prepared_fav_data('medium'))
-        except ValueError:
-            return
-
-    def get_most_listened(self, time_range: str = 'long', K: int = 50, build_playlist: bool = False) -> pd.DataFrame:
-        """Function that creates the most-listened songs playlist for a given period of time in the users profile
-
-        Args:
-            time_range (str, optional): time range ('long', 'medium', 'short'). Defaults to 'long'.
-            K (int, optional): Number of the most listened songs to return. Defaults to 50.
-
-        Raises:
-            ValueError: time range does not correspond to a valid time range ('long', 'medium', 'short')
-            ValueError: Value for K must be between 1 and 1500
-
-
-        Returns:
-            pd.DataFrame: pandas DataFrame containing the top K songs in the time range
-        """
-        if time_range not in ['long', 'medium', 'short']:
-            raise ValueError('time_range must be long, medium or short')
-
-        if not (1 < K <= 1500):
-            raise ValueError(f'Value for K must be between 1 and 1500: {time_range} term most listened')
-
-        top = requests.get_request(url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit={K}', headers=self.__headers).json()
-
-        top_songs = [
-            {
-                'id': song['id'],
-                'name': song['name'],
-                'popularity': song['popularity'],
-                'genres': self.__get_song_genres(song),
-                'artists': [artist['name'] for artist in song['artists']]
-            }
-            for song in top['items']
-        ]
-
-        for _ in range(2):
-            try:
-
-                if build_playlist:
-                    self.__write_playlist(f'most-listened-{time_range}', K, additional_info=[x['id'] for x in top_songs])
-
-            except AccessTokenExpiredError as e:
-                logging.warning('Error due to the access token expiration')
-                auth_token = auth.get_auth()
-
-                self.__auth_token = auth_token
-
-                self.__headers['Authorization'] = f'Bearer {auth_token}'
-            else:
-                break
-
-        return pd.DataFrame(
-            data=[
-                {
-                    'name': x['name'],
-                    'genres': x['genres'],
-                    'artists': x['artists'],
-                    'popularity': x['popularity']
-                }
-                for x in top_songs
-            ],
-            columns=['name', 'artists', 'genres', 'popularity']
-        )
-
-    def __playlist_needs_update(self, playlist: 'tuple[str, str, str, str]', playlist_types_to_update: 'list[str]') -> bool:
-        """Function to determine if a playlist inside the user's library needs to be updated
-
-        Args:
-            playlist (tuple[str, str, str, str]): Playlist information
-            playlist_types_to_update (list[str]): Playlist types to be updated
-
-        Returns:
-            bool: The flag that indicates whether the playlist should be updated or not
-        """
-        _, name, description, _ = playlist
-
-        if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
-            return True
-
-        elif (
-            ' - 20' not in name and
-            'Profile Recommendation' in name and
-            any(
-                playlist_type in playlist_types_to_update
-                for playlist_type in {'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}
-            )
-        ):
-            return True
-
-        elif f', within the playlist {self.__base_playlist_name}' in description or self.__update_created_files:
-            if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)) and 'song-related' in playlist_types_to_update:
-                return True
-
-            elif (re.match(r"\'(.*?)\' Mix", name) or re.match(r'\"(.*?)\" Mix', name)) and 'artist-mix' in playlist_types_to_update:
-                return True
-
-            elif (re.match(r"This once was \'(.*?)\'", name) or re.match(r'This once was \"(.*?)\"', name)) and 'artist-full' in playlist_types_to_update:
-                return True
-
-            elif 'Playlist Recommendation' in name and ' - 20' not in name and 'playlist-recommendation' in playlist_types_to_update:
-                return True
-
-            elif 'Songs related to the mood' in description and 'mood' in playlist_types_to_update:
-                return True
-
-            elif 'most listened recommendations' in name and 'most-listened-recommendation' in playlist_types_to_update:
-                return True
-
-        return False
-
-    def update_all_generated_playlists(
-            self, *,
-            K: Union[int, None] = None,
-            playlist_types_to_update: Union['list[str]', None] = None,
-            playlist_types_not_to_update: Union['list[str]', None] = None
-        ) -> None:
-        """Update all package generated playlists in batch
-
-        Note:
-            It is NOT recommended to use the K parameter in this function, unless 100% on purpose, since it will make all the playlists have the same number of songs in them
-
-        Arguments:
-            K (int, optional): Number of songs in the new playlists, if not set, defaults to the number of songs already in the playlist. Defaults to None.
-            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all == ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood', 'most-listened-recommendation'].
-            playlist_types_not_to_update (list[str], optional): List of playlist types not to update. For example, if you want to update all playlists but song-related playlists use this argument as ['song-related']. it can be used alongside with the playlist_types_to_update but it can become confusing or redundant. Defaults to none == [].
-        """
-        if playlist_types_to_update is None:
-            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood', 'most-listened-recommendation']
-
-        if playlist_types_not_to_update is None:
-            playlist_types_not_to_update = []
-
-        playlist_types_to_update = [playlist_type for playlist_type in playlist_types_to_update if playlist_type not in playlist_types_not_to_update]
-
-        if 'profile-recommendation' in playlist_types_to_update:
-            logging.info('After version 4.4.0, the profile-recommendation playlists are separated in short, medium and long term. See the update_all_created_playlists docstring or the documentation at: https://github.com/nikolas-virionis/spotify-api')
-            playlist_types_to_update.remove('profile-recommendation')
-            for playlist_type in {'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}:
-                if playlist_type not in playlist_types_to_update:
-                    playlist_types_to_update.append(playlist_type)
-
-        if 'profile-recommendation' in playlist_types_not_to_update:
-            for playlist_type in {'profile-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}:
-                if playlist_type in playlist_types_to_update:
-                    playlist_types_to_update.remove(playlist_type)
-
-        total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=0', headers=self.__headers).json()['total']
-
-        playlists = []
-
-        for offset in range(0, total_playlist_count, 50):
-            request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=self.__headers).json()
-
-            playlists += [(playlist['id'], playlist['name'], playlist['description'], playlist['tracks']['total']) for playlist in request['items']]
-
-        playlists = [
-                playlist
-                for playlist in playlists
-                if self.__playlist_needs_update(
-                        playlist=playlist,
-                        playlist_types_to_update=playlist_types_to_update
-                )
+        return self.playlist.get_dataframe().copy()[
+            [
+                'id',
+                'name',
+                'artists',
+                'genres',
+                'popularity',
+                'added_at',
+                'danceability',
+                'loudness',
+                'energy',
+                'instrumentalness',
+                'tempo',
+                'valence'
             ]
+        ]
 
-        last_printed_perc_update = 0
-
-        for index, (playlist_id, name, description, total_tracks) in enumerate(playlists):
-            try:
-                logging.debug(f'Updating song {name} - {index}/{len(playlists)}')
-                if last_printed_perc_update + 10 <= (perc_update := next((perc for perc in range(100, 0, -10) if (100 * index) / len(playlists) >= perc), 100)) < 100:
-                    logging.info(f'Playlists update operation at {perc_update}%')
-                    last_printed_perc_update = perc_update
-
-                if K is not None:
-                    total_tracks = K
-
-                if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
-                    self.get_most_listened(time_range=name.split(" ")[0].lower(), K=total_tracks, build_playlist=True)
-
-                elif f', within the playlist {self.__base_playlist_name}' in description or self.__update_created_files:
-                    if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)) and 'song-related' in playlist_types_to_update:
-                        song_name = name.replace(" Related", '')[1:-1]
-                        self.__song_name = song_name
-                        self.__write_playlist(type='song', K=total_tracks - 1, additional_info=song_name)
-
-                    elif (re.match(r"\'(.*?)\' Mix", name) or re.match(r'\"(.*?)\" Mix', name)) and 'artist-mix' in playlist_types_to_update:
-                        artist_name = name.replace(" Mix", '')[1:-1]
-                        self.__artist_name = artist_name
-                        self.artist_specific_playlist(
-                            K=total_tracks,
-                            build_playlist=True,
-                            artist_name=artist_name,
-                            complete_with_similar=True,
-                            _auto=True
-                        )
-
-                    elif (re.match(r"This once was \'(.*?)\'", name) or re.match(r'This once was \"(.*?)\"', name)) and 'artist-full' in playlist_types_to_update:
-                        artist_name = name.replace("This once was ", '')[1:-1]
-                        self.__artist_name = artist_name
-                        self.artist_specific_playlist(
-                            K=total_tracks,
-                            build_playlist=True,
-                            artist_name=artist_name,
-                            complete_with_similar=False,
-                            ensure_all_artist_songs=f'All {artist_name}' in description,
-                            _auto=True
-                        )
-
-                    # elif name == 'Recent-ish Favorites':
-                    #     self.__write_playlist(type='medium', K=total_tracks)
-
-                    # elif name == 'Latest Favorites':
-                    #     self.__write_playlist(type='short', K=total_tracks)
-
-                    elif 'Playlist Recommendation' in name and ' - 20' not in name and 'playlist-recommendation' in playlist_types_to_update:
-                        criteria = name.split('(')[1].split(')')[0]
-                        if ',' in criteria:
-                            criteria = 'mixed'
-
-                        time_range = 'all_time' if 'for all_time' in name else name.split('for the last')[-1].split('(')[0].strip()
-
-                        self.get_playlist_recommendation(
-                            K=total_tracks,
-                            build_playlist=True,
-                            time_range=time_range,
-                            main_criteria=criteria,
-                        )
-
-                    elif 'Songs related to the mood' in description and 'mood' in playlist_types_to_update:
-                        mood = ' '.join(name.split(' ')[:-1]).lower()
-
-                        exclude_mostly_instrumental = 'excluding the mostly instrumental songs' in description
-
-                        self.get_songs_by_mood(
-                            mood=mood,
-                            K=total_tracks,
-                            build_playlist=True,
-                            exclude_mostly_instrumental=exclude_mostly_instrumental,
-                        )
-
-                    elif 'most listened recommendations' in name and 'most-listened-recommendation' in playlist_types_to_update:
-                        time_range = '_'.join(name.split(' ')[:2]).lower()
-
-                        self.playlist_songs_based_on_most_listened_tracks(
-                            K=total_tracks,
-                            build_playlist=True,
-                            time_range=time_range,
-                        )
-
-                elif (
-                    ' - 20' not in name and
-                    'Profile Recommendation' in name and
-                    any(
-                        playlist_type in playlist_types_to_update
-                        for playlist_type in {'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}
-                    )
-                ):
-                    criteria = name.split('(')[1].split(')')[0]
-                    criteria_name = criteria
-
-                    if ',' in criteria:
-                        criteria = 'mixed'
-
-                    if 'term' in name.lower():
-                        time_range = '_'.join(name.split(' ')[1:3]).lower()
-                    else:
-                        time_range = 'short_term'
-                        playlist_name = f"{time_range.replace('_', ' ').capitalize()} Profile Recommendation ({criteria_name})"
-                        description = f'''{time_range.replace('_', ' ').capitalize()} Profile-based recommendations based on favorite {criteria_name}'''
-
-                        data = {
-                            "name": playlist_name,
-                            "description": description,
-                            "public": False
-                        }
-
-                        logging.info(f'Updating the name and description of the playlist {name} because of new time range specifications added to the profile_recommendation function in version 4.4.0')
-                        logging.info('In case of any problems with the feature, submit an issue at: https://github.com/nikolas-virionis/spotify-api/issues')
-
-                        update_playlist_details = requests.put_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}', headers=self.__headers, data=data)
-
-                    if f"{time_range.replace('_', '-')}-profile-recommendation" not in playlist_types_to_update:
-                        continue
-
-                    self.get_profile_recommendation(
-                        K=total_tracks,
-                        build_playlist=True,
-                        time_range=time_range,
-                        main_criteria=criteria,
-                    )
-
-            except ValueError as e:
-                logging.error(f"Unfortunately we couldn't update a playlist because\n {e}")
-
-        logging.info('Playlists update operation at 100%')
-
-    def get_playlist_trending_genres(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> Union[pd.DataFrame, None]:
+    @needs_playlist
+    def get_playlist_trending_genres(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> pd.DataFrame:
         """Calculates the amount of times each genre was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             plot_top(int|bool , optional): the number of top genres to be plotted. Must be 5, 10, 15 or False. No chart will be plotted if set to False. Defaults to False.
 
         Raises:
             ValueError: If the time_range parameter is not valid the error is raised.
             ValueError: If plot_top parameter is not valid the error is raised.
 
         Returns:
             pd.DataFrame: The dictionary that contains how many times each genre was spotted in the playlist in the given time range.
         """
-        if time_range not in ['all_time', 'month', 'trimester', 'semester', 'year']:
-            raise ValueError('time_range must be one of the following: "all_time", "month", "trimester", "semester", "year"')
-
-        if plot_top and plot_top > 30:
-            raise ValueError('plot_top must be either an int smaller than 30 or False')
 
-        playlist = self.__playlist[self.__playlist['added_at'] > util.get_datetime_by_time_range(time_range=time_range)]
-
-        if not len(playlist):
-            logging.warning(f"No songs added to the playlist in the time range {time_range} ")
-            return None
-
-        genres = list(reduce(lambda x, y: list(x) + list(y), playlist['genres'], []))
-
-        genres_dict = dict(reduce(lambda x, y: util.list_to_count_dict(dictionary=x, item=y), genres, {}))
-
-        genres_dict['total'] = len(playlist['genres'])
-
-        genres_dict = dict(sorted(genres_dict.items(), key=lambda x: x[1], reverse=True))
-
-        genres_dict = util.value_dict_to_value_and_percentage_dict(dictionary=genres_dict)
-
-        dictionary = {'name': [], 'number of songs': [], 'rate': []}
-
-        for key, value in genres_dict.items():
-            dictionary['name'].append(key)
-            dictionary['number of songs'].append(value['value'])
-            dictionary['rate'].append(value['percentage'])
-
-        df = pd.DataFrame(data=dictionary, columns=['name', 'number of songs', 'rate'])
-
-        if plot_top:
-            core.plot_bar_chart(
-                df=df,
-                top=plot_top,
-                plot_max=reduce(lambda x, y: x + y, df['rate'][1:4], 0) >= 0.50
-            )
-
-        return df
+        return self.playlist.get_playlist_trending_genres(
+            plot_top=plot_top,
+            time_range=time_range,
+        )
 
-    def get_playlist_trending_artists(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> Union[pd.DataFrame, None]:
+    @needs_playlist
+    def get_playlist_trending_artists(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> pd.DataFrame:
         """Calculates the amount of times each artist was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             plot_top(int|bool , optional): the number of top genres to be plotted. No chart will be plotted if set to False. Defaults to False.
 
         Raises:
             ValueError: If the time_range parameter is not valid the error is raised.
 
         Returns:
             pd.DataFrame: The dictionary that contains how many times each artist was spotted in the playlist in the given time range.
         """
-        if time_range not in ['all_time', 'month', 'trimester', 'semester', 'year']:
-            raise ValueError(
-                'time_range must be one of the following: "all_time", "month", "trimester", "semester", "year"')
-
-        if plot_top and plot_top > 30:
-            raise ValueError(
-                'plot_top must be either an int smaller than 30 or False')
-
-        playlist = self.__playlist[self.__playlist['added_at'] >
-                                   util.get_datetime_by_time_range(time_range=time_range)]
 
-        if not len(playlist):
-            logging.warning(f"No songs added to the playlist in the time range {time_range} ")
-            return None
-
-        artists = list(reduce(lambda x, y: list(x) + list(y), playlist['artists'], []))
-
-        artists_dict = dict(reduce(lambda x, y: util.list_to_count_dict(
-            dictionary=x, item=y), artists, {}))
-
-        artists_dict['total'] = len(playlist['artists'])
-
-        artists_dict = dict(sorted(artists_dict.items(),
-                            key=lambda x: x[1], reverse=True))
-
-        artists_dict = util.value_dict_to_value_and_percentage_dict(
-            dictionary=artists_dict)
-
-        dictionary = {'name': [], 'number of songs': [], 'rate': []}
+        return self.playlist.get_playlist_trending_artists(
+            plot_top=plot_top,
+            time_range=time_range,
+        )
 
-        for key, value in artists_dict.items():
-            dictionary['name'].append(key)
-            dictionary['number of songs'].append(value['value'])
-            dictionary['rate'].append(value['percentage'])
+    @needs_playlist
+    def artist_only_playlist(
+        self,
+        artist_name: str,
+        number_of_songs: int = 50,
+        build_playlist: bool = False,
+        ensure_all_artist_songs: bool = True
+    ) -> pd.DataFrame:
+        """Function that generates DataFrame containing only a specific artist songs, with the possibility of completing it with the closest songs to that artist
 
-        df = pd.DataFrame(data=dictionary, columns=[
-                          'name', 'number of songs', 'rate'])
+        Args:
+            artist_name (str): The name of the artist
+            number_of_songs (int, optional): Maximum number of songs. Defaults to 50.
+            with_distance (bool, optional): Whether to allow the distance column to the DataFrame returned, which will have no actual value for most use cases, since it does not obey any actual unit, it is just a mathematical value to determine the closet songs.  Defaults to False.
+            build_playlist (bool, optional): Whether to build the playlist to the user's library. Defaults to False.
+            ensure_all_artist_songs (bool, optional): Whether to ensure that all artist songs are in the playlist, regardless of the number_of_songs number specified. Defaults to True
+            print_base_caracteristics (bool, optional): Whether to print the base / informed song information, in order to check why such predictions were made by the algorithm. ONLY TAKES EFFECT IF complete_with_similar == True AND number_of_songs > NUMBER OF SONGS WITH THAT ARTIST. Defaults to False.
 
-        if plot_top:
-            core.plot_bar_chart(df=df, top=plot_top, plot_max=reduce(
-                lambda x, y: x + y, df['rate'][1:4], 0) >= 0.50)
+        Raises:
+            ValueError: Value for number_of_songs must be between 1 and 1500
+            ValueError: The artist_name specified is not valid
 
-        return df
+        Returns:
+            pd.DataFrame: DataFrame containing the new playlist based on the artist
+        """
+        return self.playlist.artist_only_playlist(
+            artist_name=artist_name,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+            ensure_all_artist_songs=ensure_all_artist_songs
+        )
 
-    def artist_specific_playlist(
+    @needs_playlist
+    def artist_and_related_playlist(
         self,
         artist_name: str,
-        K: int = 50,
+        number_of_songs: int = 50,
         with_distance: bool = False,
         build_playlist: bool = False,
-        complete_with_similar: bool = False,
-        ensure_all_artist_songs: bool = True,
         print_base_caracteristics: bool = False,
-        _auto: bool = False
-    ) -> pd.DataFrame:  # sourcery skip: extract-method
+    ) -> pd.DataFrame:
         """Function that generates DataFrame containing only a specific artist songs, with the possibility of completing it with the closest songs to that artist
 
         Args:
             artist_name (str): The name of the artist
-            K (int, optional): Maximum number of songs. Defaults to 50.
-            with_distance (bool, optional): Whether to allow the distance column to the DataFrame returned, which will have no actual value for most use cases, since it does not obey any actual unit, it is just a mathematical value to determine the closet songs. ONLY TAKES EFFECT IF complete_with_similar == True AND K > NUMBER_OF_SONGS_WITH_THAT_ARTIST. Defaults to False.
+            number_of_songs (int, optional): Maximum number of songs. Defaults to 50.
+            with_distance (bool, optional): Whether to allow the distance column to the DataFrame returned, which will have no actual value for most use cases, since it does not obey any actual unit, it is just a mathematical value to determine the closet songs. Defaults to False.
             build_playlist (bool, optional): Whether to build the playlist to the user's library. Defaults to False.
-            ensure_all_artist_songs (bool, optional): Whether to ensure that all artist songs are in the playlist, regardless of the K number specified. Defaults to True
-            complete_with_similar (bool, optional): Flag to complete the list of songs with songs that are similar to that artist, until the K number is reached. Only applies if K is greater than the number of songs by that artist in the playlist. Defaults to False.
-            print_base_caracteristics (bool, optional): Whether to print the base / informed song information, in order to check why such predictions were made by the algorithm. ONLY TAKES EFFECT IF complete_with_similar == True AND K > NUMBER OF SONGS WITH THAT ARTIST. Defaults to False.
+            print_base_caracteristics (bool, optional): Whether to print the base / informed song information, in order to check why such predictions were made by the algorithm. ONLY TAKES EFFECT IF complete_with_similar == True AND number_of_songs > NUMBER OF SONGS WITH THAT ARTIST. Defaults to False.
 
         Raises:
-            ValueError: Value for K must be between 1 and 1500
+            ValueError: Value for number_of_songs must be between 1 and 1500
             ValueError: The artist_name specified is not valid
 
         Returns:
             pd.DataFrame: DataFrame containing the new playlist based on the artist
         """
-        if not (1 < K <= 1500):
-            raise ValueError(
-                f'Value for K must be between 1 and 1500 for the {artist_name} {"Mix" if complete_with_similar else "specific playlist"}')
-
-        artist_songs = self.__playlist[self.__playlist['artists'].str.contains(
-            artist_name, regex=False)]
-
-        if not len(artist_songs):
-            raise ValueError(
-                f'{artist_name = } does not exist in the playlist')
-
-        self.__artist_name = artist_name
-
-        columns = ['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']
-
-        if complete_with_similar:
-            artist_songs_record_song_dict = [{
-                    'id': '',
-                    'name': song['name'],
-                    'artists': song['artists'],
-                    'genres': song['genres'],
-                    'artists_indexed': song['artists_indexed'],
-                    'genres_indexed': song['genres_indexed'],
-                    'popularity': song['popularity'],
-                    'added_at': song['added_at'],
-                    'danceability': song['danceability'],
-                    'loudness': song['loudness'],
-                    'energy': song['energy'],
-                    'instrumentalness': song['instrumentalness'],
-                    'tempo': song['tempo'],
-                    'valence': song['valence']
-                }
-                for song in [
-                    song
-                    for song in self.__song_dict
-                    if artist_name in song['artists']
-                ]
-            ]
-
-            artist_songs_record = self.__find_recommendations_to_songs(base_songs=artist_songs_record_song_dict, subset_name=f"{artist_name} Mix")
-
-            song_dict = [{
-                    'id': song['id'],
-                    'name': song['name'],
-                    'artists': song['artists'],
-                    'genres': song['genres'],
-                    'artists_indexed': song['artists_indexed'],
-                    'genres_indexed': song['genres_indexed'],
-                    'popularity': song['popularity'],
-                    'added_at': song['added_at'],
-                    'danceability': song['danceability'],
-                    'loudness': song['loudness'],
-                    'energy': song['energy'],
-                    'instrumentalness': song['instrumentalness'],
-                    'tempo': song['tempo'],
-                    'valence': song['valence']
-                }
-                for song in [
-                    song
-                    for song in self.__song_dict
-                    if artist_name in song['artists']
-                ]
-            ]
-
-            song_dict.append(artist_songs_record)
-
-            mix_songs = self.__get_recommendations('artist-related', song_dict, K=K-len(artist_songs) if len(artist_songs) < K else len(artist_songs) // 3)
-
-            ids = pd.concat([artist_songs['id'], mix_songs['id']]).tolist()
-
-            if with_distance:
-                df = artist_songs[columns]
-
-                columns.append('distance')
-
-                df['distance'] = pd.to_numeric(0)
-
-                df = pd.concat([df[columns], mix_songs[columns]])
-
-            else:
-                df = pd.concat([artist_songs[columns], mix_songs[columns]])
-
-            if print_base_caracteristics and not _auto:
-                name = artist_songs_record['name']
-                genres = artist_songs_record['genres']
-                artists = artist_songs_record['artists']
-                popularity = artist_songs_record['popularity']
-                danceability = artist_songs_record['danceability']
-                loudness = artist_songs_record['loudness']
-                energy = artist_songs_record['energy']
-                instrumentalness = artist_songs_record['instrumentalness']
-                tempo = artist_songs_record['tempo']
-                valence = artist_songs_record['valence']
-                util.print_base_caracteristics(name, genres, artists, popularity, danceability, loudness, energy, instrumentalness, tempo, valence)
-
-        elif not _auto and len(artist_songs) < K:
-            logging.info(f'Playlist has only {len(artist_songs)} songs')
-            logging.info(f'To fill the {K = } number of songs, consider using the flag complete_with_similar')
-            ids = artist_songs['id'].tolist()
-            df = artist_songs[columns]
-
-        elif ensure_all_artist_songs:
-            ids = artist_songs['id'].tolist()
-            df = artist_songs[columns]
-
-        else:
-            ids = artist_songs['id'][:K].tolist()
-            df = artist_songs[columns][:K]
-
-        if build_playlist:
-            self.__write_playlist(
-                K=K,
-                type=f'artist{"-related" if complete_with_similar else "-full" if ensure_all_artist_songs else ""}',
-                additional_info=ids
-            )
-
-        return df.reset_index(drop=True)
+        return self.playlist.artist_and_related_playlist(
+            artist_name=artist_name,
+            with_distance=with_distance,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+            print_base_caracteristics=print_base_caracteristics
+        )
 
+    @needs_playlist
     def audio_features_extraordinary_songs(self) -> 'dict[str, dict]':
         """Returns a dictionary with the maximum and minimum values for each audio feature used in the package
 
         Note:
             Although there are many more audio features available in Spotify Web API, these were the only ones needed to provide the best fitting recommendations within this package
 
         Note:
@@ -1523,1003 +394,169 @@
             - instrumentalness: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content
             - tempo: The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.
             - valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
 
         Returns:
             dict[str, dict]: The dictionary with the maximum and minimum values for each audio feature used in the package
         """
-        df = self.__playlist[['id', 'name', 'artists', 'genres', 'popularity','added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']]
-
-        df_danceability = df.sort_values('danceability', ascending=True)
-        df_loudness = df.sort_values('loudness', ascending=True)
-        df_energy = df.sort_values('energy', ascending=True)
-        df_instrumentalness = df.sort_values('instrumentalness', ascending=True)
-        df_tempo = df.sort_values('tempo', ascending=True)
-        df_valence = df.sort_values('valence', ascending=True)
-        max_danceability = df_danceability.tail(n=1).reset_index(drop=True)
-        min_danceability = df_danceability.head(n=1).reset_index(drop=True)
-        max_loudness = df_loudness.tail(n=1).reset_index(drop=True)
-        min_loudness = df_loudness.head(n=1).reset_index(drop=True)
-        max_energy = df_energy.tail(n=1).reset_index(drop=True)
-        min_energy = df_energy.head(n=1).reset_index(drop=True)
-        max_instrumentalness = df_instrumentalness.tail(n=1).reset_index(drop=True)
-        min_instrumentalness = df_instrumentalness.head(n=1).reset_index(drop=True)
-        max_tempo = df_tempo.tail(n=1).reset_index(drop=True)
-        min_tempo = df_tempo.head(n=1).reset_index(drop=True)
-        max_valence = df_valence.tail(n=1).reset_index(drop=True)
-        min_valence = df_valence.head(n=1).reset_index(drop=True)
-
-        return {
-            'max_loudness': {
-                'id': max_loudness['id'][0],
-                'name': max_loudness['name'][0],
-                'genres': max_loudness['genres'][0],
-                'artists': max_loudness['artists'][0],
-                'popularity': max_loudness['popularity'][0],
-                'added_at': max_loudness['added_at'][0],
-                'danceability': max_loudness['danceability'][0],
-                'loudness': max_loudness['loudness'][0],
-                'energy': max_loudness['energy'][0],
-                'instrumentalness': max_loudness['instrumentalness'][0],
-                'tempo': max_loudness['tempo'][0],
-                'valence': max_loudness['valence'][0]
-            },
-            'min_loudness': {
-                'id': min_loudness['id'][0],
-                'name': min_loudness['name'][0],
-                'genres': min_loudness['genres'][0],
-                'artists': min_loudness['artists'][0],
-                'popularity': min_loudness['popularity'][0],
-                'added_at': min_loudness['added_at'][0],
-                'danceability': min_loudness['danceability'][0],
-                'loudness': min_loudness['loudness'][0],
-                'energy': min_loudness['energy'][0],
-                'instrumentalness': min_loudness['instrumentalness'][0],
-                'tempo': min_loudness['tempo'][0],
-                'valence': min_loudness['valence'][0]
-            },
-            'max_danceability': {
-                'id': max_danceability['id'][0],
-                'name': max_danceability['name'][0],
-                'genres': max_danceability['genres'][0],
-                'artists': max_danceability['artists'][0],
-                'popularity': max_danceability['popularity'][0],
-                'added_at': max_danceability['added_at'][0],
-                'danceability': max_danceability['danceability'][0],
-                'loudness': max_danceability['loudness'][0],
-                'energy': max_danceability['energy'][0],
-                'instrumentalness': max_danceability['instrumentalness'][0],
-                'tempo': max_danceability['tempo'][0],
-                'valence': max_danceability['valence'][0]
-            },
-            'min_danceability': {
-                'id': min_danceability['id'][0],
-                'name': min_danceability['name'][0],
-                'genres': min_danceability['genres'][0],
-                'artists': min_danceability['artists'][0],
-                'popularity': min_danceability['popularity'][0],
-                'added_at': min_danceability['added_at'][0],
-                'danceability': min_danceability['danceability'][0],
-                'loudness': min_danceability['loudness'][0],
-                'energy': min_danceability['energy'][0],
-                'instrumentalness': min_danceability['instrumentalness'][0],
-                'tempo': min_danceability['tempo'][0],
-                'valence': min_danceability['valence'][0]
-            },
-            'max_energy': {
-                'id': max_energy['id'][0],
-                'name': max_energy['name'][0],
-                'genres': max_energy['genres'][0],
-                'artists': max_energy['artists'][0],
-                'popularity': max_energy['popularity'][0],
-                'added_at': max_energy['added_at'][0],
-                'danceability': max_energy['danceability'][0],
-                'loudness': max_energy['loudness'][0],
-                'energy': max_energy['energy'][0],
-                'instrumentalness': max_energy['instrumentalness'][0],
-                'tempo': max_energy['tempo'][0],
-                'valence': max_energy['valence'][0]
-            },
-            'min_energy': {
-                'id': min_energy['id'][0],
-                'name': min_energy['name'][0],
-                'genres': min_energy['genres'][0],
-                'artists': min_energy['artists'][0],
-                'popularity': min_energy['popularity'][0],
-                'added_at': min_energy['added_at'][0],
-                'danceability': min_energy['danceability'][0],
-                'loudness': min_energy['loudness'][0],
-                'energy': min_energy['energy'][0],
-                'instrumentalness': min_energy['instrumentalness'][0],
-                'tempo': min_energy['tempo'][0],
-                'valence': min_energy['valence'][0]
-            },
-            'max_instrumentalness': {
-                'id': max_instrumentalness['id'][0],
-                'name': max_instrumentalness['name'][0],
-                'genres': max_instrumentalness['genres'][0],
-                'artists': max_instrumentalness['artists'][0],
-                'popularity': max_instrumentalness['popularity'][0],
-                'added_at': max_instrumentalness['added_at'][0],
-                'danceability': max_instrumentalness['danceability'][0],
-                'loudness': max_instrumentalness['loudness'][0],
-                'energy': max_instrumentalness['energy'][0],
-                'instrumentalness': max_instrumentalness['instrumentalness'][0],
-                'tempo': max_instrumentalness['tempo'][0],
-                'valence': max_instrumentalness['valence'][0]
-            },
-            'min_instrumentalness': {
-                'id': min_instrumentalness['id'][0],
-                'name': min_instrumentalness['name'][0],
-                'genres': min_instrumentalness['genres'][0],
-                'artists': min_instrumentalness['artists'][0],
-                'popularity': min_instrumentalness['popularity'][0],
-                'added_at': min_instrumentalness['added_at'][0],
-                'danceability': min_instrumentalness['danceability'][0],
-                'loudness': min_instrumentalness['loudness'][0],
-                'energy': min_instrumentalness['energy'][0],
-                'instrumentalness': min_instrumentalness['instrumentalness'][0],
-                'tempo': min_instrumentalness['tempo'][0],
-                'valence': min_instrumentalness['valence'][0]
-            },
-            'max_tempo': {
-                'id': max_tempo['id'][0],
-                'name': max_tempo['name'][0],
-                'genres': max_tempo['genres'][0],
-                'artists': max_tempo['artists'][0],
-                'popularity': max_tempo['popularity'][0],
-                'added_at': max_tempo['added_at'][0],
-                'danceability': max_tempo['danceability'][0],
-                'loudness': max_tempo['loudness'][0],
-                'energy': max_tempo['energy'][0],
-                'instrumentalness': max_tempo['instrumentalness'][0],
-                'tempo': max_tempo['tempo'][0],
-                'valence': max_tempo['valence'][0]
-            },
-            'min_tempo': {
-                'id': min_tempo['id'][0],
-                'name': min_tempo['name'][0],
-                'genres': min_tempo['genres'][0],
-                'artists': min_tempo['artists'][0],
-                'popularity': min_tempo['popularity'][0],
-                'added_at': min_tempo['added_at'][0],
-                'danceability': min_tempo['danceability'][0],
-                'loudness': min_tempo['loudness'][0],
-                'energy': min_tempo['energy'][0],
-                'instrumentalness': min_tempo['instrumentalness'][0],
-                'tempo': min_tempo['tempo'][0],
-                'valence': min_tempo['valence'][0]
-            },
-            'max_valence': {
-                'id': max_valence['id'][0],
-                'name': max_valence['name'][0],
-                'genres': max_valence['genres'][0],
-                'artists': max_valence['artists'][0],
-                'popularity': max_valence['popularity'][0],
-                'added_at': max_valence['added_at'][0],
-                'danceability': max_valence['danceability'][0],
-                'loudness': max_valence['loudness'][0],
-                'energy': max_valence['energy'][0],
-                'instrumentalness': max_valence['instrumentalness'][0],
-                'tempo': max_valence['tempo'][0],
-                'valence': max_valence['valence'][0]
-            },
-            'min_valence': {
-                'id': min_valence['id'][0],
-                'name': min_valence['name'][0],
-                'genres': min_valence['genres'][0],
-                'artists': min_valence['artists'][0],
-                'popularity': min_valence['popularity'][0],
-                'added_at': min_valence['added_at'][0],
-                'danceability': min_valence['danceability'][0],
-                'loudness': min_valence['loudness'][0],
-                'energy': min_valence['energy'][0],
-                'instrumentalness': min_valence['instrumentalness'][0],
-                'tempo': min_valence['tempo'][0],
-                'valence': min_valence['valence'][0]
-            },
-        }
-
-    @util.deprecated
-    def refresh_token(self, token: str):
-        """###DEPRECATED METHOD###
-        Refreshes the authorization token for the Spotify API, so that it is not necessary to rerun the entire script using the package to reauthenticate
-
-        Args:
-            token (str): Token generated from the Spotify API Console, with the following scopes:
-             - user-top-read
-             - playlist-library-read
-             - playlist-read-private
-             - playlist-library-modify
-             - playlist-modify-private
-        """
-        headers = self.__headers
-        headers['Authorization'] = f'Bearer {token}'
-
-        requests.get_request(
-            url='https://api.spotify.com/v1/me/playlists?limit=0', headers=headers)
-
-        self.__auth_token = token
-        self.__headers = headers
+        return self.playlist.audio_features_extraordinary_songs()
 
+    @needs_playlist
     def audio_features_statistics(self) -> 'dict[str, float]':
-        """FUnctions that returns the statistics (max, min and mean) for the audio features within the playlist
+        """Functions that returns the statistics (max, min and mean) for the audio features within the playlist
 
         Returns:
             dict[str, float]: The dictionary with the statistics
         """
-        df: pd.DataFrame = self.__playlist[['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']]
-
-        return {
-            'min_tempo': df['tempo'].min(),
-            'max_tempo': df['tempo'].max(),
-            'mean_tempo': df['tempo'].mean(),
-            'min_energy': df['energy'].min(),
-            'max_energy': df['energy'].max(),
-            'mean_energy': df['energy'].mean(),
-            'min_valence': df['valence'].min(),
-            'max_valence': df['valence'].max(),
-            'mean_valence': df['valence'].mean(),
-            'min_danceability': df['danceability'].min(),
-            'max_danceability': df['danceability'].max(),
-            'mean_danceability': df['danceability'].mean(),
-            'min_loudness': df['loudness'].min(),
-            'max_loudness': df['loudness'].max(),
-            'mean_loudness': df['loudness'].mean(),
-            'min_instrumentalness': df['instrumentalness'].min(),
-            'max_instrumentalness': df['instrumentalness'].max(),
-            'mean_instrumentalness': df['instrumentalness'].mean(),
-        }
-
-    def get_profile_recommendation(
-            self,
-            K: int = 50,
-            main_criteria: str = 'mixed',
-            save_with_date: bool = False,
-            build_playlist: bool = False,
-            time_range: str = 'short_term'
-        ) -> Union[pd.DataFrame, None]:
-        """Builds a Profile based recommendation
-
-        Args:
-            K (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
-            main_criteria (str, optional): Main criteria for the recommendations playlist. Can be one of the following: 'mixed', 'artists', 'tracks', 'genres'. Defaults to 'mixed'.
-            save_with_date (bool, optional): Flag to save the recommendations playlist as a Point in Time Snapshot. Defaults to False.
-            build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
-            time_range (str, optional): The time range to get the profile most listened information from. Can be one of the following: 'short_term', 'medium_term', 'long_term'. Defaults to 'short_term'
-
-        Raises:
-            ValueError: K must be between 1 and 100
-            ValueError: 'mixed', 'artists', 'tracks', 'genres'
-            ValueError: time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'
-
-        Returns:
-            pd.DataFrame: Recommendations playlist
-        """
-        if not (1 < K <= 100):
-            raise ValueError('K must be between 1 and 100')
-
-        if main_criteria not in {'mixed', 'artists', 'tracks', 'genres'}:
-            raise ValueError("main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
-
-        if time_range not in {'short_term', 'medium_term', 'long_term'}:
-            raise ValueError("time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'")
-
-        tracks = []
-        genres = []
-        artists = []
-
-        for _ in range(2):
-            try:
-
-                if main_criteria != 'tracks':
-                    if self.__top_genres or self.__top_artists:
-                        genres = self.__top_genres
-                        artists = self.__top_artists
-
-                    else:
-                        top_artists_req = requests.get_request(
-                            headers=self.__headers,
-                            url=f'https://api.spotify.com/v1/me/top/artists?time_range={time_range}&limit=5',
-                        ).json()['items']
-
-                        artists = [artist['id'] for artist in top_artists_req]
-                        genres = list(set(reduce(lambda x, y: x + y, [artist['genres'] for artist in top_artists_req], [])))[:5]
-                        self.__top_genres = genres
-                        self.__top_artists = artists
-
-                if main_criteria not in ['artists']:
-                    if self.__top_tracks:
-                        tracks = self.__top_tracks
-
-                    else:
-                        tracks = [
-                            track['id']
-                            for track in requests.get_request(
-                                headers=self.__headers,
-                                url=f'https://api.spotify.com/v1/me/top/tracks?time_range={time_range}&limit=5'
-                            ).json()['items']
-                        ]
-
-                        self.__top_tracks = tracks
-
-                url = f'https://api.spotify.com/v1/recommendations?limit={K}'
-
-                if main_criteria == 'artists':
-                    url += f'&seed_artists={",".join(artists)}'
-                elif main_criteria == 'genres':
-                    url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
-                elif main_criteria == 'mixed':
-                    url += f'&seed_tracks={",".join(tracks[:2])}&seed_artists={",".join(artists[:1])}&seed_genres={",".join(genres[:2])}'
-                elif main_criteria == 'tracks':
-                    url += f'&seed_tracks={",".join(tracks)}'
-
-                recommendations = requests.get_request(url=url, headers=self.__headers).json()
-
-                if not recommendations.get("tracks"):
-                    logging.error(f'There was a problem creating the profile recommendations based on {main_criteria}')
-                    return
-
-                songs = []
-
-                for song in recommendations["tracks"]:
-                    (id, name, popularity, artist), song_genres = util.song_data(song=song, added_at=False), self.__get_song_genres(song)
-                    song['id'] = id
-                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
-                    songs.append({
-                        "id": id,
-                        "name": name,
-                        "artists": artist,
-                        "popularity": popularity,
-                        "genres": song_genres,
-                        "danceability": danceability,
-                        "loudness": loudness,
-                        "energy": energy,
-                        "instrumentalness": instrumentalness,
-                        "tempo": tempo,
-                        "valence": valence
-                    })
-
-                recommendations_playlist = pd.DataFrame(data=songs)
-
-                ids = recommendations_playlist['id'].tolist()
-
-                if build_playlist:
-                    self.__profile_recommendation_date = save_with_date
-                    self.__profile_recommendation_time_range = time_range
-                    self.__profile_recommendation_criteria = main_criteria
-
-                    self.__write_playlist(
-                        K=K,
-                        type='profile-recommendation',
-                        additional_info=ids
-                    )
-
-                return recommendations_playlist
-
-            except AccessTokenExpiredError as e:
-                logging.warning('Error due to the access token expiration')
-                auth_token = auth.get_auth()
-
-                self.__auth_token = auth_token
-
-                self.__headers['Authorization'] = f'Bearer {auth_token}'
-            else:
-                break
+        return self.playlist.audio_features_statistics()
 
+    @needs_playlist
     def get_playlist_recommendation(
         self,
-        K: int = 50,
+        number_of_songs: int = 50,
         time_range: str = 'all_time',
         main_criteria: str = 'mixed',
         save_with_date: bool = False,
         build_playlist: bool = False,
-    ) -> Union[pd.DataFrame, None]:
+    ) -> pd.DataFrame:
         """Builds a playlist based recommendation
 
         Args:
-            K (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
+            number_of_songs (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             main_criteria (str, optional): Main criteria for the recommendations playlist. Can be one of the following: 'mixed', 'artists', 'tracks', 'genres'. Defaults to 'mixed'.
             save_with_date (bool, optional): Flag to save the recommendations playlist as a Point in Time Snapshot. Defaults to False.
             build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
 
         Raises:
-            ValueError: K must be between 1 and 100
-            ValueError: 'mixed', 'artists', 'tracks', 'genres'
+            ValueError: number_of_songs must be between 1 and 100
+            ValueError: main_criteria has to be on of the following: 'mixed', 'artists', 'tracks', 'genres'
 
         Returns:
             pd.DataFrame: Recommendations playlist
         """
 
-        if not (1 < K <= 100):
-            raise ValueError('K must be between 1 and 100')
-
-        if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
-            raise ValueError(
-                "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
-
-        tracks = []
-        genres = []
-        artists = []
-
-
-        for _ in range(2):
-            try:
-                audio_statistics = self.audio_features_statistics()
-
-                if main_criteria not in ['genres', 'tracks']:
-
-                    if (top_artists := self.get_playlist_trending_artists(time_range=time_range)) is None:
-                        return None
-
-                    top_artists_names = top_artists['name'][1:6].tolist()
-
-                    artists = [
-                        requests.get_request(
-                            headers=self.__headers,
-                            url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1'
-                        ).json()['artists']['items'][0]['id']
-                        for x in top_artists_names
-                    ]
-
-                if main_criteria not in ['artists']:
-                    if self.__top_tracks:
-                        tracks = self.__top_tracks
-
-                    else:
-                        tracks = [
-                            track['id']
-                            for track in requests.get_request(
-                                headers=self.__headers,
-                                url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5',
-                            ).json()['items']
-                        ]
-
-                        self.__top_tracks = tracks
-                if main_criteria != 'artists':
-                    if (genres := self.get_playlist_trending_genres(time_range=time_range)) is None:
-                        return None
-
-                    genres = genres['name'][1:6].tolist()[:5]
-
-                min_tempo = audio_statistics['min_tempo'] * 0.8
-                max_tempo = audio_statistics['max_tempo'] * 1.2
-                target_tempo = audio_statistics['mean_tempo']
-                min_energy = audio_statistics['min_energy'] * 0.8
-                max_energy = audio_statistics['max_energy'] * 1.2
-                target_energy = audio_statistics['mean_energy']
-                min_valence = audio_statistics['min_valence'] * 0.8
-                max_valence = audio_statistics['max_valence'] * 1.2
-                target_valence = audio_statistics['mean_valence']
-                min_danceability = audio_statistics['min_danceability'] * 0.8
-                max_danceability = audio_statistics['max_danceability'] * 1.2
-                target_danceability = audio_statistics['mean_danceability']
-                min_loudness = audio_statistics['min_loudness'] * 0.8
-                max_loudness = audio_statistics['max_loudness'] * 1.2
-                target_loudness = audio_statistics['mean_loudness']
-                min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
-                max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
-                target_instrumentalness = audio_statistics['mean_instrumentalness']
-
-                url = f'https://api.spotify.com/v1/recommendations?limit={K}'
-
-                if main_criteria == 'artists':
-                    url += f'&seed_artists={",".join(artists)}'
-
-                elif main_criteria == 'genres':
-                    url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
-                elif main_criteria == 'mixed':
-                    url += f'&seed_tracks={",".join(tracks[:1])}&seed_artists={",".join(artists[:2])}&seed_genres={",".join(genres[:2])}'
-                elif main_criteria == 'tracks':
-                    url += f'&seed_tracks={",".join(tracks[:2])}&seed_genres={",".join(genres[:3])}'
-                url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
-
-                recommendations = requests.get_request(url=url, headers=self.__headers).json()
-
-                songs = []
-
-                for song in recommendations["tracks"]:
-                    (id, name, popularity, artist), song_genres = util.song_data(song=song, added_at=False), self.__get_song_genres(song)
-                    song['id'] = id
-                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
-                    songs.append({
-                        "id": id,
-                        "name": name,
-                        "artists": artist,
-                        "popularity": popularity,
-                        "genres": song_genres,
-                        "danceability": danceability,
-                        "loudness": loudness,
-                        "energy": energy,
-                        "instrumentalness": instrumentalness,
-                        "tempo": tempo,
-                        "valence": valence
-                    })
-
-                recommendations_playlist = pd.DataFrame(data=songs)
-
-                ids = recommendations_playlist['id'].tolist()
-
-                if build_playlist:
-                    self.__playlist_recommendation_date = save_with_date
-                    self.__playlist_recommendation_time_range = time_range
-                    self.__playlist_recommendation_criteria = main_criteria
-
-                    self.__write_playlist(
-                        K=K,
-                        type='playlist-recommendation',
-                        additional_info=ids
-                    )
-
-                return recommendations_playlist
-
-            except AccessTokenExpiredError as e:
-                logging.warning('Error due to the access token expiration')
-                auth_token = auth.get_auth()
-
-                self.__auth_token = auth_token
-
-                self.__headers['Authorization'] = f'Bearer {auth_token}'
-            else:
-                break
-
-    def get_general_recommendation(
-        self,
-        K: int = 50,
-        genres_info: Union['list[str]', None] = None,
-        artists_info: Union['list[str]', None] = None,
-        build_playlist: bool = False,
-        use_main_playlist_audio_features: bool = False,
-        tracks_info: Union['list[str]', 'list[tuple[str]]', 'list[list[str]]', 'dict[str, str]', None] = None,
-    ) -> Union[pd.DataFrame, None]:
-        """Builds a general recommendation based on up to 5 items spread across artists, genres, and tracks.
-
-        Args:
-            K (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
-            genres_info (list[str], optional): list of the genre names to be used in the recommendation. Defaults to [].
-            artists_info (list[str], optional): list of the artist names to be used in the recommendation. Defaults to [].
-            build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
-            use_main_playlist_audio_features (bool, optional): Flag to use the audio features of the main playlist to target better recommendations. Defaults to False.
-            tracks_info (list[str] | list[tuple[str]] | list[list[str]] | dict[str, str]], optional): List of the song names to be used in the recommendations. They can be only the song names, but since there are a lot of songs with the same name i recommend using also the artist name in a key-value format using either a tuple, or list, or dict. Defaults to [].
-
-        Raises:
-            ValueError: K must be between 1 and 100
-            ValueError: At least one of the three args must be provided: genres_info, artists_info, tracks_info
-            ValueError: The sum of the number of items in each of the three args mustn't exceed 5
-            ValueError: The argument tracks_info must be an instance of one of the following 4 types: list[str], list[tuple[str]], list[list[str]], dict[str, str]
-
-        Returns:
-            pd.DataFrame: Recommendations playlist
-        """
-
-        if not (1 < K <= 100):
-            raise ValueError('K must be between 1 and 100')
-
-        if not (genres_info or artists_info or tracks_info):
-            raise ValueError('At least one of the three args must be provided: genres_info, artists_info, tracks_info')
-
-        if genres_info is None:
-            genres_info = []
-
-        if artists_info is None:
-            artists_info = []
-
-        if tracks_info is None:
-            tracks_info = []
-
-        if len(genres_info) + len(artists_info) + len(tracks_info) > 5:
-            raise ValueError('The sum of the number of items in each of the three args mustn\'t exceed 5')
-
-        url = f'https://api.spotify.com/v1/recommendations?limit={K}'
-
-        description = 'General Recommendation based on '
-
-        for _ in range(2):
-            try:
-
-                types = []
-
-                if artists_info:
-                    types.append('artists')
-                    description += 'the artists '
-                    for artist in artists_info:
-                        description += f'{artist}, '
-
-                    description = ' and '.join(description[:-2].rsplit(', ', 1))
-
-                    artists = [
-                        requests.get_request(
-                            headers=self.__headers,
-                            url=f'https://api.spotify.com/v1/search?q={artist}&type=artist&limit=1',
-                        ).json()['artists']['items'][0]['id']
-                        for artist in artists_info
-                    ]
-
-                    url += f'&seed_artists={",".join(artists)}'
-
-                    if len(artists_info) == 1:
-                        description = description.replace('artists', 'artist')
-
-                if genres_info:
-                    types.append('genres')
-                    url += f'&seed_genres={",".join(genres_info)}'
-
-                    if artists_info and not tracks_info:
-                        description += ', and the genres '
-                        final_sep = ''
-                    elif not artists_info and tracks_info:
-                        description += 'the genres '
-                        final_sep = ', and the tracks '
-                    elif not (artists_info or tracks_info):
-                        description += 'the genres '
-                        final_sep = ''
-                    else:  # both artists and tracks exist
-                        description += ', the genres '
-                        final_sep = ', and the tracks '
-
-                    for genre in genres_info:
-                        description += f'{genre}, '
-
-                    description = f"{' and '.join(description[:-2].rsplit(', ', 1)) if len(genres_info) > 1 else description[:-2]}{final_sep}"
-
-                    if len(genres_info) == 1:
-                        description = description.replace('genres', 'genre')
-
-                if tracks_info:
-                    types.append('tracks')
-                    if artists_info and not genres_info:
-                        description += ', and the tracks '
-                    elif not artists_info and not genres_info:
-                        description += 'the tracks '
-
-                    if isinstance(tracks_info, dict):
-                        for song, artist in tracks_info.items():
-                            description += f'{song} by {artist}, '
-
-                        tracks = [
-                            requests.get_request(
-                                headers=self.__headers,
-                                url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1',
-                            ).json()['tracks']['items'][0]['id']
-                            for song, artist in tracks_info.items()
-                        ]
-
-                    elif isinstance(tracks_info[0], tuple) or isinstance(tracks_info[0], list):
-                        for song, artist in tracks_info: # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
-                            description += f'{song} by {artist}, '
-                        tracks = [
-                            requests.get_request(
-                                headers=self.__headers,
-                                url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1',
-                            ).json()['tracks']['items'][0]['id']
-                            for song, artist in tracks_info # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
-                        ]
-
-                    elif isinstance(tracks_info[0], str):
-                        for song in tracks_info:
-                            description += f'{song}, '
-                        tracks = [
-                            requests.get_request(
-                                headers=self.__headers,
-                                url=f'https://api.spotify.com/v1/search?q={song}&type=track&limit=1',
-                            ).json()['tracks']['items'][0]['id']
-                            for song in tracks_info
-                        ]
-
-                    else:
-                        raise ValueError('The argument tracks_info must be an instance of one of the following 4 types: list[str], list[tuple[str]], list[list[str]], dict[str, str]')
-
-                    description = ' and '.join(description[:-2].rsplit(', ', 1)) if len(artists_info) > 1 else description[:-2]
-
-                    url += f'&seed_tracks={",".join(tracks)}'
-
-                    if len(tracks_info) == 1:
-                        description = description.replace('tracks', 'track')
-
-                if use_main_playlist_audio_features:
-
-                    audio_statistics = self.audio_features_statistics()
-
-                    min_tempo = audio_statistics['min_tempo'] * 0.8
-                    max_tempo = audio_statistics['max_tempo'] * 1.2
-                    target_tempo = audio_statistics['mean_tempo']
-                    min_energy = audio_statistics['min_energy'] * 0.8
-                    max_energy = audio_statistics['max_energy'] * 1.2
-                    target_energy = audio_statistics['mean_energy']
-                    min_valence = audio_statistics['min_valence'] * 0.8
-                    max_valence = audio_statistics['max_valence'] * 1.2
-                    target_valence = audio_statistics['mean_valence']
-                    min_danceability = audio_statistics['min_danceability'] * 0.8
-                    max_danceability = audio_statistics['max_danceability'] * 1.2
-                    target_danceability = audio_statistics['mean_danceability']
-                    min_loudness = audio_statistics['min_loudness'] * 0.8
-                    max_loudness = audio_statistics['max_loudness'] * 1.2
-                    target_loudness = audio_statistics['mean_loudness']
-                    min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
-                    max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
-                    target_instrumentalness = audio_statistics['mean_instrumentalness']
-
-                    url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
-
-                recommendations = requests.get_request(url=url, headers=self.__headers).json()
-
-                songs = []
-
-                for song in recommendations["tracks"]:
-                    (id, name, popularity, artist), song_genres = util.song_data(song=song, added_at=False), self.__get_song_genres(song)
-                    song['id'] = id
-                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
-                    songs.append({
-                        "id": id,
-                        "name": name,
-                        "artists": artist,
-                        "popularity": popularity,
-                        "genres": song_genres,
-                        "danceability": danceability,
-                        "loudness": loudness,
-                        "energy": energy,
-                        "instrumentalness": instrumentalness,
-                        "tempo": tempo,
-                        "valence": valence
-                    })
-
-                recommendations_playlist = pd.DataFrame(data=songs)
-
-                if build_playlist:
-                    ids = recommendations_playlist['id'].tolist()
-                    types = ' and '.join(', '.join(types).rsplit(
-                        ', ', 1)) if len(types) > 1 else types[0]
-                    self.__general_recommendation_description = description
-                    self.__general_recommendation_description_types = types
-
-                    self.__write_playlist(
-                        K=K,
-                        type='general-recommendation',
-                        additional_info=ids
-                    )
-
-                return recommendations_playlist
-
-            except AccessTokenExpiredError as e:
-                logging.warning('Error due to the access token expiration')
-                auth_token = auth.get_auth()
-
-                self.__auth_token = auth_token
-
-                self.__headers['Authorization'] = f'Bearer {auth_token}'
-            else:
-                break
+        return self.playlist.get_playlist_recommendation(
+            time_range=time_range,
+            main_criteria=main_criteria,
+            save_with_date=save_with_date,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+        )
 
+    @needs_playlist
     def get_songs_by_mood(
             self,
             mood: str,
-            K: int = 50,
+            number_of_songs: int = 50,
             build_playlist: bool = False,
             exclude_mostly_instrumental: bool = False
         ) -> pd.DataFrame:
         """Function to create playlists based on the general mood of a song
 
         Args:
             mood (str): The mood of the song. Can be 'happy', 'sad' or 'calm'
-            K (int, optional): Number of songs. Defaults to 50.
+            number_of_songs (int, optional): Number of songs. Defaults to 50.
             build_playlist (bool, optional): Flag to create the playlist in the user's library. Defaults to False.
             exclude_mostly_instrumental (bool, optional): Flag to exclude the songs which are 80% or more instrumental. Defaults to False.
 
         Raises:
             ValueError: If the mood is not one of the valid options the error is raised
 
         Returns:
             pd.DataFrame: A DataFrame containing the new playlist
         """
-        if mood not in ['happy', 'sad', 'calm']: # energetic still needs work to be ready
-            raise ValueError("The mood parameter must be one of the following: 'happy', 'sad', 'calm'")
-
-        energy_threshold = 0.7
-        valence_threshold = 0.5
-        instrumentalness_threshold = 0.8
-
-        mood_queries = {
-            'sad': {
-                'ascending': True,
-                'sorting': 'energy&valence',
-                'query': 'valence < @valence_threshold and energy < @energy_threshold'
-            },
-            'calm': {
-                'ascending': True,
-                'sorting': 'energy&loudness',
-                'query': 'valence >= @valence_threshold and energy < @energy_threshold'
-            },
-            'angry': {
-                'ascending': False,
-                'sorting': 'energy&loudness',
-                'query': 'valence < @valence_threshold and energy >= @energy_threshold'
-            },
-            'happy': {
-                'ascending': False,
-                'sorting': 'energy&valence',
-                'query': 'valence >= @valence_threshold and energy >= @energy_threshold'
-            }
-        }
-
-        playlist = self.__playlist.query(mood_queries[mood]['query']).copy()
-
-        if mood_queries[mood]['sorting'] == 'energy&valence':
-            playlist['mood_index'] = playlist['energy'] + 3 * playlist['valence']
-        else:
-            playlist['mood_index'] = playlist['energy'] + 3 * playlist['loudness']
-        # this is necessary because of the moods that are not consistent in terms of the conditions applied to energy and valence, for example, happy and sad which have the same condition applied to both thresholds can use both in the sorting whereas the others can't.
-
-        if exclude_mostly_instrumental:
-            playlist = playlist.query('instrumentalness <= @instrumentalness_threshold')
-
-        playlist = playlist.sort_values(by='mood_index', ascending=mood_queries[mood]['ascending'])
-
-        if len(playlist) >= K:
-            playlist = playlist[:K]
-        else:
-            K = len(playlist)
-            logging.warning(f'The playlist does not contain {K} {mood} songs. Therefore there are only {len(playlist)} in the returned playlist. ')
-
-        if build_playlist:
-
-            for _ in range(2):
-                try:
-                    self.__mood = mood
-                    self.__exclude_mostly_instrumental = exclude_mostly_instrumental
-                    ids = playlist['id'].tolist()
-
-                    self.__write_playlist(
-                        K=K,
-                        type=f'mood',
-                        additional_info=ids
-                    )
-
-                except AccessTokenExpiredError as e:
-                    logging.warning('Error due to the access token expiration')
-                    auth_token = auth.get_auth()
-
-                    self.__auth_token = auth_token
-
-                    self.__headers['Authorization'] = f'Bearer {auth_token}'
-                else:
-                    break
-
-        return playlist
-
+        return self.playlist.get_songs_by_mood(
+            mood=mood,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+            exclude_mostly_instrumental=exclude_mostly_instrumental
+        )
 
+    @needs_playlist
     def playlist_songs_based_on_most_listened_tracks(
             self,
-            K: int = 50,
+            number_of_songs: int = 50,
             build_playlist: bool = False,
             time_range: str = 'short_term',
-        ) -> Union[pd.DataFrame, None]:
+        ) -> pd.DataFrame:
         """Function to create a playlist with songs from the base playlist that are the closest to the user's most listened songs
 
         Args:
-            K (int, optional): Number of songs. Defaults to 50.
+            number_of_songs (int, optional): Number of songs. Defaults to 50.
             build_playlist (bool, optional): Flag to create the playlist in the user's library. Defaults to False.
             time_range (str, optional): String to identify which is the time range, could be one of the following: {'short_term', 'medium_term', 'long_term'}. Defaults to 'short_term'.
 
         Raises:
             ValueError: time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'
 
         Returns:
-            Union[pd.DataFrame, None]: DataFrame that contains the information of all songs in the new playlist
+            pd.DataFrame: DataFrame that contains the information of all songs in the new playlist
         """
-        if time_range not in {'short_term', 'medium_term', 'long_term'}:
-            raise ValueError("time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'")
-
-        for _ in range(2):
-            try:
-
-                top_50 = requests.get_request(url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}&limit=50', headers=self.__headers).json()
-
-                top_50 = [
-                    {
-                        'id': song['id'],
-                        'name': song['name'],
-                        'genres': self.__get_song_genres(song),
-                        'artists': [artist['name'] for artist in song['artists']],
-                        'popularity': song['popularity']
-                    }
-                    for song in top_50['items']
-                ]
-
-                for song in top_50:
-                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
-
-                    song.update({ # not using **song because the id isnt needed
-                        'danceability': danceability,
-                        'loudness': loudness,
-                        'energy': energy,
-                        'instrumentalness': instrumentalness,
-                        'tempo': tempo,
-                        'valence': valence,
-                    })
-
-
-                most_listened_recommendation = {
-                    'id': "UNOFFICIAL_ID",
-                    'name': f"{time_range.replace('_', ' ').capitalize()} Most Listened",
-                    'genres': list(reduce(lambda acc, x: acc + x['genres'], top_50, [])),
-                    'artists': list(reduce(lambda acc, x: acc + x['artists'], top_50, [])),
-                    'popularity': int(round(reduce(lambda acc, song: acc + int(song['popularity']), top_50, 0) / len(top_50))),
-                    'genres_indexed': self.__get_genres([util.item_list_indexed(song['genres'], all_items=self.__all_genres) for song in top_50]),
-                    'artists_indexed': self.__get_artists([util.item_list_indexed(song['artists'], all_items=self.__all_artists) for song in top_50]),
-                }
-
-                for audio_feature in ['danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']:
-                    most_listened_recommendation[audio_feature] = float(reduce(lambda acc, song: acc + float(song[audio_feature]), top_50, 0) / len(top_50))
-
-                song_dict = [*self.__song_dict, most_listened_recommendation]
-
-                playlist = self.__get_recommendations(type=time_range.split('_')[0], info=song_dict, K=K)
-
-                if build_playlist:
-                    ids = playlist['id'].tolist()
-                    self.__most_listened_recommendation_time_range = time_range
-
-                    self.__write_playlist(
-                        K=K,
-                        type=f'most-listened-recommendation',
-                        additional_info=ids
-                    )
-
-                return playlist
-
-            except AccessTokenExpiredError as e:
-                logging.warning('Error due to the access token expiration')
-                auth_token = auth.get_auth()
-
-                self.__auth_token = auth_token
-
-                self.__headers['Authorization'] = f'Bearer {auth_token}'
-
+        return self.playlist.playlist_songs_based_on_most_listened_tracks(
+            time_range=time_range,
+            build_playlist=build_playlist,
+            number_of_songs=number_of_songs,
+        )
 
+    def update_all_generated_playlists(
+            self, *,
+            playlist_types_to_update: Union['list[str]', None] = None,
+            playlist_types_not_to_update: Union['list[str]', None] = None
+        ) -> None:
+        """Update all package generated playlists in batch
 
+        Arguments:
+            playlist_types_to_update (list[str], optional, keyword-argument): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all == ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood', 'most-listened-recommendation'].
+            playlist_types_not_to_update (list[str], optional, keyword-argument): List of playlist types not to update. For example, if you want to update all playlists but song-related playlists use this argument as ['song-related']. it can be used alongside with the playlist_types_to_update but it can become confusing or redundant. Defaults to none == [].
+        """
+        self.user.update_all_generated_playlists(
+            base_playlist=getattr(self, 'playlist', None),
+            playlist_types_to_update=playlist_types_to_update,
+            playlist_types_not_to_update=playlist_types_not_to_update,
+        )
 
-def start_api(user_id: str, *, playlist_url: Union[str, None] = None, playlist_id: Union[str, None] = None, liked_songs: bool = False, log_level: str = 'INFO', prepare_favorites: bool = False):
+def start_api(
+    user_id: str, *,
+    log_level: str = 'INFO',
+    liked_songs: bool = False,
+    playlist_url: Union[str, None] = None,
+    playlist_id: Union[str, None] = None,
+) -> SpotifyAPI:
     """Function that prepares for and initializes the API
 
     Note:
         Internet Connection is required
 
     Args:
         user_id(str): the id of user, present in the user account profile
 
     Keyword Arguments:
-        playlist_url(str, optional, keyword-argument only): the url for the playlist, which is visible when trying to share it. Defaults to False.
+        playlist_url (str, optional, keyword-argument only): the url for the playlist, which is visible when trying to share it. Defaults to False.
         playlist_id (str, optional, keyword-argument only): the id of the playlist, an unique big hash which identifies the playlist. Defaults to False.
         liked_songs (bool, optional, keyword-argument only): A flag to identify if the playlist to be mapped is the Liked Songs. Defaults to False.
-        prepare_favorites (bool, optional, keyword-argument only): A flag to identify if the Short and Medium term favorite playlists will be calculated. IMPORTANT to note that both are DEPRECATED. Defaults to False.
+        log_level (str, optional, keyword-argument only): The log level, of the logging library, to be used. Defaults to INFO
 
     Raises:
-        ValueError: at least one of the playlist related arguments have to be specified
-        ValueError: when asked to input the auth token, in case it is not valid, an error is raised
-        ValueError: when passing the arguments, there should be only one filled between playlist_url, playlist_id and liked_songs
+        ValueError: when passing the arguments, there should be only one or none filled between playlist_url, playlist_id and liked_songs
 
     Returns:
         SpotifyAPI: The instance of the SpotifyAPI class
-
-    Note:
-    Although both the playlist_url and playlist_id are optional, informing at least one of them is required, though the choice is up to you
     """
     if log_level.upper() not in ['DEBUG', 'INFO', 'WARNING', 'ERROR']:
         raise ValueError("log_level must be one of the following: 'DEBUG', 'INFO', 'WARNING', 'ERROR'")
 
     logging.basicConfig(
         level=log_level.upper(),
         datefmt='%Y-%m-%d %H:%M:%S',
         format='%(asctime)s.%(msecs)03d - %(levelname)s: %(message)s',
     )
 
-    if playlist_url is None and playlist_id is None and not liked_songs:
-        raise ValueError('It is necessary to specify a playlist either with playlist id or playlist url or flag the liked_songs as True')
-    if (playlist_url is not None or playlist_id is not None) and liked_songs:
-        raise ValueError('It is necessary to specify only one of the following parameters: playlist_id or playlist_url or liked_songs')
+    if (playlist_url is not None or playlist_id is not None) and liked_songs or (playlist_url is not None and playlist_id is not None):
+        raise ValueError('It is necessary to specify only one or none of the following parameters: playlist_id or playlist_url or liked_songs')
 
     logging.info('Retrieving Authentication token')
 
-    auth_token = f'Bearer {auth.get_auth()}'
+    RequestHandler.get_auth()
+    logging.debug('Authentication complete')
 
-    return SpotifyAPI(auth_token=auth_token, playlist_id=playlist_id, user_id=user_id, playlist_url=playlist_url, liked_songs=liked_songs, prepare_favorites=prepare_favorites)
+    return SpotifyAPI(playlist_id=playlist_id, user_id=user_id, playlist_url=playlist_url, liked_songs=liked_songs)
```

## spotify_recommender_api/util.py

```diff
@@ -1,16 +1,15 @@
 import logging
 import warnings
 import datetime
 import functools
-import pandas as pd
-import spotify_recommender_api.request_handler as requests
 
 from dateutil import tz
-from typing import Union, Any
+from typing import Any, Callable
+from spotify_recommender_api.requests.api_handler import PlaylistHandler
 
 
 def playlist_url_to_id(url: str) -> str:
     """Extracts the playlist id from it's URL
 
     Args:
         url (str): The playlist public url
@@ -18,147 +17,42 @@
     Returns:
         str: The Spotify playlist Id
     """
     uri = url.split('?')[0]
 
     return uri.split('open.spotify.com/playlist/')[1]
 
-
-def get_total_song_count(playlist_id: str, headers: dict) -> int:
-    """Function returns the total number of songs in the playlist
-
-    Args:
-        playlist_id (str): The Spotify playlist Id
-        headers (dict): The request headers, containing the auth information
-
-    Returns:
-        int: The total number of songs in the playlist
-    """
-
-    if playlist_id == 'liked_songs':
-        return requests.get_request(headers=headers, url='https://api.spotify.com/v1/me/tracks').json()['total']
-
-
-    playlist_res = requests.get_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}', headers=headers)
-
-    return playlist_res.json()["tracks"]["total"]
-
-
-def song_data(song: 'dict[str, Any]', added_at: bool = True) -> 'list[Union[str, float, list[str], datetime.datetime]]':
-    """Function that gets additional information about the song, like its name, artists, id, popularity, date when it was added to the playlist, etc.
-
-    Args:
-        song (dict[str, dict[str, str]]): The song dictionary fetched from the Spotify API
-
-    Returns:
-        list[str, str, float, list[str], datetime.datetime]: A list containing the song's information
-    """
-    try:
-        data = [song["track"]['id'], song["track"]['name'], song["track"]['popularity'], [artist["name"] for artist in song["track"]["artists"]]]
-    except KeyError:
-        data = [song['id'], song['name'], song['popularity'], [artist["name"] for artist in song["artists"]]]
-
-    if added_at:
-        data.append(song['added_at'])
-
-    return data
-
-
 def item_list_indexed(items: 'list[str]', all_items: 'list[str]') -> 'list[str]':
     """Function that returns the list of items, mapped to the overall list of items, in a binary format
     Useful for the overall execution of the algorithm which determines the distance between each song
 
     Args:
         items (list[str]): list of items for a given song
         all_items (list[str]): all the items inside the entire playlist
 
     Returns:
         list[int]: indexed list of items in binary format in comparison to all the items inside the playlist
     """
 
     return [str(int(all_genres_x in items)) for all_genres_x in all_items]
 
-
-def playlist_exists(name: str, base_playlist_name: str, headers: dict, _update_created_playlists: bool = False) -> Union['tuple[str, str, str]', 'tuple[()]']:
-    """Function used to check if a playlist exists inside the user's library
-    Used before the creation of a new playlist
-
-    Args:
-        name (str): name of the playlist being created, which could easily be bypassed, if the playlist names were not made automatically
-        base_playlist_name (str): name of the base playlist
-        headers (dict): Request headers
-
-    Returns:
-        str|bool: If the playlist already exists, returns the id of the playlist, otherwise returns False
-    """
-    total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=1', headers=headers).json()['total']
-    playlists = []
-    for offset in range(0, total_playlist_count, 50):
-        request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=headers).json()
-
-        playlists += [(playlist['id'], playlist['name'], playlist['description']) for playlist in request['items']]
-
-    return next(
-        (
-            playlist for playlist in playlists
-            if (
-                playlist[1] == name or
-                (
-                    name.lower().startswith('profile short term recommendation') and
-                    playlist[1] == name.replace('Short term ', '')
-                )
-            ) and
-            (
-                ' Term Most-listened Tracks' in name or
-                f', within the playlist {base_playlist_name}' in playlist[2] or
-                _update_created_playlists or
-                'Recommendation (' in name
-            )
-        ),
-        ()
-    )
-
-
-
-def query_audio_features(song: Union[pd.Series, 'dict[str, Any]'], headers: dict) -> 'list[float]':
-    """Queries the audio features for a given song and returns the ones that match the recommendations within this package
-
-    Args:
-        song (pd.Series | dict[str, Any]): song containing its base information
-        headers (dict): Request headers
-
-    Returns:
-        list[float]: list with the audio features for the given song
-    """
-
-    song_id = song['id']
-
-    audio_features = requests.get_request(
-        url=f'https://api.spotify.com/v1/audio-features/{song_id}',
-        headers=headers
-    ).json()
-
-    return [audio_features['danceability'], audio_features['loudness'] / -60, audio_features['energy'], audio_features['instrumentalness'], audio_features['tempo'], audio_features['valence']]
-
-
 def get_datetime_by_time_range(time_range: str = 'all_time') -> datetime.datetime:
     """Calculates the datetime that corresponds to the given time range before the current date
 
     Args:
         time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
 
     Raises:
         ValueError: If the time_range parameter is not valid the error is raised.
 
     Returns:
         datetime.datetime: Datetime of the specified time_range before the current date
     """
     if time_range not in ['all_time', 'month', 'trimester', 'semester', 'year']:
-        raise ValueError(
-            'time_range must be one of the following: "all_time", "month", "trimester", "semester", "year"')
+        raise ValueError('time_range must be one of the following: "all_time", "month", "trimester", "semester", "year"')
 
     now = datetime.datetime.now(tz=tz.gettz('UTC'))
     date_options = {
         'all_time': datetime.datetime(year=2000, month=1, day=1, hour=0, minute=0, second=0, microsecond=0, tzinfo=tz.gettz('UTC')),
         'month': now - datetime.timedelta(days=30),
         'trimester': now - datetime.timedelta(days=90),
         'semester': now - datetime.timedelta(days=180),
@@ -200,15 +94,14 @@
         key: {
             'value': value,
             'percentage': round(value / dictionary['total'], 5)
         }
         for key, value in dictionary.items()
     }
 
-
 def print_base_caracteristics(*args):
     """
     Function that receives a list of values and print them
 
     Args:
         name (str): name of the song
         artists (list[str]): song's artists
@@ -218,52 +111,49 @@
         loudness (float): song's loudness
         energy (float): song's energy
         instrumentalness (float): song's instrumentalness
         tempo (float): song's tempo
         valence (float): song's valence
 
     """
-    name, genres, artists, popularity, danceability, loudness, energy, instrumentalness, tempo, valence = args
+    id, name, genres, artists, popularity, danceability, loudness, energy, instrumentalness, tempo, valence = args
 
+    logging.info(f'{id = }')
     logging.info(f'{name = }')
     logging.info(f'{artists = }')
     logging.info(f'{genres = }')
     logging.info(f'{popularity = }')
     logging.info(f'{danceability = }')
     logging.info(f'{loudness = }')
     logging.info(f'{energy = }')
     logging.info(f'{instrumentalness = }')
     logging.info(f'{tempo = }')
     logging.info(f'{valence = }')
 
 
-def get_base_playlist_name(playlist_id: str, headers: dict) -> str:
+def get_base_playlist_name(playlist_id: str) -> str:
     """Returns the base playlist name given the playlist id
 
     Args:
         playlist_id (str): The Spotify playlist id
-        headers (dict): Request headers
 
     Returns:
         str: The base playlist name
     """
 
-    playlist = requests.get_request(
-        url=f'https://api.spotify.com/v1/playlists/{playlist_id}',
-        headers=headers
-    ).json()
+    playlist = PlaylistHandler.playlist_details(playlist_id)
 
-    return playlist['name']
+    return playlist.json()['name']
 
 
-def deprecated(func):
+def deprecated(func: Callable[..., Any]) -> Callable[..., Any]:
     """This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used."""
 
     @functools.wraps(func)
-    def new_func(*args, **kwargs):
+    def new_func(*args, **kwargs) -> Any:
         warnings.simplefilter('always', DeprecationWarning)  # turn off filter
         warnings.warn(f"Call to deprecated function {func.__name__}.", category=DeprecationWarning, stacklevel=2)
         warnings.simplefilter('default', DeprecationWarning)  # reset filter
         return func(*args, **kwargs)
     return new_func
```

## Comparing `spotify_recommender_api/server.py` & `spotify_recommender_api/server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import uvicorn
 import threading
 import webbrowser
 import contextlib
 
 from fastapi import FastAPI, status
 from fastapi.responses import HTMLResponse
-from spotify_recommender_api.sensitive import CLIENT_ID, CLIENT_SECRET
-from spotify_recommender_api.request_handler import post_request_with_auth
+from spotify_recommender_api.requests.auth_handler import AuthHandler
+from spotify_recommender_api.server.sensitive import CLIENT_ID, CLIENT_SECRET
 
 app = FastAPI()
 
 redirect_uri = 'http://localhost:8000/callback'
 scope = ["playlist-modify-private", "playlist-read-private", "user-library-read", "user-library-modify", "user-top-read"]
 
+
 class Server(uvicorn.Server):
     """Subclass of uvicorn.Server so that the run and shutdown methods can be done while running in a separate thread
 
     """
     def install_signal_handlers(self):
         pass
 
@@ -32,49 +33,46 @@
             while not self.started:
                 time.sleep(1e-3)
             yield
         finally:
             self.should_exit = True
             thread.join()
 
-
 def up_server():
     """Function to start the fastapi server and wait for the callback request from spotify to complete, to get the access token the shutdown the server
     """
     config = uvicorn.Config(app=app, host="127.0.0.1", port=8000)
     server = Server(config=config)
 
     with server.run_in_thread():
         webbrowser.open_new_tab('http://localhost:8000/')
         while True:
             try:
                 with open('./.spotify-recommender-util/execution-status.txt', 'r') as f:
                     auth_status = f.readline()
-            except Exception as e:
-                pass
+            except FileNotFoundError as e:
+                time.sleep(0.5)
             else:
                 break
 
 def get_access_token(auth_code: str) -> str:
     """Funciton to request for the access token request
 
     Args:
         auth_code (str): Temporary code to have access to the access token
 
     Returns:
         str: Access token
     """
-    response = post_request_with_auth(
-        "https://accounts.spotify.com/api/token",
-        auth=(CLIENT_ID, CLIENT_SECRET), # type: ignore
-        data={
-            "grant_type": "authorization_code",
-            "code": auth_code,
-            "redirect_uri": redirect_uri,
-        },
+
+    response = AuthHandler.authorization_token(
+        auth_code=auth_code,
+        client_id=CLIENT_ID,
+        redirect_uri=redirect_uri,
+        client_secret=CLIENT_SECRET
     )
 
     return response.json()["access_token"]
 
 @app.get("/", status_code=status.HTTP_200_OK)
 async def auth():
     """Primary function to request for the auth code to get the token later on
```

## Comparing `spotify_recommender_api-4.5.0.dist-info/METADATA` & `spotify_recommender_api-5.0.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 4.5.0
+Version: 5.0.0
 Summary: Python package which takes the songs of a greater playlist as starting point to make recommendations of groups of songs that might bond well within that same playlist, using K-Nearest-Neighbors Technique
 Home-page: https://github.com/nikolas-virionis/spotify-api
 Author: Nikolas B Virionis
 Author-email: nikolas.virionis@bandtec.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,103 +16,186 @@
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: seaborn
 Requires-Dist: uvicorn
 
 
 # spotify-recommender
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-recommender-api?style=plastic)
-![PyPI](https://img.shields.io/pypi/v/spotify-recommender-api?style=plastic)
 ![GitHub repo size](https://img.shields.io/github/repo-size/nikolas-virionis/spotify-api)
 ![GitHub last commit](https://img.shields.io/github/last-commit/nikolas-virionis/spotify-api?style=plastic)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-recommender-api?style=plastic)
+![PyPI](https://img.shields.io/pypi/v/spotify-recommender-api?style=plastic)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/spotify-recommender-api?style=plastic)<br>
 
 <img src='./readme-pictures/Spotify Logo.png' width='60%'>
 
-- [Use Case](#use-case)
-- [Setup](#setup)
-- [Methods](#methods)
-- [Suggestions](#suggestions)
-- [Packages used](#packages-used)
+- [spotify-recommender](#spotify-recommender)
+  - [Use Case](#use-case)
+  - [Setup](#setup)
+    - [Requirements:](#requirements)
+    - [Starting the api](#starting-the-api)
+  - [Methods](#methods)
+  - [Suggestions](#suggestions)
 - [OG Scripts](#og-scripts)
-- [Contribution Rules](#contributing)
+    - [Context](#context)
+    - [Variations](#variations)
+    - [DISCLAIMER](#disclaimer)
+- [Packages used](#packages-used)
+- [Contributing](#contributing)
+  - [PR Template](#pr-template)
+  - [Commits](#commits)
 
 
 ## Use Case
- - This is the first section of this readme, because, you will see, this package can help, but nothing is perfect, so it will, as long as you fit in this particular use case ;(
- - The perfect use case for this is that in one playlist (or more) you put a bunch of songs in different times and mood styles, and when you listen to it, you feel like only listening to a part of it, some days later, that part is useless, but some other part is awesome. The big issue here is that those "parts" are shuffled, all across the playlist. Then how would one find those songs they crave, today, tomorrow, and later? Speaking from experience, it is not worth it to map manually a 1000-song playlist and filter out 50, or 100 of them.
- - This package comes to solve this issue, roughly, because it tries to find the K (number) nearest songs taking into consideration genres, artists, popularity, and some audio features, such as danceability, energy, instrumentalness, tempo, and valence, using the KNN supervised machine learning technique to find the closest songs to some threshold.
- - One issue with this is that Spotify API is not the best, E.g. A LOT of artists do not have any genre associated with them, which, as justified in the next topic, is the main source of genre information used
- - Another issue is that Spotify API does not provide, at the time of publication of version 3.5.2, either song or album genres, which compromises a portion of the accuracy of the recommendations.  Still, I recommend you give it a try
-
+ - This is the first section of this readme, because, you will see, that this package can help, but nothing is perfect, so it will, as long as you fit in the use cases ;(
+ - There are more general recommendation features, such as profile, playlist and general recommendations, but also there are a few other features which would have the perfect use case as the one that has one playlist (or more) where you put a lot of songs in different times and mood styles, and when you listen to it, you feel like only listening to a part of it, some days later, that part is useless, but some other part is awesome. The big issue here is that those "parts" are shuffled, all across the playlist. Then how would one find those songs they crave, today, tomorrow, and later? Speaking from experience, it is not worth it to map manually a 1000-song playlist and filter out 50 or 100 of them.
+ - This package comes to solve this issue, roughly, because it tries to find the nearest songs taking into consideration genres, artists, popularity, and some audio features, such as danceability, energy, instrumentalness, tempo, and valence, using an adaptation of the KNN supervised machine learning technique to find the closest songs to some threshold.
+ - One issue with this is that Spotify API is not perfect, E.g. a lot of artists do not have any genre associated with them, which, as justified in the next topic, is the main source of genre information used
+ - Another issue is that Spotify API does not provide, at the time of publication of version 5.0.0, neither song nor album genres, which compromises a portion of the accuracy of the recommendations. Still, I recommend you give it a try since because of the use of all other variables, it has a decent to good accuracy.
 
 
 
 ## Setup
 
 ### Requirements:
   - Python installed<br>
- The ideal version, to run the package is 3.8.x, the version on top of which the package was built, older versions may have some issues, as the package uses a handful of other packages and their versions may conflict.
+ The ideal version, to run the package is 3.8.x, the version on top of which the package was built, newer version should be fine and older versions may have some issues, as the package uses a handful of other packages, and python features, and their versions may conflict.
   - Network Connection<br>
  So that a wide range of songs can be analyzed, it is imperative to have a network connection, at least for the first time executing a script using this package.
-  - <strong>A fitting playlist</strong><br>
- The perfect use case for this package is that of one big playlist (200+ songs), which you feel like listening to some of them, then others, but never, or rarely, all of them, since they belong to different genres/styles.
+  - A fitting playlist<br>
+ For the playlist related features, the perfect use case for this package is that of one big playlist (200+ songs), which you feel like listening to some of them, then others, but never, or rarely, all of them, since they belong to different genres/styles.
   - ## <strong>Patience</strong>
-    It may seem funny or a joke, but the first mapping process of the playlist to a local pandas DataFrame... it will take a good while, up to 2.5 to 3 seconds per song, at 20-40Mbps Internet connection, being in Latam. All these factors play a part in the time for it to the first load.
-    Just to make it clear, CPU, ram, sdd, etc., will not help much, the issue is to have up to 7 different HTTP requests per song, which make this take so long.
+    It may seem funny or a joke, but if one wants to use any playlist related features, the first mapping process of the playlist to a local pandas DataFrame... it will take a good while, up to 2.5 to 3 seconds per song, at 20-40Mbps Internet connection, being in Latam. All these factors play a part in the time for it to the first load.
+    Just to make it clear, CPU, ram, sdd, etc., will not help much, the issue is to have up to 7 different HTTP requests per song, to retrieve all information needed, which makes this take so long.
     Besides, as of July/2022, Spotify implemented a possible API Response: ["429: Too Many Requests"](https://http.cat/429) which forced this package to implement [Exponential Backoff](https://en.wikipedia.org/wiki/Exponential_backoff) to complete its requests, therefore what already took a while, now takes a little bit more
   - Jupyter Notebook<br>
- Not exactly a requirement but it is advised that a Jupyter notebook is used (even more recommended to use the vscode extension for Jupyter notebooks) because it is important, or at least more comfortable, to have the variable still in memory and then decide how to use it, without having to run a script multiple times, having to reconnect to Spotify, redownload the playlist, redo some computations, etc.
+ Not exactly a requirement but it is advised that a Jupyter notebook is used (even more recommended to use the vscode extension for Jupyter notebooks) because it is important, or at least more comfortable, to have the variable still in memory and then decide how to use it, without having to run and rerun a script multiple times, having to reconnect to Spotify, redownload the playlist, redo some computations, etc.
   - Spotify access<br>
  I mean, you knew that already, right?
 
   - ### Installing the package<br>
 ~~~ps1
 pip install spotify-recommender-api
 ~~~
 
 
   - ### Importing the package<br>
 
-Firstly, it's necessary to import the method start_api from the package spotify_recommender_api.recommender:
+Firstly, it's necessary to import the method start_api from the package spotify_recommender_api:
  ~~~ python
- from spotify_recommender_api.recommender import start_api
+ from spotify_recommender_api import start_api
  ~~~
 
 ### Starting the api
   - Gathering the initial information: (playlist_url, user_id)<br>
+  - The only mandatory parameter is user_id. If the user wants to use the playlist related features, they need to provide a playlist either on the start_api function or the api.select_playlist method.
 
   --- Playlist URL: The playlist URL is available when right-clicking the playlist name / or going to the three dots that represent the playlist options <br>
   --- Playlist ID: The playlist id is available as the hash string between the last '/' in and the '?' in the playlist url<br>
   <img src='./readme-pictures/Playlist Configs.png' width='25%'><br>
   --- User ID: The user id is available when clicking the account, and accessing its information, on Spotify's website<br>
   <img src='./readme-pictures/Account.png' width='25%'><br>
   --- Liked Songs: A flag to pass in case the playlist you want to use is your profile Liked Songs <br>
   --- Log level: the logging package log level. Defaults to INFO, but can be DEBUG, INFO, WARNING and ERROR
 
   - Calling the function:
 ~~~python
-api = start_api(playlist_url='<PLAYLIST_URL>', user_id='<USER_ID>')
+api = start_api(user_id='<USER_ID>')
 ~~~
 Or
 ~~~python
-api = start_api(playlist_id='<PLAYLIST_ID>', user_id='<USER_ID>')
+api = start_api(user_id='<USER_ID>', playlist_url='<PLAYLIST_URL>')
 ~~~
 Or
 ~~~python
-api = start_api(liked_songs=True, user_id='<USER_ID>', log_level='DEBUG')
+api = start_api(user_id='<USER_ID>', playlist_id='<PLAYLIST_ID>')
 ~~~
-Though, to be honest, it is easier and more convenient to use the playlist URL or the liked_songs flag
+Or
+~~~python
+api = start_api(user_id='<USER_ID>', liked_songs=True)
+~~~
+Though, to be honest, it is easier and more convenient to use either the playlist URL or the liked_songs flag
 
   - Getting the Auth Token:
-  It is a hash token that expires 60 minutes after it is generated, and after April 22nd, 2023 it has been fully refactored, due to a change in the Spotify API Authentication methods, which invalidated the previous way. Now As soon as you call the start_api to function a fast API server will be launched in port 8000.<br>
+  It is a hash token that expires 60 minutes after it is generated, and after April 22nd, 2023 it has been fully refactored, due to a change in the Spotify API Authentication methods, which invalidated the previous way.
+  Now As soon as you call the start_api to function a fast API server will be launched in port 8000.<br>
   Also there will be a web browser opened so that the user can click on the button Authorize, log in with their Spotify account, and then, the authentication is completed for that usage of the package.
+  After version 5.0.0 (July 15th, 2023), within this 60 minute period, the Access token will be "cached" locally for faster access, and after this 60 minute period, there are two things that can happen. If no function was running, nothing will happen, and the next time any function is called, it will be necessary to login again. Or if there is a function running, the access token expired error will be caught, and automatically the fast API server will be launched again, so that the user can reauthenticate, and automatically after the authentication the function which was running will continue from where it left off.
 
 
 ## Methods
+ - select_playlist
+~~~python
+# Parameters
+select_playlist(
+    playlist_id: str = None,
+    playlist_url: str = None,
+    liked_songs: bool = False
+)
+# Method Use Example
+api.select_playlist(liked_songs=True)
+# Function to select a playlist to be mapped and be available on all the playlist-related recommendation
+# functions on an already existing authentication context
+~~~~~~
+ - get_most_listened
+~~~python
+# Parameters
+get_most_listened(
+    number_of_songs: int = 50,
+    build_playlist: bool = False,
+    time_range: str = 'long_term',
+)
+# Method Use Example
+api.get_most_listened(time_range='short_term', number_of_songs=50)
+# Function that returns the pandas DataFrame representing the
+# given the time range most listened to tracks playlist
+# No parameters are mandatory but the default values should be noted
+# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
+~~~
+ - get_profile_recommendation
+~~~python
+# Parameters
+get_profile_recommendation(
+    number_of_songs: int = 50,
+    main_criteria: str = 'mixed',
+    save_with_date: bool = False,
+    build_playlist: bool = False,
+    time_range: str = 'short_term'
+)
+# Method Use Example
+api.get_profile_recommendation(number_of_songs=50, main_criteria='tracks')
+# Function that returns a pandas DataFrame with profile-based recommendations, and creates it in the user account
+# main_criteria is the base info to get the recommendations
+# save_with_date is a flag to save the recommendations as a playlist at a point in time Snapshot
+# time_range refers to the range from the profile information that will be used to get the recommendation
+# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
+~~~
+ - get_general_recommendation
+~~~python
+# Parameters
+get_general_recommendation(
+    number_of_songs: int = 50,
+    genres_info: list[str] = [],
+    artists_info: list[str] = [],
+    build_playlist: bool = False,
+    use_main_playlist_audio_features: bool = False,
+    tracks_info: list[str] | list[tuple[str, str]] | list[list[str]] | dict[str, str] = [],
+)
+# Method Use Example
+api.get_general_recommendation(
+    build_playlist=True,
+    genres_info=['rap'],
+    artists_info=['NF', 'Logic'],
+    tracks_info={'Clouds': 'NF'},
+)
+# Function that returns a pandas DataFrame with artists, genres, and/or tracks-based recommendations, and creates it in the user account
+# genres_info, artists_info, and tracks_info are the lists of information that the recommendation would be based on, and the sim of their lengths must not surpass 5.
+# use_main_playlist_audio_features is the flag to indicate if the playlist-provided audio features will be used as the target for a better recommendation, BUT IT ONLY IS ALLOWED WHEN THE USER PASSED A PLAYLIST, OTHERWISE IT WILL RAISE AN ERROR.
+# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
+~~~~~~
  - get_playlist
 ~~~python
 # Method Use Example
 api.get_playlist()
 # Function that returns the pandas DataFrame representing the base playlist
 ~~~
  - playlist_to_csv
@@ -121,252 +204,251 @@
 api.playlist_to_csv()
 # Function that creates a CSV format file containing the items in the playlist
 # Especially useful when re-running the script without having changed the playlist
 ~~~
  - get_recommendations_for_song
 ~~~python
 # Parameters
-get_recommendations_for_song(song: str, K: int, with_distance: bool, generate_csv: bool,
-                        generate_parquet: bool, build_playlist: bool, print_base_caracteristics: bool)
-# Method Use Example
-api.get_recommendations_for_song(song='<SONG_NAME>', K=50)
+get_recommendations_for_song(
+    song_name: str,
+    artist_name: str,
+    with_distance: bool,
+    build_playlist: bool,
+    number_of_songs: int,
+    print_base_caracteristics: bool
+)
+# Method Use Example
+api.get_recommendations_for_song(
+    number_of_songs=50,
+    song_name='<SONG_NAME>',
+    artist_name='<ARTIST_NAME>'
+)
 # Function that returns the pandas DataFrame representing the
 # given song recommendation playlist
-# The 'song' and 'K' parameters are mandatory and the rest is
+# The 'song_name', 'artist_name' and 'number_of_songs' parameters are mandatory and the rest is
 # defaulted to False
 # The "distance" is a mathematical value with no explicit units, that is
 # used by the algorithm to find the closest songs
 # print_base_caracteristics will display the parameter song information
 # Note that it can be used to update a playlist if the given song already
-# Has its playlist generated by this package
-# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
-~~~
- - get_most_listened
-~~~python
-# Parameters
-get_most_listened(time_range: str = 'long', K: int = 50, build_playlist: bool = False)
-# Method Use Example
-api.get_most_listened(time_range='short', K=53)
-# Function that returns the pandas DataFrame representing the
-# given the time range most listened to tracks playlist
-# No parameters are mandatory but the default values should be noted
+# has its playlist generated by this package
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
- - update_all_generated_playlists
-### WILL CHANGE THE USER'S LIBRARY DRASTICALLY
-~~~python
-# Parameters
-update_all_generated_playlists(K: int = None, playlist_types_to_update: list[str] = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'], playlist_types_not_to_update: list[str] = [])
-# Method Use Example
-api.update_all_generated_playlists()
-# or for example api.update_all_generated_playlists(playlist_types_to_update=['playlist-recommendation'])
-# Function updates all the playlists once generated by this package in batch
-# Note that if only a few updates are preferred, the methods above are a better fit
-# No parameters are mandatory but the default values should be noted, and if a value for K
-# is not specified, it takes as default the already existing playlist total song count which is recommended,
-~~~
  - get_playlist_trending_genres
 ~~~python
 # Parameters
 get_playlist_trending_genres(time_range: str = 'all_time', plot_top: int|bool = False)
 # Method Use Example
 api.get_playlist_trending_genres()
 # Function that returns a pandas DataFrame with all genres within the playlist and both their
 # overall appearance and the percentage of their appearance over the entire playlist
 # in the given time_range
-# Setting the plot_top parameter to one of the following [5, 10, 15] will plot a barplot
+# Setting the plot_top parameter to any integer less tha or equal to 30 will plot a barplot with that many top genres
 # With this number of the most listened genres in the playlist
 ~~~
  - get_playlist_trending_artists
 ~~~python
 # Parameters
 get_playlist_trending_artists(time_range: str = 'all_time', plot_top: int|bool = False)
 # Method Use Example
 api.get_playlist_trending_artists()
 # Function that returns a pandas DataFrame with all artists within the playlist and both their
 # overall appearance and the percentage of their appearance over the entire playlist
 # in the given time_range
-# Setting the plot_top parameter to one of the following [5, 10, 15] will plot a barplot
+# Setting the plot_top parameter to any integer less tha or equal to 30 will plot a barplot with that many top artists
 # With this number of the most listened artists in the playlist
 ~~~
- - artist_specific_playlist
+ - artist_only_playlist
 ~~~python
 # Parameters
-artist_specific_playlist(artist_name: str, K: int = 50, complete_with_similar: bool = False, build_playlist: bool = False, ensure_all_artist_songs: bool = True, print_base_caracteristics: bool = False, with_distance: bool = False)
-# Method Use Example
-api.artist_specific_playlist(artist_name='Joyner Lucas', K=50, complete_with_similar=True, print_base_caracteristics=True, build_playlist=True)
-# Function that returns a pandas DataFrame with all songs from a specific artist within the playlist
-# and can complete that new playlist with the closest songs to that artist, and create it in the user account
-# complete_with_similar is a Flag that indicates if the playlist will be completed with the closet songs related to the artist or only their songs
-# The ensure_all_artist_songs Flag serves the purpose of making sure all the artist's songs are present in a "This is" type playlist, regardless of the K value.
+artist_only_playlist(
+    artist_name: str,
+    number_of_songs: int = 50,
+    build_playlist: bool = False,
+    ensure_all_artist_songs: bool = True
+)
+# Method Use Example
+api.artist_only_playlist(
+    number_of_songs=50,
+    build_playlist=True,
+    artist_name='Joyner Lucas',
+)
+# Function that returns a pandas DataFrame with all songs from a specific artist within the playlist and create it in the user account
+# The ensure_all_artist_songs Flag serves the purpose of making sure all the artist's songs are present in a "This is" type playlist, regardless of the number_of_songs.
 # This behavior is turned off by setting the Flag as False
+# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
+~~~
+ - artist_specific_playlist
+~~~python
+# Parameters
+artist_specific_playlist(
+    artist_name: str,
+    number_of_songs: int = 50,
+    with_distance: bool = False,
+    build_playlist: bool = False,
+    print_base_caracteristics: bool = False,
+)
+# Method Use Example
+api.artist_specific_playlist(
+    number_of_songs=50,
+    build_playlist=True,
+    artist_name='Joyner Lucas',
+    print_base_caracteristics=True,
+)
+# Function that returns a pandas DataFrame with all songs from a specific artist within the playlist and complete that new playlist with the closest songs to that artist, and create it in the user account
 # print_base_caracteristics will display the parameter song information
 # The "distance" is a mathematical value with no explicit units, that is
 # used by the algorithm to find the closest songs
-# If complete_with_similar is True and K is more than all the songs with that artist, an Artist Mix is created,
-# otherwise, a "This once was" Playlist is created
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - audio_features_extraordinary_songs
 ~~~python
 # Parameters
 audio_features_extraordinary_songs()
 # Method Use Example
 api.audio_features_extraordinary_songs()
 # Function that returns a dictionary containing the songs that have the maximum and minimum values
 # for the 5 audio features used in this package: ['danceability', 'energy', 'instrumentalness', 'tempo', 'valence']
 ~~~
- - get_profile_recommendation
+ - audio_features_statistics
 ~~~python
 # Parameters
-get_profile_recommendation(K: int = 50, main_criteria: str = 'mixed', save_with_date: bool = False,
-build_playlist: bool = False, time_range: str = 'short_term')
+audio_features_statistics()
 # Method Use Example
-api.get_profile_recommendation(build_playlist=True)
-# Function that returns a pandas DataFrame with profile-based recommendations, and creates it in the user account
-# main_criteria is the base info to get the recommendations
-# save_with_date is a flag to save the recommendations as a playlist at a point in time Snapshot
-# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
+api.audio_features_statistics()
+# Function that returns the statistics (max, min and mean) for the audio features within the playlist.
+# The 5 audio features used in this package: ['danceability', 'energy', 'instrumentalness', 'tempo', 'valence']
 ~~~
  - get_playlist_recommendation
 ~~~python
 # Parameters
-get_playlist_recommendation(K: int = 50, time_range: str = 'all_time', main_criteria: str = 'mixed', save_with_date: bool = False,
-build_playlist: bool = False)
+get_playlist_recommendation(
+    number_of_songs: int = 50,
+    time_range: str = 'all_time',
+    main_criteria: str = 'mixed',
+    save_with_date: bool = False,
+    build_playlist: bool = False,
+)
 # Method Use Example
 api.get_playlist_recommendation(build_playlist=True)
 # Function that returns a pandas DataFrame with playlist-based recommendations, and creates it in the user account
 # main_criteria is the base info to get the recommendations
 # time_range is the time range to be looked at for the recommendations baseline
 # save_with_date is a flag to save the recommendations as a playlist as a point in time Snapshot
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
- - get_general_recommendation
-~~~python
-# Parameters
-get_general_recommendation(K: int = 50, genres_info: 'list[str]' = [], artists_info: 'list[str]' = [], build_playlist: bool = False, use_main_playlist_audio_features: bool = False, tracks_info: Union['list[str]', 'list[tuple[str]]', 'list[list[str]]', 'dict[str, str]'] = [])
-# Method Use Example
-api.get_general_recommendation(build_playlist=True, artists_info=['NF', 'Logic'], use_main_playlist_audio_features=True)
-# Function that returns a pandas DataFrame with artists, genres, and/or tracks-based recommendations, and creates it in the user account
-# genres_info, artists_info, and tracks_info are the lists of information that the recommendation would be based on
-# use_main_playlist_audio_features is the flag to indicate if the playlist-provided audio features will be used as the target for a better recommendation
-# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
-~~~~~~
- - select_playlist
-~~~python
-# Parameters
-select_playlist(user_id: str, playlist_id: str = None, playlist_url: str = None, liked_songs: bool = False)
-# Method Use Example
-api.select_playlist(user_id='USER_ID', liked_songs=True)
-# Function to select a playlist to be mapped and be available on all the playlist-related recommendation
-# functions on an already existing authorization context
-~~~~~~
  - get_songs_by_mood
 ~~~python
 # Parameters
-get_songs_by_mood(mood: str, K: int = 50, build_playlist: bool = False, exclude_mostly_instrumental: bool = False)
+get_songs_by_mood(
+    mood: str,
+    number_of_songs: int = 50,
+    build_playlist: bool = False,
+    exclude_mostly_instrumental: bool = False
+)
 # Method Use Example
 api.get_songs_by_mood(mood='happy', build_playlist=True)
 # Function to create a playlist based on the general mood of its songs
+# exclude_mostly_instrumental is a flag to remove the songs that are more than 80% instrumental from the song base
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~~~~
  - playlist_songs_based_on_most_listened_tracks
 ~~~python
 # Parameters
-playlist_songs_based_on_most_listened_tracks(K: int = 50, build_playlist: bool = False, time_range: str = 'short_term')
-# Method Use Example
-api.playlist_songs_based_on_most_listened_tracks(time_range='medium_term', build_playlist=True)
+playlist_songs_based_on_most_listened_tracks(
+    number_of_songs: int = 50,
+    build_playlist: bool = False,
+    time_range: str = 'short_term',
+)
+# Method Use Example
+api.playlist_songs_based_on_most_listened_tracks(
+    number_of_songs=50,
+    build_playlist=True,
+    time_range='medium_term',
+)
 # Function to create a playlist with songs from the base playlist that are the closest to the user's most listened songs
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~~~~
- - get_medium_term_favorites_playlist - DEPRECATED
-~~~python
-# Parameters
-get_medium_term_favorites_playlist(with_distance: bool, generate_csv: bool,
-                        generate_parquet: bool, build_playlist: bool)
-# Method Use Example
-api.get_medium_term_favorites_playlist(generate_csv=True, build_playlist=True)
-# Function that returns the pandas DataFrame representing the
-# medium term top 5 recommendation playlist
-# All parameters are defaulted to False
-# The "distance" is a mathematical value with no explicit units, that is
-# used by te algorithm to find the closest songs
-# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
-~~~
- - get_short_term_favorites_playlist - DEPRECATED
-~~~python
-# Parameters
-get_short_term_favorites_playlist(with_distance: bool, generate_csv: bool,
-                        generate_parquet: bool, build_playlist: bool)
-# Method Use Example
-api.get_short_term_favorites_playlist(generate_csv=True, build_playlist=True)
-# Function that returns the pandas DataFrame representing the
-# short term top 5 recommendation playlist
-# All parameters are defaulted to False
-# The "distance" is a mathematical value with no explicit units, that is
-# used by te algorithm to find the closest songs
-# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
-~~~
- - refresh_token - DEPRECATED
+ - update_all_generated_playlists
 ~~~python
 # Parameters
-refresh_token(token: str)
+update_all_generated_playlists(
+    playlist_types_to_update: list[str] = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood', 'most-listened-recommendation'],
+    playlist_types_not_to_update: list[str] = []
+)
 # Method Use Example
-api.refresh_token(token='AUTH TOKEN')
-# Function that refreshes the auth token in order to not having to rerun the initialization every hour
+api.update_all_generated_playlists()
+# or for example api.update_all_generated_playlists(playlist_types_to_update=['playlist-recommendation'])
+# Function updates all the playlists once generated by this package in batch
+# Note that if only a few updates are preferred, the methods above are a better fit\
+# But for any combination of types of updates this method fits well
 ~~~
 
 ## Suggestions
  - ### Advice towards leaving everything more organized <br>
-   It is recommended that the user creates folders to group the playlists created by this package, because after creating more than 150 playlists, your library can, and probably will, become a mess.  Unfortunately, the Spotify API does not allow users to create or manipulate folders in the same way that a file system does. The only way to create folders is manually, through the web page or app. Some suggestions for folders that could be useful include "Song Related" for playlists created using the get_recommendations_for_song function, "Profile Recommendations" for playlists created with get_profile_recommendation, "Personal Trends" for playlists created with get_most_listened, get_short_term_favorites_playlist, or get_medium_term_favorites_playlist, and any other categories that the user thinks would be useful.
+   It is recommended that the user creates folders to group the playlists created by this package, because after creating more than 150 playlists, your library can, and probably will, become a mess. Unfortunately, the Spotify API does not allow users to create or manipulate folders in the same way that a file system would work. The only way to create folders is manually, through the web page or app. Some suggestions for folders that could be useful include "Song Related" for playlists created using the get_recommendations_for_song function, "Profile Recommendations" for playlists created with get_profile_recommendation, "Personal Trends" for playlists created with get_most_listened, and any other categories that the user thinks would be useful.
  - ### Spotify Enhance Feature vs spotify-recommender-api package <br>
-    I think it is really possible, and legitimate, to wonder if the Enhance Feature replaces the use of this package. However, in my opinion, they can actually be used in a complementary fashion. For example, you can create a profile recommendation based on your most listened tracks, and then use the Enhance feature to increase the number of new and enjoyable songs in that playlist, both from the profile recommendation playlist and from the enhancement itself. This can improve the overall listening experience. It's worth noting that while the Enhance Feature was introduced after the development of most of the package, they do not conflict with each other.
-
-
-
+    I think it is really possible, and legitimate, to wonder if the Enhance Feature (on mobile called Smart Shuffle) replaces the use of this package. However, in my opinion, they can actually be used in a complementary fashion. For example, you can create a profile recommendation based on your most listened tracks, and then use the Enhance feature to increase the number of new and enjoyable songs in that playlist, both from the profile recommendation playlist and from the enhancement itself. This can improve the overall listening experience. It's worth noting that while the Enhance Feature was introduced after the development of most of the package, they do not conflict with each other.
 
 
 # OG Scripts
-###DEPRECATED###
+###DEPRECATED### and not maintained since 2022
 ### Context
 This script, in jupyter notebook format for organization purposes, applies the technique called K Nearest Neighbors to find the 50 closest songs to either one chosen or one of the users top 5(short term), all within a specific Spotify playlist, in order to maintain the most consistency in terms of the specific chosen style, and creates a new playlist with those songs in the user's library, using their genres, artists and overall popularity as metrics to determine indexes of comparison between songs
 
 ### Variations
 There are also 2 variations from that, which consist of medium term favorites related top 100 and "short term top 5" related top 50 songs. They vary from OG model since the base song(s) is(are) not chosen by hand but statistically
 
 ### DISCLAIMER ###
 Not fit for direct use since some information such as client id, client secret, both of which are, now, in a hidden script on .gitignore so that it is not made public, have to be informed in order for the Spotify Web API to work properly.
 And also, as of January 2022, these scripts are deprecated, so they will not have any maintenance or overtime improvements or new features
 
 
 
-
-
-## Packages used
+# Packages used
  - Pandas
 ~~~ps1
 pip install pandas
 ~~~
  - Requests
 ~~~ps1
 pip install requests
 ~~~
  - Seaborn
 ~~~ps1
 pip install seaborn
 ~~~
+ - Matplotlib
+~~~ps1
+pip install matplotlib
+~~~
+ - FastAPI
+~~~ps1
+pip install fastapi
+~~~
+ - Uvicorn
+~~~ps1
+pip install uvicorn
+~~~
  - Re (re)
  - Os (os)
+ - Abc (abc)
  - Json (json)
  - Time (time)
+ - Pytz (pytz)
+ - Typing (typing)
+ - Logging (logging)
  - Datetime (datetime)
  - Dateutil (dateutil)
- - Operator (operator)
+ - Traceback (traceback)
+ - Threading (threading)
  - Functools (functools)
+ - Contextlib (contextlib)
  - Webbrowser (webbrowser)
+ - Dataclasses (dataclasses)
 
 
 # Contributing
 Well, since this is a really simple package, contributing is always welcome, just as much as creating issues experienced with the package
 
 In order to better organize these contributions, it would be ideal that all PRs follow the template:
 
@@ -378,10 +460,10 @@
 A explanation on why those changes were needed, necessary, or at least, why it was on the best interest of the package users, for the package to have this changed
 
 CHANGES: <br>
 List of changes made, can be the list of the commits made, or a simple changes list
 
 ## Commits
 Ideally the commits should make use of the convention of [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) <br>
-Something i recommend is the usage of either the [Commitizen](https://github.com/commitizen/cz-cli) terminal extension or the [Commit Message Editor](https://marketplace.visualstudio.com/items?itemName=adam-bender.commit-message-editor) VSCode Extension
+Something I recommend is the usage of either the [Commitizen](https://github.com/commitizen/cz-cli) terminal extension or the [Commit Message Editor](https://marketplace.visualstudio.com/items?itemName=adam-bender.commit-message-editor) VSCode Extension
```

## Comparing `spotify_recommender_api-4.5.0.dist-info/RECORD` & `spotify_recommender_api-5.0.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-spotify_recommender_api/__init__.py,sha256=a4qsqPKUrk6Ur9lXXKPt7KEI5zaqiA8s2bLsPUcPw9s,21
-spotify_recommender_api/authentication.py,sha256=jQ49ZXeZ9Vj6x76aooA7uQ09xRRETmMDYCfeRw0TaPQ,1263
-spotify_recommender_api/core.py,sha256=ri6BRqe6znUsacjZLPzcwE3kuH4H9-1M7uVPHPhdhbA,15896
-spotify_recommender_api/error.py,sha256=BBG5MUYuoAGElBAV058H6o13R-bYR_sGGgjAT1r7lCg,2042
-spotify_recommender_api/recommender.py,sha256=K2rvp1j4cEQvYwW8iA4TbdZXNllgyD9-3ogoBkdoJKM,121606
-spotify_recommender_api/request_handler.py,sha256=uZabNApJIdnuUL_wN8KRKWRAwEDVjK0BB4QaG4SHjRM,6217
-spotify_recommender_api/sensitive.py,sha256=Xn2FFn4uUk94Ei_It1U2iT5ZZEafHBt9q--lSPwlaoI,99
-spotify_recommender_api/server.py,sha256=Jq90Sd6GrI4txMaLFDcNoThy3jSWe8MwVUIvQXSkkYQ,6722
-spotify_recommender_api/util.py,sha256=n72S-Jsi7uu8Vvhy7ArgBTXRdSYO-FDo1lMksoVB4oM,9757
-spotify_recommender_api-4.5.0.dist-info/METADATA,sha256=X0f26shnWoXb0G4ebUD2jEijSwQihUApkJwB-ccLJEQ,22073
-spotify_recommender_api-4.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spotify_recommender_api-4.5.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
-spotify_recommender_api-4.5.0.dist-info/RECORD,,
+spotify_recommender_api/__init__.py,sha256=tXvDczYdvTalg2gkintwACof0DmnunrBzFAQYy7uaWY,80
+spotify_recommender_api/error.py,sha256=tFJoG2kYUrxTniSUaHoQSInHoT0E13JLctOyB3lr-rk,2653
+spotify_recommender_api/recommender.py,sha256=QXL3rT0g-S4so8XYqM_IoxzLGrZelB5j0Jk9tZZMvlY,29365
+spotify_recommender_api/util.py,sha256=CBI8w7l53sE0Gv8tSszVTKR_tbf-SDXHPFuGQgqJz_c,5610
+spotify_recommender_api/visualization.py,sha256=ayPKAO402RDnpAoxhR_Lv5NedsfDQveTShIHmWdxqHE,1186
+spotify_recommender_api/artist/__init__.py,sha256=19lfn5R5_1uZSL5R21GafrvL9s1Xq1G9T4mARCQ1CYo,56
+spotify_recommender_api/artist/artist.py,sha256=-692NZa7SZpcLOEnVlIz5IZdSLhaR-RJ_K9LjNw9i5w,617
+spotify_recommender_api/server/__init__.py,sha256=w-_dMgzh6D4McZ3sn2Kee6_w-IRLo30dXJKOjMCCs20,59
+spotify_recommender_api/server/sensitive.py,sha256=Xn2FFn4uUk94Ei_It1U2iT5ZZEafHBt9q--lSPwlaoI,99
+spotify_recommender_api/server/server.py,sha256=1XrwjzjWbs8YTFjDB7SLWvedIw_dcwgkS28PFUjcxu0,6629
+spotify_recommender_api/song/__init__.py,sha256=2ghcJscaLBqwneQZwHdr9XvyhnYTxLFzdbNVHQs2VpQ,50
+spotify_recommender_api/song/song.py,sha256=vokKic-E7JGtGqTOIgXHMXyKEeYz2ipKKA_5K42iLz0,2706
+spotify_recommender_api/song/util.py,sha256=4XRTTDHeqz7Xhr8yrnP16D53CpiZIFPMoXzg98O0W-o,1480
+spotify_recommender_api/user/__init__.py,sha256=s4Zo1pkb8UOlUdV-2vwjJOkoexmlU0v2XNZctUu-c3w,50
+spotify_recommender_api/user/user.py,sha256=32Lr_A5_hgdYmq58pFcYEAHSUXCXbrdornV-mos_ZgA,11265
+spotify_recommender_api/user/util.py,sha256=BZlDYC-fe9oxnSisyt23m9LtlbEMEYVWuhqH-21r8h8,36708
+spotify_recommender_api-5.0.0.dist-info/METADATA,sha256=OPLGf07YsorKxA-nE4Waym1rExTopEjQKUU3h3-dbp0,23528
+spotify_recommender_api-5.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spotify_recommender_api-5.0.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
+spotify_recommender_api-5.0.0.dist-info/RECORD,,
```

