# Comparing `tmp/yams-0.50.1.tar.gz` & `tmp/yams-0.50.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yams-0.50.1.tar", last modified: Thu Aug  3 15:34:15 2023, max compression
+gzip compressed data, was "yams-0.50.2.tar", last modified: Fri Aug  4 12:25:02 2023, max compression
```

## Comparing `yams-0.50.1.tar` & `yams-0.50.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.519949 yams-0.50.1/
--rw-rw-rw-   0 root         (0) root         (0)    17987 2023-08-03 15:33:19.000000 yams-0.50.1/COPYING
--rw-rw-rw-   0 root         (0) root         (0)    26527 2023-08-03 15:33:19.000000 yams-0.50.1/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)    13724 2023-08-03 15:33:19.000000 yams-0.50.1/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-08-03 15:33:19.000000 yams-0.50.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1397 2023-08-03 15:34:15.515949 yams-0.50.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-08-03 15:33:19.000000 yams-0.50.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-08-03 15:33:19.000000 yams-0.50.1/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.219945 yams-0.50.1/bin/
--rwxrwxrwx   0 root         (0) root         (0)     3838 2023-08-03 15:33:19.000000 yams-0.50.1/bin/owl2yams
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-check
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-check.bat
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-view
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-view.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.247945 yams-0.50.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-08-03 15:33:19.000000 yams-0.50.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1923 2023-08-03 15:33:19.000000 yams-0.50.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-08-03 15:33:19.000000 yams-0.50.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-08-03 15:33:19.000000 yams-0.50.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-08-03 15:33:19.000000 yams-0.50.1/docs/yams.rst
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-08-03 15:33:19.000000 yams-0.50.1/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-08-03 15:33:19.000000 yams-0.50.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 15:34:15.519949 yams-0.50.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-08-03 15:33:19.000000 yams-0.50.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.315946 yams-0.50.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.323946 yams-0.50.1/test/data/
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.331946 yams-0.50.1/test/data/dbmodel/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/dbmodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/dbmodel/blog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.331946 yams-0.50.1/test/data/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/Company.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/Dates.py
--rw-rw-rw-   0 root         (0) root         (0)     3252 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/State.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3610 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/toignore
--rw-rw-rw-   0 root         (0) root         (0)     1625 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema1.txt
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema2.txt
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema_post_build_callback.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.335946 yams-0.50.1/test/data2/
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-08-03 15:33:19.000000 yams-0.50.1/test/data2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-08-03 15:33:19.000000 yams-0.50.1/test/data2/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    13040 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)     6356 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_diff.py
--rw-rw-rw-   0 root         (0) root         (0)    36195 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    29219 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2742 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_schema2dot.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     9932 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_specialization.py
--rw-rw-rw-   0 root         (0) root         (0)     2497 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_xy.py
--rw-rw-rw-   0 root         (0) root         (0)     2559 2023-08-03 15:33:19.000000 yams-0.50.1/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.471948 yams-0.50.1/yams/
--rw-rw-rw-   0 root         (0) root         (0)     7211 2023-08-03 15:33:19.000000 yams-0.50.1/yams/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5163 2023-08-03 15:33:19.000000 yams-0.50.1/yams/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39988 2023-08-03 15:33:19.000000 yams-0.50.1/yams/buildobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    29418 2023-08-03 15:33:19.000000 yams-0.50.1/yams/constraints.py
--rw-rw-rw-   0 root         (0) root         (0)    12344 2023-08-03 15:33:19.000000 yams-0.50.1/yams/diff.py
--rw-rw-rw-   0 root         (0) root         (0)     6181 2023-08-03 15:33:19.000000 yams-0.50.1/yams/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 15:33:19.000000 yams-0.50.1/yams/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    16241 2023-08-03 15:33:19.000000 yams-0.50.1/yams/reader.py
--rw-rw-rw-   0 root         (0) root         (0)    71338 2023-08-03 15:33:19.000000 yams-0.50.1/yams/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12618 2023-08-03 15:33:19.000000 yams-0.50.1/yams/schema2dot.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-08-03 15:33:19.000000 yams-0.50.1/yams/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4506 2023-08-03 15:33:19.000000 yams-0.50.1/yams/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-08-03 15:33:19.000000 yams-0.50.1/yams/types.py
--rw-rw-rw-   0 root         (0) root         (0)     5851 2023-08-03 15:33:19.000000 yams-0.50.1/yams/xy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.499949 yams-0.50.1/yams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1397 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1218 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    21077 2023-08-03 15:33:19.000000 yams-0.50.1/yams.png
--rw-rw-rw-   0 root         (0) root         (0)     5326 2023-08-03 15:33:19.000000 yams-0.50.1/yams.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.044816 yams-0.50.2/
+-rw-rw-rw-   0 root         (0) root         (0)    17987 2023-08-04 12:24:40.000000 yams-0.50.2/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2023-08-04 12:24:40.000000 yams-0.50.2/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)    13724 2023-08-04 12:24:40.000000 yams-0.50.2/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-08-04 12:24:40.000000 yams-0.50.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-08-04 12:25:02.044816 yams-0.50.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-08-04 12:24:40.000000 yams-0.50.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-08-04 12:24:40.000000 yams-0.50.2/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.016815 yams-0.50.2/bin/
+-rwxrwxrwx   0 root         (0) root         (0)     3838 2023-08-04 12:24:40.000000 yams-0.50.2/bin/owl2yams
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-08-04 12:24:40.000000 yams-0.50.2/bin/yams-check
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-08-04 12:24:40.000000 yams-0.50.2/bin/yams-check.bat
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-08-04 12:24:40.000000 yams-0.50.2/bin/yams-view
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-08-04 12:24:40.000000 yams-0.50.2/bin/yams-view.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.020815 yams-0.50.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-08-04 12:24:40.000000 yams-0.50.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1923 2023-08-04 12:24:40.000000 yams-0.50.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-08-04 12:24:40.000000 yams-0.50.2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-08-04 12:24:40.000000 yams-0.50.2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-08-04 12:24:40.000000 yams-0.50.2/docs/yams.rst
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-08-04 12:24:40.000000 yams-0.50.2/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-08-04 12:24:40.000000 yams-0.50.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 12:25:02.044816 yams-0.50.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-08-04 12:24:40.000000 yams-0.50.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.024815 yams-0.50.2/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.028816 yams-0.50.2/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.028816 yams-0.50.2/test/data/dbmodel/
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/dbmodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/dbmodel/blog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.032816 yams-0.50.2/test/data/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema/Company.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema/Dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema/State.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema/toignore
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema1.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-08-04 12:24:40.000000 yams-0.50.2/test/data/schema_post_build_callback.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.036816 yams-0.50.2/test/data2/
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-08-04 12:24:40.000000 yams-0.50.2/test/data2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-08-04 12:24:40.000000 yams-0.50.2/test/data2/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    13040 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)     6356 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_diff.py
+-rw-rw-rw-   0 root         (0) root         (0)    36195 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    29219 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2742 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_schema2dot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_specialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2023-08-04 12:24:40.000000 yams-0.50.2/test/unittest_xy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2023-08-04 12:24:40.000000 yams-0.50.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.040816 yams-0.50.2/yams/
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2023-08-04 12:24:40.000000 yams-0.50.2/yams/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5163 2023-08-04 12:24:40.000000 yams-0.50.2/yams/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39988 2023-08-04 12:24:40.000000 yams-0.50.2/yams/buildobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    29418 2023-08-04 12:24:40.000000 yams-0.50.2/yams/constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)    12344 2023-08-04 12:24:40.000000 yams-0.50.2/yams/diff.py
+-rw-rw-rw-   0 root         (0) root         (0)     6181 2023-08-04 12:24:40.000000 yams-0.50.2/yams/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 12:24:40.000000 yams-0.50.2/yams/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    16241 2023-08-04 12:24:40.000000 yams-0.50.2/yams/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    71338 2023-08-04 12:24:40.000000 yams-0.50.2/yams/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12618 2023-08-04 12:24:40.000000 yams-0.50.2/yams/schema2dot.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-08-04 12:24:40.000000 yams-0.50.2/yams/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4506 2023-08-04 12:24:40.000000 yams-0.50.2/yams/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-08-04 12:24:40.000000 yams-0.50.2/yams/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2023-08-04 12:24:40.000000 yams-0.50.2/yams/xy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:25:02.044816 yams-0.50.2/yams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-08-04 12:25:01.000000 yams-0.50.2/yams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-08-04 12:25:01.000000 yams-0.50.2/yams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 12:25:01.000000 yams-0.50.2/yams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-08-04 12:25:01.000000 yams-0.50.2/yams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 12:25:01.000000 yams-0.50.2/yams.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    21077 2023-08-04 12:24:40.000000 yams-0.50.2/yams.png
+-rw-rw-rw-   0 root         (0) root         (0)     5326 2023-08-04 12:24:40.000000 yams-0.50.2/yams.svg
```

### Comparing `yams-0.50.1/COPYING` & `yams-0.50.2/COPYING`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/COPYING.LESSER` & `yams-0.50.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/ChangeLog` & `yams-0.50.2/ChangeLog`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/PKG-INFO` & `yams-0.50.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yams
-Version: 0.50.1
+Version: 0.50.2
 Summary: entity / relation schema
 Home-page: https://forge.extranet.logilab.fr/open-source/yams
 Author: Logilab
 Author-email: devel@logilab.fr
 License: LGPL
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yams-0.50.1/README.rst` & `yams-0.50.2/README.rst`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/__pkginfo__.py` & `yams-0.50.2/__pkginfo__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # pylint: disable-msg=W0622
 
 # package name
 modname = "yams"
 
 # release version
-numversion = (0, 50, 1)
+numversion = (0, 50, 2)
 version = ".".join(str(num) for num in numversion)
 
 # license and copyright
 license = "LGPL"
 
 # short and long description
 description = "entity / relation schema"
```

### Comparing `yams-0.50.1/bin/owl2yams` & `yams-0.50.2/bin/owl2yams`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/docs/Makefile` & `yams-0.50.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/docs/conf.py` & `yams-0.50.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/docs/make.bat` & `yams-0.50.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/docs/yams.rst` & `yams-0.50.2/docs/yams.rst`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/setup.py` & `yams-0.50.2/setup.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/__init__.py` & `yams-0.50.2/test/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/dbmodel/__init__.py` & `yams-0.50.2/test/data/dbmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/dbmodel/blog.py` & `yams-0.50.2/test/data/dbmodel/blog.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema/Company.py` & `yams-0.50.2/test/data/schema/Company.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema/Dates.py` & `yams-0.50.2/test/data/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema/State.py` & `yams-0.50.2/test/data/schema/State.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema/__init__.py` & `yams-0.50.2/test/data/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema/schema.py` & `yams-0.50.2/test/data/schema/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema1.txt` & `yams-0.50.2/test/data/schema1.txt`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema2.txt` & `yams-0.50.2/test/data/schema2.txt`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data/schema_post_build_callback.py` & `yams-0.50.2/test/data/schema_post_build_callback.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data2/__init__.py` & `yams-0.50.2/test/data2/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/data2/schema.py` & `yams-0.50.2/test/data2/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_constraints.py` & `yams-0.50.2/test/unittest_constraints.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_diff.py` & `yams-0.50.2/test/unittest_diff.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_reader.py` & `yams-0.50.2/test/unittest_reader.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_schema.py` & `yams-0.50.2/test/unittest_schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_schema2dot.py` & `yams-0.50.2/test/unittest_schema2dot.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_serialize.py` & `yams-0.50.2/test/unittest_serialize.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_specialization.py` & `yams-0.50.2/test/unittest_specialization.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/test/unittest_xy.py` & `yams-0.50.2/test/unittest_xy.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/tox.ini` & `yams-0.50.2/tox.ini`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/__init__.py` & `yams-0.50.2/yams/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/_exceptions.py` & `yams-0.50.2/yams/_exceptions.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/buildobjs.py` & `yams-0.50.2/yams/buildobjs.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
     # subject or object the relation, the cardinality, the constraints
     # and the symmetric property.
     # """
 
     subject: Union[nullobject, str, List[str], None] = MARKER
     object: Union[nullobject, str, List[str], None] = MARKER
     cardinality: Union[nullobject, str, None] = MARKER
-    constraints: list[BaseConstraint] = MARKER  # type: ignore
+    constraints: List[BaseConstraint] = MARKER  # type: ignore
     symmetric = MARKER
     inlined = MARKER
     formula = MARKER
 
     def __init__(
         self,
         subject: Optional[Union[str, Tuple[str]]] = None,
```

### Comparing `yams-0.50.1/yams/constraints.py` & `yams-0.50.2/yams/constraints.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/diff.py` & `yams-0.50.2/yams/diff.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/interfaces.py` & `yams-0.50.2/yams/interfaces.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/reader.py` & `yams-0.50.2/yams/reader.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/schema.py` & `yams-0.50.2/yams/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/schema2dot.py` & `yams-0.50.2/yams/schema2dot.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/serialize.py` & `yams-0.50.2/yams/serialize.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/tools.py` & `yams-0.50.2/yams/tools.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/types.py` & `yams-0.50.2/yams/types.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams/xy.py` & `yams-0.50.2/yams/xy.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams.egg-info/PKG-INFO` & `yams-0.50.2/yams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yams
-Version: 0.50.1
+Version: 0.50.2
 Summary: entity / relation schema
 Home-page: https://forge.extranet.logilab.fr/open-source/yams
 Author: Logilab
 Author-email: devel@logilab.fr
 License: LGPL
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yams-0.50.1/yams.egg-info/SOURCES.txt` & `yams-0.50.2/yams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams.png` & `yams-0.50.2/yams.png`

 * *Files identical despite different names*

### Comparing `yams-0.50.1/yams.svg` & `yams-0.50.2/yams.svg`

 * *Files identical despite different names*

