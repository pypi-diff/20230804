# Comparing `tmp/femto-admin-0.2.0.tar.gz` & `tmp/femto-admin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femto-admin-0.2.0.tar", last modified: Mon Jul 31 08:45:14 2023, max compression
+gzip compressed data, was "femto-admin-0.2.2.tar", last modified: Fri Aug  4 09:45:18 2023, max compression
```

## Comparing `femto-admin-0.2.0.tar` & `femto-admin-0.2.2.tar`

### file list

```diff
@@ -1,84 +1,91 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.955955 femto-admin-0.2.0/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 femto-admin-0.2.0/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.2.0/MANIFEST.in
--rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-31 08:45:14.955703 femto-admin-0.2.0/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1499 2023-07-20 23:49:02.000000 femto-admin-0.2.0/README.md
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.937372 femto-admin-0.2.0/femto_admin/
--rw-r--r--   0 sol        (501) staff       (20)       58 2023-07-31 08:44:53.000000 femto-admin-0.2.0/femto_admin/__init__.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.939503 femto-admin-0.2.0/femto_admin/__pycache__/
--rw-r--r--   0 sol        (501) staff       (20)      247 2023-07-28 12:51:42.000000 femto-admin-0.2.0/femto_admin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     7442 2023-07-30 21:44:10.000000 femto-admin-0.2.0/femto_admin/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)      577 2023-07-30 18:31:17.000000 femto-admin-0.2.0/femto_admin/__pycache__/consts.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     7513 2023-07-31 07:02:33.000000 femto-admin-0.2.0/femto_admin/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     3729 2023-07-30 21:43:45.000000 femto-admin-0.2.0/femto_admin/admin.py
--rw-r--r--   0 sol        (501) staff       (20)      280 2023-07-30 18:24:21.000000 femto-admin-0.2.0/femto_admin/consts.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933180 femto-admin-0.2.0/femto_admin/statics/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.939740 femto-admin-0.2.0/femto_admin/statics/js/
--rw-r--r--   0 sol        (501) staff       (20)     1251 2023-07-27 20:59:11.000000 femto-admin-0.2.0/femto_admin/statics/js/polygon.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.939989 femto-admin-0.2.0/femto_admin/statics/placeholders/
--rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.2.0/femto_admin/statics/placeholders/favicon.ico
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.940266 femto-admin-0.2.0/femto_admin/statics/placeholders/logo/
--rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.2.0/femto_admin/statics/placeholders/logo/logo-white.svg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.940498 femto-admin-0.2.0/femto_admin/statics/placeholders/users/
--rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.2.0/femto_admin/statics/placeholders/users/admin.jpg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933717 femto-admin-0.2.0/femto_admin/statics/vendor/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933469 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.940978 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/
--rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
--rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.942350 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/
--rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
--rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
--rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
--rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.943234 femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/
--rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.js
--rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933917 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.944521 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/
--rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.css
--rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.946358 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/
--rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.js
--rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
--rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.js
--rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.947625 femto-admin-0.2.0/femto_admin/templates/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.949047 femto-admin-0.2.0/femto_admin/templates/components/
--rw-r--r--   0 sol        (501) staff       (20)     4635 2023-07-28 11:21:54.000000 femto-admin-0.2.0/femto_admin/templates/components/aside.html
--rw-r--r--   0 sol        (501) staff       (20)     1021 2023-07-28 12:11:41.000000 femto-admin-0.2.0/femto_admin/templates/components/footer.html
--rw-r--r--   0 sol        (501) staff       (20)     1464 2023-07-28 11:25:51.000000 femto-admin-0.2.0/femto_admin/templates/components/global_actions.html
--rw-r--r--   0 sol        (501) staff       (20)     4458 2023-07-28 11:52:48.000000 femto-admin-0.2.0/femto_admin/templates/components/header.html
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.954979 femto-admin-0.2.0/femto_admin/templates/components/inputs/
--rw-r--r--   0 sol        (501) staff       (20)       83 2023-07-23 20:17:52.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/_help.html
--rw-r--r--   0 sol        (501) staff       (20)      472 2023-07-31 08:22:43.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/checkbox.html
--rw-r--r--   0 sol        (501) staff       (20)      579 2023-07-30 20:21:41.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/collection.html
--rw-r--r--   0 sol        (501) staff       (20)      424 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/color.html
--rw-r--r--   0 sol        (501) staff       (20)      380 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/date.html
--rw-r--r--   0 sol        (501) staff       (20)     1019 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/datetime.html
--rw-r--r--   0 sol        (501) staff       (20)     1794 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/editor.html
--rw-r--r--   0 sol        (501) staff       (20)      489 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/image.html
--rw-r--r--   0 sol        (501) staff       (20)      359 2023-07-30 20:17:37.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/input.html
--rw-r--r--   0 sol        (501) staff       (20)     1333 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/json.html
--rw-r--r--   0 sol        (501) staff       (20)     1968 2023-07-30 19:53:21.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/list.html
--rw-r--r--   0 sol        (501) staff       (20)      857 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/many_to_many.html
--rw-r--r--   0 sol        (501) staff       (20)      607 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/radio.html
--rw-r--r--   0 sol        (501) staff       (20)      781 2023-07-28 14:45:42.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/range.html
--rw-r--r--   0 sol        (501) staff       (20)      404 2023-07-28 15:47:47.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/select.html
--rw-r--r--   0 sol        (501) staff       (20)      415 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/textarea.html
--rw-r--r--   0 sol        (501) staff       (20)     2379 2023-07-31 08:19:31.000000 femto-admin-0.2.0/femto_admin/templates/components/modal.html
--rw-r--r--   0 sol        (501) staff       (20)     7353 2023-07-23 19:34:25.000000 femto-admin-0.2.0/femto_admin/templates/components/notofications.html
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.2.0/femto_admin/templates/dashboard.html
--rw-r--r--   0 sol        (501) staff       (20)      132 2023-07-28 11:13:54.000000 femto-admin-0.2.0/femto_admin/templates/index.html
--rw-r--r--   0 sol        (501) staff       (20)     2073 2023-07-28 11:32:50.000000 femto-admin-0.2.0/femto_admin/templates/layout.html
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.955429 femto-admin-0.2.0/femto_admin/templates/views/
--rw-r--r--   0 sol        (501) staff       (20)      918 2023-07-28 11:12:19.000000 femto-admin-0.2.0/femto_admin/templates/views/table.html
--rw-r--r--   0 sol        (501) staff       (20)     5395 2023-07-31 07:02:16.000000 femto-admin-0.2.0/femto_admin/utils.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.938549 femto-admin-0.2.0/femto_admin.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     2739 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       12 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/top_level.txt
--rw-r--r--   0 sol        (501) staff       (20)      766 2023-07-28 08:06:43.000000 femto-admin-0.2.0/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 08:45:14.956017 femto-admin-0.2.0/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.578168 femto-admin-0.2.2/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 femto-admin-0.2.2/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.2.2/MANIFEST.in
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-08-04 09:45:18.577941 femto-admin-0.2.2/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1499 2023-07-20 23:49:02.000000 femto-admin-0.2.2/README.md
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.526371 femto-admin-0.2.2/femto_admin/
+-rw-r--r--   0 sol        (501) staff       (20)       58 2023-08-04 09:44:24.000000 femto-admin-0.2.2/femto_admin/__init__.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.527916 femto-admin-0.2.2/femto_admin/__pycache__/
+-rw-r--r--   0 sol        (501) staff       (20)      247 2023-07-31 13:04:15.000000 femto-admin-0.2.2/femto_admin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     8911 2023-08-04 09:40:12.000000 femto-admin-0.2.2/femto_admin/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     4413 2023-08-04 09:40:07.000000 femto-admin-0.2.2/femto_admin/admin.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.523258 femto-admin-0.2.2/femto_admin/statics/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.528154 femto-admin-0.2.2/femto_admin/statics/css/
+-rw-r--r--   0 sol        (501) staff       (20)       28 2023-08-02 09:06:13.000000 femto-admin-0.2.2/femto_admin/statics/css/main.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.529044 femto-admin-0.2.2/femto_admin/statics/js/
+-rw-r--r--   0 sol        (501) staff       (20)     1326 2023-07-31 10:50:11.000000 femto-admin-0.2.2/femto_admin/statics/js/list_field.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.529640 femto-admin-0.2.2/femto_admin/statics/placeholders/
+-rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.2.2/femto_admin/statics/placeholders/favicon.ico
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.530731 femto-admin-0.2.2/femto_admin/statics/placeholders/logo/
+-rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.2.2/femto_admin/statics/placeholders/logo/logo-white.svg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.531327 femto-admin-0.2.2/femto_admin/statics/placeholders/users/
+-rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.2.2/femto_admin/statics/placeholders/users/admin.jpg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.523725 femto-admin-0.2.2/femto_admin/statics/vendor/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.523513 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.532207 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/css/
+-rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
+-rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.534756 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/
+-rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
+-rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
+-rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.537695 femto-admin-0.2.2/femto_admin/statics/vendor/jQuery/
+-rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.2.2/femto_admin/statics/vendor/jQuery/jquery.js
+-rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.2.2/femto_admin/statics/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.524003 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.544561 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.561892 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/fonts/
+-rw-r--r--   0 sol        (501) staff       (20)  2023760 2023-07-28 09:51:16.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.eot
+-rw-r--r--   0 sol        (501) staff       (20)  2023576 2023-07-28 09:51:16.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.ttf
+-rw-r--r--   0 sol        (501) staff       (20)  1025564 2023-07-28 09:51:16.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.woff
+-rw-r--r--   0 sol        (501) staff       (20)   729764 2023-07-28 09:51:16.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.woff2
+-rw-r--r--   0 sol        (501) staff       (20)   230086 2023-08-02 08:25:14.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/tabler-icons.css
+-rw-r--r--   0 sol        (501) staff       (20)   188583 2023-08-02 08:24:08.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/tabler-icons.min.css
+-rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/tabler.css
+-rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/tabler.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.566739 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/
+-rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/dark-theme.js
+-rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/tabler.js
+-rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/tabler.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.569559 femto-admin-0.2.2/femto_admin/templates/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.571039 femto-admin-0.2.2/femto_admin/templates/components/
+-rw-r--r--   0 sol        (501) staff       (20)     4059 2023-08-02 09:07:57.000000 femto-admin-0.2.2/femto_admin/templates/components/aside.html
+-rw-r--r--   0 sol        (501) staff       (20)     1021 2023-07-28 12:11:41.000000 femto-admin-0.2.2/femto_admin/templates/components/footer.html
+-rw-r--r--   0 sol        (501) staff       (20)     1028 2023-08-02 09:27:53.000000 femto-admin-0.2.2/femto_admin/templates/components/global_actions.html
+-rw-r--r--   0 sol        (501) staff       (20)     4458 2023-07-28 11:52:48.000000 femto-admin-0.2.2/femto_admin/templates/components/header.html
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.576937 femto-admin-0.2.2/femto_admin/templates/components/inputs/
+-rw-r--r--   0 sol        (501) staff       (20)       83 2023-07-23 20:17:52.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/_help.html
+-rw-r--r--   0 sol        (501) staff       (20)      472 2023-07-31 08:22:43.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/checkbox.html
+-rw-r--r--   0 sol        (501) staff       (20)      593 2023-07-31 10:06:07.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/collection.html
+-rw-r--r--   0 sol        (501) staff       (20)      424 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/color.html
+-rw-r--r--   0 sol        (501) staff       (20)      380 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/date.html
+-rw-r--r--   0 sol        (501) staff       (20)     1019 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/datetime.html
+-rw-r--r--   0 sol        (501) staff       (20)     1794 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/editor.html
+-rw-r--r--   0 sol        (501) staff       (20)      489 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/image.html
+-rw-r--r--   0 sol        (501) staff       (20)      359 2023-07-30 20:17:37.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/input.html
+-rw-r--r--   0 sol        (501) staff       (20)     1333 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/json.html
+-rw-r--r--   0 sol        (501) staff       (20)     1966 2023-08-02 09:35:25.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/list.html
+-rw-r--r--   0 sol        (501) staff       (20)      857 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/many_to_many.html
+-rw-r--r--   0 sol        (501) staff       (20)      607 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/radio.html
+-rw-r--r--   0 sol        (501) staff       (20)      785 2023-07-31 10:04:44.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/range.html
+-rw-r--r--   0 sol        (501) staff       (20)      525 2023-08-02 12:09:35.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/select.html
+-rw-r--r--   0 sol        (501) staff       (20)      415 2023-07-03 09:15:48.000000 femto-admin-0.2.2/femto_admin/templates/components/inputs/textarea.html
+-rw-r--r--   0 sol        (501) staff       (20)      871 2023-08-02 10:53:56.000000 femto-admin-0.2.2/femto_admin/templates/components/modal.html
+-rw-r--r--   0 sol        (501) staff       (20)     7353 2023-07-23 19:34:25.000000 femto-admin-0.2.2/femto_admin/templates/components/notofications.html
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.2.2/femto_admin/templates/dashboard.html
+-rw-r--r--   0 sol        (501) staff       (20)      263 2023-08-04 09:40:07.000000 femto-admin-0.2.2/femto_admin/templates/edit.html
+-rw-r--r--   0 sol        (501) staff       (20)      143 2023-08-04 09:37:29.000000 femto-admin-0.2.2/femto_admin/templates/index.html
+-rw-r--r--   0 sol        (501) staff       (20)     2290 2023-08-02 09:05:44.000000 femto-admin-0.2.2/femto_admin/templates/layout.html
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.577678 femto-admin-0.2.2/femto_admin/templates/views/
+-rw-r--r--   0 sol        (501) staff       (20)      947 2023-08-02 11:23:29.000000 femto-admin-0.2.2/femto_admin/templates/views/form.html
+-rw-r--r--   0 sol        (501) staff       (20)      928 2023-08-04 09:35:42.000000 femto-admin-0.2.2/femto_admin/templates/views/table.html
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-04 09:45:18.527460 femto-admin-0.2.2/femto_admin.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-08-04 09:45:18.000000 femto-admin-0.2.2/femto_admin.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     3070 2023-08-04 09:45:18.000000 femto-admin-0.2.2/femto_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-08-04 09:45:18.000000 femto-admin-0.2.2/femto_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-08-04 09:45:18.000000 femto-admin-0.2.2/femto_admin.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       12 2023-08-04 09:45:18.000000 femto-admin-0.2.2/femto_admin.egg-info/top_level.txt
+-rw-r--r--   0 sol        (501) staff       (20)      766 2023-07-31 11:52:33.000000 femto-admin-0.2.2/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-08-04 09:45:18.578225 femto-admin-0.2.2/setup.cfg
```

### Comparing `femto-admin-0.2.0/LICENSE` & `femto-admin-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/PKG-INFO` & `femto-admin-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femto-admin
-Version: 0.2.0
+Version: 0.2.2
 Summary: Simplest fastest minimal ASGI CRUD Admin panel for Tortoise ORM models. It's generating fully native async auto  zero config one line app
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/femto-admin
 Project-URL: Repository, https://github.com/mixartemev/femto-admin
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `femto-admin-0.2.0/README.md` & `femto-admin-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/__pycache__/admin.cpython-311.pyc` & `femto-admin-0.2.2/femto_admin/__pycache__/admin.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x91d9c664 (Sun Jul 30 21:43:45 2023 UTC)
-files sz: 3729
+moddate:  0x77c7cc64 (Fri Aug  4 09:40:07 2023 UTC)
+files sz: 4413
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d005a000100640064026c016d025a026d035a036d
       045a040100640064036c056d065a060100640064046c076d085a086d095a
       090100640064056c0a6d0b5a0b6d0c5a0c0100640064066c0d6d0e5a0e01
       00640064076c0f6d105a100100640064086c116d125a120100640064096c
-      136d145a1401006400640a6c156d165a1601006400640b6c175a17640064
-      0c6c186d195a19010002004700640d8400640e6512a6030000ab03000000
-      00000000005a1a640b5300
+      136d145a1401006400640a6c156d165a1601006400640b6c175a17020047
+      00640c8400640d6512a6030000ab0300000000000000005a18640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('datetime',))
                  6 IMPORT_NAME              0 (datetime)
                  8 IMPORT_FROM              0 (datetime)
                 10 STORE_NAME               0 (datetime)
@@ -95,349 +94,363 @@
                136 POP_TOP
    
     13         138 LOAD_CONST               0 (0)
                140 LOAD_CONST              11 (None)
                142 IMPORT_NAME             23 (femto_admin)
                144 STORE_NAME              23 (femto_admin)
    
-    14         146 LOAD_CONST               0 (0)
-               148 LOAD_CONST              12 (('_fields',))
-               150 IMPORT_NAME             24 (femto_admin.utils)
-               152 IMPORT_FROM             25 (_fields)
-               154 STORE_NAME              25 (_fields)
-               156 POP_TOP
-   
-    17         158 PUSH_NULL
-               160 LOAD_BUILD_CLASS
-               162 LOAD_CONST              13 (<code object Admin, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 17>)
-               164 MAKE_FUNCTION            0
-               166 LOAD_CONST              14 ('Admin')
-               168 LOAD_NAME               18 (Api)
-               170 PRECALL                  3
-               174 CALL                     3
-               184 STORE_NAME              26 (Admin)
-               186 LOAD_CONST              11 (None)
-               188 RETURN_VALUE
+    16         146 PUSH_NULL
+               148 LOAD_BUILD_CLASS
+               150 LOAD_CONST              12 (<code object Admin, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 16>)
+               152 MAKE_FUNCTION            0
+               154 LOAD_CONST              13 ('Admin')
+               156 LOAD_NAME               18 (Api)
+               158 PRECALL                  3
+               162 CALL                     3
+               172 STORE_NAME              24 (Admin)
+               174 LOAD_CONST              11 (None)
+               176 RETURN_VALUE
    consts
       0
       ('datetime',)
       ('ChoiceLoader', 'FileSystemLoader', 'PackageLoader')
       ('Request',)
       ('RedirectResponse', 'JSONResponse')
       ('Mount', 'Route')
       ('StaticFiles',)
       ('Jinja2Templates',)
       ('Api',)
       ('jsonify',)
       ('Model',)
       None
-      ('_fields',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 10
+         stacksize : 11
          flags     : 0
          code
-            0x8700970065005a0164005a02640d640365036404650464056504640665
-            0465037a0700006608880066016407840d5a0588006601640884085a0664
-            0965076602640a84045a08640965076602640b84045a0964096507660264
-            0c84045a0a880078015a0b5300
+            0x8700970065005a0164005a02640f640365036404650464056504640665
+            0465037a07000064076505660a880066016408840d5a0688006601640984
+            085a07640a65086602640b84045a09640a65086602640c84045a0a640a65
+            086602640d84045a0b640a65086602640e84045a0c880078015a0d5300
                        0 MAKE_CELL                0 (__class__)
          
-          17           2 RESUME                   0
+          16           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Admin')
                       10 STORE_NAME               2 (__qualname__)
          
-          18          12 LOAD_CONST              13 ((False, 'Admin', None, None))
+          17          12 LOAD_CONST              15 ((False, 'Admin', None, None, None))
                       14 LOAD_CONST               3 ('debug')
                       16 LOAD_NAME                3 (bool)
                       18 LOAD_CONST               4 ('title')
                       20 LOAD_NAME                4 (str)
                       22 LOAD_CONST               5 ('static_dir')
                       24 LOAD_NAME                4 (str)
                       26 LOAD_CONST               6 ('logo')
                       28 LOAD_NAME                4 (str)
                       30 LOAD_NAME                3 (bool)
                       32 BINARY_OP                7 (|)
-                      36 BUILD_TUPLE              8
-                      38 LOAD_CLOSURE             0 (__class__)
-                      40 BUILD_TUPLE              1
-                      42 LOAD_CONST               7 (<code object __init__, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 18>)
-                      44 MAKE_FUNCTION           13 (defaults, annotations, closure)
-                      46 STORE_NAME               5 (__init__)
+                      36 LOAD_CONST               7 ('dash_func')
+                      38 LOAD_NAME                5 (callable)
+                      40 BUILD_TUPLE             10
+                      42 LOAD_CLOSURE             0 (__class__)
+                      44 BUILD_TUPLE              1
+                      46 LOAD_CONST               8 (<code object __init__, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 17>)
+                      48 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                      50 STORE_NAME               6 (__init__)
+         
+          53          52 LOAD_CLOSURE             0 (__class__)
+                      54 BUILD_TUPLE              1
+                      56 LOAD_CONST               9 (<code object start, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 53>)
+                      58 MAKE_FUNCTION            8 (closure)
+                      60 STORE_NAME               7 (start)
          
-          53          48 LOAD_CLOSURE             0 (__class__)
-                      50 BUILD_TUPLE              1
-                      52 LOAD_CONST               8 (<code object start, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 53>)
-                      54 MAKE_FUNCTION            8 (closure)
-                      56 STORE_NAME               6 (start)
+          59          62 LOAD_CONST              10 ('request')
+                      64 LOAD_NAME                8 (Request)
+                      66 BUILD_TUPLE              2
+                      68 LOAD_CONST              11 (<code object dash, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 59>)
+                      70 MAKE_FUNCTION            4 (annotations)
+                      72 STORE_NAME               9 (dash)
          
-          59          58 LOAD_CONST               9 ('request')
-                      60 LOAD_NAME                7 (Request)
-                      62 BUILD_TUPLE              2
-                      64 LOAD_CONST              10 (<code object dash, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 59>)
-                      66 MAKE_FUNCTION            4 (annotations)
-                      68 STORE_NAME               8 (dash)
+          66          74 LOAD_CONST              10 ('request')
+                      76 LOAD_NAME                8 (Request)
+                      78 BUILD_TUPLE              2
+                      80 LOAD_CONST              12 (<code object index, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 66>)
+                      82 MAKE_FUNCTION            4 (annotations)
+                      84 STORE_NAME              10 (index)
          
-          66          70 LOAD_CONST               9 ('request')
-                      72 LOAD_NAME                7 (Request)
-                      74 BUILD_TUPLE              2
-                      76 LOAD_CONST              11 (<code object index, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 66>)
-                      78 MAKE_FUNCTION            4 (annotations)
-                      80 STORE_NAME               9 (index)
+          75          86 LOAD_CONST              10 ('request')
+                      88 LOAD_NAME                8 (Request)
+                      90 BUILD_TUPLE              2
+                      92 LOAD_CONST              13 (<code object edit, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 75>)
+                      94 MAKE_FUNCTION            4 (annotations)
+                      96 STORE_NAME              11 (edit)
          
-          75          82 LOAD_CONST               9 ('request')
-                      84 LOAD_NAME                7 (Request)
-                      86 BUILD_TUPLE              2
-                      88 LOAD_CONST              12 (<code object dt, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 75>)
-                      90 MAKE_FUNCTION            4 (annotations)
-                      92 STORE_NAME              10 (dt)
-                      94 LOAD_CLOSURE             0 (__class__)
-                      96 COPY                     1
-                      98 STORE_NAME              11 (__classcell__)
-                     100 RETURN_VALUE
+          90          98 LOAD_CONST              10 ('request')
+                     100 LOAD_NAME                8 (Request)
+                     102 BUILD_TUPLE              2
+                     104 LOAD_CONST              14 (<code object dt, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 90>)
+                     106 MAKE_FUNCTION            4 (annotations)
+                     108 STORE_NAME              12 (dt)
+                     110 LOAD_CLOSURE             0 (__class__)
+                     112 COPY                     1
+                     114 STORE_NAME              13 (__classcell__)
+                     116 RETURN_VALUE
          consts
             'Admin'
             False
             None
             'debug'
             'title'
             'static_dir'
             'logo'
+            'dash_func'
             code
-               argcount  : 5
-               nlocals   : 6
-               stacksize : 9
+               argcount  : 6
+               nlocals   : 7
+               stacksize : 10
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   01000000000000000001007c027c005f0200000000000000007407000000
-                  00000000000000640174090000000000000000000064026701ac03a60100
-                  00ab0100000000000000006404ac05a6030000ab03000000000000000074
-                  070000000000000000000064067c006a050000000000000000ac07a60200
-                  00ab020000000000000000740d0000000000000000000064086409840064
-                  0a6701ac0ba6030000ab030000000000000000740d000000000000000000
-                  00640c7c006a070000000000000000a6020000ab02000000000000000074
-                  0d00000000000000000000640d7c006a080000000000000000a6020000ab
-                  020000000000000000740d00000000000000000000640e7c006a09000000
-                  0000000000a6020000ab02000000000000000067067c005f050000000000
-                  0000007c006a050000000000000000640f190000000000000000006a0500
-                  00000000000000a00a000000000000000000000000000000000000000064
-                  0fa6010000ab010000000000000000010074170000000000000000000064
-                  10a6010000ab0100000000000000007d057c03724c7c006a050000000000
-                  000000a00c00000000000000000000000000000000000000007407000000
-                  00000000000000640e7c037a0000007409000000000000000000007c03ac
-                  11a6010000ab0100000000000000006412ac05a6030000ab030000000000
-                  000000a6010000ab01000000000000000001007c04810f7c047c056a0d00
-                  000000000000006a0e000000000000000064143c000000741f0000000000
-                  00000000007421000000000000000000006410a6010000ab010000000000
-                  00000074230000000000000000000064026410a6020000ab020000000000
-                  0000006702a6010000ab0100000000000000007c056a0d00000000000000
-                  005f1200000000000000007c006a0200000000000000007c056a0d000000
-                  00000000006a0e000000000000000064153c000000742700000000000000
-                  0000006a140000000000000000a6000000ab0000000000000000006a1500
-                  00000000000000742c000000000000000000006a17000000000000000064
-                  169c027c056a0d00000000000000006a0e000000000000000064173c0000
-                  007c01720264186e0164197c056a0d00000000000000006a0e0000000000
-                  000000641a3c0000007c057c005f18000000000000000064135300
+                  0000000000000064017c0570067c006a040000000000000000a6020000ab
+                  020000000000000000740b0000000000000000000064027c006a06000000
+                  0000000000ac03a6020000ab020000000000000000740b00000000000000
+                  0000006404740f0000000000000000000064056701ac06a6010000ab0100
+                  000000000000006407ac08a6030000ab0300000000000000007407000000
+                  000000000000006409640a8400640b6701ac0ca6030000ab030000000000
+                  000000740700000000000000000000640d7c006a080000000000000000a6
+                  020000ab020000000000000000740700000000000000000000640e7c006a
+                  090000000000000000a6020000ab02000000000000000074070000000000
+                  0000000000640f7c006a0a0000000000000000a6020000ab020000000000
+                  00000067077c005f0600000000000000007c006a06000000000000000064
+                  10190000000000000000006a060000000000000000a00b00000000000000
+                  000000000000000000000000006410a6010000ab01000000000000000001
+                  007419000000000000000000006411a6010000ab0100000000000000007d
+                  067c03724c7c006a060000000000000000a00d0000000000000000000000
+                  000000000000000000740b0000000000000000000064017c037a00000074
+                  0f000000000000000000007c03ac12a6010000ab01000000000000000064
+                  13ac08a6030000ab030000000000000000a6010000ab0100000000000000
+                  0001007c04810f7c047c066a0e00000000000000006a0f00000000000000
+                  0064153c0000007421000000000000000000007423000000000000000000
+                  006411a6010000ab01000000000000000074250000000000000000000064
+                  056411a6020000ab0200000000000000006702a6010000ab010000000000
+                  0000007c066a0e00000000000000005f1300000000000000007c006a0200
+                  000000000000007c066a0e00000000000000006a0f000000000000000064
+                  163c0000007429000000000000000000006a150000000000000000a60000
+                  00ab0000000000000000006a160000000000000000742e00000000000000
+                  0000006a18000000000000000064179c027c066a0e00000000000000006a
+                  0f000000000000000064183c0000007c01720264196e01641a7c066a0e00
+                  000000000000006a0f0000000000000000641b3c0000007c067c005f1900
+                  0000000000000064145300
                              0 COPY_FREE_VARS           1
                
-                18           2 RESUME                   0
+                17           2 RESUME                   0
                
-                24           4 LOAD_GLOBAL              1 (NULL + super)
+                23           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 LOAD_FAST                1 (debug)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-                25          70 LOAD_FAST                2 (title)
+                24          70 LOAD_FAST                2 (title)
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (title)
                
-                28          84 LOAD_GLOBAL              7 (NULL + Mount)
-                            96 LOAD_CONST               1 ('/static')
-                            98 LOAD_GLOBAL              9 (NULL + StaticFiles)
-                           110 LOAD_CONST               2 ('femto_admin')
-                           112 BUILD_LIST               1
-                           114 KW_NAMES                 3
-                           116 PRECALL                  1
-                           120 CALL                     1
-                           130 LOAD_CONST               4 ('public')
-                           132 KW_NAMES                 5
-                           134 PRECALL                  3
-                           138 CALL                     3
-               
-                29         148 LOAD_GLOBAL              7 (NULL + Mount)
-                           160 LOAD_CONST               6 ('/api')
-                           162 LOAD_FAST                0 (self)
-                           164 LOAD_ATTR                5 (routes)
-                           174 KW_NAMES                 7
-                           176 PRECALL                  2
-                           180 CALL                     2
-               
-                30         190 LOAD_GLOBAL             13 (NULL + Route)
-                           202 LOAD_CONST               8 ('/favicon.ico')
-                           204 LOAD_CONST               9 (<code object <lambda>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 30>)
-                           206 MAKE_FUNCTION            0
-                           208 LOAD_CONST              10 ('GET')
-                           210 BUILD_LIST               1
-                           212 KW_NAMES                11
-                           214 PRECALL                  3
-                           218 CALL                     3
-               
-                31         228 LOAD_GLOBAL             13 (NULL + Route)
-                           240 LOAD_CONST              12 ('/{model}')
-                           242 LOAD_FAST                0 (self)
-                           244 LOAD_ATTR                7 (index)
-                           254 PRECALL                  2
-                           258 CALL                     2
-               
-                32         268 LOAD_GLOBAL             13 (NULL + Route)
-                           280 LOAD_CONST              13 ('/dt/{model}')
-                           282 LOAD_FAST                0 (self)
-                           284 LOAD_ATTR                8 (dt)
-                           294 PRECALL                  2
-                           298 CALL                     2
-               
-                33         308 LOAD_GLOBAL             13 (NULL + Route)
-                           320 LOAD_CONST              14 ('/')
-                           322 LOAD_FAST                0 (self)
-                           324 LOAD_ATTR                9 (dash)
-                           334 PRECALL                  2
-                           338 CALL                     2
-               
-                27         348 BUILD_LIST               6
-                           350 LOAD_FAST                0 (self)
-                           352 STORE_ATTR               5 (routes)
-               
-                35         362 LOAD_FAST                0 (self)
-                           364 LOAD_ATTR                5 (routes)
-                           374 LOAD_CONST              15 (1)
-                           376 BINARY_SUBSCR
-                           386 LOAD_ATTR                5 (routes)
-                           396 LOAD_METHOD             10 (pop)
-                           418 LOAD_CONST              15 (1)
-                           420 PRECALL                  1
-                           424 CALL                     1
-                           434 POP_TOP
-               
-                37         436 LOAD_GLOBAL             23 (NULL + Jinja2Templates)
-                           448 LOAD_CONST              16 ('templates')
-                           450 PRECALL                  1
-                           454 CALL                     1
-                           464 STORE_FAST               5 (templates)
-               
-                38         466 LOAD_FAST                3 (static_dir)
-                           468 POP_JUMP_FORWARD_IF_FALSE    76 (to 622)
-               
-                39         470 LOAD_FAST                0 (self)
-                           472 LOAD_ATTR                5 (routes)
-                           482 LOAD_METHOD             12 (append)
-                           504 LOAD_GLOBAL              7 (NULL + Mount)
-                           516 LOAD_CONST              14 ('/')
-                           518 LOAD_FAST                3 (static_dir)
-                           520 BINARY_OP                0 (+)
-                           524 LOAD_GLOBAL              9 (NULL + StaticFiles)
-                           536 LOAD_FAST                3 (static_dir)
-                           538 KW_NAMES                17
-                           540 PRECALL                  1
-                           544 CALL                     1
-                           554 LOAD_CONST              18 ('my-public')
-                           556 KW_NAMES                 5
-                           558 PRECALL                  3
-                           562 CALL                     3
-                           572 PRECALL                  1
-                           576 CALL                     1
-                           586 POP_TOP
-               
-                40         588 LOAD_FAST                4 (logo)
-                           590 POP_JUMP_FORWARD_IF_NONE    15 (to 622)
-               
-                41         592 LOAD_FAST                4 (logo)
-                           594 LOAD_FAST                5 (templates)
-                           596 LOAD_ATTR               13 (env)
-                           606 LOAD_ATTR               14 (globals)
-                           616 LOAD_CONST              20 ('logo')
-                           618 STORE_SUBSCR
-               
-                42     >>  622 LOAD_GLOBAL             31 (NULL + ChoiceLoader)
-               
-                44         634 LOAD_GLOBAL             33 (NULL + FileSystemLoader)
-                           646 LOAD_CONST              16 ('templates')
-                           648 PRECALL                  1
-                           652 CALL                     1
-               
-                45         662 LOAD_GLOBAL             35 (NULL + PackageLoader)
-                           674 LOAD_CONST               2 ('femto_admin')
-                           676 LOAD_CONST              16 ('templates')
-                           678 PRECALL                  2
-                           682 CALL                     2
-               
-                43         692 BUILD_LIST               2
-               
-                42         694 PRECALL                  1
-                           698 CALL                     1
-                           708 LOAD_FAST                5 (templates)
-                           710 LOAD_ATTR               13 (env)
-                           720 STORE_ATTR              18 (loader)
-               
-                48         730 LOAD_FAST                0 (self)
-                           732 LOAD_ATTR                2 (title)
-                           742 LOAD_FAST                5 (templates)
-                           744 LOAD_ATTR               13 (env)
-                           754 LOAD_ATTR               14 (globals)
-                           764 LOAD_CONST              21 ('title')
-                           766 STORE_SUBSCR
-               
-                49         770 LOAD_GLOBAL             39 (NULL + datetime)
-                           782 LOAD_ATTR               20 (now)
-                           792 PRECALL                  0
-                           796 CALL                     0
-                           806 LOAD_ATTR               21 (year)
-                           816 LOAD_GLOBAL             44 (femto_admin)
-                           828 LOAD_ATTR               23 (__version__)
-                           838 LOAD_CONST              22 (('year', 'ver'))
-                           840 BUILD_CONST_KEY_MAP      2
-                           842 LOAD_FAST                5 (templates)
-                           844 LOAD_ATTR               13 (env)
-                           854 LOAD_ATTR               14 (globals)
-                           864 LOAD_CONST              23 ('meta')
-                           866 STORE_SUBSCR
-               
-                50         870 LOAD_FAST                1 (debug)
-                           872 POP_JUMP_FORWARD_IF_FALSE     2 (to 878)
-                           874 LOAD_CONST              24 ('')
-                           876 JUMP_FORWARD             1 (to 880)
-                       >>  878 LOAD_CONST              25 ('min.')
-                       >>  880 LOAD_FAST                5 (templates)
-                           882 LOAD_ATTR               13 (env)
-                           892 LOAD_ATTR               14 (globals)
-                           902 LOAD_CONST              26 ('minify')
-                           904 STORE_SUBSCR
-               
-                51         908 LOAD_FAST                5 (templates)
-                           910 LOAD_FAST                0 (self)
-                           912 STORE_ATTR              24 (templates)
-                           922 LOAD_CONST              19 (None)
-                           924 RETURN_VALUE
+                27          84 LOAD_GLOBAL              7 (NULL + Route)
+                            96 LOAD_CONST               1 ('/')
+                            98 LOAD_FAST                5 (dash_func)
+                           100 JUMP_IF_TRUE_OR_POP      6 (to 114)
+                           102 LOAD_FAST                0 (self)
+                           104 LOAD_ATTR                4 (dash)
+                       >>  114 PRECALL                  2
+                           118 CALL                     2
+               
+                28         128 LOAD_GLOBAL             11 (NULL + Mount)
+                           140 LOAD_CONST               2 ('/api')
+                           142 LOAD_FAST                0 (self)
+                           144 LOAD_ATTR                6 (routes)
+                           154 KW_NAMES                 3
+                           156 PRECALL                  2
+                           160 CALL                     2
+               
+                29         170 LOAD_GLOBAL             11 (NULL + Mount)
+                           182 LOAD_CONST               4 ('/static')
+                           184 LOAD_GLOBAL             15 (NULL + StaticFiles)
+                           196 LOAD_CONST               5 ('femto_admin')
+                           198 BUILD_LIST               1
+                           200 KW_NAMES                 6
+                           202 PRECALL                  1
+                           206 CALL                     1
+                           216 LOAD_CONST               7 ('public')
+                           218 KW_NAMES                 8
+                           220 PRECALL                  3
+                           224 CALL                     3
+               
+                30         234 LOAD_GLOBAL              7 (NULL + Route)
+                           246 LOAD_CONST               9 ('/favicon.ico')
+                           248 LOAD_CONST              10 (<code object <lambda>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 30>)
+                           250 MAKE_FUNCTION            0
+                           252 LOAD_CONST              11 ('GET')
+                           254 BUILD_LIST               1
+                           256 KW_NAMES                12
+                           258 PRECALL                  3
+                           262 CALL                     3
+               
+                31         272 LOAD_GLOBAL              7 (NULL + Route)
+                           284 LOAD_CONST              13 ('/{model}')
+                           286 LOAD_FAST                0 (self)
+                           288 LOAD_ATTR                8 (index)
+                           298 PRECALL                  2
+                           302 CALL                     2
+               
+                32         312 LOAD_GLOBAL              7 (NULL + Route)
+                           324 LOAD_CONST              14 ('/dt/{model}')
+                           326 LOAD_FAST                0 (self)
+                           328 LOAD_ATTR                9 (dt)
+                           338 PRECALL                  2
+                           342 CALL                     2
+               
+                33         352 LOAD_GLOBAL              7 (NULL + Route)
+                           364 LOAD_CONST              15 ('/{model}/{oid}')
+                           366 LOAD_FAST                0 (self)
+                           368 LOAD_ATTR               10 (edit)
+                           378 PRECALL                  2
+                           382 CALL                     2
+               
+                26         392 BUILD_LIST               7
+                           394 LOAD_FAST                0 (self)
+                           396 STORE_ATTR               6 (routes)
+               
+                35         406 LOAD_FAST                0 (self)
+                           408 LOAD_ATTR                6 (routes)
+                           418 LOAD_CONST              16 (1)
+                           420 BINARY_SUBSCR
+                           430 LOAD_ATTR                6 (routes)
+                           440 LOAD_METHOD             11 (pop)
+                           462 LOAD_CONST              16 (1)
+                           464 PRECALL                  1
+                           468 CALL                     1
+                           478 POP_TOP
+               
+                37         480 LOAD_GLOBAL             25 (NULL + Jinja2Templates)
+                           492 LOAD_CONST              17 ('templates')
+                           494 PRECALL                  1
+                           498 CALL                     1
+                           508 STORE_FAST               6 (templates)
+               
+                38         510 LOAD_FAST                3 (static_dir)
+                           512 POP_JUMP_FORWARD_IF_FALSE    76 (to 666)
+               
+                39         514 LOAD_FAST                0 (self)
+                           516 LOAD_ATTR                6 (routes)
+                           526 LOAD_METHOD             13 (append)
+                           548 LOAD_GLOBAL             11 (NULL + Mount)
+                           560 LOAD_CONST               1 ('/')
+                           562 LOAD_FAST                3 (static_dir)
+                           564 BINARY_OP                0 (+)
+                           568 LOAD_GLOBAL             15 (NULL + StaticFiles)
+                           580 LOAD_FAST                3 (static_dir)
+                           582 KW_NAMES                18
+                           584 PRECALL                  1
+                           588 CALL                     1
+                           598 LOAD_CONST              19 ('my-public')
+                           600 KW_NAMES                 8
+                           602 PRECALL                  3
+                           606 CALL                     3
+                           616 PRECALL                  1
+                           620 CALL                     1
+                           630 POP_TOP
+               
+                40         632 LOAD_FAST                4 (logo)
+                           634 POP_JUMP_FORWARD_IF_NONE    15 (to 666)
+               
+                41         636 LOAD_FAST                4 (logo)
+                           638 LOAD_FAST                6 (templates)
+                           640 LOAD_ATTR               14 (env)
+                           650 LOAD_ATTR               15 (globals)
+                           660 LOAD_CONST              21 ('logo')
+                           662 STORE_SUBSCR
+               
+                42     >>  666 LOAD_GLOBAL             33 (NULL + ChoiceLoader)
+               
+                44         678 LOAD_GLOBAL             35 (NULL + FileSystemLoader)
+                           690 LOAD_CONST              17 ('templates')
+                           692 PRECALL                  1
+                           696 CALL                     1
+               
+                45         706 LOAD_GLOBAL             37 (NULL + PackageLoader)
+                           718 LOAD_CONST               5 ('femto_admin')
+                           720 LOAD_CONST              17 ('templates')
+                           722 PRECALL                  2
+                           726 CALL                     2
+               
+                43         736 BUILD_LIST               2
+               
+                42         738 PRECALL                  1
+                           742 CALL                     1
+                           752 LOAD_FAST                6 (templates)
+                           754 LOAD_ATTR               14 (env)
+                           764 STORE_ATTR              19 (loader)
+               
+                48         774 LOAD_FAST                0 (self)
+                           776 LOAD_ATTR                2 (title)
+                           786 LOAD_FAST                6 (templates)
+                           788 LOAD_ATTR               14 (env)
+                           798 LOAD_ATTR               15 (globals)
+                           808 LOAD_CONST              22 ('title')
+                           810 STORE_SUBSCR
+               
+                49         814 LOAD_GLOBAL             41 (NULL + datetime)
+                           826 LOAD_ATTR               21 (now)
+                           836 PRECALL                  0
+                           840 CALL                     0
+                           850 LOAD_ATTR               22 (year)
+                           860 LOAD_GLOBAL             46 (femto_admin)
+                           872 LOAD_ATTR               24 (__version__)
+                           882 LOAD_CONST              23 (('year', 'ver'))
+                           884 BUILD_CONST_KEY_MAP      2
+                           886 LOAD_FAST                6 (templates)
+                           888 LOAD_ATTR               14 (env)
+                           898 LOAD_ATTR               15 (globals)
+                           908 LOAD_CONST              24 ('meta')
+                           910 STORE_SUBSCR
+               
+                50         914 LOAD_FAST                1 (debug)
+                           916 POP_JUMP_FORWARD_IF_FALSE     2 (to 922)
+                           918 LOAD_CONST              25 ('')
+                           920 JUMP_FORWARD             1 (to 924)
+                       >>  922 LOAD_CONST              26 ('min.')
+                       >>  924 LOAD_FAST                6 (templates)
+                           926 LOAD_ATTR               14 (env)
+                           936 LOAD_ATTR               15 (globals)
+                           946 LOAD_CONST              27 ('minify')
+                           948 STORE_SUBSCR
+               
+                51         952 LOAD_FAST                6 (templates)
+                           954 LOAD_FAST                0 (self)
+                           956 STORE_ATTR              25 (templates)
+                           966 LOAD_CONST              20 (None)
+                           968 RETURN_VALUE
                consts
                   '\n        Parameters:\n            title: Admin title.\n            # auth_provider: Authentication Provider\n        '
+                  '/'
+                  '/api'
+                  ('routes',)
                   '/static'
                   'femto_admin'
                   ('packages',)
                   'public'
                   ('name',)
-                  '/api'
-                  ('routes',)
                   '/favicon.ico'
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 4
                      flags     : 19
                      code
@@ -464,37 +477,37 @@
                      name       '<lambda>'
                      firstlineno 30
                      lnotab 0x
                   'GET'
                   ('methods',)
                   '/{model}'
                   '/dt/{model}'
-                  '/'
+                  '/{model}/{oid}'
                   1
                   'templates'
                   ('directory',)
                   'my-public'
                   None
                   'logo'
                   'title'
                   ('year', 'ver')
                   'meta'
                   ''
                   'min.'
                   'minify'
-               names      ('super', '__init__', 'title', 'Mount', 'StaticFiles', 'routes', 'Route', 'index', 'dt', 'dash', 'pop', 'Jinja2Templates', 'append', 'env', 'globals', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'loader', 'datetime', 'now', 'year', 'femto_admin', '__version__', 'templates')
-               varnames   ('self', 'debug', 'title', 'static_dir', 'logo', 'templates')
+               names      ('super', '__init__', 'title', 'Route', 'dash', 'Mount', 'routes', 'StaticFiles', 'index', 'dt', 'edit', 'pop', 'Jinja2Templates', 'append', 'env', 'globals', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'loader', 'datetime', 'now', 'year', 'femto_admin', '__version__', 'templates')
+               varnames   ('self', 'debug', 'title', 'static_dir', 'logo', 'dash_func', 'templates')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       '__init__'
-               firstlineno 18
+               firstlineno 17
                lnotab
-                  0x040642010e0340012a0126012801280128fa0e084a021e010401760104
-                  011e010c021c011efe02ff2406280164012601
+                  0x040642010e032c012a01400126012801280128f90e094a021e01040176
+                  0104011e010c021c011efe02ff2406280164012601
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
@@ -577,77 +590,282 @@
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'dash'
                firstlineno 59
                lnotab 0x06012402020102fd
             code
                argcount  : 2
                nlocals   : 3
-               stacksize : 9
+               stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c00a00000000000000000000000000000000000000000
-                  007c01a6010000ab0100000000000000007d027c006a0100000000000000
-                  00a002000000000000000000000000000000000000000064017c026a0300
-                  000000000000007c026a0400000000000000006a0500000000000000007c
-                  01740d000000000000000000007c02a6010000ab01000000000000000083
-                  0064007b0356009703860464029c04a6020000ab02000000000000000053
-                  00
+                  007c01a6010000ab0100000000000000007d027c02a00100000000000000
+                  00000000000000000000000000a6000000ab000000000000000000830064
+                  007b0356009703860401007c006a020000000000000000a0030000000000
+                  00000000000000000000000000000064017c027c026a0400000000000000
+                  006a0500000000000000007c0164029c03a6020000ab0200000000000000
+                  005300
                 66           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 67           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (_get_model)
                             30 LOAD_FAST                1 (request)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 STORE_FAST               2 (model)
                
-                68          48 LOAD_FAST                0 (self)
-                            50 LOAD_ATTR                1 (templates)
-                            60 LOAD_METHOD              2 (TemplateResponse)
-                            82 LOAD_CONST               1 ('index.html')
-               
-                69          84 LOAD_FAST                2 (model)
-                            86 LOAD_ATTR                3 (__name__)
-               
-                70          96 LOAD_FAST                2 (model)
-                            98 LOAD_ATTR                4 (_meta)
-                           108 LOAD_ATTR                5 (table_description)
-               
-                71         118 LOAD_FAST                1 (request)
-               
-                72         120 LOAD_GLOBAL             13 (NULL + _fields)
-                           132 LOAD_FAST                2 (model)
-                           134 PRECALL                  1
-                           138 CALL                     1
-                           148 GET_AWAITABLE            0
-                           150 LOAD_CONST               0 (None)
-                       >>  152 SEND                     3 (to 160)
-                           154 YIELD_VALUE
-                           156 RESUME                   3
-                           158 JUMP_BACKWARD_NO_INTERRUPT     4 (to 152)
-               
-                68     >>  160 LOAD_CONST               2 (('model', 'subtitle', 'request', 'fields'))
-                           162 BUILD_CONST_KEY_MAP      4
-                           164 PRECALL                  2
-                           168 CALL                     2
-                           178 RETURN_VALUE
+                68          48 LOAD_FAST                2 (model)
+                            50 LOAD_METHOD              1 (load_rel_options)
+                            72 PRECALL                  0
+                            76 CALL                     0
+                            86 GET_AWAITABLE            0
+                            88 LOAD_CONST               0 (None)
+                       >>   90 SEND                     3 (to 98)
+                            92 YIELD_VALUE
+                            94 RESUME                   3
+                            96 JUMP_BACKWARD_NO_INTERRUPT     4 (to 90)
+                       >>   98 POP_TOP
+               
+                69         100 LOAD_FAST                0 (self)
+                           102 LOAD_ATTR                2 (templates)
+                           112 LOAD_METHOD              3 (TemplateResponse)
+                           134 LOAD_CONST               1 ('index.html')
+               
+                70         136 LOAD_FAST                2 (model)
+               
+                71         138 LOAD_FAST                2 (model)
+                           140 LOAD_ATTR                4 (_meta)
+                           150 LOAD_ATTR                5 (table_description)
+               
+                72         160 LOAD_FAST                1 (request)
+               
+                69         162 LOAD_CONST               2 (('model', 'subtitle', 'request'))
+                           164 BUILD_CONST_KEY_MAP      3
+                           166 PRECALL                  2
+                           170 CALL                     2
+                           180 RETURN_VALUE
                consts
                   None
                   'index.html'
-                  ('model', 'subtitle', 'request', 'fields')
-               names      ('_get_model', 'templates', 'TemplateResponse', '__name__', '_meta', 'table_description', '_fields')
+                  ('model', 'subtitle', 'request')
+               names      ('_get_model', 'load_rel_options', 'templates', 'TemplateResponse', '_meta', 'table_description')
                varnames   ('self', 'request', 'model')
                freevars   ()
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'index'
                firstlineno 66
-               lnotab 0x06012a0124010c011601020128fc
+               lnotab 0x06012a01340124010201160102fd
+            code
+               argcount  : 2
+               nlocals   : 5
+               stacksize : 9
+               flags     : 131
+               code
+                  0x87054b00010097007c00a0000000000000000000000000000000000000
+                  0000007c01a6010000ab0100000000000000007d027c016a010000000000
+                  0000006401190000000000000000007d037c02a002000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000830064007b
+                  03560097038604010002007c02a003000000000000000000000000000000
+                  00000000007c03ac02a6010000ab0100000000000000006a040000000000
+                  0000007c026a0500000000000000006a0600000000000000008e00830064
+                  007b035600970386048a0588056601640384087c026a0500000000000000
+                  006a0700000000000000004400a6000000ab0000000000000000007d0464
+                  0484007c044400a6000000ab000000000000000000830064007b03560097
+                  03860401007c006a080000000000000000a0090000000000000000000000
+                  00000000000000000064057c027c026a0500000000000000006a0a000000
+                  00000000007c0189057c0464069c05a6020000ab02000000000000000053
+                  00
+                             0 MAKE_CELL                5 (obj)
+               
+                75           2 RETURN_GENERATOR
+                             4 POP_TOP
+                             6 RESUME                   0
+               
+                76           8 LOAD_FAST                0 (self)
+                            10 LOAD_METHOD              0 (_get_model)
+                            32 LOAD_FAST                1 (request)
+                            34 PRECALL                  1
+                            38 CALL                     1
+                            48 STORE_FAST               2 (model)
+               
+                77          50 LOAD_FAST                1 (request)
+                            52 LOAD_ATTR                1 (path_params)
+                            62 LOAD_CONST               1 ('oid')
+                            64 BINARY_SUBSCR
+                            74 STORE_FAST               3 (oid)
+               
+                78          76 LOAD_FAST                2 (model)
+                            78 LOAD_METHOD              2 (load_rel_options)
+                           100 PRECALL                  0
+                           104 CALL                     0
+                           114 GET_AWAITABLE            0
+                           116 LOAD_CONST               0 (None)
+                       >>  118 SEND                     3 (to 126)
+                           120 YIELD_VALUE
+                           122 RESUME                   3
+                           124 JUMP_BACKWARD_NO_INTERRUPT     4 (to 118)
+                       >>  126 POP_TOP
+               
+                79         128 PUSH_NULL
+                           130 LOAD_FAST                2 (model)
+                           132 LOAD_METHOD              3 (get)
+                           154 LOAD_FAST                3 (oid)
+                           156 KW_NAMES                 2
+                           158 PRECALL                  1
+                           162 CALL                     1
+                           172 LOAD_ATTR                4 (prefetch_related)
+                           182 LOAD_FAST                2 (model)
+                           184 LOAD_ATTR                5 (_meta)
+                           194 LOAD_ATTR                6 (fetch_fields)
+                           204 CALL_FUNCTION_EX         0
+                           206 GET_AWAITABLE            0
+                           208 LOAD_CONST               0 (None)
+                       >>  210 SEND                     3 (to 218)
+                           212 YIELD_VALUE
+                           214 RESUME                   3
+                           216 JUMP_BACKWARD_NO_INTERRUPT     4 (to 210)
+                       >>  218 STORE_DEREF              5 (obj)
+               
+                80         220 LOAD_CLOSURE             5 (obj)
+                           222 BUILD_TUPLE              1
+                           224 LOAD_CONST               3 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 80>)
+                           226 MAKE_FUNCTION            8 (closure)
+                           228 LOAD_FAST                2 (model)
+                           230 LOAD_ATTR                5 (_meta)
+                           240 LOAD_ATTR                7 (backward_fk_fields)
+                           250 GET_ITER
+                           252 PRECALL                  0
+                           256 CALL                     0
+                           266 STORE_FAST               4 (bfms)
+               
+                81         268 LOAD_CONST               4 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 81>)
+                           270 MAKE_FUNCTION            0
+                           272 LOAD_FAST                4 (bfms)
+                           274 GET_ITER
+                           276 PRECALL                  0
+                           280 CALL                     0
+                           290 GET_AWAITABLE            0
+                           292 LOAD_CONST               0 (None)
+                       >>  294 SEND                     3 (to 302)
+                           296 YIELD_VALUE
+                           298 RESUME                   3
+                           300 JUMP_BACKWARD_NO_INTERRUPT     4 (to 294)
+                       >>  302 POP_TOP
+               
+                82         304 LOAD_FAST                0 (self)
+                           306 LOAD_ATTR                8 (templates)
+                           316 LOAD_METHOD              9 (TemplateResponse)
+                           338 LOAD_CONST               5 ('edit.html')
+               
+                83         340 LOAD_FAST                2 (model)
+               
+                84         342 LOAD_FAST                2 (model)
+                           344 LOAD_ATTR                5 (_meta)
+                           354 LOAD_ATTR               10 (table_description)
+               
+                85         364 LOAD_FAST                1 (request)
+               
+                86         366 LOAD_DEREF               5 (obj)
+               
+                87         368 LOAD_FAST                4 (bfms)
+               
+                82         370 LOAD_CONST               6 (('model', 'subtitle', 'request', 'obj', 'bfms'))
+                           372 BUILD_CONST_KEY_MAP      5
+                           374 PRECALL                  2
+                           378 CALL                     2
+                           388 RETURN_VALUE
+               consts
+                  None
+                  'oid'
+                  ('id',)
+                  code
+                     argcount  : 1
+                     nlocals   : 2
+                     stacksize : 6
+                     flags     : 19
+                     code
+                        0x9501970067007c005d177d0174010000000000000000000089027c01a6
+                        020000ab0200000000000000006a01000000000000000091028c185300
+                                   0 COPY_FREE_VARS           1
+                     
+                      80           2 RESUME                   0
+                                   4 BUILD_LIST               0
+                                   6 LOAD_FAST                0 (.0)
+                             >>    8 FOR_ITER                23 (to 56)
+                                  10 STORE_FAST               1 (k)
+                                  12 LOAD_GLOBAL              1 (NULL + getattr)
+                                  24 LOAD_DEREF               2 (obj)
+                                  26 LOAD_FAST                1 (k)
+                                  28 PRECALL                  2
+                                  32 CALL                     2
+                                  42 LOAD_ATTR                1 (remote_model)
+                                  52 LIST_APPEND              2
+                                  54 JUMP_BACKWARD           24 (to 8)
+                             >>   56 RETURN_VALUE
+                     consts
+                     names      ('getattr', 'remote_model')
+                     varnames   ('.0', 'k')
+                     freevars   ('obj',)
+                     cellvars   ()
+                     filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
+                     name       '<listcomp>'
+                     firstlineno 80
+                     lnotab 0x
+                  code
+                     argcount  : 1
+                     nlocals   : 2
+                     stacksize : 4
+                     flags     : 147
+                     code
+                        0x4b000100970067007c005d1c7d017c01a0000000000000000000000000
+                        000000000000000000a6000000ab000000000000000000830064007b0356
+                        009703860491028c1d5300
+                      81           0 RETURN_GENERATOR
+                                   2 POP_TOP
+                                   4 RESUME                   0
+                                   6 BUILD_LIST               0
+                                   8 LOAD_FAST                0 (.0)
+                             >>   10 FOR_ITER                28 (to 68)
+                                  12 STORE_FAST               1 (bfm)
+                                  14 LOAD_FAST                1 (bfm)
+                                  16 LOAD_METHOD              0 (load_rel_options)
+                                  38 PRECALL                  0
+                                  42 CALL                     0
+                                  52 GET_AWAITABLE            0
+                                  54 LOAD_CONST               0 (None)
+                             >>   56 SEND                     3 (to 64)
+                                  58 YIELD_VALUE
+                                  60 RESUME                   3
+                                  62 JUMP_BACKWARD_NO_INTERRUPT     4 (to 56)
+                             >>   64 LIST_APPEND              2
+                                  66 JUMP_BACKWARD           29 (to 10)
+                             >>   68 RETURN_VALUE
+                     consts
+                        None
+                     names      ('load_rel_options',)
+                     varnames   ('.0', 'bfm')
+                     freevars   ()
+                     cellvars   ()
+                     filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
+                     name       '<listcomp>'
+                     firstlineno 81
+                     lnotab 0x
+                  'edit.html'
+                  ('model', 'subtitle', 'request', 'obj', 'bfms')
+               names      ('_get_model', 'path_params', 'load_rel_options', 'get', 'prefetch_related', '_meta', 'fetch_fields', 'backward_fk_fields', 'templates', 'TemplateResponse', 'table_description')
+               varnames   ('self', 'request', 'model', 'oid', 'bfms')
+               freevars   ()
+               cellvars   ('obj',)
+               filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
+               name       'edit'
+               firstlineno 75
+               lnotab 0x08012a011a0134015c01300124012401020116010201020102fb
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 4
                flags     : 131
                code
                   0x87054b000100970064017400000000000000000000006602640284048a
@@ -656,33 +874,33 @@
                   000000000000000000a6000000ab0000000000000000006a030000000000
                   0000007c026a0400000000000000006a0500000000000000008e00830064
                   007b035600970386047d0388056601640384087c034400a6000000ab0000
                   000000000000007d04740d0000000000000000000064047c046901a60100
                   00ab0100000000000000005300
                              0 MAKE_CELL                5 (render)
                
-                75           2 RETURN_GENERATOR
+                90           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                76           8 LOAD_CONST               1 ('dct')
+                91           8 LOAD_CONST               1 ('dct')
                             10 LOAD_GLOBAL              0 (dict)
                             22 BUILD_TUPLE              2
-                            24 LOAD_CONST               2 (<code object render, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 76>)
+                            24 LOAD_CONST               2 (<code object render, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 91>)
                             26 MAKE_FUNCTION            4 (annotations)
                             28 STORE_DEREF              5 (render)
                
-                88          30 LOAD_FAST                0 (self)
+               103          30 LOAD_FAST                0 (self)
                             32 LOAD_METHOD              1 (_get_model)
                             54 LOAD_FAST                1 (request)
                             56 PRECALL                  1
                             60 CALL                     1
                             70 STORE_FAST               2 (model)
                
-                89          72 PUSH_NULL
+               104          72 PUSH_NULL
                             74 LOAD_FAST                2 (model)
                             76 LOAD_METHOD              2 (all)
                             98 PRECALL                  0
                            102 CALL                     0
                            112 LOAD_ATTR                3 (prefetch_related)
                            122 LOAD_FAST                2 (model)
                            124 LOAD_ATTR                4 (_meta)
@@ -692,25 +910,25 @@
                            148 LOAD_CONST               0 (None)
                        >>  150 SEND                     3 (to 158)
                            152 YIELD_VALUE
                            154 RESUME                   3
                            156 JUMP_BACKWARD_NO_INTERRUPT     4 (to 150)
                        >>  158 STORE_FAST               3 (objects)
                
-                90         160 LOAD_CLOSURE             5 (render)
+               105         160 LOAD_CLOSURE             5 (render)
                            162 BUILD_TUPLE              1
-                           164 LOAD_CONST               3 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 90>)
+                           164 LOAD_CONST               3 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 105>)
                            166 MAKE_FUNCTION            8 (closure)
                            168 LOAD_FAST                3 (objects)
                            170 GET_ITER
                            172 PRECALL                  0
                            176 CALL                     0
                            186 STORE_FAST               4 (data)
                
-                91         188 LOAD_GLOBAL             13 (NULL + JSONResponse)
+               106         188 LOAD_GLOBAL             13 (NULL + JSONResponse)
                            200 LOAD_CONST               4 ('data')
                            202 LOAD_FAST                4 (data)
                            204 BUILD_MAP                1
                            206 PRECALL                  1
                            210 CALL                     1
                            220 RETURN_VALUE
                consts
@@ -725,32 +943,32 @@
                         0x87018702970064017400000000000000000000006602640284048a0288
                         026601640384088a0188016601640484087c00a001000000000000000000
                         0000000000000000000000a6000000ab0000000000000000004400a60000
                         00ab0000000000000000005300
                                    0 MAKE_CELL                1 (check)
                                    2 MAKE_CELL                2 (rel)
                      
-                      76           4 RESUME                   0
+                      91           4 RESUME                   0
                      
-                      77           6 LOAD_CONST               1 ('val')
+                      92           6 LOAD_CONST               1 ('val')
                                    8 LOAD_GLOBAL              0 (dict)
                                   20 BUILD_TUPLE              2
-                                  22 LOAD_CONST               2 (<code object rel, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 77>)
+                                  22 LOAD_CONST               2 (<code object rel, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 92>)
                                   24 MAKE_FUNCTION            4 (annotations)
                                   26 STORE_DEREF              2 (rel)
                      
-                      79          28 LOAD_CLOSURE             2 (rel)
+                      94          28 LOAD_CLOSURE             2 (rel)
                                   30 BUILD_TUPLE              1
-                                  32 LOAD_CONST               3 (<code object check, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 79>)
+                                  32 LOAD_CONST               3 (<code object check, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 94>)
                                   34 MAKE_FUNCTION            8 (closure)
                                   36 STORE_DEREF              1 (check)
                      
-                      86          38 LOAD_CLOSURE             1 (check)
+                     101          38 LOAD_CLOSURE             1 (check)
                                   40 BUILD_TUPLE              1
-                                  42 LOAD_CONST               4 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 86>)
+                                  42 LOAD_CONST               4 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 101>)
                                   44 MAKE_FUNCTION            8 (closure)
                                   46 LOAD_FAST                0 (dct)
                                   48 LOAD_METHOD              1 (items)
                                   70 PRECALL                  0
                                   74 CALL                     0
                                   84 GET_ITER
                                   86 PRECALL                  0
@@ -764,17 +982,17 @@
                            nlocals   : 1
                            stacksize : 7
                            flags     : 19
                            code
                               0x970064017c006402190000000000000000009b0064037c006404190000
                               000000000000009b0064057c006406190000000000000000009b0064079d
                               075300
-                            77           0 RESUME                   0
+                            92           0 RESUME                   0
                            
-                            78           2 LOAD_CONST               1 ('<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/')
+                            93           2 LOAD_CONST               1 ('<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/')
                                          4 LOAD_FAST                0 (val)
                                          6 LOAD_CONST               2 ('type')
                                          8 BINARY_SUBSCR
                                         18 FORMAT_VALUE             0
                                         20 LOAD_CONST               3 ('/')
                                         22 LOAD_FAST                0 (val)
                                         24 LOAD_CONST               4 ('id')
@@ -799,15 +1017,15 @@
                               '</a>'
                            names      ()
                            varnames   ('val',)
                            freevars   ()
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       'rel'
-                           firstlineno 77
+                           firstlineno 92
                            lnotab 0x0201
                         code
                            argcount  : 1
                            nlocals   : 1
                            stacksize : 4
                            flags     : 19
                            code
@@ -821,38 +1039,38 @@
                               00723d64017c00640219000000000000000000a002000000000000000000
                               0000000000000000000000a6000000ab0000000000000000007600722164
                               03a004000000000000000000000000000000000000000088016601640484
                               087c004400a6000000ab000000000000000000a6010000ab010000000000
                               00000053007c005300
                                          0 COPY_FREE_VARS           1
                            
-                            79           2 RESUME                   0
+                            94           2 RESUME                   0
                            
-                            80           4 LOAD_GLOBAL              1 (NULL + isinstance)
+                            95           4 LOAD_GLOBAL              1 (NULL + isinstance)
                                         16 LOAD_FAST                0 (val)
                                         18 LOAD_GLOBAL              2 (dict)
                                         30 PRECALL                  2
                                         34 CALL                     2
                                         44 POP_JUMP_FORWARD_IF_FALSE    33 (to 112)
                                         46 LOAD_CONST               1 ('repr')
                                         48 LOAD_FAST                0 (val)
                                         50 LOAD_METHOD              2 (keys)
                                         72 PRECALL                  0
                                         76 CALL                     0
                                         86 CONTAINS_OP              0
                                         88 POP_JUMP_FORWARD_IF_FALSE    11 (to 112)
                            
-                            81          90 PUSH_NULL
+                            96          90 PUSH_NULL
                                         92 LOAD_DEREF               1 (rel)
                                         94 LOAD_FAST                0 (val)
                                         96 PRECALL                  1
                                        100 CALL                     1
                                        110 RETURN_VALUE
                            
-                            82     >>  112 LOAD_GLOBAL              1 (NULL + isinstance)
+                            97     >>  112 LOAD_GLOBAL              1 (NULL + isinstance)
                                        124 LOAD_FAST                0 (val)
                                        126 LOAD_GLOBAL              6 (list)
                                        138 PRECALL                  2
                                        142 CALL                     2
                                        152 POP_JUMP_FORWARD_IF_FALSE    90 (to 334)
                                        154 LOAD_FAST                0 (val)
                                        156 POP_JUMP_FORWARD_IF_FALSE    88 (to 334)
@@ -870,29 +1088,29 @@
                                        218 BINARY_SUBSCR
                                        228 LOAD_METHOD              2 (keys)
                                        250 PRECALL                  0
                                        254 CALL                     0
                                        264 CONTAINS_OP              0
                                        266 POP_JUMP_FORWARD_IF_FALSE    33 (to 334)
                            
-                            83         268 LOAD_CONST               3 (' ')
+                            98         268 LOAD_CONST               3 (' ')
                                        270 LOAD_METHOD              4 (join)
                                        292 LOAD_CLOSURE             1 (rel)
                                        294 BUILD_TUPLE              1
-                                       296 LOAD_CONST               4 (<code object <genexpr>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 83>)
+                                       296 LOAD_CONST               4 (<code object <genexpr>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 98>)
                                        298 MAKE_FUNCTION            8 (closure)
                                        300 LOAD_FAST                0 (val)
                                        302 GET_ITER
                                        304 PRECALL                  0
                                        308 CALL                     0
                                        318 PRECALL                  1
                                        322 CALL                     1
                                        332 RETURN_VALUE
                            
-                            84     >>  334 LOAD_FAST                0 (val)
+                            99     >>  334 LOAD_FAST                0 (val)
                                        336 RETURN_VALUE
                            consts
                               None
                               'repr'
                               0
                               ' '
                               code
@@ -901,15 +1119,15 @@
                                  stacksize : 4
                                  flags     : 51
                                  code
                                     0x95014b00010097007c005d0f7d01020089027c01a6010000ab01000000
                                     00000000005600970101008c1064005300
                                                0 COPY_FREE_VARS           1
                                  
-                                  83           2 RETURN_GENERATOR
+                                  98           2 RETURN_GENERATOR
                                                4 POP_TOP
                                                6 RESUME                   0
                                                8 LOAD_FAST                0 (.0)
                                          >>   10 FOR_ITER                15 (to 42)
                                               12 STORE_FAST               1 (v)
                                               14 PUSH_NULL
                                               16 LOAD_DEREF               2 (rel)
@@ -926,35 +1144,35 @@
                                     None
                                  names      ()
                                  varnames   ('.0', 'v')
                                  freevars   ('rel',)
                                  cellvars   ()
                                  filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                                  name       '<genexpr>'
-                                 firstlineno 83
+                                 firstlineno 98
                                  lnotab 0x
                            names      ('isinstance', 'dict', 'keys', 'list', 'join')
                            varnames   ('val',)
                            freevars   ('rel',)
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       'check'
-                           firstlineno 79
+                           firstlineno 94
                            lnotab 0x0401560116019c014201
                         code
                            argcount  : 1
                            nlocals   : 3
                            stacksize : 5
                            flags     : 19
                            code
                               0x9501970067007c005d105c0200007d017d02020089037c02a6010000ab
                               01000000000000000091028c115300
                                          0 COPY_FREE_VARS           1
                            
-                            86           2 RESUME                   0
+                           101           2 RESUME                   0
                                          4 BUILD_LIST               0
                                          6 LOAD_FAST                0 (.0)
                                    >>    8 FOR_ITER                16 (to 42)
                                         10 UNPACK_SEQUENCE          2
                                         14 STORE_FAST               1 (key)
                                         16 STORE_FAST               2 (val)
                                         18 PUSH_NULL
@@ -968,36 +1186,36 @@
                            consts
                            names      ()
                            varnames   ('.0', 'key', 'val')
                            freevars   ('check',)
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       '<listcomp>'
-                           firstlineno 86
+                           firstlineno 101
                            lnotab 0x
                      names      ('dict', 'items')
                      varnames   ('dct',)
                      freevars   ()
                      cellvars   ('check', 'rel')
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       'render'
-                     firstlineno 76
+                     firstlineno 91
                      lnotab 0x060116020a07
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 7
                      flags     : 19
                      code
                         0x9501970067007c005d1a7d01020089027401000000000000000000007c
                         01a6010000ab010000000000000000a6010000ab01000000000000000091
                         028c1b5300
                                    0 COPY_FREE_VARS           1
                      
-                      90           2 RESUME                   0
+                     105           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                26 (to 62)
                                   10 STORE_FAST               1 (obj)
                                   12 PUSH_NULL
                                   14 LOAD_DEREF               2 (render)
                                   16 LOAD_GLOBAL              1 (NULL + jsonify)
@@ -1012,36 +1230,36 @@
                      consts
                      names      ('jsonify',)
                      varnames   ('.0', 'obj')
                      freevars   ('render',)
                      cellvars   ()
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       '<listcomp>'
-                     firstlineno 90
+                     firstlineno 105
                      lnotab 0x
                   'data'
                names      ('dict', '_get_model', 'all', 'prefetch_related', '_meta', 'fetch_fields', 'JSONResponse')
                varnames   ('self', 'request', 'model', 'objects', 'data')
                freevars   ()
                cellvars   ('render',)
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'dt'
-               firstlineno 75
+               firstlineno 90
                lnotab 0x0801160c2a0158011c01
-            (False, 'Admin', None, None)
-         names      ('__name__', '__module__', '__qualname__', 'bool', 'str', '__init__', 'start', 'Request', 'dash', 'index', 'dt', '__classcell__')
+            (False, 'Admin', None, None, None)
+         names      ('__name__', '__module__', '__qualname__', 'bool', 'str', 'callable', '__init__', 'start', 'Request', 'dash', 'index', 'edit', 'dt', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
          name       'Admin'
-         firstlineno 17
-         lnotab 0x0c0124230a060c070c09
+         firstlineno 16
+         lnotab 0x0c0128240a060c070c090c0f
       'Admin'
-   names      ('datetime', 'jinja2', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'starlette.requests', 'Request', 'starlette.responses', 'RedirectResponse', 'JSONResponse', 'starlette.routing', 'Mount', 'Route', 'starlette.staticfiles', 'StaticFiles', 'starlette.templating', 'Jinja2Templates', 'tortoise_api.api', 'Api', 'tortoise_api.util', 'jsonify', 'tortoise_api_model', 'Model', 'femto_admin', 'femto_admin.utils', '_fields', 'Admin')
+   names      ('datetime', 'jinja2', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'starlette.requests', 'Request', 'starlette.responses', 'RedirectResponse', 'JSONResponse', 'starlette.routing', 'Mount', 'Route', 'starlette.staticfiles', 'StaticFiles', 'starlette.templating', 'Jinja2Templates', 'tortoise_api.api', 'Api', 'tortoise_api.util', 'jsonify', 'tortoise_api_model', 'Model', 'femto_admin', 'Admin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c0214010c01100110010c010c010c010c010c0208010c03
+   lnotab 0x00ff02010c0214010c01100110010c010c010c010c010c020803
```

### Comparing `femto-admin-0.2.0/femto_admin/admin.py` & `femto-admin-0.2.2/femto_admin/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 from starlette.staticfiles import StaticFiles
 from starlette.templating import Jinja2Templates
 from tortoise_api.api import Api
 from tortoise_api.util import jsonify
 from tortoise_api_model import Model
 
 import femto_admin
-from femto_admin.utils import _fields
 
 
 class Admin(Api):
-    def __init__(self, debug: bool = False, title: str = "Admin", static_dir: str = None, logo: str|bool = None):
+    def __init__(self, debug: bool = False, title: str = "Admin", static_dir: str = None, logo: str|bool = None, dash_func: callable = None):
         """
         Parameters:
             title: Admin title.
             # auth_provider: Authentication Provider
         """
         super().__init__(debug)
         self.title = title
         # self._views: List[BaseView] = []
         self.routes: [Route | Mount] = [
-            Mount('/static', StaticFiles(packages=["femto_admin"]), name='public'),
+            Route('/', dash_func or self.dash),
             Mount('/api', routes=self.routes), # mount api routes to /api/*
+            Mount('/static', StaticFiles(packages=["femto_admin"]), name='public'),
             Route("/favicon.ico", lambda r: RedirectResponse('./static/placeholders/favicon.ico', status_code=301), methods=['GET']),
             Route('/{model}', self.index),
             Route('/dt/{model}', self.dt),
-            Route('/', self.dash),
+            Route('/{model}/{oid}', self.edit),
         ]
         self.routes[1].routes.pop(1)  # remove apt/favicon.ico route
         # globals
         templates = Jinja2Templates("templates")
         if static_dir:
             self.routes.append(Mount('/'+static_dir, StaticFiles(directory=static_dir), name='my-public'))
             if logo is not None:
@@ -61,19 +61,34 @@
             # 'model': 'Home',
             'subtitle': 'Dashboard',
             'request': request,
         })
 
     async def index(self, request: Request):
         model: type[Model] = self._get_model(request)
+        await model.load_rel_options()
         return self.templates.TemplateResponse("index.html", {
-            'model': model.__name__,
+            'model': model,
+            'subtitle': model._meta.table_description,
+            'request': request,
+        })
+
+    async def edit(self, request: Request):
+        model: type[Model] = self._get_model(request)
+        oid = request.path_params['oid']
+        await model.load_rel_options()
+        obj: Model = await model.get(id=oid).prefetch_related(*model._meta.fetch_fields)
+        bfms = [getattr(obj, k).remote_model for k in model._meta.backward_fk_fields]
+        [await bfm.load_rel_options() for bfm in bfms]
+        return self.templates.TemplateResponse("edit.html", {
+            'model': model,
             'subtitle': model._meta.table_description,
             'request': request,
-            'fields': await _fields(model),
+            'obj': obj,
+            'bfms': bfms,
         })
 
     async def dt(self, request: Request):
         def render(dct: dict):
             def rel(val: dict):
                 return f'<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/{val["type"]}/{val["id"]}">{val["repr"]}</a>'
             def check(val):
```

### Comparing `femto-admin-0.2.0/femto_admin/statics/js/polygon.js` & `femto-admin-0.2.2/femto_admin/statics/js/list_field.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,16 @@
             const field = el.closest(".field-list");
             const baseName = field.attr("id");
             const idx = field.children("#" + $.escapeSelector(baseName) + "-next-index").val();
             const template = $(field.children(".template").text());
 
             function update_attr(el, attr) {
                 $(`[${attr}]`, el).each(function() {
-                    $(this).attr(attr, baseName + "." + idx);
+                    const sfx = this.name.endsWith('[]') ? '[]' : ''
+                    $(this).attr(attr, baseName + "." + idx + sfx);
                 });
             }
             update_attr(template, "id");
             update_attr(template, "name");
             update_attr(template, "for");
 
             template.appendTo(field.children(".list-container"));
```

### Comparing `femto-admin-0.2.0/femto_admin/statics/placeholders/favicon.ico` & `femto-admin-0.2.2/femto_admin/statics/placeholders/favicon.ico`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/placeholders/users/admin.jpg` & `femto-admin-0.2.2/femto_admin/statics/placeholders/users/admin.jpg`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css` & `femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css` & `femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/jQuery/jquery.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.min.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.css` & `femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/tabler.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.min.css` & `femto-admin-0.2.2/femto_admin/statics/vendor/tabler/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/dark-theme.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/dark-theme.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/tabler.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.min.js` & `femto-admin-0.2.2/femto_admin/statics/vendor/tabler/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/aside.html` & `femto-admin-0.2.2/femto_admin/templates/components/aside.html`

 * *Files 13% similar despite different names*

```diff
@@ -13,31 +13,25 @@
                          width="110" height="32" alt="Tabler" class="navbar-brand-image"
                     >
                 {% endif %}
             </a>
         </h1>
         <div class="collapse navbar-collapse" id="sidebar-menu">
             <ul class="navbar-nav">
-                {% for item in models %}
+                {% for key, item in models.items() %}
                     <li class="nav-item">
-                        <a class="nav-link" href="/{{ item }}">
-                          <span class="nav-link-icon d-md-none d-lg-inline-block"><!-- Download SVG icon from https://tabler-icons.io/i/home -->
-                            <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24"
-                                 viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none"
-                                 stroke-linecap="round" stroke-linejoin="round">
-                                <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
-                                <path d="M5 12l-2 0l9 -9l9 9l-2 0"/>
-                                <path d="M5 12v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-7"/>
-                                <path d="M9 21v-6a2 2 0 0 1 2 -2h2a2 2 0 0 1 2 2v6"/>
-                            </svg>
+                        <a class="nav-link dropdown-item" href="/{{ key }}">
+                          <span class="nav-link-icon d-md-none d-lg-inline-block color">
+                              <i class="ti ti-{{ item._icon }}"></i>
                           </span>
-                            <span class="nav-link-title">{{ item }}</span>
+                          <span class="nav-link-title">{{ key }}</span>
                         </a>
                     </li>
                 {% endfor %}
+                {# todo: dropdowns #}
                 {#<li class="nav-item dropdown">
                     <a class="nav-link dropdown-toggle" href="#navbar-base" data-bs-toggle="dropdown" data-bs-auto-close="false" role="button" aria-expanded="false">
                       <span class="nav-link-icon d-md-none d-lg-inline-block"><!-- Download SVG icon from https://tabler-icons.io/i/package -->
                         <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
                              stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round"
                              stroke-linejoin="round">
                             <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 
 ****** {%_if_logo_==_False_%}_{{_title_}}_{%_else_%}_[Tabler]_{%_endif_%}
 ******
-    * {% for item in models %}
-    * ________{{_item_}}
-    * {% endfor %} {#
+    * {% for key, item in models.items() %}
+    *    {{_key_}}
+    * {% endfor %} {# todo: dropdowns #} {#
     * __________Interface
       ____Errors
     * #}
```

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/footer.html` & `femto-admin-0.2.2/femto_admin/templates/components/footer.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/header.html` & `femto-admin-0.2.2/femto_admin/templates/components/header.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/collection.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/collection.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {#{% if field.input!='list' %}<fieldset class="form-fieldset">{% endif %}#}
     <div class="form-group row">
         {% for label in field.labels %}
             <label class="col-2 col-form-label">{{ label }}</label>
-            {% with value=value and value[loop.index], step=field.step or field.base_field.step, field=field.base_field, width='4' %}
+            {% with value=value and value[loop.index], step=field.step or field.base_field.step, field=field.base_field, key=key+'[]', width='4' %}
                 {% include "components/inputs/"+field.input+".html" %}
             {% endwith %}
         {% endfor %}
     </div>
 {#{% if field.input!='list' %}</fieldset>{% endif %}#}
 {% include "components/inputs/_help.html" %}
```

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/datetime.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/datetime.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/editor.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/editor.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/json.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/json.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/list.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/list.html`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                 <div class="d-flex">
                     <div class="flex-grow-1">
                         {% with field=field.base_field %}
                             {% include "components/inputs/collection.html" %}
                         {% endwith %}
                     </div>
                     <button type="button" class="field-list-btn-remove btn btn-ghost-danger btn-icon mx-2 py-0">
-                        <b class="fa fa-close">x</b>
+                        <i class="ti ti-x"></i>
                     </button>
                 </div>
             </div>
         {% endfilter %}
     </div>
     <fieldset class="list-container form-fieldset d-flex flex-column">
         {% if (data or []) | length > 0 %}
@@ -34,9 +34,9 @@
             {% endfor %}
         {% endif %}
     </fieldset>
     <a type="button" class="field-list-btn-add mt-2"><i class="fa fa-add me-2"></i>Add item</a>
 </div>
 
 {% block scripts %}
-    <script src="{{ url_for('public', path='js/polygon.js') }}" defer></script>
+    <script src="{{ url_for('public', path='js/list_field.js') }}" defer></script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [{{ (data or []) | length }}]
 {% filter forceescape %}
 {% with field=field.base_field %} {% include "components/inputs/
 collection.html" %} {% endwith %}
- x
+
 {% endfilter %}
  {% if (data or []) | length > 0 %} {% for value in data %}
 {# {% with data=value, field=field._field_at(loop.index), error=error.get
 (loop.index0, None) if (error | is_dict) else None %}#} {% include "components/
 inputs/collection.html" %} {# {% endwith %}#}
  x
 {% endfor %} {% endif %}
```

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/many_to_many.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/many_to_many.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/radio.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/radio.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/inputs/range.html` & `femto-admin-0.2.2/femto_admin/templates/components/inputs/range.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% if field.template=='range' %}<fieldset class="form-fieldset">{% endif %}
     <div class="form-group row">
         <label class="col-2 col-form-label" for="lat">From</label>
         <div class="col-4">
-            <input type="number" class="form-control col-4" name="{{ key }}" placeholder="Man value" {% if disabled %}disabled{% endif %} value="{{ value and value[0] }}">
+            <input type="number" class="form-control col-4" name="{{ key }}[]" placeholder="Man value" {% if disabled %}disabled{% endif %} value="{{ value and value[0] }}">
         </div>
         <label class="col-2 col-form-label" for="lat">To</label>
         <div class="col-4">
-            <input type="number" class="form-control col-4" name="{{ key }}" placeholder="Max Value" {% if disabled %}disabled{% endif %} value="{{ value and value[1] }}">
+            <input type="number" class="form-control col-4" name="{{ key }}[]" placeholder="Max Value" {% if disabled %}disabled{% endif %} value="{{ value and value[1] }}">
         </div>
     </div>
 {% if field.template=='range' %}</fieldset>{% endif %}
 {% include "components/inputs/_help.html" %}
```

### Comparing `femto-admin-0.2.0/femto_admin/templates/components/notofications.html` & `femto-admin-0.2.2/femto_admin/templates/components/notofications.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.2.0/femto_admin/templates/layout.html` & `femto-admin-0.2.2/femto_admin/templates/layout.html`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 <head>
     <meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover"/>
     <meta http-equiv="X-UA-Compatible" content="ie=edge"/>
     <title>{{ title }}</title>
     <!-- CSS files -->
     <link href="{{ url_for('public', path='vendor/tabler/css/tabler.'+minify+'css') }}" rel="stylesheet"/>
+    <link href="{{ url_for('public', path='vendor/tabler/css/tabler-icons.'+minify+'css') }}" rel="stylesheet"/>
+    <link href="{{ url_for('public', path='css/main.css') }}" rel="stylesheet"/>
     {% block styles %}
     {% endblock %}
 </head>
 <body data-bs-theme="dark">
 <div class="page">
     <!-- Sidebar -->
     {% include "components/aside.html" %}
@@ -24,15 +26,15 @@
                 <div class="row g-2 align-items-center">
                     <div class="col">
                         <!-- Page pre-title -->
                         <div class="page-pretitle">
                             {{ subtitle or '' }}
                         </div>
                         <h2 class="page-title">
-                            {{ model or title or '' }}
+                            {{ (obj and model.__name__+': '+obj.repr()) or (model and model.__name__) or title or '' }}
                         </h2>
                     </div>
                     <!-- Page title actions -->
                     {% include "components/global_actions.html" %}
                 </div>
             </div>
         </div>
@@ -42,15 +44,15 @@
                 {% block body %}
                 {% endblock %}
             </div>
         </div>
         {% include "components/footer.html" %}
     </div>
 </div>
-{% if request.scope['endpoint'].__name__ in ['index'] %}
+{% if model %}
     {% include "components/modal.html" %}
 {% endif %}
 <script src="{{ url_for('public', path='vendor/tabler/js/dark-theme.'+minify+'js') }}"></script>
 <script src="{{ url_for('public', path='vendor/jQuery/jquery.'+minify+'js') }}"></script>
 <script src="{{ url_for('public', path='vendor/tabler/js/tabler.'+minify+'js') }}" defer></script>
 {% block scripts %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 
 
 
+
+
  {% block styles %} {% endblock %}
  {% include "components/aside.html" %}  {% include "components/header.html" %}
 {{ subtitle or '' }}
-***** {{ model or title or '' }} *****
+***** {{ (obj and model.__name__+': '+obj.repr()) or (model and model.__name__)
+or title or '' }} *****
  {% include "components/global_actions.html" %}
 {% block body %} {% endblock %}
 {% include "components/footer.html" %}
-{% if request.scope['endpoint'].__name__ in ['index'] %} {% include
-"components/modal.html" %} {% endif %}
+{% if model %} {% include "components/modal.html" %} {% endif %}
  {% block scripts %} {% endblock %}
```

### Comparing `femto-admin-0.2.0/femto_admin/templates/views/table.html` & `femto-admin-0.2.2/femto_admin/templates/views/table.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-{% macro table() -%}
+{% macro table(model) -%}
 
     <link href="{{ url_for('public', path='vendor/DataTables/css/dataTables.bootstrap5.'+minify+'css') }}" rel="stylesheet"/>
 
     <table id="dt" class="table table-striped" style="width:100%">
         <thead>
         <tr>
-            {% for field in fields %}
+            {% for field in model.field_input_map() %}
                 {% if not field.endswith('_id') %}
                     <th>{{ field }}</th>
                 {% endif %}
             {% endfor %}
         </tr>
         </thead>
     </table>
 
     <script defer src="{{ url_for('public', path='vendor/DataTables/js/jquery.dataTables.'+minify+'js') }}"></script>
     <script defer src="{{ url_for('public', path='vendor/DataTables/js/dataTables.bootstrap5.'+minify+'js') }}"></script>
     <script>
         document.addEventListener("DOMContentLoaded", function () {
-            new DataTable('#dt', {ajax: 'dt/{{ request.path_params["model"] }}'})
+            new DataTable('#dt', {ajax: '/dt/{{ model.__name__ }}'})
         });
     </script>
 
-{% endmacro %}
+{%- endmacro %}
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
-{% macro table() -%}
+{% macro table(model) -%}
 {{ field }}
- {% endmacro %}
+ {%- endmacro %}
```

### Comparing `femto-admin-0.2.0/femto_admin.egg-info/PKG-INFO` & `femto-admin-0.2.2/femto_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femto-admin
-Version: 0.2.0
+Version: 0.2.2
 Summary: Simplest fastest minimal ASGI CRUD Admin panel for Tortoise ORM models. It's generating fully native async auto  zero config one line app
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/femto-admin
 Project-URL: Repository, https://github.com/mixartemev/femto-admin
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `femto-admin-0.2.0/femto_admin.egg-info/SOURCES.txt` & `femto-admin-0.2.2/femto_admin.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 femto_admin/__init__.py
 femto_admin/admin.py
-femto_admin/consts.py
-femto_admin/utils.py
 femto_admin.egg-info/PKG-INFO
 femto_admin.egg-info/SOURCES.txt
 femto_admin.egg-info/dependency_links.txt
 femto_admin.egg-info/requires.txt
 femto_admin.egg-info/top_level.txt
 femto_admin/__pycache__/__init__.cpython-311.pyc
 femto_admin/__pycache__/admin.cpython-311.pyc
-femto_admin/__pycache__/consts.cpython-311.pyc
-femto_admin/__pycache__/utils.cpython-311.pyc
-femto_admin/statics/js/polygon.js
+femto_admin/statics/css/main.css
+femto_admin/statics/js/list_field.js
 femto_admin/statics/placeholders/favicon.ico
 femto_admin/statics/placeholders/logo/logo-white.svg
 femto_admin/statics/placeholders/users/admin.jpg
 femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
 femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
 femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
 femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
 femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
 femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
 femto_admin/statics/vendor/jQuery/jquery.js
 femto_admin/statics/vendor/jQuery/jquery.min.js
+femto_admin/statics/vendor/tabler/css/tabler-icons.css
+femto_admin/statics/vendor/tabler/css/tabler-icons.min.css
 femto_admin/statics/vendor/tabler/css/tabler.css
 femto_admin/statics/vendor/tabler/css/tabler.min.css
+femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.eot
+femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.ttf
+femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.woff
+femto_admin/statics/vendor/tabler/css/fonts/tabler-icons.woff2
 femto_admin/statics/vendor/tabler/js/dark-theme.js
 femto_admin/statics/vendor/tabler/js/dark-theme.min.js
 femto_admin/statics/vendor/tabler/js/tabler.js
 femto_admin/statics/vendor/tabler/js/tabler.min.js
 femto_admin/templates/dashboard.html
+femto_admin/templates/edit.html
 femto_admin/templates/index.html
 femto_admin/templates/layout.html
 femto_admin/templates/components/aside.html
 femto_admin/templates/components/footer.html
 femto_admin/templates/components/global_actions.html
 femto_admin/templates/components/header.html
 femto_admin/templates/components/modal.html
@@ -54,8 +58,9 @@
 femto_admin/templates/components/inputs/json.html
 femto_admin/templates/components/inputs/list.html
 femto_admin/templates/components/inputs/many_to_many.html
 femto_admin/templates/components/inputs/radio.html
 femto_admin/templates/components/inputs/range.html
 femto_admin/templates/components/inputs/select.html
 femto_admin/templates/components/inputs/textarea.html
+femto_admin/templates/views/form.html
 femto_admin/templates/views/table.html
```

### Comparing `femto-admin-0.2.0/pyproject.toml` & `femto-admin-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     {name = "Artemiev", email = "mixartemev@gmail.com"},
 ]
 keywords = ["starlette", "fastapi", "admin", "dashboard", "datatables", "crud", "tortoise-orm", "ASGI-admin"]
 description = "Simplest fastest minimal ASGI CRUD Admin panel for Tortoise ORM models. It's generating fully native async auto  zero config one line app"
 readme = "README.md"
 license = {text = "MIT"}
 dependencies = [
-    "tortoise-api >= 0.2.2",
+    "tortoise-api >= 0.2.4",
     "jinja2"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/femto-admin"
 Repository = "https://github.com/mixartemev/femto-admin"
```

