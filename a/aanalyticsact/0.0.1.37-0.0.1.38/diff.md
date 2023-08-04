# Comparing `tmp/aanalyticsact-0.0.1.37.tar.gz` & `tmp/aanalyticsact-0.0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact-0.0.1.37.tar", last modified: Wed Aug  2 02:06:47 2023, max compression
+gzip compressed data, was "aanalyticsact-0.0.1.38.tar", last modified: Fri Aug  4 07:50:02 2023, max compression
```

## Comparing `aanalyticsact-0.0.1.37.tar` & `aanalyticsact-0.0.1.38.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:06:47.532731 aanalyticsact-0.0.1.37/
--rw-rw-rw-   0        0        0     1216 2023-08-02 02:06:47.534312 aanalyticsact-0.0.1.37/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.37/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 02:06:47.482580 aanalyticsact-0.0.1.37/aanalyticsact/
--rw-rw-rw-   0        0        0      118 2023-07-12 05:33:21.000000 aanalyticsact-0.0.1.37/aanalyticsact/__init__.py
--rw-rw-rw-   0        0        0       24 2023-08-02 02:05:35.000000 aanalyticsact-0.0.1.37/aanalyticsact/__version__.py
--rw-rw-rw-   0        0        0     6727 2023-07-20 00:15:03.000000 aanalyticsact-0.0.1.37/aanalyticsact/actExecute.py
--rw-rw-rw-   0        0        0    15611 2023-08-02 02:05:58.000000 aanalyticsact-0.0.1.37/aanalyticsact/actModuler.py
--rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.37/aanalyticsact/actRunner.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:06:47.524510 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/
--rw-rw-rw-   0        0        0     1216 2023-08-02 02:06:46.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-02 02:06:47.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 02:06:46.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-02 02:06:46.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-02 02:06:47.541452 aanalyticsact-0.0.1.37/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-08-02 02:05:36.000000 aanalyticsact-0.0.1.37/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:50:02.668269 aanalyticsact-0.0.1.38/
+-rw-rw-rw-   0        0        0     1216 2023-08-04 07:50:02.669672 aanalyticsact-0.0.1.38/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.38/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 07:50:02.625398 aanalyticsact-0.0.1.38/aanalyticsact/
+-rw-rw-rw-   0        0        0      118 2023-07-12 05:33:21.000000 aanalyticsact-0.0.1.38/aanalyticsact/__init__.py
+-rw-rw-rw-   0        0        0       24 2023-08-04 07:49:19.000000 aanalyticsact-0.0.1.38/aanalyticsact/__version__.py
+-rw-rw-rw-   0        0        0     6696 2023-08-04 07:49:04.000000 aanalyticsact-0.0.1.38/aanalyticsact/actExecute.py
+-rw-rw-rw-   0        0        0    16206 2023-08-04 07:48:17.000000 aanalyticsact-0.0.1.38/aanalyticsact/actModuler.py
+-rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.38/aanalyticsact/actRunner.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:50:02.662183 aanalyticsact-0.0.1.38/aanalyticsact.egg-info/
+-rw-rw-rw-   0        0        0     1216 2023-08-04 07:50:02.000000 aanalyticsact-0.0.1.38/aanalyticsact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-04 07:50:02.000000 aanalyticsact-0.0.1.38/aanalyticsact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:50:02.000000 aanalyticsact-0.0.1.38/aanalyticsact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-04 07:50:02.000000 aanalyticsact-0.0.1.38/aanalyticsact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-04 07:50:02.675658 aanalyticsact-0.0.1.38/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-08-04 07:49:13.000000 aanalyticsact-0.0.1.38/setup.py
```

### Comparing `aanalyticsact-0.0.1.37/PKG-INFO` & `aanalyticsact-0.0.1.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.37
+Version: 0.0.1.38
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.37/README.md` & `aanalyticsact-0.0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.37/aanalyticsact/actExecute.py` & `aanalyticsact-0.0.1.38/aanalyticsact/actExecute.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,30 +127,32 @@
 
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
                 continue
 
             stackTodb(sample, dbTableName)
 
-## 22.04.30 added
-def retrieve_by_RS_breakdown(start_date, end_date, period, jsonLocation, jsonLocation_breakdown, rsInput, tbColumn, dbTableName, epp, limit):
-    dateCaller = dateGenerator(start_date, end_date, period)
-    # site_code_rs = False
-    # tbColumn = tbColumnGenerator(tbColumn, False, True, True, site_code_rs)
-    tbColumn = ["rs_name", "dimension", "breakdown", "period", "start_date", "end_date", "is_epp", "is_epp_integ"]
+def retrieve_by_RS_breakdown(startDate, endDate, period, jsonFile, jsonFilebreakdown, rsInput, tbColumn, dbTableName, limit, epp, extra = "", start_hour = "00:00", end_hour = "00:00"):
+    dateCaller = dateGenerator(startDate, endDate, period)
+    defaultColumn = ["site_code", "dimension", "breakdown", "period", "start_date", "end_date", "is_epp"]
     
+    if extra != "":
+        defaultColumn.append("extra")
+
+    newColumn = defaultColumn + tbColumn
+
     startDate = dateCaller[0]
     endDate = dateCaller[1]
 
     rsList = returnRsList(epp, rsInput)
 
     for i in range(len(startDate)):
         for j in range(len(rsList)):
             try:
-                sample = refineRsIDChange_breakdown(startDate[i], endDate[i], jsonLocation, jsonLocation_breakdown, rsList[j], period, tbColumn, epp, limit)
+                secondCaller(startDate[i], endDate[i], jsonFile, jsonFilebreakdown, rsList[j], limit, period, newColumn, dbTableName, epp, extra, start_hour, end_hour)
 
             except KeyError:
                 print("Server Error occurred, please wait for the next response")
                 continue
 
             except IndexError:
                 print("Index Error occurred, please wait for the next response")
@@ -162,10 +164,9 @@
 
             except ConnectionError:
                 print("Connection Error occurred, please wait for the next response")
                 continue
 
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
-                continue                
-
-            stackTodb(sample, dbTableName)
+                continue
+
```

### Comparing `aanalyticsact-0.0.1.37/aanalyticsact/actModuler.py` & `aanalyticsact-0.0.1.38/aanalyticsact/actModuler.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,14 +237,29 @@
         itemIDlist = itemIDdfFiltered[['site_code', 'item_id']].values.tolist()        
 
     else:
         itemIDlist = itemIDdf[['site_code', 'item_id']].values.tolist()
 
     return itemIDlist
 
+def returnItemID_rs(jsonItemID):
+    dataInitiator()
+
+    itemIDdf = dataretriever_data_breakdown(jsonItemID)
+
+    columnList = list(map(str, range(itemIDdf.shape[1])))   
+
+    columnList[0] = 'site_code'
+    columnList[-1] = 'item_id'
+
+    itemIDdf.columns = columnList
+    itemIDlist = itemIDdf[['site_code', 'item_id']].values.tolist()
+
+    return itemIDlist
+
 
 # Save as dictionary format return in tuple
 def ReturnJsonchanged(startDate, endDate, jsonFile, jsonFilebreakdown, start_hour, end_hour):
     itemIDList = returnItemID(startDate, endDate, jsonFile, start_hour, end_hour)
 
     itemIDdict = {}
     for i in range(len(itemIDList)):
@@ -358,48 +373,46 @@
     else:
         dataFrame.insert(6, "is_epp_integ", "N", True)
             
     dataFrame.columns = tbColumn
     
     return dataFrame
 
-## 22.04.30 added
-def refineRsIDChange_breakdown(startDate, endDate, jsonFile, jsonFile_breakdown, rsList, period, tbColumn, epp, limit):
-    datechanged = jsonDateChange(startDate, endDate, jsonFile)
-    datechanged_breakdown = jsonDateChange(startDate, endDate, jsonFile_breakdown)
-    rschanged_jsonFile = rsIDchange(datechanged, rsList[1])
-    rschanged_jsonFile_breakdown = rsIDchange(datechanged_breakdown, rsList[1])
+def secondCaller(startDate, endDate, jsonFile, jsonFilebreakdown, rsList, limit, period, tbColumn, dbTableName, epp, extra="", start_hour="00:00", end_hour="00:00"):
+    dateChanged_json = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
+    dateChanged_bd_json = jsonDateChange(startDate, endDate, jsonFilebreakdown, start_hour, end_hour)
+    
+    rsChanged_json = rsIDchange(dateChanged_json, rsList[1])
+    rsChanged_json_bd = rsIDchange(dateChanged_bd_json, rsList[1])
+
+    itemIDList = returnItemID_rs(rsChanged_json)
+
+    itemIDdict = {}
+    for i in range(len(itemIDList)):
+        itemIDdict[itemIDList[i][0]] = ChangeItemID(itemIDList[i][1], rsChanged_json_bd)
+    
+    itemIDdict = list(zip(itemIDdict.keys(), itemIDdict.values()))
 
-    itemIDdict = ReturnJsonchanged(startDate, endDate, rschanged_jsonFile, rschanged_jsonFile_breakdown)
     for i in range(len(itemIDdict)):
         dataFrame = dataretriever_data(itemIDdict[i][1])
-
-        # limit 추가 시 넣기
+        
         if limit == 0:
-            dataFrame = dataFrame
+            dataFrame2 = dataFrame
         else:
-            dataFrame = dataFrame.head(limit)
-
-        # columnList = []
-        # for i in range(dataFrame.shape[1]):
-        #     columnList.append(i)
-
-         # dataFrame.columns = columnList
-
-        dataFrame.insert(0, "site_code", rsList[0], True)
-        dataFrame.insert(2, "period", period, True)
-        dataFrame.insert(3, "start_date", startDate, True)
-        dataFrame.insert(4, "end_date", endDate, True)
+            dataFrame2 = dataFrame.head(limit)
 
-        if epp == True:
-            dataFrame.insert(5, "is_epp", "Y", True)
-        else:
-            dataFrame.insert(5, "is_epp", "N", True)
+        # 나중에 덮어쓸 컬럼명
+        dataFrame2.insert(0, "site_code", rsList[0], True)
+        dataFrame2.insert(1, "dimension", itemIDdict[i][0], True)
+        dataFrame2.insert(3, "period", period, True)
+        if start_hour == "00:00" and end_hour == "00:00":
+            dataFrame.insert(4, "start_date", startDate, True)
+            dataFrame.insert(5, "end_date", endDate, True)
+        else :
+            dataFrame.insert(4, "start_date", "{0} {1}".format(startDate, start_hour), True)
+            dataFrame.insert(5, "end_date", "{0} {1}".format(EndDateCalculation("0", endDate)[1], end_hour), True)
+        dataFrame2.insert(6, "epp", epp, True)
+        if extra != "":
+            dataFrame2.insert(7, "extra", extra, True)
 
-        if (rsList[1] == "sssamsungnewus" or rsList[1] == "sssamsung4sec"):
-            dataFrame.insert(6, "is_epp_integ", "Y", True)
-        else:
-            dataFrame.insert(6, "is_epp_integ", "N", True)
-                
-        dataFrame.columns = tbColumn
-        
-        return dataFrame
+        dataFrame2.columns = tbColumn
+        stackTodb(dataFrame2, dbTableName)
```

### Comparing `aanalyticsact-0.0.1.37/aanalyticsact/actRunner.py` & `aanalyticsact-0.0.1.38/aanalyticsact/actRunner.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.37/aanalyticsact.egg-info/PKG-INFO` & `aanalyticsact-0.0.1.38/aanalyticsact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.37
+Version: 0.0.1.38
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.37/setup.py` & `aanalyticsact-0.0.1.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aanalyticsact",
-    version="0.0.1.37",
+    version="0.0.1.38",
     author="Sunkyeong Lee",
     author_email="sunkyeong.lee@concentrix.com",
     description="adobe analytics library for Team ACT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunkyeongLee/aanalyticsact",
     packages=setuptools.find_packages(),
```

