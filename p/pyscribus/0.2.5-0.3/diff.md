# Comparing `tmp/pyscribus-0.2.5.tar.gz` & `tmp/pyscribus-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscribus-0.2.5.tar", last modified: Sat Jul 22 20:09:30 2023, max compression
+gzip compressed data, was "pyscribus-0.3.tar", last modified: Fri Aug  4 16:51:24 2023, max compression
```

## Comparing `pyscribus-0.2.5.tar` & `pyscribus-0.3.tar`

### file list

```diff
@@ -1,50 +1,61 @@
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.166119 pyscribus-0.2.5/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    34494 2023-03-11 18:49:33.000000 pyscribus-0.2.5/LICENSE
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1519 2023-07-22 20:09:30.166119 pyscribus-0.2.5/PKG-INFO
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.158119 pyscribus-0.2.5/pyscribus/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      949 2023-07-22 20:02:37.000000 pyscribus-0.2.5/pyscribus/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20868 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/colors.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/common/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      930 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/common/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2632 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/common/math.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    13845 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/common/xml.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35340 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/dimensions.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    61630 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/document.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3648 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/exceptions.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/extra/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      971 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/extra/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    14384 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/extra/wireframe.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/headless/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3506 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/headless/__init__.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/headless/scripts/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/headless/scripts/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1192 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/headless/scripts/topdf.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5178 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/itemattribute.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5591 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/layers.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1715 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/logs.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    10991 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/marks.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8644 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/notes.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)   108431 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/pageobjects.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35269 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/pages.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/papers/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      942 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3783 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/afnor.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2216 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/ansi.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3259 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/iso216.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1738 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/iso217.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2347 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/iso269.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1615 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/newspaper.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5605 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/patterns.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    24054 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/printing.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     9877 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/sla.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    45306 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/stories.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    59441 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/styles.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     7565 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/toc.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus.egg-info/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1519 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/PKG-INFO
--rw-rw-r--   0 etienne   (1000) etienne   (1000)      990 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/SOURCES.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/dependency_links.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       14 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/requires.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       10 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/top_level.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       38 2023-07-22 20:09:30.166119 pyscribus-0.2.5/setup.cfg
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1292 2023-07-22 20:02:37.000000 pyscribus-0.2.5/setup.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.506249 pyscribus-0.3/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    34494 2023-03-11 18:49:33.000000 pyscribus-0.3/LICENSE
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1517 2023-08-04 16:51:24.506249 pyscribus-0.3/PKG-INFO
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.498249 pyscribus-0.3/pyscribus/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      916 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.498249 pyscribus-0.3/pyscribus/file/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    13484 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/file/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3527 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/file/colors.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    10602 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/file/document.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2479 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/file/exceptions.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8368 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/file/hyphenation.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20239 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/file/pageobjects.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    11465 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/file/stories.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20151 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/file/ui.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.502249 pyscribus-0.3/pyscribus/model/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      949 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20899 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/colors.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.502249 pyscribus-0.3/pyscribus/model/common/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      930 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/common/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5006 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/common/math.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    13845 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/common/xml.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    36326 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/dimensions.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    81025 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/document.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3648 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/exceptions.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.502249 pyscribus-0.3/pyscribus/model/extra/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      971 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/extra/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    14402 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/extra/wireframe.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.502249 pyscribus-0.3/pyscribus/model/headless/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3512 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/headless/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.502249 pyscribus-0.3/pyscribus/model/headless/scripts/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/headless/scripts/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1198 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/headless/scripts/topdf.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5190 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/itemattribute.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5609 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/layers.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1715 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/logs.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    11003 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/marks.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8656 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/notes.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)   109481 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/pageobjects.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35509 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/pages.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.506249 pyscribus-0.3/pyscribus/model/papers/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      942 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/papers/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3789 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/papers/afnor.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2222 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/papers/ansi.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3265 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/papers/iso216.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1744 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/papers/iso217.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2353 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/papers/iso269.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1621 2023-08-04 15:48:35.000000 pyscribus-0.3/pyscribus/model/papers/newspaper.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5629 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/patterns.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    24084 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/printing.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     6133 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/sla.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    43865 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/stories.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    59870 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/styles.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     7577 2023-08-04 15:57:54.000000 pyscribus-0.3/pyscribus/model/toc.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 16:51:24.506249 pyscribus-0.3/pyscribus.egg-info/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1517 2023-08-04 16:51:24.000000 pyscribus-0.3/pyscribus.egg-info/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2754 2023-08-04 16:51:24.000000 pyscribus-0.3/pyscribus.egg-info/SOURCES.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-08-04 16:51:24.000000 pyscribus-0.3/pyscribus.egg-info/dependency_links.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       14 2023-08-04 16:51:24.000000 pyscribus-0.3/pyscribus.egg-info/requires.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       10 2023-08-04 16:51:24.000000 pyscribus-0.3/pyscribus.egg-info/top_level.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       38 2023-08-04 16:51:24.506249 pyscribus-0.3/setup.cfg
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2039 2023-08-04 16:50:39.000000 pyscribus-0.3/setup.py
```

### Comparing `pyscribus-0.2.5/LICENSE` & `pyscribus-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.5/PKG-INFO` & `pyscribus-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscribus
-Version: 0.2.5
+Version: 0.3
 Summary: Read, create and update Scribus .sla files.
 Author: Étienne Nadji
 Author-email: etnadji@eml.cc
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://etnadji.fr/pyscribus
 Project-URL: Source Code, https://framagit.org/etnadji/pyscribus
 Project-URL: Issue tracker, https://framagit.org/etnadji/pyscribus/-/issues
```

### Comparing `pyscribus-0.2.5/pyscribus/__init__.py` & `pyscribus-0.3/pyscribus/model/papers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """
-PyScribus
+PyScribus submodule for paper sizes
 """
 
-from pyscribus.sla import SLA
-
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
-__version__ = "0.2.5"
+__version__ = "0.1"
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-0.2.5/pyscribus/colors.py` & `pyscribus-0.3/pyscribus/model/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 from __future__ import annotations
 
 from typing import Union, NoReturn, Literal, List
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
-import pyscribus.common.math as pmath
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.common.math as pmath
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 ColorSpace = Literal["cmyk", "rgb"]
 
@@ -121,14 +121,15 @@
 
         self.set_space_colors(space, colors)
 
         self._quick_setup(kwargs)
 
     # Color management -----------------------------------------
 
+    @property
     def space(self):
         try:
             return {True: "cmyk", False: "rgb"}[self.is_cmyk]
         except KeyError:
             return None
 
     def set_space_colors(
@@ -153,15 +154,15 @@
            color.set_space_colors("cmyk", [0, 0, 0, 0])
 
         """
 
         spaced = self.set_space(space)
 
         if spaced:
-            self.set_colors(colors, self.space())
+            self.set_colors(colors, self.space)
 
     def set_colors(
         self, colors: List[float], space: Union[ColorSpace, bool]
     ) -> bool:
         """
         :type colors: list
         :param colors: List of inks values (float).
@@ -247,14 +248,15 @@
            # with fromdefault method :
            black = Color()
            black.fromdefault("Black")
 
            # with quick setup :
            blue = Color(default="Blue")
 
+
         .. seealso::
             **For fromdefault explanation**:
             `pyscribus.common.xml.PyScribusElement.fromdefault`
 
             **For current class default sets**:
             `pyscribus.colors.Color.listdefaults`
 
@@ -310,15 +312,15 @@
                 raise exceptions.InvalidColor("No inks.")
 
             if None in colors:
                 raise exceptions.InvalidColor(
                     "Invalid inks <{}>.".format(",".join(colors))
                 )
 
-            self.set_colors(colors, self.space())
+            self.set_colors(colors, self.space)
 
         # Register ---------------------------------------------------
 
         if (reg := xml.get("Register")) is None:
             self.register = False
         else:
             if int(reg):
@@ -387,23 +389,23 @@
 
                 if setting_name == "rgb":
                     if len(setting_value) < 3:
                         while len(setting_value) < 3:
                             setting_value.append(float(0))
 
                     setting_value = setting_value[:3]
-                    self.set_colors(setting_value, self.space())
+                    self.set_colors(setting_value, self.space)
 
                 if setting_name == "cmyk":
                     if len(setting_value) < 4:
                         while len(setting_value) < 4:
                             setting_value.append(float(0))
 
                     setting_value = setting_value[:4]
-                    self.set_colors(setting_value, self.space())
+                    self.set_colors(setting_value, self.space)
 
     def same_space(self, other: Color) -> bool:
         """
         Is that color and other color share the same color space ?
 
         :param other: Color instance to compare.
         :type other: pyscribus.colors.Color
```

### Comparing `pyscribus-0.2.5/pyscribus/common/__init__.py` & `pyscribus-0.3/pyscribus/model/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.5/pyscribus/common/xml.py` & `pyscribus-0.3/pyscribus/model/common/xml.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.5/pyscribus/dimensions.py` & `pyscribus-0.3/pyscribus/model/dimensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 from __future__ import annotations
 
 import copy
 import math
 
 from typing import Union, Literal
 
-from pyscribus.common.math import PICA_TO_MM
+from pyscribus.model.common.math import PICA_TO_MM
 
-import pyscribus.logs as logs
-import pyscribus.exceptions as exceptions
+import pyscribus.model.logs as logs
+import pyscribus.model.exceptions as exceptions
 
-import pyscribus.papers.ansi as ansipaper
-import pyscribus.papers.iso216 as iso216paper
+import pyscribus.model.papers.ansi as ansipaper
+import pyscribus.model.papers.iso216 as iso216paper
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 XY = Literal["x", "y"]
 DimValue = Union[float, int]
@@ -109,20 +109,35 @@
         "mm": ["mm"],
         "pica": ["pica", "pct"],
         "pt": ["pt"],
         "perc": ["perc", "pc"],
         "pcdecim": ["pcdecim", "pcd"],
         "pcscale": ["pcscale"],
         "cdeg": ["cdeg"],
+        "pdeg": ["pdeg"],
         "deg": ["deg"],
         "dpi": ["dpi", "ppp", "ppi"],
         "lpi": ["lpi"],
         "sec": ["s", "sec"],
     }
 
+    # Units that can be converted into picas at export.
+    NOT_TO_PICAS = [
+        "perc",
+        "pcdecim",
+        "pcscale",
+        "cdeg",
+        "pdeg",
+        "deg",
+        "lpi",
+        "dpi",
+        "pt",
+        "sec",
+    ]
+
     def __init__(self, value: DimValue, **kwargs: dict):
         self.value = value
         self.integer = False
         self.allow_negative = False
 
         if "integer" in kwargs:
             self.integer = bool(kwargs["integer"])
@@ -182,14 +197,27 @@
 
         if self.unit == "sec":
             if int(float(self.value)) != float(self.value):
                 raise exceptions.InvalidDim(
                     "Second Dim must be an integer, is {}".format(self.value)
                 )
 
+        if self.unit == "pdeg":
+            if self.value >= -180:
+                if self.value <= 180:
+                    return True
+
+                raise exceptions.InvalidDim(
+                    "Polygon tool rotation angle must range from -180 to 180"
+                )
+
+            raise exceptions.InvalidDim(
+                "Polygon tool rotation angle must range from -180 to 180"
+            )
+
         if self.unit == "cdeg":
 
             if self.value >= 0:
                 if self.value <= 180:
                     return True
 
                 raise exceptions.InvalidDim(
@@ -237,14 +265,16 @@
         | also negative)           |               |
         +--------------------------+---------------+
         | Percentage (decimal, can | pcscale       |
         | be more than 1.0)        |               |
         +--------------------------+---------------+
         | Calligraphic pen degree  | cdeg          |
         +--------------------------+---------------+
+        | Polygon tool degree      | pdeg          |
+        +--------------------------+---------------+
         | Regular degree           | deg           |
         +--------------------------+---------------+
         | Dot per inch (DPI/PPP)   | dpi, ppp, ppi |
         +--------------------------+---------------+
         | Line per inch (LPI)      | lpi           |
         +--------------------------+---------------+
         | Second                   | s, sec        |
@@ -276,46 +306,45 @@
         :type no_useless_decimals: boolean
         :param no_useless_decimals: Returns integer instead of float if
             decimals are 0. So 1.0 -> 1 ; 1.1 -> 1.1.
         :rtype: str
         :return: str
         """
 
+        # Function to remove useless decimals ----------------------------
+
         def decimals(number):
             if float(number) == int(number):
                 return int(number)
 
             return number
 
-        if self.unit not in [
-            "perc",
-            "pcdecim",
-            "pcscale",
-            "cdeg",
-            "deg",
-            "lpi",
-            "dpi",
-            "pt",
-        ]:
+        # The value must be converted into picas points ------------------
+
+        if self.unit not in Dim.NOT_TO_PICAS:
             if no_useless_decimals:
                 pica = self.topica()
 
                 return str(decimals(pica))
 
             return str(self.topica())
 
+        # Percentage as a decimal export ---------------------------------
+
         if self.unit == "pcdecim":
             if self.value == 1.0:
                 return "1"
 
             if no_useless_decimals:
                 return str(decimals(self.value))
 
             return str(self.value)
 
+        # Other units ----------------------------------------------------
+
         if no_useless_decimals:
             return str(decimals(self.value))
 
         return str(self.value)
 
     def toxml(self) -> str:
         """
@@ -365,15 +394,15 @@
         """
         :rtype: boolean
         :return: If the Dim instance is a convertable length
         """
 
         return not (
             self.unit
-            in ["perc", "pcdecim", "pcscale", "cdeg", "deg", "dpi", "lpi"]
+            in ["perc", "pcdecim", "pcscale", "cdeg", "pdeg", "deg", "dpi", "lpi"]
         )
 
     def topica(
         self, ceil: bool = False, obj: bool = False
     ) -> Union[float, int, Dim]:
         """
         Returns the value of Dim in pica point unit.
@@ -517,15 +546,15 @@
 
         if self.unit in Dim.UNIT_ARGS.keys():
             short = {"mm": "mm", "perc": "%", "pica": "pct", "lpi": "lpi"}
 
             if self.unit in short:
                 u = short[self.unit]
 
-            if self.unit in ["cdeg", "deg"]:
+            if self.unit in ["cdeg", "deg", "pdeg"]:
                 u = "°"
 
         else:
             raise exceptions.UnknownDimUnit(self.unit)
 
         return f"{r} {u}"
```

### Comparing `pyscribus-0.2.5/pyscribus/document.py` & `pyscribus-0.3/pyscribus/model/document.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,34 +23,35 @@
 
 # Imports ===============================================================#
 
 # To avoid Sphinx complaints from methods annotations referencing same class
 from __future__ import annotations
 
 from typing import Union, NoReturn, Optional, Any, List
+from collections import OrderedDict
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
+import pyscribus.model.exceptions as exceptions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
-import pyscribus.dimensions as dimensions
-import pyscribus.colors as pscolors
-import pyscribus.toc as toc
-import pyscribus.marks as marks
-import pyscribus.pages as pages
-import pyscribus.styles as styles
-import pyscribus.itemattribute as itemattribute
-import pyscribus.patterns as patterns
-import pyscribus.layers as layers
-import pyscribus.pageobjects as pageobjects
-import pyscribus.notes as notes
-import pyscribus.printing as printing
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.colors as pscolors
+import pyscribus.model.toc as toc
+import pyscribus.model.marks as marks
+import pyscribus.model.pages as pages
+import pyscribus.model.styles as styles
+import pyscribus.model.itemattribute as itemattribute
+import pyscribus.model.patterns as patterns
+import pyscribus.model.layers as layers
+import pyscribus.model.pageobjects as pageobjects
+import pyscribus.model.notes as notes
+import pyscribus.model.printing as printing
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 BoolOrElement = Union[bool, ET.Element]
 
@@ -69,90 +70,135 @@
     """
     SLA Document (DOCUMENT) in SLA file.
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     """
 
-    metadata_xml = {
-        "AUTHOR": "author",
-        "COMMENTS": "comments",
-        "PUBLISHER": "publisher",
-        "DOCDATE": "date",
-        "DOCTYPE": "type",
-        "DOCFORMAT": "format",
-        "DOCIDENT": "identifier",
-        "DOCSOURCE": "source",
-        "DOCLANGINFO": "lang",
-        "DOCRELATION": "related",
-        "DOCCOVER": "cover",
-        "DOCRIGHTS": "rights",
-        "TITLE": "title",
-        "SUBJECT": "subject",
-        "DOCCONTRIB": "contributor",
+    metadata_xml = OrderedDict(
+        AUTHOR="author",
+        COMMENTS="comments",
+        KEYWORDS="keywords",
+        PUBLISHER="publisher",
+        DOCDATE="date",
+        DOCTYPE="type",
+        DOCFORMAT="format",
+        DOCIDENT="identifier",
+        DOCSOURCE="source",
+        DOCLANGINFO="lang",
+        DOCRELATION="related",
+        DOCCOVER="cover",
+        DOCRIGHTS="rights",
+        DOCCONTRIB="contributor",
+        TITLE="title",
+        SUBJECT="subject",
+    )
+
+    ui_show_xml = OrderedDict(
+        SHOWGRID="grid",
+        SHOWGUIDES="guides",
+        showcolborders="colborders",
+        SHOWFRAME="frames",
+        SHOWControl="caracters",
+        SHOWLAYERM="layer_hints",
+        SHOWMARGIN="margins",
+        SHOWBASE="baseline",
+        SHOWPICT="images",
+        SHOWLINK="links",
+        # rulerMode
+        showrulers="rulers",
+        showBleed="bleeds",
+    )
+
+    icc_xml = OrderedDict(
+        DPPr="printer",
+        DPIn="rgb_images",
+        DPInCMYK="cmyk_images",
+        DPIn2="rgb_colors",
+        DPIn3="cmyk_colors",
+    )
+
+    autoframes_xml = OrderedDict(
+        AUTOSPALTEN="columns",
+        ABSTSPALTEN="colgap",
+    )
+
+    bleed_xml = OrderedDict(
+        BleedTop="top",
+        BleedLeft="left",
+        BleedRight="right",
+        BleedBottom="bottom",
+    )
+
+    scratchspace_xml = OrderedDict(
+        ScratchBottom="bottom",
+        ScratchLeft="left",
+        ScratchRight="right",
+        ScratchTop="top",
+        GapHorizontal="horizontal_gap",
+        GapVertical="vertical_gap",
+    )
+
+    units_xml = {
+        "0": "points",
+        "1": "millimeters",
+        "2": "inches",
+        "3": "picas",
+        "4": "centimeters",
+        "5": "ciceros",
     }
 
-    ui_show_xml = {
-        "SHOWMARGIN": "margins",
-        "SHOWBASE": "baseline",
-        "SHOWPICT": "images",
-        "SHOWLINK": "links",
-        "SHOWGRID": "grid",
-        "SHOWGUIDES": "guides",
-        "showcolborders": "colborders",
-        "showrulers": "rulers",
-    }
-
-    autoframes_xml = {
-        "AUTOSPALTEN": "columns",
-        "ABSTSPALTEN": "colgap",
-    }
-
-    bleed_xml = {
-        "BleedTop": "top",
-        "BleedRight": "right",
-        "BleedLeft": "left",
-        "BleedBottom": "bottom",
+    ui_stack = {
+        "0": "objects",
+        "1": "guides",
+        "2": "grids",
+        "3": "baseline",
+        "4": "margins",
     }
 
     def __init__(self, sla_parent=False):
         super().__init__()
 
         self.sla_parent = sla_parent
 
+        self.units = "points"
+
         # ----------------------------------------------
 
         self.profiles = []
         self.pdf_settings = []
         self.printer_settings = []
 
         # ----------------------------------------------
 
+        self.hyphenation = None
+
+        # ----------------------------------------------
+
         self.colors = []
         self.layers = []
         self.patterns = []
         self.gradients = []
 
         # ----------------------------------------------
 
         self.pages = []
         self.page_sets = []
+        self.page_number = 0
         self.master_pages = []
         self.page_objects = []
 
         # ----------------------------------------------
 
         self.tocs = []
         self.marks = []
         self.sections = []
 
         # ----------------------------------------------
 
-        self.page_number = 0
-
         # Page dimensions, borders, bleeds
 
         self.dims = {
             "width": dimensions.Dim(595.275590551181),
             "height": dimensions.Dim(841.889763779528),
         }
 
@@ -166,14 +212,45 @@
         self.bleed = {
             "top": dimensions.Dim(0),
             "right": dimensions.Dim(0),
             "left": dimensions.Dim(0),
             "bottom": dimensions.Dim(0),
         }
 
+        self.scratchspace = {
+            # Space at the top of the scratch space, before the pages
+            "top": dimensions.Dim(20),
+            # Space at the right of the scratch space
+            "right": dimensions.Dim(100),
+            # Space at the left of the scratch space
+            "left": dimensions.Dim(100),
+            # Space at the bottom of the scratch space, after the last page
+            "bottom": dimensions.Dim(20),
+            # Horizontal gap between two pages
+            "horizontal_gap": dimensions.Dim(0),
+            # Vertical gap between two pages
+            "vertical_gap": dimensions.Dim(40),
+        }
+
+        self.grids = {
+            "minor": {
+                "spacing": dimensions.Dim(20),
+                "color": "#00ff00",
+            },
+            "major": {
+                "spacing": dimensions.Dim(100),
+                "color": "#00ff00",
+            },
+            "baseline": {
+                "spacing": dimensions.Dim(14.4, unit="pt"),
+                "offset": dimensions.Dim(0, unit="pt"),
+                "color": "#c0c0c0",
+            },
+        }
+
         # ----------------------------------------------
 
         self.notes = []
         self.notes_frames = []
 
         self.styles = {
             "note": [],
@@ -189,15 +266,15 @@
 
         # ----------------------------------------------
 
         self.metadata = {
             "title": "",
             "author": "",
             "subject": "",
-            "keywords": [],
+            "keywords": None,
             "comments": "",
             "publisher": "",
             "contributor": "",
             "date": "",
             "type": "",
             "format": "",
             "identifier": "",
@@ -216,53 +293,112 @@
             "rgb_colors": "",
             "cmyk_colors": "",
             "printer": "",
         }
 
         # ----------------------------------------------
 
-        self.ui_snapping = {"guides": False, "grid": False, "element": False}
+        self.ui_snapping = OrderedDict(
+            guides=False,
+            grid=False,
+            element=False,
+        )
 
         # ----------------------------------------------
 
         self.ui_show = {
-            "margins": True,
             "baseline": False,
-            "images": True,
-            "links": False,
+            "bleeds": True,
+            "caracters": False,
+            "colborders": True,
             "grid": False,
             "guides": True,
-            "colborders": True,
+            "images": True,
+            "layer_hints": False,
+            "links": False,
+            "margins": True,
             "rulers": True,
-        }
-
-        # ----------------------------------------------
-
-        self.calligraphicpen = {
-            "angle": dimensions.Dim(0, unit="cdeg", integer=True),
-            "line_width": dimensions.Dim(0, unit="pica"),
-            "line_shade": dimensions.Dim(100, unit="perc", integer=True),
-            "line_color": "",
-            "width": dimensions.Dim(0, unit="pica"),
-            "style": "1",
-            "fill_color": "",
-            "fill_shade": dimensions.Dim(100, unit="perc", is_int=True),
+            "stack": [
+                # Default is 2 0 4 1 3
+                "grids",
+                "objects",
+                "margins",
+                "guides",
+                "baseline",
+            ]
         }
 
         # ----------------------------------------------
 
         self.autoframes = {
             # Number of Columns in automatic Textframes
             # AUTOSPALTEN = "1"
             "columns": 1,
             # Distance between Columns in automatic Textframes
             # ABSTSPALTEN = "11"
             "colgap": dimensions.Dim(11, unit="pt"),
         }
 
+        # Default settings for tools -------------------
+
+        self.tools = {
+            "text": {
+                "font": None,
+                "size": dimensions.Dim(12, unit="pt"),
+                "columns": 1,
+                "columns_gap": dimensions.Dim(0),
+            },
+            "shape": {
+                "pen": {
+                    "color": "Black",
+                    "shade": dimensions.Dim(100, unit="perc", is_int=True)
+                },
+                "brush": {
+                    "color": "None",
+                    "shade": dimensions.Dim(100, unit="perc", is_int=True)
+                },
+                "style": 1,
+                "width": dimensions.Dim(1, unit="pica"),
+            },
+            "polygon": {
+                "sides": 4,
+                "rotation": dimensions.Dim(0, unit="pdeg", integer=True),
+                # Convex/Concave polygon
+                "convconc": {
+                    "active": False,
+                    # POLYF = intensity. Unknown numeric type:
+                    # Value             GUI
+                    # 0                 -100
+                    # 0.923879532511287 0
+                    # 1.08239220029239  100
+                    "intensity": float(0),
+                    "curb_in": dimensions.Dim(0, unit="pcdecim"),
+                    "curb_out": dimensions.Dim(0, unit="pcdecim"),
+                    "rot_in": dimensions.Dim(0, unit="pdeg", integer=True),
+                }
+            },
+            "line": {
+                "arrows": {"start": 0, "end": 0},
+                "color": "Black",
+                "style": 1,
+                "width": dimensions.Dim(1, unit="pica"),
+                "shade": dimensions.Dim(100, unit="perc", is_int=True)
+            },
+            "calligraphicpen": {
+                "angle": dimensions.Dim(0, unit="cdeg", integer=True),
+                "line_width": dimensions.Dim(0, unit="pica"),
+                "line_shade": dimensions.Dim(100, unit="perc", integer=True),
+                "line_color": "",
+                "width": dimensions.Dim(0, unit="pica"),
+                "style": 1,
+                "fill_color": "",
+                "fill_shade": dimensions.Dim(100, unit="perc", is_int=True),
+            }
+        }
+
         # ----------------------------------------------
 
         # FIXME Not documented -------------------------
         # PRESET="0"
 
         # FIXME ---- À faire ---------------------------
 
@@ -281,28 +417,14 @@
             # TODO : Link this value to pages sets in Document object
             "set": 0,
         }
 
         # (optional) First page number in the Doc
         FIRSTNUM = "1"
 
-        # (optional) Measurement unit for the Doc
-        # 0 = Points 1 = Millimeters 2 = Inches 3 = Picas
-        UNITS = "1"
-
-        # Default Font
-        DFONT = "Arial Regular"
-        # Default Fontsize
-        DSIZE = "12"
-
-        # (optional) Number of Columns in Textframes
-        DCOL = "1"
-        # (optional) Default Gap between Columns in Textframes
-        DGAP = "0"
-
         # FIXME Not documented -------------------------
         # TabFill=""
 
         # Default width for tabs in text frames
         TabWidth = "36"
 
         # FIXME Not documented -------------------------
@@ -320,19 +442,14 @@
         # Percentage for Subscript
         VTIEF = "33"
         # Percentage for scaling of the Glyphs in Subscript
         VTIEFSC = "66"
         # Percentage for scaling of the Glyphs in Small Caps
         VKAPIT = "75"
 
-        # (optional) Width of the Baseline Grid
-        BASEGRID = "14.4"
-        # (optional) Startoffset for the Baseline Grid
-        BASEO = "0"
-
         # FIXME Not documented -------------------------
         # AUTOL="100"
         # UnderlinePos="-1"
         # UnderlineWidth="-1"
         # StrikeThruPos="-1"
         # StrikeThruWidth="-1"
 
@@ -367,111 +484,64 @@
         # (optional) Automatic Hyphenation during typing 0 = off, 1 = on
         AUTOCHECK = "0"
         # (optional) Guides locked 0 = off, 1 = on
         GUIDELOCK = "0"
 
         # FIXME ---- À faire ---------------------------
 
-        # (optional) Distance of the minor Gridlines
-        MINGRID = "20"
-        # (optional) Distance of the major Gridlines
-        MAJGRID = "100"
-
-        # FIXME Not documented -------------------------
-        # SHOWFRAME="1"
-        # SHOWControl="0"
-        # SHOWLAYERM="0"
-
-        # FIXME ---- À faire ---------------------------
-
         # FIXME Not documented -------------------------
         # rulerMode="1"
 
         # FIXME Not documented -------------------------
-        # showBleed="1"
         # rulerXoffset="0"
         # rulerYoffset="0"
         # GuideRad="10"
         # GRAB="4"
-        # POLYC="4"
-        # POLYF="0.5"
-        # POLYR="0"
-        # POLYIR="0"
-        # POLYCUR="0"
-        # POLYOCUR="0"
-        # POLYS="0"
         # arcStartAngle="30"
         # arcSweepAngle="300"
         # spiralStartAngle="0"
         # spiralEndAngle="1080"
         # spiralFactor="1.2"
         # AutoSave="1"
         # AutoSaveTime="600000" # milisec ?
         # AutoSaveCount="1"
         # AutoSaveKeep="0"
         # AUtoSaveInDocDir="1"
         # AutoSaveDir=""
 
-        # Space at the bottom of the scratch space, after the last page
-        ScratchBottom = "20"
-        # Space at the left of the scratch space
-        ScratchLeft = "100"
-        # Space at the right of the scratch space
-        ScratchRight = "100"
-        # Space at the top of the scratch space, before the pages
-        ScratchTop = "20"
-
         # FIXME Not documented -------------------------
-        # GapHorizontal="0"
-        # GapVertical="40"
-        # StartArrow="0"
-        # EndArrow="0"
-        # PEN="Black"
-        # BRUSH="None"
-        # PENLINE="Black"
         # PENTEXT="Black"
         # StrokeText="Black"
         # TextBackGround="None"
         # TextLineColor="None"
         # TextBackGroundShade="100"
         # TextLineShade="100"
         # TextPenShade="100"
         # TextStrokeShade="100"
-        # STIL="1"
-        # STILLINE="1"
-        # WIDTH="1"
-        # WIDTHLINE="1"
-        # PENSHADE="100"
-        # LINESHADE="100"
-        # BRUSHSHADE="100"
         # CPICT="None"
         # PICTSHADE="100"
         # CSPICT="None"
         # PICTSSHADE="100"
         # PICTSCX="1"
         # PICTSCY="1"
         # PSCALE="1"
         # PASPECT="1"
         # EmbeddedPath="0"
         # HalfRes="1"
         # dispX="10"
         # dispY="10"
         # constrain="15"
 
-        # MINORC="#00ff00"
-        # MAJORC="#00ff00"
         # GuideC="#000080"
-        # BaseC="#c0c0c0"
 
         # Scribus GUI Page background
         PAGEC = "#ffffff"
 
         # MARGC="#0000ff"
 
-        # renderStack="2 0 4 1 3"
         # GridType="0"
         # RANDF="0"
 
         # currentProfile="PDF 1.4"
 
         # ----------------------------------------------
 
@@ -550,30 +620,40 @@
 
     def _default_ui_show(self) -> NoReturn:
         """
         Set default UI view options.
         """
 
         self.ui_show = {
-            "margins": True,
             "baseline": False,
-            "images": True,
-            "links": False,
+            "bleeds": True,
+            "caracters": False,
+            "colborders": True,
             "grid": False,
             "guides": True,
-            "colborders": True,
+            "images": True,
+            "layer_hints": False,
+            "links": False,
+            "margins": True,
             "rulers": True,
+            "stack": [
+                "grids",
+                "objects",
+                "margins",
+                "guides",
+                "baseline",
+            ]
         }
 
     def _default_calligraphic_pen(self) -> NoReturn:
         """
         Set default calligraphic pen options.
         """
 
-        self.calligraphicpen = {
+        self.tools["calligraphicpen"] = {
             "angle": dimensions.Dim(0, unit="cdeg", integer=True),
             "line_width": dimensions.Dim(0, unit="pica"),
             "line_shade": dimensions.Dim(100, unit="perc", integer=True),
             "line_color": "",
             "width": dimensions.Dim(0, unit="pica"),
             "style": 1,
             "fill_color": "",
@@ -747,21 +827,166 @@
             features[f]()
 
     # =======================================================================
 
     def fromxml(self, xml: ET.Element) -> bool:
         # --- DOCUMENT attributes ----------------------------------------
 
-        # TODO DOCUMENT many attribs…
+        # Default settings for Scribus' tools -----------------------
+
+        # Text tool __________________________________
+
+        if (text_tool_font := xml.get("DFONT")) is not None:
+            self.tools["text"]["font"] = text_tool_font
+
+        if (text_tool_size := xml.get("DSIZE")) is not None:
+            self.tools["text"]["size"].value = float(text_tool_size)
+
+        if (text_tool_columns := xml.get("DCOL")) is not None:
+            self.tools["text"]["columns"] = int(text_tool_columns)
+
+        if (text_tool_colsgap := xml.get("DGAP")) is not None:
+            self.tools["text"]["columns_gap"].value = float(text_tool_colsgap)
+
+        # Shape tool _________________________________
+
+        if (shape_tool_style := xml.get("STIL")) is not None:
+            shape_tool_style = int(shape_tool_style)
+
+            # Shape tool line style range from 0 to 37
+            if shape_tool_style > 37 or shape_tool_style < 0:
+                shape_tool_style = 0
+
+            self.tools["shape"]["style"] = shape_tool_style
+
+        if (shape_tool_width := xml.get("WIDTH")) is not None:
+            self.tools["shape"]["width"].value = float(shape_tool_width)
+
+        if (shape_tool_pen_shade := xml.get("PENSHADE")) is not None:
+            self.tools["shape"]["pen"]["shade"].value = int(shape_tool_pen_shade)
+
+        if (shape_tool_brush_shade := xml.get("BRUSHSHADE")) is not None:
+            self.tools["shape"]["brush"]["shade"].value = int(shape_tool_brush_shade)
+
+        if (shape_tool_pen_color := xml.get("PEN")) is not None:
+            self.tools["shape"]["pen"]["color"] = shape_tool_pen_color
+
+        if (shape_tool_brush_color := xml.get("BRUSH")) is not None:
+            self.tools["shape"]["brush"]["color"] = shape_tool_brush_color
+
+        # Line tool __________________________________
+
+        for att_name, human in [["StartArrow", "start"], ["EndArrow", "end"]]:
+
+            if (att := xml.get(att_name)) is not None:
+                att = int(att)
+
+                # Arrows type for line tool range from 0 to 36
+                if att > 36 or att < 0:
+                    att = 0
+
+                self.tools["line"]["arrows"][human] = att
+
+        if (line_tool_width := xml.get("WIDTHLINE")) is not None:
+            self.tools["line"]["width"].value = float(line_tool_width)
+
+        if (line_tool_shade := xml.get("LINESHADE")) is not None:
+            self.tools["line"]["shade"].value = int(line_tool_shade)
+
+        if (line_tool_color := xml.get("PENLINE")) is not None:
+            self.tools["line"]["color"] = line_tool_color
+
+        if (line_tool_style := xml.get("STILLINE")) is not None:
+            line_tool_style = int(line_tool_style)
+
+            # Line tool line style range from 0 to 37
+            if line_tool_style > 37 or line_tool_style < 0:
+                line_tool_style = 0
+
+            self.tools["line"]["style"] = line_tool_style
+
+        # Poylgon tool _______________________________
+
+        if (poly_tool_convconc := xml.get("POLYS")) is not None:
+            self.tools["polygon"]["convconc"]["active"] = num_to_bool(
+                poly_tool_convconc
+            )
+
+        if (poly_tool_sides := xml.get("POLYC")) is not None:
+            self.tools["polygon"]["sides"] = int(poly_tool_sides)
+
+        if (poly_tool_rot := xml.get("POLYR")) is not None:
+            self.tools["polygon"]["rotation"].value = int(poly_tool_rot)
+
+        if (poly_tool_cc_intensity := xml.get("POLYF")) is not None:
+            self.tools["polygon"]["convconc"]["intensity"] = float(
+                poly_tool_cc_intensity
+            )
+
+        for att_name, human in [
+                ["POLYR", "rot_in"], ["POLYCUR", "curb_in"],
+                ["POLYOCUR", "curb_out"]]:
+            if (att := xml.get(att_name)) is not None:
+                if human == "rot_in":
+                    att = int(att)
+                else:
+                    att = float(att)
+
+                self.tools["polygon"]["convconc"][human].value = att
+
+        # Calligraphic pen tool ______________________
+
+        for att_base, key in [
+            ["Angle", "angle"],
+            ["LineColorShade", "line_shade"],
+            ["FillColorShade", "fill_shade"],
+        ]:
+            att_name = f"calligraphicPen{att_base}"
+
+            if (att := xml.get(att_name)) is not None:
+                self.tools["calligraphicpen"][key].value = int(att)
+
+        for att_base, key in [["LineWidth", "line_width"], ["Width", "width"]]:
+            att_name = f"calligraphicPen{att_base}"
+
+            if (att := xml.get(att_name)) is not None:
+                self.tools["calligraphicpen"][key].value = float(att)
+
+        for att_base, key in [
+            ["LineColor", "line_color"],
+            ["FillColor", "fill_color"],
+            ["PenStyle", "style"],
+        ]:
+
+            att_name = f"calligraphicPen{att_base}"
+
+            if (att := xml.get(att_name)) is not None:
+                if att_base == "PenStyle":
+                    self.tools["calligraphicpen"][key] = int(att)
+                else:
+                    self.tools["calligraphicpen"][key] = att
+
+        # Document units --------------------------------------------
+
+        if (doc_units := xml.get("UNITS")) is not None:
+            self.units = Document.units_xml[doc_units]
+
+        # Scratch space ---------------------------------------------
+
+        for att_name, human in Document.scratchspace_xml.items():
+            if (att := xml.get(att_name)) is not None:
+                self.scratchspace[human].value = float(att)
+
+        # Borders ---------------------------------------------------
 
         for border in ["LEFT", "RIGHT", "TOP", "BOTTM"]:
             if (border_side := xml.get(f"BORDER{border}")) is not None:
                 self.borders[border.lower()].value = float(border_side)
 
-        # Pages settings
+        # Pages settings --------------------------------------------
 
         if (pagenumber := xml.get("ANZPAGES")) is not None:
             self.page_number = int(pagenumber)
 
         if (att_value := xml.get("orientation")) is not None:
             if int(att_value):
                 self.doc_pages["orientation"] = pages.Orientation.LANDSCAPE
@@ -777,92 +1002,95 @@
         for page_dim in ["WIDTH", "HEIGHT"]:
             if (pgdim := xml.get(f"PAGE{page_dim}")) is not None:
                 self.dims[page_dim.lower()].value = float(pgdim)
 
         if (att_value := xml.get("BOOK")) is not None:
             self.doc_pages["set"] = int(att_value)
 
-        # Metadatas
+        # Metadatas -------------------------------------------------
 
         for att, key in Document.metadata_xml.items():
             if (meta_value := xml.get(att)) is not None:
-                self.metadata[key] = meta_value
 
-        if (keywords := xml.get("KEYWORDS")) is not None:
-            self.metadata["keywords"] = keywords.split("; ")
+                # Make keywords a list
+                if att == "KEYWORDS":
+                    self.metadata[key] = meta_value.split("; ")
+                    continue
+
+                self.metadata[key] = meta_value
 
-        # Auto text frames
+        # Auto text frames ------------------------------------------
 
         for att, human in Document.autoframes_xml.items():
             if (att_value := xml.get(att)) is not None:
                 if human == "colums":
                     self.autoframes[human] = int(att_value)
                 if human == "colgap":
                     self.autoframes[human].value = float(att_value)
 
-        # UI snapping
+        # UI snapping -----------------------------------------------
 
         for snap_thing in ["grid", "guides", "element"]:
             att_name = "SnapTo{}".format(snap_thing.capitalize())
 
             if (att := xml.get(att_name)) is not None:
                 self.ui_snapping[snap_thing] = num_to_bool(att)
 
-        # Bleed settings
+        # Bleed settings --------------------------------------------
 
         for att, human in Document.bleed_xml.items():
             if (att_value := xml.get(att)) is not None:
-                self.bleed[human] = float(att_value)
+                self.bleed[human].value = float(att_value)
 
-        # UI show
+        # Grid settings ---------------------------------------------
 
-        for att_name, ui_name in Document.ui_show_xml.items():
+        for grid_name, grid_setting, att_name in [
+                ["minor", "spacing", "MINGRID"],
+                ["major", "spacing", "MAJGRID"],
+                ["baseline", "offset", "BASEO"],
+                ["baseline", "spacing", "BASEGRID"],
+            ]:
             if (att := xml.get(att_name)) is not None:
-                self.ui_show[ui_name] = num_to_bool(att)
+                self.grids[grid_name][grid_setting].value = float(att)
 
-        # ICC color profiles
+        # UI show ---------------------------------------------------
 
-        for att_name, icc_key in [
-            ["DPIn", "rgb_images"],
-            ["DPInCMYK", "cmyk_images"],
-            ["DPIn2", "rgb_colors"],
-            ["DPIn3", "cmyk_colors"],
-            ["DPPr", "printer"],
-        ]:
+        for att_name, ui_name in Document.ui_show_xml.items():
             if (att := xml.get(att_name)) is not None:
-                self.icc_profiles[icc_key] = att
+                self.ui_show[ui_name] = num_to_bool(att)
 
-        # Calligraphic pen -----------------------------------------------
+        if (ui_show_stack := xml.get("renderStack")) is not None:
+            stack = ui_show_stack.split()
 
-        for att_base, key in [
-            ["Angle", "angle"],
-            ["LineColorShade", "line_shade"],
-            ["FillColorShade", "fill_shade"],
-        ]:
-            att_name = f"calligraphicPen{att_base}"
+            if len(stack) == 5:
+                self.ui_show["stack"] = []
 
-            if (att := xml.get(att_name)) is not None:
-                self.calligraphicpen[key].value = int(att)
+                for stack_element in stack:
+                    try:
+                        self.ui_show["stack"].append(
+                            Document.ui_stack[stack_element]
+                        )
+                    except KeyError:
+                        continue
 
-        for att_base, key in [["LineWidth", "line_width"], ["Width", "width"]]:
-            att_name = f"calligraphicPen{att_base}"
+        # UI grid colors --------------------------------------------
 
+        for grid_name, grid_setting, att_name in [
+                ["minor", "color", "MINORC"],
+                ["major", "color", "MAJORC"],
+                ["baseline", "color", "BaseC"],
+            ]:
             if (att := xml.get(att_name)) is not None:
-                self.calligraphicpen[key].value = float(att)
-
-        for att_base, key in [
-            ["LineColor", "line_color"],
-            ["FillColor", "fill_color"],
-            ["PenStyle", "style"],
-        ]:
+                self.grids[grid_name][grid_setting] = att
 
-            att_name = f"calligraphicPen{att_base}"
+        # ICC color profiles ----------------------------------------
 
+        for att_name, icc_key in Document.icc_xml.items():
             if (att := xml.get(att_name)) is not None:
-                self.calligraphicpen[key] = att
+                self.icc_profiles[icc_key] = att
 
         # --- DOCUMENT childs --------------------------------------------
 
         for child in xml:
 
             self.__fromxml_item(child, "CheckProfile", Profile, self.profiles)
 
@@ -872,15 +1100,17 @@
 
             self.__fromxml_item(child, "COLOR", pscolors.Color, self.colors)
 
             self.__fromxml_item(
                 child, "Pattern", patterns.Pattern, self.patterns
             )
 
-            # TODO FIXME hyphen
+            self.__fromxml_item(
+                child, "HYPHEN", Hyphenation, self.hyphenation
+            )
 
             self.__fromxml_item(
                 child, "STYLE", styles.ParagraphStyle, self.styles["paragraph"],
                 True
             )
 
             self.__fromxml_item(
@@ -994,15 +1224,15 @@
                 ptype = child.get("PTYPE")
 
                 if ptype is None:
                     continue
 
                 try:
                     p_object = pageobjects.new_from_type(
-                            ptype, self.sla_parent, self
+                        ptype, self.sla_parent, self
                     )
 
                     if (success := p_object.fromxml(child)):
                         self.page_objects.append(p_object)
 
                 except ValueError:
                     pass
@@ -1010,99 +1240,478 @@
         # ----------------------------------------------------------------
 
         return True
 
     def toxml(self, optional: bool = True) -> ET.Element:
         xml = ET.Element("DOCUMENT")
 
-        # === DOCUMENT attributes ========================================
-
-        # Pages settings -------------------------------------------------
+        # === DOCUMENT attributes : new order (WIP) ======================
 
+        # DONE: 001 — ANZPAGES
+        # DONE: 002 — PAGEWIDTH
+        # DONE: 003 — PAGEHEIGHT
         xml.attrib["ANZPAGES"] = str(self.page_number)
+        xml.attrib["PAGEWIDTH"] = self.dims["width"].toxmlstr()
+        xml.attrib["PAGEHEIGHT"] = self.dims["height"].toxmlstr()
+
+        # Borders --------------------------------------------------------
+        # DONE: 004 — BORDERLEFT
+        # DONE: 005 — BORDERRIGHT
+        # DONE: 006 — BORDERTOP
+        # DONE: 007 — BORDERBOTTOM
+
+        for border_side, border_value in self.borders.items():
+            att = "BORDER{}".format(border_side.upper())
+            xml.attrib[att] = border_value.toxmlstr()
+
+        # 008 — PRESET
+
+        # Bleed settings -------------------------------------------------
+
+        # DONE: 009 — BleedTop
+        # DONE: 010 — BleedLeft
+        # DONE: 011 — BleedRight
+        # DONE: 012 — BleedBottom
+
+        for att, human in Document.bleed_xml.items():
+            xml.attrib[att] = self.bleed[human].toxmlstr(True)
+
+        # ----------------------------------------------------------------
+
+        # DONE: 013 — ORIENTATION
 
         xml.attrib["ORIENTATION"] = str(int(self.doc_pages["orientation"]))
 
+        # DONE: 014 — PAGESIZE
+
         for att, human in pages.xml_size.items():
             if human == self.doc_pages["size"]:
                 xml.attrib["PAGESIZE"] = att
                 break
 
+        # 015 — FIRSTNUM
+
+        # DONE: 016 — BOOK
         xml.attrib["BOOK"] = str(self.doc_pages["set"])
 
         # Auto text frames -----------------------------------------------
 
+        # DONE: 017 — AUTOSPALTEN
+        # DONE: 018 — ABSTSPALTEN
+
         for att, human in Document.autoframes_xml.items():
 
             if human == "columns":
                 xml.attrib[att] = str(self.autoframes[human])
 
             if human == "colgap":
                 xml.attrib[att] = self.autoframes[human].toxmlstr(True)
 
-        # Bleed settings -------------------------------------------------
+        # Document units -------------------------------------------------
+        # DONE: 019 — UNITS
 
-        for att, human in Document.bleed_xml.items():
-            xml.attrib[att] = str(self.bleed[human])
+        # Optional if the units are points
+        if self.units != "points":
+            for code, human in Document.units_xml.items():
+                if self.units == human:
+                    xml.attrib["UNITS"] = code
+                    break
 
-        # Dimensions -----------------------------------------------------
+        # Default settings -----------------------------------------------
+        # DONE: 020 — DFONT
+        # DONE: 021 — DSIZE
+        # DONE: 022 — DCOL
+        # DONE: 023 — DGAP
 
-        xml.attrib["PAGEWIDTH"] = self.dims["width"].toxmlstr()
-        xml.attrib["PAGEHEIGHT"] = self.dims["height"].toxmlstr()
+        if self.tools["text"]["font"] is not None:
+            xml.attrib["DFONT"] = self.tools["text"]["font"]
 
-        # Borders --------------------------------------------------------
+        xml.attrib["DSIZE"] = self.tools["text"]["size"].toxmlstr(True)
 
-        for border_side, border_value in self.borders.items():
-            att = "BORDER{}".format(border_side.upper())
-            xml.attrib[att] = border_value.toxmlstr()
+        # NOTE Marked as optional but is not
+        xml.attrib["DCOL"] = str(self.tools["text"]["columns"])
+
+        xml.attrib["DGAP"] = self.tools["text"]["columns_gap"].toxmlstr()
+
+        # ----------------------------------------------------------------
+
+        # 024 — TabFill
+
+        # 025 — TabWidth
+
+        # 026 — TextDistLeft
+
+        # 027 — TextDistRight
+
+        # 028 — TextDistBottom
+
+        # 029 — TextDistTop
+
+        # 030 — FirstLineOffset
 
         # Metadatas ------------------------------------------------------
+        # DONE: 031 — AUTHOR
+        # DONE: 032 — COMMENTS
+        # DONE: 033 — KEYWORDS
+        # DONE: 034 — PUBLISHER
+        # DONE: 035 — DOCDATE
+        # DONE: 036 — DOCTYPE
+        # DONE: 037 — DOCFORMAT
+        # DONE: 038 — DOCIDENT
+        # DONE: 039 — DOCSOURCE
+        # DONE: 040 — DOCLANGINFO
+        # DONE: 041 — DOCRELATION
+        # DONE: 042 — DOCCOVER
+        # DONE: 043 — DOCRIGHTS
+        # DONE: 044 — DOCCONTRIB
+        # DONE: 045 — TITLE
+        # DONE: 046 — SUBJECT
+
+        for att, human in Document.metadata_xml.items():
+            if human == "keywords":
+                xml.attrib[att] = "; ".join(self.metadata[human])
+                continue
 
-        for att, key in Document.metadata_xml.items():
-            xml.attrib[att] = self.metadata[key]
+            xml.attrib[att] = self.metadata[human]
+
+        # ----------------------------------------------------------------
+
+        # 047 — VHOCH
+
+        # 048 — VHOCHSC
+
+        # 049 — VTIEF
+
+        # 050 — VTIEFSC
+
+        # 051 — VKAPIT
+
+        # UI grids (baseline grid) ---------------------------------------
+        # DONE: 052 — BASEGRID
+        # DONE: 053 — BASEO
+        xml.attrib["BASEGRID"] = self.grids["baseline"]["spacing"].toxmlstr(True)
+        xml.attrib["BASEO"] = self.grids["baseline"]["offset"].toxmlstr(True)
+
+        # ----------------------------------------------------------------
+
+        # 054 — AUTOL
+
+        # 055 — UnderlinePos
+
+        # 056 — UnderlineWidth
 
-        xml.attrib["KEYWORDS"] = "; ".join(self.metadata["keywords"])
+        # 057 — StrikeThruPos
+
+        # 058 — StrikeThruWidth
+
+        # 059 — GROUPC
+
+        # 060 — HCMS
+
+        # 061 — DPSo
+
+        # 062 — DPSFo
+
+        # 063 — DPuse
+
+        # 064 — DPgam
+
+        # 065 — DPbla
+
+        # ICC profiles ---------------------------------------------------
+        # DONE: 066 — DPPr
+        # DONE: 067 — DPIn
+        # DONE: 068 — DPInCMYK
+        # DONE: 069 — DPIn2
+        # DONE: 070 — DPIn3
+
+        for att, human in Document.icc_xml.items():
+            xml.attrib[att] = self.icc_profiles[human]
+
+        # ----------------------------------------------------------------
+
+        # 071 — DISc
+
+        # 072 — DIIm
+
+        # 073 — ALAYER
+
+        # 074 — LANGUAGE
+
+        # 075 — AUTOMATIC
+
+        # 076 — AUTOCHECK
+
+        # 077 — GUIDELOCK
 
         # UI snapping ----------------------------------------------------
+        # DONE: 078 — SnapToGuides
+        # DONE: 079 — SnapToGrid
+        # DONE: 080 — SnapToElement
 
         for att_base, snap_value in self.ui_snapping.items():
             att = "SnapTo{}".format(att_base.capitalize())
             xml.attrib[att] = bool_to_num(snap_value)
 
+        # UI grids -------------------------------------------------------
+        # DONE: 081 — MINGRID (minor grid)
+        # DONE: 082 — MAJGRID (major grid)
+        xml.attrib["MINGRID"] = self.grids["minor"]["spacing"].toxmlstr()
+        xml.attrib["MAJGRID"] = self.grids["major"]["spacing"].toxmlstr()
+
         # UI show --------------------------------------------------------
+        # DONE: 083 — SHOWGRID
+        # DONE: 084 — SHOWGUIDES
+        # DONE: 085 — showcolborders
+        # DONE: 086 — SHOWFRAME
+        # DONE: 087 — SHOWControl
+        # DONE: 088 — SHOWLAYERM
+        # DONE: 089 — SHOWMARGIN
+        # DONE: 090 — SHOWBASE
+        # DONE: 091 — SHOWPICT
+        # DONE: 092 — SHOWLINK
 
-        for att_name, ui_name in Document.ui_show_xml.items():
-            xml.attrib[att_name] = bool_to_num(self.ui_show[ui_name])
+        for att, human in Document.ui_show_xml.items():
+            if att == "showrulers":
+                break
 
-        # ICC profiles ---------------------------------------------------
+            xml.attrib[att] = bool_to_num(self.ui_show[human])
 
-        for key_out, key_in in [
-            ["DPIn", "rgb_images"],
-            ["DPInCMYK", "cmyk_images"],
-            ["DPIn2", "rgb_colors"],
-            ["DPIn3", "cmyk_colors"],
-            ["DPPr", "printer"],
-        ]:
-            xml.attrib[key_out] = self.icc_profiles[key_in]
+        # ----------------------------------------------------------------
+
+        # 093 — rulerMode
+
+        # DONE: 094 — showrulers
+        # DONE: 095 — showBleed
+
+        for att in ["showrulers", "showBleed"]:
+            for att_name, ui_name in Document.ui_show_xml.items():
+                if att_name != att:
+                    continue
+
+                xml.attrib[att_name] = bool_to_num(self.ui_show[ui_name])
+
+        # 096 — rulerXoffset
+
+        # 097 — rulerYoffset
+
+        # 098 — GuideRad
+
+        # 099 — GRAB
+
+        # Polygon tool -------------------------------------------
+
+        # DONE: DONE: 100 — POLYC
+        # DONE: 101 — POLYF — FIXME : Unknown float numeric type with Dim unit
+        # DONE: 102 — POLYR
+        # DONE: 103 — POLYIR
+        # DONE: 104 — POLYCUR
+        # DONE: 105 — POLYOCUR
+        # DONE: 106 — POLYS
+
+        xml.attrib["POLYC"] = str(self.tools["polygon"]["sides"])
+
+        convconc_intensity = self.tools["polygon"]["convconc"]["intensity"]
+
+        if float(convconc_intensity) == float(int(convconc_intensity)):
+            xml.attrib["POLYF"] = str(int(convconc_intensity))
+
+        xml.attrib["POLYF"] = str(convconc_intensity)
+
+        xml.attrib["POLYR"] = self.tools["polygon"]["rotation"].toxmlstr()
+
+        for att, hmn in [
+                ["POLYR", "rot_in"], ["POLYCUR", "curb_in"],
+                ["POLYOCUR", "curb_out"]]:
+            xml.attrib[att] = self.tools["polygon"]["convconc"][hmn].toxmlstr()
+
+        xml.attrib["POLYS"] = bool_to_num(
+            self.tools["polygon"]["convconc"]["active"]
+        )
+
+        # --------------------------------------------------------
+
+        # 107 — arcStartAngle
+
+        # 108 — arcSweepAngle
+
+        # 109 — spiralStartAngle
+
+        # 110 — spiralEndAngle
+
+        # 111 — spiralFactor
+
+        # 112 — AutoSave
+
+        # 113 — AutoSaveTime
+
+        # 114 — AutoSaveCount
+
+        # 115 — AutoSaveKeep
+
+        # 116 — AUtoSaveInDocDir
+
+        # 117 — AutoSaveDir
+
+        # Scratch space ------------------------------------------
+        # DONE: 118 — ScratchBottom
+        # DONE: 119 — ScratchLeft
+        # DONE: 120 — ScratchRight
+        # DONE: 121 — ScratchTop
+        # DONE: 122 — GapHorizontal
+        # DONE: 123 — GapVertical
+
+        for att, human in Document.scratchspace_xml.items():
+            xml.attrib[att] = self.scratchspace[human].toxmlstr(True)
+
+        # --------------------------------------------------------
+
+        # Line tool ----------------------------------------------
+        # 0 is no arrow, arrow styles goes from 1 to 36 (incl)
+        #
+        # DONE: 124 — StartArrow
+        # DONE: 125 — EndArrow
+
+        for att, human in [["StartArrow", "start"], ["EndArrow", "end"]]:
+            xml.attrib[att] = str(self.tools["line"]["arrows"][human])
+
+        # ------------------------------------------------------
+
+        # DONE: 126 — PEN (Shape tool, pen)
+        xml.attrib["PEN"] = str(self.tools["shape"]["pen"]["color"])
+
+        # DONE: 127 — BRUSH (Shape tool, brush)
+        xml.attrib["BRUSH"] = str(self.tools["shape"]["brush"]["color"])
+
+        # 128 — PENLINE (Line tool)
+        xml.attrib["PENLINE"] = str(self.tools["line"]["color"])
+
+        # 129 — PENTEXT
+
+        # 130 — StrokeText
+
+        # 131 — TextBackGround
+        # 132 — TextLineColor
+        # 133 — TextBackGroundShade
+        # 134 — TextLineShade
+        # 135 — TextPenShade
+        # 136 — TextStrokeShade
+
+        # DONE: 137 — STIL (Shape tool)
+        xml.attrib["STIL"] = str(self.tools["shape"]["style"])
+
+        # DONE: 138 — STILLINE (Line tool)
+        xml.attrib["STILLINE"] = str(self.tools["line"]["style"])
+
+        # DONE: 139 — WIDTH (Shape tool)
+        xml.attrib["WIDTH"] = self.tools["shape"]["width"].toxmlstr(True)
+
+        # DONE: 140 — WIDTHLINE (Line tool)
+        xml.attrib["WIDTHLINE"] = self.tools["line"]["width"].toxmlstr(True)
+
+        # DONE: 141 — PENSHADE (Shape tool, pen)
+        xml.attrib["PENSHADE"] = self.tools["shape"]["pen"]["shade"].toxmlstr()
+
+        # DONE: 142 — LINESHADE (Line tool)
+        xml.attrib["LINESHADE"] = self.tools["line"]["shade"].toxmlstr()
+
+        # DONE: 143 — BRUSHSHADE (Shape tool, brush)
+        xml.attrib["BRUSHSHADE"] = self.tools["shape"]["brush"]["shade"].toxmlstr()
+
+        # ------------------------------------------------------
+
+        # TODO: From 144 to 156, most probably Image tool settings
+
+        # 144 — CPICT
+        # 145 — PICTSHADE
+
+        # 146 — CSPICT
+        # 147 — PICTSSHADE
+
+        # 148 — PICTSCX
+        # 149 — PICTSCY
+
+        # 150 — PSCALE
+
+        # 151 — PASPECT
+
+        # 152 — EmbeddedPath
+
+        # 153 — HalfRes
+
+        # 154 — dispX
+        # 155 — dispY
+
+        # 156 — constrain
+
+        # ------------------------------------------------------
+
+        # DONE: 157 — MINORC
+        # DONE: 158 — MAJORC
+        xml.attrib["MINORC"] = self.grids["minor"]["color"]
+        xml.attrib["MAJORC"] = self.grids["major"]["color"]
+
+        # 159 — GuideC
+
+        # DONE: 160 — BaseC
+        xml.attrib["BaseC"] = self.grids["baseline"]["color"]
+
+        # DONE: 161 — renderStack
+
+        if self.ui_show["stack"]:
+            stack = []
+
+            for stack_element in self.ui_show["stack"]:
+                for code, human in Document.ui_stack.items():
+                    if human != stack_element:
+                        continue
+                    stack.append(code)
+                    break
+
+            if stack:
+                stack = " ".join(stack)
+            else:
+                stack = "2 0 4 1 3"
+        else:
+            stack = "2 0 4 1 3"
+
+        xml.attrib["renderStack"] = stack
+
+        # 162 — GridType
+
+        # 163 — PAGEC
+
+        # 164 — MARGC
+
+        # 165 — RANDF
+
+        # 166 — currentProfile
 
         # Calligraphic pen -----------------------------------------------
+        # DONE: 167 — calligraphicPenFillColor
+        # DONE: 168 — calligraphicPenLineColor
+        # DONE: 169 — calligraphicPenFillColorShade
+        # DONE: 170 — calligraphicPenLineColorShade
+        # DONE: 171 — calligraphicPenLineWidth
+        # DONE: 172 — calligraphicPenAngle
+        # DONE: 173 — calligraphicPenWidth
+        # DONE: 174 — calligraphicPenStyle
 
         for key_out_suffix, key_in, as_string in [
-            ["Angle", "angle", True],
-            ["LineWidth", "line_width", True],
-            ["LineColorShade", "line_shade", True],
+            ["FillColor", "fill_color", False],
             ["LineColor", "line_color", False],
+            ["FillColorShade", "fill_shade", True],
+            ["LineColorShade", "line_shade", True],
+            ["LineWidth", "line_width", True],
+            ["Angle", "angle", True],
             ["Width", "width", True],
             ["Style", "style", False],
-            ["FillColor", "fill_color", False],
-            ["FillColorShade", "fill_shade", True],
         ]:
-
             att_name = f"calligraphicPen{key_out_suffix}"
-            att_value = self.calligraphicpen[key_in]
+            att_value = self.tools["calligraphicpen"][key_in]
 
             if as_string:
                 att_value = att_value.toxmlstr()
 
             if key_out_suffix == "Style":
                 att_value = str(att_value)
 
@@ -1114,24 +1723,31 @@
 
         for profile in self.profiles:
             profile_xml = profile.toxml()
 
             if not isinstance(profile_xml, bool):
                 xml.append(profile_xml)
 
-        # ----------------------------------------------------------------
+        # Colors ---------------------------------------------------------
 
-        # Colors
         xml = self.__toxml_items(xml, self.colors)
 
-        # TODO FIXME hyphen
+        # Hyphenation settings -------------------------------------------
+
+        if self.hyphenation is None:
+            hyphen = Hyphenation(default=True)
+            hyphen_xml = hyphen.toxml()
+        else:
+            hyphen_xml = self.hyphenation.toxml()
+
+        xml.append(hyphen_xml)
 
         # Styles ---------------------------------------------------------
 
-        for style_type in ["paragraph", "character", "table", "cell"]:
+        for style_type in ["character", "paragraph", "table", "cell"]:
 
             for style_item in self.styles[style_type]:
                 item_xml = style_item.toxml()
                 xml.append(item_xml)
 
         # ----------------------------------------------------------------
 
@@ -1210,15 +1826,18 @@
 
         if parent:
             item_object = object_class(self)
         else:
             item_object = object_class()
 
         if (success := item_object.fromxml(xml)):
-            attribute.append(item_object)
+            if isinstance(attribute, list):
+                attribute.append(item_object)
+            else:
+                attribute = item_object
 
     def __fromxml_section(
         self,
         xml,
         section_tag: str,
         item_tag: str,
         object_class,
@@ -1321,123 +1940,18 @@
                 if name != style.name:
                     continue
 
                 result.append(style)
 
         return result
 
-    def pageobjects(
-        self, object_type=False, templatable: bool = False
-    ) -> list:
-        """
-        Return document page objets.
-
-        :type object_type: string,bool
-        :param object_type: Page object type to filter, or do not filter at
-            all. See pageobjects.po_type_classes for valid values.
-        :type templatable: bool
-        :param templatable: Only return templatable page objects.
-        """
-
-        pos_ret = []
-
-        # If there is a object type filter, we filter before checking
-        # if we must return only templatable objects
-
-        if object_type:
-
-            if object_type in pageobjects.po_type_classes:
-                pos = []
-
-                for po in self.page_objects:
-                    if isinstance(
-                        po, pageobjects.po_type_classes[object_type]
-                    ):
-                        pos.append(po)
-
-        if templatable:
-
-            if self.sla_parent.templating["active"]:
-                lookup_set = []
-                templatable_set = []
-
-                if object_type:
-                    lookup_set = pos
-                else:
-                    lookup_set = self.page_objects
-
-                for po in lookup_set:
-                    # If the page object is a text frame with templatable
-                    # stories, we add these templatable stories
-
-                    if isinstance(po, pageobjects.TextObject):
-                        po_templatable_stories = po.templatable()
-
-                        if po_templatable_stories:
-                            templatable_set.extend(po_templatable_stories)
-
-                    else:
-                        # TODO If this page object is another type of page
-                        # object, we look its properties and find if it
-                        # is templatable through sla.SLA.templating settings
-
-                        if po.templatable():
-                            templatable_set.append(po)
-
-                pos_ret = templatable_set
-
-        else:
-            if object_type:
-                pos_ret = pos
-            else:
-                pos_ret = self.page_objects
-
-        return pos_ret
-
-    def stories(self) -> list:
-        """
-        Returns all stories in the document.
-
-        :rtype: list
-        :returns: List of stories
-        """
-
-        stories = []
-
-        # Text frames stories --------------------------------------------
-
-        filtered = [
-            po for po in self.page_objects if po.have_stories and po.stories
-        ]
-
-        if filtered:
-
-            for po in filtered:
-                stories.extend(po.stories)
-
-        # Table cells stories --------------------------------------------
-
-        tables = [po for po in self.page_objects if po.ptype == "table"]
-
-        if tables:
-            cells = []
-
-            for po in tables:
-                cells.extend(po.cells)
-
-            for cell in cells:
-                if cell.story is not None:
-                    stories.append(cell.story)
-
-        # ----------------------------------------------------------------
-
-        return stories
-
     # =======================================================================
 
+    # TODO Maybe delete page_number ?
+
     def page_number(self) -> int:
         """
         Get document pages number.
         """
 
         pn = 0
 
@@ -1500,15 +2014,15 @@
                     same_layer = kwargs["overlap_layer"]
                 else:
                     same_layer = True
 
                 if same_layer:
                     page_objets = [
                         po
-                        for po in self.page_objets
+                        for po in self.page_objects
                         if po.layer == sla_object.layer
                     ]
                 else:
                     page_objets = self.page_objects
 
                 for po in page_objets:
                     # TODO FIXME Test coordinates
@@ -2031,8 +2545,121 @@
                     "checkFontIsOpenType",
                 ]
             )
 
         return True
 
 
+class HyphenationRule(PyScribusElement):
+    """
+    Abstract class for hyphenation rules listed in <HYPHEN>.
+    """
+
+    def __init__(self, rule_type: str):
+        super().__init__()
+
+        if rule_type == "exception":
+            self.tag = "EXCEPTION"
+        if rule_type == "exclusion":
+            self.tag = "IGNORE"
+
+        self.word = None
+
+    # PyScribus standard methods -------------------------------
+
+    def toxml(self) -> BoolOrElement:
+        xml = ET.Element(self.tag)
+
+        xml.attrib["WORD"] = self.word
+
+        return xml
+
+    def fromxml(self, xml: ET.Element) -> bool:
+        word = xml.get("WORD")
+
+        if word is None:
+            return False
+
+        self.word = word
+
+        return True
+
+
+class HyphenationException(HyphenationRule):
+    """
+    Hyphenation exception rule (DOCUMENT/HYPHEN/EXCEPTION).
+    """
+
+    def __init__(self):
+        HyphenationRule.__init__(self, "exception")
+
+    def toxml(self) -> BoolOrElement:
+        xml = HyphenationRule.toxml(self)
+        xml.attrib["HYPHENATED"] = self.word
+
+        return xml
+
+
+class HyphenationExclusion(HyphenationRule):
+    """
+    Hyphenation exclusion rule (DOCUMENT/HYPHEN/IGNORE).
+    """
+
+    def __init__(self):
+        HyphenationRule.__init__(self, "exclusion")
+
+
+class Hyphenation(PyScribusElement):
+    """
+    Hyphenation settings of the document (DOCUMENT/HYPHEN).
+    """
+
+    def __init__(self, default=False):
+        super().__init__()
+
+        self.rules = []
+
+        if default:
+            self.fromdefault(default)
+
+    # PyScribus standard methods -------------------------------
+
+    def toxml(self) -> BoolOrElement:
+        xml = ET.Element("HYPHEN")
+
+        for rule in self.rules:
+            rule_xml = rule.toxml()
+            xml.append(rule_xml)
+
+        return xml
+
+    def fromxml(self, xml: ET.Element) -> bool:
+        for element in xml:
+
+            if element.tag not in ["EXCEPTION", "IGNORE"]:
+                continue
+
+            if element.tag == "EXCEPTION":
+                new_rule = HyphenationException()
+
+            if element.tag == "IGNORE":
+                new_rule = HyphenationExclusion()
+
+            if new_rule.fromxml(element):
+                self.rules.append(new_rule)
+
+        return True
+
+    def fromdefault(self, name: str) -> bool:
+        """
+        Set default settings for hyphenation.
+
+        By default, there is no rules (this does not mean anomy).
+
+        :rtype: bool
+        """
+
+        self.rules = []
+
+        return True
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-0.2.5/pyscribus/exceptions.py` & `pyscribus-0.3/pyscribus/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.5/pyscribus/extra/__init__.py` & `pyscribus-0.3/pyscribus/model/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.5/pyscribus/extra/wireframe.py` & `pyscribus-0.3/pyscribus/model/extra/wireframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 and page objects.
 """
 
 # Imports ===============================================================#
 
 from PIL import Image, ImageDraw
 
-import pyscribus.dimensions as dimensions
-import pyscribus.pageobjects as pageobjects
-import pyscribus.pages as pages
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.pageobjects as pageobjects
+import pyscribus.model.pages as pages
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus/headless/__init__.py` & `pyscribus-0.3/pyscribus/model/headless/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Imports ===============================================================#
 
 import copy
 import subprocess
 
 from pathlib import Path
 
-import pyscribus.headless.scripts.topdf as script_to_pdf
+import pyscribus.model.headless.scripts.topdf as script_to_pdf
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 SCRIPTS = {
     "topdf": script_to_pdf,
```

### Comparing `pyscribus-0.2.5/pyscribus/headless/scripts/topdf.py` & `pyscribus-0.3/pyscribus/model/headless/scripts/topdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Usage in Pyscribus:
 
 :Example:
 
 .. code:: python
 
-   from pyscribus.headless import run_pyh_script
+   from pyscribus.model.headless import run_pyh_script
    run_pyh_script("topdf", sla_input="/home/user/example.sla")
 
 Usage in command-line:
 
 .. code:: bash
 
    scribus -g -py to-pdf.py -- file.sla
```

### Comparing `pyscribus-0.2.5/pyscribus/itemattribute.py` & `pyscribus-0.3/pyscribus/model/itemattribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 from __future__ import annotations
 
 from typing import Union, NoReturn
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
+import pyscribus.model.exceptions as exceptions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus/layers.py` & `pyscribus-0.3/pyscribus/model/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 from __future__ import annotations
 
 from typing import Union, NoReturn
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus/logs.py` & `pyscribus-0.3/pyscribus/model/logs.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.5/pyscribus/marks.py` & `pyscribus-0.3/pyscribus/model/marks.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from __future__ import annotations
 
 from typing import NoReturn, Literal, Optional, Union
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
-import pyscribus.exceptions as exceptions
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.exceptions as exceptions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 MarkType = Literal["anchor", "objectref", "markref", "variable", "note"]
```

### Comparing `pyscribus-0.2.5/pyscribus/notes.py` & `pyscribus-0.3/pyscribus/model/notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 import copy
 
 from typing import Union, NoReturn
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
+import pyscribus.model.exceptions as exceptions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus/pageobjects.py` & `pyscribus-0.3/pyscribus/model/pageobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 import math
 
 import lxml
 import lxml.etree as ET
 
 import svg.path as svg
 
-import pyscribus.common.xml as xmlc
-import pyscribus.logs as logs
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
-import pyscribus.itemattribute as itemattribute
-import pyscribus.stories as stories
-import pyscribus.styles as pstyles
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.logs as logs
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.itemattribute as itemattribute
+import pyscribus.model.stories as stories
+import pyscribus.model.styles as pstyles
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 po_type_xml = {
     "image": 2,
@@ -57,16 +57,16 @@
     "symbol": 11,
     "group": 12,
     "table": 16,
 }
 
 # Classes ===============================================================#
 
-# NOTE PageObject est une classe obèse, mais il serait compliqué de gérer
-# autrement les évolutions du SLA dans PyScribus
+# NOTE PageObject is a giant class, but it would be complicated to handle
+# evolutions of SLA in PyScribus otherwise
 
 
 class PageObject(xmlc.PyScribusElement):
     """
     Page object in SLA (``/DOCUMENT/PAGEOBJECT``)
 
     You should rather use :class:`TableObject`, :class:`TextObject`,
@@ -603,15 +603,17 @@
                 ]
             )
 
         xml.attrib["XPOS"] = self.box.coords["top-left"][0].toxmlstr()
         xml.attrib["YPOS"] = self.box.coords["top-left"][1].toxmlstr()
         xml.attrib["WIDTH"] = self.box.dims["width"].toxmlstr()
         xml.attrib["HEIGHT"] = self.box.dims["height"].toxmlstr()
-        xml.attrib["ROT"] = self.rotated_box.rotation.toxmlstr(True)
+
+        if self.rotated_box.rotation.value == 0:
+            xml.attrib["ROT"] = self.rotated_box.rotation.toxmlstr(True)
 
         xml.attrib["ItemID"] = self.object_id
 
         # NOTE OwnPage doit exister quitte à juste être faux (= 0)
         # sinon plantage de Scribus.
         # wiki.scribus.net/canvas/
         # (FR)_Introdution_au_Format_de_fichier_SLA_pour_Scribus_1.4
@@ -619,41 +621,43 @@
         xml.attrib["OwnPage"] = xmlc.bool_or_else_to_num(self.own_page)
 
         # NOTE ANNAME is optional
         if self.name is not None:
             if self.name:
                 xml.attrib["ANNAME"] = self.name
 
-        xml.attrib["LOCALSCX"] = str(self.image_scale["horizontal"])
-        xml.attrib["LOCALSCY"] = str(self.image_scale["vertical"])
+        xml.attrib["LOCALSCX"] = self.image_scale["horizontal"].toxmlstr(True)
+        xml.attrib["LOCALSCY"] = self.image_scale["vertical"].toxmlstr(True)
 
         # Image frame of an image object
 
-        xml.attrib["LOCALX"] = self.image_box.coords["top-left"][0].toxmlstr()
-        xml.attrib["LOCALY"] = self.image_box.coords["top-left"][1].toxmlstr()
+        xml.attrib["LOCALX"] = self.image_box.coords["top-left"][0].toxmlstr(True)
+        xml.attrib["LOCALY"] = self.image_box.coords["top-left"][1].toxmlstr(True)
         xml.attrib["LOCALROT"] = self.image_rotated_box.rotation.toxmlstr(True)
 
         xml.attrib["PICART"] = xmlc.bool_to_num(self.image_box.visible)
 
-        # Undocumented gbox
+        # Undocumented gbox ---------------------------------------------------
 
         xml.attrib["gXpos"] = self.gbox.coords["top-left"][0].toxmlstr()
         xml.attrib["gYpos"] = self.gbox.coords["top-left"][1].toxmlstr()
-        xml.attrib["gWidth"] = self.gbox.dims["width"].toxmlstr()
-        xml.attrib["gHeight"] = self.gbox.dims["height"].toxmlstr()
+        xml.attrib["gWidth"] = self.gbox.dims["width"].toxmlstr(True)
+        xml.attrib["gHeight"] = self.gbox.dims["height"].toxmlstr(True)
+
+        # ---------------------------------------------------------------------
 
         # Page object type
         xml.attrib["PTYPE"] = str(po_type_xml[self.ptype])
 
         # Layer
         xml.attrib["LAYER"] = str(self.layer)
 
         # --- Opacity of the object ----------------------------------
 
-        if self.opacity.value <= float(1):
+        if self.opacity.value < float(1):
             xml.attrib["TransValue"] = self.opacity.toxmlstr(True)
 
         # ------------------------------------------------------------
 
         if self.shape["type"] is None:
             # If the shape type is not defined, we assume the frame has
             # a rectangular shape, as it is the most common
@@ -714,15 +718,15 @@
 
         if self.outline["fill"] is not None:
             xml.attrib["PCOLOR"] = self.outline["fill"]
 
         if self.outline["stroke"] is not None:
             xml.attrib["PCOLOR2"] = self.outline["stroke"]
 
-        xml.attrib["PWIDTH"] = self.outline["thickness"].toxmlstr()
+        xml.attrib["PWIDTH"] = self.outline["thickness"].toxmlstr(True)
 
         # ------------------------------------------------------------
 
         if self.ptype in ["image", "render"]:
             xml.attrib["EMBEDDED"] = xmlc.bool_to_num(self.embedded_icc["use"])
 
             if self.embedded_icc["profile"]:
@@ -851,14 +855,23 @@
 
                 if setting_name == "height":
                     self.box.dims["height"].value = float(setting_value)
 
                 if setting_name == "layer":
                     self.layer = setting_value
 
+                if setting_name == "outline_fill":
+                    self.outline["fill"] = setting_value
+
+                if setting_name == "outline_stroke":
+                    self.outline["stroke"] = setting_value
+
+                if setting_name == "object_id":
+                    self.object_id = setting_value
+
 
 # Inherited from PageObject =============================================#
 
 
 class TableObject(PageObject):
     """
     Table frame.
@@ -1759,22 +1772,37 @@
 
                 if setting_name == "columns":
                     self.columns["count"] = int(setting_value)
 
                 if setting_name == "columnsgap":
                     self.columns["gap"].value = float(setting_value)
 
-    def fromdefault(self, default="with-story"):
-        story = stories.Story()
-        story.fromdefault()
-        self.stories.append(story)
-        self.have_stories = True
+    def fromdefault(self, default: str = "with-story"):
+        # Page object default
+
+        # FIXME Those two line are hacks
+        self.text_flow = PageObject.text_flow_xml["2"]
+        self.path_options["text_on_path"] = {
+            "show": False,
+            "offset": dimensions.Dim(0)
+        }
+
+        self.outline["fill"] = None
+        self.outline["stroke"] = None
 
         self.columns = {"gap": dimensions.Dim(0), "count": 1}
 
+        # Stories default
+
+        if default == "with-story":
+            story = stories.Story()
+            story.fromdefault()
+            self.stories.append(story)
+            self.have_stories = True
+
     def templatable(self):
         temp_stories = []
 
         if self.have_stories and self.stories:
 
             for story in self.stories:
 
@@ -1881,15 +1909,15 @@
 
         if not isinstance(xml, ET._Element):
             return False
 
         # Attributes -------------------------------------------------
 
         xml.attrib["COLUMNS"] = str(self.columns["count"])
-        xml.attrib["COLGAP"] = self.columns["gap"].toxmlstr()
+        xml.attrib["COLGAP"] = self.columns["gap"].toxmlstr(True)
 
         if self.alignment is not None:
             xml.attrib["ALIGN"] = xmlc.alignment[self.alignment]
 
         xml.attrib["VAlign"] = TextObject.vertical_alignment_xml[
             self.vertical_alignment
         ]
@@ -2136,15 +2164,17 @@
         # Compression method ------------------------------
 
         # @CMethod and @COMPRESSIONMETHOD follow the same syntax
 
         cmethod = xml.get("CMethod")
         cmethod_long = xml.get("COMPRESSIONMETHOD")
 
-        for att, value in [[cmethod_long], [cmethod]]:
+        for att, value in [
+            ["COMPRESSIONMETHOD", cmethod_long], ["CMethod", cmethod]
+        ]:
             if value is None:
                 continue
 
             self.compression["method"] = ImageObject.compression_method_xml[value]
             self.compression["__method"] = att
 
         # -------------------------------------------------
```

### Comparing `pyscribus-0.2.5/pyscribus/pages.py` & `pyscribus-0.3/pyscribus/model/pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 from typing import Optional, NoReturn, Literal
 
 from enum import Enum, IntEnum
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.logs as logs
-import pyscribus.common.xml as xmlc
-import pyscribus.common.math as mathc
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.logs as logs
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.common.math as mathc
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 PageOrientation = Literal["portrait", "landscape"]
 
@@ -429,17 +429,25 @@
             self.auto_guides["selection"]["posy"].value = agy
             self.auto_guides["selection"]["width"].value = agw
             self.auto_guides["selection"]["height"].value = agh
 
         # PDF effects ----------------------------------------------------
 
         if (duration := xml.get("pageEffectDuration")) is not None:
+            # FIXME Maybe a hack
+            if duration == "None":
+                duration = 1
+
             self.effect["duration"].value = int(duration)
 
         if (view_duration := xml.get("pageViewDuration")) is not None:
+            # FIXME Maybe a hack
+            if view_duration == "None":
+                view_duration = 1
+
             self.effect["view-duration"].value = int(view_duration)
 
         if (effect_type := xml.get("effectType")) is not None:
             for human, code in PageAbstract.effect_type_xml.items():
                 if effect_type == code:
                     self.effect["type"] = human
                     break
@@ -550,15 +558,15 @@
             # Page lines / columns origin
             # 0 = Page 1 = Margins
             # AGhorizontalAutoRefer="0"
             # AGverticalAutoRefer="0"
             orig_att = f"AG{orientation}AutoRefer"
 
             xml.attrib[count_att] = str(self.auto_guides[items]["count"])
-            xml.attrib[gap_att] = self.auto_guides[items]["gap"].toxmlstr()
+            xml.attrib[gap_att] = self.auto_guides[items]["gap"].toxmlstr(True)
             xml.attrib[orig_att] = PageAbstract.autoguides_origin_xml[
                 self.auto_guides[items]["origin"]
             ]
 
         # Check if auto guides if different from default value
         # If the X, Y, W, H of the selection are 0, then it is not custom
```

### Comparing `pyscribus-0.2.5/pyscribus/papers/__init__.py` & `pyscribus-0.3/pyscribus/model/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """
-PyScribus submodule for paper sizes
+PyScribus
+
+SLA file model
 """
 
+from pyscribus.model.sla import SLA
+
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
-__version__ = "0.1"
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-0.2.5/pyscribus/papers/afnor.py` & `pyscribus-0.3/pyscribus/model/papers/afnor.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Petit Aigle, Grand Aigle, Grand Monde, Univers
 
 For more common and international paper sizes, see iso216paper module.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 
 class Cloche(FloatEnum):
```

### Comparing `pyscribus-0.2.5/pyscribus/papers/ansi.py` & `pyscribus-0.3/pyscribus/model/papers/ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ANSI A to E formats.
 
 Yes, this is the module for Letter paper sizes, as Letter = ANSI A.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM, INCH_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM, INCH_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus/papers/iso216.py` & `pyscribus-0.3/pyscribus/model/papers/iso216.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 See iso269paper module for C format.
 See iso217paper module for RA, SRA formats.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus/papers/iso217.py` & `pyscribus-0.3/pyscribus/model/papers/iso217.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 See iso216paper module for A, B formats.
 See iso269paper module for C format (including DL).
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Raw A -----------------------------------------
```

### Comparing `pyscribus-0.2.5/pyscribus/papers/iso269.py` & `pyscribus-0.3/pyscribus/model/papers/iso269.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 See iso216paper module for A, B formats.
 See iso217paper module for RA, SRA formats.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 
 class C0(FloatEnum):
```

### Comparing `pyscribus-0.2.5/pyscribus/papers/newspaper.py` & `pyscribus-0.3/pyscribus/model/papers/newspaper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Often used newspapers sizes.
 
 Berliner, Belgian, Tabloid, Broadsheet formats.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 
 class Berliner(FloatEnum):
```

### Comparing `pyscribus-0.2.5/pyscribus/patterns.py` & `pyscribus-0.3/pyscribus/model/patterns.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 
 # To avoid Sphinx complaints from methods annotations referencing same class
 from __future__ import annotations
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
-import pyscribus.pageobjects as pageobjects
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.pageobjects as pageobjects
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus/printing.py` & `pyscribus-0.3/pyscribus/model/printing.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 import collections
 
 from typing import NoReturn, Union
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
+import pyscribus.model.exceptions as exceptions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
-import pyscribus.dimensions as dimensions
+import pyscribus.model.dimensions as dimensions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
@@ -490,17 +490,17 @@
         for bleed_config, bleed_value in self.bleeds.items():
 
             if bleed_config != "document":
                 att_name = "B{}".format(bleed_config.capitalize())
                 # FIXME Sometimes raises errors (when PDF/@BTop="0") because
                 # not a list
                 try:
-                    xml.attrib[att_name] = bleed_value[0].toxmlstr()
+                    xml.attrib[att_name] = bleed_value[0].toxmlstr(True)
                 except:
-                    xml.attrib[att_name] = bleed_value.toxmlstr()
+                    xml.attrib[att_name] = bleed_value.toxmlstr(True)
 
         xml.attrib["useDocBleeds"] = bool_to_num(self.bleeds["document"])
 
         # PDF marks settings -------------------------------
 
         for mark_tag, mark_key in [
                 ["bleedMarks", "bleeds"],
@@ -772,15 +772,15 @@
 
         # TODO
 
         for bleed_config, bleed_value in self.bleeds.items():
 
             if bleed_config != "document":
                 att_name = "Bleed{}".format(bleed_config.capitalize())
-                xml.attrib[att_name] = bleed_value[0].toxmlstr()
+                xml.attrib[att_name] = bleed_value[0].toxmlstr(True)
 
         xml.attrib["mirrorH"] = bool_to_num(self.mirror_pages["horizontal"])
         xml.attrib["mirrorV"] = bool_to_num(self.mirror_pages["vertical"])
 
         xml.attrib["useDocBleeds"] = bool_to_num(self.bleeds["document"])
 
         for key, value in self.marks.items():
```

### Comparing `pyscribus-0.2.5/pyscribus/stories.py` & `pyscribus-0.3/pyscribus/model/stories.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 import copy
 
 from typing import Union, NoReturn, List
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
-import pyscribus.marks as marks
-import pyscribus.notes as notes
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.marks as marks
+import pyscribus.model.notes as notes
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
@@ -77,21 +77,57 @@
 
         if (parent := xml.get("PARENT")) is not None:
             self.parent = parent
 
         return True
 
 
-class StoryDefaultStyle(OrphanElement):
+class StoryDefaultStyle(PyScribusElement):
     """
     Default style marker in Scribus stories (DefaultStyle)
     """
 
     def __init__(self):
-        OrphanElement.__init__(self, "DefaultStyle")
+        super().__init__()
+
+        self.parent_paragraph = None
+        self.parent_character = None
+
+    def fromxml(self, xml: ET.Element) -> bool:
+        """
+        :rtype: boolean
+        :returns: True if XML parsing succeed
+        """
+
+        if xml.tag != "DefaultStyle":
+            return False
+
+        if (para_parent := xml.get("PARENT")) is not None:
+            self.parent_paragraph = para_parent
+
+        if (chara_parent := xml.get("CPARENT")) is not None:
+            self.parent_character = chara_parent
+
+        return True
+
+    def toxml(self) -> ET.Element:
+        """
+        :rtype: lxml.etree._Element
+        :returns: XML representation of default style marker.
+        """
+
+        xml = ET.Element("DefaultStyle")
+
+        if self.parent_paragraph is not None:
+            xml.attrib["PARENT"] = self.parent_paragraph
+
+        if self.parent_character is not None:
+            xml.attrib["CPARENT"] = self.parent_character
+
+        return xml
 
 
 class StoryLineBreak(OrphanElement):
     """
     Line break marker in Scribus stories (breakline)
     """
 
@@ -258,14 +294,16 @@
 
         self.text = ""
 
         # To not export to XML. This is defined by the following
         # StoryParagraphEnding in Story.sequence
         self.paragraph_style = False
 
+        self.parent_character = None
+
         self.font = {
             "name": False,
             "size": False,
             "color": False,
             "opacity": False,
         }
 
@@ -391,22 +429,28 @@
             xml.attrib["FEATURES"] = features
 
         for human, attr_name in StoryFragment.font_xml:
 
             if self.font[human]:
                 xml.attrib[attr_name] = self.font[human]
 
+        if self.parent_character is not None:
+            xml.attrib["CPARENT"] = self.parent_character
+
         xml.attrib["CH"] = self.text
 
         return xml
 
     def fromxml(self, xml: ET._Element) -> bool:
         if (fragtext := xml.get("CH")) is None:
             return False
 
+        if (chara_parent := xml.get("CPARENT")) is not None:
+            self.parent_character = chara_parent
+
         # NOTE Don't do any strip, rstrip to @CH, as it may
         # contains legitimate spaces
         self.text = fragtext
 
         if (features := xml.get("FEATURES")) is not None:
             self.set_features(features)
 
@@ -1229,15 +1273,19 @@
 
         if xml.tag != "StoryText":
             return False
 
         for element in xml:
 
             if element.tag == "DefaultStyle":
-                self.sequence.append(StoryDefaultStyle())
+                default_xml = StoryDefaultStyle()
+                success = default_xml.fromxml(element)
+
+                if success:
+                    self.sequence.append(default_xml)
 
             if element.tag == "ITEXT":
 
                 frag = StoryFragment()
                 success = frag.fromxml(element)
 
                 if success:
@@ -1473,107 +1521,9 @@
 
                 if isinstance(element, class_test):
                     tmp.append(element)
                     break
 
         return pars
 
-    def rawtext(self) -> str:
-        """
-        Returns a text string equivalent to *what Scribus story editor
-        saves* as txt file.
-
-        :rtype: string
-        """
-        text = ""
-
-        for par in self.bypars():
-
-            for element in par:
-
-                # NOTE Text formatting is not saved
-                if isinstance(element, StoryFragment):
-                    text += element.text
-
-                if isinstance(element, NonBreakingSpace):
-                    text += " "
-
-                # NOTE Line breaks are exported by Scribus... as spaces
-                if isinstance(element, StoryLineBreak):
-                    text += " "
-
-                # NOTE We dont care about StoryFrameBreak and StoryColumnBreak
-
-                if isinstance(element, StoryParagraphEnding):
-                    text += "\n"
-
-        return text
-
-    def templatable(self) -> list:
-        """
-        Return elements of Story sequence that are available for templating.
-
-        :rtype: list
-        :returns: List of pyscribus.stories.StoryFragment
-        """
-
-        contents = []
-
-        pattern = self.sla_parent.templating["intext-pattern"]
-
-        for element in self.sequence:
-
-            if isinstance(element, StoryFragment):
-
-                if pattern.findall(element.text) is not None:
-                    contents.append(element)
-
-        return contents
-
-    def feed_templatable(self, datas: dict) -> Union[bool, List[StoryFragment]]:
-        """
-        Feed template-able datas into this story.
-
-        :returns: List of modified elements in this story, or False
-        :rtype: Union[bool, list]
-        """
-
-        elements = self.templatable()
-
-        if elements:
-            modified = []
-
-            for element in elements:
-
-                for template_key, template_value in datas.items():
-
-                    if template_key not in element.text:
-                        continue
-
-                    new_value = None
-
-                    if isinstance(datas[template_key], list):
-                        # We have %key% -> ["Value1", "Value2", …]
-                        # So the first occurrence of %key% is "Value1", the
-                        # second "Value2", etc.
-
-                        if len(datas[template_key]):
-                            new_value = datas[template_key].pop(0)
-                    else:
-                        # We have %key% -> "Value"
-                        new_value = template_value
-
-                    if new_value is None:
-                        continue
-
-                    element.text = element.text.replace(
-                        template_key, new_value
-                    )
-
-                    modified.append(element)
-
-            return modified
-
-        return False
-
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-0.2.5/pyscribus/styles.py` & `pyscribus-0.3/pyscribus/model/styles.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from typing import Union, Optional, NoReturn, Literal
 from enum import IntEnum
 from pathlib import Path
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
-import pyscribus.common.math as mathc
-import pyscribus.logs as logs
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.common.math as mathc
+import pyscribus.model.logs as logs
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 StringOrPath = Union[str, Path]
 BoolOrElement = Union[bool, ET.Element]
@@ -255,15 +255,15 @@
         if self.style_type in ["paragraph", "character"]:
             # TODO FIXME Handle font features as a dict instead
             # of a list, like in other styles
             # Features: -clig, inherit
 
             self.font = {
                 "name": "",
-                "size": 0,
+                "size": dimensions.Dim(0, unit="pt"),
                 "features": [],
                 "color": "",
                 "alignment": "left",
                 "strike": {"width": None, "offset": None},
                 "underline": {"width": None, "offset": None},
                 "shadow": {"hoffset": None, "voffset": None},
                 # NOTE There is no offset setting for outline, obviously
@@ -417,15 +417,15 @@
 
             # Font and font features ---------------------------------
 
             if (font := xml.get("FONT")) is not None:
                 self.font["name"] = font
 
             if (font_size := xml.get("FONTSIZE")) is not None:
-                self.font["size"] = float(font_size)
+                self.font["size"].value = float(font_size)
 
             if (font_features := xml.get("FONTFEATURES")) is not None:
                 self.font["features"] = font_features.split(",")
 
             if (font_color := xml.get("FCOLOR")) is not None:
                 self.font["color"] = font_color
 
@@ -551,22 +551,27 @@
         # Common attributes to paragraphs + characters ---------
 
         if self.style_type in ["paragraph", "character"]:
 
             bshade_att = self._choose_att(StyleAbstract.bg_shade_xml)
             bcolor_att = self._choose_att(StyleAbstract.bg_color_xml)
 
-            xml.attrib[bcolor_att] = self.background["color"]
-            xml.attrib[bshade_att] = self.background["shade"].toxmlstr(True)
+            if self.background["color"] == "None":
+                xml.attrib[bcolor_att] = "None"
+            else:
+                xml.attrib[bcolor_att] = self.background["color"]
+
+            if self.background["shade"].value <= 100:
+                xml.attrib[bshade_att] = self.background["shade"].toxmlstr(True)
 
             if self.font["name"]:
                 xml.attrib["FONT"] = self.font["name"]
 
             if self.style_type == "character":
-                xml.attrib["FONTSIZE"] = str(self.font["size"])
+                xml.attrib["FONTSIZE"] = self.font["size"].toxmlstr(True)
 
             # TODO FIXME Handle font features as a dict instead
             # of a list, like in other styles
             # xml.attrib["FONTFEATURES"] = " ".join(self.font["features"].keys())
 
             if self.font["features"]:
                 xml.attrib["FONTFEATURES"] = ",".join(self.font["features"])
@@ -982,26 +987,27 @@
             xml.attrib["HyphenConsecutiveLines"] = str(
                 self.hyphen_following_lines
             )
 
         # Optical margins -----------------------------------------------
 
         if self.optical_margins is not None:
-            xml.attrib["OpticalMargins"] = str(
-                ParagraphStyle.optical_margins_xml[self.optical_margins]
-            )
+            if self.optical_margins != "undef":
+                xml.attrib["OpticalMargins"] = str(
+                    ParagraphStyle.optical_margins_xml[self.optical_margins]
+                )
 
         # Initial capital (aka drop capital) ----------------------------
 
         xml.attrib["DROP"] = xmlc.bool_to_num(self.initial["active"])
         xml.attrib["DROPLIN"] = str(self.initial["lines"])
 
         xml.attrib[self.initial["__offset_att"]] = self.initial[
             "offset"
-        ].toxmlstr()
+        ].toxmlstr(True)
 
         if self.initial["auto_indent"]:
             xml.attrib["ParagraphEffectIndent"] = xmlc.bool_to_num(
                 self.initial["auto_indent"]
             )
 
         # Glyph scaling ---------------------------------------------
@@ -1017,28 +1023,28 @@
         if self.leading["mode"] is not None:
             xml.attrib["LINESPMode"] = ParagraphStyle.leading_xml[
                 self.leading["mode"]
             ]
 
         if self.leading["mode"] in ["fixed", "automatic"]:
             if self.leading["value"].value > 0:
-                xml.attrib["LINESP"] = self.leading["value"].toxmlstr()
+                xml.attrib["LINESP"] = self.leading["value"].toxmlstr(True)
 
         # Indentation -----------------------------------------------
 
         for case in [
             ["left", "INDENT"],
             ["right", "RMARGIN"],
             ["first-line", "FIRST"],
         ]:
 
             if self.indentations[case[0]] is None:
                 xml.attrib[case[1]] = "0"
             else:
-                xml.attrib[case[1]] = self.indentations[case[0]].toxmlstr()
+                xml.attrib[case[1]] = self.indentations[case[0]].toxmlstr(True)
 
         # Lists ---------------------------------------------------------
 
         if self.listing["type"] == "ol":
             att_seq = [False, True]
         elif self.listing["type"] == "ul":
             att_seq = [True, False]
@@ -1049,15 +1055,16 @@
             xml.attrib[list_att] = xmlc.bool_to_num(list_val)
 
         if self.listing["type"] == "ol":
             xml.attrib["NumerationFormat"] = ParagraphStyle.ol_types[
                 self.listing["subtype"]
             ]
 
-        xml.attrib["BulletStr"] = xmlc.none_or_str(self.listing["char"])
+        if self.listing["type"] is not None:
+            xml.attrib["BulletStr"] = xmlc.none_or_str(self.listing["char"])
 
         # Parent character style ------------------------------------
 
         # NOTE To not confuse with parent paragraph style which is
         # in @PARENT, and handled in StyleAbstract
 
         if self.character_parent:
@@ -1068,24 +1075,26 @@
                 xml.attrib[case[1]] = self.space[case[0]].toxmlstr(True)
 
         # xml.attrib["VOR"] = self.space["before"].toxmlstr()
         # xml.attrib["NACH"] = self.space["after"].toxmlstr()
 
         # FONT SIZE -------------------------------------------------
 
-        font_size = str(self.font["size"])
+        font_size = str(self.font["size"]).strip()
 
-        if self.character_parent and font_size == "0":
-            # If the font size of the paragraph is not defined
-            # because it is defined in a parent character style,
-            # don't write FONTSIZE attribute
-            pass
-        else:
-            if font_size != "0":
-                xml.attrib["FONTSIZE"] = font_size
+        if font_size != "0":
+            xml.attrib["FONTSIZE"] = str(
+                mathc.necessary_float(float(font_size))
+            )
+
+            if self.character_parent:
+                # If the font size of the paragraph is not defined
+                # because it is defined in a parent character style,
+                # don't write FONTSIZE attribute
+                pass
 
         # -----------------------------------------------------------
 
         try:
             xml, undoc_attribs = xmlc.all_undocumented_to_xml(
                 xml,
                 self.undocumented,
@@ -1289,15 +1298,15 @@
 
     def toxml(self) -> ET.Element:
         xml = StyleAbstract.toxml(self)
 
         # Stroke settings -----------------------------------------------
 
         xml.attrib["SCOLOR"] = self.stroke["color"]
-        xml.attrib["SSHADE"] = self.stroke["shade"].toxmlstr()
+        xml.attrib["SSHADE"] = self.stroke["shade"].toxmlstr(True)
 
         # Hyphenation ---------------------------------------------------
 
         if self.hyphen_word_min is not None:
             xml.attrib["HyphenWordMin"] = str(self.hyphen_word_min)
 
         # Font settings -------------------------------------------------
```

### Comparing `pyscribus-0.2.5/pyscribus/toc.py` & `pyscribus-0.3/pyscribus/model/toc.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from __future__ import annotations
 
 from typing import Union, NoReturn
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
-import pyscribus.exceptions as exceptions
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.exceptions as exceptions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-0.2.5/pyscribus.egg-info/PKG-INFO` & `pyscribus-0.3/pyscribus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscribus
-Version: 0.2.5
+Version: 0.3
 Summary: Read, create and update Scribus .sla files.
 Author: Étienne Nadji
 Author-email: etnadji@eml.cc
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://etnadji.fr/pyscribus
 Project-URL: Source Code, https://framagit.org/etnadji/pyscribus
 Project-URL: Issue tracker, https://framagit.org/etnadji/pyscribus/-/issues
```

### Comparing `pyscribus-0.2.5/setup.py` & `pyscribus-0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,53 @@
 #!/usr/bin/python3
 # -*- coding:Utf-8 -*-
 
 import setuptools
 
+# from distutils import util
+
 with open("../README.pypi.rst", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.2.5"
+VERSION = "0.3"
 DESCRIPTION = "Read, create and update Scribus .sla files."
 
 REQUIRED = ['lxml', 'svg.path']
 
+# pyscribus_path = util.convert_path('pyscribus')
+# subp_file = util.convert_path('pyscribus/file')
+# subp_model = util.convert_path('pyscribus/model')
+
 setuptools.setup(
     name="pyscribus",
     version=VERSION,
     author="Étienne Nadji",
     author_email="etnadji@eml.cc",
     description=DESCRIPTION,
     long_description=long_description,
+
     packages=setuptools.find_packages(),
+
+    # package_dir={'':'source/pyscribus'},
+    # packages=setuptools.find_packages("source", include=["pyscribus"]),
+
+    # package_dir={
+        # 'pyscribus': pyscribus_path,
+        # 'pyscribus.file': subp_file,
+        # 'pyscribus.model': subp_model,
+    # },
+    # packages=['pyscribus', 'pyscribus.file', 'pyscribus.model'],
+
+    # packages=setuptools.find_packages("pyscribus"),
+
+    # package_dir={"":".", "pyscribus.model": "pyscribus/model", "pyscribus.file": "pyscribus/file"},
+
+    # package_dir={"":"."},
+    # packages=setuptools.find_packages(),
+
     platforms='any',
     license="GNU Affero General Public License v3 or later (AGPLv3+)",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: OS Independent",
         "Topic :: Multimedia :: Graphics",
```

