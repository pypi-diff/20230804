# Comparing `tmp/vnac-0.1.0.tar.gz` & `tmp/vnac-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnac-0.1.0.tar", max compression
+gzip compressed data, was "vnac-0.1.1.tar", max compression
```

## Comparing `vnac-0.1.0.tar` & `vnac-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      764 2023-08-04 07:41:51.074989 vnac-0.1.0/README.md
--rw-r--r--   0        0        0     1095 2023-08-04 07:33:42.074072 vnac-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 02:08:52.463150 vnac-0.1.0/vnac/__init__.py
--rw-r--r--   0        0        0     5585 2023-08-04 06:58:41.733549 vnac-0.1.0/vnac/corrector.py
--rw-r--r--   0        0        0     1433 2023-08-04 06:31:11.542491 vnac-0.1.0/vnac/schemas.py
--rw-r--r--   0        0        0       96 2023-08-02 02:08:25.035092 vnac-0.1.0/vnac/utils.py
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 vnac-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-08-04 08:27:23.581636 vnac-0.1.1/README.md
+-rw-r--r--   0        0        0      961 2023-08-04 08:30:08.983707 vnac-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 02:08:52.463150 vnac-0.1.1/vnac/__init__.py
+-rw-r--r--   0        0        0     5585 2023-08-04 06:58:41.733549 vnac-0.1.1/vnac/corrector.py
+-rw-r--r--   0        0        0     1433 2023-08-04 06:31:11.542491 vnac-0.1.1/vnac/schemas.py
+-rw-r--r--   0        0        0       96 2023-08-02 02:08:25.035092 vnac-0.1.1/vnac/utils.py
+-rw-r--r--   0        0        0     2133 1970-01-01 00:00:00.000000 vnac-0.1.1/PKG-INFO
```

### Comparing `vnac-0.1.0/README.md` & `vnac-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # VNAddressCorrector
 
-Correct level ward (Phường/Xã), district (Quận/Huyện), province(Tỉnh/Thành Phố) in Vietnam address.
+Correct name of 3 level division: ward (Phường/Xã), district (Quận/Huyện), province(Tỉnh/Thành Phố) in Vietnam address.
 
 ## Installation
 ```bash
 pip install vnac
 ```
 ## Usage
 ```python
 >>> from vnac.corrector import AddressCorrector
+>>> # Address must be in string format "..., {ward}, {district}, {province}" (split by ',')
 >>> address = "Số 36A Đường 29, Ấp Tân Tiến, Tân Thìng Hội, Củ Chí, HCM"
 >>> corrector = AddressCorrector()
 >>> corrected = corrector.correct(address)
 >>> corrected
 Address(country=None, province=Division(name='HCM', code=79), district=Division(name='Củ Chi', code=None), ward=Division(name='Tân Thông Hội', code=None), street=Division(name='Số 36A Đường 29, Ấp Tân Tiến', code=None))
 >>>str(corrected)
-Số 36A Đường 29, Ấp Tân Tiến, Tân Thông Hội, Củ Chi, HCM
+"Số 36A Đường 29, Ấp Tân Tiến, Tân Thông Hội, Củ Chi, HCM"
 ```
```

### Comparing `vnac-0.1.0/pyproject.toml` & `vnac-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vnac"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Ngô Trần Ngọc Sơn <ntns1607@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jasonntn/VNAddressCorrector"
 keywords = ["Vietnam", "division", "address", "locality"]
 classifiers = [
     'Natural Language :: Vietnamese',
@@ -23,18 +23,11 @@
 vietnam-provinces = "^0.5.0"
 rapidfuzz = "^3.1.2"
 python-rapidjson = "^1.10"
 loguru = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
-ipykernel = "^6.25.0"
-
-[tool.black]
-line-length = 120
-target-version = ['py310']
-include = '\.pyi?$'
-skip-string-normalization = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vnac-0.1.0/vnac/corrector.py` & `vnac-0.1.1/vnac/corrector.py`

 * *Files identical despite different names*

### Comparing `vnac-0.1.0/vnac/schemas.py` & `vnac-0.1.1/vnac/schemas.py`

 * *Files identical despite different names*

### Comparing `vnac-0.1.0/PKG-INFO` & `vnac-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnac
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/jasonntn/VNAddressCorrector
 Keywords: Vietnam,division,address,locality
 Author: Ngô Trần Ngọc Sơn
 Author-email: ntns1607@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -26,25 +26,26 @@
 Requires-Dist: rapidfuzz (>=3.1.2,<4.0.0)
 Requires-Dist: vietnam-provinces (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/jasonntn/VNAddressCorrector
 Description-Content-Type: text/markdown
 
 # VNAddressCorrector
 
-Correct level ward (Phường/Xã), district (Quận/Huyện), province(Tỉnh/Thành Phố) in Vietnam address.
+Correct name of 3 level division: ward (Phường/Xã), district (Quận/Huyện), province(Tỉnh/Thành Phố) in Vietnam address.
 
 ## Installation
 ```bash
 pip install vnac
 ```
 ## Usage
 ```python
 >>> from vnac.corrector import AddressCorrector
+>>> # Address must be in string format "..., {ward}, {district}, {province}" (split by ',')
 >>> address = "Số 36A Đường 29, Ấp Tân Tiến, Tân Thìng Hội, Củ Chí, HCM"
 >>> corrector = AddressCorrector()
 >>> corrected = corrector.correct(address)
 >>> corrected
 Address(country=None, province=Division(name='HCM', code=79), district=Division(name='Củ Chi', code=None), ward=Division(name='Tân Thông Hội', code=None), street=Division(name='Số 36A Đường 29, Ấp Tân Tiến', code=None))
 >>>str(corrected)
-Số 36A Đường 29, Ấp Tân Tiến, Tân Thông Hội, Củ Chi, HCM
+"Số 36A Đường 29, Ấp Tân Tiến, Tân Thông Hội, Củ Chi, HCM"
 ```
```

