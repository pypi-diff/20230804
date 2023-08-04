# Comparing `tmp/liveramp_automation-0.1.7.tar.gz` & `tmp/liveramp_automation-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.1.7.tar", last modified: Wed Aug  2 08:05:15 2023, max compression
+gzip compressed data, was "liveramp_automation-0.2.2.tar", last modified: Fri Aug  4 06:08:12 2023, max compression
```

## Comparing `liveramp_automation-0.1.7.tar` & `liveramp_automation-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.376174 liveramp_automation-0.1.7/
--rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.7/LICENSE
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 08:05:15.375715 liveramp_automation-0.1.7/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.347791 liveramp_automation-0.1.7/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.7/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-02 08:05:03.000000 liveramp_automation-0.1.7/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.359014 liveramp_automation-0.1.7/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3786 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3957 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.368823 liveramp_automation-0.1.7/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.7/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1369 2023-08-02 08:00:32.000000 liveramp_automation-0.1.7/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.7/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      993 2023-08-02 08:00:32.000000 liveramp_automation-0.1.7/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     8161 2023-08-02 08:00:32.000000 liveramp_automation-0.1.7/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (502) staff       (20)      744 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1091 2023-08-02 08:02:29.000000 liveramp_automation-0.1.7/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.353211 liveramp_automation-0.1.7/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 08:05:15.376343 liveramp_automation-0.1.7/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1334 2023-08-02 08:05:03.000000 liveramp_automation-0.1.7/setup.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.370020 liveramp_automation-0.1.7/tests/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.7/tests/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.371550 liveramp_automation-0.1.7/tests/test_helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.7/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.7/tests/test_helpers/test_file.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.374186 liveramp_automation-0.1.7/tests/test_utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.7/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/tests/test_utils/test_request.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.351239 liveramp_automation-0.2.2/
+-rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.2.2/LICENSE
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-04 06:08:12.350253 liveramp_automation-0.2.2/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.2.2/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.317031 liveramp_automation-0.2.2/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)      116 2023-08-03 08:05:33.000000 liveramp_automation-0.2.2/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-04 06:08:07.000000 liveramp_automation-0.2.2/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.328669 liveramp_automation-0.2.2/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.2.2/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.2.2/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     4020 2023-08-02 08:53:12.000000 liveramp_automation-0.2.2/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3921 2023-08-04 06:07:09.000000 liveramp_automation-0.2.2/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.2.2/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.340523 liveramp_automation-0.2.2/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.2.2/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1369 2023-08-02 08:00:32.000000 liveramp_automation-0.2.2/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.2.2/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      993 2023-08-02 08:00:32.000000 liveramp_automation-0.2.2/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1285 2023-08-02 08:22:54.000000 liveramp_automation-0.2.2/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     8485 2023-08-03 08:57:37.000000 liveramp_automation-0.2.2/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1282 2023-08-02 08:22:54.000000 liveramp_automation-0.2.2/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1091 2023-08-02 08:02:29.000000 liveramp_automation-0.2.2/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.322128 liveramp_automation-0.2.2/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-04 06:08:12.000000 liveramp_automation-0.2.2/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-04 06:08:12.000000 liveramp_automation-0.2.2/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-04 06:08:12.000000 liveramp_automation-0.2.2/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-04 06:08:12.000000 liveramp_automation-0.2.2/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-04 06:08:12.000000 liveramp_automation-0.2.2/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-04 06:08:12.351564 liveramp_automation-0.2.2/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1335 2023-08-02 08:44:39.000000 liveramp_automation-0.2.2/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.342171 liveramp_automation-0.2.2/tests/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.2.2/tests/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.344488 liveramp_automation-0.2.2/tests/test_helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.2.2/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.2.2/tests/test_helpers/test_file.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 06:08:12.348508 liveramp_automation-0.2.2/tests/test_utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.2.2/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.2.2/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.2.2/tests/test_utils/test_request.py
```

### Comparing `liveramp_automation-0.1.7/LICENSE` & `liveramp_automation-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/PKG-INFO` & `liveramp_automation-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 0.1.7
+Version: 0.2.2
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.7/README.md` & `liveramp_automation-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/liveramp_automation/helpers/bucket.py` & `liveramp_automation-0.2.2/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/liveramp_automation/helpers/file.py` & `liveramp_automation-0.2.2/liveramp_automation/helpers/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,33 @@
 from liveramp_automation.utils.log import Logger
 
 
 class FileHelper:
 
     @staticmethod
     def read_json_report(path) -> dict:
+        """Read all the content of the json file
+
+        :param path:
+        :return:
+        """
         with open(path, 'r') as file:
-            # Read all the content of the json file
             json_string = file.read()
             data = json.loads(json_string)
         return data
 
     @staticmethod
     def read_init_file(file_path, file_name, file_mode="r") -> dict:
+        """Read all the content of the init file
+
+        :param file_path:
+        :param file_name:
+        :param file_mode:
+        :return: data_dict
+        """
         try:
             full_path = os.path.join(file_path, file_name)
             with open(full_path, mode=file_mode) as file:
                 data_dict = {}
                 current_module = None
                 for line in file:
                     line = line.strip()
@@ -45,22 +56,33 @@
             Logger.error(f"Permission denied to read the file '{file_name}' in the specified path: '{file_path}'.")
             return None
         except Exception as e:
             Logger.error(f"An error occurred while reading the file: {e}")
             return None
 
     @staticmethod
-    def load_env_yaml(path,file_prefix, env):
-        # This method is to read the resources accroding to different envrionments
-        file_name = path+"/"+file_prefix+".{env}.yaml".format(env)
+    def load_env_yaml(path, file_prefix, env):
+        """read the resources accroding to different envrionments
+
+        :param path:
+        :param file_prefix:
+        :param env:
+        :return:
+        """
+        file_name = path + "/" + file_prefix + ".{env}.yaml".format(env)
         with open(file_name) as f:
             return yaml.safe_load(f)
 
     @staticmethod
     def deal_testcase_json(file_path):
+        """ read the report.json file and return the testcase object
+
+        :param file_path:
+        :return:
+        """
         with open(file_path, "r") as file:
             item = json.load(file)
         nodeid = item["nodeid"]
         outcome = item["outcome"]
         groupName = nodeid.split("/")[1]
         testcase = {}
         testcase["groupName"] = groupName
@@ -75,23 +97,26 @@
         testcase["flag"] = flag
         testcase["errorMessage"] = errorMessage
         testcase["duration"] = float(item["call"]["duration"])
         return testcase
 
     @staticmethod
     def read_junit_xml_report(path):
+        """ read the junit.xml and retrun the result_dict
+
+        :param path:
+        :return:
+        """
         import xml.etree.ElementTree as ET
         tree = ET.parse(path)
-        # Get the root element of the XML tree
         root = tree.getroot()
-        # Get the values of the errors, failures, skipped, and tests attributes from the testsuite element
-        testsuite = root.find('testsuite')
-        errors = int(testsuite.get('errors'))
-        failures = int(testsuite.get('failures'))
-        skipped = int(testsuite.get('skipped'))
-        tests = int(testsuite.get('tests'))
-        if errors == 0 and failures == 0 and tests > 0:
-            Logger.info("All test cases run sucessfully")
-        elif errors == 0 and failures != 0 and tests > 0:
-            Logger.info("Some test cases run failed")
-        elif errors != 0:
-            Logger.info("Some scripts have issues and please check")
+        test_cases = int(root.attrib.get('tests', 0))
+        failures = int(root.attrib.get('failures', 0))
+        errors = int(root.attrib.get('errors', 0))
+        skipped = int(root.attrib.get('skipped', 0))
+        result_dict = {
+            "Cases": test_cases,
+            "Failures": failures,
+            "Errors": errors,
+            "Skipped": skipped
+        }
+        return result_dict
```

### Comparing `liveramp_automation-0.1.7/liveramp_automation/helpers/login.py` & `liveramp_automation-0.2.2/liveramp_automation/helpers/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,29 @@
         Please invoke this API with the username and password provided in os.environ[].
         :param page:
         :param config:
         :param username:
         :param password:
         :return:
         """
-        Logger.info("We are going to login to OKTA")
+        Logger.info("Going to login to OKTA...")
         url = config['login_url']
         Logger.info("The login url is {}".format(url))
         page.goto(url)
         fixed_wait()
         url_new = page.url
-        Logger.info("The current url is {}".format(url_new))
+        Logger.info("The current url is {}.".format(url_new))
         if url_new.__contains__(url):
-            Logger.info("We've already logan to OKTA succefully")
+            Logger.info("Login to OKTA succefully.")
         else:
             page.fill('#idp-discovery-username', username)
             page.get_by_role("button", name="Next").click()
             page.get_by_role("textbox", name="Password").fill(password)
             page.get_by_role("button", name="Sign In").click()
-            Logger.info("We could login to OKTA successfully")
+            Logger.info("We could login to OKTA successfully.")
             # wait for the login process to complete
             fixed_wait(20)
 
     #
     @staticmethod
     def liveramp_okta_login_driver(driver, config, username, password):
         """
@@ -46,52 +46,52 @@
          Please utilize this API by providing the username and password from os.environ[].
         :param driver:
         :param config:
         :param username:
         :param password:
         :return:
         """
-        Logger.info("We are going to login to OKTA")
+        Logger.info("Going to login to OKTA...")
         url = config['login_url']
-        Logger.info("The login url is {}".format(url))
+        Logger.info("The login url is {}.".format(url))
         driver.get(url)
         fixed_wait()
         if driver.current_url.__contains__(url):
-            Logger.info("We've already logan to OKTA succefully")
+            Logger.info("Login to OKTA succefully.")
         else:
             username_box = driver.find_element(by=By.ID, value='idp-discovery-username')
             username_box.send_keys(username)
             username_box.send_keys(Keys.ENTER)
             fixed_wait()
             password_box = driver.find_element(by=By.ID, value='okta-signin-password')
             password_box.send_keys(password)
             submit_button = driver.find_element(by=By.ID, value='okta-signin-submit')
             submit_button.click()
-            Logger.info("We could login to OKTA successfully")
-            # wait for the login process to complete
-            fixed_wait(20)
+            Logger.info("We could login to OKTA successfully.")
+            fixed_wait(10)
 
     #
     @staticmethod
     def call_oauth2_get_token(username, password) -> str:
         """
         The purpose of the method `call_oauth2_get_token` is to initiate an OAuth2 login.
         Both the API username and password (sensitive) are mandatory for this process.
         Please ensure that you provide the required username and password from os.environ[] when calling this API.
         :param username:
         :param password:
         :return:
         """
-        params = {
+        data = {
             "grant_type": "password",
             "scope": "openid",
             "client_id": "liveramp-api"
         }
-        Logger.info("The default params are the {}".format(params))
+        Logger.info("The default params are the {}".format(data))
         headers = {"content-type": "application/x-www-form-urlencoded"}
-        params.update(username=username)
-        params.update(password=password)
+        data.update(username=username)
+        data.update(password=password)
         response = requests.post(
-            "https://serviceaccounts.liveramp.com/authn/v1/oauth2/token", params=params, headers=headers)
+            "https://serviceaccounts.liveramp.com/authn/v1/oauth2/token", data=data, headers=headers)
         assert 200 == response.status_code
         access_token = response.json()['access_token']
-        return "Bearer {}".format(access_token)
+        token_type = response.json()['token_type']
+        return "{} {}".format(token_type, access_token)
```

### Comparing `liveramp_automation-0.1.7/liveramp_automation/utils/allure.py` & `liveramp_automation-0.2.2/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/liveramp_automation/utils/log.py` & `liveramp_automation-0.2.2/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/liveramp_automation/utils/parsers.py` & `liveramp_automation-0.2.2/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/liveramp_automation/utils/request.py` & `liveramp_automation-0.2.2/liveramp_automation/utils/request.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_delete(url, headers, data=None, json=None, **kwargs):
-    """
+    """Sends a DELETE request.
 
     :param url:
     :param headers:
     :param data:
     :param json:
     :param kwargs:
     :return:
@@ -124,15 +124,15 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_head(url, headers, data=None, json=None, **kwargs):
-    """
+    """Sends a HEAD request.
 
     :param url:
     :param headers:
     :param data:
     :param json:
     :param kwargs:
     :return:
@@ -154,14 +154,23 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_put(url, headers, data=None, json=None, **kwargs):
+    """Sends a PUT request.
+
+    :param url:
+    :param headers:
+    :param data:
+    :param json:
+    :param kwargs:
+    :return:
+    """
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is PUT")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is PUT", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
@@ -175,14 +184,23 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_patch(url, headers, data=None, json=None, **kwargs):
+    """Sends a PATCH request.
+
+    :param url:
+    :param headers:
+    :param data:
+    :param json:
+    :param kwargs:
+    :return:
+    """
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is PATCH")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is PATCH", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
```

### Comparing `liveramp_automation-0.1.7/liveramp_automation/utils/time.py` & `liveramp_automation-0.2.2/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.2.2/liveramp_automation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.1.7
+Version: 0.2.2
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.7/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-0.2.2/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.7/setup.py` & `liveramp_automation-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from setuptools import setup,find_packages
+from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 import os
+
 version_ns = {}
 with open(os.path.join("liveramp_automation", "__version__.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns['__version__']
 
 setup(
     name='liveramp_automation',
     version=version,
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/liveramp-automation",
-    packages= find_packages(),
+    packages=find_packages(),
     install_requires=[
         'pytest',
         'pytest-bdd',
         'pytest-playwright',
         'allure-pytest-bdd',
         'allure-python-commons',
         'google',
```

