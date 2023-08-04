# Comparing `tmp/citrusdb-0.5.1.tar.gz` & `tmp/citrusdb-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.5.1.tar", last modified: Mon Jun 26 18:40:38 2023, max compression
+gzip compressed data, was "citrusdb-0.5.2.tar", last modified: Fri Aug  4 10:07:18 2023, max compression
```

## Comparing `citrusdb-0.5.1.tar` & `citrusdb-0.5.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.524660 citrusdb-0.5.1/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.5.1/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-26 18:40:38.524540 citrusdb-0.5.1/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1828 2023-06-19 14:22:45.000000 citrusdb-0.5.1/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.521252 citrusdb-0.5.1/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-16 18:28:46.000000 citrusdb-0.5.1/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.522228 citrusdb-0.5.1/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     4017 2023-06-19 15:43:59.000000 citrusdb-0.5.1/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     7418 2023-06-26 18:09:39.000000 citrusdb-0.5.1/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.522365 citrusdb-0.5.1/citrusdb/db/
--rw-r--r--   0 debabrata   (501) staff       (20)     1282 2023-06-26 15:57:37.000000 citrusdb-0.5.1/citrusdb/db/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.522624 citrusdb-0.5.1/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.5.1/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.523025 citrusdb-0.5.1/citrusdb/db/postgres/
--rw-r--r--   0 debabrata   (501) staff       (20)     6929 2023-06-26 18:09:32.000000 citrusdb-0.5.1/citrusdb/db/postgres/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1771 2023-06-26 17:28:44.000000 citrusdb-0.5.1/citrusdb/db/postgres/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1533 2023-06-19 15:14:26.000000 citrusdb-0.5.1/citrusdb/db/postgres/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.523466 citrusdb-0.5.1/citrusdb/db/sqlite/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.1/citrusdb/db/sqlite/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     5250 2023-06-26 15:54:34.000000 citrusdb-0.5.1/citrusdb/db/sqlite/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1742 2023-06-26 15:16:54.000000 citrusdb-0.5.1/citrusdb/db/sqlite/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1382 2023-06-19 15:10:21.000000 citrusdb-0.5.1/citrusdb/db/sqlite/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.523691 citrusdb-0.5.1/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.524032 citrusdb-0.5.1/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.1/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      236 2023-06-19 15:39:24.000000 citrusdb-0.5.1/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1018 2023-06-26 15:48:25.000000 citrusdb-0.5.1/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.521857 citrusdb-0.5.1/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      792 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/top_level.txt
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.524371 citrusdb-0.5.1/cloud-temp/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.5.1/cloud-temp/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2248 2023-06-16 13:03:05.000000 citrusdb-0.5.1/cloud-temp/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2826 2023-06-16 18:18:23.000000 citrusdb-0.5.1/cloud-temp/main-pg.py
--rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-06-26 18:39:30.000000 citrusdb-0.5.1/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-26 18:40:38.524691 citrusdb-0.5.1/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-06-26 18:39:42.000000 citrusdb-0.5.1/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.619748 citrusdb-0.5.2/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.5.2/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2300 2023-08-04 10:07:18.619629 citrusdb-0.5.2/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1717 2023-08-04 10:05:38.000000 citrusdb-0.5.2/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.616413 citrusdb-0.5.2/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-16 18:28:46.000000 citrusdb-0.5.2/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617290 citrusdb-0.5.2/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     4050 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     9141 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617407 citrusdb-0.5.2/citrusdb/db/
+-rw-r--r--   0 debabrata   (501) staff       (20)     1426 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617597 citrusdb-0.5.2/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.5.2/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617927 citrusdb-0.5.2/citrusdb/db/postgres/
+-rw-r--r--   0 debabrata   (501) staff       (20)     7767 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/postgres/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1866 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/postgres/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1533 2023-06-27 16:19:28.000000 citrusdb-0.5.2/citrusdb/db/postgres/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.618327 citrusdb-0.5.2/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.2/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     5989 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1836 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1382 2023-06-27 16:19:28.000000 citrusdb-0.5.2/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.618835 citrusdb-0.5.2/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/embedding/openai.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      297 2023-08-04 09:37:45.000000 citrusdb-0.5.2/citrusdb/embedding/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.619197 citrusdb-0.5.2/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.2/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      236 2023-06-27 16:19:28.000000 citrusdb-0.5.2/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1479 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.616938 citrusdb-0.5.2/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2300 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      820 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/top_level.txt
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.619482 citrusdb-0.5.2/cloud-temp/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.5.2/cloud-temp/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2248 2023-06-16 13:03:05.000000 citrusdb-0.5.2/cloud-temp/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2826 2023-06-16 18:18:23.000000 citrusdb-0.5.2/cloud-temp/main-pg.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-08-04 10:07:00.000000 citrusdb-0.5.2/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-08-04 10:07:18.619779 citrusdb-0.5.2/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-08-04 10:07:14.000000 citrusdb-0.5.2/setup.py
```

### Comparing `citrusdb-0.5.1/LICENSE` & `citrusdb-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.1/PKG-INFO` & `citrusdb-0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6369 7472  : 2.1.Name: citr
 00000020: 7573 6462 0a56 6572 7369 6f6e 3a20 302e  usdb.Version: 0.
-00000030: 352e 310a 5375 6d6d 6172 793a 206f 7065  5.1.Summary: ope
+00000030: 352e 320a 5375 6d6d 6172 793a 206f 7065  5.2.Summary: ope
 00000040: 6e2d 736f 7572 6365 2076 6563 746f 7220  n-source vector 
 00000050: 6461 7461 6261 7365 2e20 7374 6f72 6520  database. store 
 00000060: 616e 6420 7265 7472 6965 7665 2065 6d62  and retrieve emb
 00000070: 6564 6469 6e67 7320 666f 7220 796f 7572  eddings for your
 00000080: 206e 6578 7420 7072 6f6a 6563 7421 0a48   next project!.H
 00000090: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
 000000a0: 2f2f 6769 7468 7562 2e63 6f6d 2f30 7844  //github.com/0xD
@@ -34,118 +34,111 @@
 00000210: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 00000220: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 00000230: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 00000240: 4345 4e53 450a 0a23 20f0 9f8d 8b20 6369  CENSE..# .... ci
 00000250: 7472 7573 2e0a 2323 2320 6f70 656e 2d73  trus..### open-s
 00000260: 6f75 7263 6520 2864 6973 7472 6962 7574  ource (distribut
 00000270: 6564 2920 7665 6374 6f72 2064 6174 6162  ed) vector datab
-00000280: 6173 650a 0a3c 7020 616c 6967 6e3d 2263  ase..<p align="c
-00000290: 656e 7465 7222 3e0a 2020 5370 6563 6961  enter">.  Specia
-000002a0: 6c20 7468 616e 6b73 2074 6f0a 3c2f 703e  l thanks to.</p>
-000002b0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000002c0: 7222 3e0a 2020 3c69 6d67 2061 6c69 676e  r">.  <img align
-000002d0: 3d22 6365 6e74 6572 2220 7372 633d 2268  ="center" src="h
-000002e0: 7474 7073 3a2f 2f77 7777 2e67 6574 6465  ttps://www.getde
-000002f0: 766b 6974 2e63 6f6d 2f6c 6f67 6f2e 706e  vkit.com/logo.pn
-00000300: 6722 2077 6964 7468 3d31 3030 2068 6569  g" width=100 hei
-00000310: 6768 743d 3130 3020 616c 743d 2244 6576  ght=100 alt="Dev
-00000320: 4b69 7422 202f 3e0a 3c2f 703e 0a3c 7020  Kit" />.</p>.<p 
-00000330: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000340: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000350: 3a2f 2f77 7777 2e67 6574 6465 766b 6974  ://www.getdevkit
-00000360: 2e63 6f6d 223e 4465 764b 6974 202d 2054  .com">DevKit - T
-00000370: 6865 2045 7373 656e 7469 616c 2044 6576  he Essential Dev
-00000380: 656c 6f70 6572 2054 6f6f 6c6b 6974 3c2f  eloper Toolkit</
-00000390: 613e 3c62 7220 2f3e 0a20 2044 536f 4320  a><br />.  DSoC 
-000003a0: 3230 3233 0a3c 2f70 3e0a 0a0a 2323 2049  2023.</p>...## I
-000003b0: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
-000003c0: 0a70 6970 2069 6e73 7461 6c6c 2063 6974  .pip install cit
-000003d0: 7275 7364 620a 6060 600a 0a23 2320 4765  rusdb.```..## Ge
-000003e0: 7474 696e 6720 7374 6172 7465 640a 0a23  tting started..#
-000003f0: 2323 2320 312e 2043 7265 6174 6520 696e  ### 1. Create in
-00000400: 6465 780a 6060 6070 790a 696d 706f 7274  dex.```py.import
-00000410: 2063 6974 7275 7364 620a 0a23 2049 6e69   citrusdb..# Ini
-00000420: 7469 616c 697a 6520 636c 6965 6e74 0a63  tialize client.c
-00000430: 6974 7275 7320 3d20 6369 7472 7573 6462  itrus = citrusdb
-00000440: 2e43 6c69 656e 7428 290a 0a23 2043 7265  .Client()..# Cre
-00000450: 6174 6520 696e 6465 780a 6369 7472 7573  ate index.citrus
-00000460: 2e63 7265 6174 655f 696e 6465 7828 0a20  .create_index(. 
-00000470: 206e 616d 653d 2265 7861 6d70 6c65 222c   name="example",
-00000480: 0a20 206d 6178 5f65 6c65 6d65 6e74 733d  .  max_elements=
-00000490: 3130 3030 2c20 2020 2020 2020 2020 2020  1000,           
-000004a0: 2023 2069 6e63 7265 6173 6573 2064 796e   # increases dyn
-000004b0: 616d 6963 616c 6c79 2061 7320 796f 7520  amically as you 
-000004c0: 696e 7365 7274 206d 6f72 6520 7665 6374  insert more vect
-000004d0: 6f72 730a 290a 6060 600a 0a23 2323 2320  ors.).```..#### 
-000004e0: 322e 2049 6e73 6572 7420 656c 656d 656e  2. Insert elemen
-000004f0: 7473 0a60 6060 7079 0a69 6473 203d 205b  ts.```py.ids = [
-00000500: 312c 2032 2c20 335d 0a64 6f63 756d 656e  1, 2, 3].documen
-00000510: 7473 203d 205b 0a20 2022 596f 7572 2074  ts = [.  "Your t
-00000520: 696d 6520 6973 206c 696d 6974 6564 2c20  ime is limited, 
-00000530: 736f 2064 6f6e 2774 2077 6173 7465 2069  so don't waste i
-00000540: 7420 6c69 7669 6e67 2073 6f6d 656f 6e65  t living someone
-00000550: 2065 6c73 6527 7320 6c69 6665 222c 0a20   else's life",. 
-00000560: 2022 4927 6420 7261 7468 6572 2062 6520   "I'd rather be 
-00000570: 6f70 7469 6d69 7374 6963 2061 6e64 2077  optimistic and w
-00000580: 726f 6e67 2074 6861 6e20 7065 7373 696d  rong than pessim
-00000590: 6973 7469 6320 616e 6420 7269 6768 742e  istic and right.
-000005a0: 222c 0a20 2022 5275 6e6e 696e 6720 6120  ",.  "Running a 
-000005b0: 7374 6172 742d 7570 2069 7320 6c69 6b65  start-up is like
-000005c0: 2063 6865 7769 6e67 2067 6c61 7373 2061   chewing glass a
-000005d0: 6e64 2073 7461 7269 6e67 2069 6e74 6f20  nd staring into 
-000005e0: 7468 6520 6162 7973 732e 220a 5d0a 0a63  the abyss.".]..c
-000005f0: 6974 7275 732e 6164 6428 696e 6465 783d  itrus.add(index=
-00000600: 2265 7861 6d70 6c65 222c 2069 6473 3d69  "example", ids=i
-00000610: 6473 2c20 646f 6375 6d65 6e74 733d 646f  ds, documents=do
-00000620: 6375 6d65 6e74 7329 0a60 6060 0a59 6f75  cuments).```.You
-00000630: 2063 616e 2064 6972 6563 746c 7920 7061   can directly pa
-00000640: 7373 2076 6563 746f 7220 656d 6265 6464  ss vector embedd
-00000650: 696e 6773 2061 7320 7765 6c6c 2e20 4966  ings as well. If
-00000660: 2079 6f75 2772 6520 7061 7373 696e 6720   you're passing 
-00000670: 6120 6c69 7374 206f 6620 7374 7269 6e67  a list of string
-00000680: 7320 6c69 6b65 2077 6520 6861 7665 2064  s like we have d
-00000690: 6f6e 6520 6865 7265 2c20 656e 7375 7265  one here, ensure
-000006a0: 2079 6f75 2068 6176 6520 796f 7572 2060   you have your `
-000006b0: 4f50 454e 4149 5f41 5049 5f4b 4559 6020  OPENAI_API_KEY` 
-000006c0: 696e 2074 6865 2065 6e76 6972 6f6e 6d65  in the environme
-000006d0: 6e74 2e20 4279 2064 6566 6175 6c74 2077  nt. By default w
-000006e0: 6520 7573 6520 4f70 656e 4149 2074 6f20  e use OpenAI to 
-000006f0: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
-00000700: 656d 6265 6464 696e 6773 2e20 506c 6561  embeddings. Plea
-00000710: 7365 2072 6561 6368 206f 7574 2069 6620  se reach out if 
-00000720: 796f 7527 7265 206c 6f6f 6b69 6e67 2066  you're looking f
-00000730: 6f72 2073 7570 706f 7274 2066 726f 6d20  or support from 
-00000740: 6120 6469 6666 6572 656e 7420 7072 6f76  a different prov
-00000750: 6964 6572 210a 0a23 2323 2320 332e 2053  ider!..#### 3. S
-00000760: 6561 7263 680a 6060 6070 790a 7265 7375  earch.```py.resu
-00000770: 6c74 2c20 6469 7374 616e 6365 7320 3d20  lt, distances = 
-00000780: 6369 7472 7573 2e71 7565 7279 2869 6e64  citrus.query(ind
-00000790: 6578 3d22 6578 616d 706c 6522 2c20 646f  ex="example", do
-000007a0: 6375 6d65 6e74 733d 5b22 5768 6174 2069  cuments=["What i
-000007b0: 7320 6974 206c 696b 6520 746f 206c 6175  s it like to lau
-000007c0: 6e63 6820 6120 7374 6172 7475 7022 5d2c  nch a startup"],
-000007d0: 206b 3d31 290a 6060 600a 476f 206c 6175   k=1).```.Go lau
-000007e0: 6e63 6820 6120 7265 706c 206f 6e20 5b52  nch a repl on [R
-000007f0: 6570 6c69 745d 2868 7474 7073 3a2f 2f72  eplit](https://r
-00000800: 6570 6c69 742e 636f 6d29 2061 6e64 2073  eplit.com) and s
-00000810: 6565 2077 6861 7420 7265 7375 6c74 2079  ee what result y
-00000820: 6f75 2067 6574 2061 6674 6572 2072 756e  ou get after run
-00000830: 6e69 6e67 2074 6865 2071 7565 7279 2120  ning the query! 
-00000840: 6072 6573 756c 7460 2077 696c 6c20 636f  `result` will co
-00000850: 6e74 6169 6e20 7468 6520 6069 6473 6020  ntain the `ids` 
-00000860: 6f66 2074 6865 2074 6f70 2060 6b60 2073  of the top `k` s
-00000870: 6561 7263 6820 6869 7473 2e0a 0a23 2320  earch hits...## 
-00000880: 4578 616d 706c 650a 5b70 6f6b 6564 6578  Example.[pokedex
-00000890: 2073 6561 7263 685d 2868 7474 7073 3a2f   search](https:/
-000008a0: 2f72 6570 6c69 742e 636f 6d2f 4064 6562  /replit.com/@deb
-000008b0: 6162 7261 7461 6a72 2f70 6f6b 6564 6578  abratajr/pokedex
-000008c0: 2d73 6561 7263 6829 0a0a 2323 2046 6163  -search)..## Fac
-000008d0: 696e 6720 6973 7375 6573 3f0a 4665 656c  ing issues?.Feel
-000008e0: 2066 7265 6520 746f 206f 7065 6e20 6973   free to open is
-000008f0: 7375 6573 206f 6e20 7468 6973 2072 6570  sues on this rep
-00000900: 6f73 6974 6f72 7921 2044 6973 636f 7264  ository! Discord
-00000910: 2073 6572 7665 7220 636f 6d69 6e67 2073   server coming s
-00000920: 6f6f 6e21 0a0a 5053 3a20 6369 7472 7573  oon!..PS: citrus
-00000930: 2069 736e 2774 2064 6973 7472 6962 7574   isn't distribut
-00000940: 6564 206a 7573 7420 7965 742e 2057 6527  ed just yet. We'
-00000950: 7265 2067 6574 7469 6e67 2074 6865 7265  re getting there
-00000960: 2074 686f 7567 6820 3b29 0a               though ;).
+00000280: 6173 650a 0a23 2320 496e 7374 616c 6c61  ase..## Installa
+00000290: 7469 6f6e 0a0a 6060 600a 7069 7020 696e  tion..```.pip in
+000002a0: 7374 616c 6c20 6369 7472 7573 6462 0a60  stall citrusdb.`
+000002b0: 6060 0a0a 2323 2047 6574 7469 6e67 2073  ``..## Getting s
+000002c0: 7461 7274 6564 0a0a 2323 2323 2031 2e20  tarted..#### 1. 
+000002d0: 4372 6561 7465 2069 6e64 6578 0a60 6060  Create index.```
+000002e0: 7079 0a69 6d70 6f72 7420 6369 7472 7573  py.import citrus
+000002f0: 6462 0a0a 2320 496e 6974 6961 6c69 7a65  db..# Initialize
+00000300: 2063 6c69 656e 740a 6369 7472 7573 203d   client.citrus =
+00000310: 2063 6974 7275 7364 622e 436c 6965 6e74   citrusdb.Client
+00000320: 2829 0a0a 2320 4372 6561 7465 2069 6e64  ()..# Create ind
+00000330: 6578 0a63 6974 7275 732e 6372 6561 7465  ex.citrus.create
+00000340: 5f69 6e64 6578 280a 2020 6e61 6d65 3d22  _index(.  name="
+00000350: 6578 616d 706c 6522 2c0a 2020 6d61 785f  example",.  max_
+00000360: 656c 656d 656e 7473 3d31 3030 302c 2020  elements=1000,  
+00000370: 2020 2020 2020 2020 2020 2320 696e 6372            # incr
+00000380: 6561 7365 7320 6479 6e61 6d69 6361 6c6c  eases dynamicall
+00000390: 7920 6173 2079 6f75 2069 6e73 6572 7420  y as you insert 
+000003a0: 6d6f 7265 2076 6563 746f 7273 0a29 0a60  more vectors.).`
+000003b0: 6060 0a0a 2323 2323 2032 2e20 496e 7365  ``..#### 2. Inse
+000003c0: 7274 2065 6c65 6d65 6e74 730a 6060 6070  rt elements.```p
+000003d0: 790a 6964 7320 3d20 5b31 2c20 322c 2033  y.ids = [1, 2, 3
+000003e0: 5d0a 646f 6375 6d65 6e74 7320 3d20 5b0a  ].documents = [.
+000003f0: 2020 2259 6f75 7220 7469 6d65 2069 7320    "Your time is 
+00000400: 6c69 6d69 7465 642c 2073 6f20 646f 6e27  limited, so don'
+00000410: 7420 7761 7374 6520 6974 206c 6976 696e  t waste it livin
+00000420: 6720 736f 6d65 6f6e 6520 656c 7365 2773  g someone else's
+00000430: 206c 6966 6522 2c0a 2020 2249 2764 2072   life",.  "I'd r
+00000440: 6174 6865 7220 6265 206f 7074 696d 6973  ather be optimis
+00000450: 7469 6320 616e 6420 7772 6f6e 6720 7468  tic and wrong th
+00000460: 616e 2070 6573 7369 6d69 7374 6963 2061  an pessimistic a
+00000470: 6e64 2072 6967 6874 2e22 2c0a 2020 2252  nd right.",.  "R
+00000480: 756e 6e69 6e67 2061 2073 7461 7274 2d75  unning a start-u
+00000490: 7020 6973 206c 696b 6520 6368 6577 696e  p is like chewin
+000004a0: 6720 676c 6173 7320 616e 6420 7374 6172  g glass and star
+000004b0: 696e 6720 696e 746f 2074 6865 2061 6279  ing into the aby
+000004c0: 7373 2e22 0a5d 0a0a 6369 7472 7573 2e61  ss.".]..citrus.a
+000004d0: 6464 2869 6e64 6578 3d22 6578 616d 706c  dd(index="exampl
+000004e0: 6522 2c20 6964 733d 6964 732c 2064 6f63  e", ids=ids, doc
+000004f0: 756d 656e 7473 3d64 6f63 756d 656e 7473  uments=documents
+00000500: 290a 6060 600a 596f 7520 6361 6e20 6469  ).```.You can di
+00000510: 7265 6374 6c79 2070 6173 7320 7665 6374  rectly pass vect
+00000520: 6f72 2065 6d62 6564 6469 6e67 7320 6173  or embeddings as
+00000530: 2077 656c 6c2e 2049 6620 796f 7527 7265   well. If you're
+00000540: 2070 6173 7369 6e67 2061 206c 6973 7420   passing a list 
+00000550: 6f66 2073 7472 696e 6773 206c 696b 6520  of strings like 
+00000560: 7765 2068 6176 6520 646f 6e65 2068 6572  we have done her
+00000570: 652c 2065 6e73 7572 6520 796f 7520 6861  e, ensure you ha
+00000580: 7665 2079 6f75 7220 604f 5045 4e41 495f  ve your `OPENAI_
+00000590: 4150 495f 4b45 5960 2069 6e20 7468 6520  API_KEY` in the 
+000005a0: 656e 7669 726f 6e6d 656e 742e 2042 7920  environment. By 
+000005b0: 6465 6661 756c 7420 7765 2075 7365 204f  default we use O
+000005c0: 7065 6e41 4920 746f 2074 6f20 6765 6e65  penAI to to gene
+000005d0: 7261 7465 2074 6865 2065 6d62 6564 6469  rate the embeddi
+000005e0: 6e67 732e 2050 6c65 6173 6520 7265 6163  ngs. Please reac
+000005f0: 6820 6f75 7420 6966 2079 6f75 2772 6520  h out if you're 
+00000600: 6c6f 6f6b 696e 6720 666f 7220 7375 7070  looking for supp
+00000610: 6f72 7420 6672 6f6d 2061 2064 6966 6665  ort from a diffe
+00000620: 7265 6e74 2070 726f 7669 6465 7221 0a0a  rent provider!..
+00000630: 2323 2323 2033 2e20 5365 6172 6368 0a60  #### 3. Search.`
+00000640: 6060 7079 0a72 6573 756c 7473 203d 2063  ``py.results = c
+00000650: 6974 7275 732e 7175 6572 7928 0a20 2020  itrus.query(.   
+00000660: 2069 6e64 6578 3d22 6578 616d 706c 6522   index="example"
+00000670: 2c0a 2020 2020 646f 6375 6d65 6e74 733d  ,.    documents=
+00000680: 5b22 5768 6174 2069 7320 6974 206c 696b  ["What is it lik
+00000690: 6520 746f 206c 6175 6e63 6820 6120 7374  e to launch a st
+000006a0: 6172 7475 7022 5d2c 0a20 2020 206b 3d31  artup"],.    k=1
+000006b0: 2c0a 2020 2020 696e 636c 7564 653d 5b22  ,.    include=["
+000006c0: 646f 6375 6d65 6e74 222c 2022 6d65 7461  document", "meta
+000006d0: 6461 7461 225d 0a29 0a0a 7072 696e 7428  data"].)..print(
+000006e0: 7265 7375 6c74 7329 0a60 6060 0a59 6f75  results).```.You
+000006f0: 2063 616e 2073 7065 6369 6679 2069 6620   can specify if 
+00000700: 796f 7520 7761 6e74 2074 6865 2061 7373  you want the ass
+00000710: 6f63 6961 7465 6420 7465 7874 2064 6f63  ociated text doc
+00000720: 756d 656e 7420 616e 6420 6d65 7461 6461  ument and metada
+00000730: 7461 2074 6f20 6265 2072 6574 7572 6e65  ta to be returne
+00000740: 642e 0a42 7920 6465 6661 756c 742c 206f  d..By default, o
+00000750: 6e6c 7920 7468 6520 4944 7320 6172 6520  nly the IDs are 
+00000760: 7265 7475 726e 6564 2e0a 0a47 6f20 6c61  returned...Go la
+00000770: 756e 6368 2061 2072 6570 6c20 6f6e 205b  unch a repl on [
+00000780: 5265 706c 6974 5d28 6874 7470 733a 2f2f  Replit](https://
+00000790: 7265 706c 6974 2e63 6f6d 2920 616e 6420  replit.com) and 
+000007a0: 7365 6520 7768 6174 2072 6573 756c 7420  see what result 
+000007b0: 796f 7520 6765 7420 6166 7465 7220 7275  you get after ru
+000007c0: 6e6e 696e 6720 7468 6520 7175 6572 7921  nning the query!
+000007d0: 2060 7265 7375 6c74 6020 7769 6c6c 2063   `result` will c
+000007e0: 6f6e 7461 696e 2074 6865 2060 6964 7360  ontain the `ids`
+000007f0: 206f 6620 7468 6520 746f 7020 606b 6020   of the top `k` 
+00000800: 7365 6172 6368 2068 6974 732e 0a0a 2323  search hits...##
+00000810: 2045 7861 6d70 6c65 0a5b 706f 6b65 6465   Example.[pokede
+00000820: 7820 7365 6172 6368 5d28 6874 7470 733a  x search](https:
+00000830: 2f2f 7265 706c 6974 2e63 6f6d 2f40 6465  //replit.com/@de
+00000840: 6261 6272 6174 616a 722f 706f 6b65 6465  babratajr/pokede
+00000850: 782d 7365 6172 6368 290a 0a23 2320 4661  x-search)..## Fa
+00000860: 6369 6e67 2069 7373 7565 733f 0a46 6565  cing issues?.Fee
+00000870: 6c20 6672 6565 2074 6f20 6f70 656e 2069  l free to open i
+00000880: 7373 7565 7320 6f6e 2074 6869 7320 7265  ssues on this re
+00000890: 706f 7369 746f 7279 2120 4469 7363 6f72  pository! Discor
+000008a0: 6420 7365 7276 6572 2063 6f6d 696e 6720  d server coming 
+000008b0: 736f 6f6e 210a 0a50 533a 2063 6974 7275  soon!..PS: citru
+000008c0: 7320 6973 6e27 7420 6469 7374 7269 6275  s isn't distribu
+000008d0: 7465 6420 6a75 7374 2079 6574 2e20 5765  ted just yet. We
+000008e0: 2772 6520 6765 7474 696e 6720 7468 6572  're getting ther
+000008f0: 6520 7468 6f75 6768 203b 290a            e though ;).
```

### Comparing `citrusdb-0.5.1/README.md` & `citrusdb-0.5.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,108 @@
 00000000: 2320 f09f 8d8b 2063 6974 7275 732e 0a23  # .... citrus..#
 00000010: 2323 206f 7065 6e2d 736f 7572 6365 2028  ## open-source (
 00000020: 6469 7374 7269 6275 7465 6429 2076 6563  distributed) vec
-00000030: 746f 7220 6461 7461 6261 7365 0a0a 3c70  tor database..<p
-00000040: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000050: 0a20 2053 7065 6369 616c 2074 6861 6e6b  .  Special thank
-00000060: 7320 746f 0a3c 2f70 3e0a 3c70 2061 6c69  s to.</p>.<p ali
-00000070: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
-00000080: 696d 6720 616c 6967 6e3d 2263 656e 7465  img align="cente
-00000090: 7222 2073 7263 3d22 6874 7470 733a 2f2f  r" src="https://
-000000a0: 7777 772e 6765 7464 6576 6b69 742e 636f  www.getdevkit.co
-000000b0: 6d2f 6c6f 676f 2e70 6e67 2220 7769 6474  m/logo.png" widt
-000000c0: 683d 3130 3020 6865 6967 6874 3d31 3030  h=100 height=100
-000000d0: 2061 6c74 3d22 4465 764b 6974 2220 2f3e   alt="DevKit" />
-000000e0: 0a3c 2f70 3e0a 3c70 2061 6c69 676e 3d22  .</p>.<p align="
-000000f0: 6365 6e74 6572 223e 0a20 203c 6120 6872  center">.  <a hr
-00000100: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-00000110: 6765 7464 6576 6b69 742e 636f 6d22 3e44  getdevkit.com">D
-00000120: 6576 4b69 7420 2d20 5468 6520 4573 7365  evKit - The Esse
-00000130: 6e74 6961 6c20 4465 7665 6c6f 7065 7220  ntial Developer 
-00000140: 546f 6f6c 6b69 743c 2f61 3e3c 6272 202f  Toolkit</a><br /
-00000150: 3e0a 2020 4453 6f43 2032 3032 330a 3c2f  >.  DSoC 2023.</
-00000160: 703e 0a0a 0a23 2320 496e 7374 616c 6c61  p>...## Installa
-00000170: 7469 6f6e 0a0a 6060 600a 7069 7020 696e  tion..```.pip in
-00000180: 7374 616c 6c20 6369 7472 7573 6462 0a60  stall citrusdb.`
-00000190: 6060 0a0a 2323 2047 6574 7469 6e67 2073  ``..## Getting s
-000001a0: 7461 7274 6564 0a0a 2323 2323 2031 2e20  tarted..#### 1. 
-000001b0: 4372 6561 7465 2069 6e64 6578 0a60 6060  Create index.```
-000001c0: 7079 0a69 6d70 6f72 7420 6369 7472 7573  py.import citrus
-000001d0: 6462 0a0a 2320 496e 6974 6961 6c69 7a65  db..# Initialize
-000001e0: 2063 6c69 656e 740a 6369 7472 7573 203d   client.citrus =
-000001f0: 2063 6974 7275 7364 622e 436c 6965 6e74   citrusdb.Client
-00000200: 2829 0a0a 2320 4372 6561 7465 2069 6e64  ()..# Create ind
-00000210: 6578 0a63 6974 7275 732e 6372 6561 7465  ex.citrus.create
-00000220: 5f69 6e64 6578 280a 2020 6e61 6d65 3d22  _index(.  name="
-00000230: 6578 616d 706c 6522 2c0a 2020 6d61 785f  example",.  max_
-00000240: 656c 656d 656e 7473 3d31 3030 302c 2020  elements=1000,  
-00000250: 2020 2020 2020 2020 2020 2320 696e 6372            # incr
-00000260: 6561 7365 7320 6479 6e61 6d69 6361 6c6c  eases dynamicall
-00000270: 7920 6173 2079 6f75 2069 6e73 6572 7420  y as you insert 
-00000280: 6d6f 7265 2076 6563 746f 7273 0a29 0a60  more vectors.).`
-00000290: 6060 0a0a 2323 2323 2032 2e20 496e 7365  ``..#### 2. Inse
-000002a0: 7274 2065 6c65 6d65 6e74 730a 6060 6070  rt elements.```p
-000002b0: 790a 6964 7320 3d20 5b31 2c20 322c 2033  y.ids = [1, 2, 3
-000002c0: 5d0a 646f 6375 6d65 6e74 7320 3d20 5b0a  ].documents = [.
-000002d0: 2020 2259 6f75 7220 7469 6d65 2069 7320    "Your time is 
-000002e0: 6c69 6d69 7465 642c 2073 6f20 646f 6e27  limited, so don'
-000002f0: 7420 7761 7374 6520 6974 206c 6976 696e  t waste it livin
-00000300: 6720 736f 6d65 6f6e 6520 656c 7365 2773  g someone else's
-00000310: 206c 6966 6522 2c0a 2020 2249 2764 2072   life",.  "I'd r
-00000320: 6174 6865 7220 6265 206f 7074 696d 6973  ather be optimis
-00000330: 7469 6320 616e 6420 7772 6f6e 6720 7468  tic and wrong th
-00000340: 616e 2070 6573 7369 6d69 7374 6963 2061  an pessimistic a
-00000350: 6e64 2072 6967 6874 2e22 2c0a 2020 2252  nd right.",.  "R
-00000360: 756e 6e69 6e67 2061 2073 7461 7274 2d75  unning a start-u
-00000370: 7020 6973 206c 696b 6520 6368 6577 696e  p is like chewin
-00000380: 6720 676c 6173 7320 616e 6420 7374 6172  g glass and star
-00000390: 696e 6720 696e 746f 2074 6865 2061 6279  ing into the aby
-000003a0: 7373 2e22 0a5d 0a0a 6369 7472 7573 2e61  ss.".]..citrus.a
-000003b0: 6464 2869 6e64 6578 3d22 6578 616d 706c  dd(index="exampl
-000003c0: 6522 2c20 6964 733d 6964 732c 2064 6f63  e", ids=ids, doc
-000003d0: 756d 656e 7473 3d64 6f63 756d 656e 7473  uments=documents
-000003e0: 290a 6060 600a 596f 7520 6361 6e20 6469  ).```.You can di
-000003f0: 7265 6374 6c79 2070 6173 7320 7665 6374  rectly pass vect
-00000400: 6f72 2065 6d62 6564 6469 6e67 7320 6173  or embeddings as
-00000410: 2077 656c 6c2e 2049 6620 796f 7527 7265   well. If you're
-00000420: 2070 6173 7369 6e67 2061 206c 6973 7420   passing a list 
-00000430: 6f66 2073 7472 696e 6773 206c 696b 6520  of strings like 
-00000440: 7765 2068 6176 6520 646f 6e65 2068 6572  we have done her
-00000450: 652c 2065 6e73 7572 6520 796f 7520 6861  e, ensure you ha
-00000460: 7665 2079 6f75 7220 604f 5045 4e41 495f  ve your `OPENAI_
-00000470: 4150 495f 4b45 5960 2069 6e20 7468 6520  API_KEY` in the 
-00000480: 656e 7669 726f 6e6d 656e 742e 2042 7920  environment. By 
-00000490: 6465 6661 756c 7420 7765 2075 7365 204f  default we use O
-000004a0: 7065 6e41 4920 746f 2074 6f20 6765 6e65  penAI to to gene
-000004b0: 7261 7465 2074 6865 2065 6d62 6564 6469  rate the embeddi
-000004c0: 6e67 732e 2050 6c65 6173 6520 7265 6163  ngs. Please reac
-000004d0: 6820 6f75 7420 6966 2079 6f75 2772 6520  h out if you're 
-000004e0: 6c6f 6f6b 696e 6720 666f 7220 7375 7070  looking for supp
-000004f0: 6f72 7420 6672 6f6d 2061 2064 6966 6665  ort from a diffe
-00000500: 7265 6e74 2070 726f 7669 6465 7221 0a0a  rent provider!..
-00000510: 2323 2323 2033 2e20 5365 6172 6368 0a60  #### 3. Search.`
-00000520: 6060 7079 0a72 6573 756c 742c 2064 6973  ``py.result, dis
-00000530: 7461 6e63 6573 203d 2063 6974 7275 732e  tances = citrus.
-00000540: 7175 6572 7928 696e 6465 783d 2265 7861  query(index="exa
-00000550: 6d70 6c65 222c 2064 6f63 756d 656e 7473  mple", documents
-00000560: 3d5b 2257 6861 7420 6973 2069 7420 6c69  =["What is it li
-00000570: 6b65 2074 6f20 6c61 756e 6368 2061 2073  ke to launch a s
-00000580: 7461 7274 7570 225d 2c20 6b3d 3129 0a60  tartup"], k=1).`
-00000590: 6060 0a47 6f20 6c61 756e 6368 2061 2072  ``.Go launch a r
-000005a0: 6570 6c20 6f6e 205b 5265 706c 6974 5d28  epl on [Replit](
-000005b0: 6874 7470 733a 2f2f 7265 706c 6974 2e63  https://replit.c
-000005c0: 6f6d 2920 616e 6420 7365 6520 7768 6174  om) and see what
-000005d0: 2072 6573 756c 7420 796f 7520 6765 7420   result you get 
-000005e0: 6166 7465 7220 7275 6e6e 696e 6720 7468  after running th
-000005f0: 6520 7175 6572 7921 2060 7265 7375 6c74  e query! `result
-00000600: 6020 7769 6c6c 2063 6f6e 7461 696e 2074  ` will contain t
-00000610: 6865 2060 6964 7360 206f 6620 7468 6520  he `ids` of the 
-00000620: 746f 7020 606b 6020 7365 6172 6368 2068  top `k` search h
-00000630: 6974 732e 0a0a 2323 2045 7861 6d70 6c65  its...## Example
-00000640: 0a5b 706f 6b65 6465 7820 7365 6172 6368  .[pokedex search
-00000650: 5d28 6874 7470 733a 2f2f 7265 706c 6974  ](https://replit
-00000660: 2e63 6f6d 2f40 6465 6261 6272 6174 616a  .com/@debabrataj
-00000670: 722f 706f 6b65 6465 782d 7365 6172 6368  r/pokedex-search
-00000680: 290a 0a23 2320 4661 6369 6e67 2069 7373  )..## Facing iss
-00000690: 7565 733f 0a46 6565 6c20 6672 6565 2074  ues?.Feel free t
-000006a0: 6f20 6f70 656e 2069 7373 7565 7320 6f6e  o open issues on
-000006b0: 2074 6869 7320 7265 706f 7369 746f 7279   this repository
-000006c0: 2120 4469 7363 6f72 6420 7365 7276 6572  ! Discord server
-000006d0: 2063 6f6d 696e 6720 736f 6f6e 210a 0a50   coming soon!..P
-000006e0: 533a 2063 6974 7275 7320 6973 6e27 7420  S: citrus isn't 
-000006f0: 6469 7374 7269 6275 7465 6420 6a75 7374  distributed just
-00000700: 2079 6574 2e20 5765 2772 6520 6765 7474   yet. We're gett
-00000710: 696e 6720 7468 6572 6520 7468 6f75 6768  ing there though
-00000720: 203b 290a                                 ;).
+00000030: 746f 7220 6461 7461 6261 7365 0a0a 2323  tor database..##
+00000040: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
+00000050: 6060 0a70 6970 2069 6e73 7461 6c6c 2063  ``.pip install c
+00000060: 6974 7275 7364 620a 6060 600a 0a23 2320  itrusdb.```..## 
+00000070: 4765 7474 696e 6720 7374 6172 7465 640a  Getting started.
+00000080: 0a23 2323 2320 312e 2043 7265 6174 6520  .#### 1. Create 
+00000090: 696e 6465 780a 6060 6070 790a 696d 706f  index.```py.impo
+000000a0: 7274 2063 6974 7275 7364 620a 0a23 2049  rt citrusdb..# I
+000000b0: 6e69 7469 616c 697a 6520 636c 6965 6e74  nitialize client
+000000c0: 0a63 6974 7275 7320 3d20 6369 7472 7573  .citrus = citrus
+000000d0: 6462 2e43 6c69 656e 7428 290a 0a23 2043  db.Client()..# C
+000000e0: 7265 6174 6520 696e 6465 780a 6369 7472  reate index.citr
+000000f0: 7573 2e63 7265 6174 655f 696e 6465 7828  us.create_index(
+00000100: 0a20 206e 616d 653d 2265 7861 6d70 6c65  .  name="example
+00000110: 222c 0a20 206d 6178 5f65 6c65 6d65 6e74  ",.  max_element
+00000120: 733d 3130 3030 2c20 2020 2020 2020 2020  s=1000,         
+00000130: 2020 2023 2069 6e63 7265 6173 6573 2064     # increases d
+00000140: 796e 616d 6963 616c 6c79 2061 7320 796f  ynamically as yo
+00000150: 7520 696e 7365 7274 206d 6f72 6520 7665  u insert more ve
+00000160: 6374 6f72 730a 290a 6060 600a 0a23 2323  ctors.).```..###
+00000170: 2320 322e 2049 6e73 6572 7420 656c 656d  # 2. Insert elem
+00000180: 656e 7473 0a60 6060 7079 0a69 6473 203d  ents.```py.ids =
+00000190: 205b 312c 2032 2c20 335d 0a64 6f63 756d   [1, 2, 3].docum
+000001a0: 656e 7473 203d 205b 0a20 2022 596f 7572  ents = [.  "Your
+000001b0: 2074 696d 6520 6973 206c 696d 6974 6564   time is limited
+000001c0: 2c20 736f 2064 6f6e 2774 2077 6173 7465  , so don't waste
+000001d0: 2069 7420 6c69 7669 6e67 2073 6f6d 656f   it living someo
+000001e0: 6e65 2065 6c73 6527 7320 6c69 6665 222c  ne else's life",
+000001f0: 0a20 2022 4927 6420 7261 7468 6572 2062  .  "I'd rather b
+00000200: 6520 6f70 7469 6d69 7374 6963 2061 6e64  e optimistic and
+00000210: 2077 726f 6e67 2074 6861 6e20 7065 7373   wrong than pess
+00000220: 696d 6973 7469 6320 616e 6420 7269 6768  imistic and righ
+00000230: 742e 222c 0a20 2022 5275 6e6e 696e 6720  t.",.  "Running 
+00000240: 6120 7374 6172 742d 7570 2069 7320 6c69  a start-up is li
+00000250: 6b65 2063 6865 7769 6e67 2067 6c61 7373  ke chewing glass
+00000260: 2061 6e64 2073 7461 7269 6e67 2069 6e74   and staring int
+00000270: 6f20 7468 6520 6162 7973 732e 220a 5d0a  o the abyss.".].
+00000280: 0a63 6974 7275 732e 6164 6428 696e 6465  .citrus.add(inde
+00000290: 783d 2265 7861 6d70 6c65 222c 2069 6473  x="example", ids
+000002a0: 3d69 6473 2c20 646f 6375 6d65 6e74 733d  =ids, documents=
+000002b0: 646f 6375 6d65 6e74 7329 0a60 6060 0a59  documents).```.Y
+000002c0: 6f75 2063 616e 2064 6972 6563 746c 7920  ou can directly 
+000002d0: 7061 7373 2076 6563 746f 7220 656d 6265  pass vector embe
+000002e0: 6464 696e 6773 2061 7320 7765 6c6c 2e20  ddings as well. 
+000002f0: 4966 2079 6f75 2772 6520 7061 7373 696e  If you're passin
+00000300: 6720 6120 6c69 7374 206f 6620 7374 7269  g a list of stri
+00000310: 6e67 7320 6c69 6b65 2077 6520 6861 7665  ngs like we have
+00000320: 2064 6f6e 6520 6865 7265 2c20 656e 7375   done here, ensu
+00000330: 7265 2079 6f75 2068 6176 6520 796f 7572  re you have your
+00000340: 2060 4f50 454e 4149 5f41 5049 5f4b 4559   `OPENAI_API_KEY
+00000350: 6020 696e 2074 6865 2065 6e76 6972 6f6e  ` in the environ
+00000360: 6d65 6e74 2e20 4279 2064 6566 6175 6c74  ment. By default
+00000370: 2077 6520 7573 6520 4f70 656e 4149 2074   we use OpenAI t
+00000380: 6f20 746f 2067 656e 6572 6174 6520 7468  o to generate th
+00000390: 6520 656d 6265 6464 696e 6773 2e20 506c  e embeddings. Pl
+000003a0: 6561 7365 2072 6561 6368 206f 7574 2069  ease reach out i
+000003b0: 6620 796f 7527 7265 206c 6f6f 6b69 6e67  f you're looking
+000003c0: 2066 6f72 2073 7570 706f 7274 2066 726f   for support fro
+000003d0: 6d20 6120 6469 6666 6572 656e 7420 7072  m a different pr
+000003e0: 6f76 6964 6572 210a 0a23 2323 2320 332e  ovider!..#### 3.
+000003f0: 2053 6561 7263 680a 6060 6070 790a 7265   Search.```py.re
+00000400: 7375 6c74 7320 3d20 6369 7472 7573 2e71  sults = citrus.q
+00000410: 7565 7279 280a 2020 2020 696e 6465 783d  uery(.    index=
+00000420: 2265 7861 6d70 6c65 222c 0a20 2020 2064  "example",.    d
+00000430: 6f63 756d 656e 7473 3d5b 2257 6861 7420  ocuments=["What 
+00000440: 6973 2069 7420 6c69 6b65 2074 6f20 6c61  is it like to la
+00000450: 756e 6368 2061 2073 7461 7274 7570 225d  unch a startup"]
+00000460: 2c0a 2020 2020 6b3d 312c 0a20 2020 2069  ,.    k=1,.    i
+00000470: 6e63 6c75 6465 3d5b 2264 6f63 756d 656e  nclude=["documen
+00000480: 7422 2c20 226d 6574 6164 6174 6122 5d0a  t", "metadata"].
+00000490: 290a 0a70 7269 6e74 2872 6573 756c 7473  )..print(results
+000004a0: 290a 6060 600a 596f 7520 6361 6e20 7370  ).```.You can sp
+000004b0: 6563 6966 7920 6966 2079 6f75 2077 616e  ecify if you wan
+000004c0: 7420 7468 6520 6173 736f 6369 6174 6564  t the associated
+000004d0: 2074 6578 7420 646f 6375 6d65 6e74 2061   text document a
+000004e0: 6e64 206d 6574 6164 6174 6120 746f 2062  nd metadata to b
+000004f0: 6520 7265 7475 726e 6564 2e0a 4279 2064  e returned..By d
+00000500: 6566 6175 6c74 2c20 6f6e 6c79 2074 6865  efault, only the
+00000510: 2049 4473 2061 7265 2072 6574 7572 6e65   IDs are returne
+00000520: 642e 0a0a 476f 206c 6175 6e63 6820 6120  d...Go launch a 
+00000530: 7265 706c 206f 6e20 5b52 6570 6c69 745d  repl on [Replit]
+00000540: 2868 7474 7073 3a2f 2f72 6570 6c69 742e  (https://replit.
+00000550: 636f 6d29 2061 6e64 2073 6565 2077 6861  com) and see wha
+00000560: 7420 7265 7375 6c74 2079 6f75 2067 6574  t result you get
+00000570: 2061 6674 6572 2072 756e 6e69 6e67 2074   after running t
+00000580: 6865 2071 7565 7279 2120 6072 6573 756c  he query! `resul
+00000590: 7460 2077 696c 6c20 636f 6e74 6169 6e20  t` will contain 
+000005a0: 7468 6520 6069 6473 6020 6f66 2074 6865  the `ids` of the
+000005b0: 2074 6f70 2060 6b60 2073 6561 7263 6820   top `k` search 
+000005c0: 6869 7473 2e0a 0a23 2320 4578 616d 706c  hits...## Exampl
+000005d0: 650a 5b70 6f6b 6564 6578 2073 6561 7263  e.[pokedex searc
+000005e0: 685d 2868 7474 7073 3a2f 2f72 6570 6c69  h](https://repli
+000005f0: 742e 636f 6d2f 4064 6562 6162 7261 7461  t.com/@debabrata
+00000600: 6a72 2f70 6f6b 6564 6578 2d73 6561 7263  jr/pokedex-searc
+00000610: 6829 0a0a 2323 2046 6163 696e 6720 6973  h)..## Facing is
+00000620: 7375 6573 3f0a 4665 656c 2066 7265 6520  sues?.Feel free 
+00000630: 746f 206f 7065 6e20 6973 7375 6573 206f  to open issues o
+00000640: 6e20 7468 6973 2072 6570 6f73 6974 6f72  n this repositor
+00000650: 7921 2044 6973 636f 7264 2073 6572 7665  y! Discord serve
+00000660: 7220 636f 6d69 6e67 2073 6f6f 6e21 0a0a  r coming soon!..
+00000670: 5053 3a20 6369 7472 7573 2069 736e 2774  PS: citrus isn't
+00000680: 2064 6973 7472 6962 7574 6564 206a 7573   distributed jus
+00000690: 7420 7965 742e 2057 6527 7265 2067 6574  t yet. We're get
+000006a0: 7469 6e67 2074 6865 7265 2074 686f 7567  ting there thoug
+000006b0: 6820 3b29 0a                             h ;).
```

### Comparing `citrusdb-0.5.1/citrusdb/api/index.py` & `citrusdb-0.5.2/citrusdb/api/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         query_embeddings: Optional[NDArray[float32]] = None,
         k=1,
         filter_function=None
     ):
         if query_embeddings is None and documents is None:
             raise ValueError("Please provide either an embedding" + " or a document.")
 
-        if documents is not None:
+        if (query_embeddings is None) and (documents is not None):
             from citrusdb.embedding.openai import get_embeddings
 
             embeddings = get_embeddings(documents)
             query_embeddings = embeddings
 
         return self._db.knn_query(query_embeddings, k, filter_function)
```

### Comparing `citrusdb-0.5.1/citrusdb/api/local.py` & `citrusdb-0.5.2/citrusdb/api/local.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import enum
 import os
 import json
 from typing import Any, Dict, List, Optional
 from numpy import float32
 from numpy._typing import NDArray
 import shutil
 
 from citrusdb.api.index import Index
 from citrusdb.db import BaseDB
 from citrusdb.db.postgres.db import PostgresDB
 from citrusdb.db.sqlite.db import SQLiteDB
+from citrusdb.embedding.utils import get_cosine_similarity
 from citrusdb.utils.types import IDs
 
 
 class LocalAPI:
     _db: Dict[str, Index] 
     _SQLClient: BaseDB
     persist_directory: Optional[str]
@@ -98,15 +98,15 @@
             index_id = index_details[0]
             index_dim = index_details[2]
             replace_deleted = True if index_details[7] else False
 
             # Check whether the dimensions are equal
             if embedding_dim != index_dim:
                 raise ValueError(
-                        f"Embedding dimenstion ({embedding_dim}) and index "
+                        f"Embedding dimension ({embedding_dim}) and index "
                         + f"dimension ({index_dim}) do not match."
                         )
 
             # Ensure no of ids = no of embeddings
             if len(ids) != len(embeddings):
                 raise ValueError(f"Number of embeddings" + " and ids are different.")
 
@@ -196,34 +196,62 @@
         if "metadata" in include:
             included_columns["metadata"] = True
 
         flag = 1
         for key in self._db.keys():
             if key == index:
                 flag = 0
-                results, distances = self._db[key].query(
-                    documents=documents,
-                    query_embeddings=query_embeddings,
-                    k=k,
-                    filter_function=None if filters is None else filter_function
-                )
-                elements = self._SQLClient.get_vector_ids_of_results(
-                    name=index,
-                    results=results,
-                    include=included_columns
-                )
-                for i, rows in enumerate(elements):
-                    for j, row in enumerate(rows):
-                        row["distance"] = distances[i][j]
-                return elements
 
+                try:
+                    results, distances = self._db[key].query(
+                        documents=documents,
+                        query_embeddings=query_embeddings,
+                        k=k,
+                        filter_function=None if filters is None else filter_function
+                    )
+                    elements = self._SQLClient.get_vector_ids_of_results(
+                        name=index,
+                        results=results,
+                        include=included_columns
+                    )
+                    for i, rows in enumerate(elements):
+                        for j, row in enumerate(rows):
+                            row["distance"] = distances[i][j]
+                    return elements
+                except RuntimeError as error:
+                    # Return all vectors currently in index
+                    # Deals with error when top_k is higher than no. of vectors indexed.
+                    # Error: Cannot return the results in a contigious 2D array. Probably ef or M is too small
+                    print("ERROR:", error, "-- Falling back to existing vectors in index")
+                    indexed_elements = self._SQLClient.get_all_vectors_in_index(
+                        name=index,
+                        include=included_columns
+                    )
+                    if (query_embeddings is None):
+                        if documents is None:
+                            raise Exception("Neither documents nor query embeddings provided.")
+                        from citrusdb.embedding.openai import get_embeddings
+
+                        embeddings = get_embeddings(documents)
+                        query_embeddings = embeddings
+
+                    returning_elements = []
+                    for i, query in enumerate(query_embeddings):
+                        results = []
+                        for element in indexed_elements:
+                            item = {**element}
+                            item["distance"] = 1 - get_cosine_similarity(query, element["embedding"])
+                            del item["embedding"]
+                            results.append(item)
+                        results.sort(key=lambda e : e["distance"])
+                        returning_elements.append(results)
+                    return returning_elements
         if flag:
             raise ValueError(f"Could not find index: {index}")
 
-
     def get_status(self, index: str):
         flag = 1
         for key in self._db.keys():
             if key == index:
                 flag = 0
                 self._db[key].get_status()
```

### Comparing `citrusdb-0.5.1/citrusdb/db/__init__.py` & `citrusdb-0.5.2/citrusdb/db/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,22 @@
     def get_index_details(
         self,
         name: str
     ) -> Optional[Tuple[int, str, int, int, int, int, int, bool]]:
         pass
 
     @abstractmethod
+    def get_all_vectors_in_index(
+        self,
+        name: str,
+        include: Dict
+    ) -> List[Dict]:
+        pass
+
+    @abstractmethod
     def get_vector_ids_of_results(
         self,
         name: str,
         results: List[List[int]],
         include: Dict
     ) -> List[List[Dict]]:
         pass
```

### Comparing `citrusdb-0.5.1/citrusdb/db/index/hnswlib.py` & `citrusdb-0.5.2/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.1/citrusdb/db/postgres/db.py` & `citrusdb-0.5.2/citrusdb/db/postgres/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,29 +100,49 @@
         """
         parameters = (name,)
         with self._pool.connection() as conn:
             with conn.cursor() as cur:
                 cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
                 return cur.fetchone()
 
+    def get_all_vectors_in_index(self, name: str, include: Dict) -> List[Dict]:
+        """
+        Get all vectors in index
+
+        name: Name of index
+        include: Dictionary of columns to be returned
+        """
+        index_details = self.get_index_details(name)
+        if index_details is None:
+            raise ValueError(f"Index '{name}' does not exist")
+
+        index_id = index_details[0]
+        parameters = (index_id,)
+        with self._pool.connection() as conn:
+            with conn.cursor() as cur:
+                cur.execute(queries.GET_ALL_VECTORS, parameters)
+                rows = cur.fetchall()
+                return [convert_row_to_dict(row=row, include=include, with_embedding=True) for row in rows]
+
     def get_vector_ids_of_results(
         self,
         name: str,
         results: List[List[int]],
         include: Dict
     ):
         """
         Get user facing IDs of results
 
         name: Name of index
         results: List of list of integer HNSW labels
+        include: Dictionary of columns to be returned
         """
         index_details = self.get_index_details(name)
-        if not(index_details):
-            return
+        if index_details is None:
+            raise ValueError(f"Index '{name}' does not exist")
 
         cols = [sql.Identifier("id")]
         if include["document"]:
             cols.append(sql.Identifier("text"))
             if include["metadata"]:
                 cols.append(sql.Identifier("metadata"))
         elif include["metadata"]:
```

### Comparing `citrusdb-0.5.1/citrusdb/db/postgres/queries.py` & `citrusdb-0.5.2/citrusdb/db/postgres/queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 
 DELETE_VECTORS_FROM_INDEX = '''
 DELETE FROM index_data
 WHERE id = ANY(%s) AND index_id = %s
 RETURNING vector_id
 '''
 
+GET_ALL_VECTORS = '''
+SELECT vector_id, embedding, {}
+FROM index_data
+WHERE index_id = %s
+'''
+
 GET_ALL_INDEX_DETAILS = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 '''
 
 GET_INDEX_DETAILS_BY_NAME = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
```

### Comparing `citrusdb-0.5.1/citrusdb/db/postgres/query_builder.py` & `citrusdb-0.5.2/citrusdb/db/postgres/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.1/citrusdb/db/sqlite/db.py` & `citrusdb-0.5.2/citrusdb/db/sqlite/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,14 +94,35 @@
         cur = self._con.cursor()
         parameters = (name,)
         res = cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
         row = res.fetchone()
         cur.close()
         return row
 
+    def get_all_vectors_in_index(self, name: str, include: Dict) -> List[Dict]:
+        cols = "id"
+        if include["document"]:
+            cols += ", text"
+            if include["metadata"]:
+                cols += ", metadata"
+        elif include["metadata"]:
+            cols += ", metadata"
+
+        index_details = self.get_index_details(name)
+        index_id = index_details[0]                 # type: ignore
+
+        cur = self._con.cursor()
+        query = queries.GET_ALL_VECTORS.format(cols)
+        parameters = (index_id,)
+        res = cur.execute(query, parameters)
+        rows = res.fetchall()
+        cur.close()
+
+        return [convert_row_to_dict(row=row, include=include, with_embedding=True) for row in rows]
+
     def get_vector_ids_of_results(
         self,
         name: str,
         results: List[List[int]],
         include: Dict
     ) -> List[List[Dict]]:
         cols = "id"
```

### Comparing `citrusdb-0.5.1/citrusdb/db/sqlite/queries.py` & `citrusdb-0.5.2/citrusdb/db/sqlite/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 '''
 
 GET_ALL_INDEX_DETAILS = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 '''
 
+GET_ALL_VECTORS = '''
+SELECT vector_id, embedding, {}
+FROM index_data
+WHERE index_id = ?
+'''
+
 GET_INDEX_DETAILS_BY_NAME = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 WHERE name = ?
 '''
 
 GET_VECTOR_IDS_OF_RESULTS = '''
```

### Comparing `citrusdb-0.5.1/citrusdb/db/sqlite/query_builder.py` & `citrusdb-0.5.2/citrusdb/db/sqlite/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.1/citrusdb/utils/utils.py` & `citrusdb-0.5.2/citrusdb/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import os
+import json
 from typing import Dict, Optional, Tuple
 
-def convert_row_to_dict(row: Tuple, include: Dict):
-    returning_dict = {"id": row[1]}
-    if include["document"]:
-        returning_dict["document"] = row[2]
-        if include["metadata"]:
+def convert_row_to_dict(row: Tuple, include: Dict, with_embedding: bool = False):
+    if with_embedding:
+        returning_dict = {"id": row[2], "embedding": json.loads(row[1])}
+        if include["document"]:
+            returning_dict["document"] = row[3]
+            if include["metadata"]:
+                returning_dict["metadata"] = row[4]
+        elif include["metadata"]:
             returning_dict["metadata"] = row[3]
-    elif include["metadata"]:
-        returning_dict["metadata"] = row[2]
 
-    return returning_dict
+        return returning_dict
+    else:
+        returning_dict = {"id": row[1]}
+        if include["document"]:
+            returning_dict["document"] = row[2]
+            if include["metadata"]:
+                returning_dict["metadata"] = row[3]
+        elif include["metadata"]:
+            returning_dict["metadata"] = row[2]
+
+        return returning_dict
 
 def ensure_valid_path(persist_directory: str, file_name: Optional[str] = None) -> bool:
     """
     Creates required directories if they do not exist.
 
     If only persist_directory is passed, returns True.
     When file_name is passed, function returns boolean based on whether the
```

### Comparing `citrusdb-0.5.1/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.5.2/citrusdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6369 7472  : 2.1.Name: citr
 00000020: 7573 6462 0a56 6572 7369 6f6e 3a20 302e  usdb.Version: 0.
-00000030: 352e 310a 5375 6d6d 6172 793a 206f 7065  5.1.Summary: ope
+00000030: 352e 320a 5375 6d6d 6172 793a 206f 7065  5.2.Summary: ope
 00000040: 6e2d 736f 7572 6365 2076 6563 746f 7220  n-source vector 
 00000050: 6461 7461 6261 7365 2e20 7374 6f72 6520  database. store 
 00000060: 616e 6420 7265 7472 6965 7665 2065 6d62  and retrieve emb
 00000070: 6564 6469 6e67 7320 666f 7220 796f 7572  eddings for your
 00000080: 206e 6578 7420 7072 6f6a 6563 7421 0a48   next project!.H
 00000090: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
 000000a0: 2f2f 6769 7468 7562 2e63 6f6d 2f30 7844  //github.com/0xD
@@ -34,118 +34,111 @@
 00000210: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 00000220: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 00000230: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 00000240: 4345 4e53 450a 0a23 20f0 9f8d 8b20 6369  CENSE..# .... ci
 00000250: 7472 7573 2e0a 2323 2320 6f70 656e 2d73  trus..### open-s
 00000260: 6f75 7263 6520 2864 6973 7472 6962 7574  ource (distribut
 00000270: 6564 2920 7665 6374 6f72 2064 6174 6162  ed) vector datab
-00000280: 6173 650a 0a3c 7020 616c 6967 6e3d 2263  ase..<p align="c
-00000290: 656e 7465 7222 3e0a 2020 5370 6563 6961  enter">.  Specia
-000002a0: 6c20 7468 616e 6b73 2074 6f0a 3c2f 703e  l thanks to.</p>
-000002b0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000002c0: 7222 3e0a 2020 3c69 6d67 2061 6c69 676e  r">.  <img align
-000002d0: 3d22 6365 6e74 6572 2220 7372 633d 2268  ="center" src="h
-000002e0: 7474 7073 3a2f 2f77 7777 2e67 6574 6465  ttps://www.getde
-000002f0: 766b 6974 2e63 6f6d 2f6c 6f67 6f2e 706e  vkit.com/logo.pn
-00000300: 6722 2077 6964 7468 3d31 3030 2068 6569  g" width=100 hei
-00000310: 6768 743d 3130 3020 616c 743d 2244 6576  ght=100 alt="Dev
-00000320: 4b69 7422 202f 3e0a 3c2f 703e 0a3c 7020  Kit" />.</p>.<p 
-00000330: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000340: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000350: 3a2f 2f77 7777 2e67 6574 6465 766b 6974  ://www.getdevkit
-00000360: 2e63 6f6d 223e 4465 764b 6974 202d 2054  .com">DevKit - T
-00000370: 6865 2045 7373 656e 7469 616c 2044 6576  he Essential Dev
-00000380: 656c 6f70 6572 2054 6f6f 6c6b 6974 3c2f  eloper Toolkit</
-00000390: 613e 3c62 7220 2f3e 0a20 2044 536f 4320  a><br />.  DSoC 
-000003a0: 3230 3233 0a3c 2f70 3e0a 0a0a 2323 2049  2023.</p>...## I
-000003b0: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
-000003c0: 0a70 6970 2069 6e73 7461 6c6c 2063 6974  .pip install cit
-000003d0: 7275 7364 620a 6060 600a 0a23 2320 4765  rusdb.```..## Ge
-000003e0: 7474 696e 6720 7374 6172 7465 640a 0a23  tting started..#
-000003f0: 2323 2320 312e 2043 7265 6174 6520 696e  ### 1. Create in
-00000400: 6465 780a 6060 6070 790a 696d 706f 7274  dex.```py.import
-00000410: 2063 6974 7275 7364 620a 0a23 2049 6e69   citrusdb..# Ini
-00000420: 7469 616c 697a 6520 636c 6965 6e74 0a63  tialize client.c
-00000430: 6974 7275 7320 3d20 6369 7472 7573 6462  itrus = citrusdb
-00000440: 2e43 6c69 656e 7428 290a 0a23 2043 7265  .Client()..# Cre
-00000450: 6174 6520 696e 6465 780a 6369 7472 7573  ate index.citrus
-00000460: 2e63 7265 6174 655f 696e 6465 7828 0a20  .create_index(. 
-00000470: 206e 616d 653d 2265 7861 6d70 6c65 222c   name="example",
-00000480: 0a20 206d 6178 5f65 6c65 6d65 6e74 733d  .  max_elements=
-00000490: 3130 3030 2c20 2020 2020 2020 2020 2020  1000,           
-000004a0: 2023 2069 6e63 7265 6173 6573 2064 796e   # increases dyn
-000004b0: 616d 6963 616c 6c79 2061 7320 796f 7520  amically as you 
-000004c0: 696e 7365 7274 206d 6f72 6520 7665 6374  insert more vect
-000004d0: 6f72 730a 290a 6060 600a 0a23 2323 2320  ors.).```..#### 
-000004e0: 322e 2049 6e73 6572 7420 656c 656d 656e  2. Insert elemen
-000004f0: 7473 0a60 6060 7079 0a69 6473 203d 205b  ts.```py.ids = [
-00000500: 312c 2032 2c20 335d 0a64 6f63 756d 656e  1, 2, 3].documen
-00000510: 7473 203d 205b 0a20 2022 596f 7572 2074  ts = [.  "Your t
-00000520: 696d 6520 6973 206c 696d 6974 6564 2c20  ime is limited, 
-00000530: 736f 2064 6f6e 2774 2077 6173 7465 2069  so don't waste i
-00000540: 7420 6c69 7669 6e67 2073 6f6d 656f 6e65  t living someone
-00000550: 2065 6c73 6527 7320 6c69 6665 222c 0a20   else's life",. 
-00000560: 2022 4927 6420 7261 7468 6572 2062 6520   "I'd rather be 
-00000570: 6f70 7469 6d69 7374 6963 2061 6e64 2077  optimistic and w
-00000580: 726f 6e67 2074 6861 6e20 7065 7373 696d  rong than pessim
-00000590: 6973 7469 6320 616e 6420 7269 6768 742e  istic and right.
-000005a0: 222c 0a20 2022 5275 6e6e 696e 6720 6120  ",.  "Running a 
-000005b0: 7374 6172 742d 7570 2069 7320 6c69 6b65  start-up is like
-000005c0: 2063 6865 7769 6e67 2067 6c61 7373 2061   chewing glass a
-000005d0: 6e64 2073 7461 7269 6e67 2069 6e74 6f20  nd staring into 
-000005e0: 7468 6520 6162 7973 732e 220a 5d0a 0a63  the abyss.".]..c
-000005f0: 6974 7275 732e 6164 6428 696e 6465 783d  itrus.add(index=
-00000600: 2265 7861 6d70 6c65 222c 2069 6473 3d69  "example", ids=i
-00000610: 6473 2c20 646f 6375 6d65 6e74 733d 646f  ds, documents=do
-00000620: 6375 6d65 6e74 7329 0a60 6060 0a59 6f75  cuments).```.You
-00000630: 2063 616e 2064 6972 6563 746c 7920 7061   can directly pa
-00000640: 7373 2076 6563 746f 7220 656d 6265 6464  ss vector embedd
-00000650: 696e 6773 2061 7320 7765 6c6c 2e20 4966  ings as well. If
-00000660: 2079 6f75 2772 6520 7061 7373 696e 6720   you're passing 
-00000670: 6120 6c69 7374 206f 6620 7374 7269 6e67  a list of string
-00000680: 7320 6c69 6b65 2077 6520 6861 7665 2064  s like we have d
-00000690: 6f6e 6520 6865 7265 2c20 656e 7375 7265  one here, ensure
-000006a0: 2079 6f75 2068 6176 6520 796f 7572 2060   you have your `
-000006b0: 4f50 454e 4149 5f41 5049 5f4b 4559 6020  OPENAI_API_KEY` 
-000006c0: 696e 2074 6865 2065 6e76 6972 6f6e 6d65  in the environme
-000006d0: 6e74 2e20 4279 2064 6566 6175 6c74 2077  nt. By default w
-000006e0: 6520 7573 6520 4f70 656e 4149 2074 6f20  e use OpenAI to 
-000006f0: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
-00000700: 656d 6265 6464 696e 6773 2e20 506c 6561  embeddings. Plea
-00000710: 7365 2072 6561 6368 206f 7574 2069 6620  se reach out if 
-00000720: 796f 7527 7265 206c 6f6f 6b69 6e67 2066  you're looking f
-00000730: 6f72 2073 7570 706f 7274 2066 726f 6d20  or support from 
-00000740: 6120 6469 6666 6572 656e 7420 7072 6f76  a different prov
-00000750: 6964 6572 210a 0a23 2323 2320 332e 2053  ider!..#### 3. S
-00000760: 6561 7263 680a 6060 6070 790a 7265 7375  earch.```py.resu
-00000770: 6c74 2c20 6469 7374 616e 6365 7320 3d20  lt, distances = 
-00000780: 6369 7472 7573 2e71 7565 7279 2869 6e64  citrus.query(ind
-00000790: 6578 3d22 6578 616d 706c 6522 2c20 646f  ex="example", do
-000007a0: 6375 6d65 6e74 733d 5b22 5768 6174 2069  cuments=["What i
-000007b0: 7320 6974 206c 696b 6520 746f 206c 6175  s it like to lau
-000007c0: 6e63 6820 6120 7374 6172 7475 7022 5d2c  nch a startup"],
-000007d0: 206b 3d31 290a 6060 600a 476f 206c 6175   k=1).```.Go lau
-000007e0: 6e63 6820 6120 7265 706c 206f 6e20 5b52  nch a repl on [R
-000007f0: 6570 6c69 745d 2868 7474 7073 3a2f 2f72  eplit](https://r
-00000800: 6570 6c69 742e 636f 6d29 2061 6e64 2073  eplit.com) and s
-00000810: 6565 2077 6861 7420 7265 7375 6c74 2079  ee what result y
-00000820: 6f75 2067 6574 2061 6674 6572 2072 756e  ou get after run
-00000830: 6e69 6e67 2074 6865 2071 7565 7279 2120  ning the query! 
-00000840: 6072 6573 756c 7460 2077 696c 6c20 636f  `result` will co
-00000850: 6e74 6169 6e20 7468 6520 6069 6473 6020  ntain the `ids` 
-00000860: 6f66 2074 6865 2074 6f70 2060 6b60 2073  of the top `k` s
-00000870: 6561 7263 6820 6869 7473 2e0a 0a23 2320  earch hits...## 
-00000880: 4578 616d 706c 650a 5b70 6f6b 6564 6578  Example.[pokedex
-00000890: 2073 6561 7263 685d 2868 7474 7073 3a2f   search](https:/
-000008a0: 2f72 6570 6c69 742e 636f 6d2f 4064 6562  /replit.com/@deb
-000008b0: 6162 7261 7461 6a72 2f70 6f6b 6564 6578  abratajr/pokedex
-000008c0: 2d73 6561 7263 6829 0a0a 2323 2046 6163  -search)..## Fac
-000008d0: 696e 6720 6973 7375 6573 3f0a 4665 656c  ing issues?.Feel
-000008e0: 2066 7265 6520 746f 206f 7065 6e20 6973   free to open is
-000008f0: 7375 6573 206f 6e20 7468 6973 2072 6570  sues on this rep
-00000900: 6f73 6974 6f72 7921 2044 6973 636f 7264  ository! Discord
-00000910: 2073 6572 7665 7220 636f 6d69 6e67 2073   server coming s
-00000920: 6f6f 6e21 0a0a 5053 3a20 6369 7472 7573  oon!..PS: citrus
-00000930: 2069 736e 2774 2064 6973 7472 6962 7574   isn't distribut
-00000940: 6564 206a 7573 7420 7965 742e 2057 6527  ed just yet. We'
-00000950: 7265 2067 6574 7469 6e67 2074 6865 7265  re getting there
-00000960: 2074 686f 7567 6820 3b29 0a               though ;).
+00000280: 6173 650a 0a23 2320 496e 7374 616c 6c61  ase..## Installa
+00000290: 7469 6f6e 0a0a 6060 600a 7069 7020 696e  tion..```.pip in
+000002a0: 7374 616c 6c20 6369 7472 7573 6462 0a60  stall citrusdb.`
+000002b0: 6060 0a0a 2323 2047 6574 7469 6e67 2073  ``..## Getting s
+000002c0: 7461 7274 6564 0a0a 2323 2323 2031 2e20  tarted..#### 1. 
+000002d0: 4372 6561 7465 2069 6e64 6578 0a60 6060  Create index.```
+000002e0: 7079 0a69 6d70 6f72 7420 6369 7472 7573  py.import citrus
+000002f0: 6462 0a0a 2320 496e 6974 6961 6c69 7a65  db..# Initialize
+00000300: 2063 6c69 656e 740a 6369 7472 7573 203d   client.citrus =
+00000310: 2063 6974 7275 7364 622e 436c 6965 6e74   citrusdb.Client
+00000320: 2829 0a0a 2320 4372 6561 7465 2069 6e64  ()..# Create ind
+00000330: 6578 0a63 6974 7275 732e 6372 6561 7465  ex.citrus.create
+00000340: 5f69 6e64 6578 280a 2020 6e61 6d65 3d22  _index(.  name="
+00000350: 6578 616d 706c 6522 2c0a 2020 6d61 785f  example",.  max_
+00000360: 656c 656d 656e 7473 3d31 3030 302c 2020  elements=1000,  
+00000370: 2020 2020 2020 2020 2020 2320 696e 6372            # incr
+00000380: 6561 7365 7320 6479 6e61 6d69 6361 6c6c  eases dynamicall
+00000390: 7920 6173 2079 6f75 2069 6e73 6572 7420  y as you insert 
+000003a0: 6d6f 7265 2076 6563 746f 7273 0a29 0a60  more vectors.).`
+000003b0: 6060 0a0a 2323 2323 2032 2e20 496e 7365  ``..#### 2. Inse
+000003c0: 7274 2065 6c65 6d65 6e74 730a 6060 6070  rt elements.```p
+000003d0: 790a 6964 7320 3d20 5b31 2c20 322c 2033  y.ids = [1, 2, 3
+000003e0: 5d0a 646f 6375 6d65 6e74 7320 3d20 5b0a  ].documents = [.
+000003f0: 2020 2259 6f75 7220 7469 6d65 2069 7320    "Your time is 
+00000400: 6c69 6d69 7465 642c 2073 6f20 646f 6e27  limited, so don'
+00000410: 7420 7761 7374 6520 6974 206c 6976 696e  t waste it livin
+00000420: 6720 736f 6d65 6f6e 6520 656c 7365 2773  g someone else's
+00000430: 206c 6966 6522 2c0a 2020 2249 2764 2072   life",.  "I'd r
+00000440: 6174 6865 7220 6265 206f 7074 696d 6973  ather be optimis
+00000450: 7469 6320 616e 6420 7772 6f6e 6720 7468  tic and wrong th
+00000460: 616e 2070 6573 7369 6d69 7374 6963 2061  an pessimistic a
+00000470: 6e64 2072 6967 6874 2e22 2c0a 2020 2252  nd right.",.  "R
+00000480: 756e 6e69 6e67 2061 2073 7461 7274 2d75  unning a start-u
+00000490: 7020 6973 206c 696b 6520 6368 6577 696e  p is like chewin
+000004a0: 6720 676c 6173 7320 616e 6420 7374 6172  g glass and star
+000004b0: 696e 6720 696e 746f 2074 6865 2061 6279  ing into the aby
+000004c0: 7373 2e22 0a5d 0a0a 6369 7472 7573 2e61  ss.".]..citrus.a
+000004d0: 6464 2869 6e64 6578 3d22 6578 616d 706c  dd(index="exampl
+000004e0: 6522 2c20 6964 733d 6964 732c 2064 6f63  e", ids=ids, doc
+000004f0: 756d 656e 7473 3d64 6f63 756d 656e 7473  uments=documents
+00000500: 290a 6060 600a 596f 7520 6361 6e20 6469  ).```.You can di
+00000510: 7265 6374 6c79 2070 6173 7320 7665 6374  rectly pass vect
+00000520: 6f72 2065 6d62 6564 6469 6e67 7320 6173  or embeddings as
+00000530: 2077 656c 6c2e 2049 6620 796f 7527 7265   well. If you're
+00000540: 2070 6173 7369 6e67 2061 206c 6973 7420   passing a list 
+00000550: 6f66 2073 7472 696e 6773 206c 696b 6520  of strings like 
+00000560: 7765 2068 6176 6520 646f 6e65 2068 6572  we have done her
+00000570: 652c 2065 6e73 7572 6520 796f 7520 6861  e, ensure you ha
+00000580: 7665 2079 6f75 7220 604f 5045 4e41 495f  ve your `OPENAI_
+00000590: 4150 495f 4b45 5960 2069 6e20 7468 6520  API_KEY` in the 
+000005a0: 656e 7669 726f 6e6d 656e 742e 2042 7920  environment. By 
+000005b0: 6465 6661 756c 7420 7765 2075 7365 204f  default we use O
+000005c0: 7065 6e41 4920 746f 2074 6f20 6765 6e65  penAI to to gene
+000005d0: 7261 7465 2074 6865 2065 6d62 6564 6469  rate the embeddi
+000005e0: 6e67 732e 2050 6c65 6173 6520 7265 6163  ngs. Please reac
+000005f0: 6820 6f75 7420 6966 2079 6f75 2772 6520  h out if you're 
+00000600: 6c6f 6f6b 696e 6720 666f 7220 7375 7070  looking for supp
+00000610: 6f72 7420 6672 6f6d 2061 2064 6966 6665  ort from a diffe
+00000620: 7265 6e74 2070 726f 7669 6465 7221 0a0a  rent provider!..
+00000630: 2323 2323 2033 2e20 5365 6172 6368 0a60  #### 3. Search.`
+00000640: 6060 7079 0a72 6573 756c 7473 203d 2063  ``py.results = c
+00000650: 6974 7275 732e 7175 6572 7928 0a20 2020  itrus.query(.   
+00000660: 2069 6e64 6578 3d22 6578 616d 706c 6522   index="example"
+00000670: 2c0a 2020 2020 646f 6375 6d65 6e74 733d  ,.    documents=
+00000680: 5b22 5768 6174 2069 7320 6974 206c 696b  ["What is it lik
+00000690: 6520 746f 206c 6175 6e63 6820 6120 7374  e to launch a st
+000006a0: 6172 7475 7022 5d2c 0a20 2020 206b 3d31  artup"],.    k=1
+000006b0: 2c0a 2020 2020 696e 636c 7564 653d 5b22  ,.    include=["
+000006c0: 646f 6375 6d65 6e74 222c 2022 6d65 7461  document", "meta
+000006d0: 6461 7461 225d 0a29 0a0a 7072 696e 7428  data"].)..print(
+000006e0: 7265 7375 6c74 7329 0a60 6060 0a59 6f75  results).```.You
+000006f0: 2063 616e 2073 7065 6369 6679 2069 6620   can specify if 
+00000700: 796f 7520 7761 6e74 2074 6865 2061 7373  you want the ass
+00000710: 6f63 6961 7465 6420 7465 7874 2064 6f63  ociated text doc
+00000720: 756d 656e 7420 616e 6420 6d65 7461 6461  ument and metada
+00000730: 7461 2074 6f20 6265 2072 6574 7572 6e65  ta to be returne
+00000740: 642e 0a42 7920 6465 6661 756c 742c 206f  d..By default, o
+00000750: 6e6c 7920 7468 6520 4944 7320 6172 6520  nly the IDs are 
+00000760: 7265 7475 726e 6564 2e0a 0a47 6f20 6c61  returned...Go la
+00000770: 756e 6368 2061 2072 6570 6c20 6f6e 205b  unch a repl on [
+00000780: 5265 706c 6974 5d28 6874 7470 733a 2f2f  Replit](https://
+00000790: 7265 706c 6974 2e63 6f6d 2920 616e 6420  replit.com) and 
+000007a0: 7365 6520 7768 6174 2072 6573 756c 7420  see what result 
+000007b0: 796f 7520 6765 7420 6166 7465 7220 7275  you get after ru
+000007c0: 6e6e 696e 6720 7468 6520 7175 6572 7921  nning the query!
+000007d0: 2060 7265 7375 6c74 6020 7769 6c6c 2063   `result` will c
+000007e0: 6f6e 7461 696e 2074 6865 2060 6964 7360  ontain the `ids`
+000007f0: 206f 6620 7468 6520 746f 7020 606b 6020   of the top `k` 
+00000800: 7365 6172 6368 2068 6974 732e 0a0a 2323  search hits...##
+00000810: 2045 7861 6d70 6c65 0a5b 706f 6b65 6465   Example.[pokede
+00000820: 7820 7365 6172 6368 5d28 6874 7470 733a  x search](https:
+00000830: 2f2f 7265 706c 6974 2e63 6f6d 2f40 6465  //replit.com/@de
+00000840: 6261 6272 6174 616a 722f 706f 6b65 6465  babratajr/pokede
+00000850: 782d 7365 6172 6368 290a 0a23 2320 4661  x-search)..## Fa
+00000860: 6369 6e67 2069 7373 7565 733f 0a46 6565  cing issues?.Fee
+00000870: 6c20 6672 6565 2074 6f20 6f70 656e 2069  l free to open i
+00000880: 7373 7565 7320 6f6e 2074 6869 7320 7265  ssues on this re
+00000890: 706f 7369 746f 7279 2120 4469 7363 6f72  pository! Discor
+000008a0: 6420 7365 7276 6572 2063 6f6d 696e 6720  d server coming 
+000008b0: 736f 6f6e 210a 0a50 533a 2063 6974 7275  soon!..PS: citru
+000008c0: 7320 6973 6e27 7420 6469 7374 7269 6275  s isn't distribu
+000008d0: 7465 6420 6a75 7374 2079 6574 2e20 5765  ted just yet. We
+000008e0: 2772 6520 6765 7474 696e 6720 7468 6572  're getting ther
+000008f0: 6520 7468 6f75 6768 203b 290a            e though ;).
```

### Comparing `citrusdb-0.5.1/citrusdb.egg-info/SOURCES.txt` & `citrusdb-0.5.2/citrusdb.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 citrusdb/db/postgres/query_builder.py
 citrusdb/db/sqlite/__init__.py
 citrusdb/db/sqlite/db.py
 citrusdb/db/sqlite/queries.py
 citrusdb/db/sqlite/query_builder.py
 citrusdb/embedding/__init__.py
 citrusdb/embedding/openai.py
+citrusdb/embedding/utils.py
 citrusdb/utils/__init__.py
 citrusdb/utils/types.py
 citrusdb/utils/utils.py
 cloud-temp/__init__.py
 cloud-temp/index.py
 cloud-temp/main-pg.py
```

### Comparing `citrusdb-0.5.1/cloud-temp/index.py` & `citrusdb-0.5.2/cloud-temp/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.1/cloud-temp/main-pg.py` & `citrusdb-0.5.2/cloud-temp/main-pg.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.1/pyproject.toml` & `citrusdb-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.5.1"
+version = "0.5.2"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "open-source vector database. store and retrieve embeddings for your next project!"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.5.1/setup.py` & `citrusdb-0.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.5.1",
+    version="0.5.2",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=(
```

