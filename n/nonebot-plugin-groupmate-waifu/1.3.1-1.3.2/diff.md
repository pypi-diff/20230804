# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.3.1.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.3.1.tar", last modified: Sat Jul 29 06:13:02 2023, max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.3.2.tar", last modified: Fri Aug  4 21:23:11 2023, max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.3.1.tar` & `nonebot_plugin_groupmate_waifu-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 06:13:02.759354 nonebot_plugin_groupmate_waifu-1.3.1/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      279 2023-07-29 06:13:02.758854 nonebot_plugin_groupmate_waifu-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 06:13:02.746871 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/
--rw-rw-rw-   0        0        0    21882 2023-07-29 06:10:31.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/__init__.py
--rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/config.py
--rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 06:13:02.757353 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 06:13:02.759855 nonebot_plugin_groupmate_waifu-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-07-29 06:12:58.000000 nonebot_plugin_groupmate_waifu-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 21:23:11.078557 nonebot_plugin_groupmate_waifu-1.3.2/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      279 2023-08-04 21:23:11.078055 nonebot_plugin_groupmate_waifu-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 21:23:11.067554 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/
+-rw-rw-rw-   0        0        0    21218 2023-08-04 21:21:34.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/config.py
+-rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 21:23:11.076554 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 21:23:11.079055 nonebot_plugin_groupmate_waifu-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-08-04 21:23:07.000000 nonebot_plugin_groupmate_waifu-1.3.2/setup.py
```

### Comparing `nonebot_plugin_groupmate_waifu-1.3.1/LICENSE` & `nonebot_plugin_groupmate_waifu-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     GROUP_ADMIN,
     GROUP_OWNER,
     Bot,
     GroupMessageEvent,
     Message,
     MessageSegment,
     )
-
+from nonebot.log import logger
 import nonebot
 import os
 import random
 import asyncio
 import time
 
 from pathlib import Path
@@ -43,119 +43,91 @@
 BE = HE + waifu_config.waifu_be
 NTR = waifu_config.waifu_ntr
 yinpa_HE = waifu_config.yinpa_he
 yinpa_BE = yinpa_HE + waifu_config.yinpa_be
 yinpa_CP = waifu_config.yinpa_cp
 yinpa_CP = yinpa_HE if yinpa_CP == 0 else yinpa_CP
 
+# 判断文件时效
+timestr = time.strftime('%Y-%m-%d',time.localtime(time.time()))
+timeArray = time.strptime(timestr,'%Y-%m-%d')
+Zero_today = time.mktime(timeArray)
+
+def load(file,waifu_reset):
+    if waifu_reset and file.exists() and os.path.getmtime(file) > Zero_today:
+        with open(file,'r') as f:
+            line = f.read()
+            record = eval(line)
+        logger.info(f"{file} 已加载")
+    else:
+        record = {}
+        logger.info(f"{file} 已重置")
+    return record
+
+if waifu_save:
+    def save(file, data):
+        with open(file, "w", encoding="utf8") as f:
+            f.write(str(data))
+else:
+    def save(file, data):
+        pass
+
 waifu_file = Path() / "data" / "waifu"
 
 if not waifu_file.exists():
     os.makedirs(waifu_file)
 
 record_CP_file = waifu_file / "record_CP"
-
-if record_CP_file.exists():
-    with open(record_CP_file,'r') as f:
-        line = f.read()
-        record_CP = eval(line)
-else:
-    record_CP = {}
-
 record_waifu_file = waifu_file / "record_waifu"
-if record_waifu_file.exists():
-    with open(record_waifu_file,'r') as f:
-        line = f.read()
-        record_waifu = eval(line)
-else:
-    record_waifu = {}
-
 record_lock_file = waifu_file / "record_lock"
-if record_lock_file.exists():
-    with open(record_lock_file,'r') as f:
-        line = f.read()
-        record_lock = eval(line)
-else:
-    record_lock = {}
-
 record_yinpa1_file = waifu_file / "record_yinpa1"
-if record_yinpa1_file.exists():
-    with open(record_yinpa1_file,'r') as f:
-        line = f.read()
-        record_yinpa1 = eval(line)
-else:
-    record_yinpa1 = {}
 record_yinpa2_file = waifu_file / "record_yinpa2"
-if record_yinpa2_file.exists():
-    with open(record_yinpa2_file,'r') as f:
-        line = f.read()
-        record_yinpa2 = eval(line)
-else:
-    record_yinpa2 = {}
 
+record_CP = load(record_CP_file,waifu_reset)
+record_waifu = load(record_waifu_file,waifu_reset)
+record_lock = load(record_lock_file,waifu_reset)
+record_yinpa1 = load(record_yinpa1_file,waifu_reset)
+record_yinpa2 = load(record_yinpa2_file,waifu_reset)
 
-if waifu_save:
-    def save(file, data):
-        with open(file, "w", encoding="utf8") as f:
-            f.write(str(data))
-else:
-    def save(file, data):
-        pass
+protect_list_file = waifu_file / "list_protect"
 
+if protect_list_file.exists():
+    with open(protect_list_file,'r') as f:
+        line = f.read()
+        protect_list = eval(line)
+else:
+    protect_list = {}
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 if waifu_reset:
-
-    # 判断文件时效
-    timestr = time.strftime('%Y-%m-%d',time.localtime(time.time()))
-    timeArray = time.strptime(timestr,'%Y-%m-%d')
-    Zero_today = time.mktime(timeArray)
-
-    if record_CP_file.exists() and os.path.getmtime(record_CP_file) < Zero_today:
-        record_CP = {}
-    if record_waifu_file.exists() and os.path.getmtime(record_waifu_file) > Zero_today:
-        record_waifu = {}
-    if record_lock_file.exists() and os.path.getmtime(record_lock_file) > Zero_today:
-        record_lock = {}
-    if record_yinpa1_file.exists() and os.path.getmtime(record_yinpa1_file) > Zero_today:
-        record_yinpa1 = {}
-    if record_yinpa2_file.exists() and os.path.getmtime(record_yinpa2_file) > Zero_today:
-        record_yinpa2 = {}
-
     # 重置记录
     def reset_record():
         global record_CP,record_waifu,record_lock,record_yinpa1,record_yinpa2
         record_CP = {}
         record_waifu = {}
         record_lock = {}
         record_yinpa1 = {}
         record_yinpa2 = {}
+        logger.info(f"娶群友记录已重置")
 else:
     # 重置记录
     def reset_record():
         global record_CP,record_yinpa1,record_yinpa2
         for group_id in record_CP:
             for user_id in record_CP[group_id]:
                 if record_CP[group_id][user_id] == user_id:
                     record_CP[group_id][user_id] = 0
         record_yinpa1 = {}
         record_yinpa2 = {}
+        logger.info(f"娶群友记录已重置")
 
 on_command("重置记录", priority = 80, block = True).append_handler(reset_record)
 scheduler.add_job(reset_record,"cron",hour = 0, misfire_grace_time = 120)
 
-protect_list_file = waifu_file / "list_protect"
-if protect_list_file.exists():
-    with open(protect_list_file,'r') as f:
-        line = f.read()
-        protect_list = eval(line)
-else:
-    protect_list = {}
-
 #设置保护名单
 
 protect = on_command("娶群友保护", priority = 80, block = True)
 
 @protect.handle()
 async def _(bot:Bot, event: GroupMessageEvent, permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER):
     group_id = event.group_id
@@ -255,17 +227,17 @@
             member = None
             waifu_id = user_id
         if member:
             if at and at != user_id:
                 if waifu_id == at:
                     msg = "这是你的CP！" + random.choice(happy_end) + MessageSegment.image(file = await user_img(waifu_id))
                     if user_id in record_waifu.get(group_id,set()):
-                        record_lock.setdefault(group_id,{})
-                        record_lock[group_id][waifu_id] = user_id
-                        record_lock[group_id][user_id] = waifu_id
+                        lock = record_lock.setdefault(group_id,{})
+                        lock[waifu_id] = user_id
+                        lock[user_id] = waifu_id
                         save(record_lock_file,record_lock)
                         msg += "\ncp已锁！"
                 else:
                     msg = "你已经有CP了，不许花心哦~" + MessageSegment.image(file = await user_img(waifu_id)) + f"你的CP：{member['card'] or member['nickname']}"
             else:
                 msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{member['card'] or member['nickname']}』！"
             await bot.send(event,msg,at_sender = True)
@@ -304,37 +276,39 @@
 waifu = on_message(rule = waifu_rule, priority = 90, block = True)
 
 @waifu.handle()
 async def _(bot:Bot, event: GroupMessageEvent, state:T_State):
     group_id = event.group_id
     user_id = event.user_id
     waifu_id,tips = state["waifu"]
+    rec = record_CP.setdefault(group_id,{})
     if waifu_id == user_id:
-        record_CP[group_id][user_id] = user_id
+        rec[user_id] = user_id
         save(record_CP_file,record_CP)
         await waifu.finish(random.choice(no_waifu),at_sender = True)
-    rec = record_CP.setdefault(group_id,{})
     waifu_set = record_waifu.setdefault(group_id,set())
     if waifu_id in rec:
         waifu_cp = rec[waifu_id]
         member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_cp)
         msg = "人家已经名花有主了~" + MessageSegment.image(file = await user_img(waifu_cp)) + "ta的cp：" + (member['card'] or member['nickname'])
         if waifu_id in record_lock.get(group_id,{}).keys():
             await waifu.finish(msg + "\n本对cp已锁！",at_sender = True)
         X = random.randint(1,100)
         if X > NTR:
-            record_CP[group_id][user_id] = user_id
+            rec[user_id] = user_id
+            save(record_CP_file,record_CP)
+            await waifu.finish(msg, at_sender=True)
         else:
             rec.pop(waifu_cp)
             waifu_set.discard(waifu_cp)
             await waifu.send(msg + "\n但是...",at_sender = True)        
             await asyncio.sleep(1)
 
-    record_CP[group_id][user_id] = waifu_id
-    record_CP[group_id][waifu_id] = user_id
+    rec[user_id] = waifu_id
+    rec[waifu_id] = user_id
     waifu_set.add(waifu_id)
     member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_id)
     msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{(member['card'] or member['nickname'])}』！"
     save(record_waifu_file,record_waifu)
     save(record_CP_file,record_CP)
     await waifu.finish(msg, at_sender=True)
```

### Comparing `nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/utils.py` & `nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.3.1/setup.py` & `nonebot_plugin_groupmate_waifu-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_groupmate_waifu',
-version='1.3.1',
+version='1.3.2',
 description='娶群友',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_groupmate_waifu"]),
```

