# Comparing `tmp/whatsapp-converter-0.6.3.tar.gz` & `tmp/whatsapp-converter-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-converter-0.6.3.tar", last modified: Thu Aug  3 12:19:32 2023, max compression
+gzip compressed data, was "whatsapp-converter-0.6.4.tar", last modified: Fri Aug  4 15:53:46 2023, max compression
```

## Comparing `whatsapp-converter-0.6.3.tar` & `whatsapp-converter-0.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.675329 whatsapp-converter-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/tests/test_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/whatsapp_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/whatsapp_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:53:46.008349 whatsapp-converter-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-04 15:53:46.008349 whatsapp-converter-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:53:46.008349 whatsapp-converter-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:53:46.004349 whatsapp-converter-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:53:46.008349 whatsapp-converter-0.6.4/whatsapp_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/whatsapp_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/whatsapp_converter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/whatsapp_converter/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/whatsapp_converter/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-08-04 15:53:37.000000 whatsapp-converter-0.6.4/whatsapp_converter/whatsapp_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:53:46.008349 whatsapp-converter-0.6.4/whatsapp_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-04 15:53:45.000000 whatsapp-converter-0.6.4/whatsapp_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-04 15:53:46.000000 whatsapp-converter-0.6.4/whatsapp_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:53:45.000000 whatsapp-converter-0.6.4/whatsapp_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 15:53:46.000000 whatsapp-converter-0.6.4/whatsapp_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-04 15:53:46.000000 whatsapp-converter-0.6.4/whatsapp_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 15:53:46.000000 whatsapp-converter-0.6.4/whatsapp_converter.egg-info/top_level.txt
```

### Comparing `whatsapp-converter-0.6.3/LICENSE` & `whatsapp-converter-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.3/PKG-INFO` & `whatsapp-converter-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-converter
-Version: 0.6.3
+Version: 0.6.4
 Summary: Use whatsapp-converter to convert your exported WhatsApp chat to a CSV or XLS (Excel spreadsheet) file.
 Home-page: https://github.com/sandsturm/whatsapp-converter
 Author: Martin Sand
 Author-email: marti.sand.dev@gmail.com
 License: LICENSE.txt
 Project-URL: Source, https://github.com/sandsturm/whatsapp-converter/
 Project-URL: Bug Reports, https://github.com/sandsturm/whatsapp-converter/issues
```

### Comparing `whatsapp-converter-0.6.3/README.md` & `whatsapp-converter-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.3/setup.py` & `whatsapp-converter-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.3/tests/test_parse.py` & `whatsapp-converter-0.6.4/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.3/whatsapp_converter/__main__.py` & `whatsapp-converter-0.6.4/whatsapp_converter/__main__.py`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.3/whatsapp_converter/whatsapp_converter.py` & `whatsapp-converter-0.6.4/whatsapp_converter/whatsapp_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     pattern_date = re.compile('^\[?((\d{1,2})([\/|\.])(\d{1,2})[\/|\.](\d{1,4}))\,?\ (\d{1,2}[:|.]\d{1,2})([:|.]\d{1,2})?\ ?(AM|PM|am|pm)?([\:\ |\ \-\ |\]\ ][^:])(.+?)\:\ (.*)')
     match = pattern_date.match(line)
     dataset = ['empty', '', '', '', '', '']
 
     # ---------------------------------------------
     # if verbose: print(prefix + line)
     # if verbose: print(BCOLORS.FAIL + prefix + line)
-    # Identify the date format in the chat line
+    # Identify the in the chat line
 
     if match:
 
         if match and match.group(10) !=  'M':
 
             date = datetime.datetime.strptime(match.group(1), date_formats["date_format"]).date()
 
@@ -89,15 +89,15 @@
             lastentry["lasttime"] = time.strftime("%H:%M")
             lastentry["lastname"] = match.group(10)
 
             # ---------------------------------------------
             # Create the dataset for the new message
             dataset = ['new', date.strftime("%Y-%m-%d") + " " + time.strftime("%H:%M"), date.strftime("%Y-%m-%d"), time.strftime("%H:%M"), str(match.group(10)), match.group(11)]
 
-            if verbose | debug:
+            if verbose or debug:
                 print(dataset)
 
     elif re.match(re.compile(r"^[\t ]*\n", re.VERBOSE), line):
 
         # ---------------------------------------------
         # Empty line
         if debug:
@@ -111,15 +111,15 @@
             print("Appending line found")
 
         text = (re.match(re.compile(r"^(.*)", re.VERBOSE), line))
 
         # ---------------------------------------------
         # Create the dataset if commandline argument was to create a new line
         # TODO if (newline):
-        print(newline)
+        # print(newline)
         if newline:
             dataset = ['new', str(lastentry["lastdate"]) + " " + str(lastentry["lasttime"]), str(lastentry["lastdate"]), str(lastentry["lasttime"]), lastentry["lastname"], text.group(0)]
 
         else:
             dataset = ['append', str(lastentry["lastdate"]) + " " + str(lastentry["lasttime"]), str(lastentry["lastdate"]), str(lastentry["lasttime"]), lastentry["lastname"], text.group(0)]
 
     return dataset
@@ -145,53 +145,62 @@
 
     try:
         with io.open(filename, "r", encoding="utf-8") as file:
             print("Reading import file")
 
             content = file.readlines()  # Read all lines at once
             line_count = len(content)  # Get the number of read lines
+            confirmed_date = False  # Exit condition for For loop based on a date > 12
 
-                if re.match(re.compile(pattern, re.VERBOSE), line):
+            for line in content:
 
-                    # ---------------------------------------------
-                    # Make the match, assign to the groups
-                    match = re.match(re.compile(pattern, re.VERBOSE), line)
+                if confirmed_date == True:
+                    break
+
+                if not line.strip():  # Check if the line is empty or contains only whitespace
+                    continue  # Skip the rest of the loop and move to the next iteration
+
+                # ---------------------------------------------
+                # Make the match, assign to the groups
+                match = re.match(re.compile(pattern, re.VERBOSE), line)
+                
+                if match:
 
                     # ---------------------------------------------
-                    # 21/12/19 Date Format
-                    if match.group(3) == '/' and match.group(9) == ': ':
+                    # 21/12/19
+                    if match.group(3) == '/' and (match.group(9) == ' -' or match.group(9) == '- ' or match.group(9) == ': '):
                         if debug:
-                            print("d/m/y Date Format")
+                            print("Date format d/m/y")
                         if len(match.group(5)) == 4:
                             date_formats["date_format"] = "%d/%m/%Y"
                         else:
                             date_formats["date_format"] = "%d/%m/%y"
 
                     # ---------------------------------------------
-                    # 12/21/19 Date Format
+                    # 12/21/19
                     elif match.group(3) == '/' and (match.group(9) == ' -' or match.group(9) == '- '):
                         if debug:
-                            print("m/d/y Date Format")
+                            print("Date format m/d/y")
                         if len(match.group(5)) == 4 and match.group(7) is None:
                             date_formats["date_format"] = "%m/%d/%Y"
                         else:
                             date_formats["date_format"] = "%m/%d/%y"
 
                     # ---------------------------------------------
-                    # 21/12/2019 Date Format with square brackets and am
+                    # 21/12/2019 with square brackets and am
                     elif match.group(3) == '/' and match.group(9) == '] ' and (match.group(8) == 'am' or match.group(8) == 'pm'):
                         if debug:
-                            print("d/m/Y Date Format with [square brackets] and am/pm")
+                            print("Date format d/m/Y with [square brackets] and am/pm")
                         date_formats["date_format"] = "%d/%m/%Y"
 
                     # ---------------------------------------------
-                    # 12/21/2019 Date Format with square brackets
+                    # 12/21/2019 with square brackets
                     elif match.group(3) == '/' and match.group(9) == '] ':
                         if debug:
-                            print("m/d/Y Date Format with [square brackets]")
+                            print("Date format m/d/Y with [square brackets]")
                         if check_monthfirst(match.group(1)) and not date_formats["mdyS"]:
                             date_formats["mdyS"] = True
                             date_formats["date_format"] = "%d/%m/%Y"
                         if date_formats["mdyS"]:
                             if len(match.group(5)) == 4:
                                 date_formats["date_format"] = "%d/%m/%Y"
                             else:
@@ -199,29 +208,29 @@
                         else:
                             if len(match.group(5)) == 4:
                                 date_formats["date_format"] = "%m/%d/%Y"
                             else:
                                 date_formats["date_format"] = "%m/%d/%y"
 
                     # ---------------------------------------------
-                    # 21.12.19 Date Format
+                    # 21.12.19
                     else:
                         if debug:
-                            print("d.m.y Date Format")
+                            print("Date format d.m.y")
                         if len(match.group(5)) == 4:
                             date = datetime.datetime.strptime(match.group(1), "%d.%m.%Y").date()
                             date_formats["date_format"] = "%d.%m.%Y"
                         else:
                             date_formats["date_format"] = "%d.%m.%y"
 
     except IOError as e:
         print("File \"" + filename + "\" cannot be found.")
         sys.exit()
 
-    print("Converting data now")
+    print("Converting data now with data format " + date_formats["date_format"])
 
     # ---------------------------------------------
     # Count number of chatlines without  linesError: Excel 2003 only supports a maximum of 65535 lines.
     # Whatsapp-converter found more than 65535 lines for input which might lead to an error.\n
     counter = 0
 
     if debug:
```

### Comparing `whatsapp-converter-0.6.3/whatsapp_converter.egg-info/PKG-INFO` & `whatsapp-converter-0.6.4/whatsapp_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-converter
-Version: 0.6.3
+Version: 0.6.4
 Summary: Use whatsapp-converter to convert your exported WhatsApp chat to a CSV or XLS (Excel spreadsheet) file.
 Home-page: https://github.com/sandsturm/whatsapp-converter
 Author: Martin Sand
 Author-email: marti.sand.dev@gmail.com
 License: LICENSE.txt
 Project-URL: Source, https://github.com/sandsturm/whatsapp-converter/
 Project-URL: Bug Reports, https://github.com/sandsturm/whatsapp-converter/issues
```

