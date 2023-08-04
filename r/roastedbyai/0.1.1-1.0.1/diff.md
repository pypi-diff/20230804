# Comparing `tmp/roastedbyai-0.1.1.tar.gz` & `tmp/roastedbyai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roastedbyai-0.1.1.tar", last modified: Thu May 11 11:23:22 2023, max compression
+gzip compressed data, was "roastedbyai-1.0.1.tar", last modified: Fri Aug  4 11:20:41 2023, max compression
```

## Comparing `roastedbyai-0.1.1.tar` & `roastedbyai-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:23:22.394282 roastedbyai-0.1.1/
--rw-rw-rw-   0        0        0     1097 2023-05-11 10:58:37.000000 roastedbyai-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2554 2023-05-11 11:23:22.393281 roastedbyai-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      946 2023-05-11 11:11:09.000000 roastedbyai-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 11:23:22.388143 roastedbyai-0.1.1/roastedbyai/
--rw-rw-rw-   0        0        0     1207 2023-05-11 11:11:18.000000 roastedbyai-0.1.1/roastedbyai/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-05-11 11:09:12.000000 roastedbyai-0.1.1/roastedbyai/errors.py
--rw-rw-rw-   0        0        0     6574 2023-05-11 11:22:55.000000 roastedbyai-0.1.1/roastedbyai/roasted.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:23:22.392281 roastedbyai-0.1.1/roastedbyai.egg-info/
--rw-rw-rw-   0        0        0     2554 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 11:23:22.394282 roastedbyai-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3097 2023-05-11 11:10:25.000000 roastedbyai-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:20:41.472826 roastedbyai-1.0.1/
+-rw-rw-rw-   0        0        0     1097 2023-05-11 10:58:37.000000 roastedbyai-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2875 2023-08-04 11:20:41.472826 roastedbyai-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2023-08-04 11:16:48.000000 roastedbyai-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 11:20:41.467673 roastedbyai-1.0.1/roastedbyai/
+-rw-rw-rw-   0        0        0     1207 2023-08-04 10:52:04.000000 roastedbyai-1.0.1/roastedbyai/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-08-04 10:55:40.000000 roastedbyai-1.0.1/roastedbyai/errors.py
+-rw-rw-rw-   0        0        0     6207 2023-08-04 11:17:24.000000 roastedbyai-1.0.1/roastedbyai/roasted.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:20:41.471817 roastedbyai-1.0.1/roastedbyai.egg-info/
+-rw-rw-rw-   0        0        0     2875 2023-08-04 11:20:41.000000 roastedbyai-1.0.1/roastedbyai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-08-04 11:20:41.000000 roastedbyai-1.0.1/roastedbyai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:20:41.000000 roastedbyai-1.0.1/roastedbyai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-04 11:20:41.000000 roastedbyai-1.0.1/roastedbyai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 11:20:41.000000 roastedbyai-1.0.1/roastedbyai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:20:41.472826 roastedbyai-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3088 2023-08-04 11:20:31.000000 roastedbyai-1.0.1/setup.py
```

### Comparing `roastedbyai-0.1.1/LICENSE` & `roastedbyai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roastedbyai-0.1.1/PKG-INFO` & `roastedbyai-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: roastedbyai
-Version: 0.1.1
-Summary: A package to get roasted by AI (using Selenium).
+Version: 1.0.1
+Summary: A package to roast and get roasted by AI.
 Home-page: https://github.com/jvherck/roastedbyai
 Author: jvherck
 Author-email: contact@janvh.be
 Maintainer: jvherck
 Maintainer-email: contact@janvh.be
 License: MIT License
 Project-URL: Documentation, https://github.com/jvherck/roastedbyai
 Project-URL: Source, https://github.com/jvherck/roastedbyai
 Project-URL: Tracker, https://github.com/jvherck/roastedbyai/issues
-Keywords: python,ai,roasting,roasted,roast,roastedbyai,selenium
+Keywords: python,ai,roasting,roasted,roast,roastedbyai
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -32,52 +32,71 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RoastedByAI
-This is an *unofficial* Python package that uses Selenium to communicate with 
-https://roastedby.ai as the website doesn't have an official API.
+This is an *unofficial* Python package for https://roastedby.ai to roast and get roasted by AI.
 
 
 ---
 
 
 ## How to install
-Run `pip install roastbyai` \
-If that doesn't work, try `py -m pip install roastedbyai`
+Install the package using one of these pip commands (they both 
+install the same package, the first command just does not always 
+work properly on all devices, the second one should always work)
+
+```shell
+pip install roastedbyai
+```
+Windows:
+```shell
+python -m pip install roastedbyai
+```
+Linux:
+```shell
+python3 -m pip install roastedbyai
+```
 
 
 ---
 
 
 ## Usage
-Important note: the package uses Selenium, which means a browser will be 
-opened!
+
 ```python
 from roastedbyai import Conversation
-from time import sleep
 
 convo = Conversation()
 
 user_input = input("Start by roasting the AI:\n>>> ")
-
 response1 = convo.send(user_input)
-while response1 is None:
-    sleep(1)
-
 print(response1)
-sleep(5)
-
-user_input = input("Roast the AI again:\n>>> ")
 
+user_input = input("\nRoast the AI again:\n>>> ")
 response2 = convo.send(user_input)
-while response2 is None:
-    sleep(1)
-
 print(response2)
 
-convo.quit()
-# This step isn't necessary, the moment you don't use the `convo` object 
+convo.kill()
+# This step isn't necessary, the moment you don't use the `convo` object
 # anymore, python will automatically handle it
+
+print("\n---\n")
+for msg in convo.history:
+    print(msg["role"], msg["content"], sep=": ")
 ```
+
+
+---
+
+
+## Contributing
+Feel free to open Pull Requests with new features, improvements or fixes.
+
+
+---
+
+
+## Disclaimer/Credits
+I am not affiliated with https://roastedby.ai, all credits for the AI go to them.
```

### Comparing `roastedbyai-0.1.1/roastedbyai/__init__.py` & `roastedbyai-1.0.1/roastedbyai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .roasted import *
 from .errors import *
 
-__version__ = "0.1.1"
+__version__ = "1.0.1"
```

### Comparing `roastedbyai-0.1.1/roastedbyai/errors.py` & `roastedbyai-1.0.1/roastedbyai/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,10 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 class MessageLimitExceeded(Exception):
     def __init__(self, _):
         super().__init__(_)
 
-
 class CharacterLimitExceeded(Exception):
     def __init__(self, _):
         super().__init__(_)
```

### Comparing `roastedbyai-0.1.1/roastedbyai/roasted.py` & `roastedbyai-1.0.1/roastedbyai/roasted.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,152 +16,160 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from selenium import webdriver
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.common.exceptions import NoSuchElementException, StaleElementReferenceException
-import html
+import requests
+from typing import List
 
 from .errors import MessageLimitExceeded, CharacterLimitExceeded
 
 
 __all__ = ("Conversation",)
 
 
 # Create a new object of this class for every simultaneous conversation you want to have
 class Conversation:
     """
-    An object of this class represents a conversation with the AI.
-    Make a new object if this conversation reached its message limit.
+    An instance of this class represents a conversation with the AI.
+    Create a new instance of this class if this conversation reached its message limit.
     """
     def __init__(self):
         """
-        Creates an object of this class that represents a conversation with the AI.
-        Make a new object if this conversation reached its message limit.
+        Creates an instance of this class that represents a conversation with the AI.
+        Create a new instance if this conversation reached its message limit.
         """
-        # Initialising variables, do NOT change these!
-        # Private variables start with _
-        self._aimessages: list = []
-        self._usermessages: list = []
-        self._alive: bool = True
-        self._selnumber: int = 1
-        self._selector: str = '/html/body/div/div/div[2]/div[2]/div[2]/div/div[{}]/div'
-        self._cooldown: int = 10
-
-        # Opening browser and waiting until initial message is shown
-        self._driver = webdriver.Chrome()
-        self._driver.get('https://roastedby.ai')
-        WebDriverWait(self._driver, self._cooldown).until(
-            EC.presence_of_element_located(
-                (By.XPATH, self._selector.format(self._selnumber))
-            )
-        )
-
-        # Locating input box
-        WebDriverWait(self._driver, self._cooldown).until(
-            EC.presence_of_element_located(
-                (By.CLASS_NAME, 'inputBox')
-            )
-        )
-        self._input_box = self._driver.find_element(by=By.CLASS_NAME, value='inputBox')
+        self.__history: list = [{
+            "role": "assistant",
+            "content": "Hello there. I'm here to roast you."
+        }]
+        self.__alive: bool = True
+        self.__url: str = "https://roastedby.ai/api/generate"
 
+    def __str__(self):
+        """
+        :returns: the content of the last message in `Conversation.history`
+        """
+        return self.__history[len(self.__history)-1]["content"]
+
+    def __len__(self):
+        """
+        :returns: the amount of messages in `Conversation.history`
+        """
+        return len(self.__history)
 
     @property
-    def aimessages(self):
-        return self._aimessages
+    def aimessages(self) -> list:
+        """
+        Get the list of the AI's messages.
+
+        :returns: list: the list of messages
+        """
+        aimsgs = []
+        for msg in self.__history:
+            if msg["role"] == "assistant":
+                aimsgs.append(msg["content"])
+        return aimsgs
 
     @property
-    def usermessages(self):
-        return self._usermessages
+    def usermessages(self) -> list:
+        """
+        Get the list of the user's messages.
+
+        :returns: list: the list of messages
+        """
+        aimsgs = []
+        for msg in self.__history:
+            if msg["role"] == "user":
+                aimsgs.append(msg["content"])
+        return aimsgs
 
     @property
-    def alive(self):
-        return self._alive
+    def history(self) -> List[dict]:
+        """
+        Return the full history of this Conversation.
 
+        [
+        {"role": "assistant","content": "..."},
+        {"role": "user","content": "..."},
+        ...
+        ]
 
-    def _scrollToBottom(self):
-        self._driver.execute_script(
-            """
-            var elem = document.getElementsByClassName("chatMessages")[0];
-            elem.scrollTo(0, elem.scrollHeight);
-            """
-        )
+        :returns: list[dict]: the history list which contains dicts
+        """
+        return self.__history
 
+    @property
+    def alive(self) -> bool:
+        """
+        Whether you are still able to participate in this Conversation.
+        If this returns False, you can no longer use the `Conversation.send` function, but you can still access the message history.
+
+        :returns: bool: True if you can still send messages, else False
+        """
+        return self.__alive
 
     def send(self, message: str) -> str:
         """
         Sends the user input to the AI and the AI returns a roast as output.
 
-        :param message: the user input for the AI
+        :param message: str: the user input for the AI
         :type message: str
         :return: returns a string containing the AI's (roast) response to the user's input
         """
-        # Checking if message limit isn't reached yet
-        if self.alive is False:
-            raise MessageLimitExceeded('Message limit is exceeded, create a new object of this class to continue again.')
+        if self.__alive is False:
+            raise MessageLimitExceeded('Message limit exceeded, you can not send any more messages to this Conversation.')
 
-        # Checking for max character length
         if len(message) > 250:
-            raise CharacterLimitExceeded('Character limit is exceeded: maximum allowed number of characters is 250!')
+            raise CharacterLimitExceeded('Character limit exceeded: maximum allowed number of characters is 250!')
 
-        # Removing all unsupported characters
+        # Removing non-allowed characters
         for char in message:
             if ord(char) > 65535:
                 message = message.replace(char, '￿')
 
-        # Insert user input to input box
-        self._input_box.send_keys(message)
-        self._input_box.send_keys(Keys.RETURN)
-
-        # Increase selector number by 2 to get the next AI message
-        # (every odd number is an AI's message, note that the initial value is 1)
-        self._selnumber += 2
-
-        # Wait for the AI to respond (as soon as the 3 loading symbols disappear, the AI's response is shown)
-        ie = (NoSuchElementException, StaleElementReferenceException,)
-        WebDriverWait(self._driver, self._cooldown, ignored_exceptions=ie).until_not(
-            EC.text_to_be_present_in_element_attribute(
-                (By.XPATH, self._selector.format(self._selnumber)),
-                'innerHTML',
-                # Note that the following string is ONE string on two separate lines! (readability)
-                '<span class="circle animate-loader"></span><span class="circle animate-loader animation-delay-200">'
-                '</span><span class="circle animate-loader animation-delay-400"></span>'
-            )
-        )
-
-        # Scroll to bottom of chat window
-        self._scrollToBottom()
-
-        # Get AI's response
-        result = self._driver.find_element(by=By.XPATH, value=self._selector.format(self._selnumber)) \
-            .get_attribute('innerHTML')
-        result = html.unescape(result)
-
-        # Storing messages
-        self._aimessages.append(result)
-        self._usermessages.append(message)
+        _json_body = {
+            "userMessage": {
+                "role": "user",
+                "content": message
+            },
+            "history": self.__history,
+            "style": "default"
+        }
+        _headers = {
+            "Accept": "*/*",
+            "Accept-Encoding": "br",
+            "Accept-Language": "en-GB,en;q=0.9",
+            "Content-Length": str(len(str(_json_body))),
+            "Content-Type": "application/json",
+            "Origin": "https://roastedby.ai",
+            "Referer": "https://roastedby.ai/",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36",
+        }
+
+        result = requests.post(self.__url, json=_json_body, headers=_headers).json()["content"]
+
+        self.__history.append({
+            "role": "user",
+            "content": message
+        })
+        self.__history.append({
+            "role": "assistant",
+            "content": result
+        })
 
-        # Checking if message limit is reached
         if result == 'Too many messages. Thanks for playing!':
-            self._alive = False
-            self.quit()
+            self.kill()
         elif result == 'Can you calm down?! You exceeded the rate limit. Please try again later.':
-            self._alive = False
-            self.quit()
+            self.kill()
 
         return result
 
-
-    def quit(self) -> None:
+    def kill(self) -> None:
         """
         Quit and close the conversation.
-        User and AI messages are still available using `.usermessages` and `.aimessages`
+        User and AI messages are still available using `Conversation.usermessages` and `Conversation.aimessages`.
+        The full conversation is available in `Conversation.history`.
         """
-        self._alive = False
-        self._driver.quit()
+        self.__alive = False
```

### Comparing `roastedbyai-0.1.1/roastedbyai.egg-info/PKG-INFO` & `roastedbyai-1.0.1/roastedbyai.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: roastedbyai
-Version: 0.1.1
-Summary: A package to get roasted by AI (using Selenium).
+Version: 1.0.1
+Summary: A package to roast and get roasted by AI.
 Home-page: https://github.com/jvherck/roastedbyai
 Author: jvherck
 Author-email: contact@janvh.be
 Maintainer: jvherck
 Maintainer-email: contact@janvh.be
 License: MIT License
 Project-URL: Documentation, https://github.com/jvherck/roastedbyai
 Project-URL: Source, https://github.com/jvherck/roastedbyai
 Project-URL: Tracker, https://github.com/jvherck/roastedbyai/issues
-Keywords: python,ai,roasting,roasted,roast,roastedbyai,selenium
+Keywords: python,ai,roasting,roasted,roast,roastedbyai
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -32,52 +32,71 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RoastedByAI
-This is an *unofficial* Python package that uses Selenium to communicate with 
-https://roastedby.ai as the website doesn't have an official API.
+This is an *unofficial* Python package for https://roastedby.ai to roast and get roasted by AI.
 
 
 ---
 
 
 ## How to install
-Run `pip install roastbyai` \
-If that doesn't work, try `py -m pip install roastedbyai`
+Install the package using one of these pip commands (they both 
+install the same package, the first command just does not always 
+work properly on all devices, the second one should always work)
+
+```shell
+pip install roastedbyai
+```
+Windows:
+```shell
+python -m pip install roastedbyai
+```
+Linux:
+```shell
+python3 -m pip install roastedbyai
+```
 
 
 ---
 
 
 ## Usage
-Important note: the package uses Selenium, which means a browser will be 
-opened!
+
 ```python
 from roastedbyai import Conversation
-from time import sleep
 
 convo = Conversation()
 
 user_input = input("Start by roasting the AI:\n>>> ")
-
 response1 = convo.send(user_input)
-while response1 is None:
-    sleep(1)
-
 print(response1)
-sleep(5)
-
-user_input = input("Roast the AI again:\n>>> ")
 
+user_input = input("\nRoast the AI again:\n>>> ")
 response2 = convo.send(user_input)
-while response2 is None:
-    sleep(1)
-
 print(response2)
 
-convo.quit()
-# This step isn't necessary, the moment you don't use the `convo` object 
+convo.kill()
+# This step isn't necessary, the moment you don't use the `convo` object
 # anymore, python will automatically handle it
+
+print("\n---\n")
+for msg in convo.history:
+    print(msg["role"], msg["content"], sep=": ")
 ```
+
+
+---
+
+
+## Contributing
+Feel free to open Pull Requests with new features, improvements or fixes.
+
+
+---
+
+
+## Disclaimer/Credits
+I am not affiliated with https://roastedby.ai, all credits for the AI go to them.
```

### Comparing `roastedbyai-0.1.1/setup.py` & `roastedbyai-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     license="MIT License",
     author="jvherck",
     author_email="contact@janvh.be",
     maintainer="jvherck",
     maintainer_email="contact@janvh.be",
     url="https://github.com/jvherck/roastedbyai",
     project_urls={"Documentation": "https://github.com/jvherck/roastedbyai", "Source": "https://github.com/jvherck/roastedbyai", "Tracker": "https://github.com/jvherck/roastedbyai/issues"},
-    description="A package to get roasted by AI (using Selenium).",
+    description="A package to roast and get roasted by AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=['selenium'],
+    install_requires=['requests', 'brotli'],
     python_requires='>=3.7',
-    keywords=['python', 'ai', 'roasting', 'roasted', 'roast', 'roastedbyai', 'selenium'],
+    keywords=['python', 'ai', 'roasting', 'roasted', 'roast', 'roastedbyai'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Other Audience",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
```

