# Comparing `tmp/scPANTHEON-0.3.9.1.tar.gz` & `tmp/scPANTHEON-0.3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.3.9.1.tar", last modified: Wed Aug  2 08:25:03 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.9.2.tar", last modified: Fri Aug  4 13:13:02 2023, max compression
```

## Comparing `scPANTHEON-0.3.9.1.tar` & `scPANTHEON-0.3.9.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.377318 scPANTHEON-0.3.9.1/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2023-08-02 08:25:03.377318 scPANTHEON-0.3.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.362903 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      290 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.366924 scPANTHEON-0.3.9.1/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.1/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.369526 scPANTHEON-0.3.9.1/scpantheon/app/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.1/scpantheon/app/__init__.py
--rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.9.1/scpantheon/app/bokeh_qt.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.374386 scPANTHEON-0.3.9.1/scpantheon/front_end/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.1/scpantheon/front_end/__init__.py
--rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.9.1/scpantheon/front_end/data_qt.py
--rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.9.1/scpantheon/front_end/save_qt.py
--rw-rw-rw-   0        0        0     1363 2023-07-20 07:37:16.000000 scPANTHEON-0.3.9.1/scpantheon/main.py
--rw-rw-rw-   0        0        0    66241 2023-07-20 07:40:37.000000 scPANTHEON-0.3.9.1/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2023-08-02 08:25:03.377318 scPANTHEON-0.3.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-08-02 08:24:06.000000 scPANTHEON-0.3.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:13:02.273760 scPANTHEON-0.3.9.2/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2023-08-04 13:13:02.273760 scPANTHEON-0.3.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 13:13:02.258916 scPANTHEON-0.3.9.2/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      290 2023-08-04 13:13:01.000000 scPANTHEON-0.3.9.2/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-08-04 13:13:02.000000 scPANTHEON-0.3.9.2/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 13:13:01.000000 scPANTHEON-0.3.9.2/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-04 13:13:01.000000 scPANTHEON-0.3.9.2/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-08-04 13:13:01.000000 scPANTHEON-0.3.9.2/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 13:13:01.000000 scPANTHEON-0.3.9.2/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 13:13:02.262772 scPANTHEON-0.3.9.2/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.2/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:13:02.265886 scPANTHEON-0.3.9.2/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.2/scpantheon/app/__init__.py
+-rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.9.2/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:13:02.271732 scPANTHEON-0.3.9.2/scpantheon/front_end/
+-rw-rw-rw-   0        0        0     6887 2023-08-04 12:24:07.000000 scPANTHEON-0.3.9.2/scpantheon/front_end/R_data_qt.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.2/scpantheon/front_end/__init__.py
+-rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.9.2/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.9.2/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1363 2023-08-04 11:26:27.000000 scPANTHEON-0.3.9.2/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66286 2023-08-04 12:36:11.000000 scPANTHEON-0.3.9.2/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2023-08-04 13:13:02.273760 scPANTHEON-0.3.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-08-04 13:12:34.000000 scPANTHEON-0.3.9.2/setup.py
```

### Comparing `scPANTHEON-0.3.9.1/scpantheon/app/bokeh_qt.py` & `scPANTHEON-0.3.9.2/scpantheon/app/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.1/scpantheon/front_end/data_qt.py` & `scPANTHEON-0.3.9.2/scpantheon/front_end/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.1/scpantheon/front_end/save_qt.py` & `scPANTHEON-0.3.9.2/scpantheon/front_end/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.1/scpantheon/main.py` & `scPANTHEON-0.3.9.2/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.1/scpantheon/source.py` & `scPANTHEON-0.3.9.2/scpantheon/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         self.data_columns = self.data_df.columns.values.tolist()
         self.data_df['color'] = pandas.Series(d3['Category20c'][20][0], index=self.data_df.index)
         self.data_log['color'] = pandas.Series(d3['Category20c'][20][0], index=self.data_df.index)
         self.data_df['hl_gene'] = pandas.Series(np.full(self.data_df.shape[0], 3), index=self.data_df.index)    
         self.source = ColumnDataSource(data=self.data_df[self.data_columns[0:2]+['color']+['hl_gene']])                             
         self.opts = dict(plot_width=500, plot_height=500, min_border=0, tools="pan,lasso_select,box_select,wheel_zoom,save")
         views = list(self.adata.obsm.keys())
+        # print('views:!!!!!!!!!!!', views)
         if views != []:
             for view_name in views:
                 for i in range(self.adata.obsm[view_name].shape[1]):
                     self.data_df[view_name+str(i)] = pandas.Series(self.adata.obsm[view_name][:,i],index=self.data_df.index)
                     self.data_log[view_name+str(i)] = self.data_df[view_name+str(i)]
             view_existed = True
         else:
```

### Comparing `scPANTHEON-0.3.9.1/setup.py` & `scPANTHEON-0.3.9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.9.1',#版本
+    version='0.3.9.2',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
-                        'appdirs',], # 依赖包,如果没有,可以不要
+                        'appdirs','rpy2'], # 依赖包,如果没有,可以不要
     extras_require={
         'tomas': ['tomas'], 'leidenalg': ['leidenalg']
     }, # 依赖包,深度使用需手动安装
     entry_points={
         'console_scripts': [
             'sc-pantheon = scpantheon.main:main' # scripts -> multiprocessing
         ]
```

