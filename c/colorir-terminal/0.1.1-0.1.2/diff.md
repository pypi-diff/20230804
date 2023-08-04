# Comparing `tmp/colorir_terminal-0.1.1.tar.gz` & `tmp/colorir_terminal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorir_terminal-0.1.1.tar", max compression
+gzip compressed data, was "colorir_terminal-0.1.2.tar", max compression
```

## Comparing `colorir_terminal-0.1.1.tar` & `colorir_terminal-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       40 2023-08-04 14:44:48.954820 colorir_terminal-0.1.1/colorir_terminal/__init__.py
--rw-r--r--   0        0        0     2554 2023-08-04 14:21:10.011368 colorir_terminal-0.1.1/colorir_terminal/app.py
--rw-r--r--   0        0        0      375 2023-08-04 14:54:58.391258 colorir_terminal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-08-04 14:22:17.781123 colorir_terminal-0.1.1/README.md
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 colorir_terminal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2023-08-04 14:57:30.847808 colorir_terminal-0.1.2/colorir_terminal/__init__.py
+-rw-r--r--   0        0        0     2554 2023-08-04 14:21:10.011368 colorir_terminal-0.1.2/colorir_terminal/app.py
+-rw-r--r--   0        0        0      375 2023-08-04 14:57:43.689164 colorir_terminal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1373 2023-08-04 14:22:17.781123 colorir_terminal-0.1.2/README.md
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 colorir_terminal-0.1.2/PKG-INFO
```

### Comparing `colorir_terminal-0.1.1/colorir_terminal/app.py` & `colorir_terminal-0.1.2/colorir_terminal/app.py`

 * *Files identical despite different names*

### Comparing `colorir_terminal-0.1.1/README.md` & `colorir_terminal-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `colorir_terminal-0.1.1/PKG-INFO` & `colorir_terminal-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorir-terminal
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Jefferson L. Alionco
 Author-email: Jeffersonalionco@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: color-terminal (>=1.0,<2.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colorir-terminal Version: 0.1.1 Summary: Author:
+Metadata-Version: 2.1 Name: colorir-terminal Version: 0.1.2 Summary: Author:
 Jefferson L. Alionco Author-email: Jeffersonalionco@gmail.com Requires-Python:
 >=3.11,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: color-terminal
 (>=1.0,<2.0) Description-Content-Type: text/markdown # color-terminal - Colorir
 terminal Python Um pacote para vocÃª colorir seu terminal python, e deixar as
 coisas mais animada. !["TELA"](./imagem.PNG) ### InstalaÃ§Ã£o do Projeto Local
 + Baixe o Repositorio: `git clone https://github.com/jeffersonalionco/color-
```

