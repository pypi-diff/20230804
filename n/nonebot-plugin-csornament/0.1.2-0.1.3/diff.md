# Comparing `tmp/nonebot_plugin_csornament-0.1.2.tar.gz` & `tmp/nonebot_plugin_csornament-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_csornament-0.1.2.tar", last modified: Thu Aug  3 16:05:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_csornament-0.1.3.tar", last modified: Fri Aug  4 03:19:18 2023, max compression
```

## Comparing `nonebot_plugin_csornament-0.1.2.tar` & `nonebot_plugin_csornament-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1063 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/LICENSE
--rw-r--r--   0        0        0     2377 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/README.md
--rw-r--r--   0        0        0     6187 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/nonebot_plugin_csornament/__init__.py
--rw-r--r--   0        0        0      114 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/nonebot_plugin_csornament/config.py
--rw-r--r--   0        0        0      453 2023-08-03 16:05:51.408127 nonebot_plugin_csornament-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 nonebot_plugin_csornament-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-04 03:19:09.233047 nonebot_plugin_csornament-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2377 2023-08-04 03:19:09.233047 nonebot_plugin_csornament-0.1.3/README.md
+-rw-r--r--   0        0        0     5993 2023-08-04 03:19:09.233047 nonebot_plugin_csornament-0.1.3/nonebot_plugin_csornament/__init__.py
+-rw-r--r--   0        0        0      453 2023-08-04 03:19:18.469406 nonebot_plugin_csornament-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 nonebot_plugin_csornament-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_csornament-0.1.2/LICENSE` & `nonebot_plugin_csornament-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_csornament-0.1.2/README.md` & `nonebot_plugin_csornament-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_csornament-0.1.2/nonebot_plugin_csornament/__init__.py` & `nonebot_plugin_csornament-0.1.3/nonebot_plugin_csornament/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-from nonebot.plugin import PluginMetadata
-from .config import Config
 __plugin_meta__ = PluginMetadata(
-    name="nonebot-plugin-csornament",
+    name="CSGO饰品查询机器人",
     description="一款模拟查找饰品价格的机器人",
     usage="输入 查询/搜索/查 xxx 按照机器人的提示，将会获取到目前市场上最低的饰品价格",
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
     homepage="https://github.com/Sydrr0/nonebot-plugin-csornament",
     # 发布必填。
 )
-
-
-# 插件初始化
-from nonebot import get_driver
-from .config import Config
-global_config = get_driver().config
-config = Config.parse_obj(global_config)
-
 # nonebot2 的函数导入
+from nonebot import get_driver
 from nonebot.matcher import Matcher
 from nonebot.plugin import on_command
 from nonebot.params import ArgPlainText # 提取消息内的字符串的方法
 from nonebot.adapters import Message
 from nonebot.params import CommandArg 
 from nonebot.typing import T_State   # 继承上一个函数的方法
 from nonebot import get_bot
```

### Comparing `nonebot_plugin_csornament-0.1.2/PKG-INFO` & `nonebot_plugin_csornament-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_csornament
-Version: 0.1.2
+Version: 0.1.3
 Summary: nonebot社区插件，查询CSGO饰品
 Author-Email: Sydrr0 <2562312527@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: lxml>=4.9.3
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: nonebot2>=2.0.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_csornament Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_csornament Version: 0.1.3 Summary:
 nonebotç¤¾åºæä»¶ï¼æ¥è¯¢CSGOé¥°å Author-Email: Sydrr0 <2562312527@qq.com>
 License: MIT Requires-Python: >=3.8 Requires-Dist: lxml>=4.9.3 Requires-Dist:
 bs4>=0.0.1 Requires-Dist: nonebot2>=2.0.1 Requires-Dist: httpx>=0.23.3
 Description-Content-Type: text/markdown
            [https://pic.imgdb.cn/item/64ca75781ddac507ccf21163.webp]
               _ð¼å¥½çåï¼å¥½ççè¯å°±ç¹ä¸ªâ­å§ï¼è¿
 (~å§å§~)å¯ä»¥ç»äºä½èæå¤§çå¨åå¦ð¼_ # nonebot-plugin-csornament
```

