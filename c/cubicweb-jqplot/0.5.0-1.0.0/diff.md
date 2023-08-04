# Comparing `tmp/cubicweb-jqplot-0.5.0.tar.gz` & `tmp/cubicweb-jqplot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-jqplot-0.5.0.tar", last modified: Thu Jul 18 11:35:42 2019, max compression
+gzip compressed data, was "cubicweb-jqplot-1.0.0.tar", last modified: Fri Aug  4 13:36:40 2023, max compression
```

## Comparing `cubicweb-jqplot-0.5.0.tar` & `cubicweb-jqplot-1.0.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      329 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/MANIFEST.in
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2618 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/setup.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      426 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/tox.ini
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       43 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       16 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/top_level.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     4193 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       17 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      625 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/PKG-INFO
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      648 2019-07-18 11:34:46.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/__pkginfo__.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    14746 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/views.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       82 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/__init__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    13301 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/cubes.jqplot.ext.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      228 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/icon_csv.gif
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      266 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/cubes.jqplot.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)   173216 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1082 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/MIT-LICENSE.txt
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       77 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/cubes.jqplot.css
--rw-------   0 ppepiot   (1000) ppepiot   (1000)   464537 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     5600 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.css
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      103 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/icon_png.gif
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2217 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/copyright.txt
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     3561 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.min.css
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     7585 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.trendline.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     8981 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    12840 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2091 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mobile.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     9494 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    17280 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.json2.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    34262 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     5373 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    10651 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    29618 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     9155 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     9605 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     8474 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    20119 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    37209 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    17991 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    21630 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    15493 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    10536 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    42865 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    14475 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    15248 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    31038 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     5665 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.json2.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     6274 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     9487 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dragable.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    21255 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    33910 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    12102 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     5204 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    15136 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     3073 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mobile.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    25532 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    14563 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     8137 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    24364 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    11452 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    11771 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    20876 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.cursor.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    46088 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.cursor.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    39777 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    15756 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    35500 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     4129 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    30209 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    18945 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     4438 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.trendline.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    27960 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    21112 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    14531 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    13728 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2899 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    15448 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     6719 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     9604 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    22490 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     6922 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)    15336 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     4808 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.min.js
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     6285 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dragable.min.js
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/setup.cfg
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      148 2019-06-04 23:54:18.000000 cubicweb-jqplot-0.5.0/README
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      625 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/PKG-INFO
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 11:35:42.000000 cubicweb-jqplot-0.5.0/test/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1010 2019-06-13 07:04:34.000000 cubicweb-jqplot-0.5.0/test/test_jqplot.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:36:40.062229 cubicweb-jqplot-1.0.0/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      412 2023-08-04 12:34:18.000000 cubicweb-jqplot-1.0.0/MANIFEST.in
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      570 2023-08-04 13:36:40.058228 cubicweb-jqplot-1.0.0/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      148 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/README.rst
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:36:40.006228 cubicweb-jqplot-1.0.0/cubicweb_jqplot/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       82 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/__init__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      698 2023-08-04 12:34:18.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/__pkginfo__.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:36:40.018228 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1082 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/MIT-LICENSE.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2217 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/copyright.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       77 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/cubes.jqplot.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    13301 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/cubes.jqplot.ext.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      266 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/cubes.jqplot.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      228 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/icon_csv.gif
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      103 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/icon_png.gif
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     5600 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)   464537 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     3561 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.min.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)   173216 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.min.js
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:36:40.058228 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    14475 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     8474 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    34262 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    15493 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     9155 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     5373 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    31038 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    15136 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     8137 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     4808 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     9604 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     5204 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    37209 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    14563 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    24364 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    17991 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    27960 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    11771 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     4129 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2899 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    46088 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.cursor.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    20876 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.cursor.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    30209 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    12102 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    33910 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    15336 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     9487 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dragable.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     6285 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dragable.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    13728 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     6922 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    39777 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    15448 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    21255 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     9605 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    17280 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.json2.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     5665 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.json2.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    21630 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     9494 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    25532 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    11452 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    18945 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     8981 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    42865 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    20119 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2091 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mobile.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     3073 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mobile.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    15248 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     6274 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    35500 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    15756 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    14531 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     6719 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    29618 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    12840 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    22490 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    10536 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    21112 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    10651 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     7585 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.trendline.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     4438 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.trendline.min.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    14778 2023-05-04 09:03:31.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot/views.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:36:40.010228 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      570 2023-08-04 13:36:39.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     4197 2023-08-04 13:36:39.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/SOURCES.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-08-04 13:36:39.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/dependency_links.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       42 2023-08-04 13:36:39.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/entry_points.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-05-04 09:06:07.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/not-zip-safe
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-08-04 13:36:39.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/requires.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       16 2023-08-04 13:36:39.000000 cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/top_level.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       38 2023-08-04 13:36:40.062229 cubicweb-jqplot-1.0.0/setup.cfg
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2622 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/setup.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:36:40.058228 cubicweb-jqplot-1.0.0/test/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1015 2023-05-04 09:02:49.000000 cubicweb-jqplot-1.0.0/test/test_jqplot.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1116 2023-08-04 13:26:26.000000 cubicweb-jqplot-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-jqplot-0.5.0/setup.py` & `cubicweb-jqplot-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2016 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2021 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of a cubicweb-jqplot.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -42,15 +42,15 @@
 license = __pkginfo__['license']
 description = __pkginfo__['description']
 web = __pkginfo__['web']
 author = __pkginfo__['author']
 author_email = __pkginfo__['author_email']
 classifiers = __pkginfo__['classifiers']
 
-with open(join(here, 'README')) as f:
+with open(join(here, 'README.rst')) as f:
     long_description = f.read()
 
 # get optional metadatas
 data_files = __pkginfo__.get('data_files', None)
 dependency_links = __pkginfo__.get('dependency_links', ())
 
 requires = {}
```

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot.egg-info/SOURCES.txt` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MANIFEST.in
-README
+README.rst
 setup.py
 tox.ini
 cubicweb_jqplot/__init__.py
 cubicweb_jqplot/__pkginfo__.py
 cubicweb_jqplot/views.py
 cubicweb_jqplot.egg-info/PKG-INFO
 cubicweb_jqplot.egg-info/SOURCES.txt
```

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/__pkginfo__.py` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/__pkginfo__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # pylint: disable=W0622
 """cubicweb-jqplot application packaging information"""
 
 
 modname = 'cubicweb_jqplot'
 distname = 'cubicweb-jqplot'
 
-numversion = (0, 5, 0)
+numversion = (1, 0, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 author = 'LOGILAB S.A. (Paris, FRANCE)'
 author_email = 'contact@logilab.fr'
 description = 'views wrapping jqPlot graphic library'
 web = 'http://www.cubicweb.org/project/%s' % distname
 
-__depends__ = {'cubicweb': '>= 3.24.0'}
+__depends__ = {
+    'cubicweb': '>=4.0.0,<5.0.0',
+    'cubicweb_web': '>=1.0.0,<2.0.0',
+}
 __recommends__ = {}
 
 classifiers = [
     'Environment :: Web Environment',
     'Framework :: CubicWeb',
     'Programming Language :: Python :: 3',
     'Programming Language :: JavaScript',
```

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/views.py` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2011-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2011-2021 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of CubicWeb.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -17,15 +17,15 @@
 # with CubicWeb.  If not, see <http://www.gnu.org/licenses/>.
 """basic plot views based on jqplot (http://www.jqplot.com)
 """
 
 __docformat__ = "restructuredtext en"
 from cubicweb.predicates import multi_columns_rset, match_kwargs
 from cubicweb.utils import json_dumps, JSString, js_dumps
-from cubicweb.view import AnyRsetView
+from cubicweb_web.view import AnyRsetView
 from cubicweb import NoSelectableObject
 from logilab.mtconverter import xml_escape
 from logilab.common.date import datetime2ticks
 from cubicweb import _
 
 
 def filterout_nulls(abscissa, plot):
@@ -178,15 +178,15 @@
             self._cw.add_js('plugins/jqplot.highlighter.js')
             highlighter_ = self.default_highlighter
             if isinstance(highlighter, dict):
                 highlighter_ = highlighter_.copy()
                 highlighter_.update(highlighter)
             highlighter = highlighter_
         axes = axes.copy()
-        for axis, options in axes.iteritems():
+        for axis, options in axes.items():
             if 'renderer' in options:
                 options = options.copy()
                 options['renderer'] = self.renderer(self.axis_renderers,
                                                     options['renderer'])
                 axes[axis] = options
             if 'tickRenderer' in options:
                 options = options.copy()
@@ -303,14 +303,15 @@
         super(JQPlotView, self).call(**kwargs)
 
     def iter_series(self):
         return self.cw_extra_kwargs['series']
 
 
 class JQPlotSimpleView(JQPlotRsetView):
+    __regid__ = 'jqplot.simple'
 
     onload = 'cw.cubes.jqplot.buildPlot("%(id)s", %(data)s, %(options)s);'
     default_legend = {'show': True,
                       'placement': 'e',
                       }
     default_options = {'showDataLabels': True}
     default_renderer = 'bar'
```

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/cubes.jqplot.ext.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/cubes.jqplot.ext.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/MIT-LICENSE.txt` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.css` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.css`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/copyright.txt` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/copyright.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/jquery.jqplot.min.css` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/jquery.jqplot.min.css`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.trendline.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.trendline.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mobile.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mobile.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.json2.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.json2.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidAxisRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.blockRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.logAxisRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.barRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.meterGaugeRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.BezierCurveRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.json2.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.json2.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ohlcRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dragable.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dragable.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.highlighter.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.bubbleRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mobile.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mobile.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasOverlay.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasTextRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoAxisRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.cursor.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.cursor.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.cursor.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.cursor.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pieRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dateAxisRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.mekkoRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.trendline.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.trendline.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.categoryAxisRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.ciParser.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.funnelRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pointLabels.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisTickRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.pyramidGridRenderer.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.enhancedLegendRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.donutRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.canvasAxisLabelRenderer.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/cubicweb_jqplot/data/plugins/jqplot.dragable.min.js` & `cubicweb-jqplot-1.0.0/cubicweb_jqplot/data/plugins/jqplot.dragable.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-jqplot-0.5.0/test/test_jqplot.py` & `cubicweb-jqplot-1.0.0/test/test_jqplot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2012-2021 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

