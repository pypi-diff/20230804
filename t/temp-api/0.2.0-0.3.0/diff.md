# Comparing `tmp/temp_api-0.2.0.tar.gz` & `tmp/temp_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temp_api-0.2.0.tar", max compression
+gzip compressed data, was "temp_api-0.3.0.tar", max compression
```

## Comparing `temp_api-0.2.0.tar` & `temp_api-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       11 2023-07-23 17:08:16.357430 temp_api-0.2.0/README.md
--rw-r--r--   0        0        0      378 2023-07-26 09:31:29.513699 temp_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-23 16:30:51.992714 temp_api-0.2.0/temp_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 16:31:04.296478 temp_api-0.2.0/temp_api/__main__.py
--rw-r--r--   0        0        0     1304 2023-07-26 09:30:26.256746 temp_api-0.2.0/temp_api/main.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 temp_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-07-23 17:08:16.357430 temp_api-0.3.0/README.md
+-rw-r--r--   0        0        0      436 2023-08-04 19:01:10.765237 temp_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-23 16:30:51.992714 temp_api-0.3.0/temp_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 16:31:04.296478 temp_api-0.3.0/temp_api/__main__.py
+-rw-r--r--   0        0        0     1986 2023-08-04 19:00:47.414964 temp_api-0.3.0/temp_api/main.py
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 temp_api-0.3.0/PKG-INFO
```

### Comparing `temp_api-0.2.0/temp_api/main.py` & `temp_api-0.3.0/temp_api/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,22 @@
+import logging
+import os
 from typing import Union, List, Dict
 
 import time
 from fastapi import FastAPI
 from pydantic import BaseModel
+import sentry_sdk
+
+
+logging.basicConfig(level=logging.INFO)
+
+if (sentry_dsn := os.environ.get("SENTRY_DSN")) is not None:
+    sentry_sdk.init(sentry_dsn)
+    logging.info("Sentry enabled")
 
 
 class Measurement(BaseModel):
     mac: str
     humidity: int
     temperature: int
     pressure: int
@@ -39,20 +49,35 @@
     return MEASUREMENTS.get(mac)
 
 
 def fetch_all_measurements() -> List[MeasurementWithTs]:
     return list(MEASUREMENTS.values())
 
 
-@app.post("/measurements", status_code=201)
+@app.post("/measurements", status_code=201, deprecated=True)
 def add_measurement(measurement: Measurement):
     store_measurement(measurement)
 
 
-@app.get("/measurements")
+@app.get("/measurements", deprecated=True)
 def get_all_measurements() -> List[MeasurementWithTs]:
     return fetch_all_measurements()
 
 
-@app.get("/measurements/{mac}")
+@app.get("/measurements/{mac}", deprecated=True)
 def get_measurement_by_mac(mac: str) -> Union[MeasurementWithTs, None]:
     return fetch_measurement(mac)
+
+
+@app.post("/api/v0/measurements", status_code=201)
+def v0_add_measurement(measurement: Measurement):
+    store_measurement(measurement)
+
+
+@app.get("/api/v0/measurements")
+def v0_get_all_measurements() -> List[MeasurementWithTs]:
+    return fetch_all_measurements()
+
+
+@app.get("/api/v0/measurements/{mac}")
+def v0_get_measurement_by_mac(mac: str) -> Union[MeasurementWithTs, None]:
+    return fetch_measurement(mac)
```

