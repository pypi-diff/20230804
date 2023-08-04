# Comparing `tmp/fpdf2-2.7.4.tar.gz` & `tmp/fpdf2-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpdf2-2.7.4.tar", last modified: Fri Apr 28 10:37:06 2023, max compression
+gzip compressed data, was "fpdf2-2.7.5.tar", last modified: Fri Aug  4 16:13:10 2023, max compression
```

## Comparing `fpdf2-2.7.4.tar` & `fpdf2-2.7.5.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:37:06.284544 fpdf2-2.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-28 10:13:25.000000 fpdf2-2.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 10:13:25.000000 fpdf2-2.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    47046 2023-04-28 10:37:06.284544 fpdf2-2.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45679 2023-04-28 10:13:25.000000 fpdf2-2.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:37:06.280544 fpdf2-2.7.4/fpdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)   148148 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    26118 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    42341 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)   192125 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/fpdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/graphics_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/html.py
--rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/image_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/line_break.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/linearization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/outline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38984 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/prefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/structure_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-28 10:13:25.000000 fpdf2-2.7.4/fpdf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:37:06.284544 fpdf2-2.7.4/fpdf2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47046 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 10:37:06.000000 fpdf2-2.7.4/fpdf2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 10:37:06.284544 fpdf2-2.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-28 10:13:25.000000 fpdf2-2.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:13:10.635532 fpdf2-2.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    46911 2023-08-04 15:54:16.000000 fpdf2-2.7.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-04 15:54:16.000000 fpdf2-2.7.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 15:54:16.000000 fpdf2-2.7.5/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-08-04 15:54:16.000000 fpdf2-2.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50174 2023-08-04 16:13:10.639532 fpdf2-2.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    48807 2023-08-04 15:54:16.000000 fpdf2-2.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:13:10.635532 fpdf2-2.7.5/fpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147817 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57305 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   191426 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/fpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/graphics_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26726 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/image_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20339 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/line_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/linearization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37091 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/prefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/structure_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30979 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-08-04 15:54:16.000000 fpdf2-2.7.5/fpdf/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:13:10.635532 fpdf2-2.7.5/fpdf2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50174 2023-08-04 16:13:10.000000 fpdf2-2.7.5/fpdf2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-04 16:13:10.000000 fpdf2-2.7.5/fpdf2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:13:10.000000 fpdf2-2.7.5/fpdf2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 16:13:10.000000 fpdf2-2.7.5/fpdf2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 16:13:10.000000 fpdf2-2.7.5/fpdf2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-04 16:13:10.639532 fpdf2-2.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-04 15:54:16.000000 fpdf2-2.7.5/setup.py
```

### Comparing `fpdf2-2.7.4/LICENSE` & `fpdf2-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/PKG-INFO` & `fpdf2-2.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: fpdf2
-Version: 2.7.4
-Summary: Simple & fast PDF generation for Python
-Home-page: https://pyfpdf.github.io/fpdf2/
-Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.4
-Author: Olivier PLATHEY ported by Max
-Maintainer: Lucas Cimon
-License: LGPLv3+
-Project-URL: Documentation, https://pyfpdf.github.io/fpdf2/
-Project-URL: Code, https://github.com/PyFPDF/fpdf2
-Project-URL: Issue tracker, https://github.com/PyFPDF/fpdf2/issues
-Keywords: pdf,unicode,png,jpg,ttf,barcode
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Printing
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Graphics :: Presentation
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Pypi latest version](https://img.shields.io/pypi/v/fpdf2.svg)](https://pypi.org/pypi/fpdf2#history)
 [![Python Support](https://img.shields.io/pypi/pyversions/fpdf2.svg)](https://pypi.org/project/fpdf2/)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 [![build status](https://github.com/PyFPDF/fpdf2/workflows/build/badge.svg)](https://github.com/PyFPDF/fpdf2/actions?query=branch%3Amaster)
 [![codecov](https://codecov.io/gh/PyFPDF/fpdf2/branch/master/graph/badge.svg)](https://codecov.io/gh/PyFPDF/fpdf2)
 ![security: bandit, pylint, semgrep](https://img.shields.io/badge/linters-bandit,pylint,semgrep-yellow.svg)
@@ -95,15 +63,15 @@
  * Internal / external [links](https://pyfpdf.github.io/fpdf2/Links.html)
  * Embedding images, including transparency and alpha channel
  * Arbitrary path drawing and basic [SVG](https://pyfpdf.github.io/fpdf2/SVG.html) import
  * Embedding [barcodes](https://pyfpdf.github.io/fpdf2/Barcodes.html), [charts & graphs](https://pyfpdf.github.io/fpdf2/Maths.html), [emojis, symbols & dingbats](https://pyfpdf.github.io/fpdf2/EmojisSymbolsDingbats.html)
  * [Tables](https://pyfpdf.github.io/fpdf2/Tables.html) and also [cell / multi-cell / plaintext writing](https://pyfpdf.github.io/fpdf2/Text.html), with [automatic page breaks](https://pyfpdf.github.io/fpdf2/PageBreaks.html), line break and text justification
  * Choice of measurement unit, page format & margins. Optional page header and footer
  * Basic [conversion from HTML to PDF](https://pyfpdf.github.io/fpdf2/HTML.html)
- * A [templating system](https://pyfpdf.github.io/fpdf2/Templates.html) to render PDFs in batchs
+ * A [templating system](https://pyfpdf.github.io/fpdf2/Templates.html) to render PDFs in batches
  * Images & links alternative descriptions, for accessibility
  * Table of contents & [document outline](https://pyfpdf.github.io/fpdf2/DocumentOutlineAndTableOfContents.html)
  * [Document encryption](https://pyfpdf.github.io/fpdf2/Encryption.html) & [document signing](https://pyfpdf.github.io/fpdf2/Signing.html)
  * [Annotations](https://pyfpdf.github.io/fpdf2/Annotations.html), including text highlights, and [file attachments](https://pyfpdf.github.io/fpdf2/FileAttachments.html)
  * [Presentation mode](https://pyfpdf.github.io/fpdf2/Presentations.html) with control over page display duration & transitions
  * Optional basic Markdown-like styling: `**bold**, __italics__`
  * Can render [mathematical equations & charts](https://pyfpdf.github.io/fpdf2/Maths.html)
@@ -132,15 +100,15 @@
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/PyFPDF/fpdf2&t=fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-facebook-1976D2?logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/PyFPDF/fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/PyFPDF/fpdf2&title=fpdf2)
 
 ## Documentation
 
 - [Documentation Home](https://pyfpdf.github.io/fpdf2/)
-- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html)
+- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html) - [ភាសខ្មែរ](https://pyfpdf.github.io/fpdf2/Tutorial-km.md) - [日本語](https://pyfpdf.github.io/fpdf2/Tutorial-ja.html)
 - Release notes: [CHANGELOG.md](https://github.com/PyFPDF/fpdf2/blob/master/CHANGELOG.md)
 - A series of blog posts: [fpdf2 tag @ ludochaordic](https://chezsoi.org/lucas/blog/tag/fpdf2.html)
 
 You can also have a look at the `tests/`, they're great usage examples!
 
 ## Developement
 
@@ -245,15 +213,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zenigata"><img src="https://avatars.githubusercontent.com/u/1022393?v=4?s=100" width="100px;" alt="Johan Bonneau"/><br /><sub><b>Johan Bonneau</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Zenigata" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jmunoz94"><img src="https://avatars.githubusercontent.com/u/48921408?v=4?s=100" width="100px;" alt="Jesús Alberto Muñoz Mesa"/><br /><sub><b>Jesús Alberto Muñoz Mesa</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Tests">⚠️</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jdeep.me"><img src="https://avatars.githubusercontent.com/u/64089730?v=4?s=100" width="100px;" alt="Jaydeep Das"/><br /><sub><b>Jaydeep Das</b></sub></a><br /><a href="#question-JDeepD" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/seanpmulholland"><img src="https://avatars.githubusercontent.com/u/79894395?v=4?s=100" width="100px;" alt="Sean"/><br /><sub><b>Sean</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=seanpmulholland" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Documentation">📖</a> <a href="#ideas-andersonhc" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/yiweelan"><img src="https://avatars.githubusercontent.com/u/117787188?v=4?s=100" width="100px;" alt="Yi Wei Lan"/><br /><sub><b>Yi Wei Lan</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=yiweelan" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bubbu0129"><img src="https://avatars.githubusercontent.com/u/93034081?v=4?s=100" width="100px;" alt="CpDong"/><br /><sub><b>CpDong</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Bubbu0129" title="Code">💻</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ABubbu0129" title="Bug reports">🐛</a> <a href="#translation-Bubbu0129" title="Translation">🌍</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/CY-Qiu"><img src="https://avatars.githubusercontent.com/u/23075447?v=4?s=100" width="100px;" alt="CY-Qiu"/><br /><sub><b>CY-Qiu</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ACY-Qiu" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Markovvn1"><img src="https://avatars.githubusercontent.com/u/32509100?v=4?s=100" width="100px;" alt="Markovvn1"/><br /><sub><b>Markovvn1</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Markovvn1" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/erap129"><img src="https://avatars.githubusercontent.com/u/30405025?v=4?s=100" width="100px;" alt="Elad Rapaport"/><br /><sub><b>Elad Rapaport</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=erap129" title="Code">💻</a></td>
@@ -266,14 +234,24 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruiz-manuel"><img src="https://avatars.githubusercontent.com/u/43274578?v=4?s=100" width="100px;" alt="Manuel Ruiz"/><br /><sub><b>Manuel Ruiz</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aruiz-manuel" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nsimonovici"><img src="https://avatars.githubusercontent.com/u/44460830?v=4?s=100" width="100px;" alt="Noel"/><br /><sub><b>Noel</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Ansimonovici" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a> <a href="#question-ssavi-ict" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aeris07"><img src="https://avatars.githubusercontent.com/u/129675592?v=4?s=100" width="100px;" alt="aeris07"/><br /><sub><b>aeris07</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aaeris07" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/KamarulAdha"><img src="https://avatars.githubusercontent.com/u/52944294?v=4?s=100" width="100px;" alt="KamarulAdha"/><br /><sub><b>KamarulAdha</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=KamarulAdha" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Valerus5685"><img src="https://avatars.githubusercontent.com/u/7953869?v=4?s=100" width="100px;" alt="Valerus5685"/><br /><sub><b>Valerus5685</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3AValerus5685" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sebastiantia"><img src="https://avatars.githubusercontent.com/u/75666019?v=4?s=100" width="100px;" alt="Sebastian Tia"/><br /><sub><b>Sebastian Tia</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=sebastiantia" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/1nv"><img src="https://avatars.githubusercontent.com/u/10288828?v=4?s=100" width="100px;" alt="Eugene Selifonov"/><br /><sub><b>Eugene Selifonov</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3A1nv" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://ez-startup.com"><img src="https://avatars.githubusercontent.com/u/69514175?v=4?s=100" width="100px;" alt="Kuth"/><br /><sub><b>Kuth</b></sub></a><br /><a href="#translation-kuth-chi" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://rdbr.nl"><img src="https://avatars.githubusercontent.com/u/34062862?v=4?s=100" width="100px;" alt="Ruben de Bruin"/><br /><sub><b>Ruben de Bruin</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ARubendeBruin" title="Bug reports">🐛</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=RubendeBruin" title="Code">💻</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=RubendeBruin" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/stenci"><img src="https://avatars.githubusercontent.com/u/5955495?v=4?s=100" width="100px;" alt="stenci"/><br /><sub><b>stenci</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Astenci" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alcnaka"><img src="https://avatars.githubusercontent.com/u/47954083?v=4?s=100" width="100px;" alt="alcnaka"/><br /><sub><b>alcnaka</b></sub></a><br /><a href="#translation-alcnaka" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tolker-KU"><img src="https://avatars.githubusercontent.com/u/55140581?v=4?s=100" width="100px;" alt="Tolker-KU"/><br /><sub><b>Tolker-KU</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Tolker-KU" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://lfavole.eu.pythonanywhere.com"><img src="https://avatars.githubusercontent.com/u/88188568?v=4?s=100" width="100px;" alt="lfavole"/><br /><sub><b>lfavole</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=lfavole" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `fpdf2-2.7.4/README.md` & `fpdf2-2.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: fpdf2
+Version: 2.7.5
+Summary: Simple & fast PDF generation for Python
+Home-page: https://pyfpdf.github.io/fpdf2/
+Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.5
+Author: Olivier PLATHEY ported by Max
+Maintainer: Lucas Cimon
+License: LGPLv3+
+Project-URL: Documentation, https://pyfpdf.github.io/fpdf2/
+Project-URL: Code, https://github.com/PyFPDF/fpdf2
+Project-URL: Issue tracker, https://github.com/PyFPDF/fpdf2/issues
+Keywords: pdf,unicode,png,jpg,ttf,barcode
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Printing
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: Presentation
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Pypi latest version](https://img.shields.io/pypi/v/fpdf2.svg)](https://pypi.org/pypi/fpdf2#history)
 [![Python Support](https://img.shields.io/pypi/pyversions/fpdf2.svg)](https://pypi.org/project/fpdf2/)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 [![build status](https://github.com/PyFPDF/fpdf2/workflows/build/badge.svg)](https://github.com/PyFPDF/fpdf2/actions?query=branch%3Amaster)
 [![codecov](https://codecov.io/gh/PyFPDF/fpdf2/branch/master/graph/badge.svg)](https://codecov.io/gh/PyFPDF/fpdf2)
 ![security: bandit, pylint, semgrep](https://img.shields.io/badge/linters-bandit,pylint,semgrep-yellow.svg)
@@ -63,15 +95,15 @@
  * Internal / external [links](https://pyfpdf.github.io/fpdf2/Links.html)
  * Embedding images, including transparency and alpha channel
  * Arbitrary path drawing and basic [SVG](https://pyfpdf.github.io/fpdf2/SVG.html) import
  * Embedding [barcodes](https://pyfpdf.github.io/fpdf2/Barcodes.html), [charts & graphs](https://pyfpdf.github.io/fpdf2/Maths.html), [emojis, symbols & dingbats](https://pyfpdf.github.io/fpdf2/EmojisSymbolsDingbats.html)
  * [Tables](https://pyfpdf.github.io/fpdf2/Tables.html) and also [cell / multi-cell / plaintext writing](https://pyfpdf.github.io/fpdf2/Text.html), with [automatic page breaks](https://pyfpdf.github.io/fpdf2/PageBreaks.html), line break and text justification
  * Choice of measurement unit, page format & margins. Optional page header and footer
  * Basic [conversion from HTML to PDF](https://pyfpdf.github.io/fpdf2/HTML.html)
- * A [templating system](https://pyfpdf.github.io/fpdf2/Templates.html) to render PDFs in batchs
+ * A [templating system](https://pyfpdf.github.io/fpdf2/Templates.html) to render PDFs in batches
  * Images & links alternative descriptions, for accessibility
  * Table of contents & [document outline](https://pyfpdf.github.io/fpdf2/DocumentOutlineAndTableOfContents.html)
  * [Document encryption](https://pyfpdf.github.io/fpdf2/Encryption.html) & [document signing](https://pyfpdf.github.io/fpdf2/Signing.html)
  * [Annotations](https://pyfpdf.github.io/fpdf2/Annotations.html), including text highlights, and [file attachments](https://pyfpdf.github.io/fpdf2/FileAttachments.html)
  * [Presentation mode](https://pyfpdf.github.io/fpdf2/Presentations.html) with control over page display duration & transitions
  * Optional basic Markdown-like styling: `**bold**, __italics__`
  * Can render [mathematical equations & charts](https://pyfpdf.github.io/fpdf2/Maths.html)
@@ -100,15 +132,15 @@
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/PyFPDF/fpdf2&t=fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-facebook-1976D2?logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/PyFPDF/fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/PyFPDF/fpdf2&title=fpdf2)
 
 ## Documentation
 
 - [Documentation Home](https://pyfpdf.github.io/fpdf2/)
-- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html)
+- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html) - [ភាសខ្មែរ](https://pyfpdf.github.io/fpdf2/Tutorial-km.md) - [日本語](https://pyfpdf.github.io/fpdf2/Tutorial-ja.html)
 - Release notes: [CHANGELOG.md](https://github.com/PyFPDF/fpdf2/blob/master/CHANGELOG.md)
 - A series of blog posts: [fpdf2 tag @ ludochaordic](https://chezsoi.org/lucas/blog/tag/fpdf2.html)
 
 You can also have a look at the `tests/`, they're great usage examples!
 
 ## Developement
 
@@ -213,15 +245,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zenigata"><img src="https://avatars.githubusercontent.com/u/1022393?v=4?s=100" width="100px;" alt="Johan Bonneau"/><br /><sub><b>Johan Bonneau</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Zenigata" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jmunoz94"><img src="https://avatars.githubusercontent.com/u/48921408?v=4?s=100" width="100px;" alt="Jesús Alberto Muñoz Mesa"/><br /><sub><b>Jesús Alberto Muñoz Mesa</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Tests">⚠️</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jdeep.me"><img src="https://avatars.githubusercontent.com/u/64089730?v=4?s=100" width="100px;" alt="Jaydeep Das"/><br /><sub><b>Jaydeep Das</b></sub></a><br /><a href="#question-JDeepD" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/seanpmulholland"><img src="https://avatars.githubusercontent.com/u/79894395?v=4?s=100" width="100px;" alt="Sean"/><br /><sub><b>Sean</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=seanpmulholland" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Documentation">📖</a> <a href="#ideas-andersonhc" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/yiweelan"><img src="https://avatars.githubusercontent.com/u/117787188?v=4?s=100" width="100px;" alt="Yi Wei Lan"/><br /><sub><b>Yi Wei Lan</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=yiweelan" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bubbu0129"><img src="https://avatars.githubusercontent.com/u/93034081?v=4?s=100" width="100px;" alt="CpDong"/><br /><sub><b>CpDong</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Bubbu0129" title="Code">💻</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ABubbu0129" title="Bug reports">🐛</a> <a href="#translation-Bubbu0129" title="Translation">🌍</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/CY-Qiu"><img src="https://avatars.githubusercontent.com/u/23075447?v=4?s=100" width="100px;" alt="CY-Qiu"/><br /><sub><b>CY-Qiu</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ACY-Qiu" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Markovvn1"><img src="https://avatars.githubusercontent.com/u/32509100?v=4?s=100" width="100px;" alt="Markovvn1"/><br /><sub><b>Markovvn1</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Markovvn1" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/erap129"><img src="https://avatars.githubusercontent.com/u/30405025?v=4?s=100" width="100px;" alt="Elad Rapaport"/><br /><sub><b>Elad Rapaport</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=erap129" title="Code">💻</a></td>
@@ -234,14 +266,24 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruiz-manuel"><img src="https://avatars.githubusercontent.com/u/43274578?v=4?s=100" width="100px;" alt="Manuel Ruiz"/><br /><sub><b>Manuel Ruiz</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aruiz-manuel" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nsimonovici"><img src="https://avatars.githubusercontent.com/u/44460830?v=4?s=100" width="100px;" alt="Noel"/><br /><sub><b>Noel</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Ansimonovici" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a> <a href="#question-ssavi-ict" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aeris07"><img src="https://avatars.githubusercontent.com/u/129675592?v=4?s=100" width="100px;" alt="aeris07"/><br /><sub><b>aeris07</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aaeris07" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/KamarulAdha"><img src="https://avatars.githubusercontent.com/u/52944294?v=4?s=100" width="100px;" alt="KamarulAdha"/><br /><sub><b>KamarulAdha</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=KamarulAdha" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Valerus5685"><img src="https://avatars.githubusercontent.com/u/7953869?v=4?s=100" width="100px;" alt="Valerus5685"/><br /><sub><b>Valerus5685</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3AValerus5685" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sebastiantia"><img src="https://avatars.githubusercontent.com/u/75666019?v=4?s=100" width="100px;" alt="Sebastian Tia"/><br /><sub><b>Sebastian Tia</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=sebastiantia" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/1nv"><img src="https://avatars.githubusercontent.com/u/10288828?v=4?s=100" width="100px;" alt="Eugene Selifonov"/><br /><sub><b>Eugene Selifonov</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3A1nv" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://ez-startup.com"><img src="https://avatars.githubusercontent.com/u/69514175?v=4?s=100" width="100px;" alt="Kuth"/><br /><sub><b>Kuth</b></sub></a><br /><a href="#translation-kuth-chi" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://rdbr.nl"><img src="https://avatars.githubusercontent.com/u/34062862?v=4?s=100" width="100px;" alt="Ruben de Bruin"/><br /><sub><b>Ruben de Bruin</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ARubendeBruin" title="Bug reports">🐛</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=RubendeBruin" title="Code">💻</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=RubendeBruin" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/stenci"><img src="https://avatars.githubusercontent.com/u/5955495?v=4?s=100" width="100px;" alt="stenci"/><br /><sub><b>stenci</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Astenci" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alcnaka"><img src="https://avatars.githubusercontent.com/u/47954083?v=4?s=100" width="100px;" alt="alcnaka"/><br /><sub><b>alcnaka</b></sub></a><br /><a href="#translation-alcnaka" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tolker-KU"><img src="https://avatars.githubusercontent.com/u/55140581?v=4?s=100" width="100px;" alt="Tolker-KU"/><br /><sub><b>Tolker-KU</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Tolker-KU" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://lfavole.eu.pythonanywhere.com"><img src="https://avatars.githubusercontent.com/u/88188568?v=4?s=100" width="100px;" alt="lfavole"/><br /><sub><b>lfavole</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=lfavole" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `fpdf2-2.7.4/fpdf/__init__.py` & `fpdf2-2.7.5/fpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/actions.py` & `fpdf2-2.7.5/fpdf/actions.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/annotations.py` & `fpdf2-2.7.5/fpdf/annotations.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         self.type = Name("Annot")
         self.subtype = Name(subtype)
         self.rect = f"[{x:.2f} {y:.2f} {x + width:.2f} {y - height:.2f}]"
         self.border = f"[0 0 {border_width}]"
         self.f_t = Name(field_type) if field_type else None
         self.v = value
         self.f = sum(flags)
-        self.contents = PDFString(contents) if contents else None
+        self.contents = PDFString(contents, encrypt=True) if contents else None
         self.a = action
         self.dest = dest
         self.c = f"[{color[0]} {color[1]} {color[2]}]" if color else None
-        self.t = PDFString(title) if title else None
-        self.m = PDFDate(modification_time) if modification_time else None
+        self.t = PDFString(title, encrypt=True) if title else None
+        self.m = PDFDate(modification_time, encrypt=True) if modification_time else None
         self.quad_points = (
             pdf_list(f"{quad_point:.2f}" for quad_point in quad_points)
             if quad_points
             else None
         )
         self.p = None  # must always be set before calling .serialize()
         self.name = name
```

### Comparing `fpdf2-2.7.4/fpdf/drawing.py` & `fpdf2-2.7.5/fpdf/drawing.py`

 * *Files 1% similar despite different names*

```diff
@@ -4686,4575 +4686,4554 @@
 000124d0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
 000124e0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
 000124f0: 2074 7570 6c65 206f 6620 6028 7374 722c   tuple of `(str,
 00012500: 206e 6577 5f6c 6173 745f 6974 656d 2960   new_last_item)`
 00012510: 2c20 7768 6572 6520 606e 6577 5f6c 6173  , where `new_las
 00012520: 745f 6974 656d 6020 6973 2060 7365 6c66  t_item` is `self
 00012530: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
-00012540: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
-00012550: 2064 6973 6162 6c65 3d75 6e75 7365 642d   disable=unused-
-00012560: 6172 6775 6d65 6e74 0a20 2020 2020 2020  argument.       
-00012570: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-00012580: 2020 2020 2020 7365 6c66 2e74 6f5f 6375        self.to_cu
-00012590: 6269 635f 6375 7276 6528 6c61 7374 5f69  bic_curve(last_i
-000125a0: 7465 6d2e 656e 645f 706f 696e 7429 2e72  tem.end_point).r
-000125b0: 656e 6465 7228 0a20 2020 2020 2020 2020  ender(.         
-000125c0: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
-000125d0: 7472 792c 2073 7479 6c65 2c20 6c61 7374  try, style, last
-000125e0: 5f69 7465 6d2c 2069 6e69 7469 616c 5f70  _item, initial_p
-000125f0: 6f69 6e74 0a20 2020 2020 2020 2020 2020  oint.           
-00012600: 2029 5b30 5d2c 0a20 2020 2020 2020 2020   )[0],.         
-00012610: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00012620: 2020 2020 2069 6e69 7469 616c 5f70 6f69       initial_poi
-00012630: 6e74 2c0a 2020 2020 2020 2020 290a 0a20  nt,.        ).. 
-00012640: 2020 2040 666f 7263 655f 6e6f 646f 6375     @force_nodocu
-00012650: 6d65 6e74 0a20 2020 2064 6566 2072 656e  ment.    def ren
-00012660: 6465 725f 6465 6275 6728 0a20 2020 2020  der_debug(.     
-00012670: 2020 2073 656c 662c 2067 7364 5f72 6567     self, gsd_reg
-00012680: 6973 7472 792c 2073 7479 6c65 2c20 6c61  istry, style, la
-00012690: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
-000126a0: 5f70 6f69 6e74 2c20 6465 6275 675f 7374  _point, debug_st
-000126b0: 7265 616d 2c20 7066 780a 2020 2020 293a  ream, pfx.    ):
-000126c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000126d0: 2020 2020 2052 656e 6465 7220 7468 6973       Render this
-000126e0: 2070 6174 6820 656c 656d 656e 7420 746f   path element to
-000126f0: 2069 7473 2050 4446 2072 6570 7265 7365   its PDF represe
-00012700: 6e74 6174 696f 6e20 616e 6420 7072 6f64  ntation and prod
-00012710: 7563 6520 6465 6275 670a 2020 2020 2020  uce debug.      
-00012720: 2020 696e 666f 726d 6174 696f 6e2e 0a0a    information...
-00012730: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00012740: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-00012750: 6769 7374 7279 2028 4772 6170 6869 6373  gistry (Graphics
-00012760: 5374 6174 6544 6963 7452 6567 6973 7472  StateDictRegistr
-00012770: 7929 3a20 7468 6520 6f77 6e65 7227 7320  y): the owner's 
-00012780: 6772 6170 6869 6373 2073 7461 7465 0a20  graphics state. 
-00012790: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000127a0: 6963 7469 6f6e 6172 7920 7265 6769 7374  ictionary regist
-000127b0: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
-000127c0: 7374 796c 6520 2847 7261 7068 6963 7353  style (GraphicsS
-000127d0: 7479 6c65 293a 2074 6865 2063 7572 7265  tyle): the curre
-000127e0: 6e74 2072 6573 6f6c 7665 6420 6772 6170  nt resolved grap
-000127f0: 6869 6373 2073 7479 6c65 0a20 2020 2020  hics style.     
-00012800: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
-00012810: 3a20 7468 6520 7072 6576 696f 7573 2070  : the previous p
-00012820: 6174 6820 656c 656d 656e 742e 0a20 2020  ath element..   
-00012830: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
-00012840: 5f70 6f69 6e74 3a20 6c61 7374 2070 6f73  _point: last pos
-00012850: 6974 696f 6e20 7365 7420 6279 2061 2022  ition set by a "
-00012860: 4d22 206f 7220 226d 2220 636f 6d6d 616e  M" or "m" comman
-00012870: 640a 2020 2020 2020 2020 2020 2020 6465  d.            de
-00012880: 6275 675f 7374 7265 616d 2028 696f 2e54  bug_stream (io.T
-00012890: 6578 7449 4f29 3a20 7468 6520 7374 7265  extIO): the stre
-000128a0: 616d 2074 6f20 7768 6963 6820 7468 6520  am to which the 
-000128b0: 6465 6275 6720 6f75 7470 7574 2073 686f  debug output sho
-000128c0: 756c 6420 6265 0a20 2020 2020 2020 2020  uld be.         
-000128d0: 2020 2020 2020 2077 7269 7474 656e 2e20         written. 
-000128e0: 5468 6973 2069 7320 6e6f 7420 6775 6172  This is not guar
-000128f0: 616e 7465 6564 2074 6f20 6265 2073 6565  anteed to be see
-00012900: 6b61 626c 6520 2865 2e67 2e20 6974 206d  kable (e.g. it m
-00012910: 6179 2062 6520 7374 646f 7574 206f 720a  ay be stdout or.
-00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012930: 7374 6465 7272 292e 0a20 2020 2020 2020  stderr)..       
-00012940: 2020 2020 2070 6678 2028 7374 7229 3a20       pfx (str): 
-00012950: 7468 6520 6375 7272 656e 7420 6465 6275  the current debu
-00012960: 6720 6f75 7470 7574 2070 7265 6669 7820  g output prefix 
-00012970: 7374 7269 6e67 2028 6f6e 6c79 206e 6565  string (only nee
-00012980: 6465 6420 6966 2065 6d69 7474 696e 670a  ded if emitting.
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 6d6f 7265 2074 6861 6e20 6f6e 6520 6c69  more than one li
-000129b0: 6e65 292e 0a0a 2020 2020 2020 2020 5265  ne)...        Re
-000129c0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-000129d0: 2020 2054 6865 2073 616d 6520 7475 706c     The same tupl
-000129e0: 6520 6173 2060 5175 6164 7261 7469 6342  e as `QuadraticB
-000129f0: 657a 6965 7243 7572 7665 2e72 656e 6465  ezierCurve.rende
-00012a00: 7260 2e0a 2020 2020 2020 2020 2222 220a  r`..        """.
-00012a10: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
-00012a20: 3a20 6469 7361 626c 653d 756e 7573 6564  : disable=unused
-00012a30: 2d61 7267 756d 656e 740a 2020 2020 2020  -argument.      
-00012a40: 2020 7265 6e64 6572 6564 2c20 7265 736f    rendered, reso
-00012a50: 6c76 6564 2c20 696e 6974 6961 6c5f 706f  lved, initial_po
-00012a60: 696e 7420 3d20 7365 6c66 2e72 656e 6465  int = self.rende
-00012a70: 7228 0a20 2020 2020 2020 2020 2020 2067  r(.            g
-00012a80: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
-00012a90: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
-00012aa0: 6e69 7469 616c 5f70 6f69 6e74 0a20 2020  nitial_point.   
-00012ab0: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
-00012ac0: 6562 7567 5f73 7472 6561 6d2e 7772 6974  ebug_stream.writ
-00012ad0: 6528 0a20 2020 2020 2020 2020 2020 2066  e(.            f
-00012ae0: 227b 7365 6c66 7d20 7265 736f 6c76 6564  "{self} resolved
-00012af0: 2074 6f20 7b73 656c 662e 746f 5f63 7562   to {self.to_cub
-00012b00: 6963 5f63 7572 7665 286c 6173 745f 6974  ic_curve(last_it
-00012b10: 656d 2e65 6e64 5f70 6f69 6e74 297d 5c6e  em.end_point)}\n
-00012b20: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
-00012b30: 2020 2020 2072 6574 7572 6e20 7265 6e64       return rend
-00012b40: 6572 6564 2c20 7265 736f 6c76 6564 2c20  ered, resolved, 
-00012b50: 696e 6974 6961 6c5f 706f 696e 740a 0a0a  initial_point...
-00012b60: 636c 6173 7320 5265 6c61 7469 7665 5175  class RelativeQu
-00012b70: 6164 7261 7469 6342 657a 6965 7243 7572  adraticBezierCur
-00012b80: 7665 284e 616d 6564 5475 706c 6529 3a0a  ve(NamedTuple):.
-00012b90: 2020 2020 2222 220a 2020 2020 4120 7175      """.    A qu
-00012ba0: 6164 7261 7469 6320 42c3 a97a 6965 7220  adratic B..zier 
-00012bb0: 6375 7276 6520 7061 7468 2065 6c65 6d65  curve path eleme
-00012bc0: 6e74 2077 686f 7365 2070 6f69 6e74 7320  nt whose points 
-00012bd0: 6172 6520 7370 6563 6966 6965 6420 7265  are specified re
-00012be0: 6c61 7469 7665 2074 6f20 7468 6520 656e  lative to the en
-00012bf0: 640a 2020 2020 706f 696e 7420 6f66 2074  d.    point of t
-00012c00: 6865 2070 7265 7669 6f75 7320 7061 7468  he previous path
-00012c10: 2065 6c65 6d65 6e74 2e0a 0a20 2020 2053   element...    S
-00012c20: 6565 3a20 6050 6169 6e74 6564 5061 7468  ee: `PaintedPath
-00012c30: 2e71 7561 6472 6174 6963 5f63 7572 7665  .quadratic_curve
-00012c40: 5f72 656c 6174 6976 6560 0a20 2020 2022  _relative`.    "
-00012c50: 2222 0a0a 2020 2020 6374 726c 3a20 506f  ""..    ctrl: Po
-00012c60: 696e 740a 2020 2020 2222 2254 6865 2063  int.    """The c
-00012c70: 7572 7665 2773 2063 6f6e 7472 6f6c 2070  urve's control p
-00012c80: 6f69 6e74 2072 656c 6174 6976 6520 746f  oint relative to
-00012c90: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
-00012ca0: 7072 6576 696f 7573 2070 6174 6820 656c  previous path el
-00012cb0: 656d 656e 742e 2222 220a 2020 2020 656e  ement.""".    en
-00012cc0: 643a 2050 6f69 6e74 0a20 2020 2022 2222  d: Point.    """
-00012cd0: 5468 6520 6375 7276 6527 7320 656e 6420  The curve's end 
-00012ce0: 706f 696e 7420 7265 6c61 7469 7665 2074  point relative t
-00012cf0: 6f20 7468 6520 656e 6420 6f66 2074 6865  o the end of the
-00012d00: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
-00012d10: 6c65 6d65 6e74 2e22 2222 0a0a 2020 2020  lement."""..    
-00012d20: 4066 6f72 6365 5f6e 6f64 6f63 756d 656e  @force_nodocumen
-00012d30: 740a 2020 2020 6465 6620 7265 6e64 6572  t.    def render
-00012d40: 2873 656c 662c 2067 7364 5f72 6567 6973  (self, gsd_regis
-00012d50: 7472 792c 2073 7479 6c65 2c20 6c61 7374  try, style, last
-00012d60: 5f69 7465 6d2c 2069 6e69 7469 616c 5f70  _item, initial_p
-00012d70: 6f69 6e74 293a 0a20 2020 2020 2020 2022  oint):.        "
-00012d80: 2222 0a20 2020 2020 2020 2052 656e 6465  "".        Rende
-00012d90: 7220 7468 6973 2070 6174 6820 656c 656d  r this path elem
-00012da0: 656e 7420 746f 2069 7473 2050 4446 2072  ent to its PDF r
-00012db0: 6570 7265 7365 6e74 6174 696f 6e2e 0a0a  epresentation...
-00012dc0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00012dd0: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-00012de0: 6769 7374 7279 2028 4772 6170 6869 6373  gistry (Graphics
-00012df0: 5374 6174 6544 6963 7452 6567 6973 7472  StateDictRegistr
-00012e00: 7929 3a20 7468 6520 6f77 6e65 7227 7320  y): the owner's 
-00012e10: 6772 6170 6869 6373 2073 7461 7465 0a20  graphics state. 
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00012e30: 6963 7469 6f6e 6172 7920 7265 6769 7374  ictionary regist
-00012e40: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
-00012e50: 7374 796c 6520 2847 7261 7068 6963 7353  style (GraphicsS
-00012e60: 7479 6c65 293a 2074 6865 2063 7572 7265  tyle): the curre
-00012e70: 6e74 2072 6573 6f6c 7665 6420 6772 6170  nt resolved grap
-00012e80: 6869 6373 2073 7479 6c65 0a20 2020 2020  hics style.     
-00012e90: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
-00012ea0: 3a20 7468 6520 7072 6576 696f 7573 2070  : the previous p
-00012eb0: 6174 6820 656c 656d 656e 742e 0a20 2020  ath element..   
-00012ec0: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
-00012ed0: 5f70 6f69 6e74 3a20 6c61 7374 2070 6f73  _point: last pos
-00012ee0: 6974 696f 6e20 7365 7420 6279 2061 2022  ition set by a "
-00012ef0: 4d22 206f 7220 226d 2220 636f 6d6d 616e  M" or "m" comman
-00012f00: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
-00012f10: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00012f20: 6120 7475 706c 6520 6f66 2060 2873 7472  a tuple of `(str
-00012f30: 2c20 6e65 775f 6c61 7374 5f69 7465 6d29  , new_last_item)
-00012f40: 602c 2077 6865 7265 2060 6e65 775f 6c61  `, where `new_la
-00012f50: 7374 5f69 7465 6d60 2069 7320 7468 6520  st_item` is the 
-00012f60: 7265 736f 6c76 6564 0a20 2020 2020 2020  resolved.       
-00012f70: 2020 2020 2060 5175 6164 7261 7469 6342       `QuadraticB
-00012f80: 657a 6965 7243 7572 7665 602e 0a20 2020  ezierCurve`..   
-00012f90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012fa0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-00012fb0: 6c65 3d75 6e75 7365 642d 6172 6775 6d65  le=unused-argume
-00012fc0: 6e74 0a20 2020 2020 2020 206c 6173 745f  nt.        last_
-00012fd0: 706f 696e 7420 3d20 6c61 7374 5f69 7465  point = last_ite
-00012fe0: 6d2e 656e 645f 706f 696e 740a 0a20 2020  m.end_point..   
-00012ff0: 2020 2020 2063 7472 6c20 3d20 6c61 7374       ctrl = last
-00013000: 5f70 6f69 6e74 202b 2073 656c 662e 6374  _point + self.ct
-00013010: 726c 0a20 2020 2020 2020 2065 6e64 203d  rl.        end =
-00013020: 206c 6173 745f 706f 696e 7420 2b20 7365   last_point + se
-00013030: 6c66 2e65 6e64 0a0a 2020 2020 2020 2020  lf.end..        
-00013040: 6162 736f 6c75 7465 203d 2051 7561 6472  absolute = Quadr
-00013050: 6174 6963 4265 7a69 6572 4375 7276 6528  aticBezierCurve(
-00013060: 6374 726c 3d63 7472 6c2c 2065 6e64 3d65  ctrl=ctrl, end=e
-00013070: 6e64 290a 2020 2020 2020 2020 7265 7475  nd).        retu
-00013080: 726e 2061 6273 6f6c 7574 652e 7265 6e64  rn absolute.rend
-00013090: 6572 2867 7364 5f72 6567 6973 7472 792c  er(gsd_registry,
-000130a0: 2073 7479 6c65 2c20 6c61 7374 5f69 7465   style, last_ite
-000130b0: 6d2c 2069 6e69 7469 616c 5f70 6f69 6e74  m, initial_point
-000130c0: 290a 0a20 2020 2040 666f 7263 655f 6e6f  )..    @force_no
-000130d0: 646f 6375 6d65 6e74 0a20 2020 2064 6566  document.    def
-000130e0: 2072 656e 6465 725f 6465 6275 6728 0a20   render_debug(. 
-000130f0: 2020 2020 2020 2073 656c 662c 2067 7364         self, gsd
-00013100: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
-00013110: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
-00013120: 7469 616c 5f70 6f69 6e74 2c20 6465 6275  tial_point, debu
-00013130: 675f 7374 7265 616d 2c20 7066 780a 2020  g_stream, pfx.  
-00013140: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-00013150: 0a20 2020 2020 2020 2052 656e 6465 7220  .        Render 
-00013160: 7468 6973 2070 6174 6820 656c 656d 656e  this path elemen
-00013170: 7420 746f 2069 7473 2050 4446 2072 6570  t to its PDF rep
-00013180: 7265 7365 6e74 6174 696f 6e20 616e 6420  resentation and 
-00013190: 7072 6f64 7563 6520 6465 6275 670a 2020  produce debug.  
-000131a0: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
-000131b0: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
-000131c0: 3a0a 2020 2020 2020 2020 2020 2020 6773  :.            gs
-000131d0: 645f 7265 6769 7374 7279 2028 4772 6170  d_registry (Grap
-000131e0: 6869 6373 5374 6174 6544 6963 7452 6567  hicsStateDictReg
-000131f0: 6973 7472 7929 3a20 7468 6520 6f77 6e65  istry): the owne
-00013200: 7227 7320 6772 6170 6869 6373 2073 7461  r's graphics sta
-00013210: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
-00013220: 2020 2064 6963 7469 6f6e 6172 7920 7265     dictionary re
-00013230: 6769 7374 7279 2e0a 2020 2020 2020 2020  gistry..        
-00013240: 2020 2020 7374 796c 6520 2847 7261 7068      style (Graph
-00013250: 6963 7353 7479 6c65 293a 2074 6865 2063  icsStyle): the c
-00013260: 7572 7265 6e74 2072 6573 6f6c 7665 6420  urrent resolved 
-00013270: 6772 6170 6869 6373 2073 7479 6c65 0a20  graphics style. 
-00013280: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-00013290: 6974 656d 3a20 7468 6520 7072 6576 696f  item: the previo
-000132a0: 7573 2070 6174 6820 656c 656d 656e 742e  us path element.
-000132b0: 0a20 2020 2020 2020 2020 2020 2069 6e69  .            ini
-000132c0: 7469 616c 5f70 6f69 6e74 3a20 6c61 7374  tial_point: last
-000132d0: 2070 6f73 6974 696f 6e20 7365 7420 6279   position set by
-000132e0: 2061 2022 4d22 206f 7220 226d 2220 636f   a "M" or "m" co
-000132f0: 6d6d 616e 640a 2020 2020 2020 2020 2020  mmand.          
-00013300: 2020 6465 6275 675f 7374 7265 616d 2028    debug_stream (
-00013310: 696f 2e54 6578 7449 4f29 3a20 7468 6520  io.TextIO): the 
-00013320: 7374 7265 616d 2074 6f20 7768 6963 6820  stream to which 
-00013330: 7468 6520 6465 6275 6720 6f75 7470 7574  the debug output
-00013340: 2073 686f 756c 6420 6265 0a20 2020 2020   should be.     
-00013350: 2020 2020 2020 2020 2020 2077 7269 7474             writt
-00013360: 656e 2e20 5468 6973 2069 7320 6e6f 7420  en. This is not 
-00013370: 6775 6172 616e 7465 6564 2074 6f20 6265  guaranteed to be
-00013380: 2073 6565 6b61 626c 6520 2865 2e67 2e20   seekable (e.g. 
-00013390: 6974 206d 6179 2062 6520 7374 646f 7574  it may be stdout
-000133a0: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-000133b0: 2020 2020 7374 6465 7272 292e 0a20 2020      stderr)..   
-000133c0: 2020 2020 2020 2020 2070 6678 2028 7374           pfx (st
-000133d0: 7229 3a20 7468 6520 6375 7272 656e 7420  r): the current 
-000133e0: 6465 6275 6720 6f75 7470 7574 2070 7265  debug output pre
-000133f0: 6669 7820 7374 7269 6e67 2028 6f6e 6c79  fix string (only
-00013400: 206e 6565 6465 6420 6966 2065 6d69 7474   needed if emitt
-00013410: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00013420: 2020 2020 6d6f 7265 2074 6861 6e20 6f6e      more than on
-00013430: 6520 6c69 6e65 292e 0a0a 2020 2020 2020  e line)...      
-00013440: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00013450: 2020 2020 2020 2054 6865 2073 616d 6520         The same 
-00013460: 7475 706c 6520 6173 2060 5265 6c61 7469  tuple as `Relati
-00013470: 7665 5175 6164 7261 7469 6342 657a 6965  veQuadraticBezie
-00013480: 7243 7572 7665 2e72 656e 6465 7260 2e0a  rCurve.render`..
-00013490: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000134a0: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-000134b0: 7361 626c 653d 756e 7573 6564 2d61 7267  sable=unused-arg
-000134c0: 756d 656e 740a 2020 2020 2020 2020 7265  ument.        re
-000134d0: 6e64 6572 6564 2c20 7265 736f 6c76 6564  ndered, resolved
-000134e0: 2c20 696e 6974 6961 6c5f 706f 696e 7420  , initial_point 
-000134f0: 3d20 7365 6c66 2e72 656e 6465 7228 0a20  = self.render(. 
-00013500: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
-00013510: 6567 6973 7472 792c 2073 7479 6c65 2c20  egistry, style, 
-00013520: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
-00013530: 616c 5f70 6f69 6e74 0a20 2020 2020 2020  al_point.       
-00013540: 2029 0a20 2020 2020 2020 2064 6562 7567   ).        debug
-00013550: 5f73 7472 6561 6d2e 7772 6974 6528 0a20  _stream.write(. 
-00013560: 2020 2020 2020 2020 2020 2066 227b 7365             f"{se
-00013570: 6c66 7d20 7265 736f 6c76 6564 2074 6f20  lf} resolved to 
-00013580: 7b72 6573 6f6c 7665 647d 2022 0a20 2020  {resolved} ".   
-00013590: 2020 2020 2020 2020 2066 2274 6865 6e20           f"then 
-000135a0: 746f 207b 7265 736f 6c76 6564 2e74 6f5f  to {resolved.to_
-000135b0: 6375 6269 635f 6375 7276 6528 6c61 7374  cubic_curve(last
-000135c0: 5f69 7465 6d2e 656e 645f 706f 696e 7429  _item.end_point)
-000135d0: 7d5c 6e22 0a20 2020 2020 2020 2029 0a0a  }\n".        )..
-000135e0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000135f0: 656e 6465 7265 642c 2072 6573 6f6c 7665  endered, resolve
-00013600: 642c 2069 6e69 7469 616c 5f70 6f69 6e74  d, initial_point
-00013610: 0a0a 0a63 6c61 7373 2041 7263 284e 616d  ...class Arc(Nam
-00013620: 6564 5475 706c 6529 3a0a 2020 2020 2222  edTuple):.    ""
-00013630: 220a 2020 2020 416e 2065 6c6c 6970 7469  ".    An ellipti
-00013640: 6361 6c20 6172 6320 7061 7468 2065 6c65  cal arc path ele
-00013650: 6d65 6e74 2e0a 0a20 2020 2054 6865 2061  ment...    The a
-00013660: 7263 2069 7320 6472 6177 6e20 6672 6f6d  rc is drawn from
-00013670: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
-00013680: 6375 7272 656e 7420 7061 7468 2065 6c65  current path ele
-00013690: 6d65 6e74 2074 6f20 6974 7320 7370 6563  ment to its spec
-000136a0: 6966 6965 6420 656e 6420 706f 696e 740a  ified end point.
-000136b0: 2020 2020 7573 696e 6720 6120 6e75 6d62      using a numb
-000136c0: 6572 206f 6620 7061 7261 6d65 7465 7273  er of parameters
-000136d0: 2074 6f20 6465 7465 726d 696e 6520 686f   to determine ho
-000136e0: 7720 6974 2069 7320 636f 6e73 7472 7563  w it is construc
-000136f0: 7465 642e 0a0a 2020 2020 5365 653a 2060  ted...    See: `
-00013700: 5061 696e 7465 6450 6174 682e 6172 635f  PaintedPath.arc_
-00013710: 746f 600a 2020 2020 2222 220a 0a20 2020  to`.    """..   
-00013720: 2072 6164 6969 3a20 506f 696e 740a 2020   radii: Point.  
-00013730: 2020 2222 220a 2020 2020 5468 6520 782d    """.    The x-
-00013740: 2061 6e64 2079 2d72 6164 6969 206f 6620   and y-radii of 
-00013750: 7468 6520 6172 632e 2049 6620 6072 6164  the arc. If `rad
-00013760: 6969 2e78 203d 3d20 7261 6469 692e 7960  ii.x == radii.y`
-00013770: 2074 6865 2061 7263 2077 696c 6c20 6265   the arc will be
-00013780: 2063 6972 6375 6c61 722e 0a20 2020 2022   circular..    "
-00013790: 2222 0a20 2020 2072 6f74 6174 696f 6e3a  "".    rotation:
-000137a0: 204e 756d 6265 720a 2020 2020 2222 2254   Number.    """T
-000137b0: 6865 2072 6f74 6174 696f 6e20 6f66 2074  he rotation of t
-000137c0: 6865 2061 7263 2773 206d 616a 6f72 2f6d  he arc's major/m
-000137d0: 696e 6f72 2061 7865 7320 7265 6c61 7469  inor axes relati
-000137e0: 7665 2074 6f20 7468 6520 636f 6f72 6469  ve to the coordi
-000137f0: 6e61 7465 2066 7261 6d65 2e22 2222 0a20  nate frame.""". 
-00013800: 2020 206c 6172 6765 3a20 626f 6f6c 0a20     large: bool. 
-00013810: 2020 2022 2222 4966 2054 7275 652c 2073     """If True, s
-00013820: 7765 6570 2074 6865 2061 7263 206f 7665  weep the arc ove
-00013830: 7220 616e 2061 6e67 6c65 2067 7265 6174  r an angle great
-00013840: 6572 2074 6861 6e20 6f72 2065 7175 616c  er than or equal
-00013850: 2074 6f20 3138 3020 6465 6772 6565 732e   to 180 degrees.
-00013860: 2222 220a 2020 2020 7377 6565 703a 2062  """.    sweep: b
-00013870: 6f6f 6c0a 2020 2020 2222 2249 6620 5472  ool.    """If Tr
-00013880: 7565 2c20 7468 6520 6172 6320 6973 2073  ue, the arc is s
-00013890: 7765 7074 2069 6e20 7468 6520 706f 7369  wept in the posi
-000138a0: 7469 7665 2061 6e67 756c 6172 2064 6972  tive angular dir
-000138b0: 6563 7469 6f6e 2e22 2222 0a20 2020 2065  ection.""".    e
-000138c0: 6e64 3a20 506f 696e 740a 2020 2020 2222  nd: Point.    ""
-000138d0: 2254 6865 2065 6e64 2070 6f69 6e74 206f  "The end point o
-000138e0: 6620 7468 6520 6172 632e 2222 220a 0a20  f the arc.""".. 
-000138f0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00013900: 0a20 2020 2040 666f 7263 655f 6e6f 646f  .    @force_nodo
-00013910: 6375 6d65 6e74 0a20 2020 2064 6566 2073  cument.    def s
-00013920: 7562 6469 7664 655f 7377 6565 7028 7377  ubdivde_sweep(sw
-00013930: 6565 705f 616e 676c 6529 3a0a 2020 2020  eep_angle):.    
-00013940: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013950: 4120 6765 6e65 7261 746f 7220 7468 6174  A generator that
-00013960: 2073 7562 6469 7669 6465 7320 6120 7377   subdivides a sw
-00013970: 6570 7420 616e 676c 6520 696e 746f 2073  ept angle into s
-00013980: 6567 6d65 6e74 7320 6e6f 206c 6172 6765  egments no large
-00013990: 7220 7468 616e 2061 2071 7561 7274 6572  r than a quarter
-000139a0: 0a20 2020 2020 2020 2074 7572 6e2e 0a0a  .        turn...
-000139b0: 2020 2020 2020 2020 416e 7920 7377 6565          Any swee
-000139c0: 7020 7468 6174 2069 7320 6c61 7267 6572  p that is larger
-000139d0: 2074 6861 6e20 6120 7175 6172 7465 7220   than a quarter 
-000139e0: 7475 726e 2069 7320 7375 6264 6976 6964  turn is subdivid
-000139f0: 6564 2069 6e74 6f20 6173 206d 616e 7920  ed into as many 
-00013a00: 6571 7561 6c6c 790a 2020 2020 2020 2020  equally.        
-00013a10: 7369 7a65 6420 7365 676d 656e 7473 2061  sized segments a
-00013a20: 7320 6e65 6365 7373 6172 7920 746f 2070  s necessary to p
-00013a30: 7265 7665 6e74 2061 6e79 2069 6e64 6976  revent any indiv
-00013a40: 6964 7561 6c20 7365 676d 656e 7420 6672  idual segment fr
-00013a50: 6f6d 2062 6569 6e67 206c 6172 6765 720a  om being larger.
-00013a60: 2020 2020 2020 2020 7468 616e 2061 2071          than a q
-00013a70: 7561 7274 6572 2074 7572 6e2e 0a0a 2020  uarter turn...  
-00013a80: 2020 2020 2020 5468 6973 2069 7320 7573        This is us
-00013a90: 6564 2066 6f72 2061 7070 726f 7869 6d61  ed for approxima
-00013aa0: 7469 6e67 2061 2063 6972 6375 6c61 7220  ting a circular 
-00013ab0: 6375 7276 6520 7365 676d 656e 7420 7573  curve segment us
-00013ac0: 696e 6720 6375 6269 6320 42c3 a97a 6965  ing cubic B..zie
-00013ad0: 720a 2020 2020 2020 2020 6375 7276 6573  r.        curves
-00013ae0: 2e20 5468 6973 2063 6f6d 7075 7465 7320  . This computes 
-00013af0: 7468 6520 7061 7261 6d65 7465 7273 2075  the parameters u
-00013b00: 7365 6420 666f 7220 7468 6520 42c3 a97a  sed for the B..z
-00013b10: 6965 7220 6170 7072 6f78 696d 6174 696f  ier approximatio
-00013b20: 6e20 7570 0a20 2020 2020 2020 2066 726f  n up.        fro
-00013b30: 6e74 2c20 6173 2077 656c 6c20 6173 2074  nt, as well as t
-00013b40: 6865 2074 7261 6e73 666f 726d 206e 6563  he transform nec
-00013b50: 6573 7361 7279 2074 6f20 706c 6163 6520  essary to place 
-00013b60: 7468 6520 7365 676d 656e 7420 696e 2074  the segment in t
-00013b70: 6865 2063 6f72 7265 6374 0a20 2020 2020  he correct.     
-00013b80: 2020 2070 6f73 6974 696f 6e2e 0a0a 2020     position...  
-00013b90: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00013ba0: 2020 2020 2020 2020 7377 6565 705f 616e          sweep_an
-00013bb0: 676c 6520 284e 756d 6265 7229 3a20 7468  gle (Number): th
-00013bc0: 6520 616e 676c 6520 746f 2073 7562 6469  e angle to subdi
-00013bd0: 7669 6465 2e0a 0a20 2020 2020 2020 2059  vide...        Y
-00013be0: 6965 6c64 733a 0a20 2020 2020 2020 2020  ields:.         
-00013bf0: 2020 2041 2074 7570 6c65 206f 6620 2863     A tuple of (c
-00013c00: 7472 6c31 2c20 6374 726c 322c 2065 6e64  trl1, ctrl2, end
-00013c10: 2920 7265 7072 6573 656e 7469 6e67 2074  ) representing t
-00013c20: 6865 2063 6f6e 7472 6f6c 2061 6e64 2065  he control and e
-00013c30: 6e64 2070 6f69 6e74 7320 6f66 0a20 2020  nd points of.   
-00013c40: 2020 2020 2020 2020 2074 6865 2063 7562           the cub
-00013c50: 6963 2042 c3a9 7a69 6572 2063 7572 7665  ic B..zier curve
-00013c60: 2061 7070 726f 7869 6d61 7469 6e67 2074   approximating t
-00013c70: 6865 2073 6567 6d65 6e74 2061 7320 6120  he segment as a 
-00013c80: 756e 6974 2063 6972 636c 6520 6365 6e74  unit circle cent
-00013c90: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
-00013ca0: 2061 7420 7468 6520 6f72 6967 696e 2e0a   at the origin..
-00013cb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013cc0: 2020 2020 7377 6565 705f 616e 676c 6520      sweep_angle 
-00013cd0: 3d20 6162 7328 7377 6565 705f 616e 676c  = abs(sweep_angl
-00013ce0: 6529 0a20 2020 2020 2020 2073 7765 6570  e).        sweep
-00013cf0: 5f6c 6566 7420 3d20 7377 6565 705f 616e  _left = sweep_an
-00013d00: 676c 650a 0a20 2020 2020 2020 2071 7561  gle..        qua
-00013d10: 7274 6572 7475 726e 203d 206d 6174 682e  rterturn = math.
-00013d20: 7069 202f 2032 0a20 2020 2020 2020 2063  pi / 2.        c
-00013d30: 6875 6e6b 7320 3d20 6d61 7468 2e63 6569  hunks = math.cei
-00013d40: 6c28 7377 6565 705f 616e 676c 6520 2f20  l(sweep_angle / 
-00013d50: 7175 6172 7465 7274 7572 6e29 0a0a 2020  quarterturn)..  
-00013d60: 2020 2020 2020 7377 6565 705f 7365 676d        sweep_segm
-00013d70: 656e 7420 3d20 7377 6565 705f 616e 676c  ent = sweep_angl
-00013d80: 6520 2f20 6368 756e 6b73 0a20 2020 2020  e / chunks.     
-00013d90: 2020 2063 6f73 5f74 203d 206d 6174 682e     cos_t = math.
-00013da0: 636f 7328 7377 6565 705f 7365 676d 656e  cos(sweep_segmen
-00013db0: 7429 0a20 2020 2020 2020 2073 696e 5f74  t).        sin_t
-00013dc0: 203d 206d 6174 682e 7369 6e28 7377 6565   = math.sin(swee
-00013dd0: 705f 7365 676d 656e 7429 0a20 2020 2020  p_segment).     
-00013de0: 2020 206b 6170 7061 203d 2034 202f 2033     kappa = 4 / 3
-00013df0: 202a 206d 6174 682e 7461 6e28 7377 6565   * math.tan(swee
-00013e00: 705f 7365 676d 656e 7420 2f20 3429 0a0a  p_segment / 4)..
-00013e10: 2020 2020 2020 2020 6374 726c 3120 3d20          ctrl1 = 
-00013e20: 506f 696e 7428 312c 206b 6170 7061 290a  Point(1, kappa).
-00013e30: 2020 2020 2020 2020 6374 726c 3220 3d20          ctrl2 = 
-00013e40: 506f 696e 7428 636f 735f 7420 2b20 6b61  Point(cos_t + ka
-00013e50: 7070 6120 2a20 7369 6e5f 742c 2073 696e  ppa * sin_t, sin
-00013e60: 5f74 202d 206b 6170 7061 202a 2063 6f73  _t - kappa * cos
-00013e70: 5f74 290a 2020 2020 2020 2020 656e 6420  _t).        end 
-00013e80: 3d20 506f 696e 7428 636f 735f 742c 2073  = Point(cos_t, s
-00013e90: 696e 5f74 290a 0a20 2020 2020 2020 2066  in_t)..        f
-00013ea0: 6f72 205f 2069 6e20 7261 6e67 6528 6368  or _ in range(ch
-00013eb0: 756e 6b73 293a 0a20 2020 2020 2020 2020  unks):.         
-00013ec0: 2020 206f 6666 7365 7420 3d20 7377 6565     offset = swee
-00013ed0: 705f 616e 676c 6520 2d20 7377 6565 705f  p_angle - sweep_
-00013ee0: 6c65 6674 0a0a 2020 2020 2020 2020 2020  left..          
-00013ef0: 2020 7472 616e 7366 6f72 6d20 3d20 5472    transform = Tr
-00013f00: 616e 7366 6f72 6d2e 726f 7461 7469 6f6e  ansform.rotation
-00013f10: 286f 6666 7365 7429 0a20 2020 2020 2020  (offset).       
-00013f20: 2020 2020 2079 6965 6c64 2063 7472 6c31       yield ctrl1
-00013f30: 2040 2074 7261 6e73 666f 726d 2c20 6374   @ transform, ct
-00013f40: 726c 3220 4020 7472 616e 7366 6f72 6d2c  rl2 @ transform,
-00013f50: 2065 6e64 2040 2074 7261 6e73 666f 726d   end @ transform
-00013f60: 0a0a 2020 2020 2020 2020 2020 2020 7377  ..            sw
-00013f70: 6565 705f 6c65 6674 202d 3d20 7377 6565  eep_left -= swee
-00013f80: 705f 7365 676d 656e 740a 0a20 2020 2064  p_segment..    d
-00013f90: 6566 205f 6170 7072 6f78 696d 6174 655f  ef _approximate_
-00013fa0: 6172 6328 7365 6c66 2c20 6c61 7374 5f69  arc(self, last_i
-00013fb0: 7465 6d29 3a0a 2020 2020 2020 2020 2222  tem):.        ""
-00013fc0: 220a 2020 2020 2020 2020 4170 7072 6f78  ".        Approx
-00013fd0: 696d 6174 6520 7468 6973 2061 7263 2077  imate this arc w
-00013fe0: 6974 6820 6120 7365 7175 656e 6365 206f  ith a sequence o
-00013ff0: 6620 6042 657a 6965 7243 7572 7665 602e  f `BezierCurve`.
-00014000: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00014010: 2020 2020 2020 2020 2020 2020 6c61 7374              last
-00014020: 5f69 7465 6d3a 2074 6865 2070 7265 7669  _item: the previ
-00014030: 6f75 7320 7061 7468 2065 6c65 6d65 6e74  ous path element
-00014040: 2028 7573 6564 2066 6f72 2069 7473 2065   (used for its e
-00014050: 6e64 2070 6f69 6e74 290a 0a20 2020 2020  nd point)..     
-00014060: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00014070: 2020 2020 2020 2020 6120 6c69 7374 206f          a list o
-00014080: 6620 6042 657a 6965 7243 7572 7665 602e  f `BezierCurve`.
-00014090: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000140a0: 2020 2020 2072 6164 6969 203d 2073 656c       radii = sel
-000140b0: 662e 7261 6469 690a 0a20 2020 2020 2020  f.radii..       
-000140c0: 2072 6576 6572 7365 203d 2054 7261 6e73   reverse = Trans
-000140d0: 666f 726d 2e72 6f74 6174 696f 6e28 2d73  form.rotation(-s
-000140e0: 656c 662e 726f 7461 7469 6f6e 290a 2020  elf.rotation).  
-000140f0: 2020 2020 2020 666f 7277 6172 6420 3d20        forward = 
-00014100: 5472 616e 7366 6f72 6d2e 726f 7461 7469  Transform.rotati
-00014110: 6f6e 2873 656c 662e 726f 7461 7469 6f6e  on(self.rotation
-00014120: 290a 0a20 2020 2020 2020 2070 7269 6d65  )..        prime
-00014130: 203d 2028 286c 6173 745f 6974 656d 2e65   = ((last_item.e
-00014140: 6e64 5f70 6f69 6e74 202d 2073 656c 662e  nd_point - self.
-00014150: 656e 6429 202a 2030 2e35 2920 4020 7265  end) * 0.5) @ re
-00014160: 7665 7273 650a 0a20 2020 2020 2020 206c  verse..        l
-00014170: 616d 5f64 6120 3d20 2870 7269 6d65 2e78  am_da = (prime.x
-00014180: 202f 2072 6164 6969 2e78 2920 2a2a 2032   / radii.x) ** 2
-00014190: 202b 2028 7072 696d 652e 7920 2f20 7261   + (prime.y / ra
-000141a0: 6469 692e 7929 202a 2a20 320a 0a20 2020  dii.y) ** 2..   
-000141b0: 2020 2020 2069 6620 6c61 6d5f 6461 203e       if lam_da >
-000141c0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-000141d0: 7261 6469 6920 3d20 506f 696e 7428 783d  radii = Point(x=
-000141e0: 286c 616d 5f64 612a 2a30 2e35 2920 2a20  (lam_da**0.5) * 
-000141f0: 7261 6469 692e 782c 2079 3d28 6c61 6d5f  radii.x, y=(lam_
-00014200: 6461 2a2a 302e 3529 202a 2072 6164 6969  da**0.5) * radii
-00014210: 2e79 290a 0a20 2020 2020 2020 2073 6967  .y)..        sig
-00014220: 6e20 3d20 2873 656c 662e 6c61 7267 6520  n = (self.large 
-00014230: 213d 2073 656c 662e 7377 6565 7029 202d  != self.sweep) -
-00014240: 2028 7365 6c66 2e6c 6172 6765 203d 3d20   (self.large == 
-00014250: 7365 6c66 2e73 7765 6570 290a 2020 2020  self.sweep).    
-00014260: 2020 2020 7278 7279 3220 3d20 2872 6164      rxry2 = (rad
-00014270: 6969 2e78 202a 2072 6164 6969 2e79 2920  ii.x * radii.y) 
-00014280: 2a2a 2032 0a20 2020 2020 2020 2072 7870  ** 2.        rxp
-00014290: 7932 203d 2028 7261 6469 692e 7820 2a20  y2 = (radii.x * 
-000142a0: 7072 696d 652e 7929 202a 2a20 320a 2020  prime.y) ** 2.  
-000142b0: 2020 2020 2020 7279 7078 3220 3d20 2872        rypx2 = (r
-000142c0: 6164 6969 2e79 202a 2070 7269 6d65 2e78  adii.y * prime.x
-000142d0: 2920 2a2a 2032 0a0a 2020 2020 2020 2020  ) ** 2..        
-000142e0: 6365 6e74 6572 7072 696d 6520 3d20 280a  centerprime = (.
-000142f0: 2020 2020 2020 2020 2020 2020 7369 676e              sign
-00014300: 0a20 2020 2020 2020 2020 2020 202a 206d  .            * m
-00014310: 6174 682e 7371 7274 2872 6f75 6e64 2872  ath.sqrt(round(r
-00014320: 7872 7932 202d 2072 7870 7932 202d 2072  xry2 - rxpy2 - r
-00014330: 7970 7832 2c20 3829 202f 2028 7278 7079  ypx2, 8) / (rxpy
-00014340: 3220 2b20 7279 7078 3229 290a 2020 2020  2 + rypx2)).    
-00014350: 2020 2020 2020 2020 2a20 506f 696e 7428          * Point(
-00014360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014370: 2078 3d72 6164 6969 2e78 202a 2070 7269   x=radii.x * pri
-00014380: 6d65 2e79 202f 2072 6164 6969 2e79 2c0a  me.y / radii.y,.
-00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143a0: 793d 2d72 6164 6969 2e79 202a 2070 7269  y=-radii.y * pri
-000143b0: 6d65 2e78 202f 2072 6164 6969 2e78 2c0a  me.x / radii.x,.
-000143c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000143d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000143e0: 2063 656e 7465 7220 3d20 2863 656e 7465   center = (cente
-000143f0: 7270 7269 6d65 2040 2066 6f72 7761 7264  rprime @ forward
-00014400: 2920 2b20 2828 6c61 7374 5f69 7465 6d2e  ) + ((last_item.
-00014410: 656e 645f 706f 696e 7420 2b20 7365 6c66  end_point + self
-00014420: 2e65 6e64 2920 2a20 302e 3529 0a0a 2020  .end) * 0.5)..  
-00014430: 2020 2020 2020 6172 6373 7461 7274 203d        arcstart =
-00014440: 2050 6f69 6e74 280a 2020 2020 2020 2020   Point(.        
-00014450: 2020 2020 783d 2870 7269 6d65 2e78 202d      x=(prime.x -
-00014460: 2063 656e 7465 7270 7269 6d65 2e78 2920   centerprime.x) 
-00014470: 2f20 7261 6469 692e 782c 0a20 2020 2020  / radii.x,.     
-00014480: 2020 2020 2020 2079 3d28 7072 696d 652e         y=(prime.
-00014490: 7920 2d20 6365 6e74 6572 7072 696d 652e  y - centerprime.
-000144a0: 7929 202f 2072 6164 6969 2e79 2c0a 2020  y) / radii.y,.  
-000144b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000144c0: 6172 6365 6e64 203d 2050 6f69 6e74 280a  arcend = Point(.
-000144d0: 2020 2020 2020 2020 2020 2020 783d 282d              x=(-
-000144e0: 7072 696d 652e 7820 2d20 6365 6e74 6572  prime.x - center
-000144f0: 7072 696d 652e 7829 202f 2072 6164 6969  prime.x) / radii
-00014500: 2e78 2c0a 2020 2020 2020 2020 2020 2020  .x,.            
-00014510: 793d 282d 7072 696d 652e 7920 2d20 6365  y=(-prime.y - ce
-00014520: 6e74 6572 7072 696d 652e 7929 202f 2072  nterprime.y) / r
-00014530: 6164 6969 2e79 2c0a 2020 2020 2020 2020  adii.y,.        
-00014540: 290a 0a20 2020 2020 2020 2074 6865 7461  )..        theta
-00014550: 203d 2050 6f69 6e74 2831 2c20 3029 2e61   = Point(1, 0).a
-00014560: 6e67 6c65 2861 7263 7374 6172 7429 0a20  ngle(arcstart). 
-00014570: 2020 2020 2020 2064 656c 7461 7468 6574         deltathet
-00014580: 6120 3d20 6172 6373 7461 7274 2e61 6e67  a = arcstart.ang
-00014590: 6c65 2861 7263 656e 6429 0a0a 2020 2020  le(arcend)..    
-000145a0: 2020 2020 6966 2028 7365 6c66 2e73 7765      if (self.swe
-000145b0: 6570 2069 7320 4661 6c73 6529 2061 6e64  ep is False) and
-000145c0: 2028 6465 6c74 6174 6865 7461 203e 2030   (deltatheta > 0
-000145d0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-000145e0: 656c 7461 7468 6574 6120 2d3d 206d 6174  eltatheta -= mat
-000145f0: 682e 7461 750a 2020 2020 2020 2020 656c  h.tau.        el
-00014600: 6966 2028 7365 6c66 2e73 7765 6570 2069  if (self.sweep i
-00014610: 7320 5472 7565 2920 616e 6420 2864 656c  s True) and (del
-00014620: 7461 7468 6574 6120 3c20 3029 3a0a 2020  tatheta < 0):.  
-00014630: 2020 2020 2020 2020 2020 6465 6c74 6174            deltat
-00014640: 6865 7461 202b 3d20 6d61 7468 2e74 6175  heta += math.tau
-00014650: 0a0a 2020 2020 2020 2020 7377 6565 705f  ..        sweep_
-00014660: 7369 676e 203d 2028 6465 6c74 6174 6865  sign = (deltathe
-00014670: 7461 203e 3d20 3029 202d 2028 6465 6c74  ta >= 0) - (delt
-00014680: 6174 6865 7461 203c 2030 290a 2020 2020  atheta < 0).    
-00014690: 2020 2020 6669 6e61 6c5f 7466 203d 2028      final_tf = (
-000146a0: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
-000146b0: 6e73 666f 726d 2e73 6361 6c69 6e67 2878  nsform.scaling(x
-000146c0: 3d31 2c20 793d 7377 6565 705f 7369 676e  =1, y=sweep_sign
-000146d0: 2920 2023 2066 6c69 7020 6e65 6761 7469  )  # flip negati
-000146e0: 7665 2073 7765 6570 730a 2020 2020 2020  ve sweeps.      
-000146f0: 2020 2020 2020 2e72 6f74 6174 6528 7468        .rotate(th
-00014700: 6574 6129 2020 2320 726f 7461 7465 2073  eta)  # rotate s
-00014710: 7461 7274 206f 6620 6172 6320 746f 2063  tart of arc to c
-00014720: 6f72 7265 6374 2070 6f73 6974 696f 6e0a  orrect position.
-00014730: 2020 2020 2020 2020 2020 2020 2e73 6361              .sca
-00014740: 6c65 2872 6164 6969 2e78 2c20 7261 6469  le(radii.x, radi
-00014750: 692e 7929 2020 2320 7363 616c 6520 756e  i.y)  # scale un
-00014760: 6974 2063 6972 636c 6520 696e 746f 2074  it circle into t
-00014770: 6865 2066 696e 616c 2065 6c6c 6970 7365  he final ellipse
-00014780: 2073 6861 7065 0a20 2020 2020 2020 2020   shape.         
-00014790: 2020 202e 726f 7461 7465 2873 656c 662e     .rotate(self.
-000147a0: 726f 7461 7469 6f6e 2920 2023 2072 6f74  rotation)  # rot
-000147b0: 6174 6520 7468 6520 656c 6c69 7073 6520  ate the ellipse 
-000147c0: 7468 6520 7370 6563 6966 6965 6420 616e  the specified an
-000147d0: 676c 650a 2020 2020 2020 2020 2020 2020  gle.            
-000147e0: 2e74 7261 6e73 6c61 7465 2863 656e 7465  .translate(cente
-000147f0: 722e 782c 2063 656e 7465 722e 7929 2020  r.x, center.y)  
-00014800: 2320 7472 616e 736c 6174 6520 746f 2074  # translate to t
-00014810: 6865 2066 696e 616c 2063 6f6f 7264 696e  he final coordin
-00014820: 6174 6573 0a20 2020 2020 2020 2029 0a0a  ates.        )..
-00014830: 2020 2020 2020 2020 6375 7276 6573 203d          curves =
-00014840: 205b 5d0a 0a20 2020 2020 2020 2066 6f72   []..        for
-00014850: 2063 7472 6c31 2c20 6374 726c 322c 2065   ctrl1, ctrl2, e
-00014860: 6e64 2069 6e20 7365 6c66 2e73 7562 6469  nd in self.subdi
-00014870: 7664 655f 7377 6565 7028 6465 6c74 6174  vde_sweep(deltat
-00014880: 6865 7461 293a 0a20 2020 2020 2020 2020  heta):.         
-00014890: 2020 2063 7572 7665 732e 6170 7065 6e64     curves.append
-000148a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000148b0: 2020 4265 7a69 6572 4375 7276 6528 6374    BezierCurve(ct
-000148c0: 726c 3120 4020 6669 6e61 6c5f 7466 2c20  rl1 @ final_tf, 
-000148d0: 6374 726c 3220 4020 6669 6e61 6c5f 7466  ctrl2 @ final_tf
-000148e0: 2c20 656e 6420 4020 6669 6e61 6c5f 7466  , end @ final_tf
-000148f0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00014900: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014910: 6375 7276 6573 0a0a 2020 2020 4066 6f72  curves..    @for
-00014920: 6365 5f6e 6f64 6f63 756d 656e 740a 2020  ce_nodocument.  
-00014930: 2020 6465 6620 7265 6e64 6572 2873 656c    def render(sel
-00014940: 662c 2067 7364 5f72 6567 6973 7472 792c  f, gsd_registry,
-00014950: 2073 7479 6c65 2c20 6c61 7374 5f69 7465   style, last_ite
-00014960: 6d2c 2069 6e69 7469 616c 5f70 6f69 6e74  m, initial_point
-00014970: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00014980: 2020 2020 2020 2052 656e 6465 7220 7468         Render th
-00014990: 6973 2070 6174 6820 656c 656d 656e 7420  is path element 
-000149a0: 746f 2069 7473 2050 4446 2072 6570 7265  to its PDF repre
-000149b0: 7365 6e74 6174 696f 6e2e 0a0a 2020 2020  sentation...    
-000149c0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000149d0: 2020 2020 2020 6773 645f 7265 6769 7374        gsd_regist
-000149e0: 7279 2028 4772 6170 6869 6373 5374 6174  ry (GraphicsStat
-000149f0: 6544 6963 7452 6567 6973 7472 7929 3a20  eDictRegistry): 
-00014a00: 7468 6520 6f77 6e65 7227 7320 6772 6170  the owner's grap
-00014a10: 6869 6373 2073 7461 7465 0a20 2020 2020  hics state.     
-00014a20: 2020 2020 2020 2020 2020 2064 6963 7469             dicti
-00014a30: 6f6e 6172 7920 7265 6769 7374 7279 2e0a  onary registry..
-00014a40: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00014a50: 6520 2847 7261 7068 6963 7353 7479 6c65  e (GraphicsStyle
-00014a60: 293a 2074 6865 2063 7572 7265 6e74 2072  ): the current r
-00014a70: 6573 6f6c 7665 6420 6772 6170 6869 6373  esolved graphics
-00014a80: 2073 7479 6c65 0a20 2020 2020 2020 2020   style.         
-00014a90: 2020 206c 6173 745f 6974 656d 3a20 7468     last_item: th
-00014aa0: 6520 7072 6576 696f 7573 2070 6174 6820  e previous path 
-00014ab0: 656c 656d 656e 742e 0a20 2020 2020 2020  element..       
-00014ac0: 2020 2020 2069 6e69 7469 616c 5f70 6f69       initial_poi
-00014ad0: 6e74 3a20 6c61 7374 2070 6f73 6974 696f  nt: last positio
-00014ae0: 6e20 7365 7420 6279 2061 2022 4d22 206f  n set by a "M" o
-00014af0: 7220 226d 2220 636f 6d6d 616e 640a 0a20  r "m" command.. 
-00014b00: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00014b10: 2020 2020 2020 2020 2020 2020 6120 7475              a tu
-00014b20: 706c 6520 6f66 2060 2873 7472 2c20 6e65  ple of `(str, ne
-00014b30: 775f 6c61 7374 5f69 7465 6d29 602c 2077  w_last_item)`, w
-00014b40: 6865 7265 2060 6e65 775f 6c61 7374 5f69  here `new_last_i
-00014b50: 7465 6d60 2069 7320 6120 7265 736f 6c76  tem` is a resolv
-00014b60: 6564 0a20 2020 2020 2020 2020 2020 2060  ed.            `
-00014b70: 4265 7a69 6572 4375 7276 6560 2e0a 2020  BezierCurve`..  
-00014b80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014b90: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-00014ba0: 626c 653d 756e 7573 6564 2d61 7267 756d  ble=unused-argum
-00014bb0: 656e 740a 2020 2020 2020 2020 6375 7276  ent.        curv
-00014bc0: 6573 203d 2073 656c 662e 5f61 7070 726f  es = self._appro
-00014bd0: 7869 6d61 7465 5f61 7263 286c 6173 745f  ximate_arc(last_
-00014be0: 6974 656d 290a 0a20 2020 2020 2020 2069  item)..        i
-00014bf0: 6620 6e6f 7420 6375 7276 6573 3a0a 2020  f not curves:.  
-00014c00: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014c10: 2022 222c 206c 6173 745f 6974 656d 0a0a   "", last_item..
-00014c20: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-00014c30: 0a20 2020 2020 2020 2020 2020 2022 2022  .            " "
-00014c40: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
-00014c50: 2020 2020 2020 2063 7572 7665 2e72 656e         curve.ren
-00014c60: 6465 7228 6773 645f 7265 6769 7374 7279  der(gsd_registry
-00014c70: 2c20 7374 796c 652c 2070 7265 762c 2069  , style, prev, i
-00014c80: 6e69 7469 616c 5f70 6f69 6e74 295b 305d  nitial_point)[0]
-00014c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ca0: 2066 6f72 2070 7265 762c 2063 7572 7665   for prev, curve
-00014cb0: 2069 6e20 7a69 7028 5b6c 6173 745f 6974   in zip([last_it
-00014cc0: 656d 2c20 2a63 7572 7665 735b 3a2d 315d  em, *curves[:-1]
-00014cd0: 5d2c 2063 7572 7665 7329 0a20 2020 2020  ], curves).     
-00014ce0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00014cf0: 2020 2020 2020 6375 7276 6573 5b2d 315d        curves[-1]
-00014d00: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-00014d10: 6974 6961 6c5f 706f 696e 742c 0a20 2020  itial_point,.   
-00014d20: 2020 2020 2029 0a0a 2020 2020 4066 6f72       )..    @for
-00014d30: 6365 5f6e 6f64 6f63 756d 656e 740a 2020  ce_nodocument.  
-00014d40: 2020 6465 6620 7265 6e64 6572 5f64 6562    def render_deb
-00014d50: 7567 280a 2020 2020 2020 2020 7365 6c66  ug(.        self
-00014d60: 2c20 6773 645f 7265 6769 7374 7279 2c20  , gsd_registry, 
-00014d70: 7374 796c 652c 206c 6173 745f 6974 656d  style, last_item
-00014d80: 2c20 696e 6974 6961 6c5f 706f 696e 742c  , initial_point,
-00014d90: 2064 6562 7567 5f73 7472 6561 6d2c 2070   debug_stream, p
-00014da0: 6678 0a20 2020 2029 3a0a 2020 2020 2020  fx.    ):.      
-00014db0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00014dc0: 6e64 6572 2074 6869 7320 7061 7468 2065  nder this path e
-00014dd0: 6c65 6d65 6e74 2074 6f20 6974 7320 5044  lement to its PD
-00014de0: 4620 7265 7072 6573 656e 7461 7469 6f6e  F representation
-00014df0: 2061 6e64 2070 726f 6475 6365 2064 6562   and produce deb
-00014e00: 7567 0a20 2020 2020 2020 2069 6e66 6f72  ug.        infor
-00014e10: 6d61 7469 6f6e 2e0a 0a20 2020 2020 2020  mation...       
-00014e20: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00014e30: 2020 2067 7364 5f72 6567 6973 7472 7920     gsd_registry 
-00014e40: 2847 7261 7068 6963 7353 7461 7465 4469  (GraphicsStateDi
-00014e50: 6374 5265 6769 7374 7279 293a 2074 6865  ctRegistry): the
-00014e60: 206f 776e 6572 2773 2067 7261 7068 6963   owner's graphic
-00014e70: 7320 7374 6174 650a 2020 2020 2020 2020  s state.        
-00014e80: 2020 2020 2020 2020 6469 6374 696f 6e61          dictiona
-00014e90: 7279 2072 6567 6973 7472 792e 0a20 2020  ry registry..   
-00014ea0: 2020 2020 2020 2020 2073 7479 6c65 2028           style (
-00014eb0: 4772 6170 6869 6373 5374 796c 6529 3a20  GraphicsStyle): 
-00014ec0: 7468 6520 6375 7272 656e 7420 7265 736f  the current reso
-00014ed0: 6c76 6564 2067 7261 7068 6963 7320 7374  lved graphics st
-00014ee0: 796c 650a 2020 2020 2020 2020 2020 2020  yle.            
-00014ef0: 6c61 7374 5f69 7465 6d3a 2074 6865 2070  last_item: the p
-00014f00: 7265 7669 6f75 7320 7061 7468 2065 6c65  revious path ele
-00014f10: 6d65 6e74 2e0a 2020 2020 2020 2020 2020  ment..          
-00014f20: 2020 696e 6974 6961 6c5f 706f 696e 743a    initial_point:
-00014f30: 206c 6173 7420 706f 7369 7469 6f6e 2073   last position s
-00014f40: 6574 2062 7920 6120 224d 2220 6f72 2022  et by a "M" or "
-00014f50: 6d22 2063 6f6d 6d61 6e64 0a20 2020 2020  m" command.     
-00014f60: 2020 2020 2020 2064 6562 7567 5f73 7472         debug_str
-00014f70: 6561 6d20 2869 6f2e 5465 7874 494f 293a  eam (io.TextIO):
-00014f80: 2074 6865 2073 7472 6561 6d20 746f 2077   the stream to w
-00014f90: 6869 6368 2074 6865 2064 6562 7567 206f  hich the debug o
-00014fa0: 7574 7075 7420 7368 6f75 6c64 2062 650a  utput should be.
-00014fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fc0: 7772 6974 7465 6e2e 2054 6869 7320 6973  written. This is
-00014fd0: 206e 6f74 2067 7561 7261 6e74 6565 6420   not guaranteed 
-00014fe0: 746f 2062 6520 7365 656b 6162 6c65 2028  to be seekable (
-00014ff0: 652e 672e 2069 7420 6d61 7920 6265 2073  e.g. it may be s
-00015000: 7464 6f75 7420 6f72 0a20 2020 2020 2020  tdout or.       
-00015010: 2020 2020 2020 2020 2073 7464 6572 7229           stderr)
-00015020: 2e0a 2020 2020 2020 2020 2020 2020 7066  ..            pf
-00015030: 7820 2873 7472 293a 2074 6865 2063 7572  x (str): the cur
-00015040: 7265 6e74 2064 6562 7567 206f 7574 7075  rent debug outpu
-00015050: 7420 7072 6566 6978 2073 7472 696e 6720  t prefix string 
-00015060: 286f 6e6c 7920 6e65 6564 6564 2069 6620  (only needed if 
-00015070: 656d 6974 7469 6e67 0a20 2020 2020 2020  emitting.       
-00015080: 2020 2020 2020 2020 206d 6f72 6520 7468           more th
-00015090: 616e 206f 6e65 206c 696e 6529 2e0a 0a20  an one line)... 
-000150a0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-000150b0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000150c0: 7361 6d65 2074 7570 6c65 2061 7320 6041  same tuple as `A
-000150d0: 7263 2e72 656e 6465 7260 2e0a 2020 2020  rc.render`..    
-000150e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000150f0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00015100: 653d 756e 7573 6564 2d61 7267 756d 656e  e=unused-argumen
-00015110: 740a 2020 2020 2020 2020 6375 7276 6573  t.        curves
-00015120: 203d 2073 656c 662e 5f61 7070 726f 7869   = self._approxi
-00015130: 6d61 7465 5f61 7263 286c 6173 745f 6974  mate_arc(last_it
-00015140: 656d 290a 0a20 2020 2020 2020 2064 6562  em)..        deb
-00015150: 7567 5f73 7472 6561 6d2e 7772 6974 6528  ug_stream.write(
-00015160: 6622 7b73 656c 667d 2072 6573 6f6c 7665  f"{self} resolve
-00015170: 6420 746f 3a5c 6e22 290a 2020 2020 2020  d to:\n").      
-00015180: 2020 6966 206e 6f74 2063 7572 7665 733a    if not curves:
-00015190: 0a20 2020 2020 2020 2020 2020 2064 6562  .            deb
-000151a0: 7567 5f73 7472 6561 6d2e 7772 6974 6528  ug_stream.write(
-000151b0: 7066 7820 2b20 2220 e294 94e2 9480 206e  pfx + " ...... n
-000151c0: 6f74 6869 6e67 5c6e 2229 0a20 2020 2020  othing\n").     
-000151d0: 2020 2020 2020 2072 6574 7572 6e20 2222         return ""
-000151e0: 2c20 6c61 7374 5f69 7465 6d0a 0a20 2020  , last_item..   
-000151f0: 2020 2020 2070 7265 7669 6f75 7320 3d20       previous = 
-00015200: 5b6c 6173 745f 6974 656d 5d0a 2020 2020  [last_item].    
-00015210: 2020 2020 666f 7220 6375 7276 6520 696e      for curve in
-00015220: 2063 7572 7665 735b 3a2d 315d 3a0a 2020   curves[:-1]:.  
-00015230: 2020 2020 2020 2020 2020 7072 6576 696f            previo
-00015240: 7573 2e61 7070 656e 6428 6375 7276 6529  us.append(curve)
-00015250: 0a20 2020 2020 2020 2020 2020 2064 6562  .            deb
-00015260: 7567 5f73 7472 6561 6d2e 7772 6974 6528  ug_stream.write(
-00015270: 7066 7820 2b20 6622 20e2 949c e294 8020  pfx + f" ...... 
-00015280: 7b63 7572 7665 7d5c 6e22 290a 2020 2020  {curve}\n").    
-00015290: 2020 2020 6465 6275 675f 7374 7265 616d      debug_stream
-000152a0: 2e77 7269 7465 2870 6678 202b 2066 2220  .write(pfx + f" 
-000152b0: e294 94e2 9480 207b 6375 7276 6573 5b2d  ...... {curves[-
-000152c0: 315d 7d5c 6e22 290a 0a20 2020 2020 2020  1]}\n")..       
-000152d0: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-000152e0: 2020 2020 2020 2220 222e 6a6f 696e 280a        " ".join(.
-000152f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015300: 6375 7276 652e 7265 6e64 6572 2867 7364  curve.render(gsd
-00015310: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
-00015320: 2c20 7072 6576 2c20 696e 6974 6961 6c5f  , prev, initial_
-00015330: 706f 696e 7429 5b30 5d0a 2020 2020 2020  point)[0].      
-00015340: 2020 2020 2020 2020 2020 666f 7220 7072            for pr
-00015350: 6576 2c20 6375 7276 6520 696e 207a 6970  ev, curve in zip
-00015360: 2870 7265 7669 6f75 732c 2063 7572 7665  (previous, curve
-00015370: 7329 0a20 2020 2020 2020 2020 2020 2029  s).            )
-00015380: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
-00015390: 7276 6573 5b2d 315d 2c0a 2020 2020 2020  rves[-1],.      
-000153a0: 2020 2020 2020 696e 6974 6961 6c5f 706f        initial_po
-000153b0: 696e 742c 0a20 2020 2020 2020 2029 0a0a  int,.        )..
-000153c0: 0a63 6c61 7373 2052 656c 6174 6976 6541  .class RelativeA
-000153d0: 7263 284e 616d 6564 5475 706c 6529 3a0a  rc(NamedTuple):.
-000153e0: 2020 2020 2222 220a 2020 2020 416e 2065      """.    An e
-000153f0: 6c6c 6970 7469 6361 6c20 6172 6320 7061  lliptical arc pa
-00015400: 7468 2065 6c65 6d65 6e74 2e0a 0a20 2020  th element...   
-00015410: 2054 6865 2061 7263 2069 7320 6472 6177   The arc is draw
-00015420: 6e20 6672 6f6d 2074 6865 2065 6e64 206f  n from the end o
-00015430: 6620 7468 6520 6375 7272 656e 7420 7061  f the current pa
-00015440: 7468 2065 6c65 6d65 6e74 2074 6f20 6974  th element to it
-00015450: 7320 7370 6563 6966 6965 6420 656e 6420  s specified end 
-00015460: 706f 696e 740a 2020 2020 7573 696e 6720  point.    using 
-00015470: 6120 6e75 6d62 6572 206f 6620 7061 7261  a number of para
-00015480: 6d65 7465 7273 2074 6f20 6465 7465 726d  meters to determ
-00015490: 696e 6520 686f 7720 6974 2069 7320 636f  ine how it is co
-000154a0: 6e73 7472 7563 7465 642e 0a0a 2020 2020  nstructed...    
-000154b0: 5365 653a 2060 5061 696e 7465 6450 6174  See: `PaintedPat
-000154c0: 682e 6172 635f 7265 6c61 7469 7665 600a  h.arc_relative`.
-000154d0: 2020 2020 2222 220a 0a20 2020 2072 6164      """..    rad
-000154e0: 6969 3a20 506f 696e 740a 2020 2020 2222  ii: Point.    ""
-000154f0: 220a 2020 2020 5468 6520 782d 2061 6e64  ".    The x- and
-00015500: 2079 2d72 6164 6969 206f 6620 7468 6520   y-radii of the 
-00015510: 6172 632e 2049 6620 6072 6164 6969 2e78  arc. If `radii.x
-00015520: 203d 3d20 7261 6469 692e 7960 2074 6865   == radii.y` the
-00015530: 2061 7263 2077 696c 6c20 6265 2063 6972   arc will be cir
-00015540: 6375 6c61 722e 0a20 2020 2022 2222 0a20  cular..    """. 
-00015550: 2020 2072 6f74 6174 696f 6e3a 204e 756d     rotation: Num
-00015560: 6265 720a 2020 2020 2222 2254 6865 2072  ber.    """The r
-00015570: 6f74 6174 696f 6e20 6f66 2074 6865 2061  otation of the a
-00015580: 7263 2773 206d 616a 6f72 2f6d 696e 6f72  rc's major/minor
-00015590: 2061 7865 7320 7265 6c61 7469 7665 2074   axes relative t
-000155a0: 6f20 7468 6520 636f 6f72 6469 6e61 7465  o the coordinate
-000155b0: 2066 7261 6d65 2e22 2222 0a20 2020 206c   frame.""".    l
-000155c0: 6172 6765 3a20 626f 6f6c 0a20 2020 2022  arge: bool.    "
-000155d0: 2222 4966 2054 7275 652c 2073 7765 6570  ""If True, sweep
-000155e0: 2074 6865 2061 7263 206f 7665 7220 616e   the arc over an
-000155f0: 2061 6e67 6c65 2067 7265 6174 6572 2074   angle greater t
-00015600: 6861 6e20 6f72 2065 7175 616c 2074 6f20  han or equal to 
-00015610: 3138 3020 6465 6772 6565 732e 2222 220a  180 degrees.""".
-00015620: 2020 2020 7377 6565 703a 2062 6f6f 6c0a      sweep: bool.
-00015630: 2020 2020 2222 2249 6620 5472 7565 2c20      """If True, 
-00015640: 7468 6520 6172 6320 6973 2073 7765 7074  the arc is swept
-00015650: 2069 6e20 7468 6520 706f 7369 7469 7665   in the positive
-00015660: 2061 6e67 756c 6172 2064 6972 6563 7469   angular directi
-00015670: 6f6e 2e22 2222 0a20 2020 2065 6e64 3a20  on.""".    end: 
-00015680: 506f 696e 740a 2020 2020 2222 2254 6865  Point.    """The
-00015690: 2065 6e64 2070 6f69 6e74 206f 6620 7468   end point of th
-000156a0: 6520 6172 6320 7265 6c61 7469 7665 2074  e arc relative t
-000156b0: 6f20 7468 6520 656e 6420 6f66 2074 6865  o the end of the
-000156c0: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
-000156d0: 6c65 6d65 6e74 2e22 2222 0a0a 2020 2020  lement."""..    
-000156e0: 4066 6f72 6365 5f6e 6f64 6f63 756d 656e  @force_nodocumen
-000156f0: 740a 2020 2020 6465 6620 7265 6e64 6572  t.    def render
-00015700: 2873 656c 662c 2067 7364 5f72 6567 6973  (self, gsd_regis
-00015710: 7472 792c 2073 7479 6c65 2c20 6c61 7374  try, style, last
-00015720: 5f69 7465 6d2c 2069 6e69 7469 616c 5f70  _item, initial_p
-00015730: 6f69 6e74 293a 0a20 2020 2020 2020 2022  oint):.        "
-00015740: 2222 0a20 2020 2020 2020 2052 656e 6465  "".        Rende
-00015750: 7220 7468 6973 2070 6174 6820 656c 656d  r this path elem
-00015760: 656e 7420 746f 2069 7473 2050 4446 2072  ent to its PDF r
-00015770: 6570 7265 7365 6e74 6174 696f 6e2e 0a0a  epresentation...
-00015780: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00015790: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-000157a0: 6769 7374 7279 2028 4772 6170 6869 6373  gistry (Graphics
-000157b0: 5374 6174 6544 6963 7452 6567 6973 7472  StateDictRegistr
-000157c0: 7929 3a20 7468 6520 6f77 6e65 7227 7320  y): the owner's 
-000157d0: 6772 6170 6869 6373 2073 7461 7465 0a20  graphics state. 
-000157e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000157f0: 6963 7469 6f6e 6172 7920 7265 6769 7374  ictionary regist
-00015800: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
-00015810: 7374 796c 6520 2847 7261 7068 6963 7353  style (GraphicsS
-00015820: 7479 6c65 293a 2074 6865 2063 7572 7265  tyle): the curre
-00015830: 6e74 2072 6573 6f6c 7665 6420 6772 6170  nt resolved grap
-00015840: 6869 6373 2073 7479 6c65 0a20 2020 2020  hics style.     
-00015850: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
-00015860: 3a20 7468 6520 7072 6576 696f 7573 2070  : the previous p
-00015870: 6174 6820 656c 656d 656e 742e 0a20 2020  ath element..   
-00015880: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
-00015890: 5f70 6f69 6e74 3a20 6c61 7374 2070 6f73  _point: last pos
-000158a0: 6974 696f 6e20 7365 7420 6279 2061 2022  ition set by a "
-000158b0: 4d22 206f 7220 226d 2220 636f 6d6d 616e  M" or "m" comman
-000158c0: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
-000158d0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-000158e0: 6120 7475 706c 6520 6f66 2060 2873 7472  a tuple of `(str
-000158f0: 2c20 6e65 775f 6c61 7374 5f69 7465 6d29  , new_last_item)
-00015900: 602c 2077 6865 7265 2060 6e65 775f 6c61  `, where `new_la
-00015910: 7374 5f69 7465 6d60 2069 7320 6120 7265  st_item` is a re
-00015920: 736f 6c76 6564 0a20 2020 2020 2020 2020  solved.         
-00015930: 2020 2060 4265 7a69 6572 4375 7276 6560     `BezierCurve`
-00015940: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00015950: 2020 2020 2020 2320 7079 6c69 6e74 3a20        # pylint: 
-00015960: 6469 7361 626c 653d 756e 7573 6564 2d61  disable=unused-a
-00015970: 7267 756d 656e 740a 2020 2020 2020 2020  rgument.        
-00015980: 7265 7475 726e 2041 7263 280a 2020 2020  return Arc(.    
-00015990: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-000159a0: 6969 2c0a 2020 2020 2020 2020 2020 2020  ii,.            
-000159b0: 7365 6c66 2e72 6f74 6174 696f 6e2c 0a20  self.rotation,. 
-000159c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000159d0: 6c61 7267 652c 0a20 2020 2020 2020 2020  large,.         
-000159e0: 2020 2073 656c 662e 7377 6565 702c 0a20     self.sweep,. 
-000159f0: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-00015a00: 6974 656d 2e65 6e64 5f70 6f69 6e74 202b  item.end_point +
-00015a10: 2073 656c 662e 656e 642c 0a20 2020 2020   self.end,.     
-00015a20: 2020 2029 2e72 656e 6465 7228 6773 645f     ).render(gsd_
-00015a30: 7265 6769 7374 7279 2c20 7374 796c 652c  registry, style,
-00015a40: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
-00015a50: 6961 6c5f 706f 696e 7429 0a0a 2020 2020  ial_point)..    
-00015a60: 4066 6f72 6365 5f6e 6f64 6f63 756d 656e  @force_nodocumen
-00015a70: 740a 2020 2020 6465 6620 7265 6e64 6572  t.    def render
-00015a80: 5f64 6562 7567 280a 2020 2020 2020 2020  _debug(.        
-00015a90: 7365 6c66 2c20 6773 645f 7265 6769 7374  self, gsd_regist
-00015aa0: 7279 2c20 7374 796c 652c 206c 6173 745f  ry, style, last_
-00015ab0: 6974 656d 2c20 696e 6974 6961 6c5f 706f  item, initial_po
-00015ac0: 696e 742c 2064 6562 7567 5f73 7472 6561  int, debug_strea
-00015ad0: 6d2c 2070 6678 0a20 2020 2029 3a0a 2020  m, pfx.    ):.  
-00015ae0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00015af0: 2020 5265 6e64 6572 2074 6869 7320 7061    Render this pa
-00015b00: 7468 2065 6c65 6d65 6e74 2074 6f20 6974  th element to it
-00015b10: 7320 5044 4620 7265 7072 6573 656e 7461  s PDF representa
-00015b20: 7469 6f6e 2061 6e64 2070 726f 6475 6365  tion and produce
-00015b30: 2064 6562 7567 0a20 2020 2020 2020 2069   debug.        i
-00015b40: 6e66 6f72 6d61 7469 6f6e 2e0a 0a20 2020  nformation...   
-00015b50: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00015b60: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
-00015b70: 7472 7920 2847 7261 7068 6963 7353 7461  try (GraphicsSta
-00015b80: 7465 4469 6374 5265 6769 7374 7279 293a  teDictRegistry):
-00015b90: 2074 6865 206f 776e 6572 2773 2067 7261   the owner's gra
-00015ba0: 7068 6963 7320 7374 6174 650a 2020 2020  phics state.    
-00015bb0: 2020 2020 2020 2020 2020 2020 6469 6374              dict
-00015bc0: 696f 6e61 7279 2072 6567 6973 7472 792e  ionary registry.
-00015bd0: 0a20 2020 2020 2020 2020 2020 2073 7479  .            sty
-00015be0: 6c65 2028 4772 6170 6869 6373 5374 796c  le (GraphicsStyl
-00015bf0: 6529 3a20 7468 6520 6375 7272 656e 7420  e): the current 
-00015c00: 7265 736f 6c76 6564 2067 7261 7068 6963  resolved graphic
-00015c10: 7320 7374 796c 650a 2020 2020 2020 2020  s style.        
-00015c20: 2020 2020 6c61 7374 5f69 7465 6d3a 2074      last_item: t
-00015c30: 6865 2070 7265 7669 6f75 7320 7061 7468  he previous path
-00015c40: 2065 6c65 6d65 6e74 2e0a 2020 2020 2020   element..      
-00015c50: 2020 2020 2020 696e 6974 6961 6c5f 706f        initial_po
-00015c60: 696e 743a 206c 6173 7420 706f 7369 7469  int: last positi
-00015c70: 6f6e 2073 6574 2062 7920 6120 224d 2220  on set by a "M" 
-00015c80: 6f72 2022 6d22 2063 6f6d 6d61 6e64 0a20  or "m" command. 
-00015c90: 2020 2020 2020 2020 2020 2064 6562 7567             debug
-00015ca0: 5f73 7472 6561 6d20 2869 6f2e 5465 7874  _stream (io.Text
-00015cb0: 494f 293a 2074 6865 2073 7472 6561 6d20  IO): the stream 
-00015cc0: 746f 2077 6869 6368 2074 6865 2064 6562  to which the deb
-00015cd0: 7567 206f 7574 7075 7420 7368 6f75 6c64  ug output should
-00015ce0: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
-00015cf0: 2020 2020 7772 6974 7465 6e2e 2054 6869      written. Thi
-00015d00: 7320 6973 206e 6f74 2067 7561 7261 6e74  s is not guarant
-00015d10: 6565 6420 746f 2062 6520 7365 656b 6162  eed to be seekab
-00015d20: 6c65 2028 652e 672e 2069 7420 6d61 7920  le (e.g. it may 
-00015d30: 6265 2073 7464 6f75 7420 6f72 0a20 2020  be stdout or.   
-00015d40: 2020 2020 2020 2020 2020 2020 2073 7464               std
-00015d50: 6572 7229 2e0a 2020 2020 2020 2020 2020  err)..          
-00015d60: 2020 7066 7820 2873 7472 293a 2074 6865    pfx (str): the
-00015d70: 2063 7572 7265 6e74 2064 6562 7567 206f   current debug o
-00015d80: 7574 7075 7420 7072 6566 6978 2073 7472  utput prefix str
-00015d90: 696e 6720 286f 6e6c 7920 6e65 6564 6564  ing (only needed
-00015da0: 2069 6620 656d 6974 7469 6e67 0a20 2020   if emitting.   
-00015db0: 2020 2020 2020 2020 2020 2020 206d 6f72               mor
-00015dc0: 6520 7468 616e 206f 6e65 206c 696e 6529  e than one line)
-00015dd0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00015de0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00015df0: 5468 6520 7361 6d65 2074 7570 6c65 2061  The same tuple a
-00015e00: 7320 6052 656c 6174 6976 6541 7263 2e72  s `RelativeArc.r
-00015e10: 656e 6465 7260 2e0a 2020 2020 2020 2020  ender`..        
-00015e20: 2222 220a 2020 2020 2020 2020 2320 7079  """.        # py
-00015e30: 6c69 6e74 3a20 6469 7361 626c 653d 756e  lint: disable=un
-00015e40: 7573 6564 2d61 7267 756d 656e 740a 2020  used-argument.  
-00015e50: 2020 2020 2020 2320 6e65 776c 696e 6520        # newline 
-00015e60: 6973 2069 6e74 656e 7469 6f6e 616c 6c79  is intentionally
-00015e70: 206d 6973 7369 6e67 2068 6572 650a 2020   missing here.  
-00015e80: 2020 2020 2020 6465 6275 675f 7374 7265        debug_stre
-00015e90: 616d 2e77 7269 7465 2866 227b 7365 6c66  am.write(f"{self
-00015ea0: 7d20 7265 736f 6c76 6564 2074 6f20 2229  } resolved to ")
-00015eb0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00015ec0: 2041 7263 280a 2020 2020 2020 2020 2020   Arc(.          
-00015ed0: 2020 7365 6c66 2e72 6164 6969 2c0a 2020    self.radii,.  
-00015ee0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00015ef0: 6f74 6174 696f 6e2c 0a20 2020 2020 2020  otation,.       
-00015f00: 2020 2020 2073 656c 662e 6c61 7267 652c       self.large,
-00015f10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015f20: 662e 7377 6565 702c 0a20 2020 2020 2020  f.sweep,.       
-00015f30: 2020 2020 206c 6173 745f 6974 656d 2e65       last_item.e
-00015f40: 6e64 5f70 6f69 6e74 202b 2073 656c 662e  nd_point + self.
-00015f50: 656e 642c 0a20 2020 2020 2020 2029 2e72  end,.        ).r
-00015f60: 656e 6465 725f 6465 6275 6728 6773 645f  ender_debug(gsd_
-00015f70: 7265 6769 7374 7279 2c20 7374 796c 652c  registry, style,
-00015f80: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
-00015f90: 6961 6c5f 706f 696e 742c 2064 6562 7567  ial_point, debug
-00015fa0: 5f73 7472 6561 6d2c 2070 6678 290a 0a0a  _stream, pfx)...
-00015fb0: 636c 6173 7320 5265 6374 616e 676c 6528  class Rectangle(
-00015fc0: 4e61 6d65 6454 7570 6c65 293a 0a20 2020  NamedTuple):.   
-00015fd0: 2022 2222 4120 7064 6620 7072 696d 6974   """A pdf primit
-00015fe0: 6976 6520 7265 6374 616e 676c 652e 2222  ive rectangle.""
-00015ff0: 220a 0a20 2020 206f 7267 3a20 506f 696e  "..    org: Poin
-00016000: 740a 2020 2020 2222 2254 6865 2074 6f70  t.    """The top
-00016010: 2d6c 6566 7420 636f 726e 6572 206f 6620  -left corner of 
-00016020: 7468 6520 7265 6374 616e 676c 652e 2222  the rectangle.""
-00016030: 220a 2020 2020 7369 7a65 3a20 506f 696e  ".    size: Poin
-00016040: 740a 2020 2020 2222 2254 6865 2077 6964  t.    """The wid
-00016050: 7468 2061 6e64 2068 6569 6768 7420 6f66  th and height of
-00016060: 2074 6865 2072 6563 7461 6e67 6c65 2e22   the rectangle."
-00016070: 2222 0a0a 2020 2020 4066 6f72 6365 5f6e  ""..    @force_n
-00016080: 6f64 6f63 756d 656e 740a 2020 2020 6465  odocument.    de
-00016090: 6620 7265 6e64 6572 2873 656c 662c 2067  f render(self, g
-000160a0: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
-000160b0: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
-000160c0: 6e69 7469 616c 5f70 6f69 6e74 293a 0a20  nitial_point):. 
-000160d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000160e0: 2020 2052 656e 6465 7220 7468 6973 2070     Render this p
-000160f0: 6174 6820 656c 656d 656e 7420 746f 2069  ath element to i
-00016100: 7473 2050 4446 2072 6570 7265 7365 6e74  ts PDF represent
-00016110: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-00016120: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00016130: 2020 6773 645f 7265 6769 7374 7279 2028    gsd_registry (
-00016140: 4772 6170 6869 6373 5374 6174 6544 6963  GraphicsStateDic
-00016150: 7452 6567 6973 7472 7929 3a20 7468 6520  tRegistry): the 
-00016160: 6f77 6e65 7227 7320 6772 6170 6869 6373  owner's graphics
-00016170: 2073 7461 7465 0a20 2020 2020 2020 2020   state.         
-00016180: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
-00016190: 7920 7265 6769 7374 7279 2e0a 2020 2020  y registry..    
-000161a0: 2020 2020 2020 2020 7374 796c 6520 2847          style (G
-000161b0: 7261 7068 6963 7353 7479 6c65 293a 2074  raphicsStyle): t
-000161c0: 6865 2063 7572 7265 6e74 2072 6573 6f6c  he current resol
-000161d0: 7665 6420 6772 6170 6869 6373 2073 7479  ved graphics sty
-000161e0: 6c65 0a20 2020 2020 2020 2020 2020 206c  le.            l
-000161f0: 6173 745f 6974 656d 3a20 7468 6520 7072  ast_item: the pr
-00016200: 6576 696f 7573 2070 6174 6820 656c 656d  evious path elem
-00016210: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
-00016220: 2069 6e69 7469 616c 5f70 6f69 6e74 3a20   initial_point: 
-00016230: 6c61 7374 2070 6f73 6974 696f 6e20 7365  last position se
-00016240: 7420 6279 2061 2022 4d22 206f 7220 226d  t by a "M" or "m
-00016250: 2220 636f 6d6d 616e 640a 0a20 2020 2020  " command..     
-00016260: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00016270: 2020 2020 2020 2020 6120 7475 706c 6520          a tuple 
-00016280: 6f66 2060 2873 7472 2c20 6e65 775f 6c61  of `(str, new_la
-00016290: 7374 5f69 7465 6d29 602c 2077 6865 7265  st_item)`, where
-000162a0: 2060 6e65 775f 6c61 7374 5f69 7465 6d60   `new_last_item`
-000162b0: 2069 7320 6120 604c 696e 6560 2062 6163   is a `Line` bac
-000162c0: 6b20 746f 0a20 2020 2020 2020 2020 2020  k to.           
-000162d0: 2074 6865 2072 6563 7461 6e67 6c65 2773   the rectangle's
-000162e0: 206f 7269 6769 6e2e 0a20 2020 2020 2020   origin..       
-000162f0: 2022 2222 0a20 2020 2020 2020 2023 2070   """.        # p
-00016300: 796c 696e 743a 2064 6973 6162 6c65 3d75  ylint: disable=u
-00016310: 6e75 7365 642d 6172 6775 6d65 6e74 0a0a  nused-argument..
-00016320: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-00016330: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
-00016340: 7365 6c66 2e6f 7267 2e72 656e 6465 7228  self.org.render(
-00016350: 297d 207b 7365 6c66 2e73 697a 652e 7265  )} {self.size.re
-00016360: 6e64 6572 2829 7d20 7265 222c 0a20 2020  nder()} re",.   
-00016370: 2020 2020 2020 2020 204c 696e 6528 7365           Line(se
-00016380: 6c66 2e6f 7267 292c 0a20 2020 2020 2020  lf.org),.       
-00016390: 2020 2020 2069 6e69 7469 616c 5f70 6f69       initial_poi
-000163a0: 6e74 2c0a 2020 2020 2020 2020 290a 0a20  nt,.        ).. 
-000163b0: 2020 2040 666f 7263 655f 6e6f 646f 6375     @force_nodocu
-000163c0: 6d65 6e74 0a20 2020 2064 6566 2072 656e  ment.    def ren
-000163d0: 6465 725f 6465 6275 6728 0a20 2020 2020  der_debug(.     
-000163e0: 2020 2073 656c 662c 2067 7364 5f72 6567     self, gsd_reg
-000163f0: 6973 7472 792c 2073 7479 6c65 2c20 6c61  istry, style, la
-00016400: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
-00016410: 5f70 6f69 6e74 2c20 6465 6275 675f 7374  _point, debug_st
-00016420: 7265 616d 2c20 7066 780a 2020 2020 293a  ream, pfx.    ):
-00016430: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016440: 2020 2020 2052 656e 6465 7220 7468 6973       Render this
-00016450: 2070 6174 6820 656c 656d 656e 7420 746f   path element to
-00016460: 2069 7473 2050 4446 2072 6570 7265 7365   its PDF represe
-00016470: 6e74 6174 696f 6e20 616e 6420 7072 6f64  ntation and prod
-00016480: 7563 6520 6465 6275 670a 2020 2020 2020  uce debug.      
-00016490: 2020 696e 666f 726d 6174 696f 6e2e 0a0a    information...
-000164a0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000164b0: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-000164c0: 6769 7374 7279 2028 4772 6170 6869 6373  gistry (Graphics
-000164d0: 5374 6174 6544 6963 7452 6567 6973 7472  StateDictRegistr
-000164e0: 7929 3a20 7468 6520 6f77 6e65 7227 7320  y): the owner's 
-000164f0: 6772 6170 6869 6373 2073 7461 7465 0a20  graphics state. 
-00016500: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00016510: 6963 7469 6f6e 6172 7920 7265 6769 7374  ictionary regist
-00016520: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
-00016530: 7374 796c 6520 2847 7261 7068 6963 7353  style (GraphicsS
-00016540: 7479 6c65 293a 2074 6865 2063 7572 7265  tyle): the curre
-00016550: 6e74 2072 6573 6f6c 7665 6420 6772 6170  nt resolved grap
-00016560: 6869 6373 2073 7479 6c65 0a20 2020 2020  hics style.     
-00016570: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
-00016580: 3a20 7468 6520 7072 6576 696f 7573 2070  : the previous p
-00016590: 6174 6820 656c 656d 656e 742e 0a20 2020  ath element..   
-000165a0: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
-000165b0: 5f70 6f69 6e74 3a20 6c61 7374 2070 6f73  _point: last pos
-000165c0: 6974 696f 6e20 7365 7420 6279 2061 2022  ition set by a "
-000165d0: 4d22 206f 7220 226d 2220 636f 6d6d 616e  M" or "m" comman
-000165e0: 640a 2020 2020 2020 2020 2020 2020 6465  d.            de
-000165f0: 6275 675f 7374 7265 616d 2028 696f 2e54  bug_stream (io.T
-00016600: 6578 7449 4f29 3a20 7468 6520 7374 7265  extIO): the stre
-00016610: 616d 2074 6f20 7768 6963 6820 7468 6520  am to which the 
-00016620: 6465 6275 6720 6f75 7470 7574 2073 686f  debug output sho
-00016630: 756c 6420 6265 0a20 2020 2020 2020 2020  uld be.         
-00016640: 2020 2020 2020 2077 7269 7474 656e 2e20         written. 
-00016650: 5468 6973 2069 7320 6e6f 7420 6775 6172  This is not guar
-00016660: 616e 7465 6564 2074 6f20 6265 2073 6565  anteed to be see
-00016670: 6b61 626c 6520 2865 2e67 2e20 6974 206d  kable (e.g. it m
-00016680: 6179 2062 6520 7374 646f 7574 206f 720a  ay be stdout or.
-00016690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166a0: 7374 6465 7272 292e 0a20 2020 2020 2020  stderr)..       
-000166b0: 2020 2020 2070 6678 2028 7374 7229 3a20       pfx (str): 
-000166c0: 7468 6520 6375 7272 656e 7420 6465 6275  the current debu
-000166d0: 6720 6f75 7470 7574 2070 7265 6669 7820  g output prefix 
-000166e0: 7374 7269 6e67 2028 6f6e 6c79 206e 6565  string (only nee
-000166f0: 6465 6420 6966 2065 6d69 7474 696e 670a  ded if emitting.
-00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016710: 6d6f 7265 2074 6861 6e20 6f6e 6520 6c69  more than one li
-00016720: 6e65 292e 0a0a 2020 2020 2020 2020 5265  ne)...        Re
-00016730: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00016740: 2020 2054 6865 2073 616d 6520 7475 706c     The same tupl
-00016750: 6520 6173 2060 5265 6374 616e 676c 652e  e as `Rectangle.
-00016760: 7265 6e64 6572 602e 0a20 2020 2020 2020  render`..       
-00016770: 2022 2222 0a20 2020 2020 2020 2023 2070   """.        # p
-00016780: 796c 696e 743a 2064 6973 6162 6c65 3d75  ylint: disable=u
-00016790: 6e75 7365 642d 6172 6775 6d65 6e74 0a20  nused-argument. 
-000167a0: 2020 2020 2020 2072 656e 6465 7265 642c         rendered,
-000167b0: 2072 6573 6f6c 7665 642c 2069 6e69 7469   resolved, initi
-000167c0: 616c 5f70 6f69 6e74 203d 2073 656c 662e  al_point = self.
-000167d0: 7265 6e64 6572 280a 2020 2020 2020 2020  render(.        
-000167e0: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
-000167f0: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
-00016800: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
-00016810: 740a 2020 2020 2020 2020 290a 2020 2020  t.        ).    
-00016820: 2020 2020 6465 6275 675f 7374 7265 616d      debug_stream
-00016830: 2e77 7269 7465 2866 227b 7365 6c66 7d20  .write(f"{self} 
-00016840: 7265 736f 6c76 6564 2074 6f20 7b72 656e  resolved to {ren
-00016850: 6465 7265 647d 5c6e 2229 0a0a 2020 2020  dered}\n")..    
-00016860: 2020 2020 7265 7475 726e 2072 656e 6465      return rende
-00016870: 7265 642c 2072 6573 6f6c 7665 642c 2069  red, resolved, i
-00016880: 6e69 7469 616c 5f70 6f69 6e74 0a0a 0a63  nitial_point...c
-00016890: 6c61 7373 2052 6f75 6e64 6564 5265 6374  lass RoundedRect
-000168a0: 616e 676c 6528 4e61 6d65 6454 7570 6c65  angle(NamedTuple
-000168b0: 293a 0a20 2020 2022 2222 0a20 2020 2041  ):.    """.    A
-000168c0: 2072 6563 7461 6e67 6c65 2077 6974 6820   rectangle with 
-000168d0: 726f 756e 6465 6420 636f 726e 6572 732e  rounded corners.
-000168e0: 0a0a 2020 2020 5365 653a 2060 5061 696e  ..    See: `Pain
-000168f0: 7465 6450 6174 682e 7265 6374 616e 676c  tedPath.rectangl
-00016900: 6560 0a20 2020 2022 2222 0a0a 2020 2020  e`.    """..    
-00016910: 6f72 673a 2050 6f69 6e74 0a20 2020 2022  org: Point.    "
-00016920: 2222 5468 6520 746f 702d 6c65 6674 2063  ""The top-left c
-00016930: 6f72 6e65 7220 6f66 2074 6865 2072 6563  orner of the rec
-00016940: 7461 6e67 6c65 2e22 2222 0a20 2020 2073  tangle.""".    s
-00016950: 697a 653a 2050 6f69 6e74 0a20 2020 2022  ize: Point.    "
-00016960: 2222 5468 6520 7769 6474 6820 616e 6420  ""The width and 
-00016970: 6865 6967 6874 206f 6620 7468 6520 7265  height of the re
-00016980: 6374 616e 676c 652e 2222 220a 2020 2020  ctangle.""".    
-00016990: 636f 726e 6572 5f72 6164 6969 3a20 506f  corner_radii: Po
-000169a0: 696e 740a 2020 2020 2222 2254 6865 2078  int.    """The x
-000169b0: 2d20 616e 6420 792d 7261 6469 7573 206f  - and y-radius o
-000169c0: 6620 7468 6520 636f 726e 6572 732e 2222  f the corners.""
-000169d0: 220a 0a20 2020 2064 6566 205f 6465 636f  "..    def _deco
-000169e0: 6d70 6f73 6528 7365 6c66 293a 0a20 2020  mpose(self):.   
-000169f0: 2020 2020 2069 7465 6d73 203d 205b 5d0a       items = [].
-00016a00: 0a20 2020 2020 2020 2069 6620 2873 656c  .        if (sel
-00016a10: 662e 7369 7a65 2e78 203d 3d20 3029 2061  f.size.x == 0) a
-00016a20: 6e64 2028 7365 6c66 2e73 697a 652e 7920  nd (self.size.y 
-00016a30: 3d3d 2030 293a 0a20 2020 2020 2020 2020  == 0):.         
-00016a40: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00016a50: 656c 6966 2028 7365 6c66 2e73 697a 652e  elif (self.size.
-00016a60: 7820 3d3d 2030 2920 6f72 2028 7365 6c66  x == 0) or (self
-00016a70: 2e73 697a 652e 7920 3d3d 2030 293a 0a20  .size.y == 0):. 
-00016a80: 2020 2020 2020 2020 2020 2069 7465 6d73             items
-00016a90: 2e61 7070 656e 6428 4d6f 7665 2873 656c  .append(Move(sel
-00016aa0: 662e 6f72 6729 290a 2020 2020 2020 2020  f.org)).        
-00016ab0: 2020 2020 6974 656d 732e 6170 7065 6e64      items.append
-00016ac0: 284c 696e 6528 7365 6c66 2e6f 7267 202b  (Line(self.org +
-00016ad0: 2073 656c 662e 7369 7a65 2929 0a20 2020   self.size)).   
-00016ae0: 2020 2020 2020 2020 2069 7465 6d73 2e61           items.a
-00016af0: 7070 656e 6428 436c 6f73 6528 2929 0a20  ppend(Close()). 
-00016b00: 2020 2020 2020 2065 6c69 6620 2873 656c         elif (sel
-00016b10: 662e 636f 726e 6572 5f72 6164 6969 2e78  f.corner_radii.x
-00016b20: 203d 3d20 3029 206f 7220 2873 656c 662e   == 0) or (self.
-00016b30: 636f 726e 6572 5f72 6164 6969 2e79 203d  corner_radii.y =
-00016b40: 3d20 3029 3a0a 2020 2020 2020 2020 2020  = 0):.          
-00016b50: 2020 6974 656d 732e 6170 7065 6e64 2852    items.append(R
-00016b60: 6563 7461 6e67 6c65 2873 656c 662e 6f72  ectangle(self.or
-00016b70: 672c 2073 656c 662e 7369 7a65 2929 0a20  g, self.size)). 
-00016b80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00016b90: 2020 2020 2020 2020 2078 2c20 7920 3d20           x, y = 
-00016ba0: 7365 6c66 2e6f 7267 0a20 2020 2020 2020  self.org.       
-00016bb0: 2020 2020 2077 2c20 6820 3d20 7365 6c66       w, h = self
-00016bc0: 2e73 697a 650a 2020 2020 2020 2020 2020  .size.          
-00016bd0: 2020 7278 2c20 7279 203d 2073 656c 662e    rx, ry = self.
-00016be0: 636f 726e 6572 5f72 6164 6969 0a20 2020  corner_radii.   
-00016bf0: 2020 2020 2020 2020 2073 6967 6e5f 7769           sign_wi
-00016c00: 6474 6820 3d20 2873 656c 662e 7369 7a65  dth = (self.size
-00016c10: 2e78 203e 3d20 3029 202d 2028 7365 6c66  .x >= 0) - (self
-00016c20: 2e73 697a 652e 7820 3c20 3029 0a20 2020  .size.x < 0).   
-00016c30: 2020 2020 2020 2020 2073 6967 6e5f 6865           sign_he
-00016c40: 6967 6874 203d 2028 7365 6c66 2e73 697a  ight = (self.siz
-00016c50: 652e 7920 3e3d 2030 2920 2d20 2873 656c  e.y >= 0) - (sel
-00016c60: 662e 7369 7a65 2e79 203c 2030 290a 0a20  f.size.y < 0).. 
-00016c70: 2020 2020 2020 2020 2020 2069 6620 6162             if ab
-00016c80: 7328 7278 2920 3e20 6162 7328 7729 3a0a  s(rx) > abs(w):.
-00016c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ca0: 7278 203d 2073 656c 662e 7369 7a65 2e78  rx = self.size.x
-00016cb0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00016cc0: 2061 6273 2872 7929 203e 2061 6273 2868   abs(ry) > abs(h
-00016cd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00016ce0: 2020 2072 7920 3d20 7365 6c66 2e73 697a     ry = self.siz
-00016cf0: 652e 790a 0a20 2020 2020 2020 2020 2020  e.y..           
-00016d00: 2072 7820 3d20 7369 676e 5f77 6964 7468   rx = sign_width
-00016d10: 202a 2061 6273 2872 7829 0a20 2020 2020   * abs(rx).     
-00016d20: 2020 2020 2020 2072 7920 3d20 7369 676e         ry = sign
-00016d30: 5f68 6569 6768 7420 2a20 6162 7328 7279  _height * abs(ry
-00016d40: 290a 2020 2020 2020 2020 2020 2020 6172  ).            ar
-00016d50: 635f 7261 6420 3d20 506f 696e 7428 7278  c_rad = Point(rx
-00016d60: 2c20 7279 290a 0a20 2020 2020 2020 2020  , ry)..         
-00016d70: 2020 2069 7465 6d73 2e61 7070 656e 6428     items.append(
-00016d80: 4d6f 7665 2850 6f69 6e74 2878 202b 2072  Move(Point(x + r
-00016d90: 782c 2079 2929 290a 2020 2020 2020 2020  x, y))).        
-00016da0: 2020 2020 6974 656d 732e 6170 7065 6e64      items.append
-00016db0: 284c 696e 6528 506f 696e 7428 7820 2b20  (Line(Point(x + 
-00016dc0: 7720 2d20 7278 2c20 7929 2929 0a20 2020  w - rx, y))).   
-00016dd0: 2020 2020 2020 2020 2069 7465 6d73 2e61           items.a
-00016de0: 7070 656e 6428 4172 6328 6172 635f 7261  ppend(Arc(arc_ra
-00016df0: 642c 2030 2c20 4661 6c73 652c 2054 7275  d, 0, False, Tru
-00016e00: 652c 2050 6f69 6e74 2878 202b 2077 2c20  e, Point(x + w, 
-00016e10: 7920 2b20 7279 2929 290a 2020 2020 2020  y + ry))).      
-00016e20: 2020 2020 2020 6974 656d 732e 6170 7065        items.appe
-00016e30: 6e64 284c 696e 6528 506f 696e 7428 7820  nd(Line(Point(x 
-00016e40: 2b20 772c 2079 202b 2068 202d 2072 7929  + w, y + h - ry)
-00016e50: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
-00016e60: 7465 6d73 2e61 7070 656e 6428 4172 6328  tems.append(Arc(
-00016e70: 6172 635f 7261 642c 2030 2c20 4661 6c73  arc_rad, 0, Fals
-00016e80: 652c 2054 7275 652c 2050 6f69 6e74 2878  e, True, Point(x
-00016e90: 202b 2077 202d 2072 782c 2079 202b 2068   + w - rx, y + h
+00012540: 2020 2020 2020 2072 6574 7572 6e20 280a         return (.
+00012550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012560: 2e74 6f5f 6375 6269 635f 6375 7276 6528  .to_cubic_curve(
+00012570: 6c61 7374 5f69 7465 6d2e 656e 645f 706f  last_item.end_po
+00012580: 696e 7429 2e72 656e 6465 7228 0a20 2020  int).render(.   
+00012590: 2020 2020 2020 2020 2020 2020 2067 7364               gsd
+000125a0: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
+000125b0: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
+000125c0: 7469 616c 5f70 6f69 6e74 0a20 2020 2020  tial_point.     
+000125d0: 2020 2020 2020 2029 5b30 5d2c 0a20 2020         )[0],.   
+000125e0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+000125f0: 2020 2020 2020 2020 2020 2069 6e69 7469             initi
+00012600: 616c 5f70 6f69 6e74 2c0a 2020 2020 2020  al_point,.      
+00012610: 2020 290a 0a20 2020 2040 666f 7263 655f    )..    @force_
+00012620: 6e6f 646f 6375 6d65 6e74 0a20 2020 2064  nodocument.    d
+00012630: 6566 2072 656e 6465 725f 6465 6275 6728  ef render_debug(
+00012640: 0a20 2020 2020 2020 2073 656c 662c 2067  .        self, g
+00012650: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
+00012660: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
+00012670: 6e69 7469 616c 5f70 6f69 6e74 2c20 6465  nitial_point, de
+00012680: 6275 675f 7374 7265 616d 2c20 7066 780a  bug_stream, pfx.
+00012690: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+000126a0: 2222 0a20 2020 2020 2020 2052 656e 6465  "".        Rende
+000126b0: 7220 7468 6973 2070 6174 6820 656c 656d  r this path elem
+000126c0: 656e 7420 746f 2069 7473 2050 4446 2072  ent to its PDF r
+000126d0: 6570 7265 7365 6e74 6174 696f 6e20 616e  epresentation an
+000126e0: 6420 7072 6f64 7563 6520 6465 6275 670a  d produce debug.
+000126f0: 2020 2020 2020 2020 696e 666f 726d 6174          informat
+00012700: 696f 6e2e 0a0a 2020 2020 2020 2020 4172  ion...        Ar
+00012710: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00012720: 6773 645f 7265 6769 7374 7279 2028 4772  gsd_registry (Gr
+00012730: 6170 6869 6373 5374 6174 6544 6963 7452  aphicsStateDictR
+00012740: 6567 6973 7472 7929 3a20 7468 6520 6f77  egistry): the ow
+00012750: 6e65 7227 7320 6772 6170 6869 6373 2073  ner's graphics s
+00012760: 7461 7465 0a20 2020 2020 2020 2020 2020  tate.           
+00012770: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
+00012780: 7265 6769 7374 7279 2e0a 2020 2020 2020  registry..      
+00012790: 2020 2020 2020 7374 796c 6520 2847 7261        style (Gra
+000127a0: 7068 6963 7353 7479 6c65 293a 2074 6865  phicsStyle): the
+000127b0: 2063 7572 7265 6e74 2072 6573 6f6c 7665   current resolve
+000127c0: 6420 6772 6170 6869 6373 2073 7479 6c65  d graphics style
+000127d0: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
+000127e0: 745f 6974 656d 3a20 7468 6520 7072 6576  t_item: the prev
+000127f0: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
+00012800: 742e 0a20 2020 2020 2020 2020 2020 2069  t..            i
+00012810: 6e69 7469 616c 5f70 6f69 6e74 3a20 6c61  nitial_point: la
+00012820: 7374 2070 6f73 6974 696f 6e20 7365 7420  st position set 
+00012830: 6279 2061 2022 4d22 206f 7220 226d 2220  by a "M" or "m" 
+00012840: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
+00012850: 2020 2020 6465 6275 675f 7374 7265 616d      debug_stream
+00012860: 2028 696f 2e54 6578 7449 4f29 3a20 7468   (io.TextIO): th
+00012870: 6520 7374 7265 616d 2074 6f20 7768 6963  e stream to whic
+00012880: 6820 7468 6520 6465 6275 6720 6f75 7470  h the debug outp
+00012890: 7574 2073 686f 756c 6420 6265 0a20 2020  ut should be.   
+000128a0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+000128b0: 7474 656e 2e20 5468 6973 2069 7320 6e6f  tten. This is no
+000128c0: 7420 6775 6172 616e 7465 6564 2074 6f20  t guaranteed to 
+000128d0: 6265 2073 6565 6b61 626c 6520 2865 2e67  be seekable (e.g
+000128e0: 2e20 6974 206d 6179 2062 6520 7374 646f  . it may be stdo
+000128f0: 7574 206f 720a 2020 2020 2020 2020 2020  ut or.          
+00012900: 2020 2020 2020 7374 6465 7272 292e 0a20        stderr).. 
+00012910: 2020 2020 2020 2020 2020 2070 6678 2028             pfx (
+00012920: 7374 7229 3a20 7468 6520 6375 7272 656e  str): the curren
+00012930: 7420 6465 6275 6720 6f75 7470 7574 2070  t debug output p
+00012940: 7265 6669 7820 7374 7269 6e67 2028 6f6e  refix string (on
+00012950: 6c79 206e 6565 6465 6420 6966 2065 6d69  ly needed if emi
+00012960: 7474 696e 670a 2020 2020 2020 2020 2020  tting.          
+00012970: 2020 2020 2020 6d6f 7265 2074 6861 6e20        more than 
+00012980: 6f6e 6520 6c69 6e65 292e 0a0a 2020 2020  one line)...    
+00012990: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000129a0: 2020 2020 2020 2020 2054 6865 2073 616d           The sam
+000129b0: 6520 7475 706c 6520 6173 2060 5175 6164  e tuple as `Quad
+000129c0: 7261 7469 6342 657a 6965 7243 7572 7665  raticBezierCurve
+000129d0: 2e72 656e 6465 7260 2e0a 2020 2020 2020  .render`..      
+000129e0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+000129f0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00012a00: 756e 7573 6564 2d61 7267 756d 656e 740a  unused-argument.
+00012a10: 2020 2020 2020 2020 7265 6e64 6572 6564          rendered
+00012a20: 2c20 7265 736f 6c76 6564 2c20 696e 6974  , resolved, init
+00012a30: 6961 6c5f 706f 696e 7420 3d20 7365 6c66  ial_point = self
+00012a40: 2e72 656e 6465 7228 0a20 2020 2020 2020  .render(.       
+00012a50: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
+00012a60: 792c 2073 7479 6c65 2c20 6c61 7374 5f69  y, style, last_i
+00012a70: 7465 6d2c 2069 6e69 7469 616c 5f70 6f69  tem, initial_poi
+00012a80: 6e74 0a20 2020 2020 2020 2029 0a20 2020  nt.        ).   
+00012a90: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+00012aa0: 6d2e 7772 6974 6528 0a20 2020 2020 2020  m.write(.       
+00012ab0: 2020 2020 2066 227b 7365 6c66 7d20 7265       f"{self} re
+00012ac0: 736f 6c76 6564 2074 6f20 7b73 656c 662e  solved to {self.
+00012ad0: 746f 5f63 7562 6963 5f63 7572 7665 286c  to_cubic_curve(l
+00012ae0: 6173 745f 6974 656d 2e65 6e64 5f70 6f69  ast_item.end_poi
+00012af0: 6e74 297d 5c6e 220a 2020 2020 2020 2020  nt)}\n".        
+00012b00: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00012b10: 6e20 7265 6e64 6572 6564 2c20 7265 736f  n rendered, reso
+00012b20: 6c76 6564 2c20 696e 6974 6961 6c5f 706f  lved, initial_po
+00012b30: 696e 740a 0a0a 636c 6173 7320 5265 6c61  int...class Rela
+00012b40: 7469 7665 5175 6164 7261 7469 6342 657a  tiveQuadraticBez
+00012b50: 6965 7243 7572 7665 284e 616d 6564 5475  ierCurve(NamedTu
+00012b60: 706c 6529 3a0a 2020 2020 2222 220a 2020  ple):.    """.  
+00012b70: 2020 4120 7175 6164 7261 7469 6320 42c3    A quadratic B.
+00012b80: a97a 6965 7220 6375 7276 6520 7061 7468  .zier curve path
+00012b90: 2065 6c65 6d65 6e74 2077 686f 7365 2070   element whose p
+00012ba0: 6f69 6e74 7320 6172 6520 7370 6563 6966  oints are specif
+00012bb0: 6965 6420 7265 6c61 7469 7665 2074 6f20  ied relative to 
+00012bc0: 7468 6520 656e 640a 2020 2020 706f 696e  the end.    poin
+00012bd0: 7420 6f66 2074 6865 2070 7265 7669 6f75  t of the previou
+00012be0: 7320 7061 7468 2065 6c65 6d65 6e74 2e0a  s path element..
+00012bf0: 0a20 2020 2053 6565 3a20 6050 6169 6e74  .    See: `Paint
+00012c00: 6564 5061 7468 2e71 7561 6472 6174 6963  edPath.quadratic
+00012c10: 5f63 7572 7665 5f72 656c 6174 6976 6560  _curve_relative`
+00012c20: 0a20 2020 2022 2222 0a0a 2020 2020 6374  .    """..    ct
+00012c30: 726c 3a20 506f 696e 740a 2020 2020 2222  rl: Point.    ""
+00012c40: 2254 6865 2063 7572 7665 2773 2063 6f6e  "The curve's con
+00012c50: 7472 6f6c 2070 6f69 6e74 2072 656c 6174  trol point relat
+00012c60: 6976 6520 746f 2074 6865 2065 6e64 206f  ive to the end o
+00012c70: 6620 7468 6520 7072 6576 696f 7573 2070  f the previous p
+00012c80: 6174 6820 656c 656d 656e 742e 2222 220a  ath element.""".
+00012c90: 2020 2020 656e 643a 2050 6f69 6e74 0a20      end: Point. 
+00012ca0: 2020 2022 2222 5468 6520 6375 7276 6527     """The curve'
+00012cb0: 7320 656e 6420 706f 696e 7420 7265 6c61  s end point rela
+00012cc0: 7469 7665 2074 6f20 7468 6520 656e 6420  tive to the end 
+00012cd0: 6f66 2074 6865 2070 7265 7669 6f75 7320  of the previous 
+00012ce0: 7061 7468 2065 6c65 6d65 6e74 2e22 2222  path element."""
+00012cf0: 0a0a 2020 2020 4066 6f72 6365 5f6e 6f64  ..    @force_nod
+00012d00: 6f63 756d 656e 740a 2020 2020 6465 6620  ocument.    def 
+00012d10: 7265 6e64 6572 2873 656c 662c 2067 7364  render(self, gsd
+00012d20: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
+00012d30: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
+00012d40: 7469 616c 5f70 6f69 6e74 293a 0a20 2020  tial_point):.   
+00012d50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012d60: 2052 656e 6465 7220 7468 6973 2070 6174   Render this pat
+00012d70: 6820 656c 656d 656e 7420 746f 2069 7473  h element to its
+00012d80: 2050 4446 2072 6570 7265 7365 6e74 6174   PDF representat
+00012d90: 696f 6e2e 0a0a 2020 2020 2020 2020 4172  ion...        Ar
+00012da0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00012db0: 6773 645f 7265 6769 7374 7279 2028 4772  gsd_registry (Gr
+00012dc0: 6170 6869 6373 5374 6174 6544 6963 7452  aphicsStateDictR
+00012dd0: 6567 6973 7472 7929 3a20 7468 6520 6f77  egistry): the ow
+00012de0: 6e65 7227 7320 6772 6170 6869 6373 2073  ner's graphics s
+00012df0: 7461 7465 0a20 2020 2020 2020 2020 2020  tate.           
+00012e00: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
+00012e10: 7265 6769 7374 7279 2e0a 2020 2020 2020  registry..      
+00012e20: 2020 2020 2020 7374 796c 6520 2847 7261        style (Gra
+00012e30: 7068 6963 7353 7479 6c65 293a 2074 6865  phicsStyle): the
+00012e40: 2063 7572 7265 6e74 2072 6573 6f6c 7665   current resolve
+00012e50: 6420 6772 6170 6869 6373 2073 7479 6c65  d graphics style
+00012e60: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
+00012e70: 745f 6974 656d 3a20 7468 6520 7072 6576  t_item: the prev
+00012e80: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
+00012e90: 742e 0a20 2020 2020 2020 2020 2020 2069  t..            i
+00012ea0: 6e69 7469 616c 5f70 6f69 6e74 3a20 6c61  nitial_point: la
+00012eb0: 7374 2070 6f73 6974 696f 6e20 7365 7420  st position set 
+00012ec0: 6279 2061 2022 4d22 206f 7220 226d 2220  by a "M" or "m" 
+00012ed0: 636f 6d6d 616e 640a 0a20 2020 2020 2020  command..       
+00012ee0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00012ef0: 2020 2020 2020 6120 7475 706c 6520 6f66        a tuple of
+00012f00: 2060 2873 7472 2c20 6e65 775f 6c61 7374   `(str, new_last
+00012f10: 5f69 7465 6d29 602c 2077 6865 7265 2060  _item)`, where `
+00012f20: 6e65 775f 6c61 7374 5f69 7465 6d60 2069  new_last_item` i
+00012f30: 7320 7468 6520 7265 736f 6c76 6564 0a20  s the resolved. 
+00012f40: 2020 2020 2020 2020 2020 2060 5175 6164             `Quad
+00012f50: 7261 7469 6342 657a 6965 7243 7572 7665  raticBezierCurve
+00012f60: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
+00012f70: 2020 2020 2020 206c 6173 745f 706f 696e         last_poin
+00012f80: 7420 3d20 6c61 7374 5f69 7465 6d2e 656e  t = last_item.en
+00012f90: 645f 706f 696e 740a 0a20 2020 2020 2020  d_point..       
+00012fa0: 2063 7472 6c20 3d20 6c61 7374 5f70 6f69   ctrl = last_poi
+00012fb0: 6e74 202b 2073 656c 662e 6374 726c 0a20  nt + self.ctrl. 
+00012fc0: 2020 2020 2020 2065 6e64 203d 206c 6173         end = las
+00012fd0: 745f 706f 696e 7420 2b20 7365 6c66 2e65  t_point + self.e
+00012fe0: 6e64 0a0a 2020 2020 2020 2020 6162 736f  nd..        abso
+00012ff0: 6c75 7465 203d 2051 7561 6472 6174 6963  lute = Quadratic
+00013000: 4265 7a69 6572 4375 7276 6528 6374 726c  BezierCurve(ctrl
+00013010: 3d63 7472 6c2c 2065 6e64 3d65 6e64 290a  =ctrl, end=end).
+00013020: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00013030: 6273 6f6c 7574 652e 7265 6e64 6572 2867  bsolute.render(g
+00013040: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
+00013050: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
+00013060: 6e69 7469 616c 5f70 6f69 6e74 290a 0a20  nitial_point).. 
+00013070: 2020 2040 666f 7263 655f 6e6f 646f 6375     @force_nodocu
+00013080: 6d65 6e74 0a20 2020 2064 6566 2072 656e  ment.    def ren
+00013090: 6465 725f 6465 6275 6728 0a20 2020 2020  der_debug(.     
+000130a0: 2020 2073 656c 662c 2067 7364 5f72 6567     self, gsd_reg
+000130b0: 6973 7472 792c 2073 7479 6c65 2c20 6c61  istry, style, la
+000130c0: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
+000130d0: 5f70 6f69 6e74 2c20 6465 6275 675f 7374  _point, debug_st
+000130e0: 7265 616d 2c20 7066 780a 2020 2020 293a  ream, pfx.    ):
+000130f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013100: 2020 2020 2052 656e 6465 7220 7468 6973       Render this
+00013110: 2070 6174 6820 656c 656d 656e 7420 746f   path element to
+00013120: 2069 7473 2050 4446 2072 6570 7265 7365   its PDF represe
+00013130: 6e74 6174 696f 6e20 616e 6420 7072 6f64  ntation and prod
+00013140: 7563 6520 6465 6275 670a 2020 2020 2020  uce debug.      
+00013150: 2020 696e 666f 726d 6174 696f 6e2e 0a0a    information...
+00013160: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00013170: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
+00013180: 6769 7374 7279 2028 4772 6170 6869 6373  gistry (Graphics
+00013190: 5374 6174 6544 6963 7452 6567 6973 7472  StateDictRegistr
+000131a0: 7929 3a20 7468 6520 6f77 6e65 7227 7320  y): the owner's 
+000131b0: 6772 6170 6869 6373 2073 7461 7465 0a20  graphics state. 
+000131c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000131d0: 6963 7469 6f6e 6172 7920 7265 6769 7374  ictionary regist
+000131e0: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
+000131f0: 7374 796c 6520 2847 7261 7068 6963 7353  style (GraphicsS
+00013200: 7479 6c65 293a 2074 6865 2063 7572 7265  tyle): the curre
+00013210: 6e74 2072 6573 6f6c 7665 6420 6772 6170  nt resolved grap
+00013220: 6869 6373 2073 7479 6c65 0a20 2020 2020  hics style.     
+00013230: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
+00013240: 3a20 7468 6520 7072 6576 696f 7573 2070  : the previous p
+00013250: 6174 6820 656c 656d 656e 742e 0a20 2020  ath element..   
+00013260: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
+00013270: 5f70 6f69 6e74 3a20 6c61 7374 2070 6f73  _point: last pos
+00013280: 6974 696f 6e20 7365 7420 6279 2061 2022  ition set by a "
+00013290: 4d22 206f 7220 226d 2220 636f 6d6d 616e  M" or "m" comman
+000132a0: 640a 2020 2020 2020 2020 2020 2020 6465  d.            de
+000132b0: 6275 675f 7374 7265 616d 2028 696f 2e54  bug_stream (io.T
+000132c0: 6578 7449 4f29 3a20 7468 6520 7374 7265  extIO): the stre
+000132d0: 616d 2074 6f20 7768 6963 6820 7468 6520  am to which the 
+000132e0: 6465 6275 6720 6f75 7470 7574 2073 686f  debug output sho
+000132f0: 756c 6420 6265 0a20 2020 2020 2020 2020  uld be.         
+00013300: 2020 2020 2020 2077 7269 7474 656e 2e20         written. 
+00013310: 5468 6973 2069 7320 6e6f 7420 6775 6172  This is not guar
+00013320: 616e 7465 6564 2074 6f20 6265 2073 6565  anteed to be see
+00013330: 6b61 626c 6520 2865 2e67 2e20 6974 206d  kable (e.g. it m
+00013340: 6179 2062 6520 7374 646f 7574 206f 720a  ay be stdout or.
+00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013360: 7374 6465 7272 292e 0a20 2020 2020 2020  stderr)..       
+00013370: 2020 2020 2070 6678 2028 7374 7229 3a20       pfx (str): 
+00013380: 7468 6520 6375 7272 656e 7420 6465 6275  the current debu
+00013390: 6720 6f75 7470 7574 2070 7265 6669 7820  g output prefix 
+000133a0: 7374 7269 6e67 2028 6f6e 6c79 206e 6565  string (only nee
+000133b0: 6465 6420 6966 2065 6d69 7474 696e 670a  ded if emitting.
+000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133d0: 6d6f 7265 2074 6861 6e20 6f6e 6520 6c69  more than one li
+000133e0: 6e65 292e 0a0a 2020 2020 2020 2020 5265  ne)...        Re
+000133f0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00013400: 2020 2054 6865 2073 616d 6520 7475 706c     The same tupl
+00013410: 6520 6173 2060 5265 6c61 7469 7665 5175  e as `RelativeQu
+00013420: 6164 7261 7469 6342 657a 6965 7243 7572  adraticBezierCur
+00013430: 7665 2e72 656e 6465 7260 2e0a 2020 2020  ve.render`..    
+00013440: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013450: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+00013460: 653d 756e 7573 6564 2d61 7267 756d 656e  e=unused-argumen
+00013470: 740a 2020 2020 2020 2020 7265 6e64 6572  t.        render
+00013480: 6564 2c20 7265 736f 6c76 6564 2c20 696e  ed, resolved, in
+00013490: 6974 6961 6c5f 706f 696e 7420 3d20 7365  itial_point = se
+000134a0: 6c66 2e72 656e 6465 7228 0a20 2020 2020  lf.render(.     
+000134b0: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
+000134c0: 7472 792c 2073 7479 6c65 2c20 6c61 7374  try, style, last
+000134d0: 5f69 7465 6d2c 2069 6e69 7469 616c 5f70  _item, initial_p
+000134e0: 6f69 6e74 0a20 2020 2020 2020 2029 0a20  oint.        ). 
+000134f0: 2020 2020 2020 2064 6562 7567 5f73 7472         debug_str
+00013500: 6561 6d2e 7772 6974 6528 0a20 2020 2020  eam.write(.     
+00013510: 2020 2020 2020 2066 227b 7365 6c66 7d20         f"{self} 
+00013520: 7265 736f 6c76 6564 2074 6f20 7b72 6573  resolved to {res
+00013530: 6f6c 7665 647d 2022 0a20 2020 2020 2020  olved} ".       
+00013540: 2020 2020 2066 2274 6865 6e20 746f 207b       f"then to {
+00013550: 7265 736f 6c76 6564 2e74 6f5f 6375 6269  resolved.to_cubi
+00013560: 635f 6375 7276 6528 6c61 7374 5f69 7465  c_curve(last_ite
+00013570: 6d2e 656e 645f 706f 696e 7429 7d5c 6e22  m.end_point)}\n"
+00013580: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00013590: 2020 2020 7265 7475 726e 2072 656e 6465      return rende
+000135a0: 7265 642c 2072 6573 6f6c 7665 642c 2069  red, resolved, i
+000135b0: 6e69 7469 616c 5f70 6f69 6e74 0a0a 0a63  nitial_point...c
+000135c0: 6c61 7373 2041 7263 284e 616d 6564 5475  lass Arc(NamedTu
+000135d0: 706c 6529 3a0a 2020 2020 2222 220a 2020  ple):.    """.  
+000135e0: 2020 416e 2065 6c6c 6970 7469 6361 6c20    An elliptical 
+000135f0: 6172 6320 7061 7468 2065 6c65 6d65 6e74  arc path element
+00013600: 2e0a 0a20 2020 2054 6865 2061 7263 2069  ...    The arc i
+00013610: 7320 6472 6177 6e20 6672 6f6d 2074 6865  s drawn from the
+00013620: 2065 6e64 206f 6620 7468 6520 6375 7272   end of the curr
+00013630: 656e 7420 7061 7468 2065 6c65 6d65 6e74  ent path element
+00013640: 2074 6f20 6974 7320 7370 6563 6966 6965   to its specifie
+00013650: 6420 656e 6420 706f 696e 740a 2020 2020  d end point.    
+00013660: 7573 696e 6720 6120 6e75 6d62 6572 206f  using a number o
+00013670: 6620 7061 7261 6d65 7465 7273 2074 6f20  f parameters to 
+00013680: 6465 7465 726d 696e 6520 686f 7720 6974  determine how it
+00013690: 2069 7320 636f 6e73 7472 7563 7465 642e   is constructed.
+000136a0: 0a0a 2020 2020 5365 653a 2060 5061 696e  ..    See: `Pain
+000136b0: 7465 6450 6174 682e 6172 635f 746f 600a  tedPath.arc_to`.
+000136c0: 2020 2020 2222 220a 0a20 2020 2072 6164      """..    rad
+000136d0: 6969 3a20 506f 696e 740a 2020 2020 2222  ii: Point.    ""
+000136e0: 220a 2020 2020 5468 6520 782d 2061 6e64  ".    The x- and
+000136f0: 2079 2d72 6164 6969 206f 6620 7468 6520   y-radii of the 
+00013700: 6172 632e 2049 6620 6072 6164 6969 2e78  arc. If `radii.x
+00013710: 203d 3d20 7261 6469 692e 7960 2074 6865   == radii.y` the
+00013720: 2061 7263 2077 696c 6c20 6265 2063 6972   arc will be cir
+00013730: 6375 6c61 722e 0a20 2020 2022 2222 0a20  cular..    """. 
+00013740: 2020 2072 6f74 6174 696f 6e3a 204e 756d     rotation: Num
+00013750: 6265 720a 2020 2020 2222 2254 6865 2072  ber.    """The r
+00013760: 6f74 6174 696f 6e20 6f66 2074 6865 2061  otation of the a
+00013770: 7263 2773 206d 616a 6f72 2f6d 696e 6f72  rc's major/minor
+00013780: 2061 7865 7320 7265 6c61 7469 7665 2074   axes relative t
+00013790: 6f20 7468 6520 636f 6f72 6469 6e61 7465  o the coordinate
+000137a0: 2066 7261 6d65 2e22 2222 0a20 2020 206c   frame.""".    l
+000137b0: 6172 6765 3a20 626f 6f6c 0a20 2020 2022  arge: bool.    "
+000137c0: 2222 4966 2054 7275 652c 2073 7765 6570  ""If True, sweep
+000137d0: 2074 6865 2061 7263 206f 7665 7220 616e   the arc over an
+000137e0: 2061 6e67 6c65 2067 7265 6174 6572 2074   angle greater t
+000137f0: 6861 6e20 6f72 2065 7175 616c 2074 6f20  han or equal to 
+00013800: 3138 3020 6465 6772 6565 732e 2222 220a  180 degrees.""".
+00013810: 2020 2020 7377 6565 703a 2062 6f6f 6c0a      sweep: bool.
+00013820: 2020 2020 2222 2249 6620 5472 7565 2c20      """If True, 
+00013830: 7468 6520 6172 6320 6973 2073 7765 7074  the arc is swept
+00013840: 2069 6e20 7468 6520 706f 7369 7469 7665   in the positive
+00013850: 2061 6e67 756c 6172 2064 6972 6563 7469   angular directi
+00013860: 6f6e 2e22 2222 0a20 2020 2065 6e64 3a20  on.""".    end: 
+00013870: 506f 696e 740a 2020 2020 2222 2254 6865  Point.    """The
+00013880: 2065 6e64 2070 6f69 6e74 206f 6620 7468   end point of th
+00013890: 6520 6172 632e 2222 220a 0a20 2020 2040  e arc."""..    @
+000138a0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+000138b0: 2040 666f 7263 655f 6e6f 646f 6375 6d65   @force_nodocume
+000138c0: 6e74 0a20 2020 2064 6566 2073 7562 6469  nt.    def subdi
+000138d0: 7664 655f 7377 6565 7028 7377 6565 705f  vde_sweep(sweep_
+000138e0: 616e 676c 6529 3a0a 2020 2020 2020 2020  angle):.        
+000138f0: 2222 220a 2020 2020 2020 2020 4120 6765  """.        A ge
+00013900: 6e65 7261 746f 7220 7468 6174 2073 7562  nerator that sub
+00013910: 6469 7669 6465 7320 6120 7377 6570 7420  divides a swept 
+00013920: 616e 676c 6520 696e 746f 2073 6567 6d65  angle into segme
+00013930: 6e74 7320 6e6f 206c 6172 6765 7220 7468  nts no larger th
+00013940: 616e 2061 2071 7561 7274 6572 0a20 2020  an a quarter.   
+00013950: 2020 2020 2074 7572 6e2e 0a0a 2020 2020       turn...    
+00013960: 2020 2020 416e 7920 7377 6565 7020 7468      Any sweep th
+00013970: 6174 2069 7320 6c61 7267 6572 2074 6861  at is larger tha
+00013980: 6e20 6120 7175 6172 7465 7220 7475 726e  n a quarter turn
+00013990: 2069 7320 7375 6264 6976 6964 6564 2069   is subdivided i
+000139a0: 6e74 6f20 6173 206d 616e 7920 6571 7561  nto as many equa
+000139b0: 6c6c 790a 2020 2020 2020 2020 7369 7a65  lly.        size
+000139c0: 6420 7365 676d 656e 7473 2061 7320 6e65  d segments as ne
+000139d0: 6365 7373 6172 7920 746f 2070 7265 7665  cessary to preve
+000139e0: 6e74 2061 6e79 2069 6e64 6976 6964 7561  nt any individua
+000139f0: 6c20 7365 676d 656e 7420 6672 6f6d 2062  l segment from b
+00013a00: 6569 6e67 206c 6172 6765 720a 2020 2020  eing larger.    
+00013a10: 2020 2020 7468 616e 2061 2071 7561 7274      than a quart
+00013a20: 6572 2074 7572 6e2e 0a0a 2020 2020 2020  er turn...      
+00013a30: 2020 5468 6973 2069 7320 7573 6564 2066    This is used f
+00013a40: 6f72 2061 7070 726f 7869 6d61 7469 6e67  or approximating
+00013a50: 2061 2063 6972 6375 6c61 7220 6375 7276   a circular curv
+00013a60: 6520 7365 676d 656e 7420 7573 696e 6720  e segment using 
+00013a70: 6375 6269 6320 42c3 a97a 6965 720a 2020  cubic B..zier.  
+00013a80: 2020 2020 2020 6375 7276 6573 2e20 5468        curves. Th
+00013a90: 6973 2063 6f6d 7075 7465 7320 7468 6520  is computes the 
+00013aa0: 7061 7261 6d65 7465 7273 2075 7365 6420  parameters used 
+00013ab0: 666f 7220 7468 6520 42c3 a97a 6965 7220  for the B..zier 
+00013ac0: 6170 7072 6f78 696d 6174 696f 6e20 7570  approximation up
+00013ad0: 0a20 2020 2020 2020 2066 726f 6e74 2c20  .        front, 
+00013ae0: 6173 2077 656c 6c20 6173 2074 6865 2074  as well as the t
+00013af0: 7261 6e73 666f 726d 206e 6563 6573 7361  ransform necessa
+00013b00: 7279 2074 6f20 706c 6163 6520 7468 6520  ry to place the 
+00013b10: 7365 676d 656e 7420 696e 2074 6865 2063  segment in the c
+00013b20: 6f72 7265 6374 0a20 2020 2020 2020 2070  orrect.        p
+00013b30: 6f73 6974 696f 6e2e 0a0a 2020 2020 2020  osition...      
+00013b40: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00013b50: 2020 2020 7377 6565 705f 616e 676c 6520      sweep_angle 
+00013b60: 284e 756d 6265 7229 3a20 7468 6520 616e  (Number): the an
+00013b70: 676c 6520 746f 2073 7562 6469 7669 6465  gle to subdivide
+00013b80: 2e0a 0a20 2020 2020 2020 2059 6965 6c64  ...        Yield
+00013b90: 733a 0a20 2020 2020 2020 2020 2020 2041  s:.            A
+00013ba0: 2074 7570 6c65 206f 6620 2863 7472 6c31   tuple of (ctrl1
+00013bb0: 2c20 6374 726c 322c 2065 6e64 2920 7265  , ctrl2, end) re
+00013bc0: 7072 6573 656e 7469 6e67 2074 6865 2063  presenting the c
+00013bd0: 6f6e 7472 6f6c 2061 6e64 2065 6e64 2070  ontrol and end p
+00013be0: 6f69 6e74 7320 6f66 0a20 2020 2020 2020  oints of.       
+00013bf0: 2020 2020 2074 6865 2063 7562 6963 2042       the cubic B
+00013c00: c3a9 7a69 6572 2063 7572 7665 2061 7070  ..zier curve app
+00013c10: 726f 7869 6d61 7469 6e67 2074 6865 2073  roximating the s
+00013c20: 6567 6d65 6e74 2061 7320 6120 756e 6974  egment as a unit
+00013c30: 2063 6972 636c 6520 6365 6e74 6572 6564   circle centered
+00013c40: 0a20 2020 2020 2020 2020 2020 2061 7420  .            at 
+00013c50: 7468 6520 6f72 6967 696e 2e0a 2020 2020  the origin..    
+00013c60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013c70: 7377 6565 705f 616e 676c 6520 3d20 6162  sweep_angle = ab
+00013c80: 7328 7377 6565 705f 616e 676c 6529 0a20  s(sweep_angle). 
+00013c90: 2020 2020 2020 2073 7765 6570 5f6c 6566         sweep_lef
+00013ca0: 7420 3d20 7377 6565 705f 616e 676c 650a  t = sweep_angle.
+00013cb0: 0a20 2020 2020 2020 2071 7561 7274 6572  .        quarter
+00013cc0: 7475 726e 203d 206d 6174 682e 7069 202f  turn = math.pi /
+00013cd0: 2032 0a20 2020 2020 2020 2063 6875 6e6b   2.        chunk
+00013ce0: 7320 3d20 6d61 7468 2e63 6569 6c28 7377  s = math.ceil(sw
+00013cf0: 6565 705f 616e 676c 6520 2f20 7175 6172  eep_angle / quar
+00013d00: 7465 7274 7572 6e29 0a0a 2020 2020 2020  terturn)..      
+00013d10: 2020 7377 6565 705f 7365 676d 656e 7420    sweep_segment 
+00013d20: 3d20 7377 6565 705f 616e 676c 6520 2f20  = sweep_angle / 
+00013d30: 6368 756e 6b73 0a20 2020 2020 2020 2063  chunks.        c
+00013d40: 6f73 5f74 203d 206d 6174 682e 636f 7328  os_t = math.cos(
+00013d50: 7377 6565 705f 7365 676d 656e 7429 0a20  sweep_segment). 
+00013d60: 2020 2020 2020 2073 696e 5f74 203d 206d         sin_t = m
+00013d70: 6174 682e 7369 6e28 7377 6565 705f 7365  ath.sin(sweep_se
+00013d80: 676d 656e 7429 0a20 2020 2020 2020 206b  gment).        k
+00013d90: 6170 7061 203d 2034 202f 2033 202a 206d  appa = 4 / 3 * m
+00013da0: 6174 682e 7461 6e28 7377 6565 705f 7365  ath.tan(sweep_se
+00013db0: 676d 656e 7420 2f20 3429 0a0a 2020 2020  gment / 4)..    
+00013dc0: 2020 2020 6374 726c 3120 3d20 506f 696e      ctrl1 = Poin
+00013dd0: 7428 312c 206b 6170 7061 290a 2020 2020  t(1, kappa).    
+00013de0: 2020 2020 6374 726c 3220 3d20 506f 696e      ctrl2 = Poin
+00013df0: 7428 636f 735f 7420 2b20 6b61 7070 6120  t(cos_t + kappa 
+00013e00: 2a20 7369 6e5f 742c 2073 696e 5f74 202d  * sin_t, sin_t -
+00013e10: 206b 6170 7061 202a 2063 6f73 5f74 290a   kappa * cos_t).
+00013e20: 2020 2020 2020 2020 656e 6420 3d20 506f          end = Po
+00013e30: 696e 7428 636f 735f 742c 2073 696e 5f74  int(cos_t, sin_t
+00013e40: 290a 0a20 2020 2020 2020 2066 6f72 205f  )..        for _
+00013e50: 2069 6e20 7261 6e67 6528 6368 756e 6b73   in range(chunks
+00013e60: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
+00013e70: 6666 7365 7420 3d20 7377 6565 705f 616e  ffset = sweep_an
+00013e80: 676c 6520 2d20 7377 6565 705f 6c65 6674  gle - sweep_left
+00013e90: 0a0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+00013ea0: 616e 7366 6f72 6d20 3d20 5472 616e 7366  ansform = Transf
+00013eb0: 6f72 6d2e 726f 7461 7469 6f6e 286f 6666  orm.rotation(off
+00013ec0: 7365 7429 0a20 2020 2020 2020 2020 2020  set).           
+00013ed0: 2079 6965 6c64 2063 7472 6c31 2040 2074   yield ctrl1 @ t
+00013ee0: 7261 6e73 666f 726d 2c20 6374 726c 3220  ransform, ctrl2 
+00013ef0: 4020 7472 616e 7366 6f72 6d2c 2065 6e64  @ transform, end
+00013f00: 2040 2074 7261 6e73 666f 726d 0a0a 2020   @ transform..  
+00013f10: 2020 2020 2020 2020 2020 7377 6565 705f            sweep_
+00013f20: 6c65 6674 202d 3d20 7377 6565 705f 7365  left -= sweep_se
+00013f30: 676d 656e 740a 0a20 2020 2064 6566 205f  gment..    def _
+00013f40: 6170 7072 6f78 696d 6174 655f 6172 6328  approximate_arc(
+00013f50: 7365 6c66 2c20 6c61 7374 5f69 7465 6d29  self, last_item)
+00013f60: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013f70: 2020 2020 2020 4170 7072 6f78 696d 6174        Approximat
+00013f80: 6520 7468 6973 2061 7263 2077 6974 6820  e this arc with 
+00013f90: 6120 7365 7175 656e 6365 206f 6620 6042  a sequence of `B
+00013fa0: 657a 6965 7243 7572 7665 602e 0a0a 2020  ezierCurve`...  
+00013fb0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00013fc0: 2020 2020 2020 2020 6c61 7374 5f69 7465          last_ite
+00013fd0: 6d3a 2074 6865 2070 7265 7669 6f75 7320  m: the previous 
+00013fe0: 7061 7468 2065 6c65 6d65 6e74 2028 7573  path element (us
+00013ff0: 6564 2066 6f72 2069 7473 2065 6e64 2070  ed for its end p
+00014000: 6f69 6e74 290a 0a20 2020 2020 2020 2052  oint)..        R
+00014010: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00014020: 2020 2020 6120 6c69 7374 206f 6620 6042      a list of `B
+00014030: 657a 6965 7243 7572 7665 602e 0a20 2020  ezierCurve`..   
+00014040: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014050: 2072 6164 6969 203d 2073 656c 662e 7261   radii = self.ra
+00014060: 6469 690a 0a20 2020 2020 2020 2072 6576  dii..        rev
+00014070: 6572 7365 203d 2054 7261 6e73 666f 726d  erse = Transform
+00014080: 2e72 6f74 6174 696f 6e28 2d73 656c 662e  .rotation(-self.
+00014090: 726f 7461 7469 6f6e 290a 2020 2020 2020  rotation).      
+000140a0: 2020 666f 7277 6172 6420 3d20 5472 616e    forward = Tran
+000140b0: 7366 6f72 6d2e 726f 7461 7469 6f6e 2873  sform.rotation(s
+000140c0: 656c 662e 726f 7461 7469 6f6e 290a 0a20  elf.rotation).. 
+000140d0: 2020 2020 2020 2070 7269 6d65 203d 2028         prime = (
+000140e0: 286c 6173 745f 6974 656d 2e65 6e64 5f70  (last_item.end_p
+000140f0: 6f69 6e74 202d 2073 656c 662e 656e 6429  oint - self.end)
+00014100: 202a 2030 2e35 2920 4020 7265 7665 7273   * 0.5) @ revers
+00014110: 650a 0a20 2020 2020 2020 206c 616d 5f64  e..        lam_d
+00014120: 6120 3d20 2870 7269 6d65 2e78 202f 2072  a = (prime.x / r
+00014130: 6164 6969 2e78 2920 2a2a 2032 202b 2028  adii.x) ** 2 + (
+00014140: 7072 696d 652e 7920 2f20 7261 6469 692e  prime.y / radii.
+00014150: 7929 202a 2a20 320a 0a20 2020 2020 2020  y) ** 2..       
+00014160: 2069 6620 6c61 6d5f 6461 203e 2031 3a0a   if lam_da > 1:.
+00014170: 2020 2020 2020 2020 2020 2020 7261 6469              radi
+00014180: 6920 3d20 506f 696e 7428 783d 286c 616d  i = Point(x=(lam
+00014190: 5f64 612a 2a30 2e35 2920 2a20 7261 6469  _da**0.5) * radi
+000141a0: 692e 782c 2079 3d28 6c61 6d5f 6461 2a2a  i.x, y=(lam_da**
+000141b0: 302e 3529 202a 2072 6164 6969 2e79 290a  0.5) * radii.y).
+000141c0: 0a20 2020 2020 2020 2073 6967 6e20 3d20  .        sign = 
+000141d0: 2873 656c 662e 6c61 7267 6520 213d 2073  (self.large != s
+000141e0: 656c 662e 7377 6565 7029 202d 2028 7365  elf.sweep) - (se
+000141f0: 6c66 2e6c 6172 6765 203d 3d20 7365 6c66  lf.large == self
+00014200: 2e73 7765 6570 290a 2020 2020 2020 2020  .sweep).        
+00014210: 7278 7279 3220 3d20 2872 6164 6969 2e78  rxry2 = (radii.x
+00014220: 202a 2072 6164 6969 2e79 2920 2a2a 2032   * radii.y) ** 2
+00014230: 0a20 2020 2020 2020 2072 7870 7932 203d  .        rxpy2 =
+00014240: 2028 7261 6469 692e 7820 2a20 7072 696d   (radii.x * prim
+00014250: 652e 7929 202a 2a20 320a 2020 2020 2020  e.y) ** 2.      
+00014260: 2020 7279 7078 3220 3d20 2872 6164 6969    rypx2 = (radii
+00014270: 2e79 202a 2070 7269 6d65 2e78 2920 2a2a  .y * prime.x) **
+00014280: 2032 0a0a 2020 2020 2020 2020 6365 6e74   2..        cent
+00014290: 6572 7072 696d 6520 3d20 280a 2020 2020  erprime = (.    
+000142a0: 2020 2020 2020 2020 7369 676e 0a20 2020          sign.   
+000142b0: 2020 2020 2020 2020 202a 206d 6174 682e           * math.
+000142c0: 7371 7274 2872 6f75 6e64 2872 7872 7932  sqrt(round(rxry2
+000142d0: 202d 2072 7870 7932 202d 2072 7970 7832   - rxpy2 - rypx2
+000142e0: 2c20 3829 202f 2028 7278 7079 3220 2b20  , 8) / (rxpy2 + 
+000142f0: 7279 7078 3229 290a 2020 2020 2020 2020  rypx2)).        
+00014300: 2020 2020 2a20 506f 696e 7428 0a20 2020      * Point(.   
+00014310: 2020 2020 2020 2020 2020 2020 2078 3d72               x=r
+00014320: 6164 6969 2e78 202a 2070 7269 6d65 2e79  adii.x * prime.y
+00014330: 202f 2072 6164 6969 2e79 2c0a 2020 2020   / radii.y,.    
+00014340: 2020 2020 2020 2020 2020 2020 793d 2d72              y=-r
+00014350: 6164 6969 2e79 202a 2070 7269 6d65 2e78  adii.y * prime.x
+00014360: 202f 2072 6164 6969 2e78 2c0a 2020 2020   / radii.x,.    
+00014370: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00014380: 2020 290a 0a20 2020 2020 2020 2063 656e    )..        cen
+00014390: 7465 7220 3d20 2863 656e 7465 7270 7269  ter = (centerpri
+000143a0: 6d65 2040 2066 6f72 7761 7264 2920 2b20  me @ forward) + 
+000143b0: 2828 6c61 7374 5f69 7465 6d2e 656e 645f  ((last_item.end_
+000143c0: 706f 696e 7420 2b20 7365 6c66 2e65 6e64  point + self.end
+000143d0: 2920 2a20 302e 3529 0a0a 2020 2020 2020  ) * 0.5)..      
+000143e0: 2020 6172 6373 7461 7274 203d 2050 6f69    arcstart = Poi
+000143f0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+00014400: 783d 2870 7269 6d65 2e78 202d 2063 656e  x=(prime.x - cen
+00014410: 7465 7270 7269 6d65 2e78 2920 2f20 7261  terprime.x) / ra
+00014420: 6469 692e 782c 0a20 2020 2020 2020 2020  dii.x,.         
+00014430: 2020 2079 3d28 7072 696d 652e 7920 2d20     y=(prime.y - 
+00014440: 6365 6e74 6572 7072 696d 652e 7929 202f  centerprime.y) /
+00014450: 2072 6164 6969 2e79 2c0a 2020 2020 2020   radii.y,.      
+00014460: 2020 290a 2020 2020 2020 2020 6172 6365    ).        arce
+00014470: 6e64 203d 2050 6f69 6e74 280a 2020 2020  nd = Point(.    
+00014480: 2020 2020 2020 2020 783d 282d 7072 696d          x=(-prim
+00014490: 652e 7820 2d20 6365 6e74 6572 7072 696d  e.x - centerprim
+000144a0: 652e 7829 202f 2072 6164 6969 2e78 2c0a  e.x) / radii.x,.
+000144b0: 2020 2020 2020 2020 2020 2020 793d 282d              y=(-
+000144c0: 7072 696d 652e 7920 2d20 6365 6e74 6572  prime.y - center
+000144d0: 7072 696d 652e 7929 202f 2072 6164 6969  prime.y) / radii
+000144e0: 2e79 2c0a 2020 2020 2020 2020 290a 0a20  .y,.        ).. 
+000144f0: 2020 2020 2020 2074 6865 7461 203d 2050         theta = P
+00014500: 6f69 6e74 2831 2c20 3029 2e61 6e67 6c65  oint(1, 0).angle
+00014510: 2861 7263 7374 6172 7429 0a20 2020 2020  (arcstart).     
+00014520: 2020 2064 656c 7461 7468 6574 6120 3d20     deltatheta = 
+00014530: 6172 6373 7461 7274 2e61 6e67 6c65 2861  arcstart.angle(a
+00014540: 7263 656e 6429 0a0a 2020 2020 2020 2020  rcend)..        
+00014550: 6966 2028 7365 6c66 2e73 7765 6570 2069  if (self.sweep i
+00014560: 7320 4661 6c73 6529 2061 6e64 2028 6465  s False) and (de
+00014570: 6c74 6174 6865 7461 203e 2030 293a 0a20  ltatheta > 0):. 
+00014580: 2020 2020 2020 2020 2020 2064 656c 7461             delta
+00014590: 7468 6574 6120 2d3d 206d 6174 682e 7461  theta -= math.ta
+000145a0: 750a 2020 2020 2020 2020 656c 6966 2028  u.        elif (
+000145b0: 7365 6c66 2e73 7765 6570 2069 7320 5472  self.sweep is Tr
+000145c0: 7565 2920 616e 6420 2864 656c 7461 7468  ue) and (deltath
+000145d0: 6574 6120 3c20 3029 3a0a 2020 2020 2020  eta < 0):.      
+000145e0: 2020 2020 2020 6465 6c74 6174 6865 7461        deltatheta
+000145f0: 202b 3d20 6d61 7468 2e74 6175 0a0a 2020   += math.tau..  
+00014600: 2020 2020 2020 7377 6565 705f 7369 676e        sweep_sign
+00014610: 203d 2028 6465 6c74 6174 6865 7461 203e   = (deltatheta >
+00014620: 3d20 3029 202d 2028 6465 6c74 6174 6865  = 0) - (deltathe
+00014630: 7461 203c 2030 290a 2020 2020 2020 2020  ta < 0).        
+00014640: 6669 6e61 6c5f 7466 203d 2028 0a20 2020  final_tf = (.   
+00014650: 2020 2020 2020 2020 2054 7261 6e73 666f           Transfo
+00014660: 726d 2e73 6361 6c69 6e67 2878 3d31 2c20  rm.scaling(x=1, 
+00014670: 793d 7377 6565 705f 7369 676e 2920 2023  y=sweep_sign)  #
+00014680: 2066 6c69 7020 6e65 6761 7469 7665 2073   flip negative s
+00014690: 7765 6570 730a 2020 2020 2020 2020 2020  weeps.          
+000146a0: 2020 2e72 6f74 6174 6528 7468 6574 6129    .rotate(theta)
+000146b0: 2020 2320 726f 7461 7465 2073 7461 7274    # rotate start
+000146c0: 206f 6620 6172 6320 746f 2063 6f72 7265   of arc to corre
+000146d0: 6374 2070 6f73 6974 696f 6e0a 2020 2020  ct position.    
+000146e0: 2020 2020 2020 2020 2e73 6361 6c65 2872          .scale(r
+000146f0: 6164 6969 2e78 2c20 7261 6469 692e 7929  adii.x, radii.y)
+00014700: 2020 2320 7363 616c 6520 756e 6974 2063    # scale unit c
+00014710: 6972 636c 6520 696e 746f 2074 6865 2066  ircle into the f
+00014720: 696e 616c 2065 6c6c 6970 7365 2073 6861  inal ellipse sha
+00014730: 7065 0a20 2020 2020 2020 2020 2020 202e  pe.            .
+00014740: 726f 7461 7465 2873 656c 662e 726f 7461  rotate(self.rota
+00014750: 7469 6f6e 2920 2023 2072 6f74 6174 6520  tion)  # rotate 
+00014760: 7468 6520 656c 6c69 7073 6520 7468 6520  the ellipse the 
+00014770: 7370 6563 6966 6965 6420 616e 676c 650a  specified angle.
+00014780: 2020 2020 2020 2020 2020 2020 2e74 7261              .tra
+00014790: 6e73 6c61 7465 2863 656e 7465 722e 782c  nslate(center.x,
+000147a0: 2063 656e 7465 722e 7929 2020 2320 7472   center.y)  # tr
+000147b0: 616e 736c 6174 6520 746f 2074 6865 2066  anslate to the f
+000147c0: 696e 616c 2063 6f6f 7264 696e 6174 6573  inal coordinates
+000147d0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+000147e0: 2020 2020 6375 7276 6573 203d 205b 5d0a      curves = [].
+000147f0: 0a20 2020 2020 2020 2066 6f72 2063 7472  .        for ctr
+00014800: 6c31 2c20 6374 726c 322c 2065 6e64 2069  l1, ctrl2, end i
+00014810: 6e20 7365 6c66 2e73 7562 6469 7664 655f  n self.subdivde_
+00014820: 7377 6565 7028 6465 6c74 6174 6865 7461  sweep(deltatheta
+00014830: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00014840: 7572 7665 732e 6170 7065 6e64 280a 2020  urves.append(.  
+00014850: 2020 2020 2020 2020 2020 2020 2020 4265                Be
+00014860: 7a69 6572 4375 7276 6528 6374 726c 3120  zierCurve(ctrl1 
+00014870: 4020 6669 6e61 6c5f 7466 2c20 6374 726c  @ final_tf, ctrl
+00014880: 3220 4020 6669 6e61 6c5f 7466 2c20 656e  2 @ final_tf, en
+00014890: 6420 4020 6669 6e61 6c5f 7466 290a 2020  d @ final_tf).  
+000148a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000148b0: 2020 2020 2072 6574 7572 6e20 6375 7276       return curv
+000148c0: 6573 0a0a 2020 2020 4066 6f72 6365 5f6e  es..    @force_n
+000148d0: 6f64 6f63 756d 656e 740a 2020 2020 6465  odocument.    de
+000148e0: 6620 7265 6e64 6572 2873 656c 662c 2067  f render(self, g
+000148f0: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
+00014900: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
+00014910: 6e69 7469 616c 5f70 6f69 6e74 293a 0a20  nitial_point):. 
+00014920: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014930: 2020 2052 656e 6465 7220 7468 6973 2070     Render this p
+00014940: 6174 6820 656c 656d 656e 7420 746f 2069  ath element to i
+00014950: 7473 2050 4446 2072 6570 7265 7365 6e74  ts PDF represent
+00014960: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+00014970: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00014980: 2020 6773 645f 7265 6769 7374 7279 2028    gsd_registry (
+00014990: 4772 6170 6869 6373 5374 6174 6544 6963  GraphicsStateDic
+000149a0: 7452 6567 6973 7472 7929 3a20 7468 6520  tRegistry): the 
+000149b0: 6f77 6e65 7227 7320 6772 6170 6869 6373  owner's graphics
+000149c0: 2073 7461 7465 0a20 2020 2020 2020 2020   state.         
+000149d0: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
+000149e0: 7920 7265 6769 7374 7279 2e0a 2020 2020  y registry..    
+000149f0: 2020 2020 2020 2020 7374 796c 6520 2847          style (G
+00014a00: 7261 7068 6963 7353 7479 6c65 293a 2074  raphicsStyle): t
+00014a10: 6865 2063 7572 7265 6e74 2072 6573 6f6c  he current resol
+00014a20: 7665 6420 6772 6170 6869 6373 2073 7479  ved graphics sty
+00014a30: 6c65 0a20 2020 2020 2020 2020 2020 206c  le.            l
+00014a40: 6173 745f 6974 656d 3a20 7468 6520 7072  ast_item: the pr
+00014a50: 6576 696f 7573 2070 6174 6820 656c 656d  evious path elem
+00014a60: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
+00014a70: 2069 6e69 7469 616c 5f70 6f69 6e74 3a20   initial_point: 
+00014a80: 6c61 7374 2070 6f73 6974 696f 6e20 7365  last position se
+00014a90: 7420 6279 2061 2022 4d22 206f 7220 226d  t by a "M" or "m
+00014aa0: 2220 636f 6d6d 616e 640a 0a20 2020 2020  " command..     
+00014ab0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00014ac0: 2020 2020 2020 2020 6120 7475 706c 6520          a tuple 
+00014ad0: 6f66 2060 2873 7472 2c20 6e65 775f 6c61  of `(str, new_la
+00014ae0: 7374 5f69 7465 6d29 602c 2077 6865 7265  st_item)`, where
+00014af0: 2060 6e65 775f 6c61 7374 5f69 7465 6d60   `new_last_item`
+00014b00: 2069 7320 6120 7265 736f 6c76 6564 0a20   is a resolved. 
+00014b10: 2020 2020 2020 2020 2020 2060 4265 7a69             `Bezi
+00014b20: 6572 4375 7276 6560 2e0a 2020 2020 2020  erCurve`..      
+00014b30: 2020 2222 220a 2020 2020 2020 2020 6375    """.        cu
+00014b40: 7276 6573 203d 2073 656c 662e 5f61 7070  rves = self._app
+00014b50: 726f 7869 6d61 7465 5f61 7263 286c 6173  roximate_arc(las
+00014b60: 745f 6974 656d 290a 0a20 2020 2020 2020  t_item)..       
+00014b70: 2069 6620 6e6f 7420 6375 7276 6573 3a0a   if not curves:.
+00014b80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014b90: 726e 2022 222c 206c 6173 745f 6974 656d  rn "", last_item
+00014ba0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00014bb0: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
+00014bc0: 2022 2e6a 6f69 6e28 0a20 2020 2020 2020   ".join(.       
+00014bd0: 2020 2020 2020 2020 2063 7572 7665 2e72           curve.r
+00014be0: 656e 6465 7228 6773 645f 7265 6769 7374  ender(gsd_regist
+00014bf0: 7279 2c20 7374 796c 652c 2070 7265 762c  ry, style, prev,
+00014c00: 2069 6e69 7469 616c 5f70 6f69 6e74 295b   initial_point)[
+00014c10: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+00014c20: 2020 2066 6f72 2070 7265 762c 2063 7572     for prev, cur
+00014c30: 7665 2069 6e20 7a69 7028 5b6c 6173 745f  ve in zip([last_
+00014c40: 6974 656d 2c20 2a63 7572 7665 735b 3a2d  item, *curves[:-
+00014c50: 315d 5d2c 2063 7572 7665 7329 0a20 2020  1]], curves).   
+00014c60: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00014c70: 2020 2020 2020 2020 6375 7276 6573 5b2d          curves[-
+00014c80: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00014c90: 696e 6974 6961 6c5f 706f 696e 742c 0a20  initial_point,. 
+00014ca0: 2020 2020 2020 2029 0a0a 2020 2020 4066         )..    @f
+00014cb0: 6f72 6365 5f6e 6f64 6f63 756d 656e 740a  orce_nodocument.
+00014cc0: 2020 2020 6465 6620 7265 6e64 6572 5f64      def render_d
+00014cd0: 6562 7567 280a 2020 2020 2020 2020 7365  ebug(.        se
+00014ce0: 6c66 2c20 6773 645f 7265 6769 7374 7279  lf, gsd_registry
+00014cf0: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
+00014d00: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
+00014d10: 742c 2064 6562 7567 5f73 7472 6561 6d2c  t, debug_stream,
+00014d20: 2070 6678 0a20 2020 2029 3a0a 2020 2020   pfx.    ):.    
+00014d30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014d40: 5265 6e64 6572 2074 6869 7320 7061 7468  Render this path
+00014d50: 2065 6c65 6d65 6e74 2074 6f20 6974 7320   element to its 
+00014d60: 5044 4620 7265 7072 6573 656e 7461 7469  PDF representati
+00014d70: 6f6e 2061 6e64 2070 726f 6475 6365 2064  on and produce d
+00014d80: 6562 7567 0a20 2020 2020 2020 2069 6e66  ebug.        inf
+00014d90: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
+00014da0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00014db0: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
+00014dc0: 7920 2847 7261 7068 6963 7353 7461 7465  y (GraphicsState
+00014dd0: 4469 6374 5265 6769 7374 7279 293a 2074  DictRegistry): t
+00014de0: 6865 206f 776e 6572 2773 2067 7261 7068  he owner's graph
+00014df0: 6963 7320 7374 6174 650a 2020 2020 2020  ics state.      
+00014e00: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
+00014e10: 6e61 7279 2072 6567 6973 7472 792e 0a20  nary registry.. 
+00014e20: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00014e30: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
+00014e40: 3a20 7468 6520 6375 7272 656e 7420 7265  : the current re
+00014e50: 736f 6c76 6564 2067 7261 7068 6963 7320  solved graphics 
+00014e60: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
+00014e70: 2020 6c61 7374 5f69 7465 6d3a 2074 6865    last_item: the
+00014e80: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
+00014e90: 6c65 6d65 6e74 2e0a 2020 2020 2020 2020  lement..        
+00014ea0: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
+00014eb0: 743a 206c 6173 7420 706f 7369 7469 6f6e  t: last position
+00014ec0: 2073 6574 2062 7920 6120 224d 2220 6f72   set by a "M" or
+00014ed0: 2022 6d22 2063 6f6d 6d61 6e64 0a20 2020   "m" command.   
+00014ee0: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
+00014ef0: 7472 6561 6d20 2869 6f2e 5465 7874 494f  tream (io.TextIO
+00014f00: 293a 2074 6865 2073 7472 6561 6d20 746f  ): the stream to
+00014f10: 2077 6869 6368 2074 6865 2064 6562 7567   which the debug
+00014f20: 206f 7574 7075 7420 7368 6f75 6c64 2062   output should b
+00014f30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00014f40: 2020 7772 6974 7465 6e2e 2054 6869 7320    written. This 
+00014f50: 6973 206e 6f74 2067 7561 7261 6e74 6565  is not guarantee
+00014f60: 6420 746f 2062 6520 7365 656b 6162 6c65  d to be seekable
+00014f70: 2028 652e 672e 2069 7420 6d61 7920 6265   (e.g. it may be
+00014f80: 2073 7464 6f75 7420 6f72 0a20 2020 2020   stdout or.     
+00014f90: 2020 2020 2020 2020 2020 2073 7464 6572             stder
+00014fa0: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
+00014fb0: 7066 7820 2873 7472 293a 2074 6865 2063  pfx (str): the c
+00014fc0: 7572 7265 6e74 2064 6562 7567 206f 7574  urrent debug out
+00014fd0: 7075 7420 7072 6566 6978 2073 7472 696e  put prefix strin
+00014fe0: 6720 286f 6e6c 7920 6e65 6564 6564 2069  g (only needed i
+00014ff0: 6620 656d 6974 7469 6e67 0a20 2020 2020  f emitting.     
+00015000: 2020 2020 2020 2020 2020 206d 6f72 6520             more 
+00015010: 7468 616e 206f 6e65 206c 696e 6529 2e0a  than one line)..
+00015020: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00015030: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00015040: 6520 7361 6d65 2074 7570 6c65 2061 7320  e same tuple as 
+00015050: 6041 7263 2e72 656e 6465 7260 2e0a 2020  `Arc.render`..  
+00015060: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015070: 2020 6375 7276 6573 203d 2073 656c 662e    curves = self.
+00015080: 5f61 7070 726f 7869 6d61 7465 5f61 7263  _approximate_arc
+00015090: 286c 6173 745f 6974 656d 290a 0a20 2020  (last_item)..   
+000150a0: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+000150b0: 6d2e 7772 6974 6528 6622 7b73 656c 667d  m.write(f"{self}
+000150c0: 2072 6573 6f6c 7665 6420 746f 3a5c 6e22   resolved to:\n"
+000150d0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+000150e0: 2063 7572 7665 733a 0a20 2020 2020 2020   curves:.       
+000150f0: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+00015100: 6d2e 7772 6974 6528 7066 7820 2b20 2220  m.write(pfx + " 
+00015110: e294 94e2 9480 206e 6f74 6869 6e67 5c6e  ...... nothing\n
+00015120: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00015130: 6574 7572 6e20 2222 2c20 6c61 7374 5f69  eturn "", last_i
+00015140: 7465 6d0a 0a20 2020 2020 2020 2070 7265  tem..        pre
+00015150: 7669 6f75 7320 3d20 5b6c 6173 745f 6974  vious = [last_it
+00015160: 656d 5d0a 2020 2020 2020 2020 666f 7220  em].        for 
+00015170: 6375 7276 6520 696e 2063 7572 7665 735b  curve in curves[
+00015180: 3a2d 315d 3a0a 2020 2020 2020 2020 2020  :-1]:.          
+00015190: 2020 7072 6576 696f 7573 2e61 7070 656e    previous.appen
+000151a0: 6428 6375 7276 6529 0a20 2020 2020 2020  d(curve).       
+000151b0: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+000151c0: 6d2e 7772 6974 6528 7066 7820 2b20 6622  m.write(pfx + f"
+000151d0: 20e2 949c e294 8020 7b63 7572 7665 7d5c   ...... {curve}\
+000151e0: 6e22 290a 2020 2020 2020 2020 6465 6275  n").        debu
+000151f0: 675f 7374 7265 616d 2e77 7269 7465 2870  g_stream.write(p
+00015200: 6678 202b 2066 2220 e294 94e2 9480 207b  fx + f" ...... {
+00015210: 6375 7276 6573 5b2d 315d 7d5c 6e22 290a  curves[-1]}\n").
+00015220: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00015230: 280a 2020 2020 2020 2020 2020 2020 2220  (.            " 
+00015240: 222e 6a6f 696e 280a 2020 2020 2020 2020  ".join(.        
+00015250: 2020 2020 2020 2020 6375 7276 652e 7265          curve.re
+00015260: 6e64 6572 2867 7364 5f72 6567 6973 7472  nder(gsd_registr
+00015270: 792c 2073 7479 6c65 2c20 7072 6576 2c20  y, style, prev, 
+00015280: 696e 6974 6961 6c5f 706f 696e 7429 5b30  initial_point)[0
+00015290: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000152a0: 2020 666f 7220 7072 6576 2c20 6375 7276    for prev, curv
+000152b0: 6520 696e 207a 6970 2870 7265 7669 6f75  e in zip(previou
+000152c0: 732c 2063 7572 7665 7329 0a20 2020 2020  s, curves).     
+000152d0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+000152e0: 2020 2020 2020 6375 7276 6573 5b2d 315d        curves[-1]
+000152f0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+00015300: 6974 6961 6c5f 706f 696e 742c 0a20 2020  itial_point,.   
+00015310: 2020 2020 2029 0a0a 0a63 6c61 7373 2052       )...class R
+00015320: 656c 6174 6976 6541 7263 284e 616d 6564  elativeArc(Named
+00015330: 5475 706c 6529 3a0a 2020 2020 2222 220a  Tuple):.    """.
+00015340: 2020 2020 416e 2065 6c6c 6970 7469 6361      An elliptica
+00015350: 6c20 6172 6320 7061 7468 2065 6c65 6d65  l arc path eleme
+00015360: 6e74 2e0a 0a20 2020 2054 6865 2061 7263  nt...    The arc
+00015370: 2069 7320 6472 6177 6e20 6672 6f6d 2074   is drawn from t
+00015380: 6865 2065 6e64 206f 6620 7468 6520 6375  he end of the cu
+00015390: 7272 656e 7420 7061 7468 2065 6c65 6d65  rrent path eleme
+000153a0: 6e74 2074 6f20 6974 7320 7370 6563 6966  nt to its specif
+000153b0: 6965 6420 656e 6420 706f 696e 740a 2020  ied end point.  
+000153c0: 2020 7573 696e 6720 6120 6e75 6d62 6572    using a number
+000153d0: 206f 6620 7061 7261 6d65 7465 7273 2074   of parameters t
+000153e0: 6f20 6465 7465 726d 696e 6520 686f 7720  o determine how 
+000153f0: 6974 2069 7320 636f 6e73 7472 7563 7465  it is constructe
+00015400: 642e 0a0a 2020 2020 5365 653a 2060 5061  d...    See: `Pa
+00015410: 696e 7465 6450 6174 682e 6172 635f 7265  intedPath.arc_re
+00015420: 6c61 7469 7665 600a 2020 2020 2222 220a  lative`.    """.
+00015430: 0a20 2020 2072 6164 6969 3a20 506f 696e  .    radii: Poin
+00015440: 740a 2020 2020 2222 220a 2020 2020 5468  t.    """.    Th
+00015450: 6520 782d 2061 6e64 2079 2d72 6164 6969  e x- and y-radii
+00015460: 206f 6620 7468 6520 6172 632e 2049 6620   of the arc. If 
+00015470: 6072 6164 6969 2e78 203d 3d20 7261 6469  `radii.x == radi
+00015480: 692e 7960 2074 6865 2061 7263 2077 696c  i.y` the arc wil
+00015490: 6c20 6265 2063 6972 6375 6c61 722e 0a20  l be circular.. 
+000154a0: 2020 2022 2222 0a20 2020 2072 6f74 6174     """.    rotat
+000154b0: 696f 6e3a 204e 756d 6265 720a 2020 2020  ion: Number.    
+000154c0: 2222 2254 6865 2072 6f74 6174 696f 6e20  """The rotation 
+000154d0: 6f66 2074 6865 2061 7263 2773 206d 616a  of the arc's maj
+000154e0: 6f72 2f6d 696e 6f72 2061 7865 7320 7265  or/minor axes re
+000154f0: 6c61 7469 7665 2074 6f20 7468 6520 636f  lative to the co
+00015500: 6f72 6469 6e61 7465 2066 7261 6d65 2e22  ordinate frame."
+00015510: 2222 0a20 2020 206c 6172 6765 3a20 626f  "".    large: bo
+00015520: 6f6c 0a20 2020 2022 2222 4966 2054 7275  ol.    """If Tru
+00015530: 652c 2073 7765 6570 2074 6865 2061 7263  e, sweep the arc
+00015540: 206f 7665 7220 616e 2061 6e67 6c65 2067   over an angle g
+00015550: 7265 6174 6572 2074 6861 6e20 6f72 2065  reater than or e
+00015560: 7175 616c 2074 6f20 3138 3020 6465 6772  qual to 180 degr
+00015570: 6565 732e 2222 220a 2020 2020 7377 6565  ees.""".    swee
+00015580: 703a 2062 6f6f 6c0a 2020 2020 2222 2249  p: bool.    """I
+00015590: 6620 5472 7565 2c20 7468 6520 6172 6320  f True, the arc 
+000155a0: 6973 2073 7765 7074 2069 6e20 7468 6520  is swept in the 
+000155b0: 706f 7369 7469 7665 2061 6e67 756c 6172  positive angular
+000155c0: 2064 6972 6563 7469 6f6e 2e22 2222 0a20   direction.""". 
+000155d0: 2020 2065 6e64 3a20 506f 696e 740a 2020     end: Point.  
+000155e0: 2020 2222 2254 6865 2065 6e64 2070 6f69    """The end poi
+000155f0: 6e74 206f 6620 7468 6520 6172 6320 7265  nt of the arc re
+00015600: 6c61 7469 7665 2074 6f20 7468 6520 656e  lative to the en
+00015610: 6420 6f66 2074 6865 2070 7265 7669 6f75  d of the previou
+00015620: 7320 7061 7468 2065 6c65 6d65 6e74 2e22  s path element."
+00015630: 2222 0a0a 2020 2020 4066 6f72 6365 5f6e  ""..    @force_n
+00015640: 6f64 6f63 756d 656e 740a 2020 2020 6465  odocument.    de
+00015650: 6620 7265 6e64 6572 2873 656c 662c 2067  f render(self, g
+00015660: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
+00015670: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
+00015680: 6e69 7469 616c 5f70 6f69 6e74 293a 0a20  nitial_point):. 
+00015690: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000156a0: 2020 2052 656e 6465 7220 7468 6973 2070     Render this p
+000156b0: 6174 6820 656c 656d 656e 7420 746f 2069  ath element to i
+000156c0: 7473 2050 4446 2072 6570 7265 7365 6e74  ts PDF represent
+000156d0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+000156e0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000156f0: 2020 6773 645f 7265 6769 7374 7279 2028    gsd_registry (
+00015700: 4772 6170 6869 6373 5374 6174 6544 6963  GraphicsStateDic
+00015710: 7452 6567 6973 7472 7929 3a20 7468 6520  tRegistry): the 
+00015720: 6f77 6e65 7227 7320 6772 6170 6869 6373  owner's graphics
+00015730: 2073 7461 7465 0a20 2020 2020 2020 2020   state.         
+00015740: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
+00015750: 7920 7265 6769 7374 7279 2e0a 2020 2020  y registry..    
+00015760: 2020 2020 2020 2020 7374 796c 6520 2847          style (G
+00015770: 7261 7068 6963 7353 7479 6c65 293a 2074  raphicsStyle): t
+00015780: 6865 2063 7572 7265 6e74 2072 6573 6f6c  he current resol
+00015790: 7665 6420 6772 6170 6869 6373 2073 7479  ved graphics sty
+000157a0: 6c65 0a20 2020 2020 2020 2020 2020 206c  le.            l
+000157b0: 6173 745f 6974 656d 3a20 7468 6520 7072  ast_item: the pr
+000157c0: 6576 696f 7573 2070 6174 6820 656c 656d  evious path elem
+000157d0: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
+000157e0: 2069 6e69 7469 616c 5f70 6f69 6e74 3a20   initial_point: 
+000157f0: 6c61 7374 2070 6f73 6974 696f 6e20 7365  last position se
+00015800: 7420 6279 2061 2022 4d22 206f 7220 226d  t by a "M" or "m
+00015810: 2220 636f 6d6d 616e 640a 0a20 2020 2020  " command..     
+00015820: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00015830: 2020 2020 2020 2020 6120 7475 706c 6520          a tuple 
+00015840: 6f66 2060 2873 7472 2c20 6e65 775f 6c61  of `(str, new_la
+00015850: 7374 5f69 7465 6d29 602c 2077 6865 7265  st_item)`, where
+00015860: 2060 6e65 775f 6c61 7374 5f69 7465 6d60   `new_last_item`
+00015870: 2069 7320 6120 7265 736f 6c76 6564 0a20   is a resolved. 
+00015880: 2020 2020 2020 2020 2020 2060 4265 7a69             `Bezi
+00015890: 6572 4375 7276 6560 2e0a 2020 2020 2020  erCurve`..      
+000158a0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+000158b0: 7475 726e 2041 7263 280a 2020 2020 2020  turn Arc(.      
+000158c0: 2020 2020 2020 7365 6c66 2e72 6164 6969        self.radii
+000158d0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+000158e0: 6c66 2e72 6f74 6174 696f 6e2c 0a20 2020  lf.rotation,.   
+000158f0: 2020 2020 2020 2020 2073 656c 662e 6c61           self.la
+00015900: 7267 652c 0a20 2020 2020 2020 2020 2020  rge,.           
+00015910: 2073 656c 662e 7377 6565 702c 0a20 2020   self.sweep,.   
+00015920: 2020 2020 2020 2020 206c 6173 745f 6974           last_it
+00015930: 656d 2e65 6e64 5f70 6f69 6e74 202b 2073  em.end_point + s
+00015940: 656c 662e 656e 642c 0a20 2020 2020 2020  elf.end,.       
+00015950: 2029 2e72 656e 6465 7228 6773 645f 7265   ).render(gsd_re
+00015960: 6769 7374 7279 2c20 7374 796c 652c 206c  gistry, style, l
+00015970: 6173 745f 6974 656d 2c20 696e 6974 6961  ast_item, initia
+00015980: 6c5f 706f 696e 7429 0a0a 2020 2020 4066  l_point)..    @f
+00015990: 6f72 6365 5f6e 6f64 6f63 756d 656e 740a  orce_nodocument.
+000159a0: 2020 2020 6465 6620 7265 6e64 6572 5f64      def render_d
+000159b0: 6562 7567 280a 2020 2020 2020 2020 7365  ebug(.        se
+000159c0: 6c66 2c20 6773 645f 7265 6769 7374 7279  lf, gsd_registry
+000159d0: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
+000159e0: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
+000159f0: 742c 2064 6562 7567 5f73 7472 6561 6d2c  t, debug_stream,
+00015a00: 2070 6678 0a20 2020 2029 3a0a 2020 2020   pfx.    ):.    
+00015a10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015a20: 5265 6e64 6572 2074 6869 7320 7061 7468  Render this path
+00015a30: 2065 6c65 6d65 6e74 2074 6f20 6974 7320   element to its 
+00015a40: 5044 4620 7265 7072 6573 656e 7461 7469  PDF representati
+00015a50: 6f6e 2061 6e64 2070 726f 6475 6365 2064  on and produce d
+00015a60: 6562 7567 0a20 2020 2020 2020 2069 6e66  ebug.        inf
+00015a70: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
+00015a80: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00015a90: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
+00015aa0: 7920 2847 7261 7068 6963 7353 7461 7465  y (GraphicsState
+00015ab0: 4469 6374 5265 6769 7374 7279 293a 2074  DictRegistry): t
+00015ac0: 6865 206f 776e 6572 2773 2067 7261 7068  he owner's graph
+00015ad0: 6963 7320 7374 6174 650a 2020 2020 2020  ics state.      
+00015ae0: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
+00015af0: 6e61 7279 2072 6567 6973 7472 792e 0a20  nary registry.. 
+00015b00: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00015b10: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
+00015b20: 3a20 7468 6520 6375 7272 656e 7420 7265  : the current re
+00015b30: 736f 6c76 6564 2067 7261 7068 6963 7320  solved graphics 
+00015b40: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
+00015b50: 2020 6c61 7374 5f69 7465 6d3a 2074 6865    last_item: the
+00015b60: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
+00015b70: 6c65 6d65 6e74 2e0a 2020 2020 2020 2020  lement..        
+00015b80: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
+00015b90: 743a 206c 6173 7420 706f 7369 7469 6f6e  t: last position
+00015ba0: 2073 6574 2062 7920 6120 224d 2220 6f72   set by a "M" or
+00015bb0: 2022 6d22 2063 6f6d 6d61 6e64 0a20 2020   "m" command.   
+00015bc0: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
+00015bd0: 7472 6561 6d20 2869 6f2e 5465 7874 494f  tream (io.TextIO
+00015be0: 293a 2074 6865 2073 7472 6561 6d20 746f  ): the stream to
+00015bf0: 2077 6869 6368 2074 6865 2064 6562 7567   which the debug
+00015c00: 206f 7574 7075 7420 7368 6f75 6c64 2062   output should b
+00015c10: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00015c20: 2020 7772 6974 7465 6e2e 2054 6869 7320    written. This 
+00015c30: 6973 206e 6f74 2067 7561 7261 6e74 6565  is not guarantee
+00015c40: 6420 746f 2062 6520 7365 656b 6162 6c65  d to be seekable
+00015c50: 2028 652e 672e 2069 7420 6d61 7920 6265   (e.g. it may be
+00015c60: 2073 7464 6f75 7420 6f72 0a20 2020 2020   stdout or.     
+00015c70: 2020 2020 2020 2020 2020 2073 7464 6572             stder
+00015c80: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
+00015c90: 7066 7820 2873 7472 293a 2074 6865 2063  pfx (str): the c
+00015ca0: 7572 7265 6e74 2064 6562 7567 206f 7574  urrent debug out
+00015cb0: 7075 7420 7072 6566 6978 2073 7472 696e  put prefix strin
+00015cc0: 6720 286f 6e6c 7920 6e65 6564 6564 2069  g (only needed i
+00015cd0: 6620 656d 6974 7469 6e67 0a20 2020 2020  f emitting.     
+00015ce0: 2020 2020 2020 2020 2020 206d 6f72 6520             more 
+00015cf0: 7468 616e 206f 6e65 206c 696e 6529 2e0a  than one line)..
+00015d00: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00015d10: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00015d20: 6520 7361 6d65 2074 7570 6c65 2061 7320  e same tuple as 
+00015d30: 6052 656c 6174 6976 6541 7263 2e72 656e  `RelativeArc.ren
+00015d40: 6465 7260 2e0a 2020 2020 2020 2020 2222  der`..        ""
+00015d50: 220a 2020 2020 2020 2020 2320 6e65 776c  ".        # newl
+00015d60: 696e 6520 6973 2069 6e74 656e 7469 6f6e  ine is intention
+00015d70: 616c 6c79 206d 6973 7369 6e67 2068 6572  ally missing her
+00015d80: 650a 2020 2020 2020 2020 6465 6275 675f  e.        debug_
+00015d90: 7374 7265 616d 2e77 7269 7465 2866 227b  stream.write(f"{
+00015da0: 7365 6c66 7d20 7265 736f 6c76 6564 2074  self} resolved t
+00015db0: 6f20 2229 0a0a 2020 2020 2020 2020 7265  o ")..        re
+00015dc0: 7475 726e 2041 7263 280a 2020 2020 2020  turn Arc(.      
+00015dd0: 2020 2020 2020 7365 6c66 2e72 6164 6969        self.radii
+00015de0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00015df0: 6c66 2e72 6f74 6174 696f 6e2c 0a20 2020  lf.rotation,.   
+00015e00: 2020 2020 2020 2020 2073 656c 662e 6c61           self.la
+00015e10: 7267 652c 0a20 2020 2020 2020 2020 2020  rge,.           
+00015e20: 2073 656c 662e 7377 6565 702c 0a20 2020   self.sweep,.   
+00015e30: 2020 2020 2020 2020 206c 6173 745f 6974           last_it
+00015e40: 656d 2e65 6e64 5f70 6f69 6e74 202b 2073  em.end_point + s
+00015e50: 656c 662e 656e 642c 0a20 2020 2020 2020  elf.end,.       
+00015e60: 2029 2e72 656e 6465 725f 6465 6275 6728   ).render_debug(
+00015e70: 6773 645f 7265 6769 7374 7279 2c20 7374  gsd_registry, st
+00015e80: 796c 652c 206c 6173 745f 6974 656d 2c20  yle, last_item, 
+00015e90: 696e 6974 6961 6c5f 706f 696e 742c 2064  initial_point, d
+00015ea0: 6562 7567 5f73 7472 6561 6d2c 2070 6678  ebug_stream, pfx
+00015eb0: 290a 0a0a 636c 6173 7320 5265 6374 616e  )...class Rectan
+00015ec0: 676c 6528 4e61 6d65 6454 7570 6c65 293a  gle(NamedTuple):
+00015ed0: 0a20 2020 2022 2222 4120 7064 6620 7072  .    """A pdf pr
+00015ee0: 696d 6974 6976 6520 7265 6374 616e 676c  imitive rectangl
+00015ef0: 652e 2222 220a 0a20 2020 206f 7267 3a20  e."""..    org: 
+00015f00: 506f 696e 740a 2020 2020 2222 2254 6865  Point.    """The
+00015f10: 2074 6f70 2d6c 6566 7420 636f 726e 6572   top-left corner
+00015f20: 206f 6620 7468 6520 7265 6374 616e 676c   of the rectangl
+00015f30: 652e 2222 220a 2020 2020 7369 7a65 3a20  e.""".    size: 
+00015f40: 506f 696e 740a 2020 2020 2222 2254 6865  Point.    """The
+00015f50: 2077 6964 7468 2061 6e64 2068 6569 6768   width and heigh
+00015f60: 7420 6f66 2074 6865 2072 6563 7461 6e67  t of the rectang
+00015f70: 6c65 2e22 2222 0a0a 2020 2020 4066 6f72  le."""..    @for
+00015f80: 6365 5f6e 6f64 6f63 756d 656e 740a 2020  ce_nodocument.  
+00015f90: 2020 6465 6620 7265 6e64 6572 2873 656c    def render(sel
+00015fa0: 662c 2067 7364 5f72 6567 6973 7472 792c  f, gsd_registry,
+00015fb0: 2073 7479 6c65 2c20 6c61 7374 5f69 7465   style, last_ite
+00015fc0: 6d2c 2069 6e69 7469 616c 5f70 6f69 6e74  m, initial_point
+00015fd0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00015fe0: 2020 2020 2020 2052 656e 6465 7220 7468         Render th
+00015ff0: 6973 2070 6174 6820 656c 656d 656e 7420  is path element 
+00016000: 746f 2069 7473 2050 4446 2072 6570 7265  to its PDF repre
+00016010: 7365 6e74 6174 696f 6e2e 0a0a 2020 2020  sentation...    
+00016020: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00016030: 2020 2020 2020 6773 645f 7265 6769 7374        gsd_regist
+00016040: 7279 2028 4772 6170 6869 6373 5374 6174  ry (GraphicsStat
+00016050: 6544 6963 7452 6567 6973 7472 7929 3a20  eDictRegistry): 
+00016060: 7468 6520 6f77 6e65 7227 7320 6772 6170  the owner's grap
+00016070: 6869 6373 2073 7461 7465 0a20 2020 2020  hics state.     
+00016080: 2020 2020 2020 2020 2020 2064 6963 7469             dicti
+00016090: 6f6e 6172 7920 7265 6769 7374 7279 2e0a  onary registry..
+000160a0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
+000160b0: 6520 2847 7261 7068 6963 7353 7479 6c65  e (GraphicsStyle
+000160c0: 293a 2074 6865 2063 7572 7265 6e74 2072  ): the current r
+000160d0: 6573 6f6c 7665 6420 6772 6170 6869 6373  esolved graphics
+000160e0: 2073 7479 6c65 0a20 2020 2020 2020 2020   style.         
+000160f0: 2020 206c 6173 745f 6974 656d 3a20 7468     last_item: th
+00016100: 6520 7072 6576 696f 7573 2070 6174 6820  e previous path 
+00016110: 656c 656d 656e 742e 0a20 2020 2020 2020  element..       
+00016120: 2020 2020 2069 6e69 7469 616c 5f70 6f69       initial_poi
+00016130: 6e74 3a20 6c61 7374 2070 6f73 6974 696f  nt: last positio
+00016140: 6e20 7365 7420 6279 2061 2022 4d22 206f  n set by a "M" o
+00016150: 7220 226d 2220 636f 6d6d 616e 640a 0a20  r "m" command.. 
+00016160: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00016170: 2020 2020 2020 2020 2020 2020 6120 7475              a tu
+00016180: 706c 6520 6f66 2060 2873 7472 2c20 6e65  ple of `(str, ne
+00016190: 775f 6c61 7374 5f69 7465 6d29 602c 2077  w_last_item)`, w
+000161a0: 6865 7265 2060 6e65 775f 6c61 7374 5f69  here `new_last_i
+000161b0: 7465 6d60 2069 7320 6120 604c 696e 6560  tem` is a `Line`
+000161c0: 2062 6163 6b20 746f 0a20 2020 2020 2020   back to.       
+000161d0: 2020 2020 2074 6865 2072 6563 7461 6e67       the rectang
+000161e0: 6c65 2773 206f 7269 6769 6e2e 0a20 2020  le's origin..   
+000161f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016200: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00016210: 6c65 3d75 6e75 7365 642d 6172 6775 6d65  le=unused-argume
+00016220: 6e74 0a0a 2020 2020 2020 2020 7265 7475  nt..        retu
+00016230: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
+00016240: 2066 227b 7365 6c66 2e6f 7267 2e72 656e   f"{self.org.ren
+00016250: 6465 7228 297d 207b 7365 6c66 2e73 697a  der()} {self.siz
+00016260: 652e 7265 6e64 6572 2829 7d20 7265 222c  e.render()} re",
+00016270: 0a20 2020 2020 2020 2020 2020 204c 696e  .            Lin
+00016280: 6528 7365 6c66 2e6f 7267 292c 0a20 2020  e(self.org),.   
+00016290: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
+000162a0: 5f70 6f69 6e74 2c0a 2020 2020 2020 2020  _point,.        
+000162b0: 290a 0a20 2020 2040 666f 7263 655f 6e6f  )..    @force_no
+000162c0: 646f 6375 6d65 6e74 0a20 2020 2064 6566  document.    def
+000162d0: 2072 656e 6465 725f 6465 6275 6728 0a20   render_debug(. 
+000162e0: 2020 2020 2020 2073 656c 662c 2067 7364         self, gsd
+000162f0: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
+00016300: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
+00016310: 7469 616c 5f70 6f69 6e74 2c20 6465 6275  tial_point, debu
+00016320: 675f 7374 7265 616d 2c20 7066 780a 2020  g_stream, pfx.  
+00016330: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+00016340: 0a20 2020 2020 2020 2052 656e 6465 7220  .        Render 
+00016350: 7468 6973 2070 6174 6820 656c 656d 656e  this path elemen
+00016360: 7420 746f 2069 7473 2050 4446 2072 6570  t to its PDF rep
+00016370: 7265 7365 6e74 6174 696f 6e20 616e 6420  resentation and 
+00016380: 7072 6f64 7563 6520 6465 6275 670a 2020  produce debug.  
+00016390: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
+000163a0: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
+000163b0: 3a0a 2020 2020 2020 2020 2020 2020 6773  :.            gs
+000163c0: 645f 7265 6769 7374 7279 2028 4772 6170  d_registry (Grap
+000163d0: 6869 6373 5374 6174 6544 6963 7452 6567  hicsStateDictReg
+000163e0: 6973 7472 7929 3a20 7468 6520 6f77 6e65  istry): the owne
+000163f0: 7227 7320 6772 6170 6869 6373 2073 7461  r's graphics sta
+00016400: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
+00016410: 2020 2064 6963 7469 6f6e 6172 7920 7265     dictionary re
+00016420: 6769 7374 7279 2e0a 2020 2020 2020 2020  gistry..        
+00016430: 2020 2020 7374 796c 6520 2847 7261 7068      style (Graph
+00016440: 6963 7353 7479 6c65 293a 2074 6865 2063  icsStyle): the c
+00016450: 7572 7265 6e74 2072 6573 6f6c 7665 6420  urrent resolved 
+00016460: 6772 6170 6869 6373 2073 7479 6c65 0a20  graphics style. 
+00016470: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+00016480: 6974 656d 3a20 7468 6520 7072 6576 696f  item: the previo
+00016490: 7573 2070 6174 6820 656c 656d 656e 742e  us path element.
+000164a0: 0a20 2020 2020 2020 2020 2020 2069 6e69  .            ini
+000164b0: 7469 616c 5f70 6f69 6e74 3a20 6c61 7374  tial_point: last
+000164c0: 2070 6f73 6974 696f 6e20 7365 7420 6279   position set by
+000164d0: 2061 2022 4d22 206f 7220 226d 2220 636f   a "M" or "m" co
+000164e0: 6d6d 616e 640a 2020 2020 2020 2020 2020  mmand.          
+000164f0: 2020 6465 6275 675f 7374 7265 616d 2028    debug_stream (
+00016500: 696f 2e54 6578 7449 4f29 3a20 7468 6520  io.TextIO): the 
+00016510: 7374 7265 616d 2074 6f20 7768 6963 6820  stream to which 
+00016520: 7468 6520 6465 6275 6720 6f75 7470 7574  the debug output
+00016530: 2073 686f 756c 6420 6265 0a20 2020 2020   should be.     
+00016540: 2020 2020 2020 2020 2020 2077 7269 7474             writt
+00016550: 656e 2e20 5468 6973 2069 7320 6e6f 7420  en. This is not 
+00016560: 6775 6172 616e 7465 6564 2074 6f20 6265  guaranteed to be
+00016570: 2073 6565 6b61 626c 6520 2865 2e67 2e20   seekable (e.g. 
+00016580: 6974 206d 6179 2062 6520 7374 646f 7574  it may be stdout
+00016590: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
+000165a0: 2020 2020 7374 6465 7272 292e 0a20 2020      stderr)..   
+000165b0: 2020 2020 2020 2020 2070 6678 2028 7374           pfx (st
+000165c0: 7229 3a20 7468 6520 6375 7272 656e 7420  r): the current 
+000165d0: 6465 6275 6720 6f75 7470 7574 2070 7265  debug output pre
+000165e0: 6669 7820 7374 7269 6e67 2028 6f6e 6c79  fix string (only
+000165f0: 206e 6565 6465 6420 6966 2065 6d69 7474   needed if emitt
+00016600: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00016610: 2020 2020 6d6f 7265 2074 6861 6e20 6f6e      more than on
+00016620: 6520 6c69 6e65 292e 0a0a 2020 2020 2020  e line)...      
+00016630: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00016640: 2020 2020 2020 2054 6865 2073 616d 6520         The same 
+00016650: 7475 706c 6520 6173 2060 5265 6374 616e  tuple as `Rectan
+00016660: 676c 652e 7265 6e64 6572 602e 0a20 2020  gle.render`..   
+00016670: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016680: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00016690: 6c65 3d75 6e75 7365 642d 6172 6775 6d65  le=unused-argume
+000166a0: 6e74 0a20 2020 2020 2020 2072 656e 6465  nt.        rende
+000166b0: 7265 642c 2072 6573 6f6c 7665 642c 2069  red, resolved, i
+000166c0: 6e69 7469 616c 5f70 6f69 6e74 203d 2073  nitial_point = s
+000166d0: 656c 662e 7265 6e64 6572 280a 2020 2020  elf.render(.    
+000166e0: 2020 2020 2020 2020 6773 645f 7265 6769          gsd_regi
+000166f0: 7374 7279 2c20 7374 796c 652c 206c 6173  stry, style, las
+00016700: 745f 6974 656d 2c20 696e 6974 6961 6c5f  t_item, initial_
+00016710: 706f 696e 740a 2020 2020 2020 2020 290a  point.        ).
+00016720: 2020 2020 2020 2020 6465 6275 675f 7374          debug_st
+00016730: 7265 616d 2e77 7269 7465 2866 227b 7365  ream.write(f"{se
+00016740: 6c66 7d20 7265 736f 6c76 6564 2074 6f20  lf} resolved to 
+00016750: 7b72 656e 6465 7265 647d 5c6e 2229 0a0a  {rendered}\n")..
+00016760: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00016770: 656e 6465 7265 642c 2072 6573 6f6c 7665  endered, resolve
+00016780: 642c 2069 6e69 7469 616c 5f70 6f69 6e74  d, initial_point
+00016790: 0a0a 0a63 6c61 7373 2052 6f75 6e64 6564  ...class Rounded
+000167a0: 5265 6374 616e 676c 6528 4e61 6d65 6454  Rectangle(NamedT
+000167b0: 7570 6c65 293a 0a20 2020 2022 2222 0a20  uple):.    """. 
+000167c0: 2020 2041 2072 6563 7461 6e67 6c65 2077     A rectangle w
+000167d0: 6974 6820 726f 756e 6465 6420 636f 726e  ith rounded corn
+000167e0: 6572 732e 0a0a 2020 2020 5365 653a 2060  ers...    See: `
+000167f0: 5061 696e 7465 6450 6174 682e 7265 6374  PaintedPath.rect
+00016800: 616e 676c 6560 0a20 2020 2022 2222 0a0a  angle`.    """..
+00016810: 2020 2020 6f72 673a 2050 6f69 6e74 0a20      org: Point. 
+00016820: 2020 2022 2222 5468 6520 746f 702d 6c65     """The top-le
+00016830: 6674 2063 6f72 6e65 7220 6f66 2074 6865  ft corner of the
+00016840: 2072 6563 7461 6e67 6c65 2e22 2222 0a20   rectangle.""". 
+00016850: 2020 2073 697a 653a 2050 6f69 6e74 0a20     size: Point. 
+00016860: 2020 2022 2222 5468 6520 7769 6474 6820     """The width 
+00016870: 616e 6420 6865 6967 6874 206f 6620 7468  and height of th
+00016880: 6520 7265 6374 616e 676c 652e 2222 220a  e rectangle.""".
+00016890: 2020 2020 636f 726e 6572 5f72 6164 6969      corner_radii
+000168a0: 3a20 506f 696e 740a 2020 2020 2222 2254  : Point.    """T
+000168b0: 6865 2078 2d20 616e 6420 792d 7261 6469  he x- and y-radi
+000168c0: 7573 206f 6620 7468 6520 636f 726e 6572  us of the corner
+000168d0: 732e 2222 220a 0a20 2020 2064 6566 205f  s."""..    def _
+000168e0: 6465 636f 6d70 6f73 6528 7365 6c66 293a  decompose(self):
+000168f0: 0a20 2020 2020 2020 2069 7465 6d73 203d  .        items =
+00016900: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
+00016910: 2873 656c 662e 7369 7a65 2e78 203d 3d20  (self.size.x == 
+00016920: 3029 2061 6e64 2028 7365 6c66 2e73 697a  0) and (self.siz
+00016930: 652e 7920 3d3d 2030 293a 0a20 2020 2020  e.y == 0):.     
+00016940: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00016950: 2020 2020 656c 6966 2028 7365 6c66 2e73      elif (self.s
+00016960: 697a 652e 7820 3d3d 2030 2920 6f72 2028  ize.x == 0) or (
+00016970: 7365 6c66 2e73 697a 652e 7920 3d3d 2030  self.size.y == 0
+00016980: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00016990: 7465 6d73 2e61 7070 656e 6428 4d6f 7665  tems.append(Move
+000169a0: 2873 656c 662e 6f72 6729 290a 2020 2020  (self.org)).    
+000169b0: 2020 2020 2020 2020 6974 656d 732e 6170          items.ap
+000169c0: 7065 6e64 284c 696e 6528 7365 6c66 2e6f  pend(Line(self.o
+000169d0: 7267 202b 2073 656c 662e 7369 7a65 2929  rg + self.size))
+000169e0: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
+000169f0: 6d73 2e61 7070 656e 6428 436c 6f73 6528  ms.append(Close(
+00016a00: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
+00016a10: 2873 656c 662e 636f 726e 6572 5f72 6164  (self.corner_rad
+00016a20: 6969 2e78 203d 3d20 3029 206f 7220 2873  ii.x == 0) or (s
+00016a30: 656c 662e 636f 726e 6572 5f72 6164 6969  elf.corner_radii
+00016a40: 2e79 203d 3d20 3029 3a0a 2020 2020 2020  .y == 0):.      
+00016a50: 2020 2020 2020 6974 656d 732e 6170 7065        items.appe
+00016a60: 6e64 2852 6563 7461 6e67 6c65 2873 656c  nd(Rectangle(sel
+00016a70: 662e 6f72 672c 2073 656c 662e 7369 7a65  f.org, self.size
+00016a80: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
+00016a90: 0a20 2020 2020 2020 2020 2020 2078 2c20  .            x, 
+00016aa0: 7920 3d20 7365 6c66 2e6f 7267 0a20 2020  y = self.org.   
+00016ab0: 2020 2020 2020 2020 2077 2c20 6820 3d20           w, h = 
+00016ac0: 7365 6c66 2e73 697a 650a 2020 2020 2020  self.size.      
+00016ad0: 2020 2020 2020 7278 2c20 7279 203d 2073        rx, ry = s
+00016ae0: 656c 662e 636f 726e 6572 5f72 6164 6969  elf.corner_radii
+00016af0: 0a20 2020 2020 2020 2020 2020 2073 6967  .            sig
+00016b00: 6e5f 7769 6474 6820 3d20 2873 656c 662e  n_width = (self.
+00016b10: 7369 7a65 2e78 203e 3d20 3029 202d 2028  size.x >= 0) - (
+00016b20: 7365 6c66 2e73 697a 652e 7820 3c20 3029  self.size.x < 0)
+00016b30: 0a20 2020 2020 2020 2020 2020 2073 6967  .            sig
+00016b40: 6e5f 6865 6967 6874 203d 2028 7365 6c66  n_height = (self
+00016b50: 2e73 697a 652e 7920 3e3d 2030 2920 2d20  .size.y >= 0) - 
+00016b60: 2873 656c 662e 7369 7a65 2e79 203c 2030  (self.size.y < 0
+00016b70: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00016b80: 6620 6162 7328 7278 2920 3e20 6162 7328  f abs(rx) > abs(
+00016b90: 7729 3a0a 2020 2020 2020 2020 2020 2020  w):.            
+00016ba0: 2020 2020 7278 203d 2073 656c 662e 7369      rx = self.si
+00016bb0: 7a65 2e78 0a0a 2020 2020 2020 2020 2020  ze.x..          
+00016bc0: 2020 6966 2061 6273 2872 7929 203e 2061    if abs(ry) > a
+00016bd0: 6273 2868 293a 0a20 2020 2020 2020 2020  bs(h):.         
+00016be0: 2020 2020 2020 2072 7920 3d20 7365 6c66         ry = self
+00016bf0: 2e73 697a 652e 790a 0a20 2020 2020 2020  .size.y..       
+00016c00: 2020 2020 2072 7820 3d20 7369 676e 5f77       rx = sign_w
+00016c10: 6964 7468 202a 2061 6273 2872 7829 0a20  idth * abs(rx). 
+00016c20: 2020 2020 2020 2020 2020 2072 7920 3d20             ry = 
+00016c30: 7369 676e 5f68 6569 6768 7420 2a20 6162  sign_height * ab
+00016c40: 7328 7279 290a 2020 2020 2020 2020 2020  s(ry).          
+00016c50: 2020 6172 635f 7261 6420 3d20 506f 696e    arc_rad = Poin
+00016c60: 7428 7278 2c20 7279 290a 0a20 2020 2020  t(rx, ry)..     
+00016c70: 2020 2020 2020 2069 7465 6d73 2e61 7070         items.app
+00016c80: 656e 6428 4d6f 7665 2850 6f69 6e74 2878  end(Move(Point(x
+00016c90: 202b 2072 782c 2079 2929 290a 2020 2020   + rx, y))).    
+00016ca0: 2020 2020 2020 2020 6974 656d 732e 6170          items.ap
+00016cb0: 7065 6e64 284c 696e 6528 506f 696e 7428  pend(Line(Point(
+00016cc0: 7820 2b20 7720 2d20 7278 2c20 7929 2929  x + w - rx, y)))
+00016cd0: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
+00016ce0: 6d73 2e61 7070 656e 6428 4172 6328 6172  ms.append(Arc(ar
+00016cf0: 635f 7261 642c 2030 2c20 4661 6c73 652c  c_rad, 0, False,
+00016d00: 2054 7275 652c 2050 6f69 6e74 2878 202b   True, Point(x +
+00016d10: 2077 2c20 7920 2b20 7279 2929 290a 2020   w, y + ry))).  
+00016d20: 2020 2020 2020 2020 2020 6974 656d 732e            items.
+00016d30: 6170 7065 6e64 284c 696e 6528 506f 696e  append(Line(Poin
+00016d40: 7428 7820 2b20 772c 2079 202b 2068 202d  t(x + w, y + h -
+00016d50: 2072 7929 2929 0a20 2020 2020 2020 2020   ry))).         
+00016d60: 2020 2069 7465 6d73 2e61 7070 656e 6428     items.append(
+00016d70: 4172 6328 6172 635f 7261 642c 2030 2c20  Arc(arc_rad, 0, 
+00016d80: 4661 6c73 652c 2054 7275 652c 2050 6f69  False, True, Poi
+00016d90: 6e74 2878 202b 2077 202d 2072 782c 2079  nt(x + w - rx, y
+00016da0: 202b 2068 2929 290a 2020 2020 2020 2020   + h))).        
+00016db0: 2020 2020 6974 656d 732e 6170 7065 6e64      items.append
+00016dc0: 284c 696e 6528 506f 696e 7428 7820 2b20  (Line(Point(x + 
+00016dd0: 7278 2c20 7920 2b20 6829 2929 0a20 2020  rx, y + h))).   
+00016de0: 2020 2020 2020 2020 2069 7465 6d73 2e61           items.a
+00016df0: 7070 656e 6428 4172 6328 6172 635f 7261  ppend(Arc(arc_ra
+00016e00: 642c 2030 2c20 4661 6c73 652c 2054 7275  d, 0, False, Tru
+00016e10: 652c 2050 6f69 6e74 2878 2c20 7920 2b20  e, Point(x, y + 
+00016e20: 6820 2d20 7279 2929 290a 2020 2020 2020  h - ry))).      
+00016e30: 2020 2020 2020 6974 656d 732e 6170 7065        items.appe
+00016e40: 6e64 284c 696e 6528 506f 696e 7428 782c  nd(Line(Point(x,
+00016e50: 2079 202b 2072 7929 2929 0a20 2020 2020   y + ry))).     
+00016e60: 2020 2020 2020 2069 7465 6d73 2e61 7070         items.app
+00016e70: 656e 6428 4172 6328 6172 635f 7261 642c  end(Arc(arc_rad,
+00016e80: 2030 2c20 4661 6c73 652c 2054 7275 652c   0, False, True,
+00016e90: 2050 6f69 6e74 2878 202b 2072 782c 2079   Point(x + rx, y
 00016ea0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00016eb0: 6974 656d 732e 6170 7065 6e64 284c 696e  items.append(Lin
-00016ec0: 6528 506f 696e 7428 7820 2b20 7278 2c20  e(Point(x + rx, 
-00016ed0: 7920 2b20 6829 2929 0a20 2020 2020 2020  y + h))).       
-00016ee0: 2020 2020 2069 7465 6d73 2e61 7070 656e       items.appen
-00016ef0: 6428 4172 6328 6172 635f 7261 642c 2030  d(Arc(arc_rad, 0
-00016f00: 2c20 4661 6c73 652c 2054 7275 652c 2050  , False, True, P
-00016f10: 6f69 6e74 2878 2c20 7920 2b20 6820 2d20  oint(x, y + h - 
-00016f20: 7279 2929 290a 2020 2020 2020 2020 2020  ry))).          
-00016f30: 2020 6974 656d 732e 6170 7065 6e64 284c    items.append(L
-00016f40: 696e 6528 506f 696e 7428 782c 2079 202b  ine(Point(x, y +
-00016f50: 2072 7929 2929 0a20 2020 2020 2020 2020   ry))).         
-00016f60: 2020 2069 7465 6d73 2e61 7070 656e 6428     items.append(
-00016f70: 4172 6328 6172 635f 7261 642c 2030 2c20  Arc(arc_rad, 0, 
-00016f80: 4661 6c73 652c 2054 7275 652c 2050 6f69  False, True, Poi
-00016f90: 6e74 2878 202b 2072 782c 2079 2929 290a  nt(x + rx, y))).
-00016fa0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-00016fb0: 732e 6170 7065 6e64 2843 6c6f 7365 2829  s.append(Close()
-00016fc0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00016fd0: 6e20 6974 656d 730a 0a20 2020 2040 666f  n items..    @fo
-00016fe0: 7263 655f 6e6f 646f 6375 6d65 6e74 0a20  rce_nodocument. 
-00016ff0: 2020 2064 6566 2072 656e 6465 7228 7365     def render(se
-00017000: 6c66 2c20 6773 645f 7265 6769 7374 7279  lf, gsd_registry
-00017010: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
-00017020: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
-00017030: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
-00017040: 2020 2020 2020 2020 5265 6e64 6572 2074          Render t
-00017050: 6869 7320 7061 7468 2065 6c65 6d65 6e74  his path element
-00017060: 2074 6f20 6974 7320 5044 4620 7265 7072   to its PDF repr
-00017070: 6573 656e 7461 7469 6f6e 2e0a 0a20 2020  esentation...   
-00017080: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00017090: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
-000170a0: 7472 7920 2847 7261 7068 6963 7353 7461  try (GraphicsSta
-000170b0: 7465 4469 6374 5265 6769 7374 7279 293a  teDictRegistry):
-000170c0: 2074 6865 206f 776e 6572 2773 2067 7261   the owner's gra
-000170d0: 7068 6963 7320 7374 6174 650a 2020 2020  phics state.    
-000170e0: 2020 2020 2020 2020 2020 2020 6469 6374              dict
-000170f0: 696f 6e61 7279 2072 6567 6973 7472 792e  ionary registry.
-00017100: 0a20 2020 2020 2020 2020 2020 2073 7479  .            sty
-00017110: 6c65 2028 4772 6170 6869 6373 5374 796c  le (GraphicsStyl
-00017120: 6529 3a20 7468 6520 6375 7272 656e 7420  e): the current 
-00017130: 7265 736f 6c76 6564 2067 7261 7068 6963  resolved graphic
-00017140: 7320 7374 796c 650a 2020 2020 2020 2020  s style.        
-00017150: 2020 2020 6c61 7374 5f69 7465 6d3a 2074      last_item: t
-00017160: 6865 2070 7265 7669 6f75 7320 7061 7468  he previous path
-00017170: 2065 6c65 6d65 6e74 2e0a 2020 2020 2020   element..      
-00017180: 2020 2020 2020 696e 6974 6961 6c5f 706f        initial_po
-00017190: 696e 743a 206c 6173 7420 706f 7369 7469  int: last positi
-000171a0: 6f6e 2073 6574 2062 7920 6120 224d 2220  on set by a "M" 
-000171b0: 6f72 2022 6d22 2063 6f6d 6d61 6e64 0a0a  or "m" command..
-000171c0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-000171d0: 0a20 2020 2020 2020 2020 2020 2061 2074  .            a t
-000171e0: 7570 6c65 206f 6620 6028 7374 722c 206e  uple of `(str, n
-000171f0: 6577 5f6c 6173 745f 6974 656d 2960 2c20  ew_last_item)`, 
-00017200: 7768 6572 6520 606e 6577 5f6c 6173 745f  where `new_last_
-00017210: 6974 656d 6020 6973 2061 2072 6573 6f6c  item` is a resol
-00017220: 7665 640a 2020 2020 2020 2020 2020 2020  ved.            
-00017230: 604c 696e 6560 2e0a 2020 2020 2020 2020  `Line`..        
-00017240: 2222 220a 2020 2020 2020 2020 2320 7079  """.        # py
-00017250: 6c69 6e74 3a20 6469 7361 626c 653d 756e  lint: disable=un
-00017260: 7573 6564 2d61 7267 756d 656e 740a 2020  used-argument.  
-00017270: 2020 2020 2020 636f 6d70 6f6e 656e 7473        components
-00017280: 203d 2073 656c 662e 5f64 6563 6f6d 706f   = self._decompo
-00017290: 7365 2829 0a0a 2020 2020 2020 2020 6966  se()..        if
-000172a0: 206e 6f74 2063 6f6d 706f 6e65 6e74 733a   not components:
-000172b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000172c0: 7572 6e20 2222 2c20 6c61 7374 5f69 7465  urn "", last_ite
-000172d0: 6d0a 0a20 2020 2020 2020 2072 656e 6465  m..        rende
-000172e0: 725f 6c69 7374 203d 205b 5d0a 2020 2020  r_list = [].    
-000172f0: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
-00017300: 636f 6d70 6f6e 656e 7473 3a0a 2020 2020  components:.    
-00017310: 2020 2020 2020 2020 7265 6e64 6572 6564          rendered
-00017320: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
-00017330: 7469 616c 5f70 6f69 6e74 203d 2069 7465  tial_point = ite
-00017340: 6d2e 7265 6e64 6572 280a 2020 2020 2020  m.render(.      
-00017350: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-00017360: 6769 7374 7279 2c20 7374 796c 652c 206c  gistry, style, l
-00017370: 6173 745f 6974 656d 2c20 696e 6974 6961  ast_item, initia
-00017380: 6c5f 706f 696e 740a 2020 2020 2020 2020  l_point.        
-00017390: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000173a0: 2020 7265 6e64 6572 5f6c 6973 742e 6170    render_list.ap
-000173b0: 7065 6e64 2872 656e 6465 7265 6429 0a0a  pend(rendered)..
-000173c0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-000173d0: 2022 2e6a 6f69 6e28 7265 6e64 6572 5f6c   ".join(render_l
-000173e0: 6973 7429 2c20 4c69 6e65 2873 656c 662e  ist), Line(self.
-000173f0: 6f72 6729 2c20 696e 6974 6961 6c5f 706f  org), initial_po
-00017400: 696e 740a 0a20 2020 2040 666f 7263 655f  int..    @force_
-00017410: 6e6f 646f 6375 6d65 6e74 0a20 2020 2064  nodocument.    d
-00017420: 6566 2072 656e 6465 725f 6465 6275 6728  ef render_debug(
-00017430: 0a20 2020 2020 2020 2073 656c 662c 2067  .        self, g
-00017440: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
-00017450: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
-00017460: 6e69 7469 616c 5f70 6f69 6e74 2c20 6465  nitial_point, de
-00017470: 6275 675f 7374 7265 616d 2c20 7066 780a  bug_stream, pfx.
-00017480: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00017490: 2222 0a20 2020 2020 2020 2052 656e 6465  "".        Rende
-000174a0: 7220 7468 6973 2070 6174 6820 656c 656d  r this path elem
-000174b0: 656e 7420 746f 2069 7473 2050 4446 2072  ent to its PDF r
-000174c0: 6570 7265 7365 6e74 6174 696f 6e20 616e  epresentation an
-000174d0: 6420 7072 6f64 7563 6520 6465 6275 670a  d produce debug.
-000174e0: 2020 2020 2020 2020 696e 666f 726d 6174          informat
-000174f0: 696f 6e2e 0a0a 2020 2020 2020 2020 4172  ion...        Ar
-00017500: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00017510: 6773 645f 7265 6769 7374 7279 2028 4772  gsd_registry (Gr
-00017520: 6170 6869 6373 5374 6174 6544 6963 7452  aphicsStateDictR
-00017530: 6567 6973 7472 7929 3a20 7468 6520 6f77  egistry): the ow
-00017540: 6e65 7227 7320 6772 6170 6869 6373 2073  ner's graphics s
-00017550: 7461 7465 0a20 2020 2020 2020 2020 2020  tate.           
-00017560: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
-00017570: 7265 6769 7374 7279 2e0a 2020 2020 2020  registry..      
-00017580: 2020 2020 2020 7374 796c 6520 2847 7261        style (Gra
-00017590: 7068 6963 7353 7479 6c65 293a 2074 6865  phicsStyle): the
-000175a0: 2063 7572 7265 6e74 2072 6573 6f6c 7665   current resolve
-000175b0: 6420 6772 6170 6869 6373 2073 7479 6c65  d graphics style
-000175c0: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
-000175d0: 745f 6974 656d 3a20 7468 6520 7072 6576  t_item: the prev
-000175e0: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
-000175f0: 742e 0a20 2020 2020 2020 2020 2020 2069  t..            i
-00017600: 6e69 7469 616c 5f70 6f69 6e74 3a20 6c61  nitial_point: la
-00017610: 7374 2070 6f73 6974 696f 6e20 7365 7420  st position set 
-00017620: 6279 2061 2022 4d22 206f 7220 226d 2220  by a "M" or "m" 
-00017630: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
-00017640: 2020 2020 6465 6275 675f 7374 7265 616d      debug_stream
-00017650: 2028 696f 2e54 6578 7449 4f29 3a20 7468   (io.TextIO): th
-00017660: 6520 7374 7265 616d 2074 6f20 7768 6963  e stream to whic
-00017670: 6820 7468 6520 6465 6275 6720 6f75 7470  h the debug outp
-00017680: 7574 2073 686f 756c 6420 6265 0a20 2020  ut should be.   
-00017690: 2020 2020 2020 2020 2020 2020 2077 7269               wri
-000176a0: 7474 656e 2e20 5468 6973 2069 7320 6e6f  tten. This is no
-000176b0: 7420 6775 6172 616e 7465 6564 2074 6f20  t guaranteed to 
-000176c0: 6265 2073 6565 6b61 626c 6520 2865 2e67  be seekable (e.g
-000176d0: 2e20 6974 206d 6179 2062 6520 7374 646f  . it may be stdo
-000176e0: 7574 206f 720a 2020 2020 2020 2020 2020  ut or.          
-000176f0: 2020 2020 2020 7374 6465 7272 292e 0a20        stderr).. 
-00017700: 2020 2020 2020 2020 2020 2070 6678 2028             pfx (
-00017710: 7374 7229 3a20 7468 6520 6375 7272 656e  str): the curren
-00017720: 7420 6465 6275 6720 6f75 7470 7574 2070  t debug output p
-00017730: 7265 6669 7820 7374 7269 6e67 2028 6f6e  refix string (on
-00017740: 6c79 206e 6565 6465 6420 6966 2065 6d69  ly needed if emi
-00017750: 7474 696e 670a 2020 2020 2020 2020 2020  tting.          
-00017760: 2020 2020 2020 6d6f 7265 2074 6861 6e20        more than 
-00017770: 6f6e 6520 6c69 6e65 292e 0a0a 2020 2020  one line)...    
-00017780: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00017790: 2020 2020 2020 2020 2054 6865 2073 616d           The sam
-000177a0: 6520 7475 706c 6520 6173 2060 526f 756e  e tuple as `Roun
-000177b0: 6465 6452 6563 7461 6e67 6c65 2e72 656e  dedRectangle.ren
-000177c0: 6465 7260 2e0a 2020 2020 2020 2020 2222  der`..        ""
-000177d0: 220a 2020 2020 2020 2020 2320 7079 6c69  ".        # pyli
-000177e0: 6e74 3a20 6469 7361 626c 653d 756e 7573  nt: disable=unus
-000177f0: 6564 2d61 7267 756d 656e 740a 2020 2020  ed-argument.    
-00017800: 2020 2020 636f 6d70 6f6e 656e 7473 203d      components =
-00017810: 2073 656c 662e 5f64 6563 6f6d 706f 7365   self._decompose
-00017820: 2829 0a0a 2020 2020 2020 2020 6465 6275  ()..        debu
-00017830: 675f 7374 7265 616d 2e77 7269 7465 2866  g_stream.write(f
-00017840: 227b 7365 6c66 7d20 7265 736f 6c76 6564  "{self} resolved
-00017850: 2074 6f3a 5c6e 2229 0a20 2020 2020 2020   to:\n").       
-00017860: 2069 6620 6e6f 7420 636f 6d70 6f6e 656e   if not componen
-00017870: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00017880: 6465 6275 675f 7374 7265 616d 2e77 7269  debug_stream.wri
-00017890: 7465 2870 6678 202b 2022 20e2 9494 e294  te(pfx + " .....
-000178a0: 8020 6e6f 7468 696e 675c 6e22 290a 2020  . nothing\n").  
-000178b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000178c0: 2022 222c 206c 6173 745f 6974 656d 0a0a   "", last_item..
-000178d0: 2020 2020 2020 2020 7265 6e64 6572 5f6c          render_l
-000178e0: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
-000178f0: 2066 6f72 2069 7465 6d20 696e 2063 6f6d   for item in com
-00017900: 706f 6e65 6e74 735b 3a2d 315d 3a0a 2020  ponents[:-1]:.  
-00017910: 2020 2020 2020 2020 2020 7265 6e64 6572            render
-00017920: 6564 2c20 6c61 7374 5f69 7465 6d2c 2069  ed, last_item, i
-00017930: 6e69 7469 616c 5f70 6f69 6e74 203d 2069  nitial_point = i
-00017940: 7465 6d2e 7265 6e64 6572 280a 2020 2020  tem.render(.    
-00017950: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
-00017960: 7265 6769 7374 7279 2c20 7374 796c 652c  registry, style,
-00017970: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
-00017980: 6961 6c5f 706f 696e 740a 2020 2020 2020  ial_point.      
-00017990: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000179a0: 2020 2020 6465 6275 675f 7374 7265 616d      debug_stream
-000179b0: 2e77 7269 7465 2870 6678 202b 2066 2220  .write(pfx + f" 
-000179c0: e294 9ce2 9480 207b 6974 656d 7d5c 6e22  ...... {item}\n"
-000179d0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000179e0: 6e64 6572 5f6c 6973 742e 6170 7065 6e64  nder_list.append
-000179f0: 2872 656e 6465 7265 6429 0a0a 2020 2020  (rendered)..    
-00017a00: 2020 2020 7265 6e64 6572 6564 2c20 6c61      rendered, la
-00017a10: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
-00017a20: 5f70 6f69 6e74 203d 2063 6f6d 706f 6e65  _point = compone
-00017a30: 6e74 735b 2d31 5d2e 7265 6e64 6572 280a  nts[-1].render(.
-00017a40: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
-00017a50: 7265 6769 7374 7279 2c20 7374 796c 652c  registry, style,
-00017a60: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
-00017a70: 6961 6c5f 706f 696e 740a 2020 2020 2020  ial_point.      
-00017a80: 2020 290a 2020 2020 2020 2020 6465 6275    ).        debu
-00017a90: 675f 7374 7265 616d 2e77 7269 7465 2870  g_stream.write(p
-00017aa0: 6678 202b 2066 2220 e294 94e2 9480 207b  fx + f" ...... {
-00017ab0: 636f 6d70 6f6e 656e 7473 5b2d 315d 7d5c  components[-1]}\
-00017ac0: 6e22 290a 2020 2020 2020 2020 7265 6e64  n").        rend
-00017ad0: 6572 5f6c 6973 742e 6170 7065 6e64 2872  er_list.append(r
-00017ae0: 656e 6465 7265 6429 0a0a 2020 2020 2020  endered)..      
-00017af0: 2020 7265 7475 726e 2022 2022 2e6a 6f69    return " ".joi
-00017b00: 6e28 7265 6e64 6572 5f6c 6973 7429 2c20  n(render_list), 
-00017b10: 4c69 6e65 2873 656c 662e 6f72 6729 2c20  Line(self.org), 
-00017b20: 696e 6974 6961 6c5f 706f 696e 740a 0a0a  initial_point...
-00017b30: 636c 6173 7320 456c 6c69 7073 6528 4e61  class Ellipse(Na
-00017b40: 6d65 6454 7570 6c65 293a 0a20 2020 2022  medTuple):.    "
-00017b50: 2222 0a20 2020 2041 6e20 656c 6c69 7073  "".    An ellips
-00017b60: 652e 0a0a 2020 2020 5365 653a 2060 5061  e...    See: `Pa
-00017b70: 696e 7465 6450 6174 682e 656c 6c69 7073  intedPath.ellips
-00017b80: 6560 0a20 2020 2022 2222 0a0a 2020 2020  e`.    """..    
-00017b90: 7261 6469 693a 2050 6f69 6e74 0a20 2020  radii: Point.   
-00017ba0: 2022 2222 5468 6520 782d 2061 6e64 2079   """The x- and y
-00017bb0: 2d72 6164 6969 206f 6620 7468 6520 656c  -radii of the el
-00017bc0: 6c69 7073 6522 2222 0a20 2020 2063 656e  lipse""".    cen
-00017bd0: 7465 723a 2050 6f69 6e74 0a20 2020 2022  ter: Point.    "
-00017be0: 2222 5468 6520 6162 7363 6973 7361 2061  ""The abscissa a
-00017bf0: 6e64 206f 7264 696e 6174 6520 6f66 2074  nd ordinate of t
-00017c00: 6865 2063 656e 7465 7220 6f66 2074 6865  he center of the
-00017c10: 2065 6c6c 6970 7365 2222 220a 0a20 2020   ellipse"""..   
-00017c20: 2064 6566 205f 6465 636f 6d70 6f73 6528   def _decompose(
-00017c30: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00017c40: 7465 6d73 203d 205b 5d0a 0a20 2020 2020  tems = []..     
-00017c50: 2020 2072 7820 3d20 6162 7328 7365 6c66     rx = abs(self
-00017c60: 2e72 6164 6969 2e78 290a 2020 2020 2020  .radii.x).      
-00017c70: 2020 7279 203d 2061 6273 2873 656c 662e    ry = abs(self.
-00017c80: 7261 6469 692e 7929 0a20 2020 2020 2020  radii.y).       
-00017c90: 2063 782c 2063 7920 3d20 7365 6c66 2e63   cx, cy = self.c
-00017ca0: 656e 7465 720a 0a20 2020 2020 2020 2061  enter..        a
-00017cb0: 7263 5f72 6164 203d 2050 6f69 6e74 2872  rc_rad = Point(r
-00017cc0: 782c 2072 7929 0a0a 2020 2020 2020 2020  x, ry)..        
-00017cd0: 2320 7468 6973 2069 736e 2774 2074 6865  # this isn't the
-00017ce0: 206d 6f73 7420 6566 6669 6369 656e 7420   most efficient 
-00017cf0: 7761 7920 746f 2064 6f20 7468 6973 2c20  way to do this, 
-00017d00: 636f 6d70 7574 6174 696f 6e61 6c6c 792c  computationally,
-00017d10: 2062 7574 2069 7427 730a 2020 2020 2020   but it's.      
-00017d20: 2020 2320 696e 7465 726e 616c 6c79 2063    # internally c
-00017d30: 6f6e 7369 7374 656e 742e 0a20 2020 2020  onsistent..     
-00017d40: 2020 2069 6620 2872 7820 213d 2030 2920     if (rx != 0) 
-00017d50: 616e 6420 2872 7920 213d 2030 293a 0a20  and (ry != 0):. 
-00017d60: 2020 2020 2020 2020 2020 2069 7465 6d73             items
-00017d70: 2e61 7070 656e 6428 4d6f 7665 2850 6f69  .append(Move(Poi
-00017d80: 6e74 2863 7820 2b20 7278 2c20 6379 2929  nt(cx + rx, cy))
-00017d90: 290a 2020 2020 2020 2020 2020 2020 6974  ).            it
-00017da0: 656d 732e 6170 7065 6e64 2841 7263 2861  ems.append(Arc(a
-00017db0: 7263 5f72 6164 2c20 302c 2046 616c 7365  rc_rad, 0, False
-00017dc0: 2c20 5472 7565 2c20 506f 696e 7428 6378  , True, Point(cx
-00017dd0: 2c20 6379 202b 2072 7929 2929 0a20 2020  , cy + ry))).   
-00017de0: 2020 2020 2020 2020 2069 7465 6d73 2e61           items.a
-00017df0: 7070 656e 6428 4172 6328 6172 635f 7261  ppend(Arc(arc_ra
-00017e00: 642c 2030 2c20 4661 6c73 652c 2054 7275  d, 0, False, Tru
-00017e10: 652c 2050 6f69 6e74 2863 7820 2d20 7278  e, Point(cx - rx
-00017e20: 2c20 6379 2929 290a 2020 2020 2020 2020  , cy))).        
-00017e30: 2020 2020 6974 656d 732e 6170 7065 6e64      items.append
-00017e40: 2841 7263 2861 7263 5f72 6164 2c20 302c  (Arc(arc_rad, 0,
-00017e50: 2046 616c 7365 2c20 5472 7565 2c20 506f   False, True, Po
-00017e60: 696e 7428 6378 2c20 6379 202d 2072 7929  int(cx, cy - ry)
-00017e70: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
-00017e80: 7465 6d73 2e61 7070 656e 6428 4172 6328  tems.append(Arc(
-00017e90: 6172 635f 7261 642c 2030 2c20 4661 6c73  arc_rad, 0, Fals
-00017ea0: 652c 2054 7275 652c 2050 6f69 6e74 2863  e, True, Point(c
-00017eb0: 7820 2b20 7278 2c20 6379 2929 290a 2020  x + rx, cy))).  
-00017ec0: 2020 2020 2020 2020 2020 6974 656d 732e            items.
-00017ed0: 6170 7065 6e64 2843 6c6f 7365 2829 290a  append(Close()).
-00017ee0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017ef0: 6974 656d 730a 0a20 2020 2040 666f 7263  items..    @forc
-00017f00: 655f 6e6f 646f 6375 6d65 6e74 0a20 2020  e_nodocument.   
-00017f10: 2064 6566 2072 656e 6465 7228 7365 6c66   def render(self
-00017f20: 2c20 6773 645f 7265 6769 7374 7279 2c20  , gsd_registry, 
-00017f30: 7374 796c 652c 206c 6173 745f 6974 656d  style, last_item
-00017f40: 2c20 696e 6974 6961 6c5f 706f 696e 7429  , initial_point)
-00017f50: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00017f60: 2020 2020 2020 5265 6e64 6572 2074 6869        Render thi
-00017f70: 7320 7061 7468 2065 6c65 6d65 6e74 2074  s path element t
-00017f80: 6f20 6974 7320 5044 4620 7265 7072 6573  o its PDF repres
-00017f90: 656e 7461 7469 6f6e 2e0a 0a20 2020 2020  entation...     
-00017fa0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00017fb0: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
-00017fc0: 7920 2847 7261 7068 6963 7353 7461 7465  y (GraphicsState
-00017fd0: 4469 6374 5265 6769 7374 7279 293a 2074  DictRegistry): t
-00017fe0: 6865 206f 776e 6572 2773 2067 7261 7068  he owner's graph
-00017ff0: 6963 7320 7374 6174 650a 2020 2020 2020  ics state.      
-00018000: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
-00018010: 6e61 7279 2072 6567 6973 7472 792e 0a20  nary registry.. 
-00018020: 2020 2020 2020 2020 2020 2073 7479 6c65             style
-00018030: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
-00018040: 3a20 7468 6520 6375 7272 656e 7420 7265  : the current re
-00018050: 736f 6c76 6564 2067 7261 7068 6963 7320  solved graphics 
-00018060: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
-00018070: 2020 6c61 7374 5f69 7465 6d3a 2074 6865    last_item: the
-00018080: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
-00018090: 6c65 6d65 6e74 2e0a 2020 2020 2020 2020  lement..        
-000180a0: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
-000180b0: 743a 206c 6173 7420 706f 7369 7469 6f6e  t: last position
-000180c0: 2073 6574 2062 7920 6120 224d 2220 6f72   set by a "M" or
-000180d0: 2022 6d22 2063 6f6d 6d61 6e64 0a0a 2020   "m" command..  
-000180e0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-000180f0: 2020 2020 2020 2020 2020 2061 2074 7570             a tup
-00018100: 6c65 206f 6620 6028 7374 722c 206e 6577  le of `(str, new
-00018110: 5f6c 6173 745f 6974 656d 2960 2c20 7768  _last_item)`, wh
-00018120: 6572 6520 606e 6577 5f6c 6173 745f 6974  ere `new_last_it
-00018130: 656d 6020 6973 2061 2072 6573 6f6c 7665  em` is a resolve
-00018140: 640a 2020 2020 2020 2020 2020 2020 604d  d.            `M
-00018150: 6f76 6560 2074 6f20 7468 6520 6365 6e74  ove` to the cent
-00018160: 6572 206f 6620 7468 6520 656c 6c69 7073  er of the ellips
-00018170: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00018180: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
-00018190: 2064 6973 6162 6c65 3d75 6e75 7365 642d   disable=unused-
-000181a0: 6172 6775 6d65 6e74 0a20 2020 2020 2020  argument.       
-000181b0: 2063 6f6d 706f 6e65 6e74 7320 3d20 7365   components = se
-000181c0: 6c66 2e5f 6465 636f 6d70 6f73 6528 290a  lf._decompose().
-000181d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000181e0: 636f 6d70 6f6e 656e 7473 3a0a 2020 2020  components:.    
-000181f0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00018200: 222c 206c 6173 745f 6974 656d 0a0a 2020  ", last_item..  
-00018210: 2020 2020 2020 7265 6e64 6572 5f6c 6973        render_lis
-00018220: 7420 3d20 5b5d 0a20 2020 2020 2020 2066  t = [].        f
-00018230: 6f72 2069 7465 6d20 696e 2063 6f6d 706f  or item in compo
-00018240: 6e65 6e74 733a 0a20 2020 2020 2020 2020  nents:.         
-00018250: 2020 2072 656e 6465 7265 642c 206c 6173     rendered, las
-00018260: 745f 6974 656d 2c20 696e 6974 6961 6c5f  t_item, initial_
-00018270: 706f 696e 7420 3d20 6974 656d 2e72 656e  point = item.ren
-00018280: 6465 7228 0a20 2020 2020 2020 2020 2020  der(.           
-00018290: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
-000182a0: 792c 2073 7479 6c65 2c20 6c61 7374 5f69  y, style, last_i
-000182b0: 7465 6d2c 2069 6e69 7469 616c 5f70 6f69  tem, initial_poi
-000182c0: 6e74 0a20 2020 2020 2020 2020 2020 2029  nt.            )
-000182d0: 0a20 2020 2020 2020 2020 2020 2072 656e  .            ren
-000182e0: 6465 725f 6c69 7374 2e61 7070 656e 6428  der_list.append(
-000182f0: 7265 6e64 6572 6564 290a 0a20 2020 2020  rendered)..     
-00018300: 2020 2072 6574 7572 6e20 2220 222e 6a6f     return " ".jo
-00018310: 696e 2872 656e 6465 725f 6c69 7374 292c  in(render_list),
-00018320: 204d 6f76 6528 7365 6c66 2e63 656e 7465   Move(self.cente
-00018330: 7229 2c20 696e 6974 6961 6c5f 706f 696e  r), initial_poin
-00018340: 740a 0a20 2020 2040 666f 7263 655f 6e6f  t..    @force_no
-00018350: 646f 6375 6d65 6e74 0a20 2020 2064 6566  document.    def
-00018360: 2072 656e 6465 725f 6465 6275 6728 0a20   render_debug(. 
-00018370: 2020 2020 2020 2073 656c 662c 2067 7364         self, gsd
-00018380: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
-00018390: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
-000183a0: 7469 616c 5f70 6f69 6e74 2c20 6465 6275  tial_point, debu
-000183b0: 675f 7374 7265 616d 2c20 7066 780a 2020  g_stream, pfx.  
-000183c0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-000183d0: 0a20 2020 2020 2020 2052 656e 6465 7220  .        Render 
-000183e0: 7468 6973 2070 6174 6820 656c 656d 656e  this path elemen
-000183f0: 7420 746f 2069 7473 2050 4446 2072 6570  t to its PDF rep
-00018400: 7265 7365 6e74 6174 696f 6e20 616e 6420  resentation and 
-00018410: 7072 6f64 7563 6520 6465 6275 670a 2020  produce debug.  
-00018420: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
-00018430: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
-00018440: 3a0a 2020 2020 2020 2020 2020 2020 6773  :.            gs
-00018450: 645f 7265 6769 7374 7279 2028 4772 6170  d_registry (Grap
-00018460: 6869 6373 5374 6174 6544 6963 7452 6567  hicsStateDictReg
-00018470: 6973 7472 7929 3a20 7468 6520 6f77 6e65  istry): the owne
-00018480: 7227 7320 6772 6170 6869 6373 2073 7461  r's graphics sta
-00018490: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
-000184a0: 2020 2064 6963 7469 6f6e 6172 7920 7265     dictionary re
-000184b0: 6769 7374 7279 2e0a 2020 2020 2020 2020  gistry..        
-000184c0: 2020 2020 7374 796c 6520 2847 7261 7068      style (Graph
-000184d0: 6963 7353 7479 6c65 293a 2074 6865 2063  icsStyle): the c
-000184e0: 7572 7265 6e74 2072 6573 6f6c 7665 6420  urrent resolved 
-000184f0: 6772 6170 6869 6373 2073 7479 6c65 0a20  graphics style. 
-00018500: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-00018510: 6974 656d 3a20 7468 6520 7072 6576 696f  item: the previo
-00018520: 7573 2070 6174 6820 656c 656d 656e 742e  us path element.
-00018530: 0a20 2020 2020 2020 2020 2020 2069 6e69  .            ini
-00018540: 7469 616c 5f70 6f69 6e74 3a20 6c61 7374  tial_point: last
-00018550: 2070 6f73 6974 696f 6e20 7365 7420 6279   position set by
-00018560: 2061 2022 4d22 206f 7220 226d 2220 636f   a "M" or "m" co
-00018570: 6d6d 616e 640a 2020 2020 2020 2020 2020  mmand.          
-00018580: 2020 6465 6275 675f 7374 7265 616d 2028    debug_stream (
-00018590: 696f 2e54 6578 7449 4f29 3a20 7468 6520  io.TextIO): the 
-000185a0: 7374 7265 616d 2074 6f20 7768 6963 6820  stream to which 
-000185b0: 7468 6520 6465 6275 6720 6f75 7470 7574  the debug output
-000185c0: 2073 686f 756c 6420 6265 0a20 2020 2020   should be.     
-000185d0: 2020 2020 2020 2020 2020 2077 7269 7474             writt
-000185e0: 656e 2e20 5468 6973 2069 7320 6e6f 7420  en. This is not 
-000185f0: 6775 6172 616e 7465 6564 2074 6f20 6265  guaranteed to be
-00018600: 2073 6565 6b61 626c 6520 2865 2e67 2e20   seekable (e.g. 
-00018610: 6974 206d 6179 2062 6520 7374 646f 7574  it may be stdout
-00018620: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-00018630: 2020 2020 7374 6465 7272 292e 0a20 2020      stderr)..   
-00018640: 2020 2020 2020 2020 2070 6678 2028 7374           pfx (st
-00018650: 7229 3a20 7468 6520 6375 7272 656e 7420  r): the current 
-00018660: 6465 6275 6720 6f75 7470 7574 2070 7265  debug output pre
-00018670: 6669 7820 7374 7269 6e67 2028 6f6e 6c79  fix string (only
-00018680: 206e 6565 6465 6420 6966 2065 6d69 7474   needed if emitt
-00018690: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-000186a0: 2020 2020 6d6f 7265 2074 6861 6e20 6f6e      more than on
-000186b0: 6520 6c69 6e65 292e 0a0a 2020 2020 2020  e line)...      
-000186c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000186d0: 2020 2020 2020 2054 6865 2073 616d 6520         The same 
-000186e0: 7475 706c 6520 6173 2060 456c 6c69 7073  tuple as `Ellips
-000186f0: 652e 7265 6e64 6572 602e 0a20 2020 2020  e.render`..     
-00018700: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00018710: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-00018720: 3d75 6e75 7365 642d 6172 6775 6d65 6e74  =unused-argument
-00018730: 0a20 2020 2020 2020 2063 6f6d 706f 6e65  .        compone
-00018740: 6e74 7320 3d20 7365 6c66 2e5f 6465 636f  nts = self._deco
-00018750: 6d70 6f73 6528 290a 0a20 2020 2020 2020  mpose()..       
-00018760: 2064 6562 7567 5f73 7472 6561 6d2e 7772   debug_stream.wr
-00018770: 6974 6528 6622 7b73 656c 667d 2072 6573  ite(f"{self} res
-00018780: 6f6c 7665 6420 746f 3a5c 6e22 290a 2020  olved to:\n").  
-00018790: 2020 2020 2020 6966 206e 6f74 2063 6f6d        if not com
-000187a0: 706f 6e65 6e74 733a 0a20 2020 2020 2020  ponents:.       
-000187b0: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
-000187c0: 6d2e 7772 6974 6528 7066 7820 2b20 2220  m.write(pfx + " 
-000187d0: e294 94e2 9480 206e 6f74 6869 6e67 5c6e  ...... nothing\n
-000187e0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-000187f0: 6574 7572 6e20 2222 2c20 6c61 7374 5f69  eturn "", last_i
-00018800: 7465 6d0a 0a20 2020 2020 2020 2072 656e  tem..        ren
-00018810: 6465 725f 6c69 7374 203d 205b 5d0a 2020  der_list = [].  
-00018820: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
-00018830: 6e20 636f 6d70 6f6e 656e 7473 5b3a 2d31  n components[:-1
-00018840: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
-00018850: 656e 6465 7265 642c 206c 6173 745f 6974  endered, last_it
-00018860: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
-00018870: 7420 3d20 6974 656d 2e72 656e 6465 7228  t = item.render(
-00018880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018890: 2067 7364 5f72 6567 6973 7472 792c 2073   gsd_registry, s
-000188a0: 7479 6c65 2c20 6c61 7374 5f69 7465 6d2c  tyle, last_item,
-000188b0: 2069 6e69 7469 616c 5f70 6f69 6e74 0a20   initial_point. 
-000188c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000188d0: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
-000188e0: 7472 6561 6d2e 7772 6974 6528 7066 7820  tream.write(pfx 
-000188f0: 2b20 6622 20e2 949c e294 8020 7b69 7465  + f" ...... {ite
-00018900: 6d7d 5c6e 2229 0a20 2020 2020 2020 2020  m}\n").         
-00018910: 2020 2072 656e 6465 725f 6c69 7374 2e61     render_list.a
-00018920: 7070 656e 6428 7265 6e64 6572 6564 290a  ppend(rendered).
-00018930: 0a20 2020 2020 2020 2072 656e 6465 7265  .        rendere
-00018940: 642c 206c 6173 745f 6974 656d 2c20 696e  d, last_item, in
-00018950: 6974 6961 6c5f 706f 696e 7420 3d20 636f  itial_point = co
-00018960: 6d70 6f6e 656e 7473 5b2d 315d 2e72 656e  mponents[-1].ren
-00018970: 6465 7228 0a20 2020 2020 2020 2020 2020  der(.           
-00018980: 2067 7364 5f72 6567 6973 7472 792c 2073   gsd_registry, s
-00018990: 7479 6c65 2c20 6c61 7374 5f69 7465 6d2c  tyle, last_item,
-000189a0: 2069 6e69 7469 616c 5f70 6f69 6e74 0a20   initial_point. 
-000189b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000189c0: 2064 6562 7567 5f73 7472 6561 6d2e 7772   debug_stream.wr
-000189d0: 6974 6528 7066 7820 2b20 6622 20e2 9494  ite(pfx + f" ...
-000189e0: e294 8020 7b63 6f6d 706f 6e65 6e74 735b  ... {components[
-000189f0: 2d31 5d7d 5c6e 2229 0a20 2020 2020 2020  -1]}\n").       
-00018a00: 2072 656e 6465 725f 6c69 7374 2e61 7070   render_list.app
-00018a10: 656e 6428 7265 6e64 6572 6564 290a 0a20  end(rendered).. 
-00018a20: 2020 2020 2020 2072 6574 7572 6e20 2220         return " 
-00018a30: 222e 6a6f 696e 2872 656e 6465 725f 6c69  ".join(render_li
-00018a40: 7374 292c 204d 6f76 6528 7365 6c66 2e63  st), Move(self.c
-00018a50: 656e 7465 7229 2c20 696e 6974 6961 6c5f  enter), initial_
-00018a60: 706f 696e 740a 0a0a 636c 6173 7320 496d  point...class Im
-00018a70: 706c 6963 6974 436c 6f73 6528 4e61 6d65  plicitClose(Name
-00018a80: 6454 7570 6c65 293a 0a20 2020 2022 2222  dTuple):.    """
-00018a90: 0a20 2020 2041 2070 6174 6820 636c 6f73  .    A path clos
-00018aa0: 6520 656c 656d 656e 7420 7468 6174 2069  e element that i
-00018ab0: 7320 636f 6e64 6974 696f 6e61 6c6c 7920  s conditionally 
-00018ac0: 7265 6e64 6572 6564 2064 6570 656e 6469  rendered dependi
-00018ad0: 6e67 206f 6e20 7468 6520 7661 6c75 6520  ng on the value 
-00018ae0: 6f66 0a20 2020 2060 4772 6170 6869 6373  of.    `Graphics
-00018af0: 5374 796c 652e 6175 746f 5f63 6c6f 7365  Style.auto_close
-00018b00: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
-00018b10: 4066 6f72 6365 5f6e 6f64 6f63 756d 656e  @force_nodocumen
-00018b20: 740a 2020 2020 6465 6620 7265 6e64 6572  t.    def render
-00018b30: 2873 656c 662c 2067 7364 5f72 6567 6973  (self, gsd_regis
-00018b40: 7472 792c 2073 7479 6c65 2c20 6c61 7374  try, style, last
-00018b50: 5f69 7465 6d2c 2069 6e69 7469 616c 5f70  _item, initial_p
-00018b60: 6f69 6e74 293a 0a20 2020 2020 2020 2022  oint):.        "
-00018b70: 2222 0a20 2020 2020 2020 2052 656e 6465  "".        Rende
-00018b80: 7220 7468 6973 2070 6174 6820 656c 656d  r this path elem
-00018b90: 656e 7420 746f 2069 7473 2050 4446 2072  ent to its PDF r
-00018ba0: 6570 7265 7365 6e74 6174 696f 6e2e 0a0a  epresentation...
-00018bb0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00018bc0: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-00018bd0: 6769 7374 7279 2028 4772 6170 6869 6373  gistry (Graphics
-00018be0: 5374 6174 6544 6963 7452 6567 6973 7472  StateDictRegistr
-00018bf0: 7929 3a20 7468 6520 6f77 6e65 7227 7320  y): the owner's 
-00018c00: 6772 6170 6869 6373 2073 7461 7465 0a20  graphics state. 
-00018c10: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00018c20: 6963 7469 6f6e 6172 7920 7265 6769 7374  ictionary regist
-00018c30: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
-00018c40: 7374 796c 6520 2847 7261 7068 6963 7353  style (GraphicsS
-00018c50: 7479 6c65 293a 2074 6865 2063 7572 7265  tyle): the curre
-00018c60: 6e74 2072 6573 6f6c 7665 6420 6772 6170  nt resolved grap
-00018c70: 6869 6373 2073 7479 6c65 0a20 2020 2020  hics style.     
-00018c80: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
-00018c90: 3a20 7468 6520 7072 6576 696f 7573 2070  : the previous p
-00018ca0: 6174 6820 656c 656d 656e 742e 0a20 2020  ath element..   
-00018cb0: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
-00018cc0: 5f70 6f69 6e74 3a20 6c61 7374 2070 6f73  _point: last pos
-00018cd0: 6974 696f 6e20 7365 7420 6279 2061 2022  ition set by a "
-00018ce0: 4d22 206f 7220 226d 2220 636f 6d6d 616e  M" or "m" comman
-00018cf0: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
-00018d00: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00018d10: 6120 7475 706c 6520 6f66 2060 2873 7472  a tuple of `(str
-00018d20: 2c20 6e65 775f 6c61 7374 5f69 7465 6d29  , new_last_item)
-00018d30: 602c 2077 6865 7265 2060 6e65 775f 6c61  `, where `new_la
-00018d40: 7374 5f69 7465 6d60 2069 7320 7768 6174  st_item` is what
-00018d50: 6576 6572 2074 6865 206f 6c64 0a20 2020  ever the old.   
-00018d60: 2020 2020 2020 2020 206c 6173 745f 6974           last_it
-00018d70: 656d 2077 6173 2e0a 2020 2020 2020 2020  em was..        
-00018d80: 2222 220a 2020 2020 2020 2020 2320 7079  """.        # py
-00018d90: 6c69 6e74 3a20 6469 7361 626c 653d 756e  lint: disable=un
-00018da0: 7573 6564 2d61 7267 756d 656e 740a 2020  used-argument.  
-00018db0: 2020 2020 2020 6966 2073 7479 6c65 2e61        if style.a
-00018dc0: 7574 6f5f 636c 6f73 653a 0a20 2020 2020  uto_close:.     
-00018dd0: 2020 2020 2020 2072 6574 7572 6e20 2268         return "h
-00018de0: 222c 206c 6173 745f 6974 656d 2c20 696e  ", last_item, in
-00018df0: 6974 6961 6c5f 706f 696e 740a 0a20 2020  itial_point..   
-00018e00: 2020 2020 2072 6574 7572 6e20 2222 2c20       return "", 
-00018e10: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
-00018e20: 616c 5f70 6f69 6e74 0a0a 2020 2020 4066  al_point..    @f
-00018e30: 6f72 6365 5f6e 6f64 6f63 756d 656e 740a  orce_nodocument.
-00018e40: 2020 2020 6465 6620 7265 6e64 6572 5f64      def render_d
-00018e50: 6562 7567 280a 2020 2020 2020 2020 7365  ebug(.        se
-00018e60: 6c66 2c20 6773 645f 7265 6769 7374 7279  lf, gsd_registry
-00018e70: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
-00018e80: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
-00018e90: 742c 2064 6562 7567 5f73 7472 6561 6d2c  t, debug_stream,
-00018ea0: 2070 6678 0a20 2020 2029 3a0a 2020 2020   pfx.    ):.    
-00018eb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00018ec0: 5265 6e64 6572 2074 6869 7320 7061 7468  Render this path
-00018ed0: 2065 6c65 6d65 6e74 2074 6f20 6974 7320   element to its 
-00018ee0: 5044 4620 7265 7072 6573 656e 7461 7469  PDF representati
-00018ef0: 6f6e 2061 6e64 2070 726f 6475 6365 2064  on and produce d
-00018f00: 6562 7567 0a20 2020 2020 2020 2069 6e66  ebug.        inf
-00018f10: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
-00018f20: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00018f30: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
-00018f40: 7920 2847 7261 7068 6963 7353 7461 7465  y (GraphicsState
-00018f50: 4469 6374 5265 6769 7374 7279 293a 2074  DictRegistry): t
-00018f60: 6865 206f 776e 6572 2773 2067 7261 7068  he owner's graph
-00018f70: 6963 7320 7374 6174 650a 2020 2020 2020  ics state.      
-00018f80: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
-00018f90: 6e61 7279 2072 6567 6973 7472 792e 0a20  nary registry.. 
-00018fa0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
-00018fb0: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
-00018fc0: 3a20 7468 6520 6375 7272 656e 7420 7265  : the current re
-00018fd0: 736f 6c76 6564 2067 7261 7068 6963 7320  solved graphics 
-00018fe0: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
-00018ff0: 2020 6c61 7374 5f69 7465 6d3a 2074 6865    last_item: the
-00019000: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
-00019010: 6c65 6d65 6e74 2e0a 2020 2020 2020 2020  lement..        
-00019020: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
-00019030: 743a 206c 6173 7420 706f 7369 7469 6f6e  t: last position
-00019040: 2073 6574 2062 7920 6120 224d 2220 6f72   set by a "M" or
-00019050: 2022 6d22 2063 6f6d 6d61 6e64 0a20 2020   "m" command.   
-00019060: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
-00019070: 7472 6561 6d20 2869 6f2e 5465 7874 494f  tream (io.TextIO
-00019080: 293a 2074 6865 2073 7472 6561 6d20 746f  ): the stream to
-00019090: 2077 6869 6368 2074 6865 2064 6562 7567   which the debug
-000190a0: 206f 7574 7075 7420 7368 6f75 6c64 2062   output should b
-000190b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000190c0: 2020 7772 6974 7465 6e2e 2054 6869 7320    written. This 
-000190d0: 6973 206e 6f74 2067 7561 7261 6e74 6565  is not guarantee
-000190e0: 6420 746f 2062 6520 7365 656b 6162 6c65  d to be seekable
-000190f0: 2028 652e 672e 2069 7420 6d61 7920 6265   (e.g. it may be
-00019100: 2073 7464 6f75 7420 6f72 0a20 2020 2020   stdout or.     
-00019110: 2020 2020 2020 2020 2020 2073 7464 6572             stder
-00019120: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
-00019130: 7066 7820 2873 7472 293a 2074 6865 2063  pfx (str): the c
-00019140: 7572 7265 6e74 2064 6562 7567 206f 7574  urrent debug out
-00019150: 7075 7420 7072 6566 6978 2073 7472 696e  put prefix strin
-00019160: 6720 286f 6e6c 7920 6e65 6564 6564 2069  g (only needed i
-00019170: 6620 656d 6974 7469 6e67 0a20 2020 2020  f emitting.     
-00019180: 2020 2020 2020 2020 2020 206d 6f72 6520             more 
-00019190: 7468 616e 206f 6e65 206c 696e 6529 2e0a  than one line)..
-000191a0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000191b0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-000191c0: 6520 7361 6d65 2074 7570 6c65 2061 7320  e same tuple as 
-000191d0: 6049 6d70 6c69 6369 7443 6c6f 7365 2e72  `ImplicitClose.r
-000191e0: 656e 6465 7260 2e0a 2020 2020 2020 2020  ender`..        
-000191f0: 2222 220a 2020 2020 2020 2020 2320 7079  """.        # py
-00019200: 6c69 6e74 3a20 6469 7361 626c 653d 756e  lint: disable=un
-00019210: 7573 6564 2d61 7267 756d 656e 740a 2020  used-argument.  
-00019220: 2020 2020 2020 7265 6e64 6572 6564 2c20        rendered, 
-00019230: 7265 736f 6c76 6564 2c20 696e 6974 6961  resolved, initia
-00019240: 6c5f 706f 696e 7420 3d20 7365 6c66 2e72  l_point = self.r
-00019250: 656e 6465 7228 0a20 2020 2020 2020 2020  ender(.         
-00019260: 2020 2067 7364 5f72 6567 6973 7472 792c     gsd_registry,
-00019270: 2073 7479 6c65 2c20 6c61 7374 5f69 7465   style, last_ite
-00019280: 6d2c 2069 6e69 7469 616c 5f70 6f69 6e74  m, initial_point
-00019290: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000192a0: 2020 2064 6562 7567 5f73 7472 6561 6d2e     debug_stream.
-000192b0: 7772 6974 6528 6622 7b73 656c 667d 2072  write(f"{self} r
-000192c0: 6573 6f6c 7665 6420 746f 207b 7265 6e64  esolved to {rend
-000192d0: 6572 6564 7d5c 6e22 290a 0a20 2020 2020  ered}\n")..     
-000192e0: 2020 2072 6574 7572 6e20 7265 6e64 6572     return render
-000192f0: 6564 2c20 7265 736f 6c76 6564 2c20 696e  ed, resolved, in
-00019300: 6974 6961 6c5f 706f 696e 740a 0a0a 636c  itial_point...cl
-00019310: 6173 7320 436c 6f73 6528 4e61 6d65 6454  ass Close(NamedT
-00019320: 7570 6c65 293a 0a20 2020 2022 2222 0a20  uple):.    """. 
-00019330: 2020 2041 2070 6174 6820 636c 6f73 6520     A path close 
-00019340: 656c 656d 656e 742e 0a0a 2020 2020 496e  element...    In
-00019350: 7374 7275 6374 7320 7468 6520 7265 6e64  structs the rend
-00019360: 6572 6572 2074 6f20 6472 6177 2061 2073  erer to draw a s
-00019370: 7472 6169 6768 7420 6c69 6e65 2066 726f  traight line fro
-00019380: 6d20 7468 6520 656e 6420 6f66 2074 6865  m the end of the
-00019390: 206c 6173 7420 7061 7468 2065 6c65 6d65   last path eleme
-000193a0: 6e74 0a20 2020 2074 6f20 7468 6520 7374  nt.    to the st
-000193b0: 6172 7420 6f66 2074 6865 2063 7572 7265  art of the curre
-000193c0: 6e74 2070 6174 682e 0a0a 2020 2020 5365  nt path...    Se
-000193d0: 653a 2060 5061 696e 7465 6450 6174 682e  e: `PaintedPath.
-000193e0: 636c 6f73 6560 0a20 2020 2022 2222 0a0a  close`.    """..
-000193f0: 2020 2020 4066 6f72 6365 5f6e 6f64 6f63      @force_nodoc
-00019400: 756d 656e 740a 2020 2020 6465 6620 7265  ument.    def re
-00019410: 6e64 6572 2873 656c 662c 2067 7364 5f72  nder(self, gsd_r
-00019420: 6567 6973 7472 792c 2073 7479 6c65 2c20  egistry, style, 
-00019430: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
-00019440: 616c 5f70 6f69 6e74 293a 0a20 2020 2020  al_point):.     
-00019450: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00019460: 656e 6465 7220 7468 6973 2070 6174 6820  ender this path 
-00019470: 656c 656d 656e 7420 746f 2069 7473 2050  element to its P
-00019480: 4446 2072 6570 7265 7365 6e74 6174 696f  DF representatio
-00019490: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
-000194a0: 3a0a 2020 2020 2020 2020 2020 2020 6773  :.            gs
-000194b0: 645f 7265 6769 7374 7279 2028 4772 6170  d_registry (Grap
-000194c0: 6869 6373 5374 6174 6544 6963 7452 6567  hicsStateDictReg
-000194d0: 6973 7472 7929 3a20 7468 6520 6f77 6e65  istry): the owne
-000194e0: 7227 7320 6772 6170 6869 6373 2073 7461  r's graphics sta
-000194f0: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
-00019500: 2020 2064 6963 7469 6f6e 6172 7920 7265     dictionary re
-00019510: 6769 7374 7279 2e0a 2020 2020 2020 2020  gistry..        
-00019520: 2020 2020 7374 796c 6520 2847 7261 7068      style (Graph
-00019530: 6963 7353 7479 6c65 293a 2074 6865 2063  icsStyle): the c
-00019540: 7572 7265 6e74 2072 6573 6f6c 7665 6420  urrent resolved 
-00019550: 6772 6170 6869 6373 2073 7479 6c65 0a20  graphics style. 
-00019560: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-00019570: 6974 656d 3a20 7468 6520 7072 6576 696f  item: the previo
-00019580: 7573 2070 6174 6820 656c 656d 656e 742e  us path element.
-00019590: 0a20 2020 2020 2020 2020 2020 2069 6e69  .            ini
-000195a0: 7469 616c 5f70 6f69 6e74 3a20 6c61 7374  tial_point: last
-000195b0: 2070 6f73 6974 696f 6e20 7365 7420 6279   position set by
-000195c0: 2061 2022 4d22 206f 7220 226d 2220 636f   a "M" or "m" co
-000195d0: 6d6d 616e 640a 0a20 2020 2020 2020 2052  mmand..        R
-000195e0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000195f0: 2020 2020 6120 7475 706c 6520 6f66 2060      a tuple of `
-00019600: 2873 7472 2c20 6e65 775f 6c61 7374 5f69  (str, new_last_i
-00019610: 7465 6d29 602c 2077 6865 7265 2060 6e65  tem)`, where `ne
-00019620: 775f 6c61 7374 5f69 7465 6d60 2069 7320  w_last_item` is 
-00019630: 7768 6174 6576 6572 2074 6865 206f 6c64  whatever the old
-00019640: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
-00019650: 745f 6974 656d 2077 6173 2e0a 2020 2020  t_item was..    
-00019660: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00019670: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00019680: 653d 756e 7573 6564 2d61 7267 756d 656e  e=unused-argumen
-00019690: 740a 2020 2020 2020 2020 7265 7475 726e  t.        return
-000196a0: 2022 6822 2c20 4d6f 7665 2869 6e69 7469   "h", Move(initi
-000196b0: 616c 5f70 6f69 6e74 292c 2069 6e69 7469  al_point), initi
-000196c0: 616c 5f70 6f69 6e74 0a0a 2020 2020 4066  al_point..    @f
-000196d0: 6f72 6365 5f6e 6f64 6f63 756d 656e 740a  orce_nodocument.
-000196e0: 2020 2020 6465 6620 7265 6e64 6572 5f64      def render_d
-000196f0: 6562 7567 280a 2020 2020 2020 2020 7365  ebug(.        se
-00019700: 6c66 2c20 6773 645f 7265 6769 7374 7279  lf, gsd_registry
-00019710: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
-00019720: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
-00019730: 742c 2064 6562 7567 5f73 7472 6561 6d2c  t, debug_stream,
-00019740: 2070 6678 0a20 2020 2029 3a0a 2020 2020   pfx.    ):.    
-00019750: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00019760: 5265 6e64 6572 2074 6869 7320 7061 7468  Render this path
-00019770: 2065 6c65 6d65 6e74 2074 6f20 6974 7320   element to its 
-00019780: 5044 4620 7265 7072 6573 656e 7461 7469  PDF representati
-00019790: 6f6e 2061 6e64 2070 726f 6475 6365 2064  on and produce d
-000197a0: 6562 7567 0a20 2020 2020 2020 2069 6e66  ebug.        inf
-000197b0: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
-000197c0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-000197d0: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
-000197e0: 7920 2847 7261 7068 6963 7353 7461 7465  y (GraphicsState
-000197f0: 4469 6374 5265 6769 7374 7279 293a 2074  DictRegistry): t
-00019800: 6865 206f 776e 6572 2773 2067 7261 7068  he owner's graph
-00019810: 6963 7320 7374 6174 650a 2020 2020 2020  ics state.      
-00019820: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
-00019830: 6e61 7279 2072 6567 6973 7472 792e 0a20  nary registry.. 
-00019840: 2020 2020 2020 2020 2020 2073 7479 6c65             style
-00019850: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
-00019860: 3a20 7468 6520 6375 7272 656e 7420 7265  : the current re
-00019870: 736f 6c76 6564 2067 7261 7068 6963 7320  solved graphics 
-00019880: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
-00019890: 2020 6c61 7374 5f69 7465 6d3a 2074 6865    last_item: the
-000198a0: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
-000198b0: 6c65 6d65 6e74 2e0a 2020 2020 2020 2020  lement..        
-000198c0: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
-000198d0: 743a 206c 6173 7420 706f 7369 7469 6f6e  t: last position
-000198e0: 2073 6574 2062 7920 6120 224d 2220 6f72   set by a "M" or
-000198f0: 2022 6d22 2063 6f6d 6d61 6e64 0a20 2020   "m" command.   
-00019900: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
-00019910: 7472 6561 6d20 2869 6f2e 5465 7874 494f  tream (io.TextIO
-00019920: 293a 2074 6865 2073 7472 6561 6d20 746f  ): the stream to
-00019930: 2077 6869 6368 2074 6865 2064 6562 7567   which the debug
-00019940: 206f 7574 7075 7420 7368 6f75 6c64 2062   output should b
-00019950: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00019960: 2020 7772 6974 7465 6e2e 2054 6869 7320    written. This 
-00019970: 6973 206e 6f74 2067 7561 7261 6e74 6565  is not guarantee
-00019980: 6420 746f 2062 6520 7365 656b 6162 6c65  d to be seekable
-00019990: 2028 652e 672e 2069 7420 6d61 7920 6265   (e.g. it may be
-000199a0: 2073 7464 6f75 7420 6f72 0a20 2020 2020   stdout or.     
-000199b0: 2020 2020 2020 2020 2020 2073 7464 6572             stder
-000199c0: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
-000199d0: 7066 7820 2873 7472 293a 2074 6865 2063  pfx (str): the c
-000199e0: 7572 7265 6e74 2064 6562 7567 206f 7574  urrent debug out
-000199f0: 7075 7420 7072 6566 6978 2073 7472 696e  put prefix strin
-00019a00: 6720 286f 6e6c 7920 6e65 6564 6564 2069  g (only needed i
-00019a10: 6620 656d 6974 7469 6e67 0a20 2020 2020  f emitting.     
-00019a20: 2020 2020 2020 2020 2020 206d 6f72 6520             more 
-00019a30: 7468 616e 206f 6e65 206c 696e 6529 2e0a  than one line)..
-00019a40: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00019a50: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-00019a60: 6520 7361 6d65 2074 7570 6c65 2061 7320  e same tuple as 
-00019a70: 6043 6c6f 7365 2e72 656e 6465 7260 2e0a  `Close.render`..
-00019a80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00019a90: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-00019aa0: 7361 626c 653d 756e 7573 6564 2d61 7267  sable=unused-arg
-00019ab0: 756d 656e 740a 2020 2020 2020 2020 7265  ument.        re
-00019ac0: 6e64 6572 6564 2c20 7265 736f 6c76 6564  ndered, resolved
-00019ad0: 2c20 696e 6974 6961 6c5f 706f 696e 7420  , initial_point 
-00019ae0: 3d20 7365 6c66 2e72 656e 6465 7228 0a20  = self.render(. 
-00019af0: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
-00019b00: 6567 6973 7472 792c 2073 7479 6c65 2c20  egistry, style, 
-00019b10: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
-00019b20: 616c 5f70 6f69 6e74 0a20 2020 2020 2020  al_point.       
-00019b30: 2029 0a20 2020 2020 2020 2064 6562 7567   ).        debug
-00019b40: 5f73 7472 6561 6d2e 7772 6974 6528 7374  _stream.write(st
-00019b50: 7228 7365 6c66 2920 2b20 225c 6e22 290a  r(self) + "\n").
-00019b60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00019b70: 7265 6e64 6572 6564 2c20 7265 736f 6c76  rendered, resolv
-00019b80: 6564 2c20 696e 6974 6961 6c5f 706f 696e  ed, initial_poin
-00019b90: 740a 0a0a 636c 6173 7320 4472 6177 696e  t...class Drawin
-00019ba0: 6743 6f6e 7465 7874 3a0a 2020 2020 2222  gContext:.    ""
-00019bb0: 220a 2020 2020 4261 7365 2063 6f6e 7465  ".    Base conte
-00019bc0: 7874 2066 6f72 2061 2064 7261 7769 6e67  xt for a drawing
-00019bd0: 2069 6e20 6120 5044 460a 0a20 2020 2054   in a PDF..    T
-00019be0: 6869 7320 636f 6e74 6578 7420 6973 206e  his context is n
-00019bf0: 6f74 2073 7479 6c61 626c 6520 616e 6420  ot stylable and 
-00019c00: 6973 206d 6169 6e6c 7920 7265 7370 6f6e  is mainly respon
-00019c10: 7369 626c 6520 666f 7220 7472 616e 7366  sible for transf
-00019c20: 6f72 6d69 6e67 2070 6174 680a 2020 2020  orming path.    
-00019c30: 6472 6177 696e 6720 636f 6f72 6469 6e61  drawing coordina
-00019c40: 7465 7320 696e 746f 2075 7365 7220 636f  tes into user co
-00019c50: 6f72 6469 6e61 7465 7320 2869 2e65 2e20  ordinates (i.e. 
-00019c60: 6974 2065 6e73 7572 6573 2074 6861 7420  it ensures that 
-00019c70: 7468 6520 6f75 7470 7574 2064 7261 7769  the output drawi
-00019c80: 6e67 0a20 2020 2069 7320 636f 7272 6563  ng.    is correc
-00019c90: 746c 7920 7363 616c 6564 292e 0a20 2020  tly scaled)..   
-00019ca0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
-00019cb0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-00019cc0: 2020 2020 2020 7365 6c66 2e5f 7375 6269        self._subi
-00019cd0: 7465 6d73 203d 205b 5d0a 0a20 2020 2064  tems = []..    d
-00019ce0: 6566 2061 6464 5f69 7465 6d28 7365 6c66  ef add_item(self
-00019cf0: 2c20 6974 656d 2c20 5f63 6f70 793d 5472  , item, _copy=Tr
-00019d00: 7565 293a 0a20 2020 2020 2020 2022 2222  ue):.        """
-00019d10: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
-00019d20: 616e 2069 7465 6d20 746f 2074 6869 7320  an item to this 
-00019d30: 6472 6177 696e 6720 636f 6e74 6578 740a  drawing context.
-00019d40: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00019d50: 2020 2020 2020 2020 2020 2069 7465 6d20             item 
-00019d60: 2847 7261 7068 6963 7343 6f6e 7465 7874  (GraphicsContext
-00019d70: 2c20 5061 696e 7465 6450 6174 6829 3a20  , PaintedPath): 
-00019d80: 7468 6520 6974 656d 2074 6f20 6265 2061  the item to be a
-00019d90: 7070 656e 6465 642e 0a20 2020 2020 2020  ppended..       
-00019da0: 2020 2020 205f 636f 7079 2028 626f 6f6c       _copy (bool
-00019db0: 293a 2069 6620 7472 7565 2028 7468 6520  ): if true (the 
-00019dc0: 6465 6661 756c 7429 2c20 7468 6520 6974  default), the it
-00019dd0: 656d 2077 696c 6c20 6265 2063 6f70 6965  em will be copie
-00019de0: 6420 6265 666f 7265 2062 6569 6e67 0a20  d before being. 
-00019df0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00019e00: 7070 656e 6465 642e 2054 6869 7320 7072  ppended. This pr
-00019e10: 6576 656e 7473 206d 6f64 6966 6963 6174  events modificat
-00019e20: 696f 6e73 2074 6f20 6120 7265 6665 7265  ions to a refere
-00019e30: 6e63 6564 206f 626a 6563 7420 6672 6f6d  nced object from
-00019e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019e50: 2022 7265 7472 6f61 6374 6976 656c 7922   "retroactively"
-00019e60: 2061 6c74 6572 696e 6720 6974 7320 7374   altering its st
-00019e70: 796c 652f 7368 6170 6520 616e 6420 7368  yle/shape and sh
-00019e80: 6f75 6c64 2062 6520 6469 7361 626c 6564  ould be disabled
-00019e90: 2077 6974 680a 2020 2020 2020 2020 2020   with.          
-00019ea0: 2020 2020 2020 6361 7574 696f 6e2e 0a20        caution.. 
-00019eb0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00019ec0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00019ed0: 7461 6e63 6528 6974 656d 2c20 2847 7261  tance(item, (Gra
-00019ee0: 7068 6963 7343 6f6e 7465 7874 2c20 5061  phicsContext, Pa
-00019ef0: 696e 7465 6450 6174 6829 293a 0a20 2020  intedPath)):.   
-00019f00: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00019f10: 7970 6545 7272 6f72 2866 227b 6974 656d  ypeError(f"{item
-00019f20: 7d20 646f 6573 6e27 7420 6265 6c6f 6e67  } doesn't belong
-00019f30: 2069 6e20 6120 4472 6177 696e 6743 6f6e   in a DrawingCon
-00019f40: 7465 7874 2229 0a0a 2020 2020 2020 2020  text")..        
-00019f50: 6966 205f 636f 7079 3a0a 2020 2020 2020  if _copy:.      
-00019f60: 2020 2020 2020 6974 656d 203d 2063 6f70        item = cop
-00019f70: 792e 6465 6570 636f 7079 2869 7465 6d29  y.deepcopy(item)
-00019f80: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00019f90: 7375 6269 7465 6d73 2e61 7070 656e 6428  subitems.append(
-00019fa0: 6974 656d 290a 0a20 2020 2040 7374 6174  item)..    @stat
-00019fb0: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00019fc0: 205f 7365 7475 705f 7265 6e64 6572 5f70   _setup_render_p
-00019fd0: 7265 7265 7173 2873 7479 6c65 2c20 6669  rereqs(style, fi
-00019fe0: 7273 745f 706f 696e 742c 2073 6361 6c65  rst_point, scale
-00019ff0: 2c20 6865 6967 6874 293a 0a20 2020 2020  , height):.     
-0001a000: 2020 2073 7479 6c65 2e61 7574 6f5f 636c     style.auto_cl
-0001a010: 6f73 6520 3d20 5472 7565 0a20 2020 2020  ose = True.     
-0001a020: 2020 2073 7479 6c65 2e70 6169 6e74 5f72     style.paint_r
-0001a030: 756c 6520 3d20 5061 7468 5061 696e 7452  ule = PathPaintR
-0001a040: 756c 652e 4155 544f 0a20 2020 2020 2020  ule.AUTO.       
-0001a050: 2073 7479 6c65 2e69 6e74 6572 7365 6374   style.intersect
-0001a060: 696f 6e5f 7275 6c65 203d 2049 6e74 6572  ion_rule = Inter
-0001a070: 7365 6374 696f 6e52 756c 652e 4e4f 4e5a  sectionRule.NONZ
-0001a080: 4552 4f0a 0a20 2020 2020 2020 206c 6173  ERO..        las
-0001a090: 745f 6974 656d 203d 204d 6f76 6528 6669  t_item = Move(fi
-0001a0a0: 7273 745f 706f 696e 7429 0a20 2020 2020  rst_point).     
-0001a0b0: 2020 2073 6361 6c65 2c20 6c61 7374 5f69     scale, last_i
-0001a0c0: 7465 6d20 3d20 280a 2020 2020 2020 2020  tem = (.        
-0001a0d0: 2020 2020 5472 616e 7366 6f72 6d2e 7363      Transform.sc
-0001a0e0: 616c 696e 6728 783d 312c 2079 3d2d 3129  aling(x=1, y=-1)
-0001a0f0: 0a20 2020 2020 2020 2020 2020 202e 6162  .            .ab
-0001a100: 6f75 7428 783d 302c 2079 3d68 6569 6768  out(x=0, y=heigh
-0001a110: 7420 2f20 3229 0a20 2020 2020 2020 2020  t / 2).         
-0001a120: 2020 202e 7363 616c 6528 7363 616c 6529     .scale(scale)
-0001a130: 0a20 2020 2020 2020 2020 2020 202e 7265  .            .re
-0001a140: 6e64 6572 286c 6173 745f 6974 656d 290a  nder(last_item).
-0001a150: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0001a160: 2020 2072 656e 6465 725f 6c69 7374 203d     render_list =
-0001a170: 205b 2271 222c 2073 6361 6c65 5d0a 0a20   ["q", scale].. 
-0001a180: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0001a190: 6e64 6572 5f6c 6973 742c 2073 7479 6c65  nder_list, style
-0001a1a0: 2c20 6c61 7374 5f69 7465 6d0a 0a20 2020  , last_item..   
-0001a1b0: 2064 6566 2072 656e 6465 7228 7365 6c66   def render(self
-0001a1c0: 2c20 6773 645f 7265 6769 7374 7279 2c20  , gsd_registry, 
-0001a1d0: 6669 7273 745f 706f 696e 742c 2073 6361  first_point, sca
-0001a1e0: 6c65 2c20 6865 6967 6874 2c20 7374 6172  le, height, star
-0001a1f0: 7469 6e67 5f73 7479 6c65 293a 0a20 2020  ting_style):.   
-0001a200: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001a210: 2052 656e 6465 7220 7468 6520 6472 6177   Render the draw
-0001a220: 696e 6720 636f 6e74 6578 7420 746f 2050  ing context to P
-0001a230: 4446 2066 6f72 6d61 742e 0a0a 2020 2020  DF format...    
-0001a240: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0001a250: 2020 2020 2020 6773 645f 7265 6769 7374        gsd_regist
-0001a260: 7279 2028 4772 6170 6869 6373 5374 6174  ry (GraphicsStat
-0001a270: 6544 6963 7452 6567 6973 7472 7929 3a20  eDictRegistry): 
-0001a280: 7468 6520 7061 7265 6e74 2064 6f63 756d  the parent docum
-0001a290: 656e 7427 7320 6772 6170 6869 6373 0a20  ent's graphics. 
-0001a2a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a2b0: 7461 7465 2072 6567 6973 7472 792e 0a20  tate registry.. 
-0001a2c0: 2020 2020 2020 2020 2020 2066 6972 7374             first
-0001a2d0: 5f70 6f69 6e74 2028 506f 696e 7429 3a20  _point (Point): 
-0001a2e0: 7468 6520 7374 6172 7469 6e67 2070 6f69  the starting poi
-0001a2f0: 6e74 2074 6f20 7573 6520 6966 2074 6865  nt to use if the
-0001a300: 2066 6972 7374 2070 6174 6820 656c 656d   first path elem
-0001a310: 656e 7420 6973 0a20 2020 2020 2020 2020  ent is.         
-0001a320: 2020 2020 2020 2061 2072 656c 6174 6976         a relativ
-0001a330: 6520 656c 656d 656e 742e 0a20 2020 2020  e element..     
-0001a340: 2020 2020 2020 2073 6361 6c65 2028 4e75         scale (Nu
-0001a350: 6d62 6572 293a 2074 6865 2073 6361 6c65  mber): the scale
-0001a360: 2066 6163 746f 7220 746f 2063 6f6e 7665   factor to conve
-0001a370: 7274 2066 726f 6d20 5044 4620 7074 2075  rt from PDF pt u
-0001a380: 6e69 7473 2069 6e74 6f20 7468 650a 2020  nits into the.  
-0001a390: 2020 2020 2020 2020 2020 2020 2020 646f                do
-0001a3a0: 6375 6d65 6e74 2773 2073 656d 616e 7469  cument's semanti
-0001a3b0: 6320 756e 6974 7320 2865 2e67 2e20 6d6d  c units (e.g. mm
-0001a3c0: 206f 7220 696e 292e 0a20 2020 2020 2020   or in)..       
-0001a3d0: 2020 2020 2068 6569 6768 7420 284e 756d       height (Num
-0001a3e0: 6265 7229 3a20 7468 6520 7061 6765 2068  ber): the page h
-0001a3f0: 6569 6768 742e 2054 6869 7320 6973 2075  eight. This is u
-0001a400: 7365 6420 746f 2072 656d 6170 2074 6865  sed to remap the
-0001a410: 2063 6f6f 7264 696e 6174 6573 2074 6f0a   coordinates to.
-0001a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a430: 6265 2066 726f 6d20 7468 6520 746f 702d  be from the top-
-0001a440: 6c65 6674 2063 6f72 6e65 7220 6f66 2074  left corner of t
-0001a450: 6865 2070 6167 6520 286d 6174 6368 696e  he page (matchin
-0001a460: 6720 6670 6466 2773 2062 6568 6176 696f  g fpdf's behavio
-0001a470: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-0001a480: 2020 2069 6e73 7465 6164 206f 6620 7468     instead of th
-0001a490: 6520 5044 4620 6e61 7469 7665 2062 6568  e PDF native beh
-0001a4a0: 6176 696f 7220 6f66 2062 6f74 746f 6d2d  avior of bottom-
-0001a4b0: 6c65 6674 2e0a 2020 2020 2020 2020 2020  left..          
-0001a4c0: 2020 7374 6172 7469 6e67 5f73 7479 6c65    starting_style
-0001a4d0: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
-0001a4e0: 3a20 7468 6520 6261 7365 2073 7479 6c65  : the base style
-0001a4f0: 2066 6f72 2074 6869 7320 6472 6177 696e   for this drawin
-0001a500: 6720 636f 6e74 6578 742c 0a20 2020 2020  g context,.     
-0001a510: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
-0001a520: 6564 2066 726f 6d20 7468 6520 646f 6375  ed from the docu
-0001a530: 6d65 6e74 2773 2063 7572 7265 6e74 2073  ment's current s
-0001a540: 7479 6c65 2064 6566 6175 6c74 732e 0a0a  tyle defaults...
-0001a550: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0001a560: 0a20 2020 2020 2020 2020 2020 2041 2073  .            A s
-0001a570: 7472 696e 6720 636f 6d70 6f73 6564 206f  tring composed o
-0001a580: 6620 7468 6520 5044 4620 7265 7072 6573  f the PDF repres
-0001a590: 656e 7461 7469 6f6e 206f 6620 616c 6c20  entation of all 
-0001a5a0: 7468 6520 7061 7468 7320 616e 6420 6772  the paths and gr
-0001a5b0: 6f75 7073 2069 6e0a 2020 2020 2020 2020  oups in.        
-0001a5c0: 2020 2020 7468 6973 2063 6f6e 7465 7874      this context
-0001a5d0: 2028 616e 2065 6d70 7479 2073 7472 696e   (an empty strin
-0001a5e0: 6720 6973 2072 6574 7572 6e65 6420 6966  g is returned if
-0001a5f0: 2074 6865 7265 2061 7265 206e 6f20 7061   there are no pa
-0001a600: 7468 7320 6f72 2067 726f 7570 7329 0a20  ths or groups). 
-0001a610: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001a620: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-0001a630: 7375 6269 7465 6d73 3a0a 2020 2020 2020  subitems:.      
-0001a640: 2020 2020 2020 7265 7475 726e 2022 220a        return "".
-0001a650: 0a20 2020 2020 2020 2072 656e 6465 725f  .        render_
-0001a660: 6c69 7374 2c20 7374 796c 652c 206c 6173  list, style, las
-0001a670: 745f 6974 656d 203d 2073 656c 662e 5f73  t_item = self._s
-0001a680: 6574 7570 5f72 656e 6465 725f 7072 6572  etup_render_prer
-0001a690: 6571 7328 0a20 2020 2020 2020 2020 2020  eqs(.           
-0001a6a0: 2073 7461 7274 696e 675f 7374 796c 652c   starting_style,
-0001a6b0: 2066 6972 7374 5f70 6f69 6e74 2c20 7363   first_point, sc
-0001a6c0: 616c 652c 2068 6569 6768 740a 2020 2020  ale, height.    
-0001a6d0: 2020 2020 290a 0a20 2020 2020 2020 2066      )..        f
-0001a6e0: 6f72 2069 7465 6d20 696e 2073 656c 662e  or item in self.
-0001a6f0: 5f73 7562 6974 656d 733a 0a20 2020 2020  _subitems:.     
-0001a700: 2020 2020 2020 2072 656e 6465 7265 642c         rendered,
-0001a710: 206c 6173 745f 6974 656d 2c20 6669 7273   last_item, firs
-0001a720: 745f 706f 696e 7420 3d20 6974 656d 2e72  t_point = item.r
-0001a730: 656e 6465 7228 0a20 2020 2020 2020 2020  ender(.         
-0001a740: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
-0001a750: 7472 792c 2073 7479 6c65 2c20 6c61 7374  try, style, last
-0001a760: 5f69 7465 6d2c 2066 6972 7374 5f70 6f69  _item, first_poi
-0001a770: 6e74 0a20 2020 2020 2020 2020 2020 2029  nt.            )
-0001a780: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001a790: 7265 6e64 6572 6564 3a0a 2020 2020 2020  rendered:.      
-0001a7a0: 2020 2020 2020 2020 2020 7265 6e64 6572            render
-0001a7b0: 5f6c 6973 742e 6170 7065 6e64 2872 656e  _list.append(ren
-0001a7c0: 6465 7265 6429 0a0a 2020 2020 2020 2020  dered)..        
-0001a7d0: 2320 7468 6572 6520 7761 7320 6e6f 7468  # there was noth
-0001a7e0: 696e 6720 746f 2072 656e 6465 723a 2074  ing to render: t
-0001a7f0: 6865 206f 6e6c 7920 6974 656d 7320 6172  he only items ar
-0001a800: 6520 7468 6520 7374 6172 7420 6772 6f75  e the start grou
-0001a810: 7020 616e 6420 7363 616c 650a 2020 2020  p and scale.    
-0001a820: 2020 2020 2320 7472 616e 7366 6f72 6d2e      # transform.
-0001a830: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001a840: 7265 6e64 6572 5f6c 6973 7429 203d 3d20  render_list) == 
-0001a850: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
-0001a860: 6574 7572 6e20 2222 0a0a 2020 2020 2020  eturn ""..      
-0001a870: 2020 7374 796c 655f 6469 6374 5f6e 616d    style_dict_nam
-0001a880: 6520 3d20 6773 645f 7265 6769 7374 7279  e = gsd_registry
-0001a890: 2e72 6567 6973 7465 725f 7374 796c 6528  .register_style(
-0001a8a0: 7374 796c 6529 0a0a 2020 2020 2020 2020  style)..        
-0001a8b0: 6966 2073 7479 6c65 5f64 6963 745f 6e61  if style_dict_na
-0001a8c0: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-0001a8d0: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
-0001a8e0: 6572 5f6c 6973 742e 696e 7365 7274 2832  er_list.insert(2
-0001a8f0: 2c20 6622 7b72 656e 6465 725f 7064 665f  , f"{render_pdf_
-0001a900: 7072 696d 6974 6976 6528 7374 796c 655f  primitive(style_
-0001a910: 6469 6374 5f6e 616d 6529 7d20 6773 2229  dict_name)} gs")
-0001a920: 0a20 2020 2020 2020 2020 2020 2072 656e  .            ren
-0001a930: 6465 725f 6c69 7374 2e69 6e73 6572 7428  der_list.insert(
-0001a940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a950: 2033 2c0a 2020 2020 2020 2020 2020 2020   3,.            
-0001a960: 2020 2020 7265 6e64 6572 5f70 6466 5f70      render_pdf_p
-0001a970: 7269 6d69 7469 7665 2873 7479 6c65 2e73  rimitive(style.s
-0001a980: 7472 6f6b 655f 6461 7368 5f70 6174 7465  troke_dash_patte
-0001a990: 726e 290a 2020 2020 2020 2020 2020 2020  rn).            
-0001a9a0: 2020 2020 2b20 6622 207b 6e75 6d62 6572      + f" {number
-0001a9b0: 5f74 6f5f 7374 7228 7374 796c 652e 7374  _to_str(style.st
-0001a9c0: 726f 6b65 5f64 6173 685f 7068 6173 6529  roke_dash_phase)
-0001a9d0: 7d20 6422 2c0a 2020 2020 2020 2020 2020  } d",.          
-0001a9e0: 2020 290a 0a20 2020 2020 2020 2072 656e    )..        ren
-0001a9f0: 6465 725f 6c69 7374 2e61 7070 656e 6428  der_list.append(
-0001aa00: 2251 2229 0a0a 2020 2020 2020 2020 7265  "Q")..        re
-0001aa10: 7475 726e 2022 2022 2e6a 6f69 6e28 7265  turn " ".join(re
-0001aa20: 6e64 6572 5f6c 6973 7429 0a0a 2020 2020  nder_list)..    
-0001aa30: 6465 6620 7265 6e64 6572 5f64 6562 7567  def render_debug
-0001aa40: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0001aa50: 6773 645f 7265 6769 7374 7279 2c20 6669  gsd_registry, fi
-0001aa60: 7273 745f 706f 696e 742c 2073 6361 6c65  rst_point, scale
-0001aa70: 2c20 6865 6967 6874 2c20 7374 6172 7469  , height, starti
-0001aa80: 6e67 5f73 7479 6c65 2c20 6465 6275 675f  ng_style, debug_
-0001aa90: 7374 7265 616d 0a20 2020 2029 3a0a 2020  stream.    ):.  
-0001aaa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001aab0: 2020 5265 6e64 6572 2074 6865 2064 7261    Render the dra
-0001aac0: 7769 6e67 2063 6f6e 7465 7874 2074 6f20  wing context to 
-0001aad0: 5044 4620 666f 726d 6174 2e0a 0a20 2020  PDF format...   
-0001aae0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0001aaf0: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
-0001ab00: 7472 7920 2847 7261 7068 6963 7353 7461  try (GraphicsSta
-0001ab10: 7465 4469 6374 5265 6769 7374 7279 293a  teDictRegistry):
-0001ab20: 2074 6865 2070 6172 656e 7420 646f 6375   the parent docu
-0001ab30: 6d65 6e74 2773 2067 7261 7068 6963 730a  ment's graphics.
-0001ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab50: 7374 6174 6520 7265 6769 7374 7279 2e0a  state registry..
-0001ab60: 2020 2020 2020 2020 2020 2020 6669 7273              firs
-0001ab70: 745f 706f 696e 7420 2850 6f69 6e74 293a  t_point (Point):
-0001ab80: 2074 6865 2073 7461 7274 696e 6720 706f   the starting po
-0001ab90: 696e 7420 746f 2075 7365 2069 6620 7468  int to use if th
-0001aba0: 6520 6669 7273 7420 7061 7468 2065 6c65  e first path ele
-0001abb0: 6d65 6e74 2069 730a 2020 2020 2020 2020  ment is.        
-0001abc0: 2020 2020 2020 2020 6120 7265 6c61 7469          a relati
-0001abd0: 7665 2065 6c65 6d65 6e74 2e0a 2020 2020  ve element..    
-0001abe0: 2020 2020 2020 2020 7363 616c 6520 284e          scale (N
-0001abf0: 756d 6265 7229 3a20 7468 6520 7363 616c  umber): the scal
-0001ac00: 6520 6661 6374 6f72 2074 6f20 636f 6e76  e factor to conv
-0001ac10: 6572 7420 6672 6f6d 2050 4446 2070 7420  ert from PDF pt 
-0001ac20: 756e 6974 7320 696e 746f 2074 6865 0a20  units into the. 
-0001ac30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001ac40: 6f63 756d 656e 7427 7320 7365 6d61 6e74  ocument's semant
-0001ac50: 6963 2075 6e69 7473 2028 652e 672e 206d  ic units (e.g. m
-0001ac60: 6d20 6f72 2069 6e29 2e0a 2020 2020 2020  m or in)..      
-0001ac70: 2020 2020 2020 6865 6967 6874 2028 4e75        height (Nu
-0001ac80: 6d62 6572 293a 2074 6865 2070 6167 6520  mber): the page 
-0001ac90: 6865 6967 6874 2e20 5468 6973 2069 7320  height. This is 
-0001aca0: 7573 6564 2074 6f20 7265 6d61 7020 7468  used to remap th
-0001acb0: 6520 636f 6f72 6469 6e61 7465 7320 746f  e coordinates to
-0001acc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001acd0: 2062 6520 6672 6f6d 2074 6865 2074 6f70   be from the top
-0001ace0: 2d6c 6566 7420 636f 726e 6572 206f 6620  -left corner of 
-0001acf0: 7468 6520 7061 6765 2028 6d61 7463 6869  the page (matchi
-0001ad00: 6e67 2066 7064 6627 7320 6265 6861 7669  ng fpdf's behavi
-0001ad10: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
-0001ad20: 2020 2020 696e 7374 6561 6420 6f66 2074      instead of t
-0001ad30: 6865 2050 4446 206e 6174 6976 6520 6265  he PDF native be
-0001ad40: 6861 7669 6f72 206f 6620 626f 7474 6f6d  havior of bottom
-0001ad50: 2d6c 6566 742e 0a20 2020 2020 2020 2020  -left..         
-0001ad60: 2020 2073 7461 7274 696e 675f 7374 796c     starting_styl
-0001ad70: 6520 2847 7261 7068 6963 7353 7479 6c65  e (GraphicsStyle
-0001ad80: 293a 2074 6865 2062 6173 6520 7374 796c  ): the base styl
-0001ad90: 6520 666f 7220 7468 6973 2064 7261 7769  e for this drawi
-0001ada0: 6e67 2063 6f6e 7465 7874 2c0a 2020 2020  ng context,.    
-0001adb0: 2020 2020 2020 2020 2020 2020 6465 7269              deri
-0001adc0: 7665 6420 6672 6f6d 2074 6865 2064 6f63  ved from the doc
-0001add0: 756d 656e 7427 7320 6375 7272 656e 7420  ument's current 
-0001ade0: 7374 796c 6520 6465 6661 756c 7473 2e0a  style defaults..
-0001adf0: 2020 2020 2020 2020 2020 2020 6465 6275              debu
-0001ae00: 675f 7374 7265 616d 2028 5465 7874 494f  g_stream (TextIO
-0001ae10: 293a 2061 2074 6578 7420 7374 7265 616d  ): a text stream
-0001ae20: 2074 6f20 7768 6963 6820 6120 6465 6275   to which a debu
-0001ae30: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
-0001ae40: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-0001ae50: 2020 2020 2020 2020 6472 6177 696e 6720          drawing 
-0001ae60: 7374 7275 6374 7572 6520 7769 6c6c 2062  structure will b
-0001ae70: 6520 7772 6974 7465 6e2e 0a0a 2020 2020  e written...    
-0001ae80: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0001ae90: 2020 2020 2020 2020 2041 2073 7472 696e           A strin
-0001aea0: 6720 636f 6d70 6f73 6564 206f 6620 7468  g composed of th
-0001aeb0: 6520 5044 4620 7265 7072 6573 656e 7461  e PDF representa
-0001aec0: 7469 6f6e 206f 6620 616c 6c20 7468 6520  tion of all the 
-0001aed0: 7061 7468 7320 616e 6420 6772 6f75 7073  paths and groups
-0001aee0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
-0001aef0: 7468 6973 2063 6f6e 7465 7874 2028 616e  this context (an
-0001af00: 2065 6d70 7479 2073 7472 696e 6720 6973   empty string is
-0001af10: 2072 6574 7572 6e65 6420 6966 2074 6865   returned if the
-0001af20: 7265 2061 7265 206e 6f20 7061 7468 7320  re are no paths 
-0001af30: 6f72 2067 726f 7570 7329 0a20 2020 2020  or groups).     
-0001af40: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0001af50: 656e 6465 725f 6c69 7374 2c20 7374 796c  ender_list, styl
-0001af60: 652c 206c 6173 745f 6974 656d 203d 2073  e, last_item = s
-0001af70: 656c 662e 5f73 6574 7570 5f72 656e 6465  elf._setup_rende
-0001af80: 725f 7072 6572 6571 7328 0a20 2020 2020  r_prereqs(.     
-0001af90: 2020 2020 2020 2073 7461 7274 696e 675f         starting_
-0001afa0: 7374 796c 652c 2066 6972 7374 5f70 6f69  style, first_poi
-0001afb0: 6e74 2c20 7363 616c 652c 2068 6569 6768  nt, scale, heigh
-0001afc0: 740a 2020 2020 2020 2020 290a 0a20 2020  t.        )..   
-0001afd0: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
-0001afe0: 6d2e 7772 6974 6528 2252 4f4f 545c 6e22  m.write("ROOT\n"
-0001aff0: 290a 2020 2020 2020 2020 666f 7220 6368  ).        for ch
-0001b000: 696c 6420 696e 2073 656c 662e 5f73 7562  ild in self._sub
-0001b010: 6974 656d 735b 3a2d 315d 3a0a 2020 2020  items[:-1]:.    
-0001b020: 2020 2020 2020 2020 6465 6275 675f 7374          debug_st
-0001b030: 7265 616d 2e77 7269 7465 2822 20e2 949c  ream.write(" ...
-0001b040: e294 8020 2229 0a20 2020 2020 2020 2020  ... ").         
-0001b050: 2020 2072 656e 6465 7265 642c 206c 6173     rendered, las
-0001b060: 745f 6974 656d 203d 2063 6869 6c64 2e72  t_item = child.r
-0001b070: 656e 6465 725f 6465 6275 6728 0a20 2020  ender_debug(.   
-0001b080: 2020 2020 2020 2020 2020 2020 2067 7364               gsd
-0001b090: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
-0001b0a0: 2c20 6c61 7374 5f69 7465 6d2c 2064 6562  , last_item, deb
-0001b0b0: 7567 5f73 7472 6561 6d2c 2022 20e2 9482  ug_stream, " ...
-0001b0c0: 2020 220a 2020 2020 2020 2020 2020 2020    ".            
-0001b0d0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001b0e0: 2072 656e 6465 7265 643a 0a20 2020 2020   rendered:.     
-0001b0f0: 2020 2020 2020 2020 2020 2072 656e 6465             rende
-0001b100: 725f 6c69 7374 2e61 7070 656e 6428 7265  r_list.append(re
-0001b110: 6e64 6572 6564 290a 0a20 2020 2020 2020  ndered)..       
-0001b120: 2069 6620 7365 6c66 2e5f 7375 6269 7465   if self._subite
-0001b130: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-0001b140: 6465 6275 675f 7374 7265 616d 2e77 7269  debug_stream.wri
-0001b150: 7465 2822 20e2 9494 e294 8020 2229 0a20  te(" ...... "). 
-0001b160: 2020 2020 2020 2020 2020 2072 656e 6465             rende
-0001b170: 7265 642c 206c 6173 745f 6974 656d 2c20  red, last_item, 
-0001b180: 6669 7273 745f 706f 696e 7420 3d20 7365  first_point = se
-0001b190: 6c66 2e5f 7375 6269 7465 6d73 5b2d 315d  lf._subitems[-1]
-0001b1a0: 2e72 656e 6465 725f 6465 6275 6728 0a20  .render_debug(. 
-0001b1b0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0001b1c0: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
-0001b1d0: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2066  le, last_item, f
-0001b1e0: 6972 7374 5f70 6f69 6e74 2c20 6465 6275  irst_point, debu
-0001b1f0: 675f 7374 7265 616d 2c20 2220 2020 2022  g_stream, "    "
-0001b200: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0001b210: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-0001b220: 6e64 6572 6564 3a0a 2020 2020 2020 2020  ndered:.        
-0001b230: 2020 2020 2020 2020 7265 6e64 6572 5f6c          render_l
-0001b240: 6973 742e 6170 7065 6e64 2872 656e 6465  ist.append(rende
-0001b250: 7265 6429 0a0a 2020 2020 2020 2020 2020  red)..          
-0001b260: 2020 2320 7468 6572 6520 7761 7320 6e6f    # there was no
-0001b270: 7468 696e 6720 746f 2072 656e 6465 723a  thing to render:
-0001b280: 2074 6865 206f 6e6c 7920 6974 656d 7320   the only items 
-0001b290: 6172 6520 7468 6520 7374 6172 7420 6772  are the start gr
-0001b2a0: 6f75 7020 616e 6420 7363 616c 650a 2020  oup and scale.  
-0001b2b0: 2020 2020 2020 2020 2020 2320 7472 616e            # tran
-0001b2c0: 7366 6f72 6d2e 0a20 2020 2020 2020 2020  sform..         
-0001b2d0: 2020 2069 6620 6c65 6e28 7265 6e64 6572     if len(render
-0001b2e0: 5f6c 6973 7429 203d 3d20 323a 0a20 2020  _list) == 2:.   
-0001b2f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001b300: 7572 6e20 2222 0a0a 2020 2020 2020 2020  urn ""..        
-0001b310: 2020 2020 7374 796c 655f 6469 6374 5f6e      style_dict_n
-0001b320: 616d 6520 3d20 6773 645f 7265 6769 7374  ame = gsd_regist
-0001b330: 7279 2e72 6567 6973 7465 725f 7374 796c  ry.register_styl
-0001b340: 6528 7374 796c 6529 0a0a 2020 2020 2020  e(style)..      
-0001b350: 2020 2020 2020 6966 2073 7479 6c65 5f64        if style_d
-0001b360: 6963 745f 6e61 6d65 2069 7320 6e6f 7420  ict_name is not 
-0001b370: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001b380: 2020 2020 2020 7265 6e64 6572 5f6c 6973        render_lis
-0001b390: 742e 696e 7365 7274 2832 2c20 6622 7b72  t.insert(2, f"{r
-0001b3a0: 656e 6465 725f 7064 665f 7072 696d 6974  ender_pdf_primit
-0001b3b0: 6976 6528 7374 796c 655f 6469 6374 5f6e  ive(style_dict_n
-0001b3c0: 616d 6529 7d20 6773 2229 0a20 2020 2020  ame)} gs").     
-0001b3d0: 2020 2020 2020 2020 2020 2072 656e 6465             rende
-0001b3e0: 725f 6c69 7374 2e69 6e73 6572 7428 0a20  r_list.insert(. 
-0001b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b400: 2020 2033 2c0a 2020 2020 2020 2020 2020     3,.          
-0001b410: 2020 2020 2020 2020 2020 7265 6e64 6572            render
-0001b420: 5f70 6466 5f70 7269 6d69 7469 7665 2873  _pdf_primitive(s
-0001b430: 7479 6c65 2e73 7472 6f6b 655f 6461 7368  tyle.stroke_dash
-0001b440: 5f70 6174 7465 726e 290a 2020 2020 2020  _pattern).      
-0001b450: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001b460: 6622 207b 6e75 6d62 6572 5f74 6f5f 7374  f" {number_to_st
-0001b470: 7228 7374 796c 652e 7374 726f 6b65 5f64  r(style.stroke_d
-0001b480: 6173 685f 7068 6173 6529 7d20 6422 2c0a  ash_phase)} d",.
-0001b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4a0: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0001b4b0: 656e 6465 725f 6c69 7374 2e61 7070 656e  ender_list.appen
-0001b4c0: 6428 2251 2229 0a0a 2020 2020 2020 2020  d("Q")..        
-0001b4d0: 2020 2020 7265 7475 726e 2022 2022 2e6a      return " ".j
-0001b4e0: 6f69 6e28 7265 6e64 6572 5f6c 6973 7429  oin(render_list)
-0001b4f0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001b500: 2022 220a 0a0a 636c 6173 7320 5061 696e   ""...class Pain
-0001b510: 7465 6450 6174 683a 0a20 2020 2022 2222  tedPath:.    """
-0001b520: 0a20 2020 2041 2070 6174 6820 746f 2062  .    A path to b
-0001b530: 6520 6472 6177 6e20 6279 2074 6865 2050  e drawn by the P
-0001b540: 4446 2072 656e 6465 7265 722e 0a0a 2020  DF renderer...  
-0001b550: 2020 4120 7061 696e 7465 6420 7061 7468    A painted path
-0001b560: 2069 7320 6465 6669 6e65 6420 6279 2061   is defined by a
-0001b570: 2073 7479 6c65 2061 6e64 2061 6e20 6172   style and an ar
-0001b580: 6269 7472 6172 7920 7365 7175 656e 6365  bitrary sequence
-0001b590: 206f 6620 7061 7468 2065 6c65 6d65 6e74   of path element
-0001b5a0: 732c 0a20 2020 2077 6869 6368 2069 6e63  s,.    which inc
-0001b5b0: 6c75 6465 2074 6865 2070 7269 6d69 7469  lude the primiti
-0001b5c0: 7665 2070 6174 6820 656c 656d 656e 7473  ve path elements
-0001b5d0: 2028 604d 6f76 6560 2c20 604c 696e 6560   (`Move`, `Line`
-0001b5e0: 2c20 6042 657a 6965 7243 7572 7665 602c  , `BezierCurve`,
-0001b5f0: 202e 2e2e 2920 6173 0a20 2020 2077 656c   ...) as.    wel
-0001b600: 6c20 6173 2061 7262 6974 7261 7269 6c79  l as arbitrarily
-0001b610: 206e 6573 7465 6420 6047 7261 7068 6963   nested `Graphic
-0001b620: 7343 6f6e 7465 7874 6020 636f 6e74 6169  sContext` contai
-0001b630: 6e69 6e67 2074 6865 6972 206f 776e 2073  ning their own s
-0001b640: 6571 7565 6e63 6520 6f66 0a20 2020 2070  equence of.    p
-0001b650: 7269 6d69 7469 7665 2070 6174 6820 656c  rimitive path el
-0001b660: 656d 656e 7473 2061 6e64 2060 4772 6170  ements and `Grap
-0001b670: 6869 6373 436f 6e74 6578 7460 2e0a 2020  hicsContext`..  
-0001b680: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-0001b690: 5f69 6e69 745f 5f28 7365 6c66 2c20 783d  _init__(self, x=
-0001b6a0: 302c 2079 3d30 293a 0a20 2020 2020 2020  0, y=0):.       
-0001b6b0: 2073 656c 662e 5f72 6f6f 745f 6772 6170   self._root_grap
-0001b6c0: 6869 6373 5f63 6f6e 7465 7874 203d 2047  hics_context = G
-0001b6d0: 7261 7068 6963 7343 6f6e 7465 7874 2829  raphicsContext()
-0001b6e0: 0a20 2020 2020 2020 2073 656c 662e 5f67  .        self._g
-0001b6f0: 7261 7068 6963 735f 636f 6e74 6578 7420  raphics_context 
-0001b700: 3d20 7365 6c66 2e5f 726f 6f74 5f67 7261  = self._root_gra
-0001b710: 7068 6963 735f 636f 6e74 6578 740a 0a20  phics_context.. 
-0001b720: 2020 2020 2020 2073 656c 662e 5f63 6c6f         self._clo
-0001b730: 7365 6420 3d20 5472 7565 0a20 2020 2020  sed = True.     
-0001b740: 2020 2073 656c 662e 5f63 6c6f 7365 5f63     self._close_c
-0001b750: 6f6e 7465 7874 203d 2073 656c 662e 5f67  ontext = self._g
-0001b760: 7261 7068 6963 735f 636f 6e74 6578 740a  raphics_context.
-0001b770: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-0001b780: 7461 7274 6572 5f6d 6f76 6520 3d20 4d6f  tarter_move = Mo
-0001b790: 7665 2850 6f69 6e74 2878 2c20 7929 290a  ve(Point(x, y)).
-0001b7a0: 0a20 2020 2064 6566 205f 5f64 6565 7063  .    def __deepc
-0001b7b0: 6f70 795f 5f28 7365 6c66 2c20 6d65 6d6f  opy__(self, memo
-0001b7c0: 293a 0a20 2020 2020 2020 2023 2074 6865  ):.        # the
-0001b7d0: 7265 2773 206e 6f20 7265 616c 2077 6179  re's no real way
-0001b7e0: 2074 6f20 7265 636f 7665 7220 7468 6520   to recover the 
-0001b7f0: 6d61 7463 6869 6e67 2063 7572 7265 6e74  matching current
-0001b800: 205f 6772 6170 6869 6373 5f63 6f6e 7465   _graphics_conte
-0001b810: 7874 2061 6674 6572 0a20 2020 2020 2020  xt after.       
-0001b820: 2023 2063 6f70 7969 6e67 2074 6865 2072   # copying the r
-0001b830: 6f6f 7420 636f 6e74 6578 742c 2062 7574  oot context, but
-0001b840: 2074 6861 7427 7320 6f6b 2062 6563 6175   that's ok becau
-0001b850: 7365 2077 6520 6361 6e20 6a75 7374 2064  se we can just d
-0001b860: 6973 616c 6c6f 7720 636f 7079 696e 670a  isallow copying.
-0001b870: 2020 2020 2020 2020 2320 6f66 2070 6174          # of pat
-0001b880: 6873 2075 6e64 6572 206d 6f64 6966 6963  hs under modific
-0001b890: 6174 696f 6e20 6173 2074 6861 7420 6973  ation as that is
-0001b8a0: 2061 6c6d 6f73 7420 6365 7274 6169 6e6c   almost certainl
-0001b8b0: 7920 7772 6f6e 6720 7573 6167 652e 0a20  y wrong usage.. 
-0001b8c0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0001b8d0: 6772 6170 6869 6373 5f63 6f6e 7465 7874  graphics_context
-0001b8e0: 2069 7320 6e6f 7420 7365 6c66 2e5f 726f   is not self._ro
-0001b8f0: 6f74 5f67 7261 7068 6963 735f 636f 6e74  ot_graphics_cont
-0001b900: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-0001b910: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
-0001b920: 726f 7228 6622 6361 6e6e 6f74 2063 6f70  ror(f"cannot cop
-0001b930: 7920 7061 7468 207b 7365 6c66 7d20 7768  y path {self} wh
-0001b940: 696c 6520 6974 2069 7320 6265 696e 6720  ile it is being 
-0001b950: 6d6f 6469 6669 6564 2229 0a0a 2020 2020  modified")..    
-0001b960: 2020 2020 636f 7069 6564 203d 2073 656c      copied = sel
-0001b970: 662e 5f5f 636c 6173 735f 5f28 290a 2020  f.__class__().  
-0001b980: 2020 2020 2020 636f 7069 6564 2e5f 726f        copied._ro
-0001b990: 6f74 5f67 7261 7068 6963 735f 636f 6e74  ot_graphics_cont
-0001b9a0: 6578 7420 3d20 636f 7079 2e64 6565 7063  ext = copy.deepc
-0001b9b0: 6f70 7928 7365 6c66 2e5f 726f 6f74 5f67  opy(self._root_g
-0001b9c0: 7261 7068 6963 735f 636f 6e74 6578 742c  raphics_context,
-0001b9d0: 206d 656d 6f29 0a20 2020 2020 2020 2063   memo).        c
-0001b9e0: 6f70 6965 642e 5f67 7261 7068 6963 735f  opied._graphics_
-0001b9f0: 636f 6e74 6578 7420 3d20 636f 7069 6564  context = copied
-0001ba00: 2e5f 726f 6f74 5f67 7261 7068 6963 735f  ._root_graphics_
-0001ba10: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
-0001ba20: 636f 7069 6564 2e5f 636c 6f73 6564 203d  copied._closed =
-0001ba30: 2073 656c 662e 5f63 6c6f 7365 640a 2020   self._closed.  
-0001ba40: 2020 2020 2020 636f 7069 6564 2e5f 636c        copied._cl
-0001ba50: 6f73 655f 636f 6e74 6578 7420 3d20 636f  ose_context = co
-0001ba60: 7069 6564 2e5f 6772 6170 6869 6373 5f63  pied._graphics_c
-0001ba70: 6f6e 7465 7874 0a0a 2020 2020 2020 2020  ontext..        
-0001ba80: 7265 7475 726e 2063 6f70 6965 640a 0a20  return copied.. 
-0001ba90: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0001baa0: 2064 6566 2073 7479 6c65 2873 656c 6629   def style(self)
-0001bab0: 3a0a 2020 2020 2020 2020 2222 2254 6865  :.        """The
-0001bac0: 2060 4772 6170 6869 6373 5374 796c 6560   `GraphicsStyle`
-0001bad0: 2061 7070 6c69 6564 2074 6f20 616c 6c20   applied to all 
-0001bae0: 656c 656d 656e 7473 206f 6620 7468 6973  elements of this
-0001baf0: 2070 6174 682e 2222 220a 2020 2020 2020   path.""".      
-0001bb00: 2020 7265 7475 726e 2073 656c 662e 5f72    return self._r
-0001bb10: 6f6f 745f 6772 6170 6869 6373 5f63 6f6e  oot_graphics_con
-0001bb20: 7465 7874 2e73 7479 6c65 0a0a 2020 2020  text.style..    
-0001bb30: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0001bb40: 6620 7472 616e 7366 6f72 6d28 7365 6c66  f transform(self
-0001bb50: 293a 0a20 2020 2020 2020 2022 2222 5468  ):.        """Th
-0001bb60: 6520 6054 7261 6e73 666f 726d 6020 7468  e `Transform` th
-0001bb70: 6174 2061 7070 6c69 6573 2074 6f20 616c  at applies to al
-0001bb80: 6c20 6f66 2074 6865 2065 6c65 6d65 6e74  l of the element
-0001bb90: 7320 6f66 2074 6869 7320 7061 7468 2e22  s of this path."
-0001bba0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0001bbb0: 6e20 7365 6c66 2e5f 726f 6f74 5f67 7261  n self._root_gra
-0001bbc0: 7068 6963 735f 636f 6e74 6578 742e 7472  phics_context.tr
-0001bbd0: 616e 7366 6f72 6d0a 0a20 2020 2040 7472  ansform..    @tr
-0001bbe0: 616e 7366 6f72 6d2e 7365 7474 6572 0a20  ansform.setter. 
-0001bbf0: 2020 2064 6566 2074 7261 6e73 666f 726d     def transform
-0001bc00: 2873 656c 662c 2074 6629 3a0a 2020 2020  (self, tf):.    
-0001bc10: 2020 2020 7365 6c66 2e5f 726f 6f74 5f67      self._root_g
-0001bc20: 7261 7068 6963 735f 636f 6e74 6578 742e  raphics_context.
-0001bc30: 7472 616e 7366 6f72 6d20 3d20 7466 0a0a  transform = tf..
-0001bc40: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0001bc50: 2020 6465 6620 6175 746f 5f63 6c6f 7365    def auto_close
-0001bc60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001bc70: 2222 2249 6620 7472 7565 2c20 7468 6520  """If true, the 
-0001bc80: 7061 7468 2073 686f 756c 6420 6175 746f  path should auto
-0001bc90: 6d61 7469 6361 6c6c 7920 636c 6f73 6520  matically close 
-0001bca0: 6974 7365 6c66 2062 6566 6f72 6520 7061  itself before pa
-0001bcb0: 696e 7469 6e67 2e22 2222 0a20 2020 2020  inting.""".     
-0001bcc0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
-0001bcd0: 7479 6c65 2e61 7574 6f5f 636c 6f73 650a  tyle.auto_close.
-0001bce0: 0a20 2020 2040 6175 746f 5f63 6c6f 7365  .    @auto_close
-0001bcf0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-0001bd00: 6175 746f 5f63 6c6f 7365 2873 656c 662c  auto_close(self,
-0001bd10: 2073 686f 756c 6429 3a0a 2020 2020 2020   should):.      
-0001bd20: 2020 7365 6c66 2e73 7479 6c65 2e61 7574    self.style.aut
-0001bd30: 6f5f 636c 6f73 6520 3d20 7368 6f75 6c64  o_close = should
-0001bd40: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0001bd50: 2020 2020 6465 6620 7061 696e 745f 7275      def paint_ru
-0001bd60: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
-0001bd70: 2020 2222 224d 616e 7561 6c6c 7920 7370    """Manually sp
-0001bd80: 6563 6966 7920 7468 6520 6050 6174 6850  ecify the `PathP
-0001bd90: 6169 6e74 5275 6c65 6020 746f 2075 7365  aintRule` to use
-0001bda0: 2066 6f72 2072 656e 6465 7269 6e67 2074   for rendering t
-0001bdb0: 6865 2070 6174 682e 2222 220a 2020 2020  he path.""".    
-0001bdc0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001bdd0: 7374 796c 652e 7061 696e 745f 7275 6c65  style.paint_rule
-0001bde0: 0a0a 2020 2020 4070 6169 6e74 5f72 756c  ..    @paint_rul
-0001bdf0: 652e 7365 7474 6572 0a20 2020 2064 6566  e.setter.    def
-0001be00: 2070 6169 6e74 5f72 756c 6528 7365 6c66   paint_rule(self
-0001be10: 2c20 7374 796c 6529 3a0a 2020 2020 2020  , style):.      
-0001be20: 2020 7365 6c66 2e73 7479 6c65 2e70 6169    self.style.pai
-0001be30: 6e74 5f72 756c 6520 3d20 7374 796c 650a  nt_rule = style.
-0001be40: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0001be50: 2020 2064 6566 2063 6c69 7070 696e 675f     def clipping_
-0001be60: 7061 7468 2873 656c 6629 3a0a 2020 2020  path(self):.    
-0001be70: 2020 2020 2222 2253 6574 2074 6865 2063      """Set the c
-0001be80: 6c69 7070 696e 6720 7061 7468 2066 6f72  lipping path for
-0001be90: 2074 6869 7320 7061 7468 2e22 2222 0a20   this path.""". 
-0001bea0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001beb0: 6c66 2e5f 726f 6f74 5f67 7261 7068 6963  lf._root_graphic
-0001bec0: 735f 636f 6e74 6578 742e 636c 6970 7069  s_context.clippi
-0001bed0: 6e67 5f70 6174 680a 0a20 2020 2040 636c  ng_path..    @cl
-0001bee0: 6970 7069 6e67 5f70 6174 682e 7365 7474  ipping_path.sett
-0001bef0: 6572 0a20 2020 2064 6566 2063 6c69 7070  er.    def clipp
-0001bf00: 696e 675f 7061 7468 2873 656c 662c 206e  ing_path(self, n
-0001bf10: 6577 5f63 6c69 7061 7468 293a 0a20 2020  ew_clipath):.   
-0001bf20: 2020 2020 2073 656c 662e 5f72 6f6f 745f       self._root_
-0001bf30: 6772 6170 6869 6373 5f63 6f6e 7465 7874  graphics_context
-0001bf40: 2e63 6c69 7070 696e 675f 7061 7468 203d  .clipping_path =
-0001bf50: 206e 6577 5f63 6c69 7061 7468 0a0a 2020   new_clipath..  
-0001bf60: 2020 4063 6f6e 7465 7874 6d61 6e61 6765    @contextmanage
-0001bf70: 720a 2020 2020 6465 6620 5f6e 6577 5f67  r.    def _new_g
-0001bf80: 7261 7068 6963 735f 636f 6e74 6578 7428  raphics_context(
-0001bf90: 7365 6c66 2c20 5f61 7474 6163 683d 5472  self, _attach=Tr
-0001bfa0: 7565 293a 0a20 2020 2020 2020 206f 6c64  ue):.        old
-0001bfb0: 5f67 7261 7068 6963 735f 636f 6e74 6578  _graphics_contex
-0001bfc0: 7420 3d20 7365 6c66 2e5f 6772 6170 6869  t = self._graphi
-0001bfd0: 6373 5f63 6f6e 7465 7874 0a20 2020 2020  cs_context.     
-0001bfe0: 2020 206e 6577 5f67 7261 7068 6963 735f     new_graphics_
-0001bff0: 636f 6e74 6578 7420 3d20 4772 6170 6869  context = Graphi
-0001c000: 6373 436f 6e74 6578 7428 290a 2020 2020  csContext().    
-0001c010: 2020 2020 7365 6c66 2e5f 6772 6170 6869      self._graphi
-0001c020: 6373 5f63 6f6e 7465 7874 203d 206e 6577  cs_context = new
-0001c030: 5f67 7261 7068 6963 735f 636f 6e74 6578  _graphics_contex
-0001c040: 740a 2020 2020 2020 2020 7472 793a 0a20  t.        try:. 
-0001c050: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-0001c060: 206e 6577 5f67 7261 7068 6963 735f 636f   new_graphics_co
-0001c070: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
-0001c080: 2020 6966 205f 6174 7461 6368 3a0a 2020    if _attach:.  
-0001c090: 2020 2020 2020 2020 2020 2020 2020 6f6c                ol
-0001c0a0: 645f 6772 6170 6869 6373 5f63 6f6e 7465  d_graphics_conte
-0001c0b0: 7874 2e61 6464 5f69 7465 6d28 6e65 775f  xt.add_item(new_
-0001c0c0: 6772 6170 6869 6373 5f63 6f6e 7465 7874  graphics_context
-0001c0d0: 290a 2020 2020 2020 2020 6669 6e61 6c6c  ).        finall
-0001c0e0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0001c0f0: 656c 662e 5f67 7261 7068 6963 735f 636f  elf._graphics_co
-0001c100: 6e74 6578 7420 3d20 6f6c 645f 6772 6170  ntext = old_grap
-0001c110: 6869 6373 5f63 6f6e 7465 7874 0a0a 2020  hics_context..  
-0001c120: 2020 4063 6f6e 7465 7874 6d61 6e61 6765    @contextmanage
-0001c130: 720a 2020 2020 6465 6620 7472 616e 7366  r.    def transf
-0001c140: 6f72 6d5f 6772 6f75 7028 7365 6c66 2c20  orm_group(self, 
-0001c150: 7472 616e 7366 6f72 6d29 3a0a 2020 2020  transform):.    
-0001c160: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001c170: 4170 706c 7920 7468 6520 7072 6f76 6964  Apply the provid
-0001c180: 6564 2060 5472 616e 7366 6f72 6d60 2074  ed `Transform` t
-0001c190: 6f20 616c 6c20 706f 696e 7473 2061 6464  o all points add
-0001c1a0: 6564 2077 6974 6869 6e20 7468 6973 2063  ed within this c
-0001c1b0: 6f6e 7465 7874 2e0a 2020 2020 2020 2020  ontext..        
-0001c1c0: 2222 220a 2020 2020 2020 2020 7769 7468  """.        with
-0001c1d0: 2073 656c 662e 5f6e 6577 5f67 7261 7068   self._new_graph
-0001c1e0: 6963 735f 636f 6e74 6578 7428 2920 6173  ics_context() as
-0001c1f0: 2063 7478 743a 0a20 2020 2020 2020 2020   ctxt:.         
-0001c200: 2020 2063 7478 742e 7472 616e 7366 6f72     ctxt.transfor
-0001c210: 6d20 3d20 7472 616e 7366 6f72 6d0a 2020  m = transform.  
-0001c220: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-0001c230: 7365 6c66 0a0a 2020 2020 6465 6620 6164  self..    def ad
-0001c240: 645f 7061 7468 5f65 6c65 6d65 6e74 2873  d_path_element(s
-0001c250: 656c 662c 2069 7465 6d2c 205f 636f 7079  elf, item, _copy
-0001c260: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-0001c270: 2222 220a 2020 2020 2020 2020 4164 6420  """.        Add 
-0001c280: 7468 6520 6769 7665 6e20 656c 656d 656e  the given elemen
-0001c290: 7420 6173 2061 2070 6174 6820 6974 656d  t as a path item
-0001c2a0: 206f 6620 7468 6973 2070 6174 682e 0a0a   of this path...
-0001c2b0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0001c2c0: 2020 2020 2020 2020 2020 6974 656d 3a20            item: 
-0001c2d0: 7468 6520 6974 656d 2074 6f20 6164 6420  the item to add 
-0001c2e0: 746f 2074 6869 7320 7061 7468 2e0a 2020  to this path..  
-0001c2f0: 2020 2020 2020 2020 2020 5f63 6f70 7920            _copy 
-0001c300: 2862 6f6f 6c29 3a20 6966 2074 7275 6520  (bool): if true 
-0001c310: 2874 6865 2064 6566 6175 6c74 292c 2074  (the default), t
-0001c320: 6865 2069 7465 6d20 7769 6c6c 2062 6520  he item will be 
-0001c330: 636f 7069 6564 2062 6566 6f72 6520 6265  copied before be
-0001c340: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-0001c350: 2020 2020 6170 7065 6e64 6564 2e20 5468      appended. Th
-0001c360: 6973 2070 7265 7665 6e74 7320 6d6f 6469  is prevents modi
-0001c370: 6669 6361 7469 6f6e 7320 746f 2061 2072  fications to a r
-0001c380: 6566 6572 656e 6365 6420 6f62 6a65 6374  eferenced object
-0001c390: 2066 726f 6d0a 2020 2020 2020 2020 2020   from.          
-0001c3a0: 2020 2020 2020 2272 6574 726f 6163 7469        "retroacti
-0001c3b0: 7665 6c79 2220 616c 7465 7269 6e67 2069  vely" altering i
-0001c3c0: 7473 2073 7479 6c65 2f73 6861 7065 2061  ts style/shape a
-0001c3d0: 6e64 2073 686f 756c 6420 6265 2064 6973  nd should be dis
-0001c3e0: 6162 6c65 6420 7769 7468 0a20 2020 2020  abled with.     
-0001c3f0: 2020 2020 2020 2020 2020 2063 6175 7469             cauti
-0001c400: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-0001c410: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001c420: 5f73 7461 7274 6572 5f6d 6f76 6520 6973  _starter_move is
-0001c430: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0001c440: 2020 2020 2020 2073 656c 662e 5f63 6c6f         self._clo
-0001c450: 7365 6420 3d20 4661 6c73 650a 2020 2020  sed = False.    
-0001c460: 2020 2020 2020 2020 7365 6c66 2e5f 6772          self._gr
-0001c470: 6170 6869 6373 5f63 6f6e 7465 7874 2e61  aphics_context.a
-0001c480: 6464 5f69 7465 6d28 7365 6c66 2e5f 7374  dd_item(self._st
-0001c490: 6172 7465 725f 6d6f 7665 2c20 5f63 6f70  arter_move, _cop
-0001c4a0: 793d 4661 6c73 6529 0a20 2020 2020 2020  y=False).       
-0001c4b0: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
-0001c4c0: 5f63 6f6e 7465 7874 203d 2073 656c 662e  _context = self.
-0001c4d0: 5f67 7261 7068 6963 735f 636f 6e74 6578  _graphics_contex
-0001c4e0: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-0001c4f0: 6c66 2e5f 7374 6172 7465 725f 6d6f 7665  lf._starter_move
-0001c500: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-0001c510: 2073 656c 662e 5f67 7261 7068 6963 735f   self._graphics_
-0001c520: 636f 6e74 6578 742e 6164 645f 6974 656d  context.add_item
-0001c530: 2869 7465 6d2c 205f 636f 7079 3d5f 636f  (item, _copy=_co
-0001c540: 7079 290a 0a20 2020 2064 6566 2072 656d  py)..    def rem
-0001c550: 6f76 655f 6c61 7374 5f70 6174 685f 656c  ove_last_path_el
-0001c560: 656d 656e 7428 7365 6c66 293a 0a20 2020  ement(self):.   
-0001c570: 2020 2020 2073 656c 662e 5f67 7261 7068       self._graph
-0001c580: 6963 735f 636f 6e74 6578 742e 7265 6d6f  ics_context.remo
-0001c590: 7665 5f6c 6173 745f 6974 656d 2829 0a0a  ve_last_item()..
-0001c5a0: 2020 2020 6465 6620 7265 6374 616e 676c      def rectangl
-0001c5b0: 6528 7365 6c66 2c20 782c 2079 2c20 772c  e(self, x, y, w,
-0001c5c0: 2068 2c20 7278 3d30 2c20 7279 3d30 293a   h, rx=0, ry=0):
-0001c5d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001c5e0: 2020 2020 2041 7070 656e 6420 6120 7265       Append a re
-0001c5f0: 6374 616e 676c 6520 6173 2061 2063 6c6f  ctangle as a clo
-0001c600: 7365 6420 7375 6270 6174 6820 746f 2074  sed subpath to t
-0001c610: 6865 2063 7572 7265 6e74 2070 6174 682e  he current path.
-0001c620: 0a0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
-0001c630: 2077 6964 7468 206f 7220 7468 6520 6865   width or the he
-0001c640: 6967 6874 2061 7265 2030 2c20 7468 6520  ight are 0, the 
-0001c650: 7265 6374 616e 676c 6520 7769 6c6c 2062  rectangle will b
-0001c660: 6520 636f 6c6c 6170 7365 6420 746f 2061  e collapsed to a
-0001c670: 206c 696e 650a 2020 2020 2020 2020 2875   line.        (u
-0001c680: 6e6c 6573 7320 7468 6579 2772 6520 626f  nless they're bo
-0001c690: 7468 2030 2c20 696e 2077 6869 6368 2063  th 0, in which c
-0001c6a0: 6173 6520 6974 2773 2063 6f6c 6c61 7073  ase it's collaps
-0001c6b0: 6564 2074 6f20 6e6f 7468 696e 6729 2e0a  ed to nothing)..
-0001c6c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0001c6d0: 2020 2020 2020 2020 2020 2078 2028 4e75             x (Nu
-0001c6e0: 6d62 6572 293a 2074 6865 2061 6273 6369  mber): the absci
-0001c6f0: 7373 6120 6f66 2074 6865 2073 7461 7274  ssa of the start
-0001c700: 696e 6720 636f 726e 6572 206f 6620 7468  ing corner of th
-0001c710: 6520 7265 6374 616e 676c 652e 0a20 2020  e rectangle..   
-0001c720: 2020 2020 2020 2020 2079 2028 4e75 6d62           y (Numb
-0001c730: 6572 293a 2074 6865 206f 7264 696e 6174  er): the ordinat
-0001c740: 6520 6f66 2074 6865 2073 7461 7274 696e  e of the startin
-0001c750: 6720 636f 726e 6572 206f 6620 7468 6520  g corner of the 
-0001c760: 7265 6374 616e 676c 652e 0a20 2020 2020  rectangle..     
-0001c770: 2020 2020 2020 2077 2028 4e75 6d62 6572         w (Number
-0001c780: 293a 2074 6865 2077 6964 7468 206f 6620  ): the width of 
-0001c790: 7468 6520 7265 6374 616e 676c 6520 2869  the rectangle (i
-0001c7a0: 6620 302c 2074 6865 2072 6563 7461 6e67  f 0, the rectang
-0001c7b0: 6c65 2077 696c 6c20 6265 0a20 2020 2020  le will be.     
-0001c7c0: 2020 2020 2020 2020 2020 2072 656e 6465             rende
-0001c7d0: 7265 6420 6173 2061 2076 6572 7469 6361  red as a vertica
-0001c7e0: 6c20 6c69 6e65 292e 0a20 2020 2020 2020  l line)..       
-0001c7f0: 2020 2020 2068 2028 4e75 6d62 6572 293a       h (Number):
-0001c800: 2074 6865 2068 6569 6768 7420 6f66 2074   the height of t
-0001c810: 6865 2072 6563 7461 6e67 6c65 2028 6966  he rectangle (if
-0001c820: 2030 2c20 7468 6520 7265 6374 616e 676c   0, the rectangl
-0001c830: 6520 7769 6c6c 2062 650a 2020 2020 2020  e will be.      
-0001c840: 2020 2020 2020 2020 2020 7265 6e64 6572            render
-0001c850: 6564 2061 7320 6120 686f 7269 7a6f 6e74  ed as a horizont
-0001c860: 616c 206c 696e 6529 2e0a 2020 2020 2020  al line)..      
-0001c870: 2020 2020 2020 7278 2028 4e75 6d62 6572        rx (Number
-0001c880: 293a 2074 6865 2078 2d72 6164 6975 7320  ): the x-radius 
-0001c890: 6f66 2074 6865 2072 6563 7461 6e67 6c65  of the rectangle
-0001c8a0: 2072 6f75 6e64 6564 2063 6f72 6e65 7220   rounded corner 
-0001c8b0: 2869 6620 3020 7468 6520 636f 726e 6572  (if 0 the corner
-0001c8c0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0001c8d0: 2020 7769 6c6c 206e 6f74 2062 6520 726f    will not be ro
-0001c8e0: 756e 6465 6429 2e0a 2020 2020 2020 2020  unded)..        
-0001c8f0: 2020 2020 7279 2028 4e75 6d62 6572 293a      ry (Number):
-0001c900: 2074 6865 2079 2d72 6164 6975 7320 6f66   the y-radius of
-0001c910: 2074 6865 2072 6563 7461 6e67 6c65 2072   the rectangle r
-0001c920: 6f75 6e64 6564 2063 6f72 6e65 7220 2869  ounded corner (i
-0001c930: 6620 3020 7468 6520 636f 726e 6572 730a  f 0 the corners.
-0001c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c950: 7769 6c6c 206e 6f74 2062 6520 726f 756e  will not be roun
-0001c960: 6465 6429 2e0a 0a20 2020 2020 2020 2052  ded)...        R
-0001c970: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0001c980: 2020 2020 5468 6520 7061 7468 2c20 746f      The path, to
-0001c990: 2061 6c6c 6f77 2063 6861 696e 696e 6720   allow chaining 
-0001c9a0: 6d65 7468 6f64 2063 616c 6c73 2e0a 2020  method calls..  
-0001c9b0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0001c9c0: 2020 2073 656c 662e 5f69 6e73 6572 745f     self._insert_
-0001c9d0: 696d 706c 6963 6974 5f63 6c6f 7365 5f69  implicit_close_i
-0001c9e0: 665f 6f70 656e 2829 0a20 2020 2020 2020  f_open().       
-0001c9f0: 2073 656c 662e 6164 645f 7061 7468 5f65   self.add_path_e
-0001ca00: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-0001ca10: 2020 2020 526f 756e 6465 6452 6563 7461      RoundedRecta
-0001ca20: 6e67 6c65 2850 6f69 6e74 2878 2c20 7929  ngle(Point(x, y)
-0001ca30: 2c20 506f 696e 7428 772c 2068 292c 2050  , Point(w, h), P
-0001ca40: 6f69 6e74 2872 782c 2072 7929 292c 205f  oint(rx, ry)), _
-0001ca50: 636f 7079 3d46 616c 7365 0a20 2020 2020  copy=False.     
-0001ca60: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0001ca70: 662e 5f63 6c6f 7365 6420 3d20 5472 7565  f._closed = True
-0001ca80: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-0001ca90: 7665 5f74 6f28 782c 2079 290a 0a20 2020  ve_to(x, y)..   
-0001caa0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001cab0: 0a0a 2020 2020 6465 6620 6369 7263 6c65  ..    def circle
-0001cac0: 2873 656c 662c 2063 782c 2063 792c 2072  (self, cx, cy, r
-0001cad0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0001cae0: 2020 2020 2020 2041 7070 656e 6420 6120         Append a 
-0001caf0: 6369 7263 6c65 2061 7320 6120 636c 6f73  circle as a clos
-0001cb00: 6564 2073 7562 7061 7468 2074 6f20 7468  ed subpath to th
-0001cb10: 6520 6375 7272 656e 7420 7061 7468 2e0a  e current path..
-0001cb20: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0001cb30: 2020 2020 2020 2020 2020 2063 7820 284e             cx (N
-0001cb40: 756d 6265 7229 3a20 7468 6520 6162 7363  umber): the absc
-0001cb50: 6973 7361 206f 6620 7468 6520 6369 7263  issa of the circ
-0001cb60: 6c65 2773 2063 656e 7465 7220 706f 696e  le's center poin
-0001cb70: 742e 0a20 2020 2020 2020 2020 2020 2063  t..            c
-0001cb80: 7920 284e 756d 6265 7229 3a20 7468 6520  y (Number): the 
-0001cb90: 6f72 6469 6e61 7465 206f 6620 7468 6520  ordinate of the 
-0001cba0: 6369 7263 6c65 2773 2063 656e 7465 7220  circle's center 
-0001cbb0: 706f 696e 742e 0a20 2020 2020 2020 2020  point..         
-0001cbc0: 2020 2072 2028 4e75 6d62 6572 293a 2074     r (Number): t
-0001cbd0: 6865 2072 6164 6975 7320 6f66 2074 6865  he radius of the
-0001cbe0: 2063 6972 636c 652e 0a0a 2020 2020 2020   circle...      
-0001cbf0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0001cc00: 2020 2020 2020 2054 6865 2070 6174 682c         The path,
-0001cc10: 2074 6f20 616c 6c6f 7720 6368 6169 6e69   to allow chaini
-0001cc20: 6e67 206d 6574 686f 6420 6361 6c6c 732e  ng method calls.
-0001cc30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001cc40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001cc50: 2e65 6c6c 6970 7365 2863 782c 2063 792c  .ellipse(cx, cy,
-0001cc60: 2072 2c20 7229 0a0a 2020 2020 6465 6620   r, r)..    def 
-0001cc70: 656c 6c69 7073 6528 7365 6c66 2c20 6378  ellipse(self, cx
-0001cc80: 2c20 6379 2c20 7278 2c20 7279 293a 0a20  , cy, rx, ry):. 
-0001cc90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001cca0: 2020 2041 7070 656e 6420 616e 2065 6c6c     Append an ell
-0001ccb0: 6970 7365 2061 7320 6120 636c 6f73 6564  ipse as a closed
-0001ccc0: 2073 7562 7061 7468 2074 6f20 7468 6520   subpath to the 
-0001ccd0: 6375 7272 656e 7420 7061 7468 2e0a 0a20  current path... 
-0001cce0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0001ccf0: 2020 2020 2020 2020 2063 7820 284e 756d           cx (Num
-0001cd00: 6265 7229 3a20 7468 6520 6162 7363 6973  ber): the abscis
-0001cd10: 7361 206f 6620 7468 6520 656c 6c69 7073  sa of the ellips
-0001cd20: 6527 7320 6365 6e74 6572 2070 6f69 6e74  e's center point
-0001cd30: 2e0a 2020 2020 2020 2020 2020 2020 6379  ..            cy
-0001cd40: 2028 4e75 6d62 6572 293a 2074 6865 206f   (Number): the o
-0001cd50: 7264 696e 6174 6520 6f66 2074 6865 2065  rdinate of the e
-0001cd60: 6c6c 6970 7365 2773 2063 656e 7465 7220  llipse's center 
-0001cd70: 706f 696e 742e 0a20 2020 2020 2020 2020  point..         
-0001cd80: 2020 2072 7820 284e 756d 6265 7229 3a20     rx (Number): 
-0001cd90: 7468 6520 782d 7261 6469 7573 206f 6620  the x-radius of 
-0001cda0: 7468 6520 656c 6c69 7073 652e 0a20 2020  the ellipse..   
-0001cdb0: 2020 2020 2020 2020 2072 7920 284e 756d           ry (Num
-0001cdc0: 6265 7229 3a20 7468 6520 792d 7261 6469  ber): the y-radi
-0001cdd0: 7573 206f 6620 7468 6520 656c 6c69 7073  us of the ellips
-0001cde0: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-0001cdf0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0001ce00: 2054 6865 2070 6174 682c 2074 6f20 616c   The path, to al
-0001ce10: 6c6f 7720 6368 6169 6e69 6e67 206d 6574  low chaining met
-0001ce20: 686f 6420 6361 6c6c 732e 0a20 2020 2020  hod calls..     
-0001ce30: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-0001ce40: 656c 662e 5f69 6e73 6572 745f 696d 706c  elf._insert_impl
-0001ce50: 6963 6974 5f63 6c6f 7365 5f69 665f 6f70  icit_close_if_op
-0001ce60: 656e 2829 0a20 2020 2020 2020 2073 656c  en().        sel
-0001ce70: 662e 6164 645f 7061 7468 5f65 6c65 6d65  f.add_path_eleme
-0001ce80: 6e74 2845 6c6c 6970 7365 2850 6f69 6e74  nt(Ellipse(Point
-0001ce90: 2872 782c 2072 7929 2c20 506f 696e 7428  (rx, ry), Point(
-0001cea0: 6378 2c20 6379 2929 2c20 5f63 6f70 793d  cx, cy)), _copy=
-0001ceb0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
-0001cec0: 656c 662e 5f63 6c6f 7365 6420 3d20 5472  elf._closed = Tr
-0001ced0: 7565 0a20 2020 2020 2020 2073 656c 662e  ue.        self.
-0001cee0: 6d6f 7665 5f74 6f28 6378 2c20 6379 290a  move_to(cx, cy).
-0001cef0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001cf00: 7365 6c66 0a0a 2020 2020 6465 6620 6d6f  self..    def mo
-0001cf10: 7665 5f74 6f28 7365 6c66 2c20 782c 2079  ve_to(self, x, y
-0001cf20: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0001cf30: 2020 2020 2020 2053 7461 7274 2061 206e         Start a n
-0001cf40: 6577 2073 7562 7061 7468 206f 7220 6d6f  ew subpath or mo
-0001cf50: 7665 2074 6865 2070 6174 6820 7374 6172  ve the path star
-0001cf60: 7469 6e67 2070 6f69 6e74 2e0a 0a20 2020  ting point...   
-0001cf70: 2020 2020 2049 6620 6e6f 2070 6174 6820       If no path 
-0001cf80: 656c 656d 656e 7473 2068 6176 6520 6265  elements have be
-0001cf90: 656e 2061 6464 6564 2079 6574 2c20 7468  en added yet, th
-0001cfa0: 6973 2077 696c 6c20 6368 616e 6765 2074  is will change t
-0001cfb0: 6865 2070 6174 6820 7374 6172 7469 6e67  he path starting
-0001cfc0: 0a20 2020 2020 2020 2070 6f69 6e74 2e20  .        point. 
-0001cfd0: 4966 2070 6174 6820 656c 656d 656e 7473  If path elements
-0001cfe0: 2068 6176 6520 6265 656e 2061 6464 6564   have been added
-0001cff0: 2c20 7468 6973 2077 696c 6c20 696e 7365  , this will inse
-0001d000: 7274 2061 6e20 696d 706c 6963 6974 2063  rt an implicit c
-0001d010: 6c6f 7365 2069 6e0a 2020 2020 2020 2020  lose in.        
-0001d020: 6f72 6465 7220 746f 2073 7461 7274 2061  order to start a
-0001d030: 206e 6577 2073 7562 7061 7468 2e0a 0a20   new subpath... 
-0001d040: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0001d050: 2020 2020 2020 2020 2078 2028 4e75 6d62           x (Numb
-0001d060: 6572 293a 2061 6273 6369 7373 6120 6f66  er): abscissa of
-0001d070: 2074 6865 2028 7375 6229 7061 7468 2073   the (sub)path s
-0001d080: 7461 7274 696e 6720 706f 696e 742e 0a20  tarting point.. 
-0001d090: 2020 2020 2020 2020 2020 2079 2028 4e75             y (Nu
-0001d0a0: 6d62 6572 293a 206f 7264 696e 6174 6520  mber): ordinate 
-0001d0b0: 6f66 2074 6865 2028 7375 6229 7061 7468  of the (sub)path
-0001d0c0: 2073 7461 7274 696e 6720 706f 696e 742e   starting point.
-0001d0d0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0001d0e0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-0001d0f0: 6865 2070 6174 682c 2074 6f20 616c 6c6f  he path, to allo
-0001d100: 7720 6368 6169 6e69 6e67 206d 6574 686f  w chaining metho
-0001d110: 6420 6361 6c6c 732e 0a20 2020 2020 2020  d calls..       
-0001d120: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-0001d130: 662e 5f69 6e73 6572 745f 696d 706c 6963  f._insert_implic
-0001d140: 6974 5f63 6c6f 7365 5f69 665f 6f70 656e  it_close_if_open
-0001d150: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0001d160: 5f73 7461 7274 6572 5f6d 6f76 6520 3d20  _starter_move = 
-0001d170: 4d6f 7665 2850 6f69 6e74 2878 2c20 7929  Move(Point(x, y)
-0001d180: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0001d190: 2073 656c 660a 0a20 2020 2064 6566 206d   self..    def m
-0001d1a0: 6f76 655f 7265 6c61 7469 7665 2873 656c  ove_relative(sel
-0001d1b0: 662c 2078 2c20 7929 3a0a 2020 2020 2020  f, x, y):.      
-0001d1c0: 2020 2222 220a 2020 2020 2020 2020 5374    """.        St
-0001d1d0: 6172 7420 6120 6e65 7720 7375 6270 6174  art a new subpat
-0001d1e0: 6820 6f72 206d 6f76 6520 7468 6520 7061  h or move the pa
-0001d1f0: 7468 2073 7461 7274 2070 6f69 6e74 2072  th start point r
-0001d200: 656c 6174 6976 6520 746f 2074 6865 2070  elative to the p
-0001d210: 7265 7669 6f75 7320 706f 696e 742e 0a0a  revious point...
-0001d220: 2020 2020 2020 2020 4966 206e 6f20 7061          If no pa
-0001d230: 7468 2065 6c65 6d65 6e74 7320 6861 7665  th elements have
-0001d240: 2062 6565 6e20 6164 6465 6420 7965 742c   been added yet,
-0001d250: 2074 6869 7320 7769 6c6c 2063 6861 6e67   this will chang
-0001d260: 6520 7468 6520 7061 7468 2073 7461 7274  e the path start
-0001d270: 696e 670a 2020 2020 2020 2020 706f 696e  ing.        poin
-0001d280: 742e 2049 6620 7061 7468 2065 6c65 6d65  t. If path eleme
-0001d290: 6e74 7320 6861 7665 2062 6565 6e20 6164  nts have been ad
-0001d2a0: 6465 642c 2074 6869 7320 7769 6c6c 2069  ded, this will i
-0001d2b0: 6e73 6572 7420 616e 2069 6d70 6c69 6369  nsert an implici
-0001d2c0: 7420 636c 6f73 6520 696e 0a20 2020 2020  t close in.     
-0001d2d0: 2020 206f 7264 6572 2074 6f20 7374 6172     order to star
-0001d2e0: 7420 6120 6e65 7720 7375 6270 6174 682e  t a new subpath.
-0001d2f0: 0a0a 2020 2020 2020 2020 5468 6973 2077  ..        This w
-0001d300: 696c 6c20 6f76 6572 7772 6974 6520 616e  ill overwrite an
-0001d310: 2061 6273 6f6c 7574 6520 6d6f 7665 5f74   absolute move_t
-0001d320: 6f20 6173 206c 6f6e 6720 6173 206e 6f20  o as long as no 
-0001d330: 6e6f 6e2d 6d6f 7665 2070 6174 6820 6974  non-move path it
-0001d340: 656d 7320 6861 7665 0a20 2020 2020 2020  ems have.       
-0001d350: 2062 6565 6e20 6170 7065 6e64 6564 2e20   been appended. 
-0001d360: 5468 6520 7265 6c61 7469 7665 2070 6f73  The relative pos
-0001d370: 6974 696f 6e20 6973 2072 6573 6f6c 7665  ition is resolve
-0001d380: 6420 6672 6f6d 2074 6865 2070 7265 7669  d from the previ
-0001d390: 6f75 7320 6974 656d 2077 6865 6e0a 2020  ous item when.  
-0001d3a0: 2020 2020 2020 7468 6520 7061 7468 2069        the path i
-0001d3b0: 7320 6265 696e 6720 7265 6e64 6572 6564  s being rendered
-0001d3c0: 2c20 6f72 2066 726f 6d20 302c 2030 2069  , or from 0, 0 i
-0001d3d0: 6620 6974 2069 7320 7468 6520 6669 7273  f it is the firs
-0001d3e0: 7420 6974 656d 2e0a 0a20 2020 2020 2020  t item...       
-0001d3f0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0001d400: 2020 2078 2028 4e75 6d62 6572 293a 2061     x (Number): a
-0001d410: 6273 6369 7373 6120 6f66 2074 6865 2028  bscissa of the (
-0001d420: 7375 6229 7061 7468 2073 7461 7274 696e  sub)path startin
-0001d430: 6720 706f 696e 7420 7265 6c61 7469 7665  g point relative
-0001d440: 2074 6f20 7468 652e 0a20 2020 2020 2020   to the..       
-0001d450: 2020 2020 2079 2028 4e75 6d62 6572 293a       y (Number):
-0001d460: 206f 7264 696e 6174 6520 6f66 2074 6865   ordinate of the
-0001d470: 2028 7375 6229 7061 7468 2073 7461 7274   (sub)path start
-0001d480: 696e 6720 706f 696e 7420 7265 6c61 7469  ing point relati
-0001d490: 7665 2074 6f20 7468 652e 0a20 2020 2020  ve to the..     
-0001d4a0: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-0001d4b0: 656c 662e 5f69 6e73 6572 745f 696d 706c  elf._insert_impl
-0001d4c0: 6963 6974 5f63 6c6f 7365 5f69 665f 6f70  icit_close_if_op
-0001d4d0: 656e 2829 0a20 2020 2020 2020 2069 6620  en().        if 
-0001d4e0: 7365 6c66 2e5f 7374 6172 7465 725f 6d6f  self._starter_mo
-0001d4f0: 7665 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ve is not None:.
-0001d500: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001d510: 2e5f 636c 6f73 6564 203d 2046 616c 7365  ._closed = False
-0001d520: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001d530: 662e 5f67 7261 7068 6963 735f 636f 6e74  f._graphics_cont
-0001d540: 6578 742e 6164 645f 6974 656d 2873 656c  ext.add_item(sel
-0001d550: 662e 5f73 7461 7274 6572 5f6d 6f76 652c  f._starter_move,
-0001d560: 205f 636f 7079 3d46 616c 7365 290a 2020   _copy=False).  
-0001d570: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0001d580: 636c 6f73 655f 636f 6e74 6578 7420 3d20  close_context = 
-0001d590: 7365 6c66 2e5f 6772 6170 6869 6373 5f63  self._graphics_c
-0001d5a0: 6f6e 7465 7874 0a20 2020 2020 2020 2073  ontext.        s
-0001d5b0: 656c 662e 5f73 7461 7274 6572 5f6d 6f76  elf._starter_mov
-0001d5c0: 6520 3d20 5265 6c61 7469 7665 4d6f 7665  e = RelativeMove
-0001d5d0: 2850 6f69 6e74 2878 2c20 7929 290a 2020  (Point(x, y)).  
-0001d5e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001d5f0: 660a 0a20 2020 2064 6566 206c 696e 655f  f..    def line_
-0001d600: 746f 2873 656c 662c 2078 2c20 7929 3a0a  to(self, x, y):.
-0001d610: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001d620: 2020 2020 4170 7065 6e64 2061 2073 7472      Append a str
-0001d630: 6169 6768 7420 6c69 6e65 2074 6f20 7468  aight line to th
-0001d640: 6973 2070 6174 682e 0a0a 2020 2020 2020  is path...      
-0001d650: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0001d660: 2020 2020 7820 284e 756d 6265 7229 3a20      x (Number): 
-0001d670: 6162 7363 6973 7361 2074 6865 206c 696e  abscissa the lin
-0001d680: 6527 7320 656e 6420 706f 696e 742e 0a20  e's end point.. 
-0001d690: 2020 2020 2020 2020 2020 2079 2028 4e75             y (Nu
-0001d6a0: 6d62 6572 293a 206f 7264 696e 6174 6520  mber): ordinate 
-0001d6b0: 6f66 2074 6865 206c 696e 6527 7320 656e  of the line's en
-0001d6c0: 6420 706f 696e 742e 0a0a 2020 2020 2020  d point...      
-0001d6d0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0001d6e0: 2020 2020 2020 2054 6865 2070 6174 682c         The path,
-0001d6f0: 2074 6f20 616c 6c6f 7720 6368 6169 6e69   to allow chaini
-0001d700: 6e67 206d 6574 686f 6420 6361 6c6c 732e  ng method calls.
-0001d710: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001d720: 2020 2020 2073 656c 662e 6164 645f 7061       self.add_pa
-0001d730: 7468 5f65 6c65 6d65 6e74 284c 696e 6528  th_element(Line(
-0001d740: 506f 696e 7428 782c 2079 2929 2c20 5f63  Point(x, y)), _c
-0001d750: 6f70 793d 4661 6c73 6529 0a20 2020 2020  opy=False).     
-0001d760: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0001d770: 2020 2020 6465 6620 6c69 6e65 5f72 656c      def line_rel
-0001d780: 6174 6976 6528 7365 6c66 2c20 6478 2c20  ative(self, dx, 
-0001d790: 6479 293a 0a20 2020 2020 2020 2022 2222  dy):.        """
-0001d7a0: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
-0001d7b0: 6120 7374 7261 6967 6874 206c 696e 6520  a straight line 
-0001d7c0: 7768 6f73 6520 656e 6420 6973 2063 6f6d  whose end is com
-0001d7d0: 7075 7465 6420 6173 2061 6e20 6f66 6673  puted as an offs
-0001d7e0: 6574 2066 726f 6d20 7468 6520 656e 6420  et from the end 
-0001d7f0: 6f66 2074 6865 0a20 2020 2020 2020 2070  of the.        p
-0001d800: 7265 7669 6f75 7320 7061 7468 2065 6c65  revious path ele
-0001d810: 6d65 6e74 2e0a 0a20 2020 2020 2020 2041  ment...        A
-0001d820: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0001d830: 2078 2028 4e75 6d62 6572 293a 2061 6273   x (Number): abs
-0001d840: 6369 7373 6120 7468 6520 6c69 6e65 2773  cissa the line's
-0001d850: 2065 6e64 2070 6f69 6e74 2072 656c 6174   end point relat
-0001d860: 6976 6520 746f 2074 6865 2065 6e64 2070  ive to the end p
-0001d870: 6f69 6e74 206f 6620 7468 650a 2020 2020  oint of the.    
-0001d880: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-0001d890: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
-0001d8a0: 742e 0a20 2020 2020 2020 2020 2020 2079  t..            y
-0001d8b0: 2028 4e75 6d62 6572 293a 206f 7264 696e   (Number): ordin
-0001d8c0: 6174 6520 6f66 2074 6865 206c 696e 6527  ate of the line'
-0001d8d0: 7320 656e 6420 706f 696e 7420 7265 6c61  s end point rela
-0001d8e0: 7469 7665 2074 6f20 7468 6520 656e 6420  tive to the end 
-0001d8f0: 706f 696e 7420 6f66 0a20 2020 2020 2020  point of.       
-0001d900: 2020 2020 2020 2020 2074 6865 2070 7265           the pre
-0001d910: 7669 6f75 7320 7061 7468 2065 6c65 6d65  vious path eleme
-0001d920: 6e74 2e0a 0a20 2020 2020 2020 2052 6574  nt...        Ret
-0001d930: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0001d940: 2020 5468 6520 7061 7468 2c20 746f 2061    The path, to a
-0001d950: 6c6c 6f77 2063 6861 696e 696e 6720 6d65  llow chaining me
-0001d960: 7468 6f64 2063 616c 6c73 2e0a 2020 2020  thod calls..    
-0001d970: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001d980: 7365 6c66 2e61 6464 5f70 6174 685f 656c  self.add_path_el
-0001d990: 656d 656e 7428 5265 6c61 7469 7665 4c69  ement(RelativeLi
-0001d9a0: 6e65 2850 6f69 6e74 2864 782c 2064 7929  ne(Point(dx, dy)
-0001d9b0: 292c 205f 636f 7079 3d46 616c 7365 290a  ), _copy=False).
-0001d9c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001d9d0: 656c 660a 0a20 2020 2064 6566 2068 6f72  elf..    def hor
-0001d9e0: 697a 6f6e 7461 6c5f 6c69 6e65 5f74 6f28  izontal_line_to(
-0001d9f0: 7365 6c66 2c20 7829 3a0a 2020 2020 2020  self, x):.      
-0001da00: 2020 2222 220a 2020 2020 2020 2020 4170    """.        Ap
-0001da10: 7065 6e64 2061 2073 7472 6169 6768 7420  pend a straight 
-0001da20: 686f 7269 7a6f 6e74 616c 206c 696e 6520  horizontal line 
-0001da30: 746f 2074 6865 2067 6976 656e 2061 6273  to the given abs
-0001da40: 6369 7373 612e 2054 6865 206f 7264 696e  cissa. The ordin
-0001da50: 6174 6520 6973 0a20 2020 2020 2020 2072  ate is.        r
-0001da60: 6574 7269 6576 6564 2066 726f 6d20 7468  etrieved from th
-0001da70: 6520 656e 6420 706f 696e 7420 6f66 2074  e end point of t
-0001da80: 6865 2070 7265 7669 6f75 7320 7061 7468  he previous path
-0001da90: 2065 6c65 6d65 6e74 2e0a 0a20 2020 2020   element...     
-0001daa0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0001dab0: 2020 2020 2078 2028 4e75 6d62 6572 293a       x (Number):
-0001dac0: 2061 6273 6369 7373 6120 6f66 2074 6865   abscissa of the
-0001dad0: 206c 696e 6527 7320 656e 6420 706f 696e   line's end poin
-0001dae0: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
-0001daf0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0001db00: 2054 6865 2070 6174 682c 2074 6f20 616c   The path, to al
-0001db10: 6c6f 7720 6368 6169 6e69 6e67 206d 6574  low chaining met
-0001db20: 686f 6420 6361 6c6c 732e 0a20 2020 2020  hod calls..     
-0001db30: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-0001db40: 656c 662e 6164 645f 7061 7468 5f65 6c65  elf.add_path_ele
-0001db50: 6d65 6e74 2848 6f72 697a 6f6e 7461 6c4c  ment(HorizontalL
-0001db60: 696e 6528 7829 2c20 5f63 6f70 793d 4661  ine(x), _copy=Fa
-0001db70: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
-0001db80: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
-0001db90: 6620 686f 7269 7a6f 6e74 616c 5f6c 696e  f horizontal_lin
-0001dba0: 655f 7265 6c61 7469 7665 2873 656c 662c  e_relative(self,
-0001dbb0: 2064 7829 3a0a 2020 2020 2020 2020 2222   dx):.        ""
-0001dbc0: 220a 2020 2020 2020 2020 4170 7065 6e64  ".        Append
-0001dbd0: 2061 2073 7472 6169 6768 7420 686f 7269   a straight hori
-0001dbe0: 7a6f 6e74 616c 206c 696e 6520 746f 2074  zontal line to t
-0001dbf0: 6865 2067 6976 656e 206f 6666 7365 7420  he given offset 
-0001dc00: 6672 6f6d 2074 6865 2070 7265 7669 6f75  from the previou
-0001dc10: 7320 7061 7468 0a20 2020 2020 2020 2065  s path.        e
-0001dc20: 6c65 6d65 6e74 2e20 5468 6520 6f72 6469  lement. The ordi
-0001dc30: 6e61 7465 2069 7320 7265 7472 6965 7665  nate is retrieve
-0001dc40: 6420 6672 6f6d 2074 6865 2065 6e64 2070  d from the end p
-0001dc50: 6f69 6e74 206f 6620 7468 6520 7072 6576  oint of the prev
-0001dc60: 696f 7573 2070 6174 680a 2020 2020 2020  ious path.      
-0001dc70: 2020 656c 656d 656e 742e 0a0a 2020 2020    element...    
-0001dc80: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0001dc90: 2020 2020 2020 7820 284e 756d 6265 7229        x (Number)
-0001dca0: 3a20 6162 7363 6973 7361 206f 6620 7468  : abscissa of th
-0001dcb0: 6520 6c69 6e65 2773 2065 6e64 2070 6f69  e line's end poi
-0001dcc0: 6e74 2072 656c 6174 6976 6520 746f 2074  nt relative to t
-0001dcd0: 6865 2065 6e64 2070 6f69 6e74 206f 660a  he end point of.
-0001dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcf0: 7468 6520 7072 6576 696f 7573 2070 6174  the previous pat
-0001dd00: 6820 656c 656d 656e 742e 0a0a 2020 2020  h element...    
-0001dd10: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0001dd20: 2020 2020 2020 2020 2054 6865 2070 6174           The pat
-0001dd30: 682c 2074 6f20 616c 6c6f 7720 6368 6169  h, to allow chai
-0001dd40: 6e69 6e67 206d 6574 686f 6420 6361 6c6c  ning method call
-0001dd50: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-0001dd60: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
-0001dd70: 7061 7468 5f65 6c65 6d65 6e74 2852 656c  path_element(Rel
-0001dd80: 6174 6976 6548 6f72 697a 6f6e 7461 6c4c  ativeHorizontalL
-0001dd90: 696e 6528 6478 292c 205f 636f 7079 3d46  ine(dx), _copy=F
-0001dda0: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
-0001ddb0: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
-0001ddc0: 6566 2076 6572 7469 6361 6c5f 6c69 6e65  ef vertical_line
-0001ddd0: 5f74 6f28 7365 6c66 2c20 7929 3a0a 2020  _to(self, y):.  
-0001dde0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001ddf0: 2020 4170 7065 6e64 2061 2073 7472 6169    Append a strai
-0001de00: 6768 7420 7665 7274 6963 616c 206c 696e  ght vertical lin
-0001de10: 6520 746f 2074 6865 2067 6976 656e 206f  e to the given o
-0001de20: 7264 696e 6174 652e 2054 6865 2061 6273  rdinate. The abs
-0001de30: 6369 7373 6120 6973 0a20 2020 2020 2020  cissa is.       
-0001de40: 2072 6574 7269 6576 6564 2066 726f 6d20   retrieved from 
-0001de50: 7468 6520 656e 6420 706f 696e 7420 6f66  the end point of
-0001de60: 2074 6865 2070 7265 7669 6f75 7320 7061   the previous pa
-0001de70: 7468 2065 6c65 6d65 6e74 2e0a 0a20 2020  th element...   
-0001de80: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0001de90: 2020 2020 2020 2079 2028 4e75 6d62 6572         y (Number
-0001dea0: 293a 206f 7264 696e 6174 6520 6f66 2074  ): ordinate of t
-0001deb0: 6865 206c 696e 6527 7320 656e 6420 706f  he line's end po
-0001dec0: 696e 742e 0a0a 2020 2020 2020 2020 5265  int...        Re
-0001ded0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0001dee0: 2020 2054 6865 2070 6174 682c 2074 6f20     The path, to 
-0001def0: 616c 6c6f 7720 6368 6169 6e69 6e67 206d  allow chaining m
-0001df00: 6574 686f 6420 6361 6c6c 732e 0a20 2020  ethod calls..   
-0001df10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001df20: 2073 656c 662e 6164 645f 7061 7468 5f65   self.add_path_e
-0001df30: 6c65 6d65 6e74 2856 6572 7469 6361 6c4c  lement(VerticalL
-0001df40: 696e 6528 7929 2c20 5f63 6f70 793d 4661  ine(y), _copy=Fa
-0001df50: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
-0001df60: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
-0001df70: 6620 7665 7274 6963 616c 5f6c 696e 655f  f vertical_line_
-0001df80: 7265 6c61 7469 7665 2873 656c 662c 2064  relative(self, d
-0001df90: 7929 3a0a 2020 2020 2020 2020 2222 220a  y):.        """.
-0001dfa0: 2020 2020 2020 2020 4170 7065 6e64 2061          Append a
-0001dfb0: 2073 7472 6169 6768 7420 7665 7274 6963   straight vertic
-0001dfc0: 616c 206c 696e 6520 746f 2074 6865 2067  al line to the g
-0001dfd0: 6976 656e 206f 6666 7365 7420 6672 6f6d  iven offset from
-0001dfe0: 2074 6865 2070 7265 7669 6f75 7320 7061   the previous pa
-0001dff0: 7468 0a20 2020 2020 2020 2065 6c65 6d65  th.        eleme
-0001e000: 6e74 2e20 5468 6520 6162 7363 6973 7361  nt. The abscissa
-0001e010: 2069 7320 7265 7472 6965 7665 6420 6672   is retrieved fr
-0001e020: 6f6d 2074 6865 2065 6e64 2070 6f69 6e74  om the end point
-0001e030: 206f 6620 7468 6520 7072 6576 696f 7573   of the previous
-0001e040: 2070 6174 680a 2020 2020 2020 2020 656c   path.        el
-0001e050: 656d 656e 742e 0a0a 2020 2020 2020 2020  ement...        
-0001e060: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0001e070: 2020 7920 284e 756d 6265 7229 3a20 6f72    y (Number): or
-0001e080: 6469 6e61 7465 206f 6620 7468 6520 6c69  dinate of the li
-0001e090: 6e65 2773 2065 6e64 2070 6f69 6e74 2072  ne's end point r
-0001e0a0: 656c 6174 6976 6520 746f 2074 6865 2065  elative to the e
-0001e0b0: 6e64 2070 6f69 6e74 206f 660a 2020 2020  nd point of.    
-0001e0c0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-0001e0d0: 7072 6576 696f 7573 2070 6174 6820 656c  previous path el
-0001e0e0: 656d 656e 742e 0a0a 2020 2020 2020 2020  ement...        
-0001e0f0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-0001e100: 2020 2020 2054 6865 2070 6174 682c 2074       The path, t
-0001e110: 6f20 616c 6c6f 7720 6368 6169 6e69 6e67  o allow chaining
-0001e120: 206d 6574 686f 6420 6361 6c6c 732e 0a20   method calls.. 
-0001e130: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001e140: 2020 2073 656c 662e 6164 645f 7061 7468     self.add_path
-0001e150: 5f65 6c65 6d65 6e74 2852 656c 6174 6976  _element(Relativ
-0001e160: 6556 6572 7469 6361 6c4c 696e 6528 6479  eVerticalLine(dy
-0001e170: 292c 205f 636f 7079 3d46 616c 7365 290a  ), _copy=False).
-0001e180: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001e190: 656c 660a 0a20 2020 2064 6566 2063 7572  elf..    def cur
-0001e1a0: 7665 5f74 6f28 7365 6c66 2c20 7831 2c20  ve_to(self, x1, 
-0001e1b0: 7931 2c20 7832 2c20 7932 2c20 7833 2c20  y1, x2, y2, x3, 
-0001e1c0: 7933 293a 0a20 2020 2020 2020 2022 2222  y3):.        """
-0001e1d0: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
-0001e1e0: 6120 6375 6269 6320 42c3 a97a 6965 7220  a cubic B..zier 
-0001e1f0: 6375 7276 6520 746f 2074 6869 7320 7061  curve to this pa
-0001e200: 7468 2e0a 0a20 2020 2020 2020 2041 7267  th...        Arg
-0001e210: 733a 0a20 2020 2020 2020 2020 2020 2078  s:.            x
-0001e220: 3120 284e 756d 6265 7229 3a20 6162 7363  1 (Number): absc
-0001e230: 6973 7361 206f 6620 7468 6520 6669 7273  issa of the firs
-0001e240: 7420 636f 6e74 726f 6c20 706f 696e 740a  t control point.
-0001e250: 2020 2020 2020 2020 2020 2020 7931 2028              y1 (
-0001e260: 4e75 6d62 6572 293a 206f 7264 696e 6174  Number): ordinat
-0001e270: 6520 6f66 2074 6865 2066 6972 7374 2063  e of the first c
-0001e280: 6f6e 7472 6f6c 2070 6f69 6e74 0a20 2020  ontrol point.   
-0001e290: 2020 2020 2020 2020 2078 3220 284e 756d           x2 (Num
-0001e2a0: 6265 7229 3a20 6162 7363 6973 7361 206f  ber): abscissa o
-0001e2b0: 6620 7468 6520 7365 636f 6e64 2063 6f6e  f the second con
-0001e2c0: 7472 6f6c 2070 6f69 6e74 0a20 2020 2020  trol point.     
-0001e2d0: 2020 2020 2020 2079 3220 284e 756d 6265         y2 (Numbe
-0001e2e0: 7229 3a20 6f72 6469 6e61 7465 206f 6620  r): ordinate of 
-0001e2f0: 7468 6520 7365 636f 6e64 2063 6f6e 7472  the second contr
-0001e300: 6f6c 2070 6f69 6e74 0a20 2020 2020 2020  ol point.       
-0001e310: 2020 2020 2078 3320 284e 756d 6265 7229       x3 (Number)
-0001e320: 3a20 6162 7363 6973 7361 206f 6620 7468  : abscissa of th
-0001e330: 6520 656e 6420 706f 696e 740a 2020 2020  e end point.    
-0001e340: 2020 2020 2020 2020 7933 2028 4e75 6d62          y3 (Numb
-0001e350: 6572 293a 206f 7264 696e 6174 6520 6f66  er): ordinate of
-0001e360: 2074 6865 2065 6e64 2070 6f69 6e74 0a0a   the end point..
-0001e370: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0001e380: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-0001e390: 2070 6174 682c 2074 6f20 616c 6c6f 7720   path, to allow 
-0001e3a0: 6368 6169 6e69 6e67 206d 6574 686f 6420  chaining method 
-0001e3b0: 6361 6c6c 732e 0a20 2020 2020 2020 2022  calls..        "
-0001e3c0: 2222 0a20 2020 2020 2020 2063 7472 6c31  "".        ctrl1
-0001e3d0: 203d 2050 6f69 6e74 2878 312c 2079 3129   = Point(x1, y1)
-0001e3e0: 0a20 2020 2020 2020 2063 7472 6c32 203d  .        ctrl2 =
-0001e3f0: 2050 6f69 6e74 2878 322c 2079 3229 0a20   Point(x2, y2). 
-0001e400: 2020 2020 2020 2065 6e64 203d 2050 6f69         end = Poi
-0001e410: 6e74 2878 332c 2079 3329 0a0a 2020 2020  nt(x3, y3)..    
-0001e420: 2020 2020 7365 6c66 2e61 6464 5f70 6174      self.add_pat
-0001e430: 685f 656c 656d 656e 7428 4265 7a69 6572  h_element(Bezier
-0001e440: 4375 7276 6528 6374 726c 312c 2063 7472  Curve(ctrl1, ctr
-0001e450: 6c32 2c20 656e 6429 2c20 5f63 6f70 793d  l2, end), _copy=
-0001e460: 4661 6c73 6529 0a20 2020 2020 2020 2072  False).        r
-0001e470: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
-0001e480: 6465 6620 6375 7276 655f 7265 6c61 7469  def curve_relati
-0001e490: 7665 2873 656c 662c 2064 7831 2c20 6479  ve(self, dx1, dy
-0001e4a0: 312c 2064 7832 2c20 6479 322c 2064 7833  1, dx2, dy2, dx3
-0001e4b0: 2c20 6479 3329 3a0a 2020 2020 2020 2020  , dy3):.        
-0001e4c0: 2222 220a 2020 2020 2020 2020 4170 7065  """.        Appe
-0001e4d0: 6e64 2061 2063 7562 6963 2042 c3a9 7a69  nd a cubic B..zi
-0001e4e0: 6572 2063 7572 7665 2077 686f 7365 2070  er curve whose p
-0001e4f0: 6f69 6e74 7320 6172 6520 6578 7072 6573  oints are expres
-0001e500: 7365 6420 7265 6c61 7469 7665 2074 6f20  sed relative to 
-0001e510: 7468 650a 2020 2020 2020 2020 656e 6420  the.        end 
-0001e520: 706f 696e 7420 6f66 2074 6865 2070 7265  point of the pre
-0001e530: 7669 6f75 7320 7061 7468 2065 6c65 6d65  vious path eleme
-0001e540: 6e74 2e0a 0a20 2020 2020 2020 2045 2e67  nt...        E.g
-0001e550: 2e20 7769 7468 2061 2073 7461 7274 2070  . with a start p
-0001e560: 6f69 6e74 206f 6620 2830 2c20 3029 2c20  oint of (0, 0), 
-0001e570: 6769 7665 6e20 2831 2c20 3129 2c20 2832  given (1, 1), (2
-0001e580: 2c20 3229 2c20 2833 2c20 3329 2c20 7468  , 2), (3, 3), th
-0001e590: 6520 6f75 7470 7574 0a20 2020 2020 2020  e output.       
-0001e5a0: 2063 7572 7665 2077 6f75 6c64 2068 6176   curve would hav
-0001e5b0: 6520 7468 6520 706f 696e 7473 3a0a 0a20  e the points:.. 
-0001e5c0: 2020 2020 2020 2028 302c 2030 2920 6331         (0, 0) c1
-0001e5d0: 2028 312c 2031 2920 6332 2028 332c 2033   (1, 1) c2 (3, 3
-0001e5e0: 2920 6520 2836 2c20 3629 0a0a 2020 2020  ) e (6, 6)..    
-0001e5f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0001e600: 2020 2020 2020 6478 3120 284e 756d 6265        dx1 (Numbe
-0001e610: 7229 3a20 6162 7363 6973 7361 206f 6620  r): abscissa of 
-0001e620: 7468 6520 6669 7273 7420 636f 6e74 726f  the first contro
-0001e630: 6c20 706f 696e 7420 7265 6c61 7469 7665  l point relative
-0001e640: 2074 6f20 7468 6520 656e 6420 706f 696e   to the end poin
-0001e650: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0001e660: 2020 6f66 2074 6865 2070 7265 7669 6f75    of the previou
-0001e670: 7320 7061 7468 2065 6c65 6d65 6e74 0a20  s path element. 
-0001e680: 2020 2020 2020 2020 2020 2064 7931 2028             dy1 (
-0001e690: 4e75 6d62 6572 293a 206f 7264 696e 6174  Number): ordinat
-0001e6a0: 6520 6f66 2074 6865 2066 6972 7374 2063  e of the first c
-0001e6b0: 6f6e 7472 6f6c 2070 6f69 6e74 2072 656c  ontrol point rel
-0001e6c0: 6174 6976 6520 746f 2074 6865 2065 6e64  ative to the end
-0001e6d0: 2070 6f69 6e74 0a20 2020 2020 2020 2020   point.         
-0001e6e0: 2020 2020 2020 206f 6620 7468 6520 7072         of the pr
-0001e6f0: 6576 696f 7573 2070 6174 6820 656c 656d  evious path elem
-0001e700: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-0001e710: 6478 3220 284e 756d 6265 7229 3a20 6162  dx2 (Number): ab
-0001e720: 7363 6973 7361 206f 6666 7365 7420 6f66  scissa offset of
-0001e730: 2074 6865 2073 6563 6f6e 6420 636f 6e74   the second cont
-0001e740: 726f 6c20 706f 696e 7420 7265 6c61 7469  rol point relati
-0001e750: 7665 2074 6f20 7468 650a 2020 2020 2020  ve to the.      
-0001e760: 2020 2020 2020 2020 2020 656e 6420 706f            end po
-0001e770: 696e 7420 6f66 2074 6865 2070 7265 7669  int of the previ
-0001e780: 6f75 7320 7061 7468 2065 6c65 6d65 6e74  ous path element
-0001e790: 0a20 2020 2020 2020 2020 2020 2064 7932  .            dy2
-0001e7a0: 2028 4e75 6d62 6572 293a 206f 7264 696e   (Number): ordin
-0001e7b0: 6174 6520 6f66 6673 6574 206f 6620 7468  ate offset of th
-0001e7c0: 6520 7365 636f 6e64 2063 6f6e 7472 6f6c  e second control
-0001e7d0: 2070 6f69 6e74 2072 656c 6174 6976 6520   point relative 
-0001e7e0: 746f 2074 6865 0a20 2020 2020 2020 2020  to the.         
-0001e7f0: 2020 2020 2020 2065 6e64 2070 6f69 6e74         end point
-0001e800: 206f 6620 7468 6520 7072 6576 696f 7573   of the previous
-0001e810: 2070 6174 6820 656c 656d 656e 740a 2020   path element.  
-0001e820: 2020 2020 2020 2020 2020 6478 3320 284e            dx3 (N
-0001e830: 756d 6265 7229 3a20 6162 7363 6973 7361  umber): abscissa
-0001e840: 206f 6666 7365 7420 6f66 2074 6865 2065   offset of the e
-0001e850: 6e64 2070 6f69 6e74 2072 656c 6174 6976  nd point relativ
-0001e860: 6520 746f 2074 6865 2065 6e64 2070 6f69  e to the end poi
-0001e870: 6e74 206f 660a 2020 2020 2020 2020 2020  nt of.          
-0001e880: 2020 2020 2020 7468 6520 7072 6576 696f        the previo
-0001e890: 7573 2070 6174 6820 656c 656d 656e 740a  us path element.
-0001e8a0: 2020 2020 2020 2020 2020 2020 6479 3320              dy3 
-0001e8b0: 284e 756d 6265 7229 3a20 6f72 6469 6e61  (Number): ordina
-0001e8c0: 7465 206f 6666 7365 7420 6f66 2074 6865  te offset of the
-0001e8d0: 2065 6e64 2070 6f69 6e74 2072 656c 6174   end point relat
-0001e8e0: 6976 6520 746f 2074 6865 2065 6e64 2070  ive to the end p
-0001e8f0: 6f69 6e74 206f 660a 2020 2020 2020 2020  oint of.        
-0001e900: 2020 2020 2020 2020 7468 6520 7072 6576          the prev
-0001e910: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
-0001e920: 740a 0a20 2020 2020 2020 2052 6574 7572  t..        Retur
-0001e930: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0001e940: 5468 6520 7061 7468 2c20 746f 2061 6c6c  The path, to all
-0001e950: 6f77 2063 6861 696e 696e 6720 6d65 7468  ow chaining meth
-0001e960: 6f64 2063 616c 6c73 2e0a 2020 2020 2020  od calls..      
-0001e970: 2020 2222 220a 2020 2020 2020 2020 6331    """.        c1
-0001e980: 6420 3d20 506f 696e 7428 6478 312c 2064  d = Point(dx1, d
-0001e990: 7931 290a 2020 2020 2020 2020 6332 6420  y1).        c2d 
-0001e9a0: 3d20 506f 696e 7428 6478 322c 2064 7932  = Point(dx2, dy2
-0001e9b0: 290a 2020 2020 2020 2020 656e 6420 3d20  ).        end = 
-0001e9c0: 506f 696e 7428 6478 332c 2064 7933 290a  Point(dx3, dy3).
-0001e9d0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-0001e9e0: 645f 7061 7468 5f65 6c65 6d65 6e74 2852  d_path_element(R
-0001e9f0: 656c 6174 6976 6542 657a 6965 7243 7572  elativeBezierCur
-0001ea00: 7665 2863 3164 2c20 6332 642c 2065 6e64  ve(c1d, c2d, end
-0001ea10: 292c 205f 636f 7079 3d46 616c 7365 290a  ), _copy=False).
-0001ea20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001ea30: 656c 660a 0a20 2020 2064 6566 2071 7561  elf..    def qua
-0001ea40: 6472 6174 6963 5f63 7572 7665 5f74 6f28  dratic_curve_to(
-0001ea50: 7365 6c66 2c20 7831 2c20 7931 2c20 7832  self, x1, y1, x2
-0001ea60: 2c20 7932 293a 0a20 2020 2020 2020 2022  , y2):.        "
-0001ea70: 2222 0a20 2020 2020 2020 2041 7070 656e  "".        Appen
-0001ea80: 6420 6120 6375 6269 6320 42c3 a97a 6965  d a cubic B..zie
-0001ea90: 7220 6375 7276 6520 6d69 6d69 636b 696e  r curve mimickin
-0001eaa0: 6720 7468 6520 7370 6563 6966 6965 6420  g the specified 
-0001eab0: 7175 6164 7261 7469 6320 42c3 a97a 6965  quadratic B..zie
-0001eac0: 7220 6375 7276 652e 0a0a 2020 2020 2020  r curve...      
-0001ead0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0001eae0: 2020 2020 7831 2028 4e75 6d62 6572 293a      x1 (Number):
-0001eaf0: 2061 6273 6369 7373 6120 6f66 2074 6865   abscissa of the
-0001eb00: 2063 6f6e 7472 6f6c 2070 6f69 6e74 0a20   control point. 
-0001eb10: 2020 2020 2020 2020 2020 2079 3120 284e             y1 (N
-0001eb20: 756d 6265 7229 3a20 6f72 6469 6e61 7465  umber): ordinate
-0001eb30: 206f 6620 7468 6520 636f 6e74 726f 6c20   of the control 
-0001eb40: 706f 696e 740a 2020 2020 2020 2020 2020  point.          
-0001eb50: 2020 7832 2028 4e75 6d62 6572 293a 2061    x2 (Number): a
-0001eb60: 6273 6369 7373 6120 6f66 2074 6865 2065  bscissa of the e
-0001eb70: 6e64 2070 6f69 6e74 0a20 2020 2020 2020  nd point.       
-0001eb80: 2020 2020 2079 3220 284e 756d 6265 7229       y2 (Number)
-0001eb90: 3a20 6f72 6469 6e61 7465 206f 6620 7468  : ordinate of th
-0001eba0: 6520 656e 6420 706f 696e 740a 0a20 2020  e end point..   
-0001ebb0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0001ebc0: 2020 2020 2020 2020 2020 5468 6520 7061            The pa
-0001ebd0: 7468 2c20 746f 2061 6c6c 6f77 2063 6861  th, to allow cha
-0001ebe0: 696e 696e 6720 6d65 7468 6f64 2063 616c  ining method cal
-0001ebf0: 6c73 2e0a 2020 2020 2020 2020 2222 220a  ls..        """.
-0001ec00: 2020 2020 2020 2020 6374 726c 203d 2050          ctrl = P
-0001ec10: 6f69 6e74 2878 312c 2079 3129 0a20 2020  oint(x1, y1).   
-0001ec20: 2020 2020 2065 6e64 203d 2050 6f69 6e74       end = Point
-0001ec30: 2878 322c 2079 3229 0a20 2020 2020 2020  (x2, y2).       
-0001ec40: 2073 656c 662e 6164 645f 7061 7468 5f65   self.add_path_e
-0001ec50: 6c65 6d65 6e74 2851 7561 6472 6174 6963  lement(Quadratic
-0001ec60: 4265 7a69 6572 4375 7276 6528 6374 726c  BezierCurve(ctrl
-0001ec70: 2c20 656e 6429 2c20 5f63 6f70 793d 4661  , end), _copy=Fa
-0001ec80: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
-0001ec90: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
-0001eca0: 6620 7175 6164 7261 7469 635f 6375 7276  f quadratic_curv
-0001ecb0: 655f 7265 6c61 7469 7665 2873 656c 662c  e_relative(self,
-0001ecc0: 2064 7831 2c20 6479 312c 2064 7832 2c20   dx1, dy1, dx2, 
-0001ecd0: 6479 3229 3a0a 2020 2020 2020 2020 2222  dy2):.        ""
-0001ece0: 220a 2020 2020 2020 2020 4170 7065 6e64  ".        Append
-0001ecf0: 2061 2063 7562 6963 2042 c3a9 7a69 6572   a cubic B..zier
-0001ed00: 2063 7572 7665 206d 696d 6963 6b69 6e67   curve mimicking
-0001ed10: 2074 6865 2073 7065 6369 6669 6564 2071   the specified q
-0001ed20: 7561 6472 6174 6963 2042 c3a9 7a69 6572  uadratic B..zier
-0001ed30: 2063 7572 7665 2e0a 0a20 2020 2020 2020   curve...       
-0001ed40: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0001ed50: 2020 2064 7831 2028 4e75 6d62 6572 293a     dx1 (Number):
-0001ed60: 2061 6273 6369 7373 6120 6f66 2074 6865   abscissa of the
-0001ed70: 2063 6f6e 7472 6f6c 2070 6f69 6e74 2072   control point r
-0001ed80: 656c 6174 6976 6520 746f 2074 6865 2065  elative to the e
-0001ed90: 6e64 2070 6f69 6e74 206f 660a 2020 2020  nd point of.    
-0001eda0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-0001edb0: 7072 6576 696f 7573 2070 6174 6820 656c  previous path el
-0001edc0: 656d 656e 740a 2020 2020 2020 2020 2020  ement.          
-0001edd0: 2020 6479 3120 284e 756d 6265 7229 3a20    dy1 (Number): 
-0001ede0: 6f72 6469 6e61 7465 206f 6620 7468 6520  ordinate of the 
-0001edf0: 636f 6e74 726f 6c20 706f 696e 7420 7265  control point re
-0001ee00: 6c61 7469 7665 2074 6f20 7468 6520 656e  lative to the en
-0001ee10: 6420 706f 696e 7420 6f66 0a20 2020 2020  d point of.     
-0001ee20: 2020 2020 2020 2020 2020 2074 6865 2070             the p
-0001ee30: 7265 7669 6f75 7320 7061 7468 2065 6c65  revious path ele
-0001ee40: 6d65 6e74 0a20 2020 2020 2020 2020 2020  ment.           
-0001ee50: 2064 7832 2028 4e75 6d62 6572 293a 2061   dx2 (Number): a
-0001ee60: 6273 6369 7373 6120 6f66 6673 6574 206f  bscissa offset o
-0001ee70: 6620 7468 6520 656e 6420 706f 696e 7420  f the end point 
-0001ee80: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
-0001ee90: 656e 6420 706f 696e 7420 6f66 0a20 2020  end point of.   
-0001eea0: 2020 2020 2020 2020 2020 2020 2074 6865               the
-0001eeb0: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
-0001eec0: 6c65 6d65 6e74 0a20 2020 2020 2020 2020  lement.         
-0001eed0: 2020 2064 7932 2028 4e75 6d62 6572 293a     dy2 (Number):
-0001eee0: 206f 7264 696e 6174 6520 6f66 6673 6574   ordinate offset
-0001eef0: 206f 6620 7468 6520 656e 6420 706f 696e   of the end poin
-0001ef00: 7420 7265 6c61 7469 7665 2074 6f20 7468  t relative to th
-0001ef10: 6520 656e 6420 706f 696e 7420 6f66 0a20  e end point of. 
-0001ef20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001ef30: 6865 2070 7265 7669 6f75 7320 7061 7468  he previous path
-0001ef40: 2065 6c65 6d65 6e74 0a0a 2020 2020 2020   element..      
-0001ef50: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0001ef60: 2020 2020 2020 2054 6865 2070 6174 682c         The path,
-0001ef70: 2074 6f20 616c 6c6f 7720 6368 6169 6e69   to allow chaini
-0001ef80: 6e67 206d 6574 686f 6420 6361 6c6c 732e  ng method calls.
-0001ef90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001efa0: 2020 2020 2063 7472 6c20 3d20 506f 696e       ctrl = Poin
-0001efb0: 7428 6478 312c 2064 7931 290a 2020 2020  t(dx1, dy1).    
-0001efc0: 2020 2020 656e 6420 3d20 506f 696e 7428      end = Point(
-0001efd0: 6478 322c 2064 7932 290a 2020 2020 2020  dx2, dy2).      
-0001efe0: 2020 7365 6c66 2e61 6464 5f70 6174 685f    self.add_path_
-0001eff0: 656c 656d 656e 7428 5265 6c61 7469 7665  element(Relative
-0001f000: 5175 6164 7261 7469 6342 657a 6965 7243  QuadraticBezierC
-0001f010: 7572 7665 2863 7472 6c2c 2065 6e64 292c  urve(ctrl, end),
-0001f020: 205f 636f 7079 3d46 616c 7365 290a 2020   _copy=False).  
-0001f030: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001f040: 660a 0a20 2020 2064 6566 2061 7263 5f74  f..    def arc_t
-0001f050: 6f28 7365 6c66 2c20 7278 2c20 7279 2c20  o(self, rx, ry, 
-0001f060: 726f 7461 7469 6f6e 2c20 6c61 7267 655f  rotation, large_
-0001f070: 6172 632c 2070 6f73 6974 6976 655f 7377  arc, positive_sw
-0001f080: 6565 702c 2078 2c20 7929 3a0a 2020 2020  eep, x, y):.    
-0001f090: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001f0a0: 4170 7065 6e64 2061 6e20 656c 6c69 7074  Append an ellipt
-0001f0b0: 6963 616c 2061 7263 2066 726f 6d20 7468  ical arc from th
-0001f0c0: 6520 656e 6420 6f66 2074 6865 2070 7265  e end of the pre
-0001f0d0: 7669 6f75 7320 7061 7468 2070 6f69 6e74  vious path point
-0001f0e0: 2074 6f20 7468 650a 2020 2020 2020 2020   to the.        
-0001f0f0: 7370 6563 6966 6965 6420 656e 6420 706f  specified end po
-0001f100: 696e 742e 0a0a 2020 2020 2020 2020 5468  int...        Th
-0001f110: 6520 6172 6320 6973 2061 7070 726f 7869  e arc is approxi
-0001f120: 6d61 7465 6420 7573 696e 6720 42c3 a97a  mated using B..z
-0001f130: 6965 7220 6375 7276 6573 2c20 736f 2069  ier curves, so i
-0001f140: 7420 6973 206e 6f74 2070 6572 6665 6374  t is not perfect
-0001f150: 6c79 2061 6363 7572 6174 652e 0a20 2020  ly accurate..   
-0001f160: 2020 2020 2048 6f77 6576 6572 2c20 7468       However, th
-0001f170: 6520 6572 726f 7220 6973 2073 6d61 6c6c  e error is small
-0001f180: 2065 6e6f 7567 6820 746f 206e 6f74 2062   enough to not b
-0001f190: 6520 6e6f 7469 6365 6162 6c65 2061 7420  e noticeable at 
-0001f1a0: 616e 7920 7265 6173 6f6e 6162 6c65 0a20  any reasonable. 
-0001f1b0: 2020 2020 2020 2028 616e 6420 6576 656e         (and even
-0001f1c0: 206d 6f73 7420 756e 7265 6173 6f6e 6162   most unreasonab
-0001f1d0: 6c65 2920 7363 616c 6573 2c20 7769 7468  le) scales, with
-0001f1e0: 2061 2077 6f72 7374 2d63 6173 6520 6465   a worst-case de
-0001f1f0: 7669 6174 696f 6e20 6f66 2061 726f 756e  viation of aroun
-0001f200: 6420 33e2 80b1 2e0a 0a20 2020 2020 2020  d 3......       
-0001f210: 204e 6f74 6573 3a0a 2020 2020 2020 2020   Notes:.        
-0001f220: 2020 2020 2d20 5468 6520 7369 676e 7320      - The signs 
-0001f230: 6f66 2074 6865 2072 6164 6969 2061 7267  of the radii arg
-0001f240: 756d 656e 7473 2028 6072 7860 2061 6e64  uments (`rx` and
-0001f250: 2060 7279 6029 2061 7265 2069 676e 6f72   `ry`) are ignor
-0001f260: 6564 2028 692e 652e 2074 6865 6972 0a20  ed (i.e. their. 
-0001f270: 2020 2020 2020 2020 2020 2020 2061 6273               abs
-0001f280: 6f6c 7574 6520 7661 6c75 6573 2061 7265  olute values are
-0001f290: 2075 7365 6420 696e 7374 6561 6429 2e0a   used instead)..
-0001f2a0: 2020 2020 2020 2020 2020 2020 2d20 4966              - If
-0001f2b0: 2065 6974 6865 7220 7261 6469 7573 2069   either radius i
-0001f2c0: 7320 302c 2074 6865 6e20 6120 7374 7261  s 0, then a stra
-0001f2d0: 6967 6874 206c 696e 6520 7769 6c6c 2062  ight line will b
-0001f2e0: 6520 656d 6974 7465 6420 696e 7374 6561  e emitted instea
-0001f2f0: 6420 6f66 2061 6e0a 2020 2020 2020 2020  d of an.        
-0001f300: 2020 2020 2020 6172 632e 0a20 2020 2020        arc..     
-0001f310: 2020 2020 2020 202d 2049 6620 7468 6520         - If the 
-0001f320: 7261 6469 6920 6172 6520 746f 6f20 736d  radii are too sm
-0001f330: 616c 6c20 666f 7220 7468 6520 6172 6320  all for the arc 
-0001f340: 746f 2072 6561 6368 2066 726f 6d20 7468  to reach from th
-0001f350: 6520 6375 7272 656e 7420 706f 696e 7420  e current point 
-0001f360: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
-0001f370: 2074 6865 2073 7065 6369 6669 6564 2065   the specified e
-0001f380: 6e64 2070 6f69 6e74 2028 6078 6020 616e  nd point (`x` an
-0001f390: 6420 6079 6029 2c20 7468 656e 2074 6865  d `y`), then the
-0001f3a0: 7920 7769 6c6c 2062 6520 7072 6f70 6f72  y will be propor
-0001f3b0: 7469 6f6e 616c 6c79 0a20 2020 2020 2020  tionally.       
-0001f3c0: 2020 2020 2020 2073 6361 6c65 6420 7570         scaled up
-0001f3d0: 2075 6e74 696c 2074 6865 7920 6172 6520   until they are 
-0001f3e0: 6269 6720 656e 6f75 6768 2c20 7768 6963  big enough, whic
-0001f3f0: 6820 7769 6c6c 2061 6c77 6179 7320 7265  h will always re
-0001f400: 7375 6c74 2069 6e20 610a 2020 2020 2020  sult in a.      
-0001f410: 2020 2020 2020 2020 6861 6c66 2d65 6c6c          half-ell
-0001f420: 6970 7365 2061 7263 2028 692e 652e 2061  ipse arc (i.e. a
-0001f430: 6e20 3138 3020 6465 6772 6565 2073 7765  n 180 degree swe
-0001f440: 6570 290a 0a20 2020 2020 2020 2041 7267  ep)..        Arg
-0001f450: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-0001f460: 7820 284e 756d 6265 7229 3a20 7261 6469  x (Number): radi
-0001f470: 7573 2069 6e20 7468 6520 782d 6469 7265  us in the x-dire
-0001f480: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
-0001f490: 2020 2072 7920 284e 756d 6265 7229 3a20     ry (Number): 
-0001f4a0: 7261 6469 7573 2069 6e20 7468 6520 792d  radius in the y-
-0001f4b0: 6469 7265 6374 696f 6e2e 0a20 2020 2020  direction..     
-0001f4c0: 2020 2020 2020 2072 6f74 6174 696f 6e20         rotation 
-0001f4d0: 284e 756d 6265 7229 3a20 616e 676c 6520  (Number): angle 
-0001f4e0: 2869 6e20 6465 6772 6565 7329 2074 6861  (in degrees) tha
-0001f4f0: 7420 7468 6520 6172 6320 7368 6f75 6c64  t the arc should
-0001f500: 2062 6520 726f 7461 7465 640a 2020 2020   be rotated.    
-0001f510: 2020 2020 2020 2020 2020 2020 636c 6f63              cloc
-0001f520: 6b77 6973 6520 6672 6f6d 2074 6865 2070  kwise from the p
-0001f530: 7269 6e63 6970 6c65 2061 7865 732e 2054  rinciple axes. T
-0001f540: 6869 7320 7061 7261 6d65 7465 7220 646f  his parameter do
-0001f550: 6573 206e 6f74 2068 6176 650a 2020 2020  es not have.    
-0001f560: 2020 2020 2020 2020 2020 2020 6120 7669              a vi
-0001f570: 7375 616c 2065 6666 6563 7420 696e 2074  sual effect in t
-0001f580: 6865 2063 6173 6520 7468 6174 2060 7278  he case that `rx
-0001f590: 203d 3d20 7279 602e 0a20 2020 2020 2020   == ry`..       
-0001f5a0: 2020 2020 206c 6172 6765 5f61 7263 2028       large_arc (
-0001f5b0: 626f 6f6c 293a 2069 6620 5472 7565 2c20  bool): if True, 
-0001f5c0: 7468 6520 6172 6320 7769 6c6c 2063 6f76  the arc will cov
-0001f5d0: 6572 2061 2073 7765 6570 2061 6e67 6c65  er a sweep angle
-0001f5e0: 206f 6620 6174 206c 6561 7374 2031 3830   of at least 180
-0001f5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f600: 2064 6567 7265 6573 2e20 4f74 6865 7277   degrees. Otherw
-0001f610: 6973 652c 2074 6865 2073 7765 6570 2061  ise, the sweep a
-0001f620: 6e67 6c65 2077 696c 6c20 6265 2061 7420  ngle will be at 
-0001f630: 6d6f 7374 2031 3830 2064 6567 7265 6573  most 180 degrees
-0001f640: 2e0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-0001f650: 7369 7469 7665 5f73 7765 6570 2028 626f  sitive_sweep (bo
-0001f660: 6f6c 293a 2069 6620 5472 7565 2c20 7468  ol): if True, th
-0001f670: 6520 6172 6320 7769 6c6c 2062 6520 7377  e arc will be sw
-0001f680: 6570 7420 6f76 6572 2061 2070 6f73 6974  ept over a posit
-0001f690: 6976 6520 616e 676c 652c 0a20 2020 2020  ive angle,.     
-0001f6a0: 2020 2020 2020 2020 2020 2069 2e65 2e20             i.e. 
-0001f6b0: 636c 6f63 6b77 6973 652e 204f 7468 6572  clockwise. Other
-0001f6c0: 7769 7365 2c20 7468 6520 6172 6320 7769  wise, the arc wi
-0001f6d0: 6c6c 2062 6520 7377 6570 7420 6f76 6572  ll be swept over
-0001f6e0: 2061 206e 6567 6174 6976 650a 2020 2020   a negative.    
-0001f6f0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
-0001f700: 652e 0a20 2020 2020 2020 2020 2020 2078  e..            x
-0001f710: 2028 4e75 6d62 6572 293a 2061 6273 6369   (Number): absci
-0001f720: 7373 6120 6f66 2074 6865 2061 7263 2773  ssa of the arc's
-0001f730: 2065 6e64 2070 6f69 6e74 2e0a 2020 2020   end point..    
-0001f740: 2020 2020 2020 2020 7920 284e 756d 6265          y (Numbe
-0001f750: 7229 3a20 6f72 6469 6e61 7465 206f 6620  r): ordinate of 
-0001f760: 7468 6520 6172 6327 7320 656e 6420 706f  the arc's end po
-0001f770: 696e 742e 0a20 2020 2020 2020 2022 2222  int..        """
-0001f780: 0a0a 2020 2020 2020 2020 6966 2072 7820  ..        if rx 
-0001f790: 3d3d 2030 206f 7220 7279 203d 3d20 303a  == 0 or ry == 0:
-0001f7a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001f7b0: 7572 6e20 7365 6c66 2e6c 696e 655f 746f  urn self.line_to
-0001f7c0: 2878 2c20 7929 0a0a 2020 2020 2020 2020  (x, y)..        
-0001f7d0: 7261 6469 6920 3d20 506f 696e 7428 6162  radii = Point(ab
-0001f7e0: 7328 7278 292c 2061 6273 2872 7929 290a  s(rx), abs(ry)).
-0001f7f0: 2020 2020 2020 2020 6c61 7267 655f 6172          large_ar
-0001f800: 6320 3d20 626f 6f6c 286c 6172 6765 5f61  c = bool(large_a
-0001f810: 7263 290a 2020 2020 2020 2020 726f 7461  rc).        rota
-0001f820: 7469 6f6e 203d 206d 6174 682e 7261 6469  tion = math.radi
-0001f830: 616e 7328 726f 7461 7469 6f6e 290a 2020  ans(rotation).  
-0001f840: 2020 2020 2020 706f 7369 7469 7665 5f73        positive_s
-0001f850: 7765 6570 203d 2062 6f6f 6c28 706f 7369  weep = bool(posi
-0001f860: 7469 7665 5f73 7765 6570 290a 2020 2020  tive_sweep).    
-0001f870: 2020 2020 656e 6420 3d20 506f 696e 7428      end = Point(
-0001f880: 782c 2079 290a 0a20 2020 2020 2020 2073  x, y)..        s
-0001f890: 656c 662e 6164 645f 7061 7468 5f65 6c65  elf.add_path_ele
-0001f8a0: 6d65 6e74 280a 2020 2020 2020 2020 2020  ment(.          
-0001f8b0: 2020 4172 6328 7261 6469 692c 2072 6f74    Arc(radii, rot
-0001f8c0: 6174 696f 6e2c 206c 6172 6765 5f61 7263  ation, large_arc
-0001f8d0: 2c20 706f 7369 7469 7665 5f73 7765 6570  , positive_sweep
-0001f8e0: 2c20 656e 6429 2c20 5f63 6f70 793d 4661  , end), _copy=Fa
-0001f8f0: 6c73 650a 2020 2020 2020 2020 290a 2020  lse.        ).  
-0001f900: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001f910: 660a 0a20 2020 2064 6566 2061 7263 5f72  f..    def arc_r
-0001f920: 656c 6174 6976 6528 7365 6c66 2c20 7278  elative(self, rx
-0001f930: 2c20 7279 2c20 726f 7461 7469 6f6e 2c20  , ry, rotation, 
-0001f940: 6c61 7267 655f 6172 632c 2070 6f73 6974  large_arc, posit
-0001f950: 6976 655f 7377 6565 702c 2064 782c 2064  ive_sweep, dx, d
-0001f960: 7929 3a0a 2020 2020 2020 2020 2222 220a  y):.        """.
-0001f970: 2020 2020 2020 2020 4170 7065 6e64 2061          Append a
-0001f980: 6e20 656c 6c69 7074 6963 616c 2061 7263  n elliptical arc
-0001f990: 2066 726f 6d20 7468 6520 656e 6420 6f66   from the end of
-0001f9a0: 2074 6865 2070 7265 7669 6f75 7320 7061   the previous pa
-0001f9b0: 7468 2070 6f69 6e74 2074 6f20 616e 206f  th point to an o
-0001f9c0: 6666 7365 740a 2020 2020 2020 2020 706f  ffset.        po
-0001f9d0: 696e 742e 0a0a 2020 2020 2020 2020 5468  int...        Th
-0001f9e0: 6520 6172 6320 6973 2061 7070 726f 7869  e arc is approxi
-0001f9f0: 6d61 7465 6420 7573 696e 6720 42c3 a97a  mated using B..z
-0001fa00: 6965 7220 6375 7276 6573 2c20 736f 2069  ier curves, so i
-0001fa10: 7420 6973 206e 6f74 2070 6572 6665 6374  t is not perfect
-0001fa20: 6c79 2061 6363 7572 6174 652e 0a20 2020  ly accurate..   
-0001fa30: 2020 2020 2048 6f77 6576 6572 2c20 7468       However, th
-0001fa40: 6520 6572 726f 7220 6973 2073 6d61 6c6c  e error is small
-0001fa50: 2065 6e6f 7567 6820 746f 206e 6f74 2062   enough to not b
-0001fa60: 6520 6e6f 7469 6365 6162 6c65 2061 7420  e noticeable at 
-0001fa70: 616e 7920 7265 6173 6f6e 6162 6c65 0a20  any reasonable. 
-0001fa80: 2020 2020 2020 2028 616e 6420 6576 656e         (and even
-0001fa90: 206d 6f73 7420 756e 7265 6173 6f6e 6162   most unreasonab
-0001faa0: 6c65 2920 7363 616c 6573 2c20 7769 7468  le) scales, with
-0001fab0: 2061 2077 6f72 7374 2d63 6173 6520 6465   a worst-case de
-0001fac0: 7669 6174 696f 6e20 6f66 2061 726f 756e  viation of aroun
-0001fad0: 6420 33e2 80b1 2e0a 0a20 2020 2020 2020  d 3......       
-0001fae0: 204e 6f74 6573 3a0a 2020 2020 2020 2020   Notes:.        
-0001faf0: 2020 2020 2d20 5468 6520 7369 676e 7320      - The signs 
-0001fb00: 6f66 2074 6865 2072 6164 6969 2061 7267  of the radii arg
-0001fb10: 756d 656e 7473 2028 6072 7860 2061 6e64  uments (`rx` and
-0001fb20: 2060 7279 6029 2061 7265 2069 676e 6f72   `ry`) are ignor
-0001fb30: 6564 2028 692e 652e 2074 6865 6972 0a20  ed (i.e. their. 
-0001fb40: 2020 2020 2020 2020 2020 2020 2061 6273               abs
-0001fb50: 6f6c 7574 6520 7661 6c75 6573 2061 7265  olute values are
-0001fb60: 2075 7365 6420 696e 7374 6561 6429 2e0a   used instead)..
-0001fb70: 2020 2020 2020 2020 2020 2020 2d20 4966              - If
-0001fb80: 2065 6974 6865 7220 7261 6469 7573 2069   either radius i
-0001fb90: 7320 302c 2074 6865 6e20 6120 7374 7261  s 0, then a stra
-0001fba0: 6967 6874 206c 696e 6520 7769 6c6c 2062  ight line will b
-0001fbb0: 6520 656d 6974 7465 6420 696e 7374 6561  e emitted instea
-0001fbc0: 6420 6f66 2061 6e0a 2020 2020 2020 2020  d of an.        
-0001fbd0: 2020 2020 2020 6172 632e 0a20 2020 2020        arc..     
-0001fbe0: 2020 2020 2020 202d 2049 6620 7468 6520         - If the 
-0001fbf0: 7261 6469 6920 6172 6520 746f 6f20 736d  radii are too sm
-0001fc00: 616c 6c20 666f 7220 7468 6520 6172 6320  all for the arc 
-0001fc10: 746f 2072 6561 6368 2066 726f 6d20 7468  to reach from th
-0001fc20: 6520 6375 7272 656e 7420 706f 696e 7420  e current point 
-0001fc30: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
-0001fc40: 2074 6865 2073 7065 6369 6669 6564 2065   the specified e
-0001fc50: 6e64 2070 6f69 6e74 2028 6078 6020 616e  nd point (`x` an
-0001fc60: 6420 6079 6029 2c20 7468 656e 2074 6865  d `y`), then the
-0001fc70: 7920 7769 6c6c 2062 6520 7072 6f70 6f72  y will be propor
-0001fc80: 7469 6f6e 616c 6c79 0a20 2020 2020 2020  tionally.       
-0001fc90: 2020 2020 2020 2073 6361 6c65 6420 7570         scaled up
-0001fca0: 2075 6e74 696c 2074 6865 7920 6172 6520   until they are 
-0001fcb0: 6269 6720 656e 6f75 6768 2c20 7768 6963  big enough, whic
-0001fcc0: 6820 7769 6c6c 2061 6c77 6179 7320 7265  h will always re
-0001fcd0: 7375 6c74 2069 6e20 610a 2020 2020 2020  sult in a.      
-0001fce0: 2020 2020 2020 2020 6861 6c66 2d65 6c6c          half-ell
-0001fcf0: 6970 7365 2061 7263 2028 692e 652e 2061  ipse arc (i.e. a
-0001fd00: 6e20 3138 3020 6465 6772 6565 2073 7765  n 180 degree swe
-0001fd10: 6570 290a 0a20 2020 2020 2020 2041 7267  ep)..        Arg
-0001fd20: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-0001fd30: 7820 284e 756d 6265 7229 3a20 7261 6469  x (Number): radi
-0001fd40: 7573 2069 6e20 7468 6520 782d 6469 7265  us in the x-dire
-0001fd50: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
-0001fd60: 2020 2072 7920 284e 756d 6265 7229 3a20     ry (Number): 
-0001fd70: 7261 6469 7573 2069 6e20 7468 6520 792d  radius in the y-
-0001fd80: 6469 7265 6374 696f 6e2e 0a20 2020 2020  direction..     
-0001fd90: 2020 2020 2020 2072 6f74 6174 696f 6e20         rotation 
-0001fda0: 284e 756d 6265 7229 3a20 616e 676c 6520  (Number): angle 
-0001fdb0: 2869 6e20 6465 6772 6565 7329 2074 6861  (in degrees) tha
-0001fdc0: 7420 7468 6520 6172 6320 7368 6f75 6c64  t the arc should
-0001fdd0: 2062 6520 726f 7461 7465 640a 2020 2020   be rotated.    
-0001fde0: 2020 2020 2020 2020 2020 2020 636c 6f63              cloc
-0001fdf0: 6b77 6973 6520 6672 6f6d 2074 6865 2070  kwise from the p
-0001fe00: 7269 6e63 6970 6c65 2061 7865 732e 2054  rinciple axes. T
-0001fe10: 6869 7320 7061 7261 6d65 7465 7220 646f  his parameter do
-0001fe20: 6573 206e 6f74 2068 6176 650a 2020 2020  es not have.    
-0001fe30: 2020 2020 2020 2020 2020 2020 6120 7669              a vi
-0001fe40: 7375 616c 2065 6666 6563 7420 696e 2074  sual effect in t
-0001fe50: 6865 2063 6173 6520 7468 6174 2060 7278  he case that `rx
-0001fe60: 203d 3d20 7279 602e 0a20 2020 2020 2020   == ry`..       
-0001fe70: 2020 2020 206c 6172 6765 5f61 7263 2028       large_arc (
-0001fe80: 626f 6f6c 293a 2069 6620 5472 7565 2c20  bool): if True, 
-0001fe90: 7468 6520 6172 6320 7769 6c6c 2063 6f76  the arc will cov
-0001fea0: 6572 2061 2073 7765 6570 2061 6e67 6c65  er a sweep angle
-0001feb0: 206f 6620 6174 206c 6561 7374 2031 3830   of at least 180
-0001fec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fed0: 2064 6567 7265 6573 2e20 4f74 6865 7277   degrees. Otherw
-0001fee0: 6973 652c 2074 6865 2073 7765 6570 2061  ise, the sweep a
-0001fef0: 6e67 6c65 2077 696c 6c20 6265 2061 7420  ngle will be at 
-0001ff00: 6d6f 7374 2031 3830 2064 6567 7265 6573  most 180 degrees
-0001ff10: 2e0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-0001ff20: 7369 7469 7665 5f73 7765 6570 2028 626f  sitive_sweep (bo
-0001ff30: 6f6c 293a 2069 6620 5472 7565 2c20 7468  ol): if True, th
-0001ff40: 6520 6172 6320 7769 6c6c 2062 6520 7377  e arc will be sw
-0001ff50: 6570 7420 6f76 6572 2061 2070 6f73 6974  ept over a posit
-0001ff60: 6976 6520 616e 676c 652c 0a20 2020 2020  ive angle,.     
-0001ff70: 2020 2020 2020 2020 2020 2069 2e65 2e20             i.e. 
-0001ff80: 636c 6f63 6b77 6973 652e 204f 7468 6572  clockwise. Other
-0001ff90: 7769 7365 2c20 7468 6520 6172 6320 7769  wise, the arc wi
-0001ffa0: 6c6c 2062 6520 7377 6570 7420 6f76 6572  ll be swept over
-0001ffb0: 2061 206e 6567 6174 6976 650a 2020 2020   a negative.    
-0001ffc0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
-0001ffd0: 652e 0a20 2020 2020 2020 2020 2020 2064  e..            d
-0001ffe0: 7820 284e 756d 6265 7229 3a20 6162 7363  x (Number): absc
-0001fff0: 6973 7361 206f 6620 7468 6520 6172 6327  issa of the arc'
-00020000: 7320 656e 6420 706f 696e 7420 7265 6c61  s end point rela
-00020010: 7469 7665 2074 6f20 7468 6520 656e 6420  tive to the end 
-00020020: 706f 696e 7420 6f66 0a20 2020 2020 2020  point of.       
-00020030: 2020 2020 2020 2020 2074 6865 2070 7265           the pre
-00020040: 7669 6f75 7320 7061 7468 2065 6c65 6d65  vious path eleme
-00020050: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
-00020060: 6479 2028 4e75 6d62 6572 293a 206f 7264  dy (Number): ord
-00020070: 696e 6174 6520 6f66 2074 6865 2061 7263  inate of the arc
-00020080: 2773 2065 6e64 2070 6f69 6e74 2072 656c  's end point rel
-00020090: 6174 6976 6520 746f 2074 6865 2065 6e64  ative to the end
-000200a0: 2070 6f69 6e74 206f 660a 2020 2020 2020   point of.      
-000200b0: 2020 2020 2020 2020 2020 7468 6520 7072            the pr
-000200c0: 6576 696f 7573 2070 6174 6820 656c 656d  evious path elem
-000200d0: 656e 742e 0a20 2020 2020 2020 2022 2222  ent..        """
-000200e0: 0a20 2020 2020 2020 2069 6620 7278 203d  .        if rx =
-000200f0: 3d20 3020 6f72 2072 7920 3d3d 2030 3a0a  = 0 or ry == 0:.
-00020100: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00020110: 726e 2073 656c 662e 6c69 6e65 5f72 656c  rn self.line_rel
-00020120: 6174 6976 6528 6478 2c20 6479 290a 0a20  ative(dx, dy).. 
-00020130: 2020 2020 2020 2072 6164 6969 203d 2050         radii = P
-00020140: 6f69 6e74 2861 6273 2872 7829 2c20 6162  oint(abs(rx), ab
-00020150: 7328 7279 2929 0a20 2020 2020 2020 206c  s(ry)).        l
-00020160: 6172 6765 5f61 7263 203d 2062 6f6f 6c28  arge_arc = bool(
-00020170: 6c61 7267 655f 6172 6329 0a20 2020 2020  large_arc).     
-00020180: 2020 2072 6f74 6174 696f 6e20 3d20 6d61     rotation = ma
-00020190: 7468 2e72 6164 6961 6e73 2872 6f74 6174  th.radians(rotat
-000201a0: 696f 6e29 0a20 2020 2020 2020 2070 6f73  ion).        pos
-000201b0: 6974 6976 655f 7377 6565 7020 3d20 626f  itive_sweep = bo
-000201c0: 6f6c 2870 6f73 6974 6976 655f 7377 6565  ol(positive_swee
-000201d0: 7029 0a20 2020 2020 2020 2065 6e64 203d  p).        end =
-000201e0: 2050 6f69 6e74 2864 782c 2064 7929 0a0a   Point(dx, dy)..
-000201f0: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-00020200: 5f70 6174 685f 656c 656d 656e 7428 0a20  _path_element(. 
-00020210: 2020 2020 2020 2020 2020 2052 656c 6174             Relat
-00020220: 6976 6541 7263 2872 6164 6969 2c20 726f  iveArc(radii, ro
-00020230: 7461 7469 6f6e 2c20 6c61 7267 655f 6172  tation, large_ar
-00020240: 632c 2070 6f73 6974 6976 655f 7377 6565  c, positive_swee
-00020250: 702c 2065 6e64 292c 205f 636f 7079 3d46  p, end), _copy=F
-00020260: 616c 7365 0a20 2020 2020 2020 2029 0a20  alse.        ). 
-00020270: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00020280: 6c66 0a0a 2020 2020 6465 6620 636c 6f73  lf..    def clos
-00020290: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000202a0: 2022 2222 0a20 2020 2020 2020 2045 7870   """.        Exp
-000202b0: 6c69 6369 746c 7920 636c 6f73 6520 7468  licitly close th
-000202c0: 6520 6375 7272 656e 7420 2873 7562 2970  e current (sub)p
-000202d0: 6174 682e 0a20 2020 2020 2020 2022 2222  ath..        """
-000202e0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-000202f0: 645f 7061 7468 5f65 6c65 6d65 6e74 2843  d_path_element(C
-00020300: 6c6f 7365 2829 2c20 5f63 6f70 793d 4661  lose(), _copy=Fa
-00020310: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
-00020320: 662e 5f63 6c6f 7365 6420 3d20 5472 7565  f._closed = True
-00020330: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-00020340: 7665 5f72 656c 6174 6976 6528 302c 2030  ve_relative(0, 0
-00020350: 290a 0a20 2020 2064 6566 205f 696e 7365  )..    def _inse
-00020360: 7274 5f69 6d70 6c69 6369 745f 636c 6f73  rt_implicit_clos
-00020370: 655f 6966 5f6f 7065 6e28 7365 6c66 293a  e_if_open(self):
-00020380: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00020390: 7365 6c66 2e5f 636c 6f73 6564 3a0a 2020  self._closed:.  
-000203a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000203b0: 636c 6f73 655f 636f 6e74 6578 742e 6164  close_context.ad
-000203c0: 645f 6974 656d 2849 6d70 6c69 6369 7443  d_item(ImplicitC
-000203d0: 6c6f 7365 2829 2c20 5f63 6f70 793d 4661  lose(), _copy=Fa
-000203e0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-000203f0: 2073 656c 662e 5f63 6c6f 7365 5f63 6f6e   self._close_con
-00020400: 7465 7874 203d 2073 656c 662e 5f67 7261  text = self._gra
-00020410: 7068 6963 735f 636f 6e74 6578 740a 2020  phics_context.  
-00020420: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00020430: 636c 6f73 6564 203d 2054 7275 650a 0a20  closed = True.. 
-00020440: 2020 2064 6566 2072 656e 6465 7228 0a20     def render(. 
-00020450: 2020 2020 2020 2073 656c 662c 2067 7364         self, gsd
-00020460: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
-00020470: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
-00020480: 7469 616c 5f70 6f69 6e74 2c20 6465 6275  tial_point, debu
-00020490: 675f 7374 7265 616d 3d4e 6f6e 652c 2070  g_stream=None, p
-000204a0: 6678 3d4e 6f6e 650a 2020 2020 293a 0a20  fx=None.    ):. 
-000204b0: 2020 2020 2020 2073 656c 662e 5f69 6e73         self._ins
-000204c0: 6572 745f 696d 706c 6963 6974 5f63 6c6f  ert_implicit_clo
-000204d0: 7365 5f69 665f 6f70 656e 2829 0a0a 2020  se_if_open()..  
-000204e0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-000204f0: 2020 2020 7265 6e64 6572 5f6c 6973 742c      render_list,
-00020500: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
-00020510: 745f 6974 656d 2c0a 2020 2020 2020 2020  t_item,.        
-00020520: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
-00020530: 742c 0a20 2020 2020 2020 2029 203d 2073  t,.        ) = s
-00020540: 656c 662e 5f72 6f6f 745f 6772 6170 6869  elf._root_graphi
-00020550: 6373 5f63 6f6e 7465 7874 2e62 7569 6c64  cs_context.build
-00020560: 5f72 656e 6465 725f 6c69 7374 280a 2020  _render_list(.  
-00020570: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-00020580: 6769 7374 7279 2c20 7374 796c 652c 206c  gistry, style, l
-00020590: 6173 745f 6974 656d 2c20 696e 6974 6961  ast_item, initia
-000205a0: 6c5f 706f 696e 742c 2064 6562 7567 5f73  l_point, debug_s
-000205b0: 7472 6561 6d2c 2070 6678 0a20 2020 2020  tream, pfx.     
-000205c0: 2020 2029 0a0a 2020 2020 2020 2020 7061     )..        pa
-000205d0: 696e 745f 7275 6c65 203d 2047 7261 7068  int_rule = Graph
-000205e0: 6963 7353 7479 6c65 2e6d 6572 6765 2873  icsStyle.merge(s
-000205f0: 7479 6c65 2c20 7365 6c66 2e73 7479 6c65  tyle, self.style
-00020600: 292e 7265 736f 6c76 655f 7061 696e 745f  ).resolve_paint_
-00020610: 7275 6c65 2829 0a0a 2020 2020 2020 2020  rule()..        
-00020620: 7265 6e64 6572 5f6c 6973 742e 696e 7365  render_list.inse
-00020630: 7274 282d 312c 2070 6169 6e74 5f72 756c  rt(-1, paint_rul
-00020640: 652e 7661 6c75 6529 0a0a 2020 2020 2020  e.value)..      
-00020650: 2020 7265 7475 726e 2022 2022 2e6a 6f69    return " ".joi
-00020660: 6e28 7265 6e64 6572 5f6c 6973 7429 2c20  n(render_list), 
-00020670: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
-00020680: 616c 5f70 6f69 6e74 0a0a 2020 2020 6465  al_point..    de
-00020690: 6620 7265 6e64 6572 5f64 6562 7567 280a  f render_debug(.
-000206a0: 2020 2020 2020 2020 7365 6c66 2c20 6773          self, gs
-000206b0: 645f 7265 6769 7374 7279 2c20 7374 796c  d_registry, styl
-000206c0: 652c 206c 6173 745f 6974 656d 2c20 696e  e, last_item, in
-000206d0: 6974 6961 6c5f 706f 696e 742c 2064 6562  itial_point, deb
-000206e0: 7567 5f73 7472 6561 6d2c 2070 6678 0a20  ug_stream, pfx. 
-000206f0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00020700: 220a 2020 2020 2020 2020 5265 6e64 6572  ".        Render
-00020710: 2074 6869 7320 7061 7468 2065 6c65 6d65   this path eleme
-00020720: 6e74 2074 6f20 6974 7320 5044 4620 7265  nt to its PDF re
-00020730: 7072 6573 656e 7461 7469 6f6e 2061 6e64  presentation and
-00020740: 2070 726f 6475 6365 2064 6562 7567 0a20   produce debug. 
-00020750: 2020 2020 2020 2069 6e66 6f72 6d61 7469         informati
-00020760: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
-00020770: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
-00020780: 7364 5f72 6567 6973 7472 7920 2847 7261  sd_registry (Gra
-00020790: 7068 6963 7353 7461 7465 4469 6374 5265  phicsStateDictRe
-000207a0: 6769 7374 7279 293a 2074 6865 206f 776e  gistry): the own
-000207b0: 6572 2773 2067 7261 7068 6963 7320 7374  er's graphics st
-000207c0: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
-000207d0: 2020 2020 6469 6374 696f 6e61 7279 2072      dictionary r
-000207e0: 6567 6973 7472 792e 0a20 2020 2020 2020  egistry..       
-000207f0: 2020 2020 2073 7479 6c65 2028 4772 6170       style (Grap
-00020800: 6869 6373 5374 796c 6529 3a20 7468 6520  hicsStyle): the 
-00020810: 6375 7272 656e 7420 7265 736f 6c76 6564  current resolved
-00020820: 2067 7261 7068 6963 7320 7374 796c 650a   graphics style.
-00020830: 2020 2020 2020 2020 2020 2020 6c61 7374              last
-00020840: 5f69 7465 6d3a 2074 6865 2070 7265 7669  _item: the previ
-00020850: 6f75 7320 7061 7468 2065 6c65 6d65 6e74  ous path element
-00020860: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00020870: 6974 6961 6c5f 706f 696e 743a 206c 6173  itial_point: las
-00020880: 7420 706f 7369 7469 6f6e 2073 6574 2062  t position set b
-00020890: 7920 6120 224d 2220 6f72 2022 6d22 2063  y a "M" or "m" c
-000208a0: 6f6d 6d61 6e64 0a20 2020 2020 2020 2020  ommand.         
-000208b0: 2020 2064 6562 7567 5f73 7472 6561 6d20     debug_stream 
-000208c0: 2869 6f2e 5465 7874 494f 293a 2074 6865  (io.TextIO): the
-000208d0: 2073 7472 6561 6d20 746f 2077 6869 6368   stream to which
-000208e0: 2074 6865 2064 6562 7567 206f 7574 7075   the debug outpu
-000208f0: 7420 7368 6f75 6c64 2062 650a 2020 2020  t should be.    
-00020900: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-00020910: 7465 6e2e 2054 6869 7320 6973 206e 6f74  ten. This is not
-00020920: 2067 7561 7261 6e74 6565 6420 746f 2062   guaranteed to b
-00020930: 6520 7365 656b 6162 6c65 2028 652e 672e  e seekable (e.g.
-00020940: 2069 7420 6d61 7920 6265 2073 7464 6f75   it may be stdou
-00020950: 7420 6f72 0a20 2020 2020 2020 2020 2020  t or.           
-00020960: 2020 2020 2073 7464 6572 7229 2e0a 2020       stderr)..  
-00020970: 2020 2020 2020 2020 2020 7066 7820 2873            pfx (s
-00020980: 7472 293a 2074 6865 2063 7572 7265 6e74  tr): the current
-00020990: 2064 6562 7567 206f 7574 7075 7420 7072   debug output pr
-000209a0: 6566 6978 2073 7472 696e 6720 286f 6e6c  efix string (onl
-000209b0: 7920 6e65 6564 6564 2069 6620 656d 6974  y needed if emit
-000209c0: 7469 6e67 0a20 2020 2020 2020 2020 2020  ting.           
-000209d0: 2020 2020 206d 6f72 6520 7468 616e 206f       more than o
-000209e0: 6e65 206c 696e 6529 2e0a 0a20 2020 2020  ne line)...     
-000209f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00020a00: 2020 2020 2020 2020 5468 6520 7361 6d65          The same
-00020a10: 2074 7570 6c65 2061 7320 6050 6169 6e74   tuple as `Paint
-00020a20: 6564 5061 7468 2e72 656e 6465 7260 2e0a  edPath.render`..
-00020a30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00020a40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00020a50: 7265 6e64 6572 280a 2020 2020 2020 2020  render(.        
-00020a60: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
-00020a70: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
-00020a80: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
-00020a90: 742c 2064 6562 7567 5f73 7472 6561 6d2c  t, debug_stream,
-00020aa0: 2070 6678 0a20 2020 2020 2020 2029 0a0a   pfx.        )..
-00020ab0: 0a63 6c61 7373 2043 6c69 7070 696e 6750  .class ClippingP
-00020ac0: 6174 6828 5061 696e 7465 6450 6174 6829  ath(PaintedPath)
-00020ad0: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-00020ae0: 6520 5061 696e 7465 6450 6174 6820 4150  e PaintedPath AP
-00020af0: 4920 6275 7420 746f 2062 6520 7573 6564  I but to be used
-00020b00: 2074 6f20 6372 6561 7465 2063 6c69 7070   to create clipp
-00020b10: 696e 6720 7061 7468 732e 0a0a 2020 2020  ing paths...    
-00020b20: 2e2e 2077 6172 6e69 6e67 3a3a 0a20 2020  .. warning::.   
-00020b30: 2020 2020 2055 6e6c 6573 7320 796f 7520       Unless you 
-00020b40: 7265 616c 6c79 206b 6e6f 7720 7768 6174  really know what
-00020b50: 2079 6f75 2772 6520 646f 696e 672c 2063   you're doing, c
-00020b60: 6861 6e67 696e 6720 6174 7472 6962 7574  hanging attribut
-00020b70: 6573 206f 6620 7468 6520 636c 6970 7069  es of the clippi
-00020b80: 6e67 0a20 2020 2020 2020 2070 6174 6820  ng.        path 
-00020b90: 7374 796c 6520 6973 206c 696b 656c 7920  style is likely 
-00020ba0: 746f 2070 726f 6475 6365 2075 6e65 7870  to produce unexp
-00020bb0: 6563 7465 6420 7265 7375 6c74 732e 2054  ected results. T
-00020bc0: 6869 7320 6973 2062 6563 6175 7365 2074  his is because t
-00020bd0: 6865 0a20 2020 2020 2020 2063 6c69 7070  he.        clipp
-00020be0: 696e 6720 7061 7468 2073 7479 6c65 7320  ing path styles 
-00020bf0: 6f76 6572 7269 6465 2069 6d70 6c69 6369  override implici
-00020c00: 7420 7374 796c 6520 696e 6865 7269 7461  t style inherita
-00020c10: 6e63 6520 6f66 2074 6865 2060 5061 696e  nce of the `Pain
-00020c20: 7465 6450 6174 6860 0a20 2020 2020 2020  tedPath`.       
-00020c30: 2069 7420 6170 706c 6965 7320 746f 2e0a   it applies to..
-00020c40: 0a20 2020 2020 2020 2046 6f72 2065 7861  .        For exa
-00020c50: 6d70 6c65 2c20 6063 6c69 7070 6174 682e  mple, `clippath.
-00020c60: 7374 796c 652e 7374 726f 6b65 5f77 6964  style.stroke_wid
-00020c70: 7468 203d 2032 6020 6361 6e20 756e 6578  th = 2` can unex
-00020c80: 7065 6374 6564 6c79 206f 7665 7272 6964  pectedly overrid
-00020c90: 650a 2020 2020 2020 2020 6070 6169 6e74  e.        `paint
-00020ca0: 7061 7468 2e73 7479 6c65 2e73 7472 6f6b  path.style.strok
-00020cb0: 655f 7769 6474 6820 3d20 4772 6170 6869  e_width = Graphi
-00020cc0: 6373 5374 796c 652e 494e 4845 5249 5460  csStyle.INHERIT`
-00020cd0: 2061 6e64 2063 6175 7365 2074 6865 2070   and cause the p
-00020ce0: 6169 6e74 6564 0a20 2020 2020 2020 2070  ainted.        p
-00020cf0: 6174 6820 746f 2062 6520 7265 6e64 6572  ath to be render
-00020d00: 6564 2077 6974 6820 6120 7374 726f 6b65  ed with a stroke
-00020d10: 206f 6620 3220 696e 7374 6561 6420 6f66   of 2 instead of
-00020d20: 2077 6861 7420 6974 2077 6f75 6c64 2068   what it would h
-00020d30: 6176 6520 6e6f 726d 616c 6c79 0a20 2020  ave normally.   
-00020d40: 2020 2020 2069 6e68 6572 6974 6564 2e20       inherited. 
-00020d50: 4265 6361 7573 6520 6120 6043 6c69 7070  Because a `Clipp
-00020d60: 696e 6750 6174 6860 2063 616e 2062 6520  ingPath` can be 
-00020d70: 7061 696e 7465 6420 6c69 6b65 2061 206e  painted like a n
-00020d80: 6f72 6d61 6c20 6050 6169 6e74 6564 5061  ormal `PaintedPa
-00020d90: 7468 602c 0a20 2020 2020 2020 2069 7420  th`,.        it 
-00020da0: 776f 756c 6420 6265 206f 7665 726c 7920  would be overly 
-00020db0: 7265 7374 7269 6374 6976 6520 746f 2072  restrictive to r
-00020dc0: 656d 6f76 6520 7468 6520 6162 696c 6974  emove the abilit
-00020dd0: 7920 746f 2073 7479 6c65 2069 742c 2073  y to style it, s
-00020de0: 6f20 696e 7374 6561 640a 2020 2020 2020  o instead.      
-00020df0: 2020 7468 6973 2077 6172 6e69 6e67 2069    this warning i
-00020e00: 7320 6865 7265 2e0a 2020 2020 2222 220a  s here..    """.
-00020e10: 0a20 2020 2023 2062 6563 6175 7365 2063  .    # because c
-00020e20: 6c69 7070 696e 6720 7061 7468 7320 6361  lipping paths ca
-00020e30: 6e20 6265 2070 6169 6e74 6564 2c20 7765  n be painted, we
-00020e40: 2069 6e68 6572 6974 2066 726f 6d20 5061   inherit from Pa
-00020e50: 696e 7465 6450 6174 682e 2048 6f77 6576  intedPath. Howev
-00020e60: 6572 2c20 7768 656e 0a20 2020 2023 2073  er, when.    # s
-00020e70: 6574 7469 6e67 2074 6865 2073 7479 6c69  etting the styli
-00020e80: 6e67 206f 6e20 7468 6520 636c 6970 7069  ng on the clippi
-00020e90: 6e67 2070 6174 682c 2074 686f 7365 2076  ng path, those v
-00020ea0: 616c 7565 7320 7769 6c6c 2061 6c73 6f20  alues will also 
-00020eb0: 6265 2061 7070 6c69 6564 2074 6f0a 2020  be applied to.  
-00020ec0: 2020 2320 7468 6520 5061 696e 7465 6450    # the PaintedP
-00020ed0: 6174 6820 7468 6520 436c 6970 7069 6e67  ath the Clipping
-00020ee0: 5061 7468 2069 7320 6170 706c 6965 6420  Path is applied 
-00020ef0: 746f 2075 6e6c 6573 7320 7468 6579 2061  to unless they a
-00020f00: 7265 2065 7870 6c69 6369 746c 7920 7365  re explicitly se
-00020f10: 7420 666f 720a 2020 2020 2320 7468 6174  t for.    # that
-00020f20: 2070 6169 6e74 6564 2070 6174 682e 2054   painted path. T
-00020f30: 6869 7320 6973 206e 6f74 2069 6465 616c  his is not ideal
-00020f40: 2c20 6275 7420 7468 6572 6527 7320 6e6f  , but there's no
-00020f50: 2077 6179 2074 6f20 7265 616c 6c79 2066   way to really f
-00020f60: 6978 2069 7420 6672 6f6d 0a20 2020 2023  ix it from.    #
-00020f70: 2074 6865 2050 4446 2072 656e 6465 7269   the PDF renderi
-00020f80: 6e67 206d 6f64 656c 2c20 616e 6420 7472  ng model, and tr
-00020f90: 7969 6e67 2074 6f20 7472 6163 6b20 7468  ying to track th
-00020fa0: 6520 6170 7072 6f70 7269 6174 6520 7374  e appropriate st
-00020fb0: 6174 652f 6465 6661 756c 7473 2073 6565  ate/defaults see
-00020fc0: 6d73 0a20 2020 2023 2073 696d 696c 6172  ms.    # similar
-00020fd0: 6c79 2065 7272 6f72 2070 726f 6e65 2e0a  ly error prone..
-00020fe0: 0a20 2020 2023 2049 6e20 6765 6e65 7261  .    # In genera
-00020ff0: 6c2c 2074 6865 2065 7870 6563 7461 7469  l, the expectati
-00021000: 6f6e 2069 7320 7468 6174 2070 6169 6e74  on is that paint
-00021010: 6564 2063 6c69 7070 696e 6720 7061 7468  ed clipping path
-00021020: 7320 6172 6520 6c69 6b65 6c79 2074 6f20  s are likely to 
-00021030: 6265 2076 6572 790a 2020 2020 2320 756e  be very.    # un
-00021040: 636f 6d6d 6f6e 2c20 736f 2069 7427 7320  common, so it's 
-00021050: 616e 2065 6467 6520 6361 7365 2074 6861  an edge case tha
-00021060: 7420 6973 6e27 7420 776f 7274 6820 776f  t isn't worth wo
-00021070: 7272 7969 6e67 2074 6f6f 206d 7563 6820  rrying too much 
-00021080: 6162 6f75 742e 0a0a 2020 2020 6465 6620  about...    def 
-00021090: 5f5f 696e 6974 5f5f 2873 656c 662c 2078  __init__(self, x
-000210a0: 3d30 2c20 793d 3029 3a0a 2020 2020 2020  =0, y=0):.      
-000210b0: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-000210c0: 5f5f 2878 3d78 2c20 793d 7929 0a20 2020  __(x=x, y=y).   
-000210d0: 2020 2020 2073 656c 662e 7061 696e 745f       self.paint_
-000210e0: 7275 6c65 203d 2050 6174 6850 6169 6e74  rule = PathPaint
-000210f0: 5275 6c65 2e44 4f4e 545f 5041 494e 540a  Rule.DONT_PAINT.
-00021100: 0a20 2020 2064 6566 2072 656e 6465 7228  .    def render(
-00021110: 0a20 2020 2020 2020 2073 656c 662c 2067  .        self, g
-00021120: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
-00021130: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
-00021140: 6e69 7469 616c 5f70 6f69 6e74 2c20 6465  nitial_point, de
-00021150: 6275 675f 7374 7265 616d 3d4e 6f6e 652c  bug_stream=None,
-00021160: 2070 6678 3d4e 6f6e 650a 2020 2020 293a   pfx=None.    ):
-00021170: 0a20 2020 2020 2020 2023 2070 6169 6e74  .        # paint
-00021180: 696e 6720 7468 6520 636c 6970 7069 6e67  ing the clipping
-00021190: 2070 6174 6820 6f75 7473 6964 6520 6f66   path outside of
-000211a0: 2069 7473 2072 6f6f 7420 6772 6170 6869   its root graphi
-000211b0: 6373 2063 6f6e 7465 7874 2061 6c6c 6f77  cs context allow
-000211c0: 7320 6974 2074 6f0a 2020 2020 2020 2020  s it to.        
-000211d0: 2320 6265 2074 7261 6e73 666f 726d 6564  # be transformed
-000211e0: 2077 6974 686f 7574 2061 6666 6563 7469   without affecti
-000211f0: 6e67 2074 6865 2074 7261 6e73 666f 726d  ng the transform
-00021200: 206f 6620 7468 6520 6772 6170 6869 6373   of the graphics
-00021210: 2063 6f6e 7465 7874 206f 6620 7468 650a   context of the.
-00021220: 2020 2020 2020 2020 2320 7061 7468 2069          # path i
-00021230: 7420 6973 2062 6569 6e67 2075 7365 6420  t is being used 
-00021240: 746f 2063 6c69 702e 2054 6869 7320 6973  to clip. This is
-00021250: 2062 6563 6175 7365 2c20 756e 6c69 6b65   because, unlike
-00021260: 2061 6c6c 206f 6620 7468 6520 6f74 6865   all of the othe
-00021270: 7220 7374 796c 650a 2020 2020 2020 2020  r style.        
-00021280: 2320 7365 7474 696e 6773 2c20 7472 616e  # settings, tran
-00021290: 7366 6f72 6d61 7469 6f6e 7320 696d 6d65  sformations imme
-000212a0: 6469 6174 656c 7920 6166 6665 6374 2074  diately affect t
-000212b0: 6865 2070 6f69 6e74 7320 666f 6c6c 6f77  he points follow
-000212c0: 696e 6720 7468 656d 2c0a 2020 2020 2020  ing them,.      
-000212d0: 2020 2320 7261 7468 6572 2074 6861 6e20    # rather than 
-000212e0: 6f6e 6c79 2061 6666 6563 7469 6e67 2074  only affecting t
-000212f0: 6865 6d20 6174 2070 6169 6e74 696e 6720  hem at painting 
-00021300: 7469 6d65 2e20 7374 726f 6b65 2073 6574  time. stroke set
-00021310: 7469 6e67 7320 616e 6420 636f 6c6f 720a  tings and color.
-00021320: 2020 2020 2020 2020 2320 7365 7474 696e          # settin
-00021330: 6773 2061 7265 2061 7070 6c69 6564 206f  gs are applied o
-00021340: 6e6c 7920 6174 2070 6169 6e74 2074 696d  nly at paint tim
-00021350: 652e 0a0a 2020 2020 2020 2020 6966 2064  e...        if d
-00021360: 6562 7567 5f73 7472 6561 6d3a 0a20 2020  ebug_stream:.   
-00021370: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
-00021380: 7472 6561 6d2e 7772 6974 6528 223c 436c  tream.write("<Cl
-00021390: 6970 7069 6e67 5061 7468 3e20 2229 0a0a  ippingPath> ")..
-000213a0: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-000213b0: 2020 2020 2020 7265 6e64 6572 5f6c 6973        render_lis
-000213c0: 742c 0a20 2020 2020 2020 2020 2020 206c  t,.            l
-000213d0: 6173 745f 6974 656d 2c0a 2020 2020 2020  ast_item,.      
-000213e0: 2020 2020 2020 696e 6974 6961 6c5f 706f        initial_po
-000213f0: 696e 742c 0a20 2020 2020 2020 2029 203d  int,.        ) =
-00021400: 2073 656c 662e 5f72 6f6f 745f 6772 6170   self._root_grap
-00021410: 6869 6373 5f63 6f6e 7465 7874 2e62 7569  hics_context.bui
-00021420: 6c64 5f72 656e 6465 725f 6c69 7374 280a  ld_render_list(.
-00021430: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
-00021440: 7265 6769 7374 7279 2c0a 2020 2020 2020  registry,.      
-00021450: 2020 2020 2020 7374 796c 652c 0a20 2020        style,.   
-00021460: 2020 2020 2020 2020 206c 6173 745f 6974           last_it
-00021470: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
-00021480: 696e 6974 6961 6c5f 706f 696e 742c 0a20  initial_point,. 
-00021490: 2020 2020 2020 2020 2020 2064 6562 7567             debug
-000214a0: 5f73 7472 6561 6d2c 0a20 2020 2020 2020  _stream,.       
-000214b0: 2020 2020 2070 6678 2c0a 2020 2020 2020       pfx,.      
-000214c0: 2020 2020 2020 5f70 7573 685f 7374 6163        _push_stac
-000214d0: 6b3d 4661 6c73 652c 0a20 2020 2020 2020  k=False,.       
-000214e0: 2029 0a0a 2020 2020 2020 2020 6d65 7267   )..        merg
-000214f0: 6564 5f73 7479 6c65 203d 2047 7261 7068  ed_style = Graph
-00021500: 6963 7353 7479 6c65 2e6d 6572 6765 2873  icsStyle.merge(s
-00021510: 7479 6c65 2c20 7365 6c66 2e73 7479 6c65  tyle, self.style
-00021520: 290a 2020 2020 2020 2020 2320 7765 2073  ).        # we s
-00021530: 686f 756c 6420 6e65 7665 7220 6765 7420  hould never get 
-00021540: 6120 636f 6c6c 6973 696f 6e20 6572 726f  a collision erro
-00021550: 7220 6865 7265 0a20 2020 2020 2020 2069  r here.        i
-00021560: 6e74 6572 7365 6374 696f 6e5f 7275 6c65  ntersection_rule
-00021570: 203d 206d 6572 6765 645f 7374 796c 652e   = merged_style.
-00021580: 696e 7465 7273 6563 7469 6f6e 5f72 756c  intersection_rul
-00021590: 650a 2020 2020 2020 2020 6966 2069 6e74  e.        if int
-000215a0: 6572 7365 6374 696f 6e5f 7275 6c65 2069  ersection_rule i
-000215b0: 7320 6d65 7267 6564 5f73 7479 6c65 2e49  s merged_style.I
-000215c0: 4e48 4552 4954 3a0a 2020 2020 2020 2020  NHERIT:.        
-000215d0: 2020 2020 696e 7465 7273 6563 7469 6f6e      intersection
-000215e0: 5f72 756c 6520 3d20 436c 6970 7069 6e67  _rule = Clipping
-000215f0: 5061 7468 496e 7465 7273 6563 7469 6f6e  PathIntersection
-00021600: 5275 6c65 2e4e 4f4e 5a45 524f 0a20 2020  Rule.NONZERO.   
-00021610: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00021620: 2020 2020 2020 2069 6e74 6572 7365 6374         intersect
-00021630: 696f 6e5f 7275 6c65 203d 2043 6c69 7070  ion_rule = Clipp
-00021640: 696e 6750 6174 6849 6e74 6572 7365 6374  ingPathIntersect
-00021650: 696f 6e52 756c 655b 0a20 2020 2020 2020  ionRule[.       
-00021660: 2020 2020 2020 2020 2069 6e74 6572 7365           interse
-00021670: 6374 696f 6e5f 7275 6c65 2e6e 616d 6520  ction_rule.name 
-00021680: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-00021690: 6c65 3d6e 6f2d 6d65 6d62 6572 0a20 2020  le=no-member.   
-000216a0: 2020 2020 2020 2020 205d 0a0a 2020 2020           ]..    
-000216b0: 2020 2020 7061 696e 745f 7275 6c65 203d      paint_rule =
-000216c0: 206d 6572 6765 645f 7374 796c 652e 7265   merged_style.re
-000216d0: 736f 6c76 655f 7061 696e 745f 7275 6c65  solve_paint_rule
-000216e0: 2829 0a0a 2020 2020 2020 2020 7265 6e64  ()..        rend
-000216f0: 6572 5f6c 6973 742e 6170 7065 6e64 2869  er_list.append(i
-00021700: 6e74 6572 7365 6374 696f 6e5f 7275 6c65  ntersection_rule
-00021710: 2e76 616c 7565 290a 2020 2020 2020 2020  .value).        
-00021720: 7265 6e64 6572 5f6c 6973 742e 6170 7065  render_list.appe
-00021730: 6e64 2870 6169 6e74 5f72 756c 652e 7661  nd(paint_rule.va
-00021740: 6c75 6529 0a0a 2020 2020 2020 2020 7265  lue)..        re
-00021750: 7475 726e 2022 2022 2e6a 6f69 6e28 7265  turn " ".join(re
-00021760: 6e64 6572 5f6c 6973 7429 2c20 6c61 7374  nder_list), last
-00021770: 5f69 7465 6d2c 2069 6e69 7469 616c 5f70  _item, initial_p
-00021780: 6f69 6e74 0a0a 2020 2020 6465 6620 7265  oint..    def re
-00021790: 6e64 6572 5f64 6562 7567 280a 2020 2020  nder_debug(.    
-000217a0: 2020 2020 7365 6c66 2c20 6773 645f 7265      self, gsd_re
-000217b0: 6769 7374 7279 2c20 7374 796c 652c 206c  gistry, style, l
-000217c0: 6173 745f 6974 656d 2c20 696e 6974 6961  ast_item, initia
-000217d0: 6c5f 706f 696e 742c 2064 6562 7567 5f73  l_point, debug_s
-000217e0: 7472 6561 6d2c 2070 6678 0a20 2020 2029  tream, pfx.    )
-000217f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00021800: 2020 2020 2020 5265 6e64 6572 2074 6869        Render thi
-00021810: 7320 7061 7468 2065 6c65 6d65 6e74 2074  s path element t
-00021820: 6f20 6974 7320 5044 4620 7265 7072 6573  o its PDF repres
-00021830: 656e 7461 7469 6f6e 2061 6e64 2070 726f  entation and pro
-00021840: 6475 6365 2064 6562 7567 0a20 2020 2020  duce debug.     
-00021850: 2020 2069 6e66 6f72 6d61 7469 6f6e 2e0a     information..
-00021860: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00021870: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
-00021880: 6567 6973 7472 7920 2847 7261 7068 6963  egistry (Graphic
-00021890: 7353 7461 7465 4469 6374 5265 6769 7374  sStateDictRegist
-000218a0: 7279 293a 2074 6865 206f 776e 6572 2773  ry): the owner's
-000218b0: 2067 7261 7068 6963 7320 7374 6174 650a   graphics state.
-000218c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000218d0: 6469 6374 696f 6e61 7279 2072 6567 6973  dictionary regis
-000218e0: 7472 792e 0a20 2020 2020 2020 2020 2020  try..           
-000218f0: 2073 7479 6c65 2028 4772 6170 6869 6373   style (Graphics
-00021900: 5374 796c 6529 3a20 7468 6520 6375 7272  Style): the curr
-00021910: 656e 7420 7265 736f 6c76 6564 2067 7261  ent resolved gra
-00021920: 7068 6963 7320 7374 796c 650a 2020 2020  phics style.    
-00021930: 2020 2020 2020 2020 6c61 7374 5f69 7465          last_ite
-00021940: 6d3a 2074 6865 2070 7265 7669 6f75 7320  m: the previous 
-00021950: 7061 7468 2065 6c65 6d65 6e74 2e0a 2020  path element..  
-00021960: 2020 2020 2020 2020 2020 6465 6275 675f            debug_
-00021970: 7374 7265 616d 2028 696f 2e54 6578 7449  stream (io.TextI
-00021980: 4f29 3a20 7468 6520 7374 7265 616d 2074  O): the stream t
-00021990: 6f20 7768 6963 6820 7468 6520 6465 6275  o which the debu
-000219a0: 6720 6f75 7470 7574 2073 686f 756c 6420  g output should 
-000219b0: 6265 0a20 2020 2020 2020 2020 2020 2020  be.             
-000219c0: 2020 2077 7269 7474 656e 2e20 5468 6973     written. This
-000219d0: 2069 7320 6e6f 7420 6775 6172 616e 7465   is not guarante
-000219e0: 6564 2074 6f20 6265 2073 6565 6b61 626c  ed to be seekabl
-000219f0: 6520 2865 2e67 2e20 6974 206d 6179 2062  e (e.g. it may b
-00021a00: 6520 7374 646f 7574 206f 720a 2020 2020  e stdout or.    
-00021a10: 2020 2020 2020 2020 2020 2020 7374 6465              stde
-00021a20: 7272 292e 0a20 2020 2020 2020 2020 2020  rr)..           
-00021a30: 2070 6678 2028 7374 7229 3a20 7468 6520   pfx (str): the 
-00021a40: 6375 7272 656e 7420 6465 6275 6720 6f75  current debug ou
-00021a50: 7470 7574 2070 7265 6669 7820 7374 7269  tput prefix stri
-00021a60: 6e67 2028 6f6e 6c79 206e 6565 6465 6420  ng (only needed 
-00021a70: 6966 2065 6d69 7474 696e 670a 2020 2020  if emitting.    
-00021a80: 2020 2020 2020 2020 2020 2020 6d6f 7265              more
-00021a90: 2074 6861 6e20 6f6e 6520 6c69 6e65 292e   than one line).
-00021aa0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00021ab0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-00021ac0: 6865 2073 616d 6520 7475 706c 6520 6173  he same tuple as
-00021ad0: 2060 436c 6970 7069 6e67 5061 7468 2e72   `ClippingPath.r
-00021ae0: 656e 6465 7260 2e0a 2020 2020 2020 2020  ender`..        
-00021af0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00021b00: 726e 2073 656c 662e 7265 6e64 6572 280a  rn self.render(.
-00021b10: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
-00021b20: 7265 6769 7374 7279 2c20 7374 796c 652c  registry, style,
-00021b30: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
-00021b40: 6961 6c5f 706f 696e 742c 2064 6562 7567  ial_point, debug
-00021b50: 5f73 7472 6561 6d2c 2070 6678 0a20 2020  _stream, pfx.   
-00021b60: 2020 2020 2029 0a0a 0a63 6c61 7373 2047       )...class G
-00021b70: 7261 7068 6963 7343 6f6e 7465 7874 3a0a  raphicsContext:.
-00021b80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00021b90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00021ba0: 7365 6c66 2e73 7479 6c65 203d 2047 7261  self.style = Gra
-00021bb0: 7068 6963 7353 7479 6c65 2829 0a20 2020  phicsStyle().   
-00021bc0: 2020 2020 2073 656c 662e 7061 7468 5f69       self.path_i
-00021bd0: 7465 6d73 203d 205b 5d0a 0a20 2020 2020  tems = []..     
-00021be0: 2020 2073 656c 662e 5f74 7261 6e73 666f     self._transfo
-00021bf0: 726d 203d 204e 6f6e 650a 2020 2020 2020  rm = None.      
-00021c00: 2020 7365 6c66 2e5f 636c 6970 7069 6e67    self._clipping
-00021c10: 5f70 6174 6820 3d20 4e6f 6e65 0a0a 2020  _path = None..  
-00021c20: 2020 6465 6620 5f5f 6465 6570 636f 7079    def __deepcopy
-00021c30: 5f5f 2873 656c 662c 206d 656d 6f29 3a0a  __(self, memo):.
-00021c40: 2020 2020 2020 2020 636f 7069 6564 203d          copied =
-00021c50: 2073 656c 662e 5f5f 636c 6173 735f 5f28   self.__class__(
-00021c60: 290a 2020 2020 2020 2020 636f 7069 6564  ).        copied
-00021c70: 2e73 7479 6c65 203d 2063 6f70 792e 6465  .style = copy.de
-00021c80: 6570 636f 7079 2873 656c 662e 7374 796c  epcopy(self.styl
-00021c90: 652c 206d 656d 6f29 0a20 2020 2020 2020  e, memo).       
-00021ca0: 2063 6f70 6965 642e 7061 7468 5f69 7465   copied.path_ite
-00021cb0: 6d73 203d 2063 6f70 792e 6465 6570 636f  ms = copy.deepco
-00021cc0: 7079 2873 656c 662e 7061 7468 5f69 7465  py(self.path_ite
-00021cd0: 6d73 2c20 6d65 6d6f 290a 0a20 2020 2020  ms, memo)..     
-00021ce0: 2020 2063 6f70 6965 642e 5f74 7261 6e73     copied._trans
-00021cf0: 666f 726d 203d 2063 6f70 792e 6465 6570  form = copy.deep
-00021d00: 636f 7079 2873 656c 662e 7472 616e 7366  copy(self.transf
-00021d10: 6f72 6d2c 206d 656d 6f29 0a20 2020 2020  orm, memo).     
-00021d20: 2020 2063 6f70 6965 642e 5f63 6c69 7070     copied._clipp
-00021d30: 696e 675f 7061 7468 203d 2063 6f70 792e  ing_path = copy.
-00021d40: 6465 6570 636f 7079 2873 656c 662e 636c  deepcopy(self.cl
-00021d50: 6970 7069 6e67 5f70 6174 682c 206d 656d  ipping_path, mem
-00021d60: 6f29 0a0a 2020 2020 2020 2020 7265 7475  o)..        retu
-00021d70: 726e 2063 6f70 6965 640a 0a20 2020 2040  rn copied..    @
-00021d80: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00021d90: 2074 7261 6e73 666f 726d 2873 656c 6629   transform(self)
-00021da0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00021db0: 2073 656c 662e 5f74 7261 6e73 666f 726d   self._transform
-00021dc0: 0a0a 2020 2020 4074 7261 6e73 666f 726d  ..    @transform
-00021dd0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00021de0: 7472 616e 7366 6f72 6d28 7365 6c66 2c20  transform(self, 
-00021df0: 7466 293a 0a20 2020 2020 2020 2073 656c  tf):.        sel
-00021e00: 662e 5f74 7261 6e73 666f 726d 203d 2074  f._transform = t
-00021e10: 660a 0a20 2020 2040 7072 6f70 6572 7479  f..    @property
-00021e20: 0a20 2020 2064 6566 2063 6c69 7070 696e  .    def clippin
-00021e30: 675f 7061 7468 2873 656c 6629 3a0a 2020  g_path(self):.  
-00021e40: 2020 2020 2020 2222 2254 6865 2060 436c        """The `Cl
-00021e50: 6970 7069 6e67 5061 7468 6020 666f 7220  ippingPath` for 
-00021e60: 7468 6973 2067 7261 7068 6963 7320 636f  this graphics co
-00021e70: 6e74 6578 742e 2222 220a 2020 2020 2020  ntext.""".      
-00021e80: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
-00021e90: 6c69 7070 696e 675f 7061 7468 0a0a 2020  lipping_path..  
-00021ea0: 2020 4063 6c69 7070 696e 675f 7061 7468    @clipping_path
-00021eb0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00021ec0: 636c 6970 7069 6e67 5f70 6174 6828 7365  clipping_path(se
-00021ed0: 6c66 2c20 6e65 775f 636c 6970 6174 6829  lf, new_clipath)
-00021ee0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00021ef0: 636c 6970 7069 6e67 5f70 6174 6820 3d20  clipping_path = 
-00021f00: 6e65 775f 636c 6970 6174 680a 0a20 2020  new_clipath..   
-00021f10: 2064 6566 2061 6464 5f69 7465 6d28 7365   def add_item(se
-00021f20: 6c66 2c20 6974 656d 2c20 5f63 6f70 793d  lf, item, _copy=
-00021f30: 5472 7565 293a 0a20 2020 2020 2020 2022  True):.        "
-00021f40: 2222 0a20 2020 2020 2020 2041 6464 2061  "".        Add a
-00021f50: 2070 6174 6820 656c 656d 656e 7420 746f   path element to
-00021f60: 2074 6869 7320 6772 6170 6869 6373 2063   this graphics c
-00021f70: 6f6e 7465 7874 2e0a 0a20 2020 2020 2020  ontext...       
-00021f80: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00021f90: 2020 2069 7465 6d3a 2074 6865 2070 6174     item: the pat
-00021fa0: 6820 656c 656d 656e 7420 746f 2061 6464  h element to add
-00021fb0: 2e20 4d61 7920 6265 2061 2070 7269 6d69  . May be a primi
-00021fc0: 7469 7665 2065 6c65 6d65 6e74 206f 7220  tive element or 
-00021fd0: 616e 6f74 6865 720a 2020 2020 2020 2020  another.        
-00021fe0: 2020 2020 2020 2020 6047 7261 7068 6963          `Graphic
-00021ff0: 7343 6f6e 7465 7874 6020 6f72 2061 2060  sContext` or a `
-00022000: 5061 696e 7465 6450 6174 6860 2e0a 2020  PaintedPath`..  
-00022010: 2020 2020 2020 2020 2020 5f63 6f70 7920            _copy 
-00022020: 2862 6f6f 6c29 3a20 6966 2074 7275 6520  (bool): if true 
-00022030: 2874 6865 2064 6566 6175 6c74 292c 2074  (the default), t
-00022040: 6865 2069 7465 6d20 7769 6c6c 2062 6520  he item will be 
-00022050: 636f 7069 6564 2062 6566 6f72 6520 6265  copied before be
-00022060: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00022070: 2020 2020 6170 7065 6e64 6564 2e20 5468      appended. Th
-00022080: 6973 2070 7265 7665 6e74 7320 6d6f 6469  is prevents modi
-00022090: 6669 6361 7469 6f6e 7320 746f 2061 2072  fications to a r
-000220a0: 6566 6572 656e 6365 6420 6f62 6a65 6374  eferenced object
-000220b0: 2066 726f 6d0a 2020 2020 2020 2020 2020   from.          
-000220c0: 2020 2020 2020 2272 6574 726f 6163 7469        "retroacti
-000220d0: 7665 6c79 2220 616c 7465 7269 6e67 2069  vely" altering i
-000220e0: 7473 2073 7479 6c65 2f73 6861 7065 2061  ts style/shape a
-000220f0: 6e64 2073 686f 756c 6420 6265 2064 6973  nd should be dis
-00022100: 6162 6c65 6420 7769 7468 0a20 2020 2020  abled with.     
-00022110: 2020 2020 2020 2020 2020 2063 6175 7469             cauti
-00022120: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-00022130: 2020 2020 2020 2020 6966 205f 636f 7079          if _copy
-00022140: 3a0a 2020 2020 2020 2020 2020 2020 6974  :.            it
-00022150: 656d 203d 2063 6f70 792e 6465 6570 636f  em = copy.deepco
-00022160: 7079 2869 7465 6d29 0a0a 2020 2020 2020  py(item)..      
-00022170: 2020 7365 6c66 2e70 6174 685f 6974 656d    self.path_item
-00022180: 732e 6170 7065 6e64 2869 7465 6d29 0a0a  s.append(item)..
-00022190: 2020 2020 6465 6620 7265 6d6f 7665 5f6c      def remove_l
-000221a0: 6173 745f 6974 656d 2873 656c 6629 3a0a  ast_item(self):.
-000221b0: 2020 2020 2020 2020 6465 6c20 7365 6c66          del self
-000221c0: 2e70 6174 685f 6974 656d 735b 2d31 5d0a  .path_items[-1].
-000221d0: 0a20 2020 2064 6566 206d 6572 6765 2873  .    def merge(s
-000221e0: 656c 662c 206f 7468 6572 5f63 6f6e 7465  elf, other_conte
-000221f0: 7874 293a 0a20 2020 2020 2020 2022 2222  xt):.        """
-00022200: 436f 7079 2061 6e6f 7468 6572 2060 4772  Copy another `Gr
-00022210: 6170 6869 6373 436f 6e74 6578 7460 2773  aphicsContext`'s
-00022220: 2070 6174 6820 6974 656d 7320 696e 746f   path items into
-00022230: 2074 6869 7320 6f6e 652e 2222 220a 2020   this one.""".  
-00022240: 2020 2020 2020 7365 6c66 2e70 6174 685f        self.path_
-00022250: 6974 656d 732e 6578 7465 6e64 286f 7468  items.extend(oth
-00022260: 6572 5f63 6f6e 7465 7874 2e70 6174 685f  er_context.path_
-00022270: 6974 656d 7329 0a0a 2020 2020 4066 6f72  items)..    @for
-00022280: 6365 5f6e 6f64 6f63 756d 656e 740a 2020  ce_nodocument.  
-00022290: 2020 6465 6620 6275 696c 645f 7265 6e64    def build_rend
-000222a0: 6572 5f6c 6973 7428 0a20 2020 2020 2020  er_list(.       
-000222b0: 2073 656c 662c 0a20 2020 2020 2020 2067   self,.        g
-000222c0: 7364 5f72 6567 6973 7472 792c 0a20 2020  sd_registry,.   
-000222d0: 2020 2020 2073 7479 6c65 2c0a 2020 2020       style,.    
-000222e0: 2020 2020 6c61 7374 5f69 7465 6d2c 0a20      last_item,. 
-000222f0: 2020 2020 2020 2069 6e69 7469 616c 5f70         initial_p
-00022300: 6f69 6e74 2c0a 2020 2020 2020 2020 6465  oint,.        de
-00022310: 6275 675f 7374 7265 616d 3d4e 6f6e 652c  bug_stream=None,
-00022320: 0a20 2020 2020 2020 2070 6678 3d4e 6f6e  .        pfx=Non
-00022330: 652c 0a20 2020 2020 2020 205f 7075 7368  e,.        _push
-00022340: 5f73 7461 636b 3d54 7275 652c 0a20 2020  _stack=True,.   
-00022350: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
-00022360: 2020 2020 2020 2020 4275 696c 6420 6120          Build a 
-00022370: 6c69 7374 2063 6f6d 706f 7365 6420 6f66  list composed of
-00022380: 2061 6c6c 2061 6c6c 2074 6865 2069 6e64   all all the ind
-00022390: 6976 6964 7561 6c20 656c 656d 656e 7473  ividual elements
-000223a0: 2072 656e 6465 7265 642e 0a0a 2020 2020   rendered...    
-000223b0: 2020 2020 5468 6973 2069 7320 7573 6564      This is used
-000223c0: 2062 7920 6050 6169 6e74 6564 5061 7468   by `PaintedPath
-000223d0: 6020 616e 6420 6043 6c69 7070 696e 6750  ` and `ClippingP
-000223e0: 6174 6860 2074 6f20 7265 7573 6520 7468  ath` to reuse th
-000223f0: 6520 6047 7261 7068 6963 7343 6f6e 7465  e `GraphicsConte
-00022400: 7874 600a 2020 2020 2020 2020 7265 6e64  xt`.        rend
-00022410: 6572 696e 6720 7072 6f63 6573 7320 7768  ering process wh
-00022420: 696c 6520 7374 696c 6c20 6265 696e 6720  ile still being 
-00022430: 6162 6c65 2074 6f20 696e 6a65 6374 2073  able to inject s
-00022440: 6f6d 6520 7061 7468 2073 7065 6369 6669  ome path specifi
-00022450: 6320 6974 656d 730a 2020 2020 2020 2020  c items.        
-00022460: 2865 2e67 2e20 7468 6520 7061 696e 7469  (e.g. the painti
-00022470: 6e67 2064 6972 6563 7469 7665 2920 6265  ng directive) be
-00022480: 666f 7265 2074 6865 2072 656e 6465 7220  fore the render 
-00022490: 6973 2063 6f6c 6c61 7073 6564 2069 6e74  is collapsed int
-000224a0: 6f20 6120 7369 6e67 6c65 0a20 2020 2020  o a single.     
-000224b0: 2020 2073 7472 696e 672e 0a0a 2020 2020     string...    
-000224c0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000224d0: 2020 2020 2020 6773 645f 7265 6769 7374        gsd_regist
-000224e0: 7279 2028 4772 6170 6869 6373 5374 6174  ry (GraphicsStat
-000224f0: 6544 6963 7452 6567 6973 7472 7929 3a20  eDictRegistry): 
-00022500: 7468 6520 6f77 6e65 7227 7320 6772 6170  the owner's grap
-00022510: 6869 6373 2073 7461 7465 0a20 2020 2020  hics state.     
-00022520: 2020 2020 2020 2020 2020 2064 6963 7469             dicti
-00022530: 6f6e 6172 7920 7265 6769 7374 7279 2e0a  onary registry..
-00022540: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00022550: 6520 2847 7261 7068 6963 7353 7479 6c65  e (GraphicsStyle
-00022560: 293a 2074 6865 2063 7572 7265 6e74 2072  ): the current r
-00022570: 6573 6f6c 7665 6420 6772 6170 6869 6373  esolved graphics
-00022580: 2073 7479 6c65 0a20 2020 2020 2020 2020   style.         
-00022590: 2020 206c 6173 745f 6974 656d 3a20 7468     last_item: th
-000225a0: 6520 7072 6576 696f 7573 2070 6174 6820  e previous path 
-000225b0: 656c 656d 656e 742e 0a20 2020 2020 2020  element..       
-000225c0: 2020 2020 2069 6e69 7469 616c 5f70 6f69       initial_poi
-000225d0: 6e74 3a20 6c61 7374 2070 6f73 6974 696f  nt: last positio
-000225e0: 6e20 7365 7420 6279 2061 2022 4d22 206f  n set by a "M" o
-000225f0: 7220 226d 2220 636f 6d6d 616e 640a 2020  r "m" command.  
-00022600: 2020 2020 2020 2020 2020 6465 6275 675f            debug_
-00022610: 7374 7265 616d 2028 696f 2e54 6578 7449  stream (io.TextI
-00022620: 4f29 3a20 7468 6520 7374 7265 616d 2074  O): the stream t
-00022630: 6f20 7768 6963 6820 7468 6520 6465 6275  o which the debu
-00022640: 6720 6f75 7470 7574 2073 686f 756c 6420  g output should 
-00022650: 6265 0a20 2020 2020 2020 2020 2020 2020  be.             
-00022660: 2020 2077 7269 7474 656e 2e20 5468 6973     written. This
-00022670: 2069 7320 6e6f 7420 6775 6172 616e 7465   is not guarante
-00022680: 6564 2074 6f20 6265 2073 6565 6b61 626c  ed to be seekabl
-00022690: 6520 2865 2e67 2e20 6974 206d 6179 2062  e (e.g. it may b
-000226a0: 6520 7374 646f 7574 206f 720a 2020 2020  e stdout or.    
-000226b0: 2020 2020 2020 2020 2020 2020 7374 6465              stde
-000226c0: 7272 292e 0a20 2020 2020 2020 2020 2020  rr)..           
-000226d0: 2070 6678 2028 7374 7229 3a20 7468 6520   pfx (str): the 
-000226e0: 6375 7272 656e 7420 6465 6275 6720 6f75  current debug ou
-000226f0: 7470 7574 2070 7265 6669 7820 7374 7269  tput prefix stri
-00022700: 6e67 2028 6f6e 6c79 206e 6565 6465 6420  ng (only needed 
-00022710: 6966 2065 6d69 7474 696e 670a 2020 2020  if emitting.    
-00022720: 2020 2020 2020 2020 2020 2020 6d6f 7265              more
-00022730: 2074 6861 6e20 6f6e 6520 6c69 6e65 292e   than one line).
-00022740: 0a20 2020 2020 2020 2020 2020 205f 7075  .            _pu
-00022750: 7368 5f73 7461 636b 2028 626f 6f6c 293a  sh_stack (bool):
-00022760: 2069 6620 5472 7565 2c20 7772 6170 2074   if True, wrap t
-00022770: 6865 2072 6573 756c 7469 6e67 2072 656e  he resulting ren
-00022780: 6465 7220 6c69 7374 2069 6e20 6120 7075  der list in a pu
-00022790: 7368 2f70 6f70 0a20 2020 2020 2020 2020  sh/pop.         
-000227a0: 2020 2020 2020 2067 7261 7068 6963 7320         graphics 
-000227b0: 7374 6163 6b20 6469 7265 6374 6976 6520  stack directive 
-000227c0: 7061 6972 2e0a 0a20 2020 2020 2020 2052  pair...        R
-000227d0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000227e0: 2020 2020 6074 7570 6c65 5b6c 6973 745b      `tuple[list[
-000227f0: 7374 725d 2c20 6c61 7374 5f69 7465 6d5d  str], last_item]
-00022800: 6020 7768 6572 6520 606c 6173 745f 6974  ` where `last_it
-00022810: 656d 6020 6973 2074 6865 2070 6173 7420  em` is the past 
-00022820: 7061 7468 2065 6c65 6d65 6e74 2069 6e0a  path element in.
-00022830: 2020 2020 2020 2020 2020 2020 7468 6973              this
-00022840: 2060 4772 6170 6869 6373 436f 6e74 6578   `GraphicsContex
-00022850: 7460 0a20 2020 2020 2020 2022 2222 0a20  t`.        """. 
-00022860: 2020 2020 2020 2072 656e 6465 725f 6c69         render_li
-00022870: 7374 203d 205b 5d0a 0a20 2020 2020 2020  st = []..       
-00022880: 2069 6620 7365 6c66 2e70 6174 685f 6974   if self.path_it
-00022890: 656d 733a 0a20 2020 2020 2020 2020 2020  ems:.           
-000228a0: 2069 6620 6465 6275 675f 7374 7265 616d   if debug_stream
-000228b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000228c0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-000228d0: 6275 675f 7374 7265 616d 2e77 7269 7465  bug_stream.write
-000228e0: 2866 227b 7365 6c66 2e5f 5f63 6c61 7373  (f"{self.__class
-000228f0: 5f5f 2e5f 5f6e 616d 655f 5f7d 2229 0a0a  __.__name__}")..
-00022900: 2020 2020 2020 2020 2020 2020 6d65 7267              merg
-00022910: 6564 5f73 7479 6c65 203d 2073 7479 6c65  ed_style = style
-00022920: 2e5f 5f63 6c61 7373 5f5f 2e6d 6572 6765  .__class__.merge
-00022930: 2873 7479 6c65 2c20 7365 6c66 2e73 7479  (style, self.sty
-00022940: 6c65 290a 0a20 2020 2020 2020 2020 2020  le)..           
-00022950: 2069 6620 6465 6275 675f 7374 7265 616d   if debug_stream
-00022960: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00022970: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00022980: 2073 656c 662e 5f74 7261 6e73 666f 726d   self._transform
-00022990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000229a0: 2020 2020 2020 6465 6275 675f 7374 7265        debug_stre
-000229b0: 616d 2e77 7269 7465 2866 2228 7b73 656c  am.write(f"({sel
-000229c0: 662e 5f74 7261 6e73 666f 726d 7d29 2229  f._transform})")
-000229d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000229e0: 2020 7374 796c 6573 5f64 6267 203d 205b    styles_dbg = [
-000229f0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00022a00: 2020 666f 7220 6174 7472 2069 6e20 6d65    for attr in me
-00022a10: 7267 6564 5f73 7479 6c65 2e4d 4552 4745  rged_style.MERGE
-00022a20: 5f50 524f 5045 5254 4945 533a 0a20 2020  _PROPERTIES:.   
-00022a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a40: 2076 616c 203d 2067 6574 6174 7472 286d   val = getattr(m
-00022a50: 6572 6765 645f 7374 796c 652c 2061 7474  erged_style, att
-00022a60: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-00022a70: 2020 2020 2020 2069 6620 7661 6c20 6973         if val is
-00022a80: 206e 6f74 206d 6572 6765 645f 7374 796c   not merged_styl
-00022a90: 652e 494e 4845 5249 543a 0a20 2020 2020  e.INHERIT:.     
-00022aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022ab0: 2020 2069 6620 6765 7461 7474 7228 7365     if getattr(se
-00022ac0: 6c66 2e73 7479 6c65 2c20 6174 7472 2920  lf.style, attr) 
-00022ad0: 6973 206d 6572 6765 645f 7374 796c 652e  is merged_style.
-00022ae0: 494e 4845 5249 543a 0a20 2020 2020 2020  INHERIT:.       
-00022af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b00: 2020 2020 2069 6e68 203d 2022 2028 696e       inh = " (in
-00022b10: 6865 7269 7465 6429 220a 2020 2020 2020  herited)".      
-00022b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00022b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b50: 2020 2020 696e 6820 3d20 2222 0a0a 2020      inh = ""..  
-00022b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b70: 2020 2020 2020 7374 796c 6573 5f64 6267        styles_dbg
-00022b80: 2e61 7070 656e 6428 6622 7b61 7474 727d  .append(f"{attr}
-00022b90: 3a20 7b76 616c 7d7b 696e 687d 2229 0a0a  : {val}{inh}")..
-00022ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022bb0: 6966 2073 7479 6c65 735f 6462 673a 0a20  if styles_dbg:. 
-00022bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022bd0: 2020 2064 6562 7567 5f73 7472 6561 6d2e     debug_stream.
-00022be0: 7772 6974 6528 2220 7b5c 6e22 290a 2020  write(" {\n").  
-00022bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c00: 2020 666f 7220 7374 796c 655f 6462 675f    for style_dbg_
-00022c10: 6c69 6e65 2069 6e20 7374 796c 6573 5f64  line in styles_d
-00022c20: 6267 3a0a 2020 2020 2020 2020 2020 2020  bg:.            
-00022c30: 2020 2020 2020 2020 2020 2020 6465 6275              debu
-00022c40: 675f 7374 7265 616d 2e77 7269 7465 2870  g_stream.write(p
-00022c50: 6678 202b 2022 2020 2020 2229 0a20 2020  fx + "    ").   
-00022c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c70: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
-00022c80: 6d2e 7772 6974 6528 7374 796c 655f 6462  m.write(style_db
-00022c90: 675f 6c69 6e65 290a 2020 2020 2020 2020  g_line).        
-00022ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022cb0: 6465 6275 675f 7374 7265 616d 2e77 7269  debug_stream.wri
-00022cc0: 7465 2822 5c6e 2229 0a0a 2020 2020 2020  te("\n")..      
-00022cd0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00022ce0: 6275 675f 7374 7265 616d 2e77 7269 7465  bug_stream.write
-00022cf0: 2870 6678 202b 2022 7de2 9490 5c6e 2229  (pfx + "}...\n")
-00022d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022d10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00022d20: 2020 2020 2020 2020 2020 2064 6562 7567             debug
-00022d30: 5f73 7472 6561 6d2e 7772 6974 6528 225c  _stream.write("\
-00022d40: 6e22 290a 0a20 2020 2020 2020 2020 2020  n")..           
-00022d50: 204e 4f5f 454d 4954 5f53 4554 203d 207b   NO_EMIT_SET = {
-00022d60: 4e6f 6e65 2c20 6d65 7267 6564 5f73 7479  None, merged_sty
-00022d70: 6c65 2e49 4e48 4552 4954 7d0a 0a20 2020  le.INHERIT}..   
-00022d80: 2020 2020 2020 2020 2065 6d69 745f 7374           emit_st
-00022d90: 796c 6520 3d20 7365 6c66 2e73 7479 6c65  yle = self.style
-00022da0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00022db0: 6d65 7267 6564 5f73 7479 6c65 2e61 6c6c  merged_style.all
-00022dc0: 6f77 5f74 7261 6e73 7061 7265 6e63 7920  ow_transparency 
-00022dd0: 213d 2073 656c 662e 7374 796c 652e 616c  != self.style.al
-00022de0: 6c6f 775f 7472 616e 7370 6172 656e 6379  low_transparency
-00022df0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022e00: 2020 656d 6974 5f73 7479 6c65 203d 2063    emit_style = c
-00022e10: 6f70 792e 6465 6570 636f 7079 2873 656c  opy.deepcopy(sel
-00022e20: 662e 7374 796c 6529 0a20 2020 2020 2020  f.style).       
-00022e30: 2020 2020 2020 2020 2065 6d69 745f 7374           emit_st
-00022e40: 796c 652e 616c 6c6f 775f 7472 616e 7370  yle.allow_transp
-00022e50: 6172 656e 6379 203d 206d 6572 6765 645f  arency = merged_
-00022e60: 7374 796c 652e 616c 6c6f 775f 7472 616e  style.allow_tran
-00022e70: 7370 6172 656e 6379 0a0a 2020 2020 2020  sparency..      
-00022e80: 2020 2020 2020 2320 696e 206f 7264 6572        # in order
-00022e90: 2074 6f20 6465 636f 7570 6c65 2074 6865   to decouple the
-00022ea0: 2064 6173 6820 7061 7474 6572 6e20 616e   dash pattern an
-00022eb0: 6420 7468 6520 6461 7368 2070 6861 7365  d the dash phase
-00022ec0: 2061 7420 7468 6520 4150 4920 6c61 7965   at the API laye
-00022ed0: 722c 0a20 2020 2020 2020 2020 2020 2023  r,.            #
-00022ee0: 2077 6520 6861 7665 2074 6f20 7065 7266   we have to perf
-00022ef0: 6f72 6d20 6164 6469 7469 6f6e 616c 206c  orm additional l
-00022f00: 6f67 6963 2068 6572 6520 746f 2072 6563  ogic here to rec
-00022f10: 6f6d 6269 6e65 2074 6865 6d2e 2057 6520  ombine them. We 
-00022f20: 6361 6e20 7265 6c79 0a20 2020 2020 2020  can rely.       
-00022f30: 2020 2020 2023 206f 6e20 7468 6573 6520       # on these 
-00022f40: 6265 696e 6720 7365 7269 616c 697a 6162  being serializab
-00022f50: 6c65 2062 6563 6175 7365 2077 6520 616c  le because we al
-00022f60: 7761 7973 2067 6574 2061 2073 616e 6520  ways get a sane 
-00022f70: 7374 796c 6520 6f6e 2074 6865 0a20 2020  style on the.   
-00022f80: 2020 2020 2020 2020 2023 2064 7261 7769           # drawi
-00022f90: 6e67 2063 6f6e 7465 7874 2e0a 2020 2020  ng context..    
-00022fa0: 2020 2020 2020 2020 6461 7368 5f70 6174          dash_pat
-00022fb0: 7465 726e 203d 206d 6572 6765 645f 7374  tern = merged_st
-00022fc0: 796c 652e 7374 726f 6b65 5f64 6173 685f  yle.stroke_dash_
-00022fd0: 7061 7474 6572 6e0a 2020 2020 2020 2020  pattern.        
-00022fe0: 2020 2020 6461 7368 5f70 6861 7365 203d      dash_phase =
-00022ff0: 206d 6572 6765 645f 7374 796c 652e 7374   merged_style.st
-00023000: 726f 6b65 5f64 6173 685f 7068 6173 650a  roke_dash_phase.
-00023010: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00023020: 6461 7368 5f70 6174 7465 726e 2021 3d20  dash_pattern != 
-00023030: 7374 796c 652e 7374 726f 6b65 5f64 6173  style.stroke_das
-00023040: 685f 7061 7474 6572 6e29 206f 7220 280a  h_pattern) or (.
-00023050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023060: 6461 7368 5f70 6861 7365 2021 3d20 7374  dash_phase != st
-00023070: 796c 652e 7374 726f 6b65 5f64 6173 685f  yle.stroke_dash_
-00023080: 7068 6173 650a 2020 2020 2020 2020 2020  phase.          
-00023090: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-000230a0: 2020 2020 2069 6620 656d 6974 5f73 7479       if emit_sty
-000230b0: 6c65 2069 7320 7365 6c66 2e73 7479 6c65  le is self.style
-000230c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000230d0: 2020 2020 2020 656d 6974 5f73 7479 6c65        emit_style
-000230e0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-000230f0: 2865 6d69 745f 7374 796c 6529 0a20 2020  (emit_style).   
-00023100: 2020 2020 2020 2020 2020 2020 2065 6d69               emi
-00023110: 745f 7374 796c 652e 7374 726f 6b65 5f64  t_style.stroke_d
-00023120: 6173 685f 7061 7474 6572 6e20 3d20 6461  ash_pattern = da
-00023130: 7368 5f70 6174 7465 726e 0a20 2020 2020  sh_pattern.     
-00023140: 2020 2020 2020 2020 2020 2065 6d69 745f             emit_
-00023150: 7374 796c 652e 7374 726f 6b65 5f64 6173  style.stroke_das
-00023160: 685f 7068 6173 6520 3d20 6461 7368 5f70  h_phase = dash_p
-00023170: 6861 7365 0a0a 2020 2020 2020 2020 2020  hase..          
-00023180: 2020 2020 2020 656d 6974 5f64 6173 6820        emit_dash 
-00023190: 3d20 2864 6173 685f 7061 7474 6572 6e2c  = (dash_pattern,
-000231a0: 2064 6173 685f 7068 6173 6529 0a20 2020   dash_phase).   
-000231b0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000231c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000231d0: 6d69 745f 6461 7368 203d 204e 6f6e 650a  mit_dash = None.
-000231e0: 0a20 2020 2020 2020 2020 2020 2073 7479  .            sty
-000231f0: 6c65 5f64 6963 745f 6e61 6d65 203d 2067  le_dict_name = g
-00023200: 7364 5f72 6567 6973 7472 792e 7265 6769  sd_registry.regi
-00023210: 7374 6572 5f73 7479 6c65 2865 6d69 745f  ster_style(emit_
-00023220: 7374 796c 6529 0a0a 2020 2020 2020 2020  style)..        
-00023230: 2020 2020 6966 2073 7479 6c65 5f64 6963      if style_dic
-00023240: 745f 6e61 6d65 2069 7320 6e6f 7420 4e6f  t_name is not No
-00023250: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00023260: 2020 2020 7265 6e64 6572 5f6c 6973 742e      render_list.
-00023270: 6170 7065 6e64 2866 227b 7265 6e64 6572  append(f"{render
-00023280: 5f70 6466 5f70 7269 6d69 7469 7665 2873  _pdf_primitive(s
-00023290: 7479 6c65 5f64 6963 745f 6e61 6d65 297d  tyle_dict_name)}
-000232a0: 2067 7322 290a 0a20 2020 2020 2020 2020   gs")..         
-000232b0: 2020 2023 2077 6520 6361 6e27 7420 7365     # we can't se
-000232c0: 7420 636f 6c6f 7220 696e 2074 6865 2067  t color in the g
-000232d0: 7261 7068 6963 7320 7374 6174 6520 636f  raphics state co
-000232e0: 6e74 6578 7420 6469 6374 696f 6e61 7279  ntext dictionary
-000232f0: 2c20 736f 2077 6520 6861 7665 2074 6f0a  , so we have to.
-00023300: 2020 2020 2020 2020 2020 2020 2320 6d61              # ma
-00023310: 6e75 616c 6c79 2069 6e68 6572 6974 2069  nually inherit i
-00023320: 7420 616e 6420 656d 6974 2069 7420 6865  t and emit it he
-00023330: 7265 2e0a 2020 2020 2020 2020 2020 2020  re..            
-00023340: 6669 6c6c 5f63 6f6c 6f72 203d 2073 656c  fill_color = sel
-00023350: 662e 7374 796c 652e 6669 6c6c 5f63 6f6c  f.style.fill_col
-00023360: 6f72 0a20 2020 2020 2020 2020 2020 2073  or.            s
-00023370: 7472 6f6b 655f 636f 6c6f 7220 3d20 7365  troke_color = se
-00023380: 6c66 2e73 7479 6c65 2e73 7472 6f6b 655f  lf.style.stroke_
-00023390: 636f 6c6f 720a 0a20 2020 2020 2020 2020  color..         
-000233a0: 2020 2069 6620 6669 6c6c 5f63 6f6c 6f72     if fill_color
-000233b0: 206e 6f74 2069 6e20 4e4f 5f45 4d49 545f   not in NO_EMIT_
-000233c0: 5345 543a 0a20 2020 2020 2020 2020 2020  SET:.           
-000233d0: 2020 2020 2072 656e 6465 725f 6c69 7374       render_list
-000233e0: 2e61 7070 656e 6428 6669 6c6c 5f63 6f6c  .append(fill_col
-000233f0: 6f72 2e73 6572 6961 6c69 7a65 2829 2e6c  or.serialize().l
-00023400: 6f77 6572 2829 290a 0a20 2020 2020 2020  ower())..       
-00023410: 2020 2020 2069 6620 7374 726f 6b65 5f63       if stroke_c
-00023420: 6f6c 6f72 206e 6f74 2069 6e20 4e4f 5f45  olor not in NO_E
-00023430: 4d49 545f 5345 543a 0a20 2020 2020 2020  MIT_SET:.       
-00023440: 2020 2020 2020 2020 2072 656e 6465 725f           render_
-00023450: 6c69 7374 2e61 7070 656e 6428 7374 726f  list.append(stro
-00023460: 6b65 5f63 6f6c 6f72 2e73 6572 6961 6c69  ke_color.seriali
-00023470: 7a65 2829 2e75 7070 6572 2829 290a 0a20  ze().upper()).. 
-00023480: 2020 2020 2020 2020 2020 2069 6620 656d             if em
-00023490: 6974 5f64 6173 6820 6973 206e 6f74 204e  it_dash is not N
-000234a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000234b0: 2020 2020 2072 656e 6465 725f 6c69 7374       render_list
-000234c0: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-000234d0: 2020 2020 2020 2020 2020 2020 2072 656e               ren
-000234e0: 6465 725f 7064 665f 7072 696d 6974 6976  der_pdf_primitiv
-000234f0: 6528 656d 6974 5f64 6173 685b 305d 290a  e(emit_dash[0]).
+00016eb0: 6974 656d 732e 6170 7065 6e64 2843 6c6f  items.append(Clo
+00016ec0: 7365 2829 290a 0a20 2020 2020 2020 2072  se())..        r
+00016ed0: 6574 7572 6e20 6974 656d 730a 0a20 2020  eturn items..   
+00016ee0: 2040 666f 7263 655f 6e6f 646f 6375 6d65   @force_nodocume
+00016ef0: 6e74 0a20 2020 2064 6566 2072 656e 6465  nt.    def rende
+00016f00: 7228 7365 6c66 2c20 6773 645f 7265 6769  r(self, gsd_regi
+00016f10: 7374 7279 2c20 7374 796c 652c 206c 6173  stry, style, las
+00016f20: 745f 6974 656d 2c20 696e 6974 6961 6c5f  t_item, initial_
+00016f30: 706f 696e 7429 3a0a 2020 2020 2020 2020  point):.        
+00016f40: 2222 220a 2020 2020 2020 2020 5265 6e64  """.        Rend
+00016f50: 6572 2074 6869 7320 7061 7468 2065 6c65  er this path ele
+00016f60: 6d65 6e74 2074 6f20 6974 7320 5044 4620  ment to its PDF 
+00016f70: 7265 7072 6573 656e 7461 7469 6f6e 2e0a  representation..
+00016f80: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00016f90: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
+00016fa0: 6567 6973 7472 7920 2847 7261 7068 6963  egistry (Graphic
+00016fb0: 7353 7461 7465 4469 6374 5265 6769 7374  sStateDictRegist
+00016fc0: 7279 293a 2074 6865 206f 776e 6572 2773  ry): the owner's
+00016fd0: 2067 7261 7068 6963 7320 7374 6174 650a   graphics state.
+00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ff0: 6469 6374 696f 6e61 7279 2072 6567 6973  dictionary regis
+00017000: 7472 792e 0a20 2020 2020 2020 2020 2020  try..           
+00017010: 2073 7479 6c65 2028 4772 6170 6869 6373   style (Graphics
+00017020: 5374 796c 6529 3a20 7468 6520 6375 7272  Style): the curr
+00017030: 656e 7420 7265 736f 6c76 6564 2067 7261  ent resolved gra
+00017040: 7068 6963 7320 7374 796c 650a 2020 2020  phics style.    
+00017050: 2020 2020 2020 2020 6c61 7374 5f69 7465          last_ite
+00017060: 6d3a 2074 6865 2070 7265 7669 6f75 7320  m: the previous 
+00017070: 7061 7468 2065 6c65 6d65 6e74 2e0a 2020  path element..  
+00017080: 2020 2020 2020 2020 2020 696e 6974 6961            initia
+00017090: 6c5f 706f 696e 743a 206c 6173 7420 706f  l_point: last po
+000170a0: 7369 7469 6f6e 2073 6574 2062 7920 6120  sition set by a 
+000170b0: 224d 2220 6f72 2022 6d22 2063 6f6d 6d61  "M" or "m" comma
+000170c0: 6e64 0a0a 2020 2020 2020 2020 5265 7475  nd..        Retu
+000170d0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+000170e0: 2061 2074 7570 6c65 206f 6620 6028 7374   a tuple of `(st
+000170f0: 722c 206e 6577 5f6c 6173 745f 6974 656d  r, new_last_item
+00017100: 2960 2c20 7768 6572 6520 606e 6577 5f6c  )`, where `new_l
+00017110: 6173 745f 6974 656d 6020 6973 2061 2072  ast_item` is a r
+00017120: 6573 6f6c 7665 640a 2020 2020 2020 2020  esolved.        
+00017130: 2020 2020 604c 696e 6560 2e0a 2020 2020      `Line`..    
+00017140: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00017150: 636f 6d70 6f6e 656e 7473 203d 2073 656c  components = sel
+00017160: 662e 5f64 6563 6f6d 706f 7365 2829 0a0a  f._decompose()..
+00017170: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00017180: 6f6d 706f 6e65 6e74 733a 0a20 2020 2020  omponents:.     
+00017190: 2020 2020 2020 2072 6574 7572 6e20 2222         return ""
+000171a0: 2c20 6c61 7374 5f69 7465 6d0a 0a20 2020  , last_item..   
+000171b0: 2020 2020 2072 656e 6465 725f 6c69 7374       render_list
+000171c0: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+000171d0: 7220 6974 656d 2069 6e20 636f 6d70 6f6e  r item in compon
+000171e0: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
+000171f0: 2020 7265 6e64 6572 6564 2c20 6c61 7374    rendered, last
+00017200: 5f69 7465 6d2c 2069 6e69 7469 616c 5f70  _item, initial_p
+00017210: 6f69 6e74 203d 2069 7465 6d2e 7265 6e64  oint = item.rend
+00017220: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00017230: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
+00017240: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
+00017250: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
+00017260: 740a 2020 2020 2020 2020 2020 2020 290a  t.            ).
+00017270: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
+00017280: 6572 5f6c 6973 742e 6170 7065 6e64 2872  er_list.append(r
+00017290: 656e 6465 7265 6429 0a0a 2020 2020 2020  endered)..      
+000172a0: 2020 7265 7475 726e 2022 2022 2e6a 6f69    return " ".joi
+000172b0: 6e28 7265 6e64 6572 5f6c 6973 7429 2c20  n(render_list), 
+000172c0: 4c69 6e65 2873 656c 662e 6f72 6729 2c20  Line(self.org), 
+000172d0: 696e 6974 6961 6c5f 706f 696e 740a 0a20  initial_point.. 
+000172e0: 2020 2040 666f 7263 655f 6e6f 646f 6375     @force_nodocu
+000172f0: 6d65 6e74 0a20 2020 2064 6566 2072 656e  ment.    def ren
+00017300: 6465 725f 6465 6275 6728 0a20 2020 2020  der_debug(.     
+00017310: 2020 2073 656c 662c 2067 7364 5f72 6567     self, gsd_reg
+00017320: 6973 7472 792c 2073 7479 6c65 2c20 6c61  istry, style, la
+00017330: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
+00017340: 5f70 6f69 6e74 2c20 6465 6275 675f 7374  _point, debug_st
+00017350: 7265 616d 2c20 7066 780a 2020 2020 293a  ream, pfx.    ):
+00017360: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017370: 2020 2020 2052 656e 6465 7220 7468 6973       Render this
+00017380: 2070 6174 6820 656c 656d 656e 7420 746f   path element to
+00017390: 2069 7473 2050 4446 2072 6570 7265 7365   its PDF represe
+000173a0: 6e74 6174 696f 6e20 616e 6420 7072 6f64  ntation and prod
+000173b0: 7563 6520 6465 6275 670a 2020 2020 2020  uce debug.      
+000173c0: 2020 696e 666f 726d 6174 696f 6e2e 0a0a    information...
+000173d0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+000173e0: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
+000173f0: 6769 7374 7279 2028 4772 6170 6869 6373  gistry (Graphics
+00017400: 5374 6174 6544 6963 7452 6567 6973 7472  StateDictRegistr
+00017410: 7929 3a20 7468 6520 6f77 6e65 7227 7320  y): the owner's 
+00017420: 6772 6170 6869 6373 2073 7461 7465 0a20  graphics state. 
+00017430: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017440: 6963 7469 6f6e 6172 7920 7265 6769 7374  ictionary regist
+00017450: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
+00017460: 7374 796c 6520 2847 7261 7068 6963 7353  style (GraphicsS
+00017470: 7479 6c65 293a 2074 6865 2063 7572 7265  tyle): the curre
+00017480: 6e74 2072 6573 6f6c 7665 6420 6772 6170  nt resolved grap
+00017490: 6869 6373 2073 7479 6c65 0a20 2020 2020  hics style.     
+000174a0: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
+000174b0: 3a20 7468 6520 7072 6576 696f 7573 2070  : the previous p
+000174c0: 6174 6820 656c 656d 656e 742e 0a20 2020  ath element..   
+000174d0: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
+000174e0: 5f70 6f69 6e74 3a20 6c61 7374 2070 6f73  _point: last pos
+000174f0: 6974 696f 6e20 7365 7420 6279 2061 2022  ition set by a "
+00017500: 4d22 206f 7220 226d 2220 636f 6d6d 616e  M" or "m" comman
+00017510: 640a 2020 2020 2020 2020 2020 2020 6465  d.            de
+00017520: 6275 675f 7374 7265 616d 2028 696f 2e54  bug_stream (io.T
+00017530: 6578 7449 4f29 3a20 7468 6520 7374 7265  extIO): the stre
+00017540: 616d 2074 6f20 7768 6963 6820 7468 6520  am to which the 
+00017550: 6465 6275 6720 6f75 7470 7574 2073 686f  debug output sho
+00017560: 756c 6420 6265 0a20 2020 2020 2020 2020  uld be.         
+00017570: 2020 2020 2020 2077 7269 7474 656e 2e20         written. 
+00017580: 5468 6973 2069 7320 6e6f 7420 6775 6172  This is not guar
+00017590: 616e 7465 6564 2074 6f20 6265 2073 6565  anteed to be see
+000175a0: 6b61 626c 6520 2865 2e67 2e20 6974 206d  kable (e.g. it m
+000175b0: 6179 2062 6520 7374 646f 7574 206f 720a  ay be stdout or.
+000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175d0: 7374 6465 7272 292e 0a20 2020 2020 2020  stderr)..       
+000175e0: 2020 2020 2070 6678 2028 7374 7229 3a20       pfx (str): 
+000175f0: 7468 6520 6375 7272 656e 7420 6465 6275  the current debu
+00017600: 6720 6f75 7470 7574 2070 7265 6669 7820  g output prefix 
+00017610: 7374 7269 6e67 2028 6f6e 6c79 206e 6565  string (only nee
+00017620: 6465 6420 6966 2065 6d69 7474 696e 670a  ded if emitting.
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 6d6f 7265 2074 6861 6e20 6f6e 6520 6c69  more than one li
+00017650: 6e65 292e 0a0a 2020 2020 2020 2020 5265  ne)...        Re
+00017660: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00017670: 2020 2054 6865 2073 616d 6520 7475 706c     The same tupl
+00017680: 6520 6173 2060 526f 756e 6465 6452 6563  e as `RoundedRec
+00017690: 7461 6e67 6c65 2e72 656e 6465 7260 2e0a  tangle.render`..
+000176a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000176b0: 2020 2020 636f 6d70 6f6e 656e 7473 203d      components =
+000176c0: 2073 656c 662e 5f64 6563 6f6d 706f 7365   self._decompose
+000176d0: 2829 0a0a 2020 2020 2020 2020 6465 6275  ()..        debu
+000176e0: 675f 7374 7265 616d 2e77 7269 7465 2866  g_stream.write(f
+000176f0: 227b 7365 6c66 7d20 7265 736f 6c76 6564  "{self} resolved
+00017700: 2074 6f3a 5c6e 2229 0a20 2020 2020 2020   to:\n").       
+00017710: 2069 6620 6e6f 7420 636f 6d70 6f6e 656e   if not componen
+00017720: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00017730: 6465 6275 675f 7374 7265 616d 2e77 7269  debug_stream.wri
+00017740: 7465 2870 6678 202b 2022 20e2 9494 e294  te(pfx + " .....
+00017750: 8020 6e6f 7468 696e 675c 6e22 290a 2020  . nothing\n").  
+00017760: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017770: 2022 222c 206c 6173 745f 6974 656d 0a0a   "", last_item..
+00017780: 2020 2020 2020 2020 7265 6e64 6572 5f6c          render_l
+00017790: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
+000177a0: 2066 6f72 2069 7465 6d20 696e 2063 6f6d   for item in com
+000177b0: 706f 6e65 6e74 735b 3a2d 315d 3a0a 2020  ponents[:-1]:.  
+000177c0: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+000177d0: 6564 2c20 6c61 7374 5f69 7465 6d2c 2069  ed, last_item, i
+000177e0: 6e69 7469 616c 5f70 6f69 6e74 203d 2069  nitial_point = i
+000177f0: 7465 6d2e 7265 6e64 6572 280a 2020 2020  tem.render(.    
+00017800: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
+00017810: 7265 6769 7374 7279 2c20 7374 796c 652c  registry, style,
+00017820: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
+00017830: 6961 6c5f 706f 696e 740a 2020 2020 2020  ial_point.      
+00017840: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00017850: 2020 2020 6465 6275 675f 7374 7265 616d      debug_stream
+00017860: 2e77 7269 7465 2870 6678 202b 2066 2220  .write(pfx + f" 
+00017870: e294 9ce2 9480 207b 6974 656d 7d5c 6e22  ...... {item}\n"
+00017880: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00017890: 6e64 6572 5f6c 6973 742e 6170 7065 6e64  nder_list.append
+000178a0: 2872 656e 6465 7265 6429 0a0a 2020 2020  (rendered)..    
+000178b0: 2020 2020 7265 6e64 6572 6564 2c20 6c61      rendered, la
+000178c0: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
+000178d0: 5f70 6f69 6e74 203d 2063 6f6d 706f 6e65  _point = compone
+000178e0: 6e74 735b 2d31 5d2e 7265 6e64 6572 280a  nts[-1].render(.
+000178f0: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
+00017900: 7265 6769 7374 7279 2c20 7374 796c 652c  registry, style,
+00017910: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
+00017920: 6961 6c5f 706f 696e 740a 2020 2020 2020  ial_point.      
+00017930: 2020 290a 2020 2020 2020 2020 6465 6275    ).        debu
+00017940: 675f 7374 7265 616d 2e77 7269 7465 2870  g_stream.write(p
+00017950: 6678 202b 2066 2220 e294 94e2 9480 207b  fx + f" ...... {
+00017960: 636f 6d70 6f6e 656e 7473 5b2d 315d 7d5c  components[-1]}\
+00017970: 6e22 290a 2020 2020 2020 2020 7265 6e64  n").        rend
+00017980: 6572 5f6c 6973 742e 6170 7065 6e64 2872  er_list.append(r
+00017990: 656e 6465 7265 6429 0a0a 2020 2020 2020  endered)..      
+000179a0: 2020 7265 7475 726e 2022 2022 2e6a 6f69    return " ".joi
+000179b0: 6e28 7265 6e64 6572 5f6c 6973 7429 2c20  n(render_list), 
+000179c0: 4c69 6e65 2873 656c 662e 6f72 6729 2c20  Line(self.org), 
+000179d0: 696e 6974 6961 6c5f 706f 696e 740a 0a0a  initial_point...
+000179e0: 636c 6173 7320 456c 6c69 7073 6528 4e61  class Ellipse(Na
+000179f0: 6d65 6454 7570 6c65 293a 0a20 2020 2022  medTuple):.    "
+00017a00: 2222 0a20 2020 2041 6e20 656c 6c69 7073  "".    An ellips
+00017a10: 652e 0a0a 2020 2020 5365 653a 2060 5061  e...    See: `Pa
+00017a20: 696e 7465 6450 6174 682e 656c 6c69 7073  intedPath.ellips
+00017a30: 6560 0a20 2020 2022 2222 0a0a 2020 2020  e`.    """..    
+00017a40: 7261 6469 693a 2050 6f69 6e74 0a20 2020  radii: Point.   
+00017a50: 2022 2222 5468 6520 782d 2061 6e64 2079   """The x- and y
+00017a60: 2d72 6164 6969 206f 6620 7468 6520 656c  -radii of the el
+00017a70: 6c69 7073 6522 2222 0a20 2020 2063 656e  lipse""".    cen
+00017a80: 7465 723a 2050 6f69 6e74 0a20 2020 2022  ter: Point.    "
+00017a90: 2222 5468 6520 6162 7363 6973 7361 2061  ""The abscissa a
+00017aa0: 6e64 206f 7264 696e 6174 6520 6f66 2074  nd ordinate of t
+00017ab0: 6865 2063 656e 7465 7220 6f66 2074 6865  he center of the
+00017ac0: 2065 6c6c 6970 7365 2222 220a 0a20 2020   ellipse"""..   
+00017ad0: 2064 6566 205f 6465 636f 6d70 6f73 6528   def _decompose(
+00017ae0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00017af0: 7465 6d73 203d 205b 5d0a 0a20 2020 2020  tems = []..     
+00017b00: 2020 2072 7820 3d20 6162 7328 7365 6c66     rx = abs(self
+00017b10: 2e72 6164 6969 2e78 290a 2020 2020 2020  .radii.x).      
+00017b20: 2020 7279 203d 2061 6273 2873 656c 662e    ry = abs(self.
+00017b30: 7261 6469 692e 7929 0a20 2020 2020 2020  radii.y).       
+00017b40: 2063 782c 2063 7920 3d20 7365 6c66 2e63   cx, cy = self.c
+00017b50: 656e 7465 720a 0a20 2020 2020 2020 2061  enter..        a
+00017b60: 7263 5f72 6164 203d 2050 6f69 6e74 2872  rc_rad = Point(r
+00017b70: 782c 2072 7929 0a0a 2020 2020 2020 2020  x, ry)..        
+00017b80: 2320 7468 6973 2069 736e 2774 2074 6865  # this isn't the
+00017b90: 206d 6f73 7420 6566 6669 6369 656e 7420   most efficient 
+00017ba0: 7761 7920 746f 2064 6f20 7468 6973 2c20  way to do this, 
+00017bb0: 636f 6d70 7574 6174 696f 6e61 6c6c 792c  computationally,
+00017bc0: 2062 7574 2069 7427 730a 2020 2020 2020   but it's.      
+00017bd0: 2020 2320 696e 7465 726e 616c 6c79 2063    # internally c
+00017be0: 6f6e 7369 7374 656e 742e 0a20 2020 2020  onsistent..     
+00017bf0: 2020 2069 6620 2872 7820 213d 2030 2920     if (rx != 0) 
+00017c00: 616e 6420 2872 7920 213d 2030 293a 0a20  and (ry != 0):. 
+00017c10: 2020 2020 2020 2020 2020 2069 7465 6d73             items
+00017c20: 2e61 7070 656e 6428 4d6f 7665 2850 6f69  .append(Move(Poi
+00017c30: 6e74 2863 7820 2b20 7278 2c20 6379 2929  nt(cx + rx, cy))
+00017c40: 290a 2020 2020 2020 2020 2020 2020 6974  ).            it
+00017c50: 656d 732e 6170 7065 6e64 2841 7263 2861  ems.append(Arc(a
+00017c60: 7263 5f72 6164 2c20 302c 2046 616c 7365  rc_rad, 0, False
+00017c70: 2c20 5472 7565 2c20 506f 696e 7428 6378  , True, Point(cx
+00017c80: 2c20 6379 202b 2072 7929 2929 0a20 2020  , cy + ry))).   
+00017c90: 2020 2020 2020 2020 2069 7465 6d73 2e61           items.a
+00017ca0: 7070 656e 6428 4172 6328 6172 635f 7261  ppend(Arc(arc_ra
+00017cb0: 642c 2030 2c20 4661 6c73 652c 2054 7275  d, 0, False, Tru
+00017cc0: 652c 2050 6f69 6e74 2863 7820 2d20 7278  e, Point(cx - rx
+00017cd0: 2c20 6379 2929 290a 2020 2020 2020 2020  , cy))).        
+00017ce0: 2020 2020 6974 656d 732e 6170 7065 6e64      items.append
+00017cf0: 2841 7263 2861 7263 5f72 6164 2c20 302c  (Arc(arc_rad, 0,
+00017d00: 2046 616c 7365 2c20 5472 7565 2c20 506f   False, True, Po
+00017d10: 696e 7428 6378 2c20 6379 202d 2072 7929  int(cx, cy - ry)
+00017d20: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+00017d30: 7465 6d73 2e61 7070 656e 6428 4172 6328  tems.append(Arc(
+00017d40: 6172 635f 7261 642c 2030 2c20 4661 6c73  arc_rad, 0, Fals
+00017d50: 652c 2054 7275 652c 2050 6f69 6e74 2863  e, True, Point(c
+00017d60: 7820 2b20 7278 2c20 6379 2929 290a 2020  x + rx, cy))).  
+00017d70: 2020 2020 2020 2020 2020 6974 656d 732e            items.
+00017d80: 6170 7065 6e64 2843 6c6f 7365 2829 290a  append(Close()).
+00017d90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017da0: 6974 656d 730a 0a20 2020 2040 666f 7263  items..    @forc
+00017db0: 655f 6e6f 646f 6375 6d65 6e74 0a20 2020  e_nodocument.   
+00017dc0: 2064 6566 2072 656e 6465 7228 7365 6c66   def render(self
+00017dd0: 2c20 6773 645f 7265 6769 7374 7279 2c20  , gsd_registry, 
+00017de0: 7374 796c 652c 206c 6173 745f 6974 656d  style, last_item
+00017df0: 2c20 696e 6974 6961 6c5f 706f 696e 7429  , initial_point)
+00017e00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00017e10: 2020 2020 2020 5265 6e64 6572 2074 6869        Render thi
+00017e20: 7320 7061 7468 2065 6c65 6d65 6e74 2074  s path element t
+00017e30: 6f20 6974 7320 5044 4620 7265 7072 6573  o its PDF repres
+00017e40: 656e 7461 7469 6f6e 2e0a 0a20 2020 2020  entation...     
+00017e50: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00017e60: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
+00017e70: 7920 2847 7261 7068 6963 7353 7461 7465  y (GraphicsState
+00017e80: 4469 6374 5265 6769 7374 7279 293a 2074  DictRegistry): t
+00017e90: 6865 206f 776e 6572 2773 2067 7261 7068  he owner's graph
+00017ea0: 6963 7320 7374 6174 650a 2020 2020 2020  ics state.      
+00017eb0: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
+00017ec0: 6e61 7279 2072 6567 6973 7472 792e 0a20  nary registry.. 
+00017ed0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00017ee0: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
+00017ef0: 3a20 7468 6520 6375 7272 656e 7420 7265  : the current re
+00017f00: 736f 6c76 6564 2067 7261 7068 6963 7320  solved graphics 
+00017f10: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
+00017f20: 2020 6c61 7374 5f69 7465 6d3a 2074 6865    last_item: the
+00017f30: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
+00017f40: 6c65 6d65 6e74 2e0a 2020 2020 2020 2020  lement..        
+00017f50: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
+00017f60: 743a 206c 6173 7420 706f 7369 7469 6f6e  t: last position
+00017f70: 2073 6574 2062 7920 6120 224d 2220 6f72   set by a "M" or
+00017f80: 2022 6d22 2063 6f6d 6d61 6e64 0a0a 2020   "m" command..  
+00017f90: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00017fa0: 2020 2020 2020 2020 2020 2061 2074 7570             a tup
+00017fb0: 6c65 206f 6620 6028 7374 722c 206e 6577  le of `(str, new
+00017fc0: 5f6c 6173 745f 6974 656d 2960 2c20 7768  _last_item)`, wh
+00017fd0: 6572 6520 606e 6577 5f6c 6173 745f 6974  ere `new_last_it
+00017fe0: 656d 6020 6973 2061 2072 6573 6f6c 7665  em` is a resolve
+00017ff0: 640a 2020 2020 2020 2020 2020 2020 604d  d.            `M
+00018000: 6f76 6560 2074 6f20 7468 6520 6365 6e74  ove` to the cent
+00018010: 6572 206f 6620 7468 6520 656c 6c69 7073  er of the ellips
+00018020: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00018030: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+00018040: 7320 3d20 7365 6c66 2e5f 6465 636f 6d70  s = self._decomp
+00018050: 6f73 6528 290a 0a20 2020 2020 2020 2069  ose()..        i
+00018060: 6620 6e6f 7420 636f 6d70 6f6e 656e 7473  f not components
+00018070: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00018080: 7475 726e 2022 222c 206c 6173 745f 6974  turn "", last_it
+00018090: 656d 0a0a 2020 2020 2020 2020 7265 6e64  em..        rend
+000180a0: 6572 5f6c 6973 7420 3d20 5b5d 0a20 2020  er_list = [].   
+000180b0: 2020 2020 2066 6f72 2069 7465 6d20 696e       for item in
+000180c0: 2063 6f6d 706f 6e65 6e74 733a 0a20 2020   components:.   
+000180d0: 2020 2020 2020 2020 2072 656e 6465 7265           rendere
+000180e0: 642c 206c 6173 745f 6974 656d 2c20 696e  d, last_item, in
+000180f0: 6974 6961 6c5f 706f 696e 7420 3d20 6974  itial_point = it
+00018100: 656d 2e72 656e 6465 7228 0a20 2020 2020  em.render(.     
+00018110: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
+00018120: 6567 6973 7472 792c 2073 7479 6c65 2c20  egistry, style, 
+00018130: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
+00018140: 616c 5f70 6f69 6e74 0a20 2020 2020 2020  al_point.       
+00018150: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00018160: 2020 2072 656e 6465 725f 6c69 7374 2e61     render_list.a
+00018170: 7070 656e 6428 7265 6e64 6572 6564 290a  ppend(rendered).
+00018180: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00018190: 2220 222e 6a6f 696e 2872 656e 6465 725f  " ".join(render_
+000181a0: 6c69 7374 292c 204d 6f76 6528 7365 6c66  list), Move(self
+000181b0: 2e63 656e 7465 7229 2c20 696e 6974 6961  .center), initia
+000181c0: 6c5f 706f 696e 740a 0a20 2020 2040 666f  l_point..    @fo
+000181d0: 7263 655f 6e6f 646f 6375 6d65 6e74 0a20  rce_nodocument. 
+000181e0: 2020 2064 6566 2072 656e 6465 725f 6465     def render_de
+000181f0: 6275 6728 0a20 2020 2020 2020 2073 656c  bug(.        sel
+00018200: 662c 2067 7364 5f72 6567 6973 7472 792c  f, gsd_registry,
+00018210: 2073 7479 6c65 2c20 6c61 7374 5f69 7465   style, last_ite
+00018220: 6d2c 2069 6e69 7469 616c 5f70 6f69 6e74  m, initial_point
+00018230: 2c20 6465 6275 675f 7374 7265 616d 2c20  , debug_stream, 
+00018240: 7066 780a 2020 2020 293a 0a20 2020 2020  pfx.    ):.     
+00018250: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00018260: 656e 6465 7220 7468 6973 2070 6174 6820  ender this path 
+00018270: 656c 656d 656e 7420 746f 2069 7473 2050  element to its P
+00018280: 4446 2072 6570 7265 7365 6e74 6174 696f  DF representatio
+00018290: 6e20 616e 6420 7072 6f64 7563 6520 6465  n and produce de
+000182a0: 6275 670a 2020 2020 2020 2020 696e 666f  bug.        info
+000182b0: 726d 6174 696f 6e2e 0a0a 2020 2020 2020  rmation...      
+000182c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000182d0: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
+000182e0: 2028 4772 6170 6869 6373 5374 6174 6544   (GraphicsStateD
+000182f0: 6963 7452 6567 6973 7472 7929 3a20 7468  ictRegistry): th
+00018300: 6520 6f77 6e65 7227 7320 6772 6170 6869  e owner's graphi
+00018310: 6373 2073 7461 7465 0a20 2020 2020 2020  cs state.       
+00018320: 2020 2020 2020 2020 2064 6963 7469 6f6e           diction
+00018330: 6172 7920 7265 6769 7374 7279 2e0a 2020  ary registry..  
+00018340: 2020 2020 2020 2020 2020 7374 796c 6520            style 
+00018350: 2847 7261 7068 6963 7353 7479 6c65 293a  (GraphicsStyle):
+00018360: 2074 6865 2063 7572 7265 6e74 2072 6573   the current res
+00018370: 6f6c 7665 6420 6772 6170 6869 6373 2073  olved graphics s
+00018380: 7479 6c65 0a20 2020 2020 2020 2020 2020  tyle.           
+00018390: 206c 6173 745f 6974 656d 3a20 7468 6520   last_item: the 
+000183a0: 7072 6576 696f 7573 2070 6174 6820 656c  previous path el
+000183b0: 656d 656e 742e 0a20 2020 2020 2020 2020  ement..         
+000183c0: 2020 2069 6e69 7469 616c 5f70 6f69 6e74     initial_point
+000183d0: 3a20 6c61 7374 2070 6f73 6974 696f 6e20  : last position 
+000183e0: 7365 7420 6279 2061 2022 4d22 206f 7220  set by a "M" or 
+000183f0: 226d 2220 636f 6d6d 616e 640a 2020 2020  "m" command.    
+00018400: 2020 2020 2020 2020 6465 6275 675f 7374          debug_st
+00018410: 7265 616d 2028 696f 2e54 6578 7449 4f29  ream (io.TextIO)
+00018420: 3a20 7468 6520 7374 7265 616d 2074 6f20  : the stream to 
+00018430: 7768 6963 6820 7468 6520 6465 6275 6720  which the debug 
+00018440: 6f75 7470 7574 2073 686f 756c 6420 6265  output should be
+00018450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018460: 2077 7269 7474 656e 2e20 5468 6973 2069   written. This i
+00018470: 7320 6e6f 7420 6775 6172 616e 7465 6564  s not guaranteed
+00018480: 2074 6f20 6265 2073 6565 6b61 626c 6520   to be seekable 
+00018490: 2865 2e67 2e20 6974 206d 6179 2062 6520  (e.g. it may be 
+000184a0: 7374 646f 7574 206f 720a 2020 2020 2020  stdout or.      
+000184b0: 2020 2020 2020 2020 2020 7374 6465 7272            stderr
+000184c0: 292e 0a20 2020 2020 2020 2020 2020 2070  )..            p
+000184d0: 6678 2028 7374 7229 3a20 7468 6520 6375  fx (str): the cu
+000184e0: 7272 656e 7420 6465 6275 6720 6f75 7470  rrent debug outp
+000184f0: 7574 2070 7265 6669 7820 7374 7269 6e67  ut prefix string
+00018500: 2028 6f6e 6c79 206e 6565 6465 6420 6966   (only needed if
+00018510: 2065 6d69 7474 696e 670a 2020 2020 2020   emitting.      
+00018520: 2020 2020 2020 2020 2020 6d6f 7265 2074            more t
+00018530: 6861 6e20 6f6e 6520 6c69 6e65 292e 0a0a  han one line)...
+00018540: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00018550: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00018560: 2073 616d 6520 7475 706c 6520 6173 2060   same tuple as `
+00018570: 456c 6c69 7073 652e 7265 6e64 6572 602e  Ellipse.render`.
+00018580: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00018590: 2020 2020 2063 6f6d 706f 6e65 6e74 7320       components 
+000185a0: 3d20 7365 6c66 2e5f 6465 636f 6d70 6f73  = self._decompos
+000185b0: 6528 290a 0a20 2020 2020 2020 2064 6562  e()..        deb
+000185c0: 7567 5f73 7472 6561 6d2e 7772 6974 6528  ug_stream.write(
+000185d0: 6622 7b73 656c 667d 2072 6573 6f6c 7665  f"{self} resolve
+000185e0: 6420 746f 3a5c 6e22 290a 2020 2020 2020  d to:\n").      
+000185f0: 2020 6966 206e 6f74 2063 6f6d 706f 6e65    if not compone
+00018600: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00018610: 2064 6562 7567 5f73 7472 6561 6d2e 7772   debug_stream.wr
+00018620: 6974 6528 7066 7820 2b20 2220 e294 94e2  ite(pfx + " ....
+00018630: 9480 206e 6f74 6869 6e67 5c6e 2229 0a20  .. nothing\n"). 
+00018640: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00018650: 6e20 2222 2c20 6c61 7374 5f69 7465 6d0a  n "", last_item.
+00018660: 0a20 2020 2020 2020 2072 656e 6465 725f  .        render_
+00018670: 6c69 7374 203d 205b 5d0a 2020 2020 2020  list = [].      
+00018680: 2020 666f 7220 6974 656d 2069 6e20 636f    for item in co
+00018690: 6d70 6f6e 656e 7473 5b3a 2d31 5d3a 0a20  mponents[:-1]:. 
+000186a0: 2020 2020 2020 2020 2020 2072 656e 6465             rende
+000186b0: 7265 642c 206c 6173 745f 6974 656d 2c20  red, last_item, 
+000186c0: 696e 6974 6961 6c5f 706f 696e 7420 3d20  initial_point = 
+000186d0: 6974 656d 2e72 656e 6465 7228 0a20 2020  item.render(.   
+000186e0: 2020 2020 2020 2020 2020 2020 2067 7364               gsd
+000186f0: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
+00018700: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
+00018710: 7469 616c 5f70 6f69 6e74 0a20 2020 2020  tial_point.     
+00018720: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018730: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+00018740: 6d2e 7772 6974 6528 7066 7820 2b20 6622  m.write(pfx + f"
+00018750: 20e2 949c e294 8020 7b69 7465 6d7d 5c6e   ...... {item}\n
+00018760: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00018770: 656e 6465 725f 6c69 7374 2e61 7070 656e  ender_list.appen
+00018780: 6428 7265 6e64 6572 6564 290a 0a20 2020  d(rendered)..   
+00018790: 2020 2020 2072 656e 6465 7265 642c 206c       rendered, l
+000187a0: 6173 745f 6974 656d 2c20 696e 6974 6961  ast_item, initia
+000187b0: 6c5f 706f 696e 7420 3d20 636f 6d70 6f6e  l_point = compon
+000187c0: 656e 7473 5b2d 315d 2e72 656e 6465 7228  ents[-1].render(
+000187d0: 0a20 2020 2020 2020 2020 2020 2067 7364  .            gsd
+000187e0: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
+000187f0: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
+00018800: 7469 616c 5f70 6f69 6e74 0a20 2020 2020  tial_point.     
+00018810: 2020 2029 0a20 2020 2020 2020 2064 6562     ).        deb
+00018820: 7567 5f73 7472 6561 6d2e 7772 6974 6528  ug_stream.write(
+00018830: 7066 7820 2b20 6622 20e2 9494 e294 8020  pfx + f" ...... 
+00018840: 7b63 6f6d 706f 6e65 6e74 735b 2d31 5d7d  {components[-1]}
+00018850: 5c6e 2229 0a20 2020 2020 2020 2072 656e  \n").        ren
+00018860: 6465 725f 6c69 7374 2e61 7070 656e 6428  der_list.append(
+00018870: 7265 6e64 6572 6564 290a 0a20 2020 2020  rendered)..     
+00018880: 2020 2072 6574 7572 6e20 2220 222e 6a6f     return " ".jo
+00018890: 696e 2872 656e 6465 725f 6c69 7374 292c  in(render_list),
+000188a0: 204d 6f76 6528 7365 6c66 2e63 656e 7465   Move(self.cente
+000188b0: 7229 2c20 696e 6974 6961 6c5f 706f 696e  r), initial_poin
+000188c0: 740a 0a0a 636c 6173 7320 496d 706c 6963  t...class Implic
+000188d0: 6974 436c 6f73 6528 4e61 6d65 6454 7570  itClose(NamedTup
+000188e0: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
+000188f0: 2041 2070 6174 6820 636c 6f73 6520 656c   A path close el
+00018900: 656d 656e 7420 7468 6174 2069 7320 636f  ement that is co
+00018910: 6e64 6974 696f 6e61 6c6c 7920 7265 6e64  nditionally rend
+00018920: 6572 6564 2064 6570 656e 6469 6e67 206f  ered depending o
+00018930: 6e20 7468 6520 7661 6c75 6520 6f66 0a20  n the value of. 
+00018940: 2020 2060 4772 6170 6869 6373 5374 796c     `GraphicsStyl
+00018950: 652e 6175 746f 5f63 6c6f 7365 602e 0a20  e.auto_close`.. 
+00018960: 2020 2022 2222 0a0a 2020 2020 2320 7079     """..    # py
+00018970: 6c69 6e74 3a20 6469 7361 626c 653d 6e6f  lint: disable=no
+00018980: 2d73 656c 662d 7573 650a 2020 2020 4066  -self-use.    @f
+00018990: 6f72 6365 5f6e 6f64 6f63 756d 656e 740a  orce_nodocument.
+000189a0: 2020 2020 6465 6620 7265 6e64 6572 2873      def render(s
+000189b0: 656c 662c 2067 7364 5f72 6567 6973 7472  elf, gsd_registr
+000189c0: 792c 2073 7479 6c65 2c20 6c61 7374 5f69  y, style, last_i
+000189d0: 7465 6d2c 2069 6e69 7469 616c 5f70 6f69  tem, initial_poi
+000189e0: 6e74 293a 0a20 2020 2020 2020 2022 2222  nt):.        """
+000189f0: 0a20 2020 2020 2020 2052 656e 6465 7220  .        Render 
+00018a00: 7468 6973 2070 6174 6820 656c 656d 656e  this path elemen
+00018a10: 7420 746f 2069 7473 2050 4446 2072 6570  t to its PDF rep
+00018a20: 7265 7365 6e74 6174 696f 6e2e 0a0a 2020  resentation...  
+00018a30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00018a40: 2020 2020 2020 2020 6773 645f 7265 6769          gsd_regi
+00018a50: 7374 7279 2028 4772 6170 6869 6373 5374  stry (GraphicsSt
+00018a60: 6174 6544 6963 7452 6567 6973 7472 7929  ateDictRegistry)
+00018a70: 3a20 7468 6520 6f77 6e65 7227 7320 6772  : the owner's gr
+00018a80: 6170 6869 6373 2073 7461 7465 0a20 2020  aphics state.   
+00018a90: 2020 2020 2020 2020 2020 2020 2064 6963               dic
+00018aa0: 7469 6f6e 6172 7920 7265 6769 7374 7279  tionary registry
+00018ab0: 2e0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00018ac0: 796c 6520 2847 7261 7068 6963 7353 7479  yle (GraphicsSty
+00018ad0: 6c65 293a 2074 6865 2063 7572 7265 6e74  le): the current
+00018ae0: 2072 6573 6f6c 7665 6420 6772 6170 6869   resolved graphi
+00018af0: 6373 2073 7479 6c65 0a20 2020 2020 2020  cs style.       
+00018b00: 2020 2020 206c 6173 745f 6974 656d 3a20       last_item: 
+00018b10: 7468 6520 7072 6576 696f 7573 2070 6174  the previous pat
+00018b20: 6820 656c 656d 656e 742e 0a20 2020 2020  h element..     
+00018b30: 2020 2020 2020 2069 6e69 7469 616c 5f70         initial_p
+00018b40: 6f69 6e74 3a20 6c61 7374 2070 6f73 6974  oint: last posit
+00018b50: 696f 6e20 7365 7420 6279 2061 2022 4d22  ion set by a "M"
+00018b60: 206f 7220 226d 2220 636f 6d6d 616e 640a   or "m" command.
+00018b70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00018b80: 3a0a 2020 2020 2020 2020 2020 2020 6120  :.            a 
+00018b90: 7475 706c 6520 6f66 2060 2873 7472 2c20  tuple of `(str, 
+00018ba0: 6e65 775f 6c61 7374 5f69 7465 6d29 602c  new_last_item)`,
+00018bb0: 2077 6865 7265 2060 6e65 775f 6c61 7374   where `new_last
+00018bc0: 5f69 7465 6d60 2069 7320 7768 6174 6576  _item` is whatev
+00018bd0: 6572 2074 6865 206f 6c64 0a20 2020 2020  er the old.     
+00018be0: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
+00018bf0: 2077 6173 2e0a 2020 2020 2020 2020 2222   was..        ""
+00018c00: 220a 2020 2020 2020 2020 2320 7079 6c69  ".        # pyli
+00018c10: 6e74 3a20 6469 7361 626c 653d 756e 7573  nt: disable=unus
+00018c20: 6564 2d61 7267 756d 656e 740a 2020 2020  ed-argument.    
+00018c30: 2020 2020 6966 2073 7479 6c65 2e61 7574      if style.aut
+00018c40: 6f5f 636c 6f73 653a 0a20 2020 2020 2020  o_close:.       
+00018c50: 2020 2020 2072 6574 7572 6e20 2268 222c       return "h",
+00018c60: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
+00018c70: 6961 6c5f 706f 696e 740a 0a20 2020 2020  ial_point..     
+00018c80: 2020 2072 6574 7572 6e20 2222 2c20 6c61     return "", la
+00018c90: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
+00018ca0: 5f70 6f69 6e74 0a0a 2020 2020 4066 6f72  _point..    @for
+00018cb0: 6365 5f6e 6f64 6f63 756d 656e 740a 2020  ce_nodocument.  
+00018cc0: 2020 6465 6620 7265 6e64 6572 5f64 6562    def render_deb
+00018cd0: 7567 280a 2020 2020 2020 2020 7365 6c66  ug(.        self
+00018ce0: 2c20 6773 645f 7265 6769 7374 7279 2c20  , gsd_registry, 
+00018cf0: 7374 796c 652c 206c 6173 745f 6974 656d  style, last_item
+00018d00: 2c20 696e 6974 6961 6c5f 706f 696e 742c  , initial_point,
+00018d10: 2064 6562 7567 5f73 7472 6561 6d2c 2070   debug_stream, p
+00018d20: 6678 0a20 2020 2029 3a0a 2020 2020 2020  fx.    ):.      
+00018d30: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+00018d40: 6e64 6572 2074 6869 7320 7061 7468 2065  nder this path e
+00018d50: 6c65 6d65 6e74 2074 6f20 6974 7320 5044  lement to its PD
+00018d60: 4620 7265 7072 6573 656e 7461 7469 6f6e  F representation
+00018d70: 2061 6e64 2070 726f 6475 6365 2064 6562   and produce deb
+00018d80: 7567 0a20 2020 2020 2020 2069 6e66 6f72  ug.        infor
+00018d90: 6d61 7469 6f6e 2e0a 0a20 2020 2020 2020  mation...       
+00018da0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00018db0: 2020 2067 7364 5f72 6567 6973 7472 7920     gsd_registry 
+00018dc0: 2847 7261 7068 6963 7353 7461 7465 4469  (GraphicsStateDi
+00018dd0: 6374 5265 6769 7374 7279 293a 2074 6865  ctRegistry): the
+00018de0: 206f 776e 6572 2773 2067 7261 7068 6963   owner's graphic
+00018df0: 7320 7374 6174 650a 2020 2020 2020 2020  s state.        
+00018e00: 2020 2020 2020 2020 6469 6374 696f 6e61          dictiona
+00018e10: 7279 2072 6567 6973 7472 792e 0a20 2020  ry registry..   
+00018e20: 2020 2020 2020 2020 2073 7479 6c65 2028           style (
+00018e30: 4772 6170 6869 6373 5374 796c 6529 3a20  GraphicsStyle): 
+00018e40: 7468 6520 6375 7272 656e 7420 7265 736f  the current reso
+00018e50: 6c76 6564 2067 7261 7068 6963 7320 7374  lved graphics st
+00018e60: 796c 650a 2020 2020 2020 2020 2020 2020  yle.            
+00018e70: 6c61 7374 5f69 7465 6d3a 2074 6865 2070  last_item: the p
+00018e80: 7265 7669 6f75 7320 7061 7468 2065 6c65  revious path ele
+00018e90: 6d65 6e74 2e0a 2020 2020 2020 2020 2020  ment..          
+00018ea0: 2020 696e 6974 6961 6c5f 706f 696e 743a    initial_point:
+00018eb0: 206c 6173 7420 706f 7369 7469 6f6e 2073   last position s
+00018ec0: 6574 2062 7920 6120 224d 2220 6f72 2022  et by a "M" or "
+00018ed0: 6d22 2063 6f6d 6d61 6e64 0a20 2020 2020  m" command.     
+00018ee0: 2020 2020 2020 2064 6562 7567 5f73 7472         debug_str
+00018ef0: 6561 6d20 2869 6f2e 5465 7874 494f 293a  eam (io.TextIO):
+00018f00: 2074 6865 2073 7472 6561 6d20 746f 2077   the stream to w
+00018f10: 6869 6368 2074 6865 2064 6562 7567 206f  hich the debug o
+00018f20: 7574 7075 7420 7368 6f75 6c64 2062 650a  utput should be.
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 7772 6974 7465 6e2e 2054 6869 7320 6973  written. This is
+00018f50: 206e 6f74 2067 7561 7261 6e74 6565 6420   not guaranteed 
+00018f60: 746f 2062 6520 7365 656b 6162 6c65 2028  to be seekable (
+00018f70: 652e 672e 2069 7420 6d61 7920 6265 2073  e.g. it may be s
+00018f80: 7464 6f75 7420 6f72 0a20 2020 2020 2020  tdout or.       
+00018f90: 2020 2020 2020 2020 2073 7464 6572 7229           stderr)
+00018fa0: 2e0a 2020 2020 2020 2020 2020 2020 7066  ..            pf
+00018fb0: 7820 2873 7472 293a 2074 6865 2063 7572  x (str): the cur
+00018fc0: 7265 6e74 2064 6562 7567 206f 7574 7075  rent debug outpu
+00018fd0: 7420 7072 6566 6978 2073 7472 696e 6720  t prefix string 
+00018fe0: 286f 6e6c 7920 6e65 6564 6564 2069 6620  (only needed if 
+00018ff0: 656d 6974 7469 6e67 0a20 2020 2020 2020  emitting.       
+00019000: 2020 2020 2020 2020 206d 6f72 6520 7468           more th
+00019010: 616e 206f 6e65 206c 696e 6529 2e0a 0a20  an one line)... 
+00019020: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00019030: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00019040: 7361 6d65 2074 7570 6c65 2061 7320 6049  same tuple as `I
+00019050: 6d70 6c69 6369 7443 6c6f 7365 2e72 656e  mplicitClose.ren
+00019060: 6465 7260 2e0a 2020 2020 2020 2020 2222  der`..        ""
+00019070: 220a 2020 2020 2020 2020 2320 7079 6c69  ".        # pyli
+00019080: 6e74 3a20 6469 7361 626c 653d 756e 7573  nt: disable=unus
+00019090: 6564 2d61 7267 756d 656e 740a 2020 2020  ed-argument.    
+000190a0: 2020 2020 7265 6e64 6572 6564 2c20 7265      rendered, re
+000190b0: 736f 6c76 6564 2c20 696e 6974 6961 6c5f  solved, initial_
+000190c0: 706f 696e 7420 3d20 7365 6c66 2e72 656e  point = self.ren
+000190d0: 6465 7228 0a20 2020 2020 2020 2020 2020  der(.           
+000190e0: 2067 7364 5f72 6567 6973 7472 792c 2073   gsd_registry, s
+000190f0: 7479 6c65 2c20 6c61 7374 5f69 7465 6d2c  tyle, last_item,
+00019100: 2069 6e69 7469 616c 5f70 6f69 6e74 0a20   initial_point. 
+00019110: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00019120: 2064 6562 7567 5f73 7472 6561 6d2e 7772   debug_stream.wr
+00019130: 6974 6528 6622 7b73 656c 667d 2072 6573  ite(f"{self} res
+00019140: 6f6c 7665 6420 746f 207b 7265 6e64 6572  olved to {render
+00019150: 6564 7d5c 6e22 290a 0a20 2020 2020 2020  ed}\n")..       
+00019160: 2072 6574 7572 6e20 7265 6e64 6572 6564   return rendered
+00019170: 2c20 7265 736f 6c76 6564 2c20 696e 6974  , resolved, init
+00019180: 6961 6c5f 706f 696e 740a 0a0a 636c 6173  ial_point...clas
+00019190: 7320 436c 6f73 6528 4e61 6d65 6454 7570  s Close(NamedTup
+000191a0: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
+000191b0: 2041 2070 6174 6820 636c 6f73 6520 656c   A path close el
+000191c0: 656d 656e 742e 0a0a 2020 2020 496e 7374  ement...    Inst
+000191d0: 7275 6374 7320 7468 6520 7265 6e64 6572  ructs the render
+000191e0: 6572 2074 6f20 6472 6177 2061 2073 7472  er to draw a str
+000191f0: 6169 6768 7420 6c69 6e65 2066 726f 6d20  aight line from 
+00019200: 7468 6520 656e 6420 6f66 2074 6865 206c  the end of the l
+00019210: 6173 7420 7061 7468 2065 6c65 6d65 6e74  ast path element
+00019220: 0a20 2020 2074 6f20 7468 6520 7374 6172  .    to the star
+00019230: 7420 6f66 2074 6865 2063 7572 7265 6e74  t of the current
+00019240: 2070 6174 682e 0a0a 2020 2020 5365 653a   path...    See:
+00019250: 2060 5061 696e 7465 6450 6174 682e 636c   `PaintedPath.cl
+00019260: 6f73 6560 0a20 2020 2022 2222 0a0a 2020  ose`.    """..  
+00019270: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+00019280: 626c 653d 6e6f 2d73 656c 662d 7573 650a  ble=no-self-use.
+00019290: 2020 2020 4066 6f72 6365 5f6e 6f64 6f63      @force_nodoc
+000192a0: 756d 656e 740a 2020 2020 6465 6620 7265  ument.    def re
+000192b0: 6e64 6572 2873 656c 662c 2067 7364 5f72  nder(self, gsd_r
+000192c0: 6567 6973 7472 792c 2073 7479 6c65 2c20  egistry, style, 
+000192d0: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
+000192e0: 616c 5f70 6f69 6e74 293a 0a20 2020 2020  al_point):.     
+000192f0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00019300: 656e 6465 7220 7468 6973 2070 6174 6820  ender this path 
+00019310: 656c 656d 656e 7420 746f 2069 7473 2050  element to its P
+00019320: 4446 2072 6570 7265 7365 6e74 6174 696f  DF representatio
+00019330: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
+00019340: 3a0a 2020 2020 2020 2020 2020 2020 6773  :.            gs
+00019350: 645f 7265 6769 7374 7279 2028 4772 6170  d_registry (Grap
+00019360: 6869 6373 5374 6174 6544 6963 7452 6567  hicsStateDictReg
+00019370: 6973 7472 7929 3a20 7468 6520 6f77 6e65  istry): the owne
+00019380: 7227 7320 6772 6170 6869 6373 2073 7461  r's graphics sta
+00019390: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
+000193a0: 2020 2064 6963 7469 6f6e 6172 7920 7265     dictionary re
+000193b0: 6769 7374 7279 2e0a 2020 2020 2020 2020  gistry..        
+000193c0: 2020 2020 7374 796c 6520 2847 7261 7068      style (Graph
+000193d0: 6963 7353 7479 6c65 293a 2074 6865 2063  icsStyle): the c
+000193e0: 7572 7265 6e74 2072 6573 6f6c 7665 6420  urrent resolved 
+000193f0: 6772 6170 6869 6373 2073 7479 6c65 0a20  graphics style. 
+00019400: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+00019410: 6974 656d 3a20 7468 6520 7072 6576 696f  item: the previo
+00019420: 7573 2070 6174 6820 656c 656d 656e 742e  us path element.
+00019430: 0a20 2020 2020 2020 2020 2020 2069 6e69  .            ini
+00019440: 7469 616c 5f70 6f69 6e74 3a20 6c61 7374  tial_point: last
+00019450: 2070 6f73 6974 696f 6e20 7365 7420 6279   position set by
+00019460: 2061 2022 4d22 206f 7220 226d 2220 636f   a "M" or "m" co
+00019470: 6d6d 616e 640a 0a20 2020 2020 2020 2052  mmand..        R
+00019480: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00019490: 2020 2020 6120 7475 706c 6520 6f66 2060      a tuple of `
+000194a0: 2873 7472 2c20 6e65 775f 6c61 7374 5f69  (str, new_last_i
+000194b0: 7465 6d29 602c 2077 6865 7265 2060 6e65  tem)`, where `ne
+000194c0: 775f 6c61 7374 5f69 7465 6d60 2069 7320  w_last_item` is 
+000194d0: 7768 6174 6576 6572 2074 6865 206f 6c64  whatever the old
+000194e0: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
+000194f0: 745f 6974 656d 2077 6173 2e0a 2020 2020  t_item was..    
+00019500: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00019510: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+00019520: 653d 756e 7573 6564 2d61 7267 756d 656e  e=unused-argumen
+00019530: 740a 2020 2020 2020 2020 7265 7475 726e  t.        return
+00019540: 2022 6822 2c20 4d6f 7665 2869 6e69 7469   "h", Move(initi
+00019550: 616c 5f70 6f69 6e74 292c 2069 6e69 7469  al_point), initi
+00019560: 616c 5f70 6f69 6e74 0a0a 2020 2020 4066  al_point..    @f
+00019570: 6f72 6365 5f6e 6f64 6f63 756d 656e 740a  orce_nodocument.
+00019580: 2020 2020 6465 6620 7265 6e64 6572 5f64      def render_d
+00019590: 6562 7567 280a 2020 2020 2020 2020 7365  ebug(.        se
+000195a0: 6c66 2c20 6773 645f 7265 6769 7374 7279  lf, gsd_registry
+000195b0: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
+000195c0: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
+000195d0: 742c 2064 6562 7567 5f73 7472 6561 6d2c  t, debug_stream,
+000195e0: 2070 6678 0a20 2020 2029 3a0a 2020 2020   pfx.    ):.    
+000195f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00019600: 5265 6e64 6572 2074 6869 7320 7061 7468  Render this path
+00019610: 2065 6c65 6d65 6e74 2074 6f20 6974 7320   element to its 
+00019620: 5044 4620 7265 7072 6573 656e 7461 7469  PDF representati
+00019630: 6f6e 2061 6e64 2070 726f 6475 6365 2064  on and produce d
+00019640: 6562 7567 0a20 2020 2020 2020 2069 6e66  ebug.        inf
+00019650: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
+00019660: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00019670: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
+00019680: 7920 2847 7261 7068 6963 7353 7461 7465  y (GraphicsState
+00019690: 4469 6374 5265 6769 7374 7279 293a 2074  DictRegistry): t
+000196a0: 6865 206f 776e 6572 2773 2067 7261 7068  he owner's graph
+000196b0: 6963 7320 7374 6174 650a 2020 2020 2020  ics state.      
+000196c0: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
+000196d0: 6e61 7279 2072 6567 6973 7472 792e 0a20  nary registry.. 
+000196e0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+000196f0: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
+00019700: 3a20 7468 6520 6375 7272 656e 7420 7265  : the current re
+00019710: 736f 6c76 6564 2067 7261 7068 6963 7320  solved graphics 
+00019720: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
+00019730: 2020 6c61 7374 5f69 7465 6d3a 2074 6865    last_item: the
+00019740: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
+00019750: 6c65 6d65 6e74 2e0a 2020 2020 2020 2020  lement..        
+00019760: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
+00019770: 743a 206c 6173 7420 706f 7369 7469 6f6e  t: last position
+00019780: 2073 6574 2062 7920 6120 224d 2220 6f72   set by a "M" or
+00019790: 2022 6d22 2063 6f6d 6d61 6e64 0a20 2020   "m" command.   
+000197a0: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
+000197b0: 7472 6561 6d20 2869 6f2e 5465 7874 494f  tream (io.TextIO
+000197c0: 293a 2074 6865 2073 7472 6561 6d20 746f  ): the stream to
+000197d0: 2077 6869 6368 2074 6865 2064 6562 7567   which the debug
+000197e0: 206f 7574 7075 7420 7368 6f75 6c64 2062   output should b
+000197f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00019800: 2020 7772 6974 7465 6e2e 2054 6869 7320    written. This 
+00019810: 6973 206e 6f74 2067 7561 7261 6e74 6565  is not guarantee
+00019820: 6420 746f 2062 6520 7365 656b 6162 6c65  d to be seekable
+00019830: 2028 652e 672e 2069 7420 6d61 7920 6265   (e.g. it may be
+00019840: 2073 7464 6f75 7420 6f72 0a20 2020 2020   stdout or.     
+00019850: 2020 2020 2020 2020 2020 2073 7464 6572             stder
+00019860: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
+00019870: 7066 7820 2873 7472 293a 2074 6865 2063  pfx (str): the c
+00019880: 7572 7265 6e74 2064 6562 7567 206f 7574  urrent debug out
+00019890: 7075 7420 7072 6566 6978 2073 7472 696e  put prefix strin
+000198a0: 6720 286f 6e6c 7920 6e65 6564 6564 2069  g (only needed i
+000198b0: 6620 656d 6974 7469 6e67 0a20 2020 2020  f emitting.     
+000198c0: 2020 2020 2020 2020 2020 206d 6f72 6520             more 
+000198d0: 7468 616e 206f 6e65 206c 696e 6529 2e0a  than one line)..
+000198e0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000198f0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00019900: 6520 7361 6d65 2074 7570 6c65 2061 7320  e same tuple as 
+00019910: 6043 6c6f 7365 2e72 656e 6465 7260 2e0a  `Close.render`..
+00019920: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00019930: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
+00019940: 7361 626c 653d 756e 7573 6564 2d61 7267  sable=unused-arg
+00019950: 756d 656e 740a 2020 2020 2020 2020 7265  ument.        re
+00019960: 6e64 6572 6564 2c20 7265 736f 6c76 6564  ndered, resolved
+00019970: 2c20 696e 6974 6961 6c5f 706f 696e 7420  , initial_point 
+00019980: 3d20 7365 6c66 2e72 656e 6465 7228 0a20  = self.render(. 
+00019990: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
+000199a0: 6567 6973 7472 792c 2073 7479 6c65 2c20  egistry, style, 
+000199b0: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
+000199c0: 616c 5f70 6f69 6e74 0a20 2020 2020 2020  al_point.       
+000199d0: 2029 0a20 2020 2020 2020 2064 6562 7567   ).        debug
+000199e0: 5f73 7472 6561 6d2e 7772 6974 6528 7374  _stream.write(st
+000199f0: 7228 7365 6c66 2920 2b20 225c 6e22 290a  r(self) + "\n").
+00019a00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019a10: 7265 6e64 6572 6564 2c20 7265 736f 6c76  rendered, resolv
+00019a20: 6564 2c20 696e 6974 6961 6c5f 706f 696e  ed, initial_poin
+00019a30: 740a 0a0a 636c 6173 7320 4472 6177 696e  t...class Drawin
+00019a40: 6743 6f6e 7465 7874 3a0a 2020 2020 2222  gContext:.    ""
+00019a50: 220a 2020 2020 4261 7365 2063 6f6e 7465  ".    Base conte
+00019a60: 7874 2066 6f72 2061 2064 7261 7769 6e67  xt for a drawing
+00019a70: 2069 6e20 6120 5044 460a 0a20 2020 2054   in a PDF..    T
+00019a80: 6869 7320 636f 6e74 6578 7420 6973 206e  his context is n
+00019a90: 6f74 2073 7479 6c61 626c 6520 616e 6420  ot stylable and 
+00019aa0: 6973 206d 6169 6e6c 7920 7265 7370 6f6e  is mainly respon
+00019ab0: 7369 626c 6520 666f 7220 7472 616e 7366  sible for transf
+00019ac0: 6f72 6d69 6e67 2070 6174 680a 2020 2020  orming path.    
+00019ad0: 6472 6177 696e 6720 636f 6f72 6469 6e61  drawing coordina
+00019ae0: 7465 7320 696e 746f 2075 7365 7220 636f  tes into user co
+00019af0: 6f72 6469 6e61 7465 7320 2869 2e65 2e20  ordinates (i.e. 
+00019b00: 6974 2065 6e73 7572 6573 2074 6861 7420  it ensures that 
+00019b10: 7468 6520 6f75 7470 7574 2064 7261 7769  the output drawi
+00019b20: 6e67 0a20 2020 2069 7320 636f 7272 6563  ng.    is correc
+00019b30: 746c 7920 7363 616c 6564 292e 0a20 2020  tly scaled)..   
+00019b40: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00019b50: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+00019b60: 2020 2020 2020 7365 6c66 2e5f 7375 6269        self._subi
+00019b70: 7465 6d73 203d 205b 5d0a 0a20 2020 2064  tems = []..    d
+00019b80: 6566 2061 6464 5f69 7465 6d28 7365 6c66  ef add_item(self
+00019b90: 2c20 6974 656d 2c20 5f63 6f70 793d 5472  , item, _copy=Tr
+00019ba0: 7565 293a 0a20 2020 2020 2020 2022 2222  ue):.        """
+00019bb0: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
+00019bc0: 616e 2069 7465 6d20 746f 2074 6869 7320  an item to this 
+00019bd0: 6472 6177 696e 6720 636f 6e74 6578 740a  drawing context.
+00019be0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00019bf0: 2020 2020 2020 2020 2020 2069 7465 6d20             item 
+00019c00: 2847 7261 7068 6963 7343 6f6e 7465 7874  (GraphicsContext
+00019c10: 2c20 5061 696e 7465 6450 6174 6829 3a20  , PaintedPath): 
+00019c20: 7468 6520 6974 656d 2074 6f20 6265 2061  the item to be a
+00019c30: 7070 656e 6465 642e 0a20 2020 2020 2020  ppended..       
+00019c40: 2020 2020 205f 636f 7079 2028 626f 6f6c       _copy (bool
+00019c50: 293a 2069 6620 7472 7565 2028 7468 6520  ): if true (the 
+00019c60: 6465 6661 756c 7429 2c20 7468 6520 6974  default), the it
+00019c70: 656d 2077 696c 6c20 6265 2063 6f70 6965  em will be copie
+00019c80: 6420 6265 666f 7265 2062 6569 6e67 0a20  d before being. 
+00019c90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00019ca0: 7070 656e 6465 642e 2054 6869 7320 7072  ppended. This pr
+00019cb0: 6576 656e 7473 206d 6f64 6966 6963 6174  events modificat
+00019cc0: 696f 6e73 2074 6f20 6120 7265 6665 7265  ions to a refere
+00019cd0: 6e63 6564 206f 626a 6563 7420 6672 6f6d  nced object from
+00019ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019cf0: 2022 7265 7472 6f61 6374 6976 656c 7922   "retroactively"
+00019d00: 2061 6c74 6572 696e 6720 6974 7320 7374   altering its st
+00019d10: 796c 652f 7368 6170 6520 616e 6420 7368  yle/shape and sh
+00019d20: 6f75 6c64 2062 6520 6469 7361 626c 6564  ould be disabled
+00019d30: 2077 6974 680a 2020 2020 2020 2020 2020   with.          
+00019d40: 2020 2020 2020 6361 7574 696f 6e2e 0a20        caution.. 
+00019d50: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00019d60: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00019d70: 7461 6e63 6528 6974 656d 2c20 2847 7261  tance(item, (Gra
+00019d80: 7068 6963 7343 6f6e 7465 7874 2c20 5061  phicsContext, Pa
+00019d90: 696e 7465 6450 6174 6829 293a 0a20 2020  intedPath)):.   
+00019da0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00019db0: 7970 6545 7272 6f72 2866 227b 6974 656d  ypeError(f"{item
+00019dc0: 7d20 646f 6573 6e27 7420 6265 6c6f 6e67  } doesn't belong
+00019dd0: 2069 6e20 6120 4472 6177 696e 6743 6f6e   in a DrawingCon
+00019de0: 7465 7874 2229 0a0a 2020 2020 2020 2020  text")..        
+00019df0: 6966 205f 636f 7079 3a0a 2020 2020 2020  if _copy:.      
+00019e00: 2020 2020 2020 6974 656d 203d 2063 6f70        item = cop
+00019e10: 792e 6465 6570 636f 7079 2869 7465 6d29  y.deepcopy(item)
+00019e20: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00019e30: 7375 6269 7465 6d73 2e61 7070 656e 6428  subitems.append(
+00019e40: 6974 656d 290a 0a20 2020 2040 7374 6174  item)..    @stat
+00019e50: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+00019e60: 205f 7365 7475 705f 7265 6e64 6572 5f70   _setup_render_p
+00019e70: 7265 7265 7173 2873 7479 6c65 2c20 6669  rereqs(style, fi
+00019e80: 7273 745f 706f 696e 742c 2073 6361 6c65  rst_point, scale
+00019e90: 2c20 6865 6967 6874 293a 0a20 2020 2020  , height):.     
+00019ea0: 2020 2073 7479 6c65 2e61 7574 6f5f 636c     style.auto_cl
+00019eb0: 6f73 6520 3d20 5472 7565 0a20 2020 2020  ose = True.     
+00019ec0: 2020 2073 7479 6c65 2e70 6169 6e74 5f72     style.paint_r
+00019ed0: 756c 6520 3d20 5061 7468 5061 696e 7452  ule = PathPaintR
+00019ee0: 756c 652e 4155 544f 0a20 2020 2020 2020  ule.AUTO.       
+00019ef0: 2073 7479 6c65 2e69 6e74 6572 7365 6374   style.intersect
+00019f00: 696f 6e5f 7275 6c65 203d 2049 6e74 6572  ion_rule = Inter
+00019f10: 7365 6374 696f 6e52 756c 652e 4e4f 4e5a  sectionRule.NONZ
+00019f20: 4552 4f0a 0a20 2020 2020 2020 206c 6173  ERO..        las
+00019f30: 745f 6974 656d 203d 204d 6f76 6528 6669  t_item = Move(fi
+00019f40: 7273 745f 706f 696e 7429 0a20 2020 2020  rst_point).     
+00019f50: 2020 2073 6361 6c65 2c20 6c61 7374 5f69     scale, last_i
+00019f60: 7465 6d20 3d20 280a 2020 2020 2020 2020  tem = (.        
+00019f70: 2020 2020 5472 616e 7366 6f72 6d2e 7363      Transform.sc
+00019f80: 616c 696e 6728 783d 312c 2079 3d2d 3129  aling(x=1, y=-1)
+00019f90: 0a20 2020 2020 2020 2020 2020 202e 6162  .            .ab
+00019fa0: 6f75 7428 783d 302c 2079 3d68 6569 6768  out(x=0, y=heigh
+00019fb0: 7420 2f20 3229 0a20 2020 2020 2020 2020  t / 2).         
+00019fc0: 2020 202e 7363 616c 6528 7363 616c 6529     .scale(scale)
+00019fd0: 0a20 2020 2020 2020 2020 2020 202e 7265  .            .re
+00019fe0: 6e64 6572 286c 6173 745f 6974 656d 290a  nder(last_item).
+00019ff0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001a000: 2020 2072 656e 6465 725f 6c69 7374 203d     render_list =
+0001a010: 205b 2271 222c 2073 6361 6c65 5d0a 0a20   ["q", scale].. 
+0001a020: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0001a030: 6e64 6572 5f6c 6973 742c 2073 7479 6c65  nder_list, style
+0001a040: 2c20 6c61 7374 5f69 7465 6d0a 0a20 2020  , last_item..   
+0001a050: 2064 6566 2072 656e 6465 7228 7365 6c66   def render(self
+0001a060: 2c20 6773 645f 7265 6769 7374 7279 2c20  , gsd_registry, 
+0001a070: 6669 7273 745f 706f 696e 742c 2073 6361  first_point, sca
+0001a080: 6c65 2c20 6865 6967 6874 2c20 7374 6172  le, height, star
+0001a090: 7469 6e67 5f73 7479 6c65 293a 0a20 2020  ting_style):.   
+0001a0a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001a0b0: 2052 656e 6465 7220 7468 6520 6472 6177   Render the draw
+0001a0c0: 696e 6720 636f 6e74 6578 7420 746f 2050  ing context to P
+0001a0d0: 4446 2066 6f72 6d61 742e 0a0a 2020 2020  DF format...    
+0001a0e0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0001a0f0: 2020 2020 2020 6773 645f 7265 6769 7374        gsd_regist
+0001a100: 7279 2028 4772 6170 6869 6373 5374 6174  ry (GraphicsStat
+0001a110: 6544 6963 7452 6567 6973 7472 7929 3a20  eDictRegistry): 
+0001a120: 7468 6520 7061 7265 6e74 2064 6f63 756d  the parent docum
+0001a130: 656e 7427 7320 6772 6170 6869 6373 0a20  ent's graphics. 
+0001a140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a150: 7461 7465 2072 6567 6973 7472 792e 0a20  tate registry.. 
+0001a160: 2020 2020 2020 2020 2020 2066 6972 7374             first
+0001a170: 5f70 6f69 6e74 2028 506f 696e 7429 3a20  _point (Point): 
+0001a180: 7468 6520 7374 6172 7469 6e67 2070 6f69  the starting poi
+0001a190: 6e74 2074 6f20 7573 6520 6966 2074 6865  nt to use if the
+0001a1a0: 2066 6972 7374 2070 6174 6820 656c 656d   first path elem
+0001a1b0: 656e 7420 6973 0a20 2020 2020 2020 2020  ent is.         
+0001a1c0: 2020 2020 2020 2061 2072 656c 6174 6976         a relativ
+0001a1d0: 6520 656c 656d 656e 742e 0a20 2020 2020  e element..     
+0001a1e0: 2020 2020 2020 2073 6361 6c65 2028 4e75         scale (Nu
+0001a1f0: 6d62 6572 293a 2074 6865 2073 6361 6c65  mber): the scale
+0001a200: 2066 6163 746f 7220 746f 2063 6f6e 7665   factor to conve
+0001a210: 7274 2066 726f 6d20 5044 4620 7074 2075  rt from PDF pt u
+0001a220: 6e69 7473 2069 6e74 6f20 7468 650a 2020  nits into the.  
+0001a230: 2020 2020 2020 2020 2020 2020 2020 646f                do
+0001a240: 6375 6d65 6e74 2773 2073 656d 616e 7469  cument's semanti
+0001a250: 6320 756e 6974 7320 2865 2e67 2e20 6d6d  c units (e.g. mm
+0001a260: 206f 7220 696e 292e 0a20 2020 2020 2020   or in)..       
+0001a270: 2020 2020 2068 6569 6768 7420 284e 756d       height (Num
+0001a280: 6265 7229 3a20 7468 6520 7061 6765 2068  ber): the page h
+0001a290: 6569 6768 742e 2054 6869 7320 6973 2075  eight. This is u
+0001a2a0: 7365 6420 746f 2072 656d 6170 2074 6865  sed to remap the
+0001a2b0: 2063 6f6f 7264 696e 6174 6573 2074 6f0a   coordinates to.
+0001a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2d0: 6265 2066 726f 6d20 7468 6520 746f 702d  be from the top-
+0001a2e0: 6c65 6674 2063 6f72 6e65 7220 6f66 2074  left corner of t
+0001a2f0: 6865 2070 6167 6520 286d 6174 6368 696e  he page (matchin
+0001a300: 6720 6670 6466 2773 2062 6568 6176 696f  g fpdf's behavio
+0001a310: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+0001a320: 2020 2069 6e73 7465 6164 206f 6620 7468     instead of th
+0001a330: 6520 5044 4620 6e61 7469 7665 2062 6568  e PDF native beh
+0001a340: 6176 696f 7220 6f66 2062 6f74 746f 6d2d  avior of bottom-
+0001a350: 6c65 6674 2e0a 2020 2020 2020 2020 2020  left..          
+0001a360: 2020 7374 6172 7469 6e67 5f73 7479 6c65    starting_style
+0001a370: 2028 4772 6170 6869 6373 5374 796c 6529   (GraphicsStyle)
+0001a380: 3a20 7468 6520 6261 7365 2073 7479 6c65  : the base style
+0001a390: 2066 6f72 2074 6869 7320 6472 6177 696e   for this drawin
+0001a3a0: 6720 636f 6e74 6578 742c 0a20 2020 2020  g context,.     
+0001a3b0: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
+0001a3c0: 6564 2066 726f 6d20 7468 6520 646f 6375  ed from the docu
+0001a3d0: 6d65 6e74 2773 2063 7572 7265 6e74 2073  ment's current s
+0001a3e0: 7479 6c65 2064 6566 6175 6c74 732e 0a0a  tyle defaults...
+0001a3f0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0001a400: 0a20 2020 2020 2020 2020 2020 2041 2073  .            A s
+0001a410: 7472 696e 6720 636f 6d70 6f73 6564 206f  tring composed o
+0001a420: 6620 7468 6520 5044 4620 7265 7072 6573  f the PDF repres
+0001a430: 656e 7461 7469 6f6e 206f 6620 616c 6c20  entation of all 
+0001a440: 7468 6520 7061 7468 7320 616e 6420 6772  the paths and gr
+0001a450: 6f75 7073 2069 6e0a 2020 2020 2020 2020  oups in.        
+0001a460: 2020 2020 7468 6973 2063 6f6e 7465 7874      this context
+0001a470: 2028 616e 2065 6d70 7479 2073 7472 696e   (an empty strin
+0001a480: 6720 6973 2072 6574 7572 6e65 6420 6966  g is returned if
+0001a490: 2074 6865 7265 2061 7265 206e 6f20 7061   there are no pa
+0001a4a0: 7468 7320 6f72 2067 726f 7570 7329 0a20  ths or groups). 
+0001a4b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001a4c0: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
+0001a4d0: 7375 6269 7465 6d73 3a0a 2020 2020 2020  subitems:.      
+0001a4e0: 2020 2020 2020 7265 7475 726e 2022 220a        return "".
+0001a4f0: 0a20 2020 2020 2020 2072 656e 6465 725f  .        render_
+0001a500: 6c69 7374 2c20 7374 796c 652c 206c 6173  list, style, las
+0001a510: 745f 6974 656d 203d 2073 656c 662e 5f73  t_item = self._s
+0001a520: 6574 7570 5f72 656e 6465 725f 7072 6572  etup_render_prer
+0001a530: 6571 7328 0a20 2020 2020 2020 2020 2020  eqs(.           
+0001a540: 2073 7461 7274 696e 675f 7374 796c 652c   starting_style,
+0001a550: 2066 6972 7374 5f70 6f69 6e74 2c20 7363   first_point, sc
+0001a560: 616c 652c 2068 6569 6768 740a 2020 2020  ale, height.    
+0001a570: 2020 2020 290a 0a20 2020 2020 2020 2066      )..        f
+0001a580: 6f72 2069 7465 6d20 696e 2073 656c 662e  or item in self.
+0001a590: 5f73 7562 6974 656d 733a 0a20 2020 2020  _subitems:.     
+0001a5a0: 2020 2020 2020 2072 656e 6465 7265 642c         rendered,
+0001a5b0: 206c 6173 745f 6974 656d 2c20 6669 7273   last_item, firs
+0001a5c0: 745f 706f 696e 7420 3d20 6974 656d 2e72  t_point = item.r
+0001a5d0: 656e 6465 7228 0a20 2020 2020 2020 2020  ender(.         
+0001a5e0: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
+0001a5f0: 7472 792c 2073 7479 6c65 2c20 6c61 7374  try, style, last
+0001a600: 5f69 7465 6d2c 2066 6972 7374 5f70 6f69  _item, first_poi
+0001a610: 6e74 0a20 2020 2020 2020 2020 2020 2029  nt.            )
+0001a620: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a630: 7265 6e64 6572 6564 3a0a 2020 2020 2020  rendered:.      
+0001a640: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+0001a650: 5f6c 6973 742e 6170 7065 6e64 2872 656e  _list.append(ren
+0001a660: 6465 7265 6429 0a0a 2020 2020 2020 2020  dered)..        
+0001a670: 2320 7468 6572 6520 7761 7320 6e6f 7468  # there was noth
+0001a680: 696e 6720 746f 2072 656e 6465 723a 2074  ing to render: t
+0001a690: 6865 206f 6e6c 7920 6974 656d 7320 6172  he only items ar
+0001a6a0: 6520 7468 6520 7374 6172 7420 6772 6f75  e the start grou
+0001a6b0: 7020 616e 6420 7363 616c 650a 2020 2020  p and scale.    
+0001a6c0: 2020 2020 2320 7472 616e 7366 6f72 6d2e      # transform.
+0001a6d0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0001a6e0: 7265 6e64 6572 5f6c 6973 7429 203d 3d20  render_list) == 
+0001a6f0: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
+0001a700: 6574 7572 6e20 2222 0a0a 2020 2020 2020  eturn ""..      
+0001a710: 2020 7374 796c 655f 6469 6374 5f6e 616d    style_dict_nam
+0001a720: 6520 3d20 6773 645f 7265 6769 7374 7279  e = gsd_registry
+0001a730: 2e72 6567 6973 7465 725f 7374 796c 6528  .register_style(
+0001a740: 7374 796c 6529 0a0a 2020 2020 2020 2020  style)..        
+0001a750: 6966 2073 7479 6c65 5f64 6963 745f 6e61  if style_dict_na
+0001a760: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+0001a770: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
+0001a780: 6572 5f6c 6973 742e 696e 7365 7274 2832  er_list.insert(2
+0001a790: 2c20 6622 7b72 656e 6465 725f 7064 665f  , f"{render_pdf_
+0001a7a0: 7072 696d 6974 6976 6528 7374 796c 655f  primitive(style_
+0001a7b0: 6469 6374 5f6e 616d 6529 7d20 6773 2229  dict_name)} gs")
+0001a7c0: 0a20 2020 2020 2020 2020 2020 2072 656e  .            ren
+0001a7d0: 6465 725f 6c69 7374 2e69 6e73 6572 7428  der_list.insert(
+0001a7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a7f0: 2033 2c0a 2020 2020 2020 2020 2020 2020   3,.            
+0001a800: 2020 2020 7265 6e64 6572 5f70 6466 5f70      render_pdf_p
+0001a810: 7269 6d69 7469 7665 2873 7479 6c65 2e73  rimitive(style.s
+0001a820: 7472 6f6b 655f 6461 7368 5f70 6174 7465  troke_dash_patte
+0001a830: 726e 290a 2020 2020 2020 2020 2020 2020  rn).            
+0001a840: 2020 2020 2b20 6622 207b 6e75 6d62 6572      + f" {number
+0001a850: 5f74 6f5f 7374 7228 7374 796c 652e 7374  _to_str(style.st
+0001a860: 726f 6b65 5f64 6173 685f 7068 6173 6529  roke_dash_phase)
+0001a870: 7d20 6422 2c0a 2020 2020 2020 2020 2020  } d",.          
+0001a880: 2020 290a 0a20 2020 2020 2020 2072 656e    )..        ren
+0001a890: 6465 725f 6c69 7374 2e61 7070 656e 6428  der_list.append(
+0001a8a0: 2251 2229 0a0a 2020 2020 2020 2020 7265  "Q")..        re
+0001a8b0: 7475 726e 2022 2022 2e6a 6f69 6e28 7265  turn " ".join(re
+0001a8c0: 6e64 6572 5f6c 6973 7429 0a0a 2020 2020  nder_list)..    
+0001a8d0: 6465 6620 7265 6e64 6572 5f64 6562 7567  def render_debug
+0001a8e0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+0001a8f0: 6773 645f 7265 6769 7374 7279 2c20 6669  gsd_registry, fi
+0001a900: 7273 745f 706f 696e 742c 2073 6361 6c65  rst_point, scale
+0001a910: 2c20 6865 6967 6874 2c20 7374 6172 7469  , height, starti
+0001a920: 6e67 5f73 7479 6c65 2c20 6465 6275 675f  ng_style, debug_
+0001a930: 7374 7265 616d 0a20 2020 2029 3a0a 2020  stream.    ):.  
+0001a940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001a950: 2020 5265 6e64 6572 2074 6865 2064 7261    Render the dra
+0001a960: 7769 6e67 2063 6f6e 7465 7874 2074 6f20  wing context to 
+0001a970: 5044 4620 666f 726d 6174 2e0a 0a20 2020  PDF format...   
+0001a980: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0001a990: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
+0001a9a0: 7472 7920 2847 7261 7068 6963 7353 7461  try (GraphicsSta
+0001a9b0: 7465 4469 6374 5265 6769 7374 7279 293a  teDictRegistry):
+0001a9c0: 2074 6865 2070 6172 656e 7420 646f 6375   the parent docu
+0001a9d0: 6d65 6e74 2773 2067 7261 7068 6963 730a  ment's graphics.
+0001a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9f0: 7374 6174 6520 7265 6769 7374 7279 2e0a  state registry..
+0001aa00: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+0001aa10: 745f 706f 696e 7420 2850 6f69 6e74 293a  t_point (Point):
+0001aa20: 2074 6865 2073 7461 7274 696e 6720 706f   the starting po
+0001aa30: 696e 7420 746f 2075 7365 2069 6620 7468  int to use if th
+0001aa40: 6520 6669 7273 7420 7061 7468 2065 6c65  e first path ele
+0001aa50: 6d65 6e74 2069 730a 2020 2020 2020 2020  ment is.        
+0001aa60: 2020 2020 2020 2020 6120 7265 6c61 7469          a relati
+0001aa70: 7665 2065 6c65 6d65 6e74 2e0a 2020 2020  ve element..    
+0001aa80: 2020 2020 2020 2020 7363 616c 6520 284e          scale (N
+0001aa90: 756d 6265 7229 3a20 7468 6520 7363 616c  umber): the scal
+0001aaa0: 6520 6661 6374 6f72 2074 6f20 636f 6e76  e factor to conv
+0001aab0: 6572 7420 6672 6f6d 2050 4446 2070 7420  ert from PDF pt 
+0001aac0: 756e 6974 7320 696e 746f 2074 6865 0a20  units into the. 
+0001aad0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001aae0: 6f63 756d 656e 7427 7320 7365 6d61 6e74  ocument's semant
+0001aaf0: 6963 2075 6e69 7473 2028 652e 672e 206d  ic units (e.g. m
+0001ab00: 6d20 6f72 2069 6e29 2e0a 2020 2020 2020  m or in)..      
+0001ab10: 2020 2020 2020 6865 6967 6874 2028 4e75        height (Nu
+0001ab20: 6d62 6572 293a 2074 6865 2070 6167 6520  mber): the page 
+0001ab30: 6865 6967 6874 2e20 5468 6973 2069 7320  height. This is 
+0001ab40: 7573 6564 2074 6f20 7265 6d61 7020 7468  used to remap th
+0001ab50: 6520 636f 6f72 6469 6e61 7465 7320 746f  e coordinates to
+0001ab60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ab70: 2062 6520 6672 6f6d 2074 6865 2074 6f70   be from the top
+0001ab80: 2d6c 6566 7420 636f 726e 6572 206f 6620  -left corner of 
+0001ab90: 7468 6520 7061 6765 2028 6d61 7463 6869  the page (matchi
+0001aba0: 6e67 2066 7064 6627 7320 6265 6861 7669  ng fpdf's behavi
+0001abb0: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+0001abc0: 2020 2020 696e 7374 6561 6420 6f66 2074      instead of t
+0001abd0: 6865 2050 4446 206e 6174 6976 6520 6265  he PDF native be
+0001abe0: 6861 7669 6f72 206f 6620 626f 7474 6f6d  havior of bottom
+0001abf0: 2d6c 6566 742e 0a20 2020 2020 2020 2020  -left..         
+0001ac00: 2020 2073 7461 7274 696e 675f 7374 796c     starting_styl
+0001ac10: 6520 2847 7261 7068 6963 7353 7479 6c65  e (GraphicsStyle
+0001ac20: 293a 2074 6865 2062 6173 6520 7374 796c  ): the base styl
+0001ac30: 6520 666f 7220 7468 6973 2064 7261 7769  e for this drawi
+0001ac40: 6e67 2063 6f6e 7465 7874 2c0a 2020 2020  ng context,.    
+0001ac50: 2020 2020 2020 2020 2020 2020 6465 7269              deri
+0001ac60: 7665 6420 6672 6f6d 2074 6865 2064 6f63  ved from the doc
+0001ac70: 756d 656e 7427 7320 6375 7272 656e 7420  ument's current 
+0001ac80: 7374 796c 6520 6465 6661 756c 7473 2e0a  style defaults..
+0001ac90: 2020 2020 2020 2020 2020 2020 6465 6275              debu
+0001aca0: 675f 7374 7265 616d 2028 5465 7874 494f  g_stream (TextIO
+0001acb0: 293a 2061 2074 6578 7420 7374 7265 616d  ): a text stream
+0001acc0: 2074 6f20 7768 6963 6820 6120 6465 6275   to which a debu
+0001acd0: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
+0001ace0: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+0001acf0: 2020 2020 2020 2020 6472 6177 696e 6720          drawing 
+0001ad00: 7374 7275 6374 7572 6520 7769 6c6c 2062  structure will b
+0001ad10: 6520 7772 6974 7465 6e2e 0a0a 2020 2020  e written...    
+0001ad20: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0001ad30: 2020 2020 2020 2020 2041 2073 7472 696e           A strin
+0001ad40: 6720 636f 6d70 6f73 6564 206f 6620 7468  g composed of th
+0001ad50: 6520 5044 4620 7265 7072 6573 656e 7461  e PDF representa
+0001ad60: 7469 6f6e 206f 6620 616c 6c20 7468 6520  tion of all the 
+0001ad70: 7061 7468 7320 616e 6420 6772 6f75 7073  paths and groups
+0001ad80: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+0001ad90: 7468 6973 2063 6f6e 7465 7874 2028 616e  this context (an
+0001ada0: 2065 6d70 7479 2073 7472 696e 6720 6973   empty string is
+0001adb0: 2072 6574 7572 6e65 6420 6966 2074 6865   returned if the
+0001adc0: 7265 2061 7265 206e 6f20 7061 7468 7320  re are no paths 
+0001add0: 6f72 2067 726f 7570 7329 0a20 2020 2020  or groups).     
+0001ade0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0001adf0: 656e 6465 725f 6c69 7374 2c20 7374 796c  ender_list, styl
+0001ae00: 652c 206c 6173 745f 6974 656d 203d 2073  e, last_item = s
+0001ae10: 656c 662e 5f73 6574 7570 5f72 656e 6465  elf._setup_rende
+0001ae20: 725f 7072 6572 6571 7328 0a20 2020 2020  r_prereqs(.     
+0001ae30: 2020 2020 2020 2073 7461 7274 696e 675f         starting_
+0001ae40: 7374 796c 652c 2066 6972 7374 5f70 6f69  style, first_poi
+0001ae50: 6e74 2c20 7363 616c 652c 2068 6569 6768  nt, scale, heigh
+0001ae60: 740a 2020 2020 2020 2020 290a 0a20 2020  t.        )..   
+0001ae70: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+0001ae80: 6d2e 7772 6974 6528 2252 4f4f 545c 6e22  m.write("ROOT\n"
+0001ae90: 290a 2020 2020 2020 2020 666f 7220 6368  ).        for ch
+0001aea0: 696c 6420 696e 2073 656c 662e 5f73 7562  ild in self._sub
+0001aeb0: 6974 656d 735b 3a2d 315d 3a0a 2020 2020  items[:-1]:.    
+0001aec0: 2020 2020 2020 2020 6465 6275 675f 7374          debug_st
+0001aed0: 7265 616d 2e77 7269 7465 2822 20e2 949c  ream.write(" ...
+0001aee0: e294 8020 2229 0a20 2020 2020 2020 2020  ... ").         
+0001aef0: 2020 2072 656e 6465 7265 642c 206c 6173     rendered, las
+0001af00: 745f 6974 656d 203d 2063 6869 6c64 2e72  t_item = child.r
+0001af10: 656e 6465 725f 6465 6275 6728 0a20 2020  ender_debug(.   
+0001af20: 2020 2020 2020 2020 2020 2020 2067 7364               gsd
+0001af30: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
+0001af40: 2c20 6c61 7374 5f69 7465 6d2c 2064 6562  , last_item, deb
+0001af50: 7567 5f73 7472 6561 6d2c 2022 20e2 9482  ug_stream, " ...
+0001af60: 2020 220a 2020 2020 2020 2020 2020 2020    ".            
+0001af70: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001af80: 2072 656e 6465 7265 643a 0a20 2020 2020   rendered:.     
+0001af90: 2020 2020 2020 2020 2020 2072 656e 6465             rende
+0001afa0: 725f 6c69 7374 2e61 7070 656e 6428 7265  r_list.append(re
+0001afb0: 6e64 6572 6564 290a 0a20 2020 2020 2020  ndered)..       
+0001afc0: 2069 6620 7365 6c66 2e5f 7375 6269 7465   if self._subite
+0001afd0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+0001afe0: 6465 6275 675f 7374 7265 616d 2e77 7269  debug_stream.wri
+0001aff0: 7465 2822 20e2 9494 e294 8020 2229 0a20  te(" ...... "). 
+0001b000: 2020 2020 2020 2020 2020 2072 656e 6465             rende
+0001b010: 7265 642c 206c 6173 745f 6974 656d 2c20  red, last_item, 
+0001b020: 6669 7273 745f 706f 696e 7420 3d20 7365  first_point = se
+0001b030: 6c66 2e5f 7375 6269 7465 6d73 5b2d 315d  lf._subitems[-1]
+0001b040: 2e72 656e 6465 725f 6465 6275 6728 0a20  .render_debug(. 
+0001b050: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0001b060: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
+0001b070: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2066  le, last_item, f
+0001b080: 6972 7374 5f70 6f69 6e74 2c20 6465 6275  irst_point, debu
+0001b090: 675f 7374 7265 616d 2c20 2220 2020 2022  g_stream, "    "
+0001b0a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0001b0b0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+0001b0c0: 6e64 6572 6564 3a0a 2020 2020 2020 2020  ndered:.        
+0001b0d0: 2020 2020 2020 2020 7265 6e64 6572 5f6c          render_l
+0001b0e0: 6973 742e 6170 7065 6e64 2872 656e 6465  ist.append(rende
+0001b0f0: 7265 6429 0a0a 2020 2020 2020 2020 2020  red)..          
+0001b100: 2020 2320 7468 6572 6520 7761 7320 6e6f    # there was no
+0001b110: 7468 696e 6720 746f 2072 656e 6465 723a  thing to render:
+0001b120: 2074 6865 206f 6e6c 7920 6974 656d 7320   the only items 
+0001b130: 6172 6520 7468 6520 7374 6172 7420 6772  are the start gr
+0001b140: 6f75 7020 616e 6420 7363 616c 650a 2020  oup and scale.  
+0001b150: 2020 2020 2020 2020 2020 2320 7472 616e            # tran
+0001b160: 7366 6f72 6d2e 0a20 2020 2020 2020 2020  sform..         
+0001b170: 2020 2069 6620 6c65 6e28 7265 6e64 6572     if len(render
+0001b180: 5f6c 6973 7429 203d 3d20 323a 0a20 2020  _list) == 2:.   
+0001b190: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001b1a0: 7572 6e20 2222 0a0a 2020 2020 2020 2020  urn ""..        
+0001b1b0: 2020 2020 7374 796c 655f 6469 6374 5f6e      style_dict_n
+0001b1c0: 616d 6520 3d20 6773 645f 7265 6769 7374  ame = gsd_regist
+0001b1d0: 7279 2e72 6567 6973 7465 725f 7374 796c  ry.register_styl
+0001b1e0: 6528 7374 796c 6529 0a0a 2020 2020 2020  e(style)..      
+0001b1f0: 2020 2020 2020 6966 2073 7479 6c65 5f64        if style_d
+0001b200: 6963 745f 6e61 6d65 2069 7320 6e6f 7420  ict_name is not 
+0001b210: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001b220: 2020 2020 2020 7265 6e64 6572 5f6c 6973        render_lis
+0001b230: 742e 696e 7365 7274 2832 2c20 6622 7b72  t.insert(2, f"{r
+0001b240: 656e 6465 725f 7064 665f 7072 696d 6974  ender_pdf_primit
+0001b250: 6976 6528 7374 796c 655f 6469 6374 5f6e  ive(style_dict_n
+0001b260: 616d 6529 7d20 6773 2229 0a20 2020 2020  ame)} gs").     
+0001b270: 2020 2020 2020 2020 2020 2072 656e 6465             rende
+0001b280: 725f 6c69 7374 2e69 6e73 6572 7428 0a20  r_list.insert(. 
+0001b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2a0: 2020 2033 2c0a 2020 2020 2020 2020 2020     3,.          
+0001b2b0: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+0001b2c0: 5f70 6466 5f70 7269 6d69 7469 7665 2873  _pdf_primitive(s
+0001b2d0: 7479 6c65 2e73 7472 6f6b 655f 6461 7368  tyle.stroke_dash
+0001b2e0: 5f70 6174 7465 726e 290a 2020 2020 2020  _pattern).      
+0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001b300: 6622 207b 6e75 6d62 6572 5f74 6f5f 7374  f" {number_to_st
+0001b310: 7228 7374 796c 652e 7374 726f 6b65 5f64  r(style.stroke_d
+0001b320: 6173 685f 7068 6173 6529 7d20 6422 2c0a  ash_phase)} d",.
+0001b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b340: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0001b350: 656e 6465 725f 6c69 7374 2e61 7070 656e  ender_list.appen
+0001b360: 6428 2251 2229 0a0a 2020 2020 2020 2020  d("Q")..        
+0001b370: 2020 2020 7265 7475 726e 2022 2022 2e6a      return " ".j
+0001b380: 6f69 6e28 7265 6e64 6572 5f6c 6973 7429  oin(render_list)
+0001b390: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001b3a0: 2022 220a 0a0a 636c 6173 7320 5061 696e   ""...class Pain
+0001b3b0: 7465 6450 6174 683a 0a20 2020 2022 2222  tedPath:.    """
+0001b3c0: 0a20 2020 2041 2070 6174 6820 746f 2062  .    A path to b
+0001b3d0: 6520 6472 6177 6e20 6279 2074 6865 2050  e drawn by the P
+0001b3e0: 4446 2072 656e 6465 7265 722e 0a0a 2020  DF renderer...  
+0001b3f0: 2020 4120 7061 696e 7465 6420 7061 7468    A painted path
+0001b400: 2069 7320 6465 6669 6e65 6420 6279 2061   is defined by a
+0001b410: 2073 7479 6c65 2061 6e64 2061 6e20 6172   style and an ar
+0001b420: 6269 7472 6172 7920 7365 7175 656e 6365  bitrary sequence
+0001b430: 206f 6620 7061 7468 2065 6c65 6d65 6e74   of path element
+0001b440: 732c 0a20 2020 2077 6869 6368 2069 6e63  s,.    which inc
+0001b450: 6c75 6465 2074 6865 2070 7269 6d69 7469  lude the primiti
+0001b460: 7665 2070 6174 6820 656c 656d 656e 7473  ve path elements
+0001b470: 2028 604d 6f76 6560 2c20 604c 696e 6560   (`Move`, `Line`
+0001b480: 2c20 6042 657a 6965 7243 7572 7665 602c  , `BezierCurve`,
+0001b490: 202e 2e2e 2920 6173 0a20 2020 2077 656c   ...) as.    wel
+0001b4a0: 6c20 6173 2061 7262 6974 7261 7269 6c79  l as arbitrarily
+0001b4b0: 206e 6573 7465 6420 6047 7261 7068 6963   nested `Graphic
+0001b4c0: 7343 6f6e 7465 7874 6020 636f 6e74 6169  sContext` contai
+0001b4d0: 6e69 6e67 2074 6865 6972 206f 776e 2073  ning their own s
+0001b4e0: 6571 7565 6e63 6520 6f66 0a20 2020 2070  equence of.    p
+0001b4f0: 7269 6d69 7469 7665 2070 6174 6820 656c  rimitive path el
+0001b500: 656d 656e 7473 2061 6e64 2060 4772 6170  ements and `Grap
+0001b510: 6869 6373 436f 6e74 6578 7460 2e0a 2020  hicsContext`..  
+0001b520: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+0001b530: 5f69 6e69 745f 5f28 7365 6c66 2c20 783d  _init__(self, x=
+0001b540: 302c 2079 3d30 293a 0a20 2020 2020 2020  0, y=0):.       
+0001b550: 2073 656c 662e 5f72 6f6f 745f 6772 6170   self._root_grap
+0001b560: 6869 6373 5f63 6f6e 7465 7874 203d 2047  hics_context = G
+0001b570: 7261 7068 6963 7343 6f6e 7465 7874 2829  raphicsContext()
+0001b580: 0a20 2020 2020 2020 2073 656c 662e 5f67  .        self._g
+0001b590: 7261 7068 6963 735f 636f 6e74 6578 7420  raphics_context 
+0001b5a0: 3d20 7365 6c66 2e5f 726f 6f74 5f67 7261  = self._root_gra
+0001b5b0: 7068 6963 735f 636f 6e74 6578 740a 0a20  phics_context.. 
+0001b5c0: 2020 2020 2020 2073 656c 662e 5f63 6c6f         self._clo
+0001b5d0: 7365 6420 3d20 5472 7565 0a20 2020 2020  sed = True.     
+0001b5e0: 2020 2073 656c 662e 5f63 6c6f 7365 5f63     self._close_c
+0001b5f0: 6f6e 7465 7874 203d 2073 656c 662e 5f67  ontext = self._g
+0001b600: 7261 7068 6963 735f 636f 6e74 6578 740a  raphics_context.
+0001b610: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+0001b620: 7461 7274 6572 5f6d 6f76 6520 3d20 4d6f  tarter_move = Mo
+0001b630: 7665 2850 6f69 6e74 2878 2c20 7929 290a  ve(Point(x, y)).
+0001b640: 0a20 2020 2064 6566 205f 5f64 6565 7063  .    def __deepc
+0001b650: 6f70 795f 5f28 7365 6c66 2c20 6d65 6d6f  opy__(self, memo
+0001b660: 293a 0a20 2020 2020 2020 2023 2074 6865  ):.        # the
+0001b670: 7265 2773 206e 6f20 7265 616c 2077 6179  re's no real way
+0001b680: 2074 6f20 7265 636f 7665 7220 7468 6520   to recover the 
+0001b690: 6d61 7463 6869 6e67 2063 7572 7265 6e74  matching current
+0001b6a0: 205f 6772 6170 6869 6373 5f63 6f6e 7465   _graphics_conte
+0001b6b0: 7874 2061 6674 6572 0a20 2020 2020 2020  xt after.       
+0001b6c0: 2023 2063 6f70 7969 6e67 2074 6865 2072   # copying the r
+0001b6d0: 6f6f 7420 636f 6e74 6578 742c 2062 7574  oot context, but
+0001b6e0: 2074 6861 7427 7320 6f6b 2062 6563 6175   that's ok becau
+0001b6f0: 7365 2077 6520 6361 6e20 6a75 7374 2064  se we can just d
+0001b700: 6973 616c 6c6f 7720 636f 7079 696e 670a  isallow copying.
+0001b710: 2020 2020 2020 2020 2320 6f66 2070 6174          # of pat
+0001b720: 6873 2075 6e64 6572 206d 6f64 6966 6963  hs under modific
+0001b730: 6174 696f 6e20 6173 2074 6861 7420 6973  ation as that is
+0001b740: 2061 6c6d 6f73 7420 6365 7274 6169 6e6c   almost certainl
+0001b750: 7920 7772 6f6e 6720 7573 6167 652e 0a20  y wrong usage.. 
+0001b760: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0001b770: 6772 6170 6869 6373 5f63 6f6e 7465 7874  graphics_context
+0001b780: 2069 7320 6e6f 7420 7365 6c66 2e5f 726f   is not self._ro
+0001b790: 6f74 5f67 7261 7068 6963 735f 636f 6e74  ot_graphics_cont
+0001b7a0: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
+0001b7b0: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+0001b7c0: 726f 7228 6622 6361 6e6e 6f74 2063 6f70  ror(f"cannot cop
+0001b7d0: 7920 7061 7468 207b 7365 6c66 7d20 7768  y path {self} wh
+0001b7e0: 696c 6520 6974 2069 7320 6265 696e 6720  ile it is being 
+0001b7f0: 6d6f 6469 6669 6564 2229 0a0a 2020 2020  modified")..    
+0001b800: 2020 2020 636f 7069 6564 203d 2073 656c      copied = sel
+0001b810: 662e 5f5f 636c 6173 735f 5f28 290a 2020  f.__class__().  
+0001b820: 2020 2020 2020 636f 7069 6564 2e5f 726f        copied._ro
+0001b830: 6f74 5f67 7261 7068 6963 735f 636f 6e74  ot_graphics_cont
+0001b840: 6578 7420 3d20 636f 7079 2e64 6565 7063  ext = copy.deepc
+0001b850: 6f70 7928 7365 6c66 2e5f 726f 6f74 5f67  opy(self._root_g
+0001b860: 7261 7068 6963 735f 636f 6e74 6578 742c  raphics_context,
+0001b870: 206d 656d 6f29 0a20 2020 2020 2020 2063   memo).        c
+0001b880: 6f70 6965 642e 5f67 7261 7068 6963 735f  opied._graphics_
+0001b890: 636f 6e74 6578 7420 3d20 636f 7069 6564  context = copied
+0001b8a0: 2e5f 726f 6f74 5f67 7261 7068 6963 735f  ._root_graphics_
+0001b8b0: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
+0001b8c0: 636f 7069 6564 2e5f 636c 6f73 6564 203d  copied._closed =
+0001b8d0: 2073 656c 662e 5f63 6c6f 7365 640a 2020   self._closed.  
+0001b8e0: 2020 2020 2020 636f 7069 6564 2e5f 636c        copied._cl
+0001b8f0: 6f73 655f 636f 6e74 6578 7420 3d20 636f  ose_context = co
+0001b900: 7069 6564 2e5f 6772 6170 6869 6373 5f63  pied._graphics_c
+0001b910: 6f6e 7465 7874 0a0a 2020 2020 2020 2020  ontext..        
+0001b920: 7265 7475 726e 2063 6f70 6965 640a 0a20  return copied.. 
+0001b930: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0001b940: 2064 6566 2073 7479 6c65 2873 656c 6629   def style(self)
+0001b950: 3a0a 2020 2020 2020 2020 2222 2254 6865  :.        """The
+0001b960: 2060 4772 6170 6869 6373 5374 796c 6560   `GraphicsStyle`
+0001b970: 2061 7070 6c69 6564 2074 6f20 616c 6c20   applied to all 
+0001b980: 656c 656d 656e 7473 206f 6620 7468 6973  elements of this
+0001b990: 2070 6174 682e 2222 220a 2020 2020 2020   path.""".      
+0001b9a0: 2020 7265 7475 726e 2073 656c 662e 5f72    return self._r
+0001b9b0: 6f6f 745f 6772 6170 6869 6373 5f63 6f6e  oot_graphics_con
+0001b9c0: 7465 7874 2e73 7479 6c65 0a0a 2020 2020  text.style..    
+0001b9d0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0001b9e0: 6620 7472 616e 7366 6f72 6d28 7365 6c66  f transform(self
+0001b9f0: 293a 0a20 2020 2020 2020 2022 2222 5468  ):.        """Th
+0001ba00: 6520 6054 7261 6e73 666f 726d 6020 7468  e `Transform` th
+0001ba10: 6174 2061 7070 6c69 6573 2074 6f20 616c  at applies to al
+0001ba20: 6c20 6f66 2074 6865 2065 6c65 6d65 6e74  l of the element
+0001ba30: 7320 6f66 2074 6869 7320 7061 7468 2e22  s of this path."
+0001ba40: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0001ba50: 6e20 7365 6c66 2e5f 726f 6f74 5f67 7261  n self._root_gra
+0001ba60: 7068 6963 735f 636f 6e74 6578 742e 7472  phics_context.tr
+0001ba70: 616e 7366 6f72 6d0a 0a20 2020 2040 7472  ansform..    @tr
+0001ba80: 616e 7366 6f72 6d2e 7365 7474 6572 0a20  ansform.setter. 
+0001ba90: 2020 2064 6566 2074 7261 6e73 666f 726d     def transform
+0001baa0: 2873 656c 662c 2074 6629 3a0a 2020 2020  (self, tf):.    
+0001bab0: 2020 2020 7365 6c66 2e5f 726f 6f74 5f67      self._root_g
+0001bac0: 7261 7068 6963 735f 636f 6e74 6578 742e  raphics_context.
+0001bad0: 7472 616e 7366 6f72 6d20 3d20 7466 0a0a  transform = tf..
+0001bae0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0001baf0: 2020 6465 6620 6175 746f 5f63 6c6f 7365    def auto_close
+0001bb00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001bb10: 2222 2249 6620 7472 7565 2c20 7468 6520  """If true, the 
+0001bb20: 7061 7468 2073 686f 756c 6420 6175 746f  path should auto
+0001bb30: 6d61 7469 6361 6c6c 7920 636c 6f73 6520  matically close 
+0001bb40: 6974 7365 6c66 2062 6566 6f72 6520 7061  itself before pa
+0001bb50: 696e 7469 6e67 2e22 2222 0a20 2020 2020  inting.""".     
+0001bb60: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+0001bb70: 7479 6c65 2e61 7574 6f5f 636c 6f73 650a  tyle.auto_close.
+0001bb80: 0a20 2020 2040 6175 746f 5f63 6c6f 7365  .    @auto_close
+0001bb90: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+0001bba0: 6175 746f 5f63 6c6f 7365 2873 656c 662c  auto_close(self,
+0001bbb0: 2073 686f 756c 6429 3a0a 2020 2020 2020   should):.      
+0001bbc0: 2020 7365 6c66 2e73 7479 6c65 2e61 7574    self.style.aut
+0001bbd0: 6f5f 636c 6f73 6520 3d20 7368 6f75 6c64  o_close = should
+0001bbe0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0001bbf0: 2020 2020 6465 6620 7061 696e 745f 7275      def paint_ru
+0001bc00: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+0001bc10: 2020 2222 224d 616e 7561 6c6c 7920 7370    """Manually sp
+0001bc20: 6563 6966 7920 7468 6520 6050 6174 6850  ecify the `PathP
+0001bc30: 6169 6e74 5275 6c65 6020 746f 2075 7365  aintRule` to use
+0001bc40: 2066 6f72 2072 656e 6465 7269 6e67 2074   for rendering t
+0001bc50: 6865 2070 6174 682e 2222 220a 2020 2020  he path.""".    
+0001bc60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0001bc70: 7374 796c 652e 7061 696e 745f 7275 6c65  style.paint_rule
+0001bc80: 0a0a 2020 2020 4070 6169 6e74 5f72 756c  ..    @paint_rul
+0001bc90: 652e 7365 7474 6572 0a20 2020 2064 6566  e.setter.    def
+0001bca0: 2070 6169 6e74 5f72 756c 6528 7365 6c66   paint_rule(self
+0001bcb0: 2c20 7374 796c 6529 3a0a 2020 2020 2020  , style):.      
+0001bcc0: 2020 7365 6c66 2e73 7479 6c65 2e70 6169    self.style.pai
+0001bcd0: 6e74 5f72 756c 6520 3d20 7374 796c 650a  nt_rule = style.
+0001bce0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0001bcf0: 2020 2064 6566 2063 6c69 7070 696e 675f     def clipping_
+0001bd00: 7061 7468 2873 656c 6629 3a0a 2020 2020  path(self):.    
+0001bd10: 2020 2020 2222 2253 6574 2074 6865 2063      """Set the c
+0001bd20: 6c69 7070 696e 6720 7061 7468 2066 6f72  lipping path for
+0001bd30: 2074 6869 7320 7061 7468 2e22 2222 0a20   this path.""". 
+0001bd40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001bd50: 6c66 2e5f 726f 6f74 5f67 7261 7068 6963  lf._root_graphic
+0001bd60: 735f 636f 6e74 6578 742e 636c 6970 7069  s_context.clippi
+0001bd70: 6e67 5f70 6174 680a 0a20 2020 2040 636c  ng_path..    @cl
+0001bd80: 6970 7069 6e67 5f70 6174 682e 7365 7474  ipping_path.sett
+0001bd90: 6572 0a20 2020 2064 6566 2063 6c69 7070  er.    def clipp
+0001bda0: 696e 675f 7061 7468 2873 656c 662c 206e  ing_path(self, n
+0001bdb0: 6577 5f63 6c69 7061 7468 293a 0a20 2020  ew_clipath):.   
+0001bdc0: 2020 2020 2073 656c 662e 5f72 6f6f 745f       self._root_
+0001bdd0: 6772 6170 6869 6373 5f63 6f6e 7465 7874  graphics_context
+0001bde0: 2e63 6c69 7070 696e 675f 7061 7468 203d  .clipping_path =
+0001bdf0: 206e 6577 5f63 6c69 7061 7468 0a0a 2020   new_clipath..  
+0001be00: 2020 4063 6f6e 7465 7874 6d61 6e61 6765    @contextmanage
+0001be10: 720a 2020 2020 6465 6620 5f6e 6577 5f67  r.    def _new_g
+0001be20: 7261 7068 6963 735f 636f 6e74 6578 7428  raphics_context(
+0001be30: 7365 6c66 2c20 5f61 7474 6163 683d 5472  self, _attach=Tr
+0001be40: 7565 293a 0a20 2020 2020 2020 206f 6c64  ue):.        old
+0001be50: 5f67 7261 7068 6963 735f 636f 6e74 6578  _graphics_contex
+0001be60: 7420 3d20 7365 6c66 2e5f 6772 6170 6869  t = self._graphi
+0001be70: 6373 5f63 6f6e 7465 7874 0a20 2020 2020  cs_context.     
+0001be80: 2020 206e 6577 5f67 7261 7068 6963 735f     new_graphics_
+0001be90: 636f 6e74 6578 7420 3d20 4772 6170 6869  context = Graphi
+0001bea0: 6373 436f 6e74 6578 7428 290a 2020 2020  csContext().    
+0001beb0: 2020 2020 7365 6c66 2e5f 6772 6170 6869      self._graphi
+0001bec0: 6373 5f63 6f6e 7465 7874 203d 206e 6577  cs_context = new
+0001bed0: 5f67 7261 7068 6963 735f 636f 6e74 6578  _graphics_contex
+0001bee0: 740a 2020 2020 2020 2020 7472 793a 0a20  t.        try:. 
+0001bef0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+0001bf00: 206e 6577 5f67 7261 7068 6963 735f 636f   new_graphics_co
+0001bf10: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
+0001bf20: 2020 6966 205f 6174 7461 6368 3a0a 2020    if _attach:.  
+0001bf30: 2020 2020 2020 2020 2020 2020 2020 6f6c                ol
+0001bf40: 645f 6772 6170 6869 6373 5f63 6f6e 7465  d_graphics_conte
+0001bf50: 7874 2e61 6464 5f69 7465 6d28 6e65 775f  xt.add_item(new_
+0001bf60: 6772 6170 6869 6373 5f63 6f6e 7465 7874  graphics_context
+0001bf70: 290a 2020 2020 2020 2020 6669 6e61 6c6c  ).        finall
+0001bf80: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+0001bf90: 656c 662e 5f67 7261 7068 6963 735f 636f  elf._graphics_co
+0001bfa0: 6e74 6578 7420 3d20 6f6c 645f 6772 6170  ntext = old_grap
+0001bfb0: 6869 6373 5f63 6f6e 7465 7874 0a0a 2020  hics_context..  
+0001bfc0: 2020 4063 6f6e 7465 7874 6d61 6e61 6765    @contextmanage
+0001bfd0: 720a 2020 2020 6465 6620 7472 616e 7366  r.    def transf
+0001bfe0: 6f72 6d5f 6772 6f75 7028 7365 6c66 2c20  orm_group(self, 
+0001bff0: 7472 616e 7366 6f72 6d29 3a0a 2020 2020  transform):.    
+0001c000: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0001c010: 4170 706c 7920 7468 6520 7072 6f76 6964  Apply the provid
+0001c020: 6564 2060 5472 616e 7366 6f72 6d60 2074  ed `Transform` t
+0001c030: 6f20 616c 6c20 706f 696e 7473 2061 6464  o all points add
+0001c040: 6564 2077 6974 6869 6e20 7468 6973 2063  ed within this c
+0001c050: 6f6e 7465 7874 2e0a 2020 2020 2020 2020  ontext..        
+0001c060: 2222 220a 2020 2020 2020 2020 7769 7468  """.        with
+0001c070: 2073 656c 662e 5f6e 6577 5f67 7261 7068   self._new_graph
+0001c080: 6963 735f 636f 6e74 6578 7428 2920 6173  ics_context() as
+0001c090: 2063 7478 743a 0a20 2020 2020 2020 2020   ctxt:.         
+0001c0a0: 2020 2063 7478 742e 7472 616e 7366 6f72     ctxt.transfor
+0001c0b0: 6d20 3d20 7472 616e 7366 6f72 6d0a 2020  m = transform.  
+0001c0c0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+0001c0d0: 7365 6c66 0a0a 2020 2020 6465 6620 6164  self..    def ad
+0001c0e0: 645f 7061 7468 5f65 6c65 6d65 6e74 2873  d_path_element(s
+0001c0f0: 656c 662c 2069 7465 6d2c 205f 636f 7079  elf, item, _copy
+0001c100: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+0001c110: 2222 220a 2020 2020 2020 2020 4164 6420  """.        Add 
+0001c120: 7468 6520 6769 7665 6e20 656c 656d 656e  the given elemen
+0001c130: 7420 6173 2061 2070 6174 6820 6974 656d  t as a path item
+0001c140: 206f 6620 7468 6973 2070 6174 682e 0a0a   of this path...
+0001c150: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0001c160: 2020 2020 2020 2020 2020 6974 656d 3a20            item: 
+0001c170: 7468 6520 6974 656d 2074 6f20 6164 6420  the item to add 
+0001c180: 746f 2074 6869 7320 7061 7468 2e0a 2020  to this path..  
+0001c190: 2020 2020 2020 2020 2020 5f63 6f70 7920            _copy 
+0001c1a0: 2862 6f6f 6c29 3a20 6966 2074 7275 6520  (bool): if true 
+0001c1b0: 2874 6865 2064 6566 6175 6c74 292c 2074  (the default), t
+0001c1c0: 6865 2069 7465 6d20 7769 6c6c 2062 6520  he item will be 
+0001c1d0: 636f 7069 6564 2062 6566 6f72 6520 6265  copied before be
+0001c1e0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+0001c1f0: 2020 2020 6170 7065 6e64 6564 2e20 5468      appended. Th
+0001c200: 6973 2070 7265 7665 6e74 7320 6d6f 6469  is prevents modi
+0001c210: 6669 6361 7469 6f6e 7320 746f 2061 2072  fications to a r
+0001c220: 6566 6572 656e 6365 6420 6f62 6a65 6374  eferenced object
+0001c230: 2066 726f 6d0a 2020 2020 2020 2020 2020   from.          
+0001c240: 2020 2020 2020 2272 6574 726f 6163 7469        "retroacti
+0001c250: 7665 6c79 2220 616c 7465 7269 6e67 2069  vely" altering i
+0001c260: 7473 2073 7479 6c65 2f73 6861 7065 2061  ts style/shape a
+0001c270: 6e64 2073 686f 756c 6420 6265 2064 6973  nd should be dis
+0001c280: 6162 6c65 6420 7769 7468 0a20 2020 2020  abled with.     
+0001c290: 2020 2020 2020 2020 2020 2063 6175 7469             cauti
+0001c2a0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
+0001c2b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001c2c0: 5f73 7461 7274 6572 5f6d 6f76 6520 6973  _starter_move is
+0001c2d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001c2e0: 2020 2020 2020 2073 656c 662e 5f63 6c6f         self._clo
+0001c2f0: 7365 6420 3d20 4661 6c73 650a 2020 2020  sed = False.    
+0001c300: 2020 2020 2020 2020 7365 6c66 2e5f 6772          self._gr
+0001c310: 6170 6869 6373 5f63 6f6e 7465 7874 2e61  aphics_context.a
+0001c320: 6464 5f69 7465 6d28 7365 6c66 2e5f 7374  dd_item(self._st
+0001c330: 6172 7465 725f 6d6f 7665 2c20 5f63 6f70  arter_move, _cop
+0001c340: 793d 4661 6c73 6529 0a20 2020 2020 2020  y=False).       
+0001c350: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
+0001c360: 5f63 6f6e 7465 7874 203d 2073 656c 662e  _context = self.
+0001c370: 5f67 7261 7068 6963 735f 636f 6e74 6578  _graphics_contex
+0001c380: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
+0001c390: 6c66 2e5f 7374 6172 7465 725f 6d6f 7665  lf._starter_move
+0001c3a0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+0001c3b0: 2073 656c 662e 5f67 7261 7068 6963 735f   self._graphics_
+0001c3c0: 636f 6e74 6578 742e 6164 645f 6974 656d  context.add_item
+0001c3d0: 2869 7465 6d2c 205f 636f 7079 3d5f 636f  (item, _copy=_co
+0001c3e0: 7079 290a 0a20 2020 2064 6566 2072 656d  py)..    def rem
+0001c3f0: 6f76 655f 6c61 7374 5f70 6174 685f 656c  ove_last_path_el
+0001c400: 656d 656e 7428 7365 6c66 293a 0a20 2020  ement(self):.   
+0001c410: 2020 2020 2073 656c 662e 5f67 7261 7068       self._graph
+0001c420: 6963 735f 636f 6e74 6578 742e 7265 6d6f  ics_context.remo
+0001c430: 7665 5f6c 6173 745f 6974 656d 2829 0a0a  ve_last_item()..
+0001c440: 2020 2020 6465 6620 7265 6374 616e 676c      def rectangl
+0001c450: 6528 7365 6c66 2c20 782c 2079 2c20 772c  e(self, x, y, w,
+0001c460: 2068 2c20 7278 3d30 2c20 7279 3d30 293a   h, rx=0, ry=0):
+0001c470: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001c480: 2020 2020 2041 7070 656e 6420 6120 7265       Append a re
+0001c490: 6374 616e 676c 6520 6173 2061 2063 6c6f  ctangle as a clo
+0001c4a0: 7365 6420 7375 6270 6174 6820 746f 2074  sed subpath to t
+0001c4b0: 6865 2063 7572 7265 6e74 2070 6174 682e  he current path.
+0001c4c0: 0a0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
+0001c4d0: 2077 6964 7468 206f 7220 7468 6520 6865   width or the he
+0001c4e0: 6967 6874 2061 7265 2030 2c20 7468 6520  ight are 0, the 
+0001c4f0: 7265 6374 616e 676c 6520 7769 6c6c 2062  rectangle will b
+0001c500: 6520 636f 6c6c 6170 7365 6420 746f 2061  e collapsed to a
+0001c510: 206c 696e 650a 2020 2020 2020 2020 2875   line.        (u
+0001c520: 6e6c 6573 7320 7468 6579 2772 6520 626f  nless they're bo
+0001c530: 7468 2030 2c20 696e 2077 6869 6368 2063  th 0, in which c
+0001c540: 6173 6520 6974 2773 2063 6f6c 6c61 7073  ase it's collaps
+0001c550: 6564 2074 6f20 6e6f 7468 696e 6729 2e0a  ed to nothing)..
+0001c560: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0001c570: 2020 2020 2020 2020 2020 2078 2028 4e75             x (Nu
+0001c580: 6d62 6572 293a 2074 6865 2061 6273 6369  mber): the absci
+0001c590: 7373 6120 6f66 2074 6865 2073 7461 7274  ssa of the start
+0001c5a0: 696e 6720 636f 726e 6572 206f 6620 7468  ing corner of th
+0001c5b0: 6520 7265 6374 616e 676c 652e 0a20 2020  e rectangle..   
+0001c5c0: 2020 2020 2020 2020 2079 2028 4e75 6d62           y (Numb
+0001c5d0: 6572 293a 2074 6865 206f 7264 696e 6174  er): the ordinat
+0001c5e0: 6520 6f66 2074 6865 2073 7461 7274 696e  e of the startin
+0001c5f0: 6720 636f 726e 6572 206f 6620 7468 6520  g corner of the 
+0001c600: 7265 6374 616e 676c 652e 0a20 2020 2020  rectangle..     
+0001c610: 2020 2020 2020 2077 2028 4e75 6d62 6572         w (Number
+0001c620: 293a 2074 6865 2077 6964 7468 206f 6620  ): the width of 
+0001c630: 7468 6520 7265 6374 616e 676c 6520 2869  the rectangle (i
+0001c640: 6620 302c 2074 6865 2072 6563 7461 6e67  f 0, the rectang
+0001c650: 6c65 2077 696c 6c20 6265 0a20 2020 2020  le will be.     
+0001c660: 2020 2020 2020 2020 2020 2072 656e 6465             rende
+0001c670: 7265 6420 6173 2061 2076 6572 7469 6361  red as a vertica
+0001c680: 6c20 6c69 6e65 292e 0a20 2020 2020 2020  l line)..       
+0001c690: 2020 2020 2068 2028 4e75 6d62 6572 293a       h (Number):
+0001c6a0: 2074 6865 2068 6569 6768 7420 6f66 2074   the height of t
+0001c6b0: 6865 2072 6563 7461 6e67 6c65 2028 6966  he rectangle (if
+0001c6c0: 2030 2c20 7468 6520 7265 6374 616e 676c   0, the rectangl
+0001c6d0: 6520 7769 6c6c 2062 650a 2020 2020 2020  e will be.      
+0001c6e0: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+0001c6f0: 6564 2061 7320 6120 686f 7269 7a6f 6e74  ed as a horizont
+0001c700: 616c 206c 696e 6529 2e0a 2020 2020 2020  al line)..      
+0001c710: 2020 2020 2020 7278 2028 4e75 6d62 6572        rx (Number
+0001c720: 293a 2074 6865 2078 2d72 6164 6975 7320  ): the x-radius 
+0001c730: 6f66 2074 6865 2072 6563 7461 6e67 6c65  of the rectangle
+0001c740: 2072 6f75 6e64 6564 2063 6f72 6e65 7220   rounded corner 
+0001c750: 2869 6620 3020 7468 6520 636f 726e 6572  (if 0 the corner
+0001c760: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001c770: 2020 7769 6c6c 206e 6f74 2062 6520 726f    will not be ro
+0001c780: 756e 6465 6429 2e0a 2020 2020 2020 2020  unded)..        
+0001c790: 2020 2020 7279 2028 4e75 6d62 6572 293a      ry (Number):
+0001c7a0: 2074 6865 2079 2d72 6164 6975 7320 6f66   the y-radius of
+0001c7b0: 2074 6865 2072 6563 7461 6e67 6c65 2072   the rectangle r
+0001c7c0: 6f75 6e64 6564 2063 6f72 6e65 7220 2869  ounded corner (i
+0001c7d0: 6620 3020 7468 6520 636f 726e 6572 730a  f 0 the corners.
+0001c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c7f0: 7769 6c6c 206e 6f74 2062 6520 726f 756e  will not be roun
+0001c800: 6465 6429 2e0a 0a20 2020 2020 2020 2052  ded)...        R
+0001c810: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0001c820: 2020 2020 5468 6520 7061 7468 2c20 746f      The path, to
+0001c830: 2061 6c6c 6f77 2063 6861 696e 696e 6720   allow chaining 
+0001c840: 6d65 7468 6f64 2063 616c 6c73 2e0a 2020  method calls..  
+0001c850: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0001c860: 2020 2073 656c 662e 5f69 6e73 6572 745f     self._insert_
+0001c870: 696d 706c 6963 6974 5f63 6c6f 7365 5f69  implicit_close_i
+0001c880: 665f 6f70 656e 2829 0a20 2020 2020 2020  f_open().       
+0001c890: 2073 656c 662e 6164 645f 7061 7468 5f65   self.add_path_e
+0001c8a0: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+0001c8b0: 2020 2020 526f 756e 6465 6452 6563 7461      RoundedRecta
+0001c8c0: 6e67 6c65 2850 6f69 6e74 2878 2c20 7929  ngle(Point(x, y)
+0001c8d0: 2c20 506f 696e 7428 772c 2068 292c 2050  , Point(w, h), P
+0001c8e0: 6f69 6e74 2872 782c 2072 7929 292c 205f  oint(rx, ry)), _
+0001c8f0: 636f 7079 3d46 616c 7365 0a20 2020 2020  copy=False.     
+0001c900: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+0001c910: 662e 5f63 6c6f 7365 6420 3d20 5472 7565  f._closed = True
+0001c920: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+0001c930: 7665 5f74 6f28 782c 2079 290a 0a20 2020  ve_to(x, y)..   
+0001c940: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001c950: 0a0a 2020 2020 6465 6620 6369 7263 6c65  ..    def circle
+0001c960: 2873 656c 662c 2063 782c 2063 792c 2072  (self, cx, cy, r
+0001c970: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0001c980: 2020 2020 2020 2041 7070 656e 6420 6120         Append a 
+0001c990: 6369 7263 6c65 2061 7320 6120 636c 6f73  circle as a clos
+0001c9a0: 6564 2073 7562 7061 7468 2074 6f20 7468  ed subpath to th
+0001c9b0: 6520 6375 7272 656e 7420 7061 7468 2e0a  e current path..
+0001c9c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0001c9d0: 2020 2020 2020 2020 2020 2063 7820 284e             cx (N
+0001c9e0: 756d 6265 7229 3a20 7468 6520 6162 7363  umber): the absc
+0001c9f0: 6973 7361 206f 6620 7468 6520 6369 7263  issa of the circ
+0001ca00: 6c65 2773 2063 656e 7465 7220 706f 696e  le's center poin
+0001ca10: 742e 0a20 2020 2020 2020 2020 2020 2063  t..            c
+0001ca20: 7920 284e 756d 6265 7229 3a20 7468 6520  y (Number): the 
+0001ca30: 6f72 6469 6e61 7465 206f 6620 7468 6520  ordinate of the 
+0001ca40: 6369 7263 6c65 2773 2063 656e 7465 7220  circle's center 
+0001ca50: 706f 696e 742e 0a20 2020 2020 2020 2020  point..         
+0001ca60: 2020 2072 2028 4e75 6d62 6572 293a 2074     r (Number): t
+0001ca70: 6865 2072 6164 6975 7320 6f66 2074 6865  he radius of the
+0001ca80: 2063 6972 636c 652e 0a0a 2020 2020 2020   circle...      
+0001ca90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0001caa0: 2020 2020 2020 2054 6865 2070 6174 682c         The path,
+0001cab0: 2074 6f20 616c 6c6f 7720 6368 6169 6e69   to allow chaini
+0001cac0: 6e67 206d 6574 686f 6420 6361 6c6c 732e  ng method calls.
+0001cad0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001cae0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001caf0: 2e65 6c6c 6970 7365 2863 782c 2063 792c  .ellipse(cx, cy,
+0001cb00: 2072 2c20 7229 0a0a 2020 2020 6465 6620   r, r)..    def 
+0001cb10: 656c 6c69 7073 6528 7365 6c66 2c20 6378  ellipse(self, cx
+0001cb20: 2c20 6379 2c20 7278 2c20 7279 293a 0a20  , cy, rx, ry):. 
+0001cb30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001cb40: 2020 2041 7070 656e 6420 616e 2065 6c6c     Append an ell
+0001cb50: 6970 7365 2061 7320 6120 636c 6f73 6564  ipse as a closed
+0001cb60: 2073 7562 7061 7468 2074 6f20 7468 6520   subpath to the 
+0001cb70: 6375 7272 656e 7420 7061 7468 2e0a 0a20  current path... 
+0001cb80: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0001cb90: 2020 2020 2020 2020 2063 7820 284e 756d           cx (Num
+0001cba0: 6265 7229 3a20 7468 6520 6162 7363 6973  ber): the abscis
+0001cbb0: 7361 206f 6620 7468 6520 656c 6c69 7073  sa of the ellips
+0001cbc0: 6527 7320 6365 6e74 6572 2070 6f69 6e74  e's center point
+0001cbd0: 2e0a 2020 2020 2020 2020 2020 2020 6379  ..            cy
+0001cbe0: 2028 4e75 6d62 6572 293a 2074 6865 206f   (Number): the o
+0001cbf0: 7264 696e 6174 6520 6f66 2074 6865 2065  rdinate of the e
+0001cc00: 6c6c 6970 7365 2773 2063 656e 7465 7220  llipse's center 
+0001cc10: 706f 696e 742e 0a20 2020 2020 2020 2020  point..         
+0001cc20: 2020 2072 7820 284e 756d 6265 7229 3a20     rx (Number): 
+0001cc30: 7468 6520 782d 7261 6469 7573 206f 6620  the x-radius of 
+0001cc40: 7468 6520 656c 6c69 7073 652e 0a20 2020  the ellipse..   
+0001cc50: 2020 2020 2020 2020 2072 7920 284e 756d           ry (Num
+0001cc60: 6265 7229 3a20 7468 6520 792d 7261 6469  ber): the y-radi
+0001cc70: 7573 206f 6620 7468 6520 656c 6c69 7073  us of the ellips
+0001cc80: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+0001cc90: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0001cca0: 2054 6865 2070 6174 682c 2074 6f20 616c   The path, to al
+0001ccb0: 6c6f 7720 6368 6169 6e69 6e67 206d 6574  low chaining met
+0001ccc0: 686f 6420 6361 6c6c 732e 0a20 2020 2020  hod calls..     
+0001ccd0: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0001cce0: 656c 662e 5f69 6e73 6572 745f 696d 706c  elf._insert_impl
+0001ccf0: 6963 6974 5f63 6c6f 7365 5f69 665f 6f70  icit_close_if_op
+0001cd00: 656e 2829 0a20 2020 2020 2020 2073 656c  en().        sel
+0001cd10: 662e 6164 645f 7061 7468 5f65 6c65 6d65  f.add_path_eleme
+0001cd20: 6e74 2845 6c6c 6970 7365 2850 6f69 6e74  nt(Ellipse(Point
+0001cd30: 2872 782c 2072 7929 2c20 506f 696e 7428  (rx, ry), Point(
+0001cd40: 6378 2c20 6379 2929 2c20 5f63 6f70 793d  cx, cy)), _copy=
+0001cd50: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
+0001cd60: 656c 662e 5f63 6c6f 7365 6420 3d20 5472  elf._closed = Tr
+0001cd70: 7565 0a20 2020 2020 2020 2073 656c 662e  ue.        self.
+0001cd80: 6d6f 7665 5f74 6f28 6378 2c20 6379 290a  move_to(cx, cy).
+0001cd90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001cda0: 7365 6c66 0a0a 2020 2020 6465 6620 6d6f  self..    def mo
+0001cdb0: 7665 5f74 6f28 7365 6c66 2c20 782c 2079  ve_to(self, x, y
+0001cdc0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0001cdd0: 2020 2020 2020 2053 7461 7274 2061 206e         Start a n
+0001cde0: 6577 2073 7562 7061 7468 206f 7220 6d6f  ew subpath or mo
+0001cdf0: 7665 2074 6865 2070 6174 6820 7374 6172  ve the path star
+0001ce00: 7469 6e67 2070 6f69 6e74 2e0a 0a20 2020  ting point...   
+0001ce10: 2020 2020 2049 6620 6e6f 2070 6174 6820       If no path 
+0001ce20: 656c 656d 656e 7473 2068 6176 6520 6265  elements have be
+0001ce30: 656e 2061 6464 6564 2079 6574 2c20 7468  en added yet, th
+0001ce40: 6973 2077 696c 6c20 6368 616e 6765 2074  is will change t
+0001ce50: 6865 2070 6174 6820 7374 6172 7469 6e67  he path starting
+0001ce60: 0a20 2020 2020 2020 2070 6f69 6e74 2e20  .        point. 
+0001ce70: 4966 2070 6174 6820 656c 656d 656e 7473  If path elements
+0001ce80: 2068 6176 6520 6265 656e 2061 6464 6564   have been added
+0001ce90: 2c20 7468 6973 2077 696c 6c20 696e 7365  , this will inse
+0001cea0: 7274 2061 6e20 696d 706c 6963 6974 2063  rt an implicit c
+0001ceb0: 6c6f 7365 2069 6e0a 2020 2020 2020 2020  lose in.        
+0001cec0: 6f72 6465 7220 746f 2073 7461 7274 2061  order to start a
+0001ced0: 206e 6577 2073 7562 7061 7468 2e0a 0a20   new subpath... 
+0001cee0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0001cef0: 2020 2020 2020 2020 2078 2028 4e75 6d62           x (Numb
+0001cf00: 6572 293a 2061 6273 6369 7373 6120 6f66  er): abscissa of
+0001cf10: 2074 6865 2028 7375 6229 7061 7468 2073   the (sub)path s
+0001cf20: 7461 7274 696e 6720 706f 696e 742e 0a20  tarting point.. 
+0001cf30: 2020 2020 2020 2020 2020 2079 2028 4e75             y (Nu
+0001cf40: 6d62 6572 293a 206f 7264 696e 6174 6520  mber): ordinate 
+0001cf50: 6f66 2074 6865 2028 7375 6229 7061 7468  of the (sub)path
+0001cf60: 2073 7461 7274 696e 6720 706f 696e 742e   starting point.
+0001cf70: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0001cf80: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+0001cf90: 6865 2070 6174 682c 2074 6f20 616c 6c6f  he path, to allo
+0001cfa0: 7720 6368 6169 6e69 6e67 206d 6574 686f  w chaining metho
+0001cfb0: 6420 6361 6c6c 732e 0a20 2020 2020 2020  d calls..       
+0001cfc0: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+0001cfd0: 662e 5f69 6e73 6572 745f 696d 706c 6963  f._insert_implic
+0001cfe0: 6974 5f63 6c6f 7365 5f69 665f 6f70 656e  it_close_if_open
+0001cff0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0001d000: 5f73 7461 7274 6572 5f6d 6f76 6520 3d20  _starter_move = 
+0001d010: 4d6f 7665 2850 6f69 6e74 2878 2c20 7929  Move(Point(x, y)
+0001d020: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001d030: 2073 656c 660a 0a20 2020 2064 6566 206d   self..    def m
+0001d040: 6f76 655f 7265 6c61 7469 7665 2873 656c  ove_relative(sel
+0001d050: 662c 2078 2c20 7929 3a0a 2020 2020 2020  f, x, y):.      
+0001d060: 2020 2222 220a 2020 2020 2020 2020 5374    """.        St
+0001d070: 6172 7420 6120 6e65 7720 7375 6270 6174  art a new subpat
+0001d080: 6820 6f72 206d 6f76 6520 7468 6520 7061  h or move the pa
+0001d090: 7468 2073 7461 7274 2070 6f69 6e74 2072  th start point r
+0001d0a0: 656c 6174 6976 6520 746f 2074 6865 2070  elative to the p
+0001d0b0: 7265 7669 6f75 7320 706f 696e 742e 0a0a  revious point...
+0001d0c0: 2020 2020 2020 2020 4966 206e 6f20 7061          If no pa
+0001d0d0: 7468 2065 6c65 6d65 6e74 7320 6861 7665  th elements have
+0001d0e0: 2062 6565 6e20 6164 6465 6420 7965 742c   been added yet,
+0001d0f0: 2074 6869 7320 7769 6c6c 2063 6861 6e67   this will chang
+0001d100: 6520 7468 6520 7061 7468 2073 7461 7274  e the path start
+0001d110: 696e 670a 2020 2020 2020 2020 706f 696e  ing.        poin
+0001d120: 742e 2049 6620 7061 7468 2065 6c65 6d65  t. If path eleme
+0001d130: 6e74 7320 6861 7665 2062 6565 6e20 6164  nts have been ad
+0001d140: 6465 642c 2074 6869 7320 7769 6c6c 2069  ded, this will i
+0001d150: 6e73 6572 7420 616e 2069 6d70 6c69 6369  nsert an implici
+0001d160: 7420 636c 6f73 6520 696e 0a20 2020 2020  t close in.     
+0001d170: 2020 206f 7264 6572 2074 6f20 7374 6172     order to star
+0001d180: 7420 6120 6e65 7720 7375 6270 6174 682e  t a new subpath.
+0001d190: 0a0a 2020 2020 2020 2020 5468 6973 2077  ..        This w
+0001d1a0: 696c 6c20 6f76 6572 7772 6974 6520 616e  ill overwrite an
+0001d1b0: 2061 6273 6f6c 7574 6520 6d6f 7665 5f74   absolute move_t
+0001d1c0: 6f20 6173 206c 6f6e 6720 6173 206e 6f20  o as long as no 
+0001d1d0: 6e6f 6e2d 6d6f 7665 2070 6174 6820 6974  non-move path it
+0001d1e0: 656d 7320 6861 7665 0a20 2020 2020 2020  ems have.       
+0001d1f0: 2062 6565 6e20 6170 7065 6e64 6564 2e20   been appended. 
+0001d200: 5468 6520 7265 6c61 7469 7665 2070 6f73  The relative pos
+0001d210: 6974 696f 6e20 6973 2072 6573 6f6c 7665  ition is resolve
+0001d220: 6420 6672 6f6d 2074 6865 2070 7265 7669  d from the previ
+0001d230: 6f75 7320 6974 656d 2077 6865 6e0a 2020  ous item when.  
+0001d240: 2020 2020 2020 7468 6520 7061 7468 2069        the path i
+0001d250: 7320 6265 696e 6720 7265 6e64 6572 6564  s being rendered
+0001d260: 2c20 6f72 2066 726f 6d20 302c 2030 2069  , or from 0, 0 i
+0001d270: 6620 6974 2069 7320 7468 6520 6669 7273  f it is the firs
+0001d280: 7420 6974 656d 2e0a 0a20 2020 2020 2020  t item...       
+0001d290: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0001d2a0: 2020 2078 2028 4e75 6d62 6572 293a 2061     x (Number): a
+0001d2b0: 6273 6369 7373 6120 6f66 2074 6865 2028  bscissa of the (
+0001d2c0: 7375 6229 7061 7468 2073 7461 7274 696e  sub)path startin
+0001d2d0: 6720 706f 696e 7420 7265 6c61 7469 7665  g point relative
+0001d2e0: 2074 6f20 7468 652e 0a20 2020 2020 2020   to the..       
+0001d2f0: 2020 2020 2079 2028 4e75 6d62 6572 293a       y (Number):
+0001d300: 206f 7264 696e 6174 6520 6f66 2074 6865   ordinate of the
+0001d310: 2028 7375 6229 7061 7468 2073 7461 7274   (sub)path start
+0001d320: 696e 6720 706f 696e 7420 7265 6c61 7469  ing point relati
+0001d330: 7665 2074 6f20 7468 652e 0a20 2020 2020  ve to the..     
+0001d340: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0001d350: 656c 662e 5f69 6e73 6572 745f 696d 706c  elf._insert_impl
+0001d360: 6963 6974 5f63 6c6f 7365 5f69 665f 6f70  icit_close_if_op
+0001d370: 656e 2829 0a20 2020 2020 2020 2069 6620  en().        if 
+0001d380: 7365 6c66 2e5f 7374 6172 7465 725f 6d6f  self._starter_mo
+0001d390: 7665 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ve is not None:.
+0001d3a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001d3b0: 2e5f 636c 6f73 6564 203d 2046 616c 7365  ._closed = False
+0001d3c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001d3d0: 662e 5f67 7261 7068 6963 735f 636f 6e74  f._graphics_cont
+0001d3e0: 6578 742e 6164 645f 6974 656d 2873 656c  ext.add_item(sel
+0001d3f0: 662e 5f73 7461 7274 6572 5f6d 6f76 652c  f._starter_move,
+0001d400: 205f 636f 7079 3d46 616c 7365 290a 2020   _copy=False).  
+0001d410: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001d420: 636c 6f73 655f 636f 6e74 6578 7420 3d20  close_context = 
+0001d430: 7365 6c66 2e5f 6772 6170 6869 6373 5f63  self._graphics_c
+0001d440: 6f6e 7465 7874 0a20 2020 2020 2020 2073  ontext.        s
+0001d450: 656c 662e 5f73 7461 7274 6572 5f6d 6f76  elf._starter_mov
+0001d460: 6520 3d20 5265 6c61 7469 7665 4d6f 7665  e = RelativeMove
+0001d470: 2850 6f69 6e74 2878 2c20 7929 290a 2020  (Point(x, y)).  
+0001d480: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001d490: 660a 0a20 2020 2064 6566 206c 696e 655f  f..    def line_
+0001d4a0: 746f 2873 656c 662c 2078 2c20 7929 3a0a  to(self, x, y):.
+0001d4b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001d4c0: 2020 2020 4170 7065 6e64 2061 2073 7472      Append a str
+0001d4d0: 6169 6768 7420 6c69 6e65 2074 6f20 7468  aight line to th
+0001d4e0: 6973 2070 6174 682e 0a0a 2020 2020 2020  is path...      
+0001d4f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0001d500: 2020 2020 7820 284e 756d 6265 7229 3a20      x (Number): 
+0001d510: 6162 7363 6973 7361 2074 6865 206c 696e  abscissa the lin
+0001d520: 6527 7320 656e 6420 706f 696e 742e 0a20  e's end point.. 
+0001d530: 2020 2020 2020 2020 2020 2079 2028 4e75             y (Nu
+0001d540: 6d62 6572 293a 206f 7264 696e 6174 6520  mber): ordinate 
+0001d550: 6f66 2074 6865 206c 696e 6527 7320 656e  of the line's en
+0001d560: 6420 706f 696e 742e 0a0a 2020 2020 2020  d point...      
+0001d570: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0001d580: 2020 2020 2020 2054 6865 2070 6174 682c         The path,
+0001d590: 2074 6f20 616c 6c6f 7720 6368 6169 6e69   to allow chaini
+0001d5a0: 6e67 206d 6574 686f 6420 6361 6c6c 732e  ng method calls.
+0001d5b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001d5c0: 2020 2020 2073 656c 662e 6164 645f 7061       self.add_pa
+0001d5d0: 7468 5f65 6c65 6d65 6e74 284c 696e 6528  th_element(Line(
+0001d5e0: 506f 696e 7428 782c 2079 2929 2c20 5f63  Point(x, y)), _c
+0001d5f0: 6f70 793d 4661 6c73 6529 0a20 2020 2020  opy=False).     
+0001d600: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0001d610: 2020 2020 6465 6620 6c69 6e65 5f72 656c      def line_rel
+0001d620: 6174 6976 6528 7365 6c66 2c20 6478 2c20  ative(self, dx, 
+0001d630: 6479 293a 0a20 2020 2020 2020 2022 2222  dy):.        """
+0001d640: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
+0001d650: 6120 7374 7261 6967 6874 206c 696e 6520  a straight line 
+0001d660: 7768 6f73 6520 656e 6420 6973 2063 6f6d  whose end is com
+0001d670: 7075 7465 6420 6173 2061 6e20 6f66 6673  puted as an offs
+0001d680: 6574 2066 726f 6d20 7468 6520 656e 6420  et from the end 
+0001d690: 6f66 2074 6865 0a20 2020 2020 2020 2070  of the.        p
+0001d6a0: 7265 7669 6f75 7320 7061 7468 2065 6c65  revious path ele
+0001d6b0: 6d65 6e74 2e0a 0a20 2020 2020 2020 2041  ment...        A
+0001d6c0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0001d6d0: 2078 2028 4e75 6d62 6572 293a 2061 6273   x (Number): abs
+0001d6e0: 6369 7373 6120 7468 6520 6c69 6e65 2773  cissa the line's
+0001d6f0: 2065 6e64 2070 6f69 6e74 2072 656c 6174   end point relat
+0001d700: 6976 6520 746f 2074 6865 2065 6e64 2070  ive to the end p
+0001d710: 6f69 6e74 206f 6620 7468 650a 2020 2020  oint of the.    
+0001d720: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+0001d730: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
+0001d740: 742e 0a20 2020 2020 2020 2020 2020 2079  t..            y
+0001d750: 2028 4e75 6d62 6572 293a 206f 7264 696e   (Number): ordin
+0001d760: 6174 6520 6f66 2074 6865 206c 696e 6527  ate of the line'
+0001d770: 7320 656e 6420 706f 696e 7420 7265 6c61  s end point rela
+0001d780: 7469 7665 2074 6f20 7468 6520 656e 6420  tive to the end 
+0001d790: 706f 696e 7420 6f66 0a20 2020 2020 2020  point of.       
+0001d7a0: 2020 2020 2020 2020 2074 6865 2070 7265           the pre
+0001d7b0: 7669 6f75 7320 7061 7468 2065 6c65 6d65  vious path eleme
+0001d7c0: 6e74 2e0a 0a20 2020 2020 2020 2052 6574  nt...        Ret
+0001d7d0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0001d7e0: 2020 5468 6520 7061 7468 2c20 746f 2061    The path, to a
+0001d7f0: 6c6c 6f77 2063 6861 696e 696e 6720 6d65  llow chaining me
+0001d800: 7468 6f64 2063 616c 6c73 2e0a 2020 2020  thod calls..    
+0001d810: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0001d820: 7365 6c66 2e61 6464 5f70 6174 685f 656c  self.add_path_el
+0001d830: 656d 656e 7428 5265 6c61 7469 7665 4c69  ement(RelativeLi
+0001d840: 6e65 2850 6f69 6e74 2864 782c 2064 7929  ne(Point(dx, dy)
+0001d850: 292c 205f 636f 7079 3d46 616c 7365 290a  ), _copy=False).
+0001d860: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001d870: 656c 660a 0a20 2020 2064 6566 2068 6f72  elf..    def hor
+0001d880: 697a 6f6e 7461 6c5f 6c69 6e65 5f74 6f28  izontal_line_to(
+0001d890: 7365 6c66 2c20 7829 3a0a 2020 2020 2020  self, x):.      
+0001d8a0: 2020 2222 220a 2020 2020 2020 2020 4170    """.        Ap
+0001d8b0: 7065 6e64 2061 2073 7472 6169 6768 7420  pend a straight 
+0001d8c0: 686f 7269 7a6f 6e74 616c 206c 696e 6520  horizontal line 
+0001d8d0: 746f 2074 6865 2067 6976 656e 2061 6273  to the given abs
+0001d8e0: 6369 7373 612e 2054 6865 206f 7264 696e  cissa. The ordin
+0001d8f0: 6174 6520 6973 0a20 2020 2020 2020 2072  ate is.        r
+0001d900: 6574 7269 6576 6564 2066 726f 6d20 7468  etrieved from th
+0001d910: 6520 656e 6420 706f 696e 7420 6f66 2074  e end point of t
+0001d920: 6865 2070 7265 7669 6f75 7320 7061 7468  he previous path
+0001d930: 2065 6c65 6d65 6e74 2e0a 0a20 2020 2020   element...     
+0001d940: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0001d950: 2020 2020 2078 2028 4e75 6d62 6572 293a       x (Number):
+0001d960: 2061 6273 6369 7373 6120 6f66 2074 6865   abscissa of the
+0001d970: 206c 696e 6527 7320 656e 6420 706f 696e   line's end poin
+0001d980: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
+0001d990: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0001d9a0: 2054 6865 2070 6174 682c 2074 6f20 616c   The path, to al
+0001d9b0: 6c6f 7720 6368 6169 6e69 6e67 206d 6574  low chaining met
+0001d9c0: 686f 6420 6361 6c6c 732e 0a20 2020 2020  hod calls..     
+0001d9d0: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0001d9e0: 656c 662e 6164 645f 7061 7468 5f65 6c65  elf.add_path_ele
+0001d9f0: 6d65 6e74 2848 6f72 697a 6f6e 7461 6c4c  ment(HorizontalL
+0001da00: 696e 6528 7829 2c20 5f63 6f70 793d 4661  ine(x), _copy=Fa
+0001da10: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
+0001da20: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
+0001da30: 6620 686f 7269 7a6f 6e74 616c 5f6c 696e  f horizontal_lin
+0001da40: 655f 7265 6c61 7469 7665 2873 656c 662c  e_relative(self,
+0001da50: 2064 7829 3a0a 2020 2020 2020 2020 2222   dx):.        ""
+0001da60: 220a 2020 2020 2020 2020 4170 7065 6e64  ".        Append
+0001da70: 2061 2073 7472 6169 6768 7420 686f 7269   a straight hori
+0001da80: 7a6f 6e74 616c 206c 696e 6520 746f 2074  zontal line to t
+0001da90: 6865 2067 6976 656e 206f 6666 7365 7420  he given offset 
+0001daa0: 6672 6f6d 2074 6865 2070 7265 7669 6f75  from the previou
+0001dab0: 7320 7061 7468 0a20 2020 2020 2020 2065  s path.        e
+0001dac0: 6c65 6d65 6e74 2e20 5468 6520 6f72 6469  lement. The ordi
+0001dad0: 6e61 7465 2069 7320 7265 7472 6965 7665  nate is retrieve
+0001dae0: 6420 6672 6f6d 2074 6865 2065 6e64 2070  d from the end p
+0001daf0: 6f69 6e74 206f 6620 7468 6520 7072 6576  oint of the prev
+0001db00: 696f 7573 2070 6174 680a 2020 2020 2020  ious path.      
+0001db10: 2020 656c 656d 656e 742e 0a0a 2020 2020    element...    
+0001db20: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0001db30: 2020 2020 2020 7820 284e 756d 6265 7229        x (Number)
+0001db40: 3a20 6162 7363 6973 7361 206f 6620 7468  : abscissa of th
+0001db50: 6520 6c69 6e65 2773 2065 6e64 2070 6f69  e line's end poi
+0001db60: 6e74 2072 656c 6174 6976 6520 746f 2074  nt relative to t
+0001db70: 6865 2065 6e64 2070 6f69 6e74 206f 660a  he end point of.
+0001db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db90: 7468 6520 7072 6576 696f 7573 2070 6174  the previous pat
+0001dba0: 6820 656c 656d 656e 742e 0a0a 2020 2020  h element...    
+0001dbb0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0001dbc0: 2020 2020 2020 2020 2054 6865 2070 6174           The pat
+0001dbd0: 682c 2074 6f20 616c 6c6f 7720 6368 6169  h, to allow chai
+0001dbe0: 6e69 6e67 206d 6574 686f 6420 6361 6c6c  ning method call
+0001dbf0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+0001dc00: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+0001dc10: 7061 7468 5f65 6c65 6d65 6e74 2852 656c  path_element(Rel
+0001dc20: 6174 6976 6548 6f72 697a 6f6e 7461 6c4c  ativeHorizontalL
+0001dc30: 696e 6528 6478 292c 205f 636f 7079 3d46  ine(dx), _copy=F
+0001dc40: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
+0001dc50: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
+0001dc60: 6566 2076 6572 7469 6361 6c5f 6c69 6e65  ef vertical_line
+0001dc70: 5f74 6f28 7365 6c66 2c20 7929 3a0a 2020  _to(self, y):.  
+0001dc80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001dc90: 2020 4170 7065 6e64 2061 2073 7472 6169    Append a strai
+0001dca0: 6768 7420 7665 7274 6963 616c 206c 696e  ght vertical lin
+0001dcb0: 6520 746f 2074 6865 2067 6976 656e 206f  e to the given o
+0001dcc0: 7264 696e 6174 652e 2054 6865 2061 6273  rdinate. The abs
+0001dcd0: 6369 7373 6120 6973 0a20 2020 2020 2020  cissa is.       
+0001dce0: 2072 6574 7269 6576 6564 2066 726f 6d20   retrieved from 
+0001dcf0: 7468 6520 656e 6420 706f 696e 7420 6f66  the end point of
+0001dd00: 2074 6865 2070 7265 7669 6f75 7320 7061   the previous pa
+0001dd10: 7468 2065 6c65 6d65 6e74 2e0a 0a20 2020  th element...   
+0001dd20: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0001dd30: 2020 2020 2020 2079 2028 4e75 6d62 6572         y (Number
+0001dd40: 293a 206f 7264 696e 6174 6520 6f66 2074  ): ordinate of t
+0001dd50: 6865 206c 696e 6527 7320 656e 6420 706f  he line's end po
+0001dd60: 696e 742e 0a0a 2020 2020 2020 2020 5265  int...        Re
+0001dd70: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0001dd80: 2020 2054 6865 2070 6174 682c 2074 6f20     The path, to 
+0001dd90: 616c 6c6f 7720 6368 6169 6e69 6e67 206d  allow chaining m
+0001dda0: 6574 686f 6420 6361 6c6c 732e 0a20 2020  ethod calls..   
+0001ddb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001ddc0: 2073 656c 662e 6164 645f 7061 7468 5f65   self.add_path_e
+0001ddd0: 6c65 6d65 6e74 2856 6572 7469 6361 6c4c  lement(VerticalL
+0001dde0: 696e 6528 7929 2c20 5f63 6f70 793d 4661  ine(y), _copy=Fa
+0001ddf0: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
+0001de00: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
+0001de10: 6620 7665 7274 6963 616c 5f6c 696e 655f  f vertical_line_
+0001de20: 7265 6c61 7469 7665 2873 656c 662c 2064  relative(self, d
+0001de30: 7929 3a0a 2020 2020 2020 2020 2222 220a  y):.        """.
+0001de40: 2020 2020 2020 2020 4170 7065 6e64 2061          Append a
+0001de50: 2073 7472 6169 6768 7420 7665 7274 6963   straight vertic
+0001de60: 616c 206c 696e 6520 746f 2074 6865 2067  al line to the g
+0001de70: 6976 656e 206f 6666 7365 7420 6672 6f6d  iven offset from
+0001de80: 2074 6865 2070 7265 7669 6f75 7320 7061   the previous pa
+0001de90: 7468 0a20 2020 2020 2020 2065 6c65 6d65  th.        eleme
+0001dea0: 6e74 2e20 5468 6520 6162 7363 6973 7361  nt. The abscissa
+0001deb0: 2069 7320 7265 7472 6965 7665 6420 6672   is retrieved fr
+0001dec0: 6f6d 2074 6865 2065 6e64 2070 6f69 6e74  om the end point
+0001ded0: 206f 6620 7468 6520 7072 6576 696f 7573   of the previous
+0001dee0: 2070 6174 680a 2020 2020 2020 2020 656c   path.        el
+0001def0: 656d 656e 742e 0a0a 2020 2020 2020 2020  ement...        
+0001df00: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0001df10: 2020 7920 284e 756d 6265 7229 3a20 6f72    y (Number): or
+0001df20: 6469 6e61 7465 206f 6620 7468 6520 6c69  dinate of the li
+0001df30: 6e65 2773 2065 6e64 2070 6f69 6e74 2072  ne's end point r
+0001df40: 656c 6174 6976 6520 746f 2074 6865 2065  elative to the e
+0001df50: 6e64 2070 6f69 6e74 206f 660a 2020 2020  nd point of.    
+0001df60: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+0001df70: 7072 6576 696f 7573 2070 6174 6820 656c  previous path el
+0001df80: 656d 656e 742e 0a0a 2020 2020 2020 2020  ement...        
+0001df90: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0001dfa0: 2020 2020 2054 6865 2070 6174 682c 2074       The path, t
+0001dfb0: 6f20 616c 6c6f 7720 6368 6169 6e69 6e67  o allow chaining
+0001dfc0: 206d 6574 686f 6420 6361 6c6c 732e 0a20   method calls.. 
+0001dfd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001dfe0: 2020 2073 656c 662e 6164 645f 7061 7468     self.add_path
+0001dff0: 5f65 6c65 6d65 6e74 2852 656c 6174 6976  _element(Relativ
+0001e000: 6556 6572 7469 6361 6c4c 696e 6528 6479  eVerticalLine(dy
+0001e010: 292c 205f 636f 7079 3d46 616c 7365 290a  ), _copy=False).
+0001e020: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001e030: 656c 660a 0a20 2020 2064 6566 2063 7572  elf..    def cur
+0001e040: 7665 5f74 6f28 7365 6c66 2c20 7831 2c20  ve_to(self, x1, 
+0001e050: 7931 2c20 7832 2c20 7932 2c20 7833 2c20  y1, x2, y2, x3, 
+0001e060: 7933 293a 0a20 2020 2020 2020 2022 2222  y3):.        """
+0001e070: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
+0001e080: 6120 6375 6269 6320 42c3 a97a 6965 7220  a cubic B..zier 
+0001e090: 6375 7276 6520 746f 2074 6869 7320 7061  curve to this pa
+0001e0a0: 7468 2e0a 0a20 2020 2020 2020 2041 7267  th...        Arg
+0001e0b0: 733a 0a20 2020 2020 2020 2020 2020 2078  s:.            x
+0001e0c0: 3120 284e 756d 6265 7229 3a20 6162 7363  1 (Number): absc
+0001e0d0: 6973 7361 206f 6620 7468 6520 6669 7273  issa of the firs
+0001e0e0: 7420 636f 6e74 726f 6c20 706f 696e 740a  t control point.
+0001e0f0: 2020 2020 2020 2020 2020 2020 7931 2028              y1 (
+0001e100: 4e75 6d62 6572 293a 206f 7264 696e 6174  Number): ordinat
+0001e110: 6520 6f66 2074 6865 2066 6972 7374 2063  e of the first c
+0001e120: 6f6e 7472 6f6c 2070 6f69 6e74 0a20 2020  ontrol point.   
+0001e130: 2020 2020 2020 2020 2078 3220 284e 756d           x2 (Num
+0001e140: 6265 7229 3a20 6162 7363 6973 7361 206f  ber): abscissa o
+0001e150: 6620 7468 6520 7365 636f 6e64 2063 6f6e  f the second con
+0001e160: 7472 6f6c 2070 6f69 6e74 0a20 2020 2020  trol point.     
+0001e170: 2020 2020 2020 2079 3220 284e 756d 6265         y2 (Numbe
+0001e180: 7229 3a20 6f72 6469 6e61 7465 206f 6620  r): ordinate of 
+0001e190: 7468 6520 7365 636f 6e64 2063 6f6e 7472  the second contr
+0001e1a0: 6f6c 2070 6f69 6e74 0a20 2020 2020 2020  ol point.       
+0001e1b0: 2020 2020 2078 3320 284e 756d 6265 7229       x3 (Number)
+0001e1c0: 3a20 6162 7363 6973 7361 206f 6620 7468  : abscissa of th
+0001e1d0: 6520 656e 6420 706f 696e 740a 2020 2020  e end point.    
+0001e1e0: 2020 2020 2020 2020 7933 2028 4e75 6d62          y3 (Numb
+0001e1f0: 6572 293a 206f 7264 696e 6174 6520 6f66  er): ordinate of
+0001e200: 2074 6865 2065 6e64 2070 6f69 6e74 0a0a   the end point..
+0001e210: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0001e220: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0001e230: 2070 6174 682c 2074 6f20 616c 6c6f 7720   path, to allow 
+0001e240: 6368 6169 6e69 6e67 206d 6574 686f 6420  chaining method 
+0001e250: 6361 6c6c 732e 0a20 2020 2020 2020 2022  calls..        "
+0001e260: 2222 0a20 2020 2020 2020 2063 7472 6c31  "".        ctrl1
+0001e270: 203d 2050 6f69 6e74 2878 312c 2079 3129   = Point(x1, y1)
+0001e280: 0a20 2020 2020 2020 2063 7472 6c32 203d  .        ctrl2 =
+0001e290: 2050 6f69 6e74 2878 322c 2079 3229 0a20   Point(x2, y2). 
+0001e2a0: 2020 2020 2020 2065 6e64 203d 2050 6f69         end = Poi
+0001e2b0: 6e74 2878 332c 2079 3329 0a0a 2020 2020  nt(x3, y3)..    
+0001e2c0: 2020 2020 7365 6c66 2e61 6464 5f70 6174      self.add_pat
+0001e2d0: 685f 656c 656d 656e 7428 4265 7a69 6572  h_element(Bezier
+0001e2e0: 4375 7276 6528 6374 726c 312c 2063 7472  Curve(ctrl1, ctr
+0001e2f0: 6c32 2c20 656e 6429 2c20 5f63 6f70 793d  l2, end), _copy=
+0001e300: 4661 6c73 6529 0a20 2020 2020 2020 2072  False).        r
+0001e310: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
+0001e320: 6465 6620 6375 7276 655f 7265 6c61 7469  def curve_relati
+0001e330: 7665 2873 656c 662c 2064 7831 2c20 6479  ve(self, dx1, dy
+0001e340: 312c 2064 7832 2c20 6479 322c 2064 7833  1, dx2, dy2, dx3
+0001e350: 2c20 6479 3329 3a0a 2020 2020 2020 2020  , dy3):.        
+0001e360: 2222 220a 2020 2020 2020 2020 4170 7065  """.        Appe
+0001e370: 6e64 2061 2063 7562 6963 2042 c3a9 7a69  nd a cubic B..zi
+0001e380: 6572 2063 7572 7665 2077 686f 7365 2070  er curve whose p
+0001e390: 6f69 6e74 7320 6172 6520 6578 7072 6573  oints are expres
+0001e3a0: 7365 6420 7265 6c61 7469 7665 2074 6f20  sed relative to 
+0001e3b0: 7468 650a 2020 2020 2020 2020 656e 6420  the.        end 
+0001e3c0: 706f 696e 7420 6f66 2074 6865 2070 7265  point of the pre
+0001e3d0: 7669 6f75 7320 7061 7468 2065 6c65 6d65  vious path eleme
+0001e3e0: 6e74 2e0a 0a20 2020 2020 2020 2045 2e67  nt...        E.g
+0001e3f0: 2e20 7769 7468 2061 2073 7461 7274 2070  . with a start p
+0001e400: 6f69 6e74 206f 6620 2830 2c20 3029 2c20  oint of (0, 0), 
+0001e410: 6769 7665 6e20 2831 2c20 3129 2c20 2832  given (1, 1), (2
+0001e420: 2c20 3229 2c20 2833 2c20 3329 2c20 7468  , 2), (3, 3), th
+0001e430: 6520 6f75 7470 7574 0a20 2020 2020 2020  e output.       
+0001e440: 2063 7572 7665 2077 6f75 6c64 2068 6176   curve would hav
+0001e450: 6520 7468 6520 706f 696e 7473 3a0a 0a20  e the points:.. 
+0001e460: 2020 2020 2020 2028 302c 2030 2920 6331         (0, 0) c1
+0001e470: 2028 312c 2031 2920 6332 2028 332c 2033   (1, 1) c2 (3, 3
+0001e480: 2920 6520 2836 2c20 3629 0a0a 2020 2020  ) e (6, 6)..    
+0001e490: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0001e4a0: 2020 2020 2020 6478 3120 284e 756d 6265        dx1 (Numbe
+0001e4b0: 7229 3a20 6162 7363 6973 7361 206f 6620  r): abscissa of 
+0001e4c0: 7468 6520 6669 7273 7420 636f 6e74 726f  the first contro
+0001e4d0: 6c20 706f 696e 7420 7265 6c61 7469 7665  l point relative
+0001e4e0: 2074 6f20 7468 6520 656e 6420 706f 696e   to the end poin
+0001e4f0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0001e500: 2020 6f66 2074 6865 2070 7265 7669 6f75    of the previou
+0001e510: 7320 7061 7468 2065 6c65 6d65 6e74 0a20  s path element. 
+0001e520: 2020 2020 2020 2020 2020 2064 7931 2028             dy1 (
+0001e530: 4e75 6d62 6572 293a 206f 7264 696e 6174  Number): ordinat
+0001e540: 6520 6f66 2074 6865 2066 6972 7374 2063  e of the first c
+0001e550: 6f6e 7472 6f6c 2070 6f69 6e74 2072 656c  ontrol point rel
+0001e560: 6174 6976 6520 746f 2074 6865 2065 6e64  ative to the end
+0001e570: 2070 6f69 6e74 0a20 2020 2020 2020 2020   point.         
+0001e580: 2020 2020 2020 206f 6620 7468 6520 7072         of the pr
+0001e590: 6576 696f 7573 2070 6174 6820 656c 656d  evious path elem
+0001e5a0: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
+0001e5b0: 6478 3220 284e 756d 6265 7229 3a20 6162  dx2 (Number): ab
+0001e5c0: 7363 6973 7361 206f 6666 7365 7420 6f66  scissa offset of
+0001e5d0: 2074 6865 2073 6563 6f6e 6420 636f 6e74   the second cont
+0001e5e0: 726f 6c20 706f 696e 7420 7265 6c61 7469  rol point relati
+0001e5f0: 7665 2074 6f20 7468 650a 2020 2020 2020  ve to the.      
+0001e600: 2020 2020 2020 2020 2020 656e 6420 706f            end po
+0001e610: 696e 7420 6f66 2074 6865 2070 7265 7669  int of the previ
+0001e620: 6f75 7320 7061 7468 2065 6c65 6d65 6e74  ous path element
+0001e630: 0a20 2020 2020 2020 2020 2020 2064 7932  .            dy2
+0001e640: 2028 4e75 6d62 6572 293a 206f 7264 696e   (Number): ordin
+0001e650: 6174 6520 6f66 6673 6574 206f 6620 7468  ate offset of th
+0001e660: 6520 7365 636f 6e64 2063 6f6e 7472 6f6c  e second control
+0001e670: 2070 6f69 6e74 2072 656c 6174 6976 6520   point relative 
+0001e680: 746f 2074 6865 0a20 2020 2020 2020 2020  to the.         
+0001e690: 2020 2020 2020 2065 6e64 2070 6f69 6e74         end point
+0001e6a0: 206f 6620 7468 6520 7072 6576 696f 7573   of the previous
+0001e6b0: 2070 6174 6820 656c 656d 656e 740a 2020   path element.  
+0001e6c0: 2020 2020 2020 2020 2020 6478 3320 284e            dx3 (N
+0001e6d0: 756d 6265 7229 3a20 6162 7363 6973 7361  umber): abscissa
+0001e6e0: 206f 6666 7365 7420 6f66 2074 6865 2065   offset of the e
+0001e6f0: 6e64 2070 6f69 6e74 2072 656c 6174 6976  nd point relativ
+0001e700: 6520 746f 2074 6865 2065 6e64 2070 6f69  e to the end poi
+0001e710: 6e74 206f 660a 2020 2020 2020 2020 2020  nt of.          
+0001e720: 2020 2020 2020 7468 6520 7072 6576 696f        the previo
+0001e730: 7573 2070 6174 6820 656c 656d 656e 740a  us path element.
+0001e740: 2020 2020 2020 2020 2020 2020 6479 3320              dy3 
+0001e750: 284e 756d 6265 7229 3a20 6f72 6469 6e61  (Number): ordina
+0001e760: 7465 206f 6666 7365 7420 6f66 2074 6865  te offset of the
+0001e770: 2065 6e64 2070 6f69 6e74 2072 656c 6174   end point relat
+0001e780: 6976 6520 746f 2074 6865 2065 6e64 2070  ive to the end p
+0001e790: 6f69 6e74 206f 660a 2020 2020 2020 2020  oint of.        
+0001e7a0: 2020 2020 2020 2020 7468 6520 7072 6576          the prev
+0001e7b0: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
+0001e7c0: 740a 0a20 2020 2020 2020 2052 6574 7572  t..        Retur
+0001e7d0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0001e7e0: 5468 6520 7061 7468 2c20 746f 2061 6c6c  The path, to all
+0001e7f0: 6f77 2063 6861 696e 696e 6720 6d65 7468  ow chaining meth
+0001e800: 6f64 2063 616c 6c73 2e0a 2020 2020 2020  od calls..      
+0001e810: 2020 2222 220a 2020 2020 2020 2020 6331    """.        c1
+0001e820: 6420 3d20 506f 696e 7428 6478 312c 2064  d = Point(dx1, d
+0001e830: 7931 290a 2020 2020 2020 2020 6332 6420  y1).        c2d 
+0001e840: 3d20 506f 696e 7428 6478 322c 2064 7932  = Point(dx2, dy2
+0001e850: 290a 2020 2020 2020 2020 656e 6420 3d20  ).        end = 
+0001e860: 506f 696e 7428 6478 332c 2064 7933 290a  Point(dx3, dy3).
+0001e870: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+0001e880: 645f 7061 7468 5f65 6c65 6d65 6e74 2852  d_path_element(R
+0001e890: 656c 6174 6976 6542 657a 6965 7243 7572  elativeBezierCur
+0001e8a0: 7665 2863 3164 2c20 6332 642c 2065 6e64  ve(c1d, c2d, end
+0001e8b0: 292c 205f 636f 7079 3d46 616c 7365 290a  ), _copy=False).
+0001e8c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001e8d0: 656c 660a 0a20 2020 2064 6566 2071 7561  elf..    def qua
+0001e8e0: 6472 6174 6963 5f63 7572 7665 5f74 6f28  dratic_curve_to(
+0001e8f0: 7365 6c66 2c20 7831 2c20 7931 2c20 7832  self, x1, y1, x2
+0001e900: 2c20 7932 293a 0a20 2020 2020 2020 2022  , y2):.        "
+0001e910: 2222 0a20 2020 2020 2020 2041 7070 656e  "".        Appen
+0001e920: 6420 6120 6375 6269 6320 42c3 a97a 6965  d a cubic B..zie
+0001e930: 7220 6375 7276 6520 6d69 6d69 636b 696e  r curve mimickin
+0001e940: 6720 7468 6520 7370 6563 6966 6965 6420  g the specified 
+0001e950: 7175 6164 7261 7469 6320 42c3 a97a 6965  quadratic B..zie
+0001e960: 7220 6375 7276 652e 0a0a 2020 2020 2020  r curve...      
+0001e970: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0001e980: 2020 2020 7831 2028 4e75 6d62 6572 293a      x1 (Number):
+0001e990: 2061 6273 6369 7373 6120 6f66 2074 6865   abscissa of the
+0001e9a0: 2063 6f6e 7472 6f6c 2070 6f69 6e74 0a20   control point. 
+0001e9b0: 2020 2020 2020 2020 2020 2079 3120 284e             y1 (N
+0001e9c0: 756d 6265 7229 3a20 6f72 6469 6e61 7465  umber): ordinate
+0001e9d0: 206f 6620 7468 6520 636f 6e74 726f 6c20   of the control 
+0001e9e0: 706f 696e 740a 2020 2020 2020 2020 2020  point.          
+0001e9f0: 2020 7832 2028 4e75 6d62 6572 293a 2061    x2 (Number): a
+0001ea00: 6273 6369 7373 6120 6f66 2074 6865 2065  bscissa of the e
+0001ea10: 6e64 2070 6f69 6e74 0a20 2020 2020 2020  nd point.       
+0001ea20: 2020 2020 2079 3220 284e 756d 6265 7229       y2 (Number)
+0001ea30: 3a20 6f72 6469 6e61 7465 206f 6620 7468  : ordinate of th
+0001ea40: 6520 656e 6420 706f 696e 740a 0a20 2020  e end point..   
+0001ea50: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0001ea60: 2020 2020 2020 2020 2020 5468 6520 7061            The pa
+0001ea70: 7468 2c20 746f 2061 6c6c 6f77 2063 6861  th, to allow cha
+0001ea80: 696e 696e 6720 6d65 7468 6f64 2063 616c  ining method cal
+0001ea90: 6c73 2e0a 2020 2020 2020 2020 2222 220a  ls..        """.
+0001eaa0: 2020 2020 2020 2020 6374 726c 203d 2050          ctrl = P
+0001eab0: 6f69 6e74 2878 312c 2079 3129 0a20 2020  oint(x1, y1).   
+0001eac0: 2020 2020 2065 6e64 203d 2050 6f69 6e74       end = Point
+0001ead0: 2878 322c 2079 3229 0a20 2020 2020 2020  (x2, y2).       
+0001eae0: 2073 656c 662e 6164 645f 7061 7468 5f65   self.add_path_e
+0001eaf0: 6c65 6d65 6e74 2851 7561 6472 6174 6963  lement(Quadratic
+0001eb00: 4265 7a69 6572 4375 7276 6528 6374 726c  BezierCurve(ctrl
+0001eb10: 2c20 656e 6429 2c20 5f63 6f70 793d 4661  , end), _copy=Fa
+0001eb20: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
+0001eb30: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
+0001eb40: 6620 7175 6164 7261 7469 635f 6375 7276  f quadratic_curv
+0001eb50: 655f 7265 6c61 7469 7665 2873 656c 662c  e_relative(self,
+0001eb60: 2064 7831 2c20 6479 312c 2064 7832 2c20   dx1, dy1, dx2, 
+0001eb70: 6479 3229 3a0a 2020 2020 2020 2020 2222  dy2):.        ""
+0001eb80: 220a 2020 2020 2020 2020 4170 7065 6e64  ".        Append
+0001eb90: 2061 2063 7562 6963 2042 c3a9 7a69 6572   a cubic B..zier
+0001eba0: 2063 7572 7665 206d 696d 6963 6b69 6e67   curve mimicking
+0001ebb0: 2074 6865 2073 7065 6369 6669 6564 2071   the specified q
+0001ebc0: 7561 6472 6174 6963 2042 c3a9 7a69 6572  uadratic B..zier
+0001ebd0: 2063 7572 7665 2e0a 0a20 2020 2020 2020   curve...       
+0001ebe0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0001ebf0: 2020 2064 7831 2028 4e75 6d62 6572 293a     dx1 (Number):
+0001ec00: 2061 6273 6369 7373 6120 6f66 2074 6865   abscissa of the
+0001ec10: 2063 6f6e 7472 6f6c 2070 6f69 6e74 2072   control point r
+0001ec20: 656c 6174 6976 6520 746f 2074 6865 2065  elative to the e
+0001ec30: 6e64 2070 6f69 6e74 206f 660a 2020 2020  nd point of.    
+0001ec40: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+0001ec50: 7072 6576 696f 7573 2070 6174 6820 656c  previous path el
+0001ec60: 656d 656e 740a 2020 2020 2020 2020 2020  ement.          
+0001ec70: 2020 6479 3120 284e 756d 6265 7229 3a20    dy1 (Number): 
+0001ec80: 6f72 6469 6e61 7465 206f 6620 7468 6520  ordinate of the 
+0001ec90: 636f 6e74 726f 6c20 706f 696e 7420 7265  control point re
+0001eca0: 6c61 7469 7665 2074 6f20 7468 6520 656e  lative to the en
+0001ecb0: 6420 706f 696e 7420 6f66 0a20 2020 2020  d point of.     
+0001ecc0: 2020 2020 2020 2020 2020 2074 6865 2070             the p
+0001ecd0: 7265 7669 6f75 7320 7061 7468 2065 6c65  revious path ele
+0001ece0: 6d65 6e74 0a20 2020 2020 2020 2020 2020  ment.           
+0001ecf0: 2064 7832 2028 4e75 6d62 6572 293a 2061   dx2 (Number): a
+0001ed00: 6273 6369 7373 6120 6f66 6673 6574 206f  bscissa offset o
+0001ed10: 6620 7468 6520 656e 6420 706f 696e 7420  f the end point 
+0001ed20: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
+0001ed30: 656e 6420 706f 696e 7420 6f66 0a20 2020  end point of.   
+0001ed40: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0001ed50: 2070 7265 7669 6f75 7320 7061 7468 2065   previous path e
+0001ed60: 6c65 6d65 6e74 0a20 2020 2020 2020 2020  lement.         
+0001ed70: 2020 2064 7932 2028 4e75 6d62 6572 293a     dy2 (Number):
+0001ed80: 206f 7264 696e 6174 6520 6f66 6673 6574   ordinate offset
+0001ed90: 206f 6620 7468 6520 656e 6420 706f 696e   of the end poin
+0001eda0: 7420 7265 6c61 7469 7665 2074 6f20 7468  t relative to th
+0001edb0: 6520 656e 6420 706f 696e 7420 6f66 0a20  e end point of. 
+0001edc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001edd0: 6865 2070 7265 7669 6f75 7320 7061 7468  he previous path
+0001ede0: 2065 6c65 6d65 6e74 0a0a 2020 2020 2020   element..      
+0001edf0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0001ee00: 2020 2020 2020 2054 6865 2070 6174 682c         The path,
+0001ee10: 2074 6f20 616c 6c6f 7720 6368 6169 6e69   to allow chaini
+0001ee20: 6e67 206d 6574 686f 6420 6361 6c6c 732e  ng method calls.
+0001ee30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001ee40: 2020 2020 2063 7472 6c20 3d20 506f 696e       ctrl = Poin
+0001ee50: 7428 6478 312c 2064 7931 290a 2020 2020  t(dx1, dy1).    
+0001ee60: 2020 2020 656e 6420 3d20 506f 696e 7428      end = Point(
+0001ee70: 6478 322c 2064 7932 290a 2020 2020 2020  dx2, dy2).      
+0001ee80: 2020 7365 6c66 2e61 6464 5f70 6174 685f    self.add_path_
+0001ee90: 656c 656d 656e 7428 5265 6c61 7469 7665  element(Relative
+0001eea0: 5175 6164 7261 7469 6342 657a 6965 7243  QuadraticBezierC
+0001eeb0: 7572 7665 2863 7472 6c2c 2065 6e64 292c  urve(ctrl, end),
+0001eec0: 205f 636f 7079 3d46 616c 7365 290a 2020   _copy=False).  
+0001eed0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001eee0: 660a 0a20 2020 2064 6566 2061 7263 5f74  f..    def arc_t
+0001eef0: 6f28 7365 6c66 2c20 7278 2c20 7279 2c20  o(self, rx, ry, 
+0001ef00: 726f 7461 7469 6f6e 2c20 6c61 7267 655f  rotation, large_
+0001ef10: 6172 632c 2070 6f73 6974 6976 655f 7377  arc, positive_sw
+0001ef20: 6565 702c 2078 2c20 7929 3a0a 2020 2020  eep, x, y):.    
+0001ef30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0001ef40: 4170 7065 6e64 2061 6e20 656c 6c69 7074  Append an ellipt
+0001ef50: 6963 616c 2061 7263 2066 726f 6d20 7468  ical arc from th
+0001ef60: 6520 656e 6420 6f66 2074 6865 2070 7265  e end of the pre
+0001ef70: 7669 6f75 7320 7061 7468 2070 6f69 6e74  vious path point
+0001ef80: 2074 6f20 7468 650a 2020 2020 2020 2020   to the.        
+0001ef90: 7370 6563 6966 6965 6420 656e 6420 706f  specified end po
+0001efa0: 696e 742e 0a0a 2020 2020 2020 2020 5468  int...        Th
+0001efb0: 6520 6172 6320 6973 2061 7070 726f 7869  e arc is approxi
+0001efc0: 6d61 7465 6420 7573 696e 6720 42c3 a97a  mated using B..z
+0001efd0: 6965 7220 6375 7276 6573 2c20 736f 2069  ier curves, so i
+0001efe0: 7420 6973 206e 6f74 2070 6572 6665 6374  t is not perfect
+0001eff0: 6c79 2061 6363 7572 6174 652e 0a20 2020  ly accurate..   
+0001f000: 2020 2020 2048 6f77 6576 6572 2c20 7468       However, th
+0001f010: 6520 6572 726f 7220 6973 2073 6d61 6c6c  e error is small
+0001f020: 2065 6e6f 7567 6820 746f 206e 6f74 2062   enough to not b
+0001f030: 6520 6e6f 7469 6365 6162 6c65 2061 7420  e noticeable at 
+0001f040: 616e 7920 7265 6173 6f6e 6162 6c65 0a20  any reasonable. 
+0001f050: 2020 2020 2020 2028 616e 6420 6576 656e         (and even
+0001f060: 206d 6f73 7420 756e 7265 6173 6f6e 6162   most unreasonab
+0001f070: 6c65 2920 7363 616c 6573 2c20 7769 7468  le) scales, with
+0001f080: 2061 2077 6f72 7374 2d63 6173 6520 6465   a worst-case de
+0001f090: 7669 6174 696f 6e20 6f66 2061 726f 756e  viation of aroun
+0001f0a0: 6420 33e2 80b1 2e0a 0a20 2020 2020 2020  d 3......       
+0001f0b0: 204e 6f74 6573 3a0a 2020 2020 2020 2020   Notes:.        
+0001f0c0: 2020 2020 2d20 5468 6520 7369 676e 7320      - The signs 
+0001f0d0: 6f66 2074 6865 2072 6164 6969 2061 7267  of the radii arg
+0001f0e0: 756d 656e 7473 2028 6072 7860 2061 6e64  uments (`rx` and
+0001f0f0: 2060 7279 6029 2061 7265 2069 676e 6f72   `ry`) are ignor
+0001f100: 6564 2028 692e 652e 2074 6865 6972 0a20  ed (i.e. their. 
+0001f110: 2020 2020 2020 2020 2020 2020 2061 6273               abs
+0001f120: 6f6c 7574 6520 7661 6c75 6573 2061 7265  olute values are
+0001f130: 2075 7365 6420 696e 7374 6561 6429 2e0a   used instead)..
+0001f140: 2020 2020 2020 2020 2020 2020 2d20 4966              - If
+0001f150: 2065 6974 6865 7220 7261 6469 7573 2069   either radius i
+0001f160: 7320 302c 2074 6865 6e20 6120 7374 7261  s 0, then a stra
+0001f170: 6967 6874 206c 696e 6520 7769 6c6c 2062  ight line will b
+0001f180: 6520 656d 6974 7465 6420 696e 7374 6561  e emitted instea
+0001f190: 6420 6f66 2061 6e0a 2020 2020 2020 2020  d of an.        
+0001f1a0: 2020 2020 2020 6172 632e 0a20 2020 2020        arc..     
+0001f1b0: 2020 2020 2020 202d 2049 6620 7468 6520         - If the 
+0001f1c0: 7261 6469 6920 6172 6520 746f 6f20 736d  radii are too sm
+0001f1d0: 616c 6c20 666f 7220 7468 6520 6172 6320  all for the arc 
+0001f1e0: 746f 2072 6561 6368 2066 726f 6d20 7468  to reach from th
+0001f1f0: 6520 6375 7272 656e 7420 706f 696e 7420  e current point 
+0001f200: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
+0001f210: 2074 6865 2073 7065 6369 6669 6564 2065   the specified e
+0001f220: 6e64 2070 6f69 6e74 2028 6078 6020 616e  nd point (`x` an
+0001f230: 6420 6079 6029 2c20 7468 656e 2074 6865  d `y`), then the
+0001f240: 7920 7769 6c6c 2062 6520 7072 6f70 6f72  y will be propor
+0001f250: 7469 6f6e 616c 6c79 0a20 2020 2020 2020  tionally.       
+0001f260: 2020 2020 2020 2073 6361 6c65 6420 7570         scaled up
+0001f270: 2075 6e74 696c 2074 6865 7920 6172 6520   until they are 
+0001f280: 6269 6720 656e 6f75 6768 2c20 7768 6963  big enough, whic
+0001f290: 6820 7769 6c6c 2061 6c77 6179 7320 7265  h will always re
+0001f2a0: 7375 6c74 2069 6e20 610a 2020 2020 2020  sult in a.      
+0001f2b0: 2020 2020 2020 2020 6861 6c66 2d65 6c6c          half-ell
+0001f2c0: 6970 7365 2061 7263 2028 692e 652e 2061  ipse arc (i.e. a
+0001f2d0: 6e20 3138 3020 6465 6772 6565 2073 7765  n 180 degree swe
+0001f2e0: 6570 290a 0a20 2020 2020 2020 2041 7267  ep)..        Arg
+0001f2f0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+0001f300: 7820 284e 756d 6265 7229 3a20 7261 6469  x (Number): radi
+0001f310: 7573 2069 6e20 7468 6520 782d 6469 7265  us in the x-dire
+0001f320: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
+0001f330: 2020 2072 7920 284e 756d 6265 7229 3a20     ry (Number): 
+0001f340: 7261 6469 7573 2069 6e20 7468 6520 792d  radius in the y-
+0001f350: 6469 7265 6374 696f 6e2e 0a20 2020 2020  direction..     
+0001f360: 2020 2020 2020 2072 6f74 6174 696f 6e20         rotation 
+0001f370: 284e 756d 6265 7229 3a20 616e 676c 6520  (Number): angle 
+0001f380: 2869 6e20 6465 6772 6565 7329 2074 6861  (in degrees) tha
+0001f390: 7420 7468 6520 6172 6320 7368 6f75 6c64  t the arc should
+0001f3a0: 2062 6520 726f 7461 7465 640a 2020 2020   be rotated.    
+0001f3b0: 2020 2020 2020 2020 2020 2020 636c 6f63              cloc
+0001f3c0: 6b77 6973 6520 6672 6f6d 2074 6865 2070  kwise from the p
+0001f3d0: 7269 6e63 6970 6c65 2061 7865 732e 2054  rinciple axes. T
+0001f3e0: 6869 7320 7061 7261 6d65 7465 7220 646f  his parameter do
+0001f3f0: 6573 206e 6f74 2068 6176 650a 2020 2020  es not have.    
+0001f400: 2020 2020 2020 2020 2020 2020 6120 7669              a vi
+0001f410: 7375 616c 2065 6666 6563 7420 696e 2074  sual effect in t
+0001f420: 6865 2063 6173 6520 7468 6174 2060 7278  he case that `rx
+0001f430: 203d 3d20 7279 602e 0a20 2020 2020 2020   == ry`..       
+0001f440: 2020 2020 206c 6172 6765 5f61 7263 2028       large_arc (
+0001f450: 626f 6f6c 293a 2069 6620 5472 7565 2c20  bool): if True, 
+0001f460: 7468 6520 6172 6320 7769 6c6c 2063 6f76  the arc will cov
+0001f470: 6572 2061 2073 7765 6570 2061 6e67 6c65  er a sweep angle
+0001f480: 206f 6620 6174 206c 6561 7374 2031 3830   of at least 180
+0001f490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f4a0: 2064 6567 7265 6573 2e20 4f74 6865 7277   degrees. Otherw
+0001f4b0: 6973 652c 2074 6865 2073 7765 6570 2061  ise, the sweep a
+0001f4c0: 6e67 6c65 2077 696c 6c20 6265 2061 7420  ngle will be at 
+0001f4d0: 6d6f 7374 2031 3830 2064 6567 7265 6573  most 180 degrees
+0001f4e0: 2e0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+0001f4f0: 7369 7469 7665 5f73 7765 6570 2028 626f  sitive_sweep (bo
+0001f500: 6f6c 293a 2069 6620 5472 7565 2c20 7468  ol): if True, th
+0001f510: 6520 6172 6320 7769 6c6c 2062 6520 7377  e arc will be sw
+0001f520: 6570 7420 6f76 6572 2061 2070 6f73 6974  ept over a posit
+0001f530: 6976 6520 616e 676c 652c 0a20 2020 2020  ive angle,.     
+0001f540: 2020 2020 2020 2020 2020 2069 2e65 2e20             i.e. 
+0001f550: 636c 6f63 6b77 6973 652e 204f 7468 6572  clockwise. Other
+0001f560: 7769 7365 2c20 7468 6520 6172 6320 7769  wise, the arc wi
+0001f570: 6c6c 2062 6520 7377 6570 7420 6f76 6572  ll be swept over
+0001f580: 2061 206e 6567 6174 6976 650a 2020 2020   a negative.    
+0001f590: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+0001f5a0: 652e 0a20 2020 2020 2020 2020 2020 2078  e..            x
+0001f5b0: 2028 4e75 6d62 6572 293a 2061 6273 6369   (Number): absci
+0001f5c0: 7373 6120 6f66 2074 6865 2061 7263 2773  ssa of the arc's
+0001f5d0: 2065 6e64 2070 6f69 6e74 2e0a 2020 2020   end point..    
+0001f5e0: 2020 2020 2020 2020 7920 284e 756d 6265          y (Numbe
+0001f5f0: 7229 3a20 6f72 6469 6e61 7465 206f 6620  r): ordinate of 
+0001f600: 7468 6520 6172 6327 7320 656e 6420 706f  the arc's end po
+0001f610: 696e 742e 0a20 2020 2020 2020 2022 2222  int..        """
+0001f620: 0a0a 2020 2020 2020 2020 6966 2072 7820  ..        if rx 
+0001f630: 3d3d 2030 206f 7220 7279 203d 3d20 303a  == 0 or ry == 0:
+0001f640: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001f650: 7572 6e20 7365 6c66 2e6c 696e 655f 746f  urn self.line_to
+0001f660: 2878 2c20 7929 0a0a 2020 2020 2020 2020  (x, y)..        
+0001f670: 7261 6469 6920 3d20 506f 696e 7428 6162  radii = Point(ab
+0001f680: 7328 7278 292c 2061 6273 2872 7929 290a  s(rx), abs(ry)).
+0001f690: 2020 2020 2020 2020 6c61 7267 655f 6172          large_ar
+0001f6a0: 6320 3d20 626f 6f6c 286c 6172 6765 5f61  c = bool(large_a
+0001f6b0: 7263 290a 2020 2020 2020 2020 726f 7461  rc).        rota
+0001f6c0: 7469 6f6e 203d 206d 6174 682e 7261 6469  tion = math.radi
+0001f6d0: 616e 7328 726f 7461 7469 6f6e 290a 2020  ans(rotation).  
+0001f6e0: 2020 2020 2020 706f 7369 7469 7665 5f73        positive_s
+0001f6f0: 7765 6570 203d 2062 6f6f 6c28 706f 7369  weep = bool(posi
+0001f700: 7469 7665 5f73 7765 6570 290a 2020 2020  tive_sweep).    
+0001f710: 2020 2020 656e 6420 3d20 506f 696e 7428      end = Point(
+0001f720: 782c 2079 290a 0a20 2020 2020 2020 2073  x, y)..        s
+0001f730: 656c 662e 6164 645f 7061 7468 5f65 6c65  elf.add_path_ele
+0001f740: 6d65 6e74 280a 2020 2020 2020 2020 2020  ment(.          
+0001f750: 2020 4172 6328 7261 6469 692c 2072 6f74    Arc(radii, rot
+0001f760: 6174 696f 6e2c 206c 6172 6765 5f61 7263  ation, large_arc
+0001f770: 2c20 706f 7369 7469 7665 5f73 7765 6570  , positive_sweep
+0001f780: 2c20 656e 6429 2c20 5f63 6f70 793d 4661  , end), _copy=Fa
+0001f790: 6c73 650a 2020 2020 2020 2020 290a 2020  lse.        ).  
+0001f7a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001f7b0: 660a 0a20 2020 2064 6566 2061 7263 5f72  f..    def arc_r
+0001f7c0: 656c 6174 6976 6528 7365 6c66 2c20 7278  elative(self, rx
+0001f7d0: 2c20 7279 2c20 726f 7461 7469 6f6e 2c20  , ry, rotation, 
+0001f7e0: 6c61 7267 655f 6172 632c 2070 6f73 6974  large_arc, posit
+0001f7f0: 6976 655f 7377 6565 702c 2064 782c 2064  ive_sweep, dx, d
+0001f800: 7929 3a0a 2020 2020 2020 2020 2222 220a  y):.        """.
+0001f810: 2020 2020 2020 2020 4170 7065 6e64 2061          Append a
+0001f820: 6e20 656c 6c69 7074 6963 616c 2061 7263  n elliptical arc
+0001f830: 2066 726f 6d20 7468 6520 656e 6420 6f66   from the end of
+0001f840: 2074 6865 2070 7265 7669 6f75 7320 7061   the previous pa
+0001f850: 7468 2070 6f69 6e74 2074 6f20 616e 206f  th point to an o
+0001f860: 6666 7365 740a 2020 2020 2020 2020 706f  ffset.        po
+0001f870: 696e 742e 0a0a 2020 2020 2020 2020 5468  int...        Th
+0001f880: 6520 6172 6320 6973 2061 7070 726f 7869  e arc is approxi
+0001f890: 6d61 7465 6420 7573 696e 6720 42c3 a97a  mated using B..z
+0001f8a0: 6965 7220 6375 7276 6573 2c20 736f 2069  ier curves, so i
+0001f8b0: 7420 6973 206e 6f74 2070 6572 6665 6374  t is not perfect
+0001f8c0: 6c79 2061 6363 7572 6174 652e 0a20 2020  ly accurate..   
+0001f8d0: 2020 2020 2048 6f77 6576 6572 2c20 7468       However, th
+0001f8e0: 6520 6572 726f 7220 6973 2073 6d61 6c6c  e error is small
+0001f8f0: 2065 6e6f 7567 6820 746f 206e 6f74 2062   enough to not b
+0001f900: 6520 6e6f 7469 6365 6162 6c65 2061 7420  e noticeable at 
+0001f910: 616e 7920 7265 6173 6f6e 6162 6c65 0a20  any reasonable. 
+0001f920: 2020 2020 2020 2028 616e 6420 6576 656e         (and even
+0001f930: 206d 6f73 7420 756e 7265 6173 6f6e 6162   most unreasonab
+0001f940: 6c65 2920 7363 616c 6573 2c20 7769 7468  le) scales, with
+0001f950: 2061 2077 6f72 7374 2d63 6173 6520 6465   a worst-case de
+0001f960: 7669 6174 696f 6e20 6f66 2061 726f 756e  viation of aroun
+0001f970: 6420 33e2 80b1 2e0a 0a20 2020 2020 2020  d 3......       
+0001f980: 204e 6f74 6573 3a0a 2020 2020 2020 2020   Notes:.        
+0001f990: 2020 2020 2d20 5468 6520 7369 676e 7320      - The signs 
+0001f9a0: 6f66 2074 6865 2072 6164 6969 2061 7267  of the radii arg
+0001f9b0: 756d 656e 7473 2028 6072 7860 2061 6e64  uments (`rx` and
+0001f9c0: 2060 7279 6029 2061 7265 2069 676e 6f72   `ry`) are ignor
+0001f9d0: 6564 2028 692e 652e 2074 6865 6972 0a20  ed (i.e. their. 
+0001f9e0: 2020 2020 2020 2020 2020 2020 2061 6273               abs
+0001f9f0: 6f6c 7574 6520 7661 6c75 6573 2061 7265  olute values are
+0001fa00: 2075 7365 6420 696e 7374 6561 6429 2e0a   used instead)..
+0001fa10: 2020 2020 2020 2020 2020 2020 2d20 4966              - If
+0001fa20: 2065 6974 6865 7220 7261 6469 7573 2069   either radius i
+0001fa30: 7320 302c 2074 6865 6e20 6120 7374 7261  s 0, then a stra
+0001fa40: 6967 6874 206c 696e 6520 7769 6c6c 2062  ight line will b
+0001fa50: 6520 656d 6974 7465 6420 696e 7374 6561  e emitted instea
+0001fa60: 6420 6f66 2061 6e0a 2020 2020 2020 2020  d of an.        
+0001fa70: 2020 2020 2020 6172 632e 0a20 2020 2020        arc..     
+0001fa80: 2020 2020 2020 202d 2049 6620 7468 6520         - If the 
+0001fa90: 7261 6469 6920 6172 6520 746f 6f20 736d  radii are too sm
+0001faa0: 616c 6c20 666f 7220 7468 6520 6172 6320  all for the arc 
+0001fab0: 746f 2072 6561 6368 2066 726f 6d20 7468  to reach from th
+0001fac0: 6520 6375 7272 656e 7420 706f 696e 7420  e current point 
+0001fad0: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
+0001fae0: 2074 6865 2073 7065 6369 6669 6564 2065   the specified e
+0001faf0: 6e64 2070 6f69 6e74 2028 6078 6020 616e  nd point (`x` an
+0001fb00: 6420 6079 6029 2c20 7468 656e 2074 6865  d `y`), then the
+0001fb10: 7920 7769 6c6c 2062 6520 7072 6f70 6f72  y will be propor
+0001fb20: 7469 6f6e 616c 6c79 0a20 2020 2020 2020  tionally.       
+0001fb30: 2020 2020 2020 2073 6361 6c65 6420 7570         scaled up
+0001fb40: 2075 6e74 696c 2074 6865 7920 6172 6520   until they are 
+0001fb50: 6269 6720 656e 6f75 6768 2c20 7768 6963  big enough, whic
+0001fb60: 6820 7769 6c6c 2061 6c77 6179 7320 7265  h will always re
+0001fb70: 7375 6c74 2069 6e20 610a 2020 2020 2020  sult in a.      
+0001fb80: 2020 2020 2020 2020 6861 6c66 2d65 6c6c          half-ell
+0001fb90: 6970 7365 2061 7263 2028 692e 652e 2061  ipse arc (i.e. a
+0001fba0: 6e20 3138 3020 6465 6772 6565 2073 7765  n 180 degree swe
+0001fbb0: 6570 290a 0a20 2020 2020 2020 2041 7267  ep)..        Arg
+0001fbc0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+0001fbd0: 7820 284e 756d 6265 7229 3a20 7261 6469  x (Number): radi
+0001fbe0: 7573 2069 6e20 7468 6520 782d 6469 7265  us in the x-dire
+0001fbf0: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
+0001fc00: 2020 2072 7920 284e 756d 6265 7229 3a20     ry (Number): 
+0001fc10: 7261 6469 7573 2069 6e20 7468 6520 792d  radius in the y-
+0001fc20: 6469 7265 6374 696f 6e2e 0a20 2020 2020  direction..     
+0001fc30: 2020 2020 2020 2072 6f74 6174 696f 6e20         rotation 
+0001fc40: 284e 756d 6265 7229 3a20 616e 676c 6520  (Number): angle 
+0001fc50: 2869 6e20 6465 6772 6565 7329 2074 6861  (in degrees) tha
+0001fc60: 7420 7468 6520 6172 6320 7368 6f75 6c64  t the arc should
+0001fc70: 2062 6520 726f 7461 7465 640a 2020 2020   be rotated.    
+0001fc80: 2020 2020 2020 2020 2020 2020 636c 6f63              cloc
+0001fc90: 6b77 6973 6520 6672 6f6d 2074 6865 2070  kwise from the p
+0001fca0: 7269 6e63 6970 6c65 2061 7865 732e 2054  rinciple axes. T
+0001fcb0: 6869 7320 7061 7261 6d65 7465 7220 646f  his parameter do
+0001fcc0: 6573 206e 6f74 2068 6176 650a 2020 2020  es not have.    
+0001fcd0: 2020 2020 2020 2020 2020 2020 6120 7669              a vi
+0001fce0: 7375 616c 2065 6666 6563 7420 696e 2074  sual effect in t
+0001fcf0: 6865 2063 6173 6520 7468 6174 2060 7278  he case that `rx
+0001fd00: 203d 3d20 7279 602e 0a20 2020 2020 2020   == ry`..       
+0001fd10: 2020 2020 206c 6172 6765 5f61 7263 2028       large_arc (
+0001fd20: 626f 6f6c 293a 2069 6620 5472 7565 2c20  bool): if True, 
+0001fd30: 7468 6520 6172 6320 7769 6c6c 2063 6f76  the arc will cov
+0001fd40: 6572 2061 2073 7765 6570 2061 6e67 6c65  er a sweep angle
+0001fd50: 206f 6620 6174 206c 6561 7374 2031 3830   of at least 180
+0001fd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fd70: 2064 6567 7265 6573 2e20 4f74 6865 7277   degrees. Otherw
+0001fd80: 6973 652c 2074 6865 2073 7765 6570 2061  ise, the sweep a
+0001fd90: 6e67 6c65 2077 696c 6c20 6265 2061 7420  ngle will be at 
+0001fda0: 6d6f 7374 2031 3830 2064 6567 7265 6573  most 180 degrees
+0001fdb0: 2e0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+0001fdc0: 7369 7469 7665 5f73 7765 6570 2028 626f  sitive_sweep (bo
+0001fdd0: 6f6c 293a 2069 6620 5472 7565 2c20 7468  ol): if True, th
+0001fde0: 6520 6172 6320 7769 6c6c 2062 6520 7377  e arc will be sw
+0001fdf0: 6570 7420 6f76 6572 2061 2070 6f73 6974  ept over a posit
+0001fe00: 6976 6520 616e 676c 652c 0a20 2020 2020  ive angle,.     
+0001fe10: 2020 2020 2020 2020 2020 2069 2e65 2e20             i.e. 
+0001fe20: 636c 6f63 6b77 6973 652e 204f 7468 6572  clockwise. Other
+0001fe30: 7769 7365 2c20 7468 6520 6172 6320 7769  wise, the arc wi
+0001fe40: 6c6c 2062 6520 7377 6570 7420 6f76 6572  ll be swept over
+0001fe50: 2061 206e 6567 6174 6976 650a 2020 2020   a negative.    
+0001fe60: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+0001fe70: 652e 0a20 2020 2020 2020 2020 2020 2064  e..            d
+0001fe80: 7820 284e 756d 6265 7229 3a20 6162 7363  x (Number): absc
+0001fe90: 6973 7361 206f 6620 7468 6520 6172 6327  issa of the arc'
+0001fea0: 7320 656e 6420 706f 696e 7420 7265 6c61  s end point rela
+0001feb0: 7469 7665 2074 6f20 7468 6520 656e 6420  tive to the end 
+0001fec0: 706f 696e 7420 6f66 0a20 2020 2020 2020  point of.       
+0001fed0: 2020 2020 2020 2020 2074 6865 2070 7265           the pre
+0001fee0: 7669 6f75 7320 7061 7468 2065 6c65 6d65  vious path eleme
+0001fef0: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
+0001ff00: 6479 2028 4e75 6d62 6572 293a 206f 7264  dy (Number): ord
+0001ff10: 696e 6174 6520 6f66 2074 6865 2061 7263  inate of the arc
+0001ff20: 2773 2065 6e64 2070 6f69 6e74 2072 656c  's end point rel
+0001ff30: 6174 6976 6520 746f 2074 6865 2065 6e64  ative to the end
+0001ff40: 2070 6f69 6e74 206f 660a 2020 2020 2020   point of.      
+0001ff50: 2020 2020 2020 2020 2020 7468 6520 7072            the pr
+0001ff60: 6576 696f 7573 2070 6174 6820 656c 656d  evious path elem
+0001ff70: 656e 742e 0a20 2020 2020 2020 2022 2222  ent..        """
+0001ff80: 0a20 2020 2020 2020 2069 6620 7278 203d  .        if rx =
+0001ff90: 3d20 3020 6f72 2072 7920 3d3d 2030 3a0a  = 0 or ry == 0:.
+0001ffa0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001ffb0: 726e 2073 656c 662e 6c69 6e65 5f72 656c  rn self.line_rel
+0001ffc0: 6174 6976 6528 6478 2c20 6479 290a 0a20  ative(dx, dy).. 
+0001ffd0: 2020 2020 2020 2072 6164 6969 203d 2050         radii = P
+0001ffe0: 6f69 6e74 2861 6273 2872 7829 2c20 6162  oint(abs(rx), ab
+0001fff0: 7328 7279 2929 0a20 2020 2020 2020 206c  s(ry)).        l
+00020000: 6172 6765 5f61 7263 203d 2062 6f6f 6c28  arge_arc = bool(
+00020010: 6c61 7267 655f 6172 6329 0a20 2020 2020  large_arc).     
+00020020: 2020 2072 6f74 6174 696f 6e20 3d20 6d61     rotation = ma
+00020030: 7468 2e72 6164 6961 6e73 2872 6f74 6174  th.radians(rotat
+00020040: 696f 6e29 0a20 2020 2020 2020 2070 6f73  ion).        pos
+00020050: 6974 6976 655f 7377 6565 7020 3d20 626f  itive_sweep = bo
+00020060: 6f6c 2870 6f73 6974 6976 655f 7377 6565  ol(positive_swee
+00020070: 7029 0a20 2020 2020 2020 2065 6e64 203d  p).        end =
+00020080: 2050 6f69 6e74 2864 782c 2064 7929 0a0a   Point(dx, dy)..
+00020090: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
+000200a0: 5f70 6174 685f 656c 656d 656e 7428 0a20  _path_element(. 
+000200b0: 2020 2020 2020 2020 2020 2052 656c 6174             Relat
+000200c0: 6976 6541 7263 2872 6164 6969 2c20 726f  iveArc(radii, ro
+000200d0: 7461 7469 6f6e 2c20 6c61 7267 655f 6172  tation, large_ar
+000200e0: 632c 2070 6f73 6974 6976 655f 7377 6565  c, positive_swee
+000200f0: 702c 2065 6e64 292c 205f 636f 7079 3d46  p, end), _copy=F
+00020100: 616c 7365 0a20 2020 2020 2020 2029 0a20  alse.        ). 
+00020110: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00020120: 6c66 0a0a 2020 2020 6465 6620 636c 6f73  lf..    def clos
+00020130: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00020140: 2022 2222 0a20 2020 2020 2020 2045 7870   """.        Exp
+00020150: 6c69 6369 746c 7920 636c 6f73 6520 7468  licitly close th
+00020160: 6520 6375 7272 656e 7420 2873 7562 2970  e current (sub)p
+00020170: 6174 682e 0a20 2020 2020 2020 2022 2222  ath..        """
+00020180: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00020190: 645f 7061 7468 5f65 6c65 6d65 6e74 2843  d_path_element(C
+000201a0: 6c6f 7365 2829 2c20 5f63 6f70 793d 4661  lose(), _copy=Fa
+000201b0: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
+000201c0: 662e 5f63 6c6f 7365 6420 3d20 5472 7565  f._closed = True
+000201d0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+000201e0: 7665 5f72 656c 6174 6976 6528 302c 2030  ve_relative(0, 0
+000201f0: 290a 0a20 2020 2064 6566 205f 696e 7365  )..    def _inse
+00020200: 7274 5f69 6d70 6c69 6369 745f 636c 6f73  rt_implicit_clos
+00020210: 655f 6966 5f6f 7065 6e28 7365 6c66 293a  e_if_open(self):
+00020220: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00020230: 7365 6c66 2e5f 636c 6f73 6564 3a0a 2020  self._closed:.  
+00020240: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00020250: 636c 6f73 655f 636f 6e74 6578 742e 6164  close_context.ad
+00020260: 645f 6974 656d 2849 6d70 6c69 6369 7443  d_item(ImplicitC
+00020270: 6c6f 7365 2829 2c20 5f63 6f70 793d 4661  lose(), _copy=Fa
+00020280: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00020290: 2073 656c 662e 5f63 6c6f 7365 5f63 6f6e   self._close_con
+000202a0: 7465 7874 203d 2073 656c 662e 5f67 7261  text = self._gra
+000202b0: 7068 6963 735f 636f 6e74 6578 740a 2020  phics_context.  
+000202c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000202d0: 636c 6f73 6564 203d 2054 7275 650a 0a20  closed = True.. 
+000202e0: 2020 2064 6566 2072 656e 6465 7228 0a20     def render(. 
+000202f0: 2020 2020 2020 2073 656c 662c 2067 7364         self, gsd
+00020300: 5f72 6567 6973 7472 792c 2073 7479 6c65  _registry, style
+00020310: 2c20 6c61 7374 5f69 7465 6d2c 2069 6e69  , last_item, ini
+00020320: 7469 616c 5f70 6f69 6e74 2c20 6465 6275  tial_point, debu
+00020330: 675f 7374 7265 616d 3d4e 6f6e 652c 2070  g_stream=None, p
+00020340: 6678 3d4e 6f6e 650a 2020 2020 293a 0a20  fx=None.    ):. 
+00020350: 2020 2020 2020 2073 656c 662e 5f69 6e73         self._ins
+00020360: 6572 745f 696d 706c 6963 6974 5f63 6c6f  ert_implicit_clo
+00020370: 7365 5f69 665f 6f70 656e 2829 0a0a 2020  se_if_open()..  
+00020380: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+00020390: 2020 2020 7265 6e64 6572 5f6c 6973 742c      render_list,
+000203a0: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
+000203b0: 745f 6974 656d 2c0a 2020 2020 2020 2020  t_item,.        
+000203c0: 2020 2020 696e 6974 6961 6c5f 706f 696e      initial_poin
+000203d0: 742c 0a20 2020 2020 2020 2029 203d 2073  t,.        ) = s
+000203e0: 656c 662e 5f72 6f6f 745f 6772 6170 6869  elf._root_graphi
+000203f0: 6373 5f63 6f6e 7465 7874 2e62 7569 6c64  cs_context.build
+00020400: 5f72 656e 6465 725f 6c69 7374 280a 2020  _render_list(.  
+00020410: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
+00020420: 6769 7374 7279 2c20 7374 796c 652c 206c  gistry, style, l
+00020430: 6173 745f 6974 656d 2c20 696e 6974 6961  ast_item, initia
+00020440: 6c5f 706f 696e 742c 2064 6562 7567 5f73  l_point, debug_s
+00020450: 7472 6561 6d2c 2070 6678 0a20 2020 2020  tream, pfx.     
+00020460: 2020 2029 0a0a 2020 2020 2020 2020 7061     )..        pa
+00020470: 696e 745f 7275 6c65 203d 2047 7261 7068  int_rule = Graph
+00020480: 6963 7353 7479 6c65 2e6d 6572 6765 2873  icsStyle.merge(s
+00020490: 7479 6c65 2c20 7365 6c66 2e73 7479 6c65  tyle, self.style
+000204a0: 292e 7265 736f 6c76 655f 7061 696e 745f  ).resolve_paint_
+000204b0: 7275 6c65 2829 0a0a 2020 2020 2020 2020  rule()..        
+000204c0: 7265 6e64 6572 5f6c 6973 742e 696e 7365  render_list.inse
+000204d0: 7274 282d 312c 2070 6169 6e74 5f72 756c  rt(-1, paint_rul
+000204e0: 652e 7661 6c75 6529 0a0a 2020 2020 2020  e.value)..      
+000204f0: 2020 7265 7475 726e 2022 2022 2e6a 6f69    return " ".joi
+00020500: 6e28 7265 6e64 6572 5f6c 6973 7429 2c20  n(render_list), 
+00020510: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
+00020520: 616c 5f70 6f69 6e74 0a0a 2020 2020 6465  al_point..    de
+00020530: 6620 7265 6e64 6572 5f64 6562 7567 280a  f render_debug(.
+00020540: 2020 2020 2020 2020 7365 6c66 2c20 6773          self, gs
+00020550: 645f 7265 6769 7374 7279 2c20 7374 796c  d_registry, styl
+00020560: 652c 206c 6173 745f 6974 656d 2c20 696e  e, last_item, in
+00020570: 6974 6961 6c5f 706f 696e 742c 2064 6562  itial_point, deb
+00020580: 7567 5f73 7472 6561 6d2c 2070 6678 0a20  ug_stream, pfx. 
+00020590: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+000205a0: 220a 2020 2020 2020 2020 5265 6e64 6572  ".        Render
+000205b0: 2074 6869 7320 7061 7468 2065 6c65 6d65   this path eleme
+000205c0: 6e74 2074 6f20 6974 7320 5044 4620 7265  nt to its PDF re
+000205d0: 7072 6573 656e 7461 7469 6f6e 2061 6e64  presentation and
+000205e0: 2070 726f 6475 6365 2064 6562 7567 0a20   produce debug. 
+000205f0: 2020 2020 2020 2069 6e66 6f72 6d61 7469         informati
+00020600: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
+00020610: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+00020620: 7364 5f72 6567 6973 7472 7920 2847 7261  sd_registry (Gra
+00020630: 7068 6963 7353 7461 7465 4469 6374 5265  phicsStateDictRe
+00020640: 6769 7374 7279 293a 2074 6865 206f 776e  gistry): the own
+00020650: 6572 2773 2067 7261 7068 6963 7320 7374  er's graphics st
+00020660: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+00020670: 2020 2020 6469 6374 696f 6e61 7279 2072      dictionary r
+00020680: 6567 6973 7472 792e 0a20 2020 2020 2020  egistry..       
+00020690: 2020 2020 2073 7479 6c65 2028 4772 6170       style (Grap
+000206a0: 6869 6373 5374 796c 6529 3a20 7468 6520  hicsStyle): the 
+000206b0: 6375 7272 656e 7420 7265 736f 6c76 6564  current resolved
+000206c0: 2067 7261 7068 6963 7320 7374 796c 650a   graphics style.
+000206d0: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+000206e0: 5f69 7465 6d3a 2074 6865 2070 7265 7669  _item: the previ
+000206f0: 6f75 7320 7061 7468 2065 6c65 6d65 6e74  ous path element
+00020700: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00020710: 6974 6961 6c5f 706f 696e 743a 206c 6173  itial_point: las
+00020720: 7420 706f 7369 7469 6f6e 2073 6574 2062  t position set b
+00020730: 7920 6120 224d 2220 6f72 2022 6d22 2063  y a "M" or "m" c
+00020740: 6f6d 6d61 6e64 0a20 2020 2020 2020 2020  ommand.         
+00020750: 2020 2064 6562 7567 5f73 7472 6561 6d20     debug_stream 
+00020760: 2869 6f2e 5465 7874 494f 293a 2074 6865  (io.TextIO): the
+00020770: 2073 7472 6561 6d20 746f 2077 6869 6368   stream to which
+00020780: 2074 6865 2064 6562 7567 206f 7574 7075   the debug outpu
+00020790: 7420 7368 6f75 6c64 2062 650a 2020 2020  t should be.    
+000207a0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+000207b0: 7465 6e2e 2054 6869 7320 6973 206e 6f74  ten. This is not
+000207c0: 2067 7561 7261 6e74 6565 6420 746f 2062   guaranteed to b
+000207d0: 6520 7365 656b 6162 6c65 2028 652e 672e  e seekable (e.g.
+000207e0: 2069 7420 6d61 7920 6265 2073 7464 6f75   it may be stdou
+000207f0: 7420 6f72 0a20 2020 2020 2020 2020 2020  t or.           
+00020800: 2020 2020 2073 7464 6572 7229 2e0a 2020       stderr)..  
+00020810: 2020 2020 2020 2020 2020 7066 7820 2873            pfx (s
+00020820: 7472 293a 2074 6865 2063 7572 7265 6e74  tr): the current
+00020830: 2064 6562 7567 206f 7574 7075 7420 7072   debug output pr
+00020840: 6566 6978 2073 7472 696e 6720 286f 6e6c  efix string (onl
+00020850: 7920 6e65 6564 6564 2069 6620 656d 6974  y needed if emit
+00020860: 7469 6e67 0a20 2020 2020 2020 2020 2020  ting.           
+00020870: 2020 2020 206d 6f72 6520 7468 616e 206f       more than o
+00020880: 6e65 206c 696e 6529 2e0a 0a20 2020 2020  ne line)...     
+00020890: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000208a0: 2020 2020 2020 2020 5468 6520 7361 6d65          The same
+000208b0: 2074 7570 6c65 2061 7320 6050 6169 6e74   tuple as `Paint
+000208c0: 6564 5061 7468 2e72 656e 6465 7260 2e0a  edPath.render`..
+000208d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000208e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000208f0: 7265 6e64 6572 280a 2020 2020 2020 2020  render(.        
+00020900: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
+00020910: 2c20 7374 796c 652c 206c 6173 745f 6974  , style, last_it
+00020920: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
+00020930: 742c 2064 6562 7567 5f73 7472 6561 6d2c  t, debug_stream,
+00020940: 2070 6678 0a20 2020 2020 2020 2029 0a0a   pfx.        )..
+00020950: 0a63 6c61 7373 2043 6c69 7070 696e 6750  .class ClippingP
+00020960: 6174 6828 5061 696e 7465 6450 6174 6829  ath(PaintedPath)
+00020970: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
+00020980: 6520 5061 696e 7465 6450 6174 6820 4150  e PaintedPath AP
+00020990: 4920 6275 7420 746f 2062 6520 7573 6564  I but to be used
+000209a0: 2074 6f20 6372 6561 7465 2063 6c69 7070   to create clipp
+000209b0: 696e 6720 7061 7468 732e 0a0a 2020 2020  ing paths...    
+000209c0: 2e2e 2077 6172 6e69 6e67 3a3a 0a20 2020  .. warning::.   
+000209d0: 2020 2020 2055 6e6c 6573 7320 796f 7520       Unless you 
+000209e0: 7265 616c 6c79 206b 6e6f 7720 7768 6174  really know what
+000209f0: 2079 6f75 2772 6520 646f 696e 672c 2063   you're doing, c
+00020a00: 6861 6e67 696e 6720 6174 7472 6962 7574  hanging attribut
+00020a10: 6573 206f 6620 7468 6520 636c 6970 7069  es of the clippi
+00020a20: 6e67 0a20 2020 2020 2020 2070 6174 6820  ng.        path 
+00020a30: 7374 796c 6520 6973 206c 696b 656c 7920  style is likely 
+00020a40: 746f 2070 726f 6475 6365 2075 6e65 7870  to produce unexp
+00020a50: 6563 7465 6420 7265 7375 6c74 732e 2054  ected results. T
+00020a60: 6869 7320 6973 2062 6563 6175 7365 2074  his is because t
+00020a70: 6865 0a20 2020 2020 2020 2063 6c69 7070  he.        clipp
+00020a80: 696e 6720 7061 7468 2073 7479 6c65 7320  ing path styles 
+00020a90: 6f76 6572 7269 6465 2069 6d70 6c69 6369  override implici
+00020aa0: 7420 7374 796c 6520 696e 6865 7269 7461  t style inherita
+00020ab0: 6e63 6520 6f66 2074 6865 2060 5061 696e  nce of the `Pain
+00020ac0: 7465 6450 6174 6860 0a20 2020 2020 2020  tedPath`.       
+00020ad0: 2069 7420 6170 706c 6965 7320 746f 2e0a   it applies to..
+00020ae0: 0a20 2020 2020 2020 2046 6f72 2065 7861  .        For exa
+00020af0: 6d70 6c65 2c20 6063 6c69 7070 6174 682e  mple, `clippath.
+00020b00: 7374 796c 652e 7374 726f 6b65 5f77 6964  style.stroke_wid
+00020b10: 7468 203d 2032 6020 6361 6e20 756e 6578  th = 2` can unex
+00020b20: 7065 6374 6564 6c79 206f 7665 7272 6964  pectedly overrid
+00020b30: 650a 2020 2020 2020 2020 6070 6169 6e74  e.        `paint
+00020b40: 7061 7468 2e73 7479 6c65 2e73 7472 6f6b  path.style.strok
+00020b50: 655f 7769 6474 6820 3d20 4772 6170 6869  e_width = Graphi
+00020b60: 6373 5374 796c 652e 494e 4845 5249 5460  csStyle.INHERIT`
+00020b70: 2061 6e64 2063 6175 7365 2074 6865 2070   and cause the p
+00020b80: 6169 6e74 6564 0a20 2020 2020 2020 2070  ainted.        p
+00020b90: 6174 6820 746f 2062 6520 7265 6e64 6572  ath to be render
+00020ba0: 6564 2077 6974 6820 6120 7374 726f 6b65  ed with a stroke
+00020bb0: 206f 6620 3220 696e 7374 6561 6420 6f66   of 2 instead of
+00020bc0: 2077 6861 7420 6974 2077 6f75 6c64 2068   what it would h
+00020bd0: 6176 6520 6e6f 726d 616c 6c79 0a20 2020  ave normally.   
+00020be0: 2020 2020 2069 6e68 6572 6974 6564 2e20       inherited. 
+00020bf0: 4265 6361 7573 6520 6120 6043 6c69 7070  Because a `Clipp
+00020c00: 696e 6750 6174 6860 2063 616e 2062 6520  ingPath` can be 
+00020c10: 7061 696e 7465 6420 6c69 6b65 2061 206e  painted like a n
+00020c20: 6f72 6d61 6c20 6050 6169 6e74 6564 5061  ormal `PaintedPa
+00020c30: 7468 602c 0a20 2020 2020 2020 2069 7420  th`,.        it 
+00020c40: 776f 756c 6420 6265 206f 7665 726c 7920  would be overly 
+00020c50: 7265 7374 7269 6374 6976 6520 746f 2072  restrictive to r
+00020c60: 656d 6f76 6520 7468 6520 6162 696c 6974  emove the abilit
+00020c70: 7920 746f 2073 7479 6c65 2069 742c 2073  y to style it, s
+00020c80: 6f20 696e 7374 6561 640a 2020 2020 2020  o instead.      
+00020c90: 2020 7468 6973 2077 6172 6e69 6e67 2069    this warning i
+00020ca0: 7320 6865 7265 2e0a 2020 2020 2222 220a  s here..    """.
+00020cb0: 0a20 2020 2023 2062 6563 6175 7365 2063  .    # because c
+00020cc0: 6c69 7070 696e 6720 7061 7468 7320 6361  lipping paths ca
+00020cd0: 6e20 6265 2070 6169 6e74 6564 2c20 7765  n be painted, we
+00020ce0: 2069 6e68 6572 6974 2066 726f 6d20 5061   inherit from Pa
+00020cf0: 696e 7465 6450 6174 682e 2048 6f77 6576  intedPath. Howev
+00020d00: 6572 2c20 7768 656e 0a20 2020 2023 2073  er, when.    # s
+00020d10: 6574 7469 6e67 2074 6865 2073 7479 6c69  etting the styli
+00020d20: 6e67 206f 6e20 7468 6520 636c 6970 7069  ng on the clippi
+00020d30: 6e67 2070 6174 682c 2074 686f 7365 2076  ng path, those v
+00020d40: 616c 7565 7320 7769 6c6c 2061 6c73 6f20  alues will also 
+00020d50: 6265 2061 7070 6c69 6564 2074 6f0a 2020  be applied to.  
+00020d60: 2020 2320 7468 6520 5061 696e 7465 6450    # the PaintedP
+00020d70: 6174 6820 7468 6520 436c 6970 7069 6e67  ath the Clipping
+00020d80: 5061 7468 2069 7320 6170 706c 6965 6420  Path is applied 
+00020d90: 746f 2075 6e6c 6573 7320 7468 6579 2061  to unless they a
+00020da0: 7265 2065 7870 6c69 6369 746c 7920 7365  re explicitly se
+00020db0: 7420 666f 720a 2020 2020 2320 7468 6174  t for.    # that
+00020dc0: 2070 6169 6e74 6564 2070 6174 682e 2054   painted path. T
+00020dd0: 6869 7320 6973 206e 6f74 2069 6465 616c  his is not ideal
+00020de0: 2c20 6275 7420 7468 6572 6527 7320 6e6f  , but there's no
+00020df0: 2077 6179 2074 6f20 7265 616c 6c79 2066   way to really f
+00020e00: 6978 2069 7420 6672 6f6d 0a20 2020 2023  ix it from.    #
+00020e10: 2074 6865 2050 4446 2072 656e 6465 7269   the PDF renderi
+00020e20: 6e67 206d 6f64 656c 2c20 616e 6420 7472  ng model, and tr
+00020e30: 7969 6e67 2074 6f20 7472 6163 6b20 7468  ying to track th
+00020e40: 6520 6170 7072 6f70 7269 6174 6520 7374  e appropriate st
+00020e50: 6174 652f 6465 6661 756c 7473 2073 6565  ate/defaults see
+00020e60: 6d73 0a20 2020 2023 2073 696d 696c 6172  ms.    # similar
+00020e70: 6c79 2065 7272 6f72 2070 726f 6e65 2e0a  ly error prone..
+00020e80: 0a20 2020 2023 2049 6e20 6765 6e65 7261  .    # In genera
+00020e90: 6c2c 2074 6865 2065 7870 6563 7461 7469  l, the expectati
+00020ea0: 6f6e 2069 7320 7468 6174 2070 6169 6e74  on is that paint
+00020eb0: 6564 2063 6c69 7070 696e 6720 7061 7468  ed clipping path
+00020ec0: 7320 6172 6520 6c69 6b65 6c79 2074 6f20  s are likely to 
+00020ed0: 6265 2076 6572 790a 2020 2020 2320 756e  be very.    # un
+00020ee0: 636f 6d6d 6f6e 2c20 736f 2069 7427 7320  common, so it's 
+00020ef0: 616e 2065 6467 6520 6361 7365 2074 6861  an edge case tha
+00020f00: 7420 6973 6e27 7420 776f 7274 6820 776f  t isn't worth wo
+00020f10: 7272 7969 6e67 2074 6f6f 206d 7563 6820  rrying too much 
+00020f20: 6162 6f75 742e 0a0a 2020 2020 6465 6620  about...    def 
+00020f30: 5f5f 696e 6974 5f5f 2873 656c 662c 2078  __init__(self, x
+00020f40: 3d30 2c20 793d 3029 3a0a 2020 2020 2020  =0, y=0):.      
+00020f50: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00020f60: 5f5f 2878 3d78 2c20 793d 7929 0a20 2020  __(x=x, y=y).   
+00020f70: 2020 2020 2073 656c 662e 7061 696e 745f       self.paint_
+00020f80: 7275 6c65 203d 2050 6174 6850 6169 6e74  rule = PathPaint
+00020f90: 5275 6c65 2e44 4f4e 545f 5041 494e 540a  Rule.DONT_PAINT.
+00020fa0: 0a20 2020 2064 6566 2072 656e 6465 7228  .    def render(
+00020fb0: 0a20 2020 2020 2020 2073 656c 662c 2067  .        self, g
+00020fc0: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
+00020fd0: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
+00020fe0: 6e69 7469 616c 5f70 6f69 6e74 2c20 6465  nitial_point, de
+00020ff0: 6275 675f 7374 7265 616d 3d4e 6f6e 652c  bug_stream=None,
+00021000: 2070 6678 3d4e 6f6e 650a 2020 2020 293a   pfx=None.    ):
+00021010: 0a20 2020 2020 2020 2023 2070 6169 6e74  .        # paint
+00021020: 696e 6720 7468 6520 636c 6970 7069 6e67  ing the clipping
+00021030: 2070 6174 6820 6f75 7473 6964 6520 6f66   path outside of
+00021040: 2069 7473 2072 6f6f 7420 6772 6170 6869   its root graphi
+00021050: 6373 2063 6f6e 7465 7874 2061 6c6c 6f77  cs context allow
+00021060: 7320 6974 2074 6f0a 2020 2020 2020 2020  s it to.        
+00021070: 2320 6265 2074 7261 6e73 666f 726d 6564  # be transformed
+00021080: 2077 6974 686f 7574 2061 6666 6563 7469   without affecti
+00021090: 6e67 2074 6865 2074 7261 6e73 666f 726d  ng the transform
+000210a0: 206f 6620 7468 6520 6772 6170 6869 6373   of the graphics
+000210b0: 2063 6f6e 7465 7874 206f 6620 7468 650a   context of the.
+000210c0: 2020 2020 2020 2020 2320 7061 7468 2069          # path i
+000210d0: 7420 6973 2062 6569 6e67 2075 7365 6420  t is being used 
+000210e0: 746f 2063 6c69 702e 2054 6869 7320 6973  to clip. This is
+000210f0: 2062 6563 6175 7365 2c20 756e 6c69 6b65   because, unlike
+00021100: 2061 6c6c 206f 6620 7468 6520 6f74 6865   all of the othe
+00021110: 7220 7374 796c 650a 2020 2020 2020 2020  r style.        
+00021120: 2320 7365 7474 696e 6773 2c20 7472 616e  # settings, tran
+00021130: 7366 6f72 6d61 7469 6f6e 7320 696d 6d65  sformations imme
+00021140: 6469 6174 656c 7920 6166 6665 6374 2074  diately affect t
+00021150: 6865 2070 6f69 6e74 7320 666f 6c6c 6f77  he points follow
+00021160: 696e 6720 7468 656d 2c0a 2020 2020 2020  ing them,.      
+00021170: 2020 2320 7261 7468 6572 2074 6861 6e20    # rather than 
+00021180: 6f6e 6c79 2061 6666 6563 7469 6e67 2074  only affecting t
+00021190: 6865 6d20 6174 2070 6169 6e74 696e 6720  hem at painting 
+000211a0: 7469 6d65 2e20 7374 726f 6b65 2073 6574  time. stroke set
+000211b0: 7469 6e67 7320 616e 6420 636f 6c6f 720a  tings and color.
+000211c0: 2020 2020 2020 2020 2320 7365 7474 696e          # settin
+000211d0: 6773 2061 7265 2061 7070 6c69 6564 206f  gs are applied o
+000211e0: 6e6c 7920 6174 2070 6169 6e74 2074 696d  nly at paint tim
+000211f0: 652e 0a0a 2020 2020 2020 2020 6966 2064  e...        if d
+00021200: 6562 7567 5f73 7472 6561 6d3a 0a20 2020  ebug_stream:.   
+00021210: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
+00021220: 7472 6561 6d2e 7772 6974 6528 223c 436c  tream.write("<Cl
+00021230: 6970 7069 6e67 5061 7468 3e20 2229 0a0a  ippingPath> ")..
+00021240: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+00021250: 2020 2020 2020 7265 6e64 6572 5f6c 6973        render_lis
+00021260: 742c 0a20 2020 2020 2020 2020 2020 206c  t,.            l
+00021270: 6173 745f 6974 656d 2c0a 2020 2020 2020  ast_item,.      
+00021280: 2020 2020 2020 696e 6974 6961 6c5f 706f        initial_po
+00021290: 696e 742c 0a20 2020 2020 2020 2029 203d  int,.        ) =
+000212a0: 2073 656c 662e 5f72 6f6f 745f 6772 6170   self._root_grap
+000212b0: 6869 6373 5f63 6f6e 7465 7874 2e62 7569  hics_context.bui
+000212c0: 6c64 5f72 656e 6465 725f 6c69 7374 280a  ld_render_list(.
+000212d0: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
+000212e0: 7265 6769 7374 7279 2c0a 2020 2020 2020  registry,.      
+000212f0: 2020 2020 2020 7374 796c 652c 0a20 2020        style,.   
+00021300: 2020 2020 2020 2020 206c 6173 745f 6974           last_it
+00021310: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
+00021320: 696e 6974 6961 6c5f 706f 696e 742c 0a20  initial_point,. 
+00021330: 2020 2020 2020 2020 2020 2064 6562 7567             debug
+00021340: 5f73 7472 6561 6d2c 0a20 2020 2020 2020  _stream,.       
+00021350: 2020 2020 2070 6678 2c0a 2020 2020 2020       pfx,.      
+00021360: 2020 2020 2020 5f70 7573 685f 7374 6163        _push_stac
+00021370: 6b3d 4661 6c73 652c 0a20 2020 2020 2020  k=False,.       
+00021380: 2029 0a0a 2020 2020 2020 2020 6d65 7267   )..        merg
+00021390: 6564 5f73 7479 6c65 203d 2047 7261 7068  ed_style = Graph
+000213a0: 6963 7353 7479 6c65 2e6d 6572 6765 2873  icsStyle.merge(s
+000213b0: 7479 6c65 2c20 7365 6c66 2e73 7479 6c65  tyle, self.style
+000213c0: 290a 2020 2020 2020 2020 2320 7765 2073  ).        # we s
+000213d0: 686f 756c 6420 6e65 7665 7220 6765 7420  hould never get 
+000213e0: 6120 636f 6c6c 6973 696f 6e20 6572 726f  a collision erro
+000213f0: 7220 6865 7265 0a20 2020 2020 2020 2069  r here.        i
+00021400: 6e74 6572 7365 6374 696f 6e5f 7275 6c65  ntersection_rule
+00021410: 203d 206d 6572 6765 645f 7374 796c 652e   = merged_style.
+00021420: 696e 7465 7273 6563 7469 6f6e 5f72 756c  intersection_rul
+00021430: 650a 2020 2020 2020 2020 6966 2069 6e74  e.        if int
+00021440: 6572 7365 6374 696f 6e5f 7275 6c65 2069  ersection_rule i
+00021450: 7320 6d65 7267 6564 5f73 7479 6c65 2e49  s merged_style.I
+00021460: 4e48 4552 4954 3a0a 2020 2020 2020 2020  NHERIT:.        
+00021470: 2020 2020 696e 7465 7273 6563 7469 6f6e      intersection
+00021480: 5f72 756c 6520 3d20 436c 6970 7069 6e67  _rule = Clipping
+00021490: 5061 7468 496e 7465 7273 6563 7469 6f6e  PathIntersection
+000214a0: 5275 6c65 2e4e 4f4e 5a45 524f 0a20 2020  Rule.NONZERO.   
+000214b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000214c0: 2020 2020 2020 2069 6e74 6572 7365 6374         intersect
+000214d0: 696f 6e5f 7275 6c65 203d 2043 6c69 7070  ion_rule = Clipp
+000214e0: 696e 6750 6174 6849 6e74 6572 7365 6374  ingPathIntersect
+000214f0: 696f 6e52 756c 655b 0a20 2020 2020 2020  ionRule[.       
+00021500: 2020 2020 2020 2020 2069 6e74 6572 7365           interse
+00021510: 6374 696f 6e5f 7275 6c65 2e6e 616d 6520  ction_rule.name 
+00021520: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00021530: 6c65 3d6e 6f2d 6d65 6d62 6572 2c20 7573  le=no-member, us
+00021540: 656c 6573 732d 7375 7070 7265 7373 696f  eless-suppressio
+00021550: 6e0a 2020 2020 2020 2020 2020 2020 5d0a  n.            ].
+00021560: 0a20 2020 2020 2020 2070 6169 6e74 5f72  .        paint_r
+00021570: 756c 6520 3d20 6d65 7267 6564 5f73 7479  ule = merged_sty
+00021580: 6c65 2e72 6573 6f6c 7665 5f70 6169 6e74  le.resolve_paint
+00021590: 5f72 756c 6528 290a 0a20 2020 2020 2020  _rule()..       
+000215a0: 2072 656e 6465 725f 6c69 7374 2e61 7070   render_list.app
+000215b0: 656e 6428 696e 7465 7273 6563 7469 6f6e  end(intersection
+000215c0: 5f72 756c 652e 7661 6c75 6529 0a20 2020  _rule.value).   
+000215d0: 2020 2020 2072 656e 6465 725f 6c69 7374       render_list
+000215e0: 2e61 7070 656e 6428 7061 696e 745f 7275  .append(paint_ru
+000215f0: 6c65 2e76 616c 7565 290a 0a20 2020 2020  le.value)..     
+00021600: 2020 2072 6574 7572 6e20 2220 222e 6a6f     return " ".jo
+00021610: 696e 2872 656e 6465 725f 6c69 7374 292c  in(render_list),
+00021620: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
+00021630: 6961 6c5f 706f 696e 740a 0a20 2020 2064  ial_point..    d
+00021640: 6566 2072 656e 6465 725f 6465 6275 6728  ef render_debug(
+00021650: 0a20 2020 2020 2020 2073 656c 662c 2067  .        self, g
+00021660: 7364 5f72 6567 6973 7472 792c 2073 7479  sd_registry, sty
+00021670: 6c65 2c20 6c61 7374 5f69 7465 6d2c 2069  le, last_item, i
+00021680: 6e69 7469 616c 5f70 6f69 6e74 2c20 6465  nitial_point, de
+00021690: 6275 675f 7374 7265 616d 2c20 7066 780a  bug_stream, pfx.
+000216a0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+000216b0: 2222 0a20 2020 2020 2020 2052 656e 6465  "".        Rende
+000216c0: 7220 7468 6973 2070 6174 6820 656c 656d  r this path elem
+000216d0: 656e 7420 746f 2069 7473 2050 4446 2072  ent to its PDF r
+000216e0: 6570 7265 7365 6e74 6174 696f 6e20 616e  epresentation an
+000216f0: 6420 7072 6f64 7563 6520 6465 6275 670a  d produce debug.
+00021700: 2020 2020 2020 2020 696e 666f 726d 6174          informat
+00021710: 696f 6e2e 0a0a 2020 2020 2020 2020 4172  ion...        Ar
+00021720: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00021730: 6773 645f 7265 6769 7374 7279 2028 4772  gsd_registry (Gr
+00021740: 6170 6869 6373 5374 6174 6544 6963 7452  aphicsStateDictR
+00021750: 6567 6973 7472 7929 3a20 7468 6520 6f77  egistry): the ow
+00021760: 6e65 7227 7320 6772 6170 6869 6373 2073  ner's graphics s
+00021770: 7461 7465 0a20 2020 2020 2020 2020 2020  tate.           
+00021780: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
+00021790: 7265 6769 7374 7279 2e0a 2020 2020 2020  registry..      
+000217a0: 2020 2020 2020 7374 796c 6520 2847 7261        style (Gra
+000217b0: 7068 6963 7353 7479 6c65 293a 2074 6865  phicsStyle): the
+000217c0: 2063 7572 7265 6e74 2072 6573 6f6c 7665   current resolve
+000217d0: 6420 6772 6170 6869 6373 2073 7479 6c65  d graphics style
+000217e0: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
+000217f0: 745f 6974 656d 3a20 7468 6520 7072 6576  t_item: the prev
+00021800: 696f 7573 2070 6174 6820 656c 656d 656e  ious path elemen
+00021810: 742e 0a20 2020 2020 2020 2020 2020 2064  t..            d
+00021820: 6562 7567 5f73 7472 6561 6d20 2869 6f2e  ebug_stream (io.
+00021830: 5465 7874 494f 293a 2074 6865 2073 7472  TextIO): the str
+00021840: 6561 6d20 746f 2077 6869 6368 2074 6865  eam to which the
+00021850: 2064 6562 7567 206f 7574 7075 7420 7368   debug output sh
+00021860: 6f75 6c64 2062 650a 2020 2020 2020 2020  ould be.        
+00021870: 2020 2020 2020 2020 7772 6974 7465 6e2e          written.
+00021880: 2054 6869 7320 6973 206e 6f74 2067 7561   This is not gua
+00021890: 7261 6e74 6565 6420 746f 2062 6520 7365  ranteed to be se
+000218a0: 656b 6162 6c65 2028 652e 672e 2069 7420  ekable (e.g. it 
+000218b0: 6d61 7920 6265 2073 7464 6f75 7420 6f72  may be stdout or
+000218c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000218d0: 2073 7464 6572 7229 2e0a 2020 2020 2020   stderr)..      
+000218e0: 2020 2020 2020 7066 7820 2873 7472 293a        pfx (str):
+000218f0: 2074 6865 2063 7572 7265 6e74 2064 6562   the current deb
+00021900: 7567 206f 7574 7075 7420 7072 6566 6978  ug output prefix
+00021910: 2073 7472 696e 6720 286f 6e6c 7920 6e65   string (only ne
+00021920: 6564 6564 2069 6620 656d 6974 7469 6e67  eded if emitting
+00021930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021940: 206d 6f72 6520 7468 616e 206f 6e65 206c   more than one l
+00021950: 696e 6529 2e0a 0a20 2020 2020 2020 2052  ine)...        R
+00021960: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00021970: 2020 2020 5468 6520 7361 6d65 2074 7570      The same tup
+00021980: 6c65 2061 7320 6043 6c69 7070 696e 6750  le as `ClippingP
+00021990: 6174 682e 7265 6e64 6572 602e 0a20 2020  ath.render`..   
+000219a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000219b0: 2072 6574 7572 6e20 7365 6c66 2e72 656e   return self.ren
+000219c0: 6465 7228 0a20 2020 2020 2020 2020 2020  der(.           
+000219d0: 2067 7364 5f72 6567 6973 7472 792c 2073   gsd_registry, s
+000219e0: 7479 6c65 2c20 6c61 7374 5f69 7465 6d2c  tyle, last_item,
+000219f0: 2069 6e69 7469 616c 5f70 6f69 6e74 2c20   initial_point, 
+00021a00: 6465 6275 675f 7374 7265 616d 2c20 7066  debug_stream, pf
+00021a10: 780a 2020 2020 2020 2020 290a 0a0a 636c  x.        )...cl
+00021a20: 6173 7320 4772 6170 6869 6373 436f 6e74  ass GraphicsCont
+00021a30: 6578 743a 0a20 2020 2064 6566 205f 5f69  ext:.    def __i
+00021a40: 6e69 745f 5f28 7365 6c66 293a 0a20 2020  nit__(self):.   
+00021a50: 2020 2020 2073 656c 662e 7374 796c 6520       self.style 
+00021a60: 3d20 4772 6170 6869 6373 5374 796c 6528  = GraphicsStyle(
+00021a70: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+00021a80: 6174 685f 6974 656d 7320 3d20 5b5d 0a0a  ath_items = []..
+00021a90: 2020 2020 2020 2020 7365 6c66 2e5f 7472          self._tr
+00021aa0: 616e 7366 6f72 6d20 3d20 4e6f 6e65 0a20  ansform = None. 
+00021ab0: 2020 2020 2020 2073 656c 662e 5f63 6c69         self._cli
+00021ac0: 7070 696e 675f 7061 7468 203d 204e 6f6e  pping_path = Non
+00021ad0: 650a 0a20 2020 2064 6566 205f 5f64 6565  e..    def __dee
+00021ae0: 7063 6f70 795f 5f28 7365 6c66 2c20 6d65  pcopy__(self, me
+00021af0: 6d6f 293a 0a20 2020 2020 2020 2063 6f70  mo):.        cop
+00021b00: 6965 6420 3d20 7365 6c66 2e5f 5f63 6c61  ied = self.__cla
+00021b10: 7373 5f5f 2829 0a20 2020 2020 2020 2063  ss__().        c
+00021b20: 6f70 6965 642e 7374 796c 6520 3d20 636f  opied.style = co
+00021b30: 7079 2e64 6565 7063 6f70 7928 7365 6c66  py.deepcopy(self
+00021b40: 2e73 7479 6c65 2c20 6d65 6d6f 290a 2020  .style, memo).  
+00021b50: 2020 2020 2020 636f 7069 6564 2e70 6174        copied.pat
+00021b60: 685f 6974 656d 7320 3d20 636f 7079 2e64  h_items = copy.d
+00021b70: 6565 7063 6f70 7928 7365 6c66 2e70 6174  eepcopy(self.pat
+00021b80: 685f 6974 656d 732c 206d 656d 6f29 0a0a  h_items, memo)..
+00021b90: 2020 2020 2020 2020 636f 7069 6564 2e5f          copied._
+00021ba0: 7472 616e 7366 6f72 6d20 3d20 636f 7079  transform = copy
+00021bb0: 2e64 6565 7063 6f70 7928 7365 6c66 2e74  .deepcopy(self.t
+00021bc0: 7261 6e73 666f 726d 2c20 6d65 6d6f 290a  ransform, memo).
+00021bd0: 2020 2020 2020 2020 636f 7069 6564 2e5f          copied._
+00021be0: 636c 6970 7069 6e67 5f70 6174 6820 3d20  clipping_path = 
+00021bf0: 636f 7079 2e64 6565 7063 6f70 7928 7365  copy.deepcopy(se
+00021c00: 6c66 2e63 6c69 7070 696e 675f 7061 7468  lf.clipping_path
+00021c10: 2c20 6d65 6d6f 290a 0a20 2020 2020 2020  , memo)..       
+00021c20: 2072 6574 7572 6e20 636f 7069 6564 0a0a   return copied..
+00021c30: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00021c40: 2020 6465 6620 7472 616e 7366 6f72 6d28    def transform(
+00021c50: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00021c60: 6574 7572 6e20 7365 6c66 2e5f 7472 616e  eturn self._tran
+00021c70: 7366 6f72 6d0a 0a20 2020 2040 7472 616e  sform..    @tran
+00021c80: 7366 6f72 6d2e 7365 7474 6572 0a20 2020  sform.setter.   
+00021c90: 2064 6566 2074 7261 6e73 666f 726d 2873   def transform(s
+00021ca0: 656c 662c 2074 6629 3a0a 2020 2020 2020  elf, tf):.      
+00021cb0: 2020 7365 6c66 2e5f 7472 616e 7366 6f72    self._transfor
+00021cc0: 6d20 3d20 7466 0a0a 2020 2020 4070 726f  m = tf..    @pro
+00021cd0: 7065 7274 790a 2020 2020 6465 6620 636c  perty.    def cl
+00021ce0: 6970 7069 6e67 5f70 6174 6828 7365 6c66  ipping_path(self
+00021cf0: 293a 0a20 2020 2020 2020 2022 2222 5468  ):.        """Th
+00021d00: 6520 6043 6c69 7070 696e 6750 6174 6860  e `ClippingPath`
+00021d10: 2066 6f72 2074 6869 7320 6772 6170 6869   for this graphi
+00021d20: 6373 2063 6f6e 7465 7874 2e22 2222 0a20  cs context.""". 
+00021d30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00021d40: 6c66 2e5f 636c 6970 7069 6e67 5f70 6174  lf._clipping_pat
+00021d50: 680a 0a20 2020 2040 636c 6970 7069 6e67  h..    @clipping
+00021d60: 5f70 6174 682e 7365 7474 6572 0a20 2020  _path.setter.   
+00021d70: 2064 6566 2063 6c69 7070 696e 675f 7061   def clipping_pa
+00021d80: 7468 2873 656c 662c 206e 6577 5f63 6c69  th(self, new_cli
+00021d90: 7061 7468 293a 0a20 2020 2020 2020 2073  path):.        s
+00021da0: 656c 662e 5f63 6c69 7070 696e 675f 7061  elf._clipping_pa
+00021db0: 7468 203d 206e 6577 5f63 6c69 7061 7468  th = new_clipath
+00021dc0: 0a0a 2020 2020 6465 6620 6164 645f 6974  ..    def add_it
+00021dd0: 656d 2873 656c 662c 2069 7465 6d2c 205f  em(self, item, _
+00021de0: 636f 7079 3d54 7275 6529 3a0a 2020 2020  copy=True):.    
+00021df0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00021e00: 4164 6420 6120 7061 7468 2065 6c65 6d65  Add a path eleme
+00021e10: 6e74 2074 6f20 7468 6973 2067 7261 7068  nt to this graph
+00021e20: 6963 7320 636f 6e74 6578 742e 0a0a 2020  ics context...  
+00021e30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00021e40: 2020 2020 2020 2020 6974 656d 3a20 7468          item: th
+00021e50: 6520 7061 7468 2065 6c65 6d65 6e74 2074  e path element t
+00021e60: 6f20 6164 642e 204d 6179 2062 6520 6120  o add. May be a 
+00021e70: 7072 696d 6974 6976 6520 656c 656d 656e  primitive elemen
+00021e80: 7420 6f72 2061 6e6f 7468 6572 0a20 2020  t or another.   
+00021e90: 2020 2020 2020 2020 2020 2020 2060 4772               `Gr
+00021ea0: 6170 6869 6373 436f 6e74 6578 7460 206f  aphicsContext` o
+00021eb0: 7220 6120 6050 6169 6e74 6564 5061 7468  r a `PaintedPath
+00021ec0: 602e 0a20 2020 2020 2020 2020 2020 205f  `..            _
+00021ed0: 636f 7079 2028 626f 6f6c 293a 2069 6620  copy (bool): if 
+00021ee0: 7472 7565 2028 7468 6520 6465 6661 756c  true (the defaul
+00021ef0: 7429 2c20 7468 6520 6974 656d 2077 696c  t), the item wil
+00021f00: 6c20 6265 2063 6f70 6965 6420 6265 666f  l be copied befo
+00021f10: 7265 2062 6569 6e67 0a20 2020 2020 2020  re being.       
+00021f20: 2020 2020 2020 2020 2061 7070 656e 6465           appende
+00021f30: 642e 2054 6869 7320 7072 6576 656e 7473  d. This prevents
+00021f40: 206d 6f64 6966 6963 6174 696f 6e73 2074   modifications t
+00021f50: 6f20 6120 7265 6665 7265 6e63 6564 206f  o a referenced o
+00021f60: 626a 6563 7420 6672 6f6d 0a20 2020 2020  bject from.     
+00021f70: 2020 2020 2020 2020 2020 2022 7265 7472             "retr
+00021f80: 6f61 6374 6976 656c 7922 2061 6c74 6572  oactively" alter
+00021f90: 696e 6720 6974 7320 7374 796c 652f 7368  ing its style/sh
+00021fa0: 6170 6520 616e 6420 7368 6f75 6c64 2062  ape and should b
+00021fb0: 6520 6469 7361 626c 6564 2077 6974 680a  e disabled with.
+00021fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021fd0: 6361 7574 696f 6e2e 0a20 2020 2020 2020  caution..       
+00021fe0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00021ff0: 5f63 6f70 793a 0a20 2020 2020 2020 2020  _copy:.         
+00022000: 2020 2069 7465 6d20 3d20 636f 7079 2e64     item = copy.d
+00022010: 6565 7063 6f70 7928 6974 656d 290a 0a20  eepcopy(item).. 
+00022020: 2020 2020 2020 2073 656c 662e 7061 7468         self.path
+00022030: 5f69 7465 6d73 2e61 7070 656e 6428 6974  _items.append(it
+00022040: 656d 290a 0a20 2020 2064 6566 2072 656d  em)..    def rem
+00022050: 6f76 655f 6c61 7374 5f69 7465 6d28 7365  ove_last_item(se
+00022060: 6c66 293a 0a20 2020 2020 2020 2064 656c  lf):.        del
+00022070: 2073 656c 662e 7061 7468 5f69 7465 6d73   self.path_items
+00022080: 5b2d 315d 0a0a 2020 2020 6465 6620 6d65  [-1]..    def me
+00022090: 7267 6528 7365 6c66 2c20 6f74 6865 725f  rge(self, other_
+000220a0: 636f 6e74 6578 7429 3a0a 2020 2020 2020  context):.      
+000220b0: 2020 2222 2243 6f70 7920 616e 6f74 6865    """Copy anothe
+000220c0: 7220 6047 7261 7068 6963 7343 6f6e 7465  r `GraphicsConte
+000220d0: 7874 6027 7320 7061 7468 2069 7465 6d73  xt`'s path items
+000220e0: 2069 6e74 6f20 7468 6973 206f 6e65 2e22   into this one."
+000220f0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00022100: 7061 7468 5f69 7465 6d73 2e65 7874 656e  path_items.exten
+00022110: 6428 6f74 6865 725f 636f 6e74 6578 742e  d(other_context.
+00022120: 7061 7468 5f69 7465 6d73 290a 0a20 2020  path_items)..   
+00022130: 2040 666f 7263 655f 6e6f 646f 6375 6d65   @force_nodocume
+00022140: 6e74 0a20 2020 2064 6566 2062 7569 6c64  nt.    def build
+00022150: 5f72 656e 6465 725f 6c69 7374 280a 2020  _render_list(.  
+00022160: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00022170: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
+00022180: 2c0a 2020 2020 2020 2020 7374 796c 652c  ,.        style,
+00022190: 0a20 2020 2020 2020 206c 6173 745f 6974  .        last_it
+000221a0: 656d 2c0a 2020 2020 2020 2020 696e 6974  em,.        init
+000221b0: 6961 6c5f 706f 696e 742c 0a20 2020 2020  ial_point,.     
+000221c0: 2020 2064 6562 7567 5f73 7472 6561 6d3d     debug_stream=
+000221d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7066  None,.        pf
+000221e0: 783d 4e6f 6e65 2c0a 2020 2020 2020 2020  x=None,.        
+000221f0: 5f70 7573 685f 7374 6163 6b3d 5472 7565  _push_stack=True
+00022200: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00022210: 2022 2222 0a20 2020 2020 2020 2042 7569   """.        Bui
+00022220: 6c64 2061 206c 6973 7420 636f 6d70 6f73  ld a list compos
+00022230: 6564 206f 6620 616c 6c20 616c 6c20 7468  ed of all all th
+00022240: 6520 696e 6469 7669 6475 616c 2065 6c65  e individual ele
+00022250: 6d65 6e74 7320 7265 6e64 6572 6564 2e0a  ments rendered..
+00022260: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
+00022270: 2075 7365 6420 6279 2060 5061 696e 7465   used by `Painte
+00022280: 6450 6174 6860 2061 6e64 2060 436c 6970  dPath` and `Clip
+00022290: 7069 6e67 5061 7468 6020 746f 2072 6575  pingPath` to reu
+000222a0: 7365 2074 6865 2060 4772 6170 6869 6373  se the `Graphics
+000222b0: 436f 6e74 6578 7460 0a20 2020 2020 2020  Context`.       
+000222c0: 2072 656e 6465 7269 6e67 2070 726f 6365   rendering proce
+000222d0: 7373 2077 6869 6c65 2073 7469 6c6c 2062  ss while still b
+000222e0: 6569 6e67 2061 626c 6520 746f 2069 6e6a  eing able to inj
+000222f0: 6563 7420 736f 6d65 2070 6174 6820 7370  ect some path sp
+00022300: 6563 6966 6963 2069 7465 6d73 0a20 2020  ecific items.   
+00022310: 2020 2020 2028 652e 672e 2074 6865 2070       (e.g. the p
+00022320: 6169 6e74 696e 6720 6469 7265 6374 6976  ainting directiv
+00022330: 6529 2062 6566 6f72 6520 7468 6520 7265  e) before the re
+00022340: 6e64 6572 2069 7320 636f 6c6c 6170 7365  nder is collapse
+00022350: 6420 696e 746f 2061 2073 696e 676c 650a  d into a single.
+00022360: 2020 2020 2020 2020 7374 7269 6e67 2e0a          string..
+00022370: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00022380: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
+00022390: 6567 6973 7472 7920 2847 7261 7068 6963  egistry (Graphic
+000223a0: 7353 7461 7465 4469 6374 5265 6769 7374  sStateDictRegist
+000223b0: 7279 293a 2074 6865 206f 776e 6572 2773  ry): the owner's
+000223c0: 2067 7261 7068 6963 7320 7374 6174 650a   graphics state.
+000223d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000223e0: 6469 6374 696f 6e61 7279 2072 6567 6973  dictionary regis
+000223f0: 7472 792e 0a20 2020 2020 2020 2020 2020  try..           
+00022400: 2073 7479 6c65 2028 4772 6170 6869 6373   style (Graphics
+00022410: 5374 796c 6529 3a20 7468 6520 6375 7272  Style): the curr
+00022420: 656e 7420 7265 736f 6c76 6564 2067 7261  ent resolved gra
+00022430: 7068 6963 7320 7374 796c 650a 2020 2020  phics style.    
+00022440: 2020 2020 2020 2020 6c61 7374 5f69 7465          last_ite
+00022450: 6d3a 2074 6865 2070 7265 7669 6f75 7320  m: the previous 
+00022460: 7061 7468 2065 6c65 6d65 6e74 2e0a 2020  path element..  
+00022470: 2020 2020 2020 2020 2020 696e 6974 6961            initia
+00022480: 6c5f 706f 696e 743a 206c 6173 7420 706f  l_point: last po
+00022490: 7369 7469 6f6e 2073 6574 2062 7920 6120  sition set by a 
+000224a0: 224d 2220 6f72 2022 6d22 2063 6f6d 6d61  "M" or "m" comma
+000224b0: 6e64 0a20 2020 2020 2020 2020 2020 2064  nd.            d
+000224c0: 6562 7567 5f73 7472 6561 6d20 2869 6f2e  ebug_stream (io.
+000224d0: 5465 7874 494f 293a 2074 6865 2073 7472  TextIO): the str
+000224e0: 6561 6d20 746f 2077 6869 6368 2074 6865  eam to which the
+000224f0: 2064 6562 7567 206f 7574 7075 7420 7368   debug output sh
+00022500: 6f75 6c64 2062 650a 2020 2020 2020 2020  ould be.        
+00022510: 2020 2020 2020 2020 7772 6974 7465 6e2e          written.
+00022520: 2054 6869 7320 6973 206e 6f74 2067 7561   This is not gua
+00022530: 7261 6e74 6565 6420 746f 2062 6520 7365  ranteed to be se
+00022540: 656b 6162 6c65 2028 652e 672e 2069 7420  ekable (e.g. it 
+00022550: 6d61 7920 6265 2073 7464 6f75 7420 6f72  may be stdout or
+00022560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022570: 2073 7464 6572 7229 2e0a 2020 2020 2020   stderr)..      
+00022580: 2020 2020 2020 7066 7820 2873 7472 293a        pfx (str):
+00022590: 2074 6865 2063 7572 7265 6e74 2064 6562   the current deb
+000225a0: 7567 206f 7574 7075 7420 7072 6566 6978  ug output prefix
+000225b0: 2073 7472 696e 6720 286f 6e6c 7920 6e65   string (only ne
+000225c0: 6564 6564 2069 6620 656d 6974 7469 6e67  eded if emitting
+000225d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000225e0: 206d 6f72 6520 7468 616e 206f 6e65 206c   more than one l
+000225f0: 696e 6529 2e0a 2020 2020 2020 2020 2020  ine)..          
+00022600: 2020 5f70 7573 685f 7374 6163 6b20 2862    _push_stack (b
+00022610: 6f6f 6c29 3a20 6966 2054 7275 652c 2077  ool): if True, w
+00022620: 7261 7020 7468 6520 7265 7375 6c74 696e  rap the resultin
+00022630: 6720 7265 6e64 6572 206c 6973 7420 696e  g render list in
+00022640: 2061 2070 7573 682f 706f 700a 2020 2020   a push/pop.    
+00022650: 2020 2020 2020 2020 2020 2020 6772 6170              grap
+00022660: 6869 6373 2073 7461 636b 2064 6972 6563  hics stack direc
+00022670: 7469 7665 2070 6169 722e 0a0a 2020 2020  tive pair...    
+00022680: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00022690: 2020 2020 2020 2020 2060 7475 706c 655b           `tuple[
+000226a0: 6c69 7374 5b73 7472 5d2c 206c 6173 745f  list[str], last_
+000226b0: 6974 656d 5d60 2077 6865 7265 2060 6c61  item]` where `la
+000226c0: 7374 5f69 7465 6d60 2069 7320 7468 6520  st_item` is the 
+000226d0: 7061 7374 2070 6174 6820 656c 656d 656e  past path elemen
+000226e0: 7420 696e 0a20 2020 2020 2020 2020 2020  t in.           
+000226f0: 2074 6869 7320 6047 7261 7068 6963 7343   this `GraphicsC
+00022700: 6f6e 7465 7874 600a 2020 2020 2020 2020  ontext`.        
+00022710: 2222 220a 2020 2020 2020 2020 7265 6e64  """.        rend
+00022720: 6572 5f6c 6973 7420 3d20 5b5d 0a0a 2020  er_list = []..  
+00022730: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
+00022740: 7468 5f69 7465 6d73 3a0a 2020 2020 2020  th_items:.      
+00022750: 2020 2020 2020 6966 2064 6562 7567 5f73        if debug_s
+00022760: 7472 6561 6d20 6973 206e 6f74 204e 6f6e  tream is not Non
+00022770: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00022780: 2020 2064 6562 7567 5f73 7472 6561 6d2e     debug_stream.
+00022790: 7772 6974 6528 6622 7b73 656c 662e 5f5f  write(f"{self.__
+000227a0: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+000227b0: 7d22 290a 0a20 2020 2020 2020 2020 2020  }")..           
+000227c0: 206d 6572 6765 645f 7374 796c 6520 3d20   merged_style = 
+000227d0: 7374 796c 652e 5f5f 636c 6173 735f 5f2e  style.__class__.
+000227e0: 6d65 7267 6528 7374 796c 652c 2073 656c  merge(style, sel
+000227f0: 662e 7374 796c 6529 0a0a 2020 2020 2020  f.style)..      
+00022800: 2020 2020 2020 6966 2064 6562 7567 5f73        if debug_s
+00022810: 7472 6561 6d20 6973 206e 6f74 204e 6f6e  tream is not Non
+00022820: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00022830: 2020 2069 6620 7365 6c66 2e5f 7472 616e     if self._tran
+00022840: 7366 6f72 6d3a 0a20 2020 2020 2020 2020  sform:.         
+00022850: 2020 2020 2020 2020 2020 2064 6562 7567             debug
+00022860: 5f73 7472 6561 6d2e 7772 6974 6528 6622  _stream.write(f"
+00022870: 287b 7365 6c66 2e5f 7472 616e 7366 6f72  ({self._transfor
+00022880: 6d7d 2922 290a 0a20 2020 2020 2020 2020  m})")..         
+00022890: 2020 2020 2020 2073 7479 6c65 735f 6462         styles_db
+000228a0: 6720 3d20 5b5d 0a20 2020 2020 2020 2020  g = [].         
+000228b0: 2020 2020 2020 2066 6f72 2061 7474 7220         for attr 
+000228c0: 696e 206d 6572 6765 645f 7374 796c 652e  in merged_style.
+000228d0: 4d45 5247 455f 5052 4f50 4552 5449 4553  MERGE_PROPERTIES
+000228e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000228f0: 2020 2020 2020 7661 6c20 3d20 6765 7461        val = geta
+00022900: 7474 7228 6d65 7267 6564 5f73 7479 6c65  ttr(merged_style
+00022910: 2c20 6174 7472 290a 2020 2020 2020 2020  , attr).        
+00022920: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00022930: 616c 2069 7320 6e6f 7420 6d65 7267 6564  al is not merged
+00022940: 5f73 7479 6c65 2e49 4e48 4552 4954 3a0a  _style.INHERIT:.
+00022950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022960: 2020 2020 2020 2020 6966 2067 6574 6174          if getat
+00022970: 7472 2873 656c 662e 7374 796c 652c 2061  tr(self.style, a
+00022980: 7474 7229 2069 7320 6d65 7267 6564 5f73  ttr) is merged_s
+00022990: 7479 6c65 2e49 4e48 4552 4954 3a0a 2020  tyle.INHERIT:.  
+000229a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229b0: 2020 2020 2020 2020 2020 696e 6820 3d20            inh = 
+000229c0: 2220 2869 6e68 6572 6974 6564 2922 0a20  " (inherited)". 
+000229d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000229f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a00: 2020 2020 2020 2020 2069 6e68 203d 2022           inh = "
+00022a10: 220a 0a20 2020 2020 2020 2020 2020 2020  "..             
+00022a20: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00022a30: 735f 6462 672e 6170 7065 6e64 2866 227b  s_dbg.append(f"{
+00022a40: 6174 7472 7d3a 207b 7661 6c7d 7b69 6e68  attr}: {val}{inh
+00022a50: 7d22 290a 0a20 2020 2020 2020 2020 2020  }")..           
+00022a60: 2020 2020 2069 6620 7374 796c 6573 5f64       if styles_d
+00022a70: 6267 3a0a 2020 2020 2020 2020 2020 2020  bg:.            
+00022a80: 2020 2020 2020 2020 6465 6275 675f 7374          debug_st
+00022a90: 7265 616d 2e77 7269 7465 2822 207b 5c6e  ream.write(" {\n
+00022aa0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00022ab0: 2020 2020 2020 2066 6f72 2073 7479 6c65         for style
+00022ac0: 5f64 6267 5f6c 696e 6520 696e 2073 7479  _dbg_line in sty
+00022ad0: 6c65 735f 6462 673a 0a20 2020 2020 2020  les_dbg:.       
+00022ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022af0: 2064 6562 7567 5f73 7472 6561 6d2e 7772   debug_stream.wr
+00022b00: 6974 6528 7066 7820 2b20 2220 2020 2022  ite(pfx + "    "
+00022b10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00022b20: 2020 2020 2020 2020 2020 6465 6275 675f            debug_
+00022b30: 7374 7265 616d 2e77 7269 7465 2873 7479  stream.write(sty
+00022b40: 6c65 5f64 6267 5f6c 696e 6529 0a20 2020  le_dbg_line).   
+00022b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b60: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+00022b70: 6d2e 7772 6974 6528 225c 6e22 290a 0a20  m.write("\n").. 
+00022b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b90: 2020 2064 6562 7567 5f73 7472 6561 6d2e     debug_stream.
+00022ba0: 7772 6974 6528 7066 7820 2b20 227d e294  write(pfx + "}..
+00022bb0: 905c 6e22 290a 2020 2020 2020 2020 2020  .\n").          
+00022bc0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00022bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022be0: 6465 6275 675f 7374 7265 616d 2e77 7269  debug_stream.wri
+00022bf0: 7465 2822 5c6e 2229 0a0a 2020 2020 2020  te("\n")..      
+00022c00: 2020 2020 2020 4e4f 5f45 4d49 545f 5345        NO_EMIT_SE
+00022c10: 5420 3d20 7b4e 6f6e 652c 206d 6572 6765  T = {None, merge
+00022c20: 645f 7374 796c 652e 494e 4845 5249 547d  d_style.INHERIT}
+00022c30: 0a0a 2020 2020 2020 2020 2020 2020 656d  ..            em
+00022c40: 6974 5f73 7479 6c65 203d 2073 656c 662e  it_style = self.
+00022c50: 7374 796c 650a 2020 2020 2020 2020 2020  style.          
+00022c60: 2020 6966 206d 6572 6765 645f 7374 796c    if merged_styl
+00022c70: 652e 616c 6c6f 775f 7472 616e 7370 6172  e.allow_transpar
+00022c80: 656e 6379 2021 3d20 7365 6c66 2e73 7479  ency != self.sty
+00022c90: 6c65 2e61 6c6c 6f77 5f74 7261 6e73 7061  le.allow_transpa
+00022ca0: 7265 6e63 793a 0a20 2020 2020 2020 2020  rency:.         
+00022cb0: 2020 2020 2020 2065 6d69 745f 7374 796c         emit_styl
+00022cc0: 6520 3d20 636f 7079 2e64 6565 7063 6f70  e = copy.deepcop
+00022cd0: 7928 7365 6c66 2e73 7479 6c65 290a 2020  y(self.style).  
+00022ce0: 2020 2020 2020 2020 2020 2020 2020 656d                em
+00022cf0: 6974 5f73 7479 6c65 2e61 6c6c 6f77 5f74  it_style.allow_t
+00022d00: 7261 6e73 7061 7265 6e63 7920 3d20 6d65  ransparency = me
+00022d10: 7267 6564 5f73 7479 6c65 2e61 6c6c 6f77  rged_style.allow
+00022d20: 5f74 7261 6e73 7061 7265 6e63 790a 0a20  _transparency.. 
+00022d30: 2020 2020 2020 2020 2020 2023 2069 6e20             # in 
+00022d40: 6f72 6465 7220 746f 2064 6563 6f75 706c  order to decoupl
+00022d50: 6520 7468 6520 6461 7368 2070 6174 7465  e the dash patte
+00022d60: 726e 2061 6e64 2074 6865 2064 6173 6820  rn and the dash 
+00022d70: 7068 6173 6520 6174 2074 6865 2041 5049  phase at the API
+00022d80: 206c 6179 6572 2c0a 2020 2020 2020 2020   layer,.        
+00022d90: 2020 2020 2320 7765 2068 6176 6520 746f      # we have to
+00022da0: 2070 6572 666f 726d 2061 6464 6974 696f   perform additio
+00022db0: 6e61 6c20 6c6f 6769 6320 6865 7265 2074  nal logic here t
+00022dc0: 6f20 7265 636f 6d62 696e 6520 7468 656d  o recombine them
+00022dd0: 2e20 5765 2063 616e 2072 656c 790a 2020  . We can rely.  
+00022de0: 2020 2020 2020 2020 2020 2320 6f6e 2074            # on t
+00022df0: 6865 7365 2062 6569 6e67 2073 6572 6961  hese being seria
+00022e00: 6c69 7a61 626c 6520 6265 6361 7573 6520  lizable because 
+00022e10: 7765 2061 6c77 6179 7320 6765 7420 6120  we always get a 
+00022e20: 7361 6e65 2073 7479 6c65 206f 6e20 7468  sane style on th
+00022e30: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
+00022e40: 6472 6177 696e 6720 636f 6e74 6578 742e  drawing context.
+00022e50: 0a20 2020 2020 2020 2020 2020 2064 6173  .            das
+00022e60: 685f 7061 7474 6572 6e20 3d20 6d65 7267  h_pattern = merg
+00022e70: 6564 5f73 7479 6c65 2e73 7472 6f6b 655f  ed_style.stroke_
+00022e80: 6461 7368 5f70 6174 7465 726e 0a20 2020  dash_pattern.   
+00022e90: 2020 2020 2020 2020 2064 6173 685f 7068           dash_ph
+00022ea0: 6173 6520 3d20 6d65 7267 6564 5f73 7479  ase = merged_sty
+00022eb0: 6c65 2e73 7472 6f6b 655f 6461 7368 5f70  le.stroke_dash_p
+00022ec0: 6861 7365 0a20 2020 2020 2020 2020 2020  hase.           
+00022ed0: 2069 6620 2864 6173 685f 7061 7474 6572   if (dash_patter
+00022ee0: 6e20 213d 2073 7479 6c65 2e73 7472 6f6b  n != style.strok
+00022ef0: 655f 6461 7368 5f70 6174 7465 726e 2920  e_dash_pattern) 
+00022f00: 6f72 2028 0a20 2020 2020 2020 2020 2020  or (.           
+00022f10: 2020 2020 2064 6173 685f 7068 6173 6520       dash_phase 
+00022f20: 213d 2073 7479 6c65 2e73 7472 6f6b 655f  != style.stroke_
+00022f30: 6461 7368 5f70 6861 7365 0a20 2020 2020  dash_phase.     
+00022f40: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00022f50: 2020 2020 2020 2020 2020 6966 2065 6d69            if emi
+00022f60: 745f 7374 796c 6520 6973 2073 656c 662e  t_style is self.
+00022f70: 7374 796c 653a 0a20 2020 2020 2020 2020  style:.         
+00022f80: 2020 2020 2020 2020 2020 2065 6d69 745f             emit_
+00022f90: 7374 796c 6520 3d20 636f 7079 2e64 6565  style = copy.dee
+00022fa0: 7063 6f70 7928 656d 6974 5f73 7479 6c65  pcopy(emit_style
+00022fb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00022fc0: 2020 656d 6974 5f73 7479 6c65 2e73 7472    emit_style.str
+00022fd0: 6f6b 655f 6461 7368 5f70 6174 7465 726e  oke_dash_pattern
+00022fe0: 203d 2064 6173 685f 7061 7474 6572 6e0a   = dash_pattern.
+00022ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023000: 656d 6974 5f73 7479 6c65 2e73 7472 6f6b  emit_style.strok
+00023010: 655f 6461 7368 5f70 6861 7365 203d 2064  e_dash_phase = d
+00023020: 6173 685f 7068 6173 650a 0a20 2020 2020  ash_phase..     
+00023030: 2020 2020 2020 2020 2020 2065 6d69 745f             emit_
+00023040: 6461 7368 203d 2028 6461 7368 5f70 6174  dash = (dash_pat
+00023050: 7465 726e 2c20 6461 7368 5f70 6861 7365  tern, dash_phase
+00023060: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00023070: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00023080: 2020 2020 656d 6974 5f64 6173 6820 3d20      emit_dash = 
+00023090: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
+000230a0: 2020 7374 796c 655f 6469 6374 5f6e 616d    style_dict_nam
+000230b0: 6520 3d20 6773 645f 7265 6769 7374 7279  e = gsd_registry
+000230c0: 2e72 6567 6973 7465 725f 7374 796c 6528  .register_style(
+000230d0: 656d 6974 5f73 7479 6c65 290a 0a20 2020  emit_style)..   
+000230e0: 2020 2020 2020 2020 2069 6620 7374 796c           if styl
+000230f0: 655f 6469 6374 5f6e 616d 6520 6973 206e  e_dict_name is n
+00023100: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00023110: 2020 2020 2020 2020 2072 656e 6465 725f           render_
+00023120: 6c69 7374 2e61 7070 656e 6428 6622 7b72  list.append(f"{r
+00023130: 656e 6465 725f 7064 665f 7072 696d 6974  ender_pdf_primit
+00023140: 6976 6528 7374 796c 655f 6469 6374 5f6e  ive(style_dict_n
+00023150: 616d 6529 7d20 6773 2229 0a0a 2020 2020  ame)} gs")..    
+00023160: 2020 2020 2020 2020 2320 7765 2063 616e          # we can
+00023170: 2774 2073 6574 2063 6f6c 6f72 2069 6e20  't set color in 
+00023180: 7468 6520 6772 6170 6869 6373 2073 7461  the graphics sta
+00023190: 7465 2063 6f6e 7465 7874 2064 6963 7469  te context dicti
+000231a0: 6f6e 6172 792c 2073 6f20 7765 2068 6176  onary, so we hav
+000231b0: 6520 746f 0a20 2020 2020 2020 2020 2020  e to.           
+000231c0: 2023 206d 616e 7561 6c6c 7920 696e 6865   # manually inhe
+000231d0: 7269 7420 6974 2061 6e64 2065 6d69 7420  rit it and emit 
+000231e0: 6974 2068 6572 652e 0a20 2020 2020 2020  it here..       
+000231f0: 2020 2020 2066 696c 6c5f 636f 6c6f 7220       fill_color 
+00023200: 3d20 7365 6c66 2e73 7479 6c65 2e66 696c  = self.style.fil
+00023210: 6c5f 636f 6c6f 720a 2020 2020 2020 2020  l_color.        
+00023220: 2020 2020 7374 726f 6b65 5f63 6f6c 6f72      stroke_color
+00023230: 203d 2073 656c 662e 7374 796c 652e 7374   = self.style.st
+00023240: 726f 6b65 5f63 6f6c 6f72 0a0a 2020 2020  roke_color..    
+00023250: 2020 2020 2020 2020 6966 2066 696c 6c5f          if fill_
+00023260: 636f 6c6f 7220 6e6f 7420 696e 204e 4f5f  color not in NO_
+00023270: 454d 4954 5f53 4554 3a0a 2020 2020 2020  EMIT_SET:.      
+00023280: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+00023290: 5f6c 6973 742e 6170 7065 6e64 2866 696c  _list.append(fil
+000232a0: 6c5f 636f 6c6f 722e 7365 7269 616c 697a  l_color.serializ
+000232b0: 6528 292e 6c6f 7765 7228 2929 0a0a 2020  e().lower())..  
+000232c0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+000232d0: 6f6b 655f 636f 6c6f 7220 6e6f 7420 696e  oke_color not in
+000232e0: 204e 4f5f 454d 4954 5f53 4554 3a0a 2020   NO_EMIT_SET:.  
+000232f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00023300: 6e64 6572 5f6c 6973 742e 6170 7065 6e64  nder_list.append
+00023310: 2873 7472 6f6b 655f 636f 6c6f 722e 7365  (stroke_color.se
+00023320: 7269 616c 697a 6528 292e 7570 7065 7228  rialize().upper(
+00023330: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00023340: 6966 2065 6d69 745f 6461 7368 2069 7320  if emit_dash is 
+00023350: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00023360: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+00023370: 5f6c 6973 742e 6170 7065 6e64 280a 2020  _list.append(.  
+00023380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023390: 2020 7265 6e64 6572 5f70 6466 5f70 7269    render_pdf_pri
+000233a0: 6d69 7469 7665 2865 6d69 745f 6461 7368  mitive(emit_dash
+000233b0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+000233c0: 2020 2020 2020 2020 202b 2066 2220 7b6e           + f" {n
+000233d0: 756d 6265 725f 746f 5f73 7472 2865 6d69  umber_to_str(emi
+000233e0: 745f 6461 7368 5b31 5d29 7d20 6422 0a20  t_dash[1])} d". 
+000233f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00023400: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00023410: 2064 6562 7567 5f73 7472 6561 6d3a 0a20   debug_stream:. 
+00023420: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00023430: 6620 7365 6c66 2e63 6c69 7070 696e 675f  f self.clipping_
+00023440: 7061 7468 2069 7320 6e6f 7420 4e6f 6e65  path is not None
+00023450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023460: 2020 2020 2020 6465 6275 675f 7374 7265        debug_stre
+00023470: 616d 2e77 7269 7465 2870 6678 202b 2022  am.write(pfx + "
+00023480: 20e2 949c e294 8020 2229 0a20 2020 2020   ...... ").     
+00023490: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000234a0: 656e 6465 7265 645f 6370 6174 682c 205f  endered_cpath, _
+000234b0: 2c20 5f5f 203d 2073 656c 662e 636c 6970  , __ = self.clip
+000234c0: 7069 6e67 5f70 6174 682e 7265 6e64 6572  ping_path.render
+000234d0: 5f64 6562 7567 280a 2020 2020 2020 2020  _debug(.        
+000234e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234f0: 6773 645f 7265 6769 7374 7279 2c0a 2020  gsd_registry,.  
 00023500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023510: 2020 2020 2b20 6622 207b 6e75 6d62 6572      + f" {number
-00023520: 5f74 6f5f 7374 7228 656d 6974 5f64 6173  _to_str(emit_das
-00023530: 685b 315d 297d 2064 220a 2020 2020 2020  h[1])} d".      
-00023540: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00023550: 2020 2020 2020 2020 2069 6620 6465 6275           if debu
-00023560: 675f 7374 7265 616d 3a0a 2020 2020 2020  g_stream:.      
-00023570: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00023580: 662e 636c 6970 7069 6e67 5f70 6174 6820  f.clipping_path 
-00023590: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000235a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235b0: 2064 6562 7567 5f73 7472 6561 6d2e 7772   debug_stream.wr
-000235c0: 6974 6528 7066 7820 2b20 2220 e294 9ce2  ite(pfx + " ....
-000235d0: 9480 2022 290a 2020 2020 2020 2020 2020  .. ").          
-000235e0: 2020 2020 2020 2020 2020 7265 6e64 6572            render
-000235f0: 6564 5f63 7061 7468 2c20 5f2c 205f 5f20  ed_cpath, _, __ 
-00023600: 3d20 7365 6c66 2e63 6c69 7070 696e 675f  = self.clipping_
-00023610: 7061 7468 2e72 656e 6465 725f 6465 6275  path.render_debu
-00023620: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-00023630: 2020 2020 2020 2020 2020 2067 7364 5f72             gsd_r
-00023640: 6567 6973 7472 792c 0a20 2020 2020 2020  egistry,.       
-00023650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023660: 206d 6572 6765 645f 7374 796c 652c 0a20   merged_style,. 
-00023670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023680: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
-00023690: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000236a0: 2020 2020 2020 2020 2020 696e 6974 6961            initia
-000236b0: 6c5f 706f 696e 742c 0a20 2020 2020 2020  l_point,.       
-000236c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000236d0: 2064 6562 7567 5f73 7472 6561 6d2c 0a20   debug_stream,. 
-000236e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000236f0: 2020 2020 2020 2070 6678 202b 2022 20e2         pfx + " .
-00023700: 9482 2020 222c 0a20 2020 2020 2020 2020  ..  ",.         
-00023710: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00023720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023730: 2069 6620 7265 6e64 6572 6564 5f63 7061   if rendered_cpa
-00023740: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
-00023750: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
-00023760: 6572 5f6c 6973 742e 6170 7065 6e64 2872  er_list.append(r
-00023770: 656e 6465 7265 645f 6370 6174 6829 0a0a  endered_cpath)..
-00023780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023790: 666f 7220 6974 656d 2069 6e20 7365 6c66  for item in self
-000237a0: 2e70 6174 685f 6974 656d 735b 3a2d 315d  .path_items[:-1]
-000237b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000237c0: 2020 2020 2020 6465 6275 675f 7374 7265        debug_stre
-000237d0: 616d 2e77 7269 7465 2870 6678 202b 2022  am.write(pfx + "
-000237e0: 20e2 949c e294 8020 2229 0a20 2020 2020   ...... ").     
-000237f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00023800: 656e 6465 7265 642c 206c 6173 745f 6974  endered, last_it
-00023810: 656d 2c20 696e 6974 6961 6c5f 706f 696e  em, initial_poin
-00023820: 7420 3d20 6974 656d 2e72 656e 6465 725f  t = item.render_
-00023830: 6465 6275 6728 0a20 2020 2020 2020 2020  debug(.         
-00023840: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00023850: 7364 5f72 6567 6973 7472 792c 0a20 2020  sd_registry,.   
-00023860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023870: 2020 2020 206d 6572 6765 645f 7374 796c       merged_styl
-00023880: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00023890: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-000238a0: 6974 656d 2c0a 2020 2020 2020 2020 2020  item,.          
-000238b0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000238c0: 6974 6961 6c5f 706f 696e 742c 0a20 2020  itial_point,.   
-000238d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238e0: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
-000238f0: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
-00023900: 2020 2020 2020 2020 2020 2070 6678 202b             pfx +
-00023910: 2022 20e2 9482 2020 222c 0a20 2020 2020   " ...  ",.     
-00023920: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00023930: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00023940: 2020 2020 2020 6966 2072 656e 6465 7265        if rendere
-00023950: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-00023960: 2020 2020 2020 2020 2020 2072 656e 6465             rende
-00023970: 725f 6c69 7374 2e61 7070 656e 6428 7265  r_list.append(re
-00023980: 6e64 6572 6564 290a 0a20 2020 2020 2020  ndered)..       
-00023990: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
-000239a0: 7472 6561 6d2e 7772 6974 6528 7066 7820  tream.write(pfx 
-000239b0: 2b20 2220 e294 94e2 9480 2022 290a 2020  + " ...... ").  
-000239c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000239d0: 6e64 6572 6564 2c20 6c61 7374 5f69 7465  ndered, last_ite
-000239e0: 6d2c 2069 6e69 7469 616c 5f70 6f69 6e74  m, initial_point
-000239f0: 203d 2073 656c 662e 7061 7468 5f69 7465   = self.path_ite
-00023a00: 6d73 5b2d 315d 2e72 656e 6465 725f 6465  ms[-1].render_de
-00023a10: 6275 6728 0a20 2020 2020 2020 2020 2020  bug(.           
-00023a20: 2020 2020 2020 2020 2067 7364 5f72 6567           gsd_reg
-00023a30: 6973 7472 792c 0a20 2020 2020 2020 2020  istry,.         
-00023a40: 2020 2020 2020 2020 2020 206d 6572 6765             merge
-00023a50: 645f 7374 796c 652c 0a20 2020 2020 2020  d_style,.       
-00023a60: 2020 2020 2020 2020 2020 2020 206c 6173               las
-00023a70: 745f 6974 656d 2c0a 2020 2020 2020 2020  t_item,.        
-00023a80: 2020 2020 2020 2020 2020 2020 696e 6974              init
-00023a90: 6961 6c5f 706f 696e 742c 0a20 2020 2020  ial_point,.     
-00023aa0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00023ab0: 6562 7567 5f73 7472 6561 6d2c 0a20 2020  ebug_stream,.   
-00023ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ad0: 2070 6678 202b 2022 2020 2020 222c 0a20   pfx + "    ",. 
-00023ae0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00023af0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00023b00: 2020 6966 2072 656e 6465 7265 643a 0a20    if rendered:. 
+00023510: 2020 2020 2020 6d65 7267 6564 5f73 7479        merged_sty
+00023520: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+00023530: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+00023540: 5f69 7465 6d2c 0a20 2020 2020 2020 2020  _item,.         
+00023550: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00023560: 6e69 7469 616c 5f70 6f69 6e74 2c0a 2020  nitial_point,.  
+00023570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023580: 2020 2020 2020 6465 6275 675f 7374 7265        debug_stre
+00023590: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
+000235a0: 2020 2020 2020 2020 2020 2020 7066 7820              pfx 
+000235b0: 2b20 2220 e294 8220 2022 2c0a 2020 2020  + " ...  ",.    
+000235c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000235d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000235e0: 2020 2020 2020 6966 2072 656e 6465 7265        if rendere
+000235f0: 645f 6370 6174 683a 0a20 2020 2020 2020  d_cpath:.       
+00023600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023610: 2072 656e 6465 725f 6c69 7374 2e61 7070   render_list.app
+00023620: 656e 6428 7265 6e64 6572 6564 5f63 7061  end(rendered_cpa
+00023630: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
+00023640: 2020 2020 2066 6f72 2069 7465 6d20 696e       for item in
+00023650: 2073 656c 662e 7061 7468 5f69 7465 6d73   self.path_items
+00023660: 5b3a 2d31 5d3a 0a20 2020 2020 2020 2020  [:-1]:.         
+00023670: 2020 2020 2020 2020 2020 2064 6562 7567             debug
+00023680: 5f73 7472 6561 6d2e 7772 6974 6528 7066  _stream.write(pf
+00023690: 7820 2b20 2220 e294 9ce2 9480 2022 290a  x + " ...... ").
+000236a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000236b0: 2020 2020 7265 6e64 6572 6564 2c20 6c61      rendered, la
+000236c0: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
+000236d0: 5f70 6f69 6e74 203d 2069 7465 6d2e 7265  _point = item.re
+000236e0: 6e64 6572 5f64 6562 7567 280a 2020 2020  nder_debug(.    
+000236f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023700: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
+00023710: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023720: 2020 2020 2020 2020 2020 6d65 7267 6564            merged
+00023730: 5f73 7479 6c65 2c0a 2020 2020 2020 2020  _style,.        
+00023740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023750: 6c61 7374 5f69 7465 6d2c 0a20 2020 2020  last_item,.     
+00023760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023770: 2020 2069 6e69 7469 616c 5f70 6f69 6e74     initial_point
+00023780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023790: 2020 2020 2020 2020 2020 6465 6275 675f            debug_
+000237a0: 7374 7265 616d 2c0a 2020 2020 2020 2020  stream,.        
+000237b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237c0: 7066 7820 2b20 2220 e294 8220 2022 2c0a  pfx + " ...  ",.
+000237d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237e0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+000237f0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00023800: 6e64 6572 6564 3a0a 2020 2020 2020 2020  ndered:.        
+00023810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023820: 7265 6e64 6572 5f6c 6973 742e 6170 7065  render_list.appe
+00023830: 6e64 2872 656e 6465 7265 6429 0a0a 2020  nd(rendered)..  
+00023840: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00023850: 6275 675f 7374 7265 616d 2e77 7269 7465  bug_stream.write
+00023860: 2870 6678 202b 2022 20e2 9494 e294 8020  (pfx + " ...... 
+00023870: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00023880: 2020 2072 656e 6465 7265 642c 206c 6173     rendered, las
+00023890: 745f 6974 656d 2c20 696e 6974 6961 6c5f  t_item, initial_
+000238a0: 706f 696e 7420 3d20 7365 6c66 2e70 6174  point = self.pat
+000238b0: 685f 6974 656d 735b 2d31 5d2e 7265 6e64  h_items[-1].rend
+000238c0: 6572 5f64 6562 7567 280a 2020 2020 2020  er_debug(.      
+000238d0: 2020 2020 2020 2020 2020 2020 2020 6773                gs
+000238e0: 645f 7265 6769 7374 7279 2c0a 2020 2020  d_registry,.    
+000238f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023900: 6d65 7267 6564 5f73 7479 6c65 2c0a 2020  merged_style,.  
+00023910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023920: 2020 6c61 7374 5f69 7465 6d2c 0a20 2020    last_item,.   
+00023930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023940: 2069 6e69 7469 616c 5f70 6f69 6e74 2c0a   initial_point,.
+00023950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023960: 2020 2020 6465 6275 675f 7374 7265 616d      debug_stream
+00023970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023980: 2020 2020 2020 7066 7820 2b20 2220 2020        pfx + "   
+00023990: 2022 2c0a 2020 2020 2020 2020 2020 2020   ",.            
+000239a0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+000239b0: 2020 2020 2020 2069 6620 7265 6e64 6572         if render
+000239c0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+000239d0: 2020 2020 2020 2020 7265 6e64 6572 5f6c          render_l
+000239e0: 6973 742e 6170 7065 6e64 2872 656e 6465  ist.append(rende
+000239f0: 7265 6429 0a0a 2020 2020 2020 2020 2020  red)..          
+00023a00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00023a10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00023a20: 636c 6970 7069 6e67 5f70 6174 6820 6973  clipping_path is
+00023a30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00023a40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00023a50: 656e 6465 7265 645f 6370 6174 682c 205f  endered_cpath, _
+00023a60: 2c20 5f5f 203d 2073 656c 662e 636c 6970  , __ = self.clip
+00023a70: 7069 6e67 5f70 6174 682e 7265 6e64 6572  ping_path.render
+00023a80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00023a90: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
+00023aa0: 6769 7374 7279 2c20 6d65 7267 6564 5f73  gistry, merged_s
+00023ab0: 7479 6c65 2c20 6c61 7374 5f69 7465 6d2c  tyle, last_item,
+00023ac0: 2069 6e69 7469 616c 5f70 6f69 6e74 0a20   initial_point. 
+00023ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ae0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00023af0: 2020 2020 2020 2020 2069 6620 7265 6e64           if rend
+00023b00: 6572 6564 5f63 7061 7468 3a0a 2020 2020  ered_cpath:.    
 00023b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023b20: 2020 2072 656e 6465 725f 6c69 7374 2e61     render_list.a
-00023b30: 7070 656e 6428 7265 6e64 6572 6564 290a  ppend(rendered).
-00023b40: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00023b50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00023b60: 2020 2069 6620 7365 6c66 2e63 6c69 7070     if self.clipp
-00023b70: 696e 675f 7061 7468 2069 7320 6e6f 7420  ing_path is not 
-00023b80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00023b90: 2020 2020 2020 2020 2020 7265 6e64 6572            render
-00023ba0: 6564 5f63 7061 7468 2c20 5f2c 205f 5f20  ed_cpath, _, __ 
-00023bb0: 3d20 7365 6c66 2e63 6c69 7070 696e 675f  = self.clipping_
-00023bc0: 7061 7468 2e72 656e 6465 7228 0a20 2020  path.render(.   
-00023bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023be0: 2020 2020 2067 7364 5f72 6567 6973 7472       gsd_registr
-00023bf0: 792c 206d 6572 6765 645f 7374 796c 652c  y, merged_style,
-00023c00: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
-00023c10: 6961 6c5f 706f 696e 740a 2020 2020 2020  ial_point.      
-00023c20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00023c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c40: 2020 2020 6966 2072 656e 6465 7265 645f      if rendered_
-00023c50: 6370 6174 683a 0a20 2020 2020 2020 2020  cpath:.         
-00023c60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00023c70: 656e 6465 725f 6c69 7374 2e61 7070 656e  ender_list.appen
-00023c80: 6428 7265 6e64 6572 6564 5f63 7061 7468  d(rendered_cpath
-00023c90: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00023ca0: 2020 2066 6f72 2069 7465 6d20 696e 2073     for item in s
-00023cb0: 656c 662e 7061 7468 5f69 7465 6d73 3a0a  elf.path_items:.
-00023cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023cd0: 2020 2020 7265 6e64 6572 6564 2c20 6c61      rendered, la
-00023ce0: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
-00023cf0: 5f70 6f69 6e74 203d 2069 7465 6d2e 7265  _point = item.re
-00023d00: 6e64 6572 280a 2020 2020 2020 2020 2020  nder(.          
-00023d10: 2020 2020 2020 2020 2020 2020 2020 6773                gs
-00023d20: 645f 7265 6769 7374 7279 2c20 6d65 7267  d_registry, merg
-00023d30: 6564 5f73 7479 6c65 2c20 6c61 7374 5f69  ed_style, last_i
-00023d40: 7465 6d2c 2069 6e69 7469 616c 5f70 6f69  tem, initial_poi
-00023d50: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00023d60: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00023d70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00023d80: 2072 656e 6465 7265 643a 0a20 2020 2020   rendered:.     
-00023d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023da0: 2020 2072 656e 6465 725f 6c69 7374 2e61     render_list.a
-00023db0: 7070 656e 6428 7265 6e64 6572 6564 290a  ppend(rendered).
-00023dc0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00023dd0: 6e73 6572 7420 7472 616e 7366 6f72 6d20  nsert transform 
-00023de0: 6265 666f 7265 2070 6f69 6e74 730a 2020  before points.  
-00023df0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00023e00: 662e 7472 616e 7366 6f72 6d20 6973 206e  f.transform is n
-00023e10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00023e20: 2020 2020 2020 2020 2072 656e 6465 725f           render_
-00023e30: 6c69 7374 2e69 6e73 6572 7428 302c 2073  list.insert(0, s
-00023e40: 656c 662e 7472 616e 7366 6f72 6d2e 7265  elf.transform.re
-00023e50: 6e64 6572 286c 6173 745f 6974 656d 295b  nder(last_item)[
-00023e60: 305d 290a 0a20 2020 2020 2020 2020 2020  0])..           
-00023e70: 2069 6620 5f70 7573 685f 7374 6163 6b3a   if _push_stack:
-00023e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023e90: 2072 656e 6465 725f 6c69 7374 2e69 6e73   render_list.ins
-00023ea0: 6572 7428 302c 2022 7122 290a 2020 2020  ert(0, "q").    
-00023eb0: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
-00023ec0: 6572 5f6c 6973 742e 6170 7065 6e64 2822  er_list.append("
-00023ed0: 5122 290a 0a20 2020 2020 2020 2072 6574  Q")..        ret
-00023ee0: 7572 6e20 7265 6e64 6572 5f6c 6973 742c  urn render_list,
-00023ef0: 206c 6173 745f 6974 656d 2c20 696e 6974   last_item, init
-00023f00: 6961 6c5f 706f 696e 740a 0a20 2020 2064  ial_point..    d
-00023f10: 6566 2072 656e 6465 7228 0a20 2020 2020  ef render(.     
-00023f20: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00023f30: 2067 7364 5f72 6567 6973 7472 792c 0a20   gsd_registry,. 
-00023f40: 2020 2020 2020 2073 7479 6c65 3a20 4472         style: Dr
-00023f50: 6177 696e 6743 6f6e 7465 7874 2c0a 2020  awingContext,.  
-00023f60: 2020 2020 2020 6c61 7374 5f69 7465 6d2c        last_item,
-00023f70: 0a20 2020 2020 2020 2069 6e69 7469 616c  .        initial
-00023f80: 5f70 6f69 6e74 2c0a 2020 2020 2020 2020  _point,.        
-00023f90: 6465 6275 675f 7374 7265 616d 3d4e 6f6e  debug_stream=Non
-00023fa0: 652c 0a20 2020 2020 2020 2070 6678 3d4e  e,.        pfx=N
-00023fb0: 6f6e 652c 0a20 2020 2020 2020 205f 7075  one,.        _pu
-00023fc0: 7368 5f73 7461 636b 3d54 7275 652c 0a20  sh_stack=True,. 
-00023fd0: 2020 2029 3a0a 2020 2020 2020 2020 7265     ):.        re
-00023fe0: 6e64 6572 5f6c 6973 742c 206c 6173 745f  nder_list, last_
-00023ff0: 6974 656d 2c20 696e 6974 6961 6c5f 706f  item, initial_po
-00024000: 696e 7420 3d20 7365 6c66 2e62 7569 6c64  int = self.build
-00024010: 5f72 656e 6465 725f 6c69 7374 280a 2020  _render_list(.  
-00024020: 2020 2020 2020 2020 2020 6773 645f 7265            gsd_re
-00024030: 6769 7374 7279 2c0a 2020 2020 2020 2020  gistry,.        
-00024040: 2020 2020 7374 796c 652c 0a20 2020 2020      style,.     
-00024050: 2020 2020 2020 206c 6173 745f 6974 656d         last_item
-00024060: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-00024070: 6974 6961 6c5f 706f 696e 742c 0a20 2020  itial_point,.   
-00024080: 2020 2020 2020 2020 2064 6562 7567 5f73           debug_s
-00024090: 7472 6561 6d2c 0a20 2020 2020 2020 2020  tream,.         
-000240a0: 2020 2070 6678 2c0a 2020 2020 2020 2020     pfx,.        
-000240b0: 2020 2020 5f70 7573 685f 7374 6163 6b3d      _push_stack=
-000240c0: 5f70 7573 685f 7374 6163 6b2c 0a20 2020  _push_stack,.   
-000240d0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000240e0: 7265 7475 726e 2022 2022 2e6a 6f69 6e28  return " ".join(
-000240f0: 7265 6e64 6572 5f6c 6973 7429 2c20 6c61  render_list), la
-00024100: 7374 5f69 7465 6d2c 2069 6e69 7469 616c  st_item, initial
-00024110: 5f70 6f69 6e74 0a0a 2020 2020 6465 6620  _point..    def 
-00024120: 7265 6e64 6572 5f64 6562 7567 280a 2020  render_debug(.  
-00024130: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00024140: 2020 2020 6773 645f 7265 6769 7374 7279      gsd_registry
-00024150: 2c0a 2020 2020 2020 2020 7374 796c 653a  ,.        style:
-00024160: 2044 7261 7769 6e67 436f 6e74 6578 742c   DrawingContext,
-00024170: 0a20 2020 2020 2020 206c 6173 745f 6974  .        last_it
-00024180: 656d 2c0a 2020 2020 2020 2020 696e 6974  em,.        init
-00024190: 6961 6c5f 706f 696e 742c 0a20 2020 2020  ial_point,.     
-000241a0: 2020 2064 6562 7567 5f73 7472 6561 6d2c     debug_stream,
-000241b0: 0a20 2020 2020 2020 2070 6678 2c0a 2020  .        pfx,.  
-000241c0: 2020 2020 2020 5f70 7573 685f 7374 6163        _push_stac
-000241d0: 6b3d 5472 7565 2c0a 2020 2020 293a 0a20  k=True,.    ):. 
-000241e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000241f0: 6c66 2e72 656e 6465 7228 0a20 2020 2020  lf.render(.     
-00024200: 2020 2020 2020 2067 7364 5f72 6567 6973         gsd_regis
-00024210: 7472 792c 0a20 2020 2020 2020 2020 2020  try,.           
-00024220: 2073 7479 6c65 2c0a 2020 2020 2020 2020   style,.        
-00024230: 2020 2020 6c61 7374 5f69 7465 6d2c 0a20      last_item,. 
-00024240: 2020 2020 2020 2020 2020 2069 6e69 7469             initi
-00024250: 616c 5f70 6f69 6e74 2c0a 2020 2020 2020  al_point,.      
-00024260: 2020 2020 2020 6465 6275 675f 7374 7265        debug_stre
-00024270: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
-00024280: 7066 782c 0a20 2020 2020 2020 2020 2020  pfx,.           
-00024290: 205f 7075 7368 5f73 7461 636b 3d5f 7075   _push_stack=_pu
-000242a0: 7368 5f73 7461 636b 2c0a 2020 2020 2020  sh_stack,.      
-000242b0: 2020 290a                                  ).
+00023b20: 2020 2020 7265 6e64 6572 5f6c 6973 742e      render_list.
+00023b30: 6170 7065 6e64 2872 656e 6465 7265 645f  append(rendered_
+00023b40: 6370 6174 6829 0a0a 2020 2020 2020 2020  cpath)..        
+00023b50: 2020 2020 2020 2020 666f 7220 6974 656d          for item
+00023b60: 2069 6e20 7365 6c66 2e70 6174 685f 6974   in self.path_it
+00023b70: 656d 733a 0a20 2020 2020 2020 2020 2020  ems:.           
+00023b80: 2020 2020 2020 2020 2072 656e 6465 7265           rendere
+00023b90: 642c 206c 6173 745f 6974 656d 2c20 696e  d, last_item, in
+00023ba0: 6974 6961 6c5f 706f 696e 7420 3d20 6974  itial_point = it
+00023bb0: 656d 2e72 656e 6465 7228 0a20 2020 2020  em.render(.     
+00023bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023bd0: 2020 2067 7364 5f72 6567 6973 7472 792c     gsd_registry,
+00023be0: 206d 6572 6765 645f 7374 796c 652c 206c   merged_style, l
+00023bf0: 6173 745f 6974 656d 2c20 696e 6974 6961  ast_item, initia
+00023c00: 6c5f 706f 696e 740a 2020 2020 2020 2020  l_point.        
+00023c10: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00023c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023c30: 2020 2069 6620 7265 6e64 6572 6564 3a0a     if rendered:.
+00023c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023c50: 2020 2020 2020 2020 7265 6e64 6572 5f6c          render_l
+00023c60: 6973 742e 6170 7065 6e64 2872 656e 6465  ist.append(rende
+00023c70: 7265 6429 0a0a 2020 2020 2020 2020 2020  red)..          
+00023c80: 2020 2320 696e 7365 7274 2074 7261 6e73    # insert trans
+00023c90: 666f 726d 2062 6566 6f72 6520 706f 696e  form before poin
+00023ca0: 7473 0a20 2020 2020 2020 2020 2020 2069  ts.            i
+00023cb0: 6620 7365 6c66 2e74 7261 6e73 666f 726d  f self.transform
+00023cc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00023cd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00023ce0: 6e64 6572 5f6c 6973 742e 696e 7365 7274  nder_list.insert
+00023cf0: 2830 2c20 7365 6c66 2e74 7261 6e73 666f  (0, self.transfo
+00023d00: 726d 2e72 656e 6465 7228 6c61 7374 5f69  rm.render(last_i
+00023d10: 7465 6d29 5b30 5d29 0a0a 2020 2020 2020  tem)[0])..      
+00023d20: 2020 2020 2020 6966 205f 7075 7368 5f73        if _push_s
+00023d30: 7461 636b 3a0a 2020 2020 2020 2020 2020  tack:.          
+00023d40: 2020 2020 2020 7265 6e64 6572 5f6c 6973        render_lis
+00023d50: 742e 696e 7365 7274 2830 2c20 2271 2229  t.insert(0, "q")
+00023d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023d70: 2072 656e 6465 725f 6c69 7374 2e61 7070   render_list.app
+00023d80: 656e 6428 2251 2229 0a0a 2020 2020 2020  end("Q")..      
+00023d90: 2020 7265 7475 726e 2072 656e 6465 725f    return render_
+00023da0: 6c69 7374 2c20 6c61 7374 5f69 7465 6d2c  list, last_item,
+00023db0: 2069 6e69 7469 616c 5f70 6f69 6e74 0a0a   initial_point..
+00023dc0: 2020 2020 6465 6620 7265 6e64 6572 280a      def render(.
+00023dd0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00023de0: 2020 2020 2020 6773 645f 7265 6769 7374        gsd_regist
+00023df0: 7279 2c0a 2020 2020 2020 2020 7374 796c  ry,.        styl
+00023e00: 653a 2044 7261 7769 6e67 436f 6e74 6578  e: DrawingContex
+00023e10: 742c 0a20 2020 2020 2020 206c 6173 745f  t,.        last_
+00023e20: 6974 656d 2c0a 2020 2020 2020 2020 696e  item,.        in
+00023e30: 6974 6961 6c5f 706f 696e 742c 0a20 2020  itial_point,.   
+00023e40: 2020 2020 2064 6562 7567 5f73 7472 6561       debug_strea
+00023e50: 6d3d 4e6f 6e65 2c0a 2020 2020 2020 2020  m=None,.        
+00023e60: 7066 783d 4e6f 6e65 2c0a 2020 2020 2020  pfx=None,.      
+00023e70: 2020 5f70 7573 685f 7374 6163 6b3d 5472    _push_stack=Tr
+00023e80: 7565 2c0a 2020 2020 293a 0a20 2020 2020  ue,.    ):.     
+00023e90: 2020 2072 656e 6465 725f 6c69 7374 2c20     render_list, 
+00023ea0: 6c61 7374 5f69 7465 6d2c 2069 6e69 7469  last_item, initi
+00023eb0: 616c 5f70 6f69 6e74 203d 2073 656c 662e  al_point = self.
+00023ec0: 6275 696c 645f 7265 6e64 6572 5f6c 6973  build_render_lis
+00023ed0: 7428 0a20 2020 2020 2020 2020 2020 2067  t(.            g
+00023ee0: 7364 5f72 6567 6973 7472 792c 0a20 2020  sd_registry,.   
+00023ef0: 2020 2020 2020 2020 2073 7479 6c65 2c0a           style,.
+00023f00: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+00023f10: 5f69 7465 6d2c 0a20 2020 2020 2020 2020  _item,.         
+00023f20: 2020 2069 6e69 7469 616c 5f70 6f69 6e74     initial_point
+00023f30: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00023f40: 6275 675f 7374 7265 616d 2c0a 2020 2020  bug_stream,.    
+00023f50: 2020 2020 2020 2020 7066 782c 0a20 2020          pfx,.   
+00023f60: 2020 2020 2020 2020 205f 7075 7368 5f73           _push_s
+00023f70: 7461 636b 3d5f 7075 7368 5f73 7461 636b  tack=_push_stack
+00023f80: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00023f90: 2020 2020 2072 6574 7572 6e20 2220 222e       return " ".
+00023fa0: 6a6f 696e 2872 656e 6465 725f 6c69 7374  join(render_list
+00023fb0: 292c 206c 6173 745f 6974 656d 2c20 696e  ), last_item, in
+00023fc0: 6974 6961 6c5f 706f 696e 740a 0a20 2020  itial_point..   
+00023fd0: 2064 6566 2072 656e 6465 725f 6465 6275   def render_debu
+00023fe0: 6728 0a20 2020 2020 2020 2073 656c 662c  g(.        self,
+00023ff0: 0a20 2020 2020 2020 2067 7364 5f72 6567  .        gsd_reg
+00024000: 6973 7472 792c 0a20 2020 2020 2020 2073  istry,.        s
+00024010: 7479 6c65 3a20 4472 6177 696e 6743 6f6e  tyle: DrawingCon
+00024020: 7465 7874 2c0a 2020 2020 2020 2020 6c61  text,.        la
+00024030: 7374 5f69 7465 6d2c 0a20 2020 2020 2020  st_item,.       
+00024040: 2069 6e69 7469 616c 5f70 6f69 6e74 2c0a   initial_point,.
+00024050: 2020 2020 2020 2020 6465 6275 675f 7374          debug_st
+00024060: 7265 616d 2c0a 2020 2020 2020 2020 7066  ream,.        pf
+00024070: 782c 0a20 2020 2020 2020 205f 7075 7368  x,.        _push
+00024080: 5f73 7461 636b 3d54 7275 652c 0a20 2020  _stack=True,.   
+00024090: 2029 3a0a 2020 2020 2020 2020 7265 7475   ):.        retu
+000240a0: 726e 2073 656c 662e 7265 6e64 6572 280a  rn self.render(.
+000240b0: 2020 2020 2020 2020 2020 2020 6773 645f              gsd_
+000240c0: 7265 6769 7374 7279 2c0a 2020 2020 2020  registry,.      
+000240d0: 2020 2020 2020 7374 796c 652c 0a20 2020        style,.   
+000240e0: 2020 2020 2020 2020 206c 6173 745f 6974           last_it
+000240f0: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
+00024100: 696e 6974 6961 6c5f 706f 696e 742c 0a20  initial_point,. 
+00024110: 2020 2020 2020 2020 2020 2064 6562 7567             debug
+00024120: 5f73 7472 6561 6d2c 0a20 2020 2020 2020  _stream,.       
+00024130: 2020 2020 2070 6678 2c0a 2020 2020 2020       pfx,.      
+00024140: 2020 2020 2020 5f70 7573 685f 7374 6163        _push_stac
+00024150: 6b3d 5f70 7573 685f 7374 6163 6b2c 0a20  k=_push_stack,. 
+00024160: 2020 2020 2020 2029 0a                          ).
```

### Comparing `fpdf2-2.7.4/fpdf/enums.py` & `fpdf2-2.7.5/fpdf/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,14 +390,26 @@
     TMARGIN = intern("TMARGIN")  # self.t_margin
     "top page margin (start of printable area)"
 
     BMARGIN = intern("BMARGIN")  # self.h - self.b_margin
     "bottom page margin (end of printable area)"
 
 
+class Angle(CoerciveIntEnum):
+    "Direction values used for mirror transformations specifying the angle of mirror line"
+    NORTH = 90
+    EAST = 0
+    SOUTH = 270
+    WEST = 180
+    NORTHEAST = 45
+    SOUTHEAST = 315
+    SOUTHWEST = 225
+    NORTHWEST = 135
+
+
 class PageLayout(CoerciveEnum):
     "Specify the page layout shall be used when the document is opened"
 
     SINGLE_PAGE = Name("SinglePage")
     "Display one page at a time"
 
     ONE_COLUMN = Name("OneColumn")
@@ -829,7 +841,8 @@
 
 class EncryptionMethod(Enum):
     "Algorithm to be used to encrypt the document"
 
     NO_ENCRYPTION = 0
     RC4 = 1
     AES_128 = 2
+    AES_256 = 3
```

### Comparing `fpdf2-2.7.4/fpdf/errors.py` & `fpdf2-2.7.5/fpdf/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 class FPDFPageFormatException(FPDFException):
     """Error is thrown when a bad page format is given"""
 
     def __init__(self, argument, unknown=False, one=False):
         super().__init__()
         if unknown and one:
             raise TypeError(
+                # pylint: disable=implicit-str-concat
                 "FPDF Page Format Exception cannot be both for "
                 "unknown type and for wrong number of arguments"
             )
         self.argument = argument
         self.unknown = unknown
         self.one = one
```

### Comparing `fpdf2-2.7.4/fpdf/fpdf.py` & `fpdf2-2.7.5/fpdf/fpdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 from datetime import datetime, timezone
 from functools import wraps
 from html import unescape
 from math import isclose
 from numbers import Number
 from os.path import splitext
 from pathlib import Path
-from typing import Callable, List, NamedTuple, Optional, Union
+from typing import Callable, NamedTuple, Optional, Union
 
 try:
     from endesive import signer
     from cryptography.hazmat.primitives.serialization import pkcs12
 except ImportError:
     pkcs12, signer = None, None
-from fontTools import ttLib
 
 try:
     from PIL.Image import Image
 except ImportError:
     warnings.warn(
         "Pillow could not be imported - fpdf2 will not be able to add any image"
     )
@@ -44,60 +43,57 @@
 from .actions import URIAction
 from .annotations import (
     AnnotationDict,
     PDFAnnotation,
     PDFEmbeddedFile,
     DEFAULT_ANNOT_FLAGS,
 )
-from .deprecation import WarnOnDeprecatedModuleAttributes
+from .deprecation import get_stack_level, WarnOnDeprecatedModuleAttributes
 from .encryption import StandardSecurityHandler
 from .enums import (
     AccessPermission,
     Align,
+    Angle,
     AnnotationFlag,
     AnnotationName,
     CharVPos,
     Corner,
     EncryptionMethod,
-    FontDescriptorFlags,
     FileAttachmentAnnotationName,
     MethodReturnValue,
     PageLayout,
     PageMode,
     PathPaintRule,
     RenderStyle,
     TextEmphasis,
     TextMarkupType,
     TextMode,
     WrapMode,
     XPos,
     YPos,
 )
 from .errors import FPDFException, FPDFPageFormatException, FPDFUnicodeEncodingException
-from .fonts import CORE_FONTS_CHARWIDTHS, FontFace
+from .fonts import CoreFont, CORE_FONTS, FontFace, TTFFont
 from .graphics_state import GraphicsStateMixin
 from .html import HTML2FPDF
 from .image_parsing import SUPPORTED_IMAGE_FILTERS, get_img_info, load_image
 from .line_break import Fragment, MultiLineBreak, TextLine
 from .linearization import LinearizedOutputProducer
-from .output import OutputProducer, PDFFontDescriptor, PDFPage, ZOOM_CONFIGS
+from .output import OutputProducer, PDFPage, ZOOM_CONFIGS
 from .outline import OutlineSection
 from .recorder import FPDFRecorder
 from .structure_tree import StructureTreeBuilder
 from .sign import Signature
 from .svg import Percent, SVGObject
 from .syntax import DestinationXYZ, PDFDate
 from .table import Table
-from .util import (
-    escape_parens,
-    get_scale_factor,
-)
+from .util import get_scale_factor
 
 # Public global variables:
-FPDF_VERSION = "2.7.4"
+FPDF_VERSION = "2.7.5"
 PAGE_FORMATS = {
     "a3": (841.89, 1190.55),
     "a4": (595.28, 841.89),
     "a5": (420.94, 595.28),
     "letter": (612, 792),
     "legal": (612, 1008),
 }
@@ -169,55 +165,14 @@
 class ToCPlaceholder(NamedTuple):
     render_function: Callable
     start_page: int
     y: int
     pages: int = 1
 
 
-class SubsetMap:
-    """Holds a mapping of used characters and their position in the font's subset
-
-    Characters that must be mapped on their actual unicode must be part of the
-    `identities` list during object instanciation. These non-negative values should
-    only appear once in the list. `pick()` can be used to get the characters
-    corresponding position in the subset. If it's not yet part of the object, a new
-    position is acquired automatically. This implementation always tries to return
-    the lowest possible representation.
-    """
-
-    def __init__(self, identities: List[int]):
-        super().__init__()
-        self._next = 0
-
-        # sort list to ease deletion once _next
-        # becomes higher than first reservation
-        self._reserved = sorted(identities)
-
-        # int(x) to ensure values are integers
-        self._map = {x: int(x) for x in self._reserved}
-
-    def __len__(self):
-        return len(self._map)
-
-    def pick(self, unicode: int):
-        if not unicode in self._map:
-            while self._next in self._reserved:
-                self._next += 1
-                if self._next > self._reserved[0]:
-                    del self._reserved[0]
-
-            self._map[unicode] = self._next
-            self._next += 1
-
-        return self._map.get(unicode)
-
-    def dict(self):
-        return self._map.copy()
-
-
 # Disabling this check due to the "format" parameter below:
 # pylint: disable=redefined-builtin
 def get_page_format(format, k=None):
     """Return page width and height size in points.
 
     Throws FPDFPageFormatException
 
@@ -267,14 +222,15 @@
 class FPDF(GraphicsStateMixin):
     "PDF Generation class"
     MARKDOWN_BOLD_MARKER = "**"
     MARKDOWN_ITALICS_MARKER = "__"
     MARKDOWN_UNDERLINE_MARKER = "--"
     MARKDOWN_LINK_REGEX = re.compile(r"^\[([^][]+)\]\(([^()]+)\)(.*)$")
     MARKDOWN_LINK_COLOR = None
+    MARKDOWN_LINK_UNDERLINE = True
 
     HTML2FPDF_CLASS = HTML2FPDF
 
     def __init__(
         self,
         orientation="portrait",
         unit="mm",
@@ -294,20 +250,20 @@
                 (width, height) expressed in the given unit. Default to "a4".
             font_cache_dir (Path or str): [**DEPRECATED since v2.5.1**] unused
         """
         if font_cache_dir != "DEPRECATED":
             warnings.warn(
                 '"font_cache_dir" parameter is deprecated, unused and will soon be removed',
                 DeprecationWarning,
-                stacklevel=2,
+                stacklevel=get_stack_level(),
             )
         super().__init__()
         self.page = 0  # current page number
         self.pages = {}  # array of PDFPage objects starting at index 1
-        self.fonts = {}  # map font string keys to dicts describing the fonts used
+        self.fonts = {}  # map font string keys to an instance of CoreFont or TTFFont
         self.images = {}  # map image identifiers to dicts describing the raster images
         self.icc_profiles = {}  # map icc profiles (bytes) to their index (number)
         self.links = {}  # array of Destination objects starting at index 1
         self.embedded_files = []  # array of PDFEmbeddedFile
 
         self.in_footer = False  # flag set while rendering footer
         # indicates that we are inside an .unbreakable() code block:
@@ -327,31 +283,14 @@
         self.oversized_images_ratio = 2  # number of pixels per UserSpace point
         self.struct_builder = StructureTreeBuilder()
         self._toc_placeholder = None  # optional ToCPlaceholder instance
         self._outline = []  # list of OutlineSection
         self._sign_key = None
         self.section_title_styles = {}  # level -> TitleStyle
 
-        # Standard fonts
-        self.core_fonts = {
-            "courier": "Courier",
-            "courierB": "Courier-Bold",
-            "courierI": "Courier-Oblique",
-            "courierBI": "Courier-BoldOblique",
-            "helvetica": "Helvetica",
-            "helveticaB": "Helvetica-Bold",
-            "helveticaI": "Helvetica-Oblique",
-            "helveticaBI": "Helvetica-BoldOblique",
-            "times": "Times-Roman",
-            "timesB": "Times-Bold",
-            "timesI": "Times-Italic",
-            "timesBI": "Times-BoldItalic",
-            "symbol": "Symbol",
-            "zapfdingbats": "ZapfDingbats",
-        }
         self.core_fonts_encoding = "latin-1"
         "Font encoding, Latin-1 by default"
         # Replace these fonts with these core fonts
         self.font_aliases = {
             "arial": "helvetica",
             "couriernew": "courier",
             "timesnewroman": "times",
@@ -363,15 +302,17 @@
         # We set their default values here.
         self.font_family = ""  # current font family
         self.font_style = ""  # current font style
         self.font_size_pt = 12  # current font size in points
         self.font_stretching = 100  # current font stretching
         self.char_spacing = 0  # current character spacing
         self.underline = False  # underlining flag
-        self.current_font = {}  # current font
+        self.current_font = (
+            None  # current font, None or an instance of CoreFont or TTFFont
+        )
         self.draw_color = self.DEFAULT_DRAW_COLOR
         self.fill_color = self.DEFAULT_FILL_COLOR
         self.text_color = self.DEFAULT_TEXT_COLOR
         self.page_background = None
         self.dash_pattern = dict(dash=0, gap=0, phase=0)
         self.line_width = 0.567 / self.k  # line width (0.2 mm)
         self.text_mode = TextMode.FILL
@@ -443,28 +384,40 @@
             encrypt_metadata=encrypt_metadata,
         )
 
     def write_html(self, text, *args, **kwargs):
         """
         Parse HTML and convert it to PDF.
         cf. https://pyfpdf.github.io/fpdf2/HTML.html
+
+        Args:
+            text (str): HTML content to render
+            image_map (function): an optional one-argument function that map <img> "src"
+                to new image URLs
+            li_tag_indent (int): numeric indentation of <li> elements
+            dd_tag_indent (int): numeric indentation of <dd> elements
+            table_line_separators (bool): enable horizontal line separators in <table>
+            ul_bullet_char (str): bullet character for <ul> elements
+            heading_sizes (dict): font size per heading level names ("h1", "h2"...)
+            pre_code_font (str): font to use for <pre> & <code> blocks
+            warn_on_tags_not_matching (bool): control warnings production for unmatched HTML tags
         """
         kwargs2 = vars(self)
         # Method arguments must override class & instance attributes:
         kwargs2.update(kwargs)
         html2pdf = self.HTML2FPDF_CLASS(self, *args, **kwargs2)
         text = unescape(text)  # To deal with HTML entities
         html2pdf.feed(text)
 
     def _set_min_pdf_version(self, version):
         self.pdf_version = max(self.pdf_version, version)
 
     @property
     def is_ttf_font(self):
-        return self.current_font.get("type") == "TTF"
+        return self.current_font and self.current_font.type == "TTF"
 
     @property
     def page_mode(self):
         return self._page_mode
 
     @page_mode.setter
     def page_mode(self, page_mode):
@@ -612,14 +565,84 @@
         """
         if zoom in ZOOM_CONFIGS or not isinstance(zoom, str):
             self.zoom_mode = zoom
         elif zoom != "default":
             raise FPDFException(f"Incorrect zoom display mode: {zoom}")
         self.page_layout = LAYOUT_ALIASES.get(layout, layout)
 
+    # Disabling this check - importing outside toplevel to check module is present
+    # pylint: disable=import-outside-toplevel, unused-import
+    def set_text_shaping(
+        self,
+        use_shaping_engine: bool = True,
+        features: dict = None,
+        direction: str = None,
+        script: str = None,
+        language: str = None,
+    ):
+        """
+        Enable or disable text shaping engine when rendering text.
+        If features, direction, script or language are not specified the shaping engine will try
+        to guess the values based on the input text.
+
+        Args:
+            use_shaping_engine: enable or disable the use of the shaping engine to process the text
+            features: a dictionary containing 4 digit OpenType features and whether each feature
+                should be enabled or disabled
+                example: features={"kern": False, "liga": False}
+            direction: the direction the text should be rendered, either "ltr" (left to right)
+                or "rtl" (right to left).
+            script: a valid OpenType script tag like "arab" or "latn"
+            language: a valid OpenType language tag like "eng" or "fra"
+        """
+        if use_shaping_engine:
+            try:
+                import uharfbuzz
+            except ImportError as exc:
+                raise FPDFException(
+                    "The uharfbuzz package could not be imported, but is required for text shaping. Try: pip install uharfbuzz"
+                ) from exc
+        else:
+            self._text_shaping = None
+            return
+        #
+        # Features must be a dictionary contaning opentype features and a boolean flag
+        # stating wether the feature should be enabled or disabled.
+        #
+        # e.g. features={"liga": True, "kern": False}
+        #
+        # https://harfbuzz.github.io/shaping-opentype-features.html
+        #
+
+        if features and not isinstance(features, dict):
+            raise FPDFException(
+                "Features must be a dictionary. See text shaping documentation"
+            )
+        if not features:
+            features = {}
+
+        # Buffer properties (direction, script and language)
+        # if the properties are not provided, Harfbuzz "guessing" logic is used.
+        # https://harfbuzz.github.io/setting-buffer-properties.html
+        # Valid harfbuzz directions are lrt (left to right), rtl (right to left),
+        # ttb (top to bottom) or btt (bottom to top)
+
+        if direction and direction not in ("ltr", "rtl"):
+            raise FPDFException(
+                "FPDF2 only accept ltr (left to right) or rtl (right to left) directions for now."
+            )
+
+        self._text_shaping = {
+            "use_shaping_engine": True,
+            "features": features,
+            "direction": direction,
+            "script": script,
+            "language": language,
+        }
+
     @property
     def page_layout(self):
         return self._page_layout
 
     @page_layout.setter
     def page_layout(self, page_layout):
         self._page_layout = PageLayout.coerce(page_layout) if page_layout else None
@@ -734,18 +757,19 @@
             opt (str): name of the option to set
             value (str) option value
 
         .. deprecated:: 2.4.0
             Simply set the `FPDF.core_fonts_encoding` property as a replacement.
         """
         warnings.warn(
-            "set_doc_option() is deprecated. "
+            # pylint: disable=implicit-str-concat
+            "set_doc_option() is deprecated and will be removed in a future release. "
             "Simply set the `.core_fonts_encoding` property as a replacement.",
             DeprecationWarning,
-            stacklevel=2,
+            stacklevel=get_stack_level(),
         )
         if opt != "core_fonts_encoding":
             raise FPDFException(f'Unknown document option "{opt}"')
         self.core_fonts_encoding = value
 
     def set_image_filter(self, image_filter):
         """
@@ -1235,15 +1259,15 @@
             * `F`: fill
             * `DF` or `FD`: draw and fill
         """
         if fill:
             warnings.warn(
                 '"fill" parameter is deprecated, use style="F" or style="DF" instead',
                 DeprecationWarning,
-                stacklevel=5 if polygon else 3,
+                stacklevel=get_stack_level(),
             )
         if fill and style is None:
             style = RenderStyle.DF
         else:
             style = RenderStyle.coerce(style)
             if fill and style == RenderStyle.D:
                 raise ValueError(
@@ -1288,18 +1312,19 @@
             dash_length (float): Length of the dash
             space_length (float): Length of the space between 2 dashes
 
         .. deprecated:: 2.4.6
             Use `FPDF.set_dash_pattern()` and the normal drawing operations instead.
         """
         warnings.warn(
+            # pylint: disable=implicit-str-concat
             "dashed_line() is deprecated, and will be removed in a future release. "
             "Use set_dash_pattern() and the normal drawing operations instead.",
             DeprecationWarning,
-            stacklevel=3,
+            stacklevel=get_stack_level(),
         )
         self.set_dash_pattern(dash_length, space_length)
         self.line(x1, y1, x2, y2)
         self.set_dash_pattern()
 
     @check_page
     def rect(self, x, y, w, h, style=None, round_corners=False, corner_radius=0):
@@ -1356,20 +1381,20 @@
         point_2 = point_3 = (x + w, y)
         point_4 = point_5 = (x + w, y + h)
         point_6 = point_7 = (x, y + h)
         coor_x = [x, x + w, x, x + w]
         coor_y = [y, y, y + h, y + h]
 
         if round_corners is True:
-            round_corners = [
+            round_corners = (
                 Corner.TOP_RIGHT.value,
                 Corner.TOP_LEFT.value,
                 Corner.BOTTOM_RIGHT.value,
                 Corner.BOTTOM_LEFT.value,
-            ]
+            )
         round_corners = tuple(Corner.coerce(rc) for rc in round_corners)
 
         if Corner.TOP_RIGHT in round_corners:
             self.arc(coor_x[0], coor_y[0], 2 * r, 180, 270, style=style)
             point_1 = (x + r, y)
             point_8 = (x, y + r)
 
@@ -1772,15 +1797,15 @@
                 " this feature is deprecated since v2.5.1 and has been removed in v2.5.3."
             )
 
         if uni != "DEPRECATED":
             warnings.warn(
                 '"uni" parameter is deprecated, unused and will soon be removed',
                 DeprecationWarning,
-                stacklevel=2,
+                stacklevel=get_stack_level(),
             )
 
         style = "".join(sorted(style.upper()))
         if any(letter not in "BI" for letter in style):
             raise ValueError(
                 f"Unknown style provided (only B & I letters are allowed): {style}"
             )
@@ -1796,87 +1821,22 @@
             raise FileNotFoundError(f"TTF Font file not found: {fname}")
 
         if family is None:
             family = font_file_path.stem
 
         fontkey = f"{family.lower()}{style}"
         # Check if font already added or one of the core fonts
-        if fontkey in self.fonts or fontkey in self.core_fonts:
-            warnings.warn(f"Core font or font already added '{fontkey}': doing nothing")
+        if fontkey in self.fonts or fontkey in CORE_FONTS:
+            warnings.warn(
+                f"Core font or font already added '{fontkey}': doing nothing",
+                stacklevel=get_stack_level(),
+            )
             return
-        font = ttLib.TTFont(font_file_path, fontNumber=0, lazy=True)
 
-        scale = 1000 / font["head"].unitsPerEm
-        default_width = round(scale * font["hmtx"].metrics[".notdef"][0])
-
-        try:
-            cap_height = font["OS/2"].sCapHeight
-        except AttributeError:
-            cap_height = font["hhea"].ascent
-
-        # entry for the PDF font descriptor specifying various characteristics of the font
-        flags = FontDescriptorFlags.SYMBOLIC
-        if font["post"].isFixedPitch:
-            flags |= FontDescriptorFlags.FIXED_PITCH
-        if font["post"].italicAngle != 0:
-            flags |= FontDescriptorFlags.ITALIC
-        if font["OS/2"].usWeightClass >= 600:
-            flags |= FontDescriptorFlags.FORCE_BOLD
-
-        desc = PDFFontDescriptor(
-            ascent=round(font["hhea"].ascent * scale),
-            descent=round(font["hhea"].descent * scale),
-            cap_height=round(cap_height * scale),
-            flags=flags,
-            font_b_box=(
-                f"[{font['head'].xMin * scale:.0f} {font['head'].yMin * scale:.0f}"
-                f" {font['head'].xMax * scale:.0f} {font['head'].yMax * scale:.0f}]"
-            ),
-            italic_angle=int(font["post"].italicAngle),
-            stem_v=round(50 + int(pow((font["OS/2"].usWeightClass / 65), 2))),
-            missing_width=default_width,
-        )
-
-        # a map unicode_char -> char_width
-        char_widths = defaultdict(lambda: default_width)
-        font_cmap = tuple(font.getBestCmap().keys())
-        for char in font_cmap:
-            # take glyph associated to char
-            glyph = font.getBestCmap()[char]
-
-            # take width associated to glyph
-            w = font["hmtx"].metrics[glyph][0]
-
-            # probably this check could be deleted
-            if w == 65535:
-                w = 0
-
-            char_widths[char] = round(scale * w + 0.001)  # ROUND_HALF_UP
-
-        # include numbers in the subset! (if alias present)
-        # ensure that alias is mapped 1-by-1 additionally (must be replaceable)
-        sbarr = "\x00 "
-        if self.str_alias_nb_pages:
-            sbarr += "0123456789"
-            sbarr += self.str_alias_nb_pages
-
-        self.fonts[fontkey] = {
-            "i": len(self.fonts) + 1,
-            "type": "TTF",
-            "name": re.sub("[ ()]", "", font["name"].getBestFullName()),
-            "desc": desc,
-            "up": round(font["post"].underlinePosition * scale),
-            "ut": round(font["post"].underlineThickness * scale),
-            "cw": char_widths,
-            "ttffile": font_file_path,
-            "fontkey": fontkey,
-            "emphasis": TextEmphasis.coerce(style),
-            "subset": SubsetMap(map(ord, sbarr)),
-            "cmap": font_cmap,
-        }
+        self.fonts[fontkey] = TTFFont(self, font_file_path, fontkey, style)
 
     def set_font(self, family=None, style="", size=0):
         """
         Sets the font used to print character strings.
         It is mandatory to call this method at least once before printing text.
 
         Default encoding is not specified, but all text writing methods accept only
@@ -1914,21 +1874,23 @@
             style = style.replace("U", "")
         else:
             self.underline = False
 
         if family in self.font_aliases and family + style not in self.fonts:
             warnings.warn(
                 f"Substituting font {family} by core font "
-                f"{self.font_aliases[family]}"
+                f"{self.font_aliases[family]}",
+                stacklevel=get_stack_level(),
             )
             family = self.font_aliases[family]
         elif family in ("symbol", "zapfdingbats") and style:
             warnings.warn(
                 f"Built-in font {family} only has a single 'style' and can't be bold "
-                f"or italic"
+                f"or italic",
+                stacklevel=get_stack_level(),
             )
             style = ""
 
         if size == 0:
             size = self.font_size_pt
 
         # Test if font is already selected
@@ -1938,38 +1900,29 @@
             and isclose(self.font_size_pt, size)
         ):
             return
 
         # Test if used for the first time
         fontkey = family + style
         if fontkey not in self.fonts:
-            if fontkey not in self.core_fonts:
+            if fontkey not in CORE_FONTS:
                 raise FPDFException(
                     f"Undefined font: {fontkey} - "
                     f"Use built-in fonts or FPDF.add_font() beforehand"
                 )
             # If it's one of the core fonts, add it to self.fonts
-            self.fonts[fontkey] = {
-                "i": len(self.fonts) + 1,
-                "type": "core",
-                "name": self.core_fonts[fontkey],
-                "up": -100,
-                "ut": 50,
-                "cw": CORE_FONTS_CHARWIDTHS[fontkey],
-                "fontkey": fontkey,
-                "emphasis": TextEmphasis.coerce(style),
-            }
+            self.fonts[fontkey] = CoreFont(self, fontkey, style)
 
         # Select it
         self.font_family = family
         self.font_style = style
         self.font_size_pt = size
         self.current_font = self.fonts[fontkey]
         if self.page > 0:
-            self._out(f"BT /F{self.current_font['i']} {self.font_size_pt:.2f} Tf ET")
+            self._out(f"BT /F{self.current_font.i} {self.font_size_pt:.2f} Tf ET")
 
     def set_font_size(self, size):
         """
         Configure the font size in points
 
         Args:
             size (float): font size in points
@@ -1978,15 +1931,15 @@
             return
         self.font_size_pt = size
         if self.page > 0:
             if not self.current_font:
                 raise FPDFException(
                     "Cannot set font size: a font must be selected first"
                 )
-            self._out(f"BT /F{self.current_font['i']} {self.font_size_pt:.2f} Tf ET")
+            self._out(f"BT /F{self.current_font.i} {self.font_size_pt:.2f} Tf ET")
 
     def set_char_spacing(self, spacing):
         """
         Sets horizontal character spacing.
         A positive value increases the space between characters, a negative value
         reduces it (which may result in glyph overlap).
         By default, no spacing is set (which is equivalent to a value of 0).
@@ -2426,28 +2379,18 @@
             x (float): abscissa of the origin
             y (float): ordinate of the origin
             txt (str): string to print
         """
         if not self.font_family:
             raise FPDFException("No font set, you need to call set_font() beforehand")
         txt = self.normalize_text(txt)
-        if self.is_ttf_font:
-            txt_mapped = ""
-            for char in txt:
-                uni = ord(char)
-                # Instead of adding the actual character to the stream its code is
-                # mapped to a position in the font's subset
-                txt_mapped += chr(self.current_font["subset"].pick(uni))
-            txt2 = escape_parens(txt_mapped.encode("utf-16-be").decode("latin-1"))
-        else:
-            txt2 = escape_parens(txt)
         sl = [f"BT {x * self.k:.2f} {(self.h - y) * self.k:.2f} Td"]
         if self.text_mode != TextMode.FILL:
             sl.append(f" {self.text_mode} Tr {self.line_width:.2f} w")
-        sl.append(f"({txt2}) Tj ET")
+        sl.append(f"{self.current_font.encode_text(txt)} ET")
         if (self.underline and txt != "") or self._record_text_quad_points:
             w = self.get_string_width(txt, normalized=True, markdown=False)
             if self.underline and txt != "":
                 sl.append(self._do_underline(x, y, w))
             if self._record_text_quad_points:
                 h = self.font_size
                 y -= 0.8 * h  # same coefficient as in _render_styled_text_line()
@@ -2462,18 +2405,20 @@
     @check_page
     def rotate(self, angle, x=None, y=None):
         """
         .. deprecated:: 2.1.0
             Use `FPDF.rotation()` instead.
         """
         warnings.warn(
+            # pylint: disable=implicit-str-concat
             "rotate() can produces malformed PDFs and is deprecated. "
+            "It will be removed in a future release. "
             "Use the rotation() context manager instead.",
             DeprecationWarning,
-            stacklevel=3,
+            stacklevel=get_stack_level(),
         )
         if x is None:
             x = self.x
         if y is None:
             y = self.y
 
         if self._angle != 0:
@@ -2491,15 +2436,15 @@
             )
             self._out(s)
 
     @check_page
     @contextmanager
     def rotation(self, angle, x=None, y=None):
         """
-        This method allows to perform a rotation around a given center.
+        Method to perform a rotation around a given center.
         It must be used as a context-manager using `with`:
 
             with rotation(angle=90, x=x, y=y):
                 pdf.something()
 
         The rotation affects all elements which are printed inside the indented
         context (with the exception of clickable areas).
@@ -2532,15 +2477,15 @@
             )
             yield
 
     @check_page
     @contextmanager
     def skew(self, ax=0, ay=0, x=None, y=None):
         """
-        This method allows to perform a skew transformation originating from a given center.
+        Method to perform a skew transformation originating from a given center.
         It must be used as a context-manager using `with`:
 
             with skew(ax=15, ay=15, x=x, y=y):
                 pdf.something()
 
         The skew transformation affects all elements which are printed inside the indented
         context (with the exception of clickable areas).
@@ -2564,14 +2509,48 @@
                 f"1 {ay:.5f} {ax:.5f} 1 {cx:.2f} {cy:.2f} cm "
                 f"1 0 0 1 -{cx:.2f} -{cy:.2f} cm"
             )
             yield
 
     @check_page
     @contextmanager
+    def mirror(self, origin, angle):
+        """
+        Method to perform a reflection transformation over a given mirror line.
+        It must be used as a context-manager using `with`:
+
+            with mirror(origin=(15,15), angle="SOUTH"):
+                pdf.something()
+
+        The mirror transformation affects all elements which are rendered inside the indented
+        context (with the exception of clickable areas).
+
+        Args:
+            origin (float, Sequence(float, float)): a point on the mirror line
+            angle: (fpdf.enums.Angle): the direction of the mirror line
+        """
+        x, y = origin
+        try:
+            theta = Angle.coerce(angle).value
+        except ValueError:
+            theta = angle
+
+        a = math.cos(math.radians(theta * 2))
+        b = math.sin(math.radians(theta * 2))
+        cx, cy = x * self.k, (self.h - y) * self.k
+
+        with self.local_context():
+            self._out(
+                f"{a:.5f} {b:.5f} {b:.5f} {a*-1:.5f} {cx:.2f} {cy:.2f} cm "
+                f"1 0 0 1 -{cx:.2f} -{cy:.2f} cm"
+            )
+            yield
+
+    @check_page
+    @contextmanager
     def local_context(
         self,
         font_family=None,
         font_style=None,
         font_size=None,
         line_width=None,
         draw_color=None,
@@ -2685,15 +2664,15 @@
         h=None,
         txt="",
         border=0,
         ln="DEPRECATED",
         align=Align.L,
         fill=False,
         link="",
-        center="DEPRECATED",
+        center=False,
         markdown=False,
         new_x=XPos.RIGHT,
         new_y=YPos.TOP,
     ):
         """
         Prints a cell (rectangular area) with optional borders, background color and
         character string. The upper-left corner of the cell corresponds to the current
@@ -2714,50 +2693,47 @@
                 The value can be either a number (`0`: no border ; `1`: frame)
                 or a string containing some or all of the following characters
                 (in any order):
                 `L`: left ; `T`: top ; `R`: right ; `B`: bottom. Default value: 0.
             new_x (fpdf.enums.XPos, str): New current position in x after the call. Default: RIGHT
             new_y (fpdf.enums.YPos, str): New current position in y after the call. Default: TOP
             ln (int): **DEPRECATED since 2.5.1**: Use `new_x` and `new_y` instead.
-            align (fpdf.enums.Align, str): Allows to center or align the text inside the cell.
+            align (fpdf.enums.Align, str): Set text alignment inside the cell.
                 Possible values are: `L` or empty string: left align (default value) ;
-                `C`: center; `X`: center around current x; `R`: right align
+                `C`: center; `X`: center around current x position; `R`: right align
             fill (bool): Indicates if the cell background must be painted (`True`)
                 or transparent (`False`). Default value: False.
             link (str): optional link to add on the cell, internal
                 (identifier returned by `FPDF.add_link`) or external URL.
-            center (bool): **DEPRECATED** since 2.5.1:
-                Use align="C" or align="X" instead.
+            center (bool): center the cell horizontally on the page.
             markdown (bool): enable minimal markdown-like markup to render part
                 of text as bold / italics / underlined. Default to False.
 
         Returns: a boolean indicating if page break was triggered
         """
         if not self.font_family:
             raise FPDFException("No font set, you need to call set_font() beforehand")
         if isinstance(w, str) or isinstance(h, str):
             raise ValueError(
+                # pylint: disable=implicit-str-concat
                 "Parameter 'w' and 'h' must be numbers, not strings."
                 " You can omit them by passing string content with txt="
             )
         if isinstance(border, int) and border not in (0, 1):
             warnings.warn(
-                'Integer values for "border" parameter other than 1 are currently '
-                "ignored"
+                'Integer values for "border" parameter other than 1 are currently ignored',
+                stacklevel=get_stack_level(),
             )
             border = 1
         new_x = XPos.coerce(new_x)
         new_y = YPos.coerce(new_y)
-        if center == "DEPRECATED":
-            center = False
-        else:
-            warnings.warn(
-                'The parameter "center" is deprecated. Use align="C" or align="X" instead.',
-                DeprecationWarning,
-                stacklevel=3,
+        align = Align.coerce(align)
+        if align == Align.J:
+            raise ValueError(
+                "cell() only produces one text line, justified alignment is not possible"
             )
         if ln != "DEPRECATED":
             # For backwards compatibility, if "ln" is used we overwrite "new_[xy]".
             if ln == 0:
                 new_x = XPos.RIGHT
                 new_y = YPos.TOP
             elif ln == 1:
@@ -2773,20 +2749,15 @@
                 )
             warnings.warn(
                 (
                     'The parameter "ln" is deprecated.'
                     f" Instead of ln={ln} use new_x=XPos.{new_x.name}, new_y=YPos.{new_y.name}."
                 ),
                 DeprecationWarning,
-                stacklevel=3,
-            )
-        align = Align.coerce(align)
-        if align == Align.J:
-            raise ValueError(
-                "cell() only produces one text line, justified alignment is not possible"
+                stacklevel=get_stack_level(),
             )
         # Font styles preloading must be performed before any call to FPDF.get_string_width:
         txt = self.normalize_text(txt)
         styled_txt_frags = self._preload_font_styles(txt, markdown)
         return self._render_styled_text_line(
             TextLine(
                 styled_txt_frags,
@@ -2848,26 +2819,22 @@
                 `L` or empty string: left align (default value);
                 `C`: center; `X`: center around current x; `R`: right align;
                 `J`: justify (if more than one word)
             fill (bool): Indicates if the cell background must be painted (`True`)
                 or transparent (`False`). Default value: False.
             link (str): optional link to add on the cell, internal
                 (identifier returned by `FPDF.add_link`) or external URL.
-            center (bool): **DEPRECATED since 2.5.1**: Use `align="C"` instead.
-            markdown (bool): enable minimal markdown-like markup to render part
-                of text as bold / italics / underlined. Default to False.
+            center (bool): center the cell horizontally on the page.
 
         Returns: a boolean indicating if page break was triggered
         """
-        if not self.font_family:
-            raise FPDFException("No font set, you need to call set_font() beforehand")
         if isinstance(border, int) and border not in (0, 1):
             warnings.warn(
-                'Integer values for "border" parameter other than 1 are currently '
-                "ignored"
+                'Integer values for "border" parameter other than 1 are currently ignored',
+                stacklevel=get_stack_level(),
             )
             border = 1
         styled_txt_width = text_line.text_width
         if not styled_txt_width:
             for i, frag in enumerate(text_line.fragments):
                 unscaled_width = frag.get_width(initial_cs=i != 0)
                 styled_txt_width += unscaled_width
@@ -2876,25 +2843,27 @@
             w = self.w - self.r_margin - self.x
         elif w is None:
             if not text_line.fragments:
                 raise ValueError(
                     "A 'text_line' parameter with fragments must be provided if 'w' is None"
                 )
             w = styled_txt_width + self.c_margin + self.c_margin
+        if center:
+            self.x = (
+                self.w / 2 if align == Align.X else self.l_margin + (self.epw - w) / 2
+            )
+        if align == Align.X:
+            self.x -= w / 2
         max_font_size = 0  # how much height we need to accomodate.
         # currently all font sizes within a line are vertically aligned on the baseline.
         for frag in text_line.fragments:
             if frag.font_size > max_font_size:
                 max_font_size = frag.font_size
         if h is None:
             h = max_font_size
-        if align == Align.X:
-            self.x -= w / 2
-        if center:
-            self.x = self.l_margin + (self.epw - w) / 2
         page_break_triggered = self._perform_page_break_if_need_be(h)
         sl = []
         k = self.k
         # pylint: disable=invalid-unary-operand-type
         # "h" can't actually be None
         if fill:
             op = "B" if border == 1 else "f"
@@ -2936,14 +2905,15 @@
         if self._record_text_quad_points:
             self._add_quad_points(self.x, self.y, w, h)
 
         s_start = self.x
         s_width, underlines = 0, []
         # We try to avoid modifying global settings for temporary changes.
         current_ws = frag_ws = 0.0
+        current_lift = 0.0
         current_char_vpos = CharVPos.LINE
         current_font = self.current_font
         current_text_mode = self.text_mode
         current_font_stretching = self.font_stretching
         current_char_spacing = self.char_spacing
         if text_line.fragments:
             if align == Align.R:
@@ -2953,25 +2923,22 @@
             else:
                 dx = self.c_margin
             s_start += dx
 
             if self.fill_color != self.text_color:
                 sl.append(self.text_color.serialize().lower())
 
-            # do this once in advance
-            u_space = escape_parens(" ".encode("utf-16-be").decode("latin-1"))
             word_spacing = 0
             if text_line.justify:
                 # Don't rely on align==Align.J here.
                 # If a line gets broken by an explicit '\n', then MultiLineBreak
                 # will set its justify to False (end of paragraph).
                 word_spacing = (
                     w - self.c_margin - self.c_margin - styled_txt_width
                 ) / text_line.number_of_spaces
-
             sl.append(
                 f"BT {(self.x + dx) * k:.2f} "
                 f"{(self.h - self.y - 0.5 * h - 0.3 * max_font_size) * k:.2f} Td"
             )
             for i, frag in enumerate(text_line.fragments):
                 if word_spacing and frag.font_stretching != 100:
                     # Space character is already stretched, extra spacing is absolute.
@@ -2984,77 +2951,60 @@
                 if current_char_spacing != frag.char_spacing:
                     current_char_spacing = frag.char_spacing
                     sl.append(f"{frag.char_spacing:.2f} Tc")
                 if current_font != frag.font or current_char_vpos != frag.char_vpos:
                     if current_char_vpos != frag.char_vpos:
                         current_char_vpos = frag.char_vpos
                     current_font = frag.font
-                    sl.append(f"/F{frag.font['i']} {frag.font_size_pt:.2f} Tf")
+                    sl.append(f"/F{frag.font.i} {frag.font_size_pt:.2f} Tf")
                 lift = frag.lift
-                if lift != 0.0:
+                if lift != current_lift:
+                    # Use text rise operator:
                     sl.append(f"{lift:.2f} Ts")
+                    current_lift = lift
                 if (
                     frag.text_mode != TextMode.FILL
                     or frag.text_mode != current_text_mode
                 ):
                     current_text_mode = frag.text_mode
                     sl.append(f"{frag.text_mode} Tr {frag.line_width:.2f} w")
 
-                if frag.is_ttf_font:
-                    mapped_text = ""
-                    for char in frag.string:
-                        uni = ord(char)
-                        mapped_text += chr(frag.font["subset"].pick(uni))
-                    if word_spacing:
-                        # "Tw" only has an effect on the ASCII space character and ignores
-                        # space characters from unicode (TTF) fonts. As a workaround,
-                        # we do word spacing using an adjustment before each space.
-                        # Determine the index of the space character (" ") in the current
-                        # subset and split words whenever this mapping code is found
-                        words = mapped_text.split(
-                            chr(frag.font["subset"].pick(ord(" ")))
-                        )
-                        words_strl = []
-                        for i, word in enumerate(words):
-                            word = escape_parens(
-                                word.encode("utf-16-be").decode("latin-1")
-                            )
-                            if i == 0:
-                                words_strl.append(f"({word})")
-                            else:
-                                adj = -(frag_ws * frag.k) * 1000 / frag.font_size_pt
-                                words_strl.append(f"{adj:.3f}({u_space}{word})")
-                        escaped_text = " ".join(words_strl)
-                        sl.append(f"[{escaped_text}] TJ")
-                    else:
-                        escaped_text = escape_parens(
-                            mapped_text.encode("utf-16-be").decode("latin-1")
-                        )
-                        sl.append(f"({escaped_text}) Tj")
-                else:  # core fonts
-                    if frag_ws != current_ws:
-                        sl.append(f"{frag_ws * frag.k:.3f} Tw")
-                        current_ws = frag_ws
-                    escaped_text = escape_parens(frag.string)
-                    sl.append(f"({escaped_text}) Tj")
+                r_text = frag.render_pdf_text(
+                    frag_ws,
+                    current_ws,
+                    word_spacing,
+                    self.x + dx + s_width,
+                    self.y + (0.5 * h + 0.3 * max_font_size),
+                    self.h,
+                )
+                if r_text:
+                    sl.append(r_text)
+
                 frag_width = frag.get_width(
                     initial_cs=i != 0
                 ) + word_spacing * frag.characters.count(" ")
                 if frag.underline:
                     underlines.append(
-                        (self.x + dx + s_width, frag_width, frag.font, frag.font_size)
+                        (
+                            self.x + dx + s_width,
+                            frag_width,
+                            frag.font,
+                            frag.font_size,
+                        )
                     )
-                if frag.url:
+                if frag.link:
                     self.link(
                         x=self.x + dx + s_width,
                         y=self.y + (0.5 * h) - (0.5 * frag.font_size),
                         w=frag_width,
                         h=frag.font_size,
-                        link=frag.url,
+                        link=frag.link,
                     )
+                if not frag.is_ttf_font:
+                    current_ws = frag_ws
                 s_width += frag_width
 
             sl.append("ET")
 
             for start_x, ul_w, ul_font, ul_font_size in underlines:
                 sl.append(
                     self._do_underline(
@@ -3075,14 +3025,15 @@
 
         if sl:
             # If any PDF settings have been left modified, wrap the line
             # in a local context.
             # pylint: disable=too-many-boolean-expressions
             if (
                 current_ws != 0.0
+                or current_lift != 0.0
                 or current_char_vpos != CharVPos.LINE
                 or current_font != self.current_font
                 or current_text_mode != self.text_mode
                 or self.fill_color != self.text_color
                 or current_font_stretching != self.font_stretching
                 or current_char_spacing != self.char_spacing
             ):
@@ -3170,15 +3121,15 @@
 
     def _parse_chars(self, txt):
         "Check if the font has all the necessary glyphs. If a glyph from a fallback font is used, break into fragments"
         fragments = []
         txt_frag = []
         if not self.is_ttf_font or not self._fallback_font_ids:
             return tuple([Fragment(txt, self._get_current_graphics_state(), self.k)])
-        font_glyphs = self.current_font["cmap"]
+        font_glyphs = self.current_font.cmap
         for char in txt:
             if char == "\n" or ord(char) in font_glyphs:
                 txt_frag.append(char)
             else:
                 if txt_frag:
                     fragments.append(
                         Fragment(txt_frag, self._get_current_graphics_state(), self.k)
@@ -3207,24 +3158,20 @@
         This method can be overriden to provide more control than the `select_mode` parameter
         of `FPDF.set_fallback_fonts()` provides.
         """
         emphasis = TextEmphasis.coerce(style)
         fonts_with_char = [
             font_id
             for font_id in self._fallback_font_ids
-            if ord(char) in self.fonts[font_id]["cmap"]
+            if ord(char) in self.fonts[font_id].cmap
         ]
         if not fonts_with_char:
             return None
         font_with_matching_emphasis = next(
-            (
-                font
-                for font in fonts_with_char
-                if self.fonts[font]["emphasis"] == emphasis
-            ),
+            (font for font in fonts_with_char if self.fonts[font].emphasis == emphasis),
             None,
         )
         if font_with_matching_emphasis:
             return font_with_matching_emphasis
         if self._fallback_font_exact_match:
             return None
         return fonts_with_char[0]
@@ -3246,15 +3193,15 @@
             gstate["underline"] = in_underline
             nonlocal txt_frag
             fragment = Fragment(txt_frag, gstate, self.k)
             txt_frag = []
             return fragment
 
         if self.is_ttf_font:
-            font_glyphs = self.current_font["cmap"]
+            font_glyphs = self.current_font.cmap
         else:
             font_glyphs = []
 
         while txt:
             is_marker = txt[:2] in (
                 self.MARKDOWN_BOLD_MARKER,
                 self.MARKDOWN_ITALICS_MARKER,
@@ -3275,22 +3222,27 @@
                     in_italics = not in_italics
                 if txt[:2] == self.MARKDOWN_UNDERLINE_MARKER:
                     in_underline = not in_underline
                 txt = txt[2:]
                 continue
             is_link = self.MARKDOWN_LINK_REGEX.match(txt)
             if is_link:
-                link_text, link_url, txt = is_link.groups()
+                link_text, link_dest, txt = is_link.groups()
                 if txt_frag:
                     yield frag()
                 gstate = self._get_current_graphics_state()
-                gstate["underline"] = True
+                gstate["underline"] = self.MARKDOWN_LINK_UNDERLINE
                 if self.MARKDOWN_LINK_COLOR:
                     gstate["text_color"] = self.MARKDOWN_LINK_COLOR
-                yield Fragment(list(link_text), gstate, self.k, url=link_url)
+                try:
+                    page = int(link_dest)
+                    link_dest = self.add_link(page=page)
+                except ValueError:
+                    pass
+                yield Fragment(list(link_text), gstate, self.k, link=link_dest)
                 continue
             if self.is_ttf_font and txt[0] != "\n" and not ord(txt[0]) in font_glyphs:
                 style = ("B" if in_bold else "") + ("I" if in_italics else "")
                 fallback_font = self.get_fallback_font(txt[0], style)
                 if fallback_font:
                     if txt_frag:
                         yield frag()
@@ -3376,14 +3328,15 @@
         markdown=False,
         print_sh=False,
         new_x=XPos.RIGHT,
         new_y=YPos.NEXT,
         wrapmode: WrapMode = WrapMode.WORD,
         dry_run=False,
         output=MethodReturnValue.PAGE_BREAK,
+        center=False,
     ):
         """
         This method allows printing text with line breaks. They can be automatic
         (breaking at the most recent space or soft-hyphen character) as soon as the text
         reaches the right border of the cell, or explicit (via the `\\n` character).
         As many cells as necessary are stacked, one below the other.
         Text can be aligned, centered or justified. The cell block can be framed and
@@ -3394,18 +3347,18 @@
             h (float): cell height. Default value: None, meaning to use the current font size.
             txt (str): string to print.
             border: Indicates if borders must be drawn around the cell.
                 The value can be either a number (`0`: no border ; `1`: frame)
                 or a string containing some or all of the following characters
                 (in any order):
                 `L`: left ; `T`: top ; `R`: right ; `B`: bottom. Default value: 0.
-            align (fpdf.enums.Align, str): Allows to center or align the text.
+            align (fpdf.enums.Align, str): Set text alignment inside the cell.
                 Possible values are:
                 `J`: justify (default value); `L` or empty string: left align;
-                `C`: center; `X`: center around current x; `R`: right align
+                `C`: center; `X`: center around current x position; `R`: right align
             fill (bool): Indicates if the cell background must be painted (`True`)
                 or transparent (`False`). Default value: False.
             split_only (bool): **DEPRECATED since 2.7.4**:
                 Use `dry_run=True` and `output=("LINES",)` instead.
             link (str): optional link to add on the cell, internal
                 (identifier returned by `add_link`) or external URL.
             new_x (fpdf.enums.XPos, str): New current position in x after the call. Default: RIGHT
@@ -3418,28 +3371,28 @@
                 character, instead of a line breaking opportunity. Default value: False
             wrapmode (fpdf.enums.WrapMode): "WORD" for word based line wrapping (default),
                 "CHAR" for character based line wrapping.
             dry_run (bool): if `True`, does not output anything in the document.
                 Can be useful when combined with `output`.
             output (fpdf.enums.MethodReturnValue): defines what this method returns.
                 If several enum values are joined, the result will be a tuple.
+            center (bool): center the cell horizontally on the page.
 
         Using `new_x=XPos.RIGHT, new_y=XPos.TOP, maximum height=pdf.font_size` is
         useful to build tables with multiline text in cells.
 
         Returns: a single value or a tuple, depending on the `output` parameter value
         """
         if split_only:
             warnings.warn(
-                (
-                    'The parameter "split_only" is deprecated.'
-                    ' Use instead dry_run=True and output="LINES".'
-                ),
+                # pylint: disable=implicit-str-concat
+                'The parameter "split_only" is deprecated.'
+                ' Use instead dry_run=True and output="LINES".',
                 DeprecationWarning,
-                stacklevel=3,
+                stacklevel=get_stack_level(),
             )
         if dry_run or split_only:
             with self._disable_writing():
                 return self.multi_cell(
                     w=w,
                     h=h,
                     txt=txt,
@@ -3453,18 +3406,22 @@
                     print_sh=print_sh,
                     new_x=new_x,
                     new_y=new_y,
                     wrapmode=wrapmode,
                     dry_run=False,
                     split_only=False,
                     output=MethodReturnValue.LINES if split_only else output,
+                    center=center,
                 )
+        if not self.font_family:
+            raise FPDFException("No font set, you need to call set_font() beforehand")
         wrapmode = WrapMode.coerce(wrapmode)
         if isinstance(w, str) or isinstance(h, str):
             raise ValueError(
+                # pylint: disable=implicit-str-concat
                 "Parameter 'w' and 'h' must be numbers, not strings."
                 " You can omit them by passing string content with txt="
             )
         new_x = XPos.coerce(new_x)
         new_y = YPos.coerce(new_y)
         if ln != "DEPRECATED":
             # For backwards compatibility, if "ln" is used we overwrite "new_[xy]".
@@ -3487,25 +3444,29 @@
                 )
             warnings.warn(
                 (
                     'The parameter "ln" is deprecated.'
                     f" Instead of ln={ln} use new_x=XPos.{new_x.name}, new_y=YPos.{new_y.name}."
                 ),
                 DeprecationWarning,
-                stacklevel=3,
+                stacklevel=get_stack_level(),
             )
         align = Align.coerce(align)
 
         page_break_triggered = False
 
         if h is None:
             h = self.font_size
         # If width is 0, set width to available width between margins
         if w == 0:
             w = self.w - self.r_margin - self.x
+        if center:
+            self.x = (
+                self.w / 2 if align == Align.X else self.l_margin + (self.epw - w) / 2
+            )
         maximum_allowed_width = w - 2 * self.c_margin
 
         # Calculate text length
         txt = self.normalize_text(txt)
         normalized_string = txt.replace("\r", "")
         styled_text_fragments = self._preload_font_styles(normalized_string, markdown)
 
@@ -3521,18 +3482,18 @@
         text_lines = []
         multi_line_break = MultiLineBreak(
             styled_text_fragments,
             justify=(align == Align.J),
             print_sh=print_sh,
             wrapmode=wrapmode,
         )
-        text_line = multi_line_break.get_line_of_given_width(maximum_allowed_width)
-        while (text_line) is not None:
-            text_lines.append(text_line)
-            text_line = multi_line_break.get_line_of_given_width(maximum_allowed_width)
+        txt_line = multi_line_break.get_line_of_given_width(maximum_allowed_width)
+        while (txt_line) is not None:
+            text_lines.append(txt_line)
+            txt_line = multi_line_break.get_line_of_given_width(maximum_allowed_width)
 
         if not text_lines:  # ensure we display at least one cell - cf. issue #349
             text_lines = [
                 TextLine(
                     "",
                     text_width=0,
                     number_of_spaces=0,
@@ -3604,15 +3565,16 @@
             )
             page_break_triggered = page_break_triggered or new_page
         if new_page and new_y == YPos.TOP:
             # When a page jump is performed and the requested y is TOP,
             # pretend we started at the top of the text block on the new page.
             # cf. test_multi_cell_table_with_automatic_page_break
             prev_y = self.y
-        if text_line.trailing_nl and new_y in (YPos.LAST, YPos.NEXT):
+        # pylint: disable=undefined-loop-variable
+        if text_line and text_line.trailing_nl and new_y in (YPos.LAST, YPos.NEXT):
             # The line renderer can't handle trailing newlines in the text.
             self.ln()
 
         if new_y == YPos.TOP:  # We may have jumped a few lines -> reset
             self.y = prev_y
 
         if markdown:
@@ -3666,14 +3628,15 @@
                 "CHAR" for character based line wrapping.
         """
         wrapmode = WrapMode.coerce(wrapmode)
         if not self.font_family:
             raise FPDFException("No font set, you need to call set_font() beforehand")
         if isinstance(h, str):
             raise ValueError(
+                # pylint: disable=implicit-str-concat
                 "Parameter 'h' must be a number, not a string."
                 " You can omit it by passing string content with txt="
             )
         if h is None:
             h = self.font_size
 
         page_break_triggered = False
@@ -3684,23 +3647,23 @@
         multi_line_break = MultiLineBreak(
             styled_text_fragments,
             print_sh=print_sh,
             wrapmode=wrapmode,
         )
         # first line from current x position to right margin
         first_width = self.w - self.x - self.r_margin
-        text_line = multi_line_break.get_line_of_given_width(
-            first_width - 2 * self.c_margin, wordsplit=False
+        txt_line = multi_line_break.get_line_of_given_width(
+            first_width - 2 * self.c_margin,
         )
         # remaining lines fill between margins
         full_width = self.w - self.l_margin - self.r_margin
         fit_width = full_width - 2 * self.c_margin
-        while (text_line) is not None:
-            text_lines.append(text_line)
-            text_line = multi_line_break.get_line_of_given_width(fit_width)
+        while txt_line is not None:
+            text_lines.append(txt_line)
+            txt_line = multi_line_break.get_line_of_given_width(fit_width)
         if not text_lines:
             return False
 
         for text_line_index, text_line in enumerate(text_lines):
             if text_line_index == 0:
                 line_width = first_width
             else:
@@ -3714,14 +3677,15 @@
                 new_x=XPos.WCONT,
                 new_y=YPos.TOP,
                 align=Align.L,
                 fill=False,
                 link=link,
             )
             page_break_triggered = page_break_triggered or new_page
+        # pylint: disable=undefined-loop-variable
         if text_line.trailing_nl:
             # The line renderer can't handle trailing newlines in the text.
             self.ln()
         return page_break_triggered
 
     @check_page
     def image(
@@ -3785,15 +3749,15 @@
 
         Returns: an instance of `ImageInfo`
         """
         if type:
             warnings.warn(
                 '"type" parameter is deprecated, unused and will soon be removed',
                 DeprecationWarning,
-                stacklevel=3,
+                stacklevel=get_stack_level(),
             )
         if str(name).endswith(".svg"):
             # Insert it as a PDF path:
             img = load_image(str(name))
             return self._vector_image(img, x, y, w, h, link, title, alt_text)
         if isinstance(name, bytes) and _is_svg(name.strip()):
             return self._vector_image(
@@ -3927,15 +3891,16 @@
         link="",
         title=None,
         alt_text=None,
     ):
         svg = SVGObject(img.getvalue())
         if not svg.viewbox and svg.width and svg.height:
             warnings.warn(
-                '<svg> has no "viewBox", using its "width" & "height" as default "viewBox"'
+                '<svg> has no "viewBox", using its "width" & "height" as default "viewBox"',
+                stacklevel=get_stack_level(),
             )
             svg.viewbox = 0, 0, svg.width, svg.height
         if w == 0 and h == 0:
             if svg.width and svg.height:
                 w = (
                     svg.width * self.epw / 100
                     if isinstance(svg.width, Percent)
@@ -4004,14 +3969,15 @@
         ):
             factor = (
                 min(info["w"] / width_in_pt, info["h"] / height_in_pt)
                 / self.oversized_images_ratio
             )
             if self.oversized_images.lower().startswith("warn"):
                 LOGGER.warning(
+                    # pylint: disable=implicit-str-concat
                     "OVERSIZED: Image %s with size %.1fx%.1fpx is rendered at size %.1fx%.1fpt."
                     " Set pdf.oversized_images = 'DOWNSCALE' to reduce embedded image size by a factor %.1f",
                     name,
                     info["w"],
                     info["h"],
                     width_in_pt,
                     height_in_pt,
@@ -4305,15 +4271,15 @@
             error_msg = f"The rendering function passed to FPDF.insert_toc_placeholder triggered too {too} page breaks: "
             error_msg += f"ToC ended on page {self.page} while it was expected to span exactly {tocp.pages} pages"
             raise FPDFException(error_msg)
         self.page, self.y = prev_page, prev_y
         del self.footer
         del self.header
 
-    def file_id(self):
+    def file_id(self):  # pylint: disable=no-self-use
         """
         This method can be overridden in inherited classes
         in order to define a custom file identifier.
         Its output must have the format "<hex_string1><hex_string2>".
         If this method returns a falsy value (None, empty string),
         no /ID will be inserted in the generated PDF document.
         """
@@ -4335,16 +4301,16 @@
         hash_hex = id_hash.hexdigest().upper()
         return f"<{hash_hex}><{hash_hex}>"
 
     def _do_underline(self, x, y, w, current_font=None):
         "Draw an horizontal line starting from (x, y) with a length equal to 'w'"
         if current_font is None:
             current_font = self.current_font
-        up = current_font["up"]
-        ut = current_font["ut"]
+        up = current_font.up
+        ut = current_font.ut
         return (
             f"{x * self.k:.2f} "
             f"{(self.h - y + up / 1000 * self.font_size) * self.k:.2f} "
             f"{w * self.k:.2f} {-ut / 1000 * self.font_size_pt:.2f} re f"
         )
 
     def _out(self, s):
@@ -4418,16 +4384,18 @@
 
     @check_page
     def code39(self, txt, x, y, w=1.5, h=5):
         """Barcode 3of9"""
         dim = {"w": w, "n": w / 3}
         if not txt.startswith("*") or not txt.endswith("*"):
             warnings.warn(
+                # pylint: disable=implicit-str-concat
                 "Code 39 input must start and end with a '*' character to be valid."
-                " This method does not insert it automatically."
+                " This method does not insert it automatically.",
+                stacklevel=get_stack_level(),
             )
         chars = {
             "0": "nnnwwnwnn",
             "1": "wnnwnnnnw",
             "2": "nnwwnnnnw",
             "3": "wnwwnnnnn",
             "4": "nnnwwnnnw",
@@ -4756,20 +4724,24 @@
             borders_layout (str, fpdf.enums.TableBordersLayout): optional, default to ALL. Control what cell borders are drawn
             cell_fill_color (int, tuple, fpdf.drawing.DeviceGray, fpdf.drawing.DeviceRGB): optional.
                 Defines the cells background color
             cell_fill_mode (str, fpdf.enums.TableCellFillMode): optional. Defines which cells are filled with color in the background
             col_widths (int, tuple): optional. Sets column width. Can be a single number or a sequence of numbers
             first_row_as_headings (bool): optional, default to True. If False, the first row of the table
                 is not styled differently from the others
+            gutter_height (float): optional vertical space between rows
+            gutter_width (float): optional horizontal space between columns
             headings_style (fpdf.fonts.FontFace): optional, default to bold.
                 Defines the visual style of the top headings row: size, color, emphasis...
             line_height (number): optional. Defines how much vertical space a line of text will occupy
             markdown (bool): optional, default to False. Enable markdown interpretation of cells textual content
             text_align (str, fpdf.enums.Align): optional, default to JUSTIFY. Control text alignment inside cells.
             width (number): optional. Sets the table width
+            wrapmode (fpdf.enums.WrapMode): "WORD" for word based line wrapping (default),
+                "CHAR" for character based line wrapping.
         """
         table = Table(self, *args, **kwargs)
         yield table
         table.render()
 
     def output(
         self, name="", dest="", linearize=False, output_producer_class=OutputProducer
@@ -4787,15 +4759,15 @@
             dest (str): [**DEPRECATED since 2.3.0**] unused, will be removed in a later version
             output_producer_class (class): use a custom class for PDF file generation
         """
         if dest:
             warnings.warn(
                 '"dest" parameter is deprecated, unused and will soon be removed',
                 DeprecationWarning,
-                stacklevel=2,
+                stacklevel=get_stack_level(),
             )
         # Finish document if necessary:
         if not self.buffer:
             if self.page == 0:
                 self.add_page()
             # Generating final page footer:
             self.in_footer = True
```

### Comparing `fpdf2-2.7.4/fpdf/graphics_state.py` & `fpdf2-2.7.5/fpdf/graphics_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                 sup_scale=0.7,
                 nom_scale=0.75,
                 denom_scale=0.75,
                 sub_lift=-0.15,
                 sup_lift=0.4,
                 nom_lift=0.2,
                 denom_lift=0.0,
+                _text_shaping=None,
             ),
         ]
         super().__init__(*args, **kwargs)
 
     def _push_local_stack(self):
         self.__statestack.append(self.__statestack[-1].copy())
 
@@ -309,14 +310,22 @@
     def denom_lift(self, v):
         """
         Set lift factor for denominator text.
         ([docs](../TextStyling.html#subscript-superscript-and-fractional-numbers))
         """
         self.__statestack[-1]["denom_lift"] = float(v)
 
+    @property
+    def _text_shaping(self):
+        return self.__statestack[-1]["_text_shaping"]
+
+    @_text_shaping.setter
+    def _text_shaping(self, v):
+        self.__statestack[-1]["_text_shaping"] = v
+
     def font_face(self):
         """
         Return a `fpdf.fonts.FontFace` instance
         representing a subset of properties of this GraphicsState.
         """
         return FontFace(
             family=self.font_family,
```

### Comparing `fpdf2-2.7.4/fpdf/html.py` & `fpdf2-2.7.5/fpdf/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 "HTML renderer"
 
 import logging, warnings
 from html.parser import HTMLParser
 
 from .enums import TextEmphasis, XPos, YPos
 from .errors import FPDFException
+from .deprecation import get_stack_level
 from .fonts import FontFace
 from .table import Table, TableBordersLayout
 
 import re
 
 LOGGER = logging.getLogger(__name__)
 BULLET_WIN1252 = "\x95"  # BULLET character in Windows-1252 encoding
@@ -215,14 +216,17 @@
             pdf (FPDF): an instance of `fpdf.FPDF`
             image_map (function): an optional one-argument function that map <img> "src"
                 to new image URLs
             li_tag_indent (int): numeric indentation of <li> elements
             dd_tag_indent (int): numeric indentation of <dd> elements
             table_line_separators (bool): enable horizontal line separators in <table>
             ul_bullet_char (str): bullet character for <ul> elements
+            heading_sizes (dict): font size per heading level names ("h1", "h2"...)
+            pre_code_font (str): font to use for <pre> & <code> blocks
+            warn_on_tags_not_matching (bool): control warnings production for unmatched HTML tags
         """
         super().__init__()
         self.pdf = pdf
         self.image_map = image_map or (lambda src: src)
         self.li_tag_indent = li_tag_indent
         self.dd_tag_indent = dd_tag_indent
         self.ul_bullet_char = ul_bullet_char
@@ -234,15 +238,15 @@
         self.align = ""
         self.page_links = {}
         self.font_stack = []
         self.indent = 0
         self.bullet = []
         self.font_size = pdf.font_size_pt
         self.set_font(pdf.font_family or "times", size=self.font_size)
-        self.font_color = 0, 0, 0  # initialize font color, r,g,b format
+        self.font_color = tuple((255 * v for v in pdf.text_color.colors))
         self.heading_level = None
         self.heading_sizes = dict(**DEFAULT_HEADING_SIZES)
         self.heading_above = 0.2  # extra space above heading, relative to font size
         self.heading_below = 0.2  # extra space below heading, relative to font size
         if heading_sizes:
             self.heading_sizes.update(heading_sizes)
         self.pre_code_font = pre_code_font
@@ -258,14 +262,25 @@
 
     def handle_data(self, data):
         trailing_space_flag = TRAILING_SPACE.search(data)
         if self.td_th is not None:
             data = data.strip()
             if not data:
                 return
+            if "inserted" in self.td_th:
+                td_th_tag = self.td_th["tag"]
+                raise NotImplementedError(
+                    f"Unsupported nested HTML tags inside <{td_th_tag}> element: <{self._tags_stack[-1]}>"
+                )
+                # We could potentially support nested <b> / <em> / <font> tags
+                # by building a list of Fragment instances from the HTML cell content
+                # and then passing those fragments to Row.cell().
+                # However there should be an incoming refactoring of this code
+                # dedicated to text layout, and we should probably wait for that
+                # before supporting this feature.
             align = self.td_th.get("align", self.tr.get("align"))
             if align:
                 align = align.upper()
             bgcolor = color_as_decimal(
                 self.td_th.get("bgcolor", self.tr.get("bgcolor", None))
             )
             colspan = int(self.td_th.get("colspan", "1"))
@@ -450,14 +465,15 @@
                 raise FPDFException("Invalid HTML: <tr> used outside any <table>")
             self.tr = {k.lower(): v for k, v in attrs.items()}
             self.table_row = self.table.row()
         if tag in ("td", "th"):
             if not self.table_row:
                 raise FPDFException(f"Invalid HTML: <{tag}> used outside any <tr>")
             self.td_th = {k.lower(): v for k, v in attrs.items()}
+            self.td_th["tag"] = tag
             if tag == "th":
                 self.td_th["align"] = "CENTER"
                 self.td_th["b"] = True
             elif len(self.table.rows) == 1 and not self.table_row.cells:
                 # => we are in the 1st <tr>, and the 1st cell is a <td>
                 # => we do not treat the first row as a header
                 # pylint: disable=protected-access
@@ -650,14 +666,15 @@
         # Put a hyperlink
         self.set_text_color(0, 0, 255)
         self.set_style("u", True)
         self.pdf.write(self.h, txt, self.href)
         self.set_style("u", False)
         self.set_text_color(*self.font_color)
 
+    # pylint: disable=no-self-use
     def render_toc(self, pdf, outline):
         "This method can be overriden by subclasses to customize the Table of Contents style."
         pdf.ln()
         for section in outline:
             link = pdf.add_link(page=section.page_number)
             text = f'{" " * section.level * 2} {section.name}'
             text += f' {"." * (60 - section.level*2 - len(section.name))} {section.page_number}'
@@ -702,12 +719,13 @@
     return trimmed_str
 
 
 class HTMLMixin:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         warnings.warn(
+            # pylint: disable=implicit-str-concat
             "The HTMLMixin class is deprecated. "
             "Simply use the FPDF class as a replacement.",
             DeprecationWarning,
-            stacklevel=2,
+            stacklevel=get_stack_level(),
         )
```

### Comparing `fpdf2-2.7.4/fpdf/image_parsing.py` & `fpdf2-2.7.5/fpdf/image_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     from PIL import ImageCms
 
     try:
         from PIL.Image import Resampling
 
         RESAMPLE = Resampling.LANCZOS
     except ImportError:  # For Pillow < 9.1.0
+        # pylint: disable=no-member
         RESAMPLE = Image.ANTIALIAS
 except ImportError:
     Image = None
 
 from .errors import FPDFException
 
 
@@ -69,15 +70,15 @@
         filename = str(filename)
     # by default loading from network is allowed for all images
     if filename.startswith(("http://", "https://")):
         # disabling bandit & semgrep rules as permitted schemes are whitelisted:
         # nosemgrep: python.lang.security.audit.dynamic-urllib-use-detected.dynamic-urllib-use-detected
         with urlopen(filename) as url_file:  # nosec B310
             return BytesIO(url_file.read())
-    elif filename.startswith("data"):
+    elif filename.startswith("data:"):
         return _decode_base64_image(filename)
     with open(filename, "rb") as local_file:
         return BytesIO(local_file.read())
 
 
 def _decode_base64_image(base64Image):
     "Decode the base 64 image string into an io byte stream."
```

### Comparing `fpdf2-2.7.4/fpdf/line_break.py` & `fpdf2-2.7.5/fpdf/line_break.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 Routines for organizing lines and larger blocks of text, with manual and
 automatic line wrapping.
 
 The contents of this file are internal to fpdf, and not part of the public API.
 They may change at any time without prior warning or any deprecation period.
 """
 
-from typing import NamedTuple, Any, Union, Sequence
+from typing import NamedTuple, Any, Optional, Union, Sequence
 
 from .enums import CharVPos, WrapMode
 from .errors import FPDFException
+from .fonts import CoreFont, TTFFont
+from .util import escape_parens
 
 SOFT_HYPHEN = "\u00ad"
 HYPHEN = "\u002d"
 SPACE = " "
 NEWLINE = "\n"
 
 
@@ -23,44 +25,42 @@
     """
 
     def __init__(
         self,
         characters: Union[list, str],
         graphics_state: dict,
         k: float,
-        url: str = None,
+        link: Optional[Union[int, str]] = None,
     ):
         if isinstance(characters, str):
             self.characters = list(characters)
         else:
             self.characters = characters
         self.graphics_state = graphics_state
         self.k = k
-        self.url = url
+        self.link = link
 
     def __repr__(self):
-        gstate = self.graphics_state.copy()
-        if "current_font" in gstate:
-            del gstate["current_font"]  # TMI
         return (
             f"Fragment(characters={self.characters},"
-            f" graphics_state={gstate}, k={self.k}, url={self.url})"
+            f" graphics_state={self.graphics_state},"
+            f" k={self.k}, link={self.link})"
         )
 
     @property
-    def font(self):
+    def font(self) -> Union[CoreFont, TTFFont]:
         return self.graphics_state["current_font"]
 
     @font.setter
     def font(self, v):
         self.graphics_state["current_font"] = v
 
     @property
     def is_ttf_font(self):
-        return self.font.get("type") == "TTF"
+        return self.font and self.font.type == "TTF"
 
     @property
     def font_style(self):
         return self.graphics_state["font_style"]
 
     @property
     def font_family(self):
@@ -132,74 +132,187 @@
         elif vpos == CharVPos.DENOM:
             lift = self.graphics_state["denom_lift"]
         else:
             lift = 0.0
         return lift * self.graphics_state["font_size_pt"]
 
     @property
+    def _text_shaping(self):
+        return self.graphics_state["_text_shaping"]
+
+    @property
     def string(self):
         return "".join(self.characters)
 
     def trim(self, index: int):
         self.characters = self.characters[:index]
 
     def __eq__(self, other: Any):
         return (
             self.characters == other.characters
             and self.graphics_state == other.graphics_state
             and self.k == other.k
         )
 
+    def __hash__(self):
+        return hash((self.characters, self.graphics_state, self.k))
+
     def get_width(
         self,
         start: int = 0,
         end: int = None,
         chars: str = None,
         initial_cs: bool = True,
     ):
         """
-        Return the witdth of the string with the given font/size/style/etc.
+        Return the width of the string with the given font/size/style/etc.
 
         Args:
             start (int): Index of the start character. Default start of fragment.
             end (int): Index of the end character. Default end of fragment.
             chars (str): Specific text to get the width for (not necessarily the
                 same as the contents of the fragment). If given, this takes
                 precedence over the start/end arguments.
         """
 
         if chars is None:
             chars = self.characters[start:end]
-        if self.is_ttf_font:
-            w = sum(self.font["cw"][ord(c)] for c in chars)
-        else:
-            w = sum(self.font["cw"][c] for c in chars)
+        (char_len, w) = self.font.get_text_width(
+            chars, self.font_size_pt, self._text_shaping
+        )
         char_spacing = self.char_spacing
         if self.font_stretching != 100:
             w *= self.font_stretching * 0.01
             char_spacing *= self.font_stretching * 0.01
-        w *= self.font_size_pt * 0.001
         if self.char_spacing != 0:
             # initial_cs must be False if the fragment is located at the
             # beginning of a text object, because the first char won't get spaced.
             if initial_cs:
-                w += char_spacing * len(chars)
+                w += char_spacing * char_len
             else:
-                w += char_spacing * (len(chars) - 1)
+                w += char_spacing * (char_len - 1)
         return w / self.k
 
     def get_character_width(self, character: str, print_sh=False, initial_cs=True):
         """
         Return the width of a single character out of the stored text.
         """
         if character == SOFT_HYPHEN and not print_sh:
             # HYPHEN is inserted instead of SOFT_HYPHEN
             character = HYPHEN
         return self.get_width(chars=character, initial_cs=initial_cs)
 
+    def render_pdf_text(self, frag_ws, current_ws, word_spacing, adjust_x, adjust_y, h):
+        if self.is_ttf_font:
+            if self._text_shaping:
+                return self.render_with_text_shaping(
+                    adjust_x, adjust_y, h, word_spacing, self._text_shaping
+                )
+            return self.render_pdf_text_ttf(frag_ws, word_spacing)
+        return self.render_pdf_text_core(frag_ws, current_ws)
+
+    def render_pdf_text_ttf(self, frag_ws, word_spacing):
+        ret = ""
+        mapped_text = ""
+        for char in self.string:
+            mapped_char = self.font.subset.pick(ord(char))
+            if mapped_char:
+                mapped_text += chr(mapped_char)
+        if word_spacing:
+            # do this once in advance
+            u_space = escape_parens(" ".encode("utf-16-be").decode("latin-1"))
+
+            # According to the PDF reference, word spacing shall be applied to every
+            # occurrence of the single-byte character code 32 in a string when using
+            # a simple font or a composite font that defines code 32 as a single-byte code.
+            # It shall not apply to occurrences of the byte value 32 in multiple-byte codes.
+            # FPDF uses 2 bytes per character (UTF-16-BE encoding) so the "Tw" operator doesn't work
+            # As a workaround, we do word spacing using an adjustment before each space.
+            # Determine the index of the space character (" ") in the current
+            # subset and split words whenever this mapping code is found
+            #
+            words = mapped_text.split(chr(self.font.subset.pick(ord(" "))))
+            words_strl = []
+            for word_i, word in enumerate(words):
+                # pylint: disable=redefined-loop-name
+                word = escape_parens(word.encode("utf-16-be").decode("latin-1"))
+                if word_i == 0:
+                    words_strl.append(f"({word})")
+                else:
+                    adj = -(frag_ws * self.k) * 1000 / self.font_size_pt
+                    words_strl.append(f"{adj:.3f}({u_space}{word})")
+            escaped_text = " ".join(words_strl)
+            ret += f"[{escaped_text}] TJ"
+        else:
+            escaped_text = escape_parens(
+                mapped_text.encode("utf-16-be").decode("latin-1")
+            )
+            ret += f"({escaped_text}) Tj"
+        return ret
+
+    def render_with_text_shaping(
+        self, pos_x, pos_y, h, word_spacing, text_shaping_parms
+    ):
+        ret = ""
+        text = ""
+        space_mapped_code = self.font.subset.pick(ord(" "))
+
+        def adjust_pos(pos):
+            return (
+                pos
+                * self.font.scale
+                * self.font_size_pt
+                * (self.font_stretching / 100)
+                / 1000
+                / self.k
+            )
+
+        char_spacing = self.char_spacing * (self.font_stretching / 100) / self.k
+        for ti in self.font.shape_text(
+            self.string, self.font_size_pt, text_shaping_parms
+        ):
+            if ti["mapped_char"] is None:  # Missing glyph
+                continue
+            char = chr(ti["mapped_char"]).encode("utf-16-be").decode("latin-1")
+            if ti["x_offset"] != 0 or ti["y_offset"] != 0:
+                if text:
+                    ret += f"({text}) Tj "
+                    text = ""
+                offsetx = pos_x + adjust_pos(ti["x_offset"])
+                offsety = pos_y - adjust_pos(ti["y_offset"])
+                ret += (
+                    f"1 0 0 1 {(offsetx) * self.k:.2f} {(h - offsety) * self.k:.2f} Tm "
+                )
+            text += char
+            pos_x += adjust_pos(ti["x_advance"]) + char_spacing
+            pos_y += adjust_pos(ti["y_advance"])
+            if word_spacing and ti["mapped_char"] == space_mapped_code:
+                pos_x += word_spacing
+
+            # if only moving "x" we don't need to move the text matrix
+            if ti["force_positioning"] or (
+                word_spacing and ti["mapped_char"] == space_mapped_code
+            ):
+                if text:
+                    ret += f"({text}) Tj "
+                    text = ""
+                ret += f"1 0 0 1 {(pos_x) * self.k:.2f} {(h - pos_y) * self.k:.2f} Tm "
+
+        if text:
+            ret += f"({text}) Tj"
+        return ret
+
+    def render_pdf_text_core(self, frag_ws, current_ws):
+        ret = ""
+        if frag_ws != current_ws:
+            ret += f"{frag_ws * self.k:.3f} Tw "
+        escaped_text = escape_parens(self.string)
+        ret += f"({escaped_text}) Tj"
+        return ret
+
 
 class TextLine(NamedTuple):
     fragments: tuple
     text_width: float
     number_of_spaces: int
     justify: bool
     trailing_nl: bool = False
@@ -387,26 +500,22 @@
         self.print_sh = print_sh
         self.wrapmode = wrapmode
         self.fragment_index = 0
         self.character_index = 0
         self.idx_last_forced_break = None
 
     # pylint: disable=too-many-return-statements
-    def get_line_of_given_width(self, maximum_width: float, wordsplit: bool = True):
+    def get_line_of_given_width(self, maximum_width: float):
         first_char = True  # "Tw" ignores the first character in a text object.
         idx_last_forced_break = self.idx_last_forced_break
         self.idx_last_forced_break = None
 
         if self.fragment_index == len(self.styled_text_fragments):
             return None
 
-        last_fragment_index = self.fragment_index
-        last_character_index = self.character_index
-        line_full = False
-
         current_line = CurrentLine(print_sh=self.print_sh)
         while self.fragment_index < len(self.styled_text_fragments):
             current_fragment = self.styled_text_fragments[self.fragment_index]
 
             if self.character_index >= len(current_fragment.characters):
                 self.character_index = 0
                 self.fragment_index += 1
@@ -435,38 +544,29 @@
                     (
                         self.fragment_index,
                         self.character_index,
                         line,
                     ) = current_line.automatic_break(self.justify)
                     self.character_index += 1
                     return line
-                if not wordsplit:
-                    line_full = True
-                    break
                 if idx_last_forced_break == self.character_index:
                     raise FPDFException(
                         "Not enough horizontal space to render a single character"
                     )
                 self.idx_last_forced_break = self.character_index
                 return current_line.manual_break()
 
             current_line.add_character(
                 character,
                 character_width,
                 current_fragment.graphics_state,
                 current_fragment.k,
                 self.fragment_index,
                 self.character_index,
-                current_fragment.url,
+                current_fragment.link,
             )
 
             self.character_index += 1
 
-        if line_full and not wordsplit:
-            # roll back and return empty line to trigger continuation
-            # on the next line.
-            self.fragment_index = last_fragment_index
-            self.character_index = last_character_index
-            return CurrentLine().manual_break(self.justify)
         if current_line.width:
             return current_line.manual_break()
         return None
```

### Comparing `fpdf2-2.7.4/fpdf/linearization.py` & `fpdf2-2.7.5/fpdf/linearization.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/outline.py` & `fpdf2-2.7.5/fpdf/outline.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/output.py` & `fpdf2-2.7.5/fpdf/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     PDFObject,
     PDFString,
 )
 from .syntax import create_dictionary_string as pdf_dict
 from .syntax import create_list_string as pdf_list
 from .syntax import iobj_ref as pdf_ref
 
-from fontTools import ttLib
 from fontTools import subset as ftsubset
 
 try:
     from endesive import signer
 except ImportError:
     signer = None
 
@@ -66,39 +65,14 @@
         self.descendant_fonts = None
         self.to_unicode = None
         self.c_i_d_system_info = None
         self.font_descriptor = None
         self.c_i_d_to_g_i_d_map = None
 
 
-class PDFFontDescriptor(PDFObject):
-    def __init__(
-        self,
-        ascent,
-        descent,
-        cap_height,
-        flags,
-        font_b_box,
-        italic_angle,
-        stem_v,
-        missing_width,
-    ):
-        super().__init__()
-        self.type = Name("FontDescriptor")
-        self.ascent = ascent
-        self.descent = descent
-        self.cap_height = cap_height
-        self.flags = flags
-        self.font_b_box = font_b_box
-        self.italic_angle = italic_angle
-        self.stem_v = stem_v
-        self.missing_width = missing_width
-        self.font_name = None
-
-
 class CIDSystemInfo(PDFObject):
     def __init__(self):
         super().__init__()
         self.registry = PDFString("Adobe", encrypt=True)
         self.ordering = PDFString("UCS", encrypt=True)
         self.supplement = 0
 
@@ -111,20 +85,20 @@
         author,
         keywords,
         creator,
         producer,
         creation_date: PDFDate,
     ):
         super().__init__()
-        self.title = PDFString(title) if title else None
-        self.subject = PDFString(subject) if subject else None
-        self.author = PDFString(author) if author else None
-        self.keywords = PDFString(keywords) if keywords else None
-        self.creator = PDFString(creator) if creator else None
-        self.producer = PDFString(producer) if producer else None
+        self.title = PDFString(title, encrypt=True) if title else None
+        self.subject = PDFString(subject, encrypt=True) if subject else None
+        self.author = PDFString(author, encrypt=True) if author else None
+        self.keywords = PDFString(keywords, encrypt=True) if keywords else None
+        self.creator = PDFString(creator, encrypt=True) if creator else None
+        self.producer = PDFString(producer, encrypt=True) if producer else None
         self.creation_date = creation_date
 
 
 class AcroForm:
     def __init__(self, fields, sig_flags):
         self.fields = fields
         self.sig_flags = sig_flags
@@ -542,137 +516,118 @@
                             sig_annotation_obj is None
                         ), "A /Sig annotation is present on more than 1 page"
                         sig_annotation_obj = annot_obj
         return sig_annotation_obj
 
     def _add_fonts(self):
         font_objs_per_index = {}
-        for font in sorted(self.fpdf.fonts.values(), key=lambda font: font["i"]):
+        for font in sorted(self.fpdf.fonts.values(), key=lambda font: font.i):
             # Standard font
-            if font["type"] == "core":
+            if font.type == "core":
                 encoding = (
                     "WinAnsiEncoding"
-                    if font["name"] not in ("Symbol", "ZapfDingbats")
+                    if font.name not in ("Symbol", "ZapfDingbats")
                     else None
                 )
                 core_font_obj = PDFFont(
-                    subtype="Type1", base_font=font["name"], encoding=encoding
+                    subtype="Type1", base_font=font.name, encoding=encoding
                 )
                 self._add_pdf_obj(core_font_obj, "fonts")
-                font_objs_per_index[font["i"]] = core_font_obj
-            elif font["type"] == "TTF":
-                fontname = f"MPDFAA+{font['name']}"
-
-                # unicode_char -> new_code_char map for chars embedded in the PDF
-                uni_to_new_code_char = font["subset"].dict()
-
-                # why we delete 0-element?
-                del uni_to_new_code_char[0]
-
-                # ---- FONTTOOLS SUBSETTER ----
-                # recalcTimestamp=False means that it doesn't modify the "modified" timestamp in head table
-                # if we leave recalcTimestamp=True the tests will break every time
-                fonttools_font = ttLib.TTFont(
-                    file=font["ttffile"], recalcTimestamp=False, fontNumber=0, lazy=True
-                )
+                font_objs_per_index[font.i] = core_font_obj
+            elif font.type == "TTF":
+                fontname = f"MPDFAA+{font.name}"
 
                 # 1. get all glyphs in PDF
-                cmap = fonttools_font["cmap"].getBestCmap()
-                glyph_names = [
-                    cmap[unicode] for unicode in uni_to_new_code_char if unicode in cmap
-                ]
+                glyph_names = font.subset.get_all_glyph_names()
 
-                missing_glyphs = [
-                    chr(unicode)
-                    for unicode in uni_to_new_code_char
-                    if unicode not in cmap
-                ]
-                if len(missing_glyphs) > 0:
+                if len(font.missing_glyphs) > 0:
                     LOGGER.warning(
                         "Font %s is missing the following glyphs: %s",
                         fontname,
-                        ", ".join(missing_glyphs),
+                        ", ".join(chr(x) for x in font.missing_glyphs),
                     )
 
                 # 2. make a subset
                 # notdef_outline=True means that keeps the white box for the .notdef glyph
                 # recommended_glyphs=True means that adds the .notdef, .null, CR, and space glyphs
                 options = ftsubset.Options(notdef_outline=True, recommended_glyphs=True)
-                # dropping the tables previous dropped in the old ttfonts.py file #issue 418
+                # dropping some tables that currently not used:
                 options.drop_tables += [
                     "FFTM",  # FontForge Timestamp table - cf. https://github.com/PyFPDF/fpdf2/issues/600
                     "GDEF",  # Glyph Definition table = various glyph properties used in OpenType layout processing
                     "GPOS",  # Glyph Positioning table = precise control over glyph placement
                     #          for sophisticated text layout and rendering in each script and language system
                     "GSUB",  # Glyph Substitution table = data for substition of glyphs for appropriate rendering of scripts
                     "MATH",  # Mathematical typesetting table = specific information necessary for math formula layout
                     "hdmx",  # Horizontal Device Metrics table, stores integer advance widths scaled to particular pixel sizes
                     #          for OpenType™ fonts with TrueType outlines
+                    "meta",  # metadata table
                 ]
                 subsetter = ftsubset.Subsetter(options)
                 subsetter.populate(glyphs=glyph_names)
-                subsetter.subset(fonttools_font)
+                subsetter.subset(font.ttfont)
 
                 # 3. make codeToGlyph
                 # is a map Character_ID -> Glyph_ID
                 # it's used for associating glyphs to new codes
                 # this basically takes the old code of the character
                 # take the glyph associated with it
                 # and then associate to the new code the glyph associated with the old code
-                code_to_glyph = {}
-                for code, new_code_mapped in uni_to_new_code_char.items():
-                    # notdef is associated if no glyph was associated to the old code
-                    # it's not necessary to do this, it seems to be done by default
-                    glyph_name = cmap.get(code, ".notdef")
-                    code_to_glyph[new_code_mapped] = fonttools_font.getGlyphID(
-                        glyph_name
-                    )
+
+                code_to_glyph = {
+                    font.subset._map[glyph]: font.ttfont.getGlyphID(glyph.glyph_name)
+                    for glyph in font.subset._map.keys()
+                }
 
                 # 4. return the ttfile
                 output = BytesIO()
-                fonttools_font.save(output)
+                font.ttfont.save(output)
 
                 output.seek(0)
                 ttfontstream = output.read()
 
                 # A composite font - a font composed of other fonts,
                 # organized hierarchically
                 composite_font_obj = PDFFont(
                     subtype="Type0", base_font=fontname, encoding="Identity-H"
                 )
                 self._add_pdf_obj(composite_font_obj, "fonts")
-                font_objs_per_index[font["i"]] = composite_font_obj
+                font_objs_per_index[font.i] = composite_font_obj
 
                 # A CIDFont whose glyph descriptions are based on
                 # TrueType font technology
                 cid_font_obj = PDFFont(
                     subtype="CIDFontType2",
                     base_font=fontname,
-                    d_w=font["desc"].missing_width,
-                    w=_tt_font_widths(font, max(uni_to_new_code_char)),
+                    d_w=font.desc.missing_width,
+                    w=_tt_font_widths(font),
                 )
                 self._add_pdf_obj(cid_font_obj, "fonts")
                 composite_font_obj.descendant_fonts = PDFArray([cid_font_obj])
 
                 # bfChar
                 # This table informs the PDF reader about the unicode
                 # character that each used 16-bit code belongs to. It
                 # allows searching the file and copying text from it.
                 bfChar = []
-                uni_to_new_code_char = font["subset"].dict()
-                for code, code_mapped in uni_to_new_code_char.items():
-                    if code > 0xFFFF:
+
+                def format_code(unicode):
+                    if unicode > 0xFFFF:
                         # Calculate surrogate pair
-                        code_high = 0xD800 | (code - 0x10000) >> 10
-                        code_low = 0xDC00 | (code & 0x3FF)
-                        bfChar.append(
-                            f"<{code_mapped:04X}> <{code_high:04X}{code_low:04X}>\n"
-                        )
-                    else:
-                        bfChar.append(f"<{code_mapped:04X}> <{code:04X}>\n")
+                        code_high = 0xD800 | (unicode - 0x10000) >> 10
+                        code_low = 0xDC00 | (unicode & 0x3FF)
+                        return f"{code_high:04X}{code_low:04X}"
+                    return f"{unicode:04X}"
+
+                for glyph, code_mapped in font.subset._map.items():
+                    if len(glyph.unicode) == 0:
+                        continue
+                    bfChar.append(
+                        f'<{code_mapped:04X}> <{"".join(format_code(code) for code in glyph.unicode)}>\n'
+                    )
 
                 to_unicode_obj = PDFContentStream(
                     "/CIDInit /ProcSet findresource begin\n"
                     "12 dict begin\n"
                     "begincmap\n"
                     "/CIDSystemInfo\n"
                     "<</Registry (Adobe)\n"
@@ -695,15 +650,15 @@
                 self._add_pdf_obj(to_unicode_obj, "fonts")
                 composite_font_obj.to_unicode = to_unicode_obj
 
                 cid_system_info_obj = CIDSystemInfo()
                 self._add_pdf_obj(cid_system_info_obj, "fonts")
                 cid_font_obj.c_i_d_system_info = cid_system_info_obj
 
-                font_descriptor_obj = font["desc"]
+                font_descriptor_obj = font.desc
                 font_descriptor_obj.font_name = Name(fontname)
                 self._add_pdf_obj(font_descriptor_obj, "fonts")
                 cid_font_obj.font_descriptor = font_descriptor_obj
 
                 # Embed CIDToGIDMap
                 # A specification of the mapping from CIDs to glyph indices
                 cid_to_gid_map = ["\x00"] * 256 * 256 * 2
@@ -719,14 +674,16 @@
                 self._add_pdf_obj(cid_to_gid_map_obj, "fonts")
                 cid_font_obj.c_i_d_to_g_i_d_map = cid_to_gid_map_obj
 
                 font_file_cs_obj = PDFFontStream(contents=ttfontstream)
                 self._add_pdf_obj(font_file_cs_obj, "fonts")
                 font_descriptor_obj.font_file2 = font_file_cs_obj
 
+                font.close()
+
         return font_objs_per_index
 
     def _add_images(self):
         img_objs_per_index = {}
         for img in sorted(self.fpdf.images.values(), key=lambda img: img["i"]):
             if img["usages"] > 0:
                 img_objs_per_index[img["i"]] = self._add_image(img)
@@ -977,57 +934,52 @@
 
     def _log_final_sections_sizes(self):
         LOGGER.debug("Final size summary of the biggest document sections:")
         for label, section_size in self.sections_size_per_trace_label.items():
             LOGGER.debug("- %s: %s", label, _sizeof_fmt(section_size))
 
 
-def _tt_font_widths(font, maxUni):
+def _tt_font_widths(font):
     rangeid = 0
     range_ = {}
     range_interval = {}
     prevcid = -2
     prevwidth = -1
     interval = False
-    startcid = 1
-    cwlen = maxUni + 1
 
-    # for each character
-    subset = font["subset"].dict()
-    for cid in range(startcid, cwlen):
-        char_width = font["cw"][cid]
-        if "dw" not in font or (font["dw"] and char_width != font["dw"]):
-            cid_mapped = subset.get(cid)
-            if cid_mapped is None:
-                continue
-            if cid_mapped == (prevcid + 1):
-                if char_width == prevwidth:
-                    if char_width == range_[rangeid][0]:
-                        range_.setdefault(rangeid, []).append(char_width)
-                    else:
-                        range_[rangeid].pop()
-                        # new range
-                        rangeid = prevcid
-                        range_[rangeid] = [prevwidth, char_width]
-                    interval = True
-                    range_interval[rangeid] = True
+    # Glyphs sorted by mapped character id
+    glyphs = dict(sorted(font.subset._map.items(), key=lambda item: item[1]))
+
+    for glyph in glyphs:
+        cid_mapped = glyphs[glyph]
+        if cid_mapped == (prevcid + 1):
+            if glyph.glyph_width == prevwidth:
+                if glyph.glyph_width == range_[rangeid][0]:
+                    range_.setdefault(rangeid, []).append(glyph.glyph_width)
                 else:
-                    if interval:
-                        # new range
-                        rangeid = cid_mapped
-                        range_[rangeid] = [char_width]
-                    else:
-                        range_[rangeid].append(char_width)
-                    interval = False
+                    range_[rangeid].pop()
+                    # new range
+                    rangeid = prevcid
+                    range_[rangeid] = [prevwidth, glyph.glyph_width]
+                interval = True
+                range_interval[rangeid] = True
             else:
-                rangeid = cid_mapped
-                range_[rangeid] = [char_width]
+                if interval:
+                    # new range
+                    rangeid = cid_mapped
+                    range_[rangeid] = [glyph.glyph_width]
+                else:
+                    range_[rangeid].append(glyph.glyph_width)
                 interval = False
-            prevcid = cid_mapped
-            prevwidth = char_width
+        else:
+            rangeid = cid_mapped
+            range_[rangeid] = [glyph.glyph_width]
+            interval = False
+        prevcid = cid_mapped
+        prevwidth = glyph.glyph_width
     prevk = -1
     nextk = -1
     prevint = False
 
     ri = range_interval
     for k, ws in sorted(range_.items()):
         cws = len(ws)
```

### Comparing `fpdf2-2.7.4/fpdf/prefs.py` & `fpdf2-2.7.5/fpdf/prefs.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/recorder.py` & `fpdf2-2.7.5/fpdf/recorder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import types, warnings
 from copy import deepcopy
 
+from .deprecation import get_stack_level
 from .errors import FPDFException
 
 
 class FPDFRecorder:
     """
     The class is aimed to be used as wrapper around fpdf.FPDF:
 
@@ -44,15 +45,16 @@
     def replay(self):
         for call in self._calls:
             func, args, kwargs = call
             try:
                 result = func(*args, **kwargs)
                 if isinstance(result, types.GeneratorType):
                     warnings.warn(
-                        "Detected usage of a context manager inside an unbreakable() section, which is not supported"
+                        "Detected usage of a context manager inside an unbreakable() section, which is not supported",
+                        stacklevel=get_stack_level(),
                     )
                 # The results of other methods can also be invalidated: .pages_count, page_no(), get_x() / get_y(), will_page_break()
             except Exception as error:
                 raise FPDFException(
                     f"Failed to replay FPDF call: {func}(*{args}, **{kwargs})"
                 ) from error
         self._calls = []
```

### Comparing `fpdf2-2.7.4/fpdf/sign.py` & `fpdf2-2.7.5/fpdf/sign.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/structure_tree.py` & `fpdf2-2.7.5/fpdf/structure_tree.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/svg.py` & `fpdf2-2.7.5/fpdf/svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 _HANDY_NAMESPACES = {
     "svg": "http://www.w3.org/2000/svg",
     "xlink": "http://www.w3.org/1999/xlink",
 }
 
 NUMBER_SPLIT = re.compile(r"(?:\s+,\s+|\s+,|,\s+|\s+|,)")
 TRANSFORM_GETTER = re.compile(
+    # pylint: disable=implicit-str-concat
     r"(matrix|rotate|scale|scaleX|scaleY|skew|skewX|skewY|translate|translateX|translateY)"
     r"\(((?:\s*(?:[-+]?[\d\.]+,?)+\s*)+)\)"
 )
 
 
 @force_nodocument
 class Percent(float):
@@ -299,16 +300,15 @@
     parse_style(svg_element)
 
     stylable.style.auto_close = False
 
     for attr_name, converter in svg_attr_map.items():
         value = svg_element.attrib.get(attr_name)
         if value:
-            attr_name, value = converter(value)
-            setattr(stylable.style, attr_name, value)
+            setattr(stylable.style, *converter(value))
 
     # handle this separately for now
     opacity = svg_element.attrib.get("opacity")
     if opacity:
         opacity = float(opacity)
         stylable.style.fill_opacity = opacity
         stylable.style.stroke_opacity = opacity
@@ -469,15 +469,15 @@
 
     # SVG 2 uses CSS transforms. SVG 1.1 transforms are slightly different. I'm really
     # not sure if it is worth it to try to support SVG 2 because it is significantly
     # more entangled with The HTML Disaster than SVG 1.1, which makes it astronomically
     # harder to support.
     # https://drafts.csswg.org/css-transforms/#two-d-transform-functions
     parsed = TRANSFORM_GETTER.findall(tfstr)
-
+    # pylint: disable=redefined-loop-name
     transform = Transform.identity()
     for tf_type, args in parsed:
         if tf_type == "matrix":
             a, b, c, d, e, f = tuple(float(n) for n in NUMBER_SPLIT.split(args))
             transform = Transform(a, b, c, d, e, f) @ transform
 
         elif tf_type == "rotate":
```

### Comparing `fpdf2-2.7.4/fpdf/syntax.py` & `fpdf2-2.7.5/fpdf/syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
     Main features of this class:
     * delay ID assignement
     * implement serializing
     """
 
     # Note: several child classes use __slots__ to save up some memory
 
-    # pylint: disable=redefined-builtin
     def __init__(self):
         self._id = None
 
     @property
     def id(self):
         if self._id is None:
             raise AttributeError(
@@ -175,14 +174,15 @@
         output.append(">>")
         content_stream = self.content_stream()
         if content_stream:
             output.append(create_stream(content_stream))
         output.append("endobj")
         return "\n".join(output)
 
+    # pylint: disable=no-self-use
     def content_stream(self):
         "Subclasses can override this method to indicate the presence of a content stream"
         return b""
 
     def _build_obj_dict(self, security_handler=None):
         """
         Build the PDF Object associative map to serialize,
@@ -230,14 +230,15 @@
         if (
             callable(value)
             or key.startswith("_")
             or key in ("id", "ref")
             or value is None
         ):
             continue
+        # pylint: disable=redefined-loop-name
         if hasattr(value, "value"):  # e.g. Enum subclass
             value = value.value
         if isinstance(value, PDFObject):  # indirect object reference
             value = value.ref
         elif hasattr(value, "serialize"):
             # e.g. PDFArray, PDFString, Name, Destination, Action...
             value = value.serialize(
@@ -319,15 +320,15 @@
 
 
 class PDFArray(list):
     def serialize(self, _security_handler=None, _obj_id=None):
         if all(isinstance(elem, str) for elem in self):
             serialized_elems = " ".join(self)
         elif all(isinstance(elem, int) for elem in self):
-            serialized_elems = " ".join(map(str, self))
+            serialized_elems = " ".join(str(elem) for elem in self)
         else:
             serialized_elems = "\n".join(
                 elem.ref
                 if isinstance(elem, PDFObject)
                 else elem.serialize(
                     _security_handler=_security_handler, _obj_id=_obj_id
                 )
@@ -354,14 +355,17 @@
         return (
             self.page_number == dest.page_number
             and self.top == dest.top
             and self.left == dest.left
             and self.zoom == dest.zoom
         )
 
+    def __hash__(self):
+        return hash((self.page_number, self.top, self.left, self.zoom))
+
     def __repr__(self):
         return f'DestinationXYZ(page_number={self.page_number}, top={self.top}, left={self.left}, zoom="{self.zoom}", page_ref={self.page_ref})'
 
     def serialize(self, _security_handler=None, _obj_id=None):
         left = round(self.left, 2) if isinstance(self.left, float) else self.left
         top = round(self.top, 2) if isinstance(self.top, float) else self.top
         assert self.page_ref
```

### Comparing `fpdf2-2.7.4/fpdf/table.py` & `fpdf2-2.7.5/fpdf/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import dataclass
 from numbers import Number
 from typing import Optional, Union
 
-from .enums import Align, TableBordersLayout, TableCellFillMode
+from .enums import Align, TableBordersLayout, TableCellFillMode, WrapMode
 from .enums import MethodReturnValue
 from .errors import FPDFException
-from .fonts import FontFace
+from .fonts import CORE_FONTS, FontFace
 
 
 DEFAULT_HEADINGS_STYLE = FontFace(emphasis="BOLD")
 
 
 @dataclass(frozen=True)
 class RowLayoutInfo:
-    height: int
+    height: float
     triggers_page_jump: bool
 
 
 class Table:
     """
     Object that `fpdf.FPDF.table()` yields, used to build a table in the document.
     Detailed usage documentation: https://pyfpdf.github.io/fpdf2/Tables.html
@@ -30,52 +30,62 @@
         *,
         align="CENTER",
         borders_layout=TableBordersLayout.ALL,
         cell_fill_color=None,
         cell_fill_mode=TableCellFillMode.NONE,
         col_widths=None,
         first_row_as_headings=True,
+        gutter_height=0,
+        gutter_width=0,
         headings_style=DEFAULT_HEADINGS_STYLE,
         line_height=None,
         markdown=False,
         text_align="JUSTIFY",
         width=None,
+        wrapmode=WrapMode.WORD,
     ):
         """
         Args:
             fpdf (fpdf.FPDF): FPDF current instance
             rows: optional. Sequence of rows (iterable) of str to initiate the table cells with text content
             align (str, fpdf.enums.Align): optional, default to CENTER. Sets the table horizontal position relative to the page,
                 when it's not using the full page width
             borders_layout (str, fpdf.enums.TableBordersLayout): optional, default to ALL. Control what cell borders are drawn
-            cell_fill_color (int, tuple, fpdf.drawing.DeviceGray, fpdf.drawing.DeviceRGB): optional.
+            cell_fill_color (float, tuple, fpdf.drawing.DeviceGray, fpdf.drawing.DeviceRGB): optional.
                 Defines the cells background color
             cell_fill_mode (str, fpdf.enums.TableCellFillMode): optional. Defines which cells are filled with color in the background
-            col_widths (int, tuple): optional. Sets column width. Can be a single number or a sequence of numbers
+            col_widths (float, tuple): optional. Sets column width. Can be a single number or a sequence of numbers
             first_row_as_headings (bool): optional, default to True. If False, the first row of the table
                 is not styled differently from the others
+            gutter_height (float): optional vertical space between rows
+            gutter_width (float): optional horizontal space between columns
             headings_style (fpdf.fonts.FontFace): optional, default to bold.
                 Defines the visual style of the top headings row: size, color, emphasis...
             line_height (number): optional. Defines how much vertical space a line of text will occupy
             markdown (bool): optional, default to False. Enable markdown interpretation of cells textual content
             text_align (str, fpdf.enums.Align): optional, default to JUSTIFY. Control text alignment inside cells.
             width (number): optional. Sets the table width
+            wrapmode (fpdf.enums.WrapMode): "WORD" for word based line wrapping (default),
+                "CHAR" for character based line wrapping.
         """
         self._fpdf = fpdf
         self._align = align
         self._borders_layout = TableBordersLayout.coerce(borders_layout)
         self._cell_fill_color = cell_fill_color
         self._cell_fill_mode = TableCellFillMode.coerce(cell_fill_mode)
         self._col_widths = col_widths
         self._first_row_as_headings = first_row_as_headings
+        self._gutter_height = gutter_height
+        self._gutter_width = gutter_width
         self._headings_style = headings_style
         self._line_height = 2 * fpdf.font_size if line_height is None else line_height
         self._markdown = markdown
         self._text_align = text_align
         self._width = fpdf.epw if width is None else width
+        self._wrapmode = wrapmode
         self.rows = []
         for row in rows:
             self.row(row)
 
     def row(self, cells=()):
         "Adds a row to the table. Yields a `Row` object."
         row = Row(self._fpdf)
@@ -100,23 +110,29 @@
             if not self._headings_style:
                 raise ValueError(
                     "headings_style must be provided to FPDF.table() if first_row_as_headings=True"
                 )
             emphasis = self._headings_style.emphasis
             if emphasis is not None:
                 family = self._headings_style.family or self._fpdf.font_family
-                font_key = family + emphasis.style
-                if (
-                    font_key not in self._fpdf.core_fonts
-                    and font_key not in self._fpdf.fonts
-                ):
+                font_key = family.lower() + emphasis.style
+                if font_key not in CORE_FONTS and font_key not in self._fpdf.fonts:
                     # Raising a more explicit error than the one from set_font():
                     raise FPDFException(
                         f"Using font emphasis '{emphasis.style}' in table headings require the corresponding font style to be added using add_font()"
                     )
+        if self.rows:
+            cols_count = self.rows[0].cols_count
+            for i, row in enumerate(self.rows[1:], start=2):
+                if row.cols_count != cols_count:
+                    raise FPDFException(
+                        f"Inconsistent column count detected on row {i}:"
+                        f" it has {row.cols_count} columns,"
+                        f" whereas the top row has {cols_count}."
+                    )
         # Defining table global horizontal position:
         prev_l_margin = self._fpdf.l_margin
         if table_align == Align.C:
             self._fpdf.l_margin = (self._fpdf.w - self._width) / 2
             self._fpdf.x = self._fpdf.l_margin
         elif table_align == Align.R:
             self._fpdf.l_margin = self._fpdf.w - self._fpdf.r_margin - self._width
@@ -126,15 +142,17 @@
         # Starting the actual rows & cells rendering:
         for i in range(len(self.rows)):
             row_layout_info = self._get_row_layout_info(i)
             if row_layout_info.triggers_page_jump:
                 # pylint: disable=protected-access
                 self._fpdf._perform_page_break()
                 if self._first_row_as_headings:  # repeat headings on top:
-                    self._render_table_row(0)
+                    self._render_table_row(0, self._get_row_layout_info(0))
+            elif i and self._gutter_height:
+                self._fpdf.y += self._gutter_height
             self._render_table_row(i, row_layout_info)
         # Restoring altered FPDF settings:
         self._fpdf.l_margin = prev_l_margin
         self._fpdf.x = self._fpdf.l_margin
 
     def get_cell_border(self, i, j):
         """
@@ -187,50 +205,51 @@
             border = list("TB")
             if i != 1 and "T" in border:
                 border.remove("T")
             if i != 0 and "B" in border:
                 border.remove("B")
         return "".join(border)
 
-    def _render_table_row(self, i, row_layout_info=None, fill=False, **kwargs):
-        if not row_layout_info:
-            row_layout_info = self._get_row_layout_info(i)
+    def _render_table_row(self, i, row_layout_info, fill=False, **kwargs):
         row = self.rows[i]
         j = 0
-        while j < len(row.cells):
+        for cell in row.cells:
             self._render_table_cell(
                 i,
                 j,
+                cell,
                 row_height=row_layout_info.height,
                 fill=fill,
                 **kwargs,
             )
-            j += row.cells[j].colspan
+            j += cell.colspan
         self._fpdf.ln(row_layout_info.height)
 
-    # pylint: disable=inconsistent-return-statements
     def _render_table_cell(
         self,
         i,
         j,
+        cell,
         row_height,
         fill=False,
         **kwargs,
     ):
         row = self.rows[i]
-        cell = row.cells[j]
         col_width = self._get_col_width(i, j, cell.colspan)
+        if j and self._gutter_width:
+            self._fpdf.x += self._gutter_width
         img_height = 0
         if cell.img:
             x, y = self._fpdf.x, self._fpdf.y
             img_height = self._fpdf.image(
                 cell.img,
                 w=col_width,
                 h=0 if cell.img_fill_width else row_height,
                 keep_aspect_ratio=True,
+                link=cell.link,
             ).rendered_height
             self._fpdf.set_xy(x, y)
         text_align = cell.align or self._text_align
         if not isinstance(text_align, (Align, str)):
             text_align = text_align[j]
         if i == 0 and self._first_row_as_headings:
             style = self._headings_style
@@ -258,57 +277,64 @@
         with self._fpdf.use_font_face(style):
             page_break, cell_height = self._fpdf.multi_cell(
                 w=col_width,
                 h=row_height,
                 txt=cell.text,
                 max_line_height=self._line_height,
                 border=self.get_cell_border(i, j),
+                link=cell.link,
                 align=text_align,
                 new_x="RIGHT",
                 new_y="TOP",
                 fill=fill,
                 markdown=self._markdown,
                 output=MethodReturnValue.PAGE_BREAK | MethodReturnValue.HEIGHT,
+                wrapmode=self._wrapmode,
                 **kwargs,
             )
         return page_break, max(img_height, cell_height)
 
     def _get_col_width(self, i, j, colspan=1):
+        cols_count = self.rows[i].cols_count
+        width = self._width - (cols_count - 1) * self._gutter_width
         if not self._col_widths:
-            cols_count = self.rows[i].cols_count
-            return colspan * (self._width / cols_count)
+            return colspan * (width / cols_count)
         if isinstance(self._col_widths, Number):
             return colspan * self._col_widths
         if j >= len(self._col_widths):
             raise ValueError(
                 f"Invalid .col_widths specified: missing width for table() column {j + 1} on row {i + 1}"
             )
-        # pylint: disable=unsubscriptable-object
         col_width = 0
         for k in range(j, j + colspan):
             col_ratio = self._col_widths[k] / sum(self._col_widths)
-            col_width += col_ratio * self._width
+            col_width += col_ratio * width
+            if k != j:
+                col_width += self._gutter_width
         return col_width
 
     def _get_row_layout_info(self, i):
         """
-        Uses FPDF.offset_rendering() to detect a potential page jump
-        and compute the cells heights.
+        Compute the cells heights & detect page jumps,
+        but disable actual rendering by using FPDF._disable_writing()
         """
         row = self.rows[i]
         heights_per_cell = []
         any_page_break = False
         # pylint: disable=protected-access
         with self._fpdf._disable_writing():
-            for j in range(len(row.cells)):
+            j = 0
+            for cell in row.cells:
                 page_break, height = self._render_table_cell(
                     i,
                     j,
+                    cell,
                     row_height=self._line_height,
                 )
+                j += cell.colspan
                 any_page_break = any_page_break or page_break
                 heights_per_cell.append(height)
         row_height = (
             max(height for height in heights_per_cell) if heights_per_cell else 0
         )
         return RowLayoutInfo(row_height, any_page_break)
 
@@ -322,58 +348,70 @@
         self.style = fpdf.font_face()
 
     @property
     def cols_count(self):
         return sum(cell.colspan for cell in self.cells)
 
     def cell(
-        self, text="", align=None, style=None, img=None, img_fill_width=False, colspan=1
+        self,
+        text="",
+        align=None,
+        style=None,
+        img=None,
+        img_fill_width=False,
+        colspan=1,
+        link=None,
     ):
         """
         Adds a cell to the row.
 
         Args:
             text (str): string content, can contain several lines.
                 In that case, the row height will grow proportionally.
             align (str, fpdf.enums.Align): optional text alignment.
             style (fpdf.fonts.FontFace): optional text style.
             img: optional. Either a string representing a file path to an image,
                 an URL to an image, an io.BytesIO, or a instance of `PIL.Image.Image`.
             img_fill_width (bool): optional, defaults to False. Indicates to render the image
                 using the full width of the current table column.
             colspan (int): optional number of columns this cell should span.
+            link (str, int): optional link, either an URL or an integer returned by `FPDF.add_link`, defining an internal link to a page
+
         """
         if text and img:
             raise NotImplementedError(
+                # pylint: disable=implicit-str-concat
                 "fpdf2 currently does not support inserting text with an image in the same table cell."
                 "Pull Requests are welcome to implement this 😊"
             )
         if not style:
             # We capture the current font settings:
             font_face = self._fpdf.font_face()
             if font_face != self.style:
                 style = font_face
-        cell = Cell(text, align, style, img, img_fill_width, colspan)
+        cell = Cell(text, align, style, img, img_fill_width, colspan, link)
         self.cells.append(cell)
         return cell
 
 
 @dataclass(frozen=True)
 class Cell:
     "Internal representation of a table cell"
     __slots__ = (  # RAM usage optimization
         "text",
         "align",
         "style",
         "img",
         "img_fill_width",
         "colspan",
+        "link",
     )
     text: str
     align: Optional[Union[str, Align]]
     style: Optional[FontFace]
     img: Optional[str]
     img_fill_width: bool
     colspan: int
+    link: Optional[Union[str, int]]
 
     def write(self, text, align=None):
         raise NotImplementedError("Not implemented yet")
```

### Comparing `fpdf2-2.7.4/fpdf/template.py` & `fpdf2-2.7.5/fpdf/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 __author__ = "Mariano Reingart <reingart@gmail.com>"
 __copyright__ = "Copyright (C) 2010 Mariano Reingart"
 __license__ = "LGPL 3.0"
 
 import csv, locale, warnings
 
+from .deprecation import get_stack_level
 from .errors import FPDFException
 from .fpdf import FPDF
 
 
 def _rgb(col):
     return (col // 65536), (col // 256 % 256), (col % 256)
 
@@ -119,15 +120,14 @@
                 else:
                     raise KeyError("Mandatory key 'x2' missing in input data")
             if not "size" in e and e["type"] == "C39":
                 if "w" in e:
                     e["size"] = e["w"]
             for k, t in key_config.items():
                 if k in e and not isinstance(e[k], t):
-                    # pylint: disable=no-member
                     ttype = (
                         t.__name__
                         if isinstance(t, type)
                         else " or ".join([f"'{x.__name__}'" for x in t])
                     )
                     raise TypeError(
                         f"Value of element item '{k}' must be {ttype}, not '{type(e[k]).__name__}'."
@@ -477,15 +477,15 @@
         h=None,
         **__,
     ):
         if x is not None or y is not None or w is not None or h is not None:
             warnings.warn(
                 "code39 arguments x/y/w/h are deprecated, please use x1/y1/y2/size instead",
                 DeprecationWarning,
-                stacklevel=2,
+                stacklevel=get_stack_level(),
             )
         pdf = self.pdf
         if pdf.fill_color.serialize().lower() != _rgb_as_str(foreground):
             pdf.set_fill_color(*_rgb(foreground))
         h = y2 - y1
         if h <= 0:
             h = 5
@@ -587,15 +587,14 @@
     A simple templating class.
 
     Allows to apply a single template definition to all pages of a document.
     """
 
     # Disabling this check due to the "format" parameter below:
     # pylint: disable=redefined-builtin
-    # pylint: disable=unused-argument
     def __init__(
         self,
         infile=None,
         elements=None,
         format="A4",
         orientation="portrait",
         unit="mm",
@@ -635,15 +634,15 @@
 
             creator (str): The creator of the document.
         """
         if infile:
             warnings.warn(
                 '"infile" is deprecated, unused and will soon be removed',
                 DeprecationWarning,
-                stacklevel=2,
+                stacklevel=get_stack_level(),
             )
         for arg in (
             "format",
             "orientation",
             "unit",
             "title",
             "author",
@@ -682,14 +681,14 @@
             dest (str):
                 [**DEPRECATED since 2.2.0**] unused, will be removed in a later version.
         """
         if dest:
             warnings.warn(
                 '"dest" is deprecated, unused and will soon be removed',
                 DeprecationWarning,
-                stacklevel=2,
+                stacklevel=get_stack_level(),
             )
         self.pdf.set_font("helvetica", "B", 16)
         self.pdf.set_auto_page_break(False, margin=0)
         super().render()
         if outfile:
             self.pdf.output(outfile)
```

### Comparing `fpdf2-2.7.4/fpdf/transitions.py` & `fpdf2-2.7.5/fpdf/transitions.py`

 * *Files identical despite different names*

### Comparing `fpdf2-2.7.4/fpdf/util.py` & `fpdf2-2.7.5/fpdf/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,15 @@
         old_unit (str, float, int): A unit accepted by fpdf.FPDF or a number
         new_unit (str, float, int): A unit accepted by fpdf.FPDF or a number
     Returns:
         (float, tuple): to_convert converted from old_unit to new_unit or a tuple of the same
     """
     unit_conversion_factor = get_scale_factor(new_unit) / get_scale_factor(old_unit)
     if isinstance(to_convert, Iterable):
-        return tuple(
-            map(lambda i: convert_unit(i, 1, unit_conversion_factor), to_convert)
-        )
+        return tuple(convert_unit(i, 1, unit_conversion_factor) for i in to_convert)
     return to_convert / unit_conversion_factor
 
 
 ################################################################################
 ################### Utility functions to track memory usage ####################
 ################################################################################
 
@@ -131,16 +129,16 @@
     pid = os.getpid()
     try:
         with open(f"/proc/{pid}/maps", encoding="utf8") as maps_file:
             maps_lines = list(maps_file)
     except FileNotFoundError:  # This file only exists under Linux
         return heap_size_in_mib, stack_size_in_mib
     for line in maps_lines:
-        line = line.split()
-        addr_range, path = line[0], line[-1]
+        words = line.split()
+        addr_range, path = words[0], words[-1]
         addr_start, addr_end = addr_range.split("-")
         addr_start, addr_end = int(addr_start, 16), int(addr_end, 16)
         size = addr_end - addr_start
         if path == "[heap]":
             heap_size_in_mib = f"{size / 1024 / 1024:.1f} MiB"
         elif path == "[stack]":
             stack_size_in_mib = f"{size / 1024 / 1024:.1f} MiB"
```

### Comparing `fpdf2-2.7.4/fpdf2.egg-info/PKG-INFO` & `fpdf2-2.7.5/fpdf2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fpdf2
-Version: 2.7.4
+Version: 2.7.5
 Summary: Simple & fast PDF generation for Python
 Home-page: https://pyfpdf.github.io/fpdf2/
-Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.4
+Download-URL: https://github.com/PyFPDF/fpdf2/tarball/2.7.5
 Author: Olivier PLATHEY ported by Max
 Maintainer: Lucas Cimon
 License: LGPLv3+
 Project-URL: Documentation, https://pyfpdf.github.io/fpdf2/
 Project-URL: Code, https://github.com/PyFPDF/fpdf2
 Project-URL: Issue tracker, https://github.com/PyFPDF/fpdf2/issues
 Keywords: pdf,unicode,png,jpg,ttf,barcode
@@ -95,15 +95,15 @@
  * Internal / external [links](https://pyfpdf.github.io/fpdf2/Links.html)
  * Embedding images, including transparency and alpha channel
  * Arbitrary path drawing and basic [SVG](https://pyfpdf.github.io/fpdf2/SVG.html) import
  * Embedding [barcodes](https://pyfpdf.github.io/fpdf2/Barcodes.html), [charts & graphs](https://pyfpdf.github.io/fpdf2/Maths.html), [emojis, symbols & dingbats](https://pyfpdf.github.io/fpdf2/EmojisSymbolsDingbats.html)
  * [Tables](https://pyfpdf.github.io/fpdf2/Tables.html) and also [cell / multi-cell / plaintext writing](https://pyfpdf.github.io/fpdf2/Text.html), with [automatic page breaks](https://pyfpdf.github.io/fpdf2/PageBreaks.html), line break and text justification
  * Choice of measurement unit, page format & margins. Optional page header and footer
  * Basic [conversion from HTML to PDF](https://pyfpdf.github.io/fpdf2/HTML.html)
- * A [templating system](https://pyfpdf.github.io/fpdf2/Templates.html) to render PDFs in batchs
+ * A [templating system](https://pyfpdf.github.io/fpdf2/Templates.html) to render PDFs in batches
  * Images & links alternative descriptions, for accessibility
  * Table of contents & [document outline](https://pyfpdf.github.io/fpdf2/DocumentOutlineAndTableOfContents.html)
  * [Document encryption](https://pyfpdf.github.io/fpdf2/Encryption.html) & [document signing](https://pyfpdf.github.io/fpdf2/Signing.html)
  * [Annotations](https://pyfpdf.github.io/fpdf2/Annotations.html), including text highlights, and [file attachments](https://pyfpdf.github.io/fpdf2/FileAttachments.html)
  * [Presentation mode](https://pyfpdf.github.io/fpdf2/Presentations.html) with control over page display duration & transitions
  * Optional basic Markdown-like styling: `**bold**, __italics__`
  * Can render [mathematical equations & charts](https://pyfpdf.github.io/fpdf2/Maths.html)
@@ -132,15 +132,15 @@
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/PyFPDF/fpdf2&t=fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-facebook-1976D2?logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/PyFPDF/fpdf2)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/PyFPDF/fpdf2&title=fpdf2)
 
 ## Documentation
 
 - [Documentation Home](https://pyfpdf.github.io/fpdf2/)
-- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html)
+- Tutorial in several languages: [English](https://pyfpdf.github.io/fpdf2/Tutorial.html) - [Deutsch](https://pyfpdf.github.io/fpdf2/Tutorial-de.html) - [español](https://pyfpdf.github.io/fpdf2/Tutorial-es.html) - [हिंदी](https://pyfpdf.github.io/fpdf2/Tutorial-hi.html) - [português](https://pyfpdf.github.io/fpdf2/Tutorial-pt.html) - [Русский](https://pyfpdf.github.io/fpdf2/Tutorial-ru.html) - [Italian](https://pyfpdf.github.io/fpdf2/Tutorial-it.html) - [français](https://pyfpdf.github.io/fpdf2/Tutorial-fr.html) - [Ελληνικά](https://pyfpdf.github.io/fpdf2/Tutorial-gr.html) - [עברית](https://pyfpdf.github.io/fpdf2/Tutorial-he.html) - [简体中文](https://pyfpdf.github.io/fpdf2/Tutorial-zh.html) - [বাংলা](https://pyfpdf.github.io/fpdf2/Tutorial-bn.html) - [ភាសខ្មែរ](https://pyfpdf.github.io/fpdf2/Tutorial-km.md) - [日本語](https://pyfpdf.github.io/fpdf2/Tutorial-ja.html)
 - Release notes: [CHANGELOG.md](https://github.com/PyFPDF/fpdf2/blob/master/CHANGELOG.md)
 - A series of blog posts: [fpdf2 tag @ ludochaordic](https://chezsoi.org/lucas/blog/tag/fpdf2.html)
 
 You can also have a look at the `tests/`, they're great usage examples!
 
 ## Developement
 
@@ -245,15 +245,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/devdev29"><img src="https://avatars.githubusercontent.com/u/88680035?v=4?s=100" width="100px;" alt="devdev29"/><br /><sub><b>devdev29</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Documentation">📖</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=devdev29" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zenigata"><img src="https://avatars.githubusercontent.com/u/1022393?v=4?s=100" width="100px;" alt="Johan Bonneau"/><br /><sub><b>Johan Bonneau</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Zenigata" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jmunoz94"><img src="https://avatars.githubusercontent.com/u/48921408?v=4?s=100" width="100px;" alt="Jesús Alberto Muñoz Mesa"/><br /><sub><b>Jesús Alberto Muñoz Mesa</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Tests">⚠️</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=jmunoz94" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jdeep.me"><img src="https://avatars.githubusercontent.com/u/64089730?v=4?s=100" width="100px;" alt="Jaydeep Das"/><br /><sub><b>Jaydeep Das</b></sub></a><br /><a href="#question-JDeepD" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/seanpmulholland"><img src="https://avatars.githubusercontent.com/u/79894395?v=4?s=100" width="100px;" alt="Sean"/><br /><sub><b>Sean</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=seanpmulholland" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andersonhc"><img src="https://avatars.githubusercontent.com/u/948125?v=4?s=100" width="100px;" alt="Anderson Herzogenrath da Costa"/><br /><sub><b>Anderson Herzogenrath da Costa</b></sub></a><br /><a href="#question-andersonhc" title="Answering Questions">💬</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Code">💻</a> <a href="#research-andersonhc" title="Research">🔬</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aandersonhc" title="Bug reports">🐛</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=andersonhc" title="Documentation">📖</a> <a href="#ideas-andersonhc" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/yiweelan"><img src="https://avatars.githubusercontent.com/u/117787188?v=4?s=100" width="100px;" alt="Yi Wei Lan"/><br /><sub><b>Yi Wei Lan</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=yiweelan" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bubbu0129"><img src="https://avatars.githubusercontent.com/u/93034081?v=4?s=100" width="100px;" alt="CpDong"/><br /><sub><b>CpDong</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Bubbu0129" title="Code">💻</a> <a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ABubbu0129" title="Bug reports">🐛</a> <a href="#translation-Bubbu0129" title="Translation">🌍</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/CY-Qiu"><img src="https://avatars.githubusercontent.com/u/23075447?v=4?s=100" width="100px;" alt="CY-Qiu"/><br /><sub><b>CY-Qiu</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ACY-Qiu" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Markovvn1"><img src="https://avatars.githubusercontent.com/u/32509100?v=4?s=100" width="100px;" alt="Markovvn1"/><br /><sub><b>Markovvn1</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Markovvn1" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/erap129"><img src="https://avatars.githubusercontent.com/u/30405025?v=4?s=100" width="100px;" alt="Elad Rapaport"/><br /><sub><b>Elad Rapaport</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=erap129" title="Code">💻</a></td>
@@ -266,14 +266,24 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruiz-manuel"><img src="https://avatars.githubusercontent.com/u/43274578?v=4?s=100" width="100px;" alt="Manuel Ruiz"/><br /><sub><b>Manuel Ruiz</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aruiz-manuel" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nsimonovici"><img src="https://avatars.githubusercontent.com/u/44460830?v=4?s=100" width="100px;" alt="Noel"/><br /><sub><b>Noel</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Ansimonovici" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/iamavik/"><img src="https://avatars.githubusercontent.com/u/14172268?v=4?s=100" width="100px;" alt="Avik Sarkar"/><br /><sub><b>Avik Sarkar</b></sub></a><br /><a href="#translation-ssavi-ict" title="Translation">🌍</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=ssavi-ict" title="Documentation">📖</a> <a href="#question-ssavi-ict" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aeris07"><img src="https://avatars.githubusercontent.com/u/129675592?v=4?s=100" width="100px;" alt="aeris07"/><br /><sub><b>aeris07</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Aaeris07" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/KamarulAdha"><img src="https://avatars.githubusercontent.com/u/52944294?v=4?s=100" width="100px;" alt="KamarulAdha"/><br /><sub><b>KamarulAdha</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=KamarulAdha" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Valerus5685"><img src="https://avatars.githubusercontent.com/u/7953869?v=4?s=100" width="100px;" alt="Valerus5685"/><br /><sub><b>Valerus5685</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3AValerus5685" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sebastiantia"><img src="https://avatars.githubusercontent.com/u/75666019?v=4?s=100" width="100px;" alt="Sebastian Tia"/><br /><sub><b>Sebastian Tia</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=sebastiantia" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/1nv"><img src="https://avatars.githubusercontent.com/u/10288828?v=4?s=100" width="100px;" alt="Eugene Selifonov"/><br /><sub><b>Eugene Selifonov</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3A1nv" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://ez-startup.com"><img src="https://avatars.githubusercontent.com/u/69514175?v=4?s=100" width="100px;" alt="Kuth"/><br /><sub><b>Kuth</b></sub></a><br /><a href="#translation-kuth-chi" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://rdbr.nl"><img src="https://avatars.githubusercontent.com/u/34062862?v=4?s=100" width="100px;" alt="Ruben de Bruin"/><br /><sub><b>Ruben de Bruin</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3ARubendeBruin" title="Bug reports">🐛</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=RubendeBruin" title="Code">💻</a> <a href="https://github.com/PyFPDF/fpdf2/commits?author=RubendeBruin" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/stenci"><img src="https://avatars.githubusercontent.com/u/5955495?v=4?s=100" width="100px;" alt="stenci"/><br /><sub><b>stenci</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/issues?q=author%3Astenci" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alcnaka"><img src="https://avatars.githubusercontent.com/u/47954083?v=4?s=100" width="100px;" alt="alcnaka"/><br /><sub><b>alcnaka</b></sub></a><br /><a href="#translation-alcnaka" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tolker-KU"><img src="https://avatars.githubusercontent.com/u/55140581?v=4?s=100" width="100px;" alt="Tolker-KU"/><br /><sub><b>Tolker-KU</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=Tolker-KU" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://lfavole.eu.pythonanywhere.com"><img src="https://avatars.githubusercontent.com/u/88188568?v=4?s=100" width="100px;" alt="lfavole"/><br /><sub><b>lfavole</b></sub></a><br /><a href="https://github.com/PyFPDF/fpdf2/commits?author=lfavole" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

