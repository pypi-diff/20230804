# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.34.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.34.tar", last modified: Thu Aug  3 16:19:36 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.35.tar", last modified: Thu Aug  3 16:24:49 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.34.tar` & `basebot22-basebot_JustinGuese-0.3.35.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/backtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 16:19:25.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:19:36.000000 basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 16:19:28.000000 basebot22-basebot_JustinGuese-0.3.34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:19:36.128918 basebot22-basebot_JustinGuese-0.3.34/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:24:49.369619 basebot22-basebot_JustinGuese-0.3.35/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:24:49.369619 basebot22-basebot_JustinGuese-0.3.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 16:24:37.000000 basebot22-basebot_JustinGuese-0.3.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:24:49.369619 basebot22-basebot_JustinGuese-0.3.35/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:24:37.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:24:37.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-08-03 16:24:37.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-08-03 16:24:37.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:24:49.369619 basebot22-basebot_JustinGuese-0.3.35/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 16:24:49.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 16:24:49.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:24:49.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 16:24:49.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:24:49.000000 basebot22-basebot_JustinGuese-0.3.35/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 16:24:42.000000 basebot22-basebot_JustinGuese-0.3.35/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:24:49.369619 basebot22-basebot_JustinGuese-0.3.35/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.34/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot_JustinGuese
-Version: 0.3.34
+Version: 0.3.35
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.34/README.md` & `basebot22-basebot_JustinGuese-0.3.35/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.34/basebot22/backtest.py` & `basebot22-basebot_JustinGuese-0.3.35/basebot22/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,36 +109,42 @@
             
             for order in decisions:
                 assert isinstance(order, Order), "Decision function must return a list of orders or empty list"
                 if order.buy:
                     if order.amountInUSD == -1:
                         # all we have
                         amount = self.portfolio["USD"]
+                    else:
+                        amount = order.amountInUSD
                     fees = amount * self.commission
                     self.fees += fees
                     howMany = (amount - fees) / crntRow[order.stockname]["Close"]
                     self.portfolio["USD"] -= amount
                     self.portfolio[order.stockname] = howMany
                     
                 else:
                     # sell or short
                     if self.portfolio.get(order.stockname,0) > 0:
                         if order.amountInUSD == -1:
                             # all we have
                             amount = self.portfolio.get(order.stockname) * crntRow[order.stockname]["Close"]
+                        else:
+                            amount = order.amountInUSD
                         # sell regular
                         fees = amount * self.commission
                         self.fees += fees
                         self.portfolio["USD"] += amount - fees
                         self.portfolio[order.stockname] = 0
                     elif self.portfolio.get(order.stockname,0) == 0 and order.amountInUSD < 0:
                         # short
                         if order.amountInUSD == -1:
                             # all we have
                             amount = self.portfolio["USD"]
+                        else:
+                            amount = order.amountInUSD
                         self.boughtAt[order.stockname] = crntRow[order.stockname]["Close"]
                         fees = amount * self.commission
                         self.fees += fees
                         self.portfolio["USD"] -= amount
                         self.portfolio[order.stockname] = (amount / crntRow[order.stockname]["Close"]) * -1
                     elif self.portfolio.get(order.stockname,0) < 0:
                         # sell a short
```

### Comparing `basebot22-basebot_JustinGuese-0.3.34/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.35/basebot22/basebot.py`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.34/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.35/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basebot22-basebot-JustinGuese
-Version: 0.3.34
+Version: 0.3.35
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.34/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "basebot22-basebot_JustinGuese"
 authors = [
   { name="Justin Güse", email="guese.justin@gmail.com" },
 ]
 description = "A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots"
 readme = "README.md"
-version = "0.3.34"
+version = "0.3.35"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

