# Comparing `tmp/laminci-0.7.4.tar.gz` & `tmp/laminci-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "laminci-0.7.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `laminci-0.7.4.tar` & `laminci-0.7.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1096 2023-06-14 23:30:30.962603 laminci-0.7.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.7.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.7.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.7.4/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.7.4/README.md
--rw-r--r--   0        0        0     3534 2023-07-10 18:57:53.714480 laminci-0.7.4/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.7.4/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.7.4/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.7.4/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.7.4/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.7.4/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.7.4/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-07-10 18:57:48.829376 laminci-0.7.4/laminci/__init__.py
--rw-r--r--   0        0        0     2310 2023-06-14 23:44:38.099913 laminci-0.7.4/laminci/__main__.py
--rw-r--r--   0        0        0     2130 2023-06-14 22:24:13.327779 laminci-0.7.4/laminci/_artifacts.py
--rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.7.4/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.7.4/laminci/_docs.py
--rw-r--r--   0        0        0      948 2023-06-14 22:05:00.624145 laminci-0.7.4/laminci/_env.py
--rw-r--r--   0        0        0     2902 2023-07-10 18:57:01.095563 laminci-0.7.4/laminci/_nox.py
--rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.7.4/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.7.4/laminci/nox.py
--rw-r--r--   0        0        0      476 2023-06-14 23:30:30.962848 laminci-0.7.4/noxfile.py
--rw-r--r--   0        0        0      762 2023-06-14 23:30:30.962964 laminci-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.7.4/tests/test_artifacts.py
--rw-r--r--   0        0        0      104 2023-06-14 22:05:00.624370 laminci-0.7.4/tests/test_package_name.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 laminci-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-14 23:30:30.962603 laminci-0.7.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.7.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.7.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.7.5/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.7.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.7.5/README.md
+-rw-r--r--   0        0        0     3534 2023-07-10 18:57:53.714480 laminci-0.7.5/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.7.5/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.7.5/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.7.5/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.7.5/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.7.5/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.7.5/lamin-project.yaml
+-rw-r--r--   0        0        0      430 2023-08-04 17:05:08.523170 laminci-0.7.5/laminci/__init__.py
+-rw-r--r--   0        0        0     2310 2023-06-14 23:44:38.099913 laminci-0.7.5/laminci/__main__.py
+-rw-r--r--   0        0        0     2130 2023-06-14 22:24:13.327779 laminci-0.7.5/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.7.5/laminci/_db.py
+-rw-r--r--   0        0        0      678 2023-08-04 17:04:32.614531 laminci-0.7.5/laminci/_docs.py
+-rw-r--r--   0        0        0      948 2023-06-14 22:05:00.624145 laminci-0.7.5/laminci/_env.py
+-rw-r--r--   0        0        0     2902 2023-07-10 18:57:01.095563 laminci-0.7.5/laminci/_nox.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.7.5/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.7.5/laminci/nox.py
+-rw-r--r--   0        0        0      476 2023-06-14 23:30:30.962848 laminci-0.7.5/noxfile.py
+-rw-r--r--   0        0        0      762 2023-06-14 23:30:30.962964 laminci-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.7.5/tests/test_artifacts.py
+-rw-r--r--   0        0        0      104 2023-06-14 22:05:00.624370 laminci-0.7.5/tests/test_package_name.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 laminci-0.7.5/PKG-INFO
```

### Comparing `laminci-0.7.4/.github/workflows/build.yml` & `laminci-0.7.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/.github/workflows/latest-changes.yml` & `laminci-0.7.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/.gitignore` & `laminci-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/.pre-commit-config.yaml` & `laminci-0.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/docs/changelog.md` & `laminci-0.7.5/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/docs/guide/quickstart.ipynb` & `laminci-0.7.5/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.7.5/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/laminci/__main__.py` & `laminci-0.7.5/laminci/__main__.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/laminci/_artifacts.py` & `laminci-0.7.5/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/laminci/_db.py` & `laminci-0.7.5/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/laminci/_env.py` & `laminci-0.7.5/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/laminci/_nox.py` & `laminci-0.7.5/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.4/pyproject.toml` & `laminci-0.7.5/pyproject.toml`

 * *Files identical despite different names*

