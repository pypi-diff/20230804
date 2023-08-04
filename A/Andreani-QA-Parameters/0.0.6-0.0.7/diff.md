# Comparing `tmp/Andreani_QA_Parameters-0.0.6.tar.gz` & `tmp/Andreani_QA_Parameters-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Parameters-0.0.6.tar", last modified: Wed Jul 26 17:44:29 2023, max compression
+gzip compressed data, was "Andreani_QA_Parameters-0.0.7.tar", last modified: Fri Aug  4 14:44:13 2023, max compression
```

## Comparing `Andreani_QA_Parameters-0.0.6.tar` & `Andreani_QA_Parameters-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:44:29.719469 Andreani_QA_Parameters-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-26 17:44:29.710523 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/
--rw-rw-rw-   0        0        0      278 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 17:44:29.716053 Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/
--rw-rw-rw-   0        0        0     3107 2023-07-26 17:42:01.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/Parameters.py
--rw-rw-rw-   0        0        0       36 2023-07-17 18:24:05.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/__init__.py
--rw-rw-rw-   0        0        0      278 2023-07-26 17:44:29.718457 Andreani_QA_Parameters-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 17:44:29.719469 Andreani_QA_Parameters-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-07-26 17:42:28.000000 Andreani_QA_Parameters-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:44:13.127473 Andreani_QA_Parameters-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:44:13.118647 Andreani_QA_Parameters-0.0.7/Andreani_QA_Parameters.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-08-04 14:44:13.000000 Andreani_QA_Parameters-0.0.7/Andreani_QA_Parameters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-08-04 14:44:13.000000 Andreani_QA_Parameters-0.0.7/Andreani_QA_Parameters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:44:13.000000 Andreani_QA_Parameters-0.0.7/Andreani_QA_Parameters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-04 14:44:13.000000 Andreani_QA_Parameters-0.0.7/Andreani_QA_Parameters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 14:44:13.124475 Andreani_QA_Parameters-0.0.7/Andreani_QA_parameters/
+-rw-rw-rw-   0        0        0     2759 2023-08-04 14:20:04.000000 Andreani_QA_Parameters-0.0.7/Andreani_QA_parameters/Parameters.py
+-rw-rw-rw-   0        0        0       36 2023-07-17 18:24:05.000000 Andreani_QA_Parameters-0.0.7/Andreani_QA_parameters/__init__.py
+-rw-rw-rw-   0        0        0      278 2023-08-04 14:44:13.127473 Andreani_QA_Parameters-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 14:44:13.128797 Andreani_QA_Parameters-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-08-04 13:35:17.000000 Andreani_QA_Parameters-0.0.7/setup.py
```

### Comparing `Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/Parameters.py` & `Andreani_QA_Parameters-0.0.7/Andreani_QA_parameters/Parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     browser = 'CHROME'
     debug = False
     headless = False
     #VARIABLE LISTA DE PASOS
     steps_list = []
 
     # CONFIGURACION INCREMENTO AUTO/MANUALEXCEL
-    excel = f"{current_path}\\resources"
     manual_increment = False
     row = 2
 
     # CONFIGURACION PATH JMETER
     path_jmeter = f"C:\\Tools\\Jmeter\\bin\\jmeter.bat"
     path_jmeter_libraries_ext = f"C:\\Tools\\Jmeter\\lib\\ext"
     path_jmeter_downloads = f"{current_path}\\projects\\ApisCliente\\src\\downloads"
@@ -68,20 +67,10 @@
     server = "127.0.0.1"  # Direccion Ip de la UI desplegada por locust.
     port = 8089  # Puerto de la UI desplegada por locust.
     max_threads = 100  # Cantidad maxima de hilos (Peticiones) alcanzable.
     rate = 10  # Coeficiente incremental de carga.
     duration = 60  # Duracion de la prueba (Segundos)
     wait_time = 1  # Duracion de tiempos de espera entre peticiones.
 
-    # CONFIGURACION DE EJECUCION
-    if environment == 'Windows':
-        # DIRECTORIO DE LA EVIDENCIA
-        evidence_route = current_path
-        resource = f"{current_path}\\projects"
-
-    if environment == 'Linux':
-        # DIRECTORIO DE LA EVIDENCIA
-        evidence_route = current_path
-
     # CONFIGURACION PARA NOTIFICACIONES DE TEAMS
     teams_notifications_colors = "#5b5fc7"
     teams_focus_test_colors = "#383966"
```

### Comparing `Andreani_QA_Parameters-0.0.6/setup.py` & `Andreani_QA_Parameters-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.6'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.7'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'Andreani_QA_Parameters'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Parametros + Encriptor para ejecución de casos automatizados'  # Descripción corta
```

