# Comparing `tmp/kimariplot-1.2.5.tar.gz` & `tmp/kimariplot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.2.5.tar", last modified: Wed Aug  2 16:50:55 2023, max compression
+gzip compressed data, was "kimariplot-1.3.0.tar", last modified: Fri Aug  4 03:54:01 2023, max compression
```

## Comparing `kimariplot-1.2.5.tar` & `kimariplot-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:50:55.960501 kimariplot-1.2.5/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     4398 2023-08-02 16:50:55.960501 kimariplot-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:50:55.946605 kimariplot-1.2.5/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.5/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     9452 2023-08-02 16:50:29.000000 kimariplot-1.2.5/kimariplot/plotter.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:50:55.958502 kimariplot-1.2.5/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     4398 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 16:50:55.961536 kimariplot-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-08-02 16:50:29.000000 kimariplot-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:54:01.083075 kimariplot-1.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-07-31 06:33:53.000000 kimariplot-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4508 2023-08-04 03:54:01.082073 kimariplot-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4063 2023-08-03 06:08:36.000000 kimariplot-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 03:54:01.072047 kimariplot-1.3.0/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 13:12:07.000000 kimariplot-1.3.0/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     9281 2023-08-04 03:51:56.000000 kimariplot-1.3.0/kimariplot/plotter.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:54:01.081070 kimariplot-1.3.0/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     4508 2023-08-04 03:54:01.000000 kimariplot-1.3.0/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-04 03:54:01.000000 kimariplot-1.3.0/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 03:54:01.000000 kimariplot-1.3.0/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-04 03:54:01.000000 kimariplot-1.3.0/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 03:54:01.000000 kimariplot-1.3.0/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 03:54:01.083075 kimariplot-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-08-04 03:51:56.000000 kimariplot-1.3.0/setup.py
```

### Comparing `kimariplot-1.2.5/LICENSE` & `kimariplot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.2.5/PKG-INFO` & `kimariplot-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.5
+Version: 1.3.0
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     <img src="figure/logo.png" width="200">
 </h1><br>
 
+<img width="120%" src="https://repobeats.axiom.co/api/embed/c3ae6c194fc8f1a0989fa0afd01e39e6f32dabec.svg">
+
 KimariPlot 是一个开源的 Python 绘图脚本，用来绘制科研中的 Free Energy Profile。KimariPlot 使用简单，可以直接从命令行读取 Toml 文件绘制 Free Energy Profile，可以不需要用鼠标一直拖来拖去，是懒人绘制 Free Energy Profile 的极佳选择。
 
 ## 安装
 
 KimariPlot 可以使用 pip 工具直接安装。
 
 ```shell
```

### Comparing `kimariplot-1.2.5/README.md` & `kimariplot-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <h1 align="center">
     <img src="figure/logo.png" width="200">
 </h1><br>
 
+<img width="120%" src="https://repobeats.axiom.co/api/embed/c3ae6c194fc8f1a0989fa0afd01e39e6f32dabec.svg">
+
 KimariPlot 是一个开源的 Python 绘图脚本，用来绘制科研中的 Free Energy Profile。KimariPlot 使用简单，可以直接从命令行读取 Toml 文件绘制 Free Energy Profile，可以不需要用鼠标一直拖来拖去，是懒人绘制 Free Energy Profile 的极佳选择。
 
 ## 安装
 
 KimariPlot 可以使用 pip 工具直接安装。
 
 ```shell
```

### Comparing `kimariplot-1.2.5/kimariplot/plotter.py` & `kimariplot-1.3.0/kimariplot/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,17 @@
         # 使用上下文管理器打开文件，读取 toml 文件，并赋值给一个 toml 对象
         with file_path.open('r', encoding='utf-8') as f:
             toml_data = toml.load(f)
 
         # 创建一个空的 PlotData 对象列表
         plot_data_list = []
 
-        # 遍历 toml 对象中的所有的 profile 段落
-        for name, profile_data in toml_data['path'].items():
-            # 创建一个 PlotData 对象，并添加到 plot_data_list 中
-            plot_data = PlotData(profile_data['color'], profile_data['style'], profile_data['data'])
-            # 将读取到的 PlotData 对象放入集合中
+        # 遍历 toml 对象中的所有的 path 段落
+        for path_data in toml_data['path']:
+            plot_data = PlotData(path_data['color'], path_data['style'], path_data['data'])
             plot_data_list.append(plot_data)
 
         # 返回 PlotData 对象列表
         return plot_data_list
     except FileNotFoundError:
         raise FileNotFoundError(f"File '{file_path}' not found.")
     except (toml.TomlDecodeError, KeyError) as e:
@@ -183,16 +181,16 @@
     except Exception as e:
         raise Exception(f"An error occurred while plotting the graph: {e}")
 
 
 def main():
     # 定义版本信息
     version_info = {
-        'version': 'v1.2.5',
-        'release_date': 'Aug-3-2023',
+        'version': 'v1.3.0',
+        'release_date': 'Aug-4-2023',
         'developer': 'Kimariyb, Ryan Hsiun',
         'address': 'XiaMen University, School of Electronic Science and Engineering',
         'website': 'https://github.com/kimariyb/kimariPlot',
     }
 
     # 创建 ArgumentParser 对象
     parser = argparse.ArgumentParser(prog='KimariPlot', add_help=False,
@@ -232,8 +230,7 @@
     # 获取当前日期和时间
     now = datetime.datetime.now().strftime("%b-%d-%Y, 00:45:%S")
     # 程序结束后提示版权信息和问候语
     print(f"Thank you for using our plotting tool! Have a great day!")
     print("Copyright © 2023 Kimariyb. All rights reserved.")
     print(f"Currently timeline: {now}")
     print("============================================================================")
-
```

### Comparing `kimariplot-1.2.5/kimariplot.egg-info/PKG-INFO` & `kimariplot-1.3.0/kimariplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.5
+Version: 1.3.0
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     <img src="figure/logo.png" width="200">
 </h1><br>
 
+<img width="120%" src="https://repobeats.axiom.co/api/embed/c3ae6c194fc8f1a0989fa0afd01e39e6f32dabec.svg">
+
 KimariPlot 是一个开源的 Python 绘图脚本，用来绘制科研中的 Free Energy Profile。KimariPlot 使用简单，可以直接从命令行读取 Toml 文件绘制 Free Energy Profile，可以不需要用鼠标一直拖来拖去，是懒人绘制 Free Energy Profile 的极佳选择。
 
 ## 安装
 
 KimariPlot 可以使用 pip 工具直接安装。
 
 ```shell
```

### Comparing `kimariplot-1.2.5/setup.py` & `kimariplot-1.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.2.5",
+    version="1.3.0",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
@@ -20,8 +20,8 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
-)
+)
```

