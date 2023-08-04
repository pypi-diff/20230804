# Comparing `tmp/cntdrun-1.0.1.tar.gz` & `tmp/cntdrun-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cntdrun-1.0.1.tar", last modified: Fri Aug  4 02:00:05 2023, max compression
+gzip compressed data, was "cntdrun-1.0.2.tar", last modified: Fri Aug  4 02:03:31 2023, max compression
```

## Comparing `cntdrun-1.0.1.tar` & `cntdrun-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 02:00:05.019534 cntdrun-1.0.1/
--rw-rw-rw-   0        0        0      220 2023-08-04 02:00:05.019008 cntdrun-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-08-04 01:16:40.000000 cntdrun-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 02:00:05.017436 cntdrun-1.0.1/cntdrun.egg-info/
--rw-rw-rw-   0        0        0      220 2023-08-04 02:00:04.000000 cntdrun-1.0.1/cntdrun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-08-04 02:00:04.000000 cntdrun-1.0.1/cntdrun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 02:00:04.000000 cntdrun-1.0.1/cntdrun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-04 02:00:04.000000 cntdrun-1.0.1/cntdrun.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-08-04 02:00:04.000000 cntdrun-1.0.1/cntdrun.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-04 02:00:04.000000 cntdrun-1.0.1/cntdrun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3105 2023-08-04 01:54:22.000000 cntdrun-1.0.1/cntdrun.py
--rw-rw-rw-   0        0        0       42 2023-08-04 02:00:05.020055 cntdrun-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      475 2023-08-04 01:59:30.000000 cntdrun-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 02:03:31.229988 cntdrun-1.0.2/
+-rw-rw-rw-   0        0        0      220 2023-08-04 02:03:31.229469 cntdrun-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-08-04 01:16:40.000000 cntdrun-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 02:03:31.228951 cntdrun-1.0.2/cntdrun.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-08-04 02:03:31.000000 cntdrun-1.0.2/cntdrun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-08-04 02:03:31.000000 cntdrun-1.0.2/cntdrun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 02:03:31.000000 cntdrun-1.0.2/cntdrun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-04 02:03:31.000000 cntdrun-1.0.2/cntdrun.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 02:03:31.000000 cntdrun-1.0.2/cntdrun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-04 02:03:31.000000 cntdrun-1.0.2/cntdrun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3127 2023-08-04 02:03:15.000000 cntdrun-1.0.2/cntdrun.py
+-rw-rw-rw-   0        0        0       42 2023-08-04 02:03:31.229988 cntdrun-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-08-04 02:03:27.000000 cntdrun-1.0.2/setup.py
```

### Comparing `cntdrun-1.0.1/cntdrun.py` & `cntdrun-1.0.2/cntdrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,20 @@
                 except Exception as e:
                     print("Error occurred while executing command:", e)
 
     def keyPressEvent(self, event):
         if event.key() in (Qt.Key_Enter, Qt.Key_Return):
             self.close_button.click()
 
-if __name__ == "__main__":
+def main()
     parser = argparse.ArgumentParser()
     parser.add_argument("count", type=int, help="Countdown time in seconds")
     parser.add_argument("command", type=str, help="Command to execute after countdown")
     args = parser.parse_args()
 
     app = QApplication(sys.argv)
     window = CountdownWindow(args.count, args.command)
     window.show()
     sys.exit(app.exec_())
 
+if __name__ == "__main__":
+    main()
```

