# Comparing `tmp/dingtalk-stream-0.8.0.tar.gz` & `tmp/dingtalk-stream-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.8.0.tar", last modified: Tue Jul 25 11:43:05 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.8.1.tar", last modified: Fri Aug  4 02:58:28 2023, max compression
```

## Comparing `dingtalk-stream-0.8.0.tar` & `dingtalk-stream-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/card_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    25657 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:28.025870 dingtalk-stream-0.8.1/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25730 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-04 02:58:28.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/setup.py
```

### Comparing `dingtalk-stream-0.8.0/LICENSE` & `dingtalk-stream-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/PKG-INFO` & `dingtalk-stream-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.8.0/README.md` & `dingtalk-stream-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/__init__.py` & `dingtalk-stream-0.8.1/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/card_callback.py` & `dingtalk-stream-0.8.1/dingtalk_stream/card_callback.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.8.1/dingtalk_stream/card_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,20 +150,20 @@
         self.markdown = ""
         self.inputing_status = False
 
     def set_title_and_logo(self, title: str, logo: str):
         self.title = title
         self.logo = logo
 
-    def ai_start(self):
+    def ai_start(self, recipients: list = None):
         """
         开始执行中
         :return:
         """
-        self.card_instance_id = self.start(self.card_template_id, {})
+        self.card_instance_id = self.start(self.card_template_id, {}, recipients=recipients)
         self.inputing_status = False
 
     def ai_streaming(self, markdown: str, append: bool = False):
         """
         打字机模式
         :param append: 两种更新模式，append=true，追加的方式；append=false，全量替换。
         :param markdown:
```

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.8.1/dingtalk_stream/card_replier.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,19 @@
             'User-Agent': ('DingTalkStream/1.0 SDK/0.1.0 Python/%s '
                            '(+https://github.com/open-dingtalk/dingtalk-stream-sdk-python)'
                            ) % platform.python_version(),
         }
 
     def create_and_send_card(self, card_template_id: str, card_data: dict, callback_type: str = "",
                              callback_route_key: str = "", at_sender: bool = False,
-                             at_all: bool = False) -> str:
+                             at_all: bool = False, recipients: list = None) -> str:
         """
         发送卡片，两步骤：创建+投放。
         https://open.dingtalk.com/document/orgapp/interface-for-creating-a-card-instance
+        :param recipients:
         :param card_template_id: 卡片模板ID
         :param card_data: 卡片数据
         :param at_sender:
         :param at_all:
         :return: 卡片的实例ID
         """
         access_token = self.dingtalk_client.get_access_token()
@@ -105,14 +106,17 @@
                     "@ALL": "@ALL",
                 }
             elif at_sender:
                 body["imGroupOpenDeliverModel"]["atUserIds"] = {
                     self.incoming_message.sender_staff_id: self.incoming_message.sender_nick,
                 }
 
+            if recipients is not None:
+                body["imGroupOpenDeliverModel"]["recipients"] = recipients
+
         elif self.incoming_message.conversation_type == '1':
             body["openSpaceId"] = "dtv1.card//{spaceType}.{spaceId}".format(spaceType="IM_ROBOT",
                                                                             spaceId=self.incoming_message.sender_staff_id)
             body["imRobotOpenDeliverModel"] = {
                 "spaceType": "IM_ROBOT"
             }
 
@@ -173,24 +177,26 @@
 
 
 class AICardReplier(CardReplier):
 
     def __init__(self, dingtalk_client, incoming_message):
         super(AICardReplier, self).__init__(dingtalk_client, incoming_message)
 
-    def start(self, card_template_id: str, card_data: dict) -> str:
+    def start(self, card_template_id: str, card_data: dict, recipients: list = None) -> str:
         """
         AI卡片的创建接口
+        :param recipients:
         :param card_template_id:
         :param card_data:
         :return:
         """
         card_data_with_status = copy.deepcopy(card_data)
         card_data_with_status["flowStatus"] = AICardStatus.PROCESSING
-        return self.create_and_send_card(card_template_id, card_data_with_status, at_sender=False, at_all=False)
+        return self.create_and_send_card(card_template_id, card_data_with_status, at_sender=False, at_all=False,
+                                         recipients=recipients)
 
     def finish(self, card_instance_id: str, card_data: dict):
         """
         AI卡片执行完成的接口，整体更新
         :param card_instance_id:
         :param card_data:
         :return:
```

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.8.1/dingtalk_stream/chatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,26 +349,27 @@
         carousel_card_instance.set_title_and_logo(title, logo)
 
         carousel_card_instance.reply(markdown, image_slider, button_text)
 
         return carousel_card_instance
 
     def ai_markdown_card_start(self, incoming_message: ChatbotMessage, title: str = "",
-                               logo: str = "") -> AIMarkdownCardInstance:
+                               logo: str = "", recipients: list = None) -> AIMarkdownCardInstance:
         """
         发起一个AI卡片
+        :param recipients:
         :param incoming_message:
         :param title:
         :param logo:
         :return:
         """
         ai_markdown_card_instance = AIMarkdownCardInstance(self.dingtalk_client, incoming_message)
         ai_markdown_card_instance.set_title_and_logo(title, logo)
 
-        ai_markdown_card_instance.ai_start()
+        ai_markdown_card_instance.ai_start(recipients=recipients)
         return ai_markdown_card_instance
 
     def extract_text_from_incoming_message(self, incoming_message: ChatbotMessage) -> list:
         """
         获取文本列表
         :param incoming_message:
         :return: text list。如果是纯文本消息，结果列表中只有一个元素；如果是富文本消息，结果是长列表，按富文本消息的逻辑分割，大致是按换行符分割的。
```

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/frames.py` & `dingtalk-stream-0.8.1/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/handlers.py` & `dingtalk-stream-0.8.1/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.8.1/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream/stream.py` & `dingtalk-stream-0.8.1/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.8.1/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.8.0/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.8.1/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.0/setup.py` & `dingtalk-stream-0.8.1/setup.py`

 * *Files identical despite different names*

