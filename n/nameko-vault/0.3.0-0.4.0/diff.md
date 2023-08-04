# Comparing `tmp/nameko-vault-0.3.0.tar.gz` & `tmp/nameko_vault-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nameko-vault-0.3.0.tar", last modified: Fri Dec  4 18:29:59 2020, max compression
+gzip compressed data, was "nameko_vault-0.4.0.tar", max compression
```

## Comparing `nameko-vault-0.3.0.tar` & `nameko_vault-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1076 2020-12-04 18:28:56.749524 nameko-vault-0.3.0/LICENSE
--rw-r--r--   0        0        0     2864 2020-12-04 18:28:56.749524 nameko-vault-0.3.0/README.md
--rw-r--r--   0        0        0     2195 2020-12-04 18:28:56.749524 nameko-vault-0.3.0/nameko_vault/__init__.py
--rw-r--r--   0        0        0     1125 2020-12-04 18:28:56.749524 nameko-vault-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3771 2020-12-04 18:29:59.319685 nameko-vault-0.3.0/setup.py
--rw-r--r--   0        0        0     3698 2020-12-04 18:29:59.320011 nameko-vault-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-08-04 11:37:15.761961 nameko_vault-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3112 2023-08-04 11:37:15.761961 nameko_vault-0.4.0/README.md
+-rw-r--r--   0        0        0     3289 2023-08-04 11:37:15.761961 nameko_vault-0.4.0/nameko_vault/__init__.py
+-rw-r--r--   0        0        0     1125 2023-08-04 11:37:15.761961 nameko_vault-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 nameko_vault-0.4.0/PKG-INFO
```

### Comparing `nameko-vault-0.3.0/LICENSE` & `nameko_vault-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nameko-vault-0.3.0/README.md` & `nameko_vault-0.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 vault = VaultProvider()
 vault.get_kv_secrets_list(mount_point="example", path="path")
 ```
 ```
 ['path/test1', 'path/test2']
 ```
 
-
 ## Get KV Secret Data
 
 The method `get_kv_secret` returns the content cotained in a given path
 
 ```python
 vault = VaultProvider()
 vault.get_kv_secret(mount_point="example", path="path/test")
@@ -67,15 +66,15 @@
          "version":1
       }
    }
 ]
 ```
 
 ## Create or Update KV Secret
-Method to create an secret or update an existing one in a given path. 
+Method to create an secret or update an existing one in a given path.
 
 ```python
 vault = VaultProvider()
 secret = {"example": "Test", "number": 42}
 vault.create_or_update_kv_secret(mount_point="example", path="path/test", secret=secret)
 ```
 ```
@@ -117,7 +116,16 @@
       'version': 2
    },
    'wrap_info': None,
    'warnings': None,
    'auth': None
 }
 ```
+
+## Delete KV Secret (metadata and all versions)
+Method to delete an existing path with all his versions and metadata on a given path.
+
+```python
+vault = VaultProvider()
+path = "path/secret"
+vault.delete_metadata_and_all_versions_kv_secret(path)
+```
```

### Comparing `nameko-vault-0.3.0/pyproject.toml` & `nameko_vault-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nameko-vault"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Nameko extension to provide connection with Vault"
 authors = ["Instruct Developers <oss@instruct.com.br>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/instruct-br/nameko-vault"
 repository = "https://github.com/instruct-br/nameko-vault"
 keywords = ["nameko", "vault"]
```

### Comparing `nameko-vault-0.3.0/PKG-INFO` & `nameko_vault-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nameko-vault
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Nameko extension to provide connection with Vault
 Home-page: https://github.com/instruct-br/nameko-vault
 License: MIT
 Keywords: nameko,vault
 Author: Instruct Developers
 Author-email: oss@instruct.com.br
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hvac (>=0.10.5,<0.11.0)
 Requires-Dist: nameko (>=2.12.0,<3.0.0)
 Project-URL: Repository, https://github.com/instruct-br/nameko-vault
 Description-Content-Type: text/markdown
 
 # nameko-vault
 
@@ -62,15 +64,14 @@
 vault = VaultProvider()
 vault.get_kv_secrets_list(mount_point="example", path="path")
 ```
 ```
 ['path/test1', 'path/test2']
 ```
 
-
 ## Get KV Secret Data
 
 The method `get_kv_secret` returns the content cotained in a given path
 
 ```python
 vault = VaultProvider()
 vault.get_kv_secret(mount_point="example", path="path/test")
@@ -89,15 +90,15 @@
          "version":1
       }
    }
 ]
 ```
 
 ## Create or Update KV Secret
-Method to create an secret or update an existing one in a given path. 
+Method to create an secret or update an existing one in a given path.
 
 ```python
 vault = VaultProvider()
 secret = {"example": "Test", "number": 42}
 vault.create_or_update_kv_secret(mount_point="example", path="path/test", secret=secret)
 ```
 ```
@@ -140,7 +141,16 @@
    },
    'wrap_info': None,
    'warnings': None,
    'auth': None
 }
 ```
 
+## Delete KV Secret (metadata and all versions)
+Method to delete an existing path with all his versions and metadata on a given path.
+
+```python
+vault = VaultProvider()
+path = "path/secret"
+vault.delete_metadata_and_all_versions_kv_secret(path)
+```
+
```

