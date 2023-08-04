# Comparing `tmp/metaboatrace_models-0.4.0.tar.gz` & `tmp/metaboatrace_models-0.5.0.tar.gz`

## Comparing `metaboatrace_models-0.4.0.tar` & `metaboatrace_models-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/requirements-dev.lock
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/requirements.lock
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/metaboatrace/models/__init__.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/metaboatrace/models/boat.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/metaboatrace/models/race.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/metaboatrace/models/racer.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/metaboatrace/models/region.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/metaboatrace/models/stadium.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/tests/metaboatrace/models/test_boat.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/tests/metaboatrace/models/test_racer.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/tests/metaboatrace/models/test_region.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/tests/metaboatrace/models/test_stadium.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/tests/metaboatrace/models/race/test_bettings.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/tests/metaboatrace/models/race/test_race_entries.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/tests/metaboatrace/models/race/test_races.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/requirements-dev.lock
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/requirements.lock
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/metaboatrace/models/__init__.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/metaboatrace/models/boat.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/metaboatrace/models/race.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/metaboatrace/models/racer.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/metaboatrace/models/region.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/metaboatrace/models/stadium.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/tests/metaboatrace/models/test_boat.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/tests/metaboatrace/models/test_racer.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/tests/metaboatrace/models/test_region.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/tests/metaboatrace/models/test_stadium.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/tests/metaboatrace/models/race/test_bettings.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/tests/metaboatrace/models/race/test_race_entries.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/tests/metaboatrace/models/race/test_races.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.5.0/PKG-INFO
```

### Comparing `metaboatrace_models-0.4.0/.github/workflows/lint.yml` & `metaboatrace_models-0.5.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/.github/workflows/publish.yml` & `metaboatrace_models-0.5.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/.github/workflows/tests.yml` & `metaboatrace_models-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/metaboatrace/models/race.py` & `metaboatrace_models-0.5.0/metaboatrace/models/race.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/metaboatrace/models/racer.py` & `metaboatrace_models-0.5.0/metaboatrace/models/racer.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 
 class RacerRank(Enum):
     A1 = 1
     A2 = 2
     B1 = 3
     B2 = 4
 
+    @classmethod
+    def from_string(cls, s: str) -> "RacerRank":
+        return cls.__members__[s]
+
 
 class Racer(BaseModel):
     registration_number: StrictInt
     last_name: str
     first_name: str = ""
-    gender: Optional[Gender]
-    term: Optional[StrictInt]
-    birth_date: Optional[date]
-    height: Optional[StrictInt]
-    born_prefecture: Optional[Prefecture]
-    branch: Optional[Branch]
-    current_rating: Optional[RacerRank]
+    gender: Optional[Gender] = None
+    term: Optional[StrictInt] = None
+    birth_date: Optional[date] = None
+    height: Optional[StrictInt] = None
+    born_prefecture: Optional[Prefecture] = None
+    branch: Optional[Branch] = None
+    current_rating: Optional[RacerRank] = None
 
 
 class RacerCondition(BaseModel):
     recorded_on: date
     racer_registration_number: StrictInt
     weight: StrictInt
     adjust: float
```

### Comparing `metaboatrace_models-0.4.0/metaboatrace/models/region.py` & `metaboatrace_models-0.5.0/metaboatrace/models/region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/metaboatrace/models/stadium.py` & `metaboatrace_models-0.5.0/metaboatrace/models/stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/tests/metaboatrace/models/test_boat.py` & `metaboatrace_models-0.5.0/tests/metaboatrace/models/test_boat.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/tests/metaboatrace/models/test_racer.py` & `metaboatrace_models-0.5.0/tests/metaboatrace/models/test_racer.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/tests/metaboatrace/models/test_region.py` & `metaboatrace_models-0.5.0/tests/metaboatrace/models/test_region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/tests/metaboatrace/models/test_stadium.py` & `metaboatrace_models-0.5.0/tests/metaboatrace/models/test_stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/tests/metaboatrace/models/race/test_bettings.py` & `metaboatrace_models-0.5.0/tests/metaboatrace/models/race/test_bettings.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/tests/metaboatrace/models/race/test_race_entries.py` & `metaboatrace_models-0.5.0/tests/metaboatrace/models/race/test_race_entries.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/tests/metaboatrace/models/race/test_races.py` & `metaboatrace_models-0.5.0/tests/metaboatrace/models/race/test_races.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/.gitignore` & `metaboatrace_models-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/LICENSE.txt` & `metaboatrace_models-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.4.0/pyproject.toml` & `metaboatrace_models-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metaboatrace.models"
-version = "0.4.0"
+version = "0.5.0"
 description = "Models of Japanese boatrace"
 authors = [
     { name = "k0kishima", email = "okishimaxyz@gmail.com" }
 ]
 dependencies = [
     "pydantic>=2.0.3",
 ]
```

