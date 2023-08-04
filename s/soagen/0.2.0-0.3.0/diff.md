# Comparing `tmp/soagen-0.2.0.tar.gz` & `tmp/soagen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soagen-0.2.0.tar", last modified: Tue Aug  1 19:13:18 2023, max compression
+gzip compressed data, was "soagen-0.3.0.tar", last modified: Fri Aug  4 16:22:18 2023, max compression
```

## Comparing `soagen-0.2.0.tar` & `soagen-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.831808 soagen-0.2.0/
--rw-rw-rw-   0        0        0      515 2023-08-01 18:55:45.000000 soagen-0.2.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1844 2023-08-01 19:13:18.830810 soagen-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.2.0/README.md
--rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 19:13:18.831808 soagen-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.788809 soagen-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.810808 soagen-0.2.0/src/soagen/
--rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/__init__.py
--rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.2.0/src/soagen/column.py
--rw-rw-rw-   0        0        0     5029 2023-08-01 15:35:54.000000 soagen-0.2.0/src/soagen/config.py
--rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/configurable.py
--rw-rw-rw-   0        0        0    19130 2023-08-01 16:02:29.000000 soagen-0.2.0/src/soagen/cpp.py
--rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/errors.py
--rw-rw-rw-   0        0        0    10577 2023-08-01 13:38:11.000000 soagen-0.2.0/src/soagen/header_file.py
-drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.824809 soagen-0.2.0/src/soagen/hpp/
--rw-rw-rw-   0        0        0     5621 2023-08-01 18:58:28.000000 soagen-0.2.0/src/soagen/hpp/.clang-format
--rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/allocator.hpp
--rw-rw-rw-   0        0        0    31484 2023-08-01 17:51:18.000000 soagen-0.2.0/src/soagen/hpp/column_traits.hpp
-drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.828811 soagen-0.2.0/src/soagen/hpp/generated/
--rw-rw-rw-   0        0        0     9857 2023-08-01 18:58:28.000000 soagen-0.2.0/src/soagen/hpp/generated/compressed_pair.hpp
--rw-rw-rw-   0        0        0     2935 2023-08-01 18:58:28.000000 soagen-0.2.0/src/soagen/hpp/generated/core.hpp
--rw-rw-rw-   0        0        0     7897 2023-08-01 18:58:29.000000 soagen-0.2.0/src/soagen/hpp/generated/functions.hpp
--rw-rw-rw-   0        0        0    43876 2023-08-01 18:58:31.000000 soagen-0.2.0/src/soagen/hpp/generated/preprocessor.hpp
--rw-rw-rw-   0        0        0      420 2023-08-01 15:39:54.000000 soagen-0.2.0/src/soagen/hpp/generated/version.hpp
--rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/header_end.hpp
--rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/header_start.hpp
--rw-rw-rw-   0        0        0    15734 2023-08-01 12:49:39.000000 soagen-0.2.0/src/soagen/hpp/iterator.hpp
--rw-rw-rw-   0        0        0    25587 2023-08-01 15:53:13.000000 soagen-0.2.0/src/soagen/hpp/meta.hpp
--rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/mixins.hpp
--rw-rw-rw-   0        0        0     7841 2023-08-01 16:10:41.000000 soagen-0.2.0/src/soagen/hpp/row.hpp
-drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.829811 soagen-0.2.0/src/soagen/hpp/single/
--rw-rw-rw-   0        0        0   239553 2023-08-01 18:58:31.000000 soagen-0.2.0/src/soagen/hpp/single/soagen.hpp
--rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/soagen.hpp
--rw-rw-rw-   0        0        0    56712 2023-08-01 18:52:09.000000 soagen-0.2.0/src/soagen/hpp/table.hpp
--rw-rw-rw-   0        0        0    42558 2023-08-01 18:52:19.000000 soagen-0.2.0/src/soagen/hpp/table_traits.hpp
--rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.2.0/src/soagen/includes.py
--rw-rw-rw-   0        0        0     1534 2023-08-01 12:05:38.000000 soagen-0.2.0/src/soagen/injectors.py
--rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/log.py
--rw-rw-rw-   0        0        0    22887 2023-08-01 15:36:32.000000 soagen-0.2.0/src/soagen/main.py
--rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/metavars.py
--rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/natvis_file.py
--rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/paths.py
--rw-rw-rw-   0        0        0     6128 2023-07-30 10:13:46.000000 soagen-0.2.0/src/soagen/preprocessor.py
--rw-rw-rw-   0        0        0     2516 2023-08-01 12:07:40.000000 soagen-0.2.0/src/soagen/schemas.py
--rw-rw-rw-   0        0        0    69042 2023-08-01 18:41:49.000000 soagen-0.2.0/src/soagen/struct.py
--rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/type_list.py
--rw-rw-rw-   0        0        0     2879 2023-08-01 11:51:16.000000 soagen-0.2.0/src/soagen/utils.py
--rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.2.0/src/soagen/variable.py
--rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/version.py
--rw-rw-rw-   0        0        0        6 2023-08-01 15:39:54.000000 soagen-0.2.0/src/soagen/version.txt
--rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.2.0/src/soagen/writer.py
-drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.815808 soagen-0.2.0/src/soagen.egg-info/
--rw-rw-rw-   0        0        0     1844 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1387 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.2.0/src/soagen.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.651346 soagen-0.3.0/
+-rw-rw-rw-   0        0        0      751 2023-08-04 16:21:27.000000 soagen-0.3.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2087 2023-08-04 16:22:18.650346 soagen-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1893 2023-08-03 12:48:33.000000 soagen-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 16:22:18.651346 soagen-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.606346 soagen-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.629346 soagen-0.3.0/src/soagen/
+-rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/__init__.py
+-rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.3.0/src/soagen/column.py
+-rw-rw-rw-   0        0        0     5264 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/config.py
+-rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/configurable.py
+-rw-rw-rw-   0        0        0    19130 2023-08-01 16:02:29.000000 soagen-0.3.0/src/soagen/cpp.py
+-rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/errors.py
+-rw-rw-rw-   0        0        0    11685 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/header_file.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.646349 soagen-0.3.0/src/soagen/hpp/
+-rw-rw-rw-   0        0        0     5693 2023-08-04 16:20:02.000000 soagen-0.3.0/src/soagen/hpp/.clang-format
+-rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/allocator.hpp
+-rw-rw-rw-   0        0        0    32796 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/column_traits.hpp
+-rw-rw-rw-   0        0        0    29618 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/core.hpp
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.649346 soagen-0.3.0/src/soagen/hpp/generated/
+-rw-rw-rw-   0        0        0     9858 2023-08-04 16:20:03.000000 soagen-0.3.0/src/soagen/hpp/generated/compressed_pair.hpp
+-rw-rw-rw-   0        0        0     6006 2023-08-04 16:20:03.000000 soagen-0.3.0/src/soagen/hpp/generated/functions.hpp
+-rw-rw-rw-   0        0        0    43899 2023-08-04 16:20:05.000000 soagen-0.3.0/src/soagen/hpp/generated/preprocessor.hpp
+-rw-rw-rw-   0        0        0      420 2023-08-03 12:44:35.000000 soagen-0.3.0/src/soagen/hpp/generated/version.hpp
+-rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/header_end.hpp
+-rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/header_start.hpp
+-rw-rw-rw-   0        0        0    15734 2023-08-01 12:49:39.000000 soagen-0.3.0/src/soagen/hpp/iterator.hpp
+-rw-rw-rw-   0        0        0     5469 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/mixins.hpp
+-rw-rw-rw-   0        0        0     7841 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/row.hpp
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.649346 soagen-0.3.0/src/soagen/hpp/single/
+-rw-rw-rw-   0        0        0   233911 2023-08-04 16:21:27.000000 soagen-0.3.0/src/soagen/hpp/single/soagen.hpp
+-rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/soagen.hpp
+-rw-rw-rw-   0        0        0    56712 2023-08-01 18:52:09.000000 soagen-0.3.0/src/soagen/hpp/table.hpp
+-rw-rw-rw-   0        0        0    34607 2023-08-04 16:21:27.000000 soagen-0.3.0/src/soagen/hpp/table_traits.hpp
+-rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.3.0/src/soagen/includes.py
+-rw-rw-rw-   0        0        0     1534 2023-08-01 12:05:38.000000 soagen-0.3.0/src/soagen/injectors.py
+-rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/log.py
+-rw-rw-rw-   0        0        0    22644 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/main.py
+-rw-rw-rw-   0        0        0     3529 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/metavars.py
+-rw-rw-rw-   0        0        0     6453 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/natvis_file.py
+-rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/paths.py
+-rw-rw-rw-   0        0        0     5873 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/preprocessor.py
+-rw-rw-rw-   0        0        0     2516 2023-08-01 12:07:40.000000 soagen-0.3.0/src/soagen/schemas.py
+-rw-rw-rw-   0        0        0    69716 2023-08-04 16:21:27.000000 soagen-0.3.0/src/soagen/struct.py
+-rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/type_list.py
+-rw-rw-rw-   0        0        0     1657 2023-08-03 12:36:06.000000 soagen-0.3.0/src/soagen/utils.py
+-rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.3.0/src/soagen/variable.py
+-rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/version.py
+-rw-rw-rw-   0        0        0        6 2023-08-03 12:44:35.000000 soagen-0.3.0/src/soagen/version.txt
+-rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.3.0/src/soagen/writer.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.635346 soagen-0.3.0/src/soagen.egg-info/
+-rw-rw-rw-   0        0        0     2087 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1353 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.3.0/src/soagen.egg-info/zip-safe
```

### Comparing `soagen-0.2.0/LICENSE.txt` & `soagen-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/PKG-INFO` & `soagen-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,21 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.3.0
+
+-   Added `hpp.combined`
+-   Added `std::integral_constant<size_t>` to the overload set used by `for_each_column()`
+-   Added support for constructing rows from all `std::tuple`-like types
+-   Optimized bulk-swap operations
+
 ## v0.2.0
 
 -   Added `structs.annotations`
 -   Added `structs.attributes`
 -   Added `auto` option for `structs.default_constructible`
 -   Added `soagen::row_base`
 -   Added `soagen::table_base`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.2.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.3.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,17 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.2.0 - Added `structs.annotations` - Added
+sponsors/marzer # Changelog ## v0.3.0 - Added `hpp.combined` - Added `std::
+integral_constant` to the overload set used by `for_each_column()` - Added
+support for constructing rows from all `std::tuple`-like types - Optimized
+bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
 `structs.attributes` - Added `auto` option for `structs.default_constructible`
 - Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
 iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
 Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
 columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
 First public release ð&#xFE0F;
```

### Comparing `soagen-0.2.0/pyproject.toml` & `soagen-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	'Development Status :: 3 - Alpha',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: C++',
 	'Topic :: Software Development :: Code Generators',
 	'Topic :: Utilities',
 ]
 dependencies = [
-	'misk >= 0.7.0',
+	'misk >= 0.8.1',
 	'tomli',
 	'schema != 0.7.5',
 	'colorama',
 	'trieregex',
 ]
 dynamic = ['version', 'readme']
```

### Comparing `soagen-0.2.0/src/soagen/column.py` & `soagen-0.3.0/src/soagen/column.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/config.py` & `soagen-0.3.0/src/soagen/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -84,29 +84,33 @@
             self.all_structs = StructInjector(self, self.all_structs)
 
             # structs
             self.structs = [(k, v) for k, v in self.structs.items()]
             for i in range(len(self.structs)):
                 with SchemaContext(rf"struct '{self.structs[i][0]}'"):
                     self.structs[i] = Struct(self, self.structs[i][0], self.structs[i][1])
-            self.structs.sort(key=lambda s: s.name)
+            self.structs = tuple(sorted(self.structs, key=lambda s: s.name))
             self.struct_types = TypeList([s.type for s in self.structs])
             self.meta.push('struct_names', ', '.join([s.name for s in self.structs]))
             self.meta.push('struct_types', ', '.join([s.type for s in self.structs]))
             self.meta.push('qualified_struct_names', ', '.join([s.qualified_type for s in self.structs]))
             self.meta.push('qualified_struct_types', ', '.join([s.qualified_type for s in self.structs]))
             index = 0
             for struct in self.structs:
                 struct.set_index(index)
                 index += 1
 
-            # output file configs
-            self.hpp = HeaderFile(self, self.structs, self.hpp)
+            # hpp files (needs a little bit of special handling because of the 'combined' option)
+            self.hpp = [HeaderFile(self, self.structs, self.hpp)]
+            self.hpp += [*self.hpp[0].additional_header_files]
+            self.hpp[0].additional_header_files = []
+
+            # all outputs
             self.natvis = NatvisFile(self, self.structs)
-            self.all_outputs = [self.natvis, self.hpp]
+            self.all_outputs = [self.natvis, *self.hpp]
             log.d('\n  -> '.join([str(self.path)] + [str(o.path) for o in self.all_outputs]))
             for o in self.all_outputs:
                 if o.path.is_dir():
                     raise Error(rf"invalid output '{o.path}': outputs cannot be existing directories")
                 if o.path == self.path:
                     raise Error(rf"invalid output '{o.path}': outputs cannot overwrite input")
                 if o.path.name.lower() == r'soagen.hpp':
```

### Comparing `soagen-0.2.0/src/soagen/configurable.py` & `soagen-0.3.0/src/soagen/configurable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/cpp.py` & `soagen-0.3.0/src/soagen/cpp.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/errors.py` & `soagen-0.3.0/src/soagen/errors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/header_file.py` & `soagen-0.3.0/src/soagen/header_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 # Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 # See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 # SPDX-License-Identifier: MIT
 
 import re
+from pathlib import Path
 
 from . import utils
 from .column import *
 from .configurable import Configurable
 from .includes import *
 from .metavars import *
 from .schemas import *
@@ -17,29 +18,41 @@
 
 
 class HeaderFile(Configurable):
     __schema = Schema(
         {
             Optional(r'banner', default=''): Stripped(str),
             Optional(r'brief', default=''): Stripped(str),
+            Optional(r'combined', default=True): bool,
             Optional(r'footer', default=''): Stripped(str),
             Optional(r'header', default=''): Stripped(str),
             Optional(r'includes', default=dict): {object: object},
             Optional(r'prologue', default=''): Stripped(str),
         }
     )
 
-    def __init__(self, config, structs, vals, path=''):
+    def __init__(self, config, structs, vals):
         super().__init__(config)
-        self.path = path
-        if not self.path:
-            self.path = self.config.path.with_suffix('.hpp')
         self.__dict__.update(HeaderFile.__schema.validate(vals))
 
-        self.structs = structs if utils.is_collection(structs) else [structs]
+        self.path = self.config.path.with_suffix('.hpp')
+
+        self.structs = tuple(utils.coerce_collection(structs))
+        assert len(self.structs) >= 1
+
+        self.additional_header_files = []
+        if not self.combined:
+            self.additional_header_files = [HeaderFile(config, struct, vals) for struct in self.structs[1:]]
+            self.structs = tuple(self.structs[:1])
+            self.path = Path(self.config.path.parent, rf'{self.structs[0].name}.hpp')
+
+        self.meta = MetaVars()
+        for prefix in (r'file_', r'file::'):
+            self.meta.push(rf'{prefix}name', self.path.name)
+            self.meta.push(rf'{prefix}path', str(self.path))
 
         # includes
         with SchemaContext('includes'):
             self.includes = Includes(config, self.includes)
 
             # add any includes requested by member structs
             self.includes.internal = set(self.includes.internal)
@@ -61,250 +74,247 @@
         if self.banner:
             self.banner = [s.rstrip() for s in self.banner.split('\n')]
             self.banner = [re.sub(r'(^|\n)// ?', r'\1', s) for s in self.banner]
             self.banner = [rf'// {s}'.rstrip() for s in self.banner]
             self.banner = '\n'.join(self.banner)
 
     def write(self, o: Writer):
-        if self.banner:
+        with MetaScope(self):
+            if self.banner:
+                o(rf'//{"-"*(120 - o.indent_width - 2)}')
+                o(self.banner)
+
+            o(rf'//{"-"*(120 - o.indent_width - 2)}')
+            o(rf'// This file was generated by soagen v{VERSION_STRING} - do not modify it directly')
+            o(rf'// https://marzer.github.io/soagen')
             o(rf'//{"-"*(120 - o.indent_width - 2)}')
-            o(self.banner)
+            o(rf'#pragma once')
+            o()
+
+            if o.doxygen:
+                o(
+                    rf'''
+                /// @file
+                /// @brief {self.brief}
+                ///
+                /// @note The code and documentation in this file were generated by soagen - https://marzer.github.io/soagen
+                '''
+                )
 
-        o(rf'//{"-"*(120 - o.indent_width - 2)}')
-        o(rf'// This file was generated by soagen v{VERSION_STRING} - do not modify it directly')
-        o(rf'// https://marzer.github.io/soagen')
-        o(rf'//{"-"*(120 - o.indent_width - 2)}')
-        o(rf'#pragma once')
-        o()
+            # internal includes (#include "blah.h")
+            if self.includes.internal:
+                o()
+                for inc in self.includes.internal:
+                    o(rf'#include "{inc}"')
 
-        if o.doxygen:
+            # stick the prologue here so users can use it to override the various
+            # SOAGEN_ macros etc before including soagen.hpp
             o(
                 rf'''
-            /// @file
-            /// @brief {self.brief}
-            ///
-            /// @note The code and documentation in this file were generated by soagen - https://marzer.github.io/soagen
+            {self.prologue}
             '''
             )
 
-        # internal includes (#include "blah.h")
-        if self.includes.internal:
-            o()
-            for inc in self.includes.internal:
-                o(rf'#include "{inc}"')
+            # soagen.hpp
+            o(
+                rf'''
+            #include <soagen.hpp>
+            #if SOAGEN_VERSION_MAJOR != {VERSION[0]} || SOAGEN_VERSION_MINOR < {VERSION[1]}
+                #error soagen version mismatch - expected v{VERSION[0]}.{VERSION[1]}.X
+            #endif
+            '''
+            )
 
-        # stick the prologue here so users can use it to override the various
-        # SOAGEN_ macros etc before including soagen.hpp
-        o(
-            rf'''
-        {self.prologue}
-        '''
-        )
-
-        # soagen.hpp
-        o(
-            rf'''
-          #include <soagen.hpp>
-          #if SOAGEN_VERSION_MAJOR != {VERSION[0]} || SOAGEN_VERSION_MINOR < {VERSION[1]}
-            #error soagen version mismatch - expected v{VERSION[0]}.{VERSION[1]}.X
-          #endif
-          '''
-        )
-
-        # external/system includes (#include <blah.h>)
-        # (deferred until later so we can take advantage of detect_includes() for the whole file)
-        o('\n\n// __SOAGEN_EXTERNAL_HEADERS\n\n')
-
-        # misc preprocessor boilerplate
-        o(
-            rf'''
-        SOAGEN_PUSH_WARNINGS;
-        SOAGEN_DISABLE_SPAM_WARNINGS;
-        #if SOAGEN_CLANG >= 16
-            #pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-        #endif
-        #if SOAGEN_MSVC
-            #pragma inline_recursion(on)
-        #endif
-        #if SOAGEN_MSVC_LIKE
-            #pragma push_macro("min")
-            #pragma push_macro("max")
-            #undef min
-            #undef max
-        #endif
-        '''
-        )
+            # external/system includes (#include <blah.h>)
+            # (deferred until later so we can take advantage of detect_includes() for the whole file)
+            o('\n\n// __SOAGEN_EXTERNAL_HEADERS\n\n')
 
-        # doxygen crap
-        if o.doxygen:
+            # misc preprocessor boilerplate
             o(
                 rf'''
-            //{"-"*(120 - o.indent_width - 2)}
-            // doxygen safeguards
-            //{"-"*(120 - o.indent_width - 2)}
+            SOAGEN_PUSH_WARNINGS;
+            SOAGEN_DISABLE_SPAM_WARNINGS;
+            #if SOAGEN_CLANG >= 16
+                #pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
+            #endif
+            #if SOAGEN_MSVC
+                #pragma inline_recursion(on)
+            #endif
+            #if SOAGEN_MSVC_LIKE
+                #pragma push_macro("min")
+                #pragma push_macro("max")
+                #undef min
+                #undef max
+            #endif
+            '''
+            )
 
-            #if defined(DOXYGEN) || defined(__DOXYGEN) || defined(__DOXYGEN__) \
-                || defined(__doxygen__) || defined(__POXY__) || defined(__poxy__)
+            # doxygen crap
+            if o.doxygen:
+                o(
+                    rf'''
+                //{"-"*(120 - o.indent_width - 2)}
+                // doxygen safeguards
+                //{"-"*(120 - o.indent_width - 2)}
 
-            #ifndef SOAGEN_DOXYGEN
-                #define SOAGEN_DOXYGEN 1
-            #endif
-            #ifndef SOAGEN_MAKE_NAME
-                #define SOAGEN_MAKE_NAME(...) static_assert(true)
-            #endif
-            #ifndef SOAGEN_MAKE_COLUMN
-                #define SOAGEN_MAKE_COLUMN(...) static_assert(true)
-            #endif
-            #ifndef SOAGEN_NODISCARD
-                #define SOAGEN_NODISCARD
-            #endif
-            #ifndef SOAGEN_NODISCARD_CTOR
-                #define SOAGEN_NODISCARD_CTOR
-            #endif
-            #ifndef SOAGEN_INLINE_GETTER
-                #define SOAGEN_INLINE_GETTER inline
-            #endif
-            #ifndef SOAGEN_PURE_GETTER
-                #define SOAGEN_PURE_GETTER
-            #endif
-            #ifndef SOAGEN_PURE_INLINE_GETTER
-                #define SOAGEN_PURE_INLINE_GETTER inline
-            #endif
-            #ifndef SOAGEN_ALWAYS_INLINE
-                #define SOAGEN_ALWAYS_INLINE inline
-            #endif
-            #ifndef SOAGEN_CPP20_CONSTEXPR
-                #define SOAGEN_CPP20_CONSTEXPR constexpr
-            #endif
-            #ifndef SOAGEN_HIDDEN
-                #define SOAGEN_HIDDEN(...)
-            #endif
-            #ifndef SOAGEN_HIDDEN_BASE
-                #define SOAGEN_HIDDEN_BASE(...)
-            #endif
-            #ifndef SOAGEN_HIDDEN_CONSTRAINT
-                #define SOAGEN_HIDDEN_CONSTRAINT(...)
-            #endif
-            #ifndef SOAGEN_HIDDEN_PARAM
-                #define SOAGEN_HIDDEN_PARAM(...)
-            #endif
-            #ifndef SOAGEN_ENABLE_IF_T
-                #define SOAGEN_ENABLE_IF_T(T, ...) T
-            #endif
-            #ifndef SOAGEN_ENABLE_IF
-                #define SOAGEN_ENABLE_IF(...)
-            #endif
-            #ifndef SOAGEN_REQUIRES
-                #define SOAGEN_REQUIRES(...)
-            #endif
-            #ifndef SOAGEN_EMPTY_BASES
-                #define SOAGEN_EMPTY_BASES
-            #endif
-            #ifndef SOAGEN_COLUMN
-                #define SOAGEN_COLUMN(...)
-            #endif
-            #ifndef SOAGEN_ALIGNED_COLUMN
-                #define SOAGEN_ALIGNED_COLUMN(...)
-            #endif
-            #if !defined(POXY_IMPLEMENTATION_DETAIL) && !(defined(__POXY__) || defined(__poxy__))
-                #define POXY_IMPLEMENTATION_DETAIL(...) __VA_ARGS__
-            #endif
+                #if defined(DOXYGEN) || defined(__DOXYGEN) || defined(__DOXYGEN__) \
+                    || defined(__doxygen__) || defined(__POXY__) || defined(__poxy__)
 
-            #endif // doxygen
+                #ifndef SOAGEN_DOXYGEN
+                    #define SOAGEN_DOXYGEN 1
+                #endif
+                #ifndef SOAGEN_MAKE_NAME
+                    #define SOAGEN_MAKE_NAME(...) static_assert(true)
+                #endif
+                #ifndef SOAGEN_MAKE_COLUMN
+                    #define SOAGEN_MAKE_COLUMN(...) static_assert(true)
+                #endif
+                #ifndef SOAGEN_NODISCARD
+                    #define SOAGEN_NODISCARD
+                #endif
+                #ifndef SOAGEN_NODISCARD_CTOR
+                    #define SOAGEN_NODISCARD_CTOR
+                #endif
+                #ifndef SOAGEN_INLINE_GETTER
+                    #define SOAGEN_INLINE_GETTER inline
+                #endif
+                #ifndef SOAGEN_PURE_GETTER
+                    #define SOAGEN_PURE_GETTER
+                #endif
+                #ifndef SOAGEN_PURE_INLINE_GETTER
+                    #define SOAGEN_PURE_INLINE_GETTER inline
+                #endif
+                #ifndef SOAGEN_ALWAYS_INLINE
+                    #define SOAGEN_ALWAYS_INLINE inline
+                #endif
+                #ifndef SOAGEN_CPP20_CONSTEXPR
+                    #define SOAGEN_CPP20_CONSTEXPR constexpr
+                #endif
+                #ifndef SOAGEN_HIDDEN
+                    #define SOAGEN_HIDDEN(...)
+                #endif
+                #ifndef SOAGEN_HIDDEN_BASE
+                    #define SOAGEN_HIDDEN_BASE(...)
+                #endif
+                #ifndef SOAGEN_HIDDEN_CONSTRAINT
+                    #define SOAGEN_HIDDEN_CONSTRAINT(...)
+                #endif
+                #ifndef SOAGEN_HIDDEN_PARAM
+                    #define SOAGEN_HIDDEN_PARAM(...)
+                #endif
+                #ifndef SOAGEN_ENABLE_IF_T
+                    #define SOAGEN_ENABLE_IF_T(T, ...) T
+                #endif
+                #ifndef SOAGEN_ENABLE_IF
+                    #define SOAGEN_ENABLE_IF(...)
+                #endif
+                #ifndef SOAGEN_REQUIRES
+                    #define SOAGEN_REQUIRES(...)
+                #endif
+                #ifndef SOAGEN_EMPTY_BASES
+                    #define SOAGEN_EMPTY_BASES
+                #endif
+                #ifndef SOAGEN_COLUMN
+                    #define SOAGEN_COLUMN(...)
+                #endif
+                #ifndef SOAGEN_ALIGNED_COLUMN
+                    #define SOAGEN_ALIGNED_COLUMN(...)
+                #endif
+                #if !defined(POXY_IMPLEMENTATION_DETAIL) && !(defined(__POXY__) || defined(__poxy__))
+                    #define POXY_IMPLEMENTATION_DETAIL(...) __VA_ARGS__
+                #endif
 
-            '''
-            )
+                #endif // doxygen
 
-        # forward declarations
-        o(
-            rf'''
-        //{"-"*(120 - o.indent_width - 2)}
-        // forward declarations + soagen internal boilerplate
-        //{"-"*(120 - o.indent_width - 2)}
-        '''
-        )
-        with HiddenFromDoxygen(o), ClangFormatOff(o):
-            with Namespace(o, self.config.namespace):
-                for struct in self.structs:
-                    with MetaScope(self.config.meta_stack, struct.meta):
-                        struct.write_forward_declarations(o)
-            o()
-            with Namespace(o, 'soagen'):
-                for struct in self.structs:
-                    with MetaScope(self.config.meta_stack, struct.meta):
-                        struct.write_soagen_specializations(o)
-            o()
-            with Namespace(o, 'soagen::detail'):
-                names = set()
-                for struct in self.structs:
-                    for col in struct.columns:
-                        names.add(col.name)
-                names = sorted(list(names))
-                for name in names:
-                    sanitized_name = name.replace('::', '_')
-                    pp_define = rf'SOAGEN_NAME_{sanitized_name}'
-                    o(
-                        rf'''
-                    #ifndef {pp_define}
-                        #define {pp_define}
-                        SOAGEN_MAKE_NAME({name});
-                    #endif
-                    '''
-                    )
-                for struct in self.structs:
-                    with MetaScope(self.config.meta_stack, struct.meta):
-                        struct.write_soagen_detail_specializations(o)
+                '''
+                )
 
-        # header
-        if self.header:
+            # forward declarations
             o(
                 rf'''
             //{"-"*(120 - o.indent_width - 2)}
-            // header
+            // forward declarations + soagen internal boilerplate
             //{"-"*(120 - o.indent_width - 2)}
-
             '''
             )
-            o(self.header)
+            with HiddenFromDoxygen(o), ClangFormatOff(o):
+                with Namespace(o, self.config.namespace):
+                    for struct in self.structs:
+                        struct.write_forward_declarations(o)
+                o()
+                with Namespace(o, 'soagen'):
+                    for struct in self.structs:
+                        struct.write_soagen_specializations(o)
+                o()
+                with Namespace(o, 'soagen::detail'):
+                    names = set()
+                    for struct in self.structs:
+                        for col in struct.columns:
+                            names.add(col.name)
+                    names = sorted(list(names))
+                    for name in names:
+                        sanitized_name = name.replace('::', '_')
+                        pp_define = rf'SOAGEN_NAME_{sanitized_name}'
+                        o(
+                            rf'''
+                        #ifndef {pp_define}
+                            #define {pp_define}
+                            SOAGEN_MAKE_NAME({name});
+                        #endif
+                        '''
+                        )
+                    for struct in self.structs:
+                        struct.write_soagen_detail_specializations(o)
+
+            # header
+            if self.header:
+                o(
+                    rf'''
+                //{"-"*(120 - o.indent_width - 2)}
+                // header
+                //{"-"*(120 - o.indent_width - 2)}
+
+                '''
+                )
+                o(self.header)
 
-        # structs (class definitions, then outline member implementations)
-        for struct in self.structs:
-            with MetaScope(self.config.meta_stack, struct.meta):
+            # structs (class definitions, then outline member implementations)
+            for struct in self.structs:
                 o(
                     rf'''
                 //{"-"*(120 - o.indent_width - 2)}
                 // {struct.name}
                 //{"-"*(120 - o.indent_width - 2)}
                 '''
                 )
                 with Namespace(o, self.config.namespace):
                     struct.write_class_definition(o)
                     with HiddenFromDoxygen(o):
                         struct.write_outline_member_implementations(o)
 
-        # footer
-        if self.footer:
+            # footer
+            if self.footer:
+                o(
+                    rf'''
+                //{"-"*(120 - o.indent_width - 2)}
+                // footer
+                //{"-"*(120 - o.indent_width - 2)}
+
+                {self.footer}
+                '''
+                )
+
+            # clean up preprocessor boilerplate
             o(
                 rf'''
-            //{"-"*(120 - o.indent_width - 2)}
-            // footer
-            //{"-"*(120 - o.indent_width - 2)}
-
-            {self.footer}
-            '''
+            #if SOAGEN_MSVC_LIKE
+                #pragma pop_macro("min")
+                #pragma pop_macro("max")
+            #endif
+            #if SOAGEN_MSVC
+                #pragma inline_recursion(off)
+            #endif
+            SOAGEN_POP_WARNINGS;'''
             )
 
-        # clean up preprocessor boilerplate
-        o(
-            rf'''
-        #if SOAGEN_MSVC_LIKE
-            #pragma pop_macro("min")
-            #pragma pop_macro("max")
-        #endif
-        #if SOAGEN_MSVC
-            #pragma inline_recursion(off)
-        #endif
-        SOAGEN_POP_WARNINGS;'''
-        )
-
 
 __all__ = [r'HeaderFile']
```

### Comparing `soagen-0.2.0/src/soagen/hpp/.clang-format` & `soagen-0.3.0/src/soagen/hpp/.clang-format`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 AlwaysBreakAfterDefinitionReturnType: None
 AlwaysBreakAfterReturnType: None
 AlwaysBreakBeforeMultilineStrings: false
 AlwaysBreakTemplateDeclarations: Yes
 AttributeMacros:
     - SOAGEN_ABSTRACT_INTERFACE
     - SOAGEN_CALLCONV
+    - SOAGEN_CPP23_STATIC_CONSTEXPR
     - SOAGEN_EMPTY_BASES
     - SOAGEN_NODISCARD_CLASS
     - SOAGEN_TRIVIAL_ABI
     - SOAGEN_VECTORCALL
 BinPackArguments: false
 BinPackParameters: false
 BraceWrapping:
@@ -166,14 +167,15 @@
     - SOAGEN_CONST_GETTER
     - SOAGEN_CONST_GETTER
     - SOAGEN_CONST_INLINE_GETTER
     - SOAGEN_CONST_INLINE_GETTER
     - SOAGEN_CONSTEVAL
     - SOAGEN_CONSTRAINED_TEMPLATE
     - SOAGEN_CPP20_CONSTEXPR
+    - SOAGEN_CPP23_STATIC_CONSTEXPR
     - SOAGEN_DECLSPEC
     - SOAGEN_HIDDEN_BASE
     - SOAGEN_HIDDEN_CONSTRAINT
     - SOAGEN_INLINE_GETTER
     - SOAGEN_MALLOC
     - SOAGEN_NEVER_INLINE
     - SOAGEN_NODISCARD
```

### Comparing `soagen-0.2.0/src/soagen/hpp/allocator.hpp` & `soagen-0.3.0/src/soagen/hpp/allocator.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/hpp/column_traits.hpp` & `soagen-0.3.0/src/soagen/hpp/column_traits.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 #include "generated/functions.hpp"
 #include "header_start.hpp"
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
+#define soagen_storage_ptr(...) soagen::assume_aligned<alignof(storage_type)>(__VA_ARGS__)
+
 /// @cond
 namespace soagen::detail
 {
 	// a base class for the column traits that handles all the non-alignment-dependent stuff
 	// (to minimize template instantiation explosion)
 	template <typename StorageType>
 	struct column_traits_base
@@ -27,100 +29,96 @@
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& get(std::byte* ptr) noexcept
 		{
 			SOAGEN_ASSUME(ptr != nullptr);
 
-			return *SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(soagen::assume_aligned<alignof(storage_type)>(ptr)));
+			return *SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(soagen_storage_ptr(ptr)));
 		}
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
 		static constexpr const storage_type& get(const std::byte* ptr) noexcept
 		{
 			SOAGEN_ASSUME(ptr != nullptr);
 
-			return *SOAGEN_LAUNDER(
-				reinterpret_cast<const storage_type*>(soagen::assume_aligned<alignof(storage_type)>(ptr)));
+			return *SOAGEN_LAUNDER(reinterpret_cast<const storage_type*>(soagen_storage_ptr(ptr)));
 		}
 
 		//--- default construction -------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& default_construct(std::byte* destination) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				return *(
-					std::start_lifetime_as<storage_type>(soagen::assume_aligned<alignof(storage_type)>(destination)));
+				return *(std::start_lifetime_as<storage_type>(soagen_storage_ptr(destination)));
 			}
 			else
 			{
 #endif
-				return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-							 storage_type);
+				return *(::new (static_cast<void*>(soagen_storage_ptr(destination))) storage_type);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			}
 #endif
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& default_construct(std::byte* buffer, size_t element_index) //
+		static constexpr storage_type& default_construct(std::byte* buffer, size_t index) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
-			return default_construct(buffer + element_index * sizeof(storage_type));
+			return default_construct(buffer + index * sizeof(storage_type));
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
-		static void default_construct(std::byte* buffer, size_t start_index, size_t count) //
+		static void default_construct(std::byte* buffer, size_t index, size_t count) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 			SOAGEN_ASSUME(count);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 2022071
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				std::start_lifetime_as_array<storage_type>(soagen::assume_aligned<alignof(storage_type)>(destination),
-														   count);
+				std::start_lifetime_as_array<storage_type>(soagen_storage_ptr(destination), count);
 			}
 			else
 #endif
 				if constexpr (std::is_nothrow_default_constructible_v<storage_type>
 							  || std::is_trivially_destructible_v<storage_type>)
 			{
-				for (const size_t e = start_index + count; start_index < e; start_index++)
-					default_construct(buffer, start_index);
+				for (const size_t e = index + count; index < e; index++)
+					default_construct(buffer, index);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
-				size_t i = start_index;
+				size_t i = index;
 
 				try
 				{
-					for (const size_t e = start_index + count; i < e; i++)
+					for (const size_t e = index + count; i < e; i++)
 						default_construct(buffer, i);
 				}
 				catch (...)
 				{
-					for (; i-- > start_index;)
+					for (; i-- > index;)
 						destruct(buffer, i);
 					throw;
 				}
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
@@ -250,47 +248,45 @@
 					return construct_from_emplacer(
 						destination,
 						static_cast<Args&&>(args)...,
 						std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
 				else if constexpr (is_constructible_with_memcpy<Args&&...>)
 				{
-					std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
-								soagen::assume_aligned<alignof(storage_type)>(&args)...,
-								sizeof(storage_type));
+					std::memcpy(soagen_storage_ptr(destination), soagen_storage_ptr(&args)..., sizeof(storage_type));
 
 					return get(destination);
 				}
 				else if constexpr (std::is_aggregate_v<storage_type>)
 				{
-					return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
+					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
 								 storage_type{ static_cast<Args&&>(args)... });
 				}
 				else
 				{
-					return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
+					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
 								 storage_type(static_cast<Args&&>(args)...));
 				}
 			}
 		}
 
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& construct_at(std::byte* buffer, size_t element_index, Args&&... args) //
+		static constexpr storage_type& construct_at(std::byte* buffer, size_t index, Args&&... args) //
 			noexcept(is_nothrow_constructible<Args&&...>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			if constexpr (sizeof...(Args) == 0)
 			{
-				return default_construct(buffer + element_index * sizeof(storage_type));
+				return default_construct(buffer + index * sizeof(storage_type));
 			}
 			else
 			{
-				return construct(buffer + element_index * sizeof(storage_type), static_cast<Args&&>(args)...);
+				return construct(buffer + index * sizeof(storage_type), static_cast<Args&&>(args)...);
 			}
 		}
 
 		//--- move-construction ----------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_move_constructible = is_trivially_constructible<storage_type&&>;
 
@@ -344,25 +340,26 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_move_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_construct(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  std::byte* source_buffer,
-													  size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& move_construct(std::byte* dest_buffer,
+											size_t dest_index,
+											std::byte* source_buffer,
+											size_t source_index) //
 			noexcept(std::is_nothrow_move_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return move_construct(dest_buffer + dest_element_index * sizeof(storage_type),
-								  source_buffer + source_element_index * sizeof(storage_type));
+			return move_construct(dest_buffer + dest_index * sizeof(storage_type),
+								  source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- copy-construction ----------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_copy_constructible = is_trivially_constructible<const storage_type&>;
 
 		static constexpr bool is_copy_constructible =
@@ -415,25 +412,26 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_constructible)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_construct(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  const std::byte* source_buffer,
-													  size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& copy_construct(std::byte* dest_buffer,
+											size_t dest_index,
+											const std::byte* source_buffer,
+											size_t source_index) //
 			noexcept(is_nothrow_copy_constructible)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return copy_construct(dest_buffer + dest_element_index * sizeof(storage_type),
-								  source_buffer + source_element_index * sizeof(storage_type));
+			return copy_construct(dest_buffer + dest_index * sizeof(storage_type),
+								  source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- destruction ----------------------------------------------------------------------------------------------
 
 		SOAGEN_ATTR(nonnull)
 		static constexpr void destruct([[maybe_unused]] std::byte* target) //
 			noexcept(std::is_nothrow_destructible_v<storage_type>)
@@ -443,23 +441,23 @@
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
 				get(target).~storage_type();
 			}
 		}
 
 		SOAGEN_ATTR(nonnull)
-		static constexpr void destruct([[maybe_unused]] std::byte* buffer,	  //
-									   [[maybe_unused]] size_t element_index) //
+		static constexpr void destruct([[maybe_unused]] std::byte* buffer, //
+									   [[maybe_unused]] size_t index)	   //
 			noexcept(std::is_nothrow_destructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
-				destruct(buffer + element_index * sizeof(storage_type));
+				destruct(buffer + index * sizeof(storage_type));
 			}
 		}
 
 		//--- move-assignment ------------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_move_assignable =
 			is_constructible_with_memcpy<storage_type&&> || std::is_trivially_move_assignable_v<storage_type>;
@@ -474,25 +472,26 @@
 				? true
 				: (std::is_move_assignable_v<storage_type> ? std::is_nothrow_move_assignable_v<storage_type>
 														   : std::is_nothrow_destructible_v<storage_type>
 																 && std::is_nothrow_move_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_assign(std::byte* destination, void* source) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& move_assign(std::byte* destination, void* source) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
-							soagen::assume_aligned<alignof(storage_type)>(static_cast<std::byte*>(source)),
+				std::memcpy(soagen_storage_ptr(destination),
+							soagen_storage_ptr(static_cast<std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_move_assignable || std::is_move_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<storage_type&&>(get(static_cast<std::byte*>(source)));
@@ -507,25 +506,26 @@
 				destruct(destination);
 				return move_construct(destination, static_cast<std::byte*>(source));
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_assign(std::byte* dest_buffer,
-												   size_t dest_element_index,
-												   std::byte* source_buffer,
-												   size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& move_assign(std::byte* dest_buffer,
+										 size_t dest_index,
+										 std::byte* source_buffer,
+										 size_t source_index) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return move_assign(dest_buffer + dest_element_index * sizeof(storage_type),
-							   source_buffer + source_element_index * sizeof(storage_type));
+			return move_assign(dest_buffer + dest_index * sizeof(storage_type),
+							   source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- copy-assignment ------------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_copy_assignable =
 			is_constructible_with_memcpy<const storage_type&> || std::is_trivially_copy_assignable_v<storage_type>;
 
@@ -539,25 +539,26 @@
 				? true
 				: (std::is_copy_assignable_v<storage_type> ? std::is_nothrow_copy_assignable_v<storage_type>
 														   : std::is_nothrow_destructible_v<storage_type>
 																 && std::is_nothrow_copy_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_assign(std::byte* destination, const std::byte* source) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& copy_assign(std::byte* destination, const std::byte* source) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
-							soagen::assume_aligned<alignof(storage_type)>(static_cast<const std::byte*>(source)),
+				std::memcpy(soagen_storage_ptr(destination),
+							soagen_storage_ptr(static_cast<const std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_copy_assignable || std::is_copy_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<const storage_type&>(get(source));
@@ -572,87 +573,137 @@
 				destruct(destination);
 				return copy_construct(destination, source);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_assign(std::byte* dest_buffer,
-												   size_t dest_element_index,
-												   const std::byte* source_buffer,
-												   size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& copy_assign(std::byte* dest_buffer,
+										 size_t dest_index,
+										 const std::byte* source_buffer,
+										 size_t source_index) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return copy_assign(dest_buffer + dest_element_index * sizeof(storage_type),
-							   source_buffer + source_element_index * sizeof(storage_type));
+			return copy_assign(dest_buffer + dest_index * sizeof(storage_type),
+							   source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- swap -----------------------------------------------------------------------------------------------------
 
-		static constexpr bool is_swappable =
-			std::is_swappable_v<storage_type> || (is_move_constructible && is_move_assignable);
-
-		static constexpr bool is_nothrow_swappable = std::is_swappable_v<storage_type>
-													   ? std::is_nothrow_swappable_v<storage_type>
-													   : (is_nothrow_move_constructible && is_nothrow_move_assignable);
+		static constexpr bool is_trivially_swappable =
+			is_trivially_copyable
+			&& (std::is_scalar_v<storage_type> || std::is_fundamental_v<storage_type>
+				|| !std::is_swappable_v<storage_type> // we don't want to usurp user-defined swap() functions
+			);
+
+		static constexpr bool is_swappable = is_trivially_swappable //
+										  || std::is_swappable_v<storage_type>
+										  || (is_move_constructible && is_move_assignable);
+
+		static constexpr bool is_nothrow_swappable =
+			is_trivially_swappable
+			|| (std::is_swappable_v<storage_type> ? std::is_nothrow_swappable_v<storage_type>
+												  : (is_nothrow_move_constructible && is_nothrow_move_assignable));
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_swappable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr void swap(std::byte* lhs, std::byte* rhs) //
+		SOAGEN_CPP20_CONSTEXPR
+		static void swap(std::byte* lhs, std::byte* rhs) //
 			noexcept(is_nothrow_swappable)
 		{
 			SOAGEN_ASSUME(lhs != nullptr);
 			SOAGEN_ASSUME(rhs != nullptr);
 			SOAGEN_ASSUME(lhs != rhs);
 
-			if constexpr (std::is_swappable_v<storage_type>)
+			if constexpr (is_trivially_swappable)
+			{
+				alignas(storage_type) std::byte buf[sizeof(storage_type)];
+				std::memcpy(soagen_storage_ptr(buf), soagen_storage_ptr(lhs), sizeof(storage_type));
+				std::memcpy(soagen_storage_ptr(lhs), soagen_storage_ptr(rhs), sizeof(storage_type));
+				std::memcpy(soagen_storage_ptr(rhs), soagen_storage_ptr(buf), sizeof(storage_type));
+			}
+			else if constexpr (std::is_swappable_v<storage_type>)
 			{
 				using std::swap;
 				swap(get(lhs), get(rhs));
 			}
-			else if constexpr (is_move_constructible && is_move_assignable)
+			else
 			{
+				static_assert(is_move_constructible && is_move_assignable);
+
 				storage_type temp(static_cast<storage_type&&>(get(lhs)));
 				move_assign(lhs, rhs);
 				move_assign(rhs, &temp);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_swappable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr void swap(std::byte* lhs_buffer,
-								   size_t lhs_element_index,
-								   std::byte* rhs_buffer,
-								   size_t rhs_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static void swap(std::byte* lhs_buffer,
+						 size_t lhs_index,
+						 std::byte* rhs_buffer,
+						 size_t rhs_index,
+						 size_t count = 1) //
 			noexcept(is_nothrow_swappable)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
-			return swap(lhs_buffer + lhs_element_index * sizeof(storage_type),
-						rhs_buffer + rhs_element_index * sizeof(storage_type));
+			if SOAGEN_UNLIKELY(!count)
+				return;
+
+			lhs_buffer = soagen_storage_ptr(lhs_buffer + lhs_index * sizeof(storage_type));
+			rhs_buffer = soagen_storage_ptr(rhs_buffer + rhs_index * sizeof(storage_type));
+
+			[[maybe_unused]] SOAGEN_CPP23_STATIC_CONSTEXPR size_t trivial_buf_size = 2048u / sizeof(storage_type);
+
+			if constexpr (is_trivially_swappable && trivial_buf_size > 1)
+			{
+				for (size_t i = 0; i < count; i += trivial_buf_size)
+				{
+					const auto num = soagen::min(trivial_buf_size, count - i);
+
+					alignas(storage_type) std::byte buf[sizeof(storage_type) * trivial_buf_size];
+					std::memcpy(buf, lhs_buffer, sizeof(storage_type) * num);
+					std::memcpy(lhs_buffer, rhs_buffer, sizeof(storage_type) * num);
+					std::memcpy(rhs_buffer, buf, sizeof(storage_type) * num);
+
+					lhs_buffer = soagen_storage_ptr(lhs_buffer + trivial_buf_size * sizeof(storage_type));
+					rhs_buffer = soagen_storage_ptr(rhs_buffer + trivial_buf_size * sizeof(storage_type));
+				}
+			}
+			else
+			{
+				const auto end = lhs_buffer + count * sizeof(storage_type);
+				for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
+				{
+					swap(lhs_buffer, rhs_buffer);
+				}
+			}
 		}
 
 		//--- memmove ---------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_trivially_copyable)
 		static constexpr void memmove(std::byte* dest_buffer,
-									  size_t dest_element_index,
+									  size_t dest_index,
 									  const std::byte* source_buffer,
-									  size_t source_element_index,
-									  size_t count) noexcept
+									  size_t source_index,
+									  size_t count = 1) noexcept
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			std::memmove(dest_buffer + dest_element_index * sizeof(storage_type),
-						 source_buffer + source_element_index * sizeof(storage_type),
+			std::memmove(soagen_storage_ptr(dest_buffer + dest_index * sizeof(storage_type)),
+						 soagen_storage_ptr(source_buffer + source_index * sizeof(storage_type)),
 						 count * sizeof(storage_type));
 		}
 
 		//--- equality -------------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
 		SOAGEN_NODISCARD
@@ -666,25 +717,25 @@
 			return get(lhs) == get(rhs);
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
 		SOAGEN_NODISCARD
 		SOAGEN_ATTR(nonnull)
 		static constexpr bool equal(const std::byte* lhs_buffer,
-									size_t lhs_start_index,
+									size_t lhs_index,
 									const std::byte* rhs_buffer,
-									size_t rhs_start_index,
+									size_t rhs_index,
 									size_t count = 1) //
 			noexcept(is_nothrow_equality_comparable<storage_type>)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
-			lhs_buffer += lhs_start_index * sizeof(storage_type);
-			rhs_buffer += rhs_start_index * sizeof(storage_type);
+			lhs_buffer += lhs_index * sizeof(storage_type);
+			rhs_buffer += rhs_index * sizeof(storage_type);
 			const auto end = lhs_buffer + count * sizeof(storage_type);
 
 			for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
 			{
 				if (!equal(lhs_buffer, rhs_buffer))
 					return false;
 			}
@@ -706,24 +757,24 @@
 			return get(lhs) < get(rhs);
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_less_than_comparable<storage_type>)
 		SOAGEN_NODISCARD
 		SOAGEN_ATTR(nonnull)
 		static constexpr bool less_than(const std::byte* lhs_buffer,
-										size_t lhs_element_index,
+										size_t lhs_index,
 										const std::byte* rhs_buffer,
-										size_t rhs_element_index) //
+										size_t rhs_index) //
 			noexcept(is_nothrow_less_than_comparable<storage_type>)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
-			return less_than(lhs_buffer + lhs_element_index * sizeof(storage_type),
-							 rhs_buffer + rhs_element_index * sizeof(storage_type));
+			return less_than(lhs_buffer + lhs_index * sizeof(storage_type),
+							 rhs_buffer + rhs_index * sizeof(storage_type));
 		}
 	};
 }
 /// @endcond
 
 namespace soagen
 {
@@ -827,8 +878,10 @@
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
 }
 /// @endcond
 
+#undef soagen_storage_ptr
+
 #include "header_end.hpp"
```

### Comparing `soagen-0.2.0/src/soagen/hpp/generated/compressed_pair.hpp` & `soagen-0.3.0/src/soagen/hpp/generated/compressed_pair.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //#---------------------------------------------------------------------------------------------------------------------
 //#     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //#---------------------------------------------------------------------------------------------------------------------
 
 #pragma once
 
-#include "../meta.hpp"
+#include "../core.hpp"
 #include "../header_start.hpp"
 
 /// @cond
 
 namespace soagen
 {
 	namespace detail
@@ -142,23 +142,25 @@
 			SOAGEN_COMPRESSED_PAIR_BASE_GETTERS(First, first, *this);
 			SOAGEN_COMPRESSED_PAIR_BASE_GETTERS(Second, second, *this);
 		};
 
 #undef SOAGEN_COMPRESSED_PAIR_BASE_DEFAULTS
 #undef SOAGEN_COMPRESSED_PAIR_BASE_GETTERS
 	}
+
 	template <typename First, typename Second>
 	class SOAGEN_EMPTY_BASES compressed_pair //
 		: public detail::compressed_pair_base<First, Second>
 	{
 	  private:
 		using base = detail::compressed_pair_base<First, Second>;
 
 	  public:
-		using first_type  = First;
+		using first_type = First;
+
 		using second_type = Second;
 
 		SOAGEN_NODISCARD_CTOR
 		compressed_pair() = default;
 
 		SOAGEN_NODISCARD_CTOR
 		compressed_pair(const compressed_pair&) = default;
```

### Comparing `soagen-0.2.0/src/soagen/hpp/generated/preprocessor.hpp` & `soagen-0.3.0/src/soagen/hpp/generated/preprocessor.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,14 @@
 #ifndef SOAGEN_ARCH_X64
 	#if SOAGEN_ARCH_BITNESS == 64
 		#define SOAGEN_ARCH_X64 1
 	#else
 		#define SOAGEN_ARCH_X64 0
 	#endif
 #endif
-/// \brief `1` when targeting any 64-bit architecture, otherwise `0`.
 
 #ifdef _WIN32
 	#define SOAGEN_WINDOWS 1
 #else
 	#define SOAGEN_WINDOWS 0
 #endif
 #ifdef __unix__
@@ -424,14 +423,20 @@
 
 #if defined(__cpp_constexpr) && __cpp_constexpr >= 202002L
 	#define SOAGEN_CPP20_CONSTEXPR constexpr
 #else
 	#define SOAGEN_CPP20_CONSTEXPR
 #endif
 
+#if defined(__cpp_constexpr) && __cpp_constexpr >= 202211L
+	#define SOAGEN_CPP23_STATIC_CONSTEXPR static constexpr
+#else
+	#define SOAGEN_CPP23_STATIC_CONSTEXPR constexpr
+#endif
+
 #ifndef SOAGEN_CONCEPTS
 	#if defined(__cpp_concepts) && __cpp_concepts >= 201907
 		#define SOAGEN_CONCEPTS 1
 	#else
 		#define SOAGEN_CONCEPTS 0
 	#endif
 #endif
@@ -833,16 +838,14 @@
 			SOAGEN_POP_WARNINGS;                                                                                       \
 			static_assert(true)
 	#else
 		#define SOAGEN_ENABLE_WARNINGS static_assert(true)
 	#endif
 #endif
 
-/// \brief Re-enables compiler warnings again after using #SOAGEN_DISABLE_WARNINGS.
-
 #ifndef SOAGEN_HAS_CONSTEVAL
 	#if defined(__cpp_consteval) && __cpp_consteval >= 201811 && (!SOAGEN_MSVC || SOAGEN_MSVC >= 1934)                 \
 		&& (!SOAGEN_CLANG || SOAGEN_CLANG >= 15)
 		#define SOAGEN_HAS_CONSTEVAL 1
 	#else
 		#define SOAGEN_HAS_CONSTEVAL SOAGEN_DOXYGEN
 	#endif
```

### Comparing `soagen-0.2.0/src/soagen/hpp/header_end.hpp` & `soagen-0.3.0/src/soagen/hpp/header_end.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/hpp/header_start.hpp` & `soagen-0.3.0/src/soagen/hpp/header_start.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/hpp/iterator.hpp` & `soagen-0.3.0/src/soagen/hpp/iterator.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/hpp/meta.hpp` & `soagen-0.3.0/src/soagen/hpp/core.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
-#include "generated/core.hpp"
+#include "generated/preprocessor.hpp"
 SOAGEN_DISABLE_WARNINGS;
 
+#include <cstdint>
+#include <cstddef>
+#include <cstdlib>
+#include <cstring>
+#include <numeric>
+#include <type_traits>
+#include <new>
+#include <utility>
+#include <memory>
+#include <optional>
+
 #ifndef SOAGEN_COLUMN_SPAN_TYPE
-	#if defined(MUU_SPAN_H) || defined(MUU_SPAN_HPP)
-		#define SOAGEN_COLUMN_SPAN_TYPE				  muu::span
-		#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 1
-	#elif SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
+	#if SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
 		#include <span>
 		#define SOAGEN_COLUMN_SPAN_TYPE std::span
 	#elif SOAGEN_HAS_INCLUDE(<muu/span.h>)
 		#include <muu/span.h>
 		#define SOAGEN_COLUMN_SPAN_TYPE				  muu::span
 		#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 1
 	#elif SOAGEN_HAS_INCLUDE(<tcb/span.hpp>)
 		#include <tcb/span.hpp>
 		#define SOAGEN_COLUMN_SPAN_TYPE TCB_SPAN_NAMESPACE_NAME::span
 	#endif
 #endif
-#if defined(SOAGEN_COLUMN_SPAN_TYPE) && !defined(SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT)
+
+#ifndef SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT
 	#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 0
 #endif
 
 #ifndef SOAGEN_OPTIONAL_TYPE
 	#include <optional>
 	#define SOAGEN_OPTIONAL_TYPE std::optional
 #endif
 
 SOAGEN_ENABLE_WARNINGS;
 #include "header_start.hpp"
 
+#ifndef SOAGEN_LAUNDER
+	#if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
+		#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
+	#elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                            \
+		|| SOAGEN_HAS_BUILTIN(__builtin_launder)
+		#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
+	#else
+		#define SOAGEN_LAUNDER(...) __VA_ARGS__
+	#endif
+#endif
+
 #ifndef SOAGEN_MAKE_NAME
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
@@ -85,16 +105,23 @@
 		template <>                                                                                                    \
 		struct column_ref<const Table&&, Column>                                                                       \
 			: named_member_##Name<std::add_rvalue_reference_t<                                                         \
 				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{}
 #endif
 
+/// @brief The root namespace for the library.
 namespace soagen
 {
+	using std::size_t;
+	using std::ptrdiff_t;
+	using std::intptr_t;
+	using std::uintptr_t;
+	using std::nullptr_t;
+
 	/// @brief	Equivalent to C+20's std::remove_cvref_t.
 	template <typename T>
 	using remove_cvref = std::remove_cv_t<std::remove_reference_t<T>>;
 
 	/// @brief	Transforms `T` &rarr; `const T&`.
 	template <typename T>
 	using make_cref = std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>;
@@ -194,14 +221,32 @@
 #else
 	using SOAGEN_OPTIONAL_TYPE;
 #endif
 
 	/// @cond
 	namespace detail
 	{
+		template <template <typename...> typename Trait, typename Enabler, typename... Args>
+		struct is_detected_impl : std::false_type
+		{};
+		template <template <typename...> typename Trait, typename... Args>
+		struct is_detected_impl<Trait, std::void_t<Trait<Args...>>, Args...> : std::true_type
+		{};
+		template <template <typename...> typename Trait, typename... Args>
+		inline constexpr auto is_detected_ = is_detected_impl<Trait, void, Args...>::value;
+	}
+	/// @endcond
+
+	/// @brief Detects if a Trait can be applied to a set of Args.
+	template <template <typename...> typename Trait, typename... Args>
+	inline constexpr auto is_detected = detail::is_detected_<Trait, Args...>;
+
+	/// @cond
+	namespace detail
+	{
 		template <typename T>
 		using has_swap_member_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
 
 		template <typename T, typename Arg>
 		using has_resize_member_ = decltype(std::declval<T&>().resize(std::declval<const Arg&>()));
 
 		template <typename T, typename Arg>
@@ -341,14 +386,59 @@
 	template <typename T, typename U = T>
 	inline constexpr bool is_nothrow_less_than_comparable = detail::is_nothrow_less_than_comparable_<T, U>::value;
 
 	/// @cond
 	namespace detail
 	{
 		template <typename T>
+		using has_tuple_size_ = decltype(std::tuple_size<remove_cvref<T>>::value);
+		template <typename T>
+		using has_tuple_element_ = decltype(std::declval<typename std::tuple_element<0, remove_cvref<T>>::type>());
+	}
+	/// @endcond
+
+	/// @brief	True if `T` implements std::tuple_size and std::tuple_element.
+	template <typename T>
+	inline constexpr bool is_tuple_like =
+		is_detected<detail::has_tuple_size_, T> && is_detected<detail::has_tuple_element_, T>;
+
+#if !SOAGEN_DOXYGEN && SOAGEN_HAS_BUILTIN(__type_pack_element)
+
+	template <size_t I, typename... T>
+	using type_at_index = __type_pack_element<I, T...>;
+
+#else
+
+	/// @cond
+	namespace detail
+	{
+		template <size_t I, typename T, typename... U>
+		struct type_at_index_impl
+		{
+			using type = typename type_at_index_impl<I - 1, U...>::type;
+		};
+
+		template <typename T, typename... U>
+		struct type_at_index_impl<0, T, U...>
+		{
+			using type = T;
+		};
+	}
+	/// @endcond
+
+	/// @brief Gets the type `T` at index `I` in the parameter pack.
+	template <size_t I, typename... T>
+	using type_at_index = POXY_IMPLEMENTATION_DETAIL(typename detail::type_at_index_impl<I, T...>::type);
+
+#endif
+
+	/// @cond
+	namespace detail
+	{
+		template <typename T>
 		struct table_type_
 		{
 			using type = typename T::table_type;
 		};
 	}
 	/// @endcond
 
@@ -561,44 +651,98 @@
 	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
 	template <typename T>
 	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
 	template <typename T>
 	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
 	/// @endcond
 
-	/// @brief	True if `Func` is invocable as `Func(Arg, OptArg)`, `Func(OptArg, Arg)`, or `Func(Arg)`
-	template <typename Func, typename Arg, typename OptArg>
-	inline constexpr bool is_invocable_with_optarg = std::is_invocable_v<Func, Arg, OptArg> //
-												  || std::is_invocable_v<Func, OptArg, Arg> //
-												  || std::is_invocable_v<Func, Arg>;
-
-	/// @brief	True if `Func` is nothrow-invocable as `Func(Arg, OptArg)`, `Func(OptArg, Arg)`, or `Func(Arg)`
-	template <typename Func, typename Arg, typename OptArg>
-	inline constexpr bool is_nothrow_invocable_with_optarg =
-		std::is_invocable_v<Func, Arg, OptArg>
-			? std::is_nothrow_invocable_v<Func, Arg, OptArg>
-			: (std::is_invocable_v<Func, OptArg, Arg> ? std::is_nothrow_invocable_v<Func, OptArg, Arg>
-													  : std::is_nothrow_invocable_v<Func, Arg>);
+	/// @cond
+	namespace detail
+	{
+		// note: this machinery is so that we only instantiate the is_nothrow version
+		// when the regular version is true
+
+		template <typename...>
+		struct is_nothrow_invocable_indirect_ : std::false_type
+		{};
+
+		template <typename Func, typename... Args>
+		struct is_nothrow_invocable_indirect_<std::true_type, Func, Args...> : std::is_nothrow_invocable<Func, Args...>
+		{};
+
+		template <typename Func, typename... Args>
+		struct is_invocable_ : std::is_invocable<Func, Args...>
+		{
+			using is_nothrow =
+				is_nothrow_invocable_indirect_<std::bool_constant<std::is_invocable<Func, Args...>::value>,
+											   Func,
+											   Args...>;
+		};
+	}
+	/// @endcond
+
+	/// @brief	True if `Func` is invocable with `Args`.
+	template <typename Func, typename... Args>
+	inline constexpr bool is_invocable = detail::is_invocable_<Func, Args...>::value;
+
+	/// @brief	True if `Func` is nothrow-invocable with `Args`.
+	template <typename Func, typename... Args>
+	inline constexpr bool is_nothrow_invocable = detail::is_invocable_<Func, Args...>::is_nothrow::value;
+
+	/// @cond
+	namespace detail
+	{
+		template <size_t I, typename Func, typename Arg>
+		struct is_invocable_with_optional_index_							//
+			: std::disjunction<is_invocable_<Func, Arg, index_constant<I>>, //
+							   is_invocable_<Func, Arg, size_t>,			//
+							   is_invocable_<Func, index_constant<I>, Arg>, //
+							   is_invocable_<Func, size_t, Arg>,			//
+							   is_invocable_<Func, Arg>>
+		{};
+	}
+	/// @endcond
+
+	/// @brief	True if `Func` is invocable with `Arg` and an index_constant and/or size_t.
+	template <size_t I, typename Func, typename Arg>
+	inline constexpr bool is_invocable_with_optional_index =
+		detail::is_invocable_with_optional_index_<I, Func, Arg>::value;
+
+	/// @brief	True if `Func` is nothrow-invocable with `Arg` and an index_constant and/or size_t.
+	template <size_t I, typename Func, typename Arg>
+	inline constexpr bool is_nothrow_invocable_with_optional_index =
+		detail::is_invocable_with_optional_index_<I, Func, Arg>::is_nothrow::value;
 
-	template <typename Func, typename Arg, typename OptArg>
+	template <size_t I, typename Func, typename Arg>
 	SOAGEN_ALWAYS_INLINE
-	constexpr decltype(auto) invoke_with_optarg(Func&& func, Arg&& arg, [[maybe_unused]] OptArg&& optarg) //
-		noexcept(is_nothrow_invocable_with_optarg<Func&&, Arg&&, OptArg&&>)
+	constexpr decltype(auto) invoke_with_optional_index(Func&& func,
+														Arg&& arg) //
+		noexcept(is_nothrow_invocable_with_optional_index<I, Func&&, Arg&&>)
 	{
-		if constexpr (std::is_invocable_v<Func&&, Arg&&, OptArg&&>)
+		static_assert(is_invocable_with_optional_index<I, Func&&, Arg&&>);
+
+		if constexpr (is_invocable<Func&&, Arg&&, index_constant<I>>)
+		{
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), index_constant<I>{});
+		}
+		else if constexpr (is_invocable<Func&&, Arg&&, size_t>)
+		{
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), I);
+		}
+		else if constexpr (is_invocable<Func&&, index_constant<I>, Arg&&>)
 		{
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), static_cast<OptArg&&>(optarg));
+			return static_cast<Func&&>(func)(index_constant<I>{}, static_cast<Arg&&>(arg));
 		}
-		else if constexpr (std::is_invocable_v<Func&&, OptArg&&, Arg&&>)
+		else if constexpr (is_invocable<Func&&, size_t, Arg&&>)
 		{
-			return static_cast<Func&&>(func)(static_cast<OptArg&&>(optarg), static_cast<Arg&&>(arg));
+			return static_cast<Func&&>(func)(I, static_cast<Arg&&>(arg));
 		}
 		else
 		{
-			static_assert(std::is_invocable_v<Func&&, Arg&&>);
+			static_assert(is_invocable<Func&&, Arg&&>);
 
 			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
 		}
 	}
 
 	/// @cond
 	namespace detail
```

### Comparing `soagen-0.2.0/src/soagen/hpp/mixins.hpp` & `soagen-0.3.0/src/soagen/hpp/mixins.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
-#include "meta.hpp"
+#include "core.hpp"
 
 namespace soagen::mixins
 {
 	//--- resize() -----------------------------------------------------------------------------------------------------
 
 	template <typename Derived, bool = has_resize_member<table_type<Derived>, typename table_type<Derived>::size_type>>
 	struct SOAGEN_EMPTY_BASES resizable
```

### Comparing `soagen-0.2.0/src/soagen/hpp/row.hpp` & `soagen-0.3.0/src/soagen/hpp/row.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
-#include "meta.hpp"
+#include "core.hpp"
 #include "header_start.hpp"
 
 namespace soagen
 {
 	/// @brief		Base class for soagen::row.
 	/// @details	Specialize this to add functionality to all rows of a particular type via CRTP.
 	template <typename Derived>
```

### Comparing `soagen-0.2.0/src/soagen/hpp/single/soagen.hpp` & `soagen-0.3.0/src/soagen/hpp/single/soagen.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //----------------------------------------------------------------------------------------------------------------------
 //
-// soagen.hpp v0.2.0
+// soagen.hpp v0.3.0
 // https://github.com/marzer/soagen
 // SPDX-License-Identifier: MIT
 //
 //----------------------------------------------------------------------------------------------------------------------
 //     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //----------------------------------------------------------------------------------------------------------------------
 //
@@ -28,17 +28,17 @@
 //----------------------------------------------------------------------------------------------------------------------
 #ifndef SOAGEN_HPP
 #define SOAGEN_HPP
 
 //********  generated/version.hpp  *************************************************************************************
 
 #define SOAGEN_VERSION_MAJOR 0
-#define SOAGEN_VERSION_MINOR 2
+#define SOAGEN_VERSION_MINOR 3
 #define SOAGEN_VERSION_PATCH 0
-#define SOAGEN_VERSION_STRING "0.2.0"
+#define SOAGEN_VERSION_STRING "0.3.0"
 
 //********  generated/preprocessor.hpp  ********************************************************************************
 
 #ifndef SOAGEN_CPP
 	#ifdef _MSVC_LANG
 		#if _MSVC_LANG > __cplusplus
 			#define SOAGEN_CPP _MSVC_LANG
@@ -457,14 +457,20 @@
 
 #if defined(__cpp_constexpr) && __cpp_constexpr >= 202002L
 	#define SOAGEN_CPP20_CONSTEXPR constexpr
 #else
 	#define SOAGEN_CPP20_CONSTEXPR
 #endif
 
+#if defined(__cpp_constexpr) && __cpp_constexpr >= 202211L
+	#define SOAGEN_CPP23_STATIC_CONSTEXPR static constexpr
+#else
+	#define SOAGEN_CPP23_STATIC_CONSTEXPR constexpr
+#endif
+
 #ifndef SOAGEN_CONCEPTS
 	#if defined(__cpp_concepts) && __cpp_concepts >= 201907
 		#define SOAGEN_CONCEPTS 1
 	#else
 		#define SOAGEN_CONCEPTS 0
 	#endif
 #endif
@@ -514,14 +520,15 @@
 #endif
 
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)                                                                          \
 		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == static_cast<std::size_t>(I) && (__VA_ARGS__),                    \
 									std::size_t sfinae_col_idx = static_cast<std::size_t>(I))
 #endif
+
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)
 #endif
 
 #ifndef SOAGEN_PUSH_WARNINGS
 	#if SOAGEN_CLANG
 		#define SOAGEN_PUSH_WARNINGS                                                                                   \
@@ -1026,150 +1033,44 @@
 		SOAGEN_DEFAULT_RULE_OF_FOUR(T)
 #endif
 
 #if !defined(__POXY__) && !defined(POXY_IMPLEMENTATION_DETAIL)
 	#define POXY_IMPLEMENTATION_DETAIL(...) __VA_ARGS__
 #endif
 
-//********  generated/core.hpp  ****************************************************************************************
+//********  core.hpp  **************************************************************************************************
 
 SOAGEN_DISABLE_WARNINGS;
+
 #include <cstdint>
 #include <cstddef>
 #include <cstdlib>
 #include <cstring>
 #include <numeric>
 #include <type_traits>
 #include <new>
 #include <utility>
 #include <memory>
 #include <optional>
-SOAGEN_ENABLE_WARNINGS;
-
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
-
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
-
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
-
-#if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
-	#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
-#elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                                \
-	|| SOAGEN_HAS_BUILTIN(__builtin_launder)
-	#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
-#else
-	#define SOAGEN_LAUNDER(...) __VA_ARGS__
-#endif
-
-//--- typedefs and type traits -----------------------------------------------------------------------------------------
-
-namespace soagen
-{
-	using std::size_t;
-	using std::ptrdiff_t;
-	using std::intptr_t;
-	using std::uintptr_t;
-	using std::nullptr_t;
-
-#if SOAGEN_HAS_BUILTIN(__type_pack_element)
-
-	template <size_t I, typename... T>
-	using type_at_index = __type_pack_element<I, T...>;
-
-#else
-
-	namespace detail
-	{
-		template <size_t I, typename T, typename... U>
-		struct type_at_index_impl
-		{
-			using type = typename type_at_index_impl<I - 1, U...>::type;
-		};
-
-		template <typename T, typename... U>
-		struct type_at_index_impl<0, T, U...>
-		{
-			using type = T;
-		};
-	}
-	template <size_t I, typename... T>
-	using type_at_index = POXY_IMPLEMENTATION_DETAIL(typename detail::type_at_index_impl<I, T...>::type);
-
-#endif
-
-	namespace detail
-	{
-		template <template <typename...> typename Trait, typename Enabler, typename... Args>
-		struct is_detected_impl : std::false_type
-		{};
-		template <template <typename...> typename Trait, typename... Args>
-		struct is_detected_impl<Trait, std::void_t<Trait<Args...>>, Args...> : std::true_type
-		{};
-		template <template <typename...> typename Trait, typename... Args>
-		inline constexpr auto is_detected_ = is_detected_impl<Trait, void, Args...>::value;
-	}
-	template <template <typename...> typename Trait, typename... Args>
-	inline constexpr auto is_detected = detail::is_detected_<Trait, Args...>;
-}
-
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
-
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
-
-SOAGEN_POP_WARNINGS;
-
-//********  meta.hpp  **************************************************************************************************
-
-SOAGEN_DISABLE_WARNINGS;
 
 #ifndef SOAGEN_COLUMN_SPAN_TYPE
-	#if defined(MUU_SPAN_H) || defined(MUU_SPAN_HPP)
-		#define SOAGEN_COLUMN_SPAN_TYPE				  muu::span
-		#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 1
-	#elif SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
+	#if SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
 		#include <span>
 		#define SOAGEN_COLUMN_SPAN_TYPE std::span
 	#elif SOAGEN_HAS_INCLUDE(<muu/span.h>)
 		#include <muu/span.h>
 		#define SOAGEN_COLUMN_SPAN_TYPE				  muu::span
 		#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 1
 	#elif SOAGEN_HAS_INCLUDE(<tcb/span.hpp>)
 		#include <tcb/span.hpp>
 		#define SOAGEN_COLUMN_SPAN_TYPE TCB_SPAN_NAMESPACE_NAME::span
 	#endif
 #endif
-#if defined(SOAGEN_COLUMN_SPAN_TYPE) && !defined(SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT)
+
+#ifndef SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT
 	#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 0
 #endif
 
 #ifndef SOAGEN_OPTIONAL_TYPE
 	#include <optional>
 	#define SOAGEN_OPTIONAL_TYPE std::optional
 #endif
@@ -1194,14 +1095,25 @@
 		#pragma strict_gs_check(push, off)
 	#elif SOAGEN_GCC
 		#pragma GCC push_options
 		#pragma GCC optimize("O2")
 	#endif
 #endif
 
+#ifndef SOAGEN_LAUNDER
+	#if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
+		#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
+	#elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                            \
+		|| SOAGEN_HAS_BUILTIN(__builtin_launder)
+		#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
+	#else
+		#define SOAGEN_LAUNDER(...) __VA_ARGS__
+	#endif
+#endif
+
 #ifndef SOAGEN_MAKE_NAME
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
@@ -1250,14 +1162,20 @@
 			: named_member_##Name<std::add_rvalue_reference_t<                                                         \
 				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{}
 #endif
 
 namespace soagen
 {
+	using std::size_t;
+	using std::ptrdiff_t;
+	using std::intptr_t;
+	using std::uintptr_t;
+	using std::nullptr_t;
+
 	template <typename T>
 	using remove_cvref = std::remove_cv_t<std::remove_reference_t<T>>;
 
 	template <typename T>
 	using make_cref = std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>;
 
 	template <typename T>
@@ -1286,20 +1204,22 @@
 	inline constexpr bool is_unsigned = is_integer<T> && std::is_unsigned_v<T>;
 
 	template <typename T, typename... U>
 	inline constexpr bool any_same = (false || ... || std::is_same_v<T, U>);
 
 	template <typename T>
 	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(false); // specialized in generated code
+
 	template <typename T>
 	inline constexpr bool is_soa<const T> = is_soa<T>;
 	template <typename T>
 	inline constexpr bool is_soa<volatile T> = is_soa<T>;
 	template <typename T>
 	inline constexpr bool is_soa<const volatile T> = is_soa<T>;
+
 	template <typename T>
 	inline constexpr bool is_implicit_lifetime_type =
 		std::is_scalar_v<T> || std::is_array_v<T>
 		|| (std::is_aggregate_v<T> && std::is_trivially_constructible_v<T> && std::is_trivially_destructible_v<T>);
 
 	template <auto Value>
 	using index_constant = std::integral_constant<size_t, static_cast<size_t>(Value)>;
@@ -1327,14 +1247,29 @@
 
 #endif
 
 	using SOAGEN_OPTIONAL_TYPE;
 
 	namespace detail
 	{
+		template <template <typename...> typename Trait, typename Enabler, typename... Args>
+		struct is_detected_impl : std::false_type
+		{};
+		template <template <typename...> typename Trait, typename... Args>
+		struct is_detected_impl<Trait, std::void_t<Trait<Args...>>, Args...> : std::true_type
+		{};
+		template <template <typename...> typename Trait, typename... Args>
+		inline constexpr auto is_detected_ = is_detected_impl<Trait, void, Args...>::value;
+	}
+
+	template <template <typename...> typename Trait, typename... Args>
+	inline constexpr auto is_detected = detail::is_detected_<Trait, Args...>;
+
+	namespace detail
+	{
 		template <typename T>
 		using has_swap_member_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
 
 		template <typename T, typename Arg>
 		using has_resize_member_ = decltype(std::declval<T&>().resize(std::declval<const Arg&>()));
 
 		template <typename T, typename Arg>
@@ -1350,14 +1285,15 @@
 		using is_equality_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
 												 == std::declval<const std::remove_reference_t<U>&>());
 
 		template <typename T, typename U>
 		using is_less_than_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
 												  < std::declval<const std::remove_reference_t<U>&>());
 	}
+
 	template <typename T>
 	inline constexpr bool has_swap_member = is_detected<detail::has_swap_member_, T>;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_resize_member = is_detected<detail::has_resize_member_, T, Arg>;
 
 	template <typename T, typename Arg = size_t>
@@ -1429,14 +1365,15 @@
 			: std::bool_constant<noexcept(std::declval<const std::remove_reference_t<T>&>()
 										  < std::declval<const std::remove_reference_t<U>&>())>
 		{};
 		template <typename T, typename U>
 		struct is_nothrow_less_than_comparable_<T, U, false> : std::false_type
 		{};
 	}
+
 	template <typename T>
 	inline constexpr bool has_nothrow_swap_member = detail::has_nothrow_swap_member_<T>::value;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_nothrow_resize_member = detail::has_nothrow_resize_member_<T, Arg>::value;
 
 	template <typename T, typename Arg = size_t>
@@ -1454,42 +1391,84 @@
 
 	template <typename T, typename U = T>
 	inline constexpr bool is_nothrow_less_than_comparable = detail::is_nothrow_less_than_comparable_<T, U>::value;
 
 	namespace detail
 	{
 		template <typename T>
+		using has_tuple_size_ = decltype(std::tuple_size<remove_cvref<T>>::value);
+		template <typename T>
+		using has_tuple_element_ = decltype(std::declval<typename std::tuple_element<0, remove_cvref<T>>::type>());
+	}
+
+	template <typename T>
+	inline constexpr bool is_tuple_like =
+		is_detected<detail::has_tuple_size_, T> && is_detected<detail::has_tuple_element_, T>;
+
+#if !SOAGEN_DOXYGEN && SOAGEN_HAS_BUILTIN(__type_pack_element)
+
+	template <size_t I, typename... T>
+	using type_at_index = __type_pack_element<I, T...>;
+
+#else
+
+	namespace detail
+	{
+		template <size_t I, typename T, typename... U>
+		struct type_at_index_impl
+		{
+			using type = typename type_at_index_impl<I - 1, U...>::type;
+		};
+
+		template <typename T, typename... U>
+		struct type_at_index_impl<0, T, U...>
+		{
+			using type = T;
+		};
+	}
+
+	template <size_t I, typename... T>
+	using type_at_index = POXY_IMPLEMENTATION_DETAIL(typename detail::type_at_index_impl<I, T...>::type);
+
+#endif
+
+	namespace detail
+	{
+		template <typename T>
 		struct table_type_
 		{
 			using type = typename T::table_type;
 		};
 	}
+
 	template <typename T>
 	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<std::remove_cv_t<T>>::type);
 
 	namespace detail
 	{
 		template <typename T>
 		struct table_traits_type_
 		{
 			using type = typename T::table_traits;
 		};
 	}
+
 	template <typename T>
 	using table_traits_type =
 		POXY_IMPLEMENTATION_DETAIL(typename detail::table_traits_type_<std::remove_cv_t<T>>::type);
 
 	namespace detail
 	{
 		template <typename T>
 		struct allocator_type_
 		{
 			using type = typename T::allocator_type;
 		};
 	}
+
 	template <typename T>
 	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<std::remove_cv_t<T>>::type);
 
 	template <typename T, auto Column>
 	using value_type = POXY_IMPLEMENTATION_DETAIL(
 		typename table_traits_type<T>::template column<static_cast<size_t>(Column)>::value_type);
 
@@ -1529,14 +1508,15 @@
 		template <>
 		struct storage_type_<char> : public storage_type_<std::byte>
 		{};
 		template <>
 		struct storage_type_<unsigned char> : public storage_type_<std::byte>
 		{};
 	}
+
 	template <typename ValueType>
 	using storage_type = POXY_IMPLEMENTATION_DETAIL(typename detail::storage_type_<ValueType>::type);
 
 	namespace detail
 	{
 		template <typename T>
 		struct param_type_
@@ -1570,14 +1550,15 @@
 		template <typename T>
 		struct param_type_<const T&&> : param_type_<const T&>
 		{};
 		template <typename T>
 		struct param_type_<const volatile T&&> : param_type_<const volatile T&>
 		{};
 	}
+
 	template <typename ValueType>
 	using param_type = POXY_IMPLEMENTATION_DETAIL(typename detail::param_type_<ValueType>::type);
 
 	namespace detail
 	{
 		template <typename T>
 		struct rvalue_type_
@@ -1591,14 +1572,15 @@
 					// copy-only things
 					!std::is_move_constructible_v<remove_cvref<T>>,
 					std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>,
 					// rvalues
 					std::add_rvalue_reference_t<remove_cvref<T>>>>;
 		};
 	}
+
 	template <typename ParamType>
 	using rvalue_type = POXY_IMPLEMENTATION_DETAIL(typename detail::rvalue_type_<ParamType>::type);
 
 	template <typename... Args>
 	struct emplacer
 	{
 		static_assert(sizeof...(Args));
@@ -1615,52 +1597,103 @@
 	};
 
 	template <>
 	struct emplacer<>
 	{};
 	template <typename... Args>
 	emplacer(Args&&...) -> emplacer<Args&&...>;
+
 	template <typename T>
 	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(false);
+
 	template <typename... T>
 	inline constexpr bool is_emplacer<emplacer<T...>> = true;
 	template <typename T>
 	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
 	template <typename T>
 	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
 	template <typename T>
 	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
-	template <typename Func, typename Arg, typename OptArg>
-	inline constexpr bool is_invocable_with_optarg = std::is_invocable_v<Func, Arg, OptArg> //
-												  || std::is_invocable_v<Func, OptArg, Arg> //
-												  || std::is_invocable_v<Func, Arg>;
-
-	template <typename Func, typename Arg, typename OptArg>
-	inline constexpr bool is_nothrow_invocable_with_optarg =
-		std::is_invocable_v<Func, Arg, OptArg>
-			? std::is_nothrow_invocable_v<Func, Arg, OptArg>
-			: (std::is_invocable_v<Func, OptArg, Arg> ? std::is_nothrow_invocable_v<Func, OptArg, Arg>
-													  : std::is_nothrow_invocable_v<Func, Arg>);
 
-	template <typename Func, typename Arg, typename OptArg>
+	namespace detail
+	{
+		// note: this machinery is so that we only instantiate the is_nothrow version
+		// when the regular version is true
+
+		template <typename...>
+		struct is_nothrow_invocable_indirect_ : std::false_type
+		{};
+
+		template <typename Func, typename... Args>
+		struct is_nothrow_invocable_indirect_<std::true_type, Func, Args...> : std::is_nothrow_invocable<Func, Args...>
+		{};
+
+		template <typename Func, typename... Args>
+		struct is_invocable_ : std::is_invocable<Func, Args...>
+		{
+			using is_nothrow =
+				is_nothrow_invocable_indirect_<std::bool_constant<std::is_invocable<Func, Args...>::value>,
+											   Func,
+											   Args...>;
+		};
+	}
+
+	template <typename Func, typename... Args>
+	inline constexpr bool is_invocable = detail::is_invocable_<Func, Args...>::value;
+
+	template <typename Func, typename... Args>
+	inline constexpr bool is_nothrow_invocable = detail::is_invocable_<Func, Args...>::is_nothrow::value;
+
+	namespace detail
+	{
+		template <size_t I, typename Func, typename Arg>
+		struct is_invocable_with_optional_index_							//
+			: std::disjunction<is_invocable_<Func, Arg, index_constant<I>>, //
+							   is_invocable_<Func, Arg, size_t>,			//
+							   is_invocable_<Func, index_constant<I>, Arg>, //
+							   is_invocable_<Func, size_t, Arg>,			//
+							   is_invocable_<Func, Arg>>
+		{};
+	}
+
+	template <size_t I, typename Func, typename Arg>
+	inline constexpr bool is_invocable_with_optional_index =
+		detail::is_invocable_with_optional_index_<I, Func, Arg>::value;
+
+	template <size_t I, typename Func, typename Arg>
+	inline constexpr bool is_nothrow_invocable_with_optional_index =
+		detail::is_invocable_with_optional_index_<I, Func, Arg>::is_nothrow::value;
+
+	template <size_t I, typename Func, typename Arg>
 	SOAGEN_ALWAYS_INLINE
-	constexpr decltype(auto) invoke_with_optarg(Func&& func, Arg&& arg, [[maybe_unused]] OptArg&& optarg) //
-		noexcept(is_nothrow_invocable_with_optarg<Func&&, Arg&&, OptArg&&>)
+	constexpr decltype(auto) invoke_with_optional_index(Func&& func,
+														Arg&& arg) //
+		noexcept(is_nothrow_invocable_with_optional_index<I, Func&&, Arg&&>)
 	{
-		if constexpr (std::is_invocable_v<Func&&, Arg&&, OptArg&&>)
+		static_assert(is_invocable_with_optional_index<I, Func&&, Arg&&>);
+
+		if constexpr (is_invocable<Func&&, Arg&&, index_constant<I>>)
+		{
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), index_constant<I>{});
+		}
+		else if constexpr (is_invocable<Func&&, Arg&&, size_t>)
 		{
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), static_cast<OptArg&&>(optarg));
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), I);
 		}
-		else if constexpr (std::is_invocable_v<Func&&, OptArg&&, Arg&&>)
+		else if constexpr (is_invocable<Func&&, index_constant<I>, Arg&&>)
 		{
-			return static_cast<Func&&>(func)(static_cast<OptArg&&>(optarg), static_cast<Arg&&>(arg));
+			return static_cast<Func&&>(func)(index_constant<I>{}, static_cast<Arg&&>(arg));
+		}
+		else if constexpr (is_invocable<Func&&, size_t, Arg&&>)
+		{
+			return static_cast<Func&&>(func)(I, static_cast<Arg&&>(arg));
 		}
 		else
 		{
-			static_assert(std::is_invocable_v<Func&&, Arg&&>);
+			static_assert(is_invocable<Func&&, Arg&&>);
 
 			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
 		}
 	}
 
 	namespace detail
 	{
@@ -1738,27 +1771,25 @@
 		static_assert(std::is_reference_v<Table>,
 					  "Table must be a reference so row members can derive their reference category");
 		static_assert(std::is_empty_v<row_base<row<Table, Columns...>>>,
 					  "row_base specializations may not have data members");
 		static_assert(std::is_trivial_v<row_base<row<Table, Columns...>>>, "row_base specializations must be trivial");
 
 		// columns:
-
 		template <auto Column>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) column() const noexcept
 		{
 			static_assert(static_cast<size_t>(Column) < table_traits_type<remove_cvref<Table>>::column_count,
 						  "column index out of range");
 
 			return detail::column_ref<Table, static_cast<size_t>(Column)>::get_named_member();
 		}
 
 		// tuple protocol:
-
 		template <auto Member>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
 			return type_at_index<Member, detail::column_ref<Table, Columns>...>::get_named_member();
@@ -1843,22 +1874,24 @@
 		{
 			return row_compare_impl<0>(lhs, rhs) >= 0;
 		}
 	};
 
 	template <typename T>
 	inline constexpr bool is_row = POXY_IMPLEMENTATION_DETAIL(false);
+
 	template <typename Table, size_t... Columns>
 	inline constexpr bool is_row<row<Table, Columns...>> = true;
 	template <typename T>
 	inline constexpr bool is_row<const T> = is_row<T>;
 	template <typename T>
 	inline constexpr bool is_row<volatile T> = is_row<T>;
 	template <typename T>
 	inline constexpr bool is_row<const volatile T> = is_row<T>;
+
 	namespace detail
 	{
 		template <typename Table, size_t... Columns>
 		struct table_type_<row<Table, Columns...>>
 		{
 			using type = remove_cvref<Table>;
 		};
@@ -1876,14 +1909,15 @@
 			using type = row<Table, Columns...>;
 		};
 		template <typename Table>
 		struct row_type_<Table, std::index_sequence<>>
 			: row_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
 		{};
 	}
+
 	template <typename Table, auto... Columns>
 	using row_type = POXY_IMPLEMENTATION_DETAIL(
 		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<static_cast<size_t>(Columns)...>>::type);
 }
 
 namespace std
 {
@@ -2074,23 +2108,25 @@
 			SOAGEN_COMPRESSED_PAIR_BASE_GETTERS(First, first, *this);
 			SOAGEN_COMPRESSED_PAIR_BASE_GETTERS(Second, second, *this);
 		};
 
 #undef SOAGEN_COMPRESSED_PAIR_BASE_DEFAULTS
 #undef SOAGEN_COMPRESSED_PAIR_BASE_GETTERS
 	}
+
 	template <typename First, typename Second>
 	class SOAGEN_EMPTY_BASES compressed_pair //
 		: public detail::compressed_pair_base<First, Second>
 	{
 	  private:
 		using base = detail::compressed_pair_base<First, Second>;
 
 	  public:
-		using first_type  = First;
+		using first_type = First;
+
 		using second_type = Second;
 
 		SOAGEN_NODISCARD_CTOR
 		compressed_pair() = default;
 
 		SOAGEN_NODISCARD_CTOR
 		compressed_pair(const compressed_pair&) = default;
@@ -2330,14 +2366,87 @@
 			return has_single_bit(static_cast<std::underlying_type_t<T>>(val));
 		else
 		{
 			return val != T{} && (val & (val - T{ 1 })) == T{};
 		}
 	}
 
+	template <size_t N, typename T>
+	SOAGEN_CONST_INLINE_GETTER
+	SOAGEN_ATTR(assume_aligned(N))
+	constexpr T* assume_aligned(T* ptr) noexcept
+	{
+		static_assert(N > 0 && (N & (N - 1u)) == 0u, "assume_aligned() requires a power-of-two alignment value.");
+		static_assert(!std::is_function_v<T>, "assume_aligned may not be used on functions.");
+
+		SOAGEN_IF_CONSTEVAL
+		{
+			return ptr;
+		}
+		else
+		{
+			SOAGEN_ASSUME((reinterpret_cast<uintptr_t>(ptr) & (N - uintptr_t{ 1 })) == 0);
+
+			if constexpr (std::is_volatile_v<T>)
+			{
+				return static_cast<T*>(soagen::assume_aligned<N>(const_cast<std::remove_volatile_t<T>*>(ptr)));
+			}
+			else
+			{
+#if SOAGEN_CLANG || SOAGEN_GCC || SOAGEN_HAS_BUILTIN(__builtin_assume_aligned)
+
+				return static_cast<T*>(__builtin_assume_aligned(ptr, N));
+
+#elif SOAGEN_MSVC
+
+				if constexpr (N < 16384)
+					return static_cast<T*>(__builtin_assume_aligned(ptr, N));
+				else
+					return ptr;
+
+#elif SOAGEN_ICC
+
+				__assume_aligned(ptr, N);
+				return ptr;
+
+#elif defined(__cpp_lib_assume_aligned)
+
+				return std::assume_aligned<N>(ptr);
+
+#else
+
+				return ptr;
+
+#endif
+			}
+		}
+	}
+
+	namespace detail
+	{
+		template <typename T>
+		using has_tuple_get_member_ = decltype(std::declval<T>().template get<0>());
+	}
+
+	template <size_t I, typename T>
+	SOAGEN_NODISCARD
+	SOAGEN_ALWAYS_INLINE
+	constexpr decltype(auto) get_from_tuple_like(T&& tuple_like) noexcept
+	{
+		if constexpr (is_detected<detail::has_tuple_get_member_, T&&>)
+		{
+			return static_cast<T&&>(tuple_like).template get<I>();
+		}
+		else // adl
+		{
+			using std::get;
+			return get<I>(static_cast<T&&>(tuple_like));
+		}
+	}
+
 #if SOAGEN_CPP >= 20 && defined(__cpp_lib_bit_cast) && __cpp_lib_bit_cast >= 201806
 
 	#define SOAGEN_HAS_INTRINSIC_BIT_CAST 1
 
 	using std::bit_cast;
 
 #else
@@ -2390,62 +2499,14 @@
 			std::memcpy(&to, &from, sizeof(To));
 			return to;
 		}
 	#endif
 	}
 
 #endif
-
-#if SOAGEN_CPP >= 20 && defined(__cpp_lib_assume_aligned) && __cpp_lib_assume_aligned >= 201811
-
-	using std::assume_aligned;
-
-#else
-
-	template <size_t N, typename T>
-	SOAGEN_CONST_INLINE_GETTER
-	SOAGEN_ATTR(assume_aligned(N))
-	constexpr T* assume_aligned(T* ptr) noexcept
-	{
-		static_assert(N > 0 && (N & (N - 1u)) == 0u, "assume_aligned() requires a power-of-two alignment value.");
-		static_assert(!std::is_function_v<T>, "assume_aligned may not be used on functions.");
-
-		SOAGEN_ASSUME((reinterpret_cast<uintptr_t>(ptr) & (N - uintptr_t{ 1 })) == 0);
-
-		if constexpr (std::is_volatile_v<T>)
-		{
-			return static_cast<T*>(soagen::assume_aligned<N>(const_cast<std::remove_volatile_t<T>*>(ptr)));
-		}
-		else
-		{
-	#if SOAGEN_CLANG || SOAGEN_GCC || SOAGEN_HAS_BUILTIN(__builtin_assume_aligned)
-
-			return static_cast<T*>(__builtin_assume_aligned(ptr, N));
-
-	#elif SOAGEN_MSVC
-
-			if constexpr (N < 16384)
-				return static_cast<T*>(__builtin_assume_aligned(ptr, N));
-			else
-				return ptr;
-
-	#elif SOAGEN_ICC
-
-			__assume_aligned(ptr, N);
-			return ptr;
-
-	#else
-
-			return ptr;
-
-	#endif
-		}
-	}
-
-#endif
 }
 
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
@@ -2758,14 +2819,16 @@
 	#endif
 #endif
 
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
+#define soagen_storage_ptr(...) soagen::assume_aligned<alignof(storage_type)>(__VA_ARGS__)
+
 namespace soagen::detail
 {
 	// a base class for the column traits that handles all the non-alignment-dependent stuff
 	// (to minimize template instantiation explosion)
 	template <typename StorageType>
 	struct column_traits_base
 	{
@@ -2778,100 +2841,96 @@
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& get(std::byte* ptr) noexcept
 		{
 			SOAGEN_ASSUME(ptr != nullptr);
 
-			return *SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(soagen::assume_aligned<alignof(storage_type)>(ptr)));
+			return *SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(soagen_storage_ptr(ptr)));
 		}
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
 		static constexpr const storage_type& get(const std::byte* ptr) noexcept
 		{
 			SOAGEN_ASSUME(ptr != nullptr);
 
-			return *SOAGEN_LAUNDER(
-				reinterpret_cast<const storage_type*>(soagen::assume_aligned<alignof(storage_type)>(ptr)));
+			return *SOAGEN_LAUNDER(reinterpret_cast<const storage_type*>(soagen_storage_ptr(ptr)));
 		}
 
 		//--- default construction -------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& default_construct(std::byte* destination) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				return *(
-					std::start_lifetime_as<storage_type>(soagen::assume_aligned<alignof(storage_type)>(destination)));
+				return *(std::start_lifetime_as<storage_type>(soagen_storage_ptr(destination)));
 			}
 			else
 			{
 #endif
-				return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-							 storage_type);
+				return *(::new (static_cast<void*>(soagen_storage_ptr(destination))) storage_type);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			}
 #endif
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& default_construct(std::byte* buffer, size_t element_index) //
+		static constexpr storage_type& default_construct(std::byte* buffer, size_t index) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
-			return default_construct(buffer + element_index * sizeof(storage_type));
+			return default_construct(buffer + index * sizeof(storage_type));
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
-		static void default_construct(std::byte* buffer, size_t start_index, size_t count) //
+		static void default_construct(std::byte* buffer, size_t index, size_t count) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 			SOAGEN_ASSUME(count);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 2022071
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				std::start_lifetime_as_array<storage_type>(soagen::assume_aligned<alignof(storage_type)>(destination),
-														   count);
+				std::start_lifetime_as_array<storage_type>(soagen_storage_ptr(destination), count);
 			}
 			else
 #endif
 				if constexpr (std::is_nothrow_default_constructible_v<storage_type>
 							  || std::is_trivially_destructible_v<storage_type>)
 			{
-				for (const size_t e = start_index + count; start_index < e; start_index++)
-					default_construct(buffer, start_index);
+				for (const size_t e = index + count; index < e; index++)
+					default_construct(buffer, index);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
-				size_t i = start_index;
+				size_t i = index;
 
 				try
 				{
-					for (const size_t e = start_index + count; i < e; i++)
+					for (const size_t e = index + count; i < e; i++)
 						default_construct(buffer, i);
 				}
 				catch (...)
 				{
-					for (; i-- > start_index;)
+					for (; i-- > index;)
 						destruct(buffer, i);
 					throw;
 				}
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
@@ -3001,47 +3060,45 @@
 					return construct_from_emplacer(
 						destination,
 						static_cast<Args&&>(args)...,
 						std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
 				else if constexpr (is_constructible_with_memcpy<Args&&...>)
 				{
-					std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
-								soagen::assume_aligned<alignof(storage_type)>(&args)...,
-								sizeof(storage_type));
+					std::memcpy(soagen_storage_ptr(destination), soagen_storage_ptr(&args)..., sizeof(storage_type));
 
 					return get(destination);
 				}
 				else if constexpr (std::is_aggregate_v<storage_type>)
 				{
-					return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
+					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
 								 storage_type{ static_cast<Args&&>(args)... });
 				}
 				else
 				{
-					return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
+					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
 								 storage_type(static_cast<Args&&>(args)...));
 				}
 			}
 		}
 
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& construct_at(std::byte* buffer, size_t element_index, Args&&... args) //
+		static constexpr storage_type& construct_at(std::byte* buffer, size_t index, Args&&... args) //
 			noexcept(is_nothrow_constructible<Args&&...>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			if constexpr (sizeof...(Args) == 0)
 			{
-				return default_construct(buffer + element_index * sizeof(storage_type));
+				return default_construct(buffer + index * sizeof(storage_type));
 			}
 			else
 			{
-				return construct(buffer + element_index * sizeof(storage_type), static_cast<Args&&>(args)...);
+				return construct(buffer + index * sizeof(storage_type), static_cast<Args&&>(args)...);
 			}
 		}
 
 		//--- move-construction ----------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_move_constructible = is_trivially_constructible<storage_type&&>;
 
@@ -3095,25 +3152,26 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_move_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_construct(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  std::byte* source_buffer,
-													  size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& move_construct(std::byte* dest_buffer,
+											size_t dest_index,
+											std::byte* source_buffer,
+											size_t source_index) //
 			noexcept(std::is_nothrow_move_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return move_construct(dest_buffer + dest_element_index * sizeof(storage_type),
-								  source_buffer + source_element_index * sizeof(storage_type));
+			return move_construct(dest_buffer + dest_index * sizeof(storage_type),
+								  source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- copy-construction ----------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_copy_constructible = is_trivially_constructible<const storage_type&>;
 
 		static constexpr bool is_copy_constructible =
@@ -3166,25 +3224,26 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_constructible)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_construct(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  const std::byte* source_buffer,
-													  size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& copy_construct(std::byte* dest_buffer,
+											size_t dest_index,
+											const std::byte* source_buffer,
+											size_t source_index) //
 			noexcept(is_nothrow_copy_constructible)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return copy_construct(dest_buffer + dest_element_index * sizeof(storage_type),
-								  source_buffer + source_element_index * sizeof(storage_type));
+			return copy_construct(dest_buffer + dest_index * sizeof(storage_type),
+								  source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- destruction ----------------------------------------------------------------------------------------------
 
 		SOAGEN_ATTR(nonnull)
 		static constexpr void destruct([[maybe_unused]] std::byte* target) //
 			noexcept(std::is_nothrow_destructible_v<storage_type>)
@@ -3194,23 +3253,23 @@
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
 				get(target).~storage_type();
 			}
 		}
 
 		SOAGEN_ATTR(nonnull)
-		static constexpr void destruct([[maybe_unused]] std::byte* buffer,	  //
-									   [[maybe_unused]] size_t element_index) //
+		static constexpr void destruct([[maybe_unused]] std::byte* buffer, //
+									   [[maybe_unused]] size_t index)	   //
 			noexcept(std::is_nothrow_destructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
-				destruct(buffer + element_index * sizeof(storage_type));
+				destruct(buffer + index * sizeof(storage_type));
 			}
 		}
 
 		//--- move-assignment ------------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_move_assignable =
 			is_constructible_with_memcpy<storage_type&&> || std::is_trivially_move_assignable_v<storage_type>;
@@ -3225,25 +3284,26 @@
 				? true
 				: (std::is_move_assignable_v<storage_type> ? std::is_nothrow_move_assignable_v<storage_type>
 														   : std::is_nothrow_destructible_v<storage_type>
 																 && std::is_nothrow_move_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_assign(std::byte* destination, void* source) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& move_assign(std::byte* destination, void* source) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
-							soagen::assume_aligned<alignof(storage_type)>(static_cast<std::byte*>(source)),
+				std::memcpy(soagen_storage_ptr(destination),
+							soagen_storage_ptr(static_cast<std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_move_assignable || std::is_move_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<storage_type&&>(get(static_cast<std::byte*>(source)));
@@ -3258,25 +3318,26 @@
 				destruct(destination);
 				return move_construct(destination, static_cast<std::byte*>(source));
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_assign(std::byte* dest_buffer,
-												   size_t dest_element_index,
-												   std::byte* source_buffer,
-												   size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& move_assign(std::byte* dest_buffer,
+										 size_t dest_index,
+										 std::byte* source_buffer,
+										 size_t source_index) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return move_assign(dest_buffer + dest_element_index * sizeof(storage_type),
-							   source_buffer + source_element_index * sizeof(storage_type));
+			return move_assign(dest_buffer + dest_index * sizeof(storage_type),
+							   source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- copy-assignment ------------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_copy_assignable =
 			is_constructible_with_memcpy<const storage_type&> || std::is_trivially_copy_assignable_v<storage_type>;
 
@@ -3290,25 +3351,26 @@
 				? true
 				: (std::is_copy_assignable_v<storage_type> ? std::is_nothrow_copy_assignable_v<storage_type>
 														   : std::is_nothrow_destructible_v<storage_type>
 																 && std::is_nothrow_copy_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_assign(std::byte* destination, const std::byte* source) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& copy_assign(std::byte* destination, const std::byte* source) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
-							soagen::assume_aligned<alignof(storage_type)>(static_cast<const std::byte*>(source)),
+				std::memcpy(soagen_storage_ptr(destination),
+							soagen_storage_ptr(static_cast<const std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_copy_assignable || std::is_copy_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<const storage_type&>(get(source));
@@ -3323,87 +3385,137 @@
 				destruct(destination);
 				return copy_construct(destination, source);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_assign(std::byte* dest_buffer,
-												   size_t dest_element_index,
-												   const std::byte* source_buffer,
-												   size_t source_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static storage_type& copy_assign(std::byte* dest_buffer,
+										 size_t dest_index,
+										 const std::byte* source_buffer,
+										 size_t source_index) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			return copy_assign(dest_buffer + dest_element_index * sizeof(storage_type),
-							   source_buffer + source_element_index * sizeof(storage_type));
+			return copy_assign(dest_buffer + dest_index * sizeof(storage_type),
+							   source_buffer + source_index * sizeof(storage_type));
 		}
 
 		//--- swap -----------------------------------------------------------------------------------------------------
 
-		static constexpr bool is_swappable =
-			std::is_swappable_v<storage_type> || (is_move_constructible && is_move_assignable);
-
-		static constexpr bool is_nothrow_swappable = std::is_swappable_v<storage_type>
-													   ? std::is_nothrow_swappable_v<storage_type>
-													   : (is_nothrow_move_constructible && is_nothrow_move_assignable);
+		static constexpr bool is_trivially_swappable =
+			is_trivially_copyable
+			&& (std::is_scalar_v<storage_type> || std::is_fundamental_v<storage_type>
+				|| !std::is_swappable_v<storage_type> // we don't want to usurp user-defined swap() functions
+			);
+
+		static constexpr bool is_swappable = is_trivially_swappable //
+										  || std::is_swappable_v<storage_type>
+										  || (is_move_constructible && is_move_assignable);
+
+		static constexpr bool is_nothrow_swappable =
+			is_trivially_swappable
+			|| (std::is_swappable_v<storage_type> ? std::is_nothrow_swappable_v<storage_type>
+												  : (is_nothrow_move_constructible && is_nothrow_move_assignable));
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_swappable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr void swap(std::byte* lhs, std::byte* rhs) //
+		SOAGEN_CPP20_CONSTEXPR
+		static void swap(std::byte* lhs, std::byte* rhs) //
 			noexcept(is_nothrow_swappable)
 		{
 			SOAGEN_ASSUME(lhs != nullptr);
 			SOAGEN_ASSUME(rhs != nullptr);
 			SOAGEN_ASSUME(lhs != rhs);
 
-			if constexpr (std::is_swappable_v<storage_type>)
+			if constexpr (is_trivially_swappable)
+			{
+				alignas(storage_type) std::byte buf[sizeof(storage_type)];
+				std::memcpy(soagen_storage_ptr(buf), soagen_storage_ptr(lhs), sizeof(storage_type));
+				std::memcpy(soagen_storage_ptr(lhs), soagen_storage_ptr(rhs), sizeof(storage_type));
+				std::memcpy(soagen_storage_ptr(rhs), soagen_storage_ptr(buf), sizeof(storage_type));
+			}
+			else if constexpr (std::is_swappable_v<storage_type>)
 			{
 				using std::swap;
 				swap(get(lhs), get(rhs));
 			}
-			else if constexpr (is_move_constructible && is_move_assignable)
+			else
 			{
+				static_assert(is_move_constructible && is_move_assignable);
+
 				storage_type temp(static_cast<storage_type&&>(get(lhs)));
 				move_assign(lhs, rhs);
 				move_assign(rhs, &temp);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_swappable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr void swap(std::byte* lhs_buffer,
-								   size_t lhs_element_index,
-								   std::byte* rhs_buffer,
-								   size_t rhs_element_index) //
+		SOAGEN_CPP20_CONSTEXPR
+		static void swap(std::byte* lhs_buffer,
+						 size_t lhs_index,
+						 std::byte* rhs_buffer,
+						 size_t rhs_index,
+						 size_t count = 1) //
 			noexcept(is_nothrow_swappable)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
-			return swap(lhs_buffer + lhs_element_index * sizeof(storage_type),
-						rhs_buffer + rhs_element_index * sizeof(storage_type));
+			if SOAGEN_UNLIKELY(!count)
+				return;
+
+			lhs_buffer = soagen_storage_ptr(lhs_buffer + lhs_index * sizeof(storage_type));
+			rhs_buffer = soagen_storage_ptr(rhs_buffer + rhs_index * sizeof(storage_type));
+
+			[[maybe_unused]] SOAGEN_CPP23_STATIC_CONSTEXPR size_t trivial_buf_size = 2048u / sizeof(storage_type);
+
+			if constexpr (is_trivially_swappable && trivial_buf_size > 1)
+			{
+				for (size_t i = 0; i < count; i += trivial_buf_size)
+				{
+					const auto num = soagen::min(trivial_buf_size, count - i);
+
+					alignas(storage_type) std::byte buf[sizeof(storage_type) * trivial_buf_size];
+					std::memcpy(buf, lhs_buffer, sizeof(storage_type) * num);
+					std::memcpy(lhs_buffer, rhs_buffer, sizeof(storage_type) * num);
+					std::memcpy(rhs_buffer, buf, sizeof(storage_type) * num);
+
+					lhs_buffer = soagen_storage_ptr(lhs_buffer + trivial_buf_size * sizeof(storage_type));
+					rhs_buffer = soagen_storage_ptr(rhs_buffer + trivial_buf_size * sizeof(storage_type));
+				}
+			}
+			else
+			{
+				const auto end = lhs_buffer + count * sizeof(storage_type);
+				for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
+				{
+					swap(lhs_buffer, rhs_buffer);
+				}
+			}
 		}
 
 		//--- memmove ---------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_trivially_copyable)
 		static constexpr void memmove(std::byte* dest_buffer,
-									  size_t dest_element_index,
+									  size_t dest_index,
 									  const std::byte* source_buffer,
-									  size_t source_element_index,
-									  size_t count) noexcept
+									  size_t source_index,
+									  size_t count = 1) noexcept
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			std::memmove(dest_buffer + dest_element_index * sizeof(storage_type),
-						 source_buffer + source_element_index * sizeof(storage_type),
+			std::memmove(soagen_storage_ptr(dest_buffer + dest_index * sizeof(storage_type)),
+						 soagen_storage_ptr(source_buffer + source_index * sizeof(storage_type)),
 						 count * sizeof(storage_type));
 		}
 
 		//--- equality -------------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
 		SOAGEN_NODISCARD
@@ -3417,25 +3529,25 @@
 			return get(lhs) == get(rhs);
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
 		SOAGEN_NODISCARD
 		SOAGEN_ATTR(nonnull)
 		static constexpr bool equal(const std::byte* lhs_buffer,
-									size_t lhs_start_index,
+									size_t lhs_index,
 									const std::byte* rhs_buffer,
-									size_t rhs_start_index,
+									size_t rhs_index,
 									size_t count = 1) //
 			noexcept(is_nothrow_equality_comparable<storage_type>)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
-			lhs_buffer += lhs_start_index * sizeof(storage_type);
-			rhs_buffer += rhs_start_index * sizeof(storage_type);
+			lhs_buffer += lhs_index * sizeof(storage_type);
+			rhs_buffer += rhs_index * sizeof(storage_type);
 			const auto end = lhs_buffer + count * sizeof(storage_type);
 
 			for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
 			{
 				if (!equal(lhs_buffer, rhs_buffer))
 					return false;
 			}
@@ -3457,24 +3569,24 @@
 			return get(lhs) < get(rhs);
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_less_than_comparable<storage_type>)
 		SOAGEN_NODISCARD
 		SOAGEN_ATTR(nonnull)
 		static constexpr bool less_than(const std::byte* lhs_buffer,
-										size_t lhs_element_index,
+										size_t lhs_index,
 										const std::byte* rhs_buffer,
-										size_t rhs_element_index) //
+										size_t rhs_index) //
 			noexcept(is_nothrow_less_than_comparable<storage_type>)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
-			return less_than(lhs_buffer + lhs_element_index * sizeof(storage_type),
-							 rhs_buffer + rhs_element_index * sizeof(storage_type));
+			return less_than(lhs_buffer + lhs_index * sizeof(storage_type),
+							 rhs_buffer + rhs_index * sizeof(storage_type));
 		}
 	};
 }
 
 namespace soagen
 {
 	template <typename ValueType,
@@ -3510,14 +3622,15 @@
 		using rvalue_forward_type = forward_type<rvalue_type>;
 
 		using default_emplace_type = make_cref<rvalue_type>;
 	};
 
 	template <typename T>
 	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
+
 	template <typename ValueType, size_t Align, typename ParamType>
 	inline constexpr bool is_column_traits<column_traits<ValueType, Align, ParamType>> = true;
 	template <typename StorageType>
 	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
 	template <typename T>
 	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
 	template <typename T>
@@ -3539,14 +3652,16 @@
 		static_assert(std::is_base_of_v<type, column_traits<ValueType, Align, ParamType>>);
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
 }
 
+#undef soagen_storage_ptr
+
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
 		#pragma inline_recursion(off)
 	#elif SOAGEN_GCC
@@ -3587,19 +3702,26 @@
 
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 namespace soagen::detail
 {
-	// a base class for the table traits that handles all the non-alignment-dependent stuff
+	// a base class for the table traits that handles all the non-alignment-dependent stuff -
+	// the 'Columns' argument seen by this class should be the column_base_traits, NOT soagen::column_traits
 	// (to minimize template instantiation explosion)
-	template <typename... Columns>
-	struct table_traits_base
+	template <typename...>
+	struct table_traits_base;
+
+	template <size_t... I, typename... Columns>
+	struct table_traits_base<std::index_sequence<I...>, Columns...>
 	{
+		static_assert(std::is_same_v<std::index_sequence<I...>, std::make_index_sequence<sizeof...(Columns)>>,
+					  "index sequence must match columns");
+
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		// columns
 
 		template <auto Index>
@@ -3696,210 +3818,151 @@
 		static constexpr bool all_nothrow_less_than_comparable =
 			(is_nothrow_less_than_comparable<typename Columns::storage_type> && ...);
 
 		// row constructibility
 
 	  private:
 		template <size_t, typename...>
-		struct row_constructible_from_row_ : std::false_type
+		struct row_constructible_from_tuple_ : std::false_type
 		{};
-		template <typename Table, size_t... RowCols, size_t... RowMembers>
-		struct row_constructible_from_row_<column_count, row<Table, RowCols...>, std::index_sequence<RowMembers...>>
-			: std::bool_constant<(Columns::template is_constructible<
-									  decltype(std::declval<row<Table, RowCols...>>().template get<RowMembers>())>
-								  && ...)>
+		template <typename Tuple, size_t... Members>
+		struct row_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
+			: std::bool_constant<(
+				  Columns::template is_constructible<decltype(get_from_tuple_like<Members>(std::declval<Tuple>()))>
+				  && ...)>
 		{
-			static_assert(sizeof...(RowCols) == column_count);
-			static_assert(sizeof...(RowMembers) == column_count);
-			static_assert(std::is_same_v<std::index_sequence<RowMembers...>, std::make_index_sequence<column_count>>);
+			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_constructible_from_<false, column_count, Args...>
 			: std::bool_constant<(Columns::template is_constructible<Args> && ...)>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
-		template <typename Row>
-		struct row_constructible_from_<true, 1, Row>
-			: row_constructible_from_row_<std::tuple_size_v<remove_cvref<Row>>,
-										  remove_cvref<Row>,
-										  std::make_index_sequence<std::tuple_size_v<remove_cvref<Row>>>>
+		template <typename Tuple>
+		struct row_constructible_from_<true, 1, Tuple>
+			: row_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
+											remove_cvref<Tuple>,
+											std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_constructible_from =
-			row_constructible_from_<(is_row<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
+			row_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
 		// row constructibility (nothrow)
 
 	  private:
 		template <size_t, typename...>
-		struct row_nothrow_constructible_from_row_ : std::false_type
+		struct row_nothrow_constructible_from_tuple_ : std::false_type
 		{};
-		template <typename Table, size_t... RowCols, size_t... RowMembers>
-		struct row_nothrow_constructible_from_row_<column_count,
-												   row<Table, RowCols...>,
-												   std::index_sequence<RowMembers...>>
-			: std::bool_constant<(Columns::template is_nothrow_constructible<
-									  decltype(std::declval<row<Table, RowCols...>>().template get<RowMembers>())>
+		template <typename Tuple, size_t... Members>
+		struct row_nothrow_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
+			: std::bool_constant<(Columns::template is_nothrow_constructible<decltype(get_from_tuple_like<Members>(
+									  std::declval<Tuple>()))>
 								  && ...)>
 		{
-			static_assert(sizeof...(RowCols) == column_count);
-			static_assert(sizeof...(RowMembers) == column_count);
-			static_assert(std::is_same_v<std::index_sequence<RowMembers...>, std::make_index_sequence<column_count>>);
+			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_nothrow_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_nothrow_constructible_from_<false, column_count, Args...>
 			: std::bool_constant<(Columns::template is_nothrow_constructible<Args> && ...)>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
-		template <typename Row>
-		struct row_nothrow_constructible_from_<true, 1, Row>
-			: row_nothrow_constructible_from_row_<std::tuple_size_v<remove_cvref<Row>>,
-												  remove_cvref<Row>,
-												  std::make_index_sequence<std::tuple_size_v<remove_cvref<Row>>>>
+		template <typename Tuple>
+		struct row_nothrow_constructible_from_<true, 1, Tuple>
+			: row_nothrow_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
+													remove_cvref<Tuple>,
+													std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_nothrow_constructible_from =
-			row_nothrow_constructible_from_<(is_row<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
+			row_nothrow_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::
+				value;
 
 		//--- memmove --------------------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void memmove(column_pointers& dest_columns,
-							size_t dest_start,
-							column_pointers& source_columns,
-							size_t source_start,
-							size_t count,
-							std::index_sequence<Cols...>) //
-			noexcept
-		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			(column<Cols>::memmove(dest_columns[Cols], dest_start, source_columns[Cols], source_start, count), ...);
-		}
-
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_trivially_copyable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void memmove(column_pointers& dest_columns,
+		static void memmove(column_pointers& dest,
 							size_t dest_start,
-							column_pointers& source_columns,
+							column_pointers& source,
 							size_t source_start,
 							size_t count) //
 			noexcept
 		{
-			memmove(dest_columns,
-					dest_start,
-					source_columns,
-					source_start,
-					count,
-					std::make_index_sequence<column_count>{});
+			(column<I>::memmove(dest[I], dest_start, source[I], source_start, count), ...);
 		}
 
 		//--- destruction ----------------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void destruct_row([[maybe_unused]] column_pointers& columns,
-								 [[maybe_unused]] size_t index,
-								 [[maybe_unused]] size_t leftmost_column,
-								 [[maybe_unused]] size_t rightmost_column,
-								 std::index_sequence<Cols...>) noexcept
+		static constexpr void destruct_row(column_pointers& columns,
+										   size_t index,
+										   size_t leftmost_column,
+										   size_t rightmost_column) noexcept
 		{
 			static_assert(all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
 			if constexpr (all_trivially_destructible)
 			{
 				// nothing to do in this case :)
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
-					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
+					static constexpr size_t column_index = decltype(ic)::value;
 
 					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
-						SOAGEN_ASSUME(columns[column_index]);
-						SOAGEN_ASSUME(leftmost_column <= rightmost_column);
-						SOAGEN_ASSUME(leftmost_column < column_count);
-						SOAGEN_ASSUME(rightmost_column < column_count);
-
 						if (column_index >= leftmost_column && column_index <= rightmost_column)
 							column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
-				(destructor(index_constant<Cols>{}), ...);
+				(destructor(index_constant<column_count - I - 1u>{}), ...);
 			}
 		}
 
-		template <size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void destruct_row([[maybe_unused]] column_pointers& columns,
-								 [[maybe_unused]] size_t index,
-								 std::index_sequence<Cols...>) noexcept
+		static constexpr void destruct_row(column_pointers& columns, size_t index) noexcept
 		{
 			static_assert(all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
 			if constexpr (all_trivially_destructible)
 			{
 				// nothing to do in this case :)
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
-					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
+					static constexpr size_t column_index = decltype(ic)::value;
 
 					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
-						SOAGEN_ASSUME(columns[column_index]);
-
 						column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
-				(destructor(index_constant<Cols>{}), ...);
+				(destructor(index_constant<column_count - I - 1u>{}), ...);
 			}
 		}
 
-	  public:
-		SOAGEN_ALWAYS_INLINE
-		static constexpr void destruct_row(column_pointers& columns,
-										   size_t index,
-										   size_t leftmost_column,
-										   size_t rightmost_column) noexcept
-		{
-			destruct_row(columns, index, leftmost_column, rightmost_column, std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_ALWAYS_INLINE
-		static constexpr void destruct_row(column_pointers& columns, size_t index) noexcept
-		{
-			destruct_row(columns, index, std::make_index_sequence<column_count>{});
-		}
-
 		static constexpr void destruct_rows([[maybe_unused]] column_pointers& columns,
 											[[maybe_unused]] size_t start,
 											[[maybe_unused]] size_t count) noexcept
 		{
 			static_assert(all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
 			if constexpr (all_trivially_destructible)
@@ -3911,29 +3974,25 @@
 				for (size_t i = start + count; i-- > start;)
 					destruct_row(columns, i);
 			}
 		}
 
 		//--- default-construction -------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_default_constructible)
 		SOAGEN_CPP20_CONSTEXPR
 		static void default_construct_row(column_pointers& columns,
-										  size_t index,
-										  std::index_sequence<Cols...>) //
-			noexcept(all_nothrow_default_constructible)					//
-			SOAGEN_REQUIRES(all_default_constructible)
+										  size_t index) //
+			noexcept(all_nothrow_default_constructible) //
 		{
 			static_assert(all_default_constructible);
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
 
 			if constexpr (all_nothrow_default_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::default_construct(columns[Cols], index), ...);
+				(column<I>::default_construct(columns[I], index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
@@ -3943,37 +4002,26 @@
 					column_from_ic<decltype(ic)>::default_construct(columns[decltype(ic)::value], index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_constant<Cols>{}), ...);
+					(constructor(index_constant<I>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
 						destruct_row(columns, index, 0u, constructed_columns - 1u);
 
 					throw;
 				}
 			}
 		}
 
-	  public:
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_default_constructible)
-		SOAGEN_ALWAYS_INLINE
-		SOAGEN_CPP20_CONSTEXPR
-		static void default_construct_row(column_pointers& columns,
-										  size_t index) //
-			noexcept(all_nothrow_default_constructible) //
-		{
-			default_construct_row(columns, index, std::make_index_sequence<column_count>{});
-		}
-
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_default_constructible)
 		SOAGEN_CPP20_CONSTEXPR
 		static void default_construct_rows([[maybe_unused]] column_pointers& columns,
 										   [[maybe_unused]] size_t start,
 										   [[maybe_unused]] size_t count) //
 			noexcept(all_nothrow_destructible)
 		{
@@ -4000,57 +4048,47 @@
 					throw;
 				}
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename Row, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename Tuple, auto sfinae = row_constructible_from<Tuple&&>)
+		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row_from_row(column_pointers& columns,
-										   size_t index,
-										   Row&& row,
-										   std::index_sequence<Cols...>) //
-			noexcept(row_nothrow_constructible_from<Row&&>)
-		{
-			static_assert(is_row<remove_cvref<Row>>);
-			static_assert(row_constructible_from<Row&&>);
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-			static_assert(std::tuple_size_v<remove_cvref<Row>> == column_count);
-
-			construct_row(columns,
-						  index,
-						  std::index_sequence<Cols...>{},
-						  static_cast<Row&&>(row).template get<Cols>()...);
+		static void construct_row_from_tuple_like(column_pointers& columns,
+												  size_t index,
+												  Tuple&& tuple) //
+			noexcept(row_nothrow_constructible_from<Tuple&&>)
+		{
+			static_assert(std::tuple_size_v<remove_cvref<Tuple>> == column_count);
+
+			construct_row(columns, index, get_from_tuple_like<I>(static_cast<Tuple&&>(tuple))...);
 		}
 
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename... Args, auto sfinae = row_constructible_from<Args&&...>)
 		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row(column_pointers& columns,
-								  size_t index,
-								  std::index_sequence<Cols...>,
-								  Args&&... args) //
+		static void construct_row(column_pointers& columns, size_t index, Args&&... args) //
 			noexcept(row_nothrow_constructible_from<Args&&...>)
 		{
-			static_assert(row_constructible_from<Args&&...>);
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			if constexpr (sizeof...(Args) == 1 && (is_row<remove_cvref<Args>> && ...))
+			if constexpr (sizeof...(Args) == 0)
+			{
+				default_construct_row(columns, index, static_cast<Args&&>(args)...);
+			}
+			else if constexpr (sizeof...(Args) == 1 && (is_tuple_like<remove_cvref<Args>> && ...))
 			{
-				construct_row_from_row(columns, index, static_cast<Args&&>(args)..., std::index_sequence<Cols...>{});
+				construct_row_from_tuple_like(columns, index, static_cast<Args&&>(args)...);
 			}
 			else
 			{
-				static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-				static_assert(sizeof...(Args) == sizeof...(Cols));
+				static_assert(sizeof...(Args) == sizeof...(I));
 
 				if constexpr (row_nothrow_constructible_from<Args&&...> || all_trivially_destructible)
 				{
-					(column<Cols>::construct_at(columns[Cols], index, static_cast<Args&&>(args)), ...);
+					(column<I>::construct_at(columns[I], index, static_cast<Args&&>(args)), ...);
 				}
 				else
 				{
 					// machinery to provide strong-exception guarantee
 
 					size_t constructed_columns = {};
 
@@ -4063,475 +4101,354 @@
 																   static_cast<decltype(arg)&&>(arg));
 
 						constructed_columns++;
 					};
 
 					try
 					{
-						(constructor(index_constant<Cols>{}, static_cast<Args&&>(args)), ...);
+						(constructor(index_constant<I>{}, static_cast<Args&&>(args)), ...);
 					}
 					catch (...)
 					{
 						if (constructed_columns)
 							destruct_row(columns, index, 0u, constructed_columns - 1u);
 
 						throw;
 					}
 				}
 			}
 		}
 
-	  public:
-		template <typename... Args>
-		SOAGEN_ALWAYS_INLINE
-		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row(column_pointers& columns, size_t index, Args&&... args) //
-			noexcept(row_nothrow_constructible_from<Args&&...>)
-		{
-			if constexpr (sizeof...(Args) == 0)
-			{
-				default_construct_row(columns,
-									  index,
-									  std::make_index_sequence<column_count>{},
-									  static_cast<Args&&>(args)...);
-			}
-			else
-			{
-				construct_row(columns, index, std::make_index_sequence<column_count>{}, static_cast<Args&&>(args)...);
-			}
-		}
-
 		//--- move-construction ----------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_constructible)
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_construct_row(column_pointers& dest_columns,
+		static void move_construct_row(column_pointers& dest,
 									   size_t dest_index,
-									   column_pointers& source_columns,
-									   size_t source_index,
-									   std::index_sequence<Cols...>) //
+									   column_pointers& source,
+									   size_t source_index) //
 			noexcept(all_nothrow_move_constructible)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			if constexpr (all_nothrow_move_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::move_construct(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+				(column<I>::move_construct(dest[I], dest_index, source[I], source_index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
 					[&](auto ic) noexcept(std::is_nothrow_move_constructible_v<storage_type<decltype(ic)::value>>)
 				{
-					column_from_ic<decltype(ic)>::move_construct(dest_columns[decltype(ic)::value],
+					column_from_ic<decltype(ic)>::move_construct(dest[decltype(ic)::value],
 																 dest_index,
-																 source_columns[decltype(ic)::value],
+																 source[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_constant<Cols>{}), ...);
+					(constructor(index_constant<I>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
-						destruct_row(dest_columns, dest_index, 0u, constructed_columns - 1u);
+						destruct_row(dest, dest_index, 0u, constructed_columns - 1u);
 
 					throw;
 				}
 			}
 		}
 
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_constructible)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_construct_row(column_pointers& dest_columns,
-									   size_t dest_index,
-									   column_pointers& source_columns,
-									   size_t source_index) //
-			noexcept(all_nothrow_move_constructible)
-		{
-			move_construct_row(dest_columns,
-							   dest_index,
-							   source_columns,
-							   source_index,
-							   std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_constructible)
-		SOAGEN_CPP20_CONSTEXPR
-		static void move_construct_rows(column_pointers& dest_columns,
+		static void move_construct_rows(column_pointers& dest,
 										size_t dest_start,
-										column_pointers& source_columns,
+										column_pointers& source,
 										size_t source_start,
 										size_t count) //
 			noexcept(all_nothrow_move_constructible)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else if constexpr (all_nothrow_move_constructible)
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = 0;
 
 				try
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i-- > 0u;)
-							move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							move_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 					else
 					{
 						for (; i < count; i++)
-							move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							move_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 				}
 				catch (...)
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i < count; i++)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					else
 					{
 						for (; i-- > 0u;)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					throw;
 				}
 			}
 		}
 
 		//--- copy-construction ----------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_constructible)
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_construct_row(column_pointers& dest_columns,
+		static void copy_construct_row(column_pointers& dest,
 									   size_t dest_index,
-									   const const_column_pointers& source_columns,
-									   size_t source_index,
-									   std::index_sequence<Cols...>) //
+									   const const_column_pointers& source,
+									   size_t source_index) //
 			noexcept(all_nothrow_copy_constructible)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			if constexpr (all_nothrow_copy_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::copy_construct(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+				(column<I>::copy_construct(dest[I], dest_index, source[I], source_index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
 					[&](auto ic) noexcept(std::is_nothrow_copy_constructible_v<storage_type<decltype(ic)::value>>)
 				{
-					column_from_ic<decltype(ic)>::copy_construct(dest_columns[decltype(ic)::value],
+					column_from_ic<decltype(ic)>::copy_construct(dest[decltype(ic)::value],
 																 dest_index,
-																 source_columns[decltype(ic)::value],
+																 source[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_constant<Cols>{}), ...);
+					(constructor(index_constant<I>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
-						destruct_row(dest_columns, dest_index, 0u, constructed_columns - 1u);
+						destruct_row(dest, dest_index, 0u, constructed_columns - 1u);
 
 					throw;
 				}
 			}
 		}
 
-	  public:
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_constructible)
-		SOAGEN_ALWAYS_INLINE
-		SOAGEN_CPP20_CONSTEXPR
-		static void copy_construct_row(column_pointers& dest_columns,
-									   size_t dest_index,
-									   const const_column_pointers& source_columns,
-									   size_t source_index) //
-			noexcept(all_nothrow_copy_constructible)
-		{
-			copy_construct_row(dest_columns,
-							   dest_index,
-							   source_columns,
-							   source_index,
-							   std::make_index_sequence<column_count>{});
-		}
-
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_constructible)
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_construct_rows(column_pointers& dest_columns,
+		static void copy_construct_rows(column_pointers& dest,
 										size_t dest_start,
-										const const_column_pointers& source_columns,
+										const const_column_pointers& source,
 										size_t source_start,
 										size_t count) //
 			noexcept(all_nothrow_copy_constructible)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else if constexpr (all_nothrow_copy_constructible)
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = 0;
 
 				try
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i-- > 0u;)
-							copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							copy_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 					else
 					{
 						for (; i < count; i++)
-							copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							copy_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 				}
 				catch (...)
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i < count; i++)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					else
 					{
 						for (; i-- > 0u;)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					throw;
 				}
 			}
 		}
 
 		//--- move-assignment ------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_assignable)
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_assign_row(column_pointers& dest_columns,
+		static void move_assign_row(column_pointers& dest,
 									size_t dest_index,
-									column_pointers& source_columns,
-									size_t source_index,
-									std::index_sequence<Cols...>) //
+									column_pointers& source,
+									size_t source_index) //
 			noexcept(all_nothrow_move_assignable)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			// todo: how to provide a strong-exception guarantee here?
 
-			(column<Cols>::move_assign(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+			(column<I>::move_assign(dest[I], dest_index, source[I], source_index), ...);
 		}
 
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_assignable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_assign_row(column_pointers& dest_columns,
-									size_t dest_index,
-									column_pointers& source_columns,
-									size_t source_index) //
-			noexcept(all_nothrow_move_assignable)
-		{
-			move_assign_row(dest_columns,
-							dest_index,
-							source_columns,
-							source_index,
-							std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_assignable)
-		SOAGEN_CPP20_CONSTEXPR
-		static void move_assign_rows(column_pointers& dest_columns,
+		static void move_assign_rows(column_pointers& dest,
 									 size_t dest_start,
-									 column_pointers& source_columns,
+									 column_pointers& source,
 									 size_t source_start,
 									 size_t count) //
 			noexcept(all_nothrow_copy_assignable)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						move_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						move_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 		}
 
 		//--- copy-assignment ------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_assignable)
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_assign_row(column_pointers& dest_columns,
+		static void copy_assign_row(column_pointers& dest,
 									size_t dest_index,
-									const const_column_pointers& source_columns,
-									size_t source_index,
-									std::index_sequence<Cols...>) //
+									const const_column_pointers& source,
+									size_t source_index) //
 			noexcept(all_nothrow_copy_assignable)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			// todo: how to provide a strong-exception guarantee here?
 
-			(column<Cols>::copy_assign(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+			(column<I>::copy_assign(dest[I], dest_index, source[I], source_index), ...);
 		}
 
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_assignable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_assign_row(column_pointers& dest_columns,
-									size_t dest_index,
-									const const_column_pointers& source_columns,
-									size_t source_index) //
-			noexcept(all_nothrow_copy_assignable)
-		{
-			copy_assign_row(dest_columns,
-							dest_index,
-							source_columns,
-							source_index,
-							std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_assignable)
-		SOAGEN_CPP20_CONSTEXPR
-		static void copy_assign_rows(column_pointers& dest_columns,
+		static void copy_assign_rows(column_pointers& dest,
 									 size_t dest_start,
-									 const const_column_pointers& source_columns,
+									 const const_column_pointers& source,
 									 size_t source_start,
 									 size_t count) //
 			noexcept(all_nothrow_copy_assignable)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						copy_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						copy_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 		}
 
 		//--- swap rows ------------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void swap_rows(column_pointers& lhs_columns,
-							  size_t lhs_index,
-							  column_pointers& rhs_columns,
-							  size_t rhs_index,
-							  std::index_sequence<Cols...>) //
-			noexcept(all_nothrow_swappable)
-		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			(column<Cols>::swap(lhs_columns[Cols], lhs_index, rhs_columns[Cols], rhs_index), ...);
-		}
-
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_swappable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void swap_rows(column_pointers& lhs_columns,
+		static void swap_rows(column_pointers& lhs,
 							  size_t lhs_index,
-							  column_pointers& rhs_columns,
+							  column_pointers& rhs,
 							  size_t rhs_index) //
 			noexcept(all_nothrow_swappable)
 		{
-			swap_rows(lhs_columns, lhs_index, rhs_columns, rhs_index, std::make_index_sequence<column_count>{});
+			(column<I>::swap(lhs[I], lhs_index, rhs[I], rhs_index), ...);
 		}
 
 		//--- swap columns ---------------------------------------------------------------------------------------------
 
 		template <size_t A, size_t B>
 		static constexpr bool can_swap_columns =
 			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
@@ -4549,122 +4466,95 @@
 		{
 			if constexpr (A != B)
 			{
 				static_assert(std::is_same_v<storage_type<A>, storage_type<B>>);
 				static_assert(column<A>::is_swappable);
 				static_assert(column<B>::is_swappable);
 
-				count += start;
-				for (; start < count; start++)
-					column<A>::swap(columns[A], start, columns[B], start);
+				column<A>::swap(columns[A], start, columns[B], start, count);
 			}
 		}
 
 		//--- equality -------------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
-		SOAGEN_NODISCARD
-		constexpr static bool equal(const const_column_pointers& lhs_columns,
-									size_t lhs_start_index,
-									const const_column_pointers& rhs_columns,
-									size_t rhs_start_index,
-									size_t count,
-									std::index_sequence<Cols...>) //
-			noexcept(all_nothrow_equality_comparable)
-		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			// note that the equality-comparison is done column-major for speed (cache-locality) because
-			// equality-comparison does not need to know anything about the order of the columns,
-			// just that they are all equal (there is no lexicographic constraint)
-
-			return (column<Cols>::equal(lhs_columns[Cols], lhs_start_index, rhs_columns[Cols], rhs_start_index, count)
-					&& ...);
-		}
-
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_equality_comparable)
 		SOAGEN_NODISCARD
-		SOAGEN_ALWAYS_INLINE
-		constexpr static bool equal(const const_column_pointers& lhs_columns,
+		static constexpr bool equal(const const_column_pointers& lhs,
 									size_t lhs_start,
-									const const_column_pointers& rhs_columns,
+									const const_column_pointers& rhs,
 									size_t rhs_start,
 									size_t count) //
 			noexcept(all_nothrow_equality_comparable)
 		{
-			return equal(lhs_columns,
-						 lhs_start,
-						 rhs_columns,
-						 rhs_start,
-						 count,
-						 std::make_index_sequence<column_count>{});
+			// note that the equality-comparison is done column-major for speed (cache-locality) because
+			// equality-comparison does not need to know anything about the order of the columns,
+			// just that they are all equal (there is no lexicographic constraint)
+
+			return (column<I>::equal(lhs[I], lhs_start, rhs[I], rhs_start, count) && ...);
 		}
 
 		//--- compare --------------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_less_than_comparable)
 		SOAGEN_NODISCARD
-		constexpr static int compare(const const_column_pointers& lhs_columns,
-									 size_t lhs_start_index,
-									 const const_column_pointers& rhs_columns,
-									 size_t rhs_start_index,
-									 size_t count,
-									 std::index_sequence<Cols...>) //
+		static constexpr int compare(const const_column_pointers& lhs,
+									 size_t lhs_start,
+									 const const_column_pointers& rhs,
+									 size_t rhs_start,
+									 size_t count) //
 			noexcept(all_nothrow_less_than_comparable)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
 			for (size_t i = 0; i < count; i++)
 			{
-				if ((false || ...
-					 || column<Cols>::less_than(lhs_columns[Cols],
-												lhs_start_index + i,
-												rhs_columns[Cols],
-												rhs_start_index + i)))
+				if ((false || ... || column<I>::less_than(lhs[I], lhs_start + i, rhs[I], rhs_start + i)))
 					return -1;
 
-				if ((false || ...
-					 || column<Cols>::less_than(rhs_columns[Cols],
-												rhs_start_index + i,
-												lhs_columns[Cols],
-												lhs_start_index + i)))
+				if ((false || ... || column<I>::less_than(rhs[I], rhs_start + i, lhs[I], lhs_start + i)))
 					return 1;
 			}
 
 			return 0;
 		}
+	};
 
-	  public:
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_less_than_comparable)
-		SOAGEN_NODISCARD
-		SOAGEN_ALWAYS_INLINE
-		constexpr static int compare(const const_column_pointers& lhs_columns,
-									 size_t lhs_start,
-									 const const_column_pointers& rhs_columns,
-									 size_t rhs_start,
-									 size_t count) //
-			noexcept(all_nothrow_less_than_comparable)
-		{
-			return compare(lhs_columns,
-						   lhs_start,
-						   rhs_columns,
-						   rhs_start,
-						   count,
-						   std::make_index_sequence<column_count>{});
-		}
+	// a more specialzed base that sees the full column traits, not just the base version.
+	// (this is just for things that need the specialized information _and_ the column indices)
+	template <typename...>
+	struct table_traits_base_specialized;
+
+	template <size_t... I, typename... Columns>
+	struct table_traits_base_specialized<std::index_sequence<I...>, Columns...> //
+		: public table_traits_base<std::index_sequence<I...>, to_base_traits<Columns>...>
+	{
+		template <typename Func, bool Const = false>
+		static constexpr bool for_each_column_invocable =
+			(is_invocable_with_optional_index<I,
+											  Func,
+											  std::conditional_t<Const,
+																 std::add_const_t<typename Columns::value_type>,
+																 typename Columns::value_type>*>
+			 && ...);
+
+		template <typename Func, bool Const = false>
+		static constexpr bool for_each_column_nothrow_invocable =
+			(is_nothrow_invocable_with_optional_index<I,
+													  Func,
+													  std::conditional_t<Const,
+																		 std::add_const_t<typename Columns::value_type>,
+																		 typename Columns::value_type>*>
+			 && ...);
 	};
 }
 
 namespace soagen
 {
 	template <typename... Columns>
-	struct SOAGEN_EMPTY_BASES table_traits : public detail::table_traits_base<detail::to_base_traits<Columns>...>
+	struct SOAGEN_EMPTY_BASES table_traits //
+		SOAGEN_HIDDEN_BASE(
+			public detail::table_traits_base_specialized<std::make_index_sequence<sizeof...(Columns)>, Columns...>)
 	{
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, Columns::aligned_stride...);
 
@@ -4710,36 +4600,19 @@
 
 		template <typename BackingTable>
 		static constexpr bool rvalue_insert_is_nothrow =
 			emplace_is_nothrow<BackingTable, typename Columns::rvalue_forward_type...>;
 
 		template <typename BackingTable, typename Row>
 		static constexpr bool row_insert_is_nothrow = emplace_is_nothrow<BackingTable, Row>;
-
-		template <typename Func, bool Const = false>
-		static constexpr bool for_each_column_ptr_invocable = POXY_IMPLEMENTATION_DETAIL( //
-			(is_invocable_with_optarg<Func,
-									  std::conditional_t<Const,
-														 std::add_const_t<typename Columns::value_type>,
-														 typename Columns::value_type>*,
-									  size_t>
-			 && ...));
-
-		template <typename Func, bool Const = false>
-		static constexpr bool for_each_column_ptr_nothrow_invocable = POXY_IMPLEMENTATION_DETAIL( //
-			(is_nothrow_invocable_with_optarg<Func,
-											  std::conditional_t<Const,
-																 std::add_const_t<typename Columns::value_type>,
-																 typename Columns::value_type>*,
-											  size_t>
-			 && ...));
 	};
 
 	template <typename T>
 	inline constexpr bool is_table_traits = POXY_IMPLEMENTATION_DETAIL(false);
+
 	template <typename... Columns>
 	inline constexpr bool is_table_traits<table_traits<Columns...>> = true;
 	template <typename... Columns>
 	inline constexpr bool is_table_traits<detail::table_traits_base<Columns...>> = true;
 	template <typename T>
 	inline constexpr bool is_table_traits<const T> = is_table_traits<T>;
 	template <typename T>
@@ -6305,14 +6178,15 @@
 				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
 					base::alloc_.columns[static_cast<size_t>(Column)])));
 		}
 	};
 
 	template <typename>
 	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(false);
+
 	template <typename... Args>
 	inline constexpr bool is_table<table<Args...>> = true;
 	template <typename T>
 	inline constexpr bool is_table<const T> = is_table<T>;
 	template <typename T>
 	inline constexpr bool is_table<volatile T> = is_table<T>;
 	template <typename T>
@@ -6321,14 +6195,15 @@
 	{
 		template <typename... Args>
 		struct table_type_<table<Args...>>
 		{
 			using type = table<Args...>;
 		};
 	}
+
 	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Args...>>), typename... Args)
 	SOAGEN_ALWAYS_INLINE
 	constexpr void swap(table<Args...>& lhs, table<Args...>& rhs) //
 		noexcept(soagen::has_nothrow_swap_member<table<Args...>>)
 	{
 		lhs.swap(rhs);
 	}
@@ -6620,14 +6495,15 @@
 		template <typename Table>
 		struct iterator_storage
 		{
 			std::add_const_t<remove_cvref<Table>>* table;
 			typename remove_cvref<Table>::difference_type offset;
 		};
 	}
+
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES iterator_base
 	{};
 
 	template <typename Table, size_t... Columns>
 	class SOAGEN_EMPTY_BASES iterator
 		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>,
@@ -6659,15 +6535,14 @@
 		using iterator_category = std::random_access_iterator_tag;
 
 #if SOAGEN_CPP <= 17
 		using pointer = void;
 #endif
 
 	  private:
-
 		using base		= detail::iterator_storage<remove_cvref<Table>>;
 		using table_ptr = std::add_pointer_t<std::remove_reference_t<Table>>;
 
 		template <typename, size_t...>
 		friend class soagen::iterator;
 
 		SOAGEN_NODISCARD_CTOR
@@ -6851,22 +6726,24 @@
 													const iterator<Table, Columns...>& it) noexcept
 	{
 		return it + n;
 	}
 
 	template <typename T>
 	inline constexpr bool is_iterator = POXY_IMPLEMENTATION_DETAIL(false);
+
 	template <typename Table, size_t... Columns>
 	inline constexpr bool is_iterator<iterator<Table, Columns...>> = true;
 	template <typename T>
 	inline constexpr bool is_iterator<const T> = is_row<T>;
 	template <typename T>
 	inline constexpr bool is_iterator<volatile T> = is_row<T>;
 	template <typename T>
 	inline constexpr bool is_iterator<const volatile T> = is_row<T>;
+
 	namespace detail
 	{
 		template <typename Table, size_t... Columns>
 		struct table_type_<iterator<Table, Columns...>>
 		{
 			using type = remove_cvref<Table>;
 		};
@@ -6884,14 +6761,15 @@
 			using type = iterator<Table, Columns...>;
 		};
 		template <typename Table>
 		struct iterator_type_<Table, std::index_sequence<>>
 			: iterator_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
 		{};
 	}
+
 	template <typename Table, size_t... Columns>
 	using iterator_type = POXY_IMPLEMENTATION_DETAIL(
 		typename detail::iterator_type_<coerce_ref<Table>, std::index_sequence<Columns...>>::type);
 }
 
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
```

### Comparing `soagen-0.2.0/src/soagen/hpp/soagen.hpp` & `soagen-0.3.0/src/soagen/hpp/soagen.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/hpp/table.hpp` & `soagen-0.3.0/src/soagen/hpp/table.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/hpp/table_traits.hpp` & `soagen-0.3.0/src/soagen/hpp/table_traits.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,26 @@
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 /// @cond
 namespace soagen::detail
 {
-	// a base class for the table traits that handles all the non-alignment-dependent stuff
+	// a base class for the table traits that handles all the non-alignment-dependent stuff -
+	// the 'Columns' argument seen by this class should be the column_base_traits, NOT soagen::column_traits
 	// (to minimize template instantiation explosion)
-	template <typename... Columns>
-	struct table_traits_base
+	template <typename...>
+	struct table_traits_base;
+
+	template <size_t... I, typename... Columns>
+	struct table_traits_base<std::index_sequence<I...>, Columns...>
 	{
+		static_assert(std::is_same_v<std::index_sequence<I...>, std::make_index_sequence<sizeof...(Columns)>>,
+					  "index sequence must match columns");
+
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		// columns
 
 		template <auto Index>
@@ -119,210 +126,151 @@
 		static constexpr bool all_nothrow_less_than_comparable =
 			(is_nothrow_less_than_comparable<typename Columns::storage_type> && ...);
 
 		// row constructibility
 
 	  private:
 		template <size_t, typename...>
-		struct row_constructible_from_row_ : std::false_type
+		struct row_constructible_from_tuple_ : std::false_type
 		{};
-		template <typename Table, size_t... RowCols, size_t... RowMembers>
-		struct row_constructible_from_row_<column_count, row<Table, RowCols...>, std::index_sequence<RowMembers...>>
-			: std::bool_constant<(Columns::template is_constructible<
-									  decltype(std::declval<row<Table, RowCols...>>().template get<RowMembers>())>
-								  && ...)>
+		template <typename Tuple, size_t... Members>
+		struct row_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
+			: std::bool_constant<(
+				  Columns::template is_constructible<decltype(get_from_tuple_like<Members>(std::declval<Tuple>()))>
+				  && ...)>
 		{
-			static_assert(sizeof...(RowCols) == column_count);
-			static_assert(sizeof...(RowMembers) == column_count);
-			static_assert(std::is_same_v<std::index_sequence<RowMembers...>, std::make_index_sequence<column_count>>);
+			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_constructible_from_<false, column_count, Args...>
 			: std::bool_constant<(Columns::template is_constructible<Args> && ...)>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
-		template <typename Row>
-		struct row_constructible_from_<true, 1, Row>
-			: row_constructible_from_row_<std::tuple_size_v<remove_cvref<Row>>,
-										  remove_cvref<Row>,
-										  std::make_index_sequence<std::tuple_size_v<remove_cvref<Row>>>>
+		template <typename Tuple>
+		struct row_constructible_from_<true, 1, Tuple>
+			: row_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
+											remove_cvref<Tuple>,
+											std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_constructible_from =
-			row_constructible_from_<(is_row<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
+			row_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
 		// row constructibility (nothrow)
 
 	  private:
 		template <size_t, typename...>
-		struct row_nothrow_constructible_from_row_ : std::false_type
+		struct row_nothrow_constructible_from_tuple_ : std::false_type
 		{};
-		template <typename Table, size_t... RowCols, size_t... RowMembers>
-		struct row_nothrow_constructible_from_row_<column_count,
-												   row<Table, RowCols...>,
-												   std::index_sequence<RowMembers...>>
-			: std::bool_constant<(Columns::template is_nothrow_constructible<
-									  decltype(std::declval<row<Table, RowCols...>>().template get<RowMembers>())>
+		template <typename Tuple, size_t... Members>
+		struct row_nothrow_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
+			: std::bool_constant<(Columns::template is_nothrow_constructible<decltype(get_from_tuple_like<Members>(
+									  std::declval<Tuple>()))>
 								  && ...)>
 		{
-			static_assert(sizeof...(RowCols) == column_count);
-			static_assert(sizeof...(RowMembers) == column_count);
-			static_assert(std::is_same_v<std::index_sequence<RowMembers...>, std::make_index_sequence<column_count>>);
+			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_nothrow_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_nothrow_constructible_from_<false, column_count, Args...>
 			: std::bool_constant<(Columns::template is_nothrow_constructible<Args> && ...)>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
-		template <typename Row>
-		struct row_nothrow_constructible_from_<true, 1, Row>
-			: row_nothrow_constructible_from_row_<std::tuple_size_v<remove_cvref<Row>>,
-												  remove_cvref<Row>,
-												  std::make_index_sequence<std::tuple_size_v<remove_cvref<Row>>>>
+		template <typename Tuple>
+		struct row_nothrow_constructible_from_<true, 1, Tuple>
+			: row_nothrow_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
+													remove_cvref<Tuple>,
+													std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_nothrow_constructible_from =
-			row_nothrow_constructible_from_<(is_row<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
+			row_nothrow_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::
+				value;
 
 		//--- memmove --------------------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void memmove(column_pointers& dest_columns,
-							size_t dest_start,
-							column_pointers& source_columns,
-							size_t source_start,
-							size_t count,
-							std::index_sequence<Cols...>) //
-			noexcept
-		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			(column<Cols>::memmove(dest_columns[Cols], dest_start, source_columns[Cols], source_start, count), ...);
-		}
-
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_trivially_copyable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void memmove(column_pointers& dest_columns,
+		static void memmove(column_pointers& dest,
 							size_t dest_start,
-							column_pointers& source_columns,
+							column_pointers& source,
 							size_t source_start,
 							size_t count) //
 			noexcept
 		{
-			memmove(dest_columns,
-					dest_start,
-					source_columns,
-					source_start,
-					count,
-					std::make_index_sequence<column_count>{});
+			(column<I>::memmove(dest[I], dest_start, source[I], source_start, count), ...);
 		}
 
 		//--- destruction ----------------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void destruct_row([[maybe_unused]] column_pointers& columns,
-								 [[maybe_unused]] size_t index,
-								 [[maybe_unused]] size_t leftmost_column,
-								 [[maybe_unused]] size_t rightmost_column,
-								 std::index_sequence<Cols...>) noexcept
+		static constexpr void destruct_row(column_pointers& columns,
+										   size_t index,
+										   size_t leftmost_column,
+										   size_t rightmost_column) noexcept
 		{
 			static_assert(all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
 			if constexpr (all_trivially_destructible)
 			{
 				// nothing to do in this case :)
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
-					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
+					static constexpr size_t column_index = decltype(ic)::value;
 
 					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
-						SOAGEN_ASSUME(columns[column_index]);
-						SOAGEN_ASSUME(leftmost_column <= rightmost_column);
-						SOAGEN_ASSUME(leftmost_column < column_count);
-						SOAGEN_ASSUME(rightmost_column < column_count);
-
 						if (column_index >= leftmost_column && column_index <= rightmost_column)
 							column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
-				(destructor(index_constant<Cols>{}), ...);
+				(destructor(index_constant<column_count - I - 1u>{}), ...);
 			}
 		}
 
-		template <size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void destruct_row([[maybe_unused]] column_pointers& columns,
-								 [[maybe_unused]] size_t index,
-								 std::index_sequence<Cols...>) noexcept
+		static constexpr void destruct_row(column_pointers& columns, size_t index) noexcept
 		{
 			static_assert(all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
 			if constexpr (all_trivially_destructible)
 			{
 				// nothing to do in this case :)
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
-					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
+					static constexpr size_t column_index = decltype(ic)::value;
 
 					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
-						SOAGEN_ASSUME(columns[column_index]);
-
 						column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
-				(destructor(index_constant<Cols>{}), ...);
+				(destructor(index_constant<column_count - I - 1u>{}), ...);
 			}
 		}
 
-	  public:
-		SOAGEN_ALWAYS_INLINE
-		static constexpr void destruct_row(column_pointers& columns,
-										   size_t index,
-										   size_t leftmost_column,
-										   size_t rightmost_column) noexcept
-		{
-			destruct_row(columns, index, leftmost_column, rightmost_column, std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_ALWAYS_INLINE
-		static constexpr void destruct_row(column_pointers& columns, size_t index) noexcept
-		{
-			destruct_row(columns, index, std::make_index_sequence<column_count>{});
-		}
-
 		static constexpr void destruct_rows([[maybe_unused]] column_pointers& columns,
 											[[maybe_unused]] size_t start,
 											[[maybe_unused]] size_t count) noexcept
 		{
 			static_assert(all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
 			if constexpr (all_trivially_destructible)
@@ -334,29 +282,25 @@
 				for (size_t i = start + count; i-- > start;)
 					destruct_row(columns, i);
 			}
 		}
 
 		//--- default-construction -------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_default_constructible)
 		SOAGEN_CPP20_CONSTEXPR
 		static void default_construct_row(column_pointers& columns,
-										  size_t index,
-										  std::index_sequence<Cols...>) //
-			noexcept(all_nothrow_default_constructible)					//
-			SOAGEN_REQUIRES(all_default_constructible)
+										  size_t index) //
+			noexcept(all_nothrow_default_constructible) //
 		{
 			static_assert(all_default_constructible);
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
 
 			if constexpr (all_nothrow_default_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::default_construct(columns[Cols], index), ...);
+				(column<I>::default_construct(columns[I], index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
@@ -366,37 +310,26 @@
 					column_from_ic<decltype(ic)>::default_construct(columns[decltype(ic)::value], index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_constant<Cols>{}), ...);
+					(constructor(index_constant<I>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
 						destruct_row(columns, index, 0u, constructed_columns - 1u);
 
 					throw;
 				}
 			}
 		}
 
-	  public:
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_default_constructible)
-		SOAGEN_ALWAYS_INLINE
-		SOAGEN_CPP20_CONSTEXPR
-		static void default_construct_row(column_pointers& columns,
-										  size_t index) //
-			noexcept(all_nothrow_default_constructible) //
-		{
-			default_construct_row(columns, index, std::make_index_sequence<column_count>{});
-		}
-
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_default_constructible)
 		SOAGEN_CPP20_CONSTEXPR
 		static void default_construct_rows([[maybe_unused]] column_pointers& columns,
 										   [[maybe_unused]] size_t start,
 										   [[maybe_unused]] size_t count) //
 			noexcept(all_nothrow_destructible)
 		{
@@ -423,57 +356,47 @@
 					throw;
 				}
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename Row, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename Tuple, auto sfinae = row_constructible_from<Tuple&&>)
+		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row_from_row(column_pointers& columns,
-										   size_t index,
-										   Row&& row,
-										   std::index_sequence<Cols...>) //
-			noexcept(row_nothrow_constructible_from<Row&&>)
-		{
-			static_assert(is_row<remove_cvref<Row>>);
-			static_assert(row_constructible_from<Row&&>);
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-			static_assert(std::tuple_size_v<remove_cvref<Row>> == column_count);
-
-			construct_row(columns,
-						  index,
-						  std::index_sequence<Cols...>{},
-						  static_cast<Row&&>(row).template get<Cols>()...);
+		static void construct_row_from_tuple_like(column_pointers& columns,
+												  size_t index,
+												  Tuple&& tuple) //
+			noexcept(row_nothrow_constructible_from<Tuple&&>)
+		{
+			static_assert(std::tuple_size_v<remove_cvref<Tuple>> == column_count);
+
+			construct_row(columns, index, get_from_tuple_like<I>(static_cast<Tuple&&>(tuple))...);
 		}
 
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename... Args, auto sfinae = row_constructible_from<Args&&...>)
 		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row(column_pointers& columns,
-								  size_t index,
-								  std::index_sequence<Cols...>,
-								  Args&&... args) //
+		static void construct_row(column_pointers& columns, size_t index, Args&&... args) //
 			noexcept(row_nothrow_constructible_from<Args&&...>)
 		{
-			static_assert(row_constructible_from<Args&&...>);
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			if constexpr (sizeof...(Args) == 1 && (is_row<remove_cvref<Args>> && ...))
+			if constexpr (sizeof...(Args) == 0)
+			{
+				default_construct_row(columns, index, static_cast<Args&&>(args)...);
+			}
+			else if constexpr (sizeof...(Args) == 1 && (is_tuple_like<remove_cvref<Args>> && ...))
 			{
-				construct_row_from_row(columns, index, static_cast<Args&&>(args)..., std::index_sequence<Cols...>{});
+				construct_row_from_tuple_like(columns, index, static_cast<Args&&>(args)...);
 			}
 			else
 			{
-				static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-				static_assert(sizeof...(Args) == sizeof...(Cols));
+				static_assert(sizeof...(Args) == sizeof...(I));
 
 				if constexpr (row_nothrow_constructible_from<Args&&...> || all_trivially_destructible)
 				{
-					(column<Cols>::construct_at(columns[Cols], index, static_cast<Args&&>(args)), ...);
+					(column<I>::construct_at(columns[I], index, static_cast<Args&&>(args)), ...);
 				}
 				else
 				{
 					// machinery to provide strong-exception guarantee
 
 					size_t constructed_columns = {};
 
@@ -486,475 +409,354 @@
 																   static_cast<decltype(arg)&&>(arg));
 
 						constructed_columns++;
 					};
 
 					try
 					{
-						(constructor(index_constant<Cols>{}, static_cast<Args&&>(args)), ...);
+						(constructor(index_constant<I>{}, static_cast<Args&&>(args)), ...);
 					}
 					catch (...)
 					{
 						if (constructed_columns)
 							destruct_row(columns, index, 0u, constructed_columns - 1u);
 
 						throw;
 					}
 				}
 			}
 		}
 
-	  public:
-		template <typename... Args>
-		SOAGEN_ALWAYS_INLINE
-		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row(column_pointers& columns, size_t index, Args&&... args) //
-			noexcept(row_nothrow_constructible_from<Args&&...>)
-		{
-			if constexpr (sizeof...(Args) == 0)
-			{
-				default_construct_row(columns,
-									  index,
-									  std::make_index_sequence<column_count>{},
-									  static_cast<Args&&>(args)...);
-			}
-			else
-			{
-				construct_row(columns, index, std::make_index_sequence<column_count>{}, static_cast<Args&&>(args)...);
-			}
-		}
-
 		//--- move-construction ----------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_constructible)
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_construct_row(column_pointers& dest_columns,
+		static void move_construct_row(column_pointers& dest,
 									   size_t dest_index,
-									   column_pointers& source_columns,
-									   size_t source_index,
-									   std::index_sequence<Cols...>) //
+									   column_pointers& source,
+									   size_t source_index) //
 			noexcept(all_nothrow_move_constructible)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			if constexpr (all_nothrow_move_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::move_construct(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+				(column<I>::move_construct(dest[I], dest_index, source[I], source_index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
 					[&](auto ic) noexcept(std::is_nothrow_move_constructible_v<storage_type<decltype(ic)::value>>)
 				{
-					column_from_ic<decltype(ic)>::move_construct(dest_columns[decltype(ic)::value],
+					column_from_ic<decltype(ic)>::move_construct(dest[decltype(ic)::value],
 																 dest_index,
-																 source_columns[decltype(ic)::value],
+																 source[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_constant<Cols>{}), ...);
+					(constructor(index_constant<I>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
-						destruct_row(dest_columns, dest_index, 0u, constructed_columns - 1u);
+						destruct_row(dest, dest_index, 0u, constructed_columns - 1u);
 
 					throw;
 				}
 			}
 		}
 
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_constructible)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_construct_row(column_pointers& dest_columns,
-									   size_t dest_index,
-									   column_pointers& source_columns,
-									   size_t source_index) //
-			noexcept(all_nothrow_move_constructible)
-		{
-			move_construct_row(dest_columns,
-							   dest_index,
-							   source_columns,
-							   source_index,
-							   std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_constructible)
-		SOAGEN_CPP20_CONSTEXPR
-		static void move_construct_rows(column_pointers& dest_columns,
+		static void move_construct_rows(column_pointers& dest,
 										size_t dest_start,
-										column_pointers& source_columns,
+										column_pointers& source,
 										size_t source_start,
 										size_t count) //
 			noexcept(all_nothrow_move_constructible)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else if constexpr (all_nothrow_move_constructible)
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = 0;
 
 				try
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i-- > 0u;)
-							move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							move_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 					else
 					{
 						for (; i < count; i++)
-							move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							move_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 				}
 				catch (...)
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i < count; i++)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					else
 					{
 						for (; i-- > 0u;)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					throw;
 				}
 			}
 		}
 
 		//--- copy-construction ----------------------------------------------------------------------------------------
 
-	  private:
-		template <size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_constructible)
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_construct_row(column_pointers& dest_columns,
+		static void copy_construct_row(column_pointers& dest,
 									   size_t dest_index,
-									   const const_column_pointers& source_columns,
-									   size_t source_index,
-									   std::index_sequence<Cols...>) //
+									   const const_column_pointers& source,
+									   size_t source_index) //
 			noexcept(all_nothrow_copy_constructible)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			if constexpr (all_nothrow_copy_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::copy_construct(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+				(column<I>::copy_construct(dest[I], dest_index, source[I], source_index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
 					[&](auto ic) noexcept(std::is_nothrow_copy_constructible_v<storage_type<decltype(ic)::value>>)
 				{
-					column_from_ic<decltype(ic)>::copy_construct(dest_columns[decltype(ic)::value],
+					column_from_ic<decltype(ic)>::copy_construct(dest[decltype(ic)::value],
 																 dest_index,
-																 source_columns[decltype(ic)::value],
+																 source[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_constant<Cols>{}), ...);
+					(constructor(index_constant<I>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
-						destruct_row(dest_columns, dest_index, 0u, constructed_columns - 1u);
+						destruct_row(dest, dest_index, 0u, constructed_columns - 1u);
 
 					throw;
 				}
 			}
 		}
 
-	  public:
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_constructible)
-		SOAGEN_ALWAYS_INLINE
-		SOAGEN_CPP20_CONSTEXPR
-		static void copy_construct_row(column_pointers& dest_columns,
-									   size_t dest_index,
-									   const const_column_pointers& source_columns,
-									   size_t source_index) //
-			noexcept(all_nothrow_copy_constructible)
-		{
-			copy_construct_row(dest_columns,
-							   dest_index,
-							   source_columns,
-							   source_index,
-							   std::make_index_sequence<column_count>{});
-		}
-
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_constructible)
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_construct_rows(column_pointers& dest_columns,
+		static void copy_construct_rows(column_pointers& dest,
 										size_t dest_start,
-										const const_column_pointers& source_columns,
+										const const_column_pointers& source,
 										size_t source_start,
 										size_t count) //
 			noexcept(all_nothrow_copy_constructible)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else if constexpr (all_nothrow_copy_constructible)
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_construct_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = 0;
 
 				try
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i-- > 0u;)
-							copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							copy_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 					else
 					{
 						for (; i < count; i++)
-							copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+							copy_construct_row(dest, dest_start + i, source, source_start + i);
 					}
 				}
 				catch (...)
 				{
-					if (&dest_columns == &source_columns && dest_start > source_start)
+					if (&dest == &source && dest_start > source_start)
 					{
 						for (; i < count; i++)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					else
 					{
 						for (; i-- > 0u;)
-							destruct_row(dest_columns, dest_start + i);
+							destruct_row(dest, dest_start + i);
 					}
 					throw;
 				}
 			}
 		}
 
 		//--- move-assignment ------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_assignable)
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_assign_row(column_pointers& dest_columns,
+		static void move_assign_row(column_pointers& dest,
 									size_t dest_index,
-									column_pointers& source_columns,
-									size_t source_index,
-									std::index_sequence<Cols...>) //
+									column_pointers& source,
+									size_t source_index) //
 			noexcept(all_nothrow_move_assignable)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			// todo: how to provide a strong-exception guarantee here?
 
-			(column<Cols>::move_assign(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+			(column<I>::move_assign(dest[I], dest_index, source[I], source_index), ...);
 		}
 
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_assignable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void move_assign_row(column_pointers& dest_columns,
-									size_t dest_index,
-									column_pointers& source_columns,
-									size_t source_index) //
-			noexcept(all_nothrow_move_assignable)
-		{
-			move_assign_row(dest_columns,
-							dest_index,
-							source_columns,
-							source_index,
-							std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_assignable)
-		SOAGEN_CPP20_CONSTEXPR
-		static void move_assign_rows(column_pointers& dest_columns,
+		static void move_assign_rows(column_pointers& dest,
 									 size_t dest_start,
-									 column_pointers& source_columns,
+									 column_pointers& source,
 									 size_t source_start,
 									 size_t count) //
 			noexcept(all_nothrow_copy_assignable)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						move_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						move_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						move_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 		}
 
 		//--- copy-assignment ------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_assignable)
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_assign_row(column_pointers& dest_columns,
+		static void copy_assign_row(column_pointers& dest,
 									size_t dest_index,
-									const const_column_pointers& source_columns,
-									size_t source_index,
-									std::index_sequence<Cols...>) //
+									const const_column_pointers& source,
+									size_t source_index) //
 			noexcept(all_nothrow_copy_assignable)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
+			SOAGEN_ASSUME(&dest != &source || dest_index != source_index);
 
 			// todo: how to provide a strong-exception guarantee here?
 
-			(column<Cols>::copy_assign(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+			(column<I>::copy_assign(dest[I], dest_index, source[I], source_index), ...);
 		}
 
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_assignable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void copy_assign_row(column_pointers& dest_columns,
-									size_t dest_index,
-									const const_column_pointers& source_columns,
-									size_t source_index) //
-			noexcept(all_nothrow_copy_assignable)
-		{
-			copy_assign_row(dest_columns,
-							dest_index,
-							source_columns,
-							source_index,
-							std::make_index_sequence<column_count>{});
-		}
-
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_assignable)
-		SOAGEN_CPP20_CONSTEXPR
-		static void copy_assign_rows(column_pointers& dest_columns,
+		static void copy_assign_rows(column_pointers& dest,
 									 size_t dest_start,
-									 const const_column_pointers& source_columns,
+									 const const_column_pointers& source,
 									 size_t source_start,
 									 size_t count) //
 			noexcept(all_nothrow_copy_assignable)
 		{
-			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+			SOAGEN_ASSUME(&dest != &source || dest_start != source_start);
 
 			if constexpr (all_trivially_copyable)
 			{
-				memmove(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest, dest_start, source, source_start, count);
 			}
 			else
 			{
-				if (&dest_columns == &source_columns && dest_start > source_start)
+				if (&dest == &source && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
-						copy_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 				else
 				{
 					for (size_t i = 0; i < count; i++)
-						copy_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
+						copy_assign_row(dest, dest_start + i, source, source_start + i);
 				}
 			}
 		}
 
 		//--- swap rows ------------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
-		SOAGEN_CPP20_CONSTEXPR
-		static void swap_rows(column_pointers& lhs_columns,
-							  size_t lhs_index,
-							  column_pointers& rhs_columns,
-							  size_t rhs_index,
-							  std::index_sequence<Cols...>) //
-			noexcept(all_nothrow_swappable)
-		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			(column<Cols>::swap(lhs_columns[Cols], lhs_index, rhs_columns[Cols], rhs_index), ...);
-		}
-
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_swappable)
-		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void swap_rows(column_pointers& lhs_columns,
+		static void swap_rows(column_pointers& lhs,
 							  size_t lhs_index,
-							  column_pointers& rhs_columns,
+							  column_pointers& rhs,
 							  size_t rhs_index) //
 			noexcept(all_nothrow_swappable)
 		{
-			swap_rows(lhs_columns, lhs_index, rhs_columns, rhs_index, std::make_index_sequence<column_count>{});
+			(column<I>::swap(lhs[I], lhs_index, rhs[I], rhs_index), ...);
 		}
 
 		//--- swap columns ---------------------------------------------------------------------------------------------
 
 		template <size_t A, size_t B>
 		static constexpr bool can_swap_columns =
 			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
@@ -972,129 +774,102 @@
 		{
 			if constexpr (A != B)
 			{
 				static_assert(std::is_same_v<storage_type<A>, storage_type<B>>);
 				static_assert(column<A>::is_swappable);
 				static_assert(column<B>::is_swappable);
 
-				count += start;
-				for (; start < count; start++)
-					column<A>::swap(columns[A], start, columns[B], start);
+				column<A>::swap(columns[A], start, columns[B], start, count);
 			}
 		}
 
 		//--- equality -------------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
-		SOAGEN_NODISCARD
-		constexpr static bool equal(const const_column_pointers& lhs_columns,
-									size_t lhs_start_index,
-									const const_column_pointers& rhs_columns,
-									size_t rhs_start_index,
-									size_t count,
-									std::index_sequence<Cols...>) //
-			noexcept(all_nothrow_equality_comparable)
-		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
-			// note that the equality-comparison is done column-major for speed (cache-locality) because
-			// equality-comparison does not need to know anything about the order of the columns,
-			// just that they are all equal (there is no lexicographic constraint)
-
-			return (column<Cols>::equal(lhs_columns[Cols], lhs_start_index, rhs_columns[Cols], rhs_start_index, count)
-					&& ...);
-		}
-
-	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_equality_comparable)
 		SOAGEN_NODISCARD
-		SOAGEN_ALWAYS_INLINE
-		constexpr static bool equal(const const_column_pointers& lhs_columns,
+		static constexpr bool equal(const const_column_pointers& lhs,
 									size_t lhs_start,
-									const const_column_pointers& rhs_columns,
+									const const_column_pointers& rhs,
 									size_t rhs_start,
 									size_t count) //
 			noexcept(all_nothrow_equality_comparable)
 		{
-			return equal(lhs_columns,
-						 lhs_start,
-						 rhs_columns,
-						 rhs_start,
-						 count,
-						 std::make_index_sequence<column_count>{});
+			// note that the equality-comparison is done column-major for speed (cache-locality) because
+			// equality-comparison does not need to know anything about the order of the columns,
+			// just that they are all equal (there is no lexicographic constraint)
+
+			return (column<I>::equal(lhs[I], lhs_start, rhs[I], rhs_start, count) && ...);
 		}
 
 		//--- compare --------------------------------------------------------------------------------------------------
 
-	  private:
-		template <typename... Args, size_t... Cols>
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_less_than_comparable)
 		SOAGEN_NODISCARD
-		constexpr static int compare(const const_column_pointers& lhs_columns,
-									 size_t lhs_start_index,
-									 const const_column_pointers& rhs_columns,
-									 size_t rhs_start_index,
-									 size_t count,
-									 std::index_sequence<Cols...>) //
+		static constexpr int compare(const const_column_pointers& lhs,
+									 size_t lhs_start,
+									 const const_column_pointers& rhs,
+									 size_t rhs_start,
+									 size_t count) //
 			noexcept(all_nothrow_less_than_comparable)
 		{
-			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
-
 			for (size_t i = 0; i < count; i++)
 			{
-				if ((false || ...
-					 || column<Cols>::less_than(lhs_columns[Cols],
-												lhs_start_index + i,
-												rhs_columns[Cols],
-												rhs_start_index + i)))
+				if ((false || ... || column<I>::less_than(lhs[I], lhs_start + i, rhs[I], rhs_start + i)))
 					return -1;
 
-				if ((false || ...
-					 || column<Cols>::less_than(rhs_columns[Cols],
-												rhs_start_index + i,
-												lhs_columns[Cols],
-												lhs_start_index + i)))
+				if ((false || ... || column<I>::less_than(rhs[I], rhs_start + i, lhs[I], lhs_start + i)))
 					return 1;
 			}
 
 			return 0;
 		}
+	};
 
-	  public:
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_less_than_comparable)
-		SOAGEN_NODISCARD
-		SOAGEN_ALWAYS_INLINE
-		constexpr static int compare(const const_column_pointers& lhs_columns,
-									 size_t lhs_start,
-									 const const_column_pointers& rhs_columns,
-									 size_t rhs_start,
-									 size_t count) //
-			noexcept(all_nothrow_less_than_comparable)
-		{
-			return compare(lhs_columns,
-						   lhs_start,
-						   rhs_columns,
-						   rhs_start,
-						   count,
-						   std::make_index_sequence<column_count>{});
-		}
+	// a more specialzed base that sees the full column traits, not just the base version.
+	// (this is just for things that need the specialized information _and_ the column indices)
+	template <typename...>
+	struct table_traits_base_specialized;
+
+	template <size_t... I, typename... Columns>
+	struct table_traits_base_specialized<std::index_sequence<I...>, Columns...> //
+		: public table_traits_base<std::index_sequence<I...>, to_base_traits<Columns>...>
+	{
+		template <typename Func, bool Const = false>
+		static constexpr bool for_each_column_invocable =
+			(is_invocable_with_optional_index<I,
+											  Func,
+											  std::conditional_t<Const,
+																 std::add_const_t<typename Columns::value_type>,
+																 typename Columns::value_type>*>
+			 && ...);
+
+		template <typename Func, bool Const = false>
+		static constexpr bool for_each_column_nothrow_invocable =
+			(is_nothrow_invocable_with_optional_index<I,
+													  Func,
+													  std::conditional_t<Const,
+																		 std::add_const_t<typename Columns::value_type>,
+																		 typename Columns::value_type>*>
+			 && ...);
 	};
 }
 /// @endcond
 
 namespace soagen
 {
 	/// @brief	Traits for a table.
 	/// @tparam	Columns		The #soagen::column_traits for the columns of the table.
 	///
 	///	@attention	This class is an implementation detail for the soagen-generated Structure-of-arrays classes.
 	///				You don't need to know anything about it unless you are implementing your own SoA machinery
 	///				without using the soagen generator.
 	template <typename... Columns>
-	struct SOAGEN_EMPTY_BASES table_traits : public detail::table_traits_base<detail::to_base_traits<Columns>...>
+	struct SOAGEN_EMPTY_BASES table_traits //
+		SOAGEN_HIDDEN_BASE(
+			public detail::table_traits_base_specialized<std::make_index_sequence<sizeof...(Columns)>, Columns...>)
 	{
 		/// @brief The number of columns in the table.
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		/// @brief	The number of rows to advance to maintain the requested `alignment` for every column.
@@ -1176,37 +951,29 @@
 
 		/// @brief True if a generated class's row `insert()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		/// @tparam Row The row type.
 		template <typename BackingTable, typename Row>
 		static constexpr bool row_insert_is_nothrow = emplace_is_nothrow<BackingTable, Row>;
 
+#if SOAGEN_DOXYGEN
+
 		/// @brief True if a generated class's `for_each_column()` would be invocable with a callable.
 		/// @tparam Func The callable type being invoked.
 		/// @tparam Const True for `const` column data pointers.
 		template <typename Func, bool Const = false>
-		static constexpr bool for_each_column_ptr_invocable = POXY_IMPLEMENTATION_DETAIL( //
-			(is_invocable_with_optarg<Func,
-									  std::conditional_t<Const,
-														 std::add_const_t<typename Columns::value_type>,
-														 typename Columns::value_type>*,
-									  size_t>
-			 && ...));
+		static constexpr bool for_each_column_invocable = POXY_IMPLEMENTATION_DETAIL(void);
 
 		/// @brief True if a generated class's `for_each_column()` would be nothrow-invocable with a callable.
 		/// @tparam Func The callable type being invoked.
 		/// @tparam Const True for `const` column data pointers.
 		template <typename Func, bool Const = false>
-		static constexpr bool for_each_column_ptr_nothrow_invocable = POXY_IMPLEMENTATION_DETAIL( //
-			(is_nothrow_invocable_with_optarg<Func,
-											  std::conditional_t<Const,
-																 std::add_const_t<typename Columns::value_type>,
-																 typename Columns::value_type>*,
-											  size_t>
-			 && ...));
+		static constexpr bool for_each_column_nothrow_invocable = POXY_IMPLEMENTATION_DETAIL(void);
+
+#endif
 	};
 
 	/// @brief True if `T` is an instance of #soagen::table_traits.
 	template <typename T>
 	inline constexpr bool is_table_traits = POXY_IMPLEMENTATION_DETAIL(false);
 	/// @cond
 	template <typename... Columns>
```

### Comparing `soagen-0.2.0/src/soagen/includes.py` & `soagen-0.3.0/src/soagen/includes.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/injectors.py` & `soagen-0.3.0/src/soagen/injectors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/log.py` & `soagen-0.3.0/src/soagen/log.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/main.py` & `soagen-0.3.0/src/soagen/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,19 +207,14 @@
                         r'--namespaces',
                         r'soagen',
                         r'detail',
                         r'--macros',
                         r'SOAGEN',
                     ]
                     + ([r'--no-strip-hidden-bases'] if template.name not in (r'compressed_pair.hpp.in',) else [])
-                    + (
-                        [r'--no-strip-doxygen-from-snippets']
-                        if template.name not in (r'compressed_pair.hpp.in', r'preprocessor.hpp.in')
-                        else []
-                    )
                 )
             )
             text = utils.read_all_text_from_file(output, logger=log.i)
             try:
                 text = utils.clang_format(text, cwd=output.parent)
             except:
                 pass
@@ -445,15 +440,15 @@
 
     if configs:
         if args.clang_format and not utils.is_tool(r'clang-format'):
             log.w(r'clang-format not found on system PATH')
             args.clang_format = False
 
         for config in configs:
-            for src in (config.hpp,):
+            for src in config.hpp:
 
                 def on_flush(o: Writer, s: str) -> str:
                     nonlocal src
                     # sub in external headers
                     includes = sorted(set(src.includes.external + cpp.detect_includes(s)))
                     includes = cpp.remove_implicit_includes(includes)
                     EXTERNAL_HEADERS = r'\n[ \t]*//[ \t]*__SOAGEN_EXTERNAL_HEADERS[ \t]*\n'
```

### Comparing `soagen-0.2.0/src/soagen/metavars.py` & `soagen-0.3.0/src/soagen/metavars.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # SPDX-License-Identifier: MIT
 
 """
 Utility classes to build stacks of 'meta variables' for text substitution.
 """
 
 from . import utils
+from .configurable import Configurable
 
 
 class MetaVars(object):
 
     """
     A collection of meta-variables localized to one context (e.g. a class scope).
     """
@@ -88,23 +89,38 @@
 
 class MetaScope(object):
 
     """
     A scope that pushes a MetaVars object onto a MetaStack upon entry, and pops it upon exit.
     """
 
-    def __init__(self, stack, vars):
+    def __init__(self, stack, vars=None):
+        if isinstance(stack, Configurable):
+            vars = stack
+            stack = stack.config
+
         assert stack is not None
+        if not isinstance(stack, MetaStack):
+            if hasattr(stack, 'meta_stack'):
+                stack = stack.meta_stack
         assert isinstance(stack, MetaStack)
+
         assert vars is not None
+        if not isinstance(vars, MetaVars):
+            if hasattr(vars, 'meta_vars'):
+                vars = vars.meta_vars
+            elif hasattr(vars, 'meta'):
+                vars = vars.meta
         assert isinstance(vars, MetaVars)
+
         self.__stack = stack
-        self.__stack.push(vars)
+        self.__vars = vars
 
     def __enter__(self):
+        self.__stack.push(self.__vars)
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.__stack.pop()
 
     def __call__(self, text) -> str:
         return self.__stack(text)
```

### Comparing `soagen-0.2.0/src/soagen/natvis_file.py` & `soagen-0.3.0/src/soagen/natvis_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,107 +14,113 @@
 from .version import *
 
 
 class NatvisFile(Configurable):
     def __init__(self, config, structs):
         super().__init__(config)
         self.path = self.config.path.with_suffix('.natvis')
-        self.structs = structs if utils.is_collection(structs) else [structs]
+        self.structs = utils.coerce_collection(structs)
+
+        self.meta = MetaVars()
+        for prefix in (r'file_', r'file::'):
+            self.meta.push(rf'{prefix}name', self.path.name)
+            self.meta.push(rf'{prefix}path', str(self.path))
 
     def write(self, o: Writer):
-        o(
-            rf'''
-		<?xml version="1.0" encoding="utf-8"?>
-		<!--
-		// This file was generated by soagen v{VERSION_STRING} - do not modify it directly
-		// https://marzer.github.io/soagen
-		-->
-		<AutoVisualizer xmlns="http://schemas.microsoft.com/vstudio/debugger/natvis/2010">
-		'''
-        )
-
-        with Indent(o):
-            for struct in self.structs:
-                with MetaScope(self.config.meta_stack, struct.meta):
-                    o(
-                        rf'''
-					<!--{"="*(120 - o.indent_width - 4)}
-					{struct.name}
-					{"="*(120 - o.indent_width - 3)}-->'''
-                    )
-                    with Indent(o, pre=f'\n\n<Type Name="{escape(struct.qualified_type)}">', post='</Type>'):
+        with MetaScope(self):
+            o(
+                rf'''
+            <?xml version="1.0" encoding="utf-8"?>
+            <!--
+            // This file was generated by soagen v{VERSION_STRING} - do not modify it directly
+            // https://marzer.github.io/soagen
+            -->
+            <AutoVisualizer xmlns="http://schemas.microsoft.com/vstudio/debugger/natvis/2010">
+            '''
+            )
+
+            with Indent(o):
+                for struct in self.structs:
+                    with MetaScope(struct):
                         o(
-                            r'''
-						<Intrinsic Name="size" Expression="table_.count_" />
-						<Intrinsic Name="size_bytes" Expression="table_.alloc_.size_in_bytes" />
-						<Intrinsic Name="capacity" Expression="table_.capacity_.first_" />
-						'''
+                            rf'''
+                        <!--{"="*(120 - o.indent_width - 4)}
+                        {struct.name}
+                        {"="*(120 - o.indent_width - 3)}-->'''
                         )
-                        for col in struct.columns:
-                            o(
-                                rf'''
-							<Intrinsic
-								Name="get_{col.index}"
-								Expression="reinterpret_cast&lt;{escape(col.type)}*&gt;(table_.alloc_.columns[{col.index}])"
-							/>
-							'''
-                            )
-                        o(r'<DisplayString>{{ size={size()} }}</DisplayString>')
-                        with Indent(o, pre='<Expand>', post='</Expand>\n'):
+                        with Indent(o, pre=f'\n\n<Type Name="{escape(struct.qualified_type)}">', post='</Type>'):
                             o(
                                 r'''
-							<Item Name="[size]">size()</Item>
-							<Item Name="[capacity]">capacity()</Item>
-							<Item Name="[allocation_size]">size_bytes()</Item>
-							'''
+                            <Intrinsic Name="size" Expression="table_.count_" />
+                            <Intrinsic Name="size_bytes" Expression="table_.alloc_.size_in_bytes" />
+                            <Intrinsic Name="capacity" Expression="table_.capacity_.first_" />
+                            '''
                             )
                             for col in struct.columns:
-                                get = rf'get_{col.index}()'
                                 o(
                                     rf'''
-								<Synthetic Name="{col.name}">
-									<DisplayString Condition="size() &gt; 3u">{{{{ {{*({get})}}, {{*({get} + 1)}}, {{*({get} + 2)}}, ... }}}}</DisplayString>
-									<DisplayString Condition="size() == 3u">{{{{ {{*({get})}}, {{*({get} + 1)}}, {{*({get} + 2)}} }}}}</DisplayString>
-									<DisplayString Condition="size() == 2u">{{{{ {{*({get})}}, {{*({get} + 1)}} }}}}</DisplayString>
-									<DisplayString Condition="size() == 1u">{{{{ {{*({get})}} }}}}</DisplayString>
-									<DisplayString Condition="size() == 0u"></DisplayString>
-									<Expand>
-										<ArrayItems>
-											<Size>size()</Size>
-											<ValuePointer>{get}</ValuePointer>
-										</ArrayItems>
-									</Expand>
-								</Synthetic>
-								'''
+                                <Intrinsic
+                                    Name="get_{col.index}"
+                                    Expression="reinterpret_cast&lt;{escape(col.type)}*&gt;(table_.alloc_.columns[{col.index}])"
+                                />
+                                '''
                                 )
+                            o(r'<DisplayString>{{ size={size()} }}</DisplayString>')
+                            with Indent(o, pre='<Expand>', post='</Expand>\n'):
+                                o(
+                                    r'''
+                                <Item Name="[size]">size()</Item>
+                                <Item Name="[capacity]">capacity()</Item>
+                                <Item Name="[allocation_size]">size_bytes()</Item>
+                                '''
+                                )
+                                for col in struct.columns:
+                                    get = rf'get_{col.index}()'
+                                    o(
+                                        rf'''
+                                    <Synthetic Name="{col.name}">
+                                        <DisplayString Condition="size() &gt; 3u">{{{{ {{*({get})}}, {{*({get} + 1)}}, {{*({get} + 2)}}, ... }}}}</DisplayString>
+                                        <DisplayString Condition="size() == 3u">{{{{ {{*({get})}}, {{*({get} + 1)}}, {{*({get} + 2)}} }}}}</DisplayString>
+                                        <DisplayString Condition="size() == 2u">{{{{ {{*({get})}}, {{*({get} + 1)}} }}}}</DisplayString>
+                                        <DisplayString Condition="size() == 1u">{{{{ {{*({get})}} }}}}</DisplayString>
+                                        <DisplayString Condition="size() == 0u"></DisplayString>
+                                        <Expand>
+                                            <ArrayItems>
+                                                <Size>size()</Size>
+                                                <ValuePointer>{get}</ValuePointer>
+                                            </ArrayItems>
+                                        </Expand>
+                                    </Synthetic>
+                                    '''
+                                    )
+
+                        row_types = [
+                            rf'soagen::row<{struct.qualified_type}, {struct.column_indices}>',
+                            rf'soagen::row<{struct.qualified_type}&, {struct.column_indices}>',
+                            rf'soagen::row<{struct.qualified_type}&&, {struct.column_indices}>',
+                            rf'soagen::row<const {struct.qualified_type}, {struct.column_indices}>',
+                            rf'soagen::row<const {struct.qualified_type}&, {struct.column_indices}>',
+                            rf'soagen::row<const {struct.qualified_type}&&, {struct.column_indices}>',
+                        ]
+                        with Indent(o, pre=f'\n\n<Type Name="{escape(row_types[0])}">', post='</Type>'):
+                            for i in range(1, len(row_types)):
+                                o(rf'<AlternativeType Name="{escape(row_types[i])}" />')
+
+                            s = r''
+                            if len(struct.columns) > 1:
+                                s += r'{{ '
+                            s += r'{'
+                            s += r'}, {'.join(col.name for col in struct.columns[:8])
+                            s += r'}'
+                            if len(struct.columns) > 8:
+                                s += r', ...'
+                            if len(struct.columns) > 1:
+                                s += r' }}'
+                            o(rf'<DisplayString>{s}</DisplayString>')
+                            with Indent(o, pre='<Expand>', post='</Expand>\n'):
+                                for col in struct.columns:
+                                    o(rf'<Item Name="{col.name}">{col.name}</Item>')
 
-                    row_types = [
-                        rf'soagen::row<{struct.qualified_type}, {struct.column_indices}>',
-                        rf'soagen::row<{struct.qualified_type}&, {struct.column_indices}>',
-                        rf'soagen::row<{struct.qualified_type}&&, {struct.column_indices}>',
-                        rf'soagen::row<const {struct.qualified_type}, {struct.column_indices}>',
-                        rf'soagen::row<const {struct.qualified_type}&, {struct.column_indices}>',
-                        rf'soagen::row<const {struct.qualified_type}&&, {struct.column_indices}>',
-                    ]
-                    with Indent(o, pre=f'\n\n<Type Name="{escape(row_types[0])}">', post='</Type>'):
-                        for i in range(1, len(row_types)):
-                            o(rf'<AlternativeType Name="{escape(row_types[i])}" />')
-
-                        s = r''
-                        if len(struct.columns) > 1:
-                            s += r'{{ '
-                        s += r'{'
-                        s += r'}, {'.join(col.name for col in struct.columns[:8])
-                        s += r'}'
-                        if len(struct.columns) > 8:
-                            s += r', ...'
-                        if len(struct.columns) > 1:
-                            s += r' }}'
-                        o(rf'<DisplayString>{s}</DisplayString>')
-                        with Indent(o, pre='<Expand>', post='</Expand>\n'):
-                            for col in struct.columns:
-                                o(rf'<Item Name="{col.name}">{col.name}</Item>')
-
-        o(r'</AutoVisualizer>')
+            o(r'</AutoVisualizer>')
 
 
 __all__ = [r'NatvisFile']
```

### Comparing `soagen-0.2.0/src/soagen/paths.py` & `soagen-0.3.0/src/soagen/paths.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/preprocessor.py` & `soagen-0.3.0/src/soagen/preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,30 +46,26 @@
         self.__include_stack = []
         self.__entry_root = None
         self.__string = self.__preprocess(file)
         # do some cleanup of the preprocessed file
         while True:
             s = self.__string
             # trailing whitespace
-            self.__string = re.sub('([^ \t])[ \t]+\n', r'\1\n', s)
+            s = re.sub('([^ \t])[ \t]+\n', r'\1\n', s)
+            # double blank lines
+            s = re.sub('\n\n\n+', '\n\n', s)
             # magic comments
-            blank_line = r'(?:[ \t]*\n)'
-            magic_comment = r'(?:[ \t]*//[#!</][^\n]*)'
-            s = re.sub(rf'\n{magic_comment}\n{blank_line}+{magic_comment}\n', '\n', s)
-            s = re.sub(rf'([{{,])\s*\n(?:{magic_comment}\n|{blank_line})+', r'\1\n', s)
-            s = re.sub(rf'\n?(?:{magic_comment}\n)+', '\n', s)
+            s = re.sub(rf'(?://(?:[#!</]|[ \t]?(?:\^\^\^|vvv))).*?($)', r'\1', s, flags=re.MULTILINE)
             # consecutive header separators
             header_separator = r'(?://\*\*\*\**[ \t]+[a-zA-Z0-9_/.-]+[ \t]+\*\*\*\*+\n)'
-            s = re.sub(rf'(?:{header_separator}{blank_line}*)+({header_separator})', r'\1', s)
-            # double blank lines
-            s = re.sub('\n(?:[ \t]*\n[ \t]*)+\n', '\n\n', s)
+            s = re.sub(rf'(?:{header_separator}(?:[ \t]*\n)*)+({header_separator})', r'\1', s)
             # weird spacing edge case around pp directives
             s = re.sub('\n[}]\n#', r'\n}\n\n#', s)
-            # blank lines following opening brackets or a comma
-            s = re.sub(r'([^@][({,])\n\n', r'\1\n', s)
+            # blank lines following a comma, opening bracket, or colon
+            s = re.sub(r'([{(\[:,])\n\n', r'\1\n', s)
             # blank lines preceeding closing brackets
             s = re.sub(r'\n\n([ \t]*[})])', r'\n\1', s)
             # empty #if blocks
             s = re.sub(r'#if(n?def)?[ \t]+[a-zA-Z0-9_]+\s*?\n+\s*?#endif', r'\n', s)
             # empty #else blocks
             s = re.sub(r'#else\s*?\n+\s*?#endif', r'#endif\n', s)
             # #if SOAGEN_DOXYGEN ... #else ... #endif
```

### Comparing `soagen-0.2.0/src/soagen/schemas.py` & `soagen-0.3.0/src/soagen/schemas.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/struct.py` & `soagen-0.3.0/src/soagen/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         if self.reverse_iterators:
             log.w(rf'{current_schema_context()}reverse_iterators: not currently implemented')
             self.reverse_iterators = False
 
         self.qualified_type = rf'{self.config.namespace}::{self.type}' if self.config.namespace else self.type
         self.qualified_name = self.qualified_type
         self.index = -1  # set by the config
+
         self.meta = MetaVars()
         self.meta.push(r'name', self.name)
         self.meta.push(r'type', self.type)
         self.meta.push(r'qualified_name', self.qualified_name)
         self.meta.push(r'qualified_type', self.qualified_type)
         self.meta.push(r'struct::name', self.name)
         self.meta.push(r'struct::type', self.type)
@@ -185,75 +186,77 @@
         assert isinstance(index, int)
         assert index >= 0
         self.index = index
         self.meta.push('index', index)
         self.meta.push('struct::index', index)
 
     def write_forward_declarations(self, o: Writer):
-        with MetaScope(self.config.meta_stack, self.meta):
+        with MetaScope(self):
             o(rf'class {self.type};')
 
     def write_soagen_specializations(self, o: Writer):
-        o(
-            rf'''
-        template <>
-        inline constexpr bool is_soa<{self.qualified_name}> = true;
-        '''
-        )
+        with MetaScope(self):
+            o(
+                rf'''
+            template <>
+            inline constexpr bool is_soa<{self.qualified_name}> = true;
+            '''
+            )
 
     def write_soagen_detail_specializations(self, o: Writer):
-        max_length = 0
-        for col in self.columns:
-            max_length = max(len(col.name), max_length)
-        with StringIO() as buf:
-            buf.write('table_traits<\n')
-            for i in range(len(self.columns)):
-                if i:
-                    buf.write(f',\n')
-                col = self.columns[i]
-                buf.write(f'{o.indent_str*4}/* {col.name:>{max_length}} */ column_traits<{col.type}')
-                if col.alignment > 0:
-                    buf.write(rf', soagen::max(size_t{{ {col.alignment} }}, alignof({col.type}))')
-                if col.param_type:
-                    if not col.param_type:
-                        buf.write(rf', alignof({col.type})')
-                    buf.write(rf', {col.param_type}')
+        with MetaScope(self):
+            max_length = 0
+            for col in self.columns:
+                max_length = max(len(col.name), max_length)
+            with StringIO() as buf:
+                buf.write('table_traits<\n')
+                for i in range(len(self.columns)):
+                    if i:
+                        buf.write(f',\n')
+                    col = self.columns[i]
+                    buf.write(f'{o.indent_str*5}/* {col.name:>{max_length}} */ column_traits<{col.type}')
+                    if col.alignment > 0:
+                        buf.write(rf', soagen::max(size_t{{ {col.alignment} }}, alignof({col.type}))')
+                    if col.param_type:
+                        if not col.param_type:
+                            buf.write(rf', alignof({col.type})')
+                        buf.write(rf', {col.param_type}')
+                    buf.write(rf'>')
                 buf.write(rf'>')
-            buf.write(rf'>')
+                o(
+                    rf'''
+                template <>
+                struct table_traits_type_<{self.qualified_name}>
+                {{
+                    using type = {buf.getvalue()};
+                }};
+
+                template <>
+                struct allocator_type_<{self.qualified_name}>
+                {{
+                    using type = {self.allocator};
+                }};
+                '''
+                )
+
+                for col in self.columns:
+                    o(rf'SOAGEN_MAKE_COLUMN({self.qualified_name}, {col.index}, {col.name});')
+
             o(
                 rf'''
             template <>
-            struct table_traits_type_<{self.qualified_name}>
+            struct table_type_<{self.qualified_name}>
             {{
-                using type = {buf.getvalue()};
-            }};
-
-            template <>
-            struct allocator_type_<{self.qualified_name}>
-            {{
-                using type = {self.allocator};
+                using type = table<table_traits_type<{self.qualified_name}>, {self.allocator}>;
             }};
             '''
             )
 
-            for col in self.columns:
-                o(rf'SOAGEN_MAKE_COLUMN({self.qualified_name}, {col.index}, {col.name});')
-
-        o(
-            rf'''
-        template <>
-        struct table_type_<{self.qualified_name}>
-        {{
-            using type = table<table_traits_type<{self.qualified_name}>, {self.allocator}>;
-        }};
-        '''
-        )
-
     def write_class_definition(self, o: Writer):
-        with MetaScope(self.config.meta_stack, self.meta) as meta:
+        with MetaScope(self):
             if self.prologue:
                 o(
                     f'''
                 {self.prologue}
                 '''
                 )
 
@@ -751,19 +754,21 @@
                             r'These overloads are only available when all the column types are move-constructible and move-assignable.',
                         ),
                     ):
                         sfinae_variant = -1
                         sfinae_sig_hash = ''
                         with DoxygenMemberGroup(o, group, availability=availability):
                             for func in funcs:
-                                for row_overload in (False, True):
-                                    if row_overload and func in (r'emplace_back', r'emplace'):
+                                for tuple_overload in (False, True):
+                                    if tuple_overload and func not in (r'emplace_back', r'emplace'):
                                         continue
                                     for rvalue_overload in (False, True):
-                                        if rvalue_overload and (row_overload or func in (r'emplace_back', r'emplace')):
+                                        if rvalue_overload and (
+                                            tuple_overload or func in (r'emplace_back', r'emplace')
+                                        ):
                                             continue
                                         for iterator_overload in (None, r'iterator', r'const_iterator'):
                                             if iterator_overload and func in (r'push_back', r'emplace_back'):
                                                 continue
                                             if iterator_overload and not self.iterators:
                                                 continue
 
@@ -785,23 +790,22 @@
                                                     deduced.append(False)
                                                 else:
                                                     types.append(r'size_type')
                                                     names.append(r'index_')
                                                     forwards.append(names[-1])
                                                     deduced.append(False)
 
-                                            if row_overload:
-                                                template_params.append(r'typename Table')
-                                                template_params.append(r'auto... Columns')
-                                                template_defaults += ['', '']
-                                                types.append(r'const soagen::row<Table, Columns...>&')
-                                                names.append(r'row_')
+                                            if tuple_overload:
+                                                template_params.append(r'typename Tuple')
+                                                template_defaults += ['']
+                                                types.append(r'Tuple&&')
+                                                names.append(r'tuple_')
                                                 deduced.append(True)
                                                 defaults.append('')
-                                                forwards.append(names[-1])
+                                                forwards.append(rf'static_cast<{types[-1]}>({names[-1]})')
                                             else:
                                                 for col in self.columns:
                                                     names.append(col.name)
                                                     defaults.append(col.default)
                                                     if func in (r'emplace_back', r'emplace'):
                                                         typename = utils.to_pascal_case(col.name)
                                                         if typename == col.name:
@@ -829,16 +833,16 @@
                                                 sfinae_variant = 0 if rvalue_overload else -1
                                                 sfinae_sig_hash = sig_hash
 
                                             sfinae = []
                                             sfinae_emitted = False
                                             sfinae_template_dependent = False
                                             sfinae_condition_string = ''
-                                            if row_overload:
-                                                sfinae.append(r'soagen::is_soa<soagen::remove_cvref<Table>>')
+                                            if tuple_overload:
+                                                sfinae.append(r'table_traits::row_constructible_from<Tuple&&>')
                                                 sfinae_template_dependent = True
                                             if rvalue_overload:
                                                 sfinae.append(r'table_traits::rvalue_type_list_is_distinct')
                                             if func in (r'insert', r'emplace'):
                                                 sfinae.append(r'table_traits::all_move_constructible')
                                                 sfinae.append(r'table_traits::all_move_assignable')
                                             hidden_template = bool(sfinae) and not template_params
@@ -893,14 +897,16 @@
                                                     s += 'Inserts a new row'
                                                 elif func == r'push_back':
                                                     s += 'Adds a new row'
                                                 if func in (r'insert', r'emplace'):
                                                     s += ' at an arbitrary position in the table'
                                                 elif func.endswith(r'_back'):
                                                     s += ' at the end of the table'
+                                                if tuple_overload:
+                                                    s += ' by unpacking a tuple-like object'
                                                 if rvalue_overload:
                                                     s += ' (rvalue overload)'
                                                 s += '.\n'
                                                 if func in (r'insert', r'emplace'):
                                                     s += '///\n'
                                                     s += '/// @availability This overload is only available when all'
                                                     s += ' the column types are move-constructible and move-assignable.\n'
@@ -975,20 +981,20 @@
 
                                             # noexcept(...)
                                             backing_func = (
                                                 r'emplace' if func in (r'insert', r'emplace') else r'emplace_back'
                                             )
                                             s += '\tnoexcept('
                                             if func == 'push_back':
-                                                if row_overload:
+                                                if tuple_overload:
                                                     s += rf'table_traits::row_push_back_is_nothrow<table_type&, {types[0]}>'
                                                 else:
                                                     s += rf'table_traits::{"rvalue_" if rvalue_overload else ""}push_back_is_nothrow<table_type&>'
                                             elif func == 'insert':
-                                                if row_overload:
+                                                if tuple_overload:
                                                     s += rf'table_traits::row_insert_is_nothrow<table_type&, {types[-1]}>'
                                                 else:
                                                     s += rf'table_traits::{"rvalue_" if rvalue_overload else ""}insert_is_nothrow<table_type&>'
                                             elif func == 'emplace_back':
                                                 s += rf'table_traits::emplace_back_is_nothrow<table_type&, {", ".join(types)}>'
                                             elif func == 'emplace':
                                                 s += rf'table_traits::emplace_is_nothrow<table_type&, {", ".join(types[1:])}>'
@@ -1138,25 +1144,29 @@
                             )
                         for const in ('', 'const '):
                             o(
                                 rf'''
                             {doxygen(r"""
                             @brief Invokes a function once for each column data pointer.
 
-                            @tparam Func A callable type compatible with one of the following signatures:<br>
-                                     - `void(auto*, size_type)`
-                                     - `void(size_type, auto*)`
-                                     - `void(auto*)`
+                            @tparam Func A callable type compatible with one of the following signatures:<ul>
+                                     <li> `void(auto*, std::integral_constant<size_type, N>)`
+                                     <li> `void(auto*, size_type)`
+                                     <li> `void(std::integral_constant<size_type, N>, auto*)`
+                                     <li> `void(size_type, auto*)`
+                                     <li> `void(auto*)`
+                            </ul>
+                            Overload resolution is performed in the order listed above.
 
                             @param func The callable to invoke.""")}
                             template <typename Func>
                             constexpr void for_each_column(Func&& func) {const}//
-                                noexcept(table_traits::for_each_column_ptr_nothrow_invocable<Func&&{', true'if const else ''}>)
+                                noexcept(table_traits::for_each_column_nothrow_invocable<Func&&{', true'if const else ''}>)
                             {{
-                                {rf'{NEWLINE}{o.indent_str*8}'.join([rf'soagen::invoke_with_optarg(static_cast<Func&&>(func), this->template column<{col.index}>(), size_type{{ {col.index} }});' for col in self.columns])}
+                                {rf'{NEWLINE}{o.indent_str*8}'.join([rf'soagen::invoke_with_optional_index<{col.index}>(static_cast<Func&&>(func), this->template column<{col.index}>());' for col in self.columns])}
                             }}
                             '''
                             )
 
                 with DoxygenMemberGroup(o, 'Row access'):
                     with Public(o):
                         for const, ref in (('', '&'), ('', '&&'), ('const ', '&')):
```

### Comparing `soagen-0.2.0/src/soagen/type_list.py` & `soagen-0.3.0/src/soagen/type_list.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/variable.py` & `soagen-0.3.0/src/soagen/variable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/version.py` & `soagen-0.3.0/src/soagen/version.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen/writer.py` & `soagen-0.3.0/src/soagen/writer.py`

 * *Files identical despite different names*

### Comparing `soagen-0.2.0/src/soagen.egg-info/PKG-INFO` & `soagen-0.3.0/src/soagen.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,21 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.3.0
+
+-   Added `hpp.combined`
+-   Added `std::integral_constant<size_t>` to the overload set used by `for_each_column()`
+-   Added support for constructing rows from all `std::tuple`-like types
+-   Optimized bulk-swap operations
+
 ## v0.2.0
 
 -   Added `structs.annotations`
 -   Added `structs.attributes`
 -   Added `auto` option for `structs.default_constructible`
 -   Added `soagen::row_base`
 -   Added `soagen::table_base`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.2.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.3.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,17 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.2.0 - Added `structs.annotations` - Added
+sponsors/marzer # Changelog ## v0.3.0 - Added `hpp.combined` - Added `std::
+integral_constant` to the overload set used by `for_each_column()` - Added
+support for constructing rows from all `std::tuple`-like types - Optimized
+bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
 `structs.attributes` - Added `auto` option for `structs.default_constructible`
 - Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
 iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
 Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
 columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
 First public release ð&#xFE0F;
```

### Comparing `soagen-0.2.0/src/soagen.egg-info/SOURCES.txt` & `soagen-0.3.0/src/soagen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,21 @@
 src/soagen.egg-info/entry_points.txt
 src/soagen.egg-info/requires.txt
 src/soagen.egg-info/top_level.txt
 src/soagen.egg-info/zip-safe
 src/soagen/hpp/.clang-format
 src/soagen/hpp/allocator.hpp
 src/soagen/hpp/column_traits.hpp
+src/soagen/hpp/core.hpp
 src/soagen/hpp/header_end.hpp
 src/soagen/hpp/header_start.hpp
 src/soagen/hpp/iterator.hpp
-src/soagen/hpp/meta.hpp
 src/soagen/hpp/mixins.hpp
 src/soagen/hpp/row.hpp
 src/soagen/hpp/soagen.hpp
 src/soagen/hpp/table.hpp
 src/soagen/hpp/table_traits.hpp
 src/soagen/hpp/generated/compressed_pair.hpp
-src/soagen/hpp/generated/core.hpp
 src/soagen/hpp/generated/functions.hpp
 src/soagen/hpp/generated/preprocessor.hpp
 src/soagen/hpp/generated/version.hpp
 src/soagen/hpp/single/soagen.hpp
```

