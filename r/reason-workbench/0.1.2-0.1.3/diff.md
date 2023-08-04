# Comparing `tmp/reason_workbench-0.1.2.tar.gz` & `tmp/reason_workbench-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reason_workbench-0.1.2.tar", last modified: Fri Aug  4 19:30:59 2023, max compression
+gzip compressed data, was "reason_workbench-0.1.3.tar", last modified: Fri Aug  4 19:48:54 2023, max compression
```

## Comparing `reason_workbench-0.1.2.tar` & `reason_workbench-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:30:59.119069 reason_workbench-0.1.2/
--rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-04 19:30:59.118201 reason_workbench-0.1.2/PKG-INFO
--rw-r--r--   0 joshbottum   (501) staff       (20)      189 2023-07-29 15:22:53.000000 reason_workbench-0.1.2/README.md
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:30:59.112362 reason_workbench-0.1.2/reason_workbench/
--rw-r--r--   0 joshbottum   (501) staff       (20)       32 2023-07-29 15:18:43.000000 reason_workbench-0.1.2/reason_workbench/__init__.py
--rw-r--r--   0 joshbottum   (501) staff       (20)    17468 2023-08-03 21:31:08.000000 reason_workbench-0.1.2/reason_workbench/main.py
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:30:59.117293 reason_workbench-0.1.2/reason_workbench.egg-info/
--rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/PKG-INFO
--rw-r--r--   0 joshbottum   (501) staff       (20)      314 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/SOURCES.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)        1 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/dependency_links.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       64 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/entry_points.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       42 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/requires.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       17 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/top_level.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       38 2023-08-04 19:30:59.119277 reason_workbench-0.1.2/setup.cfg
--rw-r--r--   0 joshbottum   (501) staff       (20)      418 2023-08-04 19:29:12.000000 reason_workbench-0.1.2/setup.py
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:48:54.963528 reason_workbench-0.1.3/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-04 19:48:54.963142 reason_workbench-0.1.3/PKG-INFO
+-rw-r--r--   0 joshbottum   (501) staff       (20)    75618 2023-08-04 19:47:09.000000 reason_workbench-0.1.3/README.md
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:48:54.959083 reason_workbench-0.1.3/reason_workbench/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       32 2023-07-29 15:18:43.000000 reason_workbench-0.1.3/reason_workbench/__init__.py
+-rw-r--r--   0 joshbottum   (501) staff       (20)    17486 2023-08-04 19:48:02.000000 reason_workbench-0.1.3/reason_workbench/main.py
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:48:54.962558 reason_workbench-0.1.3/reason_workbench.egg-info/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-04 19:48:54.000000 reason_workbench-0.1.3/reason_workbench.egg-info/PKG-INFO
+-rw-r--r--   0 joshbottum   (501) staff       (20)      314 2023-08-04 19:48:54.000000 reason_workbench-0.1.3/reason_workbench.egg-info/SOURCES.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)        1 2023-08-04 19:48:54.000000 reason_workbench-0.1.3/reason_workbench.egg-info/dependency_links.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       64 2023-08-04 19:48:54.000000 reason_workbench-0.1.3/reason_workbench.egg-info/entry_points.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       42 2023-08-04 19:48:54.000000 reason_workbench-0.1.3/reason_workbench.egg-info/requires.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       17 2023-08-04 19:48:54.000000 reason_workbench-0.1.3/reason_workbench.egg-info/top_level.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       38 2023-08-04 19:48:54.963681 reason_workbench-0.1.3/setup.cfg
+-rw-r--r--   0 joshbottum   (501) staff       (20)      418 2023-08-04 19:47:56.000000 reason_workbench-0.1.3/setup.py
```

### Comparing `reason_workbench-0.1.2/reason_workbench/main.py` & `reason_workbench-0.1.3/reason_workbench/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,23 +299,24 @@
 
         # Generate prompt responses and collect data
         pbar.set_description_str("Generating responses")
         epoch_record = generate_prompt_responses(input_data, pipe, model_load_time, tokenizer_load_time, pipeline_load_time)
         pbar.update(1)
 
     valid_choices = ['1', '2', '3', '4', '5','6']
-    
+    print()
+
     while True:
         print("Select the output options (for multiple options, separate by comma e.g. 1,2):")
-        print("1. Printed Output")
-        print("2. File of Printed Output")
-        print("3. Plots of Output")
-        print("4. epoch_record.csv File")
-        print("5. epoch_record.json File")
-        print("6. Markdown Output")  # Add this option for Markdown output
+        print("1. Output report to console")
+        print("2. Output report to txt file")
+        print("3. Plots of load times and generation times")
+        print("4. epoch_record.csv file")
+        print("5. epoch_record.json file")
+        print("6. output.md Markdown file")  
         user_output_choice = input().strip()
         user_output_choices = user_output_choice.split(',')
 
         if all(choice in valid_choices for choice in user_output_choices):
             break
         else:
             print("Invalid choice. Please try again.")
@@ -345,8 +346,8 @@
         save_output_to_markdown(epoch_record)
 
 
     
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

