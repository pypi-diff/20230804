# Comparing `tmp/cvxreg-0.1.7.tar.gz` & `tmp/cvxreg-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.1.7.tar", last modified: Thu Aug  3 08:17:33 2023, max compression
+gzip compressed data, was "cvxreg-0.1.8.tar", last modified: Fri Aug  4 11:01:47 2023, max compression
```

## Comparing `cvxreg-0.1.7.tar` & `cvxreg-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.980303 cvxreg-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 08:17:20.000000 cvxreg-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-03 08:17:33.980303 cvxreg-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-03 08:17:20.000000 cvxreg-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.976303 cvxreg-0.1.7/cvxreg/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.976303 cvxreg-0.1.7/cvxreg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/_cvxpy_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/_penalized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.980303 cvxreg-0.1.7/cvxreg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/_param_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/extmath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.976303 cvxreg-0.1.7/cvxreg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:17:33.980303 cvxreg-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-03 08:17:20.000000 cvxreg-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:01:47.556548 cvxreg-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-04 11:01:38.000000 cvxreg-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-04 11:01:47.556548 cvxreg-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-04 11:01:38.000000 cvxreg-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:01:47.552548 cvxreg-0.1.8/cvxreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:01:47.556548 cvxreg-0.1.8/cvxreg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/models/_cvxpy_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/models/_penalized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:01:47.556548 cvxreg-0.1.8/cvxreg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/utils/_param_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-04 11:01:38.000000 cvxreg-0.1.8/cvxreg/utils/extmath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:01:47.556548 cvxreg-0.1.8/cvxreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-04 11:01:47.000000 cvxreg-0.1.8/cvxreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-04 11:01:47.000000 cvxreg-0.1.8/cvxreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:01:47.000000 cvxreg-0.1.8/cvxreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:01:47.000000 cvxreg-0.1.8/cvxreg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 11:01:47.000000 cvxreg-0.1.8/cvxreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 11:01:47.000000 cvxreg-0.1.8/cvxreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:01:47.556548 cvxreg-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-04 11:01:38.000000 cvxreg-0.1.8/setup.py
```

### Comparing `cvxreg-0.1.7/LICENSE` & `cvxreg-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/PKG-INFO` & `cvxreg-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
 [![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
 [![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
```

### Comparing `cvxreg-0.1.7/README.md` & `cvxreg-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg/base.py` & `cvxreg-0.1.8/cvxreg/base.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg/models/_base.py` & `cvxreg-0.1.8/cvxreg/models/_base.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg/models/_cvxpy_opt.py` & `cvxreg-0.1.8/cvxreg/models/_cvxpy_opt.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg/models/_penalized.py` & `cvxreg-0.1.8/cvxreg/models/_penalized.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg/utils/_param_check.py` & `cvxreg-0.1.8/cvxreg/utils/_param_check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg/utils/check.py` & `cvxreg-0.1.8/cvxreg/utils/check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg/utils/extmath.py` & `cvxreg-0.1.8/cvxreg/utils/extmath.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.7/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.1.8/cvxreg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
 [![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
 [![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
```

### Comparing `cvxreg-0.1.7/setup.py` & `cvxreg-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='cvxreg',
-    version='0.1.7',
+    version='0.1.8',
     description='A Python Package for Convex Regression',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Zhiqiang Liao',
     author_email='zhiqiang.liao@aalto.fi',
     keywords=['ML', 'Prediction', 'Regression'],
     url='https://github.com/ConvexRegression/cvxreg',
     download_url='https://pypi.org/project/cvxreg/',
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=3.7',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
 
 install_requires = [
-    'python>=3.7',
     'numpy>=1.19.2',
     'pandas>=1.1.3',
     'scipy>=1.5.2',
     'cvxpy>=1.1.7'
 ]
 
 if __name__ == '__main__':
```

