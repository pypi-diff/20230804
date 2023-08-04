# Comparing `tmp/miepython-2.4.0.tar.gz` & `tmp/miepython-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miepython-2.4.0.tar", last modified: Sat Jun 10 22:07:22 2023, max compression
+gzip compressed data, was "miepython-2.5.0.tar", last modified: Fri Aug  4 18:51:01 2023, max compression
```

## Comparing `miepython-2.4.0.tar` & `miepython-2.5.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.939050 miepython-2.4.0/
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.876983 miepython-2.4.0/.github/
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.887274 miepython-2.4.0/.github/workflows/
--rw-r--r--   0 prahl      (501) staff       (20)      713 2022-01-27 02:10:04.000000 miepython-2.4.0/.github/workflows/test.yml
--rw-r--r--   0 prahl      (501) staff       (20)      164 2022-01-27 02:10:04.000000 miepython-2.4.0/.gitignore
--rw-r--r--   0 prahl      (501) staff       (20)      398 2021-08-16 19:03:47.000000 miepython-2.4.0/.readthedocs.yaml
--rw-r--r--   0 prahl      (501) staff       (20)       48 2022-01-26 16:03:16.000000 miepython-2.4.0/.testignore
--rw-r--r--   0 prahl      (501) staff       (20)     5608 2023-06-10 21:51:59.000000 miepython-2.4.0/CHANGELOG.rst
--rw-r--r--   0 prahl      (501) staff       (20)      328 2023-05-26 22:17:36.000000 miepython-2.4.0/CITATION.cff
--rw-r--r--   0 prahl      (501) staff       (20)     1055 2021-03-21 17:45:57.000000 miepython-2.4.0/LICENSE.txt
--rw-r--r--   0 prahl      (501) staff       (20)      161 2023-05-26 22:17:36.000000 miepython-2.4.0/MANIFEST.in
--rw-r--r--   0 prahl      (501) staff       (20)     1767 2023-06-10 21:55:43.000000 miepython-2.4.0/Makefile
--rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-06-10 22:07:22.939377 miepython-2.4.0/PKG-INFO
--rw-r--r--   0 prahl      (501) staff       (20)     3314 2023-05-26 22:17:36.000000 miepython-2.4.0/README.rst
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.923510 miepython-2.4.0/docs/
--rw-r--r--   0 prahl      (501) staff       (20)   190191 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/01_basics.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    34904 2021-01-18 22:54:10.000000 miepython-2.4.0/docs/01_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   123686 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/02_efficiencies.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    47794 2021-01-18 22:55:06.000000 miepython-2.4.0/docs/02_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   478393 2022-01-30 19:54:28.000000 miepython-2.4.0/docs/03_angular_scattering.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    34095 2021-01-18 22:55:36.000000 miepython-2.4.0/docs/03_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   165954 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/03a_normalization.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    54959 2022-03-13 17:44:50.000000 miepython-2.4.0/docs/04_plot.png
--rw-r--r--   0 prahl      (501) staff       (20)   133775 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/04_rayleigh.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)   264354 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/05_fog.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    88000 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/06_random_deviates.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    43928 2022-01-26 16:03:16.000000 miepython-2.4.0/docs/07_algorithm.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)   565045 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/08_large_spheres.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    33297 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/09_backscattering.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)    21271 2021-05-22 14:24:13.000000 miepython-2.4.0/docs/10_basic_tests.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)   111396 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/11_performance.ipynb
--rw-r--r--   0 prahl      (501) staff       (20)       29 2020-03-30 16:00:58.000000 miepython-2.4.0/docs/changelog.rst
--rw-r--r--   0 prahl      (501) staff       (20)     1953 2022-07-05 15:41:23.000000 miepython-2.4.0/docs/conf.py
--rw-r--r--   0 prahl      (501) staff       (20)     3113 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/index.rst
--rw-r--r--   0 prahl      (501) staff       (20)      136 2022-01-27 02:10:43.000000 miepython-2.4.0/docs/miepython.rst
--rw-r--r--   0 prahl      (501) staff       (20)       76 2022-07-05 15:42:07.000000 miepython-2.4.0/docs/requirements.txt
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.927018 miepython-2.4.0/miepython/
--rw-r--r--   0 prahl      (501) staff       (20)     1498 2023-06-10 21:47:39.000000 miepython-2.4.0/miepython/__init__.py
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.933208 miepython-2.4.0/miepython/data/
--rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.4.0/miepython/data/Johnson.txt
--rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.4.0/miepython/data/ag-Johnson.txt
--rw-r--r--   0 prahl      (501) staff       (20)    36719 2022-01-27 02:10:04.000000 miepython-2.4.0/miepython/data/segelstein81_index.txt
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.937851 miepython-2.4.0/miepython/examples/
--rwxr-xr-x   0 prahl      (501) staff       (20)      684 2021-07-09 19:31:22.000000 miepython-2.4.0/miepython/examples/01_dielectric.py
--rwxr-xr-x   0 prahl      (501) staff       (20)      804 2021-07-09 19:33:51.000000 miepython-2.4.0/miepython/examples/02_glass.py
--rwxr-xr-x   0 prahl      (501) staff       (20)      921 2021-07-09 19:46:36.000000 miepython-2.4.0/miepython/examples/03_droplets.py
--rwxr-xr-x   0 prahl      (501) staff       (20)     2717 2022-03-12 23:14:57.000000 miepython-2.4.0/miepython/examples/04_gold.py
--rw-r--r--   0 prahl      (501) staff       (20)    28173 2023-06-10 21:52:43.000000 miepython-2.4.0/miepython/miepython.py
--rw-r--r--   0 prahl      (501) staff       (20)    25822 2023-06-10 21:52:20.000000 miepython-2.4.0/miepython/miepython_nojit.py
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.930642 miepython-2.4.0/miepython.egg-info/
--rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/PKG-INFO
--rw-r--r--   0 prahl      (501) staff       (20)     1156 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/SOURCES.txt
--rw-r--r--   0 prahl      (501) staff       (20)        1 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/dependency_links.txt
--rw-r--r--   0 prahl      (501) staff       (20)       23 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/requires.txt
--rw-r--r--   0 prahl      (501) staff       (20)       10 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/top_level.txt
--rw-r--r--   0 prahl      (501) staff       (20)      569 2022-07-05 15:56:06.000000 miepython-2.4.0/pyproject.toml
--rw-r--r--   0 prahl      (501) staff       (20)      602 2022-03-12 18:25:05.000000 miepython-2.4.0/release.txt
--rw-r--r--   0 prahl      (501) staff       (20)      182 2021-05-22 21:35:05.000000 miepython-2.4.0/requirements-dev.txt
--rw-r--r--   0 prahl      (501) staff       (20)       22 2021-04-25 22:33:21.000000 miepython-2.4.0/requirements.txt
--rw-r--r--   0 prahl      (501) staff       (20)      986 2023-06-10 22:07:22.940582 miepython-2.4.0/setup.cfg
--rw-r--r--   0 prahl      (501) staff       (20)     1095 2022-03-12 23:40:23.000000 miepython-2.4.0/setup.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.672263 miepython-2.5.0/
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.642866 miepython-2.5.0/.github/
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.649114 miepython-2.5.0/.github/workflows/
+-rw-r--r--   0 prahl      (501) staff       (20)      713 2022-01-27 02:10:04.000000 miepython-2.5.0/.github/workflows/test.yml
+-rw-r--r--   0 prahl      (501) staff       (20)      164 2022-01-27 02:10:04.000000 miepython-2.5.0/.gitignore
+-rw-r--r--   0 prahl      (501) staff       (20)      398 2021-08-16 19:03:47.000000 miepython-2.5.0/.readthedocs.yaml
+-rw-r--r--   0 prahl      (501) staff       (20)       48 2022-01-26 16:03:16.000000 miepython-2.5.0/.testignore
+-rw-r--r--   0 prahl      (501) staff       (20)     5698 2023-08-04 18:48:01.000000 miepython-2.5.0/CHANGELOG.rst
+-rw-r--r--   0 prahl      (501) staff       (20)      328 2023-05-26 22:17:36.000000 miepython-2.5.0/CITATION.cff
+-rw-r--r--   0 prahl      (501) staff       (20)     1055 2021-03-21 17:45:57.000000 miepython-2.5.0/LICENSE.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      161 2023-05-26 22:17:36.000000 miepython-2.5.0/MANIFEST.in
+-rw-r--r--   0 prahl      (501) staff       (20)     1767 2023-06-10 21:55:43.000000 miepython-2.5.0/Makefile
+-rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-08-04 18:51:01.672703 miepython-2.5.0/PKG-INFO
+-rw-r--r--   0 prahl      (501) staff       (20)     3314 2023-05-26 22:17:36.000000 miepython-2.5.0/README.rst
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.663404 miepython-2.5.0/docs/
+-rw-r--r--   0 prahl      (501) staff       (20)   190191 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/01_basics.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    34904 2021-01-18 22:54:10.000000 miepython-2.5.0/docs/01_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   123686 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/02_efficiencies.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    47794 2021-01-18 22:55:06.000000 miepython-2.5.0/docs/02_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   478393 2022-01-30 19:54:28.000000 miepython-2.5.0/docs/03_angular_scattering.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    34095 2021-01-18 22:55:36.000000 miepython-2.5.0/docs/03_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   165954 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/03a_normalization.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    54959 2022-03-13 17:44:50.000000 miepython-2.5.0/docs/04_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   133775 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/04_rayleigh.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)   264354 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/05_fog.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    88000 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/06_random_deviates.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    43928 2022-01-26 16:03:16.000000 miepython-2.5.0/docs/07_algorithm.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)   565045 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/08_large_spheres.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    33297 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/09_backscattering.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    21271 2021-05-22 14:24:13.000000 miepython-2.5.0/docs/10_basic_tests.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)   111396 2021-04-25 22:33:21.000000 miepython-2.5.0/docs/11_performance.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)       29 2020-03-30 16:00:58.000000 miepython-2.5.0/docs/changelog.rst
+-rw-r--r--   0 prahl      (501) staff       (20)     1953 2022-07-05 15:41:23.000000 miepython-2.5.0/docs/conf.py
+-rw-r--r--   0 prahl      (501) staff       (20)     3113 2023-05-26 22:17:36.000000 miepython-2.5.0/docs/index.rst
+-rw-r--r--   0 prahl      (501) staff       (20)      136 2022-01-27 02:10:43.000000 miepython-2.5.0/docs/miepython.rst
+-rw-r--r--   0 prahl      (501) staff       (20)       76 2022-07-05 15:42:07.000000 miepython-2.5.0/docs/requirements.txt
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.664986 miepython-2.5.0/miepython/
+-rw-r--r--   0 prahl      (501) staff       (20)     1498 2023-08-04 18:48:20.000000 miepython-2.5.0/miepython/__init__.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.669433 miepython-2.5.0/miepython/data/
+-rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.0/miepython/data/Johnson.txt
+-rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.0/miepython/data/ag-Johnson.txt
+-rw-r--r--   0 prahl      (501) staff       (20)    36719 2022-01-27 02:10:04.000000 miepython-2.5.0/miepython/data/segelstein81_index.txt
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.671791 miepython-2.5.0/miepython/examples/
+-rwxr-xr-x   0 prahl      (501) staff       (20)      684 2021-07-09 19:31:22.000000 miepython-2.5.0/miepython/examples/01_dielectric.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)      804 2021-07-09 19:33:51.000000 miepython-2.5.0/miepython/examples/02_glass.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)      921 2021-07-09 19:46:36.000000 miepython-2.5.0/miepython/examples/03_droplets.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)     2717 2022-03-12 23:14:57.000000 miepython-2.5.0/miepython/examples/04_gold.py
+-rw-r--r--   0 prahl      (501) staff       (20)    28001 2023-08-04 18:43:45.000000 miepython-2.5.0/miepython/miepython.py
+-rw-r--r--   0 prahl      (501) staff       (20)    25628 2023-08-04 18:17:11.000000 miepython-2.5.0/miepython/miepython_nojit.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-04 18:51:01.667904 miepython-2.5.0/miepython.egg-info/
+-rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/PKG-INFO
+-rw-r--r--   0 prahl      (501) staff       (20)     1156 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/SOURCES.txt
+-rw-r--r--   0 prahl      (501) staff       (20)        1 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/dependency_links.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       23 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/requires.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       10 2023-08-04 18:51:01.000000 miepython-2.5.0/miepython.egg-info/top_level.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      569 2022-07-05 15:56:06.000000 miepython-2.5.0/pyproject.toml
+-rw-r--r--   0 prahl      (501) staff       (20)      602 2022-03-12 18:25:05.000000 miepython-2.5.0/release.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      182 2021-05-22 21:35:05.000000 miepython-2.5.0/requirements-dev.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       22 2021-04-25 22:33:21.000000 miepython-2.5.0/requirements.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      986 2023-08-04 18:51:01.673884 miepython-2.5.0/setup.cfg
+-rw-r--r--   0 prahl      (501) staff       (20)     1095 2022-03-12 23:40:23.000000 miepython-2.5.0/setup.py
```

### Comparing `miepython-2.4.0/.github/workflows/test.yml` & `miepython-2.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/CHANGELOG.rst` & `miepython-2.5.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+v2.5.0 (8/4/2023)
+-------------------
+*   fix scattering function for very small spheres
+
 v2.4.0 (6/10/2023)
 -------------------
 *   add mie_phase_matrix() to calculate scattering (Mueller) matrix
 
 v2.3.2
 -------------------
 *   fix typo in README.rst that prevented pypi upload
```

### Comparing `miepython-2.4.0/LICENSE.txt` & `miepython-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/Makefile` & `miepython-2.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/PKG-INFO` & `miepython-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.4.0
+Version: 2.5.0
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `miepython-2.4.0/README.rst` & `miepython-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/01_basics.ipynb` & `miepython-2.5.0/docs/01_basics.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/01_plot.png` & `miepython-2.5.0/docs/01_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/02_efficiencies.ipynb` & `miepython-2.5.0/docs/02_efficiencies.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/02_plot.png` & `miepython-2.5.0/docs/02_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/03_angular_scattering.ipynb` & `miepython-2.5.0/docs/03_angular_scattering.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/03_plot.png` & `miepython-2.5.0/docs/03_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/03a_normalization.ipynb` & `miepython-2.5.0/docs/03a_normalization.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/04_plot.png` & `miepython-2.5.0/docs/04_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/04_rayleigh.ipynb` & `miepython-2.5.0/docs/04_rayleigh.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/05_fog.ipynb` & `miepython-2.5.0/docs/05_fog.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/06_random_deviates.ipynb` & `miepython-2.5.0/docs/06_random_deviates.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/07_algorithm.ipynb` & `miepython-2.5.0/docs/07_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/08_large_spheres.ipynb` & `miepython-2.5.0/docs/08_large_spheres.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/09_backscattering.ipynb` & `miepython-2.5.0/docs/09_backscattering.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/10_basic_tests.ipynb` & `miepython-2.5.0/docs/10_basic_tests.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/11_performance.ipynb` & `miepython-2.5.0/docs/11_performance.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/conf.py` & `miepython-2.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/docs/index.rst` & `miepython-2.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/__init__.py` & `miepython-2.5.0/miepython/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     miepython.i_unpolarized(m, x, mu, norm='one')
 
 The scattering matrix
 
     miepython.mie_phase_matrix(m, x, mu)
 
 """
-__version__ = '2.4.0'
+__version__ = '2.5.0'
 __author__ = 'Scott Prahl'
 __email__ = 'scott.prahl@oit.edu'
 __copyright__ = 'Copyright 2017-23, Scott Prahl'
 __license__ = 'MIT'
 __url__ = 'https://github.com/scottprahl/miepython.git'
 
 from .miepython import *
```

### Comparing `miepython-2.4.0/miepython/data/Johnson.txt` & `miepython-2.5.0/miepython/data/Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/data/ag-Johnson.txt` & `miepython-2.5.0/miepython/data/ag-Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/data/segelstein81_index.txt` & `miepython-2.5.0/miepython/data/segelstein81_index.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/examples/01_dielectric.py` & `miepython-2.5.0/miepython/examples/01_dielectric.py`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/examples/02_glass.py` & `miepython-2.5.0/miepython/examples/02_glass.py`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/examples/03_droplets.py` & `miepython-2.5.0/miepython/examples/03_droplets.py`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/examples/04_gold.py` & `miepython-2.5.0/miepython/examples/04_gold.py`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/miepython/miepython.py` & `miepython-2.5.0/miepython/miepython.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,61 +472,58 @@
     norm = np.sqrt(np.pi * 6 * x**3 * (ahat1 + bhat1 + 5 * ahat2 / 3).real)
     S1 /= norm
     S2 /= norm
 
     return [S1, S2]
 
 
-@njit((complex128[:], complex128[:], float64, int32), cache=True)
-def normalization_factor(a, b, x, norm_int):
+@njit((complex128, float64, int32), cache=True)
+def normalization_factor(m, x, norm_int):
     """
     Figure out scattering function normalization.
 
     Args:
         a: complex array of An coefficients
         b: complex array of Bn coefficients
         x: dimensionless sphere size
         norm_int: integer that specifies normalization
 
     Returns:
         scaling factor needed for scattering function
     """
     # Qsca normalization
     if norm_int == 3:
-        return np.sqrt(np.pi * x**2)
+        return x * np.sqrt(np.pi)
 
     # Bohren Normalization
     if norm_int == 5:
         return 0.5
 
     # Wiscombe Normalization
     if norm_int == 6:
         return 1
 
     # calculate qsca and qext
-    n = np.arange(1, len(a) + 1)
-    cn = 2.0 * n + 1.0
-    qext = 2 * np.sum(cn * (a.real + b.real)) / x**2
-    qsca = 2 * np.sum(cn * (np.abs(a)**2 + np.abs(b)**2)) / x**2
+    qext, qsca, _, _ = _mie_scalar(m, x)
 
     # albedo Normalization
     if norm_int == 0:
-        return np.sqrt(np.pi * x**2 * qext)
+        return x * np.sqrt(np.pi * qext)
 
     # Unity normalization
     if norm_int == 1:
-        return np.sqrt(qsca * np.pi * x**2)
+        return x * np.sqrt(qsca * np.pi)
 
     # 4pi Normalization
     if norm_int == 2:
-        return np.sqrt(qsca * x**2 / 4)
+        return x * np.sqrt(qsca / 4)
 
     # Qext Normalization
     if norm_int == 4:  # 4pi
-        return np.sqrt(qsca * np.pi * x**2 / qext)
+        return x * np.sqrt(qsca * np.pi / qext)
 
     raise ValueError("norm-int must be in the range 0..6")
 
 
 def norm_string_to_integer(s):
     """
     Encode normalization choice as an integer.
@@ -605,15 +602,15 @@
             S2[k] += (2 * n + 1) * (tau_nm1 * a[n - 1]
                                     + pi_nm1 * b[n - 1]) / (n + 1) / n
 
             temp = pi_nm1
             pi_nm1 = ((2 * n + 1) * mu[k] * pi_nm1 - (n + 1) * pi_nm2) / n
             pi_nm2 = temp
 
-    normalization = normalization_factor(a, b, x, norm_int)
+    normalization = normalization_factor(m, x, norm_int)
 
     S1 /= normalization
     S2 /= normalization
 
     return [S1, S2]
```

### Comparing `miepython-2.4.0/miepython/miepython_nojit.py` & `miepython-2.5.0/miepython/miepython_nojit.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,55 +461,50 @@
     norm = np.sqrt(np.pi * 6 * x**3 * (ahat1 + bhat1 + 5 * ahat2 / 3).real)
     S1 /= norm
     S2 /= norm
 
     return [S1, S2]
 
 
-def normalization_factor(a, b, x, norm_str):
+def normalization_factor(m, x, norm_str):
     """
     Figure out scattering function normalization.
 
     Args:
-        a: complex array of An coefficients
-        b: complex array of Bn coefficients
+        m: complex index of refraction of sphere
         x: dimensionless sphere size
         norm_str: string describing type of normalization
 
     Returns:
         scaling factor needed for scattering function
     """
     norm = norm_str.lower()
 
     if norm in ['bohren']:
         return 1 / 2
 
     if norm in ['wiscombe']:
         return 1
 
-    n = np.arange(1, len(a) + 1)
-    cn = 2.0 * n + 1.0
-    qext = 2 * np.sum(cn * (a.real + b.real)) / x**2
+    if norm in ['qsca', 'scattering_efficiency']:
+        return x * np.sqrt(np.pi)
 
-    if norm in ['a', 'albedo']:
-        return np.sqrt(np.pi * x**2 * qext)
+    qext, qsca, _, _ = _mie_scalar(m, x)
 
-    qsca = 2 * np.sum(cn * (np.abs(a)**2 + np.abs(b)**2)) / x**2
+    if norm in ['a', 'albedo']:
+        return x * np.sqrt(np.pi * qext)
 
     if norm in ['1', 'one', 'unity']:
-        return np.sqrt(qsca * np.pi * x**2)
+        return x * np.sqrt(qsca * np.pi)
 
     if norm in ['four_pi', '4pi']:
-        return np.sqrt(qsca * x**2 / 4)
-
-    if norm in ['qsca', 'scattering_efficiency']:
-        return np.sqrt(np.pi * x**2)
+        return x * np.sqrt(qsca / 4)
 
     if norm in ['qext', 'extinction_efficiency']:
-        return np.sqrt(qsca * np.pi * x**2 / qext)
+        return x * np.sqrt(qsca * np.pi / qext)
 
     raise ValueError("normalization must be one of 'albedo' (default), 'one'"
                      "'4pi', 'qext', 'qsca', 'bohren', or 'wiscombe'")
 
 
 def mie_S1_S2(m, x, mu, norm='albedo'):
     """
@@ -545,15 +540,15 @@
             S2[k] += (2 * n + 1) * (tau_nm1 * a[n - 1]
                                     + pi_nm1 * b[n - 1]) / (n + 1) / n
 
             temp = pi_nm1
             pi_nm1 = ((2 * n + 1) * mu[k] * pi_nm1 - (n + 1) * pi_nm2) / n
             pi_nm2 = temp
 
-    normalization = normalization_factor(a, b, x, norm)
+    normalization = normalization_factor(m, x, norm)
 
     S1 /= normalization
     S2 /= normalization
 
     return [S1, S2]
```

### Comparing `miepython-2.4.0/miepython.egg-info/PKG-INFO` & `miepython-2.5.0/miepython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.4.0
+Version: 2.5.0
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `miepython-2.4.0/miepython.egg-info/SOURCES.txt` & `miepython-2.5.0/miepython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/pyproject.toml` & `miepython-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/release.txt` & `miepython-2.5.0/release.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/setup.cfg` & `miepython-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `miepython-2.4.0/setup.py` & `miepython-2.5.0/setup.py`

 * *Files identical despite different names*

