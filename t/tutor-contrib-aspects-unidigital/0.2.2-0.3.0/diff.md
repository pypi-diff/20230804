# Comparing `tmp/tutor-contrib-aspects-unidigital-0.2.2.tar.gz` & `tmp/tutor-contrib-aspects-unidigital-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-unidigital-0.2.2.tar", last modified: Fri Aug  4 19:37:55 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-unidigital-0.3.0.tar", last modified: Fri Aug  4 19:38:01 2023, max compression
```

## Comparing `tutor-contrib-aspects-unidigital-0.2.2.tar` & `tutor-contrib-aspects-unidigital-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-04 19:37:55.000000 tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-04 19:37:55.000000 tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:37:55.000000 tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 19:37:55.000000 tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 19:37:55.000000 tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 19:37:55.000000 tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/patches/superset-extra-asset-translations
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.332864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.332864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.332864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/aspects-unidigital/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:55.336864 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/openedx-assets-unidigital/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/openedx-assets-unidigital/Aggregation_Dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/openedx-assets-unidigital/Professor_Dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-04 19:37:44.000000 tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/openedx-assets-unidigital/Student_Dashboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.543344 tutor-contrib-aspects-unidigital-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-04 19:38:01.543344 tutor-contrib-aspects-unidigital-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 19:38:01.543344 tutor-contrib-aspects-unidigital-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.539344 tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-04 19:38:01.000000 tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-04 19:38:01.000000 tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:38:01.000000 tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 19:38:01.000000 tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 19:38:01.000000 tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 19:38:01.000000 tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.539344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.539344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/patches/superset-extra-asset-translations
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.535344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.535344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.539344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.539344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.535344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.539344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/aspects-unidigital/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.535344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.539344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/charts/Total_courses.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/charts/Total_student_enrollments.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/charts/Video_count.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:01.543344 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Aggregation_Dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Professor_Dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-04 19:37:50.000000 tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Student_Dashboard.yaml
```

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/LICENSE` & `tutor-contrib-aspects-unidigital-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/PKG-INFO` & `tutor-contrib-aspects-unidigital-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects-unidigital
-Version: 0.2.2
+Version: 0.3.0
 Summary: aspects-unidigital plugin for Tutor
 Home-page: https://github.com/eduNEXT/tutor-contrib-aspects-unidigital
 Author: Felipe Montoya
 License: AGPLv3
 Project-URL: Code, https://github.com/eduNEXT/tutor-contrib-aspects-unidigital
 Project-URL: Issue tracker, https://github.com/eduNEXT/tutor-contrib-aspects-unidigital/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/README.rst` & `tutor-contrib-aspects-unidigital-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/setup.py` & `tutor-contrib-aspects-unidigital-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/PKG-INFO` & `tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects-unidigital
-Version: 0.2.2
+Version: 0.3.0
 Summary: aspects-unidigital plugin for Tutor
 Home-page: https://github.com/eduNEXT/tutor-contrib-aspects-unidigital
 Author: Felipe Montoya
 License: AGPLv3
 Project-URL: Code, https://github.com/eduNEXT/tutor-contrib-aspects-unidigital
 Project-URL: Issue tracker, https://github.com/eduNEXT/tutor-contrib-aspects-unidigital/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/tutor_contrib_aspects_unidigital.egg-info/SOURCES.txt` & `tutor-contrib-aspects-unidigital-0.3.0/tutor_contrib_aspects_unidigital.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,10 +14,13 @@
 tutoraspects_unidigital/plugin.py
 tutoraspects_unidigital/patches/.gitignore
 tutoraspects_unidigital/patches/superset-extra-asset-translations
 tutoraspects_unidigital/patches/superset-extra-assets
 tutoraspects_unidigital/templates/aspects-unidigital/apps/.gitignore
 tutoraspects_unidigital/templates/aspects-unidigital/build/.gitignore
 tutoraspects_unidigital/templates/aspects-unidigital/jobs/init/.gitignore
-tutoraspects_unidigital/templates/openedx-assets-unidigital/Aggregation_Dashboard.yaml
-tutoraspects_unidigital/templates/openedx-assets-unidigital/Professor_Dashboard.yaml
-tutoraspects_unidigital/templates/openedx-assets-unidigital/Student_Dashboard.yaml
+tutoraspects_unidigital/templates/openedx-assets-unidigital/charts/Total_courses.yaml
+tutoraspects_unidigital/templates/openedx-assets-unidigital/charts/Total_student_enrollments.yaml
+tutoraspects_unidigital/templates/openedx-assets-unidigital/charts/Video_count.yaml
+tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Aggregation_Dashboard.yaml
+tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Professor_Dashboard.yaml
+tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Student_Dashboard.yaml
```

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/patches/superset-extra-asset-translations` & `tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/patches/superset-extra-asset-translations`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 es:
   Professor Dashboard: Panel de profesorado
   Forum: Foro
   Student Ranking: Ranking de estudiantes
   File Downloads: Descarga de materiales
   Overview: Vista general
   Problems: Ejercicios
@@ -33,8 +34,16 @@
   Course Comparison: "Comparaci\xF3n de cursos"
   Demographics: "Demograf\xEDa"
   Aggregated Data: "Datos agregados"
   Enrollments: Inscripciones
   Students Activity: Actividad de estudiantes
   Temporal Evolution: "Evoluci\xF3n temporal"
   Courses: Cursos
-  Global Data: Datos globales
+  Global Data: Datos globales
+  Total courses: Total de cursos
+  Video count: Cantidad de vídeos
+  Total student enrollments: Total de inscripciones de estudiantes
+  Student Dashboard: Panel de estudiantado
+  Ranking: Ranking
+  My Activity: Mi actividad
+  My logins: Mis accesos
+  My Progress: Mi progreso
```

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/plugin.py` & `tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/openedx-assets-unidigital/Professor_Dashboard.yaml` & `tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Professor_Dashboard.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-unidigital-0.2.2/tutoraspects_unidigital/templates/openedx-assets-unidigital/Student_Dashboard.yaml` & `tutor-contrib-aspects-unidigital-0.3.0/tutoraspects_unidigital/templates/openedx-assets-unidigital/dashboards/Student_Dashboard.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 - _file_name: Student_Dashboard.yaml
   _roles:
   - {{ SUPERSET_ROLES_MAPPING.instructor }}
-  dashboard_title: Panel de estudiantado
+  dashboard_title: Student Dashboard
   description: null
   css: ''
   slug: student-dashboard
   uuid: 83660341-8acc-4f09-8f3c-ef4871e2415b
   position:
     DASHBOARD_VERSION_KEY: v2
     GRID_ID:
@@ -14,15 +14,15 @@
       id: GRID_ID
       parents:
       - ROOT_ID
       type: GRID
     HEADER_ID:
       id: HEADER_ID
       meta:
-        text: Panel de Estudiantado
+        text: Student Dashboard
       type: HEADER
     ROOT_ID:
       children:
       - GRID_ID
       id: ROOT_ID
       type: ROOT
     TAB-AVu8IhsCI:
@@ -35,35 +35,35 @@
       - GRID_ID
       - TABS-T4bhiYuKQ-
       type: TAB
     TAB-E-Tl_rVKBl:
       children: []
       id: TAB-E-Tl_rVKBl
       meta:
-        text: Mi actividad
+        text: My Activity
       parents:
       - ROOT_ID
       - GRID_ID
       - TABS-T4bhiYuKQ-
       type: TAB
     TAB-dclIZdA65:
       children: []
       id: TAB-dclIZdA65
       meta:
-        text: Mis acceso
+        text: My logins
       parents:
       - ROOT_ID
       - GRID_ID
       - TABS-T4bhiYuKQ-
       type: TAB
     TAB-xhPfZpHdL:
       children: []
       id: TAB-xhPfZpHdL
       meta:
-        text: Mi progreso
+        text: My Progress
       parents:
       - ROOT_ID
       - GRID_ID
       - TABS-T4bhiYuKQ-
       type: TAB
     TABS-T4bhiYuKQ-:
       children:
```

