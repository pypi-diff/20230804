# Comparing `tmp/A_Api_Server-1.1.5.tar.gz` & `tmp/A_Api_Server-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/A_Api_Server-1.1.5.tar", last modified: Tue Nov 10 11:17:52 2020, max compression
+gzip compressed data, was "dist/A_Api_Server-1.1.6.tar", last modified: Fri Aug  4 03:00:35 2023, max compression
```

## Comparing `A_Api_Server-1.1.5.tar` & `A_Api_Server-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14523 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/PKG-INFO
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)    10339 2020-11-10 11:09:55.000000 A_Api_Server-1.1.5/README.md
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)     3075 2020-06-17 06:16:03.000000 A_Api_Server-1.1.5/setup.py
-drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14523 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/PKG-INFO
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)      314 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)       67 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/entry_points.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)        6 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/requires.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)       13 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/top_level.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)        1 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)       38 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/setup.cfg
-drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/a_api_server/
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)        0 2020-06-17 06:28:41.000000 A_Api_Server-1.1.5/a_api_server/__init__.py
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)     6545 2020-11-10 11:14:36.000000 A_Api_Server-1.1.5/a_api_server/api_server.py
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)      436 2020-11-10 11:12:37.000000 A_Api_Server-1.1.5/a_api_server/__about__.py
+drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14556 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/PKG-INFO
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)    10364 2023-08-04 02:45:12.000000 A_Api_Server-1.1.6/README.md
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)     3075 2023-08-04 02:45:12.000000 A_Api_Server-1.1.6/setup.py
+drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/A_Api_Server.egg-info/
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14556 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/A_Api_Server.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)      314 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/A_Api_Server.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)       67 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/A_Api_Server.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)        6 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/A_Api_Server.egg-info/requires.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)       13 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/A_Api_Server.egg-info/top_level.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)        1 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/A_Api_Server.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)       38 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/setup.cfg
+drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2023-08-04 03:00:35.000000 A_Api_Server-1.1.6/a_api_server/
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)        0 2023-08-04 02:45:12.000000 A_Api_Server-1.1.6/a_api_server/__init__.py
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)     6552 2023-08-04 02:47:16.000000 A_Api_Server-1.1.6/a_api_server/api_server.py
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)      436 2023-08-04 02:48:06.000000 A_Api_Server-1.1.6/a_api_server/__about__.py
```

### Comparing `A_Api_Server-1.1.5/PKG-INFO` & `A_Api_Server-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: A_Api_Server
-Version: 1.1.5
+Version: 1.1.6
 Summary: 自建一个Resful风格的接口自助服务，方便API自动化测试工具的开发与调试！
 Home-page: https://github.com/zhuifengshen/a-api-server
 Author: devin
 Author-email: 1324556701@qq.com
 License: MIT
 Description: # A Api Server
         
         ## 一、概述
         
         A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
         
         #### 1. 本地启动服务
         
-        - （1）pipy 安装启动
+        - （1）命令行启动
         
         ```
         pip install A-Api-Server
         a_api_server 自定义端口号（默认5000）
         ```
         
         - （2）clone 源码启动
         
         ```
+        pip install gunicorn flask
         cd a_api_server
         python api_server.py 自定义端口号（默认5000）
         ```
         
         （注意：兼容 Python2 和 Python3）
         
         ### 2. 服务端启动服务，推荐使用 gunicorn
```

### Comparing `A_Api_Server-1.1.5/README.md` & `A_Api_Server-1.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 ## 一、概述
 
 A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
 
 #### 1. 本地启动服务
 
-- （1）pipy 安装启动
+- （1）命令行启动
 
 ```
 pip install A-Api-Server
 a_api_server 自定义端口号（默认5000）
 ```
 
 - （2）clone 源码启动
 
 ```
+pip install gunicorn flask
 cd a_api_server
 python api_server.py 自定义端口号（默认5000）
 ```
 
 （注意：兼容 Python2 和 Python3）
 
 ### 2. 服务端启动服务，推荐使用 gunicorn
```

### Comparing `A_Api_Server-1.1.5/setup.py` & `A_Api_Server-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `A_Api_Server-1.1.5/A_Api_Server.egg-info/PKG-INFO` & `A_Api_Server-1.1.6/A_Api_Server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: A-Api-Server
-Version: 1.1.5
+Version: 1.1.6
 Summary: 自建一个Resful风格的接口自助服务，方便API自动化测试工具的开发与调试！
 Home-page: https://github.com/zhuifengshen/a-api-server
 Author: devin
 Author-email: 1324556701@qq.com
 License: MIT
 Description: # A Api Server
         
         ## 一、概述
         
         A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
         
         #### 1. 本地启动服务
         
-        - （1）pipy 安装启动
+        - （1）命令行启动
         
         ```
         pip install A-Api-Server
         a_api_server 自定义端口号（默认5000）
         ```
         
         - （2）clone 源码启动
         
         ```
+        pip install gunicorn flask
         cd a_api_server
         python api_server.py 自定义端口号（默认5000）
         ```
         
         （注意：兼容 Python2 和 Python3）
         
         ### 2. 服务端启动服务，推荐使用 gunicorn
```

### Comparing `A_Api_Server-1.1.5/a_api_server/api_server.py` & `A_Api_Server-1.1.6/a_api_server/api_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     return """
         <div style="text-align: center;">
             <h1>A Api Server</h1>
             <p><a href="https://github.com/zhuifengshen/a-api-server">A Api Server</a>，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！</p>
         </div>
     """
 
-@app.route('/api/get-token', methods=['POST'])
+@app.route('/api/get-token/', methods=['POST'])
 def get_token():
     user_agent = request.headers.get('User-Agent', "")
     device_sn = request.headers.get('device_sn', "")
     os_platform = request.headers.get('os_platform', "")
     app_version = request.headers.get('app_version', "")
     data = request.get_json()
     sign = data.get('sign', "")
@@ -124,39 +124,39 @@
             'token': token
         }
         response = make_response(json.dumps(result))
 
     response.headers["Content-Type"] = "application/json"
     return response
 
-@app.route('/api/users')
+@app.route('/api/users/')
 @validate_request
 def get_users():
     users_list = [user for uid, user in users_dict.items()]
     users = {
         'success': True,
         'count': len(users_list),
         'items': users_list
     }
     response = make_response(json.dumps(users))
     response.headers["Content-Type"] = "application/json"
     return response
 
-@app.route('/api/reset-all')
+@app.route('/api/reset-all/')
 @validate_request
 def clear_users():
     users_dict.clear()
     result = {
         'success': True
     }
     response = make_response(json.dumps(result))
     response.headers["Content-Type"] = "application/json"
     return response
 
-@app.route('/api/users/<int:uid>', methods=['POST'])
+@app.route('/api/users/<int:uid>/', methods=['POST'])
 @validate_request
 def create_user(uid):
     user = request.get_json()
     if uid not in users_dict:
         result = {
             'success': True,
             'msg': "user created successfully."
@@ -170,15 +170,15 @@
         }
         status_code = 422
 
     response = make_response(json.dumps(result), status_code)
     response.headers["Content-Type"] = "application/json"
     return response
 
-@app.route('/api/users/<int:uid>')
+@app.route('/api/users/<int:uid>/')
 @validate_request
 def get_user(uid):
     user = users_dict.get(uid, {})
     if user:
         result = {
             'success': True,
             'data': user
@@ -191,15 +191,15 @@
         }
         status_code = 404
 
     response = make_response(json.dumps(result), status_code)
     response.headers["Content-Type"] = "application/json"
     return response
 
-@app.route('/api/users/<int:uid>', methods=['PUT'])
+@app.route('/api/users/<int:uid>/', methods=['PUT'])
 @validate_request
 def update_user(uid):
     user = users_dict.get(uid, {})
     if user:
         user = request.get_json()
         success = True
         status_code = 200
@@ -212,15 +212,15 @@
         'success': success,
         'data': user
     }
     response = make_response(json.dumps(result), status_code)
     response.headers["Content-Type"] = "application/json"
     return response
 
-@app.route('/api/users/<int:uid>', methods=['DELETE'])
+@app.route('/api/users/<int:uid>/', methods=['DELETE'])
 @validate_request
 def delete_user(uid):
     user = users_dict.pop(uid, {})
     if user:
         success = True
         status_code = 200
     else:
```

