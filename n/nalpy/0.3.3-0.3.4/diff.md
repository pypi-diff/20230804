# Comparing `tmp/nalpy-0.3.3.tar.gz` & `tmp/nalpy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalpy-0.3.3.tar", last modified: Thu Aug  3 21:39:48 2023, max compression
+gzip compressed data, was "nalpy-0.3.4.tar", last modified: Thu Aug  3 22:13:16 2023, max compression
```

## Comparing `nalpy-0.3.3.tar` & `nalpy-0.3.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.761700 nalpy-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 21:39:35.000000 nalpy-0.3.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.745699 nalpy-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.749699 nalpy-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 21:39:35.000000 nalpy-0.3.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-08-03 21:39:35.000000 nalpy-0.3.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.749699 nalpy-0.3.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-03 21:39:35.000000 nalpy-0.3.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-03 21:39:48.761700 nalpy-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 21:39:35.000000 nalpy-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.749699 nalpy-0.3.3/nalpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.749699 nalpy-0.3.3/nalpy/console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/console_utils/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.753699 nalpy-0.3.3/nalpy/humanizer/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/bytes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.753699 nalpy-0.3.3/nalpy/humanizer/inflections/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/inflections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/inflections/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.753699 nalpy-0.3.3/nalpy/humanizer/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/numbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/numbers/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/numbers/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/numbers/heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/numbers/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/numbers/number_to_roman_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/numbers/number_to_words_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/humanizer/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.753699 nalpy-0.3.3/nalpy/math/
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.757699 nalpy-0.3.3/nalpy/math/_c_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   355223 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/functions.c
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/functions.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/functions.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   538481 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/mvector2.c
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/mvector2.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/mvector2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/mvector2.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   531344 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/mvector2_int.c
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/mvector2_int.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/mvector2_int.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   757435 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2.c
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   685796 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2_int.c
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2_int.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2_int.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_c_extensions/vector2_int.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.761700 nalpy-0.3.3/nalpy/math/_legacy_vector2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_legacy_vector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_legacy_vector2/mvector2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_legacy_vector2/mvector2_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_legacy_vector2/vector2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_legacy_vector2/vector2_int.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.761700 nalpy-0.3.3/nalpy/math/_rect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_rect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_rect/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_rect/rect_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_rect/rect_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/math/_rect/rect_offset_int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-03 21:39:35.000000 nalpy-0.3.3/nalpy/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.749699 nalpy-0.3.3/nalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-03 21:39:48.000000 nalpy-0.3.3/nalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-03 21:39:48.000000 nalpy-0.3.3/nalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:39:48.000000 nalpy-0.3.3/nalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:39:48.000000 nalpy-0.3.3/nalpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 21:39:48.000000 nalpy-0.3.3/nalpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 21:39:35.000000 nalpy-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 21:39:35.000000 nalpy-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-03 21:39:35.000000 nalpy-0.3.3/script_compile_and_install.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:39:48.761700 nalpy-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-03 21:39:35.000000 nalpy-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:39:48.761700 nalpy-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 21:39:35.000000 nalpy-0.3.3/tests/float_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-03 21:39:35.000000 nalpy-0.3.3/tests/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-08-03 21:39:35.000000 nalpy-0.3.3/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-08-03 21:39:35.000000 nalpy-0.3.3/tests/test_vector2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-08-03 21:39:35.000000 nalpy-0.3.3/tests/test_vector2_int.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.848550 nalpy-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 22:13:04.000000 nalpy-0.3.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.832549 nalpy-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.832549 nalpy-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 22:13:04.000000 nalpy-0.3.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-08-03 22:13:04.000000 nalpy-0.3.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.832549 nalpy-0.3.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-03 22:13:04.000000 nalpy-0.3.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-03 22:13:16.848550 nalpy-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 22:13:04.000000 nalpy-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.836550 nalpy-0.3.4/nalpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.836550 nalpy-0.3.4/nalpy/console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/console_utils/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.836550 nalpy-0.3.4/nalpy/humanizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/bytes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.836550 nalpy-0.3.4/nalpy/humanizer/inflections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/inflections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/inflections/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.840550 nalpy-0.3.4/nalpy/humanizer/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/numbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/numbers/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/numbers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/numbers/heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/numbers/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/numbers/number_to_roman_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/numbers/number_to_words_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/humanizer/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.840550 nalpy-0.3.4/nalpy/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.844550 nalpy-0.3.4/nalpy/math/_c_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   355223 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/functions.c
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/functions.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/functions.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   538481 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/mvector2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/mvector2.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/mvector2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/mvector2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   531344 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/mvector2_int.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/mvector2_int.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/mvector2_int.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   757435 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   685796 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2_int.c
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2_int.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2_int.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_c_extensions/vector2_int.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.848550 nalpy-0.3.4/nalpy/math/_legacy_vector2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_legacy_vector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_legacy_vector2/mvector2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_legacy_vector2/mvector2_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_legacy_vector2/vector2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_legacy_vector2/vector2_int.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.848550 nalpy-0.3.4/nalpy/math/_rect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_rect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_rect/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_rect/rect_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_rect/rect_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/math/_rect/rect_offset_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-03 22:13:04.000000 nalpy-0.3.4/nalpy/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.836550 nalpy-0.3.4/nalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-03 22:13:16.000000 nalpy-0.3.4/nalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-03 22:13:16.000000 nalpy-0.3.4/nalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:13:16.000000 nalpy-0.3.4/nalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:13:16.000000 nalpy-0.3.4/nalpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 22:13:16.000000 nalpy-0.3.4/nalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 22:13:04.000000 nalpy-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 22:13:04.000000 nalpy-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-03 22:13:04.000000 nalpy-0.3.4/script_compile_and_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 22:13:16.848550 nalpy-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-03 22:13:04.000000 nalpy-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:13:16.848550 nalpy-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 22:13:04.000000 nalpy-0.3.4/tests/float_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-03 22:13:04.000000 nalpy-0.3.4/tests/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-08-03 22:13:04.000000 nalpy-0.3.4/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-08-03 22:13:04.000000 nalpy-0.3.4/tests/test_vector2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-08-03 22:13:04.000000 nalpy-0.3.4/tests/test_vector2_int.py
```

### Comparing `nalpy-0.3.3/.github/workflows/pypi-publish.yml` & `nalpy-0.3.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/.gitignore` & `nalpy-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/console_utils/__init__.py` & `nalpy-0.3.4/nalpy/console_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/console_utils/_helpers.py` & `nalpy-0.3.4/nalpy/console_utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/console_utils/commands.py` & `nalpy-0.3.4/nalpy/console_utils/commands.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/console_utils/cursor.py` & `nalpy-0.3.4/nalpy/console_utils/cursor.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/console_utils/progressbar.py` & `nalpy-0.3.4/nalpy/console_utils/progressbar.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,12 +50,14 @@
         print(message, self._style.bar_prefix, sep="", end="")
         if self._style.color is not None:
             _console_utils.set_foreground_color(self._style.color)
         print(bar, end="")
         _console_utils.reset_attributes()
         print(empty, self._style.bar_suffix, suffix, sep="", end="")
 
-    def stop(self) -> None:
+    def stop(self, *, end: str | None = "\n") -> None:
         """Resets the cursor visibility if it was modified."""
         if self._cursor_hidden:
             _console_utils.cursor_show()
             self._cursor_hidden = False
+
+        print(end=end)
```

### Comparing `nalpy-0.3.3/nalpy/console_utils/spinner.py` & `nalpy-0.3.4/nalpy/console_utils/spinner.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/console_utils/styling.py` & `nalpy-0.3.4/nalpy/console_utils/styling.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/events.py` & `nalpy-0.3.4/nalpy/events.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/inflections/__init__.py` & `nalpy-0.3.4/nalpy/humanizer/inflections/__init__.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/inflections/vocabulary.py` & `nalpy-0.3.4/nalpy/humanizer/inflections/vocabulary.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/iterable.py` & `nalpy-0.3.4/nalpy/humanizer/iterable.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/numbers/__init__.py` & `nalpy-0.3.4/nalpy/humanizer/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/numbers/count.py` & `nalpy-0.3.4/nalpy/humanizer/numbers/count.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/numbers/heading.py` & `nalpy-0.3.4/nalpy/humanizer/numbers/heading.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/numbers/metric.py` & `nalpy-0.3.4/nalpy/humanizer/numbers/metric.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/numbers/number_to_words_converter.py` & `nalpy-0.3.4/nalpy/humanizer/numbers/number_to_words_converter.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/string.py` & `nalpy-0.3.4/nalpy/humanizer/string.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/humanizer/time.py` & `nalpy-0.3.4/nalpy/humanizer/time.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/__init__.py` & `nalpy-0.3.4/nalpy/math/__init__.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/functions.c` & `nalpy-0.3.4/nalpy/math/_c_extensions/functions.c`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/functions.pyi` & `nalpy-0.3.4/nalpy/math/_c_extensions/functions.pyi`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/functions.pyx` & `nalpy-0.3.4/nalpy/math/_c_extensions/functions.pyx`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/mvector2.c` & `nalpy-0.3.4/nalpy/math/_c_extensions/mvector2.c`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/mvector2.pyi` & `nalpy-0.3.4/nalpy/math/_c_extensions/mvector2.pyi`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/mvector2.pyx` & `nalpy-0.3.4/nalpy/math/_c_extensions/mvector2.pyx`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/mvector2_int.c` & `nalpy-0.3.4/nalpy/math/_c_extensions/mvector2_int.c`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/mvector2_int.pyi` & `nalpy-0.3.4/nalpy/math/_c_extensions/mvector2_int.pyi`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/mvector2_int.pyx` & `nalpy-0.3.4/nalpy/math/_c_extensions/mvector2_int.pyx`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/vector2.c` & `nalpy-0.3.4/nalpy/math/_c_extensions/vector2.c`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/vector2.pyi` & `nalpy-0.3.4/nalpy/math/_c_extensions/vector2.pyi`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/vector2.pyx` & `nalpy-0.3.4/nalpy/math/_c_extensions/vector2.pyx`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/vector2_int.c` & `nalpy-0.3.4/nalpy/math/_c_extensions/vector2_int.c`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/vector2_int.pyi` & `nalpy-0.3.4/nalpy/math/_c_extensions/vector2_int.pyi`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_c_extensions/vector2_int.pyx` & `nalpy-0.3.4/nalpy/math/_c_extensions/vector2_int.pyx`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_legacy_vector2/mvector2.py` & `nalpy-0.3.4/nalpy/math/_legacy_vector2/mvector2.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_legacy_vector2/mvector2_int.py` & `nalpy-0.3.4/nalpy/math/_legacy_vector2/mvector2_int.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_legacy_vector2/vector2.py` & `nalpy-0.3.4/nalpy/math/_legacy_vector2/vector2.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_legacy_vector2/vector2_int.py` & `nalpy-0.3.4/nalpy/math/_legacy_vector2/vector2_int.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_rect/rect.py` & `nalpy-0.3.4/nalpy/math/_rect/rect.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_rect/rect_int.py` & `nalpy-0.3.4/nalpy/math/_rect/rect_int.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_rect/rect_offset.py` & `nalpy-0.3.4/nalpy/math/_rect/rect_offset.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy/math/_rect/rect_offset_int.py` & `nalpy-0.3.4/nalpy/math/_rect/rect_offset_int.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/nalpy.egg-info/SOURCES.txt` & `nalpy-0.3.4/nalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/script_compile_and_install.py` & `nalpy-0.3.4/script_compile_and_install.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/setup.py` & `nalpy-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/tests/performance.py` & `nalpy-0.3.4/tests/performance.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/tests/test_math.py` & `nalpy-0.3.4/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/tests/test_vector2.py` & `nalpy-0.3.4/tests/test_vector2.py`

 * *Files identical despite different names*

### Comparing `nalpy-0.3.3/tests/test_vector2_int.py` & `nalpy-0.3.4/tests/test_vector2_int.py`

 * *Files identical despite different names*

