# Comparing `tmp/s2dl-0.2.tar.gz` & `tmp/s2dl-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2dl-0.2.tar", last modified: Fri Jul 14 07:40:41 2023, max compression
+gzip compressed data, was "s2dl-0.3.tar", last modified: Fri Aug  4 00:41:44 2023, max compression
```

## Comparing `s2dl-0.2.tar` & `s2dl-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:40:41.247444 s2dl-0.2/
--rw-r--r--   0 NickW      (503) staff       (20)     1066 2023-07-14 06:27:57.000000 s2dl-0.2/LICENSE
--rw-r--r--   0 NickW      (503) staff       (20)     1570 2023-07-14 07:40:41.246920 s2dl-0.2/PKG-INFO
--rw-r--r--   0 NickW      (503) staff       (20)     1261 2023-07-14 07:31:14.000000 s2dl-0.2/README.md
-drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:40:41.243873 s2dl-0.2/s2dl/
--rw-r--r--   0 NickW      (503) staff       (20)      130 2023-07-14 06:53:41.000000 s2dl-0.2/s2dl/__init__.py
--rw-r--r--   0 NickW      (503) staff       (20)     7886 2023-07-14 06:56:01.000000 s2dl-0.2/s2dl/s2dl.py
-drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:40:41.246050 s2dl-0.2/s2dl.egg-info/
--rw-r--r--   0 NickW      (503) staff       (20)     1570 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/PKG-INFO
--rw-r--r--   0 NickW      (503) staff       (20)      168 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/SOURCES.txt
--rw-r--r--   0 NickW      (503) staff       (20)        1 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/dependency_links.txt
--rw-r--r--   0 NickW      (503) staff       (20)        5 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/top_level.txt
--rw-r--r--   0 NickW      (503) staff       (20)       38 2023-07-14 07:40:41.247616 s2dl-0.2/setup.cfg
--rw-r--r--   0 NickW      (503) staff       (20)      543 2023-07-14 07:36:30.000000 s2dl-0.2/setup.py
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-08-04 00:41:44.229135 s2dl-0.3/
+-rw-r--r--   0 NickW      (503) staff       (20)     1066 2023-08-03 12:24:52.000000 s2dl-0.3/LICENSE
+-rw-r--r--   0 NickW      (503) staff       (20)     1662 2023-08-04 00:41:44.228527 s2dl-0.3/PKG-INFO
+-rw-r--r--   0 NickW      (503) staff       (20)     1345 2023-08-04 00:37:43.000000 s2dl-0.3/README.md
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-08-04 00:41:44.224180 s2dl-0.3/s2dl/
+-rw-r--r--   0 NickW      (503) staff       (20)      130 2023-08-04 00:23:07.000000 s2dl-0.3/s2dl/__init__.py
+-rw-r--r--   0 NickW      (503) staff       (20)     8933 2023-08-04 00:33:40.000000 s2dl-0.3/s2dl/s2dl.py
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-08-04 00:41:44.227020 s2dl-0.3/s2dl.egg-info/
+-rw-r--r--   0 NickW      (503) staff       (20)     1662 2023-08-04 00:41:44.000000 s2dl-0.3/s2dl.egg-info/PKG-INFO
+-rw-r--r--   0 NickW      (503) staff       (20)      168 2023-08-04 00:41:44.000000 s2dl-0.3/s2dl.egg-info/SOURCES.txt
+-rw-r--r--   0 NickW      (503) staff       (20)        1 2023-08-04 00:41:44.000000 s2dl-0.3/s2dl.egg-info/dependency_links.txt
+-rw-r--r--   0 NickW      (503) staff       (20)        5 2023-08-04 00:41:44.000000 s2dl-0.3/s2dl.egg-info/top_level.txt
+-rw-r--r--   0 NickW      (503) staff       (20)       38 2023-08-04 00:41:44.229513 s2dl-0.3/setup.cfg
+-rw-r--r--   0 NickW      (503) staff       (20)      551 2023-08-04 00:40:54.000000 s2dl-0.3/setup.py
```

### Comparing `s2dl-0.2/LICENSE` & `s2dl-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s2dl-0.2/PKG-INFO` & `s2dl-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: s2dl
-Version: 0.2
-Summary: S2DL is a Python library for downloading Sentinel-2 L1C satellite imagery data.
+Version: 0.3
+Summary: S2DL is a Python library for downloading Sentinel-2 L1C and L2A satellite imagery data.
 Home-page: https://github.com/DPIRD-DMA/S2DL
 Author: Nick Wright
 Author-email: nicholas.wright@dpird.wa.gov.au
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # S2DL - Sentinel 2 Downloader
 
-S2DL is a Python library for downloading Sentinel-2 L1C satellite imagery data.
+S2DL is a Python library for downloading Sentinel-2 L1C and L2A satellite imagery data.
 ## Features
 
 - Download Sentinel-2 product data using product IDs
 
 ## Installation
 
 You can install the S2DL library via pip:
@@ -27,32 +27,34 @@
 
 Here's a simple usage example:
 
 ```python
 from s2dl import fetch_single_sentinel_product
 from pathlib import Path
 
-product_id = "S2B_MSIL1C_20190523T150729_N0207_R082_T18MZA_20190523T183104"
+product_id = "S2A_MSIL2A_20220111T021351_N0301_R060_T50HLK_20220111T041611"
 target_directory = Path("./data")
+target_directory.mkdir(exist_ok=True)
 
 # Fetch and save a single Sentinel-2 product's data
 scene_dir = fetch_single_sentinel_product(product_id, target_directory)
 ```
 
 For downloading multiple products:
 
 ```python
 from s2dl import fetch_multiple_sentinel_products
 from pathlib import Path
 
 product_ids = [
-    "S2B_MSIL1C_20190523T150729_N0207_R082_T18MZA_20190523T183104",
+    "S2A_MSIL2A_20220111T021351_N0301_R060_T50HLK_20220111T041611",
     "S2A_MSIL1C_20230712T032521_N0509_R018_T52WFD_20230712T051642",
 ]
 target_directory = Path("./data")
+target_directory.mkdir(exist_ok=True)
 
 # Fetch and save multiple Sentinel-2 products' data
 scene_dirs = fetch_multiple_sentinel_products(product_ids, target_directory)
 ```
 
 ## Contributions
```

### Comparing `s2dl-0.2/README.md` & `s2dl-0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # S2DL - Sentinel 2 Downloader
 
-S2DL is a Python library for downloading Sentinel-2 L1C satellite imagery data.
+S2DL is a Python library for downloading Sentinel-2 L1C and L2A satellite imagery data.
 ## Features
 
 - Download Sentinel-2 product data using product IDs
 
 ## Installation
 
 You can install the S2DL library via pip:
@@ -17,32 +17,34 @@
 
 Here's a simple usage example:
 
 ```python
 from s2dl import fetch_single_sentinel_product
 from pathlib import Path
 
-product_id = "S2B_MSIL1C_20190523T150729_N0207_R082_T18MZA_20190523T183104"
+product_id = "S2A_MSIL2A_20220111T021351_N0301_R060_T50HLK_20220111T041611"
 target_directory = Path("./data")
+target_directory.mkdir(exist_ok=True)
 
 # Fetch and save a single Sentinel-2 product's data
 scene_dir = fetch_single_sentinel_product(product_id, target_directory)
 ```
 
 For downloading multiple products:
 
 ```python
 from s2dl import fetch_multiple_sentinel_products
 from pathlib import Path
 
 product_ids = [
-    "S2B_MSIL1C_20190523T150729_N0207_R082_T18MZA_20190523T183104",
+    "S2A_MSIL2A_20220111T021351_N0301_R060_T50HLK_20220111T041611",
     "S2A_MSIL1C_20230712T032521_N0509_R018_T52WFD_20230712T051642",
 ]
 target_directory = Path("./data")
+target_directory.mkdir(exist_ok=True)
 
 # Fetch and save multiple Sentinel-2 products' data
 scene_dirs = fetch_multiple_sentinel_products(product_ids, target_directory)
 ```
 
 ## Contributions
```

### Comparing `s2dl-0.2/s2dl/s2dl.py` & `s2dl-0.3/s2dl/s2dl.py`

 * *Files 14% similar despite different names*

```diff
@@ -137,14 +137,15 @@
     session: requests.Session,
     base_url: str,
     product_id: str,
     grid_square: str,
     latitude_band: str,
     path_number: str,
     target_directory: Path,
+    processing_level: str,
 ):
     """
     Downloads Sentinel-2 product data from a given URL and saves it to a target
     directory.
 
     Args:
         session (requests.Session): The request session. base_url (str): The
@@ -156,16 +157,18 @@
     Returns:
         Path: The directory path where the scene data is saved.
     """
     download_url = build_download_url(
         base_url, product_id, grid_square, latitude_band, path_number
     )
     target_directory.mkdir(parents=True, exist_ok=True)
-
-    xml_url = f"{download_url}MTD_MSIL1C.xml"
+    if processing_level == "L1C":
+        xml_url = f"{download_url}MTD_MSIL1C.xml"
+    else:
+        xml_url = f"{download_url}MTD_MSIL2A.xml"
     xml_dom_tree = get_xml(session, xml_url)
 
     image_file_nodes = xml_dom_tree.getElementsByTagName("IMAGE_FILE")
 
     image_files_urls = [
         f"{download_url}{node.firstChild.data}.jp2" for node in image_file_nodes  # type: ignore  # noqa: E501
     ]
@@ -184,71 +187,115 @@
         unit="Scene file",
     ):
         save_file_from_url(session, url, file_path)
 
     return scene_dir
 
 
+def validate_product_id(product_id: str) -> None:
+    """
+    Validates a Sentinel-2 product ID.
+
+    Args:
+        product_id (str): The Sentinel-2 product ID.
+
+    Returns:
+        None
+    """
+    if not isinstance(product_id, str):
+        raise TypeError("Product ID must be a string")
+
+    if not product_id.startswith("S2"):
+        raise ValueError("Product ID must start with 'S2'")
+
+
+def get_processing_level(product_id: str) -> str:
+    """
+    Extracts the processing level from a Sentinel-2 product ID.
+
+    Args:
+        product_id (str): The Sentinel-2 product ID.
+
+    Returns:
+        str: The processing level.
+    """
+    return product_id.split("_")[1][-3:]
+
+
+def get_base_url(processing_level: str) -> str:
+    """
+    Gets the base URL for Sentinel-2 data, depending on the processing level.
+
+    Args:
+        processing_level (str): The Sentinel-2 processing level L1C or L2A.
+
+    Returns:
+        str: The base URL for Sentinel-2 data.
+    """
+    if processing_level == "L1C":
+        return "https://storage.googleapis.com/gcp-public-data-sentinel-2/tiles"
+    else:
+        return "https://storage.googleapis.com/gcp-public-data-sentinel-2/L2/tiles"
+
+
 def fetch_single_sentinel_product(
     product_id: str,
     target_directory: Path,
-    base_url: str = "https://storage.googleapis.com/gcp-public-data-sentinel-2/tiles",
 ) -> Path:
     """
     Fetches and saves a single Sentinel-2 product's data.
 
     Args:
-        base_url (str): The base URL for Sentinel-2 data. product_id (str): The
-        Sentinel-2 product ID. target_directory (Path): The directory where the
-        downloaded data should be saved.
+        product_id (str): The Sentinel-2 product ID. target_directory (Path):
+        The directory where the downloaded data should be saved.
 
     Returns:
         Path: The directory path where the scene data is saved.
     """
+    validate_product_id(product_id)
+    processing_level = get_processing_level(product_id)
+    base_url = get_base_url(processing_level)
     session = create_request_session()
     grid_square, latitude_band, path_number = extract_details_from_product_id(
         product_id
     )
 
     scene_dir = fetch_product_data(
         session,
         base_url,
         product_id,
         grid_square,
         latitude_band,
         path_number,
         target_directory,
+        processing_level,
     )
 
     return scene_dir
 
 
 def fetch_multiple_sentinel_products(
     product_ids: List[str],
     target_directory: Path,
-    base_url: str = "https://storage.googleapis.com/gcp-public-data-sentinel-2/tiles",
 ) -> List[Path]:
     """
     Fetches and saves multiple Sentinel-2 products' data.
 
     Args:
         product_ids (List[str]): A list of Sentinel-2 product IDs.
         target_directory (Path): The directory where the downloaded data should
-        be saved. base_url (str, optional): The base URL for Sentinel-2 data.
-        Defaults to
-        "https://storage.googleapis.com/gcp-public-data-sentinel-2/tiles".
+        be saved.
 
     Returns:
         List[Path]: A list of directory paths where each scene's data is saved.
     """
     scene_dirs = []
     for product_id in tqdm(
         product_ids, leave=False, desc="Downloading multiple scenes", unit="Scene"
     ):
         scene_dirs.append(
             fetch_single_sentinel_product(
-                base_url=base_url,
                 product_id=product_id,
                 target_directory=target_directory,
             )
         )
     return scene_dirs
```

### Comparing `s2dl-0.2/s2dl.egg-info/PKG-INFO` & `s2dl-0.3/s2dl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: s2dl
-Version: 0.2
-Summary: S2DL is a Python library for downloading Sentinel-2 L1C satellite imagery data.
+Version: 0.3
+Summary: S2DL is a Python library for downloading Sentinel-2 L1C and L2A satellite imagery data.
 Home-page: https://github.com/DPIRD-DMA/S2DL
 Author: Nick Wright
 Author-email: nicholas.wright@dpird.wa.gov.au
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # S2DL - Sentinel 2 Downloader
 
-S2DL is a Python library for downloading Sentinel-2 L1C satellite imagery data.
+S2DL is a Python library for downloading Sentinel-2 L1C and L2A satellite imagery data.
 ## Features
 
 - Download Sentinel-2 product data using product IDs
 
 ## Installation
 
 You can install the S2DL library via pip:
@@ -27,32 +27,34 @@
 
 Here's a simple usage example:
 
 ```python
 from s2dl import fetch_single_sentinel_product
 from pathlib import Path
 
-product_id = "S2B_MSIL1C_20190523T150729_N0207_R082_T18MZA_20190523T183104"
+product_id = "S2A_MSIL2A_20220111T021351_N0301_R060_T50HLK_20220111T041611"
 target_directory = Path("./data")
+target_directory.mkdir(exist_ok=True)
 
 # Fetch and save a single Sentinel-2 product's data
 scene_dir = fetch_single_sentinel_product(product_id, target_directory)
 ```
 
 For downloading multiple products:
 
 ```python
 from s2dl import fetch_multiple_sentinel_products
 from pathlib import Path
 
 product_ids = [
-    "S2B_MSIL1C_20190523T150729_N0207_R082_T18MZA_20190523T183104",
+    "S2A_MSIL2A_20220111T021351_N0301_R060_T50HLK_20220111T041611",
     "S2A_MSIL1C_20230712T032521_N0509_R018_T52WFD_20230712T051642",
 ]
 target_directory = Path("./data")
+target_directory.mkdir(exist_ok=True)
 
 # Fetch and save multiple Sentinel-2 products' data
 scene_dirs = fetch_multiple_sentinel_products(product_ids, target_directory)
 ```
 
 ## Contributions
```

### Comparing `s2dl-0.2/setup.py` & `s2dl-0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name="s2dl",
-    version="0.2",
+    version="0.3",
     url="https://github.com/DPIRD-DMA/S2DL",
     author="Nick Wright",
     author_email="nicholas.wright@dpird.wa.gov.au",
-    description="S2DL is a Python library for downloading Sentinel-2 L1C satellite imagery data.",
+    description="S2DL is a Python library for downloading Sentinel-2 L1C and L2A satellite imagery data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[],
 )
```

