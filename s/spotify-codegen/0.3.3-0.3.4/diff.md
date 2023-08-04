# Comparing `tmp/spotify_codegen-0.3.3.tar.gz` & `tmp/spotify_codegen-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_codegen-0.3.3.tar", max compression
+gzip compressed data, was "spotify_codegen-0.3.4.tar", max compression
```

## Comparing `spotify_codegen-0.3.3.tar` & `spotify_codegen-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-25 16:44:36.705545 spotify_codegen-0.3.3/LICENSE
--rw-r--r--   0        0        0     3253 2023-05-25 16:44:36.705545 spotify_codegen-0.3.3/README.md
--rw-r--r--   0        0        0     2174 2023-05-25 16:45:01.570654 spotify_codegen-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/__init__.py
--rw-r--r--   0        0        0     3166 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/cli.py
--rw-r--r--   0        0        0     7876 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/main.py
--rw-r--r--   0        0        0        0 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/py.typed
--rw-r--r--   0        0        0     4308 1970-01-01 00:00:00.000000 spotify_codegen-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 07:01:02.042300 spotify_codegen-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3277 2023-08-04 07:01:02.042300 spotify_codegen-0.3.4/README.md
+-rw-r--r--   0        0        0     2174 2023-08-04 07:01:17.746265 spotify_codegen-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-08-04 07:01:02.046300 spotify_codegen-0.3.4/src/spotifycodegen/__init__.py
+-rw-r--r--   0        0        0     3166 2023-08-04 07:01:02.046300 spotify_codegen-0.3.4/src/spotifycodegen/cli.py
+-rw-r--r--   0        0        0     7876 2023-08-04 07:01:02.046300 spotify_codegen-0.3.4/src/spotifycodegen/main.py
+-rw-r--r--   0        0        0        0 2023-08-04 07:01:02.046300 spotify_codegen-0.3.4/src/spotifycodegen/py.typed
+-rw-r--r--   0        0        0     4332 1970-01-01 00:00:00.000000 spotify_codegen-0.3.4/PKG-INFO
```

### Comparing `spotify_codegen-0.3.3/LICENSE` & `spotify_codegen-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_codegen-0.3.3/README.md` & `spotify_codegen-0.3.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,36 +19,38 @@
 [tests]: https://github.com/tilschuenemann/spotify-codegen/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/tilschuenemann/spotify-codegen
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Features
 
-Spotify removed the feature to get a stitched image of an album / artist / track cover with their own Spotify Code. This package mimicks that behaviour and creates stitches, based on supplied
+Spotify stopped giving users an easy way to grab the song, artist or album artwork with the respective Spotify Code - `spotify-codegen` to the rescue!
 
-- URL
-- URI
-- query
+You can stitch the album | track | artist artwork with the Spotify Code by supplying:
+
+- URL(s)
+- URI(s)
+- a search query
 
 It's also possible to use create stitches for:
 
-- all saved albums
+- all of your saved albums
 - 50 followed artists (limit imposed by Spotify API)
 
-[You can also try the Streamlit showcase here.](https://tilschuenemann-showcase-showcasesstart-0ndtb3.streamlit.app/spotify_codegen)
-
 ## Requirements
 
-You'll need to have a Spotify Client ID & Secret in order to make API requests. Specify as environment variable like this:
+To use the Spotify API, you'll have to login using your credentials and create an app. That apps ID and secret need to be specified as environment variables:
 
 ```console
 $ export SPOTIPY_CLIENT_ID="your_client_id"
-$ export SPOTIPY_CLIENT_ID="your_client_secret"
+$ export SPOTIPY_CLIENT_SECRET="your_client_secret"
 ```
 
+You can now use both the CLI and the Python API!
+
 ## Installation
 
 You can install _spotify-codegen_ via [pip] from [PyPI]:
 
 ```console
 $ pip install spotify-codegen
 ```
```

### Comparing `spotify_codegen-0.3.3/pyproject.toml` & `spotify_codegen-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotify-codegen"
-version = "0.3.3"
+version = "0.3.4"
 description = "spotify-codegen"
 authors = ["Til Schünemann <til.schuenemann@mailbox.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tilschuenemann/spotify-codegen"
 repository = "https://github.com/tilschuenemann/spotify-codegen"
 documentation = "https://spotify-codegen.readthedocs.io"
```

### Comparing `spotify_codegen-0.3.3/src/spotifycodegen/cli.py` & `spotify_codegen-0.3.4/src/spotifycodegen/cli.py`

 * *Files identical despite different names*

### Comparing `spotify_codegen-0.3.3/src/spotifycodegen/main.py` & `spotify_codegen-0.3.4/src/spotifycodegen/main.py`

 * *Files identical despite different names*

### Comparing `spotify_codegen-0.3.3/PKG-INFO` & `spotify_codegen-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-codegen
-Version: 0.3.3
+Version: 0.3.4
 Summary: spotify-codegen
 Home-page: https://github.com/tilschuenemann/spotify-codegen
 License: MIT
 Keywords: spotify-codegen,spoticode,spotify,spotipy,art,code,qr,album,track,song,album,generator
 Author: Til Schünemann
 Author-email: til.schuenemann@mailbox.org
 Requires-Python: >=3.10,<4.0
@@ -44,36 +44,38 @@
 [tests]: https://github.com/tilschuenemann/spotify-codegen/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/tilschuenemann/spotify-codegen
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Features
 
-Spotify removed the feature to get a stitched image of an album / artist / track cover with their own Spotify Code. This package mimicks that behaviour and creates stitches, based on supplied
+Spotify stopped giving users an easy way to grab the song, artist or album artwork with the respective Spotify Code - `spotify-codegen` to the rescue!
 
-- URL
-- URI
-- query
+You can stitch the album | track | artist artwork with the Spotify Code by supplying:
+
+- URL(s)
+- URI(s)
+- a search query
 
 It's also possible to use create stitches for:
 
-- all saved albums
+- all of your saved albums
 - 50 followed artists (limit imposed by Spotify API)
 
-[You can also try the Streamlit showcase here.](https://tilschuenemann-showcase-showcasesstart-0ndtb3.streamlit.app/spotify_codegen)
-
 ## Requirements
 
-You'll need to have a Spotify Client ID & Secret in order to make API requests. Specify as environment variable like this:
+To use the Spotify API, you'll have to login using your credentials and create an app. That apps ID and secret need to be specified as environment variables:
 
 ```console
 $ export SPOTIPY_CLIENT_ID="your_client_id"
-$ export SPOTIPY_CLIENT_ID="your_client_secret"
+$ export SPOTIPY_CLIENT_SECRET="your_client_secret"
 ```
 
+You can now use both the CLI and the Python API!
+
 ## Installation
 
 You can install _spotify-codegen_ via [pip] from [PyPI]:
 
 ```console
 $ pip install spotify-codegen
 ```
```

