# Comparing `tmp/klarf-reader-0.3.7.tar.gz` & `tmp/klarf-reader-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarf-reader-0.3.7.tar", last modified: Thu Jul 27 09:13:30 2023, max compression
+gzip compressed data, was "klarf-reader-0.3.8.tar", last modified: Fri Aug  4 11:07:07 2023, max compression
```

## Comparing `klarf-reader-0.3.7.tar` & `klarf-reader-0.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.987871 klarf-reader-0.3.7/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0      569 2023-07-27 09:13:30.986871 klarf-reader-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.949345 klarf-reader-0.3.7/klarf_reader/
--rw-rw-rw-   0        0        0     1218 2023-07-27 09:09:59.000000 klarf-reader-0.3.7/klarf_reader/klarf.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.970981 klarf-reader-0.3.7/klarf_reader/models/
--rw-rw-rw-   0        0        0     2559 2023-07-27 09:12:12.000000 klarf-reader-0.3.7/klarf_reader/models/klarf_content.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.975308 klarf-reader-0.3.7/klarf_reader/readers/
--rw-rw-rw-   0        0        0    14231 2023-07-27 09:11:10.000000 klarf-reader-0.3.7/klarf_reader/readers/klarf_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.980366 klarf-reader-0.3.7/klarf_reader/utils/
--rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.7/klarf_reader/utils/klarf_convert.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.968969 klarf-reader-0.3.7/klarf_reader.egg-info/
--rw-rw-rw-   0        0        0      569 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 09:13:30.988445 klarf-reader-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-27 09:12:25.000000 klarf-reader-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.983855 klarf-reader-0.3.7/tests/
--rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.7/tests/test_klarf.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:07:07.766423 klarf-reader-0.3.8/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      569 2023-08-04 11:07:07.764530 klarf-reader-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 11:07:07.726295 klarf-reader-0.3.8/klarf_reader/
+-rw-rw-rw-   0        0        0     1218 2023-07-27 09:09:59.000000 klarf-reader-0.3.8/klarf_reader/klarf.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:07:07.749216 klarf-reader-0.3.8/klarf_reader/models/
+-rw-rw-rw-   0        0        0     2559 2023-07-27 09:12:12.000000 klarf-reader-0.3.8/klarf_reader/models/klarf_content.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:07:07.752986 klarf-reader-0.3.8/klarf_reader/readers/
+-rw-rw-rw-   0        0        0    14354 2023-08-04 11:06:16.000000 klarf-reader-0.3.8/klarf_reader/readers/klarf_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:07:07.756879 klarf-reader-0.3.8/klarf_reader/utils/
+-rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.8/klarf_reader/utils/klarf_convert.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:07:07.746849 klarf-reader-0.3.8/klarf_reader.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-08-04 11:07:07.000000 klarf-reader-0.3.8/klarf_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-08-04 11:07:07.000000 klarf-reader-0.3.8/klarf_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:07:07.000000 klarf-reader-0.3.8/klarf_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 11:07:07.000000 klarf-reader-0.3.8/klarf_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-04 11:07:07.000000 klarf-reader-0.3.8/klarf_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:07:07.767464 klarf-reader-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-08-04 11:06:35.000000 klarf-reader-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:07:07.761412 klarf-reader-0.3.8/tests/
+-rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.8/tests/test_klarf.py
```

### Comparing `klarf-reader-0.3.7/LICENSE.txt` & `klarf-reader-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.7/PKG-INFO` & `klarf-reader-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.7
+Version: 0.3.8
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.7.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.7/README.md` & `klarf-reader-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.7/klarf_reader/klarf.py` & `klarf-reader-0.3.8/klarf_reader/klarf.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.7/klarf_reader/models/klarf_content.py` & `klarf-reader-0.3.8/klarf_reader/models/klarf_content.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.7/klarf_reader/readers/klarf_file_reader.py` & `klarf-reader-0.3.8/klarf_reader/readers/klarf_file_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,30 +270,33 @@
 
                 finebin = defect_paramters_values.get("finebinnumber")
                 finebin = int(finebin) if finebin is not None else 0
 
                 image_count = defect_paramters_values.get("imagecount")
                 image_count = int(image_count) if image_count is not None else 0
 
+                cluster_number = defect_paramters_values.get("clusternumber")
+                cluster_number = (
+                    int(cluster_number) if cluster_number is not None else 0
+                )
+
                 defects.append(
                     Defect(
                         id=int(defect_paramters_values.get("defectid")),
                         x_rel=float(defect_paramters_values.get("xrel")),
                         y_rel=float(defect_paramters_values.get("yrel")),
                         x_index=int(defect_paramters_values.get("xindex")),
                         y_index=int(defect_paramters_values.get("yindex")),
                         x_size=float(defect_paramters_values.get("xsize")),
                         y_size=float(defect_paramters_values.get("ysize")),
                         area=float(defect_paramters_values.get("defectarea")),
                         d_size=float(defect_paramters_values.get("dsize")),
                         class_number=int(defect_paramters_values.get("classnumber")),
                         test_id=int(defect_paramters_values.get("test")),
-                        cluster_number=int(
-                            defect_paramters_values.get("clusternumber")
-                        ),
+                        cluster_number=cluster_number,
                         image_count=image_count,
                         roughbin=roughbin,
                         finebin=finebin,
                         point=(x, y),
                         custom_attribute=defect_paramters_custom_values,
                     )
                 )
```

### Comparing `klarf-reader-0.3.7/klarf_reader/utils/klarf_convert.py` & `klarf-reader-0.3.8/klarf_reader/utils/klarf_convert.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.7/klarf_reader.egg-info/PKG-INFO` & `klarf-reader-0.3.8/klarf_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.7
+Version: 0.3.8
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.7.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.7/setup.py` & `klarf-reader-0.3.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.7"
+version = "0.3.8"
 
 setup(
     name="klarf-reader",
     version=version,
     packages=[
         "klarf_reader",
         "klarf_reader.models",
```

### Comparing `klarf-reader-0.3.7/tests/test_klarf.py` & `klarf-reader-0.3.8/tests/test_klarf.py`

 * *Files identical despite different names*

