# Comparing `tmp/non_iid-0.1.1.tar.gz` & `tmp/non_iid-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "non_iid-0.1.1.tar", max compression
+gzip compressed data, was "non_iid-0.1.2.tar", max compression
```

## Comparing `non_iid-0.1.1.tar` & `non_iid-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       22 2023-08-01 23:36:12.795647 non_iid-0.1.1/non_iid/__init__.py
--rw-r--r--   0        0        0     1372 2023-08-02 23:43:42.939796 non_iid-0.1.1/non_iid/bootstrap.py
--rw-r--r--   0        0        0      300 2023-08-03 03:58:14.430831 non_iid-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      495 2023-08-03 03:58:25.107152 non_iid-0.1.1/setup.py
--rw-r--r--   0        0        0      444 2023-08-03 03:58:25.107349 non_iid-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       79 2023-08-03 16:13:19.997007 non_iid-0.1.2/non_iid/__init__.py
+-rw-r--r--   0        0        0     2653 2023-08-04 04:06:47.186788 non_iid-0.1.2/non_iid/bootstrap.py
+-rw-r--r--   0        0        0       95 2023-08-03 19:27:19.844172 non_iid-0.1.2/non_iid/utils.py
+-rw-r--r--   0        0        0      300 2023-08-04 04:07:55.499038 non_iid-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      495 2023-08-04 04:10:24.918017 non_iid-0.1.2/setup.py
+-rw-r--r--   0        0        0      444 2023-08-04 04:10:24.918213 non_iid-0.1.2/PKG-INFO
```

