# Comparing `tmp/rec_spotify-1.5.1.tar.gz` & `tmp/rec_spotify-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rec_spotify-1.5.1.tar", max compression
+gzip compressed data, was "rec_spotify-1.6.tar", max compression
```

## Comparing `rec_spotify-1.5.1.tar` & `rec_spotify-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.5.1/etc/screen.png
--rw-r--r--   0        0        0     1291 2023-07-26 17:17:11.671633 rec_spotify-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     3380 2023-07-26 08:52:42.903775 rec_spotify-1.5.1/README.md
--rw-r--r--   0        0        0       21 2023-07-26 08:53:59.383139 rec_spotify-1.5.1/rec_spotify/__init__.py
--rw-r--r--   0        0        0     2167 2023-07-26 17:17:41.729242 rec_spotify-1.5.1/rec_spotify/cli.py
--rw-r--r--   0        0        0     4278 2023-07-25 10:23:46.440401 rec_spotify-1.5.1/rec_spotify/config.py
--rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.5.1/rec_spotify/console.py
--rw-r--r--   0        0        0     7312 2023-07-26 08:42:49.459812 rec_spotify-1.5.1/rec_spotify/database.py
--rw-r--r--   0        0        0     6429 2023-07-25 10:24:08.681879 rec_spotify-1.5.1/rec_spotify/items.py
--rw-r--r--   0        0        0     2197 2023-07-25 10:24:14.620839 rec_spotify-1.5.1/rec_spotify/lyrics.py
--rw-r--r--   0        0        0     7165 2023-07-26 08:48:15.677634 rec_spotify-1.5.1/rec_spotify/manager.py
--rw-r--r--   0        0        0     2398 2023-07-26 08:47:13.584024 rec_spotify-1.5.1/rec_spotify/messages.py
--rw-r--r--   0        0        0     3391 2023-07-25 10:24:40.331450 rec_spotify-1.5.1/rec_spotify/recorder.py
--rw-r--r--   0        0        0     6895 2023-07-26 08:43:31.230906 rec_spotify-1.5.1/rec_spotify/spotify.py
--rw-r--r--   0        0        0     2207 2023-07-25 10:25:06.194956 rec_spotify-1.5.1/rec_spotify/utils.py
--rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rec_spotify-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.6/etc/screen.png
+-rw-r--r--   0        0        0     1289 2023-08-04 21:14:51.210219 rec_spotify-1.6/pyproject.toml
+-rw-r--r--   0        0        0     3380 2023-07-26 08:52:42.903775 rec_spotify-1.6/README.md
+-rw-r--r--   0        0        0       21 2023-08-04 21:14:39.789341 rec_spotify-1.6/rec_spotify/__init__.py
+-rw-r--r--   0        0        0     2167 2023-08-04 19:08:19.661430 rec_spotify-1.6/rec_spotify/cli.py
+-rw-r--r--   0        0        0     4355 2023-08-04 19:52:51.427886 rec_spotify-1.6/rec_spotify/config.py
+-rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.6/rec_spotify/console.py
+-rw-r--r--   0        0        0     8076 2023-08-04 21:06:31.506170 rec_spotify-1.6/rec_spotify/database.py
+-rw-r--r--   0        0        0     6429 2023-07-25 10:24:08.681879 rec_spotify-1.6/rec_spotify/items.py
+-rw-r--r--   0        0        0     2197 2023-07-25 10:24:14.620839 rec_spotify-1.6/rec_spotify/lyrics.py
+-rw-r--r--   0        0        0     7224 2023-08-04 20:59:07.315812 rec_spotify-1.6/rec_spotify/manager.py
+-rw-r--r--   0        0        0     2612 2023-08-04 21:10:57.291823 rec_spotify-1.6/rec_spotify/messages.py
+-rw-r--r--   0        0        0     3391 2023-07-25 10:24:40.331450 rec_spotify-1.6/rec_spotify/recorder.py
+-rw-r--r--   0        0        0     7620 2023-08-04 20:17:36.300836 rec_spotify-1.6/rec_spotify/spotify.py
+-rw-r--r--   0        0        0     2207 2023-07-25 10:25:06.194956 rec_spotify-1.6/rec_spotify/utils.py
+-rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 rec_spotify-1.6/PKG-INFO
```

### Comparing `rec_spotify-1.5.1/etc/screen.png` & `rec_spotify-1.6/etc/screen.png`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/pyproject.toml` & `rec_spotify-1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rec-spotify"
-version = "1.5.1"
+version = "1.6"
 description = "📻 Record and sync Spotify tracks, albums, and playlists."
 repository = "https://github.com/oSeeLight/rec-spotify"
 authors = ["Jacov Rainz <oSeeLight@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rec_spotify"}]
 include = ["README.md", "etc"]
```

### Comparing `rec_spotify-1.5.1/README.md` & `rec_spotify-1.6/README.md`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/rec_spotify/cli.py` & `rec_spotify-1.6/rec_spotify/cli.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/rec_spotify/config.py` & `rec_spotify-1.6/rec_spotify/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     SAMPLE_RATE: int
     TRIM_SILENCE: bool
 
     _DEFAULT_FILENAME = "config.ini"
     _DEFAULT_DBNAME = "spotify.db"
     _DEFAULT_CACHE = ".cache"
 
+    _LIKED_ID = "likedVUqLsoulrg55rDqjp"
+    _LIKED_NAME = "Liked Songs"
+
     @classmethod
     def init(cls) -> None:
         """
         Initializes the Config class.
 
         This method checks if a configuration file exists and if not,
         it creates a new one.
```

### Comparing `rec_spotify-1.5.1/rec_spotify/console.py` & `rec_spotify-1.6/rec_spotify/console.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/rec_spotify/database.py` & `rec_spotify-1.6/rec_spotify/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,29 +116,48 @@
         "Parse a playlist data row into a Collection object."
         playlist = Collection(id=row[0])
         playlist.name = row[1]
         playlist.dirpath = row[2]
         return playlist
 
     @classmethod
-    def get_track(cls, id: str) -> Track | None:
+    def get_track(cls, id: str, playlist_id: str = "") -> Track | None:
         "Get track by id, returns Track or None if not found"
-        sql = "SELECT * FROM tracks WHERE id = ?;"
-        cls._cursor.execute(sql, (id,))
+        if playlist_id:
+            sql = "SELECT * FROM tracks WHERE id = ? AND playlist_id = ?;"
+            params = (id, playlist_id)
+        else:
+            sql = "SELECT * FROM tracks WHERE id = ?;"
+            params = (id,)
+        cls._cursor.execute(sql, params)
         row = cls._cursor.fetchone()
         if row is not None:
             return cls._parse_track_row(row)
         return None
 
     @classmethod
-    def add_track(cls, track: Track) -> None:
+    def add_track(cls, track: Track) -> bool:
         "Add new track to database"
         sql = "INSERT INTO tracks VALUES (?, ?, ?, ?, ?, ?, ?, ?);"
-        cls._cursor.execute(sql, (track.to_sql_fields()))
-        cls._connection.commit()
+        try:
+            cls._cursor.execute(sql, (track.to_sql_fields()))
+            cls._connection.commit()
+            return True
+        except sqlite3.IntegrityError:
+            track_ex = cls.get_track(track.id)
+            if track_ex is not None:
+                console.print(
+                    m.TRACK_DUPLICATE.format(
+                        playlist_new=track.collection.name,
+                        track_name=track_ex.title,
+                        playlist_old=track_ex.collection.name,
+                        track_path=track_ex.filepath,
+                    )
+                )
+            return False
 
     @classmethod
     def get_tracks(cls, downloaded: bool = False, total: bool = False) -> t.List[Track]:
         "Get all tracks"
         if total:
             sql = "SELECT * FROM tracks;"
         else:
```

### Comparing `rec_spotify-1.5.1/rec_spotify/items.py` & `rec_spotify-1.6/rec_spotify/items.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/rec_spotify/lyrics.py` & `rec_spotify-1.6/rec_spotify/lyrics.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/rec_spotify/manager.py` & `rec_spotify-1.6/rec_spotify/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,19 +64,20 @@
                 console.print(m.DEL_TRACK.format(track_title=track.title))
 
         # Sync Tracks
         tracks_to_download: t.Set[Track] = set()
         for sp_playlist in sp_playlists:
             processed_track_ids = []
             for sp_track in sp_playlist.get_tracks():
-                loc_track = Database.get_track(sp_track.id)
+                loc_track = Database.get_track(sp_track.id, sp_playlist.id)
                 if loc_track is None:
                     sp_track.set_download_path()
-                    Database.add_track(sp_track)
-                    console.print(m.NEW_TRACK.format(track_title=sp_track.title))
+                    added = Database.add_track(sp_track)
+                    if added:
+                        console.print(m.NEW_TRACK.format(track_title=sp_track.title))
 
                 processed_track_ids.append(sp_track.id)
 
             to_delete = Database.get_deleted_tracks(processed_track_ids, sp_playlist)
             for track in to_delete:
                 track.delete()
                 Database.delete_track(track)
```

### Comparing `rec_spotify-1.5.1/rec_spotify/messages.py` & `rec_spotify-1.6/rec_spotify/messages.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 TRACK = ":musical_note: {title}"
 NEW_TRACK = "[[green bold]ADDED[/green bold]] :musical_note: Track: {track_title}"
 DEL_TRACK = "[[red bold]DELETE[/red bold]] :x: Track: {track_title}"
 TRACK_SAVED = ":white_check_mark: Recorded: {filepath}"
 TRACK_NO_LOCAL = "[[blue bold]INFO[/blue bold]] :musical_note: [magenta bold]{track}[/magenta bold] was not located in the local library. It has been noted as not yet downloaded."
 TRACK_NOT_AVAILABLE = "[[blue bold]INFO[/blue bold]] :x: Track: {track_name} is not available for download."
-
+TRACK_DUPLICATE = "[[blue bold]DUPLICATE[/blue bold]] [ :file_folder: {playlist_new} ] :musical_note: Track: {track_name}. [blue bold]==>[/blue bold] [ :file_folder: {playlist_old} ] [ :floppy_disk: {track_path} ]"
 
 DATABASE_OK = "[[green bold]OK[/green bold]] Database initialization."
 STATS = "[[magenta bold]STATS[/magenta bold]] :file_folder: Playlists: {playlists_count} | :musical_note: Total Tracks: {tracks_count} | :fire: Tracks not downloaded: {undownloaded_count}"
 DB_CHECK_OK = "[[blue bold]INFO[/blue bold]] :white_check_mark: No issues were detected during the check process."
 
 SYNC_START = "[[blue bold]INFO[/blue bold]] The recording process has started. It will take about ~ {total_time} ({track_count} tracks)"
 SYNC_OK = "[[blue bold]INFO[/blue bold]] :white_check_mark: Everything is up to date."
```

### Comparing `rec_spotify-1.5.1/rec_spotify/recorder.py` & `rec_spotify-1.6/rec_spotify/recorder.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/rec_spotify/spotify.py` & `rec_spotify-1.6/rec_spotify/spotify.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def init(cls) -> None:
         cls._client = spotipy.Spotify(
             auth_manager=SpotifyOAuth(
                 client_id=Config.CLIENT_ID,
                 client_secret=Config.CLIENT_SECRET,
                 redirect_uri=Config.REDIRECT_URL,
                 cache_handler=CacheFileHandler(cache_path=Config.get_cache_filepath()),
-                scope="streaming, playlist-read-private, user-read-playback-state, user-modify-playback-state",
+                scope="user-library-read, streaming, playlist-read-private, user-read-playback-state, user-modify-playback-state",
             )
         )
         cls._set_device_id()
 
     @classmethod
     def get_track(cls, track: Track) -> Track:
         data: dict = cls._make_request(cls._client.track, track.id)
@@ -40,28 +40,39 @@
         return track
 
     @classmethod
     def get_collection(cls, collection: Collection) -> Collection:
         sp_col: dict
 
         if collection.kind == "playlist":
-            sp_col = cls._make_request(cls._client.playlist, collection.id)
+            if collection.id == Config._LIKED_ID:
+                sp_col = cls._make_request(cls._client.current_user_saved_tracks)
+            else:
+                sp_col = cls._make_request(cls._client.playlist, collection.id)
         else:
             sp_col = cls._make_request(cls._client.album, collection.id)
 
-        collection.name = sp_col["name"]
-        total_tracks = sp_col["tracks"]["total"]
+        if collection.id != Config._LIKED_ID:
+            collection.name = sp_col["name"]
+
+        if collection.id == Config._LIKED_ID:
+            total_tracks = sp_col["total"]
+        else:
+            total_tracks = sp_col["tracks"]["total"]
 
         for offset in range(0, total_tracks, 100):
             if collection.kind == "playlist":
-                sp_col = cls._make_request(
-                    cls._client.playlist_tracks,
-                    collection.id,
-                    offset=offset,
-                )
+                if collection.id == Config._LIKED_ID:
+                    sp_col = cls._make_request(cls._client.current_user_saved_tracks)
+                else:
+                    sp_col = cls._make_request(
+                        cls._client.playlist_tracks,
+                        collection.id,
+                        offset=offset,
+                    )
             else:
                 sp_col = cls._make_request(
                     cls._client.album_tracks,
                     collection.id,
                     offset=offset,
                 )
 
@@ -87,14 +98,19 @@
         collections: t.List[Collection] = []
         for playlist in sp_playlists["items"]:
             id = playlist["id"]
             collection = Collection(id, kind="playlist")
             collection = cls.get_collection(collection)
             collections.append(collection)
 
+        # Liked Playlist
+        liked = Collection(Config._LIKED_ID)
+        liked.name = Config._LIKED_NAME
+        collection = cls.get_collection(liked)
+        collections.append(collection)
         return collections
 
     @classmethod
     def _parse_track(cls, track: Track, data: dict) -> Track:
         track.id = data["id"]
         track.artist = cls._extract_artist(data["artists"])
         track.name = data["name"]
```

### Comparing `rec_spotify-1.5.1/rec_spotify/utils.py` & `rec_spotify-1.6/rec_spotify/utils.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5.1/PKG-INFO` & `rec_spotify-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rec-spotify
-Version: 1.5.1
+Version: 1.6
 Summary: 📻 Record and sync Spotify tracks, albums, and playlists.
 Home-page: https://github.com/oSeeLight/rec-spotify
 License: MIT
 Keywords: spotify,record
 Author: Jacov Rainz
 Author-email: oSeeLight@proton.me
 Requires-Python: >=3.11,<4.0
```

