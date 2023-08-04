# Comparing `tmp/ViTables-3.0.2.tar.gz` & `tmp/vitables-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ViTables-3.0.2.tar", last modified: Wed Dec 25 14:16:10 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ViTables-3.0.2.tar` & `vitables-3.0.3.tar`

### file list

```diff
@@ -1,264 +1,248 @@
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.449155 ViTables-3.0.2/
--rw-rw-rw-   0        0        0     1706 2019-12-25 11:57:28.000000 ViTables-3.0.2/ANNOUNCE.txt
--rw-rw-rw-   0        0        0    76706 2019-12-25 11:43:10.000000 ViTables-3.0.2/ChangeLog.txt
--rw-rw-rw-   0        0        0     2577 2019-12-25 11:58:41.000000 ViTables-3.0.2/INSTALL.txt
--rw-rw-rw-   0        0        0    35975 2019-12-13 13:36:40.000000 ViTables-3.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       49 2019-12-23 17:16:26.000000 ViTables-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1754 2019-12-25 14:16:10.449155 ViTables-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      824 2019-12-24 17:56:37.000000 ViTables-3.0.2/README.txt
--rw-rw-rw-   0        0        0      143 2017-09-07 19:55:59.000000 ViTables-3.0.2/TODO.txt
--rw-rw-rw-   0        0        0        6 2019-12-25 11:44:32.000000 ViTables-3.0.2/VERSION
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.767155 ViTables-3.0.2/ViTables.egg-info/
--rw-rw-rw-   0        0        0     1754 2019-12-25 14:16:09.000000 ViTables-3.0.2/ViTables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8138 2019-12-25 14:16:09.000000 ViTables-3.0.2/ViTables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-12-25 14:16:09.000000 ViTables-3.0.2/ViTables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      280 2019-12-25 14:16:09.000000 ViTables-3.0.2/ViTables.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2019-12-25 14:16:09.000000 ViTables-3.0.2/ViTables.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2019-12-25 14:16:09.000000 ViTables-3.0.2/ViTables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-12-25 14:16:10.464776 ViTables-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3424 2019-12-23 15:49:56.000000 ViTables-3.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.797076 ViTables-3.0.2/vitables/
--rw-rw-rw-   0        0        0    37263 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/LICENSE.html
--rw-rw-rw-   0        0        0     1092 2019-12-25 11:48:16.000000 ViTables-3.0.2/vitables/__init__.py
--rw-rw-rw-   0        0        0       43 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/__main__.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.812035 ViTables-3.0.2/vitables/calculator/
--rw-rw-rw-   0        0        0        2 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/calculator/__init__.py
--rw-rw-rw-   0        0        0    16842 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/calculator/calculator.py
--rw-rw-rw-   0        0        0     5073 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/calculator/calculator.ui
--rw-rw-rw-   0        0        0     6614 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/calculator/calculator_dlg.py
--rw-rw-rw-   0        0        0      456 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/calculator/evaluator.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.818019 ViTables-3.0.2/vitables/calculator/test/
--rw-rw-rw-   0        0        0        0 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/calculator/test/__init__.py
--rw-rw-rw-   0        0        0      922 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/calculator/test/test_calculator.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.831982 ViTables-3.0.2/vitables/csv/
--rw-rw-rw-   0        0        0      882 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/csv/__init__.py
--rw-rw-rw-   0        0        0    14890 2019-12-14 13:29:48.000000 ViTables-3.0.2/vitables/csv/csvutils.py
--rw-rw-rw-   0        0        0    11359 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/csv/export_csv.py
--rw-rw-rw-   0        0        0    18170 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/csv/import_csv.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.844948 ViTables-3.0.2/vitables/docbrowser/
--rw-rw-rw-   0        0        0      937 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/docbrowser/__init__.py
--rw-rw-rw-   0        0        0     8025 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/docbrowser/bookmarksdlg.py
--rw-rw-rw-   0        0        0    14862 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/docbrowser/browsergui.py
--rw-rw-rw-   0        0        0     8856 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/docbrowser/helpbrowser.py
--rw-rw-rw-   0        0        0     2583 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/filenodeutils.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.877860 ViTables-3.0.2/vitables/h5db/
--rw-rw-rw-   0        0        0     1039 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/__init__.py
--rw-rw-rw-   0        0        0     7089 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/dbdoc.py
--rw-rw-rw-   0        0        0    45360 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/dbstreemodel.py
--rw-rw-rw-   0        0        0    13187 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/dbstreeview.py
--rw-rw-rw-   0        0        0     4398 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/groupnode.py
--rw-rw-rw-   0        0        0     4477 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/leafnode.py
--rw-rw-rw-   0        0        0     4466 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/linknode.py
--rw-rw-rw-   0        0        0     4190 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/nodeitemdelegate.py
--rw-rw-rw-   0        0        0     4924 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/rootgroupnode.py
--rw-rw-rw-   0        0        0     5134 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/tlink_editor.py
--rw-rw-rw-   0        0        0     5873 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/h5db/tnode_editor.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.915758 ViTables-3.0.2/vitables/htmldocs/
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.949272 ViTables-3.0.2/vitables/htmldocs/_images/
--rw-rw-rw-   0        0        0    51210 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/browseDataset.png
--rw-rw-rw-   0        0        0    10844 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/editingUserAttrs.png
--rw-rw-rw-   0        0        0    64708 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/groupCreation.png
--rw-rw-rw-   0        0        0    37498 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/helpBrowser.png
--rw-rw-rw-   0        0        0    77227 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/mainWindow.png
--rw-rw-rw-   0        0        0    11102 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/newFilteredTable.png
--rw-rw-rw-   0        0        0    11087 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/propertiesDlg.png
--rw-rw-rw-   0        0        0    47789 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/title_page_plain.png
--rw-rw-rw-   0        0        0    20941 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/treeSymbols.png
--rw-rw-rw-   0        0        0    64021 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_images/zoomingCells.png
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.996137 ViTables-3.0.2/vitables/htmldocs/_static/
--rw-rw-rw-   0        0        0    12934 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/classic.css
--rw-rw-rw-   0        0        0     4525 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/classic_orig.css
--rw-rw-rw-   0        0        0       28 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/default.css
--rw-rw-rw-   0        0        0     9270 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/doctools.js
--rw-rw-rw-   0        0        0      317 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/file.png
--rw-rw-rw-   0        0        0   280364 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/jquery-3.4.1.js
--rw-rw-rw-   0        0        0    88145 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/jquery.js
--rw-rw-rw-   0        0        0    11144 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/minus.png
--rw-rw-rw-   0        0        0       90 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/plus.png
--rw-rw-rw-   0        0        0     4463 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/pygments.css
--rw-rw-rw-   0        0        0    15987 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/searchtools.js
--rw-rw-rw-   0        0        0     4961 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/sidebar.js
--rw-rw-rw-   0        0        0    35168 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    12140 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/_static/underscore.js
--rw-rw-rw-   0        0        0    11852 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/develop.html
--rw-rw-rw-   0        0        0     2793 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/genindex.html
--rw-rw-rw-   0        0        0     8393 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/index.html
--rw-rw-rw-   0        0        0      721 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/objects.inv
--rw-rw-rw-   0        0        0     3318 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/search.html
--rw-rw-rw-   0        0        0    10761 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/searchindex.js
--rw-rw-rw-   0        0        0     7548 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/usersguide-app1.html
--rw-rw-rw-   0        0        0     4948 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/usersguide-app2.html
--rw-rw-rw-   0        0        0    13557 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/usersguide-ch1.html
--rw-rw-rw-   0        0        0    18436 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/usersguide-ch2.html
--rw-rw-rw-   0        0        0    12375 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/usersguide-ch3.html
--rw-rw-rw-   0        0        0     9144 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/usersguide-ch4.html
--rw-rw-rw-   0        0        0     8546 2019-12-25 12:24:22.000000 ViTables-3.0.2/vitables/htmldocs/usersguide-ch5.html
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:09.996137 ViTables-3.0.2/vitables/i18n/
--rw-rw-rw-   0        0        0    85074 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/i18n/vitables_es_ES.qm
--rw-rw-rw-   0        0        0    48083 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/i18n/vitables_ru_RU.qm
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.011758 ViTables-3.0.2/vitables/icons/
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.152350 ViTables-3.0.2/vitables/icons/16x16/
--rw-rw-rw-   0        0        0      842 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/application-exit.png
--rw-rw-rw-   0        0        0      177 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/array.png
--rw-rw-rw-   0        0        0      763 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/bookmark_add.png
--rw-rw-rw-   0        0        0      793 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/bookmarks.png
--rw-rw-rw-   0        0        0      206 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/carray.png
--rw-rw-rw-   0        0        0      717 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/configure.png
--rw-rw-rw-   0        0        0      606 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/delete_filters.png
--rw-rw-rw-   0        0        0      848 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/dialog-cancel.png
--rw-rw-rw-   0        0        0      601 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/dialog-ok.png
--rw-rw-rw-   0        0        0      678 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/document-close.png
--rw-rw-rw-   0        0        0      614 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/16x16/document-export.png
--rw-rw-rw-   0        0        0      609 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/16x16/document-import.png
--rw-rw-rw-   0        0        0      579 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/document-new.png
--rw-rw-rw-   0        0        0      697 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/document-open-recent.png
--rw-rw-rw-   0        0        0      531 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/document-open.png
--rw-rw-rw-   0        0        0      839 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/document-save-as.png
--rw-rw-rw-   0        0        0      233 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/earray.png
--rw-rw-rw-   0        0        0      485 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/edit-copy.png
--rw-rw-rw-   0        0        0      368 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/edit-cut.png
--rw-rw-rw-   0        0        0      641 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/edit-delete.png
--rw-rw-rw-   0        0        0      529 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/edit-paste.png
--rw-rw-rw-   0        0        0      245 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/edit-rename.png
--rw-rw-rw-   0        0        0      828 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/file_ro.png
--rw-rw-rw-   0        0        0     1125 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/file_rw.png
--rw-rw-rw-   0        0        0      321 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/16x16/filenode.png
--rw-rw-rw-   0        0        0      578 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/folder-new.png
--rw-rw-rw-   0        0        0      862 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/go-first-view.png
--rw-rw-rw-   0        0        0      570 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/go-next-view.png
--rw-rw-rw-   0        0        0      575 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/go-previous-view.png
--rw-rw-rw-   0        0        0      734 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/help-about.png
--rw-rw-rw-   0        0        0      684 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/help-contents.png
--rw-rw-rw-   0        0        0      769 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/image-missing.png
--rw-rw-rw-   0        0        0      503 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/link_array.png
--rw-rw-rw-   0        0        0      510 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/link_carray.png
--rw-rw-rw-   0        0        0      549 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/link_earray.png
--rw-rw-rw-   0        0        0      853 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/link_table.png
--rw-rw-rw-   0        0        0      502 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/link_vlarray.png
--rw-rw-rw-   0        0        0      332 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/list-remove.png
--rw-rw-rw-   0        0        0     1354 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/object.png
--rw-rw-rw-   0        0        0     1014 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/table.png
--rw-rw-rw-   0        0        0      161 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/vlarray.png
--rw-rw-rw-   0        0        0      187 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/vlstring.png
--rw-rw-rw-   0        0        0      791 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/zoom-in.png
--rw-rw-rw-   0        0        0      786 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/16x16/zoom-out.png
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.230456 ViTables-3.0.2/vitables/icons/22x22/
--rw-rw-rw-   0        0        0     1134 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/application-exit.png
--rw-rw-rw-   0        0        0     4063 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/bookmark_add.png
--rw-rw-rw-   0        0        0     1208 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/bookmarks.png
--rw-rw-rw-   0        0        0      450 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/dbfilters.png
--rw-rw-rw-   0        0        0      727 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/delete_filters.png
--rw-rw-rw-   0        0        0     1018 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/document-close.png
--rw-rw-rw-   0        0        0      873 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/document-new.png
--rw-rw-rw-   0        0        0      575 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/document-open-folder.png
--rw-rw-rw-   0        0        0      796 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/document-open.png
--rw-rw-rw-   0        0        0     1233 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/document-save-as.png
--rw-rw-rw-   0        0        0     1336 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/edit-clear-history.png
--rw-rw-rw-   0        0        0      515 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/edit-copy.png
--rw-rw-rw-   0        0        0      576 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/edit-cut.png
--rw-rw-rw-   0        0        0     1121 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/edit-delete.png
--rw-rw-rw-   0        0        0      771 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/edit-paste.png
--rw-rw-rw-   0        0        0     1227 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/file_ro.png
--rw-rw-rw-   0        0        0     1641 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/file_rw.png
--rw-rw-rw-   0        0        0      923 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/folder-new.png
--rw-rw-rw-   0        0        0      540 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/folder.png
--rw-rw-rw-   0        0        0     1220 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/go-first-view.png
--rw-rw-rw-   0        0        0      810 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/go-next-view.png
--rw-rw-rw-   0        0        0      817 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/go-previous-view.png
--rw-rw-rw-   0        0        0     1054 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/help-contents.png
--rw-rw-rw-   0        0        0      617 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/view-filter.png
--rw-rw-rw-   0        0        0     1283 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/view-refresh.png
--rw-rw-rw-   0        0        0     1191 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/zoom-in.png
--rw-rw-rw-   0        0        0     1173 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/22x22/zoom-out.png
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.246078 ViTables-3.0.2/vitables/icons/64x64/
--rw-rw-rw-   0        0        0     2453 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/64x64/preferences-desktop-theme.png
--rw-rw-rw-   0        0        0     5677 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/64x64/preferences-other.png
--rw-rw-rw-   0        0        0     4417 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/64x64/preferences-plugin.png
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.246078 ViTables-3.0.2/vitables/icons/mswindows/
--rw-rw-rw-   0        0        0     7406 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/mswindows/vitables.ico
--rw-rw-rw-   0        0        0     7406 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/mswindows/vitables_file.ico
--rw-rw-rw-   0        0        0     7406 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/mswindows/vtinstaller.ico
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.277321 ViTables-3.0.2/vitables/icons/unixapp/
--rw-rw-rw-   0        0        0      481 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables.desktop
--rw-rw-rw-   0        0        0     8871 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables.svg
--rw-rw-rw-   0        0        0     8444 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables_128x128.png
--rw-rw-rw-   0        0        0      867 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables_16x16.png
--rw-rw-rw-   0        0        0     1233 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables_22x22.png
--rw-rw-rw-   0        0        0     1912 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables_32x32.png
--rw-rw-rw-   0        0        0     2973 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables_48x48.png
--rw-rw-rw-   0        0        0     4440 2019-12-11 19:06:17.000000 ViTables-3.0.2/vitables/icons/unixapp/vitables_64x64.png
--rw-rw-rw-   0        0        0    36049 2019-12-13 15:21:35.000000 ViTables-3.0.2/vitables/icons/vitables_logo.png
--rw-rw-rw-   0        0        0    26609 2019-12-13 15:19:43.000000 ViTables-3.0.2/vitables/icons/vitables_logo.svg
--rw-rw-rw-   0        0        0      828 2017-09-07 19:56:00.000000 ViTables-3.0.2/vitables/icons/vitables_wm.png
--rw-rw-rw-   0        0        0     8226 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/logger.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.308567 ViTables-3.0.2/vitables/nodeprops/
--rw-rw-rw-   0        0        0     1017 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/__init__.py
--rw-rw-rw-   0        0        0    15551 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/nodeprops/attr_prop_dlg.ui
--rw-rw-rw-   0        0        0    11774 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/attreditor.py
--rw-rw-rw-   0        0        0    18137 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/attrpropdlg.py
--rw-rw-rw-   0        0        0    10603 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/nodeprops/group_prop_page.ui
--rw-rw-rw-   0        0        0     3008 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/grouppropdlg.py
--rw-rw-rw-   0        0        0     5675 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/groupproppage.py
--rw-rw-rw-   0        0        0    14707 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/nodeprops/leaf_prop_page.ui
--rw-rw-rw-   0        0        0     2988 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/leafpropdlg.py
--rw-rw-rw-   0        0        0     6110 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/leafproppage.py
--rw-rw-rw-   0        0        0     8124 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/nodeprops/link_prop_dlg.ui
--rw-rw-rw-   0        0        0     3017 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/linkpropdlg.py
--rw-rw-rw-   0        0        0     9071 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/nodeprops/nodeinfo.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.324189 ViTables-3.0.2/vitables/plugins/
--rw-rw-rw-   0        0        0      884 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/__init__.py
--rw-rw-rw-   0        0        0     7891 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/plugins/about_page.ui
--rw-rw-rw-   0        0        0      724 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/plugins/aboutpage.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.324189 ViTables-3.0.2/vitables/plugins/columnorg/
--rw-rw-rw-   0        0        0      852 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/columnorg/__init__.py
--rw-rw-rw-   0        0        0    22028 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/columnorg/columnar_org.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.339815 ViTables-3.0.2/vitables/plugins/dbstreesort/
--rw-rw-rw-   0        0        0      853 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/dbstreesort/__init__.py
--rw-rw-rw-   0        0        0     4989 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/dbstreesort/aboutpage.py
--rw-rw-rw-   0        0        0     8658 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/dbstreesort/dbs_tree_sort.py
--rw-rw-rw-   0        0        0     8237 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/plugins/dbstreesort/dbs_tree_sort_page.ui
--rw-rw-rw-   0        0        0       36 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/plugins/dbstreesort/sorting_algorithm.ini
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.355426 ViTables-3.0.2/vitables/plugins/timeseries/
--rw-rw-rw-   0        0        0      851 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/timeseries/__init__.py
--rw-rw-rw-   0        0        0     4970 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/plugins/timeseries/aboutpage.py
--rw-rw-rw-   0        0        0       29 2019-12-23 15:35:10.000000 ViTables-3.0.2/vitables/plugins/timeseries/time_format.ini
--rw-rw-rw-   0        0        0    18167 2019-12-23 12:25:20.000000 ViTables-3.0.2/vitables/plugins/timeseries/time_series.py
--rw-rw-rw-   0        0        0    10786 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/plugins/timeseries/timeformatter_page.ui
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.371051 ViTables-3.0.2/vitables/preferences/
--rw-rw-rw-   0        0        0      952 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/preferences/__init__.py
--rw-rw-rw-   0        0        0     2255 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/preferences/cfgexception.py
--rw-rw-rw-   0        0        0     3912 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/preferences/pluginsloader.py
--rw-rw-rw-   0        0        0    17247 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/preferences/preferences.py
--rw-rw-rw-   0        0        0    14230 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/preferences/settings_dlg.ui
--rw-rw-rw-   0        0        0    23276 2019-12-25 11:48:16.000000 ViTables-3.0.2/vitables/preferences/vtconfig.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.386669 ViTables-3.0.2/vitables/queries/
--rw-rw-rw-   0        0        0      925 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/queries/__init__.py
--rw-rw-rw-   0        0        0     8151 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/queries/query.py
--rw-rw-rw-   0        0        0    12206 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/queries/query_dlg.ui
--rw-rw-rw-   0        0        0    16012 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/queries/querydlg.py
--rw-rw-rw-   0        0        0    12749 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/queries/querymgr.py
--rw-rw-rw-   0        0        0     6741 2019-12-13 13:36:39.000000 ViTables-3.0.2/vitables/start.py
--rw-rw-rw-   0        0        0    20919 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/utils.py
--rw-rw-rw-   0        0        0    54673 2019-12-25 11:30:16.000000 ViTables-3.0.2/vitables/vtapp.py
--rw-rw-rw-   0        0        0    43715 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vtgui.py
--rw-rw-rw-   0        0        0     1486 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vtsite.py
--rw-rw-rw-   0        0        0     2542 2019-12-13 15:27:58.000000 ViTables-3.0.2/vitables/vtsplash.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.417912 ViTables-3.0.2/vitables/vttables/
--rw-rw-rw-   0        0        0      972 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/__init__.py
--rw-rw-rw-   0        0        0    10306 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/buffer.py
--rw-rw-rw-   0        0        0     6042 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/datasheet.py
--rw-rw-rw-   0        0        0    10414 2019-12-23 12:15:04.000000 ViTables-3.0.2/vitables/vttables/df_model.py
--rw-rw-rw-   0        0        0     4370 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/filenodebuffer.py
--rw-rw-rw-   0        0        0     3851 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/leaf_delegate.py
--rw-rw-rw-   0        0        0     8912 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/leaf_model.py
--rw-rw-rw-   0        0        0    31779 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/leaf_view.py
--rw-rw-rw-   0        0        0     3132 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vttables/scrollbar.py
-drwxrwxrwx   0        0        0        0 2019-12-25 14:16:10.449155 ViTables-3.0.2/vitables/vtwidgets/
--rw-rw-rw-   0        0        0      933 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vtwidgets/__init__.py
--rw-rw-rw-   0        0        0     1805 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/vtwidgets/nodename_dlg.ui
--rw-rw-rw-   0        0        0     4215 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vtwidgets/nodenamedlg.py
--rw-rw-rw-   0        0        0     1795 2018-09-29 14:35:58.000000 ViTables-3.0.2/vitables/vtwidgets/rename_dlg.ui
--rw-rw-rw-   0        0        0     8047 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vtwidgets/renamedlg.py
--rw-rw-rw-   0        0        0    11411 2019-12-13 13:36:40.000000 ViTables-3.0.2/vitables/vtwidgets/zoom_cell.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vitables-3.0.3/ANNOUNCE.txt
+-rw-r--r--   0        0        0    77337 2020-02-02 00:00:00.000000 vitables-3.0.3/ChangeLog.txt
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 vitables-3.0.3/INSTALL.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 vitables-3.0.3/VERSION
+-rw-r--r--   0        0        0    37263 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/LICENSE.html
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/__main__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/filenodeutils.py
+-rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/logger.py
+-rwxr-xr-x   0        0        0     6741 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/start.py
+-rw-r--r--   0        0        0    20935 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/utils.py
+-rw-r--r--   0        0        0    54696 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtapp.py
+-rw-r--r--   0        0        0    43612 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtgui.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtsite.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtsplash.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/calculator/__init__.py
+-rw-r--r--   0        0        0    16842 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/calculator/calculator.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/calculator/calculator.ui
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/calculator/calculator_dlg.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/calculator/evaluator.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/__init__.py
+-rw-r--r--   0        0        0    14890 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/csvutils.py
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/export_csv.py
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/import_csv.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/array.csv
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/arrayND.csv
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/array_float.csv
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/array_strings.csv
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/column.csv
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/columnND.csv
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/row.csv
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/rowND.csv
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/table.csv
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/table_header.csv
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/table_integers.csv
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/csv/examples/table_strings.csv
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/docbrowser/__init__.py
+-rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/docbrowser/bookmarksdlg.py
+-rw-r--r--   0        0        0    14862 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/docbrowser/browsergui.py
+-rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/docbrowser/helpbrowser.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/__init__.py
+-rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/dbdoc.py
+-rw-r--r--   0        0        0    45488 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/dbstreemodel.py
+-rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/dbstreeview.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/groupnode.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/leafnode.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/linknode.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/nodeitemdelegate.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/rootgroupnode.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/tlink_editor.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/h5db/tnode_editor.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.buildinfo
+-rw-r--r--   0        0        0    13553 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/develop.html
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/genindex.html
+-rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/index.html
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/objects.inv
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/search.html
+-rw-r--r--   0        0        0    17633 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/searchindex.js
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/usersguide-app1.html
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/usersguide-app2.html
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/usersguide-ch1.html
+-rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/usersguide-ch2.html
+-rw-r--r--   0        0        0    13034 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/usersguide-ch3.html
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/usersguide-ch4.html
+-rw-r--r--   0        0        0     9067 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/usersguide-ch5.html
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/develop.doctree
+-rw-r--r--   0        0        0   267780 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    20434 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/index.doctree
+-rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/usersguide-app1.doctree
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/usersguide-app2.doctree
+-rw-r--r--   0        0        0    24677 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/usersguide-ch1.doctree
+-rw-r--r--   0        0        0    40266 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/usersguide-ch2.doctree
+-rw-r--r--   0        0        0    23607 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/usersguide-ch3.doctree
+-rw-r--r--   0        0        0    13569 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/usersguide-ch4.doctree
+-rw-r--r--   0        0        0    22063 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/.doctrees/usersguide-ch5.doctree
+-rw-r--r--   0        0        0    51210 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/browseDataset.png
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/editingUserAttrs.png
+-rw-r--r--   0        0        0    64708 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/groupCreation.png
+-rw-r--r--   0        0        0    37498 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/helpBrowser.png
+-rw-r--r--   0        0        0    77227 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/mainWindow.png
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/newFilteredTable.png
+-rw-r--r--   0        0        0    11087 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/propertiesDlg.png
+-rw-r--r--   0        0        0    47789 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/title_page_plain.png
+-rw-r--r--   0        0        0    20941 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/treeSymbols.png
+-rw-r--r--   0        0        0    64021 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_images/zoomingCells.png
+-rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/classic.css
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/default.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/doctools.js
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/plus.png
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/searchtools.js
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/sidebar.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/htmldocs/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    85074 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/i18n/vitables_es_ES.qm
+-rw-r--r--   0        0        0    48083 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/i18n/vitables_ru_RU.qm
+-rw-r--r--   0        0        0    36049 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/vitables_logo.png
+-rw-r--r--   0        0        0    26609 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/vitables_logo.svg
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/vitables_wm.png
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/application-exit.png
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/array.png
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/bookmark_add.png
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/bookmarks.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/carray.png
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/configure.png
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/delete_filters.png
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/dialog-cancel.png
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/dialog-ok.png
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/document-close.png
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/document-export.png
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/document-import.png
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/document-new.png
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/document-open-recent.png
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/document-open.png
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/document-save-as.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/earray.png
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/edit-copy.png
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/edit-cut.png
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/edit-delete.png
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/edit-paste.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/edit-rename.png
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/file_ro.png
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/file_rw.png
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/filenode.png
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/folder-new.png
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/go-first-view.png
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/go-next-view.png
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/go-previous-view.png
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/help-about.png
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/help-contents.png
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/image-missing.png
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/link_array.png
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/link_carray.png
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/link_earray.png
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/link_table.png
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/link_vlarray.png
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/list-remove.png
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/object.png
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/table.png
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/vlarray.png
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/vlstring.png
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/zoom-in.png
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/16x16/zoom-out.png
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/application-exit.png
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/bookmark_add.png
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/bookmarks.png
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/dbfilters.png
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/delete_filters.png
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/document-close.png
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/document-new.png
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/document-open-folder.png
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/document-open.png
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/document-save-as.png
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/edit-clear-history.png
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/edit-copy.png
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/edit-cut.png
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/edit-delete.png
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/edit-paste.png
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/file_ro.png
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/file_rw.png
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/folder-new.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/folder.png
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/go-first-view.png
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/go-next-view.png
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/go-previous-view.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/help-contents.png
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/view-filter.png
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/view-refresh.png
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/zoom-in.png
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/22x22/zoom-out.png
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/64x64/preferences-desktop-theme.png
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/64x64/preferences-other.png
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/64x64/preferences-plugin.png
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/mswindows/vitables.ico
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/mswindows/vitables_file.ico
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/mswindows/vtinstaller.ico
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables.desktop
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables.svg
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables_128x128.png
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables_16x16.png
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables_22x22.png
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables_32x32.png
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables_48x48.png
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/icons/unixapp/vitables_64x64.png
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/__init__.py
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/attr_prop_dlg.ui
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/attreditor.py
+-rw-r--r--   0        0        0    18137 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/attrpropdlg.py
+-rw-r--r--   0        0        0    10603 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/group_prop_page.ui
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/grouppropdlg.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/groupproppage.py
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/leaf_prop_page.ui
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/leafpropdlg.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/leafproppage.py
+-rw-r--r--   0        0        0     8124 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/link_prop_dlg.ui
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/linkpropdlg.py
+-rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/nodeprops/nodeinfo.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/__init__.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/about_page.ui
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/aboutpage.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/columnorg/__init__.py
+-rw-r--r--   0        0        0    22028 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/columnorg/columnar_org.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/columnorg/icons/object-group.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/columnorg/icons/object-ungroup.png
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/dbstreesort/__init__.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/dbstreesort/aboutpage.py
+-rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/dbstreesort/dbs_tree_sort.py
+-rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/dbstreesort/dbs_tree_sort_page.ui
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/dbstreesort/sorting_algorithm.ini
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/timeseries/__init__.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/timeseries/aboutpage.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/timeseries/time_format.ini
+-rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/timeseries/time_series.py
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/plugins/timeseries/timeformatter_page.ui
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/preferences/__init__.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/preferences/cfgexception.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/preferences/pluginsloader.py
+-rw-r--r--   0        0        0    17247 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/preferences/preferences.py
+-rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/preferences/settings_dlg.ui
+-rw-r--r--   0        0        0    23316 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/preferences/vtconfig.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/queries/__init__.py
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/queries/query.py
+-rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/queries/query_dlg.ui
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/queries/querydlg.py
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/queries/querymgr.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/__init__.py
+-rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/buffer.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/datasheet.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/df_model.py
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/filenodebuffer.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/leaf_delegate.py
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/leaf_model.py
+-rw-r--r--   0        0        0    31779 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/leaf_view.py
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vttables/scrollbar.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtwidgets/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtwidgets/nodename_dlg.ui
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtwidgets/nodenamedlg.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtwidgets/rename_dlg.ui
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtwidgets/renamedlg.py
+-rw-r--r--   0        0        0    11411 2020-02-02 00:00:00.000000 vitables-3.0.3/vitables/vtwidgets/zoom_cell.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vitables-3.0.3/.gitignore
+-rw-r--r--   0        0        0    35975 2020-02-02 00:00:00.000000 vitables-3.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 vitables-3.0.3/README.md
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 vitables-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 vitables-3.0.3/PKG-INFO
```

### Comparing `ViTables-3.0.2/ANNOUNCE.txt` & `vitables-3.0.3/ANNOUNCE.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 =========================
-Announcing ViTables 3.0.2
+Announcing ViTables 3.0.3
 =========================
 
 After another long period retired from development activities I'm happy to come
-back and present ViTables 3.0.2, the latest release of this viewer for
+back and present ViTables 3.0.3, the latest release of this viewer for
 PyTables/HDF5 files. Definitely this release wouldn't have been possible without
 the invaluable help of a bunch of contributors so THANKS to all of them.
 
 As it happens with the entire PyTables family, the main strength of ViTables
 is its ability to manage really large datasets in a fast and comfortable
 manner. For example, with ViTables you can open a table with one thousand
 million rows in a few tenths of second, with very low memory requirements.
@@ -34,12 +34,12 @@
 and see what is available.
 
 Share your experience
 ---------------------
 I'm very interested in your feedback about ViTables. Please send your
 opinions, suggestions, bugs, etc. to the ViTables Users Group at
 
-http://tech.groups.yahoo.com/group/vitables-users.
+https://groups.google.com/forum/#!forum/vitables-users.
 
 Thank you!
 
 Enjoy Data with ViTables, the troll of the PyTables family!
```

### Comparing `ViTables-3.0.2/ChangeLog.txt` & `vitables-3.0.3/ChangeLog.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 ViTables ChangeLog
 ==================
+** August 04, 2023 **
+Users Guide and README.md updated.
+
+pyproject.toml updated in order to package the users guide too.
+
+** August 02, 2023 **
+Updated the script that generates the users guide.
+
+Users Guide updated.
+
+** July 31, 2023 **
+Package build system changed from setuptools to flit.
+
+** July 30, 2023 **
+setup.py and setup.cfg files changed to use the new README.md file.
+
+** July 20, 2023 **
+Support PyQt6, this is useful for mac users who cant install
+PyQt5.
+
+** January 03, 2019 **
+Added script to automatically generate the Users Guide.
+
+** December 31, 2019 **
+setup.py slightly improved.
+
 ** December 25, 2019 **
 Fixed the Xmas day bug in vtapp.py.
 
 Fixed a syntax error in the setup.py description that caused PyPI to refuse
 the package upload.
 
 ** December 24, 2019 **
```

### Comparing `ViTables-3.0.2/INSTALL.txt` & `vitables-3.0.3/INSTALL.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 System requirements
 -------------------
-ViTables 3.0.2 has been tested against the latest versions of Python 3,
+ViTables 3.0.3 has been tested against the latest versions of Python 3,
 PyTables and PyQt. You can try other versions at your own risk :).
 
 Installation on a conda environment
 -----------------------------------
 Using conda you should be able to run vitables on any system, let it
 be linux, mac or windows. The following are instructions for linux-like
 systems.
@@ -27,15 +27,15 @@
 
   $ pip install ViTables
 
 Alternatively, you can download the binary package from the download area
 (see vitables.org/Downloads for details), go to the directory where you have
 downloaded the file and issue the command::
 
-  $ pip install ViTables-3.0.2-py3-none-any.whl
+  $ pip install ViTables-3.0.3-py3-none-any.whl
 
 This should install the ViTables wheel. If you experience problems installing
 the binary package then you can install from sources (provided your system fulfills
 the requirements listed in the above section). Just download the tarball from
 the download area, uncompress it, change to the distribution directory and execute
 
  $ python setup.py install
```

### Comparing `ViTables-3.0.2/LICENSE.txt` & `vitables-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/LICENSE.html` & `vitables-3.0.3/vitables/LICENSE.html`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/__init__.py` & `vitables-3.0.3/vitables/plugins/dbstreesort/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-
-#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
-#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
-#
-#       This program is free software: you can redistribute it and/or modify
-#       it under the terms of the GNU General Public License as published by
-#       the Free Software Foundation, either version 3 of the License, or
-#       (at your option) any later version.
-#
-#       This program is distributed in the hope that it will be useful,
-#       but WITHOUT ANY WARRANTY; without even the implied warranty of
-#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#       GNU General Public License for more details.
-#
-#       You should have received a copy of the GNU General Public License
-#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#       Author:  Vicent Mas - vmas@vitables.org
-
-__version__ = '3.0.2'
-__all__ = ["docbrowser", "h5db", "logger", "nodeprops", "plugins",
-           "queries", "preferences", "vttables", "vtwidgets",
-           "utils", "vtsite", "vtapp", "vtgui", "vtsplash"]
+
+#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
+#
+#       This program is free software: you can redistribute it and/or modify
+#       it under the terms of the GNU General Public License as published by
+#       the Free Software Foundation, either version 3 of the License, or
+#       (at your option) any later version.
+#
+#       This program is distributed in the hope that it will be useful,
+#       but WITHOUT ANY WARRANTY; without even the implied warranty of
+#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#       GNU General Public License for more details.
+#
+#       You should have received a copy of the GNU General Public License
+#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+#       Author:  Vicent Mas - vmas@vitables.org
+
+__all__ = ['aboutpage', 'dbs_tree_sort']
```

### Comparing `ViTables-3.0.2/vitables/calculator/calculator.py` & `vitables-3.0.3/vitables/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/calculator/calculator.ui` & `vitables-3.0.3/vitables/calculator/calculator.ui`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/calculator/calculator_dlg.py` & `vitables-3.0.3/vitables/calculator/calculator_dlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/csv/__init__.py` & `vitables-3.0.3/vitables/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/csv/csvutils.py` & `vitables-3.0.3/vitables/csv/csvutils.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/csv/export_csv.py` & `vitables-3.0.3/vitables/csv/export_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         export_info = self.getExportInfo(is_table)
         if export_info is None:
             return
         else:
             filepath, add_header = export_info
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             with open(filepath, 'ab') as out_handler:
                 if add_header:
                     from functools import reduce
                     header = reduce(lambda x, y: '{0}, {1}'.format(x, y),
                                     leaf.colnames)
                     # To be consistent with numpy.savetxt use \n line breaks
                     out_handler.write(bytearray(header + '\n', 'UTF-8'))
@@ -276,20 +276,20 @@
                 nrows = leaf.nrows
                 if chunk_size > nrows:
                     chunk_size = nrows
                 # Behavior of np.divide in Python 2 and Python 3 is different so
                 # we must explicitly ensure we get an integer
                 nchunks = numpy.floor_divide(nrows, chunk_size)
                 for i in numpy.arange(0, nchunks + 1):
-                    QtWidgets.qApp.processEvents()
+                    QtWidgets.QApplication.processEvents()
                     cstart = chunk_size * i
                     if cstart >= nrows:
                         break
                     cstop = cstart + chunk_size
                     if cstop > nrows:
                         cstop = nrows
                     numpy.savetxt(out_handler, leaf.read(cstart, cstop, 1),
                                   fmt='%s', delimiter=',')
         except OSError:
             vitables.utils.formatExceptionInfo()
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
```

### Comparing `ViTables-3.0.2/vitables/csv/import_csv.py` & `vitables-3.0.3/vitables/csv/import_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,16 +262,16 @@
         kind = 'Table'
         filepath = self.csvFilepath(kind)
         if filepath is None:
             return
 
         # Import the CSV content
         try:
-            QtWidgets.qApp.processEvents()
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.processEvents()
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             input_handler = open(filepath, 'r+')
             try:
                 (nrows, descr, has_header) = csvutils.tableInfo(input_handler)
             except Exception as inst:
                 print(traceback.format_exc())
 
             # Create the dataset
@@ -302,15 +302,15 @@
                 del idata
                 buf = read_fh(buf_size)
             dbdoc.h5file.flush()
             self.updateTree(dbdoc.filepath)
         except:
             vitables.utils.formatExceptionInfo()
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
             input_handler.close()
 
     def csv2EArray(self):
         """Import a plain `CSV` file into a `tables.EArray` object.
 
         This is a slot method. See :meth:`addEntry` method for details.
         """
@@ -318,16 +318,16 @@
         kind = 'EArray'
         filepath = self.csvFilepath(kind)
         if filepath is None:
             return
 
         # Import the CSV content
         try:
-            QtWidgets.qApp.processEvents()
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.processEvents()
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             chunk_size = 10000
             input_handler = open(filepath, 'r+')
             (nrows, atom, array_shape) = csvutils.earrayInfo(input_handler)
 
             # Create the dataset
             dbdoc = self.createDestFile(filepath)
             if dbdoc is None:
@@ -355,15 +355,15 @@
             dbdoc.h5file.flush()
             self.updateTree(dbdoc.filepath)
         except ValueError:
             log.error(TYPE_ERROR)
         except:
             vitables.utils.formatExceptionInfo()
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
             input_handler.close()
 
     def csv2CArray(self):
         """Import a plain `CSV` file into a `tables.CArray` object.
 
         This is a slot method. See :meth:`addEntry` method for details.
         """
@@ -371,16 +371,16 @@
         kind = 'CArray'
         filepath = self.csvFilepath(kind)
         if filepath is None:
             return
 
         # Import the CSV content
         try:
-            QtWidgets.qApp.processEvents()
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.processEvents()
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             chunk_size = 10000
             input_handler = open(filepath, 'r+')
             (atom, array_shape) = csvutils.carrayInfo(input_handler)
 
             # Create the dataset
             dbdoc = self.createDestFile(filepath)
             if dbdoc is None:
@@ -411,15 +411,15 @@
             dbdoc.h5file.flush()
             self.updateTree(dbdoc.filepath)
         except ValueError:
             log.error(TYPE_ERROR)
         except:
             vitables.utils.formatExceptionInfo()
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
             input_handler.close()
 
     def csv2Array(self):
         """Import a plain `CSV` file into a `tables.Array` object.
 
         This is a slot method. See :meth:`addEntry` method for details.
         """
@@ -427,16 +427,16 @@
         kind = 'Array'
         filepath = self.csvFilepath(kind)
         if filepath is None:
             return
 
         # Import the CSV content
         try:
-            QtWidgets.qApp.processEvents()
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.processEvents()
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             # The dtypes are determined by the contents of each column
             # Multidimensional columns will have string datatype
             data = numpy.genfromtxt(filepath, delimiter=',', dtype=None)
         except TypeError:
             data = None
             dbdoc = None
             log.error(TYPE_ERROR)
@@ -454,8 +454,8 @@
                 self.updateTree(dbdoc.filepath)
             except TypeError:
                 log.error(TYPE_ERROR)
             except tables.NodeError:
                 vitables.utils.formatExceptionInfo()
         finally:
             del data
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
```

### Comparing `ViTables-3.0.2/vitables/docbrowser/__init__.py` & `vitables-3.0.3/vitables/docbrowser/__init__.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/docbrowser/bookmarksdlg.py` & `vitables-3.0.3/vitables/docbrowser/bookmarksdlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/docbrowser/browsergui.py` & `vitables-3.0.3/vitables/docbrowser/browsergui.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/docbrowser/helpbrowser.py` & `vitables-3.0.3/vitables/docbrowser/helpbrowser.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/filenodeutils.py` & `vitables-3.0.3/vitables/filenodeutils.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/__init__.py` & `vitables-3.0.3/vitables/h5db/__init__.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/dbdoc.py` & `vitables-3.0.3/vitables/h5db/dbdoc.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/dbstreemodel.py` & `vitables-3.0.3/vitables/h5db/dbstreemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         :Parameters:
 
         - `filepath`: the full path of the file being created.
         - `is_tmp_db`: True if the `DBDoc` is tied to the temporary database
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(
+            QtWidgets.QApplication.setOverrideCursor(
                 QtGui.QCursor(QtCore.Qt.WaitCursor))
             # Create the dbdoc
             try:
                 db_doc = dbdoc.DBDoc(filepath, 'w', is_tmp_db)
             except (tables.NodeError, OSError):
                 log.error(
                     translate('DBsTreeModel',
@@ -307,15 +307,15 @@
                                                is_tmp_db)
             self.fdelta = frozenset([root])
             self.gdelta = frozenset([])
             self.ldelta = frozenset([])
             self.links_delta = frozenset([])
             self.insertRows(0, 1)
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
         return db_doc
 
     def __createTempDB(self):
         """
         Create a temporary database where filtered tables will be stored.
 
         The database will have a hidden group where cut nodes can be
@@ -338,15 +338,15 @@
         Delete the selected node from the model and from the database
         where it lives.
 
         :Parameter index: the index of the selected node
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             node = self.nodeFromIndex(index)
             # Deletes the node from the database
             node.editor().delete(node.nodepath)
 
             # Deletes the node from the tree of databases model/view
             parent = self.parent(index)
             position = node.row()
@@ -359,43 +359,43 @@
                 if self.ccni['is_copied'] and \
                         (self.ccni['filepath'] == node.filepath) and \
                         self.ccni['nodepath'].startswith(node.nodepath):
                     self.ccni = {}
             except KeyError:
                 pass
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
 
     def copy_node(self, index):
         """Mark a node from the tree of databases view as copied.
 
         :Parameter index: the index of the selected node
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             node = self.nodeFromIndex(index)
             self.ccni = {'is_copied': True,
                          'nodename': node.name,
                          'filepath': node.filepath,
                          'nodepath': node.nodepath,
                          'target': getattr(node, 'target', None)}
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
 
     def cutNode(self, index):
         """Cut a `tables.Node`.
 
         The cut node is stored in a hidden group of its database.
 
         :Parameter index: the index of the selected node
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             node = self.nodeFromIndex(index)
             self.ccni = {'is_copied': False,
                          'nodename': node.name,
                          'filepath': node.filepath,
                          'nodepath': node.nodepath,
                          'target': getattr(node, 'target', None)}
 
@@ -410,30 +410,30 @@
             # else the parent group will be selected
             if position == 0:
                 current = parent
             else:
                 current = self.index(position - 1, 0, parent)
             self.vtgui.dbs_tree_view.selectNode(current)
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
 
     def pasteNode(self, index, childname, overwrite=False):
         """Paste a tables.Node.
 
         Paste the last copied/cut node under the currently selected group.
 
         :Parameters:
 
         - `index`: the index of the selected node (the parent group)
         - `childname`: the name of the node being pasted
         - `overwrite`: True if a node is being overwritten
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             parent = self.nodeFromIndex(index)
 
             # If the overwritten node (if any) exists in the tree of
             # databases view then delete it
             if overwrite:
                 self.overwriteNode(parent, index, childname)
 
@@ -450,15 +450,15 @@
             # Paste the node in the tree of databases model/view
             self.lazyAddChildren(index)
             parent.updated = True
 
             # Select the pasted node
             self.selectIndex(index, childname)
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
 
     def copiedNode(self):
         """The tables.Node currently copied/cut.
         """
 
         src_filepath = self.ccni['filepath']
         if self.ccni['is_copied']:
@@ -477,15 +477,15 @@
 
         - `index`: the index of the parent node
         - `childname`: the name of the group being created
         - `overwrite`: True if a node is being overwritten
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             parent = self.nodeFromIndex(index)
             # If the overwritten node (if any) exists in the tree of
             # databases view then delete it
             if overwrite:
                 self.overwriteNode(parent, index, childname)
 
             # Create the group in the PyTables database
@@ -494,28 +494,28 @@
             # Paste the node in the tree of databases model/view
             self.lazyAddChildren(index)
             parent.updated = True
 
             # Select the pasted node
             self.selectIndex(index, childname)
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
 
     def rename_node(self, index, new_name, overwrite=False):
         """Rename a node.
 
         :Parameters:
 
         - `index`: the index of the node being renamed
         - `new_name`: the new name of the node
         - `overwrite`: True if a node is being overwritten
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             node = self.nodeFromIndex(index)
             initial_nodepath = node.nodepath
             parent_index = self.parent(index)
             parent = self.nodeFromIndex(parent_index)
             if overwrite:
                 self.overwriteNode(parent, parent_index, new_name)
 
@@ -530,15 +530,15 @@
             try:
                 if self.ccni['filepath'] == node.filepath:
                     if self.ccni['nodepath'].startswith(initial_nodepath):
                         self.ccni = {}
             except KeyError:
                 pass
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
 
     def updateDBTree(self, index, new_name, node):
         """
         After renaming a PyTables node update the tree of databases model/view.
 
         The following data must be updated:
 
@@ -591,15 +591,15 @@
           - `src_filepath`: the full path of the source database
           - `childpath`: the full path of the node being moved
           - `parent_index`: the model index of the new parent group
           - `overwrite`: True if a node is being overwritten
         """
 
         try:
-            QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+            QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
             parent_node = self.nodeFromIndex(parent_index)
             # full path of the destination database and new parent
             dst_filepath = parent_node.filepath
             parentpath = parent_node.nodepath
 
             #
             # Check if the nodename is already in use
@@ -620,15 +620,15 @@
             if hasattr(pt_node, 'target'):
                 editor = tlink_editor.TLinkEditor(db_doc)
             else:
                 editor = tnode_editor.TNodeEditor(db_doc)
             movedname = editor.move(childpath, self.getDBDoc(dst_filepath),
                                     parentpath, nodename)
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
             return movedname
 
     def validateNodename(self, src_filepath, childpath, dst_filepath,
                          parentpath):
         """
 
         :Parameters:
```

### Comparing `ViTables-3.0.2/vitables/h5db/dbstreeview.py` & `vitables-3.0.3/vitables/h5db/dbstreeview.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/groupnode.py` & `vitables-3.0.3/vitables/h5db/groupnode.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/leafnode.py` & `vitables-3.0.3/vitables/h5db/leafnode.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/linknode.py` & `vitables-3.0.3/vitables/h5db/linknode.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/nodeitemdelegate.py` & `vitables-3.0.3/vitables/h5db/nodeitemdelegate.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/rootgroupnode.py` & `vitables-3.0.3/vitables/h5db/rootgroupnode.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/tlink_editor.py` & `vitables-3.0.3/vitables/h5db/tlink_editor.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/h5db/tnode_editor.py` & `vitables-3.0.3/vitables/h5db/tnode_editor.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/browseDataset.png` & `vitables-3.0.3/vitables/htmldocs/_images/browseDataset.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/editingUserAttrs.png` & `vitables-3.0.3/vitables/htmldocs/_images/editingUserAttrs.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/groupCreation.png` & `vitables-3.0.3/vitables/htmldocs/_images/groupCreation.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/helpBrowser.png` & `vitables-3.0.3/vitables/htmldocs/_images/helpBrowser.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/mainWindow.png` & `vitables-3.0.3/vitables/htmldocs/_images/mainWindow.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/newFilteredTable.png` & `vitables-3.0.3/vitables/htmldocs/_images/newFilteredTable.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/propertiesDlg.png` & `vitables-3.0.3/vitables/htmldocs/_images/propertiesDlg.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/title_page_plain.png` & `vitables-3.0.3/vitables/htmldocs/_images/title_page_plain.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/treeSymbols.png` & `vitables-3.0.3/vitables/htmldocs/_images/treeSymbols.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_images/zoomingCells.png` & `vitables-3.0.3/vitables/htmldocs/_images/zoomingCells.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/htmldocs/_static/searchtools.js` & `vitables-3.0.3/vitables/htmldocs/_static/searchtools.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,531 +1,577 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2019 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
+"use strict";
 
-if (!Scorer) {
-    /**
-     * Simple result scoring code.
-     */
+/**
+ * Simple result scoring code.
+ */
+if (typeof Scorer === "undefined") {
     var Scorer = {
         // Implement the following function to further tweak the score for each result
-        // The function takes a result array [filename, title, anchor, descr, score]
+        // The function takes a result array [docname, title, anchor, descr, score, filename]
         // and returns the new score.
         /*
-        score: function(result) {
-          return result[4];
+        score: result => {
+          const [docname, title, anchor, descr, score, filename] = result
+          return score
         },
         */
 
         // query matches the full name of an object
         objNameMatch: 11,
         // or matches in the last dotted part of the object name
         objPartialMatch: 6,
         // Additive scores depending on the priority of the object
         objPrio: {
             0: 15, // used to be importantResults
             1: 5, // used to be objectResults
-            2: -5
-        }, // used to be unimportantResults
+            2: -5, // used to be unimportantResults
+        },
         //  Used when the priority is not in the mapping.
         objPrioDefault: 0,
 
         // query found in title
         title: 15,
         partialTitle: 7,
         // query found in terms
         term: 5,
-        partialTerm: 2
+        partialTerm: 2,
     };
 }
 
-if (!splitQuery) {
-    function splitQuery(query) {
-        return query.split(/\s+/);
+const _removeChildren = (element) => {
+    while (element && element.lastChild) element.removeChild(element.lastChild);
+};
+
+/**
+ * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
+ */
+const _escapeRegExp = (string) =>
+    string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
+
+const _displayItem = (item, searchTerms) => {
+    const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
+    const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
+    const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
+    const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
+    const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
+
+    const [docName, title, anchor, descr, score, _filename] = item;
+
+    let listItem = document.createElement("li");
+    let requestUrl;
+    let linkUrl;
+    if (docBuilder === "dirhtml") {
+        // dirhtml builder
+        let dirname = docName + "/";
+        if (dirname.match(/\/index\/$/))
+            dirname = dirname.substring(0, dirname.length - 6);
+        else if (dirname === "index/") dirname = "";
+        requestUrl = docUrlRoot + dirname;
+        linkUrl = requestUrl;
+    } else {
+        // normal html builders
+        requestUrl = docUrlRoot + docName + docFileSuffix;
+        linkUrl = docName + docLinkSuffix;
+    }
+    let linkEl = listItem.appendChild(document.createElement("a"));
+    linkEl.href = linkUrl + anchor;
+    linkEl.dataset.score = score;
+    linkEl.innerHTML = title;
+    if (descr)
+        listItem.appendChild(document.createElement("span")).innerHTML =
+        " (" + descr + ")";
+    else if (showSearchSummary)
+        fetch(requestUrl)
+        .then((responseData) => responseData.text())
+        .then((data) => {
+            if (data)
+                listItem.appendChild(
+                    Search.makeSearchSummary(data, searchTerms)
+                );
+        });
+    Search.output.appendChild(listItem);
+};
+const _finishSearch = (resultCount) => {
+    Search.stopPulse();
+    Search.title.innerText = _("Search Results");
+    if (!resultCount)
+        Search.status.innerText = Documentation.gettext(
+            "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
+        );
+    else
+        Search.status.innerText = _(
+            `Search finished, found ${resultCount} page(s) matching the search query.`
+        );
+};
+const _displayNextItem = (
+    results,
+    resultCount,
+    searchTerms
+) => {
+    // results left, load the summary and display it
+    // this is intended to be dynamic (don't sub resultsCount)
+    if (results.length) {
+        _displayItem(results.pop(), searchTerms);
+        setTimeout(
+            () => _displayNextItem(results, resultCount, searchTerms),
+            5
+        );
     }
+    // search finished, update title and status message
+    else _finishSearch(resultCount);
+};
+
+/**
+ * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
+ * custom function per language.
+ *
+ * The regular expression works by splitting the string on consecutive characters
+ * that are not Unicode letters, numbers, underscores, or emoji characters.
+ * This is the same as ``\W+`` in Python, preserving the surrogate pair area.
+ */
+if (typeof splitQuery === "undefined") {
+    var splitQuery = (query) => query
+        .split(/[^\p{Letter}\p{Number}_\p{Emoji_Presentation}]+/gu)
+        .filter(term => term) // remove remaining empty strings
 }
 
 /**
  * Search Module
  */
-var Search = {
-
+const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: function(htmlString) {
-        var htmlElement = document.createElement('span');
-        htmlElement.innerHTML = htmlString;
-        $(htmlElement).find('.headerlink').remove();
-        docContent = $(htmlElement).find('[role=main]')[0];
-        return docContent.textContent || docContent.innerText;
-    },
-
-    init: function() {
-        var params = $.getQueryParameters();
-        if (params.q) {
-            var query = params.q[0];
-            $('input[name="q"]')[0].value = query;
-            this.performSearch(query);
-        }
-    },
-
-    loadIndex: function(url) {
-        $.ajax({
-            type: "GET",
-            url: url,
-            data: null,
-            dataType: "script",
-            cache: true,
-            complete: function(jqxhr, textstatus) {
-                if (textstatus != "success") {
-                    document.getElementById("searchindexloader").src = url;
-                }
-            }
+    htmlToText: (htmlString) => {
+        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
+        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
+            el.remove()
         });
-    },
-
-    setIndex: function(index) {
-        var q;
-        this._index = index;
-        if ((q = this._queued_query) !== null) {
-            this._queued_query = null;
-            Search.query(q);
+        const docContent = htmlElement.querySelector('[role="main"]');
+        if (docContent !== undefined) return docContent.textContent;
+        console.warn(
+            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+        );
+        return "";
+    },
+
+    init: () => {
+        const query = new URLSearchParams(window.location.search).get("q");
+        document
+            .querySelectorAll('input[name="q"]')
+            .forEach((el) => (el.value = query));
+        if (query) Search.performSearch(query);
+    },
+
+    loadIndex: (url) =>
+        (document.body.appendChild(document.createElement("script")).src = url),
+
+    setIndex: (index) => {
+        Search._index = index;
+        if (Search._queued_query !== null) {
+            const query = Search._queued_query;
+            Search._queued_query = null;
+            Search.query(query);
         }
     },
 
-    hasIndex: function() {
-        return this._index !== null;
-    },
+    hasIndex: () => Search._index !== null,
 
-    deferQuery: function(query) {
-        this._queued_query = query;
-    },
+    deferQuery: (query) => (Search._queued_query = query),
 
-    stopPulse: function() {
-        this._pulse_status = 0;
-    },
+    stopPulse: () => (Search._pulse_status = -1),
 
-    startPulse: function() {
-        if (this._pulse_status >= 0)
-            return;
+    startPulse: () => {
+        if (Search._pulse_status >= 0) return;
 
-        function pulse() {
-            var i;
+        const pulse = () => {
             Search._pulse_status = (Search._pulse_status + 1) % 4;
-            var dotString = '';
-            for (i = 0; i < Search._pulse_status; i++)
-                dotString += '.';
-            Search.dots.text(dotString);
-            if (Search._pulse_status > -1)
-                window.setTimeout(pulse, 500);
-        }
+            Search.dots.innerText = ".".repeat(Search._pulse_status);
+            if (Search._pulse_status >= 0) window.setTimeout(pulse, 500);
+        };
         pulse();
     },
 
     /**
      * perform a search for something (or wait until index is loaded)
      */
-    performSearch: function(query) {
+    performSearch: (query) => {
         // create the required interface elements
-        this.out = $('#search-results');
-        this.title = $('<h2>' + _('Searching') + '</h2>').appendTo(this.out);
-        this.dots = $('<span></span>').appendTo(this.title);
-        this.status = $('<p class="search-summary">&nbsp;</p>').appendTo(this.out);
-        this.output = $('<ul class="search"/>').appendTo(this.out);
-
-        $('#search-progress').text(_('Preparing search...'));
-        this.startPulse();
+        const searchText = document.createElement("h2");
+        searchText.textContent = _("Searching");
+        const searchSummary = document.createElement("p");
+        searchSummary.classList.add("search-summary");
+        searchSummary.innerText = "";
+        const searchList = document.createElement("ul");
+        searchList.classList.add("search");
+
+        const out = document.getElementById("search-results");
+        Search.title = out.appendChild(searchText);
+        Search.dots = Search.title.appendChild(document.createElement("span"));
+        Search.status = out.appendChild(searchSummary);
+        Search.output = out.appendChild(searchList);
+
+        const searchProgress = document.getElementById("search-progress");
+        // Some themes don't use the search progress node
+        if (searchProgress) {
+            searchProgress.innerText = _("Preparing search...");
+        }
+        Search.startPulse();
 
         // index already loaded, the browser was quick!
-        if (this.hasIndex())
-            this.query(query);
-        else
-            this.deferQuery(query);
+        if (Search.hasIndex()) Search.query(query);
+        else Search.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
-    query: function(query) {
-        var i;
+    query: (query) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // stem the search terms and add them to the correct list
+        const stemmer = new Stemmer();
+        const searchTerms = new Set();
+        const excludedTerms = new Set();
+        const highlightTerms = new Set();
+        const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
+        splitQuery(query.trim()).forEach((queryTerm) => {
+            const queryTermLower = queryTerm.toLowerCase();
 
-        // stem the searchterms and add them to the correct list
-        var stemmer = new Stemmer();
-        var searchterms = [];
-        var excluded = [];
-        var hlterms = [];
-        var tmp = splitQuery(query);
-        var objectterms = [];
-        for (i = 0; i < tmp.length; i++) {
-            if (tmp[i] !== "") {
-                objectterms.push(tmp[i].toLowerCase());
-            }
+            // maybe skip this "word"
+            // stopwords array is from language_data.js
+            if (
+                stopwords.indexOf(queryTermLower) !== -1 ||
+                queryTerm.match(/^\d+$/)
+            )
+                return;
 
-            if ($u.indexOf(stopwords, tmp[i].toLowerCase()) != -1 || tmp[i].match(/^\d+$/) ||
-                tmp[i] === "") {
-                // skip this "word"
-                continue;
-            }
             // stem the word
-            var word = stemmer.stemWord(tmp[i].toLowerCase());
-            // prevent stemmer from cutting word smaller than two chars
-            if (word.length < 3 && tmp[i].length >= 3) {
-                word = tmp[i];
-            }
-            var toAppend;
+            let word = stemmer.stemWord(queryTermLower);
             // select the correct list
-            if (word[0] == '-') {
-                toAppend = excluded;
-                word = word.substr(1);
-            } else {
-                toAppend = searchterms;
-                hlterms.push(tmp[i].toLowerCase());
+            if (word[0] === "-") excludedTerms.add(word.substr(1));
+            else {
+                searchTerms.add(word);
+                highlightTerms.add(queryTermLower);
             }
-            // only add if not already in the list
-            if (!$u.contains(toAppend, word))
-                toAppend.push(word);
-        }
-        var highlightstring = '?highlight=' + $.urlencode(hlterms.join(" "));
+        });
 
-        // console.debug('SEARCH: searching for:');
-        // console.info('required: ', searchterms);
-        // console.info('excluded: ', excluded);
+        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
+            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+        }
 
-        // prepare search
-        var terms = this._index.terms;
-        var titleterms = this._index.titleterms;
+        // console.debug("SEARCH: searching for:");
+        // console.info("required: ", [...searchTerms]);
+        // console.info("excluded: ", [...excludedTerms]);
+
+        // array of [docname, title, anchor, descr, score, filename]
+        let results = [];
+        _removeChildren(document.getElementById("search-progress"));
+
+        const queryLower = query.toLowerCase();
+        for (const [title, foundTitles] of Object.entries(allTitles)) {
+            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+                for (const [file, id] of foundTitles) {
+                    let score = Math.round(100 * queryLower.length / title.length)
+                    results.push([
+                        docNames[file],
+                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
+                        id !== null ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
-        // array of [filename, title, anchor, descr, score]
-        var results = [];
-        $('#search-progress').empty();
+        // search for explicit entries in index directives
+        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
+            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
+                for (const [file, id] of foundEntries) {
+                    let score = Math.round(100 * queryLower.length / entry.length)
+                    results.push([
+                        docNames[file],
+                        titles[file],
+                        id ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
         // lookup as object
-        for (i = 0; i < objectterms.length; i++) {
-            var others = [].concat(objectterms.slice(0, i),
-                objectterms.slice(i + 1, objectterms.length));
-            results = results.concat(this.performObjectSearch(objectterms[i], others));
-        }
+        objectTerms.forEach((term) =>
+            results.push(...Search.performObjectSearch(term, objectTerms))
+        );
 
         // lookup as search terms in fulltext
-        results = results.concat(this.performTermsSearch(searchterms, excluded, terms, titleterms));
+        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) {
-            for (i = 0; i < results.length; i++)
-                results[i][4] = Scorer.score(results[i]);
-        }
+        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
 
         // now sort the results by score (in opposite order of appearance, since the
         // display function below uses pop() to retrieve items) and then
         // alphabetically
-        results.sort(function(a, b) {
-            var left = a[4];
-            var right = b[4];
-            if (left > right) {
-                return 1;
-            } else if (left < right) {
-                return -1;
-            } else {
+        results.sort((a, b) => {
+            const leftScore = a[4];
+            const rightScore = b[4];
+            if (leftScore === rightScore) {
                 // same score: sort alphabetically
-                left = a[1].toLowerCase();
-                right = b[1].toLowerCase();
-                return (left > right) ? -1 : ((left < right) ? 1 : 0);
+                const leftTitle = a[1].toLowerCase();
+                const rightTitle = b[1].toLowerCase();
+                if (leftTitle === rightTitle) return 0;
+                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
             }
+            return leftScore > rightScore ? 1 : -1;
         });
 
+        // remove duplicate search results
+        // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
+        let seen = new Set();
+        results = results.reverse().reduce((acc, result) => {
+            let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
+            if (!seen.has(resultStr)) {
+                acc.push(result);
+                seen.add(resultStr);
+            }
+            return acc;
+        }, []);
+
+        results = results.reverse();
+
         // for debugging
         //Search.lastresults = results.slice();  // a copy
-        //console.info('search results:', Search.lastresults);
+        // console.info("search results:", Search.lastresults);
 
         // print the results
-        var resultCount = results.length;
-
-        function displayNextItem() {
-            // results left, load the summary and display it
-            if (results.length) {
-                var item = results.pop();
-                var listItem = $('<li style="display:none"></li>');
-                if (DOCUMENTATION_OPTIONS.FILE_SUFFIX === '') {
-                    // dirhtml builder
-                    var dirname = item[0] + '/';
-                    if (dirname.match(/\/index\/$/)) {
-                        dirname = dirname.substring(0, dirname.length - 6);
-                    } else if (dirname == 'index/') {
-                        dirname = '';
-                    }
-                    listItem.append($('<a/>').attr('href',
-                        DOCUMENTATION_OPTIONS.URL_ROOT + dirname +
-                        highlightstring + item[2]).html(item[1]));
-                } else {
-                    // normal html builders
-                    listItem.append($('<a/>').attr('href',
-                        item[0] + DOCUMENTATION_OPTIONS.FILE_SUFFIX +
-                        highlightstring + item[2]).html(item[1]));
-                }
-                if (item[3]) {
-                    listItem.append($('<span> (' + item[3] + ')</span>'));
-                    Search.output.append(listItem);
-                    listItem.slideDown(5, function() {
-                        displayNextItem();
-                    });
-                } else if (DOCUMENTATION_OPTIONS.HAS_SOURCE) {
-                    $.ajax({
-                        url: DOCUMENTATION_OPTIONS.URL_ROOT + item[0] + DOCUMENTATION_OPTIONS.FILE_SUFFIX,
-                        dataType: "text",
-                        complete: function(jqxhr, textstatus) {
-                            var data = jqxhr.responseText;
-                            if (data !== '' && data !== undefined) {
-                                listItem.append(Search.makeSearchSummary(data, searchterms, hlterms));
-                            }
-                            Search.output.append(listItem);
-                            listItem.slideDown(5, function() {
-                                displayNextItem();
-                            });
-                        }
-                    });
-                } else {
-                    // no source available, just display title
-                    Search.output.append(listItem);
-                    listItem.slideDown(5, function() {
-                        displayNextItem();
-                    });
-                }
-            }
-            // search finished, update title and status message
-            else {
-                Search.stopPulse();
-                Search.title.text(_('Search Results'));
-                if (!resultCount)
-                    Search.status.text(_('Your search did not match any documents. Please make sure that all words are spelled correctly and that you\'ve selected enough categories.'));
-                else
-                    Search.status.text(_('Search finished, found %s page(s) matching the search query.').replace('%s', resultCount));
-                Search.status.fadeIn(500);
-            }
-        }
-        displayNextItem();
+        _displayNextItem(results, results.length, searchTerms);
     },
 
     /**
      * search for object names
      */
-    performObjectSearch: function(object, otherterms) {
-        var filenames = this._index.filenames;
-        var docnames = this._index.docnames;
-        var objects = this._index.objects;
-        var objnames = this._index.objnames;
-        var titles = this._index.titles;
-
-        var i;
-        var results = [];
-
-        for (var prefix in objects) {
-            for (var name in objects[prefix]) {
-                var fullname = (prefix ? prefix + '.' : '') + name;
-                var fullnameLower = fullname.toLowerCase()
-                if (fullnameLower.indexOf(object) > -1) {
-                    var score = 0;
-                    var parts = fullnameLower.split('.');
-                    // check for different match types: exact matches of full name or
-                    // "last name" (i.e. last dotted part)
-                    if (fullnameLower == object || parts[parts.length - 1] == object) {
-                        score += Scorer.objNameMatch;
-                        // matches in last name
-                    } else if (parts[parts.length - 1].indexOf(object) > -1) {
-                        score += Scorer.objPartialMatch;
-                    }
-                    var match = objects[prefix][name];
-                    var objname = objnames[match[1]][2];
-                    var title = titles[match[0]];
-                    // If more than one term searched for, we require other words to be
-                    // found in the name/title/description
-                    if (otherterms.length > 0) {
-                        var haystack = (prefix + ' ' + name + ' ' +
-                            objname + ' ' + title).toLowerCase();
-                        var allfound = true;
-                        for (i = 0; i < otherterms.length; i++) {
-                            if (haystack.indexOf(otherterms[i]) == -1) {
-                                allfound = false;
-                                break;
-                            }
-                        }
-                        if (!allfound) {
-                            continue;
-                        }
-                    }
-                    var descr = objname + _(', in ') + title;
-
-                    var anchor = match[3];
-                    if (anchor === '')
-                        anchor = fullname;
-                    else if (anchor == '-')
-                        anchor = objnames[match[1]][1] + '-' + fullname;
-                    // add custom score for some objects according to scorer
-                    if (Scorer.objPrio.hasOwnProperty(match[2])) {
-                        score += Scorer.objPrio[match[2]];
-                    } else {
-                        score += Scorer.objPrioDefault;
-                    }
-                    results.push([docnames[match[0]], fullname, '#' + anchor, descr, score, filenames[match[0]]]);
-                }
-            }
-        }
-
+    performObjectSearch: (object, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const objects = Search._index.objects;
+        const objNames = Search._index.objnames;
+        const titles = Search._index.titles;
+
+        const results = [];
+
+        const objectSearchCallback = (prefix, match) => {
+            const name = match[4]
+            const fullname = (prefix ? prefix + "." : "") + name;
+            const fullnameLower = fullname.toLowerCase();
+            if (fullnameLower.indexOf(object) < 0) return;
+
+            let score = 0;
+            const parts = fullnameLower.split(".");
+
+            // check for different match types: exact matches of full name or
+            // "last name" (i.e. last dotted part)
+            if (fullnameLower === object || parts.slice(-1)[0] === object)
+                score += Scorer.objNameMatch;
+            else if (parts.slice(-1)[0].indexOf(object) > -1)
+                score += Scorer.objPartialMatch; // matches in last name
+
+            const objName = objNames[match[1]][2];
+            const title = titles[match[0]];
+
+            // If more than one term searched for, we require other words to be
+            // found in the name/title/description
+            const otherTerms = new Set(objectTerms);
+            otherTerms.delete(object);
+            if (otherTerms.size > 0) {
+                const haystack = `${prefix} ${name} ${objName} ${title}`.toLowerCase();
+                if (
+                    [...otherTerms].some((otherTerm) => haystack.indexOf(otherTerm) < 0)
+                )
+                    return;
+            }
+
+            let anchor = match[3];
+            if (anchor === "") anchor = fullname;
+            else if (anchor === "-") anchor = objNames[match[1]][1] + "-" + fullname;
+
+            const descr = objName + _(", in ") + title;
+
+            // add custom score for some objects according to scorer
+            if (Scorer.objPrio.hasOwnProperty(match[2]))
+                score += Scorer.objPrio[match[2]];
+            else score += Scorer.objPrioDefault;
+
+            results.push([
+                docNames[match[0]],
+                fullname,
+                "#" + anchor,
+                descr,
+                score,
+                filenames[match[0]],
+            ]);
+        };
+        Object.keys(objects).forEach((prefix) =>
+            objects[prefix].forEach((array) =>
+                objectSearchCallback(prefix, array)
+            )
+        );
         return results;
     },
 
     /**
      * search for full-text terms in the index
      */
-    performTermsSearch: function(searchterms, excluded, terms, titleterms) {
-        var docnames = this._index.docnames;
-        var filenames = this._index.filenames;
-        var titles = this._index.titles;
-
-        var i, j, file;
-        var fileMap = {};
-        var scoreMap = {};
-        var results = [];
+    performTermsSearch: (searchTerms, excludedTerms) => {
+        // prepare search
+        const terms = Search._index.terms;
+        const titleTerms = Search._index.titleterms;
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+
+        const scoreMap = new Map();
+        const fileMap = new Map();
 
         // perform the search on the required terms
-        for (i = 0; i < searchterms.length; i++) {
-            var word = searchterms[i];
-            var files = [];
-            var _o = [{
+        searchTerms.forEach((word) => {
+            const files = [];
+            const arr = [{
                 files: terms[word],
                 score: Scorer.term
             }, {
-                files: titleterms[word],
+                files: titleTerms[word],
                 score: Scorer.title
-            }];
+            }, ];
             // add support for partial matches
             if (word.length > 2) {
-                for (var w in terms) {
-                    if (w.match(word) && !terms[word]) {
-                        _o.push({
-                            files: terms[w],
+                const escapedWord = _escapeRegExp(word);
+                Object.keys(terms).forEach((term) => {
+                    if (term.match(escapedWord) && !terms[word])
+                        arr.push({
+                            files: terms[term],
                             score: Scorer.partialTerm
-                        })
-                    }
-                }
-                for (var w in titleterms) {
-                    if (w.match(word) && !titleterms[word]) {
-                        _o.push({
-                            files: titleterms[w],
+                        });
+                });
+                Object.keys(titleTerms).forEach((term) => {
+                    if (term.match(escapedWord) && !titleTerms[word])
+                        arr.push({
+                            files: titleTerms[word],
                             score: Scorer.partialTitle
-                        })
-                    }
-                }
+                        });
+                });
             }
 
             // no match but word was a required one
-            if ($u.every(_o, function(o) {
-                    return o.files === undefined;
-                })) {
-                break;
-            }
+            if (arr.every((record) => record.files === undefined)) return;
+
             // found search word in contents
-            $u.each(_o, function(o) {
-                var _files = o.files;
-                if (_files === undefined)
-                    return
-
-                if (_files.length === undefined)
-                    _files = [_files];
-                files = files.concat(_files);
-
-                // set score for the word in each file to Scorer.term
-                for (j = 0; j < _files.length; j++) {
-                    file = _files[j];
-                    if (!(file in scoreMap))
-                        scoreMap[file] = {}
-                    scoreMap[file][word] = o.score;
-                }
+            arr.forEach((record) => {
+                if (record.files === undefined) return;
+
+                let recordFiles = record.files;
+                if (recordFiles.length === undefined) recordFiles = [recordFiles];
+                files.push(...recordFiles);
+
+                // set score for the word in each file
+                recordFiles.forEach((file) => {
+                    if (!scoreMap.has(file)) scoreMap.set(file, {});
+                    scoreMap.get(file)[word] = record.score;
+                });
             });
 
             // create the mapping
-            for (j = 0; j < files.length; j++) {
-                file = files[j];
-                if (file in fileMap)
-                    fileMap[file].push(word);
-                else
-                    fileMap[file] = [word];
-            }
-        }
+            files.forEach((file) => {
+                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
+                    fileMap.get(file).push(word);
+                else fileMap.set(file, [word]);
+            });
+        });
 
         // now check if the files don't contain excluded terms
-        for (file in fileMap) {
-            var valid = true;
-
+        const results = [];
+        for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
-            var filteredTermCount = // as search terms with length < 3 are discarded: ignore
-                searchterms.filter(function(term) {
-                    return term.length > 2
-                }).length
+
+            // as search terms with length < 3 are discarded
+            const filteredTermCount = [...searchTerms].filter(
+                (term) => term.length > 2
+            ).length;
             if (
-                fileMap[file].length != searchterms.length &&
-                fileMap[file].length != filteredTermCount
-            ) continue;
+                wordList.length !== searchTerms.size &&
+                wordList.length !== filteredTermCount
+            )
+                continue;
 
             // ensure that none of the excluded terms is in the search result
-            for (i = 0; i < excluded.length; i++) {
-                if (terms[excluded[i]] == file ||
-                    titleterms[excluded[i]] == file ||
-                    $u.contains(terms[excluded[i]] || [], file) ||
-                    $u.contains(titleterms[excluded[i]] || [], file)) {
-                    valid = false;
-                    break;
-                }
-            }
+            if (
+                [...excludedTerms].some(
+                    (term) =>
+                    terms[term] === file ||
+                    titleTerms[term] === file ||
+                    (terms[term] || []).includes(file) ||
+                    (titleTerms[term] || []).includes(file)
+                )
+            )
+                break;
 
-            // if we have still a valid result we can add it to the result list
-            if (valid) {
-                // select one (max) score for the file.
-                // for better ranking, we should calculate ranking by using words statistics like basic tf-idf...
-                var score = $u.max($u.map(fileMap[file], function(w) {
-                    return scoreMap[file][w]
-                }));
-                results.push([docnames[file], titles[file], '', null, score, filenames[file]]);
-            }
+            // select one (max) score for the file.
+            const score = Math.max(...wordList.map((w) => scoreMap.get(file)[w]));
+            // add result to the result list
+            results.push([
+                docNames[file],
+                titles[file],
+                "",
+                null,
+                score,
+                filenames[file],
+            ]);
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words, hlwords is the list of normal, unstemmed
-     * words. the first one is used to find the occurrence, the
-     * latter for highlighting it.
+     * of stemmed words.
      */
-    makeSearchSummary: function(htmlText, keywords, hlwords) {
-        var text = Search.htmlToText(htmlText);
-        var textLower = text.toLowerCase();
-        var start = 0;
-        $.each(keywords, function() {
-            var i = textLower.indexOf(this.toLowerCase());
-            if (i > -1)
-                start = i;
-        });
-        start = Math.max(start - 120, 0);
-        var excerpt = ((start > 0) ? '...' : '') +
-            $.trim(text.substr(start, 240)) +
-            ((start + 240 - text.length) ? '...' : '');
-        var rv = $('<div class="context"></div>').text(excerpt);
-        $.each(hlwords, function() {
-            rv = rv.highlightText(this, 'highlighted');
-        });
-        return rv;
-    }
+    makeSearchSummary: (htmlText, keywords) => {
+        const text = Search.htmlToText(htmlText);
+        if (text === "") return null;
+
+        const textLower = text.toLowerCase();
+        const actualStartPosition = [...keywords]
+            .map((k) => textLower.indexOf(k.toLowerCase()))
+            .filter((i) => i > -1)
+            .slice(-1)[0];
+        const startWithContext = Math.max(actualStartPosition - 120, 0);
+
+        const top = startWithContext === 0 ? "" : "...";
+        const tail = startWithContext + 240 < text.length ? "..." : "";
+
+        let summary = document.createElement("p");
+        summary.classList.add("context");
+        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
+
+        return summary;
+    },
 };
 
-$(document).ready(function() {
-    Search.init();
-});
+_ready(Search.init);
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/genindex.html` & `vitables-3.0.3/vitables/htmldocs/genindex.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>Index &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="#" />
-    <link rel="search" title="Search" href="search.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="#" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-
-<h1 id="index">Index</h1>
-
-<div class="genindex-jumpbox">
- 
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="#" title="General Index"
-             >index</a></li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+    <title>Index &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="#" />
+    <link rel="search" title="Search" href="search.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="#" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href="">Index</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+
+<h1 id="index">Index</h1>
+
+<div class="genindex-jumpbox">
+ 
+</div>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="#" title="General Index"
+             >index</a></li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href="">Index</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 
 
 
 
 **** Navigation ****
     * index
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * Index
 ****** Index ******
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * Index
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/usersguide-app1.html` & `vitables-3.0.3/vitables/htmldocs/usersguide-app1.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,125 @@
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>6. About Plugins &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="7. The Help Browser" href="usersguide-app2.html" />
-    <link rel="prev" title="5. Configuring ViTables" href="usersguide-ch5.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="right" >
-          <a href="usersguide-app2.html" title="7. The Help Browser"
-             accesskey="N">next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
-             accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-  <div class="section" id="about-plugins">
-<span id="appendix-a"></span><h1>6. About Plugins<a class="headerlink" href="#about-plugins" title="Permalink to this headline">¶</a></h1>
-<p>Since version 2.1 <cite>ViTables</cite> has a simple but powerful plugins framework.</p>
-<p>If you are interested in writing plugins the next paragraphs can be of utility. If not you can skip to the list of available plugins.</p>
-<p>Plugins live in the plugins subdirectory of the root directory where the source code is installed. A plugin can be a pure Python module or can have a package structure (i.e. a directory with a <code class="xref py py-mod docutils literal notranslate"><span class="pre">__init__.py</span></code> file). Packages can have as many directories as you want but plugins must be located at top level of the package.</p>
-<p>The use of contracts is not enforced when writing plugins so you have nearly complete freedom for writing them. Nevertheless a plugin must declare the following variables. <code class="xref py py-const docutils literal notranslate"><span class="pre">plugin_class</span></code> which is set to the name of the class invoqued when your plugin is executed by <cite>ViTables</cite>,
-<code class="xref py py-const docutils literal notranslate"><span class="pre">plugin_name</span></code> which is set to the descriptive name of the plugin and will be used in the Plugins page of the Preferences dialog and, finally, <code class="xref py py-const docutils literal notranslate"><span class="pre">comment</span></code> which is set to a short description of the plugin and will be used too in the Plugins page of the Preferences dialog.</p>
-<p>In some cases it can be useful to use convenience variables or methods. For instance, suppose than in the Preferences dialog you want to show a more complete description of your plugin that that provided by the <code class="xref py py-const docutils literal notranslate"><span class="pre">comment</span></code> variable. Then you may be interested in define a method <code class="xref py py-meth docutils literal notranslate"><span class="pre">helpAbout()</span></code> in your plugin.</p>
-<p>Of course some knowledge (not necessarily a deep one) of the <cite>ViTables</cite> code is required in order to bind your plugin to the application core. This task is commonly achieved via the menu bar of the main window or via the signals/slots mechanism (convenience signals can be defined in the application if needed).</p>
-<p>If you need more help just send an email to developers or ask to the <cite>ViTables</cite> Users’ Group.</p>
-<p>Three plugins are currently distributed along with the application:</p>
-<blockquote>
-<div><dl class="simple">
-<dt>Time series formatter</dt><dd><p>formats time series in a human friendly way. It supports PyTables time datatypes and PyTables time series created via <a class="reference external" href="https://pandas.pydata.org">pandas</a> or the obsolete scikits.timeseries module. The format used for displaying times can be configured by user via the Preferences dialog or editing by hand the <code class="file docutils literal notranslate"><span class="pre">time_format.ini</span></code> configuration file.</p>
-</dd>
-<dt>Tree of DBs sorting</dt><dd><p>sorts the display of the databases tree.</p>
-</dd>
-<dt>Columnar organization of arrays</dt><dd><p>rearranges several arrays with the same number of rows and displays them in a unique widget.</p>
-</dd>
-</dl>
-</div></blockquote>
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="usersguide-ch5.html"
-                        title="previous chapter">5. Configuring ViTables</a></p>
-  <h4>Next topic</h4>
-  <p class="topless"><a href="usersguide-app2.html"
-                        title="next chapter">7. The Help Browser</a></p>
-  <div role="note" aria-label="source link">
-    <h3>This Page</h3>
-    <ul class="this-page-menu">
-      <li><a href="_sources/usersguide-app1.rst.txt"
-            rel="nofollow">Show Source</a></li>
-    </ul>
-   </div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             >index</a></li>
-        <li class="right" >
-          <a href="usersguide-app2.html" title="7. The Help Browser"
-             >next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
-             >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+    <title>6. About Plugins &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="7. The Help Browser" href="usersguide-app2.html" />
+    <link rel="prev" title="5. Configuring ViTables" href="usersguide-ch5.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="right" >
+          <a href="usersguide-app2.html" title="7. The Help Browser"
+             accesskey="N">next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
+             accesskey="P">previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">6. </span>About Plugins</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+  <section id="about-plugins">
+<span id="appendix-a"></span><h1><span class="section-number">6. </span>About Plugins<a class="headerlink" href="#about-plugins" title="Permalink to this heading">¶</a></h1>
+<p>Since version 2.1 <cite>ViTables</cite> has a simple but powerful plugins framework.</p>
+<p>If you are interested in writing plugins the next paragraphs can be of utility. If not you can skip to the list of available plugins.</p>
+<p>Plugins live in the plugins subdirectory of the root directory where the source code is installed. A plugin can be a pure Python module or can have a package structure (i.e. a directory with a <code class="xref py py-mod docutils literal notranslate"><span class="pre">__init__.py</span></code> file). Packages can have as many directories as you want but plugins must be located at top level of the package.</p>
+<p>The use of contracts is not enforced when writing plugins so you have nearly complete freedom for writing them. Nevertheless a plugin must declare the following variables. <code class="xref py py-const docutils literal notranslate"><span class="pre">plugin_class</span></code> which is set to the name of the class invoqued when your plugin is executed by <cite>ViTables</cite>,
+<code class="xref py py-const docutils literal notranslate"><span class="pre">plugin_name</span></code> which is set to the descriptive name of the plugin and will be used in the Plugins page of the Preferences dialog and, finally, <code class="xref py py-const docutils literal notranslate"><span class="pre">comment</span></code> which is set to a short description of the plugin and will be used too in the Plugins page of the Preferences dialog.</p>
+<p>In some cases it can be useful to use convenience variables or methods. For instance, suppose than in the Preferences dialog you want to show a more complete description of your plugin that that provided by the <code class="xref py py-const docutils literal notranslate"><span class="pre">comment</span></code> variable. Then you may be interested in define a method <code class="xref py py-meth docutils literal notranslate"><span class="pre">helpAbout()</span></code> in your plugin.</p>
+<p>Of course some knowledge (not necessarily a deep one) of the <cite>ViTables</cite> code is required in order to bind your plugin to the application core. This task is commonly achieved via the menu bar of the main window or via the signals/slots mechanism (convenience signals can be defined in the application if needed).</p>
+<p>If you need more help just send an email to developers or ask to the <cite>ViTables</cite> Users’ Group.</p>
+<p>Three plugins are currently distributed along with the application:</p>
+<blockquote>
+<div><dl class="simple">
+<dt>Time series formatter</dt><dd><p>formats time series in a human friendly way. It supports PyTables time datatypes and PyTables time series created via <a class="reference external" href="https://pandas.pydata.org">pandas</a> or the obsolete scikits.timeseries module. The format used for displaying times can be configured by user via the Preferences dialog or editing by hand the <code class="file docutils literal notranslate"><span class="pre">time_format.ini</span></code> configuration file.</p>
+</dd>
+<dt>Tree of DBs sorting</dt><dd><p>sorts the display of the databases tree.</p>
+</dd>
+<dt>Columnar organization of arrays</dt><dd><p>rearranges several arrays with the same number of rows and displays them in a unique widget.</p>
+</dd>
+</dl>
+</div></blockquote>
+</section>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="usersguide-ch5.html"
+                          title="previous chapter"><span class="section-number">5. </span>Configuring ViTables</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="usersguide-app2.html"
+                          title="next chapter"><span class="section-number">7. </span>The Help Browser</a></p>
+  </div>
+  <div role="note" aria-label="source link">
+    <h3>This Page</h3>
+    <ul class="this-page-menu">
+      <li><a href="_sources/usersguide-app1.rst.txt"
+            rel="nofollow">Show Source</a></li>
+    </ul>
+   </div>
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             >index</a></li>
+        <li class="right" >
+          <a href="usersguide-app2.html" title="7. The Help Browser"
+             >next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
+             >previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">6. </span>About Plugins</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,16 @@
 
 
 
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 6. About Plugins
 ****** 6. About PluginsÂ¶ ******
 Since version 2.1ViTableshas a simple but powerful plugins framework.
 If you are interested in writing plugins the next paragraphs can be of utility.
 If not you can skip to the list of available plugins.
 Plugins live in the plugins subdirectory of the root directory where the source
 code is installed. A plugin can be a pure Python module or can have a package
 structure (i.e. a directory with a __init__.py file). Packages can have as many
@@ -56,9 +57,10 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 6. About Plugins
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/usersguide-app2.html` & `vitables-3.0.3/vitables/htmldocs/usersguide-app2.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,109 @@
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>7. The Help Browser &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="prev" title="6. About Plugins" href="usersguide-app1.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="right" >
-          <a href="usersguide-app1.html" title="6. About Plugins"
-             accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-  <div class="section" id="the-help-browser">
-<h1>7. The Help Browser<a class="headerlink" href="#the-help-browser" title="Permalink to this headline">¶</a></h1>
-<p><cite>ViTables</cite> comes with its own fully-integrated documentation browser. It allows the <cite>ViTables</cite> User’s Guide to be browsed without leaving the current working session and without opening external applications. You can start the browser issuing the
-<span class="menuselection">Help ‣ User’s Guide</span> command or from the toolbar.</p>
-<p>The help browser is a small HTML browser for <em>local</em> documents. Despite its small size it exhibits some nice features</p>
-<ul class="simple">
-<li><p>bookmarks</p></li>
-<li><p>session history</p></li>
-<li><p>easy document navigation through navigation buttons</p></li>
-</ul>
-<p>A nice feature of bookmarks is that they can be navigated while they are being edited with the Bookmarks Editing dialog. Simply double click on a bookmark and it will be displayed in the browser.</p>
-<div class="align-center figure" id="id1">
-<span id="help-browser"></span><a class="reference internal image-reference" href="_images/helpBrowser.png"><img alt="_images/helpBrowser.png" src="_images/helpBrowser.png" style="width: 80%;" /></a>
-<p class="caption"><span class="caption-text">The Users’ Guide browser</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
-</div>
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="usersguide-app1.html"
-                        title="previous chapter">6. About Plugins</a></p>
-  <div role="note" aria-label="source link">
-    <h3>This Page</h3>
-    <ul class="this-page-menu">
-      <li><a href="_sources/usersguide-app2.rst.txt"
-            rel="nofollow">Show Source</a></li>
-    </ul>
-   </div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             >index</a></li>
-        <li class="right" >
-          <a href="usersguide-app1.html" title="6. About Plugins"
-             >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+    <title>7. The Help Browser &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="prev" title="6. About Plugins" href="usersguide-app1.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="right" >
+          <a href="usersguide-app1.html" title="6. About Plugins"
+             accesskey="P">previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">7. </span>The Help Browser</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+  <section id="the-help-browser">
+<h1><span class="section-number">7. </span>The Help Browser<a class="headerlink" href="#the-help-browser" title="Permalink to this heading">¶</a></h1>
+<p><cite>ViTables</cite> comes with its own fully-integrated documentation browser. It allows the <cite>ViTables</cite> User’s Guide to be browsed without leaving the current working session and without opening external applications. You can start the browser issuing the
+<span class="menuselection">Help ‣ User’s Guide</span> command or from the toolbar.</p>
+<p>The help browser is a small HTML browser for <em>local</em> documents. Despite its small size it exhibits some nice features</p>
+<ul class="simple">
+<li><p>bookmarks</p></li>
+<li><p>session history</p></li>
+<li><p>easy document navigation through navigation buttons</p></li>
+</ul>
+<p>A nice feature of bookmarks is that they can be navigated while they are being edited with the Bookmarks Editing dialog. Simply double click on a bookmark and it will be displayed in the browser.</p>
+<figure class="align-center" id="id1">
+<span id="help-browser"></span><a class="reference internal image-reference" href="_images/helpBrowser.png"><img alt="_images/helpBrowser.png" src="_images/helpBrowser.png" style="width: 80%;" /></a>
+<figcaption>
+<p><span class="caption-text">The Users’ Guide browser</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+</section>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="usersguide-app1.html"
+                          title="previous chapter"><span class="section-number">6. </span>About Plugins</a></p>
+  </div>
+  <div role="note" aria-label="source link">
+    <h3>This Page</h3>
+    <ul class="this-page-menu">
+      <li><a href="_sources/usersguide-app2.rst.txt"
+            rel="nofollow">Show Source</a></li>
+    </ul>
+   </div>
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             >index</a></li>
+        <li class="right" >
+          <a href="usersguide-app1.html" title="6. About Plugins"
+             >previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">7. </span>The Help Browser</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -2,34 +2,37 @@
 
 
 
 
 **** Navigation ****
     * index
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 7. The Help Browser
 ****** 7. The Help BrowserÂ¶ ******
 ViTablescomes with its own fully-integrated documentation browser. It allows
 theViTablesUserâs Guide to be browsed without leaving the current working
 session and without opening external applications. You can start the browser
 issuing the Help â£ Userâs Guide command or from the toolbar.
 The help browser is a small HTML browser for local documents. Despite its small
 size it exhibits some nice features
     * bookmarks
     * session history
     * easy document navigation through navigation buttons
 A nice feature of bookmarks is that they can be navigated while they are being
 edited with the Bookmarks Editing dialog. Simply double click on a bookmark and
 it will be displayed in the browser.
-[_images/helpBrowser.png]
+ [_images/helpBrowser.png]
 The Usersâ Guide browserÂ¶
+
 *** Previous topic ***
 6._About_Plugins
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 7. The Help Browser
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/usersguide-ch1.html` & `vitables-3.0.3/vitables/htmldocs/usersguide-ch1.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,233 +1,219 @@
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>1. Introduction &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="2. First Steps" href="usersguide-ch2.html" />
-    <link rel="prev" title="Welcome to ViTables Users’ Guide!" href="index.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch2.html" title="2. First Steps"
-             accesskey="N">next</a> |</li>
-        <li class="right" >
-          <a href="index.html" title="Welcome to ViTables Users’ Guide!"
-             accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-  <div class="section" id="introduction">
-<h1>1. Introduction<a class="headerlink" href="#introduction" title="Permalink to this headline">¶</a></h1>
-<div class="section" id="overview">
-<h2>1.1. Overview<a class="headerlink" href="#overview" title="Permalink to this headline">¶</a></h2>
-<p><cite>ViTables</cite> is a member of the <cite>PyTables</cite> family. It’s a graphical tool for browsing and editing files in both PyTables and <cite>HDF5</cite> formats. With <cite>ViTables</cite> you can easily navigate through data hierarchies, request metadata, view
-real data and much more.</p>
-<p><cite>ViTables</cite> is being developed using <cite>Python</cite> and <cite>PyQt</cite>, the bindings of <cite>Qt</cite> libraries, so it can run on any platform that supports these components (which includes Windows, Mac OS X, Linux and many other Unices). The interface and features will remain the same on all platforms.</p>
-<p>Efficiency and low memory requirements are guaranteed by the fact that data is loaded only when the object that contains it is opened and by the use of data buffers for dealing with large datasets.</p>
-</div>
-<div class="section" id="capabilities">
-<h2>1.2. Capabilities<a class="headerlink" href="#capabilities" title="Permalink to this headline">¶</a></h2>
-<p>The current release provides browsing, displaying, editing and querying capabilities. Some of them are listed below. Details are discussed in the related chapters.</p>
-<div class="section" id="browsing-and-displaying-capabilities">
-<h3>1.2.1. Browsing and displaying capabilities<a class="headerlink" href="#browsing-and-displaying-capabilities" title="Permalink to this headline">¶</a></h3>
-<ul class="simple">
-<li><p>Display data hierarchy as a fully browsable object tree.</p></li>
-<li><p>Open several files simultaneously.</p></li>
-<li><p>Open files in write mode as well as in read-only mode, disabling all editing functions.</p></li>
-<li><p>Display file information (path, size, number of nodes…).</p></li>
-<li><p>Display node (group or leaf) properties, including metadata and attributes.</p></li>
-<li><p>Display numerical arrays, i.e. homogeneous tables.</p></li>
-<li><p>Display heterogeneous table entities, i.e. records.</p></li>
-<li><p>Display multidimensional table cells.</p></li>
-<li><p>Unlimited zoom into the inner dimensions of multidimensional table cells.</p></li>
-</ul>
-</div>
-<div class="section" id="editing-capabilities">
-<h3>1.2.2. Editing capabilities<a class="headerlink" href="#editing-capabilities" title="Permalink to this headline">¶</a></h3>
-<p>These editing features have been implemented for the object tree <a class="footnote-reference brackets" href="#f1" id="id1">1</a>:</p>
-<ul class="simple">
-<li><p>File creation and renaming.</p></li>
-<li><p>Node creation (only for groups), renaming and deletion.</p></li>
-<li><p>Ability to copy and move nodes from their location to a different one, even in different files.</p></li>
-<li><p>Attribute creation, renaming and deletion.</p></li>
-</ul>
-<p>All these changes automatically update the database (i.e. the file) to which the nodes belong.</p>
-</div>
-<div class="section" id="other">
-<h3>1.2.3. Other<a class="headerlink" href="#other" title="Permalink to this headline">¶</a></h3>
-<p>Other nice features include:</p>
-<ul class="simple">
-<li><p><em>Ability to smoothly navigate really large datasets</em>.</p></li>
-<li><p>Support for doing complex table queries with a low memory footprint.</p></li>
-<li><p>Import from CSV files.</p></li>
-<li><p>Flexible plugins framework. A bunch of useful plugins are already included, see the <a class="reference internal" href="usersguide-app1.html#appendix-a"><span class="std std-ref">Appendix A</span></a> for
-details.</p></li>
-<li><p>Configurable look and feel.</p></li>
-<li><p>A logger area, where errors and warnings (if any) are printed.</p></li>
-<li><p>Several levels of help are available: users guide, context help, tooltips and status bar.</p></li>
-</ul>
-<p>We have paid special attention to usability issues so making use of these features is intuitive and pleasant.
-Nevertheless, and just in case, we are providing this guide :-).</p>
-</div>
-</div>
-<div class="section" id="system-requirements">
-<h2>1.3. System Requirements<a class="headerlink" href="#system-requirements" title="Permalink to this headline">¶</a></h2>
-<p>To run <cite>ViTables</cite> you need to install recent versions of <cite>Python3</cite>, <cite>PyTables</cite> (so you have to fulfil its own requirements) and <cite>PyQt</cite>. For instance, it runs smoothly with <cite>Python</cite> 3.6, <cite>PyTables</cite> 3.4 and <cite>PyQt</cite> 5.8.</p>
-<p>At the moment, <cite>ViTables</cite> has been fully tested on Linux and Windows 10 platforms. Other Unices should run just fine when using the Linux version because all the software that <cite>ViTables</cite> relies on (i.e. <cite>Python</cite>, <cite>Qt</cite>, <cite>PyQt</cite>, <cite>HDF5</cite> and <cite>PyTables</cite>) is known to run fine on many Unix platforms as well.</p>
-</div>
-<div class="section" id="installation">
-<h2>1.4. Installation<a class="headerlink" href="#installation" title="Permalink to this headline">¶</a></h2>
-<div class="section" id="linux">
-<h3>1.4.1. Linux<a class="headerlink" href="#linux" title="Permalink to this headline">¶</a></h3>
-<p>The Python setuptools are used to build and install <cite>ViTables</cite>. You can install
-the package from PyPI issuing the command:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ pip install ViTables
-</pre></div>
-</div>
-<p>This should install the ViTables wheel. If you experience problems installing
-the binary package you can install from sources (provided your system fulfills
-the requirements listed in the above section). Just download the tarball from
-PyPI, uncompress it, change to the distribution directory and execute (as root):</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ python setup.py install
-</pre></div>
-</div>
-<p>If you are doing this on a MacOS X platform, please make sure that the
-DYLD_LIBRARY_PATH environment variable has been setup properly.</p>
-<p>By default <cite>ViTables</cite> will be installed in the system-protected area where
-your system installs third party Python packages so you will need superuser
-privileges. If you prefer to install the package in a different location
-(for instance, your home directory) so that the installation can be done by
-non privileged users, you can do it using the –prefix (or –home) tag:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ python setup.py install --prefix=/home/myuser/mystuff
-</pre></div>
-</div>
-<p>Please, remember that installing Python modules in non-standard locations
-makes it necessary to setup properly the PYTHONPATH environment variable so
-that the Python interpreter can find the new modules.</p>
-<p>If you need further customizations, please have a look to the output of the
-command:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$python setup.py install --help
-</pre></div>
-</div>
-<p>to see all the available options. Complete information about them can be
-found in the Distutils documentation.</p>
-</div>
-<div class="section" id="windows-and-mac-os-x">
-<h3>1.4.2. Windows and Mac OS X<a class="headerlink" href="#windows-and-mac-os-x" title="Permalink to this headline">¶</a></h3>
-<p>Currently there are no graphical installers available for these platforms. You
-have to install <cite>ViTables</cite> from the command line, using one of the methods
-described in the Linux section.</p>
-</div>
-</div>
-<div class="section" id="further-reading">
-<h2>1.5. Further Reading<a class="headerlink" href="#further-reading" title="Permalink to this headline">¶</a></h2>
-<p>General information about <cite>PyTables</cite> can be found at <a class="reference external" href="https://www.pytables.org">its project site</a>.</p>
-<p>Questions and feedback can be mailed to the developers.</p>
-<p class="rubric">Footnotes</p>
-<dl class="footnote brackets">
-<dt class="label" id="f1"><span class="brackets"><a class="fn-backref" href="#id1">1</a></span></dt>
-<dd><p>Dataset editing capabilities have not yet been implemented.</p>
-</dd>
-</dl>
-</div>
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-  <h3><a href="index.html">Table of Contents</a></h3>
-  <ul>
-<li><a class="reference internal" href="#">1. Introduction</a><ul>
-<li><a class="reference internal" href="#overview">1.1. Overview</a></li>
-<li><a class="reference internal" href="#capabilities">1.2. Capabilities</a><ul>
-<li><a class="reference internal" href="#browsing-and-displaying-capabilities">1.2.1. Browsing and displaying capabilities</a></li>
-<li><a class="reference internal" href="#editing-capabilities">1.2.2. Editing capabilities</a></li>
-<li><a class="reference internal" href="#other">1.2.3. Other</a></li>
-</ul>
-</li>
-<li><a class="reference internal" href="#system-requirements">1.3. System Requirements</a></li>
-<li><a class="reference internal" href="#installation">1.4. Installation</a><ul>
-<li><a class="reference internal" href="#linux">1.4.1. Linux</a></li>
-<li><a class="reference internal" href="#windows-and-mac-os-x">1.4.2. Windows and Mac OS X</a></li>
-</ul>
-</li>
-<li><a class="reference internal" href="#further-reading">1.5. Further Reading</a></li>
-</ul>
-</li>
-</ul>
-
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="index.html"
-                        title="previous chapter">Welcome to ViTables Users’ Guide!</a></p>
-  <h4>Next topic</h4>
-  <p class="topless"><a href="usersguide-ch2.html"
-                        title="next chapter">2. First Steps</a></p>
-  <div role="note" aria-label="source link">
-    <h3>This Page</h3>
-    <ul class="this-page-menu">
-      <li><a href="_sources/usersguide-ch1.rst.txt"
-            rel="nofollow">Show Source</a></li>
-    </ul>
-   </div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             >index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch2.html" title="2. First Steps"
-             >next</a> |</li>
-        <li class="right" >
-          <a href="index.html" title="Welcome to ViTables Users’ Guide!"
-             >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+    <title>1. Introduction &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="2. First Steps" href="usersguide-ch2.html" />
+    <link rel="prev" title="Welcome to ViTables Users’ Guide!" href="index.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch2.html" title="2. First Steps"
+             accesskey="N">next</a> |</li>
+        <li class="right" >
+          <a href="index.html" title="Welcome to ViTables Users’ Guide!"
+             accesskey="P">previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">1. </span>Introduction</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+  <section id="introduction">
+<h1><span class="section-number">1. </span>Introduction<a class="headerlink" href="#introduction" title="Permalink to this heading">¶</a></h1>
+<section id="overview">
+<h2><span class="section-number">1.1. </span>Overview<a class="headerlink" href="#overview" title="Permalink to this heading">¶</a></h2>
+<p><cite>ViTables</cite> is a member of the <cite>PyTables</cite> family. It’s a graphical tool for browsing and editing files in both PyTables and <cite>HDF5</cite> formats. With <cite>ViTables</cite> you can easily navigate through data hierarchies, request metadata, view
+real data and much more.</p>
+<p><cite>ViTables</cite> is being developed using <cite>Python</cite> and <cite>PyQt</cite>, the bindings of <cite>Qt</cite> libraries, so it can run on any platform that supports these components (which includes Windows, Mac OS X, Linux and many other Unices). The interface and features will remain the same on all platforms.</p>
+<p>Efficiency and low memory requirements are guaranteed by the fact that data is loaded only when the object that contains it is opened and by the use of data buffers for dealing with large datasets.</p>
+</section>
+<section id="capabilities">
+<h2><span class="section-number">1.2. </span>Capabilities<a class="headerlink" href="#capabilities" title="Permalink to this heading">¶</a></h2>
+<p>The current release provides browsing, displaying, editing and querying capabilities. Some of them are listed below. Details are discussed in the related chapters.</p>
+<section id="browsing-and-displaying-capabilities">
+<h3><span class="section-number">1.2.1. </span>Browsing and displaying capabilities<a class="headerlink" href="#browsing-and-displaying-capabilities" title="Permalink to this heading">¶</a></h3>
+<ul class="simple">
+<li><p>Display data hierarchy as a fully browsable object tree.</p></li>
+<li><p>Open several files simultaneously.</p></li>
+<li><p>Open files in write mode as well as in read-only mode, disabling all editing functions.</p></li>
+<li><p>Display file information (path, size, number of nodes…).</p></li>
+<li><p>Display node (group or leaf) properties, including metadata and attributes.</p></li>
+<li><p>Display numerical arrays, i.e. homogeneous tables.</p></li>
+<li><p>Display heterogeneous table entities, i.e. records.</p></li>
+<li><p>Display multidimensional table cells.</p></li>
+<li><p>Unlimited zoom into the inner dimensions of multidimensional table cells.</p></li>
+</ul>
+</section>
+<section id="editing-capabilities">
+<h3><span class="section-number">1.2.2. </span>Editing capabilities<a class="headerlink" href="#editing-capabilities" title="Permalink to this heading">¶</a></h3>
+<p>These editing features have been implemented for the object tree <a class="footnote-reference brackets" href="#f1" id="id1" role="doc-noteref"><span class="fn-bracket">[</span>1<span class="fn-bracket">]</span></a>:</p>
+<ul class="simple">
+<li><p>File creation and renaming.</p></li>
+<li><p>Node creation (only for groups), renaming and deletion.</p></li>
+<li><p>Ability to copy and move nodes from their location to a different one, even in different files.</p></li>
+<li><p>Attribute creation, renaming and deletion.</p></li>
+</ul>
+<p>All these changes automatically update the database (i.e. the file) to which the nodes belong.</p>
+</section>
+<section id="other">
+<h3><span class="section-number">1.2.3. </span>Other<a class="headerlink" href="#other" title="Permalink to this heading">¶</a></h3>
+<p>Other nice features include:</p>
+<ul class="simple">
+<li><p><em>Ability to smoothly navigate really large datasets</em>.</p></li>
+<li><p>Support for doing complex table queries with a low memory footprint.</p></li>
+<li><p>Import from CSV files.</p></li>
+<li><p>Flexible plugins framework. A bunch of useful plugins are already included, see the <a class="reference internal" href="usersguide-app1.html#appendix-a"><span class="std std-ref">Appendix A</span></a> for
+details.</p></li>
+<li><p>Configurable look and feel.</p></li>
+<li><p>A logger area, where errors and warnings (if any) are printed.</p></li>
+<li><p>Several levels of help are available: users guide, context help, tooltips and status bar.</p></li>
+</ul>
+<p>We have paid special attention to usability issues so making use of these features is intuitive and pleasant.
+Nevertheless, and just in case, we are providing this guide :-).</p>
+</section>
+</section>
+<section id="system-requirements">
+<h2><span class="section-number">1.3. </span>System Requirements<a class="headerlink" href="#system-requirements" title="Permalink to this heading">¶</a></h2>
+<p>To run <cite>ViTables</cite> you need to install recent versions of <cite>Python3</cite>, <cite>PyTables</cite> (so you have to fulfil its own requirements) and <cite>PyQt</cite>. For instance, it runs smoothly with <cite>Python</cite> 3.11, <cite>PyTables</cite> 3.8 and <cite>PyQt</cite> 6.5.</p>
+<p>At the moment, <cite>ViTables</cite> has been fully tested on Linux and Windows 10 platforms. Other Unices should run just fine when using the Linux version because all the software that <cite>ViTables</cite> relies on (i.e. <cite>Python</cite>, <cite>Qt</cite>, <cite>PyQt</cite>, <cite>HDF5</cite> and <cite>PyTables</cite>) is known to run fine on many Unix platforms as well.</p>
+</section>
+<section id="installation">
+<h2><span class="section-number">1.4. </span>Installation<a class="headerlink" href="#installation" title="Permalink to this heading">¶</a></h2>
+<section id="linux">
+<h3><span class="section-number">1.4.1. </span>Linux<a class="headerlink" href="#linux" title="Permalink to this heading">¶</a></h3>
+<p>A pyproject.toml (with <cite>hatch</cite> as a build-system) is used to build and install <cite>ViTables</cite>. You can install
+the package from PyPI issuing the command:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ pip install ViTables
+</pre></div>
+</div>
+<p>If you don’t have any version of <cite>PyQt</cite> installed you can pass it as an extra to the above command:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ pip install ViTables[PyQt5|PyQt6]
+</pre></div>
+</div>
+<p>In theory <cite>PySide2</cite> and <cite>PySide6</cite> should work too but they have not been tested.</p>
+</section>
+<section id="windows-and-mac-os-x">
+<h3><span class="section-number">1.4.2. </span>Windows and Mac OS X<a class="headerlink" href="#windows-and-mac-os-x" title="Permalink to this heading">¶</a></h3>
+<p>Currently there are no graphical installers available for these platforms. You
+have to install <cite>ViTables</cite> from the command line, using the method described in the Linux section.</p>
+</section>
+</section>
+<section id="further-reading">
+<h2><span class="section-number">1.5. </span>Further Reading<a class="headerlink" href="#further-reading" title="Permalink to this heading">¶</a></h2>
+<p>General information about <cite>PyTables</cite> can be found at <a class="reference external" href="https://www.pytables.org">its project site</a>.</p>
+<p>Questions and feedback can be mailed to the developers.</p>
+<p class="rubric">Footnotes</p>
+<aside class="footnote-list brackets">
+<aside class="footnote brackets" id="f1" role="doc-footnote">
+<span class="label"><span class="fn-bracket">[</span><a role="doc-backlink" href="#id1">1</a><span class="fn-bracket">]</span></span>
+<p>Dataset editing capabilities have not yet been implemented.</p>
+</aside>
+</aside>
+</section>
+</section>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+  <div>
+    <h3><a href="index.html">Table of Contents</a></h3>
+    <ul>
+<li><a class="reference internal" href="#">1. Introduction</a><ul>
+<li><a class="reference internal" href="#overview">1.1. Overview</a></li>
+<li><a class="reference internal" href="#capabilities">1.2. Capabilities</a><ul>
+<li><a class="reference internal" href="#browsing-and-displaying-capabilities">1.2.1. Browsing and displaying capabilities</a></li>
+<li><a class="reference internal" href="#editing-capabilities">1.2.2. Editing capabilities</a></li>
+<li><a class="reference internal" href="#other">1.2.3. Other</a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#system-requirements">1.3. System Requirements</a></li>
+<li><a class="reference internal" href="#installation">1.4. Installation</a><ul>
+<li><a class="reference internal" href="#linux">1.4.1. Linux</a></li>
+<li><a class="reference internal" href="#windows-and-mac-os-x">1.4.2. Windows and Mac OS X</a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#further-reading">1.5. Further Reading</a></li>
+</ul>
+</li>
+</ul>
+
+  </div>
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="index.html"
+                          title="previous chapter">Welcome to ViTables Users’ Guide!</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="usersguide-ch2.html"
+                          title="next chapter"><span class="section-number">2. </span>First Steps</a></p>
+  </div>
+  <div role="note" aria-label="source link">
+    <h3>This Page</h3>
+    <ul class="this-page-menu">
+      <li><a href="_sources/usersguide-ch1.rst.txt"
+            rel="nofollow">Show Source</a></li>
+    </ul>
+   </div>
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             >index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch2.html" title="2. First Steps"
+             >next</a> |</li>
+        <li class="right" >
+          <a href="index.html" title="Welcome to ViTables Users’ Guide!"
+             >previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">1. </span>Introduction</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -4,28 +4,30 @@
 
 
 
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 1. Introduction
 ****** 1. IntroductionÂ¶ ******
 ***** 1.1. OverviewÂ¶ *****
 ViTablesis a member of thePyTablesfamily. Itâs a graphical tool for browsing
 and editing files in both PyTables andHDF5formats. WithViTablesyou can easily
 navigate through data hierarchies, request metadata, view real data and much
 more.
 ViTablesis being developed usingPythonandPyQt, the bindings ofQtlibraries, so
 it can run on any platform that supports these components (which includes
 Windows, Mac OS X, Linux and many other Unices). The interface and features
 will remain the same on all platforms.
 Efficiency and low memory requirements are guaranteed by the fact that data is
 loaded only when the object that contains it is opened and by the use of data
 buffers for dealing with large datasets.
+
 ***** 1.2. CapabilitiesÂ¶ *****
 The current release provides browsing, displaying, editing and querying
 capabilities. Some of them are listed below. Details are discussed in the
 related chapters.
 **** 1.2.1. Browsing and displaying capabilitiesÂ¶ ****
     * Display data hierarchy as a fully browsable object tree.
     * Open several files simultaneously.
@@ -34,82 +36,71 @@
     * Display file information (path, size, number of nodesâ¦).
     * Display node (group or leaf) properties, including metadata and
       attributes.
     * Display numerical arrays, i.e. homogeneous tables.
     * Display heterogeneous table entities, i.e. records.
     * Display multidimensional table cells.
     * Unlimited zoom into the inner dimensions of multidimensional table cells.
+
 **** 1.2.2. Editing capabilitiesÂ¶ ****
-These editing features have been implemented for the object tree 1:
+These editing features have been implemented for the object tree [1]:
     * File creation and renaming.
     * Node creation (only for groups), renaming and deletion.
     * Ability to copy and move nodes from their location to a different one,
       even in different files.
     * Attribute creation, renaming and deletion.
 All these changes automatically update the database (i.e. the file) to which
 the nodes belong.
+
 **** 1.2.3. OtherÂ¶ ****
 Other nice features include:
     * Ability to smoothly navigate really large datasets.
     * Support for doing complex table queries with a low memory footprint.
     * Import from CSV files.
     * Flexible plugins framework. A bunch of useful plugins are already
       included, see the Appendix_A for details.
     * Configurable look and feel.
     * A logger area, where errors and warnings (if any) are printed.
     * Several levels of help are available: users guide, context help, tooltips
       and status bar.
 We have paid special attention to usability issues so making use of these
 features is intuitive and pleasant. Nevertheless, and just in case, we are
 providing this guide :-).
+
 ***** 1.3. System RequirementsÂ¶ *****
 To runViTablesyou need to install recent versions ofPython3,PyTables(so you
 have to fulfil its own requirements) andPyQt. For instance, it runs smoothly
-withPython3.6,PyTables3.4 andPyQt5.8.
+withPython3.11,PyTables3.8 andPyQt6.5.
 At the moment,ViTableshas been fully tested on Linux and Windows 10 platforms.
 Other Unices should run just fine when using the Linux version because all the
 software thatViTablesrelies on (i.e.Python,Qt,PyQt,HDF5andPyTables) is known to
 run fine on many Unix platforms as well.
+
 ***** 1.4. InstallationÂ¶ *****
 **** 1.4.1. LinuxÂ¶ ****
-The Python setuptools are used to build and installViTables. You can install
-the package from PyPI issuing the command:
+A pyproject.toml (withhatchas a build-system) is used to build and
+installViTables. You can install the package from PyPI issuing the command:
 $ pip install ViTables
-This should install the ViTables wheel. If you experience problems installing
-the binary package you can install from sources (provided your system fulfills
-the requirements listed in the above section). Just download the tarball from
-PyPI, uncompress it, change to the distribution directory and execute (as
-root):
-$ python setup.py install
-If you are doing this on a MacOS X platform, please make sure that the
-DYLD_LIBRARY_PATH environment variable has been setup properly.
-By defaultViTableswill be installed in the system-protected area where your
-system installs third party Python packages so you will need superuser
-privileges. If you prefer to install the package in a different location (for
-instance, your home directory) so that the installation can be done by non
-privileged users, you can do it using the âprefix (or âhome) tag:
-$ python setup.py install --prefix=/home/myuser/mystuff
-Please, remember that installing Python modules in non-standard locations makes
-it necessary to setup properly the PYTHONPATH environment variable so that the
-Python interpreter can find the new modules.
-If you need further customizations, please have a look to the output of the
-command:
-$python setup.py install --help
-to see all the available options. Complete information about them can be found
-in the Distutils documentation.
+If you donât have any version ofPyQtinstalled you can pass it as an extra to
+the above command:
+$ pip install ViTables[PyQt5|PyQt6]
+In theoryPySide2andPySide6should work too but they have not been tested.
+
 **** 1.4.2. Windows and Mac OS XÂ¶ ****
 Currently there are no graphical installers available for these platforms. You
-have to installViTablesfrom the command line, using one of the methods
-described in the Linux section.
+have to installViTablesfrom the command line, using the method described in the
+Linux section.
+
 ***** 1.5. Further ReadingÂ¶ *****
 General information aboutPyTablescan be found at its_project_site.
 Questions and feedback can be mailed to the developers.
 Footnotes
-  1
-      Dataset editing capabilities have not yet been implemented.
+  [1]
+Dataset editing capabilities have not yet been implemented.
+
 **** Table_of_Contents ****
     * 1._Introduction
           o 1.1._Overview
           o 1.2._Capabilities
                 # 1.2.1._Browsing_and_displaying_capabilities
                 # 1.2.2._Editing_capabilities
                 # 1.2.3._Other
@@ -126,9 +117,10 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 1. Introduction
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/usersguide-ch2.html` & `vitables-3.0.3/vitables/htmldocs/usersguide-ch2.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,240 +1,252 @@
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>2. First Steps &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="3. Browsing and Querying Datasets" href="usersguide-ch3.html" />
-    <link rel="prev" title="1. Introduction" href="usersguide-ch1.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
-             accesskey="N">next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch1.html" title="1. Introduction"
-             accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-  <div class="section" id="first-steps">
-<h1>2. First Steps<a class="headerlink" href="#first-steps" title="Permalink to this headline">¶</a></h1>
-<p>In this chapter we are going to describe briefly the main elements  that you will meet throughout your working sessions.</p>
-<div class="section" id="how-to-start">
-<h2>2.1. How to Start<a class="headerlink" href="#how-to-start" title="Permalink to this headline">¶</a></h2>
-<p>You can start <cite>ViTables</cite> from a desktop shortcut or from a terminal emulator.
-If you launch the program from the command line the following options are available:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables --help
-
-usage: vitables [option]... [h5file]...
-
-positional arguments:
-  h5file
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --version             show program&#39;s version number and exit
-
-h5files:
-  -m MODE, --mode MODE  mode access for a database. Can be r(ead) or a(ppend)
-  -d DBLIST, --dblist DBLIST
-                        a file with the list of HDF5 filepaths to be open
-
-logging:
-  -l LOG_FILE, --log-file LOG_FILE
-                        log file path
-  -v, --verbose         log verbosity level
-</pre></div>
-</div>
-<p>Basically you can specify a file to open or a file containing a list of files to open. For example:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables myh5file
-</pre></div>
-</div>
-<p>will start <cite>ViTables</cite> and open the file myh5file in read-write mode. If you want to open it in read-only mode then execute the command:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables -m r myh5file
-</pre></div>
-</div>
-<p>In order to open a set of files at once put them in a list file with the syntax</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">mode</span> <span class="n">path</span>
-</pre></div>
-</div>
-<p>(one pair per line) and execute:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables -d h5list
-</pre></div>
-</div>
-<p>Once the application is running the <a class="reference internal" href="#main-window"><span class="std std-ref">main window</span></a> appears. It consists of a <a class="reference internal" href="#menu-bar"><span class="std std-ref">menu bar</span></a>, a set of tool bars, a <a class="reference internal" href="#viewing-area"><span class="std std-ref">viewing area</span></a> and a status bar.</p>
-<p>The viewing area of the window is divided into three parts. The <a class="reference internal" href="#tree-pane"><span class="std std-ref">tree of databases viewer</span></a> is the narrow region placed at top left side. It will display a tree representation of the data hierarchies we want to access. The big panel next to the tree viewer is called the <a class="reference internal" href="#workspace"><span class="std std-ref">workspace</span></a>, and will display the real data contained in a given node of the data hierarchy. Finally, the bottom region is the <a class="reference internal" href="#logger"><span class="std std-ref">logger</span></a>, a kind of text non interactive console where information about your requested operations will be shown.</p>
-<p>As usual, you can launch commands from the menu bar, from
-context menus or, if a shortcut button is available, from a toolbar.
-Also keyboard shortcuts are available for most commands.</p>
-<p>After starting your session, you are likely to open some files. Just drag the file(s) you want to open into the tree of databases viewer and they will be opened in read-write mode. Opening can be done from the file manager dialog too; simply issue an open command, <span class="menuselection">File ‣ Open File</span> (<kbd class="kbd docutils literal notranslate">Ctrl-O</kbd>) and choose a file.</p>
-<div class="align-center figure" id="id1">
-<span id="main-window"></span><a class="reference internal image-reference" href="_images/mainWindow.png"><img alt="_images/mainWindow.png" src="_images/mainWindow.png" style="width: 90%;" /></a>
-<p class="caption"><span class="caption-text">The main window</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
-</div>
-</div>
-<div class="section" id="the-menu-bar">
-<span id="menu-bar"></span><h2>2.2. The Menu Bar<a class="headerlink" href="#the-menu-bar" title="Permalink to this headline">¶</a></h2>
-<p>The menu bar is placed at top of the main window. It is composed of six pulldown menus.</p>
-<p><strong>File menu</strong></p>
-<p>This menu contains commands to manipulate files in several ways: open, close, create, save and so on. It also gives to you quick access to the most recently opened files.</p>
-<p><strong>Node menu</strong></p>
-<p>The <span class="guilabel">Node</span> menu contains commands to manipulate the nodes displayed in the tree of databases viewer. From this menu you can edit nodes in a variety of ways as well as access their properties.</p>
-<p><strong>Dataset menu</strong></p>
-<p>With this menu you can make selects in any table (the result of your selects will be available under the Query Results node in the tree pane). The number of entries for this menu depends on the list of enabled plugins.</p>
-<p><strong>Settings menu</strong></p>
-<p>This is the menu from which the application can be customized.
-Customization includes startup behavior, look and feel and plugins management. You can add/remove paths for loading plugins, enable and disable plugins. Changes in the enabled/disabled status of a given plugin take effect after restarting <cite>ViTables</cite>.  See <a class="reference internal" href="usersguide-ch5.html#configuration-chapter"><span class="std std-ref">the ViTables Configuration chapter</span></a> for more information on this subject.</p>
-<p>Also from this menu you can show, hide and line up the application toolbars. At the moment four toolbars are available, <span class="guilabel">File</span>, <span class="guilabel">Node</span>, <span class="guilabel">Query</span> and <span class="guilabel">Help</span>.</p>
-<p><strong>Window menu</strong></p>
-<p>The <span class="guilabel">Window</span> menu can be used to change the arrangement of the workspace contents, sorting the open windows as a cascade or as a tile. By selecting a window name from this menu, you can raise (bring to the front) that window. Any open window can be closed from this menu.</p>
-<p><strong>Help menu</strong></p>
-<p>The <span class="guilabel">Help</span> menu displays this User’s Guide in :<cite>HTML4</cite> format and a couple of <em>About</em> boxes, one for the <cite>ViTables</cite> itself and one for the underlying Qt libraries. The <span class="guilabel">Show Versions</span> entry shows the version numbers of the libraries being used by <cite>ViTables</cite> (Qt, PyQt, PyTables and PyTables related libraries, like Zlib or <cite>LZO</cite>). Finally, from this menu you can enter the <em>What’s This</em> mode which will show context help for the components of the viewing area (the databases tree viewer, the workspace and the logger).</p>
-</div>
-<div class="section" id="the-viewing-area">
-<span id="viewing-area"></span><h2>2.3. The Viewing Area<a class="headerlink" href="#the-viewing-area" title="Permalink to this headline">¶</a></h2>
-<p>As mentioned before, the viewing area is divided into three regions: the databases tree viewer (also called tree pane), the workspace and the logger. Now we are going to describe these regions in more detail.</p>
-<div class="section" id="the-databases-tree-viewer">
-<span id="tree-pane"></span><h3>2.3.1. The Databases Tree Viewer<a class="headerlink" href="#the-databases-tree-viewer" title="Permalink to this headline">¶</a></h3>
-<p>Due to the hierarchical model of the underlying <cite>HDF5</cite> library, PyTables files store their data on disk in a tree-like structure. Every time you open a PyTables file, its so-called object tree (a representation of the data hierarchy) is dynamically created and added to the tree of databases viewer, at the top left side of the viewing area (see <a class="reference internal" href="#main-window"><span class="std std-ref">the main window Figure</span></a>).</p>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>since PyTables-1.2 the object tree of an opened file is made on demand: nodes are added to the tree when they are accessed. <cite>ViTables</cite> makes use of this feature, which results in stunningly fast opening times for files with a large number of nodes.</p>
-</div>
-<p>Any object tree is made of nodes which can be classified as follows:</p>
-<blockquote>
-<div><dl class="simple">
-<dt>Root node</dt><dd><p>It is the node from which all other nodes hang.</p>
-</dd>
-<dt>Groups</dt><dd><p>Groups are nodes that can contain other nodes.</p>
-</dd>
-<dt>Leaves</dt><dd><p>Leaves are nodes that contain real data. They can be tables or arrays.</p>
-</dd>
-</dl>
-</div></blockquote>
-<p>Working with object trees is really easy. By double-clicking
-on it, a root node is opened, and the tree structure below it is displayed. Groups are presented as folders. They can be expanded with a double-click, giving you immediate access to their contents. A group can contain groups and/or leaves (or
-may be empty). A double click on a leaf will display its content on the workspace. You can access the available options for a given node just with a right mouse click on it. A context menu will appear from which commands can be launched. The contents of the menu depend on the kind of node being clicked (root nodes, groups, tables and arrays have all of
-them their own context menu). Alternatively you can select the node with a single mouse click and choose a command from the
-<span class="guilabel">Node</span> menu. There is also a context menu
-for the tree pane itself that will pop up by right-clicking any empty area of the tree viewer. Last but not least, the object tree can be navigated with the keyboard too. Pressing the Enter key the selected node will be expanded (if it is a group) or opened (if it is a leaf). The + and - keys expand an collapse groups.</p>
-<p>Every node in a given object tree has an associated icon that
-allows you to identify its type quickly. The following icons are available:</p>
-<div class="align-center figure" id="id2">
-<span id="node-symbols"></span><img alt="_images/treeSymbols.png" src="_images/treeSymbols.png" />
-<p class="caption"><span class="caption-text">The node symbols</span><a class="headerlink" href="#id2" title="Permalink to this image">¶</a></p>
-</div>
-</div>
-<div class="section" id="the-workspace">
-<span id="workspace"></span><h3>2.3.2. The Workspace<a class="headerlink" href="#the-workspace" title="Permalink to this headline">¶</a></h3>
-<p>At this point you should have one or more files opened, and their object trees displayed in the databases tree viewer. Your next step will be to select a leaf and display its data. Remember that the object tree imitates the structure on disk, which makes it very easy to browse the hierarchy of the file and locate the leaf you want to open.</p>
-<p>A double-click on a leaf of your choice will open it and display its contents in a window (a <em>view</em> in the
-<cite>ViTables</cite> jargon) placed in the workspace, the big panel at the top right side of the viewing area (see <a class="reference internal" href="#main-window"><span class="std std-ref">the main window Figure</span></a>).</p>
-<p>Note that the databases tree viewer and the workspace are always synchronized: if you select a node in the tree viewer and that node has a view, then that view becomes the active view on the workspace. The opposite is also true, click on a view on the workspace and its node will be automatically selected on the databases tree viewer.</p>
-<p>The <span class="guilabel">Window</span> pulldown menu provides some
-additional commands that will help you to manage your
-views. From this menu you can, for instance, rearrange views, see the list of views (which is particularly useful when the workspace is cluttered with so many views that it’s difficult to find the one you want) or close all the views at once.</p>
-<p>There is also a context menu for the workspace. It can be used to change the workspace view mode: you can display views as regular windows (default behavior) or with tabs in a tab bar. In addition it give you access to the <span class="guilabel">Window</span> pulldown menu.</p>
-</div>
-<div class="section" id="the-logger">
-<span id="logger"></span><h3>2.3.3. The Logger<a class="headerlink" href="#the-logger" title="Permalink to this headline">¶</a></h3>
-<p>The logger is a read-only (i.e. non interactive) console placed at the bottom of the viewing area (see <a class="reference internal" href="#main-window"><span class="std std-ref">the main window Figure</span></a>). It is an info panel where <cite>ViTables</cite> reports the result of requested operations (namely if they were not successful). Also runtime errors are caught and reported to you through the logger (so you can mail the error to <cite>ViTables</cite>
-developers and help to improve the quality of the package :-). Errors and warning messages are highlighted in red and orange respectively.</p>
-<p>Of course there is also a context menu for the logger that
-provides you with some handy operations, like to copy selected text or to empty the logger.</p>
-</div>
-</div>
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-  <h3><a href="index.html">Table of Contents</a></h3>
-  <ul>
-<li><a class="reference internal" href="#">2. First Steps</a><ul>
-<li><a class="reference internal" href="#how-to-start">2.1. How to Start</a></li>
-<li><a class="reference internal" href="#the-menu-bar">2.2. The Menu Bar</a></li>
-<li><a class="reference internal" href="#the-viewing-area">2.3. The Viewing Area</a><ul>
-<li><a class="reference internal" href="#the-databases-tree-viewer">2.3.1. The Databases Tree Viewer</a></li>
-<li><a class="reference internal" href="#the-workspace">2.3.2. The Workspace</a></li>
-<li><a class="reference internal" href="#the-logger">2.3.3. The Logger</a></li>
-</ul>
-</li>
-</ul>
-</li>
-</ul>
-
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="usersguide-ch1.html"
-                        title="previous chapter">1. Introduction</a></p>
-  <h4>Next topic</h4>
-  <p class="topless"><a href="usersguide-ch3.html"
-                        title="next chapter">3. Browsing and Querying Datasets</a></p>
-  <div role="note" aria-label="source link">
-    <h3>This Page</h3>
-    <ul class="this-page-menu">
-      <li><a href="_sources/usersguide-ch2.rst.txt"
-            rel="nofollow">Show Source</a></li>
-    </ul>
-   </div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             >index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
-             >next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch1.html" title="1. Introduction"
-             >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+    <title>2. First Steps &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="3. Browsing and Querying Datasets" href="usersguide-ch3.html" />
+    <link rel="prev" title="1. Introduction" href="usersguide-ch1.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
+             accesskey="N">next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch1.html" title="1. Introduction"
+             accesskey="P">previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">2. </span>First Steps</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+  <section id="first-steps">
+<h1><span class="section-number">2. </span>First Steps<a class="headerlink" href="#first-steps" title="Permalink to this heading">¶</a></h1>
+<p>In this chapter we are going to describe briefly the main elements  that you will meet throughout your working sessions.</p>
+<section id="how-to-start">
+<h2><span class="section-number">2.1. </span>How to Start<a class="headerlink" href="#how-to-start" title="Permalink to this heading">¶</a></h2>
+<p>You can start <cite>ViTables</cite> from a desktop shortcut or from a terminal emulator.
+If you launch the program from the command line the following options are available:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables --help
+
+usage: vitables [option]... [h5file]...
+
+positional arguments:
+  h5file
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --version             show program&#39;s version number and exit
+
+h5files:
+  -m MODE, --mode MODE  mode access for a database. Can be r(ead) or a(ppend)
+  -d DBLIST, --dblist DBLIST
+                        a file with the list of HDF5 filepaths to be open
+
+logging:
+  -l LOG_FILE, --log-file LOG_FILE
+                        log file path
+  -v, --verbose         log verbosity level
+</pre></div>
+</div>
+<p>Basically you can specify a file to open or a file containing a list of files to open. For example:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables myh5file
+</pre></div>
+</div>
+<p>will start <cite>ViTables</cite> and open the file myh5file in read-write mode. If you want to open it in read-only mode then execute the command:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables -m r myh5file
+</pre></div>
+</div>
+<p>In order to open a set of files at once put them in a list file with the syntax</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">mode</span> <span class="n">path</span>
+</pre></div>
+</div>
+<p>(one pair per line) and execute:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ vitables -d h5list
+</pre></div>
+</div>
+<p>Once the application is running the <a class="reference internal" href="#main-window"><span class="std std-ref">main window</span></a> appears. It consists of a <a class="reference internal" href="#menu-bar"><span class="std std-ref">menu bar</span></a>, a set of tool bars, a <a class="reference internal" href="#viewing-area"><span class="std std-ref">viewing area</span></a> and a status bar.</p>
+<p>The viewing area of the window is divided into three parts. The <a class="reference internal" href="#tree-pane"><span class="std std-ref">tree of databases viewer</span></a> is the narrow region placed at top left side. It will display a tree representation of the data hierarchies we want to access. The big panel next to the tree viewer is called the <a class="reference internal" href="#workspace"><span class="std std-ref">workspace</span></a>, and will display the real data contained in a given node of the data hierarchy. Finally, the bottom region is the <a class="reference internal" href="#logger"><span class="std std-ref">logger</span></a>, a kind of text non interactive console where information about your requested operations will be shown.</p>
+<p>As usual, you can launch commands from the menu bar, from
+context menus or, if a shortcut button is available, from a toolbar.
+Also keyboard shortcuts are available for most commands.</p>
+<p>After starting your session, you are likely to open some files. Just drag the file(s) you want to open into the tree of databases viewer and they will be opened in read-write mode. Opening can be done from the file manager dialog too; simply issue an open command, <span class="menuselection">File ‣ Open File</span> (<kbd class="kbd compound docutils literal notranslate"><kbd class="kbd docutils literal notranslate">Ctrl</kbd>-<kbd class="kbd docutils literal notranslate">O</kbd></kbd>) and choose a file.</p>
+<figure class="align-center" id="id1">
+<span id="main-window"></span><a class="reference internal image-reference" href="_images/mainWindow.png"><img alt="_images/mainWindow.png" src="_images/mainWindow.png" style="width: 90%;" /></a>
+<figcaption>
+<p><span class="caption-text">The main window</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+</section>
+<section id="the-menu-bar">
+<span id="menu-bar"></span><h2><span class="section-number">2.2. </span>The Menu Bar<a class="headerlink" href="#the-menu-bar" title="Permalink to this heading">¶</a></h2>
+<p>The menu bar is placed at top of the main window. It is composed of six pulldown menus.</p>
+<p><strong>File menu</strong></p>
+<p>This menu contains commands to manipulate files in several ways: open, close, create, save and so on. It also gives to you quick access to the most recently opened files.</p>
+<p><strong>Node menu</strong></p>
+<p>The <span class="guilabel">Node</span> menu contains commands to manipulate the nodes displayed in the tree of databases viewer. From this menu you can edit nodes in a variety of ways as well as access their properties.</p>
+<p><strong>Dataset menu</strong></p>
+<p>With this menu you can make selects in any table (the result of your selects will be available under the Query Results node in the tree pane). The number of entries for this menu depends on the list of enabled plugins.</p>
+<p><strong>Settings menu</strong></p>
+<p>This is the menu from which the application can be customized.
+Customization includes startup behavior, look and feel and plugins management. You can add/remove paths for loading plugins, enable and disable plugins. Changes in the enabled/disabled status of a given plugin take effect after restarting <cite>ViTables</cite>.  See <a class="reference internal" href="usersguide-ch5.html#configuration-chapter"><span class="std std-ref">the ViTables Configuration chapter</span></a> for more information on this subject.</p>
+<p>Also from this menu you can show, hide and line up the application toolbars. At the moment four toolbars are available, <span class="guilabel">File</span>, <span class="guilabel">Node</span>, <span class="guilabel">Query</span> and <span class="guilabel">Help</span>.</p>
+<p><strong>Window menu</strong></p>
+<p>The <span class="guilabel">Window</span> menu can be used to change the arrangement of the workspace contents, sorting the open windows as a cascade or as a tile. By selecting a window name from this menu, you can raise (bring to the front) that window. Any open window can be closed from this menu.</p>
+<p><strong>Help menu</strong></p>
+<p>The <span class="guilabel">Help</span> menu displays this User’s Guide in :<cite>HTML4</cite> format and a couple of <em>About</em> boxes, one for the <cite>ViTables</cite> itself and one for the underlying Qt libraries. The <span class="guilabel">Show Versions</span> entry shows the version numbers of the libraries being used by <cite>ViTables</cite> (Qt, PyQt, PyTables and PyTables related libraries, like Zlib or <cite>LZO</cite>). Finally, from this menu you can enter the <em>What’s This</em> mode which will show context help for the components of the viewing area (the databases tree viewer, the workspace and the logger).</p>
+</section>
+<section id="the-viewing-area">
+<span id="viewing-area"></span><h2><span class="section-number">2.3. </span>The Viewing Area<a class="headerlink" href="#the-viewing-area" title="Permalink to this heading">¶</a></h2>
+<p>As mentioned before, the viewing area is divided into three regions: the databases tree viewer (also called tree pane), the workspace and the logger. Now we are going to describe these regions in more detail.</p>
+<section id="the-databases-tree-viewer">
+<span id="tree-pane"></span><h3><span class="section-number">2.3.1. </span>The Databases Tree Viewer<a class="headerlink" href="#the-databases-tree-viewer" title="Permalink to this heading">¶</a></h3>
+<p>Due to the hierarchical model of the underlying <cite>HDF5</cite> library, PyTables files store their data on disk in a tree-like structure. Every time you open a PyTables file, its so-called object tree (a representation of the data hierarchy) is dynamically created and added to the tree of databases viewer, at the top left side of the viewing area (see <a class="reference internal" href="#main-window"><span class="std std-ref">the main window Figure</span></a>).</p>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>since PyTables-1.2 the object tree of an opened file is made on demand: nodes are added to the tree when they are accessed. <cite>ViTables</cite> makes use of this feature, which results in stunningly fast opening times for files with a large number of nodes.</p>
+</div>
+<p>Any object tree is made of nodes which can be classified as follows:</p>
+<blockquote>
+<div><dl class="simple">
+<dt>Root node</dt><dd><p>It is the node from which all other nodes hang.</p>
+</dd>
+<dt>Groups</dt><dd><p>Groups are nodes that can contain other nodes.</p>
+</dd>
+<dt>Leaves</dt><dd><p>Leaves are nodes that contain real data. They can be tables or arrays.</p>
+</dd>
+</dl>
+</div></blockquote>
+<p>Working with object trees is really easy. By double-clicking
+on it, a root node is opened, and the tree structure below it is displayed. Groups are presented as folders. They can be expanded with a double-click, giving you immediate access to their contents. A group can contain groups and/or leaves (or
+may be empty). A double click on a leaf will display its content on the workspace. You can access the available options for a given node just with a right mouse click on it. A context menu will appear from which commands can be launched. The contents of the menu depend on the kind of node being clicked (root nodes, groups, tables and arrays have all of
+them their own context menu). Alternatively you can select the node with a single mouse click and choose a command from the
+<span class="guilabel">Node</span> menu. There is also a context menu
+for the tree pane itself that will pop up by right-clicking any empty area of the tree viewer. Last but not least, the object tree can be navigated with the keyboard too. Pressing the Enter key the selected node will be expanded (if it is a group) or opened (if it is a leaf). The + and - keys expand an collapse groups.</p>
+<p>Every node in a given object tree has an associated icon that
+allows you to identify its type quickly. The following icons are available:</p>
+<figure class="align-center" id="id2">
+<span id="node-symbols"></span><img alt="_images/treeSymbols.png" src="_images/treeSymbols.png" />
+<figcaption>
+<p><span class="caption-text">The node symbols</span><a class="headerlink" href="#id2" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+</section>
+<section id="the-workspace">
+<span id="workspace"></span><h3><span class="section-number">2.3.2. </span>The Workspace<a class="headerlink" href="#the-workspace" title="Permalink to this heading">¶</a></h3>
+<p>At this point you should have one or more files opened, and their object trees displayed in the databases tree viewer. Your next step will be to select a leaf and display its data. Remember that the object tree imitates the structure on disk, which makes it very easy to browse the hierarchy of the file and locate the leaf you want to open.</p>
+<p>A double-click on a leaf of your choice will open it and display its contents in a window (a <em>view</em> in the
+<cite>ViTables</cite> jargon) placed in the workspace, the big panel at the top right side of the viewing area (see <a class="reference internal" href="#main-window"><span class="std std-ref">the main window Figure</span></a>).</p>
+<p>Note that the databases tree viewer and the workspace are always synchronized: if you select a node in the tree viewer and that node has a view, then that view becomes the active view on the workspace. The opposite is also true, click on a view on the workspace and its node will be automatically selected on the databases tree viewer.</p>
+<p>The <span class="guilabel">Window</span> pulldown menu provides some
+additional commands that will help you to manage your
+views. From this menu you can, for instance, rearrange views, see the list of views (which is particularly useful when the workspace is cluttered with so many views that it’s difficult to find the one you want) or close all the views at once.</p>
+<p>There is also a context menu for the workspace. It can be used to change the workspace view mode: you can display views as regular windows (default behavior) or with tabs in a tab bar. In addition it give you access to the <span class="guilabel">Window</span> pulldown menu.</p>
+</section>
+<section id="the-logger">
+<span id="logger"></span><h3><span class="section-number">2.3.3. </span>The Logger<a class="headerlink" href="#the-logger" title="Permalink to this heading">¶</a></h3>
+<p>The logger is a read-only (i.e. non interactive) console placed at the bottom of the viewing area (see <a class="reference internal" href="#main-window"><span class="std std-ref">the main window Figure</span></a>). It is an info panel where <cite>ViTables</cite> reports the result of requested operations (namely if they were not successful). Also runtime errors are caught and reported to you through the logger (so you can mail the error to <cite>ViTables</cite>
+developers and help to improve the quality of the package :-). Errors and warning messages are highlighted in red and orange respectively.</p>
+<p>Of course there is also a context menu for the logger that
+provides you with some handy operations, like to copy selected text or to empty the logger.</p>
+</section>
+</section>
+</section>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+  <div>
+    <h3><a href="index.html">Table of Contents</a></h3>
+    <ul>
+<li><a class="reference internal" href="#">2. First Steps</a><ul>
+<li><a class="reference internal" href="#how-to-start">2.1. How to Start</a></li>
+<li><a class="reference internal" href="#the-menu-bar">2.2. The Menu Bar</a></li>
+<li><a class="reference internal" href="#the-viewing-area">2.3. The Viewing Area</a><ul>
+<li><a class="reference internal" href="#the-databases-tree-viewer">2.3.1. The Databases Tree Viewer</a></li>
+<li><a class="reference internal" href="#the-workspace">2.3.2. The Workspace</a></li>
+<li><a class="reference internal" href="#the-logger">2.3.3. The Logger</a></li>
+</ul>
+</li>
+</ul>
+</li>
+</ul>
+
+  </div>
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="usersguide-ch1.html"
+                          title="previous chapter"><span class="section-number">1. </span>Introduction</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="usersguide-ch3.html"
+                          title="next chapter"><span class="section-number">3. </span>Browsing and Querying Datasets</a></p>
+  </div>
+  <div role="note" aria-label="source link">
+    <h3>This Page</h3>
+    <ul class="this-page-menu">
+      <li><a href="_sources/usersguide-ch2.rst.txt"
+            rel="nofollow">Show Source</a></li>
+    </ul>
+   </div>
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             >index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
+             >next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch1.html" title="1. Introduction"
+             >previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">2. </span>First Steps</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,16 @@
 
 
 
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 2. First Steps
 ****** 2. First StepsÂ¶ ******
 In this chapter we are going to describe briefly the main elements that you
 will meet throughout your working sessions.
 ***** 2.1. How to StartÂ¶ *****
 You can startViTablesfrom a desktop shortcut or from a terminal emulator. If
 you launch the program from the command line the following options are
 available:
@@ -59,16 +60,17 @@
 a shortcut button is available, from a toolbar. Also keyboard shortcuts are
 available for most commands.
 After starting your session, you are likely to open some files. Just drag the
 file(s) you want to open into the tree of databases viewer and they will be
 opened in read-write mode. Opening can be done from the file manager dialog
 too; simply issue an open command, File â£ Open File (Ctrl-O) and choose a
 file.
-[_images/mainWindow.png]
+ [_images/mainWindow.png]
 The main windowÂ¶
+
 ***** 2.2. The Menu BarÂ¶ *****
 The menu bar is placed at top of the main window. It is composed of six
 pulldown menus.
 File menu
 This menu contains commands to manipulate files in several ways: open, close,
 create, save and so on. It also gives to you quick access to the most recently
 opened files.
@@ -97,14 +99,15 @@
 The Help menu displays this Userâs Guide in :HTML4format and a couple of
 About boxes, one for theViTablesitself and one for the underlying Qt libraries.
 The Show Versions entry shows the version numbers of the libraries being used
 byViTables(Qt, PyQt, PyTables and PyTables related libraries, like Zlib orLZO).
 Finally, from this menu you can enter the Whatâs This mode which will show
 context help for the components of the viewing area (the databases tree viewer,
 the workspace and the logger).
+
 ***** 2.3. The Viewing AreaÂ¶ *****
 As mentioned before, the viewing area is divided into three regions: the
 databases tree viewer (also called tree pane), the workspace and the logger.
 Now we are going to describe these regions in more detail.
 **** 2.3.1. The Databases Tree ViewerÂ¶ ****
 Due to the hierarchical model of the underlyingHDF5library, PyTables files
 store their data on disk in a tree-like structure. Every time you open a
@@ -137,16 +140,17 @@
 command from the Node menu. There is also a context menu for the tree pane
 itself that will pop up by right-clicking any empty area of the tree viewer.
 Last but not least, the object tree can be navigated with the keyboard too.
 Pressing the Enter key the selected node will be expanded (if it is a group) or
 opened (if it is a leaf). The + and - keys expand an collapse groups.
 Every node in a given object tree has an associated icon that allows you to
 identify its type quickly. The following icons are available:
-[_images/treeSymbols.png]
+ [_images/treeSymbols.png]
 The node symbolsÂ¶
+
 **** 2.3.2. The WorkspaceÂ¶ ****
 At this point you should have one or more files opened, and their object trees
 displayed in the databases tree viewer. Your next step will be to select a leaf
 and display its data. Remember that the object tree imitates the structure on
 disk, which makes it very easy to browse the hierarchy of the file and locate
 the leaf you want to open.
 A double-click on a leaf of your choice will open it and display its contents
@@ -162,24 +166,26 @@
 see the list of views (which is particularly useful when the workspace is
 cluttered with so many views that itâs difficult to find the one you want) or
 close all the views at once.
 There is also a context menu for the workspace. It can be used to change the
 workspace view mode: you can display views as regular windows (default
 behavior) or with tabs in a tab bar. In addition it give you access to the
 Window pulldown menu.
+
 **** 2.3.3. The LoggerÂ¶ ****
 The logger is a read-only (i.e. non interactive) console placed at the bottom
 of the viewing area (see the_main_window_Figure). It is an info panel
 whereViTablesreports the result of requested operations (namely if they were
 not successful). Also runtime errors are caught and reported to you through the
 logger (so you can mail the error toViTablesdevelopers and help to improve the
 quality of the package :-). Errors and warning messages are highlighted in red
 and orange respectively.
 Of course there is also a context menu for the logger that provides you with
 some handy operations, like to copy selected text or to empty the logger.
+
 **** Table_of_Contents ****
     * 2._First_Steps
           o 2.1._How_to_Start
           o 2.2._The_Menu_Bar
           o 2.3._The_Viewing_Area
                 # 2.3.1._The_Databases_Tree_Viewer
                 # 2.3.2._The_Workspace
@@ -192,9 +198,10 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 2. First Steps
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/usersguide-ch3.html` & `vitables-3.0.3/vitables/htmldocs/usersguide-ch3.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,182 +1,199 @@
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>3. Browsing and Querying Datasets &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="4. Editing Files" href="usersguide-ch4.html" />
-    <link rel="prev" title="2. First Steps" href="usersguide-ch2.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch4.html" title="4. Editing Files"
-             accesskey="N">next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch2.html" title="2. First Steps"
-             accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-  <div class="section" id="browsing-and-querying-datasets">
-<h1>3. Browsing and Querying Datasets<a class="headerlink" href="#browsing-and-querying-datasets" title="Permalink to this headline">¶</a></h1>
-<p>In this chapter we are going to describe how the information
-contained in a dataset can be navigated and filtered.</p>
-<div class="section" id="browsing-datasets">
-<h2>3.1. Browsing Datasets<a class="headerlink" href="#browsing-datasets" title="Permalink to this headline">¶</a></h2>
-<p>A noticeable aspect of views is the visualization speed. Views show data nearly as quickly as PyTables accesses them. As a consequence, very large datasets (with up to 2^64 rows) can be browsed stunningly fast.</p>
-<div class="align-center figure" id="id2">
-<span id="browse-large-dataset"></span><a class="reference internal image-reference" href="_images/browseDataset.png"><img alt="_images/browseDataset.png" src="_images/browseDataset.png" style="width: 80%;" /></a>
-<p class="caption"><span class="caption-text">Browsing a large dataset</span><a class="headerlink" href="#id2" title="Permalink to this image">¶</a></p>
-</div>
-<p>As said in the previous chapter, datasets are displayed in views. They are spreadsheet-like windows so can be navigated as you would expect: via scrollbar, keyboard or wheel of mouse.</p>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>what makes <cite>ViTables</cite> views interesting is that <em>the navigation speed is independent of the view size</em>: a table with several thousand million rows is navigated as quickly as a table with just a few dozens rows.</p>
-</div>
-<p>Another interesting feature of views is the ability to zoom in on cells that contain multidimensional data. When you double-click in a cell,
-it is displayed in its own view, reducing by two the number of
-dimensions of the displayed data. For instance, a cell containing a vector is displayed as a one column table of scalars. A cell that contains two-dimensional data will be shown as a bidimensional table of scalars. And so on. In general, a cell containing N-dimensional data will be
-displayed as a table of N-2 dimensions data. Zoom can be applied as many times as needed, so that multi-dimensional cells can be inspected until you get a table of scalars. Finally, if you try to zoom in on a cell that contains a scalar value, this value will be presented alone in a view;
-this can be useful to visualize large scalar values (for example, large strings) that doesn’t fit on regular columns.</p>
-<div class="align-center figure" id="id3">
-<span id="zoom-cell"></span><a class="reference internal image-reference" href="_images/zoomingCells.png"><img alt="_images/zoomingCells.png" src="_images/zoomingCells.png" style="width: 80%;" /></a>
-<p class="caption"><span class="caption-text">Zooming a cell</span><a class="headerlink" href="#id3" title="Permalink to this image">¶</a></p>
-</div>
-</div>
-<div class="section" id="getting-info">
-<h2>3.2. Getting Info<a class="headerlink" href="#getting-info" title="Permalink to this headline">¶</a></h2>
-<p>For a given node two kinds of information are available: metadata and data. From their metadata you can retrieve information about the objects on disk, such as table and column names, titles, number of rows, data types in columns or attributes, among others.</p>
-<p>The available metadata about a given node (group or leaf) can be accessed by right-clicking the mouse on the node and launching the <span class="guilabel">Properties</span> command from the context menu that appears. This can also be achieved from the <span class="guilabel">Node</span> menu. Then the <a class="reference internal" href="#properties-dialog"><span class="std std-ref">Properties dialog</span></a>, that contains the requested metadata, is displayed. The dialog is made of three tabs labelled as General, System attributes and User attributes. The General tab contains generic information about the selected node, i.e. name, path, etc. The System and User tabs contain tables that describe the attributes of the node.</p>
-<div class="align-center figure" id="id4">
-<span id="properties-dialog"></span><img alt="_images/propertiesDlg.png" src="_images/propertiesDlg.png" />
-<p class="caption"><span class="caption-text">The Properties dialog</span><a class="headerlink" href="#id4" title="Permalink to this image">¶</a></p>
-</div>
-<p>Aside from the Properties dialog, you can get information in
-several other ways.</p>
-<p>The full path of the node currently selected in the tree view is displayed in the status bar. This can be useful when the object tree is large and guessing a full path is not easy.</p>
-<p>The top left icon of views shows the kind of displayed data
-(array or table).</p>
-<p>Finally, some generic information can be obtained by launching the command <span class="menuselection">Help ‣ WhatIsThis</span>
-(or clicking the appropriate button on the corresponding toolbar).</p>
-</div>
-<div class="section" id="querying-tables">
-<h2>3.3. Querying Tables<a class="headerlink" href="#querying-tables" title="Permalink to this headline">¶</a></h2>
-<p>An interesting feature of <cite>ViTables</cite> is its capability to make table selections. This means that we can select a set of table rows that fulfill a given condition. You can filter any table
-(even if it is closed) by issuing the command <span class="menuselection">Dataset ‣ Query…</span>.</p>
-<p>A dialog (see <a class="reference internal" href="#query-dlg"><span class="std std-ref">this Figure</span></a>) will be displayed where you can create a query and select the range of rows to
-which the query will apply. Notice that, <em>you can make complex queries, i.e. queries that involve more than one table field.
-However the queried fields cannot be multidimensional or contain data with Complex data type</em>.</p>
-<p><cite>ViTables</cite> always do its best for not being frozen due to out of memory problems when you do complex queries or the queried table is huge (or both) but it is not guarateed that it can achieve this goal.</p>
-<p>The selected rows are stored in a new table (but not removed from its original location) that we will call filtered table from here on. Filtered tables are stored in a temporary database <a class="footnote-reference brackets" href="#f2" id="id1">1</a> labeled as <em>Query results</em> in the databases tree viewer. The <em>Query results</em> node is always placed at the bottom of the databases tree.</p>
-<p>Filtered tables can be edited as any other leaf opened in read-write mode.</p>
-<p>By default an automatic title FilteredTable_X is given to the X-th filtered table created. In addition, those tables have three user attributes that are, in principle, only defined for filtered tables. These attributes are:</p>
-<blockquote>
-<div><dl class="simple">
-<dt>query</dt><dd><p>the applied query</p>
-</dd>
-<dt>query_path</dt><dd><p>the full path of the queried file</p>
-</dd>
-<dt>query_table</dt><dd><p>the full path of the queried table in the object tree hierarchy</p>
-</dd>
-</dl>
-</div></blockquote>
-<div class="align-center figure" id="id5">
-<span id="query-dlg"></span><img alt="_images/newFilteredTable.png" src="_images/newFilteredTable.png" />
-<p class="caption"><span class="caption-text">The New Query dialog</span><a class="headerlink" href="#id5" title="Permalink to this image">¶</a></p>
-</div>
-<p class="rubric">Footnotes</p>
-<dl class="footnote brackets">
-<dt class="label" id="f2"><span class="brackets"><a class="fn-backref" href="#id1">1</a></span></dt>
-<dd><p>Every time a <cite>ViTables</cite> session starts, a new temporary database is created from scratch. This database has a flat structure and is stored with a unique name in a temporary directory so the operating system will remove it every time the directory is cleaned.</p>
-</dd>
-</dl>
-</div>
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-  <h3><a href="index.html">Table of Contents</a></h3>
-  <ul>
-<li><a class="reference internal" href="#">3. Browsing and Querying Datasets</a><ul>
-<li><a class="reference internal" href="#browsing-datasets">3.1. Browsing Datasets</a></li>
-<li><a class="reference internal" href="#getting-info">3.2. Getting Info</a></li>
-<li><a class="reference internal" href="#querying-tables">3.3. Querying Tables</a></li>
-</ul>
-</li>
-</ul>
-
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="usersguide-ch2.html"
-                        title="previous chapter">2. First Steps</a></p>
-  <h4>Next topic</h4>
-  <p class="topless"><a href="usersguide-ch4.html"
-                        title="next chapter">4. Editing Files</a></p>
-  <div role="note" aria-label="source link">
-    <h3>This Page</h3>
-    <ul class="this-page-menu">
-      <li><a href="_sources/usersguide-ch3.rst.txt"
-            rel="nofollow">Show Source</a></li>
-    </ul>
-   </div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             >index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch4.html" title="4. Editing Files"
-             >next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch2.html" title="2. First Steps"
-             >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+    <title>3. Browsing and Querying Datasets &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="4. Editing Files" href="usersguide-ch4.html" />
+    <link rel="prev" title="2. First Steps" href="usersguide-ch2.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch4.html" title="4. Editing Files"
+             accesskey="N">next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch2.html" title="2. First Steps"
+             accesskey="P">previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">3. </span>Browsing and Querying Datasets</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+  <section id="browsing-and-querying-datasets">
+<h1><span class="section-number">3. </span>Browsing and Querying Datasets<a class="headerlink" href="#browsing-and-querying-datasets" title="Permalink to this heading">¶</a></h1>
+<p>In this chapter we are going to describe how the information
+contained in a dataset can be navigated and filtered.</p>
+<section id="browsing-datasets">
+<h2><span class="section-number">3.1. </span>Browsing Datasets<a class="headerlink" href="#browsing-datasets" title="Permalink to this heading">¶</a></h2>
+<p>A noticeable aspect of views is the visualization speed. Views show data nearly as quickly as PyTables accesses them. As a consequence, very large datasets (with up to 2^64 rows) can be browsed stunningly fast.</p>
+<figure class="align-center" id="id2">
+<span id="browse-large-dataset"></span><a class="reference internal image-reference" href="_images/browseDataset.png"><img alt="_images/browseDataset.png" src="_images/browseDataset.png" style="width: 80%;" /></a>
+<figcaption>
+<p><span class="caption-text">Browsing a large dataset</span><a class="headerlink" href="#id2" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+<p>As said in the previous chapter, datasets are displayed in views. They are spreadsheet-like windows so can be navigated as you would expect: via scrollbar, keyboard or wheel of mouse.</p>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>what makes <cite>ViTables</cite> views interesting is that <em>the navigation speed is independent of the view size</em>: a table with several thousand million rows is navigated as quickly as a table with just a few dozens rows.</p>
+</div>
+<p>Another interesting feature of views is the ability to zoom in on cells that contain multidimensional data. When you double-click in a cell,
+it is displayed in its own view, reducing by two the number of
+dimensions of the displayed data. For instance, a cell containing a vector is displayed as a one column table of scalars. A cell that contains two-dimensional data will be shown as a bidimensional table of scalars. And so on. In general, a cell containing N-dimensional data will be
+displayed as a table of N-2 dimensions data. Zoom can be applied as many times as needed, so that multi-dimensional cells can be inspected until you get a table of scalars. Finally, if you try to zoom in on a cell that contains a scalar value, this value will be presented alone in a view;
+this can be useful to visualize large scalar values (for example, large strings) that doesn’t fit on regular columns.</p>
+<figure class="align-center" id="id3">
+<span id="zoom-cell"></span><a class="reference internal image-reference" href="_images/zoomingCells.png"><img alt="_images/zoomingCells.png" src="_images/zoomingCells.png" style="width: 80%;" /></a>
+<figcaption>
+<p><span class="caption-text">Zooming a cell</span><a class="headerlink" href="#id3" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+</section>
+<section id="getting-info">
+<h2><span class="section-number">3.2. </span>Getting Info<a class="headerlink" href="#getting-info" title="Permalink to this heading">¶</a></h2>
+<p>For a given node two kinds of information are available: metadata and data. From their metadata you can retrieve information about the objects on disk, such as table and column names, titles, number of rows, data types in columns or attributes, among others.</p>
+<p>The available metadata about a given node (group or leaf) can be accessed by right-clicking the mouse on the node and launching the <span class="guilabel">Properties</span> command from the context menu that appears. This can also be achieved from the <span class="guilabel">Node</span> menu. Then the <a class="reference internal" href="#properties-dialog"><span class="std std-ref">Properties dialog</span></a>, that contains the requested metadata, is displayed. The dialog is made of three tabs labelled as General, System attributes and User attributes. The General tab contains generic information about the selected node, i.e. name, path, etc. The System and User tabs contain tables that describe the attributes of the node.</p>
+<figure class="align-center" id="id4">
+<span id="properties-dialog"></span><img alt="_images/propertiesDlg.png" src="_images/propertiesDlg.png" />
+<figcaption>
+<p><span class="caption-text">The Properties dialog</span><a class="headerlink" href="#id4" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+<p>Aside from the Properties dialog, you can get information in
+several other ways.</p>
+<p>The full path of the node currently selected in the tree view is displayed in the status bar. This can be useful when the object tree is large and guessing a full path is not easy.</p>
+<p>The top left icon of views shows the kind of displayed data
+(array or table).</p>
+<p>Finally, some generic information can be obtained by launching the command <span class="menuselection">Help ‣ WhatIsThis</span>
+(or clicking the appropriate button on the corresponding toolbar).</p>
+</section>
+<section id="querying-tables">
+<h2><span class="section-number">3.3. </span>Querying Tables<a class="headerlink" href="#querying-tables" title="Permalink to this heading">¶</a></h2>
+<p>An interesting feature of <cite>ViTables</cite> is its capability to make table selections. This means that we can select a set of table rows that fulfill a given condition. You can filter any table
+(even if it is closed) by issuing the command <span class="menuselection">Dataset ‣ Query…</span>.</p>
+<p>A dialog (see <a class="reference internal" href="#query-dlg"><span class="std std-ref">this Figure</span></a>) will be displayed where you can create a query and select the range of rows to
+which the query will apply. Notice that, <em>you can make complex queries, i.e. queries that involve more than one table field.
+However the queried fields cannot be multidimensional or contain data with Complex data type</em>.</p>
+<p><cite>ViTables</cite> always do its best for not being frozen due to out of memory problems when you do complex queries or the queried table is huge (or both) but it is not guarateed that it can achieve this goal.</p>
+<p>The selected rows are stored in a new table (but not removed from its original location) that we will call filtered table from here on. Filtered tables are stored in a temporary database <a class="footnote-reference brackets" href="#f2" id="id1" role="doc-noteref"><span class="fn-bracket">[</span>1<span class="fn-bracket">]</span></a> labeled as <em>Query results</em> in the databases tree viewer. The <em>Query results</em> node is always placed at the bottom of the databases tree.</p>
+<p>Filtered tables can be edited as any other leaf opened in read-write mode.</p>
+<p>By default an automatic title FilteredTable_X is given to the X-th filtered table created. In addition, those tables have three user attributes that are, in principle, only defined for filtered tables. These attributes are:</p>
+<blockquote>
+<div><dl class="simple">
+<dt>query</dt><dd><p>the applied query</p>
+</dd>
+<dt>query_path</dt><dd><p>the full path of the queried file</p>
+</dd>
+<dt>query_table</dt><dd><p>the full path of the queried table in the object tree hierarchy</p>
+</dd>
+</dl>
+</div></blockquote>
+<figure class="align-center" id="id5">
+<span id="query-dlg"></span><img alt="_images/newFilteredTable.png" src="_images/newFilteredTable.png" />
+<figcaption>
+<p><span class="caption-text">The New Query dialog</span><a class="headerlink" href="#id5" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+<p class="rubric">Footnotes</p>
+<aside class="footnote-list brackets">
+<aside class="footnote brackets" id="f2" role="doc-footnote">
+<span class="label"><span class="fn-bracket">[</span><a role="doc-backlink" href="#id1">1</a><span class="fn-bracket">]</span></span>
+<p>Every time a <cite>ViTables</cite> session starts, a new temporary database is created from scratch. This database has a flat structure and is stored with a unique name in a temporary directory so the operating system will remove it every time the directory is cleaned.</p>
+</aside>
+</aside>
+</section>
+</section>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+  <div>
+    <h3><a href="index.html">Table of Contents</a></h3>
+    <ul>
+<li><a class="reference internal" href="#">3. Browsing and Querying Datasets</a><ul>
+<li><a class="reference internal" href="#browsing-datasets">3.1. Browsing Datasets</a></li>
+<li><a class="reference internal" href="#getting-info">3.2. Getting Info</a></li>
+<li><a class="reference internal" href="#querying-tables">3.3. Querying Tables</a></li>
+</ul>
+</li>
+</ul>
+
+  </div>
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="usersguide-ch2.html"
+                          title="previous chapter"><span class="section-number">2. </span>First Steps</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="usersguide-ch4.html"
+                          title="next chapter"><span class="section-number">4. </span>Editing Files</a></p>
+  </div>
+  <div role="note" aria-label="source link">
+    <h3>This Page</h3>
+    <ul class="this-page-menu">
+      <li><a href="_sources/usersguide-ch3.rst.txt"
+            rel="nofollow">Show Source</a></li>
+    </ul>
+   </div>
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             >index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch4.html" title="4. Editing Files"
+             >next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch2.html" title="2. First Steps"
+             >previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">3. </span>Browsing and Querying Datasets</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -4,24 +4,26 @@
 
 
 
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 3. Browsing and Querying Datasets
 ****** 3. Browsing and Querying DatasetsÂ¶ ******
 In this chapter we are going to describe how the information contained in a
 dataset can be navigated and filtered.
 ***** 3.1. Browsing DatasetsÂ¶ *****
 A noticeable aspect of views is the visualization speed. Views show data nearly
 as quickly as PyTables accesses them. As a consequence, very large datasets
 (with up to 2^64 rows) can be browsed stunningly fast.
-[_images/browseDataset.png]
+ [_images/browseDataset.png]
 Browsing a large datasetÂ¶
+
 As said in the previous chapter, datasets are displayed in views. They are
 spreadsheet-like windows so can be navigated as you would expect: via
 scrollbar, keyboard or wheel of mouse.
 Note
 what makesViTablesviews interesting is that the navigation speed is independent
 of the view size: a table with several thousand million rows is navigated as
 quickly as a table with just a few dozens rows.
@@ -33,40 +35,43 @@
 bidimensional table of scalars. And so on. In general, a cell containing N-
 dimensional data will be displayed as a table of N-2 dimensions data. Zoom can
 be applied as many times as needed, so that multi-dimensional cells can be
 inspected until you get a table of scalars. Finally, if you try to zoom in on a
 cell that contains a scalar value, this value will be presented alone in a
 view; this can be useful to visualize large scalar values (for example, large
 strings) that doesnât fit on regular columns.
-[_images/zoomingCells.png]
+ [_images/zoomingCells.png]
 Zooming a cellÂ¶
+
 ***** 3.2. Getting InfoÂ¶ *****
 For a given node two kinds of information are available: metadata and data.
 From their metadata you can retrieve information about the objects on disk,
 such as table and column names, titles, number of rows, data types in columns
 or attributes, among others.
 The available metadata about a given node (group or leaf) can be accessed by
 right-clicking the mouse on the node and launching the Properties command from
 the context menu that appears. This can also be achieved from the Node menu.
 Then the Properties_dialog, that contains the requested metadata, is displayed.
 The dialog is made of three tabs labelled as General, System attributes and
 User attributes. The General tab contains generic information about the
 selected node, i.e. name, path, etc. The System and User tabs contain tables
 that describe the attributes of the node.
-[_images/propertiesDlg.png]
+ [_images/propertiesDlg.png]
 The Properties dialogÂ¶
+
 Aside from the Properties dialog, you can get information in several other
 ways.
 The full path of the node currently selected in the tree view is displayed in
 the status bar. This can be useful when the object tree is large and guessing a
 full path is not easy.
 The top left icon of views shows the kind of displayed data (array or table).
 Finally, some generic information can be obtained by launching the command Help
 â£ WhatIsThis (or clicking the appropriate button on the corresponding
 toolbar).
+
 ***** 3.3. Querying TablesÂ¶ *****
 An interesting feature ofViTablesis its capability to make table selections.
 This means that we can select a set of table rows that fulfill a given
 condition. You can filter any table (even if it is closed) by issuing the
 command Dataset â£ Queryâ¦.
 A dialog (see this_Figure) will be displayed where you can create a query and
 select the range of rows to which the query will apply. Notice that, you can
@@ -74,35 +79,37 @@
 However the queried fields cannot be multidimensional or contain data with
 Complex data type.
 ViTablesalways do its best for not being frozen due to out of memory problems
 when you do complex queries or the queried table is huge (or both) but it is
 not guarateed that it can achieve this goal.
 The selected rows are stored in a new table (but not removed from its original
 location) that we will call filtered table from here on. Filtered tables are
-stored in a temporary database 1 labeled as Query results in the databases tree
-viewer. The Query results node is always placed at the bottom of the databases
-tree.
+stored in a temporary database [1] labeled as Query results in the databases
+tree viewer. The Query results node is always placed at the bottom of the
+databases tree.
 Filtered tables can be edited as any other leaf opened in read-write mode.
 By default an automatic title FilteredTable_X is given to the X-th filtered
 table created. In addition, those tables have three user attributes that are,
 in principle, only defined for filtered tables. These attributes are:
        query
            the applied query
        query_path
            the full path of the queried file
        query_table
            the full path of the queried table in the object tree hierarchy
-[_images/newFilteredTable.png]
+ [_images/newFilteredTable.png]
 The New Query dialogÂ¶
+
 Footnotes
-  1
-      Every time aViTablessession starts, a new temporary database is created
-      from scratch. This database has a flat structure and is stored with a
-      unique name in a temporary directory so the operating system will remove
-      it every time the directory is cleaned.
+  [1]
+Every time aViTablessession starts, a new temporary database is created from
+scratch. This database has a flat structure and is stored with a unique name in
+a temporary directory so the operating system will remove it every time the
+directory is cleaned.
+
 **** Table_of_Contents ****
     * 3._Browsing_and_Querying_Datasets
           o 3.1._Browsing_Datasets
           o 3.2._Getting_Info
           o 3.3._Querying_Tables
 *** Previous topic ***
 2._First_Steps
@@ -112,9 +119,10 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 3. Browsing and Querying Datasets
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/usersguide-ch4.html` & `vitables-3.0.3/vitables/htmldocs/usersguide-ch4.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,159 @@
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>4. Editing Files &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="5. Configuring ViTables" href="usersguide-ch5.html" />
-    <link rel="prev" title="3. Browsing and Querying Datasets" href="usersguide-ch3.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
-             accesskey="N">next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
-             accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-  <div class="section" id="editing-files">
-<h1>4. Editing Files<a class="headerlink" href="#editing-files" title="Permalink to this headline">¶</a></h1>
-<p>In this chapter we are going to describe briefly the editing
-capabilities of <cite>ViTables</cite>.</p>
-<div class="section" id="creating-complex-hierarchies">
-<h2>4.1. Creating Complex Hierarchies<a class="headerlink" href="#creating-complex-hierarchies" title="Permalink to this headline">¶</a></h2>
-<p><cite>ViTables</cite> supports a complete set of editing operations on files and nodes. The result of these operations is made immediately visible on the databases tree viewer.</p>
-<p>To create a new file in write mode, just issue the command <span class="menuselection">File ‣ New…</span> (<kbd class="kbd docutils literal notranslate">Ctrl-N</kbd>). By default, the file will be created with a <code class="docutils literal notranslate"><span class="pre">.h5</span></code> extension but you can provide your desired extension.</p>
-<p>You can add new empty groups to a writable file as easily as you
-create a new file. Simply select a group on the the tree pane and launch the command <span class="menuselection">Node ‣ New group…</span>. A new, empty group will be added to the previously selected group. By combining this operation with file creation, you can easily create complex hierarchies. Later on, you can populate the hierarchies with real data using your PyTables programs.</p>
-<div class="align-center figure" id="id1">
-<span id="group-creation"></span><a class="reference internal image-reference" href="_images/groupCreation.png"><img alt="_images/groupCreation.png" src="_images/groupCreation.png" style="width: 80%;" /></a>
-<p class="caption"><span class="caption-text">Creating a new group</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
-</div>
-</div>
-<div class="section" id="editing-object-trees">
-<h2>4.2. Editing Object Trees<a class="headerlink" href="#editing-object-trees" title="Permalink to this headline">¶</a></h2>
-<p>Files opened in write mode can be modified by moving their nodes (groups and leaves) around. From the <span class="guilabel">Node</span>
-menu you can copy, paste, cut, rename or delete any selected node (except root groups). Typical keyboard shortcuts are available for copy and paste operations. Of course, you can drag and drop nodes from one location to a different one using the mouse.</p>
-<p>Nodes can be moved to a different location in the object tree, but can also be reallocated in a different file. This way you can <em>merge</em> open files in a very flexible and comfortable
-way.</p>
-<p>As usual, while an operation is being performed on a given node, the shape of the mouse cursor will change into a clock, reminding you that a PyTables operation is being executed.</p>
-<p>Given a node opened in read-write mode you can edit its user attributes from the User attributes page (see <a class="reference internal" href="#editing-user-attributes"><span class="std std-ref">this Figure</span></a>) in the node Properties dialog. This page contains the user attributes table. You can add and remove attributes with the respective buttons or you can edit any existing attribute by clicking the table cell that you want to modify and introducing the new value. This way you can change name, value and type of any existing attribute.</p>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>multidimensional attribute values are not supported by <cite>ViTables</cite>. Also be aware that scalar attributes will be saved as scalar Numpy objects instead of serialized using cPickle (which used to be the default PyTables behavior). This way you will be able to read them using generic <cite>HDF5</cite> tools, not just PyTables.</p>
-</div>
-<p>Finally, the value of the TITLE system attribute can also be
-edited. Just click its cell in the System Attributes tab and enter the desired value.</p>
-<div class="align-center figure" id="id2">
-<span id="editing-user-attributes"></span><img alt="_images/editingUserAttrs.png" src="_images/editingUserAttrs.png" />
-<p class="caption"><span class="caption-text">Editing user attributes</span><a class="headerlink" href="#id2" title="Permalink to this image">¶</a></p>
-</div>
-</div>
-<div class="section" id="editing-leaves">
-<h2>4.3. Editing Leaves<a class="headerlink" href="#editing-leaves" title="Permalink to this headline">¶</a></h2>
-<p>At the moment of writing, editing the real data stored in leaves
-has not yet been implemented.</p>
-</div>
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-  <h3><a href="index.html">Table of Contents</a></h3>
-  <ul>
-<li><a class="reference internal" href="#">4. Editing Files</a><ul>
-<li><a class="reference internal" href="#creating-complex-hierarchies">4.1. Creating Complex Hierarchies</a></li>
-<li><a class="reference internal" href="#editing-object-trees">4.2. Editing Object Trees</a></li>
-<li><a class="reference internal" href="#editing-leaves">4.3. Editing Leaves</a></li>
-</ul>
-</li>
-</ul>
-
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="usersguide-ch3.html"
-                        title="previous chapter">3. Browsing and Querying Datasets</a></p>
-  <h4>Next topic</h4>
-  <p class="topless"><a href="usersguide-ch5.html"
-                        title="next chapter">5. Configuring ViTables</a></p>
-  <div role="note" aria-label="source link">
-    <h3>This Page</h3>
-    <ul class="this-page-menu">
-      <li><a href="_sources/usersguide-ch4.rst.txt"
-            rel="nofollow">Show Source</a></li>
-    </ul>
-   </div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             >index</a></li>
-        <li class="right" >
-          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
-             >next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
-             >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+    <title>4. Editing Files &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="5. Configuring ViTables" href="usersguide-ch5.html" />
+    <link rel="prev" title="3. Browsing and Querying Datasets" href="usersguide-ch3.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
+             accesskey="N">next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
+             accesskey="P">previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">4. </span>Editing Files</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+  <section id="editing-files">
+<h1><span class="section-number">4. </span>Editing Files<a class="headerlink" href="#editing-files" title="Permalink to this heading">¶</a></h1>
+<p>In this chapter we are going to describe briefly the editing
+capabilities of <cite>ViTables</cite>.</p>
+<section id="creating-complex-hierarchies">
+<h2><span class="section-number">4.1. </span>Creating Complex Hierarchies<a class="headerlink" href="#creating-complex-hierarchies" title="Permalink to this heading">¶</a></h2>
+<p><cite>ViTables</cite> supports a complete set of editing operations on files and nodes. The result of these operations is made immediately visible on the databases tree viewer.</p>
+<p>To create a new file in write mode, just issue the command <span class="menuselection">File ‣ New…</span> (<kbd class="kbd compound docutils literal notranslate"><kbd class="kbd docutils literal notranslate">Ctrl</kbd>-<kbd class="kbd docutils literal notranslate">N</kbd></kbd>). By default, the file will be created with a <code class="docutils literal notranslate"><span class="pre">.h5</span></code> extension but you can provide your desired extension.</p>
+<p>You can add new empty groups to a writable file as easily as you
+create a new file. Simply select a group on the the tree pane and launch the command <span class="menuselection">Node ‣ New group…</span>. A new, empty group will be added to the previously selected group. By combining this operation with file creation, you can easily create complex hierarchies. Later on, you can populate the hierarchies with real data using your PyTables programs.</p>
+<figure class="align-center" id="id1">
+<span id="group-creation"></span><a class="reference internal image-reference" href="_images/groupCreation.png"><img alt="_images/groupCreation.png" src="_images/groupCreation.png" style="width: 80%;" /></a>
+<figcaption>
+<p><span class="caption-text">Creating a new group</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+</section>
+<section id="editing-object-trees">
+<h2><span class="section-number">4.2. </span>Editing Object Trees<a class="headerlink" href="#editing-object-trees" title="Permalink to this heading">¶</a></h2>
+<p>Files opened in write mode can be modified by moving their nodes (groups and leaves) around. From the <span class="guilabel">Node</span>
+menu you can copy, paste, cut, rename or delete any selected node (except root groups). Typical keyboard shortcuts are available for copy and paste operations. Of course, you can drag and drop nodes from one location to a different one using the mouse.</p>
+<p>Nodes can be moved to a different location in the object tree, but can also be reallocated in a different file. This way you can <em>merge</em> open files in a very flexible and comfortable
+way.</p>
+<p>As usual, while an operation is being performed on a given node, the shape of the mouse cursor will change into a clock, reminding you that a PyTables operation is being executed.</p>
+<p>Given a node opened in read-write mode you can edit its user attributes from the User attributes page (see <a class="reference internal" href="#editing-user-attributes"><span class="std std-ref">this Figure</span></a>) in the node Properties dialog. This page contains the user attributes table. You can add and remove attributes with the respective buttons or you can edit any existing attribute by clicking the table cell that you want to modify and introducing the new value. This way you can change name, value and type of any existing attribute.</p>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>multidimensional attribute values are not supported by <cite>ViTables</cite>. Also be aware that scalar attributes will be saved as scalar Numpy objects instead of serialized using cPickle (which used to be the default PyTables behavior). This way you will be able to read them using generic <cite>HDF5</cite> tools, not just PyTables.</p>
+</div>
+<p>Finally, the value of the TITLE system attribute can also be
+edited. Just click its cell in the System Attributes tab and enter the desired value.</p>
+<figure class="align-center" id="id2">
+<span id="editing-user-attributes"></span><img alt="_images/editingUserAttrs.png" src="_images/editingUserAttrs.png" />
+<figcaption>
+<p><span class="caption-text">Editing user attributes</span><a class="headerlink" href="#id2" title="Permalink to this image">¶</a></p>
+</figcaption>
+</figure>
+</section>
+<section id="editing-leaves">
+<h2><span class="section-number">4.3. </span>Editing Leaves<a class="headerlink" href="#editing-leaves" title="Permalink to this heading">¶</a></h2>
+<p>At the moment of writing, editing the real data stored in leaves
+has not yet been implemented.</p>
+</section>
+</section>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+  <div>
+    <h3><a href="index.html">Table of Contents</a></h3>
+    <ul>
+<li><a class="reference internal" href="#">4. Editing Files</a><ul>
+<li><a class="reference internal" href="#creating-complex-hierarchies">4.1. Creating Complex Hierarchies</a></li>
+<li><a class="reference internal" href="#editing-object-trees">4.2. Editing Object Trees</a></li>
+<li><a class="reference internal" href="#editing-leaves">4.3. Editing Leaves</a></li>
+</ul>
+</li>
+</ul>
+
+  </div>
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="usersguide-ch3.html"
+                          title="previous chapter"><span class="section-number">3. </span>Browsing and Querying Datasets</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="usersguide-ch5.html"
+                          title="next chapter"><span class="section-number">5. </span>Configuring ViTables</a></p>
+  </div>
+  <div role="note" aria-label="source link">
+    <h3>This Page</h3>
+    <ul class="this-page-menu">
+      <li><a href="_sources/usersguide-ch4.rst.txt"
+            rel="nofollow">Show Source</a></li>
+    </ul>
+   </div>
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             >index</a></li>
+        <li class="right" >
+          <a href="usersguide-ch5.html" title="5. Configuring ViTables"
+             >next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch3.html" title="3. Browsing and Querying Datasets"
+             >previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">4. </span>Editing Files</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,16 @@
 
 
 
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 4. Editing Files
 ****** 4. Editing FilesÂ¶ ******
 In this chapter we are going to describe briefly the editing capabilities
 ofViTables.
 ***** 4.1. Creating Complex HierarchiesÂ¶ *****
 ViTablessupports a complete set of editing operations on files and nodes. The
 result of these operations is made immediately visible on the databases tree
 viewer.
@@ -21,16 +22,17 @@
 provide your desired extension.
 You can add new empty groups to a writable file as easily as you create a new
 file. Simply select a group on the the tree pane and launch the command Node
 â£ New groupâ¦. A new, empty group will be added to the previously selected
 group. By combining this operation with file creation, you can easily create
 complex hierarchies. Later on, you can populate the hierarchies with real data
 using your PyTables programs.
-[_images/groupCreation.png]
+ [_images/groupCreation.png]
 Creating a new groupÂ¶
+
 ***** 4.2. Editing Object TreesÂ¶ *****
 Files opened in write mode can be modified by moving their nodes (groups and
 leaves) around. From the Node menu you can copy, paste, cut, rename or delete
 any selected node (except root groups). Typical keyboard shortcuts are
 available for copy and paste operations. Of course, you can drag and drop nodes
 from one location to a different one using the mouse.
 Nodes can be moved to a different location in the object tree, but can also be
@@ -48,19 +50,21 @@
 Note
 multidimensional attribute values are not supported byViTables. Also be aware
 that scalar attributes will be saved as scalar Numpy objects instead of
 serialized using cPickle (which used to be the default PyTables behavior). This
 way you will be able to read them using genericHDF5tools, not just PyTables.
 Finally, the value of the TITLE system attribute can also be edited. Just click
 its cell in the System Attributes tab and enter the desired value.
-[_images/editingUserAttrs.png]
+ [_images/editingUserAttrs.png]
 Editing user attributesÂ¶
+
 ***** 4.3. Editing LeavesÂ¶ *****
 At the moment of writing, editing the real data stored in leaves has not yet
 been implemented.
+
 **** Table_of_Contents ****
     * 4._Editing_Files
           o 4.1._Creating_Complex_Hierarchies
           o 4.2._Editing_Object_Trees
           o 4.3._Editing_Leaves
 *** Previous topic ***
 3._Browsing_and_Querying_Datasets
@@ -70,9 +74,10 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 4. Editing Files
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/htmldocs/usersguide-ch5.html` & `vitables-3.0.3/vitables/htmldocs/usersguide-ch5.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,165 @@
-
-<!DOCTYPE html>
-
-<html xmlns="http://www.w3.org/1999/xhtml">
-  <head>
-    <meta charset="utf-8" />
-    <title>5. Configuring ViTables &#8212; ViTables Users&#39; Guide 3.0.2 documentation</title>
-    <link rel="stylesheet" href="_static/classic.css" type="text/css" />
-    <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
-    
-    <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
-    <script type="text/javascript" src="_static/jquery.js"></script>
-    <script type="text/javascript" src="_static/underscore.js"></script>
-    <script type="text/javascript" src="_static/doctools.js"></script>
-    <script type="text/javascript" src="_static/language_data.js"></script>
-    
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="6. About Plugins" href="usersguide-app1.html" />
-    <link rel="prev" title="4. Editing Files" href="usersguide-ch4.html" /> 
-  </head><body>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             accesskey="I">index</a></li>
-        <li class="right" >
-          <a href="usersguide-app1.html" title="6. About Plugins"
-             accesskey="N">next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch4.html" title="4. Editing Files"
-             accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>  
-
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          <div class="body" role="main">
-            
-  <div class="section" id="configuring-vitables">
-<span id="configuration-chapter"></span><h1>5. Configuring ViTables<a class="headerlink" href="#configuring-vitables" title="Permalink to this headline">¶</a></h1>
-<p>As mentioned earlier, many aspects of the <cite>ViTables</cite> behaviour can be customized by you through the <span class="menuselection">Settings ‣ Preferences</span> command.</p>
-<p>It shows a dialog offering you several customization
-possibilities. The dialog is made of three stacked pages,
-<span class="guilabel">General</span>, <span class="guilabel">Look &amp; Feel</span> and <span class="guilabel">Plugins</span>.</p>
-<p>The <span class="guilabel">General</span> page allows to change the <cite>ViTables</cite> behavior at startup. You can set the initial working directory to be that one from which <cite>ViTables</cite> is starting or to be the last used working directory. And you can recover your last working session.</p>
-<p>The <span class="guilabel">Look &amp; Feel</span> page allows to change visual
-aspects of the application such as fonts, colors or even the general style, so you can adapt the global aspect of <cite>ViTables</cite> to what would be expected on your platform.</p>
-<p>From the <span class="guilabel">Plugins</span> page the plugins can be managed. You can enable or disable the available plugins. Changes in this page will take effect the next time you start <cite>ViTables</cite>.</p>
-<p>The <span class="guilabel">OK</span> button will apply the new settings and
-make them permanent by saving them in the Windows registry, in a configuration file (on Unix platforms) or in a plist file (on Mac OS X platforms). Even if settings are stored in a plain text file editing it by hand is not recommended. Some settings, like fonts or geometry settings <a class="footnote-reference brackets" href="#f3" id="id1">1</a>, are stored in a way not really intended to be modified manually.</p>
-<p>Anyway it can be worth how settings are stored so let’s do it.
-The configuration file is divided into sections, labeled as
-[section_name]. Every section is made of subsections written as key/value pairs and representing the item that is being
-customized. Currently the following sections/subsections are available:</p>
-<blockquote>
-<div><dl class="simple">
-<dt>[Geometry] HSplitter</dt><dd><p>the size of the horizontal splitter</p>
-</dd>
-<dt>[Geometry] Layout</dt><dd><p>the position and size of toolbars and dock widgets</p>
-</dd>
-<dt>[Geometry] Position</dt><dd><p>the position and size of the application window</p>
-</dd>
-<dt>[Geometry] VSplitter</dt><dd><p>the size of the vertical splitter</p>
-</dd>
-<dt>[HelpBrowser] Bookmarks</dt><dd><p>the list of current bookmarks of the help browser</p>
-</dd>
-<dt>[HelpBrowser] History</dt><dd><p>the navigation history of the help browser</p>
-</dd>
-<dt>[Logger] Font</dt><dd><p>the logger font</p>
-</dd>
-<dt>[Logger] Paper</dt><dd><p>the logger background color</p>
-</dd>
-<dt>[Logger] Text</dt><dd><p>the logger text color</p>
-</dd>
-<dt>[Look] currentStyle</dt><dd><p>the style that defines the application look &amp; feel. Available styles fit the most common platforms, i.e., Windows, Unix (Motif and SGI flavors), and Macintosh</p>
-</dd>
-<dt>[Plugins] Enabled</dt><dd><p>the list of full paths of enabled plugins</p>
-</dd>
-<dt>[Recent] Files</dt><dd><p>the list of files recently opened</p>
-</dd>
-<dt>[Session] Files</dt><dd><p>the list of files and views that were open the last time <cite>ViTables</cite> was closed</p>
-</dd>
-<dt>[Startup] lastWorkingDir</dt><dd><p>the last directory accessed from within <cite>ViTables</cite> via Open File dialog</p>
-</dd>
-<dt>[Startup] restoreLastSession</dt><dd><p>the last working session is restored (if possible) which means that both files and leaves that were open in the last session will be reopen at application startup.</p>
-</dd>
-<dt>[Startup] startupWorkingDir</dt><dd><p>possible values are <em>current</em>, and <em>last</em>. These values indicate how the application will setup the startup working directory.</p>
-</dd>
-<dt>[Workspace] Background</dt><dd><p>the workspace background brush</p>
-</dd>
-</dl>
-</div></blockquote>
-<p class="rubric">Footnotes</p>
-<dl class="footnote brackets">
-<dt class="label" id="f3"><span class="brackets"><a class="fn-backref" href="#id1">1</a></span></dt>
-<dd><p>Entries in the Geometry section allow for keeping the aspect, size and position of the application window between sessions.</p>
-</dd>
-</dl>
-</div>
-
-
-          </div>
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-  <h4>Previous topic</h4>
-  <p class="topless"><a href="usersguide-ch4.html"
-                        title="previous chapter">4. Editing Files</a></p>
-  <h4>Next topic</h4>
-  <p class="topless"><a href="usersguide-app1.html"
-                        title="next chapter">6. About Plugins</a></p>
-  <div role="note" aria-label="source link">
-    <h3>This Page</h3>
-    <ul class="this-page-menu">
-      <li><a href="_sources/usersguide-ch5.rst.txt"
-            rel="nofollow">Show Source</a></li>
-    </ul>
-   </div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" />
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script type="text/javascript">$('#searchbox').show(0);</script>
-        </div>
-      </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="related" role="navigation" aria-label="related navigation">
-      <h3>Navigation</h3>
-      <ul>
-        <li class="right" style="margin-right: 10px">
-          <a href="genindex.html" title="General Index"
-             >index</a></li>
-        <li class="right" >
-          <a href="usersguide-app1.html" title="6. About Plugins"
-             >next</a> |</li>
-        <li class="right" >
-          <a href="usersguide-ch4.html" title="4. Editing Files"
-             >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.2 documentation</a> &#187;</li> 
-      </ul>
-    </div>
-    <div class="footer" role="contentinfo">
-        &#169; Copyright 2017, Vicent Mas.
-      Created using <a href="http://sphinx-doc.org/">Sphinx</a> 2.2.1.
-    </div>
-  </body>
+<!DOCTYPE html>
+
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
+    <title>5. Configuring ViTables &#8212; ViTables Users&#39; Guide 3.0.3 documentation</title>
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b76e3c8a" />
+    <link rel="stylesheet" type="text/css" href="_static/classic.css?v=89b800e6" />
+    
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js?v=b94513d7"></script>
+    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/sphinx_highlight.js?v=4825356b"></script>
+    
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="6. About Plugins" href="usersguide-app1.html" />
+    <link rel="prev" title="4. Editing Files" href="usersguide-ch4.html" /> 
+  </head><body>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             accesskey="I">index</a></li>
+        <li class="right" >
+          <a href="usersguide-app1.html" title="6. About Plugins"
+             accesskey="N">next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch4.html" title="4. Editing Files"
+             accesskey="P">previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">5. </span>Configuring ViTables</a></li> 
+      </ul>
+    </div>  
+
+    <div class="document">
+      <div class="documentwrapper">
+        <div class="bodywrapper">
+          <div class="body" role="main">
+            
+  <section id="configuring-vitables">
+<span id="configuration-chapter"></span><h1><span class="section-number">5. </span>Configuring ViTables<a class="headerlink" href="#configuring-vitables" title="Permalink to this heading">¶</a></h1>
+<p>As mentioned earlier, many aspects of the <cite>ViTables</cite> behaviour can be customized by you through the <span class="menuselection">Settings ‣ Preferences</span> command.</p>
+<p>It shows a dialog offering you several customization
+possibilities. The dialog is made of three stacked pages,
+<span class="guilabel">General</span>, <span class="guilabel">Look &amp; Feel</span> and <span class="guilabel">Plugins</span>.</p>
+<p>The <span class="guilabel">General</span> page allows to change the <cite>ViTables</cite> behavior at startup. You can set the initial working directory to be that one from which <cite>ViTables</cite> is starting or to be the last used working directory. And you can recover your last working session.</p>
+<p>The <span class="guilabel">Look &amp; Feel</span> page allows to change visual
+aspects of the application such as fonts, colors or even the general style, so you can adapt the global aspect of <cite>ViTables</cite> to what would be expected on your platform.</p>
+<p>From the <span class="guilabel">Plugins</span> page the plugins can be managed. You can enable or disable the available plugins. Changes in this page will take effect the next time you start <cite>ViTables</cite>.</p>
+<p>The <span class="guilabel">OK</span> button will apply the new settings and
+make them permanent by saving them in the Windows registry, in a configuration file (on Unix platforms) or in a plist file (on Mac OS X platforms). Even if settings are stored in a plain text file editing it by hand is not recommended. Some settings, like fonts or geometry settings <a class="footnote-reference brackets" href="#f3" id="id1" role="doc-noteref"><span class="fn-bracket">[</span>1<span class="fn-bracket">]</span></a>, are stored in a way not really intended to be modified manually.</p>
+<p>Anyway it can be worth how settings are stored so let’s do it.
+The configuration file is divided into sections, labeled as
+[section_name]. Every section is made of subsections written as key/value pairs and representing the item that is being
+customized. Currently the following sections/subsections are available:</p>
+<blockquote>
+<div><dl class="simple">
+<dt>[Geometry] HSplitter</dt><dd><p>the size of the horizontal splitter</p>
+</dd>
+<dt>[Geometry] Layout</dt><dd><p>the position and size of toolbars and dock widgets</p>
+</dd>
+<dt>[Geometry] Position</dt><dd><p>the position and size of the application window</p>
+</dd>
+<dt>[Geometry] VSplitter</dt><dd><p>the size of the vertical splitter</p>
+</dd>
+<dt>[HelpBrowser] Bookmarks</dt><dd><p>the list of current bookmarks of the help browser</p>
+</dd>
+<dt>[HelpBrowser] History</dt><dd><p>the navigation history of the help browser</p>
+</dd>
+<dt>[Logger] Font</dt><dd><p>the logger font</p>
+</dd>
+<dt>[Logger] Paper</dt><dd><p>the logger background color</p>
+</dd>
+<dt>[Logger] Text</dt><dd><p>the logger text color</p>
+</dd>
+<dt>[Look] currentStyle</dt><dd><p>the style that defines the application look &amp; feel. Available styles fit the most common platforms, i.e., Windows, Unix (Motif and SGI flavors), and Macintosh</p>
+</dd>
+<dt>[Plugins] Enabled</dt><dd><p>the list of full paths of enabled plugins</p>
+</dd>
+<dt>[Recent] Files</dt><dd><p>the list of files recently opened</p>
+</dd>
+<dt>[Session] Files</dt><dd><p>the list of files and views that were open the last time <cite>ViTables</cite> was closed</p>
+</dd>
+<dt>[Startup] lastWorkingDir</dt><dd><p>the last directory accessed from within <cite>ViTables</cite> via Open File dialog</p>
+</dd>
+<dt>[Startup] restoreLastSession</dt><dd><p>the last working session is restored (if possible) which means that both files and leaves that were open in the last session will be reopen at application startup.</p>
+</dd>
+<dt>[Startup] startupWorkingDir</dt><dd><p>possible values are <em>current</em>, and <em>last</em>. These values indicate how the application will setup the startup working directory.</p>
+</dd>
+<dt>[Workspace] Background</dt><dd><p>the workspace background brush</p>
+</dd>
+</dl>
+</div></blockquote>
+<p class="rubric">Footnotes</p>
+<aside class="footnote-list brackets">
+<aside class="footnote brackets" id="f3" role="doc-footnote">
+<span class="label"><span class="fn-bracket">[</span><a role="doc-backlink" href="#id1">1</a><span class="fn-bracket">]</span></span>
+<p>Entries in the Geometry section allow for keeping the aspect, size and position of the application window between sessions.</p>
+</aside>
+</aside>
+</section>
+
+
+            <div class="clearer"></div>
+          </div>
+        </div>
+      </div>
+      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
+        <div class="sphinxsidebarwrapper">
+  <div>
+    <h4>Previous topic</h4>
+    <p class="topless"><a href="usersguide-ch4.html"
+                          title="previous chapter"><span class="section-number">4. </span>Editing Files</a></p>
+  </div>
+  <div>
+    <h4>Next topic</h4>
+    <p class="topless"><a href="usersguide-app1.html"
+                          title="next chapter"><span class="section-number">6. </span>About Plugins</a></p>
+  </div>
+  <div role="note" aria-label="source link">
+    <h3>This Page</h3>
+    <ul class="this-page-menu">
+      <li><a href="_sources/usersguide-ch5.rst.txt"
+            rel="nofollow">Show Source</a></li>
+    </ul>
+   </div>
+<div id="searchbox" style="display: none" role="search">
+  <h3 id="searchlabel">Quick search</h3>
+    <div class="searchformwrapper">
+    <form class="search" action="search.html" method="get">
+      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+      <input type="submit" value="Go" />
+    </form>
+    </div>
+</div>
+<script>document.getElementById('searchbox').style.display = "block"</script>
+        </div>
+      </div>
+      <div class="clearer"></div>
+    </div>
+    <div class="related" role="navigation" aria-label="related navigation">
+      <h3>Navigation</h3>
+      <ul>
+        <li class="right" style="margin-right: 10px">
+          <a href="genindex.html" title="General Index"
+             >index</a></li>
+        <li class="right" >
+          <a href="usersguide-app1.html" title="6. About Plugins"
+             >next</a> |</li>
+        <li class="right" >
+          <a href="usersguide-ch4.html" title="4. Editing Files"
+             >previous</a> |</li>
+        <li class="nav-item nav-item-0"><a href="index.html">ViTables Users&#39; Guide 3.0.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-this"><a href=""><span class="section-number">5. </span>Configuring ViTables</a></li> 
+      </ul>
+    </div>
+    <div class="footer" role="contentinfo">
+    &#169; Copyright 2023, Vicent Mas.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.1.1.
+    </div>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,16 @@
 
 
 
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 5. Configuring ViTables
 ****** 5. Configuring ViTablesÂ¶ ******
 As mentioned earlier, many aspects of theViTablesbehaviour can be customized by
 you through the Settings â£ Preferences command.
 It shows a dialog offering you several customization possibilities. The dialog
 is made of three stacked pages, General, Look & Feel and Plugins.
 The General page allows to change theViTablesbehavior at startup. You can set
 the initial working directory to be that one from whichViTablesis starting or
@@ -24,15 +25,15 @@
 From the Plugins page the plugins can be managed. You can enable or disable the
 available plugins. Changes in this page will take effect the next time you
 startViTables.
 The OK button will apply the new settings and make them permanent by saving
 them in the Windows registry, in a configuration file (on Unix platforms) or in
 a plist file (on Mac OS X platforms). Even if settings are stored in a plain
 text file editing it by hand is not recommended. Some settings, like fonts or
-geometry settings 1, are stored in a way not really intended to be modified
+geometry settings [1], are stored in a way not really intended to be modified
 manually.
 Anyway it can be worth how settings are stored so letâs do it. The
 configuration file is divided into sections, labeled as [section_name]. Every
 section is made of subsections written as key/value pairs and representing the
 item that is being customized. Currently the following sections/subsections are
 available:
        [Geometry] HSplitter
@@ -73,24 +74,26 @@
            will be reopen at application startup.
        [Startup] startupWorkingDir
            possible values are current, and last. These values indicate
            how the application will setup the startup working directory.
        [Workspace] Background
            the workspace background brush
 Footnotes
-  1
-      Entries in the Geometry section allow for keeping the aspect, size and
-      position of the application window between sessions.
+  [1]
+Entries in the Geometry section allow for keeping the aspect, size and position
+of the application window between sessions.
+
 *** Previous topic ***
 4._Editing_Files
 *** Next topic ***
 6._About_Plugins
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
-    * ViTables_Users'_Guide_3.0.2_documentation »
-© Copyright 2017, Vicent Mas. Created using Sphinx 2.2.1.
+    * ViTables_Users'_Guide_3.0.3_documentation »
+    * 5. Configuring ViTables
+© Copyright 2023, Vicent Mas. Created using Sphinx 7.1.1.
```

### Comparing `ViTables-3.0.2/vitables/i18n/vitables_es_ES.qm` & `vitables-3.0.3/vitables/i18n/vitables_es_ES.qm`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/i18n/vitables_ru_RU.qm` & `vitables-3.0.3/vitables/i18n/vitables_ru_RU.qm`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/application-exit.png` & `vitables-3.0.3/vitables/icons/16x16/application-exit.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/bookmark_add.png` & `vitables-3.0.3/vitables/icons/16x16/bookmark_add.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/bookmarks.png` & `vitables-3.0.3/vitables/icons/16x16/bookmarks.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/configure.png` & `vitables-3.0.3/vitables/icons/16x16/configure.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/delete_filters.png` & `vitables-3.0.3/vitables/icons/16x16/delete_filters.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/dialog-cancel.png` & `vitables-3.0.3/vitables/icons/16x16/dialog-cancel.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/dialog-ok.png` & `vitables-3.0.3/vitables/icons/16x16/dialog-ok.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/document-close.png` & `vitables-3.0.3/vitables/icons/16x16/document-close.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/document-export.png` & `vitables-3.0.3/vitables/icons/16x16/document-export.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/document-import.png` & `vitables-3.0.3/vitables/icons/16x16/document-import.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/document-new.png` & `vitables-3.0.3/vitables/icons/16x16/document-new.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/document-open-recent.png` & `vitables-3.0.3/vitables/icons/16x16/document-open-recent.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/document-open.png` & `vitables-3.0.3/vitables/icons/16x16/document-open.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/document-save-as.png` & `vitables-3.0.3/vitables/icons/16x16/document-save-as.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/edit-delete.png` & `vitables-3.0.3/vitables/icons/16x16/edit-delete.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/edit-paste.png` & `vitables-3.0.3/vitables/icons/16x16/edit-paste.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/file_ro.png` & `vitables-3.0.3/vitables/icons/16x16/file_ro.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/file_rw.png` & `vitables-3.0.3/vitables/icons/16x16/file_rw.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/folder-new.png` & `vitables-3.0.3/vitables/icons/16x16/folder-new.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/go-first-view.png` & `vitables-3.0.3/vitables/icons/16x16/go-first-view.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/go-next-view.png` & `vitables-3.0.3/vitables/icons/16x16/go-next-view.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/go-previous-view.png` & `vitables-3.0.3/vitables/icons/16x16/go-previous-view.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/help-about.png` & `vitables-3.0.3/vitables/icons/16x16/help-about.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/help-contents.png` & `vitables-3.0.3/vitables/icons/16x16/help-contents.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/image-missing.png` & `vitables-3.0.3/vitables/icons/16x16/image-missing.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/link_earray.png` & `vitables-3.0.3/vitables/icons/16x16/link_earray.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/link_table.png` & `vitables-3.0.3/vitables/icons/16x16/link_table.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/object.png` & `vitables-3.0.3/vitables/icons/16x16/object.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/table.png` & `vitables-3.0.3/vitables/icons/16x16/table.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/zoom-in.png` & `vitables-3.0.3/vitables/icons/16x16/zoom-in.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/16x16/zoom-out.png` & `vitables-3.0.3/vitables/icons/16x16/zoom-out.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/application-exit.png` & `vitables-3.0.3/vitables/icons/22x22/application-exit.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/bookmark_add.png` & `vitables-3.0.3/vitables/icons/22x22/bookmark_add.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/bookmarks.png` & `vitables-3.0.3/vitables/icons/22x22/bookmarks.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/delete_filters.png` & `vitables-3.0.3/vitables/icons/22x22/delete_filters.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/document-close.png` & `vitables-3.0.3/vitables/icons/22x22/document-close.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/document-new.png` & `vitables-3.0.3/vitables/icons/22x22/document-new.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/document-open-folder.png` & `vitables-3.0.3/vitables/icons/22x22/document-open-folder.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/document-open.png` & `vitables-3.0.3/vitables/icons/22x22/document-open.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/document-save-as.png` & `vitables-3.0.3/vitables/icons/22x22/document-save-as.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/edit-clear-history.png` & `vitables-3.0.3/vitables/icons/22x22/edit-clear-history.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/edit-copy.png` & `vitables-3.0.3/vitables/icons/22x22/edit-copy.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/edit-cut.png` & `vitables-3.0.3/vitables/icons/22x22/edit-cut.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/edit-delete.png` & `vitables-3.0.3/vitables/icons/22x22/edit-delete.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/edit-paste.png` & `vitables-3.0.3/vitables/icons/22x22/edit-paste.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/file_ro.png` & `vitables-3.0.3/vitables/icons/22x22/file_ro.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/file_rw.png` & `vitables-3.0.3/vitables/icons/22x22/file_rw.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/folder-new.png` & `vitables-3.0.3/vitables/icons/22x22/folder-new.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/folder.png` & `vitables-3.0.3/vitables/icons/22x22/folder.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/go-first-view.png` & `vitables-3.0.3/vitables/icons/22x22/go-first-view.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/go-next-view.png` & `vitables-3.0.3/vitables/icons/22x22/go-next-view.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/go-previous-view.png` & `vitables-3.0.3/vitables/icons/22x22/go-previous-view.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/help-contents.png` & `vitables-3.0.3/vitables/icons/22x22/help-contents.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/view-filter.png` & `vitables-3.0.3/vitables/icons/22x22/view-filter.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/view-refresh.png` & `vitables-3.0.3/vitables/icons/22x22/view-refresh.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/zoom-in.png` & `vitables-3.0.3/vitables/icons/22x22/zoom-in.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/22x22/zoom-out.png` & `vitables-3.0.3/vitables/icons/22x22/zoom-out.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/64x64/preferences-desktop-theme.png` & `vitables-3.0.3/vitables/icons/64x64/preferences-desktop-theme.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/64x64/preferences-other.png` & `vitables-3.0.3/vitables/icons/64x64/preferences-other.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/64x64/preferences-plugin.png` & `vitables-3.0.3/vitables/icons/64x64/preferences-plugin.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/mswindows/vitables.ico` & `vitables-3.0.3/vitables/icons/mswindows/vitables.ico`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/mswindows/vitables_file.ico` & `vitables-3.0.3/vitables/icons/mswindows/vitables_file.ico`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/mswindows/vtinstaller.ico` & `vitables-3.0.3/vitables/icons/mswindows/vtinstaller.ico`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/unixapp/vitables.svg` & `vitables-3.0.3/vitables/icons/unixapp/vitables.svg`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/unixapp/vitables_128x128.png` & `vitables-3.0.3/vitables/icons/unixapp/vitables_128x128.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/unixapp/vitables_16x16.png` & `vitables-3.0.3/vitables/icons/unixapp/vitables_16x16.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/unixapp/vitables_22x22.png` & `vitables-3.0.3/vitables/icons/unixapp/vitables_22x22.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/unixapp/vitables_32x32.png` & `vitables-3.0.3/vitables/icons/unixapp/vitables_32x32.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/unixapp/vitables_48x48.png` & `vitables-3.0.3/vitables/icons/unixapp/vitables_48x48.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/unixapp/vitables_64x64.png` & `vitables-3.0.3/vitables/icons/unixapp/vitables_64x64.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/vitables_logo.png` & `vitables-3.0.3/vitables/icons/vitables_logo.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/vitables_logo.svg` & `vitables-3.0.3/vitables/icons/vitables_logo.svg`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/icons/vitables_wm.png` & `vitables-3.0.3/vitables/icons/vitables_wm.png`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/logger.py` & `vitables-3.0.3/vitables/logger.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/__init__.py` & `vitables-3.0.3/vitables/nodeprops/__init__.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/attr_prop_dlg.ui` & `vitables-3.0.3/vitables/nodeprops/attr_prop_dlg.ui`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/attreditor.py` & `vitables-3.0.3/vitables/nodeprops/attreditor.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/attrpropdlg.py` & `vitables-3.0.3/vitables/nodeprops/attrpropdlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/group_prop_page.ui` & `vitables-3.0.3/vitables/nodeprops/group_prop_page.ui`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/grouppropdlg.py` & `vitables-3.0.3/vitables/nodeprops/grouppropdlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/groupproppage.py` & `vitables-3.0.3/vitables/nodeprops/groupproppage.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/leaf_prop_page.ui` & `vitables-3.0.3/vitables/nodeprops/leaf_prop_page.ui`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/leafpropdlg.py` & `vitables-3.0.3/vitables/nodeprops/leafpropdlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/leafproppage.py` & `vitables-3.0.3/vitables/nodeprops/leafproppage.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/link_prop_dlg.ui` & `vitables-3.0.3/vitables/nodeprops/link_prop_dlg.ui`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/linkpropdlg.py` & `vitables-3.0.3/vitables/nodeprops/linkpropdlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/nodeprops/nodeinfo.py` & `vitables-3.0.3/vitables/nodeprops/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/plugins/__init__.py` & `vitables-3.0.3/vitables/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/plugins/columnorg/__init__.py` & `vitables-3.0.3/vitables/vtwidgets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
 #       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
 #
 #       This program is free software: you can redistribute it and/or modify
 #       it under the terms of the GNU General Public License as published by
 #       the Free Software Foundation, either version 3 of the License, or
 #       (at your option) any later version.
 #
@@ -12,8 +13,8 @@
 #       GNU General Public License for more details.
 #
 #       You should have received a copy of the GNU General Public License
 #       along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #       Author:  Vicent Mas - vmas@vitables.org
 
-__all__ = ['aboutpage', 'columnar_org']
+__all__ = ["nodenamedlg", "renamedlg", "zoom_cell"]
```

### Comparing `ViTables-3.0.2/vitables/plugins/columnorg/columnar_org.py` & `vitables-3.0.3/vitables/plugins/columnorg/columnar_org.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/plugins/dbstreesort/__init__.py` & `vitables-3.0.3/vitables/queries/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
 #       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
 #
 #       This program is free software: you can redistribute it and/or modify
 #       it under the terms of the GNU General Public License as published by
 #       the Free Software Foundation, either version 3 of the License, or
 #       (at your option) any later version.
 #
@@ -12,8 +13,8 @@
 #       GNU General Public License for more details.
 #
 #       You should have received a copy of the GNU General Public License
 #       along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #       Author:  Vicent Mas - vmas@vitables.org
 
-__all__ = ['aboutpage', 'dbs_tree_sort']
+__all__ = ["query", "querydlg", "querymgr"]
```

### Comparing `ViTables-3.0.2/vitables/plugins/dbstreesort/aboutpage.py` & `vitables-3.0.3/vitables/plugins/dbstreesort/aboutpage.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/plugins/dbstreesort/dbs_tree_sort.py` & `vitables-3.0.3/vitables/plugins/dbstreesort/dbs_tree_sort.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/plugins/dbstreesort/dbs_tree_sort_page.ui` & `vitables-3.0.3/vitables/plugins/dbstreesort/dbs_tree_sort_page.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 27% similar despite different names*

```diff
@@ -1,515 +1,534 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
-00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
-00000040: 733e 4442 5472 6565 536f 7274 5061 6765  s>DBTreeSortPage
-00000050: 3c2f 636c 6173 733e 0a20 3c77 6964 6765  </class>. <widge
-00000060: 7420 636c 6173 733d 2251 5769 6467 6574  t class="QWidget
-00000070: 2220 6e61 6d65 3d22 4442 5472 6565 536f  " name="DBTreeSo
-00000080: 7274 5061 6765 223e 0a20 203c 7072 6f70  rtPage">.  <prop
-00000090: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-000000a0: 7472 7922 3e0a 2020 203c 7265 6374 3e0a  try">.   <rect>.
-000000b0: 2020 2020 3c78 3e30 3c2f 783e 0a20 2020      <x>0</x>.   
-000000c0: 203c 793e 303c 2f79 3e0a 2020 2020 3c77   <y>0</y>.    <w
-000000d0: 6964 7468 3e34 3030 3c2f 7769 6474 683e  idth>400</width>
-000000e0: 0a20 2020 203c 6865 6967 6874 3e34 3733  .    <height>473
-000000f0: 3c2f 6865 6967 6874 3e0a 2020 203c 2f72  </height>.   </r
-00000100: 6563 743e 0a20 203c 2f70 726f 7065 7274  ect>.  </propert
-00000110: 793e 0a20 203c 7072 6f70 6572 7479 206e  y>.  <property n
-00000120: 616d 653d 2277 696e 646f 7754 6974 6c65  ame="windowTitle
-00000130: 223e 0a20 2020 3c73 7472 696e 673e 466f  ">.   <string>Fo
-00000140: 726d 3c2f 7374 7269 6e67 3e0a 2020 3c2f  rm</string>.  </
-00000150: 7072 6f70 6572 7479 3e0a 2020 3c6c 6179  property>.  <lay
-00000160: 6f75 7420 636c 6173 733d 2251 5642 6f78  out class="QVBox
-00000170: 4c61 796f 7574 2220 6e61 6d65 3d22 7665  Layout" name="ve
-00000180: 7274 6963 616c 4c61 796f 7574 223e 0a20  rticalLayout">. 
-00000190: 2020 3c69 7465 6d3e 0a20 2020 203c 7769    <item>.    <wi
-000001a0: 6467 6574 2063 6c61 7373 3d22 5147 726f  dget class="QGro
-000001b0: 7570 426f 7822 206e 616d 653d 2264 6573  upBox" name="des
-000001c0: 6347 4222 3e0a 2020 2020 203c 7072 6f70  cGB">.     <prop
-000001d0: 6572 7479 206e 616d 653d 2274 6974 6c65  erty name="title
-000001e0: 223e 0a20 2020 2020 203c 7374 7269 6e67  ">.      <string
-000001f0: 3e50 6c75 6769 6e20 6465 7363 7269 7074  >Plugin descript
-00000200: 696f 6e3c 2f73 7472 696e 673e 0a20 2020  ion</string>.   
-00000210: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
-00000220: 2020 203c 6c61 796f 7574 2063 6c61 7373     <layout class
-00000230: 3d22 5147 7269 644c 6179 6f75 7422 206e  ="QGridLayout" n
-00000240: 616d 653d 2267 7269 644c 6179 6f75 7422  ame="gridLayout"
-00000250: 3e0a 2020 2020 2020 3c69 7465 6d20 726f  >.      <item ro
-00000260: 773d 2230 2220 636f 6c75 6d6e 3d22 3022  w="0" column="0"
-00000270: 3e0a 2020 2020 2020 203c 7769 6467 6574  >.       <widget
-00000280: 2063 6c61 7373 3d22 514c 6162 656c 2220   class="QLabel" 
-00000290: 6e61 6d65 3d22 7665 7273 696f 6e5f 6c61  name="version_la
-000002a0: 6265 6c22 3e0a 2020 2020 2020 2020 3c70  bel">.        <p
-000002b0: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-000002c0: 7874 223e 0a20 2020 2020 2020 2020 3c73  xt">.         <s
-000002d0: 7472 696e 673e 5665 7273 696f 6e3a 203c  tring>Version: <
-000002e0: 2f73 7472 696e 673e 0a20 2020 2020 2020  /string>.       
-000002f0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-00000300: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
-00000310: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
-00000320: 2020 3c69 7465 6d20 726f 773d 2230 2220    <item row="0" 
-00000330: 636f 6c75 6d6e 3d22 3122 3e0a 2020 2020  column="1">.    
-00000340: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00000350: 3d22 514c 696e 6545 6469 7422 206e 616d  ="QLineEdit" nam
-00000360: 653d 2276 6572 7369 6f6e 5f6c 6522 3e0a  e="version_le">.
-00000370: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00000380: 7920 6e61 6d65 3d22 7061 6c65 7474 6522  y name="palette"
-00000390: 3e0a 2020 2020 2020 2020 203c 7061 6c65  >.         <pale
-000003a0: 7474 653e 0a20 2020 2020 2020 2020 203c  tte>.          <
-000003b0: 6163 7469 7665 3e0a 2020 2020 2020 2020  active>.        
-000003c0: 2020 203c 636f 6c6f 7272 6f6c 6520 726f     <colorrole ro
-000003d0: 6c65 3d22 4261 7365 223e 0a20 2020 2020  le="Base">.     
-000003e0: 2020 2020 2020 203c 6272 7573 6820 6272         <brush br
-000003f0: 7573 6873 7479 6c65 3d22 536f 6c69 6450  ushstyle="SolidP
-00000400: 6174 7465 726e 223e 0a20 2020 2020 2020  attern">.       
-00000410: 2020 2020 2020 3c63 6f6c 6f72 2061 6c70        <color alp
-00000420: 6861 3d22 3235 3522 3e0a 2020 2020 2020  ha="255">.      
-00000430: 2020 2020 2020 2020 3c72 6564 3e32 3339          <red>239
-00000440: 3c2f 7265 643e 0a20 2020 2020 2020 2020  </red>.         
-00000450: 2020 2020 203c 6772 6565 6e3e 3233 393c       <green>239<
-00000460: 2f67 7265 656e 3e0a 2020 2020 2020 2020  /green>.        
-00000470: 2020 2020 2020 3c62 6c75 653e 3233 393c        <blue>239<
-00000480: 2f62 6c75 653e 0a20 2020 2020 2020 2020  /blue>.         
-00000490: 2020 2020 3c2f 636f 6c6f 723e 0a20 2020      </color>.   
-000004a0: 2020 2020 2020 2020 203c 2f62 7275 7368           </brush
-000004b0: 3e0a 2020 2020 2020 2020 2020 203c 2f63  >.           </c
-000004c0: 6f6c 6f72 726f 6c65 3e0a 2020 2020 2020  olorrole>.      
-000004d0: 2020 2020 3c2f 6163 7469 7665 3e0a 2020      </active>.  
-000004e0: 2020 2020 2020 2020 3c69 6e61 6374 6976          <inactiv
-000004f0: 653e 0a20 2020 2020 2020 2020 2020 3c63  e>.           <c
-00000500: 6f6c 6f72 726f 6c65 2072 6f6c 653d 2242  olorrole role="B
-00000510: 6173 6522 3e0a 2020 2020 2020 2020 2020  ase">.          
-00000520: 2020 3c62 7275 7368 2062 7275 7368 7374    <brush brushst
-00000530: 796c 653d 2253 6f6c 6964 5061 7474 6572  yle="SolidPatter
-00000540: 6e22 3e0a 2020 2020 2020 2020 2020 2020  n">.            
-00000550: 203c 636f 6c6f 7220 616c 7068 613d 2232   <color alpha="2
-00000560: 3535 223e 0a20 2020 2020 2020 2020 2020  55">.           
-00000570: 2020 203c 7265 643e 3233 393c 2f72 6564     <red>239</red
-00000580: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000590: 3c67 7265 656e 3e32 3339 3c2f 6772 6565  <green>239</gree
-000005a0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
-000005b0: 203c 626c 7565 3e32 3339 3c2f 626c 7565   <blue>239</blue
-000005c0: 3e0a 2020 2020 2020 2020 2020 2020 203c  >.             <
-000005d0: 2f63 6f6c 6f72 3e0a 2020 2020 2020 2020  /color>.        
-000005e0: 2020 2020 3c2f 6272 7573 683e 0a20 2020      </brush>.   
-000005f0: 2020 2020 2020 2020 3c2f 636f 6c6f 7272          </colorr
-00000600: 6f6c 653e 0a20 2020 2020 2020 2020 203c  ole>.          <
-00000610: 2f69 6e61 6374 6976 653e 0a20 2020 2020  /inactive>.     
-00000620: 2020 2020 203c 6469 7361 626c 6564 3e0a       <disabled>.
-00000630: 2020 2020 2020 2020 2020 203c 636f 6c6f             <colo
-00000640: 7272 6f6c 6520 726f 6c65 3d22 4261 7365  rrole role="Base
-00000650: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-00000660: 6272 7573 6820 6272 7573 6873 7479 6c65  brush brushstyle
-00000670: 3d22 536f 6c69 6450 6174 7465 726e 223e  ="SolidPattern">
-00000680: 0a20 2020 2020 2020 2020 2020 2020 3c63  .             <c
-00000690: 6f6c 6f72 2061 6c70 6861 3d22 3235 3522  olor alpha="255"
-000006a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000006b0: 3c72 6564 3e32 3434 3c2f 7265 643e 0a20  <red>244</red>. 
-000006c0: 2020 2020 2020 2020 2020 2020 203c 6772               <gr
-000006d0: 6565 6e3e 3234 343c 2f67 7265 656e 3e0a  een>244</green>.
-000006e0: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
-000006f0: 6c75 653e 3234 343c 2f62 6c75 653e 0a20  lue>244</blue>. 
-00000700: 2020 2020 2020 2020 2020 2020 3c2f 636f              </co
-00000710: 6c6f 723e 0a20 2020 2020 2020 2020 2020  lor>.           
-00000720: 203c 2f62 7275 7368 3e0a 2020 2020 2020   </brush>.      
-00000730: 2020 2020 203c 2f63 6f6c 6f72 726f 6c65       </colorrole
-00000740: 3e0a 2020 2020 2020 2020 2020 3c2f 6469  >.          </di
-00000750: 7361 626c 6564 3e0a 2020 2020 2020 2020  sabled>.        
-00000760: 203c 2f70 616c 6574 7465 3e0a 2020 2020   </palette>.    
-00000770: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00000780: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00000790: 7920 6e61 6d65 3d22 7265 6164 4f6e 6c79  y name="readOnly
-000007a0: 223e 0a20 2020 2020 2020 2020 3c62 6f6f  ">.         <boo
-000007b0: 6c3e 7472 7565 3c2f 626f 6f6c 3e0a 2020  l>true</bool>.  
-000007c0: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-000007d0: 3e0a 2020 2020 2020 203c 2f77 6964 6765  >.       </widge
-000007e0: 743e 0a20 2020 2020 203c 2f69 7465 6d3e  t>.      </item>
-000007f0: 0a20 2020 2020 203c 6974 656d 2072 6f77  .      <item row
-00000800: 3d22 3122 2063 6f6c 756d 6e3d 2230 223e  ="1" column="0">
-00000810: 0a20 2020 2020 2020 3c77 6964 6765 7420  .       <widget 
-00000820: 636c 6173 733d 2251 4c61 6265 6c22 206e  class="QLabel" n
-00000830: 616d 653d 226d 6f64 756c 655f 6e61 6d65  ame="module_name
-00000840: 5f6c 6162 656c 223e 0a20 2020 2020 2020  _label">.       
-00000850: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00000860: 2274 6578 7422 3e0a 2020 2020 2020 2020  "text">.        
-00000870: 203c 7374 7269 6e67 3e4d 6f64 756c 6520   <string>Module 
-00000880: 6e61 6d65 3a20 3c2f 7374 7269 6e67 3e0a  name: </string>.
-00000890: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-000008a0: 7479 3e0a 2020 2020 2020 203c 2f77 6964  ty>.       </wid
-000008b0: 6765 743e 0a20 2020 2020 203c 2f69 7465  get>.      </ite
-000008c0: 6d3e 0a20 2020 2020 203c 6974 656d 2072  m>.      <item r
-000008d0: 6f77 3d22 3122 2063 6f6c 756d 6e3d 2231  ow="1" column="1
-000008e0: 223e 0a20 2020 2020 2020 3c77 6964 6765  ">.       <widge
-000008f0: 7420 636c 6173 733d 2251 4c69 6e65 4564  t class="QLineEd
-00000900: 6974 2220 6e61 6d65 3d22 6d6f 6475 6c65  it" name="module
-00000910: 5f6e 616d 655f 6c65 223e 0a20 2020 2020  _name_le">.     
-00000920: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00000930: 653d 2270 616c 6574 7465 223e 0a20 2020  e="palette">.   
-00000940: 2020 2020 2020 3c70 616c 6574 7465 3e0a        <palette>.
-00000950: 2020 2020 2020 2020 2020 3c61 6374 6976            <activ
-00000960: 653e 0a20 2020 2020 2020 2020 2020 3c63  e>.           <c
-00000970: 6f6c 6f72 726f 6c65 2072 6f6c 653d 2242  olorrole role="B
-00000980: 6173 6522 3e0a 2020 2020 2020 2020 2020  ase">.          
-00000990: 2020 3c62 7275 7368 2062 7275 7368 7374    <brush brushst
-000009a0: 796c 653d 2253 6f6c 6964 5061 7474 6572  yle="SolidPatter
-000009b0: 6e22 3e0a 2020 2020 2020 2020 2020 2020  n">.            
-000009c0: 203c 636f 6c6f 7220 616c 7068 613d 2232   <color alpha="2
-000009d0: 3535 223e 0a20 2020 2020 2020 2020 2020  55">.           
-000009e0: 2020 203c 7265 643e 3233 393c 2f72 6564     <red>239</red
-000009f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000a00: 3c67 7265 656e 3e32 3339 3c2f 6772 6565  <green>239</gree
-00000a10: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
-00000a20: 203c 626c 7565 3e32 3339 3c2f 626c 7565   <blue>239</blue
-00000a30: 3e0a 2020 2020 2020 2020 2020 2020 203c  >.             <
-00000a40: 2f63 6f6c 6f72 3e0a 2020 2020 2020 2020  /color>.        
-00000a50: 2020 2020 3c2f 6272 7573 683e 0a20 2020      </brush>.   
-00000a60: 2020 2020 2020 2020 3c2f 636f 6c6f 7272          </colorr
-00000a70: 6f6c 653e 0a20 2020 2020 2020 2020 203c  ole>.          <
-00000a80: 2f61 6374 6976 653e 0a20 2020 2020 2020  /active>.       
-00000a90: 2020 203c 696e 6163 7469 7665 3e0a 2020     <inactive>.  
-00000aa0: 2020 2020 2020 2020 203c 636f 6c6f 7272           <colorr
-00000ab0: 6f6c 6520 726f 6c65 3d22 4261 7365 223e  ole role="Base">
-00000ac0: 0a20 2020 2020 2020 2020 2020 203c 6272  .            <br
-00000ad0: 7573 6820 6272 7573 6873 7479 6c65 3d22  ush brushstyle="
-00000ae0: 536f 6c69 6450 6174 7465 726e 223e 0a20  SolidPattern">. 
-00000af0: 2020 2020 2020 2020 2020 2020 3c63 6f6c              <col
-00000b00: 6f72 2061 6c70 6861 3d22 3235 3522 3e0a  or alpha="255">.
-00000b10: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
-00000b20: 6564 3e32 3339 3c2f 7265 643e 0a20 2020  ed>239</red>.   
-00000b30: 2020 2020 2020 2020 2020 203c 6772 6565             <gree
-00000b40: 6e3e 3233 393c 2f67 7265 656e 3e0a 2020  n>239</green>.  
-00000b50: 2020 2020 2020 2020 2020 2020 3c62 6c75              <blu
-00000b60: 653e 3233 393c 2f62 6c75 653e 0a20 2020  e>239</blue>.   
-00000b70: 2020 2020 2020 2020 2020 3c2f 636f 6c6f            </colo
-00000b80: 723e 0a20 2020 2020 2020 2020 2020 203c  r>.            <
-00000b90: 2f62 7275 7368 3e0a 2020 2020 2020 2020  /brush>.        
-00000ba0: 2020 203c 2f63 6f6c 6f72 726f 6c65 3e0a     </colorrole>.
-00000bb0: 2020 2020 2020 2020 2020 3c2f 696e 6163            </inac
-00000bc0: 7469 7665 3e0a 2020 2020 2020 2020 2020  tive>.          
-00000bd0: 3c64 6973 6162 6c65 643e 0a20 2020 2020  <disabled>.     
-00000be0: 2020 2020 2020 3c63 6f6c 6f72 726f 6c65        <colorrole
-00000bf0: 2072 6f6c 653d 2242 6173 6522 3e0a 2020   role="Base">.  
-00000c00: 2020 2020 2020 2020 2020 3c62 7275 7368            <brush
-00000c10: 2062 7275 7368 7374 796c 653d 2253 6f6c   brushstyle="Sol
-00000c20: 6964 5061 7474 6572 6e22 3e0a 2020 2020  idPattern">.    
-00000c30: 2020 2020 2020 2020 203c 636f 6c6f 7220           <color 
-00000c40: 616c 7068 613d 2232 3535 223e 0a20 2020  alpha="255">.   
-00000c50: 2020 2020 2020 2020 2020 203c 7265 643e             <red>
-00000c60: 3234 343c 2f72 6564 3e0a 2020 2020 2020  244</red>.      
-00000c70: 2020 2020 2020 2020 3c67 7265 656e 3e32          <green>2
-00000c80: 3434 3c2f 6772 6565 6e3e 0a20 2020 2020  44</green>.     
-00000c90: 2020 2020 2020 2020 203c 626c 7565 3e32           <blue>2
-00000ca0: 3434 3c2f 626c 7565 3e0a 2020 2020 2020  44</blue>.      
-00000cb0: 2020 2020 2020 203c 2f63 6f6c 6f72 3e0a         </color>.
-00000cc0: 2020 2020 2020 2020 2020 2020 3c2f 6272              </br
-00000cd0: 7573 683e 0a20 2020 2020 2020 2020 2020  ush>.           
-00000ce0: 3c2f 636f 6c6f 7272 6f6c 653e 0a20 2020  </colorrole>.   
-00000cf0: 2020 2020 2020 203c 2f64 6973 6162 6c65         </disable
-00000d00: 643e 0a20 2020 2020 2020 2020 3c2f 7061  d>.         </pa
-00000d10: 6c65 7474 653e 0a20 2020 2020 2020 203c  lette>.        <
-00000d20: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00000d30: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00000d40: 653d 2272 6561 644f 6e6c 7922 3e0a 2020  e="readOnly">.  
-00000d50: 2020 2020 2020 203c 626f 6f6c 3e74 7275         <bool>tru
-00000d60: 653c 2f62 6f6f 6c3e 0a20 2020 2020 2020  e</bool>.       
-00000d70: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-00000d80: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
-00000d90: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
-00000da0: 2020 3c69 7465 6d20 726f 773d 2232 2220    <item row="2" 
-00000db0: 636f 6c75 6d6e 3d22 3022 3e0a 2020 2020  column="0">.    
-00000dc0: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00000dd0: 3d22 514c 6162 656c 2220 6e61 6d65 3d22  ="QLabel" name="
-00000de0: 666f 6c64 6572 5f6c 6162 656c 223e 0a20  folder_label">. 
-00000df0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000e00: 206e 616d 653d 2274 6578 7422 3e0a 2020   name="text">.  
-00000e10: 2020 2020 2020 203c 7374 7269 6e67 3e46         <string>F
-00000e20: 6f6c 6465 723a 203c 2f73 7472 696e 673e  older: </string>
-00000e30: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
-00000e40: 7274 793e 0a20 2020 2020 2020 3c2f 7769  rty>.       </wi
-00000e50: 6467 6574 3e0a 2020 2020 2020 3c2f 6974  dget>.      </it
-00000e60: 656d 3e0a 2020 2020 2020 3c69 7465 6d20  em>.      <item 
-00000e70: 726f 773d 2232 2220 636f 6c75 6d6e 3d22  row="2" column="
-00000e80: 3122 3e0a 2020 2020 2020 203c 7769 6467  1">.       <widg
-00000e90: 6574 2063 6c61 7373 3d22 514c 696e 6545  et class="QLineE
-00000ea0: 6469 7422 206e 616d 653d 2266 6f6c 6465  dit" name="folde
-00000eb0: 725f 6c65 223e 0a20 2020 2020 2020 203c  r_le">.        <
-00000ec0: 7072 6f70 6572 7479 206e 616d 653d 2270  property name="p
-00000ed0: 616c 6574 7465 223e 0a20 2020 2020 2020  alette">.       
-00000ee0: 2020 3c70 616c 6574 7465 3e0a 2020 2020    <palette>.    
-00000ef0: 2020 2020 2020 3c61 6374 6976 653e 0a20        <active>. 
-00000f00: 2020 2020 2020 2020 2020 3c63 6f6c 6f72            <color
-00000f10: 726f 6c65 2072 6f6c 653d 2242 6173 6522  role role="Base"
-00000f20: 3e0a 2020 2020 2020 2020 2020 2020 3c62  >.            <b
-00000f30: 7275 7368 2062 7275 7368 7374 796c 653d  rush brushstyle=
-00000f40: 2253 6f6c 6964 5061 7474 6572 6e22 3e0a  "SolidPattern">.
-00000f50: 2020 2020 2020 2020 2020 2020 203c 636f               <co
-00000f60: 6c6f 7220 616c 7068 613d 2232 3535 223e  lor alpha="255">
-00000f70: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00000f80: 7265 643e 3233 393c 2f72 6564 3e0a 2020  red>239</red>.  
-00000f90: 2020 2020 2020 2020 2020 2020 3c67 7265              <gre
-00000fa0: 656e 3e32 3339 3c2f 6772 6565 6e3e 0a20  en>239</green>. 
-00000fb0: 2020 2020 2020 2020 2020 2020 203c 626c               <bl
-00000fc0: 7565 3e32 3339 3c2f 626c 7565 3e0a 2020  ue>239</blue>.  
-00000fd0: 2020 2020 2020 2020 2020 203c 2f63 6f6c             </col
-00000fe0: 6f72 3e0a 2020 2020 2020 2020 2020 2020  or>.            
-00000ff0: 3c2f 6272 7573 683e 0a20 2020 2020 2020  </brush>.       
-00001000: 2020 2020 3c2f 636f 6c6f 7272 6f6c 653e      </colorrole>
-00001010: 0a20 2020 2020 2020 2020 203c 2f61 6374  .          </act
-00001020: 6976 653e 0a20 2020 2020 2020 2020 203c  ive>.          <
-00001030: 696e 6163 7469 7665 3e0a 2020 2020 2020  inactive>.      
-00001040: 2020 2020 203c 636f 6c6f 7272 6f6c 6520       <colorrole 
-00001050: 726f 6c65 3d22 4261 7365 223e 0a20 2020  role="Base">.   
-00001060: 2020 2020 2020 2020 203c 6272 7573 6820           <brush 
-00001070: 6272 7573 6873 7479 6c65 3d22 536f 6c69  brushstyle="Soli
-00001080: 6450 6174 7465 726e 223e 0a20 2020 2020  dPattern">.     
-00001090: 2020 2020 2020 2020 3c63 6f6c 6f72 2061          <color a
-000010a0: 6c70 6861 3d22 3235 3522 3e0a 2020 2020  lpha="255">.    
-000010b0: 2020 2020 2020 2020 2020 3c72 6564 3e32            <red>2
-000010c0: 3339 3c2f 7265 643e 0a20 2020 2020 2020  39</red>.       
-000010d0: 2020 2020 2020 203c 6772 6565 6e3e 3233         <green>23
-000010e0: 393c 2f67 7265 656e 3e0a 2020 2020 2020  9</green>.      
-000010f0: 2020 2020 2020 2020 3c62 6c75 653e 3233          <blue>23
-00001100: 393c 2f62 6c75 653e 0a20 2020 2020 2020  9</blue>.       
-00001110: 2020 2020 2020 3c2f 636f 6c6f 723e 0a20        </color>. 
-00001120: 2020 2020 2020 2020 2020 203c 2f62 7275             </bru
-00001130: 7368 3e0a 2020 2020 2020 2020 2020 203c  sh>.           <
-00001140: 2f63 6f6c 6f72 726f 6c65 3e0a 2020 2020  /colorrole>.    
-00001150: 2020 2020 2020 3c2f 696e 6163 7469 7665        </inactive
-00001160: 3e0a 2020 2020 2020 2020 2020 3c64 6973  >.          <dis
-00001170: 6162 6c65 643e 0a20 2020 2020 2020 2020  abled>.         
-00001180: 2020 3c63 6f6c 6f72 726f 6c65 2072 6f6c    <colorrole rol
-00001190: 653d 2242 6173 6522 3e0a 2020 2020 2020  e="Base">.      
-000011a0: 2020 2020 2020 3c62 7275 7368 2062 7275        <brush bru
-000011b0: 7368 7374 796c 653d 2253 6f6c 6964 5061  shstyle="SolidPa
-000011c0: 7474 6572 6e22 3e0a 2020 2020 2020 2020  ttern">.        
-000011d0: 2020 2020 203c 636f 6c6f 7220 616c 7068       <color alph
-000011e0: 613d 2232 3535 223e 0a20 2020 2020 2020  a="255">.       
-000011f0: 2020 2020 2020 203c 7265 643e 3234 343c         <red>244<
-00001200: 2f72 6564 3e0a 2020 2020 2020 2020 2020  /red>.          
-00001210: 2020 2020 3c67 7265 656e 3e32 3434 3c2f      <green>244</
-00001220: 6772 6565 6e3e 0a20 2020 2020 2020 2020  green>.         
-00001230: 2020 2020 203c 626c 7565 3e32 3434 3c2f       <blue>244</
-00001240: 626c 7565 3e0a 2020 2020 2020 2020 2020  blue>.          
-00001250: 2020 203c 2f63 6f6c 6f72 3e0a 2020 2020     </color>.    
-00001260: 2020 2020 2020 2020 3c2f 6272 7573 683e          </brush>
-00001270: 0a20 2020 2020 2020 2020 2020 3c2f 636f  .           </co
-00001280: 6c6f 7272 6f6c 653e 0a20 2020 2020 2020  lorrole>.       
-00001290: 2020 203c 2f64 6973 6162 6c65 643e 0a20     </disabled>. 
-000012a0: 2020 2020 2020 2020 3c2f 7061 6c65 7474          </palett
-000012b0: 653e 0a20 2020 2020 2020 203c 2f70 726f  e>.        </pro
-000012c0: 7065 7274 793e 0a20 2020 2020 2020 203c  perty>.        <
-000012d0: 7072 6f70 6572 7479 206e 616d 653d 2272  property name="r
-000012e0: 6561 644f 6e6c 7922 3e0a 2020 2020 2020  eadOnly">.      
-000012f0: 2020 203c 626f 6f6c 3e74 7275 653c 2f62     <bool>true</b
-00001300: 6f6f 6c3e 0a20 2020 2020 2020 203c 2f70  ool>.        </p
-00001310: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00001320: 3c2f 7769 6467 6574 3e0a 2020 2020 2020  </widget>.      
-00001330: 3c2f 6974 656d 3e0a 2020 2020 2020 3c69  </item>.      <i
-00001340: 7465 6d20 726f 773d 2233 2220 636f 6c75  tem row="3" colu
-00001350: 6d6e 3d22 3022 3e0a 2020 2020 2020 203c  mn="0">.       <
-00001360: 7769 6467 6574 2063 6c61 7373 3d22 514c  widget class="QL
-00001370: 6162 656c 2220 6e61 6d65 3d22 6175 7468  abel" name="auth
-00001380: 6f72 5f6c 6162 656c 223e 0a20 2020 2020  or_label">.     
-00001390: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000013a0: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
-000013b0: 2020 203c 7374 7269 6e67 3e41 7574 686f     <string>Autho
-000013c0: 723a 203c 2f73 7472 696e 673e 0a20 2020  r: </string>.   
-000013d0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-000013e0: 0a20 2020 2020 2020 3c2f 7769 6467 6574  .       </widget
-000013f0: 3e0a 2020 2020 2020 3c2f 6974 656d 3e0a  >.      </item>.
-00001400: 2020 2020 2020 3c69 7465 6d20 726f 773d        <item row=
-00001410: 2233 2220 636f 6c75 6d6e 3d22 3122 3e0a  "3" column="1">.
-00001420: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-00001430: 6c61 7373 3d22 514c 696e 6545 6469 7422  lass="QLineEdit"
-00001440: 206e 616d 653d 2261 7574 686f 725f 6c65   name="author_le
-00001450: 223e 0a20 2020 2020 2020 203c 7072 6f70  ">.        <prop
-00001460: 6572 7479 206e 616d 653d 2270 616c 6574  erty name="palet
-00001470: 7465 223e 0a20 2020 2020 2020 2020 3c70  te">.         <p
-00001480: 616c 6574 7465 3e0a 2020 2020 2020 2020  alette>.        
-00001490: 2020 3c61 6374 6976 653e 0a20 2020 2020    <active>.     
-000014a0: 2020 2020 2020 3c63 6f6c 6f72 726f 6c65        <colorrole
-000014b0: 2072 6f6c 653d 2242 6173 6522 3e0a 2020   role="Base">.  
-000014c0: 2020 2020 2020 2020 2020 3c62 7275 7368            <brush
-000014d0: 2062 7275 7368 7374 796c 653d 2253 6f6c   brushstyle="Sol
-000014e0: 6964 5061 7474 6572 6e22 3e0a 2020 2020  idPattern">.    
-000014f0: 2020 2020 2020 2020 203c 636f 6c6f 7220           <color 
-00001500: 616c 7068 613d 2232 3535 223e 0a20 2020  alpha="255">.   
-00001510: 2020 2020 2020 2020 2020 203c 7265 643e             <red>
-00001520: 3233 393c 2f72 6564 3e0a 2020 2020 2020  239</red>.      
-00001530: 2020 2020 2020 2020 3c67 7265 656e 3e32          <green>2
-00001540: 3339 3c2f 6772 6565 6e3e 0a20 2020 2020  39</green>.     
-00001550: 2020 2020 2020 2020 203c 626c 7565 3e32           <blue>2
-00001560: 3339 3c2f 626c 7565 3e0a 2020 2020 2020  39</blue>.      
-00001570: 2020 2020 2020 203c 2f63 6f6c 6f72 3e0a         </color>.
-00001580: 2020 2020 2020 2020 2020 2020 3c2f 6272              </br
-00001590: 7573 683e 0a20 2020 2020 2020 2020 2020  ush>.           
-000015a0: 3c2f 636f 6c6f 7272 6f6c 653e 0a20 2020  </colorrole>.   
-000015b0: 2020 2020 2020 203c 2f61 6374 6976 653e         </active>
-000015c0: 0a20 2020 2020 2020 2020 203c 696e 6163  .          <inac
-000015d0: 7469 7665 3e0a 2020 2020 2020 2020 2020  tive>.          
-000015e0: 203c 636f 6c6f 7272 6f6c 6520 726f 6c65   <colorrole role
-000015f0: 3d22 4261 7365 223e 0a20 2020 2020 2020  ="Base">.       
-00001600: 2020 2020 203c 6272 7573 6820 6272 7573       <brush brus
-00001610: 6873 7479 6c65 3d22 536f 6c69 6450 6174  hstyle="SolidPat
-00001620: 7465 726e 223e 0a20 2020 2020 2020 2020  tern">.         
-00001630: 2020 2020 3c63 6f6c 6f72 2061 6c70 6861      <color alpha
-00001640: 3d22 3235 3522 3e0a 2020 2020 2020 2020  ="255">.        
-00001650: 2020 2020 2020 3c72 6564 3e32 3339 3c2f        <red>239</
-00001660: 7265 643e 0a20 2020 2020 2020 2020 2020  red>.           
-00001670: 2020 203c 6772 6565 6e3e 3233 393c 2f67     <green>239</g
-00001680: 7265 656e 3e0a 2020 2020 2020 2020 2020  reen>.          
-00001690: 2020 2020 3c62 6c75 653e 3233 393c 2f62      <blue>239</b
-000016a0: 6c75 653e 0a20 2020 2020 2020 2020 2020  lue>.           
-000016b0: 2020 3c2f 636f 6c6f 723e 0a20 2020 2020    </color>.     
-000016c0: 2020 2020 2020 203c 2f62 7275 7368 3e0a         </brush>.
-000016d0: 2020 2020 2020 2020 2020 203c 2f63 6f6c             </col
-000016e0: 6f72 726f 6c65 3e0a 2020 2020 2020 2020  orrole>.        
-000016f0: 2020 3c2f 696e 6163 7469 7665 3e0a 2020    </inactive>.  
-00001700: 2020 2020 2020 2020 3c64 6973 6162 6c65          <disable
-00001710: 643e 0a20 2020 2020 2020 2020 2020 3c63  d>.           <c
-00001720: 6f6c 6f72 726f 6c65 2072 6f6c 653d 2242  olorrole role="B
-00001730: 6173 6522 3e0a 2020 2020 2020 2020 2020  ase">.          
-00001740: 2020 3c62 7275 7368 2062 7275 7368 7374    <brush brushst
-00001750: 796c 653d 2253 6f6c 6964 5061 7474 6572  yle="SolidPatter
-00001760: 6e22 3e0a 2020 2020 2020 2020 2020 2020  n">.            
-00001770: 203c 636f 6c6f 7220 616c 7068 613d 2232   <color alpha="2
-00001780: 3535 223e 0a20 2020 2020 2020 2020 2020  55">.           
-00001790: 2020 203c 7265 643e 3234 343c 2f72 6564     <red>244</red
-000017a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000017b0: 3c67 7265 656e 3e32 3434 3c2f 6772 6565  <green>244</gree
-000017c0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
-000017d0: 203c 626c 7565 3e32 3434 3c2f 626c 7565   <blue>244</blue
-000017e0: 3e0a 2020 2020 2020 2020 2020 2020 203c  >.             <
-000017f0: 2f63 6f6c 6f72 3e0a 2020 2020 2020 2020  /color>.        
-00001800: 2020 2020 3c2f 6272 7573 683e 0a20 2020      </brush>.   
-00001810: 2020 2020 2020 2020 3c2f 636f 6c6f 7272          </colorr
-00001820: 6f6c 653e 0a20 2020 2020 2020 2020 203c  ole>.          <
-00001830: 2f64 6973 6162 6c65 643e 0a20 2020 2020  /disabled>.     
-00001840: 2020 2020 3c2f 7061 6c65 7474 653e 0a20      </palette>. 
-00001850: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00001860: 793e 0a20 2020 2020 2020 203c 7072 6f70  y>.        <prop
-00001870: 6572 7479 206e 616d 653d 2272 6561 644f  erty name="readO
-00001880: 6e6c 7922 3e0a 2020 2020 2020 2020 203c  nly">.         <
-00001890: 626f 6f6c 3e74 7275 653c 2f62 6f6f 6c3e  bool>true</bool>
-000018a0: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
-000018b0: 7274 793e 0a20 2020 2020 2020 3c2f 7769  rty>.       </wi
-000018c0: 6467 6574 3e0a 2020 2020 2020 3c2f 6974  dget>.      </it
-000018d0: 656d 3e0a 2020 2020 2020 3c69 7465 6d20  em>.      <item 
-000018e0: 726f 773d 2234 2220 636f 6c75 6d6e 3d22  row="4" column="
-000018f0: 3022 3e0a 2020 2020 2020 203c 7769 6467  0">.       <widg
-00001900: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
-00001910: 2220 6e61 6d65 3d22 6465 7363 5f6c 6162  " name="desc_lab
-00001920: 656c 223e 0a20 2020 2020 2020 203c 7072  el">.        <pr
-00001930: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
-00001940: 7422 3e0a 2020 2020 2020 2020 203c 7374  t">.         <st
-00001950: 7269 6e67 3e44 6573 7269 7074 696f 6e3a  ring>Desription:
-00001960: 203c 2f73 7472 696e 673e 0a20 2020 2020   </string>.     
-00001970: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
-00001980: 2020 2020 2020 3c2f 7769 6467 6574 3e0a        </widget>.
-00001990: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
-000019a0: 2020 2020 3c69 7465 6d20 726f 773d 2234      <item row="4
-000019b0: 2220 636f 6c75 6d6e 3d22 3122 3e0a 2020  " column="1">.  
-000019c0: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-000019d0: 7373 3d22 5154 6578 7445 6469 7422 206e  ss="QTextEdit" n
-000019e0: 616d 653d 2264 6573 635f 7465 223e 0a20  ame="desc_te">. 
-000019f0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001a00: 206e 616d 653d 2270 616c 6574 7465 223e   name="palette">
-00001a10: 0a20 2020 2020 2020 2020 3c70 616c 6574  .         <palet
-00001a20: 7465 3e0a 2020 2020 2020 2020 2020 3c61  te>.          <a
-00001a30: 6374 6976 653e 0a20 2020 2020 2020 2020  ctive>.         
-00001a40: 2020 3c63 6f6c 6f72 726f 6c65 2072 6f6c    <colorrole rol
-00001a50: 653d 2242 6173 6522 3e0a 2020 2020 2020  e="Base">.      
-00001a60: 2020 2020 2020 3c62 7275 7368 2062 7275        <brush bru
-00001a70: 7368 7374 796c 653d 2253 6f6c 6964 5061  shstyle="SolidPa
-00001a80: 7474 6572 6e22 3e0a 2020 2020 2020 2020  ttern">.        
-00001a90: 2020 2020 203c 636f 6c6f 7220 616c 7068       <color alph
-00001aa0: 613d 2232 3535 223e 0a20 2020 2020 2020  a="255">.       
-00001ab0: 2020 2020 2020 203c 7265 643e 3233 393c         <red>239<
-00001ac0: 2f72 6564 3e0a 2020 2020 2020 2020 2020  /red>.          
-00001ad0: 2020 2020 3c67 7265 656e 3e32 3339 3c2f      <green>239</
-00001ae0: 6772 6565 6e3e 0a20 2020 2020 2020 2020  green>.         
-00001af0: 2020 2020 203c 626c 7565 3e32 3339 3c2f       <blue>239</
-00001b00: 626c 7565 3e0a 2020 2020 2020 2020 2020  blue>.          
-00001b10: 2020 203c 2f63 6f6c 6f72 3e0a 2020 2020     </color>.    
-00001b20: 2020 2020 2020 2020 3c2f 6272 7573 683e          </brush>
-00001b30: 0a20 2020 2020 2020 2020 2020 3c2f 636f  .           </co
-00001b40: 6c6f 7272 6f6c 653e 0a20 2020 2020 2020  lorrole>.       
-00001b50: 2020 203c 2f61 6374 6976 653e 0a20 2020     </active>.   
-00001b60: 2020 2020 2020 203c 696e 6163 7469 7665         <inactive
-00001b70: 3e0a 2020 2020 2020 2020 2020 203c 636f  >.           <co
-00001b80: 6c6f 7272 6f6c 6520 726f 6c65 3d22 4261  lorrole role="Ba
-00001b90: 7365 223e 0a20 2020 2020 2020 2020 2020  se">.           
-00001ba0: 203c 6272 7573 6820 6272 7573 6873 7479   <brush brushsty
-00001bb0: 6c65 3d22 536f 6c69 6450 6174 7465 726e  le="SolidPattern
-00001bc0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00001bd0: 3c63 6f6c 6f72 2061 6c70 6861 3d22 3235  <color alpha="25
-00001be0: 3522 3e0a 2020 2020 2020 2020 2020 2020  5">.            
-00001bf0: 2020 3c72 6564 3e32 3339 3c2f 7265 643e    <red>239</red>
-00001c00: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00001c10: 6772 6565 6e3e 3233 393c 2f67 7265 656e  green>239</green
-00001c20: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001c30: 3c62 6c75 653e 3233 393c 2f62 6c75 653e  <blue>239</blue>
-00001c40: 0a20 2020 2020 2020 2020 2020 2020 3c2f  .             </
-00001c50: 636f 6c6f 723e 0a20 2020 2020 2020 2020  color>.         
-00001c60: 2020 203c 2f62 7275 7368 3e0a 2020 2020     </brush>.    
-00001c70: 2020 2020 2020 203c 2f63 6f6c 6f72 726f         </colorro
-00001c80: 6c65 3e0a 2020 2020 2020 2020 2020 3c2f  le>.          </
-00001c90: 696e 6163 7469 7665 3e0a 2020 2020 2020  inactive>.      
-00001ca0: 2020 2020 3c64 6973 6162 6c65 643e 0a20      <disabled>. 
-00001cb0: 2020 2020 2020 2020 2020 3c63 6f6c 6f72            <color
-00001cc0: 726f 6c65 2072 6f6c 653d 2242 6173 6522  role role="Base"
-00001cd0: 3e0a 2020 2020 2020 2020 2020 2020 3c62  >.            <b
-00001ce0: 7275 7368 2062 7275 7368 7374 796c 653d  rush brushstyle=
-00001cf0: 2253 6f6c 6964 5061 7474 6572 6e22 3e0a  "SolidPattern">.
-00001d00: 2020 2020 2020 2020 2020 2020 203c 636f               <co
-00001d10: 6c6f 7220 616c 7068 613d 2232 3535 223e  lor alpha="255">
-00001d20: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00001d30: 7265 643e 3234 343c 2f72 6564 3e0a 2020  red>244</red>.  
-00001d40: 2020 2020 2020 2020 2020 2020 3c67 7265              <gre
-00001d50: 656e 3e32 3434 3c2f 6772 6565 6e3e 0a20  en>244</green>. 
-00001d60: 2020 2020 2020 2020 2020 2020 203c 626c               <bl
-00001d70: 7565 3e32 3434 3c2f 626c 7565 3e0a 2020  ue>244</blue>.  
-00001d80: 2020 2020 2020 2020 2020 203c 2f63 6f6c             </col
-00001d90: 6f72 3e0a 2020 2020 2020 2020 2020 2020  or>.            
-00001da0: 3c2f 6272 7573 683e 0a20 2020 2020 2020  </brush>.       
-00001db0: 2020 2020 3c2f 636f 6c6f 7272 6f6c 653e      </colorrole>
-00001dc0: 0a20 2020 2020 2020 2020 203c 2f64 6973  .          </dis
-00001dd0: 6162 6c65 643e 0a20 2020 2020 2020 2020  abled>.         
-00001de0: 3c2f 7061 6c65 7474 653e 0a20 2020 2020  </palette>.     
-00001df0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
-00001e00: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001e10: 206e 616d 653d 2272 6561 644f 6e6c 7922   name="readOnly"
-00001e20: 3e0a 2020 2020 2020 2020 203c 626f 6f6c  >.         <bool
-00001e30: 3e74 7275 653c 2f62 6f6f 6c3e 0a20 2020  >true</bool>.   
-00001e40: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00001e50: 0a20 2020 2020 2020 3c2f 7769 6467 6574  .       </widget
-00001e60: 3e0a 2020 2020 2020 3c2f 6974 656d 3e0a  >.      </item>.
-00001e70: 2020 2020 203c 2f6c 6179 6f75 743e 0a20       </layout>. 
-00001e80: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
-00001e90: 3c2f 6974 656d 3e0a 2020 203c 6974 656d  </item>.   <item
-00001ea0: 3e0a 2020 2020 3c77 6964 6765 7420 636c  >.    <widget cl
-00001eb0: 6173 733d 2251 4772 6f75 7042 6f78 2220  ass="QGroupBox" 
-00001ec0: 6e61 6d65 3d22 636f 6e66 6967 4742 223e  name="configGB">
-00001ed0: 0a20 2020 2020 3c70 726f 7065 7274 7920  .     <property 
-00001ee0: 6e61 6d65 3d22 7469 746c 6522 3e0a 2020  name="title">.  
-00001ef0: 2020 2020 3c73 7472 696e 673e 536f 7274      <string>Sort
-00001f00: 696e 6720 616c 676f 7269 7468 6d3c 2f73  ing algorithm</s
-00001f10: 7472 696e 673e 0a20 2020 2020 3c2f 7072  tring>.     </pr
-00001f20: 6f70 6572 7479 3e0a 2020 2020 203c 6c61  operty>.     <la
-00001f30: 796f 7574 2063 6c61 7373 3d22 5147 7269  yout class="QGri
-00001f40: 644c 6179 6f75 7422 206e 616d 653d 2267  dLayout" name="g
-00001f50: 7269 644c 6179 6f75 745f 3222 3e0a 2020  ridLayout_2">.  
-00001f60: 2020 2020 3c69 7465 6d20 726f 773d 2230      <item row="0
-00001f70: 2220 636f 6c75 6d6e 3d22 3022 3e0a 2020  " column="0">.  
-00001f80: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-00001f90: 7373 3d22 5143 6f6d 626f 426f 7822 206e  ss="QComboBox" n
-00001fa0: 616d 653d 2261 6c67 6f72 6974 686d 735f  ame="algorithms_
-00001fb0: 636f 6d62 6f62 6f78 222f 3e0a 2020 2020  combobox"/>.    
-00001fc0: 2020 3c2f 6974 656d 3e0a 2020 2020 203c    </item>.     <
-00001fd0: 2f6c 6179 6f75 743e 0a20 2020 203c 2f77  /layout>.    </w
-00001fe0: 6964 6765 743e 0a20 2020 3c2f 6974 656d  idget>.   </item
-00001ff0: 3e0a 2020 3c2f 6c61 796f 7574 3e0a 203c  >.  </layout>. <
-00002000: 2f77 6964 6765 743e 0a20 3c72 6573 6f75  /widget>. <resou
-00002010: 7263 6573 2f3e 0a20 3c63 6f6e 6e65 6374  rces/>. <connect
-00002020: 696f 6e73 2f3e 0a3c 2f75 693e 0a         ions/>.</ui>.
+00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
+00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
+00000040: 6173 733e 4442 5472 6565 536f 7274 5061  ass>DBTreeSortPa
+00000050: 6765 3c2f 636c 6173 733e 0d0a 203c 7769  ge</class>.. <wi
+00000060: 6467 6574 2063 6c61 7373 3d22 5157 6964  dget class="QWid
+00000070: 6765 7422 206e 616d 653d 2244 4254 7265  get" name="DBTre
+00000080: 6553 6f72 7450 6167 6522 3e0d 0a20 203c  eSortPage">..  <
+00000090: 7072 6f70 6572 7479 206e 616d 653d 2267  property name="g
+000000a0: 656f 6d65 7472 7922 3e0d 0a20 2020 3c72  eometry">..   <r
+000000b0: 6563 743e 0d0a 2020 2020 3c78 3e30 3c2f  ect>..    <x>0</
+000000c0: 783e 0d0a 2020 2020 3c79 3e30 3c2f 793e  x>..    <y>0</y>
+000000d0: 0d0a 2020 2020 3c77 6964 7468 3e34 3030  ..    <width>400
+000000e0: 3c2f 7769 6474 683e 0d0a 2020 2020 3c68  </width>..    <h
+000000f0: 6569 6768 743e 3437 333c 2f68 6569 6768  eight>473</heigh
+00000100: 743e 0d0a 2020 203c 2f72 6563 743e 0d0a  t>..   </rect>..
+00000110: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
+00000120: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000130: 2277 696e 646f 7754 6974 6c65 223e 0d0a  "windowTitle">..
+00000140: 2020 203c 7374 7269 6e67 3e46 6f72 6d3c     <string>Form<
+00000150: 2f73 7472 696e 673e 0d0a 2020 3c2f 7072  /string>..  </pr
+00000160: 6f70 6572 7479 3e0d 0a20 203c 6c61 796f  operty>..  <layo
+00000170: 7574 2063 6c61 7373 3d22 5156 426f 784c  ut class="QVBoxL
+00000180: 6179 6f75 7422 206e 616d 653d 2276 6572  ayout" name="ver
+00000190: 7469 6361 6c4c 6179 6f75 7422 3e0d 0a20  ticalLayout">.. 
+000001a0: 2020 3c69 7465 6d3e 0d0a 2020 2020 3c77    <item>..    <w
+000001b0: 6964 6765 7420 636c 6173 733d 2251 4772  idget class="QGr
+000001c0: 6f75 7042 6f78 2220 6e61 6d65 3d22 6465  oupBox" name="de
+000001d0: 7363 4742 223e 0d0a 2020 2020 203c 7072  scGB">..     <pr
+000001e0: 6f70 6572 7479 206e 616d 653d 2274 6974  operty name="tit
+000001f0: 6c65 223e 0d0a 2020 2020 2020 3c73 7472  le">..      <str
+00000200: 696e 673e 506c 7567 696e 2064 6573 6372  ing>Plugin descr
+00000210: 6970 7469 6f6e 3c2f 7374 7269 6e67 3e0d  iption</string>.
+00000220: 0a20 2020 2020 3c2f 7072 6f70 6572 7479  .     </property
+00000230: 3e0d 0a20 2020 2020 3c6c 6179 6f75 7420  >..     <layout 
+00000240: 636c 6173 733d 2251 4772 6964 4c61 796f  class="QGridLayo
+00000250: 7574 2220 6e61 6d65 3d22 6772 6964 4c61  ut" name="gridLa
+00000260: 796f 7574 223e 0d0a 2020 2020 2020 3c69  yout">..      <i
+00000270: 7465 6d20 726f 773d 2230 2220 636f 6c75  tem row="0" colu
+00000280: 6d6e 3d22 3022 3e0d 0a20 2020 2020 2020  mn="0">..       
+00000290: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+000002a0: 4c61 6265 6c22 206e 616d 653d 2276 6572  Label" name="ver
+000002b0: 7369 6f6e 5f6c 6162 656c 223e 0d0a 2020  sion_label">..  
+000002c0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000002d0: 6e61 6d65 3d22 7465 7874 223e 0d0a 2020  name="text">..  
+000002e0: 2020 2020 2020 203c 7374 7269 6e67 3e56         <string>V
+000002f0: 6572 7369 6f6e 3a20 3c2f 7374 7269 6e67  ersion: </string
+00000300: 3e0d 0a20 2020 2020 2020 203c 2f70 726f  >..        </pro
+00000310: 7065 7274 793e 0d0a 2020 2020 2020 203c  perty>..       <
+00000320: 2f77 6964 6765 743e 0d0a 2020 2020 2020  /widget>..      
+00000330: 3c2f 6974 656d 3e0d 0a20 2020 2020 203c  </item>..      <
+00000340: 6974 656d 2072 6f77 3d22 3022 2063 6f6c  item row="0" col
+00000350: 756d 6e3d 2231 223e 0d0a 2020 2020 2020  umn="1">..      
+00000360: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
+00000370: 514c 696e 6545 6469 7422 206e 616d 653d  QLineEdit" name=
+00000380: 2276 6572 7369 6f6e 5f6c 6522 3e0d 0a20  "version_le">.. 
+00000390: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000003a0: 206e 616d 653d 2270 616c 6574 7465 223e   name="palette">
+000003b0: 0d0a 2020 2020 2020 2020 203c 7061 6c65  ..         <pale
+000003c0: 7474 653e 0d0a 2020 2020 2020 2020 2020  tte>..          
+000003d0: 3c61 6374 6976 653e 0d0a 2020 2020 2020  <active>..      
+000003e0: 2020 2020 203c 636f 6c6f 7272 6f6c 6520       <colorrole 
+000003f0: 726f 6c65 3d22 4261 7365 223e 0d0a 2020  role="Base">..  
+00000400: 2020 2020 2020 2020 2020 3c62 7275 7368            <brush
+00000410: 2062 7275 7368 7374 796c 653d 2253 6f6c   brushstyle="Sol
+00000420: 6964 5061 7474 6572 6e22 3e0d 0a20 2020  idPattern">..   
+00000430: 2020 2020 2020 2020 2020 3c63 6f6c 6f72            <color
+00000440: 2061 6c70 6861 3d22 3235 3522 3e0d 0a20   alpha="255">.. 
+00000450: 2020 2020 2020 2020 2020 2020 203c 7265               <re
+00000460: 643e 3233 393c 2f72 6564 3e0d 0a20 2020  d>239</red>..   
+00000470: 2020 2020 2020 2020 2020 203c 6772 6565             <gree
+00000480: 6e3e 3233 393c 2f67 7265 656e 3e0d 0a20  n>239</green>.. 
+00000490: 2020 2020 2020 2020 2020 2020 203c 626c               <bl
+000004a0: 7565 3e32 3339 3c2f 626c 7565 3e0d 0a20  ue>239</blue>.. 
+000004b0: 2020 2020 2020 2020 2020 2020 3c2f 636f              </co
+000004c0: 6c6f 723e 0d0a 2020 2020 2020 2020 2020  lor>..          
+000004d0: 2020 3c2f 6272 7573 683e 0d0a 2020 2020    </brush>..    
+000004e0: 2020 2020 2020 203c 2f63 6f6c 6f72 726f         </colorro
+000004f0: 6c65 3e0d 0a20 2020 2020 2020 2020 203c  le>..          <
+00000500: 2f61 6374 6976 653e 0d0a 2020 2020 2020  /active>..      
+00000510: 2020 2020 3c69 6e61 6374 6976 653e 0d0a      <inactive>..
+00000520: 2020 2020 2020 2020 2020 203c 636f 6c6f             <colo
+00000530: 7272 6f6c 6520 726f 6c65 3d22 4261 7365  rrole role="Base
+00000540: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00000550: 3c62 7275 7368 2062 7275 7368 7374 796c  <brush brushstyl
+00000560: 653d 2253 6f6c 6964 5061 7474 6572 6e22  e="SolidPattern"
+00000570: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000580: 3c63 6f6c 6f72 2061 6c70 6861 3d22 3235  <color alpha="25
+00000590: 3522 3e0d 0a20 2020 2020 2020 2020 2020  5">..           
+000005a0: 2020 203c 7265 643e 3233 393c 2f72 6564     <red>239</red
+000005b0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000005c0: 203c 6772 6565 6e3e 3233 393c 2f67 7265   <green>239</gre
+000005d0: 656e 3e0d 0a20 2020 2020 2020 2020 2020  en>..           
+000005e0: 2020 203c 626c 7565 3e32 3339 3c2f 626c     <blue>239</bl
+000005f0: 7565 3e0d 0a20 2020 2020 2020 2020 2020  ue>..           
+00000600: 2020 3c2f 636f 6c6f 723e 0d0a 2020 2020    </color>..    
+00000610: 2020 2020 2020 2020 3c2f 6272 7573 683e          </brush>
+00000620: 0d0a 2020 2020 2020 2020 2020 203c 2f63  ..           </c
+00000630: 6f6c 6f72 726f 6c65 3e0d 0a20 2020 2020  olorrole>..     
+00000640: 2020 2020 203c 2f69 6e61 6374 6976 653e       </inactive>
+00000650: 0d0a 2020 2020 2020 2020 2020 3c64 6973  ..          <dis
+00000660: 6162 6c65 643e 0d0a 2020 2020 2020 2020  abled>..        
+00000670: 2020 203c 636f 6c6f 7272 6f6c 6520 726f     <colorrole ro
+00000680: 6c65 3d22 4261 7365 223e 0d0a 2020 2020  le="Base">..    
+00000690: 2020 2020 2020 2020 3c62 7275 7368 2062          <brush b
+000006a0: 7275 7368 7374 796c 653d 2253 6f6c 6964  rushstyle="Solid
+000006b0: 5061 7474 6572 6e22 3e0d 0a20 2020 2020  Pattern">..     
+000006c0: 2020 2020 2020 2020 3c63 6f6c 6f72 2061          <color a
+000006d0: 6c70 6861 3d22 3235 3522 3e0d 0a20 2020  lpha="255">..   
+000006e0: 2020 2020 2020 2020 2020 203c 7265 643e             <red>
+000006f0: 3234 343c 2f72 6564 3e0d 0a20 2020 2020  244</red>..     
+00000700: 2020 2020 2020 2020 203c 6772 6565 6e3e           <green>
+00000710: 3234 343c 2f67 7265 656e 3e0d 0a20 2020  244</green>..   
+00000720: 2020 2020 2020 2020 2020 203c 626c 7565             <blue
+00000730: 3e32 3434 3c2f 626c 7565 3e0d 0a20 2020  >244</blue>..   
+00000740: 2020 2020 2020 2020 2020 3c2f 636f 6c6f            </colo
+00000750: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
+00000760: 3c2f 6272 7573 683e 0d0a 2020 2020 2020  </brush>..      
+00000770: 2020 2020 203c 2f63 6f6c 6f72 726f 6c65       </colorrole
+00000780: 3e0d 0a20 2020 2020 2020 2020 203c 2f64  >..          </d
+00000790: 6973 6162 6c65 643e 0d0a 2020 2020 2020  isabled>..      
+000007a0: 2020 203c 2f70 616c 6574 7465 3e0d 0a20     </palette>.. 
+000007b0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+000007c0: 793e 0d0a 2020 2020 2020 2020 3c70 726f  y>..        <pro
+000007d0: 7065 7274 7920 6e61 6d65 3d22 7265 6164  perty name="read
+000007e0: 4f6e 6c79 223e 0d0a 2020 2020 2020 2020  Only">..        
+000007f0: 203c 626f 6f6c 3e74 7275 653c 2f62 6f6f   <bool>true</boo
+00000800: 6c3e 0d0a 2020 2020 2020 2020 3c2f 7072  l>..        </pr
+00000810: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00000820: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
+00000830: 203c 2f69 7465 6d3e 0d0a 2020 2020 2020   </item>..      
+00000840: 3c69 7465 6d20 726f 773d 2231 2220 636f  <item row="1" co
+00000850: 6c75 6d6e 3d22 3022 3e0d 0a20 2020 2020  lumn="0">..     
+00000860: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00000870: 2251 4c61 6265 6c22 206e 616d 653d 226d  "QLabel" name="m
+00000880: 6f64 756c 655f 6e61 6d65 5f6c 6162 656c  odule_name_label
+00000890: 223e 0d0a 2020 2020 2020 2020 3c70 726f  ">..        <pro
+000008a0: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
+000008b0: 223e 0d0a 2020 2020 2020 2020 203c 7374  ">..         <st
+000008c0: 7269 6e67 3e4d 6f64 756c 6520 6e61 6d65  ring>Module name
+000008d0: 3a20 3c2f 7374 7269 6e67 3e0d 0a20 2020  : </string>..   
+000008e0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+000008f0: 0d0a 2020 2020 2020 203c 2f77 6964 6765  ..       </widge
+00000900: 743e 0d0a 2020 2020 2020 3c2f 6974 656d  t>..      </item
+00000910: 3e0d 0a20 2020 2020 203c 6974 656d 2072  >..      <item r
+00000920: 6f77 3d22 3122 2063 6f6c 756d 6e3d 2231  ow="1" column="1
+00000930: 223e 0d0a 2020 2020 2020 203c 7769 6467  ">..       <widg
+00000940: 6574 2063 6c61 7373 3d22 514c 696e 6545  et class="QLineE
+00000950: 6469 7422 206e 616d 653d 226d 6f64 756c  dit" name="modul
+00000960: 655f 6e61 6d65 5f6c 6522 3e0d 0a20 2020  e_name_le">..   
+00000970: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000980: 616d 653d 2270 616c 6574 7465 223e 0d0a  ame="palette">..
+00000990: 2020 2020 2020 2020 203c 7061 6c65 7474           <palett
+000009a0: 653e 0d0a 2020 2020 2020 2020 2020 3c61  e>..          <a
+000009b0: 6374 6976 653e 0d0a 2020 2020 2020 2020  ctive>..        
+000009c0: 2020 203c 636f 6c6f 7272 6f6c 6520 726f     <colorrole ro
+000009d0: 6c65 3d22 4261 7365 223e 0d0a 2020 2020  le="Base">..    
+000009e0: 2020 2020 2020 2020 3c62 7275 7368 2062          <brush b
+000009f0: 7275 7368 7374 796c 653d 2253 6f6c 6964  rushstyle="Solid
+00000a00: 5061 7474 6572 6e22 3e0d 0a20 2020 2020  Pattern">..     
+00000a10: 2020 2020 2020 2020 3c63 6f6c 6f72 2061          <color a
+00000a20: 6c70 6861 3d22 3235 3522 3e0d 0a20 2020  lpha="255">..   
+00000a30: 2020 2020 2020 2020 2020 203c 7265 643e             <red>
+00000a40: 3233 393c 2f72 6564 3e0d 0a20 2020 2020  239</red>..     
+00000a50: 2020 2020 2020 2020 203c 6772 6565 6e3e           <green>
+00000a60: 3233 393c 2f67 7265 656e 3e0d 0a20 2020  239</green>..   
+00000a70: 2020 2020 2020 2020 2020 203c 626c 7565             <blue
+00000a80: 3e32 3339 3c2f 626c 7565 3e0d 0a20 2020  >239</blue>..   
+00000a90: 2020 2020 2020 2020 2020 3c2f 636f 6c6f            </colo
+00000aa0: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
+00000ab0: 3c2f 6272 7573 683e 0d0a 2020 2020 2020  </brush>..      
+00000ac0: 2020 2020 203c 2f63 6f6c 6f72 726f 6c65       </colorrole
+00000ad0: 3e0d 0a20 2020 2020 2020 2020 203c 2f61  >..          </a
+00000ae0: 6374 6976 653e 0d0a 2020 2020 2020 2020  ctive>..        
+00000af0: 2020 3c69 6e61 6374 6976 653e 0d0a 2020    <inactive>..  
+00000b00: 2020 2020 2020 2020 203c 636f 6c6f 7272           <colorr
+00000b10: 6f6c 6520 726f 6c65 3d22 4261 7365 223e  ole role="Base">
+00000b20: 0d0a 2020 2020 2020 2020 2020 2020 3c62  ..            <b
+00000b30: 7275 7368 2062 7275 7368 7374 796c 653d  rush brushstyle=
+00000b40: 2253 6f6c 6964 5061 7474 6572 6e22 3e0d  "SolidPattern">.
+00000b50: 0a20 2020 2020 2020 2020 2020 2020 3c63  .             <c
+00000b60: 6f6c 6f72 2061 6c70 6861 3d22 3235 3522  olor alpha="255"
+00000b70: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000b80: 203c 7265 643e 3233 393c 2f72 6564 3e0d   <red>239</red>.
+00000b90: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00000ba0: 6772 6565 6e3e 3233 393c 2f67 7265 656e  green>239</green
+00000bb0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000bc0: 203c 626c 7565 3e32 3339 3c2f 626c 7565   <blue>239</blue
+00000bd0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000be0: 3c2f 636f 6c6f 723e 0d0a 2020 2020 2020  </color>..      
+00000bf0: 2020 2020 2020 3c2f 6272 7573 683e 0d0a        </brush>..
+00000c00: 2020 2020 2020 2020 2020 203c 2f63 6f6c             </col
+00000c10: 6f72 726f 6c65 3e0d 0a20 2020 2020 2020  orrole>..       
+00000c20: 2020 203c 2f69 6e61 6374 6976 653e 0d0a     </inactive>..
+00000c30: 2020 2020 2020 2020 2020 3c64 6973 6162            <disab
+00000c40: 6c65 643e 0d0a 2020 2020 2020 2020 2020  led>..          
+00000c50: 203c 636f 6c6f 7272 6f6c 6520 726f 6c65   <colorrole role
+00000c60: 3d22 4261 7365 223e 0d0a 2020 2020 2020  ="Base">..      
+00000c70: 2020 2020 2020 3c62 7275 7368 2062 7275        <brush bru
+00000c80: 7368 7374 796c 653d 2253 6f6c 6964 5061  shstyle="SolidPa
+00000c90: 7474 6572 6e22 3e0d 0a20 2020 2020 2020  ttern">..       
+00000ca0: 2020 2020 2020 3c63 6f6c 6f72 2061 6c70        <color alp
+00000cb0: 6861 3d22 3235 3522 3e0d 0a20 2020 2020  ha="255">..     
+00000cc0: 2020 2020 2020 2020 203c 7265 643e 3234           <red>24
+00000cd0: 343c 2f72 6564 3e0d 0a20 2020 2020 2020  4</red>..       
+00000ce0: 2020 2020 2020 203c 6772 6565 6e3e 3234         <green>24
+00000cf0: 343c 2f67 7265 656e 3e0d 0a20 2020 2020  4</green>..     
+00000d00: 2020 2020 2020 2020 203c 626c 7565 3e32           <blue>2
+00000d10: 3434 3c2f 626c 7565 3e0d 0a20 2020 2020  44</blue>..     
+00000d20: 2020 2020 2020 2020 3c2f 636f 6c6f 723e          </color>
+00000d30: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
+00000d40: 6272 7573 683e 0d0a 2020 2020 2020 2020  brush>..        
+00000d50: 2020 203c 2f63 6f6c 6f72 726f 6c65 3e0d     </colorrole>.
+00000d60: 0a20 2020 2020 2020 2020 203c 2f64 6973  .          </dis
+00000d70: 6162 6c65 643e 0d0a 2020 2020 2020 2020  abled>..        
+00000d80: 203c 2f70 616c 6574 7465 3e0d 0a20 2020   </palette>..   
+00000d90: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+00000da0: 0d0a 2020 2020 2020 2020 3c70 726f 7065  ..        <prope
+00000db0: 7274 7920 6e61 6d65 3d22 7265 6164 4f6e  rty name="readOn
+00000dc0: 6c79 223e 0d0a 2020 2020 2020 2020 203c  ly">..         <
+00000dd0: 626f 6f6c 3e74 7275 653c 2f62 6f6f 6c3e  bool>true</bool>
+00000de0: 0d0a 2020 2020 2020 2020 3c2f 7072 6f70  ..        </prop
+00000df0: 6572 7479 3e0d 0a20 2020 2020 2020 3c2f  erty>..       </
+00000e00: 7769 6467 6574 3e0d 0a20 2020 2020 203c  widget>..      <
+00000e10: 2f69 7465 6d3e 0d0a 2020 2020 2020 3c69  /item>..      <i
+00000e20: 7465 6d20 726f 773d 2232 2220 636f 6c75  tem row="2" colu
+00000e30: 6d6e 3d22 3022 3e0d 0a20 2020 2020 2020  mn="0">..       
+00000e40: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+00000e50: 4c61 6265 6c22 206e 616d 653d 2266 6f6c  Label" name="fol
+00000e60: 6465 725f 6c61 6265 6c22 3e0d 0a20 2020  der_label">..   
+00000e70: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000e80: 616d 653d 2274 6578 7422 3e0d 0a20 2020  ame="text">..   
+00000e90: 2020 2020 2020 3c73 7472 696e 673e 466f        <string>Fo
+00000ea0: 6c64 6572 3a20 3c2f 7374 7269 6e67 3e0d  lder: </string>.
+00000eb0: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
+00000ec0: 7274 793e 0d0a 2020 2020 2020 203c 2f77  rty>..       </w
+00000ed0: 6964 6765 743e 0d0a 2020 2020 2020 3c2f  idget>..      </
+00000ee0: 6974 656d 3e0d 0a20 2020 2020 203c 6974  item>..      <it
+00000ef0: 656d 2072 6f77 3d22 3222 2063 6f6c 756d  em row="2" colum
+00000f00: 6e3d 2231 223e 0d0a 2020 2020 2020 203c  n="1">..       <
+00000f10: 7769 6467 6574 2063 6c61 7373 3d22 514c  widget class="QL
+00000f20: 696e 6545 6469 7422 206e 616d 653d 2266  ineEdit" name="f
+00000f30: 6f6c 6465 725f 6c65 223e 0d0a 2020 2020  older_le">..    
+00000f40: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00000f50: 6d65 3d22 7061 6c65 7474 6522 3e0d 0a20  me="palette">.. 
+00000f60: 2020 2020 2020 2020 3c70 616c 6574 7465          <palette
+00000f70: 3e0d 0a20 2020 2020 2020 2020 203c 6163  >..          <ac
+00000f80: 7469 7665 3e0d 0a20 2020 2020 2020 2020  tive>..         
+00000f90: 2020 3c63 6f6c 6f72 726f 6c65 2072 6f6c    <colorrole rol
+00000fa0: 653d 2242 6173 6522 3e0d 0a20 2020 2020  e="Base">..     
+00000fb0: 2020 2020 2020 203c 6272 7573 6820 6272         <brush br
+00000fc0: 7573 6873 7479 6c65 3d22 536f 6c69 6450  ushstyle="SolidP
+00000fd0: 6174 7465 726e 223e 0d0a 2020 2020 2020  attern">..      
+00000fe0: 2020 2020 2020 203c 636f 6c6f 7220 616c         <color al
+00000ff0: 7068 613d 2232 3535 223e 0d0a 2020 2020  pha="255">..    
+00001000: 2020 2020 2020 2020 2020 3c72 6564 3e32            <red>2
+00001010: 3339 3c2f 7265 643e 0d0a 2020 2020 2020  39</red>..      
+00001020: 2020 2020 2020 2020 3c67 7265 656e 3e32          <green>2
+00001030: 3339 3c2f 6772 6565 6e3e 0d0a 2020 2020  39</green>..    
+00001040: 2020 2020 2020 2020 2020 3c62 6c75 653e            <blue>
+00001050: 3233 393c 2f62 6c75 653e 0d0a 2020 2020  239</blue>..    
+00001060: 2020 2020 2020 2020 203c 2f63 6f6c 6f72           </color
+00001070: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00001080: 2f62 7275 7368 3e0d 0a20 2020 2020 2020  /brush>..       
+00001090: 2020 2020 3c2f 636f 6c6f 7272 6f6c 653e      </colorrole>
+000010a0: 0d0a 2020 2020 2020 2020 2020 3c2f 6163  ..          </ac
+000010b0: 7469 7665 3e0d 0a20 2020 2020 2020 2020  tive>..         
+000010c0: 203c 696e 6163 7469 7665 3e0d 0a20 2020   <inactive>..   
+000010d0: 2020 2020 2020 2020 3c63 6f6c 6f72 726f          <colorro
+000010e0: 6c65 2072 6f6c 653d 2242 6173 6522 3e0d  le role="Base">.
+000010f0: 0a20 2020 2020 2020 2020 2020 203c 6272  .            <br
+00001100: 7573 6820 6272 7573 6873 7479 6c65 3d22  ush brushstyle="
+00001110: 536f 6c69 6450 6174 7465 726e 223e 0d0a  SolidPattern">..
+00001120: 2020 2020 2020 2020 2020 2020 203c 636f               <co
+00001130: 6c6f 7220 616c 7068 613d 2232 3535 223e  lor alpha="255">
+00001140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001150: 3c72 6564 3e32 3339 3c2f 7265 643e 0d0a  <red>239</red>..
+00001160: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
+00001170: 7265 656e 3e32 3339 3c2f 6772 6565 6e3e  reen>239</green>
+00001180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001190: 3c62 6c75 653e 3233 393c 2f62 6c75 653e  <blue>239</blue>
+000011a0: 0d0a 2020 2020 2020 2020 2020 2020 203c  ..             <
+000011b0: 2f63 6f6c 6f72 3e0d 0a20 2020 2020 2020  /color>..       
+000011c0: 2020 2020 203c 2f62 7275 7368 3e0d 0a20       </brush>.. 
+000011d0: 2020 2020 2020 2020 2020 3c2f 636f 6c6f            </colo
+000011e0: 7272 6f6c 653e 0d0a 2020 2020 2020 2020  rrole>..        
+000011f0: 2020 3c2f 696e 6163 7469 7665 3e0d 0a20    </inactive>.. 
+00001200: 2020 2020 2020 2020 203c 6469 7361 626c           <disabl
+00001210: 6564 3e0d 0a20 2020 2020 2020 2020 2020  ed>..           
+00001220: 3c63 6f6c 6f72 726f 6c65 2072 6f6c 653d  <colorrole role=
+00001230: 2242 6173 6522 3e0d 0a20 2020 2020 2020  "Base">..       
+00001240: 2020 2020 203c 6272 7573 6820 6272 7573       <brush brus
+00001250: 6873 7479 6c65 3d22 536f 6c69 6450 6174  hstyle="SolidPat
+00001260: 7465 726e 223e 0d0a 2020 2020 2020 2020  tern">..        
+00001270: 2020 2020 203c 636f 6c6f 7220 616c 7068       <color alph
+00001280: 613d 2232 3535 223e 0d0a 2020 2020 2020  a="255">..      
+00001290: 2020 2020 2020 2020 3c72 6564 3e32 3434          <red>244
+000012a0: 3c2f 7265 643e 0d0a 2020 2020 2020 2020  </red>..        
+000012b0: 2020 2020 2020 3c67 7265 656e 3e32 3434        <green>244
+000012c0: 3c2f 6772 6565 6e3e 0d0a 2020 2020 2020  </green>..      
+000012d0: 2020 2020 2020 2020 3c62 6c75 653e 3234          <blue>24
+000012e0: 343c 2f62 6c75 653e 0d0a 2020 2020 2020  4</blue>..      
+000012f0: 2020 2020 2020 203c 2f63 6f6c 6f72 3e0d         </color>.
+00001300: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+00001310: 7275 7368 3e0d 0a20 2020 2020 2020 2020  rush>..         
+00001320: 2020 3c2f 636f 6c6f 7272 6f6c 653e 0d0a    </colorrole>..
+00001330: 2020 2020 2020 2020 2020 3c2f 6469 7361            </disa
+00001340: 626c 6564 3e0d 0a20 2020 2020 2020 2020  bled>..         
+00001350: 3c2f 7061 6c65 7474 653e 0d0a 2020 2020  </palette>..    
+00001360: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
+00001370: 0a20 2020 2020 2020 203c 7072 6f70 6572  .        <proper
+00001380: 7479 206e 616d 653d 2272 6561 644f 6e6c  ty name="readOnl
+00001390: 7922 3e0d 0a20 2020 2020 2020 2020 3c62  y">..         <b
+000013a0: 6f6f 6c3e 7472 7565 3c2f 626f 6f6c 3e0d  ool>true</bool>.
+000013b0: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
+000013c0: 7274 793e 0d0a 2020 2020 2020 203c 2f77  rty>..       </w
+000013d0: 6964 6765 743e 0d0a 2020 2020 2020 3c2f  idget>..      </
+000013e0: 6974 656d 3e0d 0a20 2020 2020 203c 6974  item>..      <it
+000013f0: 656d 2072 6f77 3d22 3322 2063 6f6c 756d  em row="3" colum
+00001400: 6e3d 2230 223e 0d0a 2020 2020 2020 203c  n="0">..       <
+00001410: 7769 6467 6574 2063 6c61 7373 3d22 514c  widget class="QL
+00001420: 6162 656c 2220 6e61 6d65 3d22 6175 7468  abel" name="auth
+00001430: 6f72 5f6c 6162 656c 223e 0d0a 2020 2020  or_label">..    
+00001440: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001450: 6d65 3d22 7465 7874 223e 0d0a 2020 2020  me="text">..    
+00001460: 2020 2020 203c 7374 7269 6e67 3e41 7574       <string>Aut
+00001470: 686f 723a 203c 2f73 7472 696e 673e 0d0a  hor: </string>..
+00001480: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+00001490: 7479 3e0d 0a20 2020 2020 2020 3c2f 7769  ty>..       </wi
+000014a0: 6467 6574 3e0d 0a20 2020 2020 203c 2f69  dget>..      </i
+000014b0: 7465 6d3e 0d0a 2020 2020 2020 3c69 7465  tem>..      <ite
+000014c0: 6d20 726f 773d 2233 2220 636f 6c75 6d6e  m row="3" column
+000014d0: 3d22 3122 3e0d 0a20 2020 2020 2020 3c77  ="1">..       <w
+000014e0: 6964 6765 7420 636c 6173 733d 2251 4c69  idget class="QLi
+000014f0: 6e65 4564 6974 2220 6e61 6d65 3d22 6175  neEdit" name="au
+00001500: 7468 6f72 5f6c 6522 3e0d 0a20 2020 2020  thor_le">..     
+00001510: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00001520: 653d 2270 616c 6574 7465 223e 0d0a 2020  e="palette">..  
+00001530: 2020 2020 2020 203c 7061 6c65 7474 653e         <palette>
+00001540: 0d0a 2020 2020 2020 2020 2020 3c61 6374  ..          <act
+00001550: 6976 653e 0d0a 2020 2020 2020 2020 2020  ive>..          
+00001560: 203c 636f 6c6f 7272 6f6c 6520 726f 6c65   <colorrole role
+00001570: 3d22 4261 7365 223e 0d0a 2020 2020 2020  ="Base">..      
+00001580: 2020 2020 2020 3c62 7275 7368 2062 7275        <brush bru
+00001590: 7368 7374 796c 653d 2253 6f6c 6964 5061  shstyle="SolidPa
+000015a0: 7474 6572 6e22 3e0d 0a20 2020 2020 2020  ttern">..       
+000015b0: 2020 2020 2020 3c63 6f6c 6f72 2061 6c70        <color alp
+000015c0: 6861 3d22 3235 3522 3e0d 0a20 2020 2020  ha="255">..     
+000015d0: 2020 2020 2020 2020 203c 7265 643e 3233           <red>23
+000015e0: 393c 2f72 6564 3e0d 0a20 2020 2020 2020  9</red>..       
+000015f0: 2020 2020 2020 203c 6772 6565 6e3e 3233         <green>23
+00001600: 393c 2f67 7265 656e 3e0d 0a20 2020 2020  9</green>..     
+00001610: 2020 2020 2020 2020 203c 626c 7565 3e32           <blue>2
+00001620: 3339 3c2f 626c 7565 3e0d 0a20 2020 2020  39</blue>..     
+00001630: 2020 2020 2020 2020 3c2f 636f 6c6f 723e          </color>
+00001640: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
+00001650: 6272 7573 683e 0d0a 2020 2020 2020 2020  brush>..        
+00001660: 2020 203c 2f63 6f6c 6f72 726f 6c65 3e0d     </colorrole>.
+00001670: 0a20 2020 2020 2020 2020 203c 2f61 6374  .          </act
+00001680: 6976 653e 0d0a 2020 2020 2020 2020 2020  ive>..          
+00001690: 3c69 6e61 6374 6976 653e 0d0a 2020 2020  <inactive>..    
+000016a0: 2020 2020 2020 203c 636f 6c6f 7272 6f6c         <colorrol
+000016b0: 6520 726f 6c65 3d22 4261 7365 223e 0d0a  e role="Base">..
+000016c0: 2020 2020 2020 2020 2020 2020 3c62 7275              <bru
+000016d0: 7368 2062 7275 7368 7374 796c 653d 2253  sh brushstyle="S
+000016e0: 6f6c 6964 5061 7474 6572 6e22 3e0d 0a20  olidPattern">.. 
+000016f0: 2020 2020 2020 2020 2020 2020 3c63 6f6c              <col
+00001700: 6f72 2061 6c70 6861 3d22 3235 3522 3e0d  or alpha="255">.
+00001710: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00001720: 7265 643e 3233 393c 2f72 6564 3e0d 0a20  red>239</red>.. 
+00001730: 2020 2020 2020 2020 2020 2020 203c 6772               <gr
+00001740: 6565 6e3e 3233 393c 2f67 7265 656e 3e0d  een>239</green>.
+00001750: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00001760: 626c 7565 3e32 3339 3c2f 626c 7565 3e0d  blue>239</blue>.
+00001770: 0a20 2020 2020 2020 2020 2020 2020 3c2f  .             </
+00001780: 636f 6c6f 723e 0d0a 2020 2020 2020 2020  color>..        
+00001790: 2020 2020 3c2f 6272 7573 683e 0d0a 2020      </brush>..  
+000017a0: 2020 2020 2020 2020 203c 2f63 6f6c 6f72           </color
+000017b0: 726f 6c65 3e0d 0a20 2020 2020 2020 2020  role>..         
+000017c0: 203c 2f69 6e61 6374 6976 653e 0d0a 2020   </inactive>..  
+000017d0: 2020 2020 2020 2020 3c64 6973 6162 6c65          <disable
+000017e0: 643e 0d0a 2020 2020 2020 2020 2020 203c  d>..           <
+000017f0: 636f 6c6f 7272 6f6c 6520 726f 6c65 3d22  colorrole role="
+00001800: 4261 7365 223e 0d0a 2020 2020 2020 2020  Base">..        
+00001810: 2020 2020 3c62 7275 7368 2062 7275 7368      <brush brush
+00001820: 7374 796c 653d 2253 6f6c 6964 5061 7474  style="SolidPatt
+00001830: 6572 6e22 3e0d 0a20 2020 2020 2020 2020  ern">..         
+00001840: 2020 2020 3c63 6f6c 6f72 2061 6c70 6861      <color alpha
+00001850: 3d22 3235 3522 3e0d 0a20 2020 2020 2020  ="255">..       
+00001860: 2020 2020 2020 203c 7265 643e 3234 343c         <red>244<
+00001870: 2f72 6564 3e0d 0a20 2020 2020 2020 2020  /red>..         
+00001880: 2020 2020 203c 6772 6565 6e3e 3234 343c       <green>244<
+00001890: 2f67 7265 656e 3e0d 0a20 2020 2020 2020  /green>..       
+000018a0: 2020 2020 2020 203c 626c 7565 3e32 3434         <blue>244
+000018b0: 3c2f 626c 7565 3e0d 0a20 2020 2020 2020  </blue>..       
+000018c0: 2020 2020 2020 3c2f 636f 6c6f 723e 0d0a        </color>..
+000018d0: 2020 2020 2020 2020 2020 2020 3c2f 6272              </br
+000018e0: 7573 683e 0d0a 2020 2020 2020 2020 2020  ush>..          
+000018f0: 203c 2f63 6f6c 6f72 726f 6c65 3e0d 0a20   </colorrole>.. 
+00001900: 2020 2020 2020 2020 203c 2f64 6973 6162           </disab
+00001910: 6c65 643e 0d0a 2020 2020 2020 2020 203c  led>..         <
+00001920: 2f70 616c 6574 7465 3e0d 0a20 2020 2020  /palette>..     
+00001930: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+00001940: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00001950: 7920 6e61 6d65 3d22 7265 6164 4f6e 6c79  y name="readOnly
+00001960: 223e 0d0a 2020 2020 2020 2020 203c 626f  ">..         <bo
+00001970: 6f6c 3e74 7275 653c 2f62 6f6f 6c3e 0d0a  ol>true</bool>..
+00001980: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+00001990: 7479 3e0d 0a20 2020 2020 2020 3c2f 7769  ty>..       </wi
+000019a0: 6467 6574 3e0d 0a20 2020 2020 203c 2f69  dget>..      </i
+000019b0: 7465 6d3e 0d0a 2020 2020 2020 3c69 7465  tem>..      <ite
+000019c0: 6d20 726f 773d 2234 2220 636f 6c75 6d6e  m row="4" column
+000019d0: 3d22 3022 3e0d 0a20 2020 2020 2020 3c77  ="0">..       <w
+000019e0: 6964 6765 7420 636c 6173 733d 2251 4c61  idget class="QLa
+000019f0: 6265 6c22 206e 616d 653d 2264 6573 635f  bel" name="desc_
+00001a00: 6c61 6265 6c22 3e0d 0a20 2020 2020 2020  label">..       
+00001a10: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00001a20: 2274 6578 7422 3e0d 0a20 2020 2020 2020  "text">..       
+00001a30: 2020 3c73 7472 696e 673e 4465 7372 6970    <string>Desrip
+00001a40: 7469 6f6e 3a20 3c2f 7374 7269 6e67 3e0d  tion: </string>.
+00001a50: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
+00001a60: 7274 793e 0d0a 2020 2020 2020 203c 2f77  rty>..       </w
+00001a70: 6964 6765 743e 0d0a 2020 2020 2020 3c2f  idget>..      </
+00001a80: 6974 656d 3e0d 0a20 2020 2020 203c 6974  item>..      <it
+00001a90: 656d 2072 6f77 3d22 3422 2063 6f6c 756d  em row="4" colum
+00001aa0: 6e3d 2231 223e 0d0a 2020 2020 2020 203c  n="1">..       <
+00001ab0: 7769 6467 6574 2063 6c61 7373 3d22 5154  widget class="QT
+00001ac0: 6578 7445 6469 7422 206e 616d 653d 2264  extEdit" name="d
+00001ad0: 6573 635f 7465 223e 0d0a 2020 2020 2020  esc_te">..      
+00001ae0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00001af0: 3d22 7061 6c65 7474 6522 3e0d 0a20 2020  ="palette">..   
+00001b00: 2020 2020 2020 3c70 616c 6574 7465 3e0d        <palette>.
+00001b10: 0a20 2020 2020 2020 2020 203c 6163 7469  .          <acti
+00001b20: 7665 3e0d 0a20 2020 2020 2020 2020 2020  ve>..           
+00001b30: 3c63 6f6c 6f72 726f 6c65 2072 6f6c 653d  <colorrole role=
+00001b40: 2242 6173 6522 3e0d 0a20 2020 2020 2020  "Base">..       
+00001b50: 2020 2020 203c 6272 7573 6820 6272 7573       <brush brus
+00001b60: 6873 7479 6c65 3d22 536f 6c69 6450 6174  hstyle="SolidPat
+00001b70: 7465 726e 223e 0d0a 2020 2020 2020 2020  tern">..        
+00001b80: 2020 2020 203c 636f 6c6f 7220 616c 7068       <color alph
+00001b90: 613d 2232 3535 223e 0d0a 2020 2020 2020  a="255">..      
+00001ba0: 2020 2020 2020 2020 3c72 6564 3e32 3339          <red>239
+00001bb0: 3c2f 7265 643e 0d0a 2020 2020 2020 2020  </red>..        
+00001bc0: 2020 2020 2020 3c67 7265 656e 3e32 3339        <green>239
+00001bd0: 3c2f 6772 6565 6e3e 0d0a 2020 2020 2020  </green>..      
+00001be0: 2020 2020 2020 2020 3c62 6c75 653e 3233          <blue>23
+00001bf0: 393c 2f62 6c75 653e 0d0a 2020 2020 2020  9</blue>..      
+00001c00: 2020 2020 2020 203c 2f63 6f6c 6f72 3e0d         </color>.
+00001c10: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+00001c20: 7275 7368 3e0d 0a20 2020 2020 2020 2020  rush>..         
+00001c30: 2020 3c2f 636f 6c6f 7272 6f6c 653e 0d0a    </colorrole>..
+00001c40: 2020 2020 2020 2020 2020 3c2f 6163 7469            </acti
+00001c50: 7665 3e0d 0a20 2020 2020 2020 2020 203c  ve>..          <
+00001c60: 696e 6163 7469 7665 3e0d 0a20 2020 2020  inactive>..     
+00001c70: 2020 2020 2020 3c63 6f6c 6f72 726f 6c65        <colorrole
+00001c80: 2072 6f6c 653d 2242 6173 6522 3e0d 0a20   role="Base">.. 
+00001c90: 2020 2020 2020 2020 2020 203c 6272 7573             <brus
+00001ca0: 6820 6272 7573 6873 7479 6c65 3d22 536f  h brushstyle="So
+00001cb0: 6c69 6450 6174 7465 726e 223e 0d0a 2020  lidPattern">..  
+00001cc0: 2020 2020 2020 2020 2020 203c 636f 6c6f             <colo
+00001cd0: 7220 616c 7068 613d 2232 3535 223e 0d0a  r alpha="255">..
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
+00001cf0: 6564 3e32 3339 3c2f 7265 643e 0d0a 2020  ed>239</red>..  
+00001d00: 2020 2020 2020 2020 2020 2020 3c67 7265              <gre
+00001d10: 656e 3e32 3339 3c2f 6772 6565 6e3e 0d0a  en>239</green>..
+00001d20: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+00001d30: 6c75 653e 3233 393c 2f62 6c75 653e 0d0a  lue>239</blue>..
+00001d40: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
+00001d50: 6f6c 6f72 3e0d 0a20 2020 2020 2020 2020  olor>..         
+00001d60: 2020 203c 2f62 7275 7368 3e0d 0a20 2020     </brush>..   
+00001d70: 2020 2020 2020 2020 3c2f 636f 6c6f 7272          </colorr
+00001d80: 6f6c 653e 0d0a 2020 2020 2020 2020 2020  ole>..          
+00001d90: 3c2f 696e 6163 7469 7665 3e0d 0a20 2020  </inactive>..   
+00001da0: 2020 2020 2020 203c 6469 7361 626c 6564         <disabled
+00001db0: 3e0d 0a20 2020 2020 2020 2020 2020 3c63  >..           <c
+00001dc0: 6f6c 6f72 726f 6c65 2072 6f6c 653d 2242  olorrole role="B
+00001dd0: 6173 6522 3e0d 0a20 2020 2020 2020 2020  ase">..         
+00001de0: 2020 203c 6272 7573 6820 6272 7573 6873     <brush brushs
+00001df0: 7479 6c65 3d22 536f 6c69 6450 6174 7465  tyle="SolidPatte
+00001e00: 726e 223e 0d0a 2020 2020 2020 2020 2020  rn">..          
+00001e10: 2020 203c 636f 6c6f 7220 616c 7068 613d     <color alpha=
+00001e20: 2232 3535 223e 0d0a 2020 2020 2020 2020  "255">..        
+00001e30: 2020 2020 2020 3c72 6564 3e32 3434 3c2f        <red>244</
+00001e40: 7265 643e 0d0a 2020 2020 2020 2020 2020  red>..          
+00001e50: 2020 2020 3c67 7265 656e 3e32 3434 3c2f      <green>244</
+00001e60: 6772 6565 6e3e 0d0a 2020 2020 2020 2020  green>..        
+00001e70: 2020 2020 2020 3c62 6c75 653e 3234 343c        <blue>244<
+00001e80: 2f62 6c75 653e 0d0a 2020 2020 2020 2020  /blue>..        
+00001e90: 2020 2020 203c 2f63 6f6c 6f72 3e0d 0a20       </color>.. 
+00001ea0: 2020 2020 2020 2020 2020 203c 2f62 7275             </bru
+00001eb0: 7368 3e0d 0a20 2020 2020 2020 2020 2020  sh>..           
+00001ec0: 3c2f 636f 6c6f 7272 6f6c 653e 0d0a 2020  </colorrole>..  
+00001ed0: 2020 2020 2020 2020 3c2f 6469 7361 626c          </disabl
+00001ee0: 6564 3e0d 0a20 2020 2020 2020 2020 3c2f  ed>..         </
+00001ef0: 7061 6c65 7474 653e 0d0a 2020 2020 2020  palette>..      
+00001f00: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
+00001f10: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00001f20: 206e 616d 653d 2272 6561 644f 6e6c 7922   name="readOnly"
+00001f30: 3e0d 0a20 2020 2020 2020 2020 3c62 6f6f  >..         <boo
+00001f40: 6c3e 7472 7565 3c2f 626f 6f6c 3e0d 0a20  l>true</bool>.. 
+00001f50: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00001f60: 793e 0d0a 2020 2020 2020 203c 2f77 6964  y>..       </wid
+00001f70: 6765 743e 0d0a 2020 2020 2020 3c2f 6974  get>..      </it
+00001f80: 656d 3e0d 0a20 2020 2020 3c2f 6c61 796f  em>..     </layo
+00001f90: 7574 3e0d 0a20 2020 203c 2f77 6964 6765  ut>..    </widge
+00001fa0: 743e 0d0a 2020 203c 2f69 7465 6d3e 0d0a  t>..   </item>..
+00001fb0: 2020 203c 6974 656d 3e0d 0a20 2020 203c     <item>..    <
+00001fc0: 7769 6467 6574 2063 6c61 7373 3d22 5147  widget class="QG
+00001fd0: 726f 7570 426f 7822 206e 616d 653d 2263  roupBox" name="c
+00001fe0: 6f6e 6669 6747 4222 3e0d 0a20 2020 2020  onfigGB">..     
+00001ff0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00002000: 7469 746c 6522 3e0d 0a20 2020 2020 203c  title">..      <
+00002010: 7374 7269 6e67 3e53 6f72 7469 6e67 2061  string>Sorting a
+00002020: 6c67 6f72 6974 686d 3c2f 7374 7269 6e67  lgorithm</string
+00002030: 3e0d 0a20 2020 2020 3c2f 7072 6f70 6572  >..     </proper
+00002040: 7479 3e0d 0a20 2020 2020 3c6c 6179 6f75  ty>..     <layou
+00002050: 7420 636c 6173 733d 2251 4772 6964 4c61  t class="QGridLa
+00002060: 796f 7574 2220 6e61 6d65 3d22 6772 6964  yout" name="grid
+00002070: 4c61 796f 7574 5f32 223e 0d0a 2020 2020  Layout_2">..    
+00002080: 2020 3c69 7465 6d20 726f 773d 2230 2220    <item row="0" 
+00002090: 636f 6c75 6d6e 3d22 3022 3e0d 0a20 2020  column="0">..   
+000020a0: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
+000020b0: 733d 2251 436f 6d62 6f42 6f78 2220 6e61  s="QComboBox" na
+000020c0: 6d65 3d22 616c 676f 7269 7468 6d73 5f63  me="algorithms_c
+000020d0: 6f6d 626f 626f 7822 2f3e 0d0a 2020 2020  ombobox"/>..    
+000020e0: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
+000020f0: 3c2f 6c61 796f 7574 3e0d 0a20 2020 203c  </layout>..    <
+00002100: 2f77 6964 6765 743e 0d0a 2020 203c 2f69  /widget>..   </i
+00002110: 7465 6d3e 0d0a 2020 3c2f 6c61 796f 7574  tem>..  </layout
+00002120: 3e0d 0a20 3c2f 7769 6467 6574 3e0d 0a20  >.. </widget>.. 
+00002130: 3c72 6573 6f75 7263 6573 2f3e 0d0a 203c  <resources/>.. <
+00002140: 636f 6e6e 6563 7469 6f6e 732f 3e0d 0a3c  connections/>..<
+00002150: 2f75 693e 0d0a                           /ui>..
```

### Comparing `ViTables-3.0.2/vitables/plugins/timeseries/__init__.py` & `vitables-3.0.3/vitables/vttables/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
 #       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
 #
 #       This program is free software: you can redistribute it and/or modify
 #       it under the terms of the GNU General Public License as published by
 #       the Free Software Foundation, either version 3 of the License, or
 #       (at your option) any later version.
 #
@@ -12,8 +13,8 @@
 #       GNU General Public License for more details.
 #
 #       You should have received a copy of the GNU General Public License
 #       along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #       Author:  Vicent Mas - vmas@vitables.org
 
-__all__ = ['aboutpage', 'time_series']
+__all__ = ["buffer", "datasheet", "leaf_delegate", "leaf_model", "leaf_view", "scrollbar"]
```

### Comparing `ViTables-3.0.2/vitables/plugins/timeseries/aboutpage.py` & `vitables-3.0.3/vitables/plugins/timeseries/aboutpage.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/plugins/timeseries/time_series.py` & `vitables-3.0.3/vitables/plugins/timeseries/time_series.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/plugins/timeseries/timeformatter_page.ui` & `vitables-3.0.3/vitables/queries/query_dlg.ui`

 * *Files 26% similar despite different names*

#### Comparing `ViTables-3.0.2/vitables/plugins/timeseries/timeformatter_page.ui` & `vitables-3.0.3/vitables/queries/query_dlg.ui`

```diff
@@ -1,385 +1,351 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>TimeFormatterPage</class>
-  <widget class="QWidget" name="TimeFormatterPage">
+  <class>QueryDialog</class>
+  <widget class="QDialog" name="QueryDialog">
+    <property name="windowModality">
+      <enum>Qt::WindowModal</enum>
+    </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>400</width>
-        <height>473</height>
+        <width>435</width>
+        <height>545</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>Form</string>
+      <string>Dialog</string>
     </property>
-    <layout class="QVBoxLayout" name="verticalLayout">
+    <layout class="QVBoxLayout" name="verticalLayout_7">
       <item>
-        <widget class="QGroupBox" name="descGB">
-          <property name="title">
-            <string>Plugin description</string>
+        <layout class="QVBoxLayout" name="verticalLayout_6">
+          <property name="spacing">
+            <number>6</number>
           </property>
-          <layout class="QGridLayout" name="gridLayout">
-            <item row="0" column="0">
-              <widget class="QLabel" name="version_label">
-                <property name="text">
-                  <string>Version:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="QLineEdit" name="version_le">
-                <property name="palette">
-                  <palette>
-                    <active>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </active>
-                    <inactive>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </inactive>
-                    <disabled>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>244</red>
-                            <green>244</green>
-                            <blue>244</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </disabled>
-                  </palette>
-                </property>
-                <property name="readOnly">
-                  <bool>true</bool>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="QLabel" name="module_name_label">
-                <property name="text">
-                  <string>Module name:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="1">
-              <widget class="QLineEdit" name="module_name_le">
-                <property name="palette">
-                  <palette>
-                    <active>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </active>
-                    <inactive>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </inactive>
-                    <disabled>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>244</red>
-                            <green>244</green>
-                            <blue>244</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </disabled>
-                  </palette>
-                </property>
-                <property name="readOnly">
-                  <bool>true</bool>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="0">
-              <widget class="QLabel" name="folder_label">
-                <property name="text">
-                  <string>Folder:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="1">
-              <widget class="QLineEdit" name="folder_le">
-                <property name="palette">
-                  <palette>
-                    <active>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </active>
-                    <inactive>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </inactive>
-                    <disabled>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>244</red>
-                            <green>244</green>
-                            <blue>244</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </disabled>
-                  </palette>
-                </property>
-                <property name="readOnly">
-                  <bool>true</bool>
-                </property>
-              </widget>
-            </item>
-            <item row="3" column="0">
-              <widget class="QLabel" name="author_label">
-                <property name="text">
-                  <string>Author:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="3" column="1">
-              <widget class="QLineEdit" name="author_le">
-                <property name="palette">
-                  <palette>
-                    <active>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </active>
-                    <inactive>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </inactive>
-                    <disabled>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>244</red>
-                            <green>244</green>
-                            <blue>244</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </disabled>
-                  </palette>
-                </property>
-                <property name="readOnly">
-                  <bool>true</bool>
-                </property>
-              </widget>
-            </item>
-            <item row="4" column="0">
-              <widget class="QLabel" name="desc_label">
-                <property name="text">
-                  <string>Desription:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="4" column="1">
-              <widget class="QTextEdit" name="desc_te">
-                <property name="palette">
-                  <palette>
-                    <active>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </active>
-                    <inactive>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>239</red>
-                            <green>239</green>
-                            <blue>239</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </inactive>
-                    <disabled>
-                      <colorrole role="Base">
-                        <brush brushstyle="SolidPattern">
-                          <color alpha="255">
-                            <red>244</red>
-                            <green>244</green>
-                            <blue>244</blue>
-                          </color>
-                        </brush>
-                      </colorrole>
-                    </disabled>
-                  </palette>
-                </property>
-                <property name="readOnly">
-                  <bool>true</bool>
-                </property>
-              </widget>
-            </item>
-          </layout>
-        </widget>
-      </item>
-      <item>
-        <widget class="QGroupBox" name="configGB">
-          <property name="title">
-            <string>Configure time format</string>
+          <property name="margin">
+            <number>11</number>
           </property>
-          <layout class="QGridLayout" name="gridLayout_2">
-            <item row="0" column="0">
-              <widget class="QLabel" name="tformat_label">
-                <property name="text">
-                  <string>Time format:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0" colspan="2">
-              <layout class="QHBoxLayout" name="horizontalLayout">
-                <item>
-                  <widget class="QLabel" name="label_7">
-                    <property name="text">
-                      <string>Sample date:</string>
-                    </property>
-                  </widget>
-                </item>
+          <item>
+            <widget class="QGroupBox" name="global_opt_gb">
+              <property name="sizePolicy">
+                <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                  <horstretch>0</horstretch>
+                  <verstretch>0</verstretch>
+                </sizepolicy>
+              </property>
+              <property name="title">
+                <string>Global options</string>
+              </property>
+              <layout class="QVBoxLayout" name="verticalLayout_4">
                 <item>
-                  <spacer name="horizontalSpacer">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>81</width>
-                        <height>43</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item>
-                  <widget class="QLabel" name="today_label">
-                    <property name="text">
-                      <string>Today</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <spacer name="horizontalSpacer_2">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>117</width>
-                        <height>43</height>
-                      </size>
-                    </property>
-                  </spacer>
+                  <layout class="QVBoxLayout" name="verticalLayout_3">
+                    <property name="spacing">
+                      <number>6</number>
+                    </property>
+                    <property name="margin">
+                      <number>11</number>
+                    </property>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_2">
+                        <property name="spacing">
+                          <number>6</number>
+                        </property>
+                        <property name="margin">
+                          <number>11</number>
+                        </property>
+                        <item>
+                          <widget class="QLabel" name="label_4">
+                            <property name="text">
+                              <string>Name:</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLineEdit" name="nameLE">
+                            <property name="whatsThis">
+                              <string>&lt;qt&gt;
+        The name of the table where the query results will be added.
+        &lt;/qt&gt;</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_3">
+                        <property name="spacing">
+                          <number>6</number>
+                        </property>
+                        <property name="margin">
+                          <number>11</number>
+                        </property>
+                        <item>
+                          <widget class="QCheckBox" name="indicesCheckBox">
+                            <property name="text">
+                              <string/>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_5">
+                            <property name="text">
+                              <string>Original indices into column:</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLineEdit" name="indicesColumnLE">
+                            <property name="whatsThis">
+                              <string>&lt;qt&gt;
+        The name of the column where the indices of the selected rows
+        will be added.
+        &lt;/qt&gt;</string>
+                            </property>
+                            <property name="text">
+                              <string>Orig_idx</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                  </layout>
                 </item>
               </layout>
-            </item>
-            <item row="2" column="0" colspan="2">
-              <layout class="QHBoxLayout" name="horizontalLayout_2">
+            </widget>
+          </item>
+          <item>
+            <widget class="QGroupBox" name="condition_gb">
+              <property name="title">
+                <string>Query condition</string>
+              </property>
+              <layout class="QVBoxLayout" name="verticalLayout_2">
                 <item>
-                  <spacer name="horizontalSpacer_3">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>114</width>
-                        <height>20</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item>
-                  <widget class="QDialogButtonBox" name="buttons_box">
-                    <property name="standardButtons">
-                      <set>QDialogButtonBox::Save</set>
-                    </property>
-                  </widget>
+                  <layout class="QVBoxLayout" name="verticalLayout">
+                    <property name="spacing">
+                      <number>6</number>
+                    </property>
+                    <property name="margin">
+                      <number>11</number>
+                    </property>
+                    <item>
+                      <widget class="QLineEdit" name="queryLE">
+                        <property name="whatsThis">
+                          <string>&lt;qt&gt;
+        &lt;h3&gt;Conditions syntax&lt;/h3&gt;
+        A condition on a table is just a &lt;em&gt;string&lt;/em&gt; containing a
+        Python expression that involves &lt;em&gt;at least one column&lt;/em&gt;
+        , and maybe some constants and external variables, all combined
+        with algebraic operators or functions.
+        Beware that &lt;tt&gt;&amp;&lt;/tt&gt;, &lt;tt&gt;|&lt;/tt&gt; and &lt;tt&gt;~&lt;/tt&gt; operators
+        are used for logical comparisons. They have higher precedence
+        than logical operators so we recommend to &lt;em&gt;always use
+        parenthesis around logical operators&lt;/em&gt;.&lt;/p&gt;
+        &lt;p&gt;The following table shows some examples of conditions and
+        their equivalent Python expressions.&lt;/p&gt;
+        &lt;div align='center'&gt;&lt;table border='1'&gt;
+        &lt;tr&gt;&lt;th&gt;Condition&lt;/th&gt;&lt;th&gt;Python expression&lt;/th&gt;&lt;/tr&gt;
+        &lt;tr&gt;&lt;td&gt;&lt;code&gt;a &amp; (b == c)&lt;/code&gt;&lt;/td&gt;
+        &lt;td&gt;&lt;code&gt;a and b == c&lt;/code&gt;&lt;/td&gt;&lt;/tr&gt;
+        &lt;tr&gt;&lt;td&gt;&lt;code&gt;(0 &amp;lt; x) &amp; (x &amp;lt; 1)&lt;/code&gt;&lt;/td&gt;
+        &lt;td&gt;&lt;code&gt;0 &amp;lt; x &amp;lt; 1&lt;/code&gt;&lt;/td&gt;&lt;/tr&gt;
+        &lt;tr&gt;&lt;td&gt;&lt;code&gt;a + b  &amp;gt; c&lt;/code&gt;&lt;/td&gt;
+        &lt;td&gt;&lt;code&gt;a + b  &amp;gt; c&lt;/code&gt;&lt;/td&gt;&lt;/tr&gt;
+        &lt;tr&gt;&lt;td&gt;&lt;code&gt;where(a &gt; b, 3, 4)&lt;/code&gt;&lt;/td&gt;
+        &lt;td&gt;&lt;/td&gt;&lt;/tr&gt;
+        &lt;/table&gt;&lt;/div&gt;
+        &lt;p&gt;You can find detailed information about conditions in the
+        Appendix B of the PyTables users guide.&lt;/p&gt;
+        &lt;/qt&gt;</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout">
+                        <property name="spacing">
+                          <number>6</number>
+                        </property>
+                        <property name="margin">
+                          <number>11</number>
+                        </property>
+                        <item>
+                          <spacer name="horizontalSpacer_2">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>40</width>
+                                <height>20</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="columnsComboBox">
+                            <property name="whatsThis">
+                              <string>&lt;qt&gt;
+        The names of the searchable columns. They must
+        fulfill the following requirements:
+        &lt;ul&gt;&lt;li&gt;must be not nested&lt;/li&gt;
+        &lt;li&gt;must have a scalar data type&lt;/li&gt;
+        &lt;li&gt;their data type cannot be &lt;code&gt;complex&lt;/code&gt;&lt;/li&gt;&lt;/ul&gt;
+        Columns whose names contains blanks are automatically mapped
+        to variables whose names contain no blanks. For querying
+        those columns the mapped variables will be used.
+        &lt;/qt&gt;</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="operatorsComboBox">
+                            <property name="whatsThis">
+                              <string>&lt;qt&gt;
+        The operators that can be used in a given condition. Operators
+        can be logical, comparison and arithmetic.&lt;br&gt;Not all operators
+        are available for every data type.
+        &lt;/qt&gt;</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="functionsComboBox">
+                            <property name="whatsThis">
+                              <string>&lt;qt&gt;
+        The set of functions that can appear in a condition.
+        It includes functions for doing selections, trigonometric
+        functions and functions on complex numbers. For ease
+        of use, arguments are automatically included when a
+        function is inserted. The arguments meaning is:
+        &lt;ul&gt;&lt;li&gt;N: number&lt;/li&gt;&lt;li&gt;B: boolean&lt;/li&gt;
+        &lt;li&gt;F: float&lt;/li&gt;&lt;li&gt;C: complex&lt;/li&gt;&lt;/ul&gt;
+        &lt;/qt&gt;</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <spacer name="horizontalSpacer">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>40</width>
+                                <height>20</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                      </layout>
+                    </item>
+                  </layout>
                 </item>
+              </layout>
+            </widget>
+          </item>
+          <item>
+            <widget class="QGroupBox" name="rows_range_gb">
+              <property name="whatsThis">
+                <string>The range of rows included in the query.</string>
+              </property>
+              <property name="title">
+                <string>Range of rows</string>
+              </property>
+              <layout class="QVBoxLayout" name="verticalLayout_5">
                 <item>
-                  <spacer name="horizontalSpacer_4">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>117</width>
-                        <height>20</height>
-                      </size>
-                    </property>
-                  </spacer>
+                  <layout class="QGridLayout" name="range_layout">
+                    <property name="margin">
+                      <number>11</number>
+                    </property>
+                    <property name="spacing">
+                      <number>6</number>
+                    </property>
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label">
+                        <property name="text">
+                          <string>Start:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QLineEdit" name="rstartLE">
+                        <property name="text">
+                          <string comment="A range selector label">1</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QLabel" name="label_2">
+                        <property name="text">
+                          <string>Stop:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="1">
+                      <widget class="QLineEdit" name="rstopLE"/>
+                    </item>
+                    <item row="1" column="2">
+                      <spacer name="horizontalSpacer_3">
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                        <property name="sizeHint" stdset="0">
+                          <size>
+                            <width>40</width>
+                            <height>20</height>
+                          </size>
+                        </property>
+                      </spacer>
+                    </item>
+                    <item row="2" column="0">
+                      <widget class="QLabel" name="label_3">
+                        <property name="text">
+                          <string>Step:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="1">
+                      <widget class="QLineEdit" name="rstep">
+                        <property name="text">
+                          <string comment="A range selector label">1</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
                 </item>
               </layout>
-            </item>
-            <item row="0" column="1">
-              <widget class="QLineEdit" name="tformat_editor"/>
-            </item>
-          </layout>
-        </widget>
+            </widget>
+          </item>
+          <item>
+            <widget class="QDialogButtonBox" name="buttonBox">
+              <property name="standardButtons">
+                <set>QDialogButtonBox::Cancel|QDialogButtonBox::Help|QDialogButtonBox::Ok</set>
+              </property>
+              <property name="centerButtons">
+                <bool>true</bool>
+              </property>
+            </widget>
+          </item>
+        </layout>
       </item>
     </layout>
   </widget>
   <resources/>
-  <connections/>
+  <connections>
+    <connection>
+      <sender>buttonBox</sender>
+      <signal>rejected()</signal>
+      <receiver>QueryDialog</receiver>
+      <slot>reject()</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>217</x>
+          <y>517</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>217</x>
+          <y>272</y>
+        </hint>
+      </hints>
+    </connection>
+  </connections>
 </ui>
```

### Comparing `ViTables-3.0.2/vitables/preferences/__init__.py` & `vitables-3.0.3/vitables/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/preferences/cfgexception.py` & `vitables-3.0.3/vitables/preferences/cfgexception.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/preferences/pluginsloader.py` & `vitables-3.0.3/vitables/preferences/pluginsloader.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/preferences/preferences.py` & `vitables-3.0.3/vitables/preferences/preferences.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/preferences/settings_dlg.ui` & `vitables-3.0.3/vitables/preferences/settings_dlg.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (335)*

 * *Files 18% similar despite different names*

```diff
@@ -1,890 +1,912 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
-00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
-00000040: 733e 5365 7474 696e 6773 4469 616c 6f67  s>SettingsDialog
-00000050: 3c2f 636c 6173 733e 0a20 3c77 6964 6765  </class>. <widge
-00000060: 7420 636c 6173 733d 2251 4469 616c 6f67  t class="QDialog
-00000070: 2220 6e61 6d65 3d22 5365 7474 696e 6773  " name="Settings
-00000080: 4469 616c 6f67 223e 0a20 203c 7072 6f70  Dialog">.  <prop
-00000090: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-000000a0: 7472 7922 3e0a 2020 203c 7265 6374 3e0a  try">.   <rect>.
-000000b0: 2020 2020 3c78 3e30 3c2f 783e 0a20 2020      <x>0</x>.   
-000000c0: 203c 793e 303c 2f79 3e0a 2020 2020 3c77   <y>0</y>.    <w
-000000d0: 6964 7468 3e35 3432 3c2f 7769 6474 683e  idth>542</width>
-000000e0: 0a20 2020 203c 6865 6967 6874 3e34 3139  .    <height>419
-000000f0: 3c2f 6865 6967 6874 3e0a 2020 203c 2f72  </height>.   </r
-00000100: 6563 743e 0a20 203c 2f70 726f 7065 7274  ect>.  </propert
-00000110: 793e 0a20 203c 7072 6f70 6572 7479 206e  y>.  <property n
-00000120: 616d 653d 2277 696e 646f 7754 6974 6c65  ame="windowTitle
-00000130: 223e 0a20 2020 3c73 7472 696e 673e 5669  ">.   <string>Vi
-00000140: 5461 626c 6573 2073 6574 7469 6e67 733c  Tables settings<
-00000150: 2f73 7472 696e 673e 0a20 203c 2f70 726f  /string>.  </pro
-00000160: 7065 7274 793e 0a20 203c 6c61 796f 7574  perty>.  <layout
-00000170: 2063 6c61 7373 3d22 5156 426f 784c 6179   class="QVBoxLay
-00000180: 6f75 7422 206e 616d 653d 2276 6572 7469  out" name="verti
-00000190: 6361 6c4c 6179 6f75 745f 3222 3e0a 2020  calLayout_2">.  
-000001a0: 203c 6974 656d 3e0a 2020 2020 3c6c 6179   <item>.    <lay
-000001b0: 6f75 7420 636c 6173 733d 2251 4842 6f78  out class="QHBox
-000001c0: 4c61 796f 7574 2220 6e61 6d65 3d22 686f  Layout" name="ho
-000001d0: 7269 7a6f 6e74 616c 4c61 796f 7574 223e  rizontalLayout">
-000001e0: 0a20 2020 2020 3c69 7465 6d3e 0a20 2020  .     <item>.   
-000001f0: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00000200: 3d22 5154 7265 6556 6965 7722 206e 616d  ="QTreeView" nam
-00000210: 653d 2270 6167 6553 656c 6563 746f 7222  e="pageSelector"
-00000220: 3e0a 2020 2020 2020 203c 7072 6f70 6572  >.       <proper
-00000230: 7479 206e 616d 653d 2273 697a 6550 6f6c  ty name="sizePol
-00000240: 6963 7922 3e0a 2020 2020 2020 2020 3c73  icy">.        <s
-00000250: 697a 6570 6f6c 6963 7920 6873 697a 6574  izepolicy hsizet
-00000260: 7970 653d 224d 696e 696d 756d 4578 7061  ype="MinimumExpa
-00000270: 6e64 696e 6722 2076 7369 7a65 7479 7065  nding" vsizetype
-00000280: 3d22 4578 7061 6e64 696e 6722 3e0a 2020  ="Expanding">.  
-00000290: 2020 2020 2020 203c 686f 7273 7472 6574         <horstret
-000002a0: 6368 3e30 3c2f 686f 7273 7472 6574 6368  ch>0</horstretch
-000002b0: 3e0a 2020 2020 2020 2020 203c 7665 7273  >.         <vers
-000002c0: 7472 6574 6368 3e30 3c2f 7665 7273 7472  tretch>0</verstr
-000002d0: 6574 6368 3e0a 2020 2020 2020 2020 3c2f  etch>.        </
-000002e0: 7369 7a65 706f 6c69 6379 3e0a 2020 2020  sizepolicy>.    
-000002f0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
-00000300: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00000310: 6e61 6d65 3d22 6d69 6e69 6d75 6d53 697a  name="minimumSiz
-00000320: 6522 3e0a 2020 2020 2020 2020 3c73 697a  e">.        <siz
-00000330: 653e 0a20 2020 2020 2020 2020 3c77 6964  e>.         <wid
-00000340: 7468 3e31 3631 3c2f 7769 6474 683e 0a20  th>161</width>. 
-00000350: 2020 2020 2020 2020 3c68 6569 6768 743e          <height>
-00000360: 3338 303c 2f68 6569 6768 743e 0a20 2020  380</height>.   
-00000370: 2020 2020 203c 2f73 697a 653e 0a20 2020       </size>.   
-00000380: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00000390: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000003a0: 206e 616d 653d 226d 6178 696d 756d 5369   name="maximumSi
-000003b0: 7a65 223e 0a20 2020 2020 2020 203c 7369  ze">.        <si
-000003c0: 7a65 3e0a 2020 2020 2020 2020 203c 7769  ze>.         <wi
-000003d0: 6474 683e 3230 303c 2f77 6964 7468 3e0a  dth>200</width>.
-000003e0: 2020 2020 2020 2020 203c 6865 6967 6874           <height
-000003f0: 3e31 3637 3737 3231 353c 2f68 6569 6768  >16777215</heigh
-00000400: 743e 0a20 2020 2020 2020 203c 2f73 697a  t>.        </siz
-00000410: 653e 0a20 2020 2020 2020 3c2f 7072 6f70  e>.       </prop
-00000420: 6572 7479 3e0a 2020 2020 2020 203c 7072  erty>.       <pr
-00000430: 6f70 6572 7479 206e 616d 653d 2277 6861  operty name="wha
-00000440: 7473 5468 6973 223e 0a20 2020 2020 2020  tsThis">.       
-00000450: 203c 7374 7269 6e67 3e43 6c69 636b 2061   <string>Click a
-00000460: 6e20 6974 656d 2069 6e20 7468 6973 2074  n item in this t
-00000470: 7265 6520 746f 2073 656c 6563 7420 7468  ree to select th
-00000480: 6520 7365 7474 696e 6773 2079 6f75 2077  e settings you w
-00000490: 616e 7420 746f 2063 6861 6e67 652e 2042  ant to change. B
-000004a0: 6577 6172 6520 7468 6174 2074 6865 206c  eware that the l
-000004b0: 6973 7465 6420 706c 7567 696e 7320 6172  isted plugins ar
-000004c0: 6520 2a6c 6f61 6465 642a 2070 6c75 6769  e *loaded* plugi
-000004d0: 6e73 2028 692e 652e 2074 6865 2061 7265  ns (i.e. the are
-000004e0: 2077 6f72 6b69 6e67 2069 6e20 7468 6520   working in the 
-000004f0: 6375 7272 656e 7420 5669 5461 626c 6573  current ViTables
-00000500: 2073 6573 7369 6f6e 2920 6e6f 7420 6a75   session) not ju
-00000510: 7374 2065 6e61 626c 6564 2070 6c75 6769  st enabled plugi
-00000520: 6e73 2e3c 2f73 7472 696e 673e 0a20 2020  ns.</string>.   
-00000530: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00000540: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000550: 206e 616d 653d 2265 6469 7454 7269 6767   name="editTrigg
-00000560: 6572 7322 3e0a 2020 2020 2020 2020 3c73  ers">.        <s
-00000570: 6574 3e51 4162 7374 7261 6374 4974 656d  et>QAbstractItem
-00000580: 5669 6577 3a3a 4e6f 4564 6974 5472 6967  View::NoEditTrig
-00000590: 6765 7273 3c2f 7365 743e 0a20 2020 2020  gers</set>.     
-000005a0: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
-000005b0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-000005c0: 616d 653d 2269 636f 6e53 697a 6522 3e0a  ame="iconSize">.
-000005d0: 2020 2020 2020 2020 3c73 697a 653e 0a20          <size>. 
-000005e0: 2020 2020 2020 2020 3c77 6964 7468 3e32          <width>2
-000005f0: 323c 2f77 6964 7468 3e0a 2020 2020 2020  2</width>.      
-00000600: 2020 203c 6865 6967 6874 3e32 323c 2f68     <height>22</h
-00000610: 6569 6768 743e 0a20 2020 2020 2020 203c  eight>.        <
-00000620: 2f73 697a 653e 0a20 2020 2020 2020 3c2f  /size>.       </
-00000630: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00000640: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
-00000650: 3d22 6865 6164 6572 5669 7369 626c 6522  ="headerVisible"
-00000660: 3e0a 2020 2020 2020 2020 3c62 6f6f 6c3e  >.        <bool>
-00000670: 6661 6c73 653c 2f62 6f6f 6c3e 0a20 2020  false</bool>.   
-00000680: 2020 2020 3c2f 6174 7472 6962 7574 653e      </attribute>
-00000690: 0a20 2020 2020 2020 3c61 7474 7269 6275  .       <attribu
-000006a0: 7465 206e 616d 653d 2268 6561 6465 7244  te name="headerD
-000006b0: 6566 6175 6c74 5365 6374 696f 6e53 697a  efaultSectionSiz
-000006c0: 6522 3e0a 2020 2020 2020 2020 3c6e 756d  e">.        <num
-000006d0: 6265 723e 3130 303c 2f6e 756d 6265 723e  ber>100</number>
-000006e0: 0a20 2020 2020 2020 3c2f 6174 7472 6962  .       </attrib
-000006f0: 7574 653e 0a20 2020 2020 2020 3c61 7474  ute>.       <att
-00000700: 7269 6275 7465 206e 616d 653d 2268 6561  ribute name="hea
-00000710: 6465 7244 6566 6175 6c74 5365 6374 696f  derDefaultSectio
-00000720: 6e53 697a 6522 3e0a 2020 2020 2020 2020  nSize">.        
-00000730: 3c6e 756d 6265 723e 3130 303c 2f6e 756d  <number>100</num
-00000740: 6265 723e 0a20 2020 2020 2020 3c2f 6174  ber>.       </at
-00000750: 7472 6962 7574 653e 0a20 2020 2020 2020  tribute>.       
-00000760: 3c61 7474 7269 6275 7465 206e 616d 653d  <attribute name=
-00000770: 2268 6561 6465 7256 6973 6962 6c65 223e  "headerVisible">
-00000780: 0a20 2020 2020 2020 203c 626f 6f6c 3e66  .        <bool>f
-00000790: 616c 7365 3c2f 626f 6f6c 3e0a 2020 2020  alse</bool>.    
-000007a0: 2020 203c 2f61 7474 7269 6275 7465 3e0a     </attribute>.
-000007b0: 2020 2020 2020 3c2f 7769 6467 6574 3e0a        </widget>.
-000007c0: 2020 2020 203c 2f69 7465 6d3e 0a20 2020       </item>.   
-000007d0: 2020 3c69 7465 6d3e 0a20 2020 2020 203c    <item>.      <
-000007e0: 7769 6467 6574 2063 6c61 7373 3d22 5153  widget class="QS
-000007f0: 7461 636b 6564 5769 6467 6574 2220 6e61  tackedWidget" na
-00000800: 6d65 3d22 7374 6163 6b65 6450 6167 6573  me="stackedPages
-00000810: 223e 0a20 2020 2020 2020 3c70 726f 7065  ">.       <prope
-00000820: 7274 7920 6e61 6d65 3d22 7369 7a65 506f  rty name="sizePo
-00000830: 6c69 6379 223e 0a20 2020 2020 2020 203c  licy">.        <
-00000840: 7369 7a65 706f 6c69 6379 2068 7369 7a65  sizepolicy hsize
-00000850: 7479 7065 3d22 5072 6566 6572 7265 6422  type="Preferred"
-00000860: 2076 7369 7a65 7479 7065 3d22 5072 6566   vsizetype="Pref
-00000870: 6572 7265 6422 3e0a 2020 2020 2020 2020  erred">.        
-00000880: 203c 686f 7273 7472 6574 6368 3e30 3c2f   <horstretch>0</
-00000890: 686f 7273 7472 6574 6368 3e0a 2020 2020  horstretch>.    
-000008a0: 2020 2020 203c 7665 7273 7472 6574 6368       <verstretch
-000008b0: 3e30 3c2f 7665 7273 7472 6574 6368 3e0a  >0</verstretch>.
-000008c0: 2020 2020 2020 2020 3c2f 7369 7a65 706f          </sizepo
-000008d0: 6c69 6379 3e0a 2020 2020 2020 203c 2f70  licy>.       </p
-000008e0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-000008f0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000900: 6375 7272 656e 7449 6e64 6578 223e 0a20  currentIndex">. 
-00000910: 2020 2020 2020 203c 6e75 6d62 6572 3e32         <number>2
-00000920: 3c2f 6e75 6d62 6572 3e0a 2020 2020 2020  </number>.      
-00000930: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-00000940: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
-00000950: 733d 2251 5769 6467 6574 2220 6e61 6d65  s="QWidget" name
-00000960: 3d22 7374 6172 7475 7050 6167 6522 3e0a  ="startupPage">.
-00000970: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00000980: 7920 6e61 6d65 3d22 7369 7a65 506f 6c69  y name="sizePoli
-00000990: 6379 223e 0a20 2020 2020 2020 2020 3c73  cy">.         <s
-000009a0: 697a 6570 6f6c 6963 7920 6873 697a 6574  izepolicy hsizet
-000009b0: 7970 653d 2245 7870 616e 6469 6e67 2220  ype="Expanding" 
-000009c0: 7673 697a 6574 7970 653d 2250 7265 6665  vsizetype="Prefe
-000009d0: 7272 6564 223e 0a20 2020 2020 2020 2020  rred">.         
-000009e0: 203c 686f 7273 7472 6574 6368 3e30 3c2f   <horstretch>0</
-000009f0: 686f 7273 7472 6574 6368 3e0a 2020 2020  horstretch>.    
-00000a00: 2020 2020 2020 3c76 6572 7374 7265 7463        <verstretc
-00000a10: 683e 303c 2f76 6572 7374 7265 7463 683e  h>0</verstretch>
-00000a20: 0a20 2020 2020 2020 2020 3c2f 7369 7a65  .         </size
-00000a30: 706f 6c69 6379 3e0a 2020 2020 2020 2020  policy>.        
-00000a40: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00000a50: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00000a60: 6d65 3d22 7768 6174 7354 6869 7322 3e0a  me="whatsThis">.
-00000a70: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00000a80: 3e43 6f6e 6669 6775 7265 2074 6865 2073  >Configure the s
-00000a90: 7461 7274 7570 2062 6568 6176 696f 7220  tartup behavior 
-00000aa0: 6f66 2056 6954 6162 6c65 732e 3c2f 7374  of ViTables.</st
-00000ab0: 7269 6e67 3e0a 2020 2020 2020 2020 3c2f  ring>.        </
-00000ac0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00000ad0: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-00000ae0: 2251 4772 6f75 7042 6f78 2220 6e61 6d65  "QGroupBox" name
-00000af0: 3d22 7374 6172 7475 7047 4222 3e0a 2020  ="startupGB">.  
-00000b00: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000b10: 206e 616d 653d 2267 656f 6d65 7472 7922   name="geometry"
-00000b20: 3e0a 2020 2020 2020 2020 2020 3c72 6563  >.          <rec
-00000b30: 743e 0a20 2020 2020 2020 2020 2020 3c78  t>.           <x
-00000b40: 3e34 3c2f 783e 0a20 2020 2020 2020 2020  >4</x>.         
-00000b50: 2020 3c79 3e34 3c2f 793e 0a20 2020 2020    <y>4</y>.     
-00000b60: 2020 2020 2020 3c77 6964 7468 3e33 3531        <width>351
-00000b70: 3c2f 7769 6474 683e 0a20 2020 2020 2020  </width>.       
-00000b80: 2020 2020 3c68 6569 6768 743e 3335 313c      <height>351<
-00000b90: 2f68 6569 6768 743e 0a20 2020 2020 2020  /height>.       
-00000ba0: 2020 203c 2f72 6563 743e 0a20 2020 2020     </rect>.     
-00000bb0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00000bc0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00000bd0: 7479 206e 616d 653d 2273 697a 6550 6f6c  ty name="sizePol
-00000be0: 6963 7922 3e0a 2020 2020 2020 2020 2020  icy">.          
-00000bf0: 3c73 697a 6570 6f6c 6963 7920 6873 697a  <sizepolicy hsiz
-00000c00: 6574 7970 653d 224d 6178 696d 756d 2220  etype="Maximum" 
-00000c10: 7673 697a 6574 7970 653d 2250 7265 6665  vsizetype="Prefe
-00000c20: 7272 6564 223e 0a20 2020 2020 2020 2020  rred">.         
-00000c30: 2020 3c68 6f72 7374 7265 7463 683e 303c    <horstretch>0<
-00000c40: 2f68 6f72 7374 7265 7463 683e 0a20 2020  /horstretch>.   
-00000c50: 2020 2020 2020 2020 3c76 6572 7374 7265          <verstre
-00000c60: 7463 683e 303c 2f76 6572 7374 7265 7463  tch>0</verstretc
-00000c70: 683e 0a20 2020 2020 2020 2020 203c 2f73  h>.          </s
-00000c80: 697a 6570 6f6c 6963 793e 0a20 2020 2020  izepolicy>.     
-00000c90: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00000ca0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00000cb0: 7479 206e 616d 653d 2277 6861 7473 5468  ty name="whatsTh
-00000cc0: 6973 223e 0a20 2020 2020 2020 2020 203c  is">.          <
-00000cd0: 7374 7269 6e67 2f3e 0a20 2020 2020 2020  string/>.       
-00000ce0: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
-00000cf0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000d00: 206e 616d 653d 2274 6974 6c65 223e 0a20   name="title">. 
-00000d10: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00000d20: 2063 6f6d 6d65 6e74 3d22 5468 6520 6e61   comment="The na
-00000d30: 6d65 206f 6620 7468 6520 6772 6f75 7062  me of the groupb
-00000d40: 6f78 2077 6865 7265 2073 7461 7274 7570  ox where startup
-00000d50: 2069 7320 636f 6e66 6967 7572 6564 223e   is configured">
-00000d60: 5374 6172 7475 703c 2f73 7472 696e 673e  Startup</string>
-00000d70: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00000d80: 6572 7479 3e0a 2020 2020 2020 2020 203c  erty>.         <
-00000d90: 6c61 796f 7574 2063 6c61 7373 3d22 5156  layout class="QV
-00000da0: 426f 784c 6179 6f75 7422 206e 616d 653d  BoxLayout" name=
-00000db0: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
-00000dc0: 3322 3e0a 2020 2020 2020 2020 2020 3c69  3">.          <i
-00000dd0: 7465 6d3e 0a20 2020 2020 2020 2020 2020  tem>.           
-00000de0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-00000df0: 4368 6563 6b42 6f78 2220 6e61 6d65 3d22  CheckBox" name="
-00000e00: 7265 7374 6f72 6543 4222 3e0a 2020 2020  restoreCB">.    
-00000e10: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00000e20: 7920 6e61 6d65 3d22 7768 6174 7354 6869  y name="whatsThi
-00000e30: 7322 3e0a 2020 2020 2020 2020 2020 2020  s">.            
-00000e40: 203c 7374 7269 6e67 3e49 6620 6368 6563   <string>If chec
-00000e50: 6b65 642c 2074 6865 206c 6173 7420 776f  ked, the last wo
-00000e60: 726b 696e 6720 7365 7373 696f 6e20 2d69  rking session -i
-00000e70: 2e65 2e20 6f70 656e 2066 696c 6573 2061  .e. open files a
-00000e80: 6e64 2076 6965 7773 2d20 7769 6c6c 2062  nd views- will b
-00000e90: 6520 7265 7374 6f72 6564 2e20 4966 206e  e restored. If n
-00000ea0: 6f74 2c20 5669 5461 626c 6573 2077 696c  ot, ViTables wil
-00000eb0: 6c20 7374 6172 7420 7769 7468 2061 6e20  l start with an 
-00000ec0: 656d 7074 7920 7365 7373 696f 6e2e 3c2f  empty session.</
-00000ed0: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
-00000ee0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00000ef0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00000f00: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
-00000f10: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000f20: 3c73 7472 696e 6720 636f 6d6d 656e 743d  <string comment=
-00000f30: 224c 6162 656c 206f 6620 7468 6520 7265  "Label of the re
-00000f40: 7374 6f72 6520 6c61 7374 2073 6573 7369  store last sessi
-00000f50: 6f6e 2063 6865 636b 2062 7574 746f 6e22  on check button"
-00000f60: 3e52 6573 746f 7265 206c 6173 7420 7365  >Restore last se
-00000f70: 7373 696f 6e3c 2f73 7472 696e 673e 0a20  ssion</string>. 
-00000f80: 2020 2020 2020 2020 2020 203c 2f70 726f             </pro
-00000f90: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00000fa0: 2020 3c2f 7769 6467 6574 3e0a 2020 2020    </widget>.    
-00000fb0: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
-00000fc0: 2020 2020 2020 2020 3c69 7465 6d3e 0a20          <item>. 
-00000fd0: 2020 2020 2020 2020 2020 3c77 6964 6765            <widge
-00000fe0: 7420 636c 6173 733d 2251 4368 6563 6b42  t class="QCheckB
-00000ff0: 6f78 2220 6e61 6d65 3d22 6c61 7374 4469  ox" name="lastDi
-00001000: 7243 4222 3e0a 2020 2020 2020 2020 2020  rCB">.          
-00001010: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00001020: 3d22 7768 6174 7354 6869 7322 3e0a 2020  ="whatsThis">.  
-00001030: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
-00001040: 6e67 3e54 6865 2077 6f72 6b69 6e67 2064  ng>The working d
-00001050: 6972 6563 746f 7279 2075 7365 6420 7768  irectory used wh
-00001060: 656e 206f 7065 6e69 6e67 2074 6865 2076  en opening the v
-00001070: 6572 7920 6669 7273 7420 6669 6c65 2e20  ery first file. 
-00001080: 4974 2064 6566 6175 6c74 7320 746f 2074  It defaults to t
-00001090: 6865 2063 7572 7265 6e74 2064 6972 6563  he current direc
-000010a0: 746f 7279 2069 6620 5669 5461 626c 6573  tory if ViTables
-000010b0: 2068 6173 2062 6565 6e20 6c61 756e 6368   has been launch
-000010c0: 6564 2066 726f 6d20 7468 6520 636f 6d6d  ed from the comm
-000010d0: 616e 6420 6c69 6e65 206f 7220 746f 2074  and line or to t
-000010e0: 6865 2075 7365 7227 7320 686f 6d65 2064  he user's home d
-000010f0: 6972 6563 746f 7279 2069 6620 5669 5461  irectory if ViTa
-00001100: 626c 6573 2073 7461 7274 6564 2066 726f  bles started fro
-00001110: 6d20 6120 6d65 6e75 206f 7220 6120 6465  m a menu or a de
-00001120: 736b 746f 7020 6963 6f6e 2e20 4966 2074  sktop icon. If t
-00001130: 6865 2063 6865 636b 626f 7820 6973 2063  he checkbox is c
-00001140: 6865 636b 6564 2074 6865 6e20 7468 6520  hecked then the 
-00001150: 6c61 7374 2065 6e74 6572 6564 2064 6972  last entered dir
-00001160: 6563 746f 7279 2077 696c 6c20 6265 2075  ectory will be u
-00001170: 7365 642e 3c2f 7374 7269 6e67 3e0a 2020  sed.</string>.  
-00001180: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
-00001190: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-000011a0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-000011b0: 3d22 7465 7874 223e 0a20 2020 2020 2020  ="text">.       
-000011c0: 2020 2020 2020 3c73 7472 696e 6720 636f        <string co
-000011d0: 6d6d 656e 743d 224c 6162 656c 206f 6620  mment="Label of 
-000011e0: 7468 6520 7374 6172 7475 7020 696e 2074  the startup in t
-000011f0: 6865 206c 6173 7420 6f70 656e 2064 6972  he last open dir
-00001200: 6563 746f 7279 2063 6865 636b 2062 6f78  ectory check box
-00001210: 223e 5374 6172 7420 696e 206c 6173 7420  ">Start in last 
-00001220: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
-00001230: 793c 2f73 7472 696e 673e 0a20 2020 2020  y</string>.     
-00001240: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00001250: 793e 0a20 2020 2020 2020 2020 2020 3c2f  y>.           </
-00001260: 7769 6467 6574 3e0a 2020 2020 2020 2020  widget>.        
-00001270: 2020 3c2f 6974 656d 3e0a 2020 2020 2020    </item>.      
-00001280: 2020 203c 2f6c 6179 6f75 743e 0a20 2020     </layout>.   
-00001290: 2020 2020 203c 2f77 6964 6765 743e 0a20       </widget>. 
-000012a0: 2020 2020 2020 3c2f 7769 6467 6574 3e0a        </widget>.
-000012b0: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-000012c0: 6c61 7373 3d22 5157 6964 6765 7422 206e  lass="QWidget" n
-000012d0: 616d 653d 2273 7479 6c65 5061 6765 223e  ame="stylePage">
-000012e0: 0a20 2020 2020 2020 203c 7072 6f70 6572  .        <proper
-000012f0: 7479 206e 616d 653d 2273 697a 6550 6f6c  ty name="sizePol
-00001300: 6963 7922 3e0a 2020 2020 2020 2020 203c  icy">.         <
-00001310: 7369 7a65 706f 6c69 6379 2068 7369 7a65  sizepolicy hsize
-00001320: 7479 7065 3d22 4578 7061 6e64 696e 6722  type="Expanding"
-00001330: 2076 7369 7a65 7479 7065 3d22 5072 6566   vsizetype="Pref
-00001340: 6572 7265 6422 3e0a 2020 2020 2020 2020  erred">.        
-00001350: 2020 3c68 6f72 7374 7265 7463 683e 303c    <horstretch>0<
-00001360: 2f68 6f72 7374 7265 7463 683e 0a20 2020  /horstretch>.   
-00001370: 2020 2020 2020 203c 7665 7273 7472 6574         <verstret
-00001380: 6368 3e30 3c2f 7665 7273 7472 6574 6368  ch>0</verstretch
-00001390: 3e0a 2020 2020 2020 2020 203c 2f73 697a  >.         </siz
-000013a0: 6570 6f6c 6963 793e 0a20 2020 2020 2020  epolicy>.       
-000013b0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-000013c0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-000013d0: 616d 653d 2277 6861 7473 5468 6973 223e  ame="whatsThis">
-000013e0: 0a20 2020 2020 2020 2020 3c73 7472 696e  .         <strin
-000013f0: 673e 436f 6e66 6967 7572 6520 7468 6520  g>Configure the 
-00001400: 6c6f 6f6b 2061 6e64 2066 6565 6c20 6f66  look and feel of
-00001410: 2056 6954 6162 6c65 732e 3c2f 7374 7269   ViTables.</stri
-00001420: 6e67 3e0a 2020 2020 2020 2020 3c2f 7072  ng>.        </pr
-00001430: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00001440: 3c6c 6179 6f75 7420 636c 6173 733d 2251  <layout class="Q
-00001450: 5642 6f78 4c61 796f 7574 2220 6e61 6d65  VBoxLayout" name
-00001460: 3d22 7665 7274 6963 616c 4c61 796f 7574  ="verticalLayout
-00001470: 223e 0a20 2020 2020 2020 2020 3c69 7465  ">.         <ite
-00001480: 6d3e 0a20 2020 2020 2020 2020 203c 7769  m>.          <wi
-00001490: 6467 6574 2063 6c61 7373 3d22 5147 726f  dget class="QGro
-000014a0: 7570 426f 7822 206e 616d 653d 226c 6f67  upBox" name="log
-000014b0: 6765 7247 4222 3e0a 2020 2020 2020 2020  gerGB">.        
-000014c0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000014d0: 653d 2277 6861 7473 5468 6973 223e 0a20  e="whatsThis">. 
-000014e0: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
-000014f0: 6e67 3e43 7573 746f 6d69 7365 2066 6f6e  ng>Customise fon
-00001500: 7420 616e 6420 636f 6c6f 7273 206f 6620  t and colors of 
-00001510: 7468 6520 4c6f 6767 6572 2e3c 2f73 7472  the Logger.</str
-00001520: 696e 673e 0a20 2020 2020 2020 2020 2020  ing>.           
-00001530: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00001540: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001550: 206e 616d 653d 2274 6974 6c65 223e 0a20   name="title">. 
-00001560: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
-00001570: 6e67 2063 6f6d 6d65 6e74 3d22 5468 6520  ng comment="The 
-00001580: 7469 746c 6520 6f66 2074 6865 206c 6f67  title of the log
-00001590: 6765 7220 6772 6f75 626f 7822 3e4c 6f67  ger groubox">Log
-000015a0: 6765 723c 2f73 7472 696e 673e 0a20 2020  ger</string>.   
-000015b0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-000015c0: 7479 3e0a 2020 2020 2020 2020 2020 203c  ty>.           <
-000015d0: 6c61 796f 7574 2063 6c61 7373 3d22 5147  layout class="QG
-000015e0: 7269 644c 6179 6f75 7422 206e 616d 653d  ridLayout" name=
-000015f0: 2267 7269 644c 6179 6f75 7422 3e0a 2020  "gridLayout">.  
-00001600: 2020 2020 2020 2020 2020 3c69 7465 6d20            <item 
-00001610: 726f 773d 2230 2220 636f 6c75 6d6e 3d22  row="0" column="
-00001620: 3122 2072 6f77 7370 616e 3d22 3722 3e0a  1" rowspan="7">.
-00001630: 2020 2020 2020 2020 2020 2020 203c 7769               <wi
-00001640: 6467 6574 2063 6c61 7373 3d22 5154 6578  dget class="QTex
-00001650: 7445 6469 7422 206e 616d 653d 2273 616d  tEdit" name="sam
-00001660: 706c 6554 4522 3e0a 2020 2020 2020 2020  pleTE">.        
-00001670: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00001680: 6e61 6d65 3d22 6163 6365 7074 4472 6f70  name="acceptDrop
-00001690: 7322 3e0a 2020 2020 2020 2020 2020 2020  s">.            
-000016a0: 2020 203c 626f 6f6c 3e66 616c 7365 3c2f     <bool>false</
-000016b0: 626f 6f6c 3e0a 2020 2020 2020 2020 2020  bool>.          
-000016c0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-000016d0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000016e0: 726f 7065 7274 7920 6e61 6d65 3d22 7768  roperty name="wh
-000016f0: 6174 7354 6869 7322 3e0a 2020 2020 2020  atsThis">.      
-00001700: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00001710: 3e59 6f75 2063 616e 2070 7265 7669 6577  >You can preview
-00001720: 2079 6f75 7220 466f 6e74 2073 6574 7469   your Font setti
-00001730: 6e67 7320 6865 7265 2e3c 2f73 7472 696e  ngs here.</strin
-00001740: 673e 0a20 2020 2020 2020 2020 2020 2020  g>.             
-00001750: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-00001760: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00001770: 6572 7479 206e 616d 653d 2272 6561 644f  erty name="readO
-00001780: 6e6c 7922 3e0a 2020 2020 2020 2020 2020  nly">.          
-00001790: 2020 2020 203c 626f 6f6c 3e74 7275 653c       <bool>true<
-000017a0: 2f62 6f6f 6c3e 0a20 2020 2020 2020 2020  /bool>.         
-000017b0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-000017c0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-000017d0: 7072 6f70 6572 7479 206e 616d 653d 2268  property name="h
-000017e0: 746d 6c22 3e0a 2020 2020 2020 2020 2020  tml">.          
-000017f0: 2020 2020 203c 7374 7269 6e67 3e26 6c74       <string>&lt
-00001800: 3b21 444f 4354 5950 4520 4854 4d4c 2050  ;!DOCTYPE HTML P
-00001810: 5542 4c49 4320 2671 756f 743b 2d2f 2f57  UBLIC &quot;-//W
-00001820: 3343 2f2f 4454 4420 4854 4d4c 2034 2e30  3C//DTD HTML 4.0
-00001830: 2f2f 454e 2671 756f 743b 2026 7175 6f74  //EN&quot; &quot
-00001840: 3b68 7474 703a 2f2f 7777 772e 7733 2e6f  ;http://www.w3.o
-00001850: 7267 2f54 522f 5245 432d 6874 6d6c 3430  rg/TR/REC-html40
-00001860: 2f73 7472 6963 742e 6474 6426 7175 6f74  /strict.dtd&quot
-00001870: 3b26 6774 3b0a 266c 743b 6874 6d6c 2667  ;&gt;.&lt;html&g
-00001880: 743b 266c 743b 6865 6164 2667 743b 266c  t;&lt;head&gt;&l
-00001890: 743b 6d65 7461 206e 616d 653d 2671 756f  t;meta name=&quo
-000018a0: 743b 7172 6963 6874 6578 7426 7175 6f74  t;qrichtext&quot
-000018b0: 3b20 636f 6e74 656e 743d 2671 756f 743b  ; content=&quot;
-000018c0: 3126 7175 6f74 3b20 2f26 6774 3b26 6c74  1&quot; /&gt;&lt
-000018d0: 3b73 7479 6c65 2074 7970 653d 2671 756f  ;style type=&quo
-000018e0: 743b 7465 7874 2f63 7373 2671 756f 743b  t;text/css&quot;
-000018f0: 2667 743b 0a70 2c20 6c69 207b 2077 6869  &gt;.p, li { whi
-00001900: 7465 2d73 7061 6365 3a20 7072 652d 7772  te-space: pre-wr
-00001910: 6170 3b20 7d0a 266c 743b 2f73 7479 6c65  ap; }.&lt;/style
-00001920: 2667 743b 266c 743b 2f68 6561 6426 6774  &gt;&lt;/head&gt
-00001930: 3b26 6c74 3b62 6f64 7920 7374 796c 653d  ;&lt;body style=
-00001940: 2671 756f 743b 2066 6f6e 742d 6661 6d69  &quot; font-fami
-00001950: 6c79 3a27 4465 6a61 5675 2053 616e 7327  ly:'DejaVu Sans'
-00001960: 3b20 666f 6e74 2d73 697a 653a 3970 743b  ; font-size:9pt;
-00001970: 2066 6f6e 742d 7765 6967 6874 3a34 3030   font-weight:400
-00001980: 3b20 666f 6e74 2d73 7479 6c65 3a6e 6f72  ; font-style:nor
-00001990: 6d61 6c3b 2671 756f 743b 2667 743b 0a26  mal;&quot;&gt;.&
-000019a0: 6c74 3b74 6162 6c65 2062 6f72 6465 723d  lt;table border=
-000019b0: 2671 756f 743b 3026 7175 6f74 3b20 7374  &quot;0&quot; st
-000019c0: 796c 653d 2671 756f 743b 2d71 742d 7461  yle=&quot;-qt-ta
-000019d0: 626c 652d 7479 7065 3a20 726f 6f74 3b20  ble-type: root; 
-000019e0: 6d61 7267 696e 2d74 6f70 3a34 7078 3b20  margin-top:4px; 
-000019f0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3470  margin-bottom:4p
-00001a00: 783b 206d 6172 6769 6e2d 6c65 6674 3a34  x; margin-left:4
-00001a10: 7078 3b20 6d61 7267 696e 2d72 6967 6874  px; margin-right
-00001a20: 3a34 7078 3b26 7175 6f74 3b26 6774 3b0a  :4px;&quot;&gt;.
-00001a30: 266c 743b 7472 2667 743b 0a26 6c74 3b74  &lt;tr&gt;.&lt;t
-00001a40: 6420 7374 796c 653d 2671 756f 743b 626f  d style=&quot;bo
-00001a50: 7264 6572 3a20 6e6f 6e65 3b26 7175 6f74  rder: none;&quot
-00001a60: 3b26 6774 3b0a 266c 743b 7020 7374 796c  ;&gt;.&lt;p styl
-00001a70: 653d 2671 756f 743b 206d 6172 6769 6e2d  e=&quot; margin-
-00001a80: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
-00001a90: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
-00001aa0: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
-00001ab0: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
-00001ac0: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
-00001ad0: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
-00001ae0: 7078 3b26 7175 6f74 3b26 6774 3b45 6e20  px;&quot;&gt;En 
-00001af0: 756e 206c 7567 6172 2064 6520 4c61 204d  un lugar de La M
-00001b00: 616e 6368 612c 266c 743b 2f70 2667 743b  ancha,&lt;/p&gt;
-00001b10: 0a26 6c74 3b70 2073 7479 6c65 3d26 7175  .&lt;p style=&qu
-00001b20: 6f74 3b20 6d61 7267 696e 2d74 6f70 3a30  ot; margin-top:0
-00001b30: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
-00001b40: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
-00001b50: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
-00001b60: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
-00001b70: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
-00001b80: 7874 2d69 6e64 656e 743a 3070 783b 2671  xt-indent:0px;&q
-00001b90: 756f 743b 2667 743b 6465 2063 7579 6f20  uot;&gt;de cuyo 
-00001ba0: 6e6f 6d62 7265 206e 6f20 7175 6965 726f  nombre no quiero
-00001bb0: 2061 636f 7264 6172 6d65 2c26 6c74 3b2f   acordarme,&lt;/
-00001bc0: 7026 6774 3b0a 266c 743b 7020 7374 796c  p&gt;.&lt;p styl
-00001bd0: 653d 2671 756f 743b 206d 6172 6769 6e2d  e=&quot; margin-
-00001be0: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
-00001bf0: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
-00001c00: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
-00001c10: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
-00001c20: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
-00001c30: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
-00001c40: 7078 3b26 7175 6f74 3b26 6774 3b6e 6f20  px;&quot;&gt;no 
-00001c50: 6861 206d 7563 686f 2074 6965 6d70 6f20  ha mucho tiempo 
-00001c60: 7669 7669 6120 756e 2068 6964 616c 676f  vivia un hidalgo
-00001c70: 2e2e 266c 743b 2f70 2667 743b 0a26 6c74  ..&lt;/p&gt;.&lt
-00001c80: 3b70 2073 7479 6c65 3d26 7175 6f74 3b2d  ;p style=&quot;-
-00001c90: 7174 2d70 6172 6167 7261 7068 2d74 7970  qt-paragraph-typ
-00001ca0: 653a 656d 7074 793b 206d 6172 6769 6e2d  e:empty; margin-
-00001cb0: 746f 703a 3070 783b 206d 6172 6769 6e2d  top:0px; margin-
-00001cc0: 626f 7474 6f6d 3a30 7078 3b20 6d61 7267  bottom:0px; marg
-00001cd0: 696e 2d6c 6566 743a 3070 783b 206d 6172  in-left:0px; mar
-00001ce0: 6769 6e2d 7269 6768 743a 3070 783b 202d  gin-right:0px; -
-00001cf0: 7174 2d62 6c6f 636b 2d69 6e64 656e 743a  qt-block-indent:
-00001d00: 303b 2074 6578 742d 696e 6465 6e74 3a30  0; text-indent:0
-00001d10: 7078 3b26 7175 6f74 3b26 6774 3b26 6c74  px;&quot;&gt;&lt
-00001d20: 3b2f 7026 6774 3b26 6c74 3b2f 7464 2667  ;/p&gt;&lt;/td&g
-00001d30: 743b 266c 743b 2f74 7226 6774 3b26 6c74  t;&lt;/tr&gt;&lt
-00001d40: 3b2f 7461 626c 6526 6774 3b26 6c74 3b2f  ;/table&gt;&lt;/
-00001d50: 626f 6479 2667 743b 266c 743b 2f68 746d  body&gt;&lt;/htm
-00001d60: 6c26 6774 3b3c 2f73 7472 696e 673e 0a20  l&gt;</string>. 
-00001d70: 2020 2020 2020 2020 2020 2020 203c 2f70               </p
-00001d80: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00001d90: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001da0: 206e 616d 653d 2274 6578 7449 6e74 6572   name="textInter
-00001db0: 6163 7469 6f6e 466c 6167 7322 3e0a 2020  actionFlags">.  
-00001dc0: 2020 2020 2020 2020 2020 2020 203c 7365               <se
-00001dd0: 743e 5174 3a3a 4e6f 5465 7874 496e 7465  t>Qt::NoTextInte
-00001de0: 7261 6374 696f 6e3c 2f73 6574 3e0a 2020  raction</set>.  
-00001df0: 2020 2020 2020 2020 2020 2020 3c2f 7072              </pr
-00001e00: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00001e10: 2020 2020 203c 2f77 6964 6765 743e 0a20       </widget>. 
-00001e20: 2020 2020 2020 2020 2020 203c 2f69 7465             </ite
-00001e30: 6d3e 0a20 2020 2020 2020 2020 2020 203c  m>.            <
-00001e40: 6974 656d 2072 6f77 3d22 3322 2063 6f6c  item row="3" col
-00001e50: 756d 6e3d 2230 223e 0a20 2020 2020 2020  umn="0">.       
-00001e60: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
-00001e70: 6173 733d 2251 5075 7368 4275 7474 6f6e  ass="QPushButton
-00001e80: 2220 6e61 6d65 3d22 666f 7265 6772 6f75  " name="foregrou
-00001e90: 6e64 5042 223e 0a20 2020 2020 2020 2020  ndPB">.         
-00001ea0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00001eb0: 616d 653d 2277 6861 7473 5468 6973 223e  ame="whatsThis">
-00001ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ed0: 3c73 7472 696e 673e 5365 7475 7020 7468  <string>Setup th
-00001ee0: 6520 7465 7874 2063 6f6c 6f72 2e3c 2f73  e text color.</s
-00001ef0: 7472 696e 673e 0a20 2020 2020 2020 2020  tring>.         
-00001f00: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00001f10: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00001f20: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-00001f30: 6578 7422 3e0a 2020 2020 2020 2020 2020  ext">.          
-00001f40: 2020 2020 203c 7374 7269 6e67 2063 6f6d       <string com
-00001f50: 6d65 6e74 3d22 5468 6520 6c61 6265 6c20  ment="The label 
-00001f60: 6f66 2074 6865 206c 6f67 6765 7220 7465  of the logger te
-00001f70: 7874 2063 6f6c 6f72 2062 7574 746f 6e22  xt color button"
-00001f80: 3e46 2661 6d70 3b6f 7265 6772 6f75 6e64  >F&amp;oreground
-00001f90: 3c2f 7374 7269 6e67 3e0a 2020 2020 2020  </string>.      
-00001fa0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00001fb0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00001fc0: 203c 2f77 6964 6765 743e 0a20 2020 2020   </widget>.     
-00001fd0: 2020 2020 2020 203c 2f69 7465 6d3e 0a20         </item>. 
-00001fe0: 2020 2020 2020 2020 2020 203c 6974 656d             <item
-00001ff0: 2072 6f77 3d22 3122 2063 6f6c 756d 6e3d   row="1" column=
-00002000: 2230 223e 0a20 2020 2020 2020 2020 2020  "0">.           
-00002010: 2020 3c73 7061 6365 7220 6e61 6d65 3d22    <spacer name="
-00002020: 7665 7274 6963 616c 5370 6163 6572 223e  verticalSpacer">
-00002030: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00002040: 7072 6f70 6572 7479 206e 616d 653d 226f  property name="o
-00002050: 7269 656e 7461 7469 6f6e 223e 0a20 2020  rientation">.   
-00002060: 2020 2020 2020 2020 2020 2020 3c65 6e75              <enu
-00002070: 6d3e 5174 3a3a 5665 7274 6963 616c 3c2f  m>Qt::Vertical</
-00002080: 656e 756d 3e0a 2020 2020 2020 2020 2020  enum>.          
-00002090: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-000020a0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000020b0: 726f 7065 7274 7920 6e61 6d65 3d22 7369  roperty name="si
-000020c0: 7a65 4869 6e74 2220 7374 6473 6574 3d22  zeHint" stdset="
-000020d0: 3022 3e0a 2020 2020 2020 2020 2020 2020  0">.            
-000020e0: 2020 203c 7369 7a65 3e0a 2020 2020 2020     <size>.      
-000020f0: 2020 2020 2020 2020 2020 3c77 6964 7468            <width
-00002100: 3e32 303c 2f77 6964 7468 3e0a 2020 2020  >20</width>.    
-00002110: 2020 2020 2020 2020 2020 2020 3c68 6569              <hei
-00002120: 6768 743e 3430 3c2f 6865 6967 6874 3e0a  ght>40</height>.
-00002130: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002140: 2f73 697a 653e 0a20 2020 2020 2020 2020  /size>.         
+00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
+00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
+00000040: 6173 733e 5365 7474 696e 6773 4469 616c  ass>SettingsDial
+00000050: 6f67 3c2f 636c 6173 733e 0d0a 203c 7769  og</class>.. <wi
+00000060: 6467 6574 2063 6c61 7373 3d22 5144 6961  dget class="QDia
+00000070: 6c6f 6722 206e 616d 653d 2253 6574 7469  log" name="Setti
+00000080: 6e67 7344 6961 6c6f 6722 3e0d 0a20 203c  ngsDialog">..  <
+00000090: 7072 6f70 6572 7479 206e 616d 653d 2267  property name="g
+000000a0: 656f 6d65 7472 7922 3e0d 0a20 2020 3c72  eometry">..   <r
+000000b0: 6563 743e 0d0a 2020 2020 3c78 3e30 3c2f  ect>..    <x>0</
+000000c0: 783e 0d0a 2020 2020 3c79 3e30 3c2f 793e  x>..    <y>0</y>
+000000d0: 0d0a 2020 2020 3c77 6964 7468 3e35 3432  ..    <width>542
+000000e0: 3c2f 7769 6474 683e 0d0a 2020 2020 3c68  </width>..    <h
+000000f0: 6569 6768 743e 3431 393c 2f68 6569 6768  eight>419</heigh
+00000100: 743e 0d0a 2020 203c 2f72 6563 743e 0d0a  t>..   </rect>..
+00000110: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
+00000120: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000130: 2277 696e 646f 7754 6974 6c65 223e 0d0a  "windowTitle">..
+00000140: 2020 203c 7374 7269 6e67 3e56 6954 6162     <string>ViTab
+00000150: 6c65 7320 7365 7474 696e 6773 3c2f 7374  les settings</st
+00000160: 7269 6e67 3e0d 0a20 203c 2f70 726f 7065  ring>..  </prope
+00000170: 7274 793e 0d0a 2020 3c6c 6179 6f75 7420  rty>..  <layout 
+00000180: 636c 6173 733d 2251 5642 6f78 4c61 796f  class="QVBoxLayo
+00000190: 7574 2220 6e61 6d65 3d22 7665 7274 6963  ut" name="vertic
+000001a0: 616c 4c61 796f 7574 5f32 223e 0d0a 2020  alLayout_2">..  
+000001b0: 203c 6974 656d 3e0d 0a20 2020 203c 6c61   <item>..    <la
+000001c0: 796f 7574 2063 6c61 7373 3d22 5148 426f  yout class="QHBo
+000001d0: 784c 6179 6f75 7422 206e 616d 653d 2268  xLayout" name="h
+000001e0: 6f72 697a 6f6e 7461 6c4c 6179 6f75 7422  orizontalLayout"
+000001f0: 3e0d 0a20 2020 2020 3c69 7465 6d3e 0d0a  >..     <item>..
+00000200: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
+00000210: 6173 733d 2251 5472 6565 5669 6577 2220  ass="QTreeView" 
+00000220: 6e61 6d65 3d22 7061 6765 5365 6c65 6374  name="pageSelect
+00000230: 6f72 223e 0d0a 2020 2020 2020 203c 7072  or">..       <pr
+00000240: 6f70 6572 7479 206e 616d 653d 2273 697a  operty name="siz
+00000250: 6550 6f6c 6963 7922 3e0d 0a20 2020 2020  ePolicy">..     
+00000260: 2020 203c 7369 7a65 706f 6c69 6379 2068     <sizepolicy h
+00000270: 7369 7a65 7479 7065 3d22 4d69 6e69 6d75  sizetype="Minimu
+00000280: 6d45 7870 616e 6469 6e67 2220 7673 697a  mExpanding" vsiz
+00000290: 6574 7970 653d 2245 7870 616e 6469 6e67  etype="Expanding
+000002a0: 223e 0d0a 2020 2020 2020 2020 203c 686f  ">..         <ho
+000002b0: 7273 7472 6574 6368 3e30 3c2f 686f 7273  rstretch>0</hors
+000002c0: 7472 6574 6368 3e0d 0a20 2020 2020 2020  tretch>..       
+000002d0: 2020 3c76 6572 7374 7265 7463 683e 303c    <verstretch>0<
+000002e0: 2f76 6572 7374 7265 7463 683e 0d0a 2020  /verstretch>..  
+000002f0: 2020 2020 2020 3c2f 7369 7a65 706f 6c69        </sizepoli
+00000300: 6379 3e0d 0a20 2020 2020 2020 3c2f 7072  cy>..       </pr
+00000310: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00000320: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00000330: 6d69 6e69 6d75 6d53 697a 6522 3e0d 0a20  minimumSize">.. 
+00000340: 2020 2020 2020 203c 7369 7a65 3e0d 0a20         <size>.. 
+00000350: 2020 2020 2020 2020 3c77 6964 7468 3e31          <width>1
+00000360: 3631 3c2f 7769 6474 683e 0d0a 2020 2020  61</width>..    
+00000370: 2020 2020 203c 6865 6967 6874 3e33 3830       <height>380
+00000380: 3c2f 6865 6967 6874 3e0d 0a20 2020 2020  </height>..     
+00000390: 2020 203c 2f73 697a 653e 0d0a 2020 2020     </size>..    
+000003a0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+000003b0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000003c0: 206e 616d 653d 226d 6178 696d 756d 5369   name="maximumSi
+000003d0: 7a65 223e 0d0a 2020 2020 2020 2020 3c73  ze">..        <s
+000003e0: 697a 653e 0d0a 2020 2020 2020 2020 203c  ize>..         <
+000003f0: 7769 6474 683e 3230 303c 2f77 6964 7468  width>200</width
+00000400: 3e0d 0a20 2020 2020 2020 2020 3c68 6569  >..         <hei
+00000410: 6768 743e 3136 3737 3732 3135 3c2f 6865  ght>16777215</he
+00000420: 6967 6874 3e0d 0a20 2020 2020 2020 203c  ight>..        <
+00000430: 2f73 697a 653e 0d0a 2020 2020 2020 203c  /size>..       <
+00000440: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
+00000450: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000460: 653d 2277 6861 7473 5468 6973 223e 0d0a  e="whatsThis">..
+00000470: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
+00000480: 436c 6963 6b20 616e 2069 7465 6d20 696e  Click an item in
+00000490: 2074 6869 7320 7472 6565 2074 6f20 7365   this tree to se
+000004a0: 6c65 6374 2074 6865 2073 6574 7469 6e67  lect the setting
+000004b0: 7320 796f 7520 7761 6e74 2074 6f20 6368  s you want to ch
+000004c0: 616e 6765 2e20 4265 7761 7265 2074 6861  ange. Beware tha
+000004d0: 7420 7468 6520 6c69 7374 6564 2070 6c75  t the listed plu
+000004e0: 6769 6e73 2061 7265 202a 6c6f 6164 6564  gins are *loaded
+000004f0: 2a20 706c 7567 696e 7320 2869 2e65 2e20  * plugins (i.e. 
+00000500: 7468 6520 6172 6520 776f 726b 696e 6720  the are working 
+00000510: 696e 2074 6865 2063 7572 7265 6e74 2056  in the current V
+00000520: 6954 6162 6c65 7320 7365 7373 696f 6e29  iTables session)
+00000530: 206e 6f74 206a 7573 7420 656e 6162 6c65   not just enable
+00000540: 6420 706c 7567 696e 732e 3c2f 7374 7269  d plugins.</stri
+00000550: 6e67 3e0d 0a20 2020 2020 2020 3c2f 7072  ng>..       </pr
+00000560: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00000570: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00000580: 6564 6974 5472 6967 6765 7273 223e 0d0a  editTriggers">..
+00000590: 2020 2020 2020 2020 3c73 6574 3e51 4162          <set>QAb
+000005a0: 7374 7261 6374 4974 656d 5669 6577 3a3a  stractItemView::
+000005b0: 4e6f 4564 6974 5472 6967 6765 7273 3c2f  NoEditTriggers</
+000005c0: 7365 743e 0d0a 2020 2020 2020 203c 2f70  set>..       </p
+000005d0: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
+000005e0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000005f0: 2269 636f 6e53 697a 6522 3e0d 0a20 2020  "iconSize">..   
+00000600: 2020 2020 203c 7369 7a65 3e0d 0a20 2020       <size>..   
+00000610: 2020 2020 2020 3c77 6964 7468 3e32 323c        <width>22<
+00000620: 2f77 6964 7468 3e0d 0a20 2020 2020 2020  /width>..       
+00000630: 2020 3c68 6569 6768 743e 3232 3c2f 6865    <height>22</he
+00000640: 6967 6874 3e0d 0a20 2020 2020 2020 203c  ight>..        <
+00000650: 2f73 697a 653e 0d0a 2020 2020 2020 203c  /size>..       <
+00000660: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
+00000670: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
+00000680: 6d65 3d22 6865 6164 6572 5669 7369 626c  me="headerVisibl
+00000690: 6522 3e0d 0a20 2020 2020 2020 203c 626f  e">..        <bo
+000006a0: 6f6c 3e66 616c 7365 3c2f 626f 6f6c 3e0d  ol>false</bool>.
+000006b0: 0a20 2020 2020 2020 3c2f 6174 7472 6962  .       </attrib
+000006c0: 7574 653e 0d0a 2020 2020 2020 203c 6174  ute>..       <at
+000006d0: 7472 6962 7574 6520 6e61 6d65 3d22 6865  tribute name="he
+000006e0: 6164 6572 4465 6661 756c 7453 6563 7469  aderDefaultSecti
+000006f0: 6f6e 5369 7a65 223e 0d0a 2020 2020 2020  onSize">..      
+00000700: 2020 3c6e 756d 6265 723e 3130 303c 2f6e    <number>100</n
+00000710: 756d 6265 723e 0d0a 2020 2020 2020 203c  umber>..       <
+00000720: 2f61 7474 7269 6275 7465 3e0d 0a20 2020  /attribute>..   
+00000730: 2020 2020 3c61 7474 7269 6275 7465 206e      <attribute n
+00000740: 616d 653d 2268 6561 6465 7244 6566 6175  ame="headerDefau
+00000750: 6c74 5365 6374 696f 6e53 697a 6522 3e0d  ltSectionSize">.
+00000760: 0a20 2020 2020 2020 203c 6e75 6d62 6572  .        <number
+00000770: 3e31 3030 3c2f 6e75 6d62 6572 3e0d 0a20  >100</number>.. 
+00000780: 2020 2020 2020 3c2f 6174 7472 6962 7574        </attribut
+00000790: 653e 0d0a 2020 2020 2020 203c 6174 7472  e>..       <attr
+000007a0: 6962 7574 6520 6e61 6d65 3d22 6865 6164  ibute name="head
+000007b0: 6572 5669 7369 626c 6522 3e0d 0a20 2020  erVisible">..   
+000007c0: 2020 2020 203c 626f 6f6c 3e66 616c 7365       <bool>false
+000007d0: 3c2f 626f 6f6c 3e0d 0a20 2020 2020 2020  </bool>..       
+000007e0: 3c2f 6174 7472 6962 7574 653e 0d0a 2020  </attribute>..  
+000007f0: 2020 2020 3c2f 7769 6467 6574 3e0d 0a20      </widget>.. 
+00000800: 2020 2020 3c2f 6974 656d 3e0d 0a20 2020      </item>..   
+00000810: 2020 3c69 7465 6d3e 0d0a 2020 2020 2020    <item>..      
+00000820: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+00000830: 5374 6163 6b65 6457 6964 6765 7422 206e  StackedWidget" n
+00000840: 616d 653d 2273 7461 636b 6564 5061 6765  ame="stackedPage
+00000850: 7322 3e0d 0a20 2020 2020 2020 3c70 726f  s">..       <pro
+00000860: 7065 7274 7920 6e61 6d65 3d22 7369 7a65  perty name="size
+00000870: 506f 6c69 6379 223e 0d0a 2020 2020 2020  Policy">..      
+00000880: 2020 3c73 697a 6570 6f6c 6963 7920 6873    <sizepolicy hs
+00000890: 697a 6574 7970 653d 2250 7265 6665 7272  izetype="Preferr
+000008a0: 6564 2220 7673 697a 6574 7970 653d 2250  ed" vsizetype="P
+000008b0: 7265 6665 7272 6564 223e 0d0a 2020 2020  referred">..    
+000008c0: 2020 2020 203c 686f 7273 7472 6574 6368       <horstretch
+000008d0: 3e30 3c2f 686f 7273 7472 6574 6368 3e0d  >0</horstretch>.
+000008e0: 0a20 2020 2020 2020 2020 3c76 6572 7374  .         <verst
+000008f0: 7265 7463 683e 303c 2f76 6572 7374 7265  retch>0</verstre
+00000900: 7463 683e 0d0a 2020 2020 2020 2020 3c2f  tch>..        </
+00000910: 7369 7a65 706f 6c69 6379 3e0d 0a20 2020  sizepolicy>..   
+00000920: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
+00000930: 0a20 2020 2020 2020 3c70 726f 7065 7274  .       <propert
+00000940: 7920 6e61 6d65 3d22 6375 7272 656e 7449  y name="currentI
+00000950: 6e64 6578 223e 0d0a 2020 2020 2020 2020  ndex">..        
+00000960: 3c6e 756d 6265 723e 323c 2f6e 756d 6265  <number>2</numbe
+00000970: 723e 0d0a 2020 2020 2020 203c 2f70 726f  r>..       </pro
+00000980: 7065 7274 793e 0d0a 2020 2020 2020 203c  perty>..       <
+00000990: 7769 6467 6574 2063 6c61 7373 3d22 5157  widget class="QW
+000009a0: 6964 6765 7422 206e 616d 653d 2273 7461  idget" name="sta
+000009b0: 7274 7570 5061 6765 223e 0d0a 2020 2020  rtupPage">..    
+000009c0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+000009d0: 6d65 3d22 7369 7a65 506f 6c69 6379 223e  me="sizePolicy">
+000009e0: 0d0a 2020 2020 2020 2020 203c 7369 7a65  ..         <size
+000009f0: 706f 6c69 6379 2068 7369 7a65 7479 7065  policy hsizetype
+00000a00: 3d22 4578 7061 6e64 696e 6722 2076 7369  ="Expanding" vsi
+00000a10: 7a65 7479 7065 3d22 5072 6566 6572 7265  zetype="Preferre
+00000a20: 6422 3e0d 0a20 2020 2020 2020 2020 203c  d">..          <
+00000a30: 686f 7273 7472 6574 6368 3e30 3c2f 686f  horstretch>0</ho
+00000a40: 7273 7472 6574 6368 3e0d 0a20 2020 2020  rstretch>..     
+00000a50: 2020 2020 203c 7665 7273 7472 6574 6368       <verstretch
+00000a60: 3e30 3c2f 7665 7273 7472 6574 6368 3e0d  >0</verstretch>.
+00000a70: 0a20 2020 2020 2020 2020 3c2f 7369 7a65  .         </size
+00000a80: 706f 6c69 6379 3e0d 0a20 2020 2020 2020  policy>..       
+00000a90: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
+00000aa0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000ab0: 6e61 6d65 3d22 7768 6174 7354 6869 7322  name="whatsThis"
+00000ac0: 3e0d 0a20 2020 2020 2020 2020 3c73 7472  >..         <str
+00000ad0: 696e 673e 436f 6e66 6967 7572 6520 7468  ing>Configure th
+00000ae0: 6520 7374 6172 7475 7020 6265 6861 7669  e startup behavi
+00000af0: 6f72 206f 6620 5669 5461 626c 6573 2e3c  or of ViTables.<
+00000b00: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
+00000b10: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
+00000b20: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
+00000b30: 6c61 7373 3d22 5147 726f 7570 426f 7822  lass="QGroupBox"
+00000b40: 206e 616d 653d 2273 7461 7274 7570 4742   name="startupGB
+00000b50: 223e 0d0a 2020 2020 2020 2020 203c 7072  ">..         <pr
+00000b60: 6f70 6572 7479 206e 616d 653d 2267 656f  operty name="geo
+00000b70: 6d65 7472 7922 3e0d 0a20 2020 2020 2020  metry">..       
+00000b80: 2020 203c 7265 6374 3e0d 0a20 2020 2020     <rect>..     
+00000b90: 2020 2020 2020 3c78 3e34 3c2f 783e 0d0a        <x>4</x>..
+00000ba0: 2020 2020 2020 2020 2020 203c 793e 343c             <y>4<
+00000bb0: 2f79 3e0d 0a20 2020 2020 2020 2020 2020  /y>..           
+00000bc0: 3c77 6964 7468 3e33 3531 3c2f 7769 6474  <width>351</widt
+00000bd0: 683e 0d0a 2020 2020 2020 2020 2020 203c  h>..           <
+00000be0: 6865 6967 6874 3e33 3531 3c2f 6865 6967  height>351</heig
+00000bf0: 6874 3e0d 0a20 2020 2020 2020 2020 203c  ht>..          <
+00000c00: 2f72 6563 743e 0d0a 2020 2020 2020 2020  /rect>..        
+00000c10: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
+00000c20: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00000c30: 206e 616d 653d 2273 697a 6550 6f6c 6963   name="sizePolic
+00000c40: 7922 3e0d 0a20 2020 2020 2020 2020 203c  y">..          <
+00000c50: 7369 7a65 706f 6c69 6379 2068 7369 7a65  sizepolicy hsize
+00000c60: 7479 7065 3d22 4d61 7869 6d75 6d22 2076  type="Maximum" v
+00000c70: 7369 7a65 7479 7065 3d22 5072 6566 6572  sizetype="Prefer
+00000c80: 7265 6422 3e0d 0a20 2020 2020 2020 2020  red">..         
+00000c90: 2020 3c68 6f72 7374 7265 7463 683e 303c    <horstretch>0<
+00000ca0: 2f68 6f72 7374 7265 7463 683e 0d0a 2020  /horstretch>..  
+00000cb0: 2020 2020 2020 2020 203c 7665 7273 7472           <verstr
+00000cc0: 6574 6368 3e30 3c2f 7665 7273 7472 6574  etch>0</verstret
+00000cd0: 6368 3e0d 0a20 2020 2020 2020 2020 203c  ch>..          <
+00000ce0: 2f73 697a 6570 6f6c 6963 793e 0d0a 2020  /sizepolicy>..  
+00000cf0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00000d00: 793e 0d0a 2020 2020 2020 2020 203c 7072  y>..         <pr
+00000d10: 6f70 6572 7479 206e 616d 653d 2277 6861  operty name="wha
+00000d20: 7473 5468 6973 223e 0d0a 2020 2020 2020  tsThis">..      
+00000d30: 2020 2020 3c73 7472 696e 672f 3e0d 0a20      <string/>.. 
+00000d40: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+00000d50: 7479 3e0d 0a20 2020 2020 2020 2020 3c70  ty>..         <p
+00000d60: 726f 7065 7274 7920 6e61 6d65 3d22 7469  roperty name="ti
+00000d70: 746c 6522 3e0d 0a20 2020 2020 2020 2020  tle">..         
+00000d80: 203c 7374 7269 6e67 2063 6f6d 6d65 6e74   <string comment
+00000d90: 3d22 5468 6520 6e61 6d65 206f 6620 7468  ="The name of th
+00000da0: 6520 6772 6f75 7062 6f78 2077 6865 7265  e groupbox where
+00000db0: 2073 7461 7274 7570 2069 7320 636f 6e66   startup is conf
+00000dc0: 6967 7572 6564 223e 5374 6172 7475 703c  igured">Startup<
+00000dd0: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
+00000de0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+00000df0: 2020 2020 2020 2020 203c 6c61 796f 7574           <layout
+00000e00: 2063 6c61 7373 3d22 5156 426f 784c 6179   class="QVBoxLay
+00000e10: 6f75 7422 206e 616d 653d 2276 6572 7469  out" name="verti
+00000e20: 6361 6c4c 6179 6f75 745f 3322 3e0d 0a20  calLayout_3">.. 
+00000e30: 2020 2020 2020 2020 203c 6974 656d 3e0d           <item>.
+00000e40: 0a20 2020 2020 2020 2020 2020 3c77 6964  .           <wid
+00000e50: 6765 7420 636c 6173 733d 2251 4368 6563  get class="QChec
+00000e60: 6b42 6f78 2220 6e61 6d65 3d22 7265 7374  kBox" name="rest
+00000e70: 6f72 6543 4222 3e0d 0a20 2020 2020 2020  oreCB">..       
+00000e80: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000e90: 616d 653d 2277 6861 7473 5468 6973 223e  ame="whatsThis">
+00000ea0: 0d0a 2020 2020 2020 2020 2020 2020 203c  ..             <
+00000eb0: 7374 7269 6e67 3e49 6620 6368 6563 6b65  string>If checke
+00000ec0: 642c 2074 6865 206c 6173 7420 776f 726b  d, the last work
+00000ed0: 696e 6720 7365 7373 696f 6e20 2d69 2e65  ing session -i.e
+00000ee0: 2e20 6f70 656e 2066 696c 6573 2061 6e64  . open files and
+00000ef0: 2076 6965 7773 2d20 7769 6c6c 2062 6520   views- will be 
+00000f00: 7265 7374 6f72 6564 2e20 4966 206e 6f74  restored. If not
+00000f10: 2c20 5669 5461 626c 6573 2077 696c 6c20  , ViTables will 
+00000f20: 7374 6172 7420 7769 7468 2061 6e20 656d  start with an em
+00000f30: 7074 7920 7365 7373 696f 6e2e 3c2f 7374  pty session.</st
+00000f40: 7269 6e67 3e0d 0a20 2020 2020 2020 2020  ring>..         
+00000f50: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+00000f60: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00000f70: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
+00000f80: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00000f90: 203c 7374 7269 6e67 2063 6f6d 6d65 6e74   <string comment
+00000fa0: 3d22 4c61 6265 6c20 6f66 2074 6865 2072  ="Label of the r
+00000fb0: 6573 746f 7265 206c 6173 7420 7365 7373  estore last sess
+00000fc0: 696f 6e20 6368 6563 6b20 6275 7474 6f6e  ion check button
+00000fd0: 223e 5265 7374 6f72 6520 6c61 7374 2073  ">Restore last s
+00000fe0: 6573 7369 6f6e 3c2f 7374 7269 6e67 3e0d  ession</string>.
+00000ff0: 0a20 2020 2020 2020 2020 2020 203c 2f70  .            </p
+00001000: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
+00001010: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
+00001020: 2020 2020 2020 2020 2020 3c2f 6974 656d            </item
+00001030: 3e0d 0a20 2020 2020 2020 2020 203c 6974  >..          <it
+00001040: 656d 3e0d 0a20 2020 2020 2020 2020 2020  em>..           
+00001050: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+00001060: 4368 6563 6b42 6f78 2220 6e61 6d65 3d22  CheckBox" name="
+00001070: 6c61 7374 4469 7243 4222 3e0d 0a20 2020  lastDirCB">..   
+00001080: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00001090: 7479 206e 616d 653d 2277 6861 7473 5468  ty name="whatsTh
+000010a0: 6973 223e 0d0a 2020 2020 2020 2020 2020  is">..          
+000010b0: 2020 203c 7374 7269 6e67 3e54 6865 2077     <string>The w
+000010c0: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
+000010d0: 2075 7365 6420 7768 656e 206f 7065 6e69   used when openi
+000010e0: 6e67 2074 6865 2076 6572 7920 6669 7273  ng the very firs
+000010f0: 7420 6669 6c65 2e20 4974 2064 6566 6175  t file. It defau
+00001100: 6c74 7320 746f 2074 6865 2063 7572 7265  lts to the curre
+00001110: 6e74 2064 6972 6563 746f 7279 2069 6620  nt directory if 
+00001120: 5669 5461 626c 6573 2068 6173 2062 6565  ViTables has bee
+00001130: 6e20 6c61 756e 6368 6564 2066 726f 6d20  n launched from 
+00001140: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
+00001150: 206f 7220 746f 2074 6865 2075 7365 7227   or to the user'
+00001160: 7320 686f 6d65 2064 6972 6563 746f 7279  s home directory
+00001170: 2069 6620 5669 5461 626c 6573 2073 7461   if ViTables sta
+00001180: 7274 6564 2066 726f 6d20 6120 6d65 6e75  rted from a menu
+00001190: 206f 7220 6120 6465 736b 746f 7020 6963   or a desktop ic
+000011a0: 6f6e 2e20 4966 2074 6865 2063 6865 636b  on. If the check
+000011b0: 626f 7820 6973 2063 6865 636b 6564 2074  box is checked t
+000011c0: 6865 6e20 7468 6520 6c61 7374 2065 6e74  hen the last ent
+000011d0: 6572 6564 2064 6972 6563 746f 7279 2077  ered directory w
+000011e0: 696c 6c20 6265 2075 7365 642e 3c2f 7374  ill be used.</st
+000011f0: 7269 6e67 3e0d 0a20 2020 2020 2020 2020  ring>..         
+00001200: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+00001210: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00001220: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
+00001230: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00001240: 203c 7374 7269 6e67 2063 6f6d 6d65 6e74   <string comment
+00001250: 3d22 4c61 6265 6c20 6f66 2074 6865 2073  ="Label of the s
+00001260: 7461 7274 7570 2069 6e20 7468 6520 6c61  tartup in the la
+00001270: 7374 206f 7065 6e20 6469 7265 6374 6f72  st open director
+00001280: 7920 6368 6563 6b20 626f 7822 3e53 7461  y check box">Sta
+00001290: 7274 2069 6e20 6c61 7374 2077 6f72 6b69  rt in last worki
+000012a0: 6e67 2064 6972 6563 746f 7279 3c2f 7374  ng directory</st
+000012b0: 7269 6e67 3e0d 0a20 2020 2020 2020 2020  ring>..         
+000012c0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+000012d0: 2020 2020 2020 2020 2020 203c 2f77 6964             </wid
+000012e0: 6765 743e 0d0a 2020 2020 2020 2020 2020  get>..          
+000012f0: 3c2f 6974 656d 3e0d 0a20 2020 2020 2020  </item>..       
+00001300: 2020 3c2f 6c61 796f 7574 3e0d 0a20 2020    </layout>..   
+00001310: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
+00001320: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
+00001330: 0d0a 2020 2020 2020 203c 7769 6467 6574  ..       <widget
+00001340: 2063 6c61 7373 3d22 5157 6964 6765 7422   class="QWidget"
+00001350: 206e 616d 653d 2273 7479 6c65 5061 6765   name="stylePage
+00001360: 223e 0d0a 2020 2020 2020 2020 3c70 726f  ">..        <pro
+00001370: 7065 7274 7920 6e61 6d65 3d22 7369 7a65  perty name="size
+00001380: 506f 6c69 6379 223e 0d0a 2020 2020 2020  Policy">..      
+00001390: 2020 203c 7369 7a65 706f 6c69 6379 2068     <sizepolicy h
+000013a0: 7369 7a65 7479 7065 3d22 4578 7061 6e64  sizetype="Expand
+000013b0: 696e 6722 2076 7369 7a65 7479 7065 3d22  ing" vsizetype="
+000013c0: 5072 6566 6572 7265 6422 3e0d 0a20 2020  Preferred">..   
+000013d0: 2020 2020 2020 203c 686f 7273 7472 6574         <horstret
+000013e0: 6368 3e30 3c2f 686f 7273 7472 6574 6368  ch>0</horstretch
+000013f0: 3e0d 0a20 2020 2020 2020 2020 203c 7665  >..          <ve
+00001400: 7273 7472 6574 6368 3e30 3c2f 7665 7273  rstretch>0</vers
+00001410: 7472 6574 6368 3e0d 0a20 2020 2020 2020  tretch>..       
+00001420: 2020 3c2f 7369 7a65 706f 6c69 6379 3e0d    </sizepolicy>.
+00001430: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
+00001440: 7274 793e 0d0a 2020 2020 2020 2020 3c70  rty>..        <p
+00001450: 726f 7065 7274 7920 6e61 6d65 3d22 7768  roperty name="wh
+00001460: 6174 7354 6869 7322 3e0d 0a20 2020 2020  atsThis">..     
+00001470: 2020 2020 3c73 7472 696e 673e 436f 6e66      <string>Conf
+00001480: 6967 7572 6520 7468 6520 6c6f 6f6b 2061  igure the look a
+00001490: 6e64 2066 6565 6c20 6f66 2056 6954 6162  nd feel of ViTab
+000014a0: 6c65 732e 3c2f 7374 7269 6e67 3e0d 0a20  les.</string>.. 
+000014b0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+000014c0: 793e 0d0a 2020 2020 2020 2020 3c6c 6179  y>..        <lay
+000014d0: 6f75 7420 636c 6173 733d 2251 5642 6f78  out class="QVBox
+000014e0: 4c61 796f 7574 2220 6e61 6d65 3d22 7665  Layout" name="ve
+000014f0: 7274 6963 616c 4c61 796f 7574 223e 0d0a  rticalLayout">..
+00001500: 2020 2020 2020 2020 203c 6974 656d 3e0d           <item>.
+00001510: 0a20 2020 2020 2020 2020 203c 7769 6467  .          <widg
+00001520: 6574 2063 6c61 7373 3d22 5147 726f 7570  et class="QGroup
+00001530: 426f 7822 206e 616d 653d 226c 6f67 6765  Box" name="logge
+00001540: 7247 4222 3e0d 0a20 2020 2020 2020 2020  rGB">..         
+00001550: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00001560: 3d22 7768 6174 7354 6869 7322 3e0d 0a20  ="whatsThis">.. 
+00001570: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
+00001580: 6e67 3e43 7573 746f 6d69 7365 2066 6f6e  ng>Customise fon
+00001590: 7420 616e 6420 636f 6c6f 7273 206f 6620  t and colors of 
+000015a0: 7468 6520 4c6f 6767 6572 2e3c 2f73 7472  the Logger.</str
+000015b0: 696e 673e 0d0a 2020 2020 2020 2020 2020  ing>..          
+000015c0: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
+000015d0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+000015e0: 7479 206e 616d 653d 2274 6974 6c65 223e  ty name="title">
+000015f0: 0d0a 2020 2020 2020 2020 2020 2020 3c73  ..            <s
+00001600: 7472 696e 6720 636f 6d6d 656e 743d 2254  tring comment="T
+00001610: 6865 2074 6974 6c65 206f 6620 7468 6520  he title of the 
+00001620: 6c6f 6767 6572 2067 726f 7562 6f78 223e  logger groubox">
+00001630: 4c6f 6767 6572 3c2f 7374 7269 6e67 3e0d  Logger</string>.
+00001640: 0a20 2020 2020 2020 2020 2020 3c2f 7072  .           </pr
+00001650: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00001660: 2020 2020 3c6c 6179 6f75 7420 636c 6173      <layout clas
+00001670: 733d 2251 4772 6964 4c61 796f 7574 2220  s="QGridLayout" 
+00001680: 6e61 6d65 3d22 6772 6964 4c61 796f 7574  name="gridLayout
+00001690: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+000016a0: 3c69 7465 6d20 726f 773d 2230 2220 636f  <item row="0" co
+000016b0: 6c75 6d6e 3d22 3122 2072 6f77 7370 616e  lumn="1" rowspan
+000016c0: 3d22 3722 3e0d 0a20 2020 2020 2020 2020  ="7">..         
+000016d0: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
+000016e0: 733d 2251 5465 7874 4564 6974 2220 6e61  s="QTextEdit" na
+000016f0: 6d65 3d22 7361 6d70 6c65 5445 223e 0d0a  me="sampleTE">..
+00001700: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00001710: 726f 7065 7274 7920 6e61 6d65 3d22 6163  roperty name="ac
+00001720: 6365 7074 4472 6f70 7322 3e0d 0a20 2020  ceptDrops">..   
+00001730: 2020 2020 2020 2020 2020 2020 3c62 6f6f              <boo
+00001740: 6c3e 6661 6c73 653c 2f62 6f6f 6c3e 0d0a  l>false</bool>..
+00001750: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001760: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
+00001770: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00001780: 7479 206e 616d 653d 2277 6861 7473 5468  ty name="whatsTh
+00001790: 6973 223e 0d0a 2020 2020 2020 2020 2020  is">..          
+000017a0: 2020 2020 203c 7374 7269 6e67 3e59 6f75       <string>You
+000017b0: 2063 616e 2070 7265 7669 6577 2079 6f75   can preview you
+000017c0: 7220 466f 6e74 2073 6574 7469 6e67 7320  r Font settings 
+000017d0: 6865 7265 2e3c 2f73 7472 696e 673e 0d0a  here.</string>..
+000017e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000017f0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
+00001800: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00001810: 7479 206e 616d 653d 2272 6561 644f 6e6c  ty name="readOnl
+00001820: 7922 3e0d 0a20 2020 2020 2020 2020 2020  y">..           
+00001830: 2020 2020 3c62 6f6f 6c3e 7472 7565 3c2f      <bool>true</
+00001840: 626f 6f6c 3e0d 0a20 2020 2020 2020 2020  bool>..         
+00001850: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+00001860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001870: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00001880: 6874 6d6c 223e 0d0a 2020 2020 2020 2020  html">..        
+00001890: 2020 2020 2020 203c 7374 7269 6e67 3e26         <string>&
+000018a0: 6c74 3b21 444f 4354 5950 4520 4854 4d4c  lt;!DOCTYPE HTML
+000018b0: 2050 5542 4c49 4320 2671 756f 743b 2d2f   PUBLIC &quot;-/
+000018c0: 2f57 3343 2f2f 4454 4420 4854 4d4c 2034  /W3C//DTD HTML 4
+000018d0: 2e30 2f2f 454e 2671 756f 743b 2026 7175  .0//EN&quot; &qu
+000018e0: 6f74 3b68 7474 703a 2f2f 7777 772e 7733  ot;http://www.w3
+000018f0: 2e6f 7267 2f54 522f 5245 432d 6874 6d6c  .org/TR/REC-html
+00001900: 3430 2f73 7472 6963 742e 6474 6426 7175  40/strict.dtd&qu
+00001910: 6f74 3b26 6774 3b0d 0a26 6c74 3b68 746d  ot;&gt;..&lt;htm
+00001920: 6c26 6774 3b26 6c74 3b68 6561 6426 6774  l&gt;&lt;head&gt
+00001930: 3b26 6c74 3b6d 6574 6120 6e61 6d65 3d26  ;&lt;meta name=&
+00001940: 7175 6f74 3b71 7269 6368 7465 7874 2671  quot;qrichtext&q
+00001950: 756f 743b 2063 6f6e 7465 6e74 3d26 7175  uot; content=&qu
+00001960: 6f74 3b31 2671 756f 743b 202f 2667 743b  ot;1&quot; /&gt;
+00001970: 266c 743b 7374 796c 6520 7479 7065 3d26  &lt;style type=&
+00001980: 7175 6f74 3b74 6578 742f 6373 7326 7175  quot;text/css&qu
+00001990: 6f74 3b26 6774 3b0d 0a70 2c20 6c69 207b  ot;&gt;..p, li {
+000019a0: 2077 6869 7465 2d73 7061 6365 3a20 7072   white-space: pr
+000019b0: 652d 7772 6170 3b20 7d0d 0a26 6c74 3b2f  e-wrap; }..&lt;/
+000019c0: 7374 796c 6526 6774 3b26 6c74 3b2f 6865  style&gt;&lt;/he
+000019d0: 6164 2667 743b 266c 743b 626f 6479 2073  ad&gt;&lt;body s
+000019e0: 7479 6c65 3d26 7175 6f74 3b20 666f 6e74  tyle=&quot; font
+000019f0: 2d66 616d 696c 793a 2744 656a 6156 7520  -family:'DejaVu 
+00001a00: 5361 6e73 273b 2066 6f6e 742d 7369 7a65  Sans'; font-size
+00001a10: 3a39 7074 3b20 666f 6e74 2d77 6569 6768  :9pt; font-weigh
+00001a20: 743a 3430 303b 2066 6f6e 742d 7374 796c  t:400; font-styl
+00001a30: 653a 6e6f 726d 616c 3b26 7175 6f74 3b26  e:normal;&quot;&
+00001a40: 6774 3b0d 0a26 6c74 3b74 6162 6c65 2062  gt;..&lt;table b
+00001a50: 6f72 6465 723d 2671 756f 743b 3026 7175  order=&quot;0&qu
+00001a60: 6f74 3b20 7374 796c 653d 2671 756f 743b  ot; style=&quot;
+00001a70: 2d71 742d 7461 626c 652d 7479 7065 3a20  -qt-table-type: 
+00001a80: 726f 6f74 3b20 6d61 7267 696e 2d74 6f70  root; margin-top
+00001a90: 3a34 7078 3b20 6d61 7267 696e 2d62 6f74  :4px; margin-bot
+00001aa0: 746f 6d3a 3470 783b 206d 6172 6769 6e2d  tom:4px; margin-
+00001ab0: 6c65 6674 3a34 7078 3b20 6d61 7267 696e  left:4px; margin
+00001ac0: 2d72 6967 6874 3a34 7078 3b26 7175 6f74  -right:4px;&quot
+00001ad0: 3b26 6774 3b0d 0a26 6c74 3b74 7226 6774  ;&gt;..&lt;tr&gt
+00001ae0: 3b0d 0a26 6c74 3b74 6420 7374 796c 653d  ;..&lt;td style=
+00001af0: 2671 756f 743b 626f 7264 6572 3a20 6e6f  &quot;border: no
+00001b00: 6e65 3b26 7175 6f74 3b26 6774 3b0d 0a26  ne;&quot;&gt;..&
+00001b10: 6c74 3b70 2073 7479 6c65 3d26 7175 6f74  lt;p style=&quot
+00001b20: 3b20 6d61 7267 696e 2d74 6f70 3a30 7078  ; margin-top:0px
+00001b30: 3b20 6d61 7267 696e 2d62 6f74 746f 6d3a  ; margin-bottom:
+00001b40: 3070 783b 206d 6172 6769 6e2d 6c65 6674  0px; margin-left
+00001b50: 3a30 7078 3b20 6d61 7267 696e 2d72 6967  :0px; margin-rig
+00001b60: 6874 3a30 7078 3b20 2d71 742d 626c 6f63  ht:0px; -qt-bloc
+00001b70: 6b2d 696e 6465 6e74 3a30 3b20 7465 7874  k-indent:0; text
+00001b80: 2d69 6e64 656e 743a 3070 783b 2671 756f  -indent:0px;&quo
+00001b90: 743b 2667 743b 456e 2075 6e20 6c75 6761  t;&gt;En un luga
+00001ba0: 7220 6465 204c 6120 4d61 6e63 6861 2c26  r de La Mancha,&
+00001bb0: 6c74 3b2f 7026 6774 3b0d 0a26 6c74 3b70  lt;/p&gt;..&lt;p
+00001bc0: 2073 7479 6c65 3d26 7175 6f74 3b20 6d61   style=&quot; ma
+00001bd0: 7267 696e 2d74 6f70 3a30 7078 3b20 6d61  rgin-top:0px; ma
+00001be0: 7267 696e 2d62 6f74 746f 6d3a 3070 783b  rgin-bottom:0px;
+00001bf0: 206d 6172 6769 6e2d 6c65 6674 3a30 7078   margin-left:0px
+00001c00: 3b20 6d61 7267 696e 2d72 6967 6874 3a30  ; margin-right:0
+00001c10: 7078 3b20 2d71 742d 626c 6f63 6b2d 696e  px; -qt-block-in
+00001c20: 6465 6e74 3a30 3b20 7465 7874 2d69 6e64  dent:0; text-ind
+00001c30: 656e 743a 3070 783b 2671 756f 743b 2667  ent:0px;&quot;&g
+00001c40: 743b 6465 2063 7579 6f20 6e6f 6d62 7265  t;de cuyo nombre
+00001c50: 206e 6f20 7175 6965 726f 2061 636f 7264   no quiero acord
+00001c60: 6172 6d65 2c26 6c74 3b2f 7026 6774 3b0d  arme,&lt;/p&gt;.
+00001c70: 0a26 6c74 3b70 2073 7479 6c65 3d26 7175  .&lt;p style=&qu
+00001c80: 6f74 3b20 6d61 7267 696e 2d74 6f70 3a30  ot; margin-top:0
+00001c90: 7078 3b20 6d61 7267 696e 2d62 6f74 746f  px; margin-botto
+00001ca0: 6d3a 3070 783b 206d 6172 6769 6e2d 6c65  m:0px; margin-le
+00001cb0: 6674 3a30 7078 3b20 6d61 7267 696e 2d72  ft:0px; margin-r
+00001cc0: 6967 6874 3a30 7078 3b20 2d71 742d 626c  ight:0px; -qt-bl
+00001cd0: 6f63 6b2d 696e 6465 6e74 3a30 3b20 7465  ock-indent:0; te
+00001ce0: 7874 2d69 6e64 656e 743a 3070 783b 2671  xt-indent:0px;&q
+00001cf0: 756f 743b 2667 743b 6e6f 2068 6120 6d75  uot;&gt;no ha mu
+00001d00: 6368 6f20 7469 656d 706f 2076 6976 6961  cho tiempo vivia
+00001d10: 2075 6e20 6869 6461 6c67 6f2e 2e26 6c74   un hidalgo..&lt
+00001d20: 3b2f 7026 6774 3b0d 0a26 6c74 3b70 2073  ;/p&gt;..&lt;p s
+00001d30: 7479 6c65 3d26 7175 6f74 3b2d 7174 2d70  tyle=&quot;-qt-p
+00001d40: 6172 6167 7261 7068 2d74 7970 653a 656d  aragraph-type:em
+00001d50: 7074 793b 206d 6172 6769 6e2d 746f 703a  pty; margin-top:
+00001d60: 3070 783b 206d 6172 6769 6e2d 626f 7474  0px; margin-bott
+00001d70: 6f6d 3a30 7078 3b20 6d61 7267 696e 2d6c  om:0px; margin-l
+00001d80: 6566 743a 3070 783b 206d 6172 6769 6e2d  eft:0px; margin-
+00001d90: 7269 6768 743a 3070 783b 202d 7174 2d62  right:0px; -qt-b
+00001da0: 6c6f 636b 2d69 6e64 656e 743a 303b 2074  lock-indent:0; t
+00001db0: 6578 742d 696e 6465 6e74 3a30 7078 3b26  ext-indent:0px;&
+00001dc0: 7175 6f74 3b26 6774 3b26 6c74 3b2f 7026  quot;&gt;&lt;/p&
+00001dd0: 6774 3b26 6c74 3b2f 7464 2667 743b 266c  gt;&lt;/td&gt;&l
+00001de0: 743b 2f74 7226 6774 3b26 6c74 3b2f 7461  t;/tr&gt;&lt;/ta
+00001df0: 626c 6526 6774 3b26 6c74 3b2f 626f 6479  ble&gt;&lt;/body
+00001e00: 2667 743b 266c 743b 2f68 746d 6c26 6774  &gt;&lt;/html&gt
+00001e10: 3b3c 2f73 7472 696e 673e 0d0a 2020 2020  ;</string>..    
+00001e20: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
+00001e30: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
+00001e40: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00001e50: 616d 653d 2274 6578 7449 6e74 6572 6163  ame="textInterac
+00001e60: 7469 6f6e 466c 6167 7322 3e0d 0a20 2020  tionFlags">..   
+00001e70: 2020 2020 2020 2020 2020 2020 3c73 6574              <set
+00001e80: 3e51 743a 3a4e 6f54 6578 7449 6e74 6572  >Qt::NoTextInter
+00001e90: 6163 7469 6f6e 3c2f 7365 743e 0d0a 2020  action</set>..  
+00001ea0: 2020 2020 2020 2020 2020 2020 3c2f 7072              </pr
+00001eb0: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00001ec0: 2020 2020 2020 3c2f 7769 6467 6574 3e0d        </widget>.
+00001ed0: 0a20 2020 2020 2020 2020 2020 203c 2f69  .            </i
+00001ee0: 7465 6d3e 0d0a 2020 2020 2020 2020 2020  tem>..          
+00001ef0: 2020 3c69 7465 6d20 726f 773d 2233 2220    <item row="3" 
+00001f00: 636f 6c75 6d6e 3d22 3022 3e0d 0a20 2020  column="0">..   
+00001f10: 2020 2020 2020 2020 2020 3c77 6964 6765            <widge
+00001f20: 7420 636c 6173 733d 2251 5075 7368 4275  t class="QPushBu
+00001f30: 7474 6f6e 2220 6e61 6d65 3d22 666f 7265  tton" name="fore
+00001f40: 6772 6f75 6e64 5042 223e 0d0a 2020 2020  groundPB">..    
+00001f50: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00001f60: 7274 7920 6e61 6d65 3d22 7768 6174 7354  rty name="whatsT
+00001f70: 6869 7322 3e0d 0a20 2020 2020 2020 2020  his">..         
+00001f80: 2020 2020 2020 3c73 7472 696e 673e 5365        <string>Se
+00001f90: 7475 7020 7468 6520 7465 7874 2063 6f6c  tup the text col
+00001fa0: 6f72 2e3c 2f73 7472 696e 673e 0d0a 2020  or.</string>..  
+00001fb0: 2020 2020 2020 2020 2020 2020 3c2f 7072              </pr
+00001fc0: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00001fd0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00001fe0: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00002000: 7472 696e 6720 636f 6d6d 656e 743d 2254  tring comment="T
+00002010: 6865 206c 6162 656c 206f 6620 7468 6520  he label of the 
+00002020: 6c6f 6767 6572 2074 6578 7420 636f 6c6f  logger text colo
+00002030: 7220 6275 7474 6f6e 223e 4626 616d 703b  r button">F&amp;
+00002040: 6f72 6567 726f 756e 643c 2f73 7472 696e  oreground</strin
+00002050: 673e 0d0a 2020 2020 2020 2020 2020 2020  g>..            
+00002060: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
+00002070: 2020 2020 2020 2020 2020 2020 3c2f 7769              </wi
+00002080: 6467 6574 3e0d 0a20 2020 2020 2020 2020  dget>..         
+00002090: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
+000020a0: 2020 2020 2020 2020 3c69 7465 6d20 726f          <item ro
+000020b0: 773d 2231 2220 636f 6c75 6d6e 3d22 3022  w="1" column="0"
+000020c0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000020d0: 3c73 7061 6365 7220 6e61 6d65 3d22 7665  <spacer name="ve
+000020e0: 7274 6963 616c 5370 6163 6572 223e 0d0a  rticalSpacer">..
+000020f0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00002100: 726f 7065 7274 7920 6e61 6d65 3d22 6f72  roperty name="or
+00002110: 6965 6e74 6174 696f 6e22 3e0d 0a20 2020  ientation">..   
+00002120: 2020 2020 2020 2020 2020 2020 3c65 6e75              <enu
+00002130: 6d3e 5174 3a3a 5665 7274 6963 616c 3c2f  m>Qt::Vertical</
+00002140: 656e 756d 3e0d 0a20 2020 2020 2020 2020  enum>..         
 00002150: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00002160: 0a20 2020 2020 2020 2020 2020 2020 3c2f  .             </
-00002170: 7370 6163 6572 3e0a 2020 2020 2020 2020  spacer>.        
-00002180: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
-00002190: 2020 2020 2020 2020 3c69 7465 6d20 726f          <item ro
-000021a0: 773d 2235 2220 636f 6c75 6d6e 3d22 3022  w="5" column="0"
-000021b0: 3e0a 2020 2020 2020 2020 2020 2020 203c  >.             <
-000021c0: 7370 6163 6572 206e 616d 653d 2276 6572  spacer name="ver
-000021d0: 7469 6361 6c53 7061 6365 725f 3222 3e0a  ticalSpacer_2">.
-000021e0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000021f0: 726f 7065 7274 7920 6e61 6d65 3d22 6f72  roperty name="or
-00002200: 6965 6e74 6174 696f 6e22 3e0a 2020 2020  ientation">.    
-00002210: 2020 2020 2020 2020 2020 203c 656e 756d             <enum
-00002220: 3e51 743a 3a56 6572 7469 6361 6c3c 2f65  >Qt::Vertical</e
-00002230: 6e75 6d3e 0a20 2020 2020 2020 2020 2020  num>.           
-00002240: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
-00002250: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00002260: 6f70 6572 7479 206e 616d 653d 2273 697a  operty name="siz
-00002270: 6548 696e 7422 2073 7464 7365 743d 2230  eHint" stdset="0
-00002280: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00002290: 2020 3c73 697a 653e 0a20 2020 2020 2020    <size>.       
-000022a0: 2020 2020 2020 2020 203c 7769 6474 683e           <width>
-000022b0: 3230 3c2f 7769 6474 683e 0a20 2020 2020  20</width>.     
-000022c0: 2020 2020 2020 2020 2020 203c 6865 6967             <heig
-000022d0: 6874 3e34 303c 2f68 6569 6768 743e 0a20  ht>40</height>. 
-000022e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000022f0: 7369 7a65 3e0a 2020 2020 2020 2020 2020  size>.          
-00002300: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00002310: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
-00002320: 7061 6365 723e 0a20 2020 2020 2020 2020  pacer>.         
-00002330: 2020 203c 2f69 7465 6d3e 0a20 2020 2020     </item>.     
-00002340: 2020 2020 2020 203c 6974 656d 2072 6f77         <item row
-00002350: 3d22 3422 2063 6f6c 756d 6e3d 2230 223e  ="4" column="0">
-00002360: 0a20 2020 2020 2020 2020 2020 2020 3c77  .             <w
-00002370: 6964 6765 7420 636c 6173 733d 2251 5075  idget class="QPu
-00002380: 7368 4275 7474 6f6e 2220 6e61 6d65 3d22  shButton" name="
-00002390: 6261 636b 6772 6f75 6e64 5042 223e 0a20  backgroundPB">. 
-000023a0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-000023b0: 6f70 6572 7479 206e 616d 653d 2277 6861  operty name="wha
-000023c0: 7473 5468 6973 223e 0a20 2020 2020 2020  tsThis">.       
-000023d0: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
-000023e0: 5365 7475 7020 7468 6520 6261 636b 6772  Setup the backgr
-000023f0: 6f75 6e64 2063 6f6c 6f72 2e3c 2f73 7472  ound color.</str
-00002400: 696e 673e 0a20 2020 2020 2020 2020 2020  ing>.           
-00002410: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
-00002420: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00002430: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
-00002440: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-00002450: 2020 203c 7374 7269 6e67 2063 6f6d 6d65     <string comme
-00002460: 6e74 3d22 5468 6520 6c61 6265 6c20 6f66  nt="The label of
-00002470: 2074 6865 206c 6f67 6765 7220 636f 6c6f   the logger colo
-00002480: 7220 6275 7474 6f6e 223e 2661 6d70 3b42  r button">&amp;B
-00002490: 6163 6b67 726f 756e 643c 2f73 7472 696e  ackground</strin
-000024a0: 673e 0a20 2020 2020 2020 2020 2020 2020  g>.             
-000024b0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-000024c0: 2020 2020 2020 2020 2020 3c2f 7769 6467            </widg
-000024d0: 6574 3e0a 2020 2020 2020 2020 2020 2020  et>.            
-000024e0: 3c2f 6974 656d 3e0a 2020 2020 2020 2020  </item>.        
-000024f0: 2020 2020 3c69 7465 6d20 726f 773d 2232      <item row="2
-00002500: 2220 636f 6c75 6d6e 3d22 3022 3e0a 2020  " column="0">.  
-00002510: 2020 2020 2020 2020 2020 203c 7769 6467             <widg
-00002520: 6574 2063 6c61 7373 3d22 5150 7573 6842  et class="QPushB
-00002530: 7574 746f 6e22 206e 616d 653d 2266 6f6e  utton" name="fon
-00002540: 7450 4222 3e0a 2020 2020 2020 2020 2020  tPB">.          
-00002550: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00002560: 6d65 3d22 7768 6174 7354 6869 7322 3e0a  me="whatsThis">.
-00002570: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002580: 7374 7269 6e67 3e48 6572 6520 796f 7520  string>Here you 
-00002590: 6361 6e20 6368 6f6f 7365 2074 6865 2066  can choose the f
-000025a0: 6f6e 7420 7573 6564 2069 6e20 7468 6520  ont used in the 
-000025b0: 4c6f 6767 6572 2e3c 2f73 7472 696e 673e  Logger.</string>
-000025c0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-000025d0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-000025e0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-000025f0: 7479 206e 616d 653d 2274 6578 7422 3e0a  ty name="text">.
-00002600: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002610: 7374 7269 6e67 2063 6f6d 6d65 6e74 3d22  string comment="
-00002620: 5468 6520 6c61 6265 6c20 6f66 2074 6865  The label of the
-00002630: 206c 6f67 6765 7220 666f 6e74 2063 686f   logger font cho
-00002640: 6f73 6572 2062 7574 746f 6e22 3e26 616d  oser button">&am
-00002650: 703b 466f 6e74 3c2f 7374 7269 6e67 3e0a  p;Font</string>.
-00002660: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00002670: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00002680: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
-00002690: 0a20 2020 2020 2020 2020 2020 203c 2f69  .            </i
-000026a0: 7465 6d3e 0a20 2020 2020 2020 2020 2020  tem>.           
-000026b0: 3c2f 6c61 796f 7574 3e0a 2020 2020 2020  </layout>.      
-000026c0: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
-000026d0: 2020 2020 2020 203c 2f69 7465 6d3e 0a20         </item>. 
-000026e0: 2020 2020 2020 2020 3c69 7465 6d3e 0a20          <item>. 
-000026f0: 2020 2020 2020 2020 203c 7769 6467 6574           <widget
-00002700: 2063 6c61 7373 3d22 5147 726f 7570 426f   class="QGroupBo
-00002710: 7822 206e 616d 653d 2277 6f72 6b73 7061  x" name="workspa
-00002720: 6365 4742 223e 0a20 2020 2020 2020 2020  ceGB">.         
-00002730: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00002740: 3d22 7768 6174 7354 6869 7322 3e0a 2020  ="whatsThis">.  
-00002750: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
-00002760: 673e 5365 7475 7020 7468 6520 6261 636b  g>Setup the back
-00002770: 6772 6f75 6e64 2063 6f6c 6f72 206f 6620  ground color of 
-00002780: 7468 6520 776f 726b 7370 6163 652e 3c2f  the workspace.</
-00002790: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
-000027a0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
-000027b0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-000027c0: 7274 7920 6e61 6d65 3d22 7469 746c 6522  rty name="title"
-000027d0: 3e0a 2020 2020 2020 2020 2020 2020 3c73  >.            <s
-000027e0: 7472 696e 6720 636f 6d6d 656e 743d 2254  tring comment="T
-000027f0: 6865 2074 6974 6c65 206f 6620 7468 6520  he title of the 
-00002800: 776f 726b 7370 6163 6520 6772 6f75 7062  workspace groupb
-00002810: 6f78 223e 576f 726b 7370 6163 653c 2f73  ox">Workspace</s
-00002820: 7472 696e 673e 0a20 2020 2020 2020 2020  tring>.         
-00002830: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
-00002840: 2020 2020 2020 2020 203c 6c61 796f 7574           <layout
-00002850: 2063 6c61 7373 3d22 5148 426f 784c 6179   class="QHBoxLay
-00002860: 6f75 7422 206e 616d 653d 2268 6f72 697a  out" name="horiz
-00002870: 6f6e 7461 6c4c 6179 6f75 745f 3222 3e0a  ontalLayout_2">.
-00002880: 2020 2020 2020 2020 2020 2020 3c69 7465              <ite
-00002890: 6d3e 0a20 2020 2020 2020 2020 2020 2020  m>.             
-000028a0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-000028b0: 5075 7368 4275 7474 6f6e 2220 6e61 6d65  PushButton" name
-000028c0: 3d22 776f 726b 7370 6163 6550 4222 3e0a  ="workspacePB">.
-000028d0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000028e0: 726f 7065 7274 7920 6e61 6d65 3d22 7768  roperty name="wh
-000028f0: 6174 7354 6869 7322 3e0a 2020 2020 2020  atsThis">.      
-00002900: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00002910: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00002920: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-00002930: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00002940: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
-00002950: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002960: 203c 7374 7269 6e67 2063 6f6d 6d65 6e74   <string comment
-00002970: 3d22 5468 6520 6c61 6265 6c20 6f66 2074  ="The label of t
-00002980: 6865 2077 6f72 6b73 7061 6365 2063 6f6c  he workspace col
-00002990: 6f72 2062 7574 746f 6e22 3e26 616d 703b  or button">&amp;
-000029a0: 4261 636b 6772 6f75 6e64 3c2f 7374 7269  Background</stri
-000029b0: 6e67 3e0a 2020 2020 2020 2020 2020 2020  ng>.            
-000029c0: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
-000029d0: 2020 2020 2020 2020 2020 203c 2f77 6964             </wid
-000029e0: 6765 743e 0a20 2020 2020 2020 2020 2020  get>.           
-000029f0: 203c 2f69 7465 6d3e 0a20 2020 2020 2020   </item>.       
-00002a00: 2020 2020 203c 6974 656d 3e0a 2020 2020       <item>.    
-00002a10: 2020 2020 2020 2020 203c 7769 6467 6574           <widget
-00002a20: 2063 6c61 7373 3d22 514c 6162 656c 2220   class="QLabel" 
-00002a30: 6e61 6d65 3d22 776f 726b 7370 6163 654c  name="workspaceL
-00002a40: 6162 656c 223e 0a20 2020 2020 2020 2020  abel">.         
-00002a50: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00002a60: 616d 653d 2261 7574 6f46 696c 6c42 6163  ame="autoFillBac
-00002a70: 6b67 726f 756e 6422 3e0a 2020 2020 2020  kground">.      
-00002a80: 2020 2020 2020 2020 203c 626f 6f6c 3e74           <bool>t
-00002a90: 7275 653c 2f62 6f6f 6c3e 0a20 2020 2020  rue</bool>.     
-00002aa0: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
-00002ab0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00002ac0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002ad0: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
-00002ae0: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00002af0: 2063 6f6d 6d65 6e74 3d22 4120 6c61 6265   comment="A labe
-00002b00: 6c20 666f 7220 7468 6520 776f 726b 7370  l for the worksp
-00002b10: 6163 6520 636f 6c6f 7220 7361 6d70 6c65  ace color sample
-00002b20: 223e 4261 636b 6772 6f75 6e64 2063 6f6c  ">Background col
-00002b30: 6f72 2073 616d 706c 653c 2f73 7472 696e  or sample</strin
-00002b40: 673e 0a20 2020 2020 2020 2020 2020 2020  g>.             
-00002b50: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
-00002b60: 2020 2020 2020 2020 2020 3c2f 7769 6467            </widg
-00002b70: 6574 3e0a 2020 2020 2020 2020 2020 2020  et>.            
-00002b80: 3c2f 6974 656d 3e0a 2020 2020 2020 2020  </item>.        
-00002b90: 2020 203c 2f6c 6179 6f75 743e 0a20 2020     </layout>.   
-00002ba0: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
-00002bb0: 0a20 2020 2020 2020 2020 3c2f 6974 656d  .         </item
-00002bc0: 3e0a 2020 2020 2020 2020 203c 6974 656d  >.         <item
-00002bd0: 3e0a 2020 2020 2020 2020 2020 3c77 6964  >.          <wid
-00002be0: 6765 7420 636c 6173 733d 2251 4772 6f75  get class="QGrou
-00002bf0: 7042 6f78 2220 6e61 6d65 3d22 7374 796c  pBox" name="styl
-00002c00: 6547 4222 3e0a 2020 2020 2020 2020 2020  eGB">.          
-00002c10: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00002c20: 2277 6861 7473 5468 6973 223e 0a20 2020  "whatsThis">.   
-00002c30: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00002c40: 3e43 686f 6f73 6520 7468 6520 676c 6f62  >Choose the glob
-00002c50: 616c 2073 7479 6c65 206f 6620 5669 5461  al style of ViTa
-00002c60: 626c 6573 2068 6572 652e 3c2f 7374 7269  bles here.</stri
-00002c70: 6e67 3e0a 2020 2020 2020 2020 2020 203c  ng>.           <
-00002c80: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00002c90: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00002ca0: 6e61 6d65 3d22 7469 746c 6522 3e0a 2020  name="title">.  
-00002cb0: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
-00002cc0: 6720 636f 6d6d 656e 743d 2254 6865 2074  g comment="The t
-00002cd0: 6974 6c65 206f 6620 7468 6520 676c 6f62  itle of the glob
-00002ce0: 616c 2061 7370 6563 7420 6772 6f75 7062  al aspect groupb
-00002cf0: 6f78 223e 5374 796c 653c 2f73 7472 696e  ox">Style</strin
-00002d00: 673e 0a20 2020 2020 2020 2020 2020 3c2f  g>.           </
-00002d10: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00002d20: 2020 2020 203c 6c61 796f 7574 2063 6c61       <layout cla
-00002d30: 7373 3d22 5156 426f 784c 6179 6f75 7422  ss="QVBoxLayout"
-00002d40: 206e 616d 653d 2276 6572 7469 6361 6c4c   name="verticalL
-00002d50: 6179 6f75 745f 3422 3e0a 2020 2020 2020  ayout_4">.      
-00002d60: 2020 2020 2020 3c69 7465 6d3e 0a20 2020        <item>.   
-00002d70: 2020 2020 2020 2020 2020 3c77 6964 6765            <widge
-00002d80: 7420 636c 6173 733d 2251 436f 6d62 6f42  t class="QComboB
-00002d90: 6f78 2220 6e61 6d65 3d22 7374 796c 6573  ox" name="styles
-00002da0: 4342 223e 0a20 2020 2020 2020 2020 2020  CB">.           
-00002db0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002dc0: 653d 2277 6861 7473 5468 6973 223e 0a20  e="whatsThis">. 
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00002de0: 7472 696e 672f 3e0a 2020 2020 2020 2020  tring/>.        
-00002df0: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00002e00: 3e0a 2020 2020 2020 2020 2020 2020 203c  >.             <
-00002e10: 2f77 6964 6765 743e 0a20 2020 2020 2020  /widget>.       
-00002e20: 2020 2020 203c 2f69 7465 6d3e 0a20 2020       </item>.   
-00002e30: 2020 2020 2020 2020 3c2f 6c61 796f 7574          </layout
-00002e40: 3e0a 2020 2020 2020 2020 2020 3c2f 7769  >.          </wi
-00002e50: 6467 6574 3e0a 2020 2020 2020 2020 203c  dget>.         <
-00002e60: 2f69 7465 6d3e 0a20 2020 2020 2020 203c  /item>.        <
-00002e70: 2f6c 6179 6f75 743e 0a20 2020 2020 2020  /layout>.       
-00002e80: 3c2f 7769 6467 6574 3e0a 2020 2020 2020  </widget>.      
-00002e90: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
-00002ea0: 5157 6964 6765 7422 206e 616d 653d 2270  QWidget" name="p
-00002eb0: 6c75 6769 6e73 5061 6765 223e 0a20 2020  luginsPage">.   
-00002ec0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00002ed0: 616d 653d 2273 697a 6550 6f6c 6963 7922  ame="sizePolicy"
-00002ee0: 3e0a 2020 2020 2020 2020 203c 7369 7a65  >.         <size
-00002ef0: 706f 6c69 6379 2068 7369 7a65 7479 7065  policy hsizetype
-00002f00: 3d22 4578 7061 6e64 696e 6722 2076 7369  ="Expanding" vsi
-00002f10: 7a65 7479 7065 3d22 5072 6566 6572 7265  zetype="Preferre
-00002f20: 6422 3e0a 2020 2020 2020 2020 2020 3c68  d">.          <h
-00002f30: 6f72 7374 7265 7463 683e 303c 2f68 6f72  orstretch>0</hor
-00002f40: 7374 7265 7463 683e 0a20 2020 2020 2020  stretch>.       
-00002f50: 2020 203c 7665 7273 7472 6574 6368 3e30     <verstretch>0
-00002f60: 3c2f 7665 7273 7472 6574 6368 3e0a 2020  </verstretch>.  
-00002f70: 2020 2020 2020 203c 2f73 697a 6570 6f6c         </sizepol
-00002f80: 6963 793e 0a20 2020 2020 2020 203c 2f70  icy>.        </p
-00002f90: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00002fa0: 203c 6c61 796f 7574 2063 6c61 7373 3d22   <layout class="
-00002fb0: 5156 426f 784c 6179 6f75 7422 206e 616d  QVBoxLayout" nam
-00002fc0: 653d 2276 6572 7469 6361 6c4c 6179 6f75  e="verticalLayou
-00002fd0: 745f 3922 3e0a 2020 2020 2020 2020 203c  t_9">.         <
-00002fe0: 6974 656d 3e0a 2020 2020 2020 2020 2020  item>.          
-00002ff0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-00003000: 4772 6f75 7042 6f78 2220 6e61 6d65 3d22  GroupBox" name="
-00003010: 666f 6c64 6572 7347 4222 3e0a 2020 2020  foldersGB">.    
-00003020: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00003030: 206e 616d 653d 2277 6861 7473 5468 6973   name="whatsThis
-00003040: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-00003050: 7374 7269 6e67 2f3e 0a20 2020 2020 2020  string/>.       
-00003060: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00003070: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00003080: 6572 7479 206e 616d 653d 2274 6974 6c65  erty name="title
-00003090: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-000030a0: 7374 7269 6e67 3e41 7661 696c 6162 6c65  string>Available
-000030b0: 2070 6c75 6769 6e73 3c2f 7374 7269 6e67   plugins</string
-000030c0: 3e0a 2020 2020 2020 2020 2020 203c 2f70  >.           </p
-000030d0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-000030e0: 2020 2020 3c6c 6179 6f75 7420 636c 6173      <layout clas
-000030f0: 733d 2251 5642 6f78 4c61 796f 7574 2220  s="QVBoxLayout" 
-00003100: 6e61 6d65 3d22 7665 7274 6963 616c 4c61  name="verticalLa
-00003110: 796f 7574 5f36 223e 0a20 2020 2020 2020  yout_6">.       
-00003120: 2020 2020 203c 6974 656d 3e0a 2020 2020       <item>.    
-00003130: 2020 2020 2020 2020 203c 7769 6467 6574           <widget
-00003140: 2063 6c61 7373 3d22 5154 7265 6556 6965   class="QTreeVie
-00003150: 7722 206e 616d 653d 2270 6c75 6769 6e73  w" name="plugins
-00003160: 5456 223e 0a20 2020 2020 2020 2020 2020  TV">.           
-00003170: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00003180: 653d 2273 697a 6550 6f6c 6963 7922 3e0a  e="sizePolicy">.
-00003190: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000031a0: 7369 7a65 706f 6c69 6379 2068 7369 7a65  sizepolicy hsize
-000031b0: 7479 7065 3d22 5072 6566 6572 7265 6422  type="Preferred"
-000031c0: 2076 7369 7a65 7479 7065 3d22 5072 6566   vsizetype="Pref
-000031d0: 6572 7265 6422 3e0a 2020 2020 2020 2020  erred">.        
-000031e0: 2020 2020 2020 2020 3c68 6f72 7374 7265          <horstre
-000031f0: 7463 683e 303c 2f68 6f72 7374 7265 7463  tch>0</horstretc
-00003200: 683e 0a20 2020 2020 2020 2020 2020 2020  h>.             
-00003210: 2020 203c 7665 7273 7472 6574 6368 3e30     <verstretch>0
-00003220: 3c2f 7665 7273 7472 6574 6368 3e0a 2020  </verstretch>.  
-00003230: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
-00003240: 697a 6570 6f6c 6963 793e 0a20 2020 2020  izepolicy>.     
-00003250: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
-00003260: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00003270: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00003280: 653d 2277 6861 7473 5468 6973 223e 0a20  e="whatsThis">. 
-00003290: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-000032a0: 7472 696e 673e 5468 6520 6c69 7374 206f  tring>The list o
-000032b0: 6620 616c 6c20 6176 6169 6c61 626c 6520  f all available 
-000032c0: 706c 7567 696e 732e 2049 6620 6120 706c  plugins. If a pl
-000032d0: 7567 696e 2069 7320 6368 6563 6b65 6420  ugin is checked 
-000032e0: 7468 656e 2069 7420 6973 2065 6e61 626c  then it is enabl
-000032f0: 6564 2028 6275 7420 6e6f 7420 6e65 6365  ed (but not nece
-00003300: 7373 6172 656c 7920 6c6f 6164 6564 292c  ssarely loaded),
-00003310: 2069 6620 6974 2069 7320 756e 6368 6563   if it is unchec
-00003320: 6b65 6420 7468 656e 2069 7420 6973 2064  ked then it is d
-00003330: 6973 6162 6c65 6420 2862 7574 206e 6f74  isabled (but not
-00003340: 206e 6563 6573 7361 7265 6c79 2075 6e6c   necessarely unl
-00003350: 6f61 6465 6429 2e20 506c 6561 7365 2c20  oaded). Please, 
-00003360: 6e6f 7465 2074 6861 7420 6368 616e 6765  note that change
-00003370: 7320 696e 2074 6865 2063 6865 636b 2073  s in the check s
-00003380: 7461 7465 206f 6620 706c 7567 696e 7320  tate of plugins 
-00003390: 7769 6c6c 2074 616b 6520 6566 6665 6374  will take effect
-000033a0: 2074 6865 206e 6578 7420 7469 6d65 2079   the next time y
-000033b0: 6f75 2073 7461 7274 2056 6954 6162 6c65  ou start ViTable
-000033c0: 732e 3c2f 7374 7269 6e67 3e0a 2020 2020  s.</string>.    
-000033d0: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
-000033e0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-000033f0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00003400: 6d65 3d22 6564 6974 5472 6967 6765 7273  me="editTriggers
-00003410: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00003420: 2020 3c73 6574 3e51 4162 7374 7261 6374    <set>QAbstract
-00003430: 4974 656d 5669 6577 3a3a 4e6f 4564 6974  ItemView::NoEdit
-00003440: 5472 6967 6765 7273 3c2f 7365 743e 0a20  Triggers</set>. 
-00003450: 2020 2020 2020 2020 2020 2020 203c 2f70               </p
-00003460: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00003470: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00003480: 206e 616d 653d 2272 6f6f 7449 7344 6563   name="rootIsDec
-00003490: 6f72 6174 6564 223e 0a20 2020 2020 2020  orated">.       
-000034a0: 2020 2020 2020 2020 3c62 6f6f 6c3e 6661          <bool>fa
-000034b0: 6c73 653c 2f62 6f6f 6c3e 0a20 2020 2020  lse</bool>.     
-000034c0: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
-000034d0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-000034e0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000034f0: 653d 2265 7870 616e 6473 4f6e 446f 7562  e="expandsOnDoub
-00003500: 6c65 436c 6963 6b22 3e0a 2020 2020 2020  leClick">.      
-00003510: 2020 2020 2020 2020 203c 626f 6f6c 3e66           <bool>f
-00003520: 616c 7365 3c2f 626f 6f6c 3e0a 2020 2020  alse</bool>.    
-00003530: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
-00003540: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00003550: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
-00003560: 2020 2020 2020 2020 203c 2f69 7465 6d3e           </item>
-00003570: 0a20 2020 2020 2020 2020 2020 3c2f 6c61  .           </la
-00003580: 796f 7574 3e0a 2020 2020 2020 2020 2020  yout>.          
-00003590: 3c2f 7769 6467 6574 3e0a 2020 2020 2020  </widget>.      
-000035a0: 2020 203c 2f69 7465 6d3e 0a20 2020 2020     </item>.     
-000035b0: 2020 203c 2f6c 6179 6f75 743e 0a20 2020     </layout>.   
-000035c0: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
-000035d0: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
-000035e0: 2020 203c 2f69 7465 6d3e 0a20 2020 203c     </item>.    <
-000035f0: 2f6c 6179 6f75 743e 0a20 2020 3c2f 6974  /layout>.   </it
-00003600: 656d 3e0a 2020 203c 6974 656d 3e0a 2020  em>.   <item>.  
-00003610: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-00003620: 2251 4469 616c 6f67 4275 7474 6f6e 426f  "QDialogButtonBo
-00003630: 7822 206e 616d 653d 2262 7574 746f 6e73  x" name="buttons
-00003640: 426f 7822 3e0a 2020 2020 203c 7072 6f70  Box">.     <prop
-00003650: 6572 7479 206e 616d 653d 226f 7269 656e  erty name="orien
-00003660: 7461 7469 6f6e 223e 0a20 2020 2020 203c  tation">.      <
-00003670: 656e 756d 3e51 743a 3a48 6f72 697a 6f6e  enum>Qt::Horizon
-00003680: 7461 6c3c 2f65 6e75 6d3e 0a20 2020 2020  tal</enum>.     
-00003690: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-000036a0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000036b0: 2273 7461 6e64 6172 6442 7574 746f 6e73  "standardButtons
-000036c0: 223e 0a20 2020 2020 203c 7365 743e 5144  ">.      <set>QD
-000036d0: 6961 6c6f 6742 7574 746f 6e42 6f78 3a3a  ialogButtonBox::
-000036e0: 4361 6e63 656c 7c51 4469 616c 6f67 4275  Cancel|QDialogBu
-000036f0: 7474 6f6e 426f 783a 3a48 656c 707c 5144  ttonBox::Help|QD
-00003700: 6961 6c6f 6742 7574 746f 6e42 6f78 3a3a  ialogButtonBox::
-00003710: 4f6b 7c51 4469 616c 6f67 4275 7474 6f6e  Ok|QDialogButton
-00003720: 426f 783a 3a52 6573 6574 3c2f 7365 743e  Box::Reset</set>
-00003730: 0a20 2020 2020 3c2f 7072 6f70 6572 7479  .     </property
-00003740: 3e0a 2020 2020 3c2f 7769 6467 6574 3e0a  >.    </widget>.
-00003750: 2020 203c 2f69 7465 6d3e 0a20 203c 2f6c     </item>.  </l
-00003760: 6179 6f75 743e 0a20 3c2f 7769 6467 6574  ayout>. </widget
-00003770: 3e0a 203c 7265 736f 7572 6365 732f 3e0a  >. <resources/>.
-00003780: 203c 636f 6e6e 6563 7469 6f6e 732f 3e0a   <connections/>.
-00003790: 3c2f 7569 3e0a                           </ui>.
+00002160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002170: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00002180: 7369 7a65 4869 6e74 2220 7374 6473 6574  sizeHint" stdset
+00002190: 3d22 3022 3e0d 0a20 2020 2020 2020 2020  ="0">..         
+000021a0: 2020 2020 2020 3c73 697a 653e 0d0a 2020        <size>..  
+000021b0: 2020 2020 2020 2020 2020 2020 2020 3c77                <w
+000021c0: 6964 7468 3e32 303c 2f77 6964 7468 3e0d  idth>20</width>.
+000021d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021e0: 203c 6865 6967 6874 3e34 303c 2f68 6569   <height>40</hei
+000021f0: 6768 743e 0d0a 2020 2020 2020 2020 2020  ght>..          
+00002200: 2020 2020 203c 2f73 697a 653e 0d0a 2020       </size>..  
+00002210: 2020 2020 2020 2020 2020 2020 3c2f 7072              </pr
+00002220: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00002230: 2020 2020 2020 3c2f 7370 6163 6572 3e0d        </spacer>.
+00002240: 0a20 2020 2020 2020 2020 2020 203c 2f69  .            </i
+00002250: 7465 6d3e 0d0a 2020 2020 2020 2020 2020  tem>..          
+00002260: 2020 3c69 7465 6d20 726f 773d 2235 2220    <item row="5" 
+00002270: 636f 6c75 6d6e 3d22 3022 3e0d 0a20 2020  column="0">..   
+00002280: 2020 2020 2020 2020 2020 3c73 7061 6365            <space
+00002290: 7220 6e61 6d65 3d22 7665 7274 6963 616c  r name="vertical
+000022a0: 5370 6163 6572 5f32 223e 0d0a 2020 2020  Spacer_2">..    
+000022b0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+000022c0: 7274 7920 6e61 6d65 3d22 6f72 6965 6e74  rty name="orient
+000022d0: 6174 696f 6e22 3e0d 0a20 2020 2020 2020  ation">..       
+000022e0: 2020 2020 2020 2020 3c65 6e75 6d3e 5174          <enum>Qt
+000022f0: 3a3a 5665 7274 6963 616c 3c2f 656e 756d  ::Vertical</enum
+00002300: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002310: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
+00002320: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00002330: 7065 7274 7920 6e61 6d65 3d22 7369 7a65  perty name="size
+00002340: 4869 6e74 2220 7374 6473 6574 3d22 3022  Hint" stdset="0"
+00002350: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002360: 2020 3c73 697a 653e 0d0a 2020 2020 2020    <size>..      
+00002370: 2020 2020 2020 2020 2020 3c77 6964 7468            <width
+00002380: 3e32 303c 2f77 6964 7468 3e0d 0a20 2020  >20</width>..   
+00002390: 2020 2020 2020 2020 2020 2020 203c 6865               <he
+000023a0: 6967 6874 3e34 303c 2f68 6569 6768 743e  ight>40</height>
+000023b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000023c0: 203c 2f73 697a 653e 0d0a 2020 2020 2020   </size>..      
+000023d0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+000023e0: 7479 3e0d 0a20 2020 2020 2020 2020 2020  ty>..           
+000023f0: 2020 3c2f 7370 6163 6572 3e0d 0a20 2020    </spacer>..   
+00002400: 2020 2020 2020 2020 203c 2f69 7465 6d3e           </item>
+00002410: 0d0a 2020 2020 2020 2020 2020 2020 3c69  ..            <i
+00002420: 7465 6d20 726f 773d 2234 2220 636f 6c75  tem row="4" colu
+00002430: 6d6e 3d22 3022 3e0d 0a20 2020 2020 2020  mn="0">..       
+00002440: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
+00002450: 6173 733d 2251 5075 7368 4275 7474 6f6e  ass="QPushButton
+00002460: 2220 6e61 6d65 3d22 6261 636b 6772 6f75  " name="backgrou
+00002470: 6e64 5042 223e 0d0a 2020 2020 2020 2020  ndPB">..        
+00002480: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00002490: 6e61 6d65 3d22 7768 6174 7354 6869 7322  name="whatsThis"
+000024a0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+000024b0: 2020 3c73 7472 696e 673e 5365 7475 7020    <string>Setup 
+000024c0: 7468 6520 6261 636b 6772 6f75 6e64 2063  the background c
+000024d0: 6f6c 6f72 2e3c 2f73 7472 696e 673e 0d0a  olor.</string>..
+000024e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000024f0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
+00002500: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00002510: 7479 206e 616d 653d 2274 6578 7422 3e0d  ty name="text">.
+00002520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002530: 3c73 7472 696e 6720 636f 6d6d 656e 743d  <string comment=
+00002540: 2254 6865 206c 6162 656c 206f 6620 7468  "The label of th
+00002550: 6520 6c6f 6767 6572 2063 6f6c 6f72 2062  e logger color b
+00002560: 7574 746f 6e22 3e26 616d 703b 4261 636b  utton">&amp;Back
+00002570: 6772 6f75 6e64 3c2f 7374 7269 6e67 3e0d  ground</string>.
+00002580: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00002590: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
+000025a0: 2020 2020 2020 2020 203c 2f77 6964 6765           </widge
+000025b0: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
+000025c0: 3c2f 6974 656d 3e0d 0a20 2020 2020 2020  </item>..       
+000025d0: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
+000025e0: 3222 2063 6f6c 756d 6e3d 2230 223e 0d0a  2" column="0">..
+000025f0: 2020 2020 2020 2020 2020 2020 203c 7769               <wi
+00002600: 6467 6574 2063 6c61 7373 3d22 5150 7573  dget class="QPus
+00002610: 6842 7574 746f 6e22 206e 616d 653d 2266  hButton" name="f
+00002620: 6f6e 7450 4222 3e0d 0a20 2020 2020 2020  ontPB">..       
+00002630: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00002640: 206e 616d 653d 2277 6861 7473 5468 6973   name="whatsThis
+00002650: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00002660: 2020 203c 7374 7269 6e67 3e48 6572 6520     <string>Here 
+00002670: 796f 7520 6361 6e20 6368 6f6f 7365 2074  you can choose t
+00002680: 6865 2066 6f6e 7420 7573 6564 2069 6e20  he font used in 
+00002690: 7468 6520 4c6f 6767 6572 2e3c 2f73 7472  the Logger.</str
+000026a0: 696e 673e 0d0a 2020 2020 2020 2020 2020  ing>..          
+000026b0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
+000026c0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+000026d0: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+000026e0: 6578 7422 3e0d 0a20 2020 2020 2020 2020  ext">..         
+000026f0: 2020 2020 2020 3c73 7472 696e 6720 636f        <string co
+00002700: 6d6d 656e 743d 2254 6865 206c 6162 656c  mment="The label
+00002710: 206f 6620 7468 6520 6c6f 6767 6572 2066   of the logger f
+00002720: 6f6e 7420 6368 6f6f 7365 7220 6275 7474  ont chooser butt
+00002730: 6f6e 223e 2661 6d70 3b46 6f6e 743c 2f73  on">&amp;Font</s
+00002740: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
+00002750: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00002760: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002770: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
+00002780: 2020 2020 2020 203c 2f69 7465 6d3e 0d0a         </item>..
+00002790: 2020 2020 2020 2020 2020 203c 2f6c 6179             </lay
+000027a0: 6f75 743e 0d0a 2020 2020 2020 2020 2020  out>..          
+000027b0: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
+000027c0: 2020 2020 3c2f 6974 656d 3e0d 0a20 2020      </item>..   
+000027d0: 2020 2020 2020 3c69 7465 6d3e 0d0a 2020        <item>..  
+000027e0: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
+000027f0: 636c 6173 733d 2251 4772 6f75 7042 6f78  class="QGroupBox
+00002800: 2220 6e61 6d65 3d22 776f 726b 7370 6163  " name="workspac
+00002810: 6547 4222 3e0d 0a20 2020 2020 2020 2020  eGB">..         
+00002820: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00002830: 3d22 7768 6174 7354 6869 7322 3e0d 0a20  ="whatsThis">.. 
+00002840: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
+00002850: 6e67 3e53 6574 7570 2074 6865 2062 6163  ng>Setup the bac
+00002860: 6b67 726f 756e 6420 636f 6c6f 7220 6f66  kground color of
+00002870: 2074 6865 2077 6f72 6b73 7061 6365 2e3c   the workspace.<
+00002880: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
+00002890: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+000028a0: 0d0a 2020 2020 2020 2020 2020 203c 7072  ..           <pr
+000028b0: 6f70 6572 7479 206e 616d 653d 2274 6974  operty name="tit
+000028c0: 6c65 223e 0d0a 2020 2020 2020 2020 2020  le">..          
+000028d0: 2020 3c73 7472 696e 6720 636f 6d6d 656e    <string commen
+000028e0: 743d 2254 6865 2074 6974 6c65 206f 6620  t="The title of 
+000028f0: 7468 6520 776f 726b 7370 6163 6520 6772  the workspace gr
+00002900: 6f75 7062 6f78 223e 576f 726b 7370 6163  oupbox">Workspac
+00002910: 653c 2f73 7472 696e 673e 0d0a 2020 2020  e</string>..    
+00002920: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00002930: 793e 0d0a 2020 2020 2020 2020 2020 203c  y>..           <
+00002940: 6c61 796f 7574 2063 6c61 7373 3d22 5148  layout class="QH
+00002950: 426f 784c 6179 6f75 7422 206e 616d 653d  BoxLayout" name=
+00002960: 2268 6f72 697a 6f6e 7461 6c4c 6179 6f75  "horizontalLayou
+00002970: 745f 3222 3e0d 0a20 2020 2020 2020 2020  t_2">..         
+00002980: 2020 203c 6974 656d 3e0d 0a20 2020 2020     <item>..     
+00002990: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
+000029a0: 636c 6173 733d 2251 5075 7368 4275 7474  class="QPushButt
+000029b0: 6f6e 2220 6e61 6d65 3d22 776f 726b 7370  on" name="worksp
+000029c0: 6163 6550 4222 3e0d 0a20 2020 2020 2020  acePB">..       
+000029d0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000029e0: 206e 616d 653d 2277 6861 7473 5468 6973   name="whatsThis
+000029f0: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00002a00: 2020 203c 7374 7269 6e67 2f3e 0d0a 2020     <string/>..  
+00002a10: 2020 2020 2020 2020 2020 2020 3c2f 7072              </pr
+00002a20: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
+00002a30: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00002a40: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
+00002a50: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00002a60: 7472 696e 6720 636f 6d6d 656e 743d 2254  tring comment="T
+00002a70: 6865 206c 6162 656c 206f 6620 7468 6520  he label of the 
+00002a80: 776f 726b 7370 6163 6520 636f 6c6f 7220  workspace color 
+00002a90: 6275 7474 6f6e 223e 2661 6d70 3b42 6163  button">&amp;Bac
+00002aa0: 6b67 726f 756e 643c 2f73 7472 696e 673e  kground</string>
+00002ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002ac0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
+00002ad0: 2020 2020 2020 2020 2020 3c2f 7769 6467            </widg
+00002ae0: 6574 3e0d 0a20 2020 2020 2020 2020 2020  et>..           
+00002af0: 203c 2f69 7465 6d3e 0d0a 2020 2020 2020   </item>..      
+00002b00: 2020 2020 2020 3c69 7465 6d3e 0d0a 2020        <item>..  
+00002b10: 2020 2020 2020 2020 2020 203c 7769 6467             <widg
+00002b20: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
+00002b30: 2220 6e61 6d65 3d22 776f 726b 7370 6163  " name="workspac
+00002b40: 654c 6162 656c 223e 0d0a 2020 2020 2020  eLabel">..      
+00002b50: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00002b60: 7920 6e61 6d65 3d22 6175 746f 4669 6c6c  y name="autoFill
+00002b70: 4261 636b 6772 6f75 6e64 223e 0d0a 2020  Background">..  
+00002b80: 2020 2020 2020 2020 2020 2020 203c 626f               <bo
+00002b90: 6f6c 3e74 7275 653c 2f62 6f6f 6c3e 0d0a  ol>true</bool>..
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002bb0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
+00002bc0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00002bd0: 7479 206e 616d 653d 2274 6578 7422 3e0d  ty name="text">.
+00002be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002bf0: 3c73 7472 696e 6720 636f 6d6d 656e 743d  <string comment=
+00002c00: 2241 206c 6162 656c 2066 6f72 2074 6865  "A label for the
+00002c10: 2077 6f72 6b73 7061 6365 2063 6f6c 6f72   workspace color
+00002c20: 2073 616d 706c 6522 3e42 6163 6b67 726f   sample">Backgro
+00002c30: 756e 6420 636f 6c6f 7220 7361 6d70 6c65  und color sample
+00002c40: 3c2f 7374 7269 6e67 3e0d 0a20 2020 2020  </string>..     
+00002c50: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
+00002c60: 7274 793e 0d0a 2020 2020 2020 2020 2020  rty>..          
+00002c70: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
+00002c80: 2020 2020 2020 2020 2020 3c2f 6974 656d            </item
+00002c90: 3e0d 0a20 2020 2020 2020 2020 2020 3c2f  >..           </
+00002ca0: 6c61 796f 7574 3e0d 0a20 2020 2020 2020  layout>..       
+00002cb0: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
+00002cc0: 2020 2020 2020 203c 2f69 7465 6d3e 0d0a         </item>..
+00002cd0: 2020 2020 2020 2020 203c 6974 656d 3e0d           <item>.
+00002ce0: 0a20 2020 2020 2020 2020 203c 7769 6467  .          <widg
+00002cf0: 6574 2063 6c61 7373 3d22 5147 726f 7570  et class="QGroup
+00002d00: 426f 7822 206e 616d 653d 2273 7479 6c65  Box" name="style
+00002d10: 4742 223e 0d0a 2020 2020 2020 2020 2020  GB">..          
+00002d20: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00002d30: 2277 6861 7473 5468 6973 223e 0d0a 2020  "whatsThis">..  
+00002d40: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
+00002d50: 673e 4368 6f6f 7365 2074 6865 2067 6c6f  g>Choose the glo
+00002d60: 6261 6c20 7374 796c 6520 6f66 2056 6954  bal style of ViT
+00002d70: 6162 6c65 7320 6865 7265 2e3c 2f73 7472  ables here.</str
+00002d80: 696e 673e 0d0a 2020 2020 2020 2020 2020  ing>..          
+00002d90: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
+00002da0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00002db0: 7479 206e 616d 653d 2274 6974 6c65 223e  ty name="title">
+00002dc0: 0d0a 2020 2020 2020 2020 2020 2020 3c73  ..            <s
+00002dd0: 7472 696e 6720 636f 6d6d 656e 743d 2254  tring comment="T
+00002de0: 6865 2074 6974 6c65 206f 6620 7468 6520  he title of the 
+00002df0: 676c 6f62 616c 2061 7370 6563 7420 6772  global aspect gr
+00002e00: 6f75 7062 6f78 223e 5374 796c 653c 2f73  oupbox">Style</s
+00002e10: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
+00002e20: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+00002e30: 2020 2020 2020 2020 2020 203c 6c61 796f             <layo
+00002e40: 7574 2063 6c61 7373 3d22 5156 426f 784c  ut class="QVBoxL
+00002e50: 6179 6f75 7422 206e 616d 653d 2276 6572  ayout" name="ver
+00002e60: 7469 6361 6c4c 6179 6f75 745f 3422 3e0d  ticalLayout_4">.
+00002e70: 0a20 2020 2020 2020 2020 2020 203c 6974  .            <it
+00002e80: 656d 3e0d 0a20 2020 2020 2020 2020 2020  em>..           
+00002e90: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00002ea0: 2251 436f 6d62 6f42 6f78 2220 6e61 6d65  "QComboBox" name
+00002eb0: 3d22 7374 796c 6573 4342 223e 0d0a 2020  ="stylesCB">..  
+00002ec0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00002ed0: 7065 7274 7920 6e61 6d65 3d22 7768 6174  perty name="what
+00002ee0: 7354 6869 7322 3e0d 0a20 2020 2020 2020  sThis">..       
+00002ef0: 2020 2020 2020 2020 3c73 7472 696e 672f          <string/
+00002f00: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002f10: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
+00002f20: 2020 2020 2020 2020 2020 203c 2f77 6964             </wid
+00002f30: 6765 743e 0d0a 2020 2020 2020 2020 2020  get>..          
+00002f40: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
+00002f50: 2020 2020 2020 3c2f 6c61 796f 7574 3e0d        </layout>.
+00002f60: 0a20 2020 2020 2020 2020 203c 2f77 6964  .          </wid
+00002f70: 6765 743e 0d0a 2020 2020 2020 2020 203c  get>..         <
+00002f80: 2f69 7465 6d3e 0d0a 2020 2020 2020 2020  /item>..        
+00002f90: 3c2f 6c61 796f 7574 3e0d 0a20 2020 2020  </layout>..     
+00002fa0: 2020 3c2f 7769 6467 6574 3e0d 0a20 2020    </widget>..   
+00002fb0: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
+00002fc0: 733d 2251 5769 6467 6574 2220 6e61 6d65  s="QWidget" name
+00002fd0: 3d22 706c 7567 696e 7350 6167 6522 3e0d  ="pluginsPage">.
+00002fe0: 0a20 2020 2020 2020 203c 7072 6f70 6572  .        <proper
+00002ff0: 7479 206e 616d 653d 2273 697a 6550 6f6c  ty name="sizePol
+00003000: 6963 7922 3e0d 0a20 2020 2020 2020 2020  icy">..         
+00003010: 3c73 697a 6570 6f6c 6963 7920 6873 697a  <sizepolicy hsiz
+00003020: 6574 7970 653d 2245 7870 616e 6469 6e67  etype="Expanding
+00003030: 2220 7673 697a 6574 7970 653d 2250 7265  " vsizetype="Pre
+00003040: 6665 7272 6564 223e 0d0a 2020 2020 2020  ferred">..      
+00003050: 2020 2020 3c68 6f72 7374 7265 7463 683e      <horstretch>
+00003060: 303c 2f68 6f72 7374 7265 7463 683e 0d0a  0</horstretch>..
+00003070: 2020 2020 2020 2020 2020 3c76 6572 7374            <verst
+00003080: 7265 7463 683e 303c 2f76 6572 7374 7265  retch>0</verstre
+00003090: 7463 683e 0d0a 2020 2020 2020 2020 203c  tch>..         <
+000030a0: 2f73 697a 6570 6f6c 6963 793e 0d0a 2020  /sizepolicy>..  
+000030b0: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+000030c0: 3e0d 0a20 2020 2020 2020 203c 6c61 796f  >..        <layo
+000030d0: 7574 2063 6c61 7373 3d22 5156 426f 784c  ut class="QVBoxL
+000030e0: 6179 6f75 7422 206e 616d 653d 2276 6572  ayout" name="ver
+000030f0: 7469 6361 6c4c 6179 6f75 745f 3922 3e0d  ticalLayout_9">.
+00003100: 0a20 2020 2020 2020 2020 3c69 7465 6d3e  .         <item>
+00003110: 0d0a 2020 2020 2020 2020 2020 3c77 6964  ..          <wid
+00003120: 6765 7420 636c 6173 733d 2251 4772 6f75  get class="QGrou
+00003130: 7042 6f78 2220 6e61 6d65 3d22 666f 6c64  pBox" name="fold
+00003140: 6572 7347 4222 3e0d 0a20 2020 2020 2020  ersGB">..       
+00003150: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00003160: 6d65 3d22 7768 6174 7354 6869 7322 3e0d  me="whatsThis">.
+00003170: 0a20 2020 2020 2020 2020 2020 203c 7374  .            <st
+00003180: 7269 6e67 2f3e 0d0a 2020 2020 2020 2020  ring/>..        
+00003190: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
+000031a0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000031b0: 6572 7479 206e 616d 653d 2274 6974 6c65  erty name="title
+000031c0: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+000031d0: 3c73 7472 696e 673e 4176 6169 6c61 626c  <string>Availabl
+000031e0: 6520 706c 7567 696e 733c 2f73 7472 696e  e plugins</strin
+000031f0: 673e 0d0a 2020 2020 2020 2020 2020 203c  g>..           <
+00003200: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
+00003210: 2020 2020 2020 203c 6c61 796f 7574 2063         <layout c
+00003220: 6c61 7373 3d22 5156 426f 784c 6179 6f75  lass="QVBoxLayou
+00003230: 7422 206e 616d 653d 2276 6572 7469 6361  t" name="vertica
+00003240: 6c4c 6179 6f75 745f 3622 3e0d 0a20 2020  lLayout_6">..   
+00003250: 2020 2020 2020 2020 203c 6974 656d 3e0d           <item>.
+00003260: 0a20 2020 2020 2020 2020 2020 2020 3c77  .             <w
+00003270: 6964 6765 7420 636c 6173 733d 2251 5472  idget class="QTr
+00003280: 6565 5669 6577 2220 6e61 6d65 3d22 706c  eeView" name="pl
+00003290: 7567 696e 7354 5622 3e0d 0a20 2020 2020  uginsTV">..     
+000032a0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+000032b0: 7479 206e 616d 653d 2273 697a 6550 6f6c  ty name="sizePol
+000032c0: 6963 7922 3e0d 0a20 2020 2020 2020 2020  icy">..         
+000032d0: 2020 2020 2020 3c73 697a 6570 6f6c 6963        <sizepolic
+000032e0: 7920 6873 697a 6574 7970 653d 2250 7265  y hsizetype="Pre
+000032f0: 6665 7272 6564 2220 7673 697a 6574 7970  ferred" vsizetyp
+00003300: 653d 2250 7265 6665 7272 6564 223e 0d0a  e="Preferred">..
+00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 3c68 6f72 7374 7265 7463 683e 303c 2f68  <horstretch>0</h
+00003330: 6f72 7374 7265 7463 683e 0d0a 2020 2020  orstretch>..    
+00003340: 2020 2020 2020 2020 2020 2020 3c76 6572              <ver
+00003350: 7374 7265 7463 683e 303c 2f76 6572 7374  stretch>0</verst
+00003360: 7265 7463 683e 0d0a 2020 2020 2020 2020  retch>..        
+00003370: 2020 2020 2020 203c 2f73 697a 6570 6f6c         </sizepol
+00003380: 6963 793e 0d0a 2020 2020 2020 2020 2020  icy>..          
+00003390: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
+000033a0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+000033b0: 7072 6f70 6572 7479 206e 616d 653d 2277  property name="w
+000033c0: 6861 7473 5468 6973 223e 0d0a 2020 2020  hatsThis">..    
+000033d0: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
+000033e0: 6e67 3e54 6865 206c 6973 7420 6f66 2061  ng>The list of a
+000033f0: 6c6c 2061 7661 696c 6162 6c65 2070 6c75  ll available plu
+00003400: 6769 6e73 2e20 4966 2061 2070 6c75 6769  gins. If a plugi
+00003410: 6e20 6973 2063 6865 636b 6564 2074 6865  n is checked the
+00003420: 6e20 6974 2069 7320 656e 6162 6c65 6420  n it is enabled 
+00003430: 2862 7574 206e 6f74 206e 6563 6573 7361  (but not necessa
+00003440: 7265 6c79 206c 6f61 6465 6429 2c20 6966  rely loaded), if
+00003450: 2069 7420 6973 2075 6e63 6865 636b 6564   it is unchecked
+00003460: 2074 6865 6e20 6974 2069 7320 6469 7361   then it is disa
+00003470: 626c 6564 2028 6275 7420 6e6f 7420 6e65  bled (but not ne
+00003480: 6365 7373 6172 656c 7920 756e 6c6f 6164  cessarely unload
+00003490: 6564 292e 2050 6c65 6173 652c 206e 6f74  ed). Please, not
+000034a0: 6520 7468 6174 2063 6861 6e67 6573 2069  e that changes i
+000034b0: 6e20 7468 6520 6368 6563 6b20 7374 6174  n the check stat
+000034c0: 6520 6f66 2070 6c75 6769 6e73 2077 696c  e of plugins wil
+000034d0: 6c20 7461 6b65 2065 6666 6563 7420 7468  l take effect th
+000034e0: 6520 6e65 7874 2074 696d 6520 796f 7520  e next time you 
+000034f0: 7374 6172 7420 5669 5461 626c 6573 2e3c  start ViTables.<
+00003500: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
+00003510: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+00003520: 7479 3e0d 0a20 2020 2020 2020 2020 2020  ty>..           
+00003530: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00003540: 653d 2265 6469 7454 7269 6767 6572 7322  e="editTriggers"
+00003550: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00003560: 2020 3c73 6574 3e51 4162 7374 7261 6374    <set>QAbstract
+00003570: 4974 656d 5669 6577 3a3a 4e6f 4564 6974  ItemView::NoEdit
+00003580: 5472 6967 6765 7273 3c2f 7365 743e 0d0a  Triggers</set>..
+00003590: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000035a0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
+000035b0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+000035c0: 7479 206e 616d 653d 2272 6f6f 7449 7344  ty name="rootIsD
+000035d0: 6563 6f72 6174 6564 223e 0d0a 2020 2020  ecorated">..    
+000035e0: 2020 2020 2020 2020 2020 203c 626f 6f6c             <bool
+000035f0: 3e66 616c 7365 3c2f 626f 6f6c 3e0d 0a20  >false</bool>.. 
+00003600: 2020 2020 2020 2020 2020 2020 203c 2f70               </p
+00003610: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
+00003620: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00003630: 7920 6e61 6d65 3d22 6578 7061 6e64 734f  y name="expandsO
+00003640: 6e44 6f75 626c 6543 6c69 636b 223e 0d0a  nDoubleClick">..
+00003650: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00003660: 626f 6f6c 3e66 616c 7365 3c2f 626f 6f6c  bool>false</bool
+00003670: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00003680: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
+00003690: 2020 2020 2020 2020 2020 203c 2f77 6964             </wid
+000036a0: 6765 743e 0d0a 2020 2020 2020 2020 2020  get>..          
+000036b0: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
+000036c0: 2020 2020 2020 3c2f 6c61 796f 7574 3e0d        </layout>.
+000036d0: 0a20 2020 2020 2020 2020 203c 2f77 6964  .          </wid
+000036e0: 6765 743e 0d0a 2020 2020 2020 2020 203c  get>..         <
+000036f0: 2f69 7465 6d3e 0d0a 2020 2020 2020 2020  /item>..        
+00003700: 3c2f 6c61 796f 7574 3e0d 0a20 2020 2020  </layout>..     
+00003710: 2020 3c2f 7769 6467 6574 3e0d 0a20 2020    </widget>..   
+00003720: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
+00003730: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
+00003740: 3c2f 6c61 796f 7574 3e0d 0a20 2020 3c2f  </layout>..   </
+00003750: 6974 656d 3e0d 0a20 2020 3c69 7465 6d3e  item>..   <item>
+00003760: 0d0a 2020 2020 3c77 6964 6765 7420 636c  ..    <widget cl
+00003770: 6173 733d 2251 4469 616c 6f67 4275 7474  ass="QDialogButt
+00003780: 6f6e 426f 7822 206e 616d 653d 2262 7574  onBox" name="but
+00003790: 746f 6e73 426f 7822 3e0d 0a20 2020 2020  tonsBox">..     
+000037a0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+000037b0: 6f72 6965 6e74 6174 696f 6e22 3e0d 0a20  orientation">.. 
+000037c0: 2020 2020 203c 656e 756d 3e51 743a 3a48       <enum>Qt::H
+000037d0: 6f72 697a 6f6e 7461 6c3c 2f65 6e75 6d3e  orizontal</enum>
+000037e0: 0d0a 2020 2020 203c 2f70 726f 7065 7274  ..     </propert
+000037f0: 793e 0d0a 2020 2020 203c 7072 6f70 6572  y>..     <proper
+00003800: 7479 206e 616d 653d 2273 7461 6e64 6172  ty name="standar
+00003810: 6442 7574 746f 6e73 223e 0d0a 2020 2020  dButtons">..    
+00003820: 2020 3c73 6574 3e51 4469 616c 6f67 4275    <set>QDialogBu
+00003830: 7474 6f6e 426f 783a 3a43 616e 6365 6c7c  ttonBox::Cancel|
+00003840: 5144 6961 6c6f 6742 7574 746f 6e42 6f78  QDialogButtonBox
+00003850: 3a3a 4865 6c70 7c51 4469 616c 6f67 4275  ::Help|QDialogBu
+00003860: 7474 6f6e 426f 783a 3a4f 6b7c 5144 6961  ttonBox::Ok|QDia
+00003870: 6c6f 6742 7574 746f 6e42 6f78 3a3a 5265  logButtonBox::Re
+00003880: 7365 743c 2f73 6574 3e0d 0a20 2020 2020  set</set>..     
+00003890: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
+000038a0: 203c 2f77 6964 6765 743e 0d0a 2020 203c   </widget>..   <
+000038b0: 2f69 7465 6d3e 0d0a 2020 3c2f 6c61 796f  /item>..  </layo
+000038c0: 7574 3e0d 0a20 3c2f 7769 6467 6574 3e0d  ut>.. </widget>.
+000038d0: 0a20 3c72 6573 6f75 7263 6573 2f3e 0d0a  . <resources/>..
+000038e0: 203c 636f 6e6e 6563 7469 6f6e 732f 3e0d   <connections/>.
+000038f0: 0a3c 2f75 693e 0d0a                      .</ui>..
```

### Comparing `ViTables-3.0.2/vitables/preferences/vtconfig.py` & `vitables-3.0.3/vitables/preferences/vtconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 from qtpy import QtGui
 from qtpy import QtWidgets
 
 import vitables.vttables.datasheet as datasheet
 
 
 __docformat__ = 'restructuredtext'
-__version__ = '3.0.2'
+__version__ = '3.0.3'
 
 translate = QtWidgets.QApplication.translate
 
 
 def getVersion():
     """The application version."""
     return __version__
@@ -133,17 +133,17 @@
         standard location, either on a global or user basis (see
         docstring for more information).
 
         In all platforms QSettings format is NativeFormat and scope
         is UserScope.
         """
 
-        organization = QtWidgets.qApp.organizationName()
-        product = QtWidgets.qApp.applicationName()
-        version = QtWidgets.qApp.applicationVersion()
+        organization = QtWidgets.QApplication.organizationName()
+        product = QtWidgets.QApplication.applicationName()
+        version = QtWidgets.QApplication.applicationVersion()
         if sys.platform.startswith('win'):
             # organizationName() -> product
             # applicationName() -> version
             super(Config, self).__init__(product, version)
             self.reg_path = 'HKEY_CURRENT_USER\\Software\\{0}\\{1}'.format(
                 product, version)
             self.setPath(QtCore.QSettings.NativeFormat,
@@ -202,15 +202,15 @@
 
     def loggerFont(self):
         """
         Returns the logger font.
         """
 
         key = 'Logger/Font'
-        default_value = QtWidgets.qApp.font()
+        default_value = QtWidgets.QApplication.font()
         setting_value = self.value(key)
         if isinstance(setting_value, QtGui.QFont):
             return setting_value
         else:
             return default_value
 
     def workspaceBackground(self):
@@ -566,15 +566,15 @@
             workspace.setBackground(config[key])
             workspace.viewport().update()
 
         key = 'Look/currentStyle'
         if key in config:
             self.current_style = config[key]
             # Default style is provided by the underlying window manager
-            QtWidgets.qApp.setStyle(self.current_style)
+            QtWidgets.QApplication.setStyle(self.current_style)
 
         key = 'Plugins/Enabled'
         if key in config:
             self.enabled_plugins = config[key]
 
     def saveConfiguration(self):
         """
```

### Comparing `ViTables-3.0.2/vitables/queries/query.py` & `vitables-3.0.3/vitables/queries/query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
-#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
-#
-#       This program is free software: you can redistribute it and/or modify
-#       it under the terms of the GNU General Public License as published by
-#       the Free Software Foundation, either version 3 of the License, or
-#       (at your option) any later version.
-#
-#       This program is distributed in the hope that it will be useful,
-#       but WITHOUT ANY WARRANTY; without even the implied warranty of
-#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#       GNU General Public License for more details.
-#
-#       You should have received a copy of the GNU General Public License
-#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#       Author:  Vicent Mas - vmas@vitables.org
-
-"""
-This module executes `tables.Table` queries at low level.
-
-It collects information from the `New Query` dialog, processes it and then
-executes the query.
-"""
-
-__docformat__ = 'restructuredtext'
-
-import tables
-import numpy
-
-from qtpy import QtCore
-from qtpy import QtGui
-from qtpy import QtWidgets
-
-import vitables.utils
-
-translate = QtWidgets.QApplication.translate
-
-
-class Query(QtCore.QObject):
-    """Class implementing a tables.Table query.
-
-    Ideally queries SHOULD be sequentially executed in a secondary thread for
-    keeping the GUI responsive (i.e. not frozen) while a query (a potentially
-    long-running operation) is taking place. Unfortunately this goal has
-    proven difficult to achieve because `PyTables` is not thread-safe. So one
-    more task to the TO DO list :-)
-
-    The query is implemented in a clever way that doesn't interfer with the
-    lazy population of the tree of databases view: the query results table is
-    stored under a hidden group of the temporary database until the query
-    finishes. Then it is moved to the root node and becomes visible to the
-    world. This way, while the query results table is partially filled it
-    is not seen by the lazy population algorithm so it is not added to the
-    tree of databases view and neither the user nor ViTables will try to read
-    it. So no problems can occur trying to read a partially filled table.
-
-    :Parameters:
-
-    - `table_uid`: UID of the tables.Table instance being queried
-    - `table`: the table being queried
-    - `qdescr`: dictionary description of the query
-    """
-
-
-    query_completed = QtCore.Signal(bool, str, name="queryCompleted")
-
-
-    def __init__(self, tmp_h5file, table_uid, table, qdescr):
-        """Initialises the query."""
-
-        super(Query, self).__init__()
-
-        self.completed = False
-        self.tmp_h5file = tmp_h5file
-        self.table_uid = table_uid
-        self.table = table
-        self.qdescr = qdescr
-
-
-    def run(self):
-        """
-        Query a table and add a the result to the temporary database.
-        """
-
-        self.queryTable()
-        self.query_completed.emit(self.completed, self.table_uid)
-
-
-    def flushTable(self, ftable):
-        """Flush the filtered table and setup some user attributes.
-
-        :Parameters:
-
-        - `ftable`: the filtered table being flushed
-        """
-
-        ftable.flush()
-        # Set some user attributes that define this filtered table
-        asi = ftable.attrs
-        asi.query_path = self.qdescr['src_filepath']
-        asi.query_table = self.qdescr['src_path']
-        asi.query_condition = self.qdescr['title']
-
-
-    def queryWithIndex(self, src_dict):
-        """Do the query (`PyTables` level).
-        """
-
-        # The query range is made of numpy scalars with dtype int64
-        (start, stop, step) = self.qdescr['rows_range']
-        chunk_size = 10000
-        div = int((stop - start) // chunk_size)
-
-        # Create the destination table: its first column will contain
-        # the indices of the rows selected in the source table so a new
-        # description dictionary is needed. Int64 values are necessary
-        # to keep full 64-bit indices
-        ft_dict = {self.qdescr['indices_field_name']: tables.Int64Col(pos=-1)}
-        ft_dict.update(src_dict)
-        f_table = self.tmp_h5file.create_table(
-            '/_p_query_results',
-            self.qdescr['ft_name'],
-            ft_dict,
-            self.qdescr['title'])
-
-        # Get the array of rows that fulfill the condition
-        # Selection is done in several steps. It saves a *huge*
-        # amount of memory when querying large tables
-        for i in numpy.arange(0, div+1):
-            QtWidgets.qApp.processEvents()
-            lstart = start + chunk_size*i
-            if lstart > stop:
-                lstart = stop
-            lstop = lstart + chunk_size
-            if lstop > stop:
-                lstop = stop
-            coordinates = self.table.get_where_list(
-                self.qdescr['condition'],
-                self.qdescr['condvars'],
-                start=lstart, stop=lstop, step=step)
-            selection = self.table.read_coordinates(coordinates)
-            if selection.shape == (0, ):
-                continue
-
-            coord_dtype = numpy.dtype(
-                [(str(self.qdescr['indices_field_name']), '<i8')])
-            new_dtype = numpy.dtype(
-                coord_dtype.descr + selection.dtype.descr)
-
-            new_buffer = numpy.empty(selection.shape, dtype=new_dtype)
-            for field in selection.dtype.fields:
-                new_buffer[field] = selection[field]
-            new_buffer[str(self.qdescr['indices_field_name'])] = \
-                coordinates
-            f_table.append(new_buffer)
-            self.flushTable(f_table)
-
-        # Move the intermediate table to its final destination
-        self.tmp_h5file.move_node(
-            '/_p_query_results/' + self.qdescr['ft_name'],
-            '/', newname=self.qdescr['ft_name'],
-            overwrite=True)
-        self.completed = True
-
-
-    def queryWithNoIndex(self, src_dict):
-        """Do the query (`PyTables` level).
-        """
-
-        # The query range is made of numpy scalars with dtype int64
-        (start, stop, step) = self.qdescr['rows_range']
-        chunk_size = 10000
-        div = int((stop - start) // chunk_size)
-
-        # Create the destination table
-        f_table = self.tmp_h5file.create_table(
-            '/_p_query_results',
-            self.qdescr['ft_name'],
-            src_dict,
-            self.qdescr['title'])
-
-        # Get the array of rows that fulfill the condition
-        # Selection is done in several steps. It saves a *huge*
-        # amount of memory when querying large tables
-        for i in numpy.arange(0, div+1):
-            QtWidgets.qApp.processEvents()
-            lstart = start + chunk_size*i
-            if lstart > stop:
-                lstart = stop
-            lstop = lstart + chunk_size
-            if lstop > stop:
-                lstop = stop
-            selection = self.table.read_where(
-                self.qdescr['condition'],
-                self.qdescr['condvars'],
-                start=lstart, stop=lstop, step=step)
-            f_table.append(selection)
-            self.flushTable(f_table)
-
-        # Move the intermediate table to its final destination
-        self.tmp_h5file.move_node(
-            '/_p_query_results/' + self.qdescr['ft_name'],
-            '/', newname=self.qdescr['ft_name'],
-            overwrite=True)
-        self.completed = True
-
-
-    def queryTable(self):
-        """Do the query (`PyTables` level).
-        """
-
-        try:
-            src_dict = self.table.description._v_colobjects
-            # Add an `indexes` column to the result table
-            if self.qdescr['indices_field_name']:
-                self.queryWithIndex(src_dict)
-            # Do no add an `indexes` column to the result table
-            else:
-                self.queryWithNoIndex(src_dict)
-        except KeyError:
-            vitables.utils.formatExceptionInfo()
-            self.tmp_h5file.remove_node(
-                '/_p_query_results/' + self.qdescr['ft_name'])
-        else:
-            self.tmp_h5file.flush()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
+#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
+#
+#       This program is free software: you can redistribute it and/or modify
+#       it under the terms of the GNU General Public License as published by
+#       the Free Software Foundation, either version 3 of the License, or
+#       (at your option) any later version.
+#
+#       This program is distributed in the hope that it will be useful,
+#       but WITHOUT ANY WARRANTY; without even the implied warranty of
+#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#       GNU General Public License for more details.
+#
+#       You should have received a copy of the GNU General Public License
+#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+#       Author:  Vicent Mas - vmas@vitables.org
+
+"""
+This module executes `tables.Table` queries at low level.
+
+It collects information from the `New Query` dialog, processes it and then
+executes the query.
+"""
+
+__docformat__ = 'restructuredtext'
+
+import tables
+import numpy
+
+from qtpy import QtCore
+from qtpy import QtGui
+from qtpy import QtWidgets
+
+import vitables.utils
+
+translate = QtWidgets.QApplication.translate
+
+
+class Query(QtCore.QObject):
+    """Class implementing a tables.Table query.
+
+    Ideally queries SHOULD be sequentially executed in a secondary thread for
+    keeping the GUI responsive (i.e. not frozen) while a query (a potentially
+    long-running operation) is taking place. Unfortunately this goal has
+    proven difficult to achieve because `PyTables` is not thread-safe. So one
+    more task to the TO DO list :-)
+
+    The query is implemented in a clever way that doesn't interfer with the
+    lazy population of the tree of databases view: the query results table is
+    stored under a hidden group of the temporary database until the query
+    finishes. Then it is moved to the root node and becomes visible to the
+    world. This way, while the query results table is partially filled it
+    is not seen by the lazy population algorithm so it is not added to the
+    tree of databases view and neither the user nor ViTables will try to read
+    it. So no problems can occur trying to read a partially filled table.
+
+    :Parameters:
+
+    - `table_uid`: UID of the tables.Table instance being queried
+    - `table`: the table being queried
+    - `qdescr`: dictionary description of the query
+    """
+
+
+    query_completed = QtCore.Signal(bool, str, name="queryCompleted")
+
+
+    def __init__(self, tmp_h5file, table_uid, table, qdescr):
+        """Initialises the query."""
+
+        super(Query, self).__init__()
+
+        self.completed = False
+        self.tmp_h5file = tmp_h5file
+        self.table_uid = table_uid
+        self.table = table
+        self.qdescr = qdescr
+
+
+    def run(self):
+        """
+        Query a table and add a the result to the temporary database.
+        """
+
+        self.queryTable()
+        self.query_completed.emit(self.completed, self.table_uid)
+
+
+    def flushTable(self, ftable):
+        """Flush the filtered table and setup some user attributes.
+
+        :Parameters:
+
+        - `ftable`: the filtered table being flushed
+        """
+
+        ftable.flush()
+        # Set some user attributes that define this filtered table
+        asi = ftable.attrs
+        asi.query_path = self.qdescr['src_filepath']
+        asi.query_table = self.qdescr['src_path']
+        asi.query_condition = self.qdescr['title']
+
+
+    def queryWithIndex(self, src_dict):
+        """Do the query (`PyTables` level).
+        """
+
+        # The query range is made of numpy scalars with dtype int64
+        (start, stop, step) = self.qdescr['rows_range']
+        chunk_size = 10000
+        div = int((stop - start) // chunk_size)
+
+        # Create the destination table: its first column will contain
+        # the indices of the rows selected in the source table so a new
+        # description dictionary is needed. Int64 values are necessary
+        # to keep full 64-bit indices
+        ft_dict = {self.qdescr['indices_field_name']: tables.Int64Col(pos=-1)}
+        ft_dict.update(src_dict)
+        f_table = self.tmp_h5file.create_table(
+            '/_p_query_results',
+            self.qdescr['ft_name'],
+            ft_dict,
+            self.qdescr['title'])
+
+        # Get the array of rows that fulfill the condition
+        # Selection is done in several steps. It saves a *huge*
+        # amount of memory when querying large tables
+        for i in numpy.arange(0, div+1):
+            QtWidgets.QApplication.processEvents()
+            lstart = start + chunk_size*i
+            if lstart > stop:
+                lstart = stop
+            lstop = lstart + chunk_size
+            if lstop > stop:
+                lstop = stop
+            coordinates = self.table.get_where_list(
+                self.qdescr['condition'],
+                self.qdescr['condvars'],
+                start=lstart, stop=lstop, step=step)
+            selection = self.table.read_coordinates(coordinates)
+            if selection.shape == (0, ):
+                continue
+
+            coord_dtype = numpy.dtype(
+                [(str(self.qdescr['indices_field_name']), '<i8')])
+            new_dtype = numpy.dtype(
+                coord_dtype.descr + selection.dtype.descr)
+
+            new_buffer = numpy.empty(selection.shape, dtype=new_dtype)
+            for field in selection.dtype.fields:
+                new_buffer[field] = selection[field]
+            new_buffer[str(self.qdescr['indices_field_name'])] = \
+                coordinates
+            f_table.append(new_buffer)
+            self.flushTable(f_table)
+
+        # Move the intermediate table to its final destination
+        self.tmp_h5file.move_node(
+            '/_p_query_results/' + self.qdescr['ft_name'],
+            '/', newname=self.qdescr['ft_name'],
+            overwrite=True)
+        self.completed = True
+
+
+    def queryWithNoIndex(self, src_dict):
+        """Do the query (`PyTables` level).
+        """
+
+        # The query range is made of numpy scalars with dtype int64
+        (start, stop, step) = self.qdescr['rows_range']
+        chunk_size = 10000
+        div = int((stop - start) // chunk_size)
+
+        # Create the destination table
+        f_table = self.tmp_h5file.create_table(
+            '/_p_query_results',
+            self.qdescr['ft_name'],
+            src_dict,
+            self.qdescr['title'])
+
+        # Get the array of rows that fulfill the condition
+        # Selection is done in several steps. It saves a *huge*
+        # amount of memory when querying large tables
+        for i in numpy.arange(0, div+1):
+            QtWidgets.QApplication.processEvents()
+            lstart = start + chunk_size*i
+            if lstart > stop:
+                lstart = stop
+            lstop = lstart + chunk_size
+            if lstop > stop:
+                lstop = stop
+            selection = self.table.read_where(
+                self.qdescr['condition'],
+                self.qdescr['condvars'],
+                start=lstart, stop=lstop, step=step)
+            f_table.append(selection)
+            self.flushTable(f_table)
+
+        # Move the intermediate table to its final destination
+        self.tmp_h5file.move_node(
+            '/_p_query_results/' + self.qdescr['ft_name'],
+            '/', newname=self.qdescr['ft_name'],
+            overwrite=True)
+        self.completed = True
+
+
+    def queryTable(self):
+        """Do the query (`PyTables` level).
+        """
+
+        try:
+            src_dict = self.table.description._v_colobjects
+            # Add an `indexes` column to the result table
+            if self.qdescr['indices_field_name']:
+                self.queryWithIndex(src_dict)
+            # Do no add an `indexes` column to the result table
+            else:
+                self.queryWithNoIndex(src_dict)
+        except KeyError:
+            vitables.utils.formatExceptionInfo()
+            self.tmp_h5file.remove_node(
+                '/_p_query_results/' + self.qdescr['ft_name'])
+        else:
+            self.tmp_h5file.flush()
```

### Comparing `ViTables-3.0.2/vitables/queries/querydlg.py` & `vitables-3.0.3/vitables/queries/querydlg.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         self.query_info['condvars'] = self.condvars
         self.query_info['src_filepath'] = info['src_filepath']
         self.query_info['src_path'] = info['src_path']
 
         #
         # Create the dialog and customise the content of some widgets
         #
-        super(QueryDlg, self).__init__(QtWidgets.qApp.activeWindow())
+        super(QueryDlg, self).__init__(QtWidgets.QApplication.activeWindow())
         self.setupUi(self)
 
         self.setWindowTitle(translate('QueryDlg', 'New query on table: {0}',
                                       'A dialog caption').format(info['name']))
 
         self.nameLE.setText('FilteredTable_{0}'.format(counter))
```

### Comparing `ViTables-3.0.2/vitables/queries/querymgr.py` & `vitables-3.0.3/vitables/queries/querymgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                            query_description['condition']]
 
         # Run the query
         tmp_h5file = self.dbt_model.tmp_dbdoc.h5file
         new_query = query.Query(tmp_h5file, table_uid, table,
                                 query_description)
         new_query.query_completed.connect(self.addQueryResult)
-        QtWidgets.qApp.setOverrideCursor(QtCore.Qt.WaitCursor)
+        QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.WaitCursor)
         new_query.run()
 
     def getQueryInfo(self, info, table):
         """Retrieves useful info about the query.
 
         :Parameters:
 
@@ -227,15 +227,15 @@
         query_dlg = querydlg.QueryDlg(info, self.ft_names,
                                       self.counter, initial_condition, table)
         try:
             query_dlg.exec_()
         finally:
             query_description = dict(query_dlg.query_info)
             del query_dlg
-            QtWidgets.qApp.processEvents()
+            QtWidgets.QApplication.processEvents()
 
         if not query_description['condition']:
             return None
 
         # SET THE TITLE OF THE RESULT TABLE
         title = query_description['condition']
         for name in info['valid_fields']:
@@ -294,15 +294,15 @@
 
         :Parameters:
 
         - `completed`: whether the query has been succesful or not
         - `table_uid`: the UID of the table just queried
         """
 
-        QtWidgets.qApp.restoreOverrideCursor()
+        QtWidgets.QApplication.restoreOverrideCursor()
         if not completed:
             log.error(translate('QueriesManager',
                                 'Query on table {0} failed!',
                                 'Warning log message about a failed '
                                 'query').format(table_uid))
             return
```

### Comparing `ViTables-3.0.2/vitables/start.py` & `vitables-3.0.3/vitables/start.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/utils.py` & `vitables-3.0.3/vitables/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 def getVTApp():
     """Get a reference to the `VTApp` instance.
 
     This is useful namely for plugins.
     """
 
     vtapp = None
-    for widget in QtWidgets.qApp.topLevelWidgets():
+    for widget in QtWidgets.QApplication.topLevelWidgets():
         if widget.objectName() == 'VTGUI':
             vtapp = widget.vtapp
             break
 
     return vtapp
 
 
@@ -145,15 +145,15 @@
     - `menu`: the menu or context menu being updated
     - `entries`: QAction/Qmenu object or a list of such objects
     - `uid`: indicates the insertion position for the new entries
 
     :return: None
     """
 
-    if not isinstance(entries, collections.Iterable):
+    if not isinstance(entries, collections.abc.Iterable):
         entries = [entries]
 
     if isinstance(entries[0], QtWidgets.QAction):
         menu.insertEntry = menu.insertAction
     elif isinstance(entries[0], QtWidgets.QMenu):
         menu.insertEntry = menu.insertMenu
 
@@ -173,15 +173,15 @@
 
     - `menu`: the menu or context menu being updated
     - `entries`: QAction/QMenu object or a list of such objects
 
     :return: None
     """
 
-    if not isinstance(entries, collections.Iterable):
+    if not isinstance(entries, collections.abc.Iterable):
         entries = [entries]
 
     if isinstance(entries[0], QtWidgets.QAction):
         menu.addEntry = menu.addAction
     elif isinstance(entries[0], QtWidgets.QMenu):
         menu.addEntry = menu.addMenu
```

### Comparing `ViTables-3.0.2/vitables/vtapp.py` & `vitables-3.0.3/vitables/vtapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 """
 
 import os
 import time
 import sys
 import logging
 
+import numpy
 import tables
 
 from qtpy import QtCore
 from qtpy import QtGui
 from qtpy import QtWidgets
 
 import vitables.utils
@@ -545,20 +546,20 @@
                 node = self.gui.dbs_tree_model.nodeFromIndex(index)
                 if node.filepath == initial_filepath:
                     current_index = index
             self.gui.dbs_tree_view.setCurrentIndex(current_index)
 
         # Make a copy of the selected file
         try:
-            QtWidgets.qApp.setOverrideCursor(
+            QtWidgets.QApplication.setOverrideCursor(
                 QtGui.QCursor(QtCore.Qt.WaitCursor))
             dbdoc = self.gui.dbs_tree_model.getDBDoc(initial_filepath)
             dbdoc.copy_file(filepath)
         finally:
-            QtWidgets.qApp.restoreOverrideCursor()
+            QtWidgets.QApplication.restoreOverrideCursor()
 
         # Close the copied file (which is not necessarely selected in
         # the tree view because closing an overwritten file can change
         # the selected item) and open the new copy in read-write mode.
         # The position in the tree is kept
         for row, child in enumerate(self.gui.dbs_tree_model.root.children):
             if child.filepath == initial_filepath:
@@ -1242,15 +1243,15 @@
         pyversion = '.'.join((str(svi.major), str(svi.minor), str(svi.micro)))
         # The libraries versions dictionary
         libs_versions = {
             'title': translate('VTApp', 'Version Numbers',
                                'Caption of the Versions dialog'),
             'Python': pyversion,
             'PyTables': tables.__version__,
-            'NumPy': tables.numpy.__version__,
+            'NumPy': numpy.__version__,
             'Qt': QtCore.qVersion(),
             'PyQt': QtCore.PYQT_VERSION_STR,
             'ViTables': vtconfig.getVersion()
         }
 
         # Add new items to the dictionary
         libraries = ('HDF5', 'Zlib', 'LZO', 'BZIP2')
```

### Comparing `ViTables-3.0.2/vitables/vtgui.py` & `vitables-3.0.3/vitables/vtgui.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,16 +147,14 @@
                       <p>The diferent views can be tiled as a mosaic or
                       stacked as a cascade.
                       </qt>""",
                       'WhatsThis help for the workspace'))
 
         # The signal mapper used to keep the the Window menu updated
         self.window_mapper = QtCore.QSignalMapper(self)
-        self.window_mapper.mapped[QtWidgets.QWidget].connect(
-            self.workspace.setActiveSubWindow)
         self.workspace.installEventFilter(self)
         self.dbs_tree_view.clicked.connect(self.selection_changed)
 
     def selection_changed(self, index):
         self.updateActions()
         self.updateStatusBar()
 
@@ -674,15 +672,15 @@
         """
 
         # Do the required tidy up
         self.vtapp.fileExit()
 
         # Quit
         event.accept()
-        QtWidgets.qApp.quit()
+        QtWidgets.QApplication.quit()
 
     def makeCopy(self):
         """Copy text/leaf depending on which widget has focus.
 
         This method disambiguates the ``Ctrl+C`` shortcut. If the console has
         focus then ``Ctrl+C`` will copy the console selected text. If the
         databases tree view has focus then the selected node (if any) will be
```

### Comparing `ViTables-3.0.2/vitables/vtsite.py` & `vitables-3.0.3/vitables/vtsite.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vtsplash.py` & `vitables-3.0.3/vitables/vtsplash.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,12 @@
     def drawMessage(self, msg):
         """
         Draw the message text onto the splash screen.
 
         :Parameter msg: the message to be displayed
         """
 
-        QtWidgets.qApp.processEvents()
+        QtWidgets.QApplication.processEvents()
         self.msg = msg
         self.showMessage(self.msg)
         time.sleep(0.500)
         self.clearMessage()
```

### Comparing `ViTables-3.0.2/vitables/vttables/__init__.py` & `vitables-3.0.3/vitables/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-
-#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
-#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
-#
-#       This program is free software: you can redistribute it and/or modify
-#       it under the terms of the GNU General Public License as published by
-#       the Free Software Foundation, either version 3 of the License, or
-#       (at your option) any later version.
-#
-#       This program is distributed in the hope that it will be useful,
-#       but WITHOUT ANY WARRANTY; without even the implied warranty of
-#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#       GNU General Public License for more details.
-#
-#       You should have received a copy of the GNU General Public License
-#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#       Author:  Vicent Mas - vmas@vitables.org
-
-__all__ = ["buffer", "datasheet", "leaf_delegate", "leaf_model", "leaf_view", "scrollbar"]
+"""A viewer for HDF5 files."""
+#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
+#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
+#
+#       This program is free software: you can redistribute it and/or modify
+#       it under the terms of the GNU General Public License as published by
+#       the Free Software Foundation, either version 3 of the License, or
+#       (at your option) any later version.
+#
+#       This program is distributed in the hope that it will be useful,
+#       but WITHOUT ANY WARRANTY; without even the implied warranty of
+#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#       GNU General Public License for more details.
+#
+#       You should have received a copy of the GNU General Public License
+#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+#       Author:  Vicent Mas - vmas@vitables.org
+
+__version__ = '3.0.3'
+__all__ = ["docbrowser", "h5db", "logger", "nodeprops", "plugins",
+           "queries", "preferences", "vttables", "vtwidgets",
+           "utils", "vtsite", "vtapp", "vtgui", "vtsplash"]
```

### Comparing `ViTables-3.0.2/vitables/vttables/buffer.py` & `vitables-3.0.3/vitables/vttables/buffer.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vttables/datasheet.py` & `vitables-3.0.3/vitables/vttables/datasheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,30 +106,30 @@
         self.vtgui.updateActions()
 
         # Propagate the event. In the process, self.widget().closeEvent
         # will be called
         QtWidgets.QMdiSubWindow.closeEvent(self, event)
 
         if not self.vtgui.workspace.subWindowList():
-            self.vtgui.dbs_tree_view.setFocus(True)
+            self.vtgui.dbs_tree_view.setFocus()
 
     def focusInEvent(self, event):
         """Specialised handler for focus events.
 
         Synchronize with the tree view when the view gets keyboard focus.
 
         :Parameter event: the event being processed
         """
 
         # Sync the workspace with the tree view (if needed) but keep the
         # focus (giving focus to the tree view when a given view is
         # clicked is counter intuitive)
         QtWidgets.QMdiSubWindow.focusInEvent(self, event)
         self.syncTreeView()
-        self.setFocus(True)
+        self.setFocus()
 
     def syncTreeView(self):
         """
         If the view is activated select its leaf in the tree of databases view.
         """
 
         if self.vtgui.editing_dlg is not None:
```

### Comparing `ViTables-3.0.2/vitables/vttables/df_model.py` & `vitables-3.0.3/vitables/vttables/df_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,16 @@
             self._mode = tables_h5file.mode
             self._handle = tables_h5file
             self._filters = tables_h5file.filters
 
             pytables._tables()
 
     pgroup = leaf._g_getparent()
-    try:
-        assert pgroup._c_classid == 'GROUP'
-    except AssertionError:
-        log('Parent of {0} is not a GROUP'.format(leaf))
+    if pgroup._c_classid != 'GROUP':
+        log.debug('Parent of %s is not a GROUP', leaf)
 
     pandas_attr = getattr(pgroup._v_attrs, 'pandas_type', None)
     if pandas_attr in ['frame', 'frame_table']:
         hstore = HDFStoreWrapper(leaf._v_file)
 
         return DataFrameModel(leaf, hstore)
 
@@ -176,19 +174,19 @@
         :param length:
             The buffer size, i.e. the number of rows to be read.
         """
         # Enforce scroll limits.
         #
         start = max(start, 0)
         stop = min(start + length, self.leaf_numrows)
-        try:
-            assert stop >= start
-        except AssertionError:
-            log(('Chunk: number of rows {0}, first row {1}, '
-                 'last row {2}').format(self.numrows, start, stop))
+        if stop < start:
+            log.debug(
+                'Chunk: number of rows %s, first row %s, last row {2}',
+                self.numrows, start, stop
+            )
 
         # Ensure that the whole buffer will be filled.
         #
         actual_start = stop - self.numrows
         start = max(min(actual_start, start), 0)
 
         self._chunk = self._hstore.select(self._pgroup,
```

### Comparing `ViTables-3.0.2/vitables/vttables/filenodebuffer.py` & `vitables-3.0.3/vitables/vttables/filenodebuffer.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vttables/leaf_delegate.py` & `vitables-3.0.3/vitables/vttables/leaf_delegate.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vttables/leaf_model.py` & `vitables-3.0.3/vitables/vttables/leaf_model.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vttables/leaf_view.py` & `vitables-3.0.3/vitables/vttables/leaf_view.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vttables/scrollbar.py` & `vitables-3.0.3/vitables/vttables/scrollbar.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vtwidgets/__init__.py` & `vitables-3.0.3/vitables/plugins/columnorg/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-
-#       Copyright (C) 2005-2007 Carabos Coop. V. All rights reserved
-#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
-#
-#       This program is free software: you can redistribute it and/or modify
-#       it under the terms of the GNU General Public License as published by
-#       the Free Software Foundation, either version 3 of the License, or
-#       (at your option) any later version.
-#
-#       This program is distributed in the hope that it will be useful,
-#       but WITHOUT ANY WARRANTY; without even the implied warranty of
-#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#       GNU General Public License for more details.
-#
-#       You should have received a copy of the GNU General Public License
-#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#       Author:  Vicent Mas - vmas@vitables.org
-
-__all__ = ["nodenamedlg", "renamedlg", "zoom_cell"]
+
+#       Copyright (C) 2008-2019 Vicent Mas. All rights reserved
+#
+#       This program is free software: you can redistribute it and/or modify
+#       it under the terms of the GNU General Public License as published by
+#       the Free Software Foundation, either version 3 of the License, or
+#       (at your option) any later version.
+#
+#       This program is distributed in the hope that it will be useful,
+#       but WITHOUT ANY WARRANTY; without even the implied warranty of
+#       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#       GNU General Public License for more details.
+#
+#       You should have received a copy of the GNU General Public License
+#       along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+#       Author:  Vicent Mas - vmas@vitables.org
+
+__all__ = ['aboutpage', 'columnar_org']
```

### Comparing `ViTables-3.0.2/vitables/vtwidgets/nodename_dlg.ui` & `vitables-3.0.3/vitables/vtwidgets/nodename_dlg.ui`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vtwidgets/nodenamedlg.py` & `vitables-3.0.3/vitables/vtwidgets/nodenamedlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vtwidgets/rename_dlg.ui` & `vitables-3.0.3/vitables/vtwidgets/rename_dlg.ui`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vtwidgets/renamedlg.py` & `vitables-3.0.3/vitables/vtwidgets/renamedlg.py`

 * *Files identical despite different names*

### Comparing `ViTables-3.0.2/vitables/vtwidgets/zoom_cell.py` & `vitables-3.0.3/vitables/vtwidgets/zoom_cell.py`

 * *Files identical despite different names*

