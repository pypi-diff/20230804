# Comparing `tmp/nonebot_plugin_pjsk-0.2.4.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.4.tar", last modified: Thu Aug  3 13:43:07 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.5.tar", last modified: Fri Aug  4 14:22:46 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.4.tar` & `nonebot_plugin_pjsk-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-08-03 13:42:50.179963 nonebot_plugin_pjsk-0.2.4/LICENSE
--rw-r--r--   0        0        0     4300 2023-08-03 13:42:50.179963 nonebot_plugin_pjsk-0.2.4/README.md
--rw-r--r--   0        0        0      795 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     8728 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0     1216 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0    11191 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     4002 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2351 2023-08-03 13:42:50.255965 nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1787 2023-08-03 13:43:07.929358 nonebot_plugin_pjsk-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 14:22:25.249375 nonebot_plugin_pjsk-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4381 2023-08-04 14:22:25.249375 nonebot_plugin_pjsk-0.2.5/README.md
+-rw-r--r--   0        0        0      795 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     8728 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0     1216 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0    11191 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     3962 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2351 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1787 2023-08-04 14:22:46.189397 nonebot_plugin_pjsk-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5372 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.4/LICENSE` & `nonebot_plugin_pjsk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.4/README.md` & `nonebot_plugin_pjsk-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -147,14 +147,18 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.5
+
+- 使用自己合并的字体文件避免某些字不显示的问题
+
 ### 0.2.4
 
 - 在交互模式中提供的参数会去掉指令前缀，以防 Adapter 删掉参数开头的 Bot 昵称，导致参数不对的情况
 - 重写帮助图片的渲染（个人感觉效果还不是很好……）
 
 ### 0.2.3
```

#### html2text {}

```diff
@@ -26,15 +26,16 @@
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.4
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.5
+- ä½¿ç¨èªå·±åå¹¶çå­ä½æä»¶é¿åæäºå­ä¸æ¾ç¤ºçé®é¢ ### 0.2.4
 - å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
 å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
 éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
 0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
 nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
 æ¹ä¸ºæä¾è§åº¦å¼ï¼æ­£æ°ä¸ºé¡ºæ¶éæè½¬ -
```

### Comparing `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __plugin_meta__ = PluginMetadata(
     name="Sekai Stickers",
     description="基于 NoneBot2 的 Project Sekai 表情包制作插件",
     usage="使用指令 `pjsk -h` 查看帮助",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/__main__.py` & `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 CACHE_FOLDER = DATA_FOLDER / "cache"
 if CACHE_FOLDER.exists():
     shutil.rmtree(CACHE_FOLDER)
 CACHE_FOLDER.mkdir(parents=True)
 
 FONT_PATHS = [
-    FONT_FOLDER / "YurukaStd.ttf",
-    FONT_FOLDER / "ShangShouFangTangTi.ttf",
+    FONT_FOLDER / "YurukaFangTang.ttf",
 ]
 
 for _folder in (DATA_FOLDER, FONT_FOLDER, RESOURCE_FOLDER):
     if not _folder.exists():
         _folder.mkdir(parents=True)
```

### Comparing `nonebot_plugin_pjsk-0.2.4/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.4/pyproject.toml` & `nonebot_plugin_pjsk-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.4"
+version = "0.2.5"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_pjsk-0.2.4/PKG-INFO` & `nonebot_plugin_pjsk-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -172,14 +172,18 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.5
+
+- 使用自己合并的字体文件避免某些字不显示的问题
+
 ### 0.2.4
 
 - 在交互模式中提供的参数会去掉指令前缀，以防 Adapter 删掉参数开头的 Bot 昵称，导致参数不对的情况
 - 重写帮助图片的渲染（个人感觉效果还不是很好……）
 
 ### 0.2.3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.4 Summary: Project
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.5 Summary: Project
 Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
 https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -40,15 +40,16 @@
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.4
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.5
+- ä½¿ç¨èªå·±åå¹¶çå­ä½æä»¶é¿åæäºå­ä¸æ¾ç¤ºçé®é¢ ### 0.2.4
 - å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
 å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
 éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
 0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
 nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
 æ¹ä¸ºæä¾è§åº¦å¼ï¼æ­£æ°ä¸ºé¡ºæ¶éæè½¬ -
```

