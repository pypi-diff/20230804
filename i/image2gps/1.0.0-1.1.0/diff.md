# Comparing `tmp/image2gps-1.0.0.tar.gz` & `tmp/image2gps-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2gps-1.0.0.tar", last modified: Tue Aug  1 19:46:54 2023, max compression
+gzip compressed data, was "image2gps-1.1.0.tar", last modified: Fri Aug  4 16:14:28 2023, max compression
```

## Comparing `image2gps-1.0.0.tar` & `image2gps-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-01 19:46:54.828089 image2gps-1.0.0/
--rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 image2gps-1.0.0/LICENSE.txt
--rw-r--r--   0 abionics   (501) staff       (20)     1631 2023-08-01 19:46:54.828158 image2gps-1.0.0/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      729 2023-08-01 19:43:25.000000 image2gps-1.0.0/README.md
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-01 19:46:54.827336 image2gps-1.0.0/image2gps/
--rw-r--r--   0 abionics   (501) staff       (20)      200 2023-08-01 19:16:00.000000 image2gps-1.0.0/image2gps/__init__.py
--rw-r--r--   0 abionics   (501) staff       (20)      853 2023-08-01 18:52:38.000000 image2gps-1.0.0/image2gps/config.py
--rw-r--r--   0 abionics   (501) staff       (20)      352 2023-08-01 19:16:41.000000 image2gps-1.0.0/image2gps/fix_piexif.py
--rw-r--r--   0 abionics   (501) staff       (20)      541 2023-08-01 18:52:38.000000 image2gps-1.0.0/image2gps/image2gps.py
--rw-r--r--   0 abionics   (501) staff       (20)      850 2023-08-01 18:52:38.000000 image2gps-1.0.0/image2gps/parse_location.py
--rw-r--r--   0 abionics   (501) staff       (20)     1100 2023-08-01 18:52:38.000000 image2gps-1.0.0/image2gps/parse_time.py
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-01 19:46:54.827995 image2gps-1.0.0/image2gps.egg-info/
--rw-r--r--   0 abionics   (501) staff       (20)     1631 2023-08-01 19:46:54.000000 image2gps-1.0.0/image2gps.egg-info/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      377 2023-08-01 19:46:54.000000 image2gps-1.0.0/image2gps.egg-info/SOURCES.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-01 19:46:54.000000 image2gps-1.0.0/image2gps.egg-info/dependency_links.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-01 19:46:54.000000 image2gps-1.0.0/image2gps.egg-info/not-zip-safe
--rw-r--r--   0 abionics   (501) staff       (20)       21 2023-08-01 19:46:54.000000 image2gps-1.0.0/image2gps.egg-info/requires.txt
--rw-r--r--   0 abionics   (501) staff       (20)       10 2023-08-01 19:46:54.000000 image2gps-1.0.0/image2gps.egg-info/top_level.txt
--rw-r--r--   0 abionics   (501) staff       (20)       79 2023-08-01 19:46:54.828431 image2gps-1.0.0/setup.cfg
--rw-r--r--   0 abionics   (501) staff       (20)     1560 2023-08-01 19:13:23.000000 image2gps-1.0.0/setup.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-04 16:14:28.062861 image2gps-1.1.0/
+-rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 image2gps-1.1.0/LICENSE.txt
+-rw-r--r--   0 abionics   (501) staff       (20)     1622 2023-08-04 16:14:28.062928 image2gps-1.1.0/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      722 2023-08-04 15:56:37.000000 image2gps-1.1.0/README.md
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-04 16:14:28.062160 image2gps-1.1.0/image2gps/
+-rw-r--r--   0 abionics   (501) staff       (20)      200 2023-08-04 16:14:01.000000 image2gps-1.1.0/image2gps/__init__.py
+-rw-r--r--   0 abionics   (501) staff       (20)      851 2023-08-04 15:56:37.000000 image2gps-1.1.0/image2gps/config.py
+-rw-r--r--   0 abionics   (501) staff       (20)      352 2023-08-01 19:16:41.000000 image2gps-1.1.0/image2gps/fix_piexif.py
+-rw-r--r--   0 abionics   (501) staff       (20)      674 2023-08-04 16:06:30.000000 image2gps-1.1.0/image2gps/image2gps.py
+-rw-r--r--   0 abionics   (501) staff       (20)      844 2023-08-04 15:56:37.000000 image2gps-1.1.0/image2gps/parse_coords.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1166 2023-08-04 16:00:07.000000 image2gps-1.1.0/image2gps/parse_time.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-04 16:14:28.062773 image2gps-1.1.0/image2gps.egg-info/
+-rw-r--r--   0 abionics   (501) staff       (20)     1622 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      375 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/SOURCES.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/dependency_links.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/not-zip-safe
+-rw-r--r--   0 abionics   (501) staff       (20)       21 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/requires.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       10 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/top_level.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       79 2023-08-04 16:14:28.063281 image2gps-1.1.0/setup.cfg
+-rw-r--r--   0 abionics   (501) staff       (20)     1558 2023-08-04 15:56:37.000000 image2gps-1.1.0/setup.py
```

### Comparing `image2gps-1.0.0/LICENSE.txt` & `image2gps-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `image2gps-1.0.0/README.md` & `image2gps-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # image2gps
 
-Extract time and location from image 🖼📍⏱️
+Extract time and coords from image 🖼📍⏱️
 
 ![demo](demo.jpg)
-_[Image source](https://github.com/ianare/exif-samples/blob/master/jpg/gps/DSCN0010.jpg)_
+_[Image source](https://github.com/ianare/exif-samples/blb/master/jpg/gps/DSCN0010.jpg)_
 
 ```python
 from image2gps import image2gps
 
-time, location = image2gps('demo.jpg')
-print(f'Image taken in {location} at {time}')
+time, coords = image2gps('demo.jpg')
+print(f'Image taken in {coords} at {time}')
 # >>> Image taken in (43.467, 11.885) at 2008-11-01 21:15:07
 ```
 
 This sample can be found [here](tests/sample.py)
 
 
 ## Installation
```

### Comparing `image2gps-1.0.0/image2gps/config.py` & `image2gps-1.1.0/image2gps/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import re
 
 import loguru
 
 TimeType = datetime.datetime | None
-LocationType = tuple[float, float] | None
+CoordsType = tuple[float, float] | None
 
 LOGGER = loguru.logger
-MIN_LOCATION_DATE = datetime.datetime(1960, 1, 1)
+MIN_LOCATION_TIME = datetime.datetime(1960, 1, 1)
 MAX_LOCATION_TIMEDELTA = datetime.timedelta(days=10)
 
 # todo more patterns
 DATETIME_PATTENS = {
     re.compile(r'^\d{4}:\d{2}:\d{2} \d{2}:\d{2}:\d{2}$'): '%Y:%m:%d %H:%M:%S',
     re.compile(r'^\d{4}:\d{2}:\d{2}$'): '%Y:%m:%d',
     re.compile(r'^\d{4}:\d{2}:\d{2} \d{2}:\d{2}:\d{2}[-+]\d{2}:\d{2}$'): '%Y:%m:%d %H:%M:%S%z',
```

### Comparing `image2gps-1.0.0/image2gps/parse_location.py` & `image2gps-1.1.0/image2gps/parse_coords.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import piexif
 
-from image2gps.config import LOGGER, LocationType
+from image2gps.config import LOGGER, CoordsType
 
 
-def parse_location(exif: dict) -> LocationType:
+def parse_coords(exif: dict) -> CoordsType:
     gps = exif.get('GPS')
     if gps is None or len(gps) == 0:
         return None
     lat = gps.get(piexif.GPSIFD.GPSLatitude)
     lon = gps.get(piexif.GPSIFD.GPSLongitude)
     if lat is None or lon is None:
         LOGGER.debug(f'Failed to parse GPS "{gps}"')
```

### Comparing `image2gps-1.0.0/image2gps/parse_time.py` & `image2gps-1.1.0/image2gps/parse_time.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import datetime
 
 import piexif
 
-from image2gps.config import LOGGER, MIN_LOCATION_DATE, MAX_LOCATION_TIMEDELTA, DATETIME_PATTENS, TimeType
+from image2gps.config import LOGGER, MIN_LOCATION_TIME, MAX_LOCATION_TIMEDELTA, DATETIME_PATTENS, TimeType
 
 
+# todo parse "2000:01:01 24:01:90", "24 Фев 2016 г."
 def parse_time(exif: dict) -> TimeType:
     zero_th = exif.get('0th', {})
     time = zero_th.get(piexif.ImageIFD.DateTime)
     if time is None:
         return None
     try:
         time = time.replace(b'\x00', b'').strip().decode().removesuffix('Z')
-        if len(time) == 0 or '0000:00:00' in time:
+        if len(time) == 0 or time.startswith('0000:00:00'):
             return None
         time = _string_to_datetime(time)
     except Exception as e:
         LOGGER.debug(f'Failed to parse time "{time}" due to {e} ({type(e)})')
         return None
     max_date = datetime.datetime.now() + MAX_LOCATION_TIMEDELTA
-    if time < MIN_LOCATION_DATE or time > max_date:
+    if time < MIN_LOCATION_TIME or time > max_date:
         LOGGER.debug(f'Date "{time}" is out of range')
         return None
     return time
 
 
 def _string_to_datetime(value: str) -> datetime.datetime:
     for pattern, timelike in DATETIME_PATTENS.items():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `image2gps-1.0.0/setup.py` & `image2gps-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     with open(filename) as file:
         return file.read()
 
 
 setup(
     name=PACKAGE_NAME,
     version=get_version(),
-    description='Extract time and location from image 🖼📍⏱️',
+    description='Extract time and coords from image 🖼📍⏱️',
     long_description=load_readme(),
     long_description_content_type='text/markdown',
     author='Alex Ermolaev',
     author_email='abionics.dev@gmail.com',
     url=URL,
     license='MIT',
     keywords='image gps location extract exif',
```

