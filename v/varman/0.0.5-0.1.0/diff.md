# Comparing `tmp/varman-0.0.5.tar.gz` & `tmp/varman-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varman-0.0.5.tar", last modified: Thu Aug  3 08:20:34 2023, max compression
+gzip compressed data, was "varman-0.1.0.tar", last modified: Fri Aug  4 02:51:23 2023, max compression
```

## Comparing `varman-0.0.5.tar` & `varman-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 08:20:34.304189 varman-0.0.5/
--rw-rw-rw-   0        0        0     1084 2023-08-03 04:17:23.000000 varman-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2230 2023-08-03 08:20:34.304189 varman-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1790 2023-08-03 08:14:52.000000 varman-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 08:20:34.304189 varman-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-08-03 08:19:18.000000 varman-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:20:34.294196 varman-0.0.5/varman/
--rw-rw-rw-   0        0        0     3661 2023-08-03 08:16:12.000000 varman-0.0.5/varman/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:20:34.302205 varman-0.0.5/varman.egg-info/
--rw-rw-rw-   0        0        0     2230 2023-08-03 08:20:33.000000 varman-0.0.5/varman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-08-03 08:20:34.000000 varman-0.0.5/varman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 08:20:33.000000 varman-0.0.5/varman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 08:20:33.000000 varman-0.0.5/varman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 02:51:23.017953 varman-0.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-08-03 04:17:23.000000 varman-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3018 2023-08-04 02:51:23.016969 varman-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2578 2023-08-04 02:50:05.000000 varman-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 02:51:23.017953 varman-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      630 2023-08-04 02:48:54.000000 varman-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 02:51:22.998817 varman-0.1.0/varman/
+-rw-rw-rw-   0        0        0     4168 2023-08-04 02:43:45.000000 varman-0.1.0/varman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 02:51:23.015964 varman-0.1.0/varman.egg-info/
+-rw-rw-rw-   0        0        0     3018 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/top_level.txt
```

### Comparing `varman-0.0.5/LICENSE` & `varman-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `varman-0.0.5/PKG-INFO` & `varman-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: varman
-Version: 0.0.5
+Version: 0.1.0
 Summary: A dict like variable container, listen for variable changes.
 Home-page: https://github.com/zlolss/VarMan.py.git
 Author: zloss
 Author-email: zlos@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# VarMan.py
+# VarMan
 
 一个辅助监听变量赋值变化的类，基本用法类似dict类型
  
  
 # 应用场景示例
 
 - webapp中开关量的前后台同步，前台需要显示开关状态并且可以控制开关，后台亦然。
 - 需要监听变量改变并回调相应方法的情形
 
 
 # 使用方法
 
+```shell
+pip install varman
+```
+
 ```python
 import varman
 var = varman.VarMan()
 ```
 
 ## 获取改变值的变量名
 
@@ -44,29 +48,27 @@
 print(var.POPMODIFY())
 ```
 
     {'a'}
     set()
     {'a'}
     {'b'}
-    {'b', 'a'}
+    {'a', 'b'}
     
 
 ## 设置回调函数
 
 
 ```python
+# 对应变量“c”的回调函数
 @var.ONMODIFY('c')
 def fun(pre, nxt):
     print(f'pre c:{pre}, next c:{nxt}')  
 ```
 
-    addlistener:<function fun at 0x000001FFEEC396C0>
-    
-
 
 ```python
 var.c = 1
 ```
 
     pre c:None, next c:1
     
@@ -75,39 +77,97 @@
 ```python
 var['c'] = 4
 ```
 
     pre c:1, next c:4
     
 
-## 作为iter类型使用
+
+```python
+# var中任意变量改变时回调
+@var.ONMODIFYANY
+def func(varname, pre, nxt):
+    print(f'var:{varname}; pre: {pre}, next:{nxt}')
+```
+
+
+```python
+var.c = 1
+```
+
+    pre c:4, next c:1
+    var:c; pre: 4, next:1
+    
+
+
+```python
+var.a = 5
+```
+
+    var:a; pre: 2, next:5
+    
+
+
+```python
+var.dd = []
+```
+
+    var:dd; pre: None, next:[]
+    
+
+
+```python
+# 只能监听基本变量，或变量的id改变，无法监听list、dict等类型的内部更改
+var.dd.append(1)
+```
+
+
+```python
+# 移除监听器
+var.REMOVELISTENER('c')
+var.c = 8
+```
+
+    var:c; pre: 1, next:8
+    
+
+
+```python
+# 移除对任意变量的监听器
+var.REMOVEANYLISTENER()
+var.c = 10
+```
+
+## 作为iter类型使用(类似dict)
 
 
 ```python
 for key in var:
     print(f'{key}:{var[key]}')
 ```
 
-    a:2
+    a:5
     b:3
-    c:4
+    c:10
+    dd:[1]
     
 
 
 ```python
 # 带前缀“_”的变量将隐式调用，不会自动监听赋值状态，也不会被迭代
 # 不允许“__”前缀
 var._d = 5
 for key in var:
     print(f'{key}:{var[key]}')
 ```
 
-    a:2
+    a:5
     b:3
-    c:4
+    c:10
+    dd:[1]
     
 
 
 ```python
 print(var._d)
 ```
 
@@ -117,20 +177,20 @@
 
 ```python
 def fun2(**params):
     print(params)
 fun2(**var)
 ```
 
-    {'a': 2, 'b': 3, 'c': 4}
+    {'a': 5, 'b': 3, 'c': 10, 'dd': [1]}
     
 
 
 ```python
-## 实例化的同时添加变量
+# 实例化的同时添加变量
 var2 = varman.VarMan(d = 8, e=10)
 print(var2)
 ```
 
     {'d': 8, 'e': 10}
     
 
@@ -142,10 +202,11 @@
 
 
 
     VarMan({'d': 8, 'e': 10})
 
 
 
-# todo：
+
+# todo?
 
 - 删除变量
```

### Comparing `varman-0.0.5/setup.py` & `varman-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="varman",
-  version="0.0.5",
+  version="0.1.0",
   author="zloss",
   author_email="zlos@foxmail.com",
   description="A dict like variable container, listen for variable changes.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/zlolss/VarMan.py.git",
   packages=setuptools.find_packages(),
```

### Comparing `varman-0.0.5/varman/__init__.py` & `varman-0.1.0/varman/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,25 +22,40 @@
         
         from typing import Callable, List, Dict
         
         self.__vars = defaults
         self.__modify_sequence = []
         self.__modify_sequence_dropped = 0
         self.__consumers_seek = {'default':0}
-        self.__listeners:Dict[str,List] = {}
+        self.__listeners:Dict[str,List[Callable]] = {}
+        self.__anylisteners:List[Callable] = []
     
     
     def ONMODIFY(self, key:str):
         if key not in self.__listeners:
             self.__listeners[key] = []
         def onmodify(func):
             self.__listeners[key].append(func)
             # print(f'addlistener:{func}')
             return func
         return onmodify
+        
+    
+    def REMOVELISTENER(self, key):
+        if key in self.__listeners:
+            del(self.__listeners[key])
+            
+    
+    def REMOVEANYLISTENER(self):
+        self.__anylisteners = []
+    
+    
+    def ONMODIFYANY(self, func):
+        self.__anylisteners.append(func)
+        return func
 
     
     def POPMODIFY(self, tag = 'default'):
         seek = self.__consumers_seek.get(tag, self.__modify_sequence_dropped)
         dropped = self.__modify_sequence_dropped
         modify_sequence = self.__modify_sequence
         right = len(modify_sequence)
@@ -75,14 +90,15 @@
         return self.__vars.keys()
         
     def __str__(self):
         return str(self.__vars)
         
     def __repr__(self):
         return f'{self.__class__.__name__}({self.__str__()})'
+            
 
     # todo: remove 
     
     # -------------- wrap dict end ---------------
     
     def __getattr__(self, key):
         if not self.__isValidVarName(key):
@@ -106,14 +122,17 @@
         self.__vars[key] = value
         self.__modify_sequence.append(key)
         
         callbacks = self.__listeners.get(key, None)
         if callbacks is not None:
             for callback in callbacks:
                 callback(prevalue, value)
+                
+        for callback in self.__anylisteners:
+            callback(key, prevalue, value)
             
     
     def __len__(self):
         return 1
     
     def __isValidVarName(self, name):
         if not isinstance(name, str):
```

### Comparing `varman-0.0.5/varman.egg-info/PKG-INFO` & `varman-0.1.0/varman.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: varman
-Version: 0.0.5
+Version: 0.1.0
 Summary: A dict like variable container, listen for variable changes.
 Home-page: https://github.com/zlolss/VarMan.py.git
 Author: zloss
 Author-email: zlos@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# VarMan.py
+# VarMan
 
 一个辅助监听变量赋值变化的类，基本用法类似dict类型
  
  
 # 应用场景示例
 
 - webapp中开关量的前后台同步，前台需要显示开关状态并且可以控制开关，后台亦然。
 - 需要监听变量改变并回调相应方法的情形
 
 
 # 使用方法
 
+```shell
+pip install varman
+```
+
 ```python
 import varman
 var = varman.VarMan()
 ```
 
 ## 获取改变值的变量名
 
@@ -44,29 +48,27 @@
 print(var.POPMODIFY())
 ```
 
     {'a'}
     set()
     {'a'}
     {'b'}
-    {'b', 'a'}
+    {'a', 'b'}
     
 
 ## 设置回调函数
 
 
 ```python
+# 对应变量“c”的回调函数
 @var.ONMODIFY('c')
 def fun(pre, nxt):
     print(f'pre c:{pre}, next c:{nxt}')  
 ```
 
-    addlistener:<function fun at 0x000001FFEEC396C0>
-    
-
 
 ```python
 var.c = 1
 ```
 
     pre c:None, next c:1
     
@@ -75,39 +77,97 @@
 ```python
 var['c'] = 4
 ```
 
     pre c:1, next c:4
     
 
-## 作为iter类型使用
+
+```python
+# var中任意变量改变时回调
+@var.ONMODIFYANY
+def func(varname, pre, nxt):
+    print(f'var:{varname}; pre: {pre}, next:{nxt}')
+```
+
+
+```python
+var.c = 1
+```
+
+    pre c:4, next c:1
+    var:c; pre: 4, next:1
+    
+
+
+```python
+var.a = 5
+```
+
+    var:a; pre: 2, next:5
+    
+
+
+```python
+var.dd = []
+```
+
+    var:dd; pre: None, next:[]
+    
+
+
+```python
+# 只能监听基本变量，或变量的id改变，无法监听list、dict等类型的内部更改
+var.dd.append(1)
+```
+
+
+```python
+# 移除监听器
+var.REMOVELISTENER('c')
+var.c = 8
+```
+
+    var:c; pre: 1, next:8
+    
+
+
+```python
+# 移除对任意变量的监听器
+var.REMOVEANYLISTENER()
+var.c = 10
+```
+
+## 作为iter类型使用(类似dict)
 
 
 ```python
 for key in var:
     print(f'{key}:{var[key]}')
 ```
 
-    a:2
+    a:5
     b:3
-    c:4
+    c:10
+    dd:[1]
     
 
 
 ```python
 # 带前缀“_”的变量将隐式调用，不会自动监听赋值状态，也不会被迭代
 # 不允许“__”前缀
 var._d = 5
 for key in var:
     print(f'{key}:{var[key]}')
 ```
 
-    a:2
+    a:5
     b:3
-    c:4
+    c:10
+    dd:[1]
     
 
 
 ```python
 print(var._d)
 ```
 
@@ -117,20 +177,20 @@
 
 ```python
 def fun2(**params):
     print(params)
 fun2(**var)
 ```
 
-    {'a': 2, 'b': 3, 'c': 4}
+    {'a': 5, 'b': 3, 'c': 10, 'dd': [1]}
     
 
 
 ```python
-## 实例化的同时添加变量
+# 实例化的同时添加变量
 var2 = varman.VarMan(d = 8, e=10)
 print(var2)
 ```
 
     {'d': 8, 'e': 10}
     
 
@@ -142,10 +202,11 @@
 
 
 
     VarMan({'d': 8, 'e': 10})
 
 
 
-# todo：
+
+# todo?
 
 - 删除变量
```

