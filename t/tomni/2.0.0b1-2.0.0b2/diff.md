# Comparing `tmp/tomni-2.0.0b1.tar.gz` & `tmp/tomni-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tomni-2.0.0b1.tar", last modified: Thu Jun 29 12:39:38 2023, max compression
+gzip compressed data, was "dist/tomni-2.0.0b2.tar", last modified: Fri Aug  4 07:48:27 2023, max compression
```

## Comparing `tomni-2.0.0b1.tar` & `tomni-2.0.0b2.tar`

### file list

```diff
@@ -1,258 +1,266 @@
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5709 2023-06-29 12:39:00.000000 tomni-2.0.0b1/HISTORY.rst
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    13065 2023-06-29 12:39:00.000000 tomni-2.0.0b1/LICENSE
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      241 2023-06-29 12:39:00.000000 tomni-2.0.0b1/MANIFEST.in
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    21882 2023-06-29 12:39:38.000000 tomni-2.0.0b1/PKG-INFO
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2451 2023-06-29 12:39:00.000000 tomni-2.0.0b1/README.md
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/docs/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      634 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/Makefile
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      924 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/apidocs.rst
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2214 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/conf.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      471 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/index.rst
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      760 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/make.bat
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      333 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/quickstart.rst
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/docs/tutorials/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2859 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/tutorials/roundness_vs_circularity.rst
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      296 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/tutorials.rst
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      150 2023-06-29 12:39:00.000000 tomni-2.0.0b1/requirements.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      790 2023-06-29 12:39:38.000000 tomni-2.0.0b1/setup.cfg
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1526 2023-06-29 12:39:00.000000 tomni-2.0.0b1/setup.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      666 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      109 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      154 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/annotation/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/annotation/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      955 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/annotation/main.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/binary_mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/binary_mask/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      834 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/binary_mask/main.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7640 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6586 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/test_ellipse.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2764 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/test_ellipse_comparing.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       24 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       82 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      533 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/test_point_comparing.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7582 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    10074 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/test_polygon.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2580 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/test_polygon_comparing.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    12861 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    17618 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/test_annotation_manager.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      232 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      723 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1127 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/test_lines_equal.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       42 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      843 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2640 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/test_compress_polygon_points.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      310 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/main.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       33 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4291 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5955 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/test_overlap_object.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1072 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2798 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/test_polygon_simplify.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1435 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/test_utils.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_fitting/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      131 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2379 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6932 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       66 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1200 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3727 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_operations/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       51 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       37 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      917 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1722 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      172 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       45 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      606 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      538 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/test_get_approx_circle_by_area.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      963 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1962 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/test_circularity.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      519 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      782 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/test_get_center.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      660 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1899 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/test_roundness.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/convert_color/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/convert_color/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2803 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/convert_color/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3934 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/convert_color/test_colorConvert.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      106 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1477 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2487 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/test_absolute_difference.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1832 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      950 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2260 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3410 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/test_ratio_based.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/img_dim/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_dim/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      530 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_dim/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      937 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_dim/test_imgDim.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/img_paste/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_paste/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1756 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_paste/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    14725 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_paste/test_img_paste.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      325 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/add_area/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_area/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      780 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_area/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3132 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_area/test_add_area.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/add_center/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_center/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      434 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_center/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2158 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_center/test_add_center.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      881 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1356 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/test_add_circularity.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/cropping/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/cropping/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4284 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/cropping/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7257 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/cropping/test_crop_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/flipping/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/flipping/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1262 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/flipping/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1036 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/flipping/test_flip_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/rotation/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/rotation/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3397 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/rotation/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4236 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/rotation/test_rotate_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1663 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1785 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/test_scaleResults.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1807 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6663 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/test_summary_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/translation/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       35 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/translation/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1576 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/translation/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1931 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/translation/test_translation_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      200 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       71 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1388 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3163 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/test_circle_mask.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       36 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      949 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5774 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/test_make_mask_contour.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       65 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3275 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    36148 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/test_make_mask_ellipse.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/shape_fitting/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       54 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       42 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      827 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1875 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      573 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1134 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1222 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/test_contour2bbox.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/contours2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contours2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      648 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contours2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1011 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contours2json/test_contours2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      794 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      921 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/test_ellipse2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1902 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4228 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/test_json2bbox.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2contours/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2contours/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      553 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2contours/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1594 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2contours/test_contours2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2dict/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2dict/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1459 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2dict/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4246 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2dict/test_json2dict.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2labels/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2labels/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1296 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2labels/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3120 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2labels/test_json2labels.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2mask/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3160 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2mask/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    12303 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2mask/test_json2mask.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1941 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4183 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/test_json2vgg.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      973 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3877 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/test_labels2contours.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       39 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      578 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/integration_real_data.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      817 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1066 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/test_labels2listsOfPoints.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      603 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1312 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/test_list_of_points2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1642 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5347 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/test_mask2bbox.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/mask2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2811 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    15757 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2json/test_mask2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/positions2contour/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       36 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/positions2contour/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1877 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/positions2contour/main.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1909 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7052 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/test_vgg2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    21882 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/PKG-INFO
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     8601 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/SOURCES.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        1 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/dependency_links.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        1 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/not-zip-safe
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      145 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/requires.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        6 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/top_level.txt
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6479 2023-08-04 07:47:48.000000 tomni-2.0.0b2/HISTORY.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    13065 2023-08-04 07:47:48.000000 tomni-2.0.0b2/LICENSE
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      241 2023-08-04 07:47:48.000000 tomni-2.0.0b2/MANIFEST.in
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    22652 2023-08-04 07:48:27.000000 tomni-2.0.0b2/PKG-INFO
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2451 2023-08-04 07:47:48.000000 tomni-2.0.0b2/README.md
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/docs/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      634 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/Makefile
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      924 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/apidocs.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2214 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/conf.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      471 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/index.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      760 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/make.bat
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      333 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/quickstart.rst
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/docs/tutorials/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2859 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/tutorials/roundness_vs_circularity.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      296 2023-08-04 07:47:48.000000 tomni-2.0.0b2/docs/tutorials.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      150 2023-08-04 07:47:48.000000 tomni-2.0.0b2/requirements.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      790 2023-08-04 07:48:27.000000 tomni-2.0.0b2/setup.cfg
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1526 2023-08-04 07:47:48.000000 tomni-2.0.0b2/setup.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      683 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      109 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      154 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/annotation/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/annotation/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1126 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/annotation/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/binary_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/binary_mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      834 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/binary_mask/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/ellipse/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/ellipse/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    13635 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/ellipse/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    18717 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/ellipse/test_ellipse.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2764 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/ellipse/test_ellipse_comparing.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/point/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       24 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/point/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       82 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/point/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      533 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/point/test_point_comparing.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/polygon/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/polygon/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    14699 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/polygon/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    17803 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/polygon/test_polygon.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2517 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/annotations/polygon/test_polygon_comparing.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    15564 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    53707 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/test_annotation_manager.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      280 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/are_lines_equal/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/are_lines_equal/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      723 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/are_lines_equal/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1127 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/are_lines_equal/test_lines_equal.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/compress_polygon_points/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       42 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/compress_polygon_points/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      959 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/compress_polygon_points/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1221 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/compress_polygon_points/test_compress_polygon_points.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/contours2polygons/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       36 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/contours2polygons/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3509 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/contours2polygons/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7241 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/contours2polygons/test_contours2polygons.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      672 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/overlap_object/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       33 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/overlap_object/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4291 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/overlap_object/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5955 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/overlap_object/test_overlap_object.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/simplify_line/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/simplify_line/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1072 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/simplify_line/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2798 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/simplify_line/test_polygon_simplify.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1435 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/annotation_manager/utils/test_utils.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/bbox_fitting/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      131 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_fitting/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2379 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6932 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting_center/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       66 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting_center/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1200 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting_center/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3727 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/bbox_operations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       51 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_operations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/bbox_operations/check_overlap_bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       37 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_operations/check_overlap_bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      917 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_operations/check_overlap_bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1722 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/contour_operations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      172 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/contour_operations/approximate_circle_by_area/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       45 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/approximate_circle_by_area/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      606 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/approximate_circle_by_area/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      538 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/approximate_circle_by_area/test_get_approx_circle_by_area.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/contour_operations/circularity/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/circularity/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      963 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/circularity/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1962 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/circularity/test_circularity.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/contour_operations/get_center/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/get_center/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      519 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/get_center/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      782 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/get_center/test_get_center.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/contour_operations/roundness/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/roundness/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      660 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/roundness/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1899 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/contour_operations/roundness/test_roundness.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/convert_color/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/convert_color/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2803 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/convert_color/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3934 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/convert_color/test_colorConvert.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/illumination_correction/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      106 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/illumination_correction/absolute_difference/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/absolute_difference/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1477 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/absolute_difference/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2487 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/absolute_difference/test_absolute_difference.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/illumination_correction/fluo_tophat/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/fluo_tophat/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1832 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/fluo_tophat/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      950 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/illumination_correction/relative_difference/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/relative_difference/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2260 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/relative_difference/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3410 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/illumination_correction/relative_difference/test_ratio_based.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/img_dim/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/img_dim/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      530 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/img_dim/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      937 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/img_dim/test_imgDim.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/img_paste/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/img_paste/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1756 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/img_paste/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    14725 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/img_paste/test_img_paste.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      325 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/add_area/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_area/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      780 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_area/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3132 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_area/test_add_area.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/add_center/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_center/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      434 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_center/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2158 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_center/test_add_center.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/add_circularity/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_circularity/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      881 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_circularity/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1356 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/add_circularity/test_add_circularity.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/cropping/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/cropping/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4284 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/cropping/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7257 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/cropping/test_crop_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/flipping/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/flipping/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1262 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/flipping/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1036 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/flipping/test_flip_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/rotation/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/rotation/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3397 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/rotation/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4236 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/rotation/test_rotate_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/scale_json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/scale_json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1663 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/scale_json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1785 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/scale_json/test_scaleResults.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/summary_json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/summary_json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1807 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/summary_json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6663 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/summary_json/test_summary_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/json_operations/translation/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       35 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/translation/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1576 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/translation/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1931 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/json_operations/translation/test_translation_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/make_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      200 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/make_mask/circlair_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       71 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/circlair_mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1388 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/circlair_mask/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3163 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/circlair_mask/test_circle_mask.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/make_mask/contour_mask_maker/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       36 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/contour_mask_maker/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      949 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/contour_mask_maker/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5774 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/contour_mask_maker/test_make_mask_contour.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/make_mask/ellipse_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       65 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/ellipse_mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3275 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/ellipse_mask/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    36148 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/make_mask/ellipse_mask/test_make_mask_ellipse.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/shape_fitting/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       54 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/shape_fitting/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/shape_fitting/fit_rect_ellipse/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       42 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/shape_fitting/fit_rect_ellipse/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      827 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/shape_fitting/fit_rect_ellipse/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1875 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      663 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/binary2contours/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/binary2contours/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1719 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/binary2contours/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5727 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/binary2contours/test_binary2contours.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/contour2bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/contour2bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1134 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/contour2bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1222 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/contour2bbox/test_contour2bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/contours2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/contours2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      648 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/contours2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1011 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/contours2json/test_contours2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/ellipse2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/ellipse2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      794 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/ellipse2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      921 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/ellipse2json/test_ellipse2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/json2bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1902 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4228 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2bbox/test_json2bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/json2contours/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2contours/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      553 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2contours/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1594 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2contours/test_contours2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/json2dict/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2dict/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1459 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2dict/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4246 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2dict/test_json2dict.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/json2labels/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2labels/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1296 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2labels/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3120 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2labels/test_json2labels.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/json2mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3160 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2mask/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    12303 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2mask/test_json2mask.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/json2vgg/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2vgg/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1941 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2vgg/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4183 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/json2vgg/test_json2vgg.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/labels2contours/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/labels2contours/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      973 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/labels2contours/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3877 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/labels2contours/test_labels2contours.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       39 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      578 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/integration_real_data.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      817 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1066 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/test_labels2listsOfPoints.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/list_of_points2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/list_of_points2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      603 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/list_of_points2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1312 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/list_of_points2json/test_list_of_points2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/mask2bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/mask2bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1642 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/mask2bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5347 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/mask2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/mask2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2811 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/mask2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    15757 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/mask2json/test_mask2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/positions2contour/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       36 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/positions2contour/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1877 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/positions2contour/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni/transformers/vgg2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/vgg2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1909 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/vgg2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7052 2023-08-04 07:47:48.000000 tomni-2.0.0b2/tomni/transformers/vgg2json/test_vgg2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni.egg-info/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    22652 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni.egg-info/PKG-INFO
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     8943 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        1 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        1 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni.egg-info/not-zip-safe
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      145 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni.egg-info/requires.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        6 2023-08-04 07:48:27.000000 tomni-2.0.0b2/tomni.egg-info/top_level.txt
```

### Comparing `tomni-2.0.0b1/HISTORY.rst` & `tomni-2.0.0b2/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # History
 
+2.0.0-b2 (2023-08-04) 
+- Moved feature_multiplier and metric_unit to to_dict() from from_dict(). 
+- Added inner contours options 
+- added binary2contours
+- change parameters for from_binary_mask
+- made contours2polygon
+- test
+
+2.0.0-b1 (2023-07-06)
+------------------
+- AnnotationManager function from_dict is called with an optional list of features
+- Changed Polygon and Ellipse classes to include the list of features initialized by AnnotationManager
+- to_dict function now only returns features in the dictionary that were asked for in the feature list
+- Added `feature_multiplier` and `metric_unit` as inputs to apply to the features' name and value outputs.
+- Added all features to `ellipse` and `polygon`.
+- Features are now in camelCasing when output `to_dict`
+
 2.0.0-b0 (2022-11-29)
 ------------------
 - CDF-Main: Implement `filter` to allow filtering of annotations by feature values (aka gating).
 - CDF-Main: Implement `from_contours`.
 - CDF-Main: Implement `to_contours`.
 - CDF-Main: Implement `from_dict`.
 - CDF-Main: Implement `to_dict`. Includes rounding.
```

### Comparing `tomni-2.0.0b1/LICENSE` & `tomni-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/PKG-INFO` & `tomni-2.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomni
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Tomni is a collection of image analysis functions usefull for CytoSmart solution.
 Home-page: https://github.com/cytosmart-bv/tomni
 Author: Tom Nijhof
 License: ACADEMIC PUBLIC LICENSE
 Keywords: tomni
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -94,14 +94,31 @@
 - Marina Tzenkova
 - Tom de Vries
 - Tom Nijhof
 
 
 # History
 
+2.0.0-b2 (2023-08-04) 
+- Moved feature_multiplier and metric_unit to to_dict() from from_dict(). 
+- Added inner contours options 
+- added binary2contours
+- change parameters for from_binary_mask
+- made contours2polygon
+- test
+
+2.0.0-b1 (2023-07-06)
+------------------
+- AnnotationManager function from_dict is called with an optional list of features
+- Changed Polygon and Ellipse classes to include the list of features initialized by AnnotationManager
+- to_dict function now only returns features in the dictionary that were asked for in the feature list
+- Added `feature_multiplier` and `metric_unit` as inputs to apply to the features' name and value outputs.
+- Added all features to `ellipse` and `polygon`.
+- Features are now in camelCasing when output `to_dict`
+
 2.0.0-b0 (2022-11-29)
 ------------------
 - CDF-Main: Implement `filter` to allow filtering of annotations by feature values (aka gating).
 - CDF-Main: Implement `from_contours`.
 - CDF-Main: Implement `to_contours`.
 - CDF-Main: Implement `from_dict`.
 - CDF-Main: Implement `to_dict`. Includes rounding.
```

### Comparing `tomni-2.0.0b1/README.md` & `tomni-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/docs/Makefile` & `tomni-2.0.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/docs/apidocs.rst` & `tomni-2.0.0b2/docs/apidocs.rst`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/docs/conf.py` & `tomni-2.0.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/docs/make.bat` & `tomni-2.0.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/docs/tutorials/roundness_vs_circularity.rst` & `tomni-2.0.0b2/docs/tutorials/roundness_vs_circularity.rst`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/setup.cfg` & `tomni-2.0.0b2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.0b1
+current_version = 2.0.0b2
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)((?P<release>[a-z])(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `tomni-2.0.0b1/setup.py` & `tomni-2.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords="tomni",
     name="tomni",
     packages=find_packages(include=["tomni*"], exclude=["docs*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cytosmart-bv/tomni",
-    version="2.0.0b1",
+    version="2.0.0b2",
     zip_safe=False,
 )
```

### Comparing `tomni-2.0.0b1/tomni/__init__.py` & `tomni-2.0.0b2/tomni/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # -*- coding: utf-8 -*-
 """Tomni is a collection of image analysis functions useful for CytoSmart solution."""
 
 __author__ = """Tom Nijhof & Jelle van Kerkvoorde"""
 __email__ = "tom.nijhof@cytosmart.com"
-__version__ = "2.0.0b1"
+__version__ = "2.0.0b2"
 
 from .bbox_fitting import bbox_fitting, bbox_fitting_center
 from .bbox_operations import check_overlap_bbox
 from .convert_color import convert_color
-from .illumination_correction import absolute_difference, fluo_tophat, relative_difference
+from .illumination_correction import (
+    absolute_difference,
+    fluo_tophat,
+    relative_difference,
+)
 from .img_dim import img_dim
 from .img_paste import img_paste
 from .json_operations import *
 from .make_mask import *
 from .shape_fitting import fit_rect_around_ellipse
 from .transformers import *
```

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/annotations/annotation/main.py` & `tomni-2.0.0b2/tomni/annotation_manager/annotations/annotation/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from abc import ABC, abstractmethod
 from typing import List
 
 
 class Annotation(ABC):
-    def __init__(self, id: str, label: str, children: List, parents: List) -> None:
+    def __init__(
+        self, id: str, label: str, children: List, parents: List, accuracy: float
+    ) -> None:
         self._id: str = id
         self._label: str = label
         self._children: List[Annotation] = children
         self._parents: List[Annotation] = parents
+        self._accuracy: float = accuracy
 
     @abstractmethod
     def to_dict(self, decimals: int = 2, **kwargs) -> dict:
         """Creates a dictionary in CDF of annotation.
         Args:
             decimals (int, optional): The number of decimals to use when rounding. Defaults to 2.
 
         Returns:
             dict: CytoSmart Data Format dict.
         """
-        return {"id": self._id, "label": self._label, "children": self._children, "parents": self._parents}
+        return {
+            "id": self._id,
+            "label": self._label,
+            "children": self._children,
+            "parents": self._parents,
+            "accuracy": self._accuracy,
+        }
 
     @property
     @abstractmethod
     def label(self) -> str:
         return self._label
 
     @label.setter
```

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/annotations/binary_mask/main.py` & `tomni-2.0.0b2/tomni/annotation_manager/annotations/binary_mask/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/test_ellipse_comparing.py` & `tomni-2.0.0b2/tomni/annotation_manager/annotations/ellipse/test_ellipse_comparing.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/annotations/point/test_point_comparing.py` & `tomni-2.0.0b2/tomni/annotation_manager/annotations/point/test_point_comparing.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/main.py` & `tomni-2.0.0b2/tomni/annotation_manager/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import uuid
 from typing import Dict, List, Tuple, Union
 
 import cv2
 import numpy as np
 
-from tomni.transformers import labels2listsOfPoints, positions2contour
-
+from tomni.annotation_manager.utils.contours2polygons import contours2polygons
 from .annotations import Annotation, Ellipse, Point, Polygon
 from .utils import parse_points_to_contour
 
+MIN_NR_POINTS_POLYGON = 5
+
 
 class AnnotationManager(object):
     def __init__(self, annotations: List[Annotation]):
         """Initializes a AnnotationManager object.
 
         Args:
             annotations (List[Annotation]): Collection of annotations, e.g. polygon or ellipse.
         """
         self._annotations = annotations
 
     @classmethod
-    def from_dicts(cls, dicts: List[dict]):
+    def from_dicts(
+        cls,
+        dicts: List[dict],
+    ):
         TYPE_KEY = "type"
         LABEL_KEY = "label"
         CHILDREN_KEY = "children"
         PARENTS_KEY = "parents"
         ID_KEY = "id"
         CENTER_KEY = "center"
         annotations = []
@@ -36,111 +40,143 @@
                     id=d.get(ID_KEY, str(uuid.uuid4())),
                     children=d.get(CHILDREN_KEY, []),
                     parents=d.get(PARENTS_KEY, []),
                     radius_x=d["radiusX"],
                     radius_y=d.get("radiusY", None),
                     center=Point(x=d[CENTER_KEY]["x"], y=d[CENTER_KEY]["y"]),
                     rotation=d["angleOfRotation"],
+                    accuracy=d.get("accuracy", 1),
                 )
             elif d[TYPE_KEY] == "polygon":
+                if len(d["points"]) < MIN_NR_POINTS_POLYGON:
+                    continue
+                if "inner_points" in d:
+                    inner_points = [
+                        [Point(x=pi["x"], y=pi["y"]) for pi in inner_contour]
+                        for inner_contour in d["inner_points"]
+                    ]
+                else:
+                    inner_points = []
+
                 annotation = Polygon(
                     label=d.get(LABEL_KEY, None),
                     id=d.get(ID_KEY, str(uuid.uuid4())),
                     children=d.get(CHILDREN_KEY, []),
                     parents=d.get(PARENTS_KEY, []),
                     points=[Point(x=p["x"], y=p["y"]) for p in d["points"]],
+                    inner_points=inner_points,
+                    accuracy=d.get("accuracy", 1),
                 )
             else:
-                raise ValueError(f"CDF cannot be created. Dict with id {d.get('id', None)} misses type-key with value ellipse or polygon.")
+                raise ValueError(
+                    f"CDF cannot be created. Dict with id {d.get('id', None)} misses type-key with value ellipse or polygon."
+                )
             annotations.append(annotation)
 
         return cls(annotations)
 
     @classmethod
-    def from_contours(cls, contours: List[np.ndarray]):
-        """Initializes a AnnotationManager object from cv2 contours.
-        Contours' shape must be [N, 1, 2] with dtype of np.int32.
-
-        Args:
-            contours (List[np.ndarray]): Collection of cv2 contours.
-        """
-        annotations = []
-        for contour in contours:
-            # change shape from [N, 1, 2] to [N, 2]
-            contour = np.vstack(contour)
-
-            points: List[Point] = []
-            for i in range(contour.shape[0]):
-                points.append(Point(x=int(contour[i][0]), y=int(contour[i][1])))
-
-            annotations.append(Polygon(label="", id=str(uuid.uuid4()), children=[], parents=[], points=points))
-
-        return cls(annotations)
-
-    @classmethod
-    def from_binary_mask(cls, mask: np.ndarray, connectivity: int = 8):
+    def from_binary_mask(
+        cls, mask: np.ndarray, include_inner_contours: bool = False, label: str = ""
+    ):
         """Initializes a AnnotationManager object from a binary mask.
-        Binary mask can contain either 0 and 1 or 0 and 255.
 
         Args:
             mask (np.ndarray): Binary mask input.
-            connectivity (int): When deriving connected components connectivy determines how diagonally components are handled.
-                `8` allows for diagonally connected components to be merged, while 4 does not. In the example below `8`-connectivity
-                will treat the ones as the same object while 4 treats them as seperate two distinct components.
-                Example:
-                    [[1,0],
-                    [0,1]]
-
+            include_inner_contours (bool, optional): Include annotations that are contained within another annotation.
+                Defaults to False.
         Returns:
             AnnotationManager: New annotation manager object from binary mask.
         """
+
         unique_values = np.unique(mask)
         assert np.array_equal(unique_values, np.array([0, 1])) or np.array_equal(
             unique_values, np.array([0, 255])
         ), "A binary mask must contain either 0 and 1 or 0 and 255 only."
         mask = mask.astype(np.uint8)
 
-        _, labeled_mask = cv2.connectedComponents(mask, connectivity=connectivity)
-
-        padded_mask = cv2.copyMakeBorder(mask, top=1, bottom=1, left=1, right=1, borderType=cv2.BORDER_CONSTANT, value=0)
-
-        # If bin mask with 0's and 1's is input then canny fails, so multiply by 255 and clip.
-        if padded_mask.max() == 1:
-            padded_mask = padded_mask * 255
-        edges = cv2.Canny(padded_mask, 50, 150)
+        mode = cv2.RETR_CCOMP if include_inner_contours else cv2.RETR_EXTERNAL
+        contours, hierarchy = cv2.findContours(mask, mode, cv2.CHAIN_APPROX_SIMPLE)
 
-        edges = cv2.dilate(edges, np.ones((5, 5)))
-        edges = np.divide(edges, 255, dtype=np.float16)
-        edges = edges.astype(np.uint8)
-        edges = edges[1:-1, 1:-1]
+        annotations = contours2polygons(
+            contours=contours,
+            hierarchy=hierarchy,
+            include_inner_contours=include_inner_contours,
+            label=label,
+        )
 
-        edged_mask = edges * labeled_mask
-
-        return AnnotationManager.from_labeled_mask(edged_mask)
+        return cls(annotations)
 
     @classmethod
-    def from_labeled_mask(cls, mask: np.ndarray, include_inner_contours: bool = False):
+    def from_labeled_mask(
+        cls,
+        mask: np.ndarray,
+        labels: Union[List[str], str] = "",
+        include_inner_contours: bool = False,
+    ):
         """Initializes a AnnotationManager object from a labeled mask.
         A labeled mask contains components indicated by the same pixel values (see example below).
 
         Example containing two components yielding a AnnotationManager object with two annotations:
         [[0,0,2,1,1],
         [0,0,2,0,0],
         [0,0,2,0,]]
 
         Args:
             mask (np.ndarray): A labeled mask with a max. nr. of components limited by max(np.uint32).
-            include_inner_contours (bool, optional): Include annotations that are contained within another annotation. Defaults to False.
-
+            classes(List[str], optional): A list of class names to add to Polygon labels. Defaults to None.
+                Should have the same number of unique pixel values as classes.
+                Class names in order of low pixel value to high pixel value.
+            include_inner_contours (bool, optional): Include annotations that are contained within another annotation.
+                Defaults to False.
         Returns:
             AnnotationManager: A new AnnotationManager object.
         """
-        points = labels2listsOfPoints(mask)
-        contours = [positions2contour(point, return_inner_contours=include_inner_contours) for point in points if len(point) > 0]
-        return AnnotationManager.from_contours(contours)
+        mode = cv2.RETR_CCOMP if include_inner_contours else cv2.RETR_EXTERNAL
+
+        if isinstance(labels, str):
+            mask = mask.astype(np.uint8)
+            _, mask = cv2.threshold(mask, 0, 255, cv2.THRESH_BINARY)
+            contours, hierarchy = cv2.findContours(mask, mode, cv2.CHAIN_APPROX_SIMPLE)
+
+            annotations = contours2polygons(
+                contours=contours,
+                include_inner_contours=include_inner_contours,
+                hierarchy=hierarchy,
+                label=labels,
+            )
+
+        elif isinstance(labels, List):
+            unique_values = np.unique(mask)
+            unique_values = unique_values[unique_values != 0]
+
+            if len(labels) < len(unique_values):
+                raise ValueError(
+                    f"Not enough labels for unique pixel values. {len(labels)} labels for {len(unique_values)} unique pixel values."
+                )
+
+            annotations = []
+            # Generate seperate mask for each class and find contours.
+            for pixel_value in unique_values:
+                class_mask = np.uint8(mask == pixel_value)
+                contours, hierarchy = cv2.findContours(
+                    class_mask, mode, cv2.CHAIN_APPROX_SIMPLE
+                )
+                annotations.extend(
+                    contours2polygons(
+                        contours=contours,
+                        hierarchy=hierarchy,
+                        include_inner_contours=include_inner_contours,
+                        label=labels[pixel_value - 1],
+                    )
+                )
+        else:
+            raise ValueError("Labels must be either a string or a list of strings.")
+
+        return cls(annotations)
 
     @classmethod
     def from_darwin(cls, dicts: List[dict]):
         """must be an option"""
         pass
 
     @property
@@ -175,47 +211,89 @@
         if self.idx < self.__len__():
             annotation = self.annotations[self.idx]
             self.idx += 1
             return annotation
         else:
             raise StopIteration
 
-    def to_dict(self, decimals: int = 2, mask_json: Union[dict, None] = None, min_overlap: float = 0.9, **kwargs) -> List[Dict]:
+    def to_dict(
+        self,
+        decimals: int = 2,
+        mask_json: Union[List[dict], None] = None,
+        min_overlap: float = 0.9,
+        features: Union[List[str], None] = None,
+        metric_unit: str = "",
+        feature_multiplier: int = 1,
+        **kwargs,
+    ) -> List[Dict]:
         """Transform AM object to a collection of our format.
 
         Args:
             decimals (int, optional): The number of decimals to use when rounding. Defaults to 2.
             mask_json (Union[dict, None], optional): The dict mask that indicates what area to include in the output dict.
-            Defaults to None.
+                Defaults to None.
             min_overlap (float, optional): Minimum overlap required between the polygon and the mask, expressed as a value between 0 and 1
-            Defaults to 0.9.
+                Defaults to 0.9.
+            features (Union[List[str], None], optional): The features that you want to calculate and add to the dict objects.
+                Defaults to None, which returns all features.
+            metric_unit (str, optional): The suffix you want to add to the dict keys' names in camelCasing. Defaults to "".
+            feature_multiplier (int, optional): A multiplier used during feature calculation. For example 1/742. Defaults to 1.
+
         Returns:
-            List[Dict]: Collection of dicts.
+            List[Dict]: Output is a list of dicts in cytosmart format.
         """
+
         if mask_json is not None:
             filtered_annotations = self._annotations.copy()
-            filtered_annotations = [annotation for annotation in filtered_annotations if annotation.is_in_mask(mask_json, min_overlap)]
-
-            return [annotation.to_dict(decimals=decimals, **kwargs) for annotation in filtered_annotations]
+            filtered_annotations = [
+                annotation
+                for annotation in filtered_annotations
+                if annotation.is_in_mask(mask_json, min_overlap)
+            ]
+
+            return [
+                annotation.to_dict(
+                    decimals=decimals,
+                    features=features,
+                    metric_unit=metric_unit,
+                    feature_multiplier=feature_multiplier,
+                    **kwargs,
+                )
+                for annotation in filtered_annotations
+            ]
 
-        return [annotation.to_dict(decimals=decimals, **kwargs) for annotation in self._annotations]
+        return [
+            annotation.to_dict(
+                decimals=decimals,
+                features=features,
+                metric_unit=metric_unit,
+                feature_multiplier=feature_multiplier,
+                **kwargs,
+            )
+            for annotation in self._annotations
+        ]
 
     def to_contours(self) -> List[np.ndarray]:
         """Transform AM object to a collection of cv2 contours.
 
         Raises:
             ValueError: Raises error when annotations are not of type `Polygon`.
 
         Returns:
             List[np.ndarray]: Collection of contours as [[[x_0, y_0],..., [x_n, y_n]], ... ,[[x_0, y_0],..., [x_m, y_m]]]
         """
-        if not all([isinstance(annotation, Polygon) for annotation in self._annotations]):
+        if not all(
+            [isinstance(annotation, Polygon) for annotation in self._annotations]
+        ):
             raise ValueError("`to_contours is only supported on polygon-annotations.`")
 
-        contours = [parse_points_to_contour(annotation.points) for annotation in self._annotations]
+        contours = [
+            parse_points_to_contour(annotation.points)
+            for annotation in self._annotations
+        ]
 
         return contours
 
     def to_binary_mask(self, shape: Tuple[int, int]) -> np.ndarray:
         """Transform an AM object to a binary mask.
         Annotations can only be polygon or ellipse.
 
@@ -241,29 +319,33 @@
             np.ndarray: A new labeled mask.
         """
         mask = np.zeros(shape, dtype=np.uint8)
         label_color = 1
 
         for annotation in self._annotations:
             if isinstance(annotation, Polygon):
-                points = np.array([[point.x, point.y] for point in annotation.points], dtype=np.int32)
+                points = np.array(
+                    [[point.x, point.y] for point in annotation.points], dtype=np.int32
+                )
                 cv2.fillPoly(mask, [points], color=label_color)
             elif isinstance(annotation, Ellipse):
                 cv2.ellipse(
                     mask,
                     center=(annotation.center.x, annotation.center.y),
                     axes=(annotation.radius_x, annotation.radius_y),
                     angle=annotation.rotation,
                     startAngle=0,
                     endAngle=360,
                     color=label_color,
                     thickness=-1,
                 )
             else:
-                raise TypeError("Innapropiate annotation type for `to_labeled_mask`. Supported annotations are ellipse and polygon.")
+                raise TypeError(
+                    "Innapropiate annotation type for `to_labeled_mask`. Supported annotations are ellipse and polygon."
+                )
 
             # increase color for every annotation.
             label_color += 1
 
         return mask
 
     def to_darwin(self) -> List[Dict]:
@@ -293,29 +375,38 @@
 
     def delete_annotation(self, item: Annotation):
         """Remove an annotation from self.annotations.
         Find and delete.
         """
         pass
 
-    def filter(self, feature: str, min_val: float, max_val: float, inplace: bool = False):
+    def filter(
+        self,
+        feature: str,
+        min_val: float,
+        max_val: float,
+        feature_multiplier: int = 1,
+        inplace: bool = False,
+    ):
         """Filter annotations by feature.
 
         Args:
             feature (str): Feature name, i.e. `roundness` or `area`.
             min_val (float): Minimum value to threshold.
             max_val (float): Maximum value to threshold
+            feature_multiplier (int, optional): A multiplier used in the feature calculations. For example 1/742. Defaults to 1.
             inplace (bool, optional): If True, filter in-place. Modifies the object internally. If False, return collection of annotations. Defaults to False.
 
         Returns:
             AnnotationManager or List[Annotation]: Collection of filtered annotions or if `inplace=True` object with filterd annotations.
         """
         filtered_annotations = []
 
         for annotation in self._annotations:
+            annotation._feature_multiplier = feature_multiplier
             feature_value = getattr(annotation, feature)
             if min_val <= feature_value <= max_val:
                 filtered_annotations.append(annotation)
 
         if inplace:
             self._annotations = filtered_annotations
             return self
@@ -331,8 +422,12 @@
 
         This is not ideal and i am for suggestion. I want to avoid having to calculate over and over.
         """
         circularity = []
         for cdf_item in self._cdf_data:
             circularity.append(cdf_item.circularity)
 
-        return {"circularity": {"avg": 1, "std": 1, "min": 1, "max": 1}, "...": "...", "feature_n": {"avg_n": 1, "std_n": 1, "min_n": 1, "max_n": 1}}
+        return {
+            "circularity": {"avg": 1, "std": 1, "min": 1, "max": 1},
+            "...": "...",
+            "feature_n": {"avg_n": 1, "std_n": 1, "min_n": 1, "max_n": 1},
+        }
```

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/main.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/are_lines_equal/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/test_lines_equal.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/are_lines_equal/test_lines_equal.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/main.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/compress_polygon_points/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from simplification.cutil import simplify_coords
 from typing import List
 from tomni.annotation_manager.annotations.point import Point
 
 
-def compress_polygon_points(points: List[Point], epsilon: float = 3.0):
+def compress_polygon_points(
+    points: List[Point], epsilon: float = 3.0, min_number_of_points: int = 5
+):
     """Compresses the polygon
 
     Args:
         points (List): The points of the polygon
         epsilon (float, optional): Epsilon value in Ramer-Douglas-Peucker algorithm. The smaller the epsilon, the more points are kept and the more faithful the simplified curve is to the original one.
         Defaults to 3.0.
 
     Returns:
         _type_: A list of 2D points, each represented as an instance of the `Point` class.
     """
     assert epsilon >= 0
 
     point_arr = [[point.x, point.y] for point in points]
     point_arr_compressed = simplify_coords(point_arr, epsilon)
+    if len(point_arr_compressed) < min_number_of_points:
+        return points
     return [Point(x, y) for (x, y) in point_arr_compressed]
```

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/main.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/overlap_object/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/test_overlap_object.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/overlap_object/test_overlap_object.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/main.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/simplify_line/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/test_polygon_simplify.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/simplify_line/test_polygon_simplify.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/annotation_manager/utils/test_utils.py` & `tomni-2.0.0b2/tomni/annotation_manager/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/main.py` & `tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py` & `tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/main.py` & `tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting_center/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py` & `tomni-2.0.0b2/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/main.py` & `tomni-2.0.0b2/tomni/bbox_operations/check_overlap_bbox/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py` & `tomni-2.0.0b2/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/main.py` & `tomni-2.0.0b2/tomni/contour_operations/approximate_circle_by_area/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/test_get_approx_circle_by_area.py` & `tomni-2.0.0b2/tomni/contour_operations/approximate_circle_by_area/test_get_approx_circle_by_area.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/circularity/main.py` & `tomni-2.0.0b2/tomni/contour_operations/circularity/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/circularity/test_circularity.py` & `tomni-2.0.0b2/tomni/contour_operations/circularity/test_circularity.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/get_center/main.py` & `tomni-2.0.0b2/tomni/contour_operations/get_center/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/get_center/test_get_center.py` & `tomni-2.0.0b2/tomni/contour_operations/get_center/test_get_center.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/roundness/main.py` & `tomni-2.0.0b2/tomni/contour_operations/roundness/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/contour_operations/roundness/test_roundness.py` & `tomni-2.0.0b2/tomni/contour_operations/roundness/test_roundness.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/convert_color/main.py` & `tomni-2.0.0b2/tomni/convert_color/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/convert_color/test_colorConvert.py` & `tomni-2.0.0b2/tomni/convert_color/test_colorConvert.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/main.py` & `tomni-2.0.0b2/tomni/illumination_correction/absolute_difference/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/test_absolute_difference.py` & `tomni-2.0.0b2/tomni/illumination_correction/absolute_difference/test_absolute_difference.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/main.py` & `tomni-2.0.0b2/tomni/illumination_correction/fluo_tophat/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py` & `tomni-2.0.0b2/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/illumination_correction/relative_difference/main.py` & `tomni-2.0.0b2/tomni/illumination_correction/relative_difference/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/illumination_correction/relative_difference/test_ratio_based.py` & `tomni-2.0.0b2/tomni/illumination_correction/relative_difference/test_ratio_based.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/img_dim/main.py` & `tomni-2.0.0b2/tomni/img_dim/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/img_dim/test_imgDim.py` & `tomni-2.0.0b2/tomni/img_dim/test_imgDim.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/img_paste/main.py` & `tomni-2.0.0b2/tomni/img_paste/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/img_paste/test_img_paste.py` & `tomni-2.0.0b2/tomni/img_paste/test_img_paste.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/add_area/main.py` & `tomni-2.0.0b2/tomni/json_operations/add_area/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/add_area/test_add_area.py` & `tomni-2.0.0b2/tomni/json_operations/add_area/test_add_area.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/add_center/test_add_center.py` & `tomni-2.0.0b2/tomni/json_operations/add_center/test_add_center.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/add_circularity/main.py` & `tomni-2.0.0b2/tomni/json_operations/add_circularity/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/add_circularity/test_add_circularity.py` & `tomni-2.0.0b2/tomni/json_operations/add_circularity/test_add_circularity.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/cropping/main.py` & `tomni-2.0.0b2/tomni/json_operations/cropping/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/cropping/test_crop_json.py` & `tomni-2.0.0b2/tomni/json_operations/cropping/test_crop_json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/flipping/main.py` & `tomni-2.0.0b2/tomni/json_operations/flipping/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/flipping/test_flip_json.py` & `tomni-2.0.0b2/tomni/json_operations/flipping/test_flip_json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/rotation/main.py` & `tomni-2.0.0b2/tomni/json_operations/rotation/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/rotation/test_rotate_json.py` & `tomni-2.0.0b2/tomni/json_operations/rotation/test_rotate_json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/scale_json/main.py` & `tomni-2.0.0b2/tomni/json_operations/scale_json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/scale_json/test_scaleResults.py` & `tomni-2.0.0b2/tomni/json_operations/scale_json/test_scaleResults.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/summary_json/main.py` & `tomni-2.0.0b2/tomni/json_operations/summary_json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/summary_json/test_summary_json.py` & `tomni-2.0.0b2/tomni/json_operations/summary_json/test_summary_json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/translation/main.py` & `tomni-2.0.0b2/tomni/json_operations/translation/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/json_operations/translation/test_translation_json.py` & `tomni-2.0.0b2/tomni/json_operations/translation/test_translation_json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/make_mask/circlair_mask/main.py` & `tomni-2.0.0b2/tomni/make_mask/circlair_mask/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/make_mask/circlair_mask/test_circle_mask.py` & `tomni-2.0.0b2/tomni/make_mask/circlair_mask/test_circle_mask.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/main.py` & `tomni-2.0.0b2/tomni/make_mask/contour_mask_maker/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/test_make_mask_contour.py` & `tomni-2.0.0b2/tomni/make_mask/contour_mask_maker/test_make_mask_contour.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/make_mask/ellipse_mask/main.py` & `tomni-2.0.0b2/tomni/make_mask/ellipse_mask/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/make_mask/ellipse_mask/test_make_mask_ellipse.py` & `tomni-2.0.0b2/tomni/make_mask/ellipse_mask/test_make_mask_ellipse.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/main.py` & `tomni-2.0.0b2/tomni/shape_fitting/fit_rect_ellipse/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py` & `tomni-2.0.0b2/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/__init__.py` & `tomni-2.0.0b2/tomni/transformers/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,12 +4,14 @@
 from .json2bbox import json2bbox
 from .json2contours import json2contours
 from .json2dict import json2dict
 from .json2labels import json2labels
 from .json2mask import json2mask
 from .json2vgg import json2vgg
 from .labels2contours import labels2contours
+from .binary2contours import binary2contours
 from .labels2listsOfPoints import labels2listsOfPoints
 from .mask2bbox import mask2bbox
 from .mask2json import mask2json
 from .positions2contour import positions2contour
 from .vgg2json import vgg2json
+from .binary2contours import binary2contours
```

### Comparing `tomni-2.0.0b1/tomni/transformers/contour2bbox/main.py` & `tomni-2.0.0b2/tomni/transformers/contour2bbox/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/contour2bbox/test_contour2bbox.py` & `tomni-2.0.0b2/tomni/transformers/contour2bbox/test_contour2bbox.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/contours2json/main.py` & `tomni-2.0.0b2/tomni/transformers/contours2json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/contours2json/test_contours2json.py` & `tomni-2.0.0b2/tomni/transformers/contours2json/test_contours2json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/ellipse2json/main.py` & `tomni-2.0.0b2/tomni/transformers/ellipse2json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/ellipse2json/test_ellipse2json.py` & `tomni-2.0.0b2/tomni/transformers/ellipse2json/test_ellipse2json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2bbox/main.py` & `tomni-2.0.0b2/tomni/transformers/json2bbox/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2bbox/test_json2bbox.py` & `tomni-2.0.0b2/tomni/transformers/json2bbox/test_json2bbox.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2contours/main.py` & `tomni-2.0.0b2/tomni/transformers/json2contours/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2contours/test_contours2json.py` & `tomni-2.0.0b2/tomni/transformers/json2contours/test_contours2json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2dict/main.py` & `tomni-2.0.0b2/tomni/transformers/json2dict/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2dict/test_json2dict.py` & `tomni-2.0.0b2/tomni/transformers/json2dict/test_json2dict.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2labels/main.py` & `tomni-2.0.0b2/tomni/transformers/json2labels/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2labels/test_json2labels.py` & `tomni-2.0.0b2/tomni/transformers/json2labels/test_json2labels.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2mask/main.py` & `tomni-2.0.0b2/tomni/transformers/json2mask/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2mask/test_json2mask.py` & `tomni-2.0.0b2/tomni/transformers/json2mask/test_json2mask.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2vgg/main.py` & `tomni-2.0.0b2/tomni/transformers/json2vgg/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/json2vgg/test_json2vgg.py` & `tomni-2.0.0b2/tomni/transformers/json2vgg/test_json2vgg.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/labels2contours/main.py` & `tomni-2.0.0b2/tomni/transformers/labels2contours/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/labels2contours/test_labels2contours.py` & `tomni-2.0.0b2/tomni/transformers/labels2contours/test_labels2contours.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/integration_real_data.py` & `tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/integration_real_data.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/main.py` & `tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/test_labels2listsOfPoints.py` & `tomni-2.0.0b2/tomni/transformers/labels2listsOfPoints/test_labels2listsOfPoints.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/list_of_points2json/main.py` & `tomni-2.0.0b2/tomni/transformers/list_of_points2json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/list_of_points2json/test_list_of_points2json.py` & `tomni-2.0.0b2/tomni/transformers/list_of_points2json/test_list_of_points2json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/mask2bbox/main.py` & `tomni-2.0.0b2/tomni/transformers/mask2bbox/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/mask2bbox/test_mask2bbox.py` & `tomni-2.0.0b2/tomni/transformers/mask2bbox/test_mask2bbox.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/mask2json/main.py` & `tomni-2.0.0b2/tomni/transformers/mask2json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/mask2json/test_mask2json.py` & `tomni-2.0.0b2/tomni/transformers/mask2json/test_mask2json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/positions2contour/main.py` & `tomni-2.0.0b2/tomni/transformers/positions2contour/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/vgg2json/main.py` & `tomni-2.0.0b2/tomni/transformers/vgg2json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni/transformers/vgg2json/test_vgg2json.py` & `tomni-2.0.0b2/tomni/transformers/vgg2json/test_vgg2json.py`

 * *Files identical despite different names*

### Comparing `tomni-2.0.0b1/tomni.egg-info/PKG-INFO` & `tomni-2.0.0b2/tomni.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomni
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Tomni is a collection of image analysis functions usefull for CytoSmart solution.
 Home-page: https://github.com/cytosmart-bv/tomni
 Author: Tom Nijhof
 License: ACADEMIC PUBLIC LICENSE
 Keywords: tomni
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -94,14 +94,31 @@
 - Marina Tzenkova
 - Tom de Vries
 - Tom Nijhof
 
 
 # History
 
+2.0.0-b2 (2023-08-04) 
+- Moved feature_multiplier and metric_unit to to_dict() from from_dict(). 
+- Added inner contours options 
+- added binary2contours
+- change parameters for from_binary_mask
+- made contours2polygon
+- test
+
+2.0.0-b1 (2023-07-06)
+------------------
+- AnnotationManager function from_dict is called with an optional list of features
+- Changed Polygon and Ellipse classes to include the list of features initialized by AnnotationManager
+- to_dict function now only returns features in the dictionary that were asked for in the feature list
+- Added `feature_multiplier` and `metric_unit` as inputs to apply to the features' name and value outputs.
+- Added all features to `ellipse` and `polygon`.
+- Features are now in camelCasing when output `to_dict`
+
 2.0.0-b0 (2022-11-29)
 ------------------
 - CDF-Main: Implement `filter` to allow filtering of annotations by feature values (aka gating).
 - CDF-Main: Implement `from_contours`.
 - CDF-Main: Implement `to_contours`.
 - CDF-Main: Implement `from_dict`.
 - CDF-Main: Implement `to_dict`. Includes rounding.
```

### Comparing `tomni-2.0.0b1/tomni.egg-info/SOURCES.txt` & `tomni-2.0.0b2/tomni.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 tomni/annotation_manager/utils/test_utils.py
 tomni/annotation_manager/utils/are_lines_equal/__init__.py
 tomni/annotation_manager/utils/are_lines_equal/main.py
 tomni/annotation_manager/utils/are_lines_equal/test_lines_equal.py
 tomni/annotation_manager/utils/compress_polygon_points/__init__.py
 tomni/annotation_manager/utils/compress_polygon_points/main.py
 tomni/annotation_manager/utils/compress_polygon_points/test_compress_polygon_points.py
+tomni/annotation_manager/utils/contours2polygons/__init__.py
+tomni/annotation_manager/utils/contours2polygons/main.py
+tomni/annotation_manager/utils/contours2polygons/test_contours2polygons.py
 tomni/annotation_manager/utils/overlap_object/__init__.py
 tomni/annotation_manager/utils/overlap_object/main.py
 tomni/annotation_manager/utils/overlap_object/test_overlap_object.py
 tomni/annotation_manager/utils/simplify_line/__init__.py
 tomni/annotation_manager/utils/simplify_line/main.py
 tomni/annotation_manager/utils/simplify_line/test_polygon_simplify.py
 tomni/bbox_fitting/__init__.py
@@ -136,14 +139,17 @@
 tomni/make_mask/ellipse_mask/main.py
 tomni/make_mask/ellipse_mask/test_make_mask_ellipse.py
 tomni/shape_fitting/__init__.py
 tomni/shape_fitting/fit_rect_ellipse/__init__.py
 tomni/shape_fitting/fit_rect_ellipse/main.py
 tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py
 tomni/transformers/__init__.py
+tomni/transformers/binary2contours/__init__.py
+tomni/transformers/binary2contours/main.py
+tomni/transformers/binary2contours/test_binary2contours.py
 tomni/transformers/contour2bbox/__init__.py
 tomni/transformers/contour2bbox/main.py
 tomni/transformers/contour2bbox/test_contour2bbox.py
 tomni/transformers/contours2json/__init__.py
 tomni/transformers/contours2json/main.py
 tomni/transformers/contours2json/test_contours2json.py
 tomni/transformers/ellipse2json/__init__.py
```

