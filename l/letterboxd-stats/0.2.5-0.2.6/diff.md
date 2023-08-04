# Comparing `tmp/letterboxd_stats-0.2.5.tar.gz` & `tmp/letterboxd_stats-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.2.5.tar", last modified: Sat Jul  1 09:44:58 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.2.6.tar", last modified: Fri Aug  4 09:44:42 2023, max compression
```

## Comparing `letterboxd_stats-0.2.5.tar` & `letterboxd_stats-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.5/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.5/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1472 2023-06-30 20:22:08.000000 letterboxd_stats-0.2.5/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5331 2023-06-30 11:32:08.000000 letterboxd_stats-0.2.5/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-26 09:44:09.000000 letterboxd_stats-0.2.5/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.5/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-06-30 15:36:50.000000 letterboxd_stats-0.2.5/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     6619 2023-07-01 09:24:22.000000 letterboxd_stats-0.2.5/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      887 2023-07-01 09:43:53.000000 letterboxd_stats-0.2.5/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.6/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.6/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-04 09:44:41.997653 letterboxd_stats-0.2.6/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1472 2023-07-30 11:28:06.000000 letterboxd_stats-0.2.6/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5609 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4574 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3074 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2958 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     6619 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      158 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-08-04 09:44:41.000000 letterboxd_stats-0.2.6/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      932 2023-08-04 09:44:30.000000 letterboxd_stats-0.2.6/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-08-04 09:44:42.001653 letterboxd_stats-0.2.6/setup.cfg
```

### Comparing `letterboxd_stats-0.2.5/LICENCE` & `letterboxd_stats-0.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.5/PKG-INFO` & `letterboxd_stats-0.2.6/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd_stats
-Version: 0.2.5
+Name: letterboxd-stats
+Version: 0.2.6
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.5/README.md` & `letterboxd_stats-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.5/letterboxd_stats/__init__.py` & `letterboxd_stats-0.2.6/letterboxd_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.5/letterboxd_stats/cli.py` & `letterboxd_stats-0.2.6/letterboxd_stats/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,25 @@
         validate=lambda result: result in movies_info["Id"].values,
         filter=lambda result: None if result is None else int(result),
         invalid_message="Input must be in the resulting IDs",
     ).execute()
     return movie_id
 
 
+def select_list(names: list[str]) -> int:
+    name = inquirer.fuzzy(  # type: ignore
+        message="Select your list:",
+        mandatory=True,
+        max_height="25%",
+        choices=names,
+        validate=lambda result: result in names,
+    ).execute()
+    return name
+
+
 def select_search_result(results: list[str]) -> int:
     choices = [Choice(i, name=r) for i, r in enumerate(results)]
     result = inquirer.select(  # type: ignore
         message="Result of your search. Please select one",
         choices=choices,
         default=choices[0],
     ).execute()
```

### Comparing `letterboxd_stats-0.2.5/letterboxd_stats/data.py` & `letterboxd_stats-0.2.6/letterboxd_stats/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import pandas as pd
 import numpy as np
 from letterboxd_stats import cli
 from letterboxd_stats.web_scraper import get_tmdb_id
 from letterboxd_stats import tmdb
 import os
 from letterboxd_stats import config
+from pandarallel import pandarallel
+from tqdm import tqdm
+
+pandarallel.initialize(verbose=0)
+tqdm.pandas(desc="Fetching ids...")
 
 
 def check_if_watched(df: pd.DataFrame, row: pd.Series):
     if row["Title"] in df["Name"].values:
         watched_films_same_name = df[df["Name"] == row["Title"]]
         for _, film in watched_films_same_name.iterrows():
-            film_id = get_tmdb_id(film["Letterboxd URI"], False)
+            film_id = get_tmdb_id(film["Letterboxd URI"])
             if film_id == row["Id"]:
                 return True
     return False
 
 
 def read_watched_films(df: pd.DataFrame, path: str, name: str):
     df_profile = pd.read_csv(path)
@@ -39,15 +44,15 @@
     return df["Name"].iloc[0]
 
 
 def open_list(path: str, limit, acending):
     list_names = {
         get_list_name(os.path.join(path, letterboxd_list)): letterboxd_list for letterboxd_list in os.listdir(path)
     }
-    name = cli.select_value(sorted(list(list_names.keys())), message="Select your list")
+    name = cli.select_list(sorted(list(list_names.keys())))
     return open_file("Lists", os.path.join(path, list_names[name]), limit, acending, header=3)
 
 
 def open_file(filetype: str, path: str, limit, ascending, header=0):
     df = pd.read_csv(path, header=header)
     df.rename(columns={"Name": "Title", "Letterboxd URI": "Url"}, inplace=True)
     df["Year"] = df["Year"].fillna(0).astype(int)
@@ -66,15 +71,16 @@
     df.rename(columns={"URL": "Url"}, inplace=True)
     df = df.drop("Description", axis=1)
     df["Rating"] = df["Rating"].astype(float)
     sort_column = cli.select_value(df.columns.values.tolist(), "Select the order of your diary entries:")
     df.sort_values(by=sort_column, ascending=ascending, inplace=True)
     avg = {"Rating Mean": "{:.2f}".format(df["Rating"].mean())}
     if config["TMDB"]["get_list_runtimes"] is True:
-        df["Duration"] = df.apply(lambda row: tmdb.get_film_duration(row["Url"]), axis=1)  # type: ignore
+        ids = df["Url"].progress_map(get_tmdb_id)
+        df["Duration"] = ids.parallel_map(lambda id: tmdb.get_film_duration(id))  # type: ignore
         avg["Time-weighted Rating Mean"] = "{:.2f}".format(
             ((df["Duration"] / df["Duration"].sum()) * df["Rating"]).sum()
         )
     cli.print_film(avg, expand=False)
     return df
```

### Comparing `letterboxd_stats-0.2.5/letterboxd_stats/main.py` & `letterboxd_stats-0.2.6/letterboxd_stats/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         tmdb.get_movie_detail(movie["Id"], ws.create_movie_url(title_url, "film_page"))
         movie = data.select_film_of_person(df)
 
 
 def search_film(args_search_film: str):
     title_url = ws.search_film(args_search_film, True)
     film_url = ws.create_movie_url(title_url, "film_page")
-    tmdb.get_movie_detail(ws.get_tmdb_id(film_url, False), film_url)  # type: ignore
+    tmdb.get_movie_detail(ws.get_tmdb_id(film_url), film_url)  # type: ignore
     answer = ws.select_optional_operation()
     if answer != "Exit":
         downloader = ws.Downloader()
         downloader.login()
         downloader.perform_operation(answer, title_url)
```

### Comparing `letterboxd_stats-0.2.5/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.2.6/letterboxd_stats/tmdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from tmdbv3api import TMDb, Person, Movie, Search
+from tmdbv3api.exceptions import TMDbException
 import pandas as pd
 from letterboxd_stats import cli
 from letterboxd_stats import config
-from letterboxd_stats.web_scraper import get_tmdb_id
+from pandarallel import pandarallel
 
 tmdb = TMDb()
 tmdb.api_key = config["TMDB"]["api_key"]
 person = Person()
 movie = Movie()
 search = Search()
+pandarallel.initialize(verbose=0)
 
 
 def get_person(name: str):
     print(f"Searching for '{name}'")
     search_results = search.people({"query": name})
     names = [result.name for result in search_results]  # type: ignore
     if len(names) == 0:
@@ -36,15 +38,15 @@
     df = pd.DataFrame(list_of_films)
     department = cli.select_value(
         df["Department"].unique(), f"Select a department for {p['name']}", known_for_department
     )
     df = df[df["Department"] == department]
     df = df.drop("Department", axis=1)
     if config["TMDB"]["get_list_runtimes"] is True:
-        df["Duration"] = df.apply(lambda row: movie.details(row["Id"]).runtime, axis=1)  # type: ignore
+        df["Duration"] = df["Id"].parallel_map(get_film_duration)  # type: ignore
     return df, p["name"]
 
 
 def get_movie(movie_query: str):
     print(f"Searching for movie '{movie_query}'")
     search_results = search.movies({"query": movie_query})
     titles = [f"{result.title} ({result.release_date})" for result in search_results]  # type: ignore
@@ -69,10 +71,13 @@
         "Release Date": movie_details["release_date"],
     }
     if letterboxd_url:
         selected_details["Letterboxd Url"] = letterboxd_url
     cli.print_film(selected_details)
 
 
-def get_film_duration(url: str):
-    tmdb_id = get_tmdb_id(url, False)
-    return movie.details(tmdb_id).runtime  # type: ignore
+def get_film_duration(tmdb_id: str):
+    try:
+        runtime = movie.details(int(tmdb_id)).runtime  # type: ignore
+    except TMDbException:
+        runtime = 0
+    return runtime
```

### Comparing `letterboxd_stats-0.2.5/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.2.6/letterboxd_stats/web_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     tmdb_link = movie_page.xpath("//a[@data-track-action='TMDb']")
     if len(tmdb_link) == 0:
         raise ValueError("No Movie link found")
     id = tmdb_link[0].get("href").split("/")[-2]
     return int(id)
 
 
-def get_tmdb_id(link: str, is_diary: bool):
+def get_tmdb_id(link: str, is_diary=False):
     tmdb_id_cache = shelve.open(cache_path, writeback=False, protocol=5)
     if link in tmdb_id_cache:
         id = tmdb_id_cache[link]
     else:
         try:
             id = _get_tmdb_id_from_web(link, is_diary)
             tmdb_id_cache[link] = id
```

### Comparing `letterboxd_stats-0.2.5/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd-stats
-Version: 0.2.5
+Name: letterboxd_stats
+Version: 0.2.6
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.5/pyproject.toml` & `letterboxd_stats-0.2.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.2.5"
+version = "0.2.6"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -16,18 +16,20 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "ascii_magic~=2.3.0",
     "inquirerpy~=0.3.4",
     "lxml~=4.9.0",
     "pandas~=1.5.1",
+    "pandarallel~=1.6.5",
     "platformdirs~=3.0.0",
     "rich~=13.3.5",
     "tmdbv3api~=1.7.7",
     "tomli~=2.0.1",
+    "tqdm~=4.65.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mBaratta96/letterboxd_stats"
 "Bug Tracker" = "https://github.com/mBaratta96/letterboxd_stats/issues"
 
 [project.scripts]
```

