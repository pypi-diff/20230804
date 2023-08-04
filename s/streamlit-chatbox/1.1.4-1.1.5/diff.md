# Comparing `tmp/streamlit_chatbox-1.1.4-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6425 bytes, number of entries: 8
+Zip file size: 7202 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Jul-30 13:49 streamlit_chatbox/__init__.py
 -rw-rw-rw-  2.0 fat     4431 b- defN 23-Aug-01 03:38 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-31 01:37 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat     6118 b- defN 23-Aug-03 06:09 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/RECORD
-8 files, 16468 bytes uncompressed, 5233 bytes compressed:  68.2%
+-rw-rw-rw-  2.0 fat     7923 b- defN 23-Aug-03 08:25 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 08:27 streamlit_chatbox-1.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 08:27 streamlit_chatbox-1.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 08:27 streamlit_chatbox-1.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 08:27 streamlit_chatbox-1.1.5.dist-info/RECORD
+8 files, 18273 bytes uncompressed, 6010 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.1.4.dist-info/METADATA
+Filename: streamlit_chatbox-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.1.4.dist-info/WHEEL
+Filename: streamlit_chatbox-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.1.4.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.1.4.dist-info/RECORD
+Filename: streamlit_chatbox-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/messages.py

```diff
@@ -17,17 +17,20 @@
         self._assistant_avatar = assistant_avatar
         if not isinstance(greetings, list):
             greetings = [greetings]
         for i, greeting in enumerate(greetings):
             if isinstance(greeting, str):
                 greetings[i] = Markdown(greeting)
         self._greetings = greetings
+        self.init_session()
+
+    def init_session(self):
         if self._session_key not in st.session_state:
             st.session_state[self._session_key] = {}
-            self.reset_history()
+            self.reset_history("default")
 
     def reset_history(self, name=None):
         name = name or self._chat_name
         st.session_state[self._session_key].update({
             name: [{
                 "role": "assistant",
                 "elements": self._greetings,
@@ -79,18 +82,29 @@
             if filtered is not None:
                 result.insert(0, filtered)
                 if len(result) >= history_len:
                     break
 
         return result
 
-    # def export2md(self, chat_name="default", filter=None):
-    #     lines = []
-    #     for msg in self.history:
-    #         lines.append()
+    def export2md(self, chat_name: str ="default", filter: Callable =None) -> List[str]:
+        lines = [
+            "<style> td, th {border: none!important;}</style>\n"
+            "|  |  |\n",
+            "|--|--|\n",
+        ]
+        for msg in self.history:
+            if msg["role"] == "user":
+                avatar = '''<svg viewBox="0 0 24 24" aria-hidden="true" focusable="false" fill="currentColor" xmlns="http://www.w3.org/2000/svg" color="inherit" class="eyeqlp51 css-fblp2m ex0cdmw0"><path fill="none" d="M0 0h24v24H0V0z"></path><path d="M10.25 13a1.25 1.25 0 11-2.5 0 1.25 1.25 0 012.5 0zM15 11.75a1.25 1.25 0 100 2.5 1.25 1.25 0 000-2.5zm7 .25c0 5.52-4.48 10-10 10S2 17.52 2 12 6.48 2 12 2s10 4.48 10 10zM10.66 4.12C12.06 6.44 14.6 8 17.5 8c.46 0 .91-.05 1.34-.12C17.44 5.56 14.9 4 12 4c-.46 0-.91.05-1.34.12zM4.42 9.47a8.046 8.046 0 003.66-4.44 8.046 8.046 0 00-3.66 4.44zM20 12c0-.78-.12-1.53-.33-2.24-.7.15-1.42.24-2.17.24a10 10 0 01-7.76-3.69A10.016 10.016 0 014 11.86c.01.04 0 .09 0 .14 0 4.41 3.59 8 8 8s8-3.59 8-8z"></path></svg>'''
+            else:
+                avatar = '''<svg viewBox="0 0 24 24" aria-hidden="true" focusable="false" fill="currentColor" xmlns="http://www.w3.org/2000/svg" color="inherit" class="eyeqlp51 css-fblp2m ex0cdmw0"><rect width="24" height="24" fill="none"></rect><path d="M20 9V7c0-1.1-.9-2-2-2h-3c0-1.66-1.34-3-3-3S9 3.34 9 5H6c-1.1 0-2 .9-2 2v2c-1.66 0-3 1.34-3 3s1.34 3 3 3v4c0 1.1.9 2 2 2h12c1.1 0 2-.9 2-2v-4c1.66 0 3-1.34 3-3s-1.34-3-3-3zm-2 10H6V7h12v12zm-9-6c-.83 0-1.5-.67-1.5-1.5S8.17 10 9 10s1.5.67 1.5 1.5S9.83 13 9 13zm7.5-1.5c0 .83-.67 1.5-1.5 1.5s-1.5-.67-1.5-1.5.67-1.5 1.5-1.5 1.5.67 1.5 1.5zM8 15h8v2H8v-2z"></path></svg>'''
+            content = "\n\n".join(e._content for e in msg["elements"])
+            line = f"|{avatar}|{content}|\n"
+            lines.append(line)
+        return lines
 
     def _prepare_elements(
         self,
         elements: Union[OutputElement, str, List[Union[OutputElement, str]]],
     ) -> List[OutputElement]:
         if isinstance(elements, str):
             elements = [Markdown(elements)]
```

## Comparing `streamlit_chatbox-1.1.4.dist-info/METADATA` & `streamlit_chatbox-1.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.1.4
+Version: 1.1.5
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.24.0)
```

## Comparing `streamlit_chatbox-1.1.4.dist-info/RECORD` & `streamlit_chatbox-1.1.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 streamlit_chatbox/__init__.py,sha256=okS4bZ1sk5ma0Nawlw07pLxVR_INKIqCQQFqvzkzR4A,392
 streamlit_chatbox/elements.py,sha256=G5qNHFANT_KgLtZ9BMDZ7rcCFx6gmoeXaomMfF-3iFU,4431
 streamlit_chatbox/flows.py,sha256=RvtStf1em9vGPp_sj8V7xHKbBiI5_p58RAFuvEMq2-c,323
-streamlit_chatbox/messages.py,sha256=S2e74di03Anmf5GtAlzY-G4m6jQbuWxI_ErekCsUwcY,6118
-streamlit_chatbox-1.1.4.dist-info/METADATA,sha256=OJdJzRv5quwbMiFhL8gwa8XrCFnDllC7hWnPzIrOjBw,4417
-streamlit_chatbox-1.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-streamlit_chatbox-1.1.4.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
-streamlit_chatbox-1.1.4.dist-info/RECORD,,
+streamlit_chatbox/messages.py,sha256=yyTevs0XgwsNOZkTJZnXovk4Y3bw8No40CK3arcHFXk,7923
+streamlit_chatbox-1.1.5.dist-info/METADATA,sha256=dnBntNNGarFRY-z1L2deg4GZcdxHgAgLvOsHbSgsh_Y,4417
+streamlit_chatbox-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+streamlit_chatbox-1.1.5.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
+streamlit_chatbox-1.1.5.dist-info/RECORD,,
```

