# Comparing `tmp/nonebot_plugin_bawiki-0.8.3.tar.gz` & `tmp/nonebot_plugin_bawiki-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.8.3.tar", last modified: Thu Aug  3 11:01:01 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.8.4.tar", last modified: Fri Aug  4 12:49:32 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.8.3.tar` & `nonebot_plugin_bawiki-0.8.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1068 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/LICENSE
--rw-r--r--   0        0        0     9687 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/README.md
--rw-r--r--   0        0        0      734 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0      947 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/__init__.py
--rw-r--r--   0        0        0     3758 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/arona.py
--rw-r--r--   0        0        0     2330 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/calender.py
--rw-r--r--   0        0        0     1265 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/clear_cache.py
--rw-r--r--   0        0        0     1228 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/craft.py
--rw-r--r--   0        0        0     1013 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/emoji.py
--rw-r--r--   0        0        0     2600 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/event.py
--rw-r--r--   0        0        0      986 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/furniture.py
--rw-r--r--   0        0        0     6372 2023-08-03 11:00:38.564594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/gacha.py
--rw-r--r--   0        0        0     3555 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/global_future.py
--rw-r--r--   0        0        0     1795 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/level_guide.py
--rw-r--r--   0        0        0     1438 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/manga.py
--rw-r--r--   0        0        0     4376 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/raid.py
--rw-r--r--   0        0        0     3617 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_fav.py
--rw-r--r--   0        0        0     1878 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_rank.py
--rw-r--r--   0        0        0     1635 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
--rw-r--r--   0        0        0     2031 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_wiki_schale.py
--rw-r--r--   0        0        0     3395 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/time_atk.py
--rw-r--r--   0        0        0     4201 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/voice.py
--rw-r--r--   0        0        0     1152 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0        0 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/__init__.py
--rw-r--r--   0        0        0     1541 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/arona.py
--rw-r--r--   0        0        0     5814 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/bawiki.py
--rw-r--r--   0        0        0     7398 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gacha.py
--rw-r--r--   0        0        0    11340 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gamekee.py
--rw-r--r--   0        0        0    18840 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/schaledb.py
--rw-r--r--   0        0        0     1358 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/__init__.py
--rw-r--r--   0        0        0     1784 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/manual.py
--rw-r--r--   0        0        0     2226 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/pic_menu.py
--rw-r--r--   0        0        0     1251 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/__init__.py
--rw-r--r--   0        0        0    21514 2023-08-03 11:00:38.568594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-08-03 11:00:38.572594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-08-03 11:00:38.576594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gradient.png
--rw-r--r--   0        0        0     4668 2023-08-03 11:00:38.576594 nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1481 2023-08-03 11:01:01.006585 nonebot_plugin_bawiki-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    11138 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/LICENSE
+-rw-r--r--   0        0        0    10040 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/README.md
+-rw-r--r--   0        0        0      734 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0      947 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/__init__.py
+-rw-r--r--   0        0        0     3742 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/arona.py
+-rw-r--r--   0        0        0     2870 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/calender.py
+-rw-r--r--   0        0        0     1265 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/clear_cache.py
+-rw-r--r--   0        0        0     1228 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/craft.py
+-rw-r--r--   0        0        0     1017 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/emoji.py
+-rw-r--r--   0        0        0     2600 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/event.py
+-rw-r--r--   0        0        0      986 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/furniture.py
+-rw-r--r--   0        0        0     6372 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/gacha.py
+-rw-r--r--   0        0        0     3555 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/global_future.py
+-rw-r--r--   0        0        0     1795 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/level_guide.py
+-rw-r--r--   0        0        0     3645 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/manga.py
+-rw-r--r--   0        0        0     4376 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/raid.py
+-rw-r--r--   0        0        0     3953 2023-08-04 12:49:10.949550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_fav.py
+-rw-r--r--   0        0        0     1878 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_rank.py
+-rw-r--r--   0        0        0     1644 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
+-rw-r--r--   0        0        0     2031 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_schale.py
+-rw-r--r--   0        0        0     3395 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/time_atk.py
+-rw-r--r--   0        0        0     4210 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/voice.py
+-rw-r--r--   0        0        0     1152 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/__init__.py
+-rw-r--r--   0        0        0     1541 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/arona.py
+-rw-r--r--   0        0        0     5647 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/bawiki.py
+-rw-r--r--   0        0        0     7495 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gacha.py
+-rw-r--r--   0        0        0    15476 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gamekee.py
+-rw-r--r--   0        0        0    19374 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/schaledb.py
+-rw-r--r--   0        0        0     1358 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/__init__.py
+-rw-r--r--   0        0        0     1784 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/manual.py
+-rw-r--r--   0        0        0     2226 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/pic_menu.py
+-rw-r--r--   0        0        0     1251 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/__init__.py
+-rw-r--r--   0        0        0    21514 2023-08-04 12:49:10.953550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-08-04 12:49:10.957550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-08-04 12:49:10.961550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gradient.png
+-rw-r--r--   0        0        0     4658 2023-08-04 12:49:10.961550 nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1481 2023-08-04 12:49:32.221767 nonebot_plugin_bawiki-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    11491 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.4/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.8.3/LICENSE` & `nonebot_plugin_bawiki-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/README.md` & `nonebot_plugin_bawiki-0.8.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -171,14 +171,21 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.4
+
+- 现在会对 GameKee 的日程表分页了
+- `ba羁绊` 指令带图发送失败时会提醒用户
+- 修复 `ba学生wiki` 截图失败的 bug，同时优化截图样式
+- 漫画获取不再依赖 bawiki-data 数据源，现在直接从 GameKee 现爬；加入了搜索漫画功能，并且图片过多会使用合并转发的方式发送
+
 ## 0.8.3
 
 - 修改缓存路径
 
 ### 0.8.2
 
 - 修改了 `ba语音` 指令的特性，兼容了有中配语音的学生，请查看该指令帮助获取详细信息
```

#### html2text {}

```diff
@@ -51,16 +51,21 @@
 126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
-lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ##
-0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
+lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
+0.8.4 - ç°å¨ä¼å¯¹ GameKee çæ¥ç¨è¡¨åé¡µäº - `baç¾ç»`
+æä»¤å¸¦å¾åéå¤±è´¥æ¶ä¼æéç¨æ· - ä¿®å¤ `baå­¦çwiki`
+æªå¾å¤±è´¥ç bugï¼åæ¶ä¼åæªå¾æ ·å¼ - æ¼«ç»è·åä¸åä¾èµ
+bawiki-data æ°æ®æºï¼ç°å¨ç´æ¥ä» GameKee
+ç°ç¬ï¼å å¥äºæç´¢æ¼«ç»åè½ï¼å¹¶ä¸å¾çè¿å¤ä¼ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé
+## 0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
 æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
 - å é¤äº `arona`
 æä»¤æ¨¡ç³æç´¢å±ç¤ºç±»å«çåè½ï¼å ä¸ºæ¨¡ç³æç´¢æ¶ `type`
 åºå®ä¸º `0` äº ### 0.8.1 - ä½¿ç¨ `arona`
 æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ### 0.8.0 -
 æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona Bot
 æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from .command import load_commands  # noqa: E402
 from .config import Cfg as Cfg  # noqa: E402
 from .help import extra, register_help_cmd, usage  # noqa: E402
 
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=usage,
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki",
     type="application",
     config=Cfg,
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/__init__.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/arona.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/arona.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from nonebot import logger, on_command
 from nonebot.adapters.onebot.v11 import Message, MessageEvent, MessageSegment
 from nonebot.internal.matcher import Matcher
 from nonebot.params import ArgPlainText, CommandArg
 from nonebot.typing import T_State
 
-from ..data.arona import IMAGE_TYPE_MAP, ImageModel, get_image, search
+from ..data.arona import ImageModel, get_image, search
 
 if TYPE_CHECKING:
     from . import HelpList
 
 help_list: "HelpList" = [
     {
         "func": "Arona数据源攻略",
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/calender.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/calender.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import asyncio
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List, Union
 
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import ActionFailed, Message
-from nonebot.exception import FinishedException
+from nonebot.adapters.onebot.v11 import (
+    ActionFailed,
+    Bot,
+    GroupMessageEvent,
+    Message,
+    MessageEvent,
+    MessageSegment,
+)
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 from nonebot.params import CommandArg
 
 from ..data.gamekee import game_kee_calender
 from ..data.schaledb import schale_calender
 
@@ -33,37 +39,55 @@
 ]
 
 
 cmd_calender = on_command("ba日程表")
 
 
 @cmd_calender.handle()
-async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
+async def _(
+    bot: Bot,
+    event: MessageEvent,
+    matcher: Matcher,
+    cmd_arg: Message = CommandArg(),
+):
     arg: str = cmd_arg.extract_plain_text()
 
+    if "s" not in (arg := arg.lower()):
+        # gamekee
+        task = game_kee_calender()
+    else:
+        # schale
+        servers = []
+        if any(x in arg for x in ("日", "j")):
+            servers.append(0)
+        if any(x in arg for x in ("国", "g")):
+            servers.append(1)
+        task = asyncio.gather(*(schale_calender(x) for x in servers))
+
     await matcher.send("正在绘制图片，请稍等")
     try:
-        if "s" in (arg := arg.lower()):
-            arg = arg.replace("schale", "").strip()
-            servers = []
-
-            if (not arg) or ("日" in arg) or ("j" in arg):
-                servers.append(0)
-            if (not arg) or ("国" in arg) or ("g" in arg):
-                servers.append(1)
-
-            await asyncio.gather(
-                *[
-                    matcher.send(x)
-                    for x in (
-                        await asyncio.gather(*[schale_calender(x) for x in servers])
-                    )
-                ],
-            )
-            await matcher.finish()
-        else:
-            await matcher.finish(await game_kee_calender())
-    except (FinishedException, ActionFailed):  # type: ignore
-        raise
+        messages: Union[List[MessageSegment], str] = await task
     except Exception:
         logger.exception("绘制日程表图片出错")
         await matcher.finish("绘制日程表图片出错，请检查后台输出")
+
+    if isinstance(messages, str):
+        await matcher.finish(messages)
+
+    try:
+        forward_nodes: List[MessageSegment] = [
+            MessageSegment.node_custom(int(bot.self_id), "BAWiki", Message(x))
+            for x in messages
+        ]
+        if isinstance(event, GroupMessageEvent):
+            await bot.send_group_forward_msg(
+                group_id=event.group_id,
+                messages=forward_nodes,
+            )
+        else:
+            await bot.send_private_forward_msg(
+                user_id=event.user_id,
+                messages=forward_nodes,
+            )
+    except ActionFailed:
+        logger.warning("以合并转发形式发送失败，尝试使用普通方式发送")
+        await matcher.finish(Message(messages))
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/clear_cache.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/clear_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/craft.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/craft.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/emoji.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/emoji.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 cmd_random_emoji = on_command("ba表情")
 
 
 @cmd_random_emoji.handle()
 async def _(matcher: Matcher):
     try:
         emojis = await db_get_emoji()
-        emo = await db_get(random.choice(emojis), True)
+        emo = await db_get(random.choice(emojis), raw=True)
     except Exception:
         logger.exception("获取表情失败")
         await matcher.finish("获取表情失败，请检查后台输出")
     await matcher.finish(MessageSegment.image(emo))
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/event.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/furniture.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/furniture.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/gacha.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/global_future.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/global_future.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/level_guide.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/level_guide.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/manga.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-import asyncio
-import random
-from io import BytesIO
 from typing import TYPE_CHECKING
 
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from nonebot.adapters.onebot.v11 import Message
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
-from pil_utils import BuildImage
+from nonebot.params import CommandArg
 
-from ..data.bawiki import MangaDict, db_get_manga
-from ..util import async_req
+from ..data.bawiki import recover_stu_alia
+from ..data.gamekee import game_kee_get_stu_cid_li, send_wiki_page
 
 if TYPE_CHECKING:
     from . import HelpList
 
 help_list: "HelpList" = [
     {
-        "func": "随机漫画",
+        "func": "学生Wiki",
         "trigger_method": "指令",
-        "trigger_condition": "ba漫画",
-        "brief_des": "随机发送一话官推漫画",
-        "detail_des": "随机发送一话BA官推漫画\n来源：GameKee",
+        "trigger_condition": "ba学生wiki",
+        "brief_des": "查询学生详情（GameKee）",
+        "detail_des": (
+            "访问对应学生GameKee Wiki页面并截图，支持部分学生别名\n"
+            " \n"
+            "指令示例：\n"
+            "- <ft color=(238,120,0)>ba学生wiki 白子</ft>\n"
+            "- <ft color=(238,120,0)>ba学生wiki xcw</ft>"
+        ),
     },
 ]
 
 
-cmd_random_manga = on_command("ba漫画")
+cmd_stu_wiki = on_command("ba学生wiki", aliases={"ba学生Wiki", "ba学生WIKI"})
 
 
-@cmd_random_manga.handle()
-async def _(matcher: Matcher):
-    async def get_pic(url):
-        p = await async_req(url, raw=True)
-        if url.endswith(".webp"):
-            p = BuildImage.open(BytesIO(p)).save_png()
-        return p
+@cmd_stu_wiki.handle()
+async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
+    arg = cmd_arg.extract_plain_text().strip()
+    if not arg:
+        await matcher.finish("请提供学生名称")
 
     try:
-        manga: MangaDict = random.choice(await db_get_manga())
-        pics = await asyncio.gather(*[get_pic(x) for x in manga["pics"]])
+        ret = await game_kee_get_stu_cid_li()
     except Exception:
-        logger.exception("获取漫画失败")
-        await matcher.finish("获取漫画失败，请检查后台输出")
+        logger.exception("获取学生列表出错")
+        await matcher.finish("获取学生列表出错，请检查后台输出")
 
-    await matcher.finish(
-        Message()
-        + f'{manga["title"]}\n-=-=-=-=-=-=-=-\n{manga["detail"]}'
-        + [MessageSegment.image(x) for x in pics],
-    )
+    if not ret:
+        await matcher.finish("没有获取到学生列表数据")
+
+    if not (sid := ret.get(await recover_stu_alia(arg, game_kee=True))):
+        await matcher.finish("未找到该学生")
+
+    await send_wiki_page(sid, matcher)
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/raid.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/raid.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_fav.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_fav.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import asyncio
 from typing import TYPE_CHECKING
 
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from nonebot.adapters.onebot.v11 import ActionFailed, Message, MessageSegment
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 from nonebot.params import CommandArg
 
 from ..config import config
 from ..data.bawiki import db_get_extra_l2d_list, recover_stu_alia, schale_to_gamekee
 from ..data.gamekee import game_kee_get_stu_cid_li, game_kee_grab_l2d
@@ -83,20 +84,29 @@
         logger.exception("获取学生列表出错")
         await matcher.finish("获取学生列表表出错，请检查后台输出")
 
     if stu := ret.get(arg):
         if not (lvl := stu["MemoryLobby"]):
             await matcher.finish("该学生没有L2D")
 
-        im = MessageSegment.text(f'{stu["Name"]} 在羁绊等级 {lvl[0]} 时即可解锁L2D\nL2D预览：')
+        im = MessageSegment.text(f'{stu["Name"]} 在羁绊等级 {lvl[0]} 时即可解锁L2D\n')
+        image_seg = None
         if p := await get_l2d(await schale_to_gamekee(arg)):
-            im += [MessageSegment.image(await async_req(x, raw=True)) for x in p]
+            images = await asyncio.gather(*[async_req(x, raw=True) for x in p])
+            image_seg = "L2D预览：" + Message(MessageSegment.image(x) for x in images)
+
         else:
             im += (
                 "没找到该学生的L2D看板\n"
                 "可能原因：\n"
                 "- GameKee页面爬取不到角色L2D图片\n"
                 "- GameKee和插件没有收录该学生的L2D\n"
             )
-        await matcher.finish(im)
+
+        try:
+            await matcher.finish(im)
+        except ActionFailed:
+            if image_seg:
+                await matcher.finish(im + "抱歉，L2D 图片被 tx 风控了，或许是因为太涩了……")
+            raise
 
     await matcher.finish("未找到学生")
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_rank.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/stu_wiki_schale.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 from typing import TYPE_CHECKING
 
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import Message
+from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 from nonebot.params import CommandArg
 
+from ..config import config
 from ..data.bawiki import recover_stu_alia
-from ..data.gamekee import game_kee_get_stu_cid_li, send_wiki_page
+from ..data.schaledb import schale_get_stu_dict, schale_get_stu_info
 
 if TYPE_CHECKING:
     from . import HelpList
 
 help_list: "HelpList" = [
     {
-        "func": "学生Wiki",
+        "func": "学生图鉴",
         "trigger_method": "指令",
-        "trigger_condition": "ba学生wiki",
-        "brief_des": "查询学生详情（GameKee）",
+        "trigger_condition": "ba学生图鉴",
+        "brief_des": "查询学生详情（SchaleDB）",
         "detail_des": (
-            "访问对应学生GameKee Wiki页面并截图，支持部分学生别名\n"
+            "访问对应学生SchaleDB页面并截图，支持部分学生别名\n"
             " \n"
             "指令示例：\n"
-            "- <ft color=(238,120,0)>ba学生wiki 白子</ft>\n"
-            "- <ft color=(238,120,0)>ba学生wiki xcw</ft>"
+            "- <ft color=(238,120,0)>ba学生图鉴 白子</ft>\n"
+            "- <ft color=(238,120,0)>ba学生图鉴 xcw</ft>"
         ),
     },
 ]
 
 
-cmd_stu_wiki = on_command("ba学生wiki", aliases={"ba学生Wiki", "ba学生WIKI"})
+cmd_stu_schale = on_command("ba学生图鉴")
 
 
-@cmd_stu_wiki.handle()
+@cmd_stu_schale.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
         await matcher.finish("请提供学生名称")
 
     try:
-        ret = await game_kee_get_stu_cid_li()
+        ret = await schale_get_stu_dict()
     except Exception:
         logger.exception("获取学生列表出错")
-        await matcher.finish("获取学生列表出错，请检查后台输出")
+        await matcher.finish("获取学生列表表出错，请检查后台输出")
 
     if not ret:
         await matcher.finish("没有获取到学生列表数据")
 
-    if not (sid := ret.get(await recover_stu_alia(arg, True))):
+    if not (data := ret.get(await recover_stu_alia(arg))):
         await matcher.finish("未找到该学生")
 
-    await send_wiki_page(sid, matcher)
+    stu_name = data["PathName"]
+    await matcher.send(f"请稍等，正在截取SchaleDB页面～\n{config.ba_schale_url}?chara={stu_name}")
+
+    try:
+        img = MessageSegment.image(await schale_get_stu_info(stu_name))
+    except Exception:
+        logger.exception(f"截取schale db页面出错 chara={stu_name}")
+        await matcher.finish("截取页面出错，请检查后台输出")
+
+    await matcher.finish(img)
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/time_atk.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/time_atk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/command/voice.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/command/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         logger.exception("获取学生列表出错")
         await matcher.finish("获取学生列表出错，请检查后台输出")
 
     if not ret:
         await matcher.finish("没有获取到学生列表数据")
 
     try:
-        org_stu_name = await recover_stu_alia(name, True)
+        org_stu_name = await recover_stu_alia(name, game_kee=True)
         stu_name = await schale_to_gamekee(org_stu_name)
     except Exception:
         logger.exception("还原学生别名失败")
         await matcher.finish("还原学生别名失败，请检查后台输出")
 
     if not (stu_info := ret.get(stu_name)):
         await matcher.finish("未找到该学生")
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/arona.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/arona.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/bawiki.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/bawiki.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import asyncio
 import datetime
 from io import BytesIO
-from typing import Any, Dict, List, Literal, Optional, TypedDict, cast, overload
+from typing import Any, Dict, List, Literal, Optional, cast, overload
 
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pil_utils import BuildImage
 
 from ..config import config
 from ..util import async_req, recover_alia
 
 
-class MangaDict(TypedDict):
-    cid: int
-    title: str
-    detail: str
-    pics: List[str]
-
-
 @overload
 async def db_get(suffix: str, raw: Literal[False] = False) -> Any:
     ...
 
 
 @overload
 async def db_get(suffix: str, raw: Literal[True] = True) -> bytes:
@@ -63,18 +56,14 @@
     return await db_get("data/gacha.json")
 
 
 async def db_get_emoji() -> List[str]:
     return await db_get("data/emoji.json")
 
 
-async def db_get_manga() -> List[MangaDict]:
-    return await db_get("data/manga.json")
-
-
 async def schale_to_gamekee(o: str) -> str:
     diff = await db_get_schale_to_gamekee()
     if o in diff:
         o = diff[o]
     return o.replace("(", "（").replace(")", "）")
 
 
@@ -87,15 +76,15 @@
     return ret
 
 
 async def db_wiki_stu(name):
     wiki = (await db_get_wiki_data())["student"]
     if not (url := wiki.get(name)):
         return "没有找到该角色的角评，可能是学生名称错误或者插件还未收录该角色角评"
-    return MessageSegment.image(await db_get(url, True))
+    return MessageSegment.image(await db_get(url, raw=True))
 
 
 async def db_wiki_raid(raid_id, servers=None, is_wiki=False, terrain=None):
     if not servers:
         servers = [0, 1]
     wiki = (await db_get_wiki_data())["raid"]
 
@@ -120,63 +109,63 @@
         img_ = [terrain_raid] if terrain_raid else list(boss["terrains"].values())
         for i in img_:
             for s in servers:
                 img.append(i[s])
 
     return [
         MessageSegment.image(x)
-        for x in await asyncio.gather(*[db_get(x, True) for x in img])
+        for x in await asyncio.gather(*[db_get(x, raw=True) for x in img])
     ]
 
 
 async def db_wiki_event(event_id):
     event_id = str(event_id)
     wiki = (await db_get_wiki_data())["event"]
     if not (ev := wiki.get(event_id)):
         return "没有找到该活动"
     return [
         MessageSegment.image(x)
-        for x in await asyncio.gather(*[db_get(x, True) for x in ev])
+        for x in await asyncio.gather(*[db_get(x, raw=True) for x in ev])
     ]
 
 
 async def db_wiki_time_atk(raid_id):
     if raid_id >= 1000:
         raid_id = int(raid_id / 1000)
     wiki = (await db_get_wiki_data())["time_atk"]
     if raid_id > len(wiki):
         return f"没有找到该综合战术考试（目前共有{len(wiki)}个综合战术考试）"
     raid_id -= 1
 
-    return MessageSegment.image(await db_get(wiki[raid_id], True))  # type: ignore
+    return MessageSegment.image(await db_get(wiki[raid_id], raw=True))  # type: ignore
 
 
 async def db_wiki_craft():
     wiki = (await db_get_wiki_data())["craft"]
     return [
         MessageSegment.image(x)
-        for x in await asyncio.gather(*[db_get(y, True) for y in wiki])
+        for x in await asyncio.gather(*[db_get(y, raw=True) for y in wiki])
     ]
 
 
 async def db_wiki_furniture():
     wiki = (await db_get_wiki_data())["furniture"]
     return [
         MessageSegment.image(x)
-        for x in await asyncio.gather(*[db_get(y, True) for y in wiki])
+        for x in await asyncio.gather(*[db_get(y, raw=True) for y in wiki])
     ]
 
 
 async def db_global_future(
     date: Optional[datetime.datetime] = None,
     num=1,
     all_img=False,
 ):
     data = (await db_get_wiki_data())["global_future"]
-    img = cast(bytes, await db_get(data["img"], True))
+    img = cast(bytes, await db_get(data["img"], raw=True))
 
     if all_img:
         return MessageSegment.image(img)
 
     compare_date = date or datetime.datetime.now()
     index = -1
     for i, v in enumerate(parts := data["parts"]):
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gacha.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gacha.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,46 +96,50 @@
 
         stu_star = 0
         try:
             stu_j = stu_li[stu.id]
             stu_star: int = stu_j["StarGrade"]
             stu_img = await schale_get(
                 f"images/student/collection/{stu_j['CollectionTexture']}.webp",
-                True,
+                raw=True,
             )
             stu_img = BuildImage.open(BytesIO(stu_img))
         except Exception:
             logger.exception(f"学生数据获取失败 {stu.id}")
             stu_img = RES_GACHA_STU_ERR
 
         card_img = BuildImage.new("RGBA", RES_GACHA_CARD_MASK.size, (0, 0, 0, 0))
         card_img.image.paste(
             stu_img.resize(RES_GACHA_CARD_MASK.size, keep_ratio=True).image,
             mask=RES_GACHA_CARD_MASK.image,
         )
 
-        bg = bg.paste(card_img, (26, 13), True)
+        bg = bg.paste(card_img, (26, 13), alpha=True)
 
         star_x_offset = int(26 + (159 - 30 * stu_star) / 2)
         star_y_offset = 198
         for i in range(stu_star):
-            bg = bg.paste(RES_GACHA_STAR, (star_x_offset + i * 30, star_y_offset), True)
+            bg = bg.paste(
+                RES_GACHA_STAR,
+                (star_x_offset + i * 30, star_y_offset),
+                alpha=True,
+            )
 
         font_x_offset = 45
         font_y_offset = 2
 
         if stu.new:
-            bg = bg.paste(RES_GACHA_NEW, (font_x_offset, font_y_offset), True)
+            bg = bg.paste(RES_GACHA_NEW, (font_x_offset, font_y_offset), alpha=True)
             font_x_offset -= 2
             font_y_offset += 29
 
         if stu.pickup:
             font_x_offset -= 4
             font_y_offset -= 4
-            bg = bg.paste(RES_GACHA_PICKUP, (font_x_offset, font_y_offset), True)
+            bg = bg.paste(RES_GACHA_PICKUP, (font_x_offset, font_y_offset), alpha=True)
 
         return bg
 
     return await asyncio.gather(*[gen_single(x) for x in students])
 
 
 async def gen_gacha_img(students: Iterable[GachaStudent], count: int) -> BytesIO:
@@ -147,15 +151,15 @@
 
     x_gap = 10
     y_gap = 80
     y_offset = int((bg.height - (len(stu_cards) * (y_gap + card_h) - y_gap)) / 2)
     for line in stu_cards:
         x_offset = int((bg.width - (len(line) * (x_gap + card_w) - x_gap)) / 2)
         for card in line:
-            bg = bg.paste(card, (x_offset, y_offset), True)
+            bg = bg.paste(card, (x_offset, y_offset), alpha=True)
             x_offset += card_w + x_gap
         y_offset += card_h + y_gap
 
     bg = bg.draw_text(
         (1678, 841, 1888, 885),
         "距上个3★UP",
         max_fontsize=30,
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/gamekee.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/gamekee.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from io import BytesIO
 from typing import Any, Dict, List, NoReturn, Union, cast
 
-from bs4 import BeautifulSoup, ResultSet, Tag
+from bs4 import BeautifulSoup, PageElement, ResultSet, Tag
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot.internal.matcher import Matcher
 from nonebot_plugin_htmlrender import get_new_page
 from PIL.Image import Resampling
 from pil_utils import BuildImage, text2image
 from playwright.async_api import Page
@@ -71,39 +71,56 @@
     return {x: y["content_id"] for x, y in (await game_kee_get_stu_li()).items()}
 
 
 def game_kee_page_url(sid: int) -> str:
     return f"{config.ba_gamekee_url}{sid}.html"
 
 
+GAMEKEE_WIKI_PAGE_JS = """() => {
+  // 给内容加上 padding
+  document.querySelector('div.wiki-detail-body').style.padding = '20px';
+
+  // 隐藏 Header 避免遮挡页面
+  document.querySelector('div.wiki-header').style.display = 'none';
+
+  // 隐藏关注按钮
+  document.querySelector('div.user-box > button').style.display = 'none';
+
+  // 删掉视频播放器
+  for (const it of document.querySelectorAll('div.video-play-wrapper'))
+    it.remove();
+
+  // 展开所有选项卡内容
+  for (const it of document.querySelectorAll('div.slide-item'))
+    it.classList.add('active');
+
+  // 删掉点赞和收藏按钮
+  document.querySelector('div.article-options').remove();
+
+  // 删掉底部边距
+  document.querySelector('div.wiki-detail-body').style.marginBottom = '0';
+};"""
+
+
 async def game_kee_get_page(url: str) -> bytes:
     async with cast(Page, get_new_page()) as page:
         await page.goto(url, timeout=60 * 1000)
 
-        # 删掉header
-        await page.add_script_tag(
-            content='document.getElementsByClassName("wiki-header")'
-            ".forEach((v)=>{v.remove()})",
-        )
+        await page.evaluate(GAMEKEE_WIKI_PAGE_JS)
 
         # 展开折叠的语音
-        folds = await page.query_selector_all('xpath=//div[@class="fold-table-btn"]')
+        folds = await page.query_selector_all("div.fold-table-btn")
         for i in folds:
             with contextlib.suppress(Exception):
                 await i.click()
 
-        # 隐藏 header 和 footer
-        js_str = "(obj) => { obj.style.display = 'none' }"
-        await page.eval_on_selector(".wiki-header", js_str)
-        await page.eval_on_selector(".wiki-footer", js_str)
-
-        element = await page.query_selector('xpath=//div[@class="wiki-detail-body"]')
+        element = await page.query_selector("div.wiki-detail-body")
         if not element:
             raise ValueError
-        return await element.screenshot()
+        return await element.screenshot(type="jpeg")
 
 
 async def send_wiki_page(sid: int, matcher: Matcher) -> NoReturn:
     url = game_kee_page_url(sid)
     await matcher.send(f"请稍等，正在截取Wiki页面……\n{url}")
 
     try:
@@ -111,24 +128,42 @@
     except Exception:
         logger.exception(f"截取wiki页面出错 {url}")
         await matcher.finish("截取页面出错，请检查后台输出")
 
     await matcher.finish(MessageSegment.image(img))
 
 
-async def game_kee_calender() -> Union[MessageSegment, str]:
+async def game_kee_calender() -> Union[List[MessageSegment], str]:
     ret = await game_kee_get_calender()
     if not ret:
         return "没有获取到GameKee日程表数据"
+    return [MessageSegment.image(x) for x in await game_kee_get_calender_page(ret)]
+
 
-    pic = await game_kee_get_calender_page(ret)
-    return MessageSegment.image(pic)
+def split_images(
+    images: List[BuildImage],
+    max_height: int,
+    padding: int,
+) -> List[List[BuildImage]]:
+    ret = []
+    cur = []
+    height = 0
+    for i in images:
+        if height + i.height > max_height:
+            ret.append(cur)
+            cur = []
+            height = 0
+        cur.append(i)
+        height += i.height + padding
+    if cur:
+        ret.append(cur)
+    return ret
 
 
-async def game_kee_get_calender_page(ret, has_pic=True) -> BytesIO:
+async def game_kee_get_calender_page(ret, has_pic=True) -> List[BytesIO]:
     now = datetime.now()
 
     async def draw(it: dict):
         _p = None
         if has_pic and (_p := it.get("picture")):
             try:
                 _p = (
@@ -192,61 +227,87 @@
         )
 
         if not started:
             img.draw_rectangle((1250, 0, 1400, 60), "gray")
             img.draw_text((1250, 0, 1400, 60), "未开始", max_fontsize=50, fill="white")
 
         ii = 50
-        img.paste(title_p, (60, ii), True)
+        img.paste(title_p, (60, ii), alpha=True)
         ii += title_p.height + 25
-        img.paste(time_p, (60, ii), True)
+        img.paste(time_p, (60, ii), alpha=True)
         ii += time_p.height + 25
         if _p:
-            img.paste(_p, (60, ii), True)
+            img.paste(_p, (60, ii), alpha=True)
             ii += _p.height + 25
         if desc_p:
-            img.paste(desc_p, (60, ii), True)
+            img.paste(desc_p, (60, ii), alpha=True)
             ii += desc_p.height + 25
-        img.paste(remain_p, (60, ii), True)
-        # img = img.circle_corner(15)
+        img.paste(remain_p, (60, ii), alpha=True)
+        return img.circle_corner(15)
 
-        return img
-
-    pics: List[BuildImage] = await asyncio.gather(  # type: ignore
-        *[draw(x) for x in ret],
-    )
-
-    bg_w = 1500
-    bg_h = 200 + sum([x.height + 50 for x in pics])
-    bg = (
-        BuildImage.new("RGBA", (bg_w, bg_h))
-        .paste(RES_CALENDER_BANNER.copy().resize((1500, 150)))
-        .draw_text(
-            (50, 0, 1480, 150),
-            "GameKee丨活动日程",
-            max_fontsize=100,
-            weight="bold",
-            fill="#ffffff",
-            halign="left",
-        )
-        .paste(
-            RES_GRADIENT_BG.copy().resize(
-                (1500, bg_h - 150),
-                resample=Resampling.NEAREST,
-            ),
-            (0, 150),
+    def draw_list(li: List[BuildImage], title: str) -> BuildImage:
+        bg_w = 1500
+        bg_h = 200 + sum([x.height + 50 for x in li])
+        bg = (
+            BuildImage.new("RGBA", (bg_w, bg_h))
+            .paste(RES_CALENDER_BANNER.copy().resize((1500, 150)))
+            .draw_text(
+                (50, 0, 1480, 150),
+                title,
+                max_fontsize=100,
+                weight="bold",
+                fill="#ffffff",
+                halign="left",
+            )
+            .paste(
+                RES_GRADIENT_BG.copy().resize(
+                    (1500, bg_h - 150),
+                    resample=Resampling.NEAREST,
+                ),
+                (0, 150),
+            )
         )
+
+        index = 200
+        for p in li:
+            bg.paste(p.circle_corner(10), (50, index), alpha=True)
+            index += p.height + 50
+        return bg
+
+    important_data = []
+    common_data = []
+    for data in ret:
+        (important_data if data["importance"] else common_data).append(data)
+
+    important_pics, common_pics = await asyncio.gather(
+        asyncio.gather(*(draw(x) for x in important_data)),
+        asyncio.gather(*(draw(x) for x in common_data)),
     )
 
-    index = 200
-    for p in pics:
-        bg.paste(p.circle_corner(10), (50, index), True)
-        index += p.height + 50
+    max_height = 6000
+    if not common_pics:
+        pics = important_pics
+    else:
+        chain = itertools.chain(important_pics, common_pics)
+        pics: List[List[BuildImage]] = (
+            [list(chain)]
+            if sum(x.height + 50 for x in chain) <= max_height + 50
+            else [important_pics, *split_images(common_pics, max_height, 50)]
+        )
+
+    title_prefix = "GameKee丨活动日程"
+    if len(pics) == 1:
+        images = [draw_list(pics[0], title_prefix)]
+    else:
+        if len(pics[-1]) < 3:
+            extra = pics.pop()
+            pics[-1].extend(extra)
+        images = [draw_list(x, f"{title_prefix}丨P{i}") for i, x in enumerate(pics, 1)]
 
-    return bg.save_jpg()
+    return [x.save_jpg() for x in images]
 
 
 async def game_kee_grab_l2d(cid) -> List[str]:
     ret = cast(
         dict,
         await game_kee_request(f"v1/content/detail/{cid}"),
     )
@@ -339,16 +400,16 @@
         return []
     return list(
         itertools.chain(
             *(
                 [parse_voice_elem(x) for x in a]
                 for x in bs.select(".mould-table")
                 if (a := x.find_all("audio"))
-            )
-        )
+            ),
+        ),
     )
 
 
 async def get_level_list() -> Dict[str, int]:
     entry = cast(dict, await game_kee_request("v1/wiki/entry"))
     entry_list: List[Dict] = entry["entry_list"]
     guide_entry: List[Dict] = next(x["child"] for x in entry_list if x["id"] == 50284)
@@ -368,9 +429,86 @@
             dict,
             await game_kee_request(f"v1/content/detail/{cid}"),
         )
     )["content"]
     bs = BeautifulSoup(wiki_html, "lxml")
     img_elem = bs.find_all("img")
     img_urls = cast(List[str], [x["src"] for x in img_elem])
-    img_urls = [f"https:{x}" if x.startswith("//") else x for x in img_urls]
-    return img_urls
+    return [f"https:{x}" if x.startswith("//") else x for x in img_urls]
+
+
+@dataclass()
+class MangaMetadata:
+    category: str
+    name: str
+    cid: int
+
+
+@dataclass()
+class MangaContent:
+    title: str
+    content: str
+    images: List[str]
+
+
+async def get_manga_list() -> List[MangaMetadata]:
+    entry = cast(dict, await game_kee_request("v1/wiki/entry"))
+    entry_list: List[Dict] = entry["entry_list"]
+    guide_entry: List[Dict] = next(x["child"] for x in entry_list if x["id"] == 51508)
+
+    manga_list: List[MangaMetadata] = []
+
+    current_category = "ぶるーあーかいぶっ！"
+    for entry in guide_entry:
+        category = entry["name"]
+        if category.startswith("【"):
+            current_category = category[1 : category.find("】")]
+        manga_list.extend(
+            MangaMetadata(
+                category=current_category,
+                name=x["name"],
+                cid=x["content_id"],
+            )
+            for x in entry["child"]
+        )
+
+    return manga_list
+
+
+def tags_to_str(tag: PageElement) -> str:
+    def process(elem: PageElement) -> str:
+        if c := getattr(elem, "contents", None):
+            return "".join([s for x in c if (s := process(x))])
+        if s := elem.text.strip().replace("\u200b", ""):
+            return s
+        if hasattr(elem, "name") and (elem.name == "img" or elem.name == "br"):  # type: ignore
+            return "\n"
+        return ""
+
+    text = process(tag).strip()
+    if not text:
+        return text
+
+    lines = text.splitlines()
+    last_line = lines[-1]
+    if last_line.startswith("第") and last_line.endswith("话 >"):
+        lines.pop()
+    return "\n".join(lines).strip()
+
+
+async def get_manga_content(cid: int) -> MangaContent:
+    article = cast(dict, await game_kee_request(f"v1/content/detail/{cid}"))
+    soup = BeautifulSoup(article["content"], "lxml")
+
+    content = tags_to_str(soup).strip()
+    if "汉化：" in content:
+        content = content.replace("汉化：", "\n汉化：").replace("\n）", "）")
+
+    return MangaContent(
+        title=article["title"],
+        content=content,
+        images=[
+            f"https:{src}"
+            for x in soup.find_all("img")
+            if (not (src := x["src"]).endswith(".gif")) and "gamekee" in src
+        ],
+    )
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/data/schaledb.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/data/schaledb.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             timeout=60 * 1000,
             wait_until="networkidle",
         )
 
         # 进度条拉最大
         await page.add_script_tag(content="utilStuSetAllProgressMax();")
 
-        return await page.screenshot(full_page=True)
+        return await page.screenshot(full_page=True, type="jpeg")
 
 
 async def schale_calender(server):
     return MessageSegment.image(
         await schale_get_calender(
             server,
             *(
@@ -130,15 +130,15 @@
                     t,
                     (255, 255, 255, 0),
                     fontsize=45,
                     max_width=1350,
                     align="center",
                 ),
                 (int((1400 - ti.width) / 2), 150),
-                True,
+                alpha=True,
             )
             stu = [students[x] for x in g["characters"]]
 
             async def process_avatar(s):
                 return (
                     BuildImage.open(
                         BytesIO(
@@ -148,27 +148,27 @@
                             ),
                         ),
                     )
                     .resize((300, 340))
                     .paste(
                         BuildImage.new("RGBA", (300, 65), (255, 255, 255, 120)),
                         (0, 275),
-                        True,
+                        alpha=True,
                     )
                     .convert("RGB")
                     .circle_corner(25)
                     .draw_text((0, 275, 300, 340), s["Name"], max_fontsize=50)
                 )
 
             avatars = await asyncio.gather(*[process_avatar(x) for x in stu])
             ava_len = len(avatars)
             x_index = int((1400 - (300 + 25) * ava_len + 25) / 2)
 
             for p in avatars:
-                pic = pic.paste(p, (x_index, 250), True)
+                pic = pic.paste(p, (x_index, 250), alpha=True)
                 x_index += p.width + 25
 
             return pic
         return None
 
     async def draw_event():
         pic = pic_bg.copy().draw_text(
@@ -186,28 +186,28 @@
                     t,
                     (255, 255, 255, 0),
                     fontsize=45,
                     max_width=1350,
                     align="center",
                 ),
                 (int((1400 - ti.width) / 2), 150),
-                True,
+                alpha=True,
             )
             ev = g["event"]
             ev_name = ""
             if ev >= 10000:
                 ev_name = " (复刻)"
                 ev %= 10000
             ev_name = localization["EventName"][str(ev)] + ev_name
 
             ev_bg, ev_img = await asyncio.gather(
-                schale_get(f"images/campaign/Campaign_Event_{ev}_Normal.png", True),
+                schale_get(f"images/campaign/Campaign_Event_{ev}_Normal.png", raw=True),
                 schale_get(
                     f"images/eventlogo/Event_{ev}_{'Tw' if server else 'Jp'}.png",
-                    True,
+                    raw=True,
                 ),
             )
 
             ev_bg = (
                 BuildImage.open(BytesIO(ev_bg))
                 .convert("RGBA")
                 .resize_height(340)
@@ -224,25 +224,29 @@
                         bg_color=(255, 255, 255, 0),
                     ),
                     alpha=True,
                 )
                 .paste(
                     BuildImage.new("RGBA", (ev_bg.width, 65), (255, 255, 255, 120)),
                     (0, ev_bg.height - 65),
-                    True,
+                    alpha=True,
                 )
                 .convert("RGB")
                 .circle_corner(25)
                 .draw_text(
                     (0, ev_bg.height - 65, ev_bg.width, ev_bg.height),
                     ev_name,
                     max_fontsize=50,
                 )
             )
-            return pic.paste(ev_bg, (int((pic.width - ev_bg.width) / 2), 250), True)
+            return pic.paste(
+                ev_bg,
+                (int((pic.width - ev_bg.width) / 2), 250),
+                alpha=True,
+            )
         return None
 
     async def draw_raid():
         pic = pic_bg.copy()
         if r := find_current_event(region["current_raid"]):
             ri = r[0]
             t = format_time(*(r[1:]))
@@ -251,15 +255,15 @@
                     t,
                     (255, 255, 255, 0),
                     fontsize=45,
                     max_width=1350,
                     align="center",
                 ),
                 (int((1400 - ti.width) / 2), 150),
-                True,
+                alpha=True,
             )
 
             tp = "TimeAttack" if (time_atk := (ri["raid"] >= 1000)) else "Raid"
             raid = {x["Id"]: x for x in raids[tp]}
             c_ri = raid[ri["raid"]]
             pic = pic.draw_text(
                 (25, 25, 1375, 150),
@@ -296,50 +300,54 @@
             atk_color = color_map[
                 c_ri["BulletType" if time_atk else "BulletTypeInsane"]
             ]
             def_color = color_map[c_ri["ArmorType"]]
 
             c_bg, c_fg, icon_def, icon_atk, icon_tr = await asyncio.gather(
                 *[
-                    schale_get(bg_url, True),
-                    schale_get(fg_url, True),
-                    schale_get("images/ui/Type_Defense_s.png", True),
-                    schale_get("images/ui/Type_Attack_s.png", True),
-                    schale_get(f"images/ui/Terrain_{terrain}.png", True),
+                    schale_get(bg_url, raw=True),
+                    schale_get(fg_url, raw=True),
+                    schale_get("images/ui/Type_Defense_s.png", raw=True),
+                    schale_get("images/ui/Type_Attack_s.png", raw=True),
+                    schale_get(f"images/ui/Terrain_{terrain}.png", raw=True),
                 ],
             )
 
             icon_def = (
                 BuildImage.new("RGBA", (64, 64), def_color)
                 .paste(
-                    BuildImage.open(BytesIO(icon_def))
-                    .convert("RGBA")
-                    .resize_height(48),
+                    (
+                        BuildImage.open(BytesIO(icon_def))
+                        .convert("RGBA")
+                        .resize_height(48)
+                    ),
                     (8, 8),
-                    True,
+                    alpha=True,
                 )
                 .circle()
             )
             icon_atk = (
                 BuildImage.new("RGBA", (64, 64), atk_color)
                 .paste(
-                    BuildImage.open(BytesIO(icon_atk))
-                    .convert("RGBA")
-                    .resize_height(48),
+                    (
+                        BuildImage.open(BytesIO(icon_atk))
+                        .convert("RGBA")
+                        .resize_height(48)
+                    ),
                     (8, 8),
-                    True,
+                    alpha=True,
                 )
                 .circle()
             )
             icon_tr = (
                 BuildImage.new("RGBA", (64, 64), "#ffffff")
                 .paste(
                     img_invert_rgba(Image.open(BytesIO(icon_tr)).convert("RGBA")),
                     (-2, -2),
-                    True,
+                    alpha=True,
                 )
                 .circle()
             )
 
             c_bg = (
                 BuildImage.open(BytesIO(c_bg))
                 .convert("RGBA")
@@ -351,37 +359,37 @@
                 .convert("RGBA")
                 .resize_height(c_bg.height)
             )
             c_bg = (
                 c_bg.paste(
                     c_fg,
                     (int((c_bg.width - c_fg.width) / 2), 0),
-                    True,
+                    alpha=True,
                 )
                 .paste(
                     BuildImage.new("RGBA", (c_bg.width, 65), (255, 255, 255, 120)),
                     (0, c_bg.height - 65),
-                    True,
+                    alpha=True,
                 )
-                .paste(icon_atk, (10, 10), True)
-                .paste(icon_def, (10, 79), True)
-                .paste(icon_tr, (10, 147), True)
+                .paste(icon_atk, (10, 10), alpha=True)
+                .paste(icon_def, (10, 79), alpha=True)
+                .paste(icon_tr, (10, 147), alpha=True)
                 .convert("RGB")
                 .circle_corner(25)
                 .draw_text(
                     (0, c_bg.height - 65, c_bg.width, c_bg.height),
                     (
                         localization["TimeAttackStage"][c_ri["DungeonType"]]
                         if time_atk
                         else (c_ri["Name"])
                     ),
                     max_fontsize=50,
                 )
             )
-            return pic.paste(c_bg, (int((pic.width - c_bg.width) / 2), 250), True)
+            return pic.paste(c_bg, (int((pic.width - c_bg.width) / 2), 250), alpha=True)
         return None
 
     async def draw_birth():
         pic = pic_bg.copy().draw_text(
             (25, 25, 1375, 150),
             "学生生日",
             weight="bold",
@@ -419,15 +427,15 @@
         if p_h:
             stu_pics = [
                 BuildImage.open(BytesIO(x)).convert("RGBA").resize_height(180).circle()
                 for x in await asyncio.gather(
                     *[
                         schale_get(
                             f'images/student/icon/{x["CollectionTexture"]}.png',
-                            True,
+                            raw=True,
                         )
                         for x in birth_this_week + birth_next_week
                     ],
                 )
             ]
             y_index = int((415 - p_h) / 2) + 125
             if birth_this_week:
@@ -436,15 +444,19 @@
                 )
                 pic = pic.draw_text(
                     (x_index - 165, y_index, x_index, y_index + 180),
                     "本周",
                     max_fontsize=50,
                 )
                 for s in birth_this_week:
-                    pic.paste(stu_pics.pop(0), (x_index, y_index), True).draw_text(
+                    pic.paste(
+                        stu_pics.pop(0),
+                        (x_index, y_index),
+                        alpha=True,
+                    ).draw_text(
                         (x_index, y_index + 180, x_index + 180, y_index + 220),
                         s["BirthDay"],
                     )
                     x_index += 180 + 10
 
             if birth_next_week:
                 if birth_this_week:
@@ -454,15 +466,19 @@
                 )
                 pic = pic.draw_text(
                     (x_index - 165, y_index, x_index, y_index + 180),
                     "下周",
                     max_fontsize=50,
                 )
                 for s in birth_next_week:
-                    pic.paste(stu_pics.pop(0), (x_index, y_index), True).draw_text(
+                    pic.paste(
+                        stu_pics.pop(0),
+                        (x_index, y_index),
+                        alpha=True,
+                    ).draw_text(
                         (x_index, y_index + 180, x_index + 180, y_index + 220),
                         s["BirthDay"],
                     )
                     x_index += 180 + 10
 
             return pic
         return None
@@ -499,15 +515,15 @@
             ),
             (0, 150),
         )
     )
 
     h_index = 200
     for im in img:
-        bg.paste(im.circle_corner(10), (50, h_index), True)
+        bg.paste(im.circle_corner(10), (50, h_index), alpha=True)
         h_index += im.height + 50
     return bg.convert("RGB").save("png")
 
 
 async def draw_fav_li(lvl):
     try:
         stu_li = [
@@ -542,18 +558,18 @@
 
     async def draw_stu(name_, dev_name_, line_, index_):
         left = index_ * icon_w
         top = line_ * icon_h + 5
 
         ret = await schale_get(
             f"images/student/lobby/Lobbyillust_Icon_{dev_name_}_01.png",
-            True,
+            raw=True,
         )
         icon_img = Image.open(BytesIO(ret)).convert("RGBA")
-        img.paste(icon_img, (left, top), True)
+        img.paste(icon_img, (left, top), alpha=True)
         img.draw_text(
             (left, top + pic_h, left + icon_w, top + icon_h),
             name_,
             max_fontsize=25,
             min_fontsize=1,
         )
```

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/__init__.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/manual.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/manual.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/help/pic_menu.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/help/pic_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/__init__.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/calender_banner.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_new.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_star.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/resource/res/gradient.png` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/resource/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.3/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.8.4/nonebot_plugin_bawiki/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     TypeVar,
     Union,
-    cast,
     overload,
 )
 
 from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import Message
 from nonebot_plugin_apscheduler import scheduler
 from PIL import Image, ImageOps
```

### Comparing `nonebot_plugin_bawiki-0.8.3/pyproject.toml` & `nonebot_plugin_bawiki-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.8.3"
+version = "0.8.4"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.1",
```

### Comparing `nonebot_plugin_bawiki-0.8.3/PKG-INFO` & `nonebot_plugin_bawiki-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.8.3
+Version: 0.8.4
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -206,14 +206,21 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.4
+
+- 现在会对 GameKee 的日程表分页了
+- `ba羁绊` 指令带图发送失败时会提醒用户
+- 修复 `ba学生wiki` 截图失败的 bug，同时优化截图样式
+- 漫画获取不再依赖 bawiki-data 数据源，现在直接从 GameKee 现爬；加入了搜索漫画功能，并且图片过多会使用合并转发的方式发送
+
 ## 0.8.3
 
 - 修改缓存路径
 
 ### 0.8.2
 
 - 修改了 `ba语音` 指令的特性，兼容了有中配语音的学生，请查看该指令帮助获取详细信息
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.3 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.4 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -71,16 +71,21 @@
 126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
-lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ##
-0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
+lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
+0.8.4 - ç°å¨ä¼å¯¹ GameKee çæ¥ç¨è¡¨åé¡µäº - `baç¾ç»`
+æä»¤å¸¦å¾åéå¤±è´¥æ¶ä¼æéç¨æ· - ä¿®å¤ `baå­¦çwiki`
+æªå¾å¤±è´¥ç bugï¼åæ¶ä¼åæªå¾æ ·å¼ - æ¼«ç»è·åä¸åä¾èµ
+bawiki-data æ°æ®æºï¼ç°å¨ç´æ¥ä» GameKee
+ç°ç¬ï¼å å¥äºæç´¢æ¼«ç»åè½ï¼å¹¶ä¸å¾çè¿å¤ä¼ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé
+## 0.8.3 - ä¿®æ¹ç¼å­è·¯å¾ ### 0.8.2 - ä¿®æ¹äº `baè¯­é³`
 æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
 - å é¤äº `arona`
 æä»¤æ¨¡ç³æç´¢å±ç¤ºç±»å«çåè½ï¼å ä¸ºæ¨¡ç³æç´¢æ¶ `type`
 åºå®ä¸º `0` äº ### 0.8.1 - ä½¿ç¨ `arona`
 æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ### 0.8.0 -
 æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona Bot
 æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
```

