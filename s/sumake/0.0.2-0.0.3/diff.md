# Comparing `tmp/sumake-0.0.2.tar.gz` & `tmp/sumake-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumake-0.0.2.tar", last modified: Thu May 11 05:13:10 2023, max compression
+gzip compressed data, was "sumake-0.0.3.tar", last modified: Fri Aug  4 10:38:42 2023, max compression
```

## Comparing `sumake-0.0.2.tar` & `sumake-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-11 05:13:10.417942 sumake-0.0.2/
--rw-r--r--   0 peng       (501) staff       (20)       32 2023-05-11 04:17:43.000000 sumake-0.0.2/MANIFEST.in
--rw-r--r--   0 peng       (501) staff       (20)      228 2023-05-11 05:13:10.417726 sumake-0.0.2/PKG-INFO
--rw-r--r--   0 peng       (501) staff       (20)       39 2023-05-09 10:00:42.000000 sumake-0.0.2/README.md
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-11 05:13:10.416230 sumake-0.0.2/bin/
--rw-r--r--   0 peng       (501) staff       (20)      244 2023-05-11 05:13:10.000000 sumake-0.0.2/bin/sumake
--rw-r--r--   0 peng       (501) staff       (20)       38 2023-05-11 05:13:10.418002 sumake-0.0.2/setup.cfg
--rw-r--r--   0 peng       (501) staff       (20)     2472 2023-05-11 05:10:04.000000 sumake-0.0.2/setup.py
--rwxr--r--   0 peng       (501) staff       (20)      230 2023-05-10 05:47:17.000000 sumake-0.0.2/sumake
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-11 05:13:10.417091 sumake-0.0.2/sumake.egg-info/
--rw-r--r--   0 peng       (501) staff       (20)      228 2023-05-11 05:13:10.000000 sumake-0.0.2/sumake.egg-info/PKG-INFO
--rw-r--r--   0 peng       (501) staff       (20)      254 2023-05-11 05:13:10.000000 sumake-0.0.2/sumake.egg-info/SOURCES.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-11 05:13:10.000000 sumake-0.0.2/sumake.egg-info/dependency_links.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-11 05:13:10.000000 sumake-0.0.2/sumake.egg-info/not-zip-safe
--rw-r--r--   0 peng       (501) staff       (20)       11 2023-05-11 05:13:10.000000 sumake-0.0.2/sumake.egg-info/requires.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-11 05:13:10.000000 sumake-0.0.2/sumake.egg-info/top_level.txt
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-11 05:13:10.417249 sumake-0.0.2/test/
--rw-r--r--   0 peng       (501) staff       (20)      167 2023-05-10 05:44:52.000000 sumake-0.0.2/test/test_setup.py
--rw-r--r--   0 peng       (501) staff       (20)      771 2023-05-10 06:56:31.000000 sumake-0.0.2/utils.mk
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-08-04 10:38:42.336032 sumake-0.0.3/
+-rw-r--r--   0 peng       (501) staff       (20)       32 2023-05-11 04:17:43.000000 sumake-0.0.3/MANIFEST.in
+-rw-r--r--   0 peng       (501) staff       (20)      403 2023-08-04 10:38:42.335807 sumake-0.0.3/PKG-INFO
+-rw-r--r--   0 peng       (501) staff       (20)      214 2023-05-11 06:52:32.000000 sumake-0.0.3/README.md
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-08-04 10:38:42.333248 sumake-0.0.3/bin/
+-rw-r--r--   0 peng       (501) staff       (20)      244 2023-08-04 10:38:41.000000 sumake-0.0.3/bin/sumake
+-rw-r--r--   0 peng       (501) staff       (20)       38 2023-08-04 10:38:42.336210 sumake-0.0.3/setup.cfg
+-rw-r--r--   0 peng       (501) staff       (20)     2472 2023-08-04 10:37:14.000000 sumake-0.0.3/setup.py
+-rwxr--r--   0 peng       (501) staff       (20)      230 2023-05-10 05:47:17.000000 sumake-0.0.3/sumake
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-08-04 10:38:42.334733 sumake-0.0.3/sumake.egg-info/
+-rw-r--r--   0 peng       (501) staff       (20)      403 2023-08-04 10:38:41.000000 sumake-0.0.3/sumake.egg-info/PKG-INFO
+-rw-r--r--   0 peng       (501) staff       (20)      254 2023-08-04 10:38:42.000000 sumake-0.0.3/sumake.egg-info/SOURCES.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2023-08-04 10:38:41.000000 sumake-0.0.3/sumake.egg-info/dependency_links.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2023-08-04 10:38:41.000000 sumake-0.0.3/sumake.egg-info/not-zip-safe
+-rw-r--r--   0 peng       (501) staff       (20)       11 2023-08-04 10:38:41.000000 sumake-0.0.3/sumake.egg-info/requires.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2023-08-04 10:38:41.000000 sumake-0.0.3/sumake.egg-info/top_level.txt
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-08-04 10:38:42.335010 sumake-0.0.3/test/
+-rw-r--r--   0 peng       (501) staff       (20)      167 2023-05-10 05:44:52.000000 sumake-0.0.3/test/test_setup.py
+-rw-r--r--   0 peng       (501) staff       (20)      816 2023-08-04 10:37:56.000000 sumake-0.0.3/utils.mk
```

### Comparing `sumake-0.0.2/setup.py` & `sumake-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 install_dir = sysconfig.get_paths()['purelib']
 print(home_dir)
 print(install_dir)
 
 current = Path(__file__).parent.absolute()
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 def generate_sumake(home_dir, current):
     sumake_dir = home_dir / ".sumake"
     bin_dir = current / "bin"
 
     utils_mk = sumake_dir / "utils.mk"
```

### Comparing `sumake-0.0.2/utils.mk` & `sumake-0.0.3/utils.mk`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 .PHONY: wget_if_not_exist
 
 define wget_if_not_exist
 @if [ ! -f $(1) ]; then \
 	mkdir -p $(dir $(1)); \
 	wget -O $(1) $(2); \
+else \
+	echo "File already exists: $(1) "; \
 fi
 endef
 
 #sumake_version:
 #	@echo 2023.5.9
 
 # $(call check_conda, my_env)
```

