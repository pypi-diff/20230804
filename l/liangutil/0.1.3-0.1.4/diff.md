# Comparing `tmp/liangutil-0.1.3.tar.gz` & `tmp/liangutil-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.1.3.tar", last modified: Thu Aug  3 07:01:49 2023, max compression
+gzip compressed data, was "liangutil-0.1.4.tar", last modified: Fri Aug  4 09:49:49 2023, max compression
```

## Comparing `liangutil-0.1.3.tar` & `liangutil-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:01:49.066432 liangutil-0.1.3/
--rw-rw-rw-   0        0        0     3624 2023-08-03 07:01:49.066432 liangutil-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1866 2023-08-03 06:30:50.000000 liangutil-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 07:01:49.062370 liangutil-0.1.3/liangutil/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.3/liangutil/__init__.py
--rw-rw-rw-   0        0        0     3511 2023-08-03 06:26:44.000000 liangutil-0.1.3/liangutil/lianglog.py
--rw-rw-rw-   0        0        0     4495 2023-08-03 06:33:35.000000 liangutil-0.1.3/liangutil/liangutils.py
--rw-rw-rw-   0        0        0     1318 2023-08-02 03:25:24.000000 liangutil-0.1.3/liangutil/minioutils.py
--rw-rw-rw-   0        0        0     6640 2023-08-03 06:59:14.000000 liangutil-0.1.3/liangutil/mysqlutils.py
--rw-rw-rw-   0        0        0      551 2023-08-02 06:39:07.000000 liangutil-0.1.3/liangutil/redisutils.py
--rw-rw-rw-   0        0        0    13047 2023-08-03 06:25:17.000000 liangutil-0.1.3/liangutil/requestutils.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:01:49.065431 liangutil-0.1.3/liangutil.egg-info/
--rw-rw-rw-   0        0        0     3624 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 07:01:49.000000 liangutil-0.1.3/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:01:49.066432 liangutil-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-08-03 07:01:39.000000 liangutil-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:49:49.473883 liangutil-0.1.4/
+-rw-rw-rw-   0        0        0     3757 2023-08-04 09:49:49.472392 liangutil-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1951 2023-08-04 09:36:49.000000 liangutil-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 09:49:49.468090 liangutil-0.1.4/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.4/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     3511 2023-08-03 06:26:44.000000 liangutil-0.1.4/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     4495 2023-08-03 06:33:35.000000 liangutil-0.1.4/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     1318 2023-08-02 03:25:24.000000 liangutil-0.1.4/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     6640 2023-08-03 06:59:14.000000 liangutil-0.1.4/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      551 2023-08-02 06:39:07.000000 liangutil-0.1.4/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0    13474 2023-08-04 09:37:25.000000 liangutil-0.1.4/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:49:49.471093 liangutil-0.1.4/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     3757 2023-08-04 09:49:49.000000 liangutil-0.1.4/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-08-04 09:49:49.000000 liangutil-0.1.4/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 09:49:49.000000 liangutil-0.1.4/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 09:49:49.000000 liangutil-0.1.4/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 09:49:49.473883 liangutil-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-08-04 09:49:45.000000 liangutil-0.1.4/setup.py
```

### Comparing `liangutil-0.1.3/PKG-INFO` & `liangutil-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.1.3
+Version: 0.1.4
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -85,14 +85,20 @@
         
         # 更新日志
         
         ## 2023年
         
         ### 8月
         
+        **2023-08-04**
+        
+        `0.1.4`
+        
+        - ChromeUtils增加隐藏浏览器特征和反屏蔽
+        
         **2023-08-03**
         
         `0.1.3`
         
         - 取消了某些函数的捕获异常
         - 修复了一些Bug
```

### Comparing `liangutil-0.1.3/README.md` & `liangutil-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,20 @@
 
 # 更新日志
 
 ## 2023年
 
 ### 8月
 
+**2023-08-04**
+
+`0.1.4`
+
+- ChromeUtils增加隐藏浏览器特征和反屏蔽
+
 **2023-08-03**
 
 `0.1.3`
 
 - 取消了某些函数的捕获异常
 - 修复了一些Bug
```

### Comparing `liangutil-0.1.3/liangutil/lianglog.py` & `liangutil-0.1.4/liangutil/lianglog.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.3/liangutil/liangutils.py` & `liangutil-0.1.4/liangutil/liangutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.3/liangutil/minioutils.py` & `liangutil-0.1.4/liangutil/minioutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.3/liangutil/mysqlutils.py` & `liangutil-0.1.4/liangutil/mysqlutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.3/liangutil/redisutils.py` & `liangutil-0.1.4/liangutil/redisutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.3/liangutil/requestutils.py` & `liangutil-0.1.4/liangutil/requestutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -233,14 +233,27 @@
         #     import undetected_chromedriver as uc  # from session not created: This version of ChromeDriver only supports Chrome version 108
         #     driver = uc.Chrome(options=chrome_options)
         # else:
         #     driver = webdriver.Chrome(options=chrome_options)
         driver = webdriver.Chrome(options=chrome_options)
         driver.set_page_load_timeout(self.timeout) # 设置页面加载超时时间
         driver.set_script_timeout(self.timeout) # 设置脚本执行超时时间。
+
+        # 隐藏浏览器特征
+        with open('./stealth.min.js') as f:
+            js = f.read()
+        driver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
+            "source": js
+        })
+
+        # 反屏蔽
+        driver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
+            "source": "Object.defineProperty(navigator, 'webdriver', {get: () => undefined})"
+        })
+
         return driver
 
 
 
 
     def refresh_chrome(self):
         """重启浏览器
```

### Comparing `liangutil-0.1.3/liangutil.egg-info/PKG-INFO` & `liangutil-0.1.4/liangutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.1.3
+Version: 0.1.4
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -85,14 +85,20 @@
         
         # 更新日志
         
         ## 2023年
         
         ### 8月
         
+        **2023-08-04**
+        
+        `0.1.4`
+        
+        - ChromeUtils增加隐藏浏览器特征和反屏蔽
+        
         **2023-08-03**
         
         `0.1.3`
         
         - 取消了某些函数的捕获异常
         - 修复了一些Bug
```

### Comparing `liangutil-0.1.3/setup.py` & `liangutil-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
 
-    version='0.1.3',
+    version='0.1.4',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

