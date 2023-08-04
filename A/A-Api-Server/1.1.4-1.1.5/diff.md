# Comparing `tmp/A_Api_Server-1.1.4.tar.gz` & `tmp/A_Api_Server-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/A_Api_Server-1.1.4.tar", last modified: Fri Jun 19 12:15:19 2020, max compression
+gzip compressed data, was "dist/A_Api_Server-1.1.5.tar", last modified: Tue Nov 10 11:17:52 2020, max compression
```

## Comparing `A_Api_Server-1.1.4.tar` & `A_Api_Server-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14610 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/PKG-INFO
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)    10618 2020-06-19 05:46:46.000000 A_Api_Server-1.1.4/README.md
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)     3075 2020-06-17 06:16:03.000000 A_Api_Server-1.1.4/setup.py
-drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/A_Api_Server.egg-info/
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14610 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/A_Api_Server.egg-info/PKG-INFO
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)      314 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/A_Api_Server.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)       67 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/A_Api_Server.egg-info/entry_points.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)        6 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/A_Api_Server.egg-info/requires.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)       13 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/A_Api_Server.egg-info/top_level.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)        1 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/A_Api_Server.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)       38 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/setup.cfg
-drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-06-19 12:15:19.000000 A_Api_Server-1.1.4/a_api_server/
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)        0 2020-06-17 06:28:41.000000 A_Api_Server-1.1.4/a_api_server/__init__.py
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)     6544 2020-06-19 10:57:25.000000 A_Api_Server-1.1.4/a_api_server/api_server.py
--rw-r--r--   0 zhangchuzhao   (501) staff       (20)      436 2020-06-19 12:13:48.000000 A_Api_Server-1.1.4/a_api_server/__about__.py
+drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14523 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/PKG-INFO
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)    10339 2020-11-10 11:09:55.000000 A_Api_Server-1.1.5/README.md
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)     3075 2020-06-17 06:16:03.000000 A_Api_Server-1.1.5/setup.py
+drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)    14523 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)      314 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)       67 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)        6 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/requires.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)       13 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/top_level.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)        1 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/A_Api_Server.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)       38 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/setup.cfg
+drwxr-xr-x   0 zhangchuzhao   (501) staff       (20)        0 2020-11-10 11:17:52.000000 A_Api_Server-1.1.5/a_api_server/
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)        0 2020-06-17 06:28:41.000000 A_Api_Server-1.1.5/a_api_server/__init__.py
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)     6545 2020-11-10 11:14:36.000000 A_Api_Server-1.1.5/a_api_server/api_server.py
+-rw-r--r--   0 zhangchuzhao   (501) staff       (20)      436 2020-11-10 11:12:37.000000 A_Api_Server-1.1.5/a_api_server/__about__.py
```

### Comparing `A_Api_Server-1.1.4/PKG-INFO` & `A_Api_Server-1.1.5/A_Api_Server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,377 +1,400 @@
 Metadata-Version: 2.1
-Name: A_Api_Server
-Version: 1.1.4
+Name: A-Api-Server
+Version: 1.1.5
 Summary: 自建一个Resful风格的接口自助服务，方便API自动化测试工具的开发与调试！
 Home-page: https://github.com/zhuifengshen/a-api-server
 Author: devin
 Author-email: 1324556701@qq.com
 License: MIT
 Description: # A Api Server
         
         ## 一、概述
-        A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
         
+        A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
         
         #### 1. 本地启动服务
+        
         - （1）pipy 安装启动
+        
         ```
         pip install A-Api-Server
         a_api_server 自定义端口号（默认5000）
         ```
         
         - （2）clone 源码启动
+        
         ```
         cd a_api_server
         python api_server.py 自定义端口号（默认5000）
         ```
+        
         （注意：兼容 Python2 和 Python3）
         
         ### 2. 服务端启动服务，推荐使用 gunicorn
+        
         ```
         cd a_api_server
         gunicorn api_server:app -p api_server.pid -b 0.0.0.0:5000 -w 4 -D
         
         服务端关闭服务的命令如下：
         kill -HUP `cat api_server.pid`
         kill `cat api_server.pid`
         ```
         
         ### 3. 启动后访问地址
+        
         ```
         http://your.ip:5000
         ```
         
         ## 二、接口文档
+        
         ### 1. API V1 接口说明
         
         - 接口基准地址：http://your.ip:5000/
         - 使用 HTTP Status Code 标识状态
         - 数据返回格式统一使用 JSON
         - API V1 认证统一使用 Token 认证
         - 需要授权的 API ，必须在请求头中使用`device_sn`字段提供设备序列号和 `token` 字段提供访问令牌
         - 全局请求头
         
-        | 参数名       | 参数类型  | 参数说明     | 备注                    |
-        | ----------- | -------- | ----------- | ---------------------- |
-        | Content-Type| String   | 内容类型     | application/json       |
-        | device_sn   | String   | 设备序列号    | 唯一设备标识符           |
-        | token       | String   | 访问令牌      | 拥有token的设备才有访问权 |
+        | 参数名       | 参数类型 | 参数说明   | 备注                        |
+        | ------------ | -------- | ---------- | --------------------------- |
+        | Content-Type | String   | 内容类型   | application/json            |
+        | device_sn    | String   | 设备序列号 | 唯一设备标识符              |
+        | token        | String   | 访问令牌   | 拥有 token 的设备才有访问权 |
         
         #### 1.1. 支持的请求方法
         
         - GET（SELECT）：从服务器取出资源（一项或多项）。
         - POST（CREATE）：在服务器新建一个资源。
         - PUT（UPDATE）：在服务器更新资源（客户端提供改变后的完整资源）。
         - PATCH（UPDATE）：在服务器更新资源（客户端提供改变的属性）。
         - DELETE（DELETE）：从服务器删除资源。
         - HEAD：获取资源的元数据。
         - OPTIONS：获取信息，关于资源的哪些属性是客户端可以改变的。
         
         #### 1.2. 通用返回状态说明
         
-        | *状态码* | *含义*                | *说明*                                              |
-        | -------- | --------------------- | ------------------------------------------------- |
+        | _状态码_ | _含义_                | _说明_                                              |
+        | -------- | --------------------- | --------------------------------------------------- |
         | 200      | OK                    | 请求成功                                            |
         | 201      | CREATED               | 创建成功                                            |
         | 204      | DELETED               | 删除成功                                            |
-        | 400      | BAD REQUEST           | 请求的地址不存在或者包含不支持的参数                     |
+        | 400      | BAD REQUEST           | 请求的地址不存在或者包含不支持的参数                |
         | 401      | UNAUTHORIZED          | 未授权                                              |
-        | 403      | FORBIDDEN             | 被禁止访问                                           |
-        | 404      | NOT FOUND             | 请求的资源不存在                                      |
-        | 422      | Unprocesable entity   | [POST/PUT/PATCH] 当创建一个对象时，发生一个验证错误      |
-        | 500      | INTERNAL SERVER ERROR | 内部错误                                             |
-        ------
+        | 403      | FORBIDDEN             | 被禁止访问                                          |
+        | 404      | NOT FOUND             | 请求的资源不存在                                    |
+        | 422      | Unprocesable entity   | [POST/PUT/PATCH] 当创建一个对象时，发生一个验证错误 |
+        | 500      | INTERNAL SERVER ERROR | 内部错误                                            |
+        
+        ---
         
         ### 2. 具体接口说明
         
         #### 2.1. 获取令牌
+        
         - 请求路径：/api/get-token
         - 请求方法：post
-        - 请求头 
+        - 请求头
         
-        | 参数名       | 参数类型  | 参数说明     | 备注  |
-        | ----------- | -------- | ----------- | ---- |
-        | User-Agent  | String   | 用户代理     |      |
-        | device_sn   | String   | 设备序列号    |      |
-        | os_platform | String   | 系统平台      |      |
-        | app_version | String   | 应用版本      |      | 
+        | 参数名      | 参数类型 | 参数说明   | 备注 |
+        | ----------- | -------- | ---------- | ---- |
+        | User-Agent  | String   | 用户代理   |      |
+        | device_sn   | String   | 设备序列号 |      |
+        | os_platform | String   | 系统平台   |      |
+        | app_version | String   | 应用版本   |      |
         
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注  |
-        | ----------- | -------- | ----------- | ---- |
-        | sign        | String   | 加密签名     | 根据请求头和密钥加密生成     |
+        | 参数名 | 参数类型 | 参数说明 | 备注                     |
+        | ------ | -------- | -------- | ------------------------ |
+        | sign   | String   | 加密签名 | 根据请求头和密钥加密生成 |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注    |
-        | ----------- | -------- | ----------- | ------ |
-        | success     | Boolean  | 是否成功     |         |
-        | token       | String   | 访问令牌     | 长度16位 |
+        | 参数名  | 参数类型 | 参数说明 | 备注       |
+        | ------- | -------- | -------- | ---------- |
+        | success | Boolean  | 是否成功 |            |
+        | token   | String   | 访问令牌 | 长度 16 位 |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'token': "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1aW"
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：403
         响应体：
         {
             'success': false,
             'msg': "Authorization failed!"
         }
         ```
         
         - 签名生成算法
+        
         ```python
         def get_sign(*args):
             SECRECT_KEY = 'YouMi'
         	content = ''.join(args).encode('ascii')
         	sign_key = SECRECT_KEY.encode('ascii')
         	sign = hmac.new(sign_key, content, hashlib.sha1).hexdigest()
         	return sign
         
         sign = get_sign(user_agent, device_sn, os_platform, app_version)
         
         ```
         
-        
         #### 2.2. 新建用户
+        
         - 请求路径：/api/users/:id
         - 请求方法：post
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | id          | Int      | 用户 ID     |      |
-        | name        | String   | 用户名     |      |
-        | password    | String   | 密码       |      |
+        | 参数名   | 参数类型 | 参数说明 | 备注 |
+        | -------- | -------- | -------- | ---- |
+        | id       | Int      | 用户 ID  |      |
+        | name     | String   | 用户名   |      |
+        | password | String   | 密码     |      |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | msg         | String   | 说明信息     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
+        | msg     | String   | 说明信息 |      |
         
         - 成功返回
+        
         ```
         状态码：201
         响应体：
         {
             'success': true,
             'msg': "user created successfully."
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：422
         响应体：
         {
             'success': false,
             'msg': "user already existed."
         }
         ```
         
-        
         #### 2.3. 根据 ID 查询用户信息
+        
         - 请求路径：/api/users/:id
         - 请求方法：get
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | name        | String   | 用户名     |      |
-        | password    | String   | 密码     |      |
+        | 参数名   | 参数类型 | 参数说明 | 备注 |
+        | -------- | -------- | -------- | ---- |
+        | success  | Boolean  | 是否成功 |      |
+        | name     | String   | 用户名   |      |
+        | password | String   | 密码     |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'data': {
                 'name': 'admin',
                 'password': '123456'
             }
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：404
         响应体：
         {
             'success': fasle,
             'data': {}
         }
         ```
         
         #### 2.4. 更新用户信息
+        
         - 请求路径：/api/users/:id
         - 请求方法：put
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ---------- | ---- |
-        | id          | Int      | 用户 ID     |      |
-        | name        | String   | 用户名      |      |
-        | password    | String   | 密码        |      |
+        | 参数名   | 参数类型 | 参数说明 | 备注 |
+        | -------- | -------- | -------- | ---- |
+        | id       | Int      | 用户 ID  |      |
+        | name     | String   | 用户名   |      |
+        | password | String   | 密码     |      |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | data        | Dict     | 用户信息     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
+        | data    | Dict     | 用户信息 |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'data': {
                 'name': 'admin',
                 'password': '123456'
             }
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：404
         响应体：
         {
             'success': fasle,
             'data': {}
         }
         ```
         
-        
         #### 2.5. 删除用户信息
+        
         - 请求路径：/api/users/:id
         - 请求方法：delete
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ---------- | ---- |
-        | id          | Int      | 用户 ID     |      |
-        
+        | 参数名 | 参数类型 | 参数说明 | 备注 |
+        | ------ | -------- | -------- | ---- |
+        | id     | Int      | 用户 ID  |      |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | data        | Dict     | 用户信息     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
+        | data    | Dict     | 用户信息 |      |
         
         - 成功返回
+        
         ```
-        状态码：204
+        状态码：200
         响应体：
         {
             'success': true,
             'data': {
                 'name': 'admin',
                 'password': '123456'
             }
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：404
         响应体：
         {
             'success': fasle,
             'data': {}
         }
         ```
         
         #### 2.6. 用户数据列表
+        
         - 请求路径：/api/users
         - 请求方法：get
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | count       | Int      | 用户总数     |      |
-        | items       | Array    | 用户数据集合  |      |
+        | 参数名  | 参数类型 | 参数说明     | 备注 |
+        | ------- | -------- | ------------ | ---- |
+        | success | Boolean  | 是否成功     |      |
+        | count   | Int      | 用户总数     |      |
+        | items   | Array    | 用户数据集合 |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'count': 3,
             'items': [
                 {'name': 'admin1', 'password': '123456'},
                 {'name': 'admin2', 'password': '123456'},
                 {'name': 'admin3', 'password': '123456'}
-            ]    
+            ]
         }
         ```
         
-        
         #### 2.7. 清空用户数据
+        
         - 请求路径：/api/reset-all
         - 请求方法：get
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true
         }
         ```
         
+        ## 三、自动化发布：一键打 Tag 并上传至 PYPI
         
-        ## 三、自动化发布：一键打 Tag 并上传至 PYPI 
-        
-        每次在 __ about __.py 更新版本号后，运行以下命令，实现自动化更新打包上传至 [PYPI](https://pypi.org/) ，同时根据其版本号自动打 Tag 并推送到仓库：
+        每次在 ** about **.py 更新版本号后，运行以下命令，实现自动化更新打包上传至 [PYPI](https://pypi.org/) ，同时根据其版本号自动打 Tag 并推送到仓库：
         
         ```
         python3 setup.py pypi
         ```
-        注意：上传前需提前在twine工具中配置自己的Pypi的账号信息！！！
         
+        注意：上传前需提前在 twine 工具中配置自己的 Pypi 的账号信息！！！
         
         ### 四、CHANGELOG
         
         ```
         v1.0.0
         1、实现对用户账号进行增删改查功能的 API 服务，包含了接口的签名校验机制；
         2、完善了 API 使用文档；
         3、添加了自动化打包脚本；
         ```
         
         ## 五、致谢
-        **A-Api-Server** 工具的产生和打包，主要参考了开源项目 [HttpRunner](https://github.com/httprunner/httprunner)，受益多多，感谢！
         
+        **A-Api-Server** 工具的产生和打包，主要参考了开源项目 [HttpRunner](https://github.com/httprunner/httprunner)，受益多多，感谢！
         
         ## LICENSE
+        
         ```
         MIT License
         
         Copyright (c) 2019 Devin https://zhangchuzhao.site
         Copyright (c) 2017 Toby Qin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -388,14 +411,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         ```
+        
 Keywords: ApiServer,Api,MockServer,Api Test,接口测试,接口自动化测试
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `A_Api_Server-1.1.4/README.md` & `A_Api_Server-1.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,369 +1,392 @@
 # A Api Server
 
 ## 一、概述
-A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
 
+A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
 
 #### 1. 本地启动服务
+
 - （1）pipy 安装启动
+
 ```
 pip install A-Api-Server
 a_api_server 自定义端口号（默认5000）
 ```
 
 - （2）clone 源码启动
+
 ```
 cd a_api_server
 python api_server.py 自定义端口号（默认5000）
 ```
+
 （注意：兼容 Python2 和 Python3）
 
 ### 2. 服务端启动服务，推荐使用 gunicorn
+
 ```
 cd a_api_server
 gunicorn api_server:app -p api_server.pid -b 0.0.0.0:5000 -w 4 -D
 
 服务端关闭服务的命令如下：
 kill -HUP `cat api_server.pid`
 kill `cat api_server.pid`
 ```
 
 ### 3. 启动后访问地址
+
 ```
 http://your.ip:5000
 ```
 
 ## 二、接口文档
+
 ### 1. API V1 接口说明
 
 - 接口基准地址：http://your.ip:5000/
 - 使用 HTTP Status Code 标识状态
 - 数据返回格式统一使用 JSON
 - API V1 认证统一使用 Token 认证
 - 需要授权的 API ，必须在请求头中使用`device_sn`字段提供设备序列号和 `token` 字段提供访问令牌
 - 全局请求头
 
-| 参数名       | 参数类型  | 参数说明     | 备注                    |
-| ----------- | -------- | ----------- | ---------------------- |
-| Content-Type| String   | 内容类型     | application/json       |
-| device_sn   | String   | 设备序列号    | 唯一设备标识符           |
-| token       | String   | 访问令牌      | 拥有token的设备才有访问权 |
+| 参数名       | 参数类型 | 参数说明   | 备注                        |
+| ------------ | -------- | ---------- | --------------------------- |
+| Content-Type | String   | 内容类型   | application/json            |
+| device_sn    | String   | 设备序列号 | 唯一设备标识符              |
+| token        | String   | 访问令牌   | 拥有 token 的设备才有访问权 |
 
 #### 1.1. 支持的请求方法
 
 - GET（SELECT）：从服务器取出资源（一项或多项）。
 - POST（CREATE）：在服务器新建一个资源。
 - PUT（UPDATE）：在服务器更新资源（客户端提供改变后的完整资源）。
 - PATCH（UPDATE）：在服务器更新资源（客户端提供改变的属性）。
 - DELETE（DELETE）：从服务器删除资源。
 - HEAD：获取资源的元数据。
 - OPTIONS：获取信息，关于资源的哪些属性是客户端可以改变的。
 
 #### 1.2. 通用返回状态说明
 
-| *状态码* | *含义*                | *说明*                                              |
-| -------- | --------------------- | ------------------------------------------------- |
+| _状态码_ | _含义_                | _说明_                                              |
+| -------- | --------------------- | --------------------------------------------------- |
 | 200      | OK                    | 请求成功                                            |
 | 201      | CREATED               | 创建成功                                            |
 | 204      | DELETED               | 删除成功                                            |
-| 400      | BAD REQUEST           | 请求的地址不存在或者包含不支持的参数                     |
+| 400      | BAD REQUEST           | 请求的地址不存在或者包含不支持的参数                |
 | 401      | UNAUTHORIZED          | 未授权                                              |
-| 403      | FORBIDDEN             | 被禁止访问                                           |
-| 404      | NOT FOUND             | 请求的资源不存在                                      |
-| 422      | Unprocesable entity   | [POST/PUT/PATCH] 当创建一个对象时，发生一个验证错误      |
-| 500      | INTERNAL SERVER ERROR | 内部错误                                             |
-------
+| 403      | FORBIDDEN             | 被禁止访问                                          |
+| 404      | NOT FOUND             | 请求的资源不存在                                    |
+| 422      | Unprocesable entity   | [POST/PUT/PATCH] 当创建一个对象时，发生一个验证错误 |
+| 500      | INTERNAL SERVER ERROR | 内部错误                                            |
+
+---
 
 ### 2. 具体接口说明
 
 #### 2.1. 获取令牌
+
 - 请求路径：/api/get-token
 - 请求方法：post
-- 请求头 
+- 请求头
 
-| 参数名       | 参数类型  | 参数说明     | 备注  |
-| ----------- | -------- | ----------- | ---- |
-| User-Agent  | String   | 用户代理     |      |
-| device_sn   | String   | 设备序列号    |      |
-| os_platform | String   | 系统平台      |      |
-| app_version | String   | 应用版本      |      | 
+| 参数名      | 参数类型 | 参数说明   | 备注 |
+| ----------- | -------- | ---------- | ---- |
+| User-Agent  | String   | 用户代理   |      |
+| device_sn   | String   | 设备序列号 |      |
+| os_platform | String   | 系统平台   |      |
+| app_version | String   | 应用版本   |      |
 
 - 请求参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注  |
-| ----------- | -------- | ----------- | ---- |
-| sign        | String   | 加密签名     | 根据请求头和密钥加密生成     |
+| 参数名 | 参数类型 | 参数说明 | 备注                     |
+| ------ | -------- | -------- | ------------------------ |
+| sign   | String   | 加密签名 | 根据请求头和密钥加密生成 |
 
 - 响应参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注    |
-| ----------- | -------- | ----------- | ------ |
-| success     | Boolean  | 是否成功     |         |
-| token       | String   | 访问令牌     | 长度16位 |
+| 参数名  | 参数类型 | 参数说明 | 备注       |
+| ------- | -------- | -------- | ---------- |
+| success | Boolean  | 是否成功 |            |
+| token   | String   | 访问令牌 | 长度 16 位 |
 
 - 成功返回
+
 ```
 状态码：200
 响应体：
 {
     'success': true,
     'token': "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1aW"
 }
 ```
 
 - 失败返回
+
 ```
 状态码：403
 响应体：
 {
     'success': false,
     'msg': "Authorization failed!"
 }
 ```
 
 - 签名生成算法
+
 ```python
 def get_sign(*args):
     SECRECT_KEY = 'YouMi'
 	content = ''.join(args).encode('ascii')
 	sign_key = SECRECT_KEY.encode('ascii')
 	sign = hmac.new(sign_key, content, hashlib.sha1).hexdigest()
 	return sign
 
 sign = get_sign(user_agent, device_sn, os_platform, app_version)
 
 ```
 
-
 #### 2.2. 新建用户
+
 - 请求路径：/api/users/:id
 - 请求方法：post
 - 请求参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ----------- | ---- |
-| id          | Int      | 用户 ID     |      |
-| name        | String   | 用户名     |      |
-| password    | String   | 密码       |      |
+| 参数名   | 参数类型 | 参数说明 | 备注 |
+| -------- | -------- | -------- | ---- |
+| id       | Int      | 用户 ID  |      |
+| name     | String   | 用户名   |      |
+| password | String   | 密码     |      |
 
 - 响应参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ----------- | ---- |
-| success     | Boolean  | 是否成功     |      |
-| msg         | String   | 说明信息     |      |
+| 参数名  | 参数类型 | 参数说明 | 备注 |
+| ------- | -------- | -------- | ---- |
+| success | Boolean  | 是否成功 |      |
+| msg     | String   | 说明信息 |      |
 
 - 成功返回
+
 ```
 状态码：201
 响应体：
 {
     'success': true,
     'msg': "user created successfully."
 }
 ```
 
 - 失败返回
+
 ```
 状态码：422
 响应体：
 {
     'success': false,
     'msg': "user already existed."
 }
 ```
 
-
 #### 2.3. 根据 ID 查询用户信息
+
 - 请求路径：/api/users/:id
 - 请求方法：get
 - 响应参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ----------- | ---- |
-| success     | Boolean  | 是否成功     |      |
-| name        | String   | 用户名     |      |
-| password    | String   | 密码     |      |
+| 参数名   | 参数类型 | 参数说明 | 备注 |
+| -------- | -------- | -------- | ---- |
+| success  | Boolean  | 是否成功 |      |
+| name     | String   | 用户名   |      |
+| password | String   | 密码     |      |
 
 - 成功返回
+
 ```
 状态码：200
 响应体：
 {
     'success': true,
     'data': {
         'name': 'admin',
         'password': '123456'
     }
 }
 ```
 
 - 失败返回
+
 ```
 状态码：404
 响应体：
 {
     'success': fasle,
     'data': {}
 }
 ```
 
 #### 2.4. 更新用户信息
+
 - 请求路径：/api/users/:id
 - 请求方法：put
 - 请求参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ---------- | ---- |
-| id          | Int      | 用户 ID     |      |
-| name        | String   | 用户名      |      |
-| password    | String   | 密码        |      |
+| 参数名   | 参数类型 | 参数说明 | 备注 |
+| -------- | -------- | -------- | ---- |
+| id       | Int      | 用户 ID  |      |
+| name     | String   | 用户名   |      |
+| password | String   | 密码     |      |
 
 - 响应参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ----------- | ---- |
-| success     | Boolean  | 是否成功     |      |
-| data        | Dict     | 用户信息     |      |
+| 参数名  | 参数类型 | 参数说明 | 备注 |
+| ------- | -------- | -------- | ---- |
+| success | Boolean  | 是否成功 |      |
+| data    | Dict     | 用户信息 |      |
 
 - 成功返回
+
 ```
 状态码：200
 响应体：
 {
     'success': true,
     'data': {
         'name': 'admin',
         'password': '123456'
     }
 }
 ```
 
 - 失败返回
+
 ```
 状态码：404
 响应体：
 {
     'success': fasle,
     'data': {}
 }
 ```
 
-
 #### 2.5. 删除用户信息
+
 - 请求路径：/api/users/:id
 - 请求方法：delete
 - 请求参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ---------- | ---- |
-| id          | Int      | 用户 ID     |      |
-
+| 参数名 | 参数类型 | 参数说明 | 备注 |
+| ------ | -------- | -------- | ---- |
+| id     | Int      | 用户 ID  |      |
 
 - 响应参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ----------- | ---- |
-| success     | Boolean  | 是否成功     |      |
-| data        | Dict     | 用户信息     |      |
+| 参数名  | 参数类型 | 参数说明 | 备注 |
+| ------- | -------- | -------- | ---- |
+| success | Boolean  | 是否成功 |      |
+| data    | Dict     | 用户信息 |      |
 
 - 成功返回
+
 ```
-状态码：204
+状态码：200
 响应体：
 {
     'success': true,
     'data': {
         'name': 'admin',
         'password': '123456'
     }
 }
 ```
 
 - 失败返回
+
 ```
 状态码：404
 响应体：
 {
     'success': fasle,
     'data': {}
 }
 ```
 
 #### 2.6. 用户数据列表
+
 - 请求路径：/api/users
 - 请求方法：get
 - 响应参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ----------- | ---- |
-| success     | Boolean  | 是否成功     |      |
-| count       | Int      | 用户总数     |      |
-| items       | Array    | 用户数据集合  |      |
+| 参数名  | 参数类型 | 参数说明     | 备注 |
+| ------- | -------- | ------------ | ---- |
+| success | Boolean  | 是否成功     |      |
+| count   | Int      | 用户总数     |      |
+| items   | Array    | 用户数据集合 |      |
 
 - 成功返回
+
 ```
 状态码：200
 响应体：
 {
     'success': true,
     'count': 3,
     'items': [
         {'name': 'admin1', 'password': '123456'},
         {'name': 'admin2', 'password': '123456'},
         {'name': 'admin3', 'password': '123456'}
-    ]    
+    ]
 }
 ```
 
-
 #### 2.7. 清空用户数据
+
 - 请求路径：/api/reset-all
 - 请求方法：get
 - 响应参数
 
-| 参数名       | 参数类型  | 参数说明     | 备注 |
-| ----------- | -------- | ----------- | ---- |
-| success     | Boolean  | 是否成功     |      |
+| 参数名  | 参数类型 | 参数说明 | 备注 |
+| ------- | -------- | -------- | ---- |
+| success | Boolean  | 是否成功 |      |
 
 - 成功返回
+
 ```
 状态码：200
 响应体：
 {
     'success': true
 }
 ```
 
+## 三、自动化发布：一键打 Tag 并上传至 PYPI
 
-## 三、自动化发布：一键打 Tag 并上传至 PYPI 
-
-每次在 __ about __.py 更新版本号后，运行以下命令，实现自动化更新打包上传至 [PYPI](https://pypi.org/) ，同时根据其版本号自动打 Tag 并推送到仓库：
+每次在 ** about **.py 更新版本号后，运行以下命令，实现自动化更新打包上传至 [PYPI](https://pypi.org/) ，同时根据其版本号自动打 Tag 并推送到仓库：
 
 ```
 python3 setup.py pypi
 ```
-注意：上传前需提前在twine工具中配置自己的Pypi的账号信息！！！
 
+注意：上传前需提前在 twine 工具中配置自己的 Pypi 的账号信息！！！
 
 ### 四、CHANGELOG
 
 ```
 v1.0.0
 1、实现对用户账号进行增删改查功能的 API 服务，包含了接口的签名校验机制；
 2、完善了 API 使用文档；
 3、添加了自动化打包脚本；
 ```
 
 ## 五、致谢
-**A-Api-Server** 工具的产生和打包，主要参考了开源项目 [HttpRunner](https://github.com/httprunner/httprunner)，受益多多，感谢！
 
+**A-Api-Server** 工具的产生和打包，主要参考了开源项目 [HttpRunner](https://github.com/httprunner/httprunner)，受益多多，感谢！
 
 ## LICENSE
+
 ```
 MIT License
 
 Copyright (c) 2019 Devin https://zhangchuzhao.site
 Copyright (c) 2017 Toby Qin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -379,8 +402,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-```
+```
```

### Comparing `A_Api_Server-1.1.4/setup.py` & `A_Api_Server-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `A_Api_Server-1.1.4/A_Api_Server.egg-info/PKG-INFO` & `A_Api_Server-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,377 +1,400 @@
 Metadata-Version: 2.1
-Name: A-Api-Server
-Version: 1.1.4
+Name: A_Api_Server
+Version: 1.1.5
 Summary: 自建一个Resful风格的接口自助服务，方便API自动化测试工具的开发与调试！
 Home-page: https://github.com/zhuifengshen/a-api-server
 Author: devin
 Author-email: 1324556701@qq.com
 License: MIT
 Description: # A Api Server
         
         ## 一、概述
-        A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
         
+        A api server，是一个 Resful 风格的简易 API 服务，提供了对用户账号进行增删改查（CRUD）功能的接口服务，包含了接口的签名校验机制，方便 API 自动化测试工具的开发与调试！
         
         #### 1. 本地启动服务
+        
         - （1）pipy 安装启动
+        
         ```
         pip install A-Api-Server
         a_api_server 自定义端口号（默认5000）
         ```
         
         - （2）clone 源码启动
+        
         ```
         cd a_api_server
         python api_server.py 自定义端口号（默认5000）
         ```
+        
         （注意：兼容 Python2 和 Python3）
         
         ### 2. 服务端启动服务，推荐使用 gunicorn
+        
         ```
         cd a_api_server
         gunicorn api_server:app -p api_server.pid -b 0.0.0.0:5000 -w 4 -D
         
         服务端关闭服务的命令如下：
         kill -HUP `cat api_server.pid`
         kill `cat api_server.pid`
         ```
         
         ### 3. 启动后访问地址
+        
         ```
         http://your.ip:5000
         ```
         
         ## 二、接口文档
+        
         ### 1. API V1 接口说明
         
         - 接口基准地址：http://your.ip:5000/
         - 使用 HTTP Status Code 标识状态
         - 数据返回格式统一使用 JSON
         - API V1 认证统一使用 Token 认证
         - 需要授权的 API ，必须在请求头中使用`device_sn`字段提供设备序列号和 `token` 字段提供访问令牌
         - 全局请求头
         
-        | 参数名       | 参数类型  | 参数说明     | 备注                    |
-        | ----------- | -------- | ----------- | ---------------------- |
-        | Content-Type| String   | 内容类型     | application/json       |
-        | device_sn   | String   | 设备序列号    | 唯一设备标识符           |
-        | token       | String   | 访问令牌      | 拥有token的设备才有访问权 |
+        | 参数名       | 参数类型 | 参数说明   | 备注                        |
+        | ------------ | -------- | ---------- | --------------------------- |
+        | Content-Type | String   | 内容类型   | application/json            |
+        | device_sn    | String   | 设备序列号 | 唯一设备标识符              |
+        | token        | String   | 访问令牌   | 拥有 token 的设备才有访问权 |
         
         #### 1.1. 支持的请求方法
         
         - GET（SELECT）：从服务器取出资源（一项或多项）。
         - POST（CREATE）：在服务器新建一个资源。
         - PUT（UPDATE）：在服务器更新资源（客户端提供改变后的完整资源）。
         - PATCH（UPDATE）：在服务器更新资源（客户端提供改变的属性）。
         - DELETE（DELETE）：从服务器删除资源。
         - HEAD：获取资源的元数据。
         - OPTIONS：获取信息，关于资源的哪些属性是客户端可以改变的。
         
         #### 1.2. 通用返回状态说明
         
-        | *状态码* | *含义*                | *说明*                                              |
-        | -------- | --------------------- | ------------------------------------------------- |
+        | _状态码_ | _含义_                | _说明_                                              |
+        | -------- | --------------------- | --------------------------------------------------- |
         | 200      | OK                    | 请求成功                                            |
         | 201      | CREATED               | 创建成功                                            |
         | 204      | DELETED               | 删除成功                                            |
-        | 400      | BAD REQUEST           | 请求的地址不存在或者包含不支持的参数                     |
+        | 400      | BAD REQUEST           | 请求的地址不存在或者包含不支持的参数                |
         | 401      | UNAUTHORIZED          | 未授权                                              |
-        | 403      | FORBIDDEN             | 被禁止访问                                           |
-        | 404      | NOT FOUND             | 请求的资源不存在                                      |
-        | 422      | Unprocesable entity   | [POST/PUT/PATCH] 当创建一个对象时，发生一个验证错误      |
-        | 500      | INTERNAL SERVER ERROR | 内部错误                                             |
-        ------
+        | 403      | FORBIDDEN             | 被禁止访问                                          |
+        | 404      | NOT FOUND             | 请求的资源不存在                                    |
+        | 422      | Unprocesable entity   | [POST/PUT/PATCH] 当创建一个对象时，发生一个验证错误 |
+        | 500      | INTERNAL SERVER ERROR | 内部错误                                            |
+        
+        ---
         
         ### 2. 具体接口说明
         
         #### 2.1. 获取令牌
+        
         - 请求路径：/api/get-token
         - 请求方法：post
-        - 请求头 
+        - 请求头
         
-        | 参数名       | 参数类型  | 参数说明     | 备注  |
-        | ----------- | -------- | ----------- | ---- |
-        | User-Agent  | String   | 用户代理     |      |
-        | device_sn   | String   | 设备序列号    |      |
-        | os_platform | String   | 系统平台      |      |
-        | app_version | String   | 应用版本      |      | 
+        | 参数名      | 参数类型 | 参数说明   | 备注 |
+        | ----------- | -------- | ---------- | ---- |
+        | User-Agent  | String   | 用户代理   |      |
+        | device_sn   | String   | 设备序列号 |      |
+        | os_platform | String   | 系统平台   |      |
+        | app_version | String   | 应用版本   |      |
         
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注  |
-        | ----------- | -------- | ----------- | ---- |
-        | sign        | String   | 加密签名     | 根据请求头和密钥加密生成     |
+        | 参数名 | 参数类型 | 参数说明 | 备注                     |
+        | ------ | -------- | -------- | ------------------------ |
+        | sign   | String   | 加密签名 | 根据请求头和密钥加密生成 |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注    |
-        | ----------- | -------- | ----------- | ------ |
-        | success     | Boolean  | 是否成功     |         |
-        | token       | String   | 访问令牌     | 长度16位 |
+        | 参数名  | 参数类型 | 参数说明 | 备注       |
+        | ------- | -------- | -------- | ---------- |
+        | success | Boolean  | 是否成功 |            |
+        | token   | String   | 访问令牌 | 长度 16 位 |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'token': "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1aW"
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：403
         响应体：
         {
             'success': false,
             'msg': "Authorization failed!"
         }
         ```
         
         - 签名生成算法
+        
         ```python
         def get_sign(*args):
             SECRECT_KEY = 'YouMi'
         	content = ''.join(args).encode('ascii')
         	sign_key = SECRECT_KEY.encode('ascii')
         	sign = hmac.new(sign_key, content, hashlib.sha1).hexdigest()
         	return sign
         
         sign = get_sign(user_agent, device_sn, os_platform, app_version)
         
         ```
         
-        
         #### 2.2. 新建用户
+        
         - 请求路径：/api/users/:id
         - 请求方法：post
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | id          | Int      | 用户 ID     |      |
-        | name        | String   | 用户名     |      |
-        | password    | String   | 密码       |      |
+        | 参数名   | 参数类型 | 参数说明 | 备注 |
+        | -------- | -------- | -------- | ---- |
+        | id       | Int      | 用户 ID  |      |
+        | name     | String   | 用户名   |      |
+        | password | String   | 密码     |      |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | msg         | String   | 说明信息     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
+        | msg     | String   | 说明信息 |      |
         
         - 成功返回
+        
         ```
         状态码：201
         响应体：
         {
             'success': true,
             'msg': "user created successfully."
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：422
         响应体：
         {
             'success': false,
             'msg': "user already existed."
         }
         ```
         
-        
         #### 2.3. 根据 ID 查询用户信息
+        
         - 请求路径：/api/users/:id
         - 请求方法：get
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | name        | String   | 用户名     |      |
-        | password    | String   | 密码     |      |
+        | 参数名   | 参数类型 | 参数说明 | 备注 |
+        | -------- | -------- | -------- | ---- |
+        | success  | Boolean  | 是否成功 |      |
+        | name     | String   | 用户名   |      |
+        | password | String   | 密码     |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'data': {
                 'name': 'admin',
                 'password': '123456'
             }
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：404
         响应体：
         {
             'success': fasle,
             'data': {}
         }
         ```
         
         #### 2.4. 更新用户信息
+        
         - 请求路径：/api/users/:id
         - 请求方法：put
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ---------- | ---- |
-        | id          | Int      | 用户 ID     |      |
-        | name        | String   | 用户名      |      |
-        | password    | String   | 密码        |      |
+        | 参数名   | 参数类型 | 参数说明 | 备注 |
+        | -------- | -------- | -------- | ---- |
+        | id       | Int      | 用户 ID  |      |
+        | name     | String   | 用户名   |      |
+        | password | String   | 密码     |      |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | data        | Dict     | 用户信息     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
+        | data    | Dict     | 用户信息 |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'data': {
                 'name': 'admin',
                 'password': '123456'
             }
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：404
         响应体：
         {
             'success': fasle,
             'data': {}
         }
         ```
         
-        
         #### 2.5. 删除用户信息
+        
         - 请求路径：/api/users/:id
         - 请求方法：delete
         - 请求参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ---------- | ---- |
-        | id          | Int      | 用户 ID     |      |
-        
+        | 参数名 | 参数类型 | 参数说明 | 备注 |
+        | ------ | -------- | -------- | ---- |
+        | id     | Int      | 用户 ID  |      |
         
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | data        | Dict     | 用户信息     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
+        | data    | Dict     | 用户信息 |      |
         
         - 成功返回
+        
         ```
-        状态码：204
+        状态码：200
         响应体：
         {
             'success': true,
             'data': {
                 'name': 'admin',
                 'password': '123456'
             }
         }
         ```
         
         - 失败返回
+        
         ```
         状态码：404
         响应体：
         {
             'success': fasle,
             'data': {}
         }
         ```
         
         #### 2.6. 用户数据列表
+        
         - 请求路径：/api/users
         - 请求方法：get
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
-        | count       | Int      | 用户总数     |      |
-        | items       | Array    | 用户数据集合  |      |
+        | 参数名  | 参数类型 | 参数说明     | 备注 |
+        | ------- | -------- | ------------ | ---- |
+        | success | Boolean  | 是否成功     |      |
+        | count   | Int      | 用户总数     |      |
+        | items   | Array    | 用户数据集合 |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true,
             'count': 3,
             'items': [
                 {'name': 'admin1', 'password': '123456'},
                 {'name': 'admin2', 'password': '123456'},
                 {'name': 'admin3', 'password': '123456'}
-            ]    
+            ]
         }
         ```
         
-        
         #### 2.7. 清空用户数据
+        
         - 请求路径：/api/reset-all
         - 请求方法：get
         - 响应参数
         
-        | 参数名       | 参数类型  | 参数说明     | 备注 |
-        | ----------- | -------- | ----------- | ---- |
-        | success     | Boolean  | 是否成功     |      |
+        | 参数名  | 参数类型 | 参数说明 | 备注 |
+        | ------- | -------- | -------- | ---- |
+        | success | Boolean  | 是否成功 |      |
         
         - 成功返回
+        
         ```
         状态码：200
         响应体：
         {
             'success': true
         }
         ```
         
+        ## 三、自动化发布：一键打 Tag 并上传至 PYPI
         
-        ## 三、自动化发布：一键打 Tag 并上传至 PYPI 
-        
-        每次在 __ about __.py 更新版本号后，运行以下命令，实现自动化更新打包上传至 [PYPI](https://pypi.org/) ，同时根据其版本号自动打 Tag 并推送到仓库：
+        每次在 ** about **.py 更新版本号后，运行以下命令，实现自动化更新打包上传至 [PYPI](https://pypi.org/) ，同时根据其版本号自动打 Tag 并推送到仓库：
         
         ```
         python3 setup.py pypi
         ```
-        注意：上传前需提前在twine工具中配置自己的Pypi的账号信息！！！
         
+        注意：上传前需提前在 twine 工具中配置自己的 Pypi 的账号信息！！！
         
         ### 四、CHANGELOG
         
         ```
         v1.0.0
         1、实现对用户账号进行增删改查功能的 API 服务，包含了接口的签名校验机制；
         2、完善了 API 使用文档；
         3、添加了自动化打包脚本；
         ```
         
         ## 五、致谢
-        **A-Api-Server** 工具的产生和打包，主要参考了开源项目 [HttpRunner](https://github.com/httprunner/httprunner)，受益多多，感谢！
         
+        **A-Api-Server** 工具的产生和打包，主要参考了开源项目 [HttpRunner](https://github.com/httprunner/httprunner)，受益多多，感谢！
         
         ## LICENSE
+        
         ```
         MIT License
         
         Copyright (c) 2019 Devin https://zhangchuzhao.site
         Copyright (c) 2017 Toby Qin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -388,14 +411,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         ```
+        
 Keywords: ApiServer,Api,MockServer,Api Test,接口测试,接口自动化测试
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `A_Api_Server-1.1.4/a_api_server/api_server.py` & `A_Api_Server-1.1.5/a_api_server/api_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
 @app.route('/api/users/<int:uid>', methods=['DELETE'])
 @validate_request
 def delete_user(uid):
     user = users_dict.pop(uid, {})
     if user:
         success = True
-        status_code = 204
+        status_code = 200
     else:
         success = False
         status_code = 404
 
     result = {
         'success': success,
         'data': user
@@ -241,8 +241,8 @@
         custom_port = int(sys.argv[1])
     else:
         custom_port = FLASK_APP_PORT
     app.run(host=FLASK_APP_HOST, debug=DEBUG, port=custom_port)
 
 
 if __name__ == "__main__":
-    cli_main()
+    cli_main()
```

