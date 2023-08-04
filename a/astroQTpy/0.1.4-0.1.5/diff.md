# Comparing `tmp/astroQTpy-0.1.4.tar.gz` & `tmp/astroQTpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroQTpy-0.1.4.tar", last modified: Mon Jul 31 21:41:39 2023, max compression
+gzip compressed data, was "astroQTpy-0.1.5.tar", last modified: Fri Aug  4 16:14:31 2023, max compression
```

## Comparing `astroQTpy-0.1.4.tar` & `astroQTpy-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.215078 astroQTpy-0.1.4/
--rw-r--r--   0 calebharada   (501) staff       (20)     1069 2023-07-15 16:01:20.000000 astroQTpy-0.1.4/LICENSE
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-31 21:41:39.214590 astroQTpy-0.1.4/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)     1307 2023-07-31 21:39:08.000000 astroQTpy-0.1.4/README.md
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.207322 astroQTpy-0.1.4/astroQTpy.egg-info/
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      381 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/SOURCES.txt
--rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/dependency_links.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       47 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/requires.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       16 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/top_level.txt
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.211280 astroQTpy-0.1.4/astroqtpy/
--rw-r--r--   0 calebharada   (501) staff       (20)      135 2023-07-31 21:34:54.000000 astroQTpy-0.1.4/astroqtpy/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)    16457 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/basetree.py
--rw-r--r--   0 calebharada   (501) staff       (20)     8904 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/quadnode.py
--rw-r--r--   0 calebharada   (501) staff       (20)      831 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/quadpoint.py
--rw-r--r--   0 calebharada   (501) staff       (20)    14141 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/quadtree.py
--rw-r--r--   0 calebharada   (501) staff       (20)       79 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/pyproject.toml
--rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-31 21:41:39.215185 astroQTpy-0.1.4/setup.cfg
--rw-r--r--   0 calebharada   (501) staff       (20)      876 2023-07-26 23:07:18.000000 astroQTpy-0.1.4/setup.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.213451 astroQTpy-0.1.4/tests/
--rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-20 22:59:55.000000 astroQTpy-0.1.4/tests/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     1383 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/tests/test_quadnode.py
--rw-r--r--   0 calebharada   (501) staff       (20)      721 2023-07-20 01:38:47.000000 astroQTpy-0.1.4/tests/test_quadpoint.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-08-04 16:14:31.044959 astroQTpy-0.1.5/
+-rw-r--r--   0 calebharada   (501) staff       (20)     1069 2023-07-15 16:01:20.000000 astroQTpy-0.1.5/LICENSE
+-rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-08-04 16:14:31.044602 astroQTpy-0.1.5/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)     1307 2023-07-31 21:39:08.000000 astroQTpy-0.1.5/README.md
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-08-04 16:14:31.041811 astroQTpy-0.1.5/astroQTpy.egg-info/
+-rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-08-04 16:14:30.000000 astroQTpy-0.1.5/astroQTpy.egg-info/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)      381 2023-08-04 16:14:30.000000 astroQTpy-0.1.5/astroQTpy.egg-info/SOURCES.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-08-04 16:14:30.000000 astroQTpy-0.1.5/astroQTpy.egg-info/dependency_links.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       47 2023-08-04 16:14:30.000000 astroQTpy-0.1.5/astroQTpy.egg-info/requires.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       16 2023-08-04 16:14:30.000000 astroQTpy-0.1.5/astroQTpy.egg-info/top_level.txt
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-08-04 16:14:31.043374 astroQTpy-0.1.5/astroqtpy/
+-rw-r--r--   0 calebharada   (501) staff       (20)      135 2023-08-04 16:07:56.000000 astroQTpy-0.1.5/astroqtpy/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    16457 2023-07-26 22:04:11.000000 astroQTpy-0.1.5/astroqtpy/basetree.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     8956 2023-08-04 16:07:56.000000 astroQTpy-0.1.5/astroqtpy/quadnode.py
+-rw-r--r--   0 calebharada   (501) staff       (20)      831 2023-07-26 22:04:11.000000 astroQTpy-0.1.5/astroqtpy/quadpoint.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    14141 2023-07-26 22:04:11.000000 astroQTpy-0.1.5/astroqtpy/quadtree.py
+-rw-r--r--   0 calebharada   (501) staff       (20)       79 2023-07-26 22:04:11.000000 astroQTpy-0.1.5/pyproject.toml
+-rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-08-04 16:14:31.045045 astroQTpy-0.1.5/setup.cfg
+-rw-r--r--   0 calebharada   (501) staff       (20)      876 2023-07-26 23:07:18.000000 astroQTpy-0.1.5/setup.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-08-04 16:14:31.044204 astroQTpy-0.1.5/tests/
+-rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-20 22:59:55.000000 astroQTpy-0.1.5/tests/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1383 2023-07-26 22:04:11.000000 astroQTpy-0.1.5/tests/test_quadnode.py
+-rw-r--r--   0 calebharada   (501) staff       (20)      721 2023-07-20 01:38:47.000000 astroQTpy-0.1.5/tests/test_quadpoint.py
```

### Comparing `astroQTpy-0.1.4/LICENSE` & `astroQTpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.4/README.md` & `astroQTpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.4/astroqtpy/basetree.py` & `astroQTpy-0.1.5/astroqtpy/basetree.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.4/astroqtpy/quadnode.py` & `astroQTpy-0.1.5/astroqtpy/quadnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,18 @@
             
             if show_lines:
                 ax.plot([x1, x2, x2, x1, x1], [y2, y2, y1, y1, y2],
                         c="k", lw=1, alpha=0.5
                         )
             
             if show_points:
-                ax.scatter(*zip(*[(point.x, point.y) for point in self.node_points]),
-                           c='k', s=1, marker='.', alpha=0.8, rasterized=True
-                           )
+                if len(self.node_points) > 0:
+                    ax.scatter(*zip(*[(point.x, point.y) for point in self.node_points]),
+                            c='k', s=1, marker='.', alpha=0.8, rasterized=True
+                            )
                 
             if show_values:
                 x_mid = 0.5 * (x1 + x2)
                 y_mid = 0.5 * (y1 + y2)
                 ax.text(x_mid, y_mid, round(self.get_node_value(statistic), 2),
                         horizontalalignment="center", verticalalignment="center", c="k", size=10
                         )
```

### Comparing `astroQTpy-0.1.4/astroqtpy/quadpoint.py` & `astroQTpy-0.1.5/astroqtpy/quadpoint.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.4/astroqtpy/quadtree.py` & `astroQTpy-0.1.5/astroqtpy/quadtree.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.4/setup.py` & `astroQTpy-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.4/tests/test_quadnode.py` & `astroQTpy-0.1.5/tests/test_quadnode.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.4/tests/test_quadpoint.py` & `astroQTpy-0.1.5/tests/test_quadpoint.py`

 * *Files identical despite different names*

