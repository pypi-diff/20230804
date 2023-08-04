# Comparing `tmp/TellrawGenerator-0.0.1.tar.gz` & `tmp/TellrawGenerator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TellrawGenerator-0.0.1.tar", last modified: Fri Aug  4 13:27:56 2023, max compression
+gzip compressed data, was "TellrawGenerator-0.0.2.tar", last modified: Fri Aug  4 18:44:48 2023, max compression
```

## Comparing `TellrawGenerator-0.0.1.tar` & `TellrawGenerator-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 zoozdooz   (501) staff       (20)        0 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/
--rw-r--r--   0 zoozdooz   (501) staff       (20)     1610 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/PKG-INFO
-drwxr-xr-x   0 zoozdooz   (501) staff       (20)        0 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/TellrawGenerator.egg-info/
--rw-r--r--   0 zoozdooz   (501) staff       (20)     1610 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/TellrawGenerator.egg-info/PKG-INFO
--rw-r--r--   0 zoozdooz   (501) staff       (20)      168 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/TellrawGenerator.egg-info/SOURCES.txt
--rw-r--r--   0 zoozdooz   (501) staff       (20)        1 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/TellrawGenerator.egg-info/top_level.txt
--rw-r--r--   0 zoozdooz   (501) staff       (20)        1 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/TellrawGenerator.egg-info/dependency_links.txt
--rw-r--r--   0 zoozdooz   (501) staff       (20)     1344 2023-08-04 13:27:28.000000 TellrawGenerator-0.0.1/setup.py
--rw-r--r--   0 zoozdooz   (501) staff       (20)       38 2023-08-04 13:27:56.000000 TellrawGenerator-0.0.1/setup.cfg
+drwxr-xr-x   0 zoozdooz   (501) staff       (20)        0 2023-08-04 18:44:48.717628 TellrawGenerator-0.0.2/
+-rw-r--r--   0 zoozdooz   (501) staff       (20)     1314 2023-08-04 18:44:48.717342 TellrawGenerator-0.0.2/PKG-INFO
+drwxr-xr-x   0 zoozdooz   (501) staff       (20)        0 2023-08-04 18:44:48.715393 TellrawGenerator-0.0.2/TellrawGenerator/
+-rw-r--r--   0 zoozdooz   (501) staff       (20)     1861 2023-08-04 18:37:15.000000 TellrawGenerator-0.0.2/TellrawGenerator/TellrawGenerator.py
+-rw-r--r--   0 zoozdooz   (501) staff       (20)       25 2023-08-04 18:24:42.000000 TellrawGenerator-0.0.2/TellrawGenerator/__init__.py
+drwxr-xr-x   0 zoozdooz   (501) staff       (20)        0 2023-08-04 18:44:48.716953 TellrawGenerator-0.0.2/TellrawGenerator.egg-info/
+-rw-r--r--   0 zoozdooz   (501) staff       (20)     1314 2023-08-04 18:44:48.000000 TellrawGenerator-0.0.2/TellrawGenerator.egg-info/PKG-INFO
+-rw-r--r--   0 zoozdooz   (501) staff       (20)      234 2023-08-04 18:44:48.000000 TellrawGenerator-0.0.2/TellrawGenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 zoozdooz   (501) staff       (20)        1 2023-08-04 18:44:48.000000 TellrawGenerator-0.0.2/TellrawGenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 zoozdooz   (501) staff       (20)       17 2023-08-04 18:44:48.000000 TellrawGenerator-0.0.2/TellrawGenerator.egg-info/top_level.txt
+-rw-r--r--   0 zoozdooz   (501) staff       (20)       38 2023-08-04 18:44:48.717781 TellrawGenerator-0.0.2/setup.cfg
+-rw-r--r--   0 zoozdooz   (501) staff       (20)     1452 2023-08-04 18:42:47.000000 TellrawGenerator-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TellrawGenerator-0.0.1/PKG-INFO` & `TellrawGenerator-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: TellrawGenerator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tellraw command generator for minecraft
-Home-page: UNKNOWN
 Author: TellrawGenerator
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: 
-        This module is a tool for making tellraw commands easier to create.
-        
-        Usage:
-        
-        Even though its meant to be simple, there are still steps to creating your command.
-        
-        To create a line, you have to make an instance of the "Line" class,
-         
-        and all of the attributes are written in between the parentheses of the class.
-        
-        There is a specific order of the attributes: Text, Color, Underline, Italic, Bold, Obfuscated, and Strikethrough.
-        
-        Example: line1 = line("Hello World","orange",True,True,True,False,False)
-        
-        After you are done creating your lines, put them in a list and in the parentheses of the "GenerateCommand",
-        
-        The result will be returned.
-        
-        Example:
-        
-        line1 = line("Hello","red",True,True,True,False,False)
-        
-        line2 = line(" World!","blue",True,True,True,False,False)
-        
-        lines = [line1, line2]
-        
-        command = GenerateCommand(lines)
-        
-        print(command)
-        
-        Notes:
-        
-        In-game, every line will be combined into 1 line with no spaces, 
-        
-        so dont forget to put in spaces before each line and Backslash + N for line breaks.
-        
-        Also, replace the <targets> text in the result with your actual targets.
-        
-        
-Platform: UNKNOWN
+
+
+This module is a tool for making tellraw commands easier to create.
+
+Usage:
+
+Even though its meant to be simple, there are still steps to creating your command.
+
+To create a line, you have to make an instance of the "Line" class,
+ 
+and all of the attributes are written in between the parentheses of the class.
+
+There is a specific order of the attributes: Text, Color, Underline, Italic, Bold, Obfuscated, and Strikethrough.
+
+Example: line1 = line("Hello World","orange",True,True,True,False,False)
+
+After you are done creating your lines, put them in a list and in the parentheses of the "GenerateCommand",
+
+The result will be returned.
+
+Example:
+
+line1 = line("Hello","red",True,True,True,False,False)
+
+line2 = line(" World!","blue",True,True,True,False,False)
+
+lines = [line1, line2]
+
+command = GenerateCommand(lines)
+
+print(command)
+
+Notes:
+
+In-game, every line will be combined into 1 line with no spaces, 
+
+so dont forget to put in spaces before each line and Backslash + N for line breaks.
+
+Also, replace the <targets> text in the result with your actual targets.
+
+Update notes:
+
+0.0.1 First upload
+
+0.0.2 Fixed import not working, also fixed GenerateCommand function.
+
```

### Comparing `TellrawGenerator-0.0.1/TellrawGenerator.egg-info/PKG-INFO` & `TellrawGenerator-0.0.2/TellrawGenerator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: TellrawGenerator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tellraw command generator for minecraft
-Home-page: UNKNOWN
 Author: TellrawGenerator
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: 
-        This module is a tool for making tellraw commands easier to create.
-        
-        Usage:
-        
-        Even though its meant to be simple, there are still steps to creating your command.
-        
-        To create a line, you have to make an instance of the "Line" class,
-         
-        and all of the attributes are written in between the parentheses of the class.
-        
-        There is a specific order of the attributes: Text, Color, Underline, Italic, Bold, Obfuscated, and Strikethrough.
-        
-        Example: line1 = line("Hello World","orange",True,True,True,False,False)
-        
-        After you are done creating your lines, put them in a list and in the parentheses of the "GenerateCommand",
-        
-        The result will be returned.
-        
-        Example:
-        
-        line1 = line("Hello","red",True,True,True,False,False)
-        
-        line2 = line(" World!","blue",True,True,True,False,False)
-        
-        lines = [line1, line2]
-        
-        command = GenerateCommand(lines)
-        
-        print(command)
-        
-        Notes:
-        
-        In-game, every line will be combined into 1 line with no spaces, 
-        
-        so dont forget to put in spaces before each line and Backslash + N for line breaks.
-        
-        Also, replace the <targets> text in the result with your actual targets.
-        
-        
-Platform: UNKNOWN
+
+
+This module is a tool for making tellraw commands easier to create.
+
+Usage:
+
+Even though its meant to be simple, there are still steps to creating your command.
+
+To create a line, you have to make an instance of the "Line" class,
+ 
+and all of the attributes are written in between the parentheses of the class.
+
+There is a specific order of the attributes: Text, Color, Underline, Italic, Bold, Obfuscated, and Strikethrough.
+
+Example: line1 = line("Hello World","orange",True,True,True,False,False)
+
+After you are done creating your lines, put them in a list and in the parentheses of the "GenerateCommand",
+
+The result will be returned.
+
+Example:
+
+line1 = line("Hello","red",True,True,True,False,False)
+
+line2 = line(" World!","blue",True,True,True,False,False)
+
+lines = [line1, line2]
+
+command = GenerateCommand(lines)
+
+print(command)
+
+Notes:
+
+In-game, every line will be combined into 1 line with no spaces, 
+
+so dont forget to put in spaces before each line and Backslash + N for line breaks.
+
+Also, replace the <targets> text in the result with your actual targets.
+
+Update notes:
+
+0.0.1 First upload
+
+0.0.2 Fixed import not working, also fixed GenerateCommand function.
+
```

### Comparing `TellrawGenerator-0.0.1/setup.py` & `TellrawGenerator-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,12 +17,15 @@
 lines = [line1, line2]\n
 command = GenerateCommand(lines)\n
 print(command)\n
 Notes:\n
 In-game, every line will be combined into 1 line with no spaces, \n
 so dont forget to put in spaces before each line and Backslash + N for line breaks.\n
 Also, replace the <targets> text in the result with your actual targets.\n
+Update notes:\n
+0.0.1 First upload\n
+0.0.2 Fixed import not working, also fixed GenerateCommand function.\n
 '''
 author = 'Abdulaziz'
-version = '0.0.1'
+version = '0.0.2'
 name = 'TellrawGenerator'
 setup(name=name,version=version,author=name,description=desc,long_description=long_desc)
```

