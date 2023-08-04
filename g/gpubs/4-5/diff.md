# Comparing `tmp/gpubs-4.tar.gz` & `tmp/gpubs-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpubs-4.tar", last modified: Sat Jun 24 04:35:53 2023, max compression
+gzip compressed data, was "gpubs-5.tar", last modified: Fri Aug  4 01:43:34 2023, max compression
```

## Comparing `gpubs-4.tar` & `gpubs-5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-4/MANIFEST.in
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-24 04:35:53.032247 gpubs-4/PKG-INFO
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/gpubs/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-4/gpubs/__init__.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-06-24 04:35:52.000000 gpubs-4/gpubs/_version.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)    19754 2023-06-24 04:34:36.000000 gpubs-4/gpubs/api.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     2111 2023-06-24 02:02:55.000000 gpubs-4/gpubs/fetch.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      209 2023-06-24 01:55:43.000000 gpubs-4/gpubs/log.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     7035 2023-06-24 02:40:36.000000 gpubs-4/gpubs/models.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     4066 2023-06-24 02:04:02.000000 gpubs-4/gpubs/parse.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1301 2023-06-24 01:55:43.000000 gpubs-4/gpubs/reference.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1899 2023-06-24 03:41:23.000000 gpubs-4/gpubs/search_words.py
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/gpubs.egg-info/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/PKG-INFO
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/SOURCES.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/dependency_links.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/requires.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/top_level.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-06-23 21:37:20.000000 gpubs-4/release-info.json
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/scripts/
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-4/scripts/create_search_terms_file.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-4/scripts/download_pubs.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-4/scripts/search.awk
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-06-24 04:35:53.032247 gpubs-4/setup.cfg
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1141 2023-06-24 02:06:26.000000 gpubs-4/setup.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-5/MANIFEST.in
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-08-04 01:43:34.223223 gpubs-5/PKG-INFO
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/gpubs/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-5/gpubs/__init__.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-08-04 01:43:34.000000 gpubs-5/gpubs/_version.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)    19754 2023-06-24 04:34:36.000000 gpubs-5/gpubs/api.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     2111 2023-06-24 02:02:55.000000 gpubs-5/gpubs/fetch.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      209 2023-06-24 01:55:43.000000 gpubs-5/gpubs/log.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     7035 2023-06-24 02:40:36.000000 gpubs-5/gpubs/models.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     5065 2023-08-04 01:20:02.000000 gpubs-5/gpubs/parse.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1301 2023-06-24 01:55:43.000000 gpubs-5/gpubs/reference.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1899 2023-06-24 03:41:23.000000 gpubs-5/gpubs/search_words.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/gpubs.egg-info/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/PKG-INFO
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/SOURCES.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/dependency_links.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/requires.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/top_level.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-08-04 01:43:12.000000 gpubs-5/release-info.json
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/scripts/
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-5/scripts/create_search_terms_file.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-5/scripts/download_pubs.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-5/scripts/search.awk
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-08-04 01:43:34.223223 gpubs-5/setup.cfg
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1141 2023-06-24 02:06:26.000000 gpubs-5/setup.py
```

### Comparing `gpubs-4/gpubs/api.py` & `gpubs-5/gpubs/api.py`

 * *Files identical despite different names*

### Comparing `gpubs-4/gpubs/fetch.py` & `gpubs-5/gpubs/fetch.py`

 * *Files identical despite different names*

### Comparing `gpubs-4/gpubs/models.py` & `gpubs-5/gpubs/models.py`

 * *Files identical despite different names*

### Comparing `gpubs-4/gpubs/parse.py` & `gpubs-5/gpubs/parse.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,14 +30,34 @@
     data["MeshHeadingList"] = ",".join(mesh_heading_list)
 
     publication_types = element.findall(
         "MedlineCitation/Article/PublicationTypeList/PublicationType"
     )
     data["PublicationTypeList"] = ",".join([ptype.text for ptype in publication_types])
 
+    # find primary authors (1st, last, 2nd, next to last)
+    authors_list = element.findall("MedlineCitation/Article/AuthorList/Author")
+    # Sort authors based on their order within the list
+    authors = [
+        author.findtext(".//LastName", default="")
+        + ","
+        + author.findtext(".//ForeName", default="")
+        + " "
+        + author.findtext(".//Initials", default="")
+        for author in sorted(authors_list, key=lambda x: authors_list.index(x))
+    ]
+
+    data["Authors"] = ";".join(authors)
+    # data['FirstAuthor'] = authors[1] if authors else None  # Get the first author if authors list is not empty
+    # data['SecondAuthor'] = authors[2] if authors else None  # Get second author if authors list is not empty
+    # data['NextLastAuthor'] = authors[-2] if authors else None  # Get the second to last author if authors list is not empty
+    data["LastAuthor"] = (
+        authors[-1] if authors else None
+    )  # Get the last author if authors list is not empty
+
     return data
 
 
 def prune_df(df, length_threshold=405, verbose=2):
     # exclude articles with no abstract, no date, or abstracts that are too short (less than length_threshold letters)
     pruned_df = df[df["Abstract"].notna() & df["PublicationDate"].notna()]
```

### Comparing `gpubs-4/gpubs/reference.py` & `gpubs-5/gpubs/reference.py`

 * *Files identical despite different names*

### Comparing `gpubs-4/gpubs/search_words.py` & `gpubs-5/gpubs/search_words.py`

 * *Files identical despite different names*

### Comparing `gpubs-4/scripts/create_search_terms_file.sh` & `gpubs-5/scripts/create_search_terms_file.sh`

 * *Files identical despite different names*

### Comparing `gpubs-4/scripts/download_pubs.sh` & `gpubs-5/scripts/download_pubs.sh`

 * *Files identical despite different names*

### Comparing `gpubs-4/scripts/search.awk` & `gpubs-5/scripts/search.awk`

 * *Files identical despite different names*

### Comparing `gpubs-4/setup.py` & `gpubs-5/setup.py`

 * *Files identical despite different names*

