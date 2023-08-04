# Comparing `tmp/wfsx-1.8-py3-none-any.whl.zip` & `tmp/wfsx-1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 32794 bytes, number of entries: 20
+Zip file size: 33146 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      413 b- defN 23-Jun-06 11:13 wfsx/CONST_j.py
 -rw-rw-rw-  2.0 fat     5163 b- defN 23-Jul-28 14:45 wfsx/Excel_x.py
 -rw-rw-rw-  2.0 fat     5280 b- defN 23-Jul-28 14:45 wfsx/Report.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 11:13 wfsx/__init__.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-Jul-28 14:31 wfsx/api.py
 -rw-rw-rw-  2.0 fat     6019 b- defN 23-Jun-15 14:25 wfsx/apivalid.py
 -rw-rw-rw-  2.0 fat    16574 b- defN 23-Jul-28 14:41 wfsx/apivalidation.py
--rw-rw-rw-  2.0 fat    20715 b- defN 23-Aug-01 15:36 wfsx/common.py
--rw-rw-rw-  2.0 fat    11542 b- defN 23-Aug-01 16:30 wfsx/dataextract.py
+-rw-rw-rw-  2.0 fat    21010 b- defN 23-Aug-04 16:34 wfsx/common.py
+-rw-rw-rw-  2.0 fat    11899 b- defN 23-Aug-04 16:37 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
--rw-rw-rw-  2.0 fat     6093 b- defN 23-Aug-01 16:30 wfsx/ghelper.py
+-rw-rw-rw-  2.0 fat     7123 b- defN 23-Aug-04 16:34 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 23-Jul-27 11:01 wfsx/inix/endpointapi.ini
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1260 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1477 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/RECORD
-20 files, 135109 bytes uncompressed, 30462 bytes compressed:  77.5%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Aug-04 16:38 wfsx-1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-Aug-04 16:38 wfsx-1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 16:38 wfsx-1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-04 16:38 wfsx-1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1477 b- defN 23-Aug-04 16:38 wfsx-1.9.dist-info/RECORD
+20 files, 136791 bytes uncompressed, 30814 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: wfsx/results_validate.py
 Comment: 
 
 Filename: wfsx/inix/endpointapi.ini
 Comment: 
 
-Filename: wfsx-1.8.dist-info/LICENSE
+Filename: wfsx-1.9.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.8.dist-info/METADATA
+Filename: wfsx-1.9.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.8.dist-info/WHEEL
+Filename: wfsx-1.9.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.8.dist-info/top_level.txt
+Filename: wfsx-1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wfsx-1.8.dist-info/RECORD
+Filename: wfsx-1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wfsx/common.py

```diff
@@ -4,14 +4,15 @@
 import string
 import random
 import re
 import configparser
 from pathlib import Path
 from wfsx.parseexcel import ParseExcel
 from wfsx.apivalid import Validations
+from wfsx.ghelper import update_values_nested
 from datetime import date
 from cdxg import testdata
 
 mypath = Path.cwd()  # .parent
 # print(mypath)
 config = configparser.ConfigParser()
 data_file_path = mypath / 'config.ini'
@@ -149,25 +150,30 @@
                     if '|' in gcspt[1]:
                         getcharsx = gcspt[1].split('*')
                         mxchars = mixedcharacters(k=int(getcharsx[1]))
                     else:
                         mxchars = gcspt[1] + '_' + date_string
                     get_data[str(gcspt[0])] = str(mxchars)
                 elif xSplit[xlenn] == 'Add':
-                    gcspt = pSplit[xlenn].split('=')
-                    if '|' in gcspt[1]:
-                        getcharsx = gcspt[1].split('*')
+                    gkey, gvalue = pSplit[xlenn].split('=')
+                    if '|' in gvalue and '*' in gvalue and '.' not in gkey:
+                        getcharsx = gvalue.split('*')
                         charsx = mixedcharacters(k=int(getcharsx[1]))
+                        get_data[str(gkey)] = charsx
+                    elif '.' in gkey:
+                        cname, kname = gkey.split('.')
+                        charsx = update_values_nested(get_data, cname, kname, gvalue)
+                        get_data = charsx
                     else:
-                        mxchars = gcspt[1]
+                        mxchars = gvalue
                         if mxchars == '[]':
                             charsx = []
                         else:
                             charsx = str(mxchars)
-                    get_data[str(gcspt[0])] = charsx
+                        get_data[str(gkey)] = charsx
                 elif xSplit[xlenn] == 'Extract':
                     gcspt = pSplit[xlenn].split('=')
                     # print(gcspt)
                     gxdatax = getExtract(xdata=gcspt[1], tdata=tdata)
                     get_data[str(gcspt[0])] = gxdatax
                 elif xSplit[xlenn] == 'Dadd':
                     keyx, valuesx = pSplit[xlenn].split('=')
@@ -182,15 +188,14 @@
                         for xgmt in gmt:
                             if '.' in xgmt:
                                 grt.append(float(xgmt))
                             else:
                                 grt.append(int(xgmt))
                     except Exception:
                         for xgmt in gmt:
-                            # grt.append(xgmt+'_'+id_generator(5))
                             grt.append(xgmt)
                     get_data[str(gcspt[0])] = grt
                 else:
                     if xSplit[xlenn] == 'Remove':
                         if '=' in pSplit[xlenn]:
                             gcspt = pSplit[xlenn].split('=')
                             if '*' in gcspt[0]:
@@ -228,15 +233,14 @@
             return json.dumps(dict(get_data))
     else:
         if gtd:
             return json.dumps(dict(get_data))
         else:
             return xType
 
-
 def generate_test_api(generate_test_api, sheetname=None, exeLine=None):
     sLine, eLine = 2, None
     getxcl = ParseExcel(generate_test_api)
     getallxm = getxcl.get_sheetnames()
     getxmall = []
     if sheetname:
         for y in eval(sheetname):
```

## wfsx/dataextract.py

```diff
@@ -61,32 +61,42 @@
             # Create Splited Tables without Index
             # respdata(jsdata=getalljson, dbname=dbname)
 
         return status_code, getalljson
     except Exception as e:
         return status_code, 'httpstatus'
 
-
-def saved_request_Data(payload, vroles, tdata):
+def saved_request_Data(self, payload, vroles, tdata):
     if tdata != '!' and '!' not in tdata:
         if payload != 'None' or payload == '!' and tdata != 'None':
             try:
                 gettet = json.loads(payload)
-            except json.JSONDecodeError:
+            except Exception:
                 gettet = payload
             dp_req_file = mypath / 'test_data' / 'json_data' / 'reqdata' / vroles
             dumpData(apiselect=dp_req_file, getalljson=gettet)
 
             # Create Splited Tables with Index
             # dbname = str(vroles).split('.')[0]
             # getCreateTables(jsonDatax=gettet, dbname=dbname, reqres='request')
             # time.sleep(1)
             # Create Splited Tables without Index
             # requdata(jsdata=gettet, dbname=dbname)
 
+def get_file_headers(self, xendpoint, payload, headers):
+    files = None
+    if xendpoint.split(':')[1] == 'documents':
+        headers.pop("Content-Type", None)
+        files = payload
+        payload = {}
+    else:
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
+    return files, payload, headers
+
 def extractedValue(tdata, apipoint, ePoint=None, eValue=None, dictdata=None, gnx=0):
     global random_value, value
     getx, gnx, gxa = None, 0, None
     if ePoint is None and dictdata is None:
         if tdata != 'None' and tdata != '':
             eHome, ePoint, apxpoint, eValue = str(tdata).split('|')
             # print(eHome, ePoint, apxpoint, eValue)
```

## wfsx/ghelper.py

```diff
@@ -166,8 +166,30 @@
                 temp_data = temp_values
             elif nested_key in temp_data:
                 temp_data = temp_data[nested_key]
             else:
                 temp_data = None
                 break
         values[i] = temp_data
-    return tuple(values)
+    return tuple(values)
+
+# update_values_nested(dataxx, cname='didNo', key='didNoxxxx', new_value='+1212223|34343546546464xxx')
+# cname = root key , key = key , new_value = value, dictionary = json dict
+def update_values_nested(dictionary, cname, key, new_value):
+    if isinstance(dictionary, dict):
+        for k, v in dictionary.items():
+            if k == cname:
+                if isinstance(v, list):
+                    for item in v:
+                        if isinstance(item, dict) and key in item:
+                            item[key] = new_value
+                        else:
+                            item[key] = new_value
+                if isinstance(v, dict):
+                    v[key] = new_value
+            elif isinstance(v, dict):
+                update_values_nested(v, cname, key, new_value)
+            elif isinstance(v, list):
+                for item in v:
+                    if isinstance(item, dict):
+                        update_values_nested(item, cname, key, new_value)
+    return dictionary
```

## Comparing `wfsx-1.8.dist-info/LICENSE` & `wfsx-1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.8.dist-info/METADATA` & `wfsx-1.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.8
+Version: 1.9
 Summary: api automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfsx/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `wfsx-1.8.dist-info/RECORD` & `wfsx-1.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 wfsx/CONST_j.py,sha256=K1qp18BcG4QXmeYaMLqd8j6-_rnMj1kQ67RmtsWMFvw,413
 wfsx/Excel_x.py,sha256=-RhqrKWTi2ias2f8sMpembEYSectGn6zvhlDEaGIkIc,5163
 wfsx/Report.py,sha256=kbydYbBv0YmoOdgCQ2y92nuBNUZmYcwq4gbajGUbKMc,5280
 wfsx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfsx/api.py,sha256=4RvVwxzel6i3jpIWOw8pzM_LOCc9P9lqk8QKrvOJGXM,6310
 wfsx/apivalid.py,sha256=OZz8aFjH9BSmrvJNY7XwV1yjUYHpd7Fa6pyO-X0z0G8,6019
 wfsx/apivalidation.py,sha256=Hl6G6bv66BVnlN6iZjxATfe19LyB7yfvSHQQZ_Ue0Sg,16574
-wfsx/common.py,sha256=g4wdM0P_O3Uw4WV5jLzD4-koqIgIrWPD4CsHzXNwLoY,20715
-wfsx/dataextract.py,sha256=4Sn0xmVS8nHyqbSz0X-JJeFSgR4tJb1sLRAnLw9WH5A,11542
+wfsx/common.py,sha256=B2EIYs5TID7qYie-oHALdJJRwYg8wTXVQRhEihnAV1g,21010
+wfsx/dataextract.py,sha256=futrL_K1HFf6a1NOvOnjEOpVjtMZr5heK0eecOH4apM,11899
 wfsx/excel_json_reader.py,sha256=z4vQkNRLKCO7x3UAeI8EVd9vjY5GDTEYDOVTj2jqICA,2808
-wfsx/ghelper.py,sha256=TCUuHHBjKbuXZFOWy73Ue11JU2k8WnebFRM_E4bD2r8,6093
+wfsx/ghelper.py,sha256=OKdwitkLDX9-KNqKk9JQMB6JrJMfsNBZKsJ3H5RaWbE,7123
 wfsx/parseexcel.py,sha256=uXXUcI9AiDHqdaKd8oGAxu_3OXFmuw66CLRXvJRXHtc,5407
 wfsx/plite.py,sha256=d2yNK_XkO17OFQbr4Ecf_OSkDgys9vzdefnm03Lm3Ck,7022
 wfsx/results_validate.py,sha256=Jzx6xUHcbrTQuKhc9q48vKR7BXmSrEbD8T7SB45c_NM,23242
 wfsx/inix/endpointapi.ini,sha256=0NfMZyTdLlBseaPlWWtzLFShX2qGODskfJ7PVUVnK34,4322
-wfsx-1.8.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfsx-1.8.dist-info/METADATA,sha256=kRllBKLo55sglIyLaArN5BFExhLwLsinmCTUmPo06Kw,1260
-wfsx-1.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfsx-1.8.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
-wfsx-1.8.dist-info/RECORD,,
+wfsx-1.9.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfsx-1.9.dist-info/METADATA,sha256=Rf-Tdq0J7htgQ9f1zJ09c-PwDp-5kRjntWKTaMJ41vc,1260
+wfsx-1.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfsx-1.9.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
+wfsx-1.9.dist-info/RECORD,,
```

