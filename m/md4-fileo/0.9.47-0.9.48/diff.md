# Comparing `tmp/md4_fileo-0.9.47.tar.gz` & `tmp/md4_fileo-0.9.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md4_fileo-0.9.47.tar", max compression
+gzip compressed data, was "md4_fileo-0.9.48.tar", max compression
```

## Comparing `md4_fileo-0.9.47.tar` & `md4_fileo-0.9.48.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0       69 2023-07-27 08:05:45.042513 md4_fileo-0.9.47/fileo.py
--rw-r--r--   0        0        0     1087 2023-06-10 11:50:24.337940 md4_fileo-0.9.47/LICENSE
--rw-r--r--   0        0        0      594 2023-08-03 14:01:18.430562 md4_fileo-0.9.47/pyproject.toml
--rw-r--r--   0        0        0    11544 2023-07-27 08:05:45.041513 md4_fileo-0.9.47/README.md
--rw-r--r--   0        0        0        0 2023-06-10 11:50:24.357941 md4_fileo-0.9.47/src/__init__.py
--rw-r--r--   0        0        0     3356 2023-08-03 14:02:36.372525 md4_fileo-0.9.47/src/core/app_globals.py
--rw-r--r--   0        0        0      573 2023-07-27 08:05:45.055515 md4_fileo-0.9.47/src/core/app_signals.py
--rw-r--r--   0        0        0    10689 2023-08-03 05:51:58.723906 md4_fileo-0.9.47/src/core/bk_ut.py
--rw-r--r--   0        0        0     9163 2023-07-25 06:11:29.136975 md4_fileo-0.9.47/src/core/compact_list.py
--rw-r--r--   0        0        0     6450 2023-08-03 06:19:03.719169 md4_fileo-0.9.47/src/core/create_db.py
--rw-r--r--   0        0        0    34260 2023-08-03 05:51:58.725906 md4_fileo-0.9.47/src/core/db_ut.py
--rw-r--r--   0        0        0     9213 2023-07-24 06:13:34.750573 md4_fileo-0.9.47/src/core/drag_drop.py
--rw-r--r--   0        0        0      471 2023-07-31 16:10:38.806395 md4_fileo-0.9.47/src/core/duplicates.py
--rw-r--r--   0        0        0     7728 2023-07-31 16:10:38.807395 md4_fileo-0.9.47/src/core/edit_tree_model2.py
--rw-r--r--   0        0        0      492 2023-06-10 11:50:24.365941 md4_fileo-0.9.47/src/core/filename_editor.py
--rw-r--r--   0        0        0     2293 2023-08-03 05:51:58.726906 md4_fileo-0.9.47/src/core/history.py
--rw-r--r--   0        0        0     5645 2023-07-10 15:24:36.829270 md4_fileo-0.9.47/src/core/icons.py
--rw-r--r--   0        0        0     1603 2023-06-10 11:50:24.366941 md4_fileo-0.9.47/src/core/linux_menu.py
--rw-r--r--   0        0        0      527 2023-06-15 18:06:31.007139 md4_fileo-0.9.47/src/core/linux_win.py
--rw-r--r--   0        0        0     7233 2023-06-10 11:50:24.367940 md4_fileo-0.9.47/src/core/load_files.py
--rw-r--r--   0        0        0    27174 2023-08-03 12:23:11.252565 md4_fileo-0.9.47/src/core/low_bk.py
--rw-r--r--   0        0        0    17506 2023-08-02 17:59:48.420945 md4_fileo-0.9.47/src/core/sho.py
--rw-r--r--   0        0        0     6521 2023-07-31 16:10:38.810395 md4_fileo-0.9.47/src/core/table_model.py
--rw-r--r--   0        0        0     6664 2023-07-27 08:05:45.063517 md4_fileo-0.9.47/src/core/utils.py
--rw-r--r--   0        0        0     1498 2023-06-15 18:06:31.009136 md4_fileo-0.9.47/src/core/win_menu.py
--rw-r--r--   0        0        0      158 2023-06-15 18:06:31.009136 md4_fileo-0.9.47/src/core/win_win.py
--rw-r--r--   0        0        0     2489 2023-08-03 05:51:58.728907 md4_fileo-0.9.47/src/main.py
--rw-r--r--   0        0        0        0 2023-06-10 11:50:24.371940 md4_fileo-0.9.47/src/qss/__init__.py
--rw-r--r--   0        0        0      160 2023-06-10 11:50:24.371940 md4_fileo-0.9.47/src/qss/angle_down.svg
--rw-r--r--   0        0        0      160 2023-06-10 11:50:24.372942 md4_fileo-0.9.47/src/qss/angle_right.svg
--rw-r--r--   0        0        0     2183 2023-06-12 08:32:06.472370 md4_fileo-0.9.47/src/qss/default.param
--rw-r--r--   0        0        0     8064 2023-07-27 08:05:45.065518 md4_fileo-0.9.47/src/qss/default.qss
--rw-r--r--   0        0        0      150 2023-06-10 11:50:24.373940 md4_fileo-0.9.47/src/qss/match_case.svg
--rw-r--r--   0        0        0      226 2023-06-10 11:50:24.374941 md4_fileo-0.9.47/src/qss/match_word.svg
--rw-r--r--   0        0        0      531 2023-06-10 11:50:24.374941 md4_fileo-0.9.47/src/qss/search.svg
--rw-r--r--   0        0        0      156 2023-06-10 11:50:24.375942 md4_fileo-0.9.47/src/qss/vline3.svg
--rw-r--r--   0        0        0    31260 2023-07-27 08:05:45.066517 md4_fileo-0.9.47/src/ui/main.ui
--rw-r--r--   0        0        0    20463 2023-07-27 08:05:45.437467 md4_fileo-0.9.47/src/ui/ui_main.py
--rw-r--r--   0        0        0     2631 2023-08-03 05:51:58.729907 md4_fileo-0.9.47/src/widgets/about.py
--rw-r--r--   0        0        0    10063 2023-06-10 11:50:24.378940 md4_fileo-0.9.47/src/widgets/custom_grips.py
--rw-r--r--   0        0        0     4832 2023-07-27 08:05:45.070518 md4_fileo-0.9.47/src/widgets/file_authors.py
--rw-r--r--   0        0        0     9137 2023-08-03 05:51:58.730908 md4_fileo-0.9.47/src/widgets/file_data.py
--rw-r--r--   0        0        0     3082 2023-06-10 11:50:24.379938 md4_fileo-0.9.47/src/widgets/file_info.py
--rw-r--r--   0        0        0     4403 2023-07-31 16:10:38.812396 md4_fileo-0.9.47/src/widgets/file_note.py
--rw-r--r--   0        0        0    11941 2023-07-31 16:10:38.813396 md4_fileo-0.9.47/src/widgets/file_note.ui
--rw-r--r--   0        0        0     6734 2023-08-03 05:51:58.731908 md4_fileo-0.9.47/src/widgets/file_notes.py
--rw-r--r--   0        0        0     2257 2023-06-10 11:50:24.380939 md4_fileo-0.9.47/src/widgets/file_search.py
--rw-r--r--   0        0        0     6752 2023-06-10 11:50:24.381939 md4_fileo-0.9.47/src/widgets/file_search.ui
--rw-r--r--   0        0        0      615 2023-07-27 08:05:45.072519 md4_fileo-0.9.47/src/widgets/file_tags.py
--rw-r--r--   0        0        0    10122 2023-08-03 05:51:58.732908 md4_fileo-0.9.47/src/widgets/filter_setup.py
--rw-r--r--   0        0        0     3386 2023-08-03 05:51:58.733908 md4_fileo-0.9.47/src/widgets/find_files.py
--rw-r--r--   0        0        0    19222 2023-06-10 11:50:24.382939 md4_fileo-0.9.47/src/widgets/fold_container.py
--rw-r--r--   0        0        0     8264 2023-06-10 11:50:24.383940 md4_fileo-0.9.47/src/widgets/fold_container.ui
--rw-r--r--   0        0        0     2172 2023-06-10 11:50:24.383940 md4_fileo-0.9.47/src/widgets/foldable.py
--rw-r--r--   0        0        0     6530 2023-06-10 11:50:24.384939 md4_fileo-0.9.47/src/widgets/foldable.ui
--rw-r--r--   0        0        0     6240 2023-07-31 16:10:38.815397 md4_fileo-0.9.47/src/widgets/locations.py
--rw-r--r--   0        0        0     8941 2023-07-31 16:10:38.816397 md4_fileo-0.9.47/src/widgets/notes.ui
--rw-r--r--   0        0        0     6998 2023-08-03 05:51:58.734908 md4_fileo-0.9.47/src/widgets/open_db.py
--rw-r--r--   0        0        0     3403 2023-06-10 11:50:24.385940 md4_fileo-0.9.47/src/widgets/open_db.ui
--rw-r--r--   0        0        0     3704 2023-07-06 18:16:09.200274 md4_fileo-0.9.47/src/widgets/preferencies.py
--rw-r--r--   0        0        0    16788 2023-07-31 16:10:38.816397 md4_fileo-0.9.47/src/widgets/set_filter.ui
--rw-r--r--   0        0        0     8176 2023-07-31 16:10:39.164782 md4_fileo-0.9.47/src/widgets/ui_file_note.py
--rw-r--r--   0        0        0     6641 2023-06-10 11:50:24.386939 md4_fileo-0.9.47/src/widgets/ui_file_search.py
--rw-r--r--   0        0        0     7578 2023-06-10 11:50:24.387939 md4_fileo-0.9.47/src/widgets/ui_fold_container.py
--rw-r--r--   0        0        0     5291 2023-06-10 11:50:24.388939 md4_fileo-0.9.47/src/widgets/ui_foldable.py
--rw-r--r--   0        0        0     8028 2023-07-31 16:10:39.361565 md4_fileo-0.9.47/src/widgets/ui_notes.py
--rw-r--r--   0        0        0     3432 2023-06-10 11:50:24.388939 md4_fileo-0.9.47/src/widgets/ui_open_db.py
--rw-r--r--   0        0        0    14934 2023-07-31 16:10:39.567622 md4_fileo-0.9.47/src/widgets/ui_set_filter.py
--rw-r--r--   0        0        0     3328 2023-08-03 05:51:58.734908 md4_fileo-0.9.47/src/widgets/workers.py
--rw-r--r--   0        0        0    12483 1970-01-01 00:00:00.000000 md4_fileo-0.9.47/setup.py
--rw-r--r--   0        0        0    11988 1970-01-01 00:00:00.000000 md4_fileo-0.9.47/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-07-27 08:05:45.042513 md4_fileo-0.9.48/fileo.py
+-rw-r--r--   0        0        0     1087 2023-06-10 11:50:24.337940 md4_fileo-0.9.48/LICENSE
+-rw-r--r--   0        0        0      663 2023-08-04 08:07:20.548341 md4_fileo-0.9.48/pyproject.toml
+-rw-r--r--   0        0        0    11559 2023-08-04 07:29:31.191253 md4_fileo-0.9.48/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 11:50:24.357941 md4_fileo-0.9.48/src/__init__.py
+-rw-r--r--   0        0        0     3356 2023-08-04 07:47:33.606047 md4_fileo-0.9.48/src/core/app_globals.py
+-rw-r--r--   0        0        0      573 2023-07-27 08:05:45.055515 md4_fileo-0.9.48/src/core/app_signals.py
+-rw-r--r--   0        0        0    10689 2023-08-03 05:51:58.723906 md4_fileo-0.9.48/src/core/bk_ut.py
+-rw-r--r--   0        0        0     9163 2023-07-25 06:11:29.136975 md4_fileo-0.9.48/src/core/compact_list.py
+-rw-r--r--   0        0        0     6450 2023-08-04 06:12:36.066579 md4_fileo-0.9.48/src/core/create_db.py
+-rw-r--r--   0        0        0    34260 2023-08-04 07:32:21.814907 md4_fileo-0.9.48/src/core/db_ut.py
+-rw-r--r--   0        0        0     9213 2023-07-24 06:13:34.750573 md4_fileo-0.9.48/src/core/drag_drop.py
+-rw-r--r--   0        0        0      471 2023-07-31 16:10:38.806395 md4_fileo-0.9.48/src/core/duplicates.py
+-rw-r--r--   0        0        0     7728 2023-07-31 16:10:38.807395 md4_fileo-0.9.48/src/core/edit_tree_model2.py
+-rw-r--r--   0        0        0      492 2023-06-10 11:50:24.365941 md4_fileo-0.9.48/src/core/filename_editor.py
+-rw-r--r--   0        0        0     2293 2023-08-03 05:51:58.726906 md4_fileo-0.9.48/src/core/history.py
+-rw-r--r--   0        0        0     5645 2023-07-10 15:24:36.829270 md4_fileo-0.9.48/src/core/icons.py
+-rw-r--r--   0        0        0     1603 2023-06-10 11:50:24.366941 md4_fileo-0.9.48/src/core/linux_menu.py
+-rw-r--r--   0        0        0      527 2023-06-15 18:06:31.007139 md4_fileo-0.9.48/src/core/linux_win.py
+-rw-r--r--   0        0        0     7233 2023-06-10 11:50:24.367940 md4_fileo-0.9.48/src/core/load_files.py
+-rw-r--r--   0        0        0    26953 2023-08-04 07:42:21.085359 md4_fileo-0.9.48/src/core/low_bk.py
+-rw-r--r--   0        0        0    17506 2023-08-03 14:51:01.895608 md4_fileo-0.9.48/src/core/sho.py
+-rw-r--r--   0        0        0     6521 2023-07-31 16:10:38.810395 md4_fileo-0.9.48/src/core/table_model.py
+-rw-r--r--   0        0        0     6664 2023-07-27 08:05:45.063517 md4_fileo-0.9.48/src/core/utils.py
+-rw-r--r--   0        0        0     1498 2023-06-15 18:06:31.009136 md4_fileo-0.9.48/src/core/win_menu.py
+-rw-r--r--   0        0        0      158 2023-06-15 18:06:31.009136 md4_fileo-0.9.48/src/core/win_win.py
+-rw-r--r--   0        0        0     2489 2023-08-03 05:51:58.728907 md4_fileo-0.9.48/src/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 11:50:24.371940 md4_fileo-0.9.48/src/qss/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-10 11:50:24.371940 md4_fileo-0.9.48/src/qss/angle_down.svg
+-rw-r--r--   0        0        0      160 2023-06-10 11:50:24.372942 md4_fileo-0.9.48/src/qss/angle_right.svg
+-rw-r--r--   0        0        0     2183 2023-06-12 08:32:06.472370 md4_fileo-0.9.48/src/qss/default.param
+-rw-r--r--   0        0        0     8064 2023-07-27 08:05:45.065518 md4_fileo-0.9.48/src/qss/default.qss
+-rw-r--r--   0        0        0      150 2023-06-10 11:50:24.373940 md4_fileo-0.9.48/src/qss/match_case.svg
+-rw-r--r--   0        0        0      226 2023-06-10 11:50:24.374941 md4_fileo-0.9.48/src/qss/match_word.svg
+-rw-r--r--   0        0        0      531 2023-06-10 11:50:24.374941 md4_fileo-0.9.48/src/qss/search.svg
+-rw-r--r--   0        0        0      156 2023-06-10 11:50:24.375942 md4_fileo-0.9.48/src/qss/vline3.svg
+-rw-r--r--   0        0        0    31260 2023-07-27 08:05:45.066517 md4_fileo-0.9.48/src/ui/main.ui
+-rw-r--r--   0        0        0    20463 2023-07-27 08:05:45.437467 md4_fileo-0.9.48/src/ui/ui_main.py
+-rw-r--r--   0        0        0     2631 2023-08-03 05:51:58.729907 md4_fileo-0.9.48/src/widgets/about.py
+-rw-r--r--   0        0        0    10063 2023-06-10 11:50:24.378940 md4_fileo-0.9.48/src/widgets/custom_grips.py
+-rw-r--r--   0        0        0     4832 2023-07-27 08:05:45.070518 md4_fileo-0.9.48/src/widgets/file_authors.py
+-rw-r--r--   0        0        0     9137 2023-08-03 05:51:58.730908 md4_fileo-0.9.48/src/widgets/file_data.py
+-rw-r--r--   0        0        0     3082 2023-06-10 11:50:24.379938 md4_fileo-0.9.48/src/widgets/file_info.py
+-rw-r--r--   0        0        0     4403 2023-07-31 16:10:38.812396 md4_fileo-0.9.48/src/widgets/file_note.py
+-rw-r--r--   0        0        0    11941 2023-07-31 16:10:38.813396 md4_fileo-0.9.48/src/widgets/file_note.ui
+-rw-r--r--   0        0        0     6734 2023-08-03 05:51:58.731908 md4_fileo-0.9.48/src/widgets/file_notes.py
+-rw-r--r--   0        0        0     2257 2023-06-10 11:50:24.380939 md4_fileo-0.9.48/src/widgets/file_search.py
+-rw-r--r--   0        0        0     6752 2023-06-10 11:50:24.381939 md4_fileo-0.9.48/src/widgets/file_search.ui
+-rw-r--r--   0        0        0      615 2023-07-27 08:05:45.072519 md4_fileo-0.9.48/src/widgets/file_tags.py
+-rw-r--r--   0        0        0    10118 2023-08-04 07:05:38.563006 md4_fileo-0.9.48/src/widgets/filter_setup.py
+-rw-r--r--   0        0        0     3386 2023-08-03 05:51:58.733908 md4_fileo-0.9.48/src/widgets/find_files.py
+-rw-r--r--   0        0        0    19222 2023-06-10 11:50:24.382939 md4_fileo-0.9.48/src/widgets/fold_container.py
+-rw-r--r--   0        0        0     8264 2023-06-10 11:50:24.383940 md4_fileo-0.9.48/src/widgets/fold_container.ui
+-rw-r--r--   0        0        0     2172 2023-06-10 11:50:24.383940 md4_fileo-0.9.48/src/widgets/foldable.py
+-rw-r--r--   0        0        0     6530 2023-06-10 11:50:24.384939 md4_fileo-0.9.48/src/widgets/foldable.ui
+-rw-r--r--   0        0        0     6240 2023-07-31 16:10:38.815397 md4_fileo-0.9.48/src/widgets/locations.py
+-rw-r--r--   0        0        0     8941 2023-07-31 16:10:38.816397 md4_fileo-0.9.48/src/widgets/notes.ui
+-rw-r--r--   0        0        0     6998 2023-08-03 05:51:58.734908 md4_fileo-0.9.48/src/widgets/open_db.py
+-rw-r--r--   0        0        0     3403 2023-06-10 11:50:24.385940 md4_fileo-0.9.48/src/widgets/open_db.ui
+-rw-r--r--   0        0        0     3704 2023-07-06 18:16:09.200274 md4_fileo-0.9.48/src/widgets/preferencies.py
+-rw-r--r--   0        0        0    16788 2023-07-31 16:10:38.816397 md4_fileo-0.9.48/src/widgets/set_filter.ui
+-rw-r--r--   0        0        0     8176 2023-07-31 16:10:39.164782 md4_fileo-0.9.48/src/widgets/ui_file_note.py
+-rw-r--r--   0        0        0     6641 2023-06-10 11:50:24.386939 md4_fileo-0.9.48/src/widgets/ui_file_search.py
+-rw-r--r--   0        0        0     7578 2023-06-10 11:50:24.387939 md4_fileo-0.9.48/src/widgets/ui_fold_container.py
+-rw-r--r--   0        0        0     5291 2023-06-10 11:50:24.388939 md4_fileo-0.9.48/src/widgets/ui_foldable.py
+-rw-r--r--   0        0        0     8028 2023-07-31 16:10:39.361565 md4_fileo-0.9.48/src/widgets/ui_notes.py
+-rw-r--r--   0        0        0     3432 2023-06-10 11:50:24.388939 md4_fileo-0.9.48/src/widgets/ui_open_db.py
+-rw-r--r--   0        0        0    14934 2023-07-31 16:10:39.567622 md4_fileo-0.9.48/src/widgets/ui_set_filter.py
+-rw-r--r--   0        0        0     3328 2023-08-03 05:51:58.734908 md4_fileo-0.9.48/src/widgets/workers.py
+-rw-r--r--   0        0        0    12498 1970-01-01 00:00:00.000000 md4_fileo-0.9.48/setup.py
+-rw-r--r--   0        0        0    11998 1970-01-01 00:00:00.000000 md4_fileo-0.9.48/PKG-INFO
```

### Comparing `md4_fileo-0.9.47/LICENSE` & `md4_fileo-0.9.48/LICENSE`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/pyproject.toml` & `md4_fileo-0.9.48/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "md4_fileo"
-version = "0.9.47"
+version = "0.9.48"
 description = "Yet another file organizer"
 authors = ["mihal.d44 <mihal.d44@gmail.com>"]
 readme = "README.md"
 packages = [
 {include = "fileo.py"},
 {include = "src"},
 ]
 
+[project.urls]
+"Homepage" = "https://github.com/Michal-D4/fileo"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
 pypdf2 = "^3.0.1"
 pyqt6 = "^6.4.0"
 qtawesome = "^1.2.2"
 apsw = "^3.40.1.0"
```

### Comparing `md4_fileo-0.9.47/README.md` & `md4_fileo-0.9.48/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,44 +22,45 @@
    4. open filter settings dialog, switch to "FILTER_SETUP" mode
    5. open a dialog to upload files to the application from  the selected root folder and all its subfolders
    6. hide/show left pane
    7. menu button
 7. list of selected files (by filter, folder, etc.)
 8. current database name
 9. folder tree branch from root to current folder
-10. panel for displaying/editing file data: comments (notes), tags, authors (for books), links (links to a file can be located in several folders).
+10. panel for displaying/editing file data: notes, tags, authors (for books), links (links to a file locations, file can be located in several folders).
 
 The application works in three main modes: DIR, FILTER and FILTER_SETUP. In DIR mode, files are selected by the current directory in the "Folders" widget.
 
 In FILTER mode, the list of files depends on the filter options set in FILTER_SETUP mode. The filter may depend on the selected folders, selected tags, and selected authors in the boxes in the left pane. In FILTER_SETUP mode, the list of files does not change when changing the selected folders, tags, authors. But in FILTER mode, any changes are immediately displayed in the list of files.
 
 ## How it's done
 
 As said, the app is about files. Files have a number of attributes:
 
 1. name
-2. path, the user practically does not see it, only by opening the directory or copying the full file name and on the "File Information" page
+2. path, the user practically does not see it, only by opening the directory or copying the full file name and on the "File Info" page
 3. file extension
 4. tags
 5. rating
 6. author(s) - usually for books
 7. dates of:
     1. modification
     2. reading
     3. creation
     4. publication (books)
+    5. date of last created/modified note to the file
 8. rating
 9. file opened (times)
 10. size in bytes
 11. number of pages - usually for books
 
 The following attributes are used in filter: all dates (but only one can be used at a time), extension, tags, rating, authors, and folder which was intentionally not included in the file attributes.
 
 Folders are not associated with file system directories, the path is used for that. You can freely create, move, copy and delete folders in the folder tree, the files will remain intact. You can, for example, create multiple folder hierarchies, this can be handy. Of course, if you delete all folders it will be impossible to access files using folder tree, but they remain accessible by filter. The next time the **`@@Lost`** folder will appear, it can be used to access files that are not in any other folder.
-You can also *copy/move files from one folder to another*. **Copying** is done by dragging *with the left mouse button pressed*, dragging *with the right mouse button pressed* allows you to choose whether to **move** or **copy** *selected files*.
+You can also *copy/move files from one folder to another*  by dragging *with the left or right mouse button pressed*.
 
 
 
 ## How it works
 
 ### How to add files?
 
@@ -90,17 +91,17 @@
 
 ### How to work with filters
 
 First you should setup the filter:
 
 ![image-20230213185910924](https://github.com/Michal-D4/fileo/raw/main/img/image-20230213185910924.png)
 
-With the filter set in the picture, the list of files will include files from the any of `DB`, `ML` or `Rust` folders that have at least one of the `Math`, `ML` or `package` tags, have a rating higher than 4 and are open after `2022-09-14`.
+With the filter set in the picture, the list of files will include files from the any of `DB`, `ML` or `Rust` folders that have at least one of the `Math`, `ML` or `package` tags, have a rating higher than 4 and are open after `2022-09-14 00:00:00`. 
 
-> **Note.** Here "after" and "before" include the date in the input fields 2022-09-14 and 2022-11-14. That is, if "after" and "before" are the same, then the filter will show files with this date.
+> **Note.** In case of before &mdash; the date before or equal to `2022-11-14 23:59:59`. 
 
 The Apply button applies a specified filter without closing the Filter Setup dialog box.
 
 The Done button applies the filter, closes the dialog, and switches the application to "**Filter Mode**". In this mode, when you change the selection in any of the fields on the left panel (Folders, Tags, Extensions, Authors), the list of files immediately changes.
 
 ### How to find files by name
 
@@ -109,23 +110,27 @@
 The search is performed by pressing the Enter key. "Aa" is a case sensitive search, if checked, "ab" - exact search, but you can use wildcards: "*" - any number of any letters, or "?" - any single letter.
 
 ### How to make notes to the file
 
 ![fileo-comments](https://github.com/Michal-D4/fileo/raw/main/img/file-notes.jpg)
 
 1. "+"  plus button - add new note and open it in the editor
-6. "x" button - delete the note
 8.  the button to open the note in the editor
+3. start editing of the note
+4. "x" button - delete the note
+5. external (http) reference, can be open in the system web browser
 
 #### Note editor
 
 ![edit-comment](https://github.com/Michal-D4/fileo/raw/main/img/edit-comment.jpg)
 
-1. the save changes button
-2. the button to discard changes
+1. the save changes button, save changes and close editor
+2. the button to discard changes 
+
+> pressing any of these buttons closes the editor
 
 Note is a markdown text. You can insert web links here, but the links to files in the application are not implemented (and not planned yet)
 
 ### Tag selector
 
 ![tag-selector](https://github.com/Michal-D4/fileo/raw/main/img/tag-selector.jpg)
 
@@ -149,15 +154,15 @@
 
 1-4 are locations of the current file, 5 is a context menu.
 
 The location marked with bullet is a current location.
 
 All 4 locations end with the Poetry folder. This means that the file exists only in this folder (Poetry), the folder Poetry is presented in 4 branches. That's why the file has 4 locations.
 
-The letters "L" and "H" in brackets means "Link" and "Hidden". "Link" and "Hidden" are attributes of folder. For example, the folder "fileo" in the path 2 is a link to the folder "fileo"[^1] in the path 1; the folder "A folder"  in folder "my" is "Hidden", but it is shown in the picture below because of the "FOLDERS" widget is in "Show hidden folders" mode:
+The letters "L" and "H" in brackets means "Link" and "Hidden". "Link" and "Hidden" are attributes of folder. For example, the folder "fileo" in the branch 2 is a link to the folder "fileo"[^1] in the branch 1; the folder "A folder"  in folder "my" is "Hidden", but it is shown in the picture below because of the "FOLDERS" widget is in "Show hidden folders" mode:
 
 ![Folders](https://github.com/Michal-D4/fileo/raw/main/img/Folders.jpg)
 
 1. The current folder (Poetry).
 2. The check box. It is used to switch the "FOLDERS" widget to the "Show hidden folders" mode. The folders "@@Lost" and "Linux" are hidden; "A folder" and "fileo" in the folder "my" are links. The only difference between folder and link to it is that when you delete folder all its links and all its children will be deleted too, whereas deletion of any link of folder does not impact any other folder.
 3. The current file. "Environment Variables in Linux.md"
```

### Comparing `md4_fileo-0.9.47/src/core/app_globals.py` & `md4_fileo-0.9.48/src/core/app_globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def app_name() -> str:
     return "fileo"
 
 def app_version() -> str:
     """
     if version changed here then also change it in the "pyproject.toml" file
     """
-    return '0.9.47'
+    return '0.9.48'
 
 # only this instance of AppSignals should be used anywhere in the application
 signals_ = AppSignals()
 
 app: 'shoWindow' = None
 dir_list: QTreeView = None
 tag_list: 'aBrowser' = None
```

### Comparing `md4_fileo-0.9.47/src/core/app_signals.py` & `md4_fileo-0.9.48/src/core/app_signals.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/bk_ut.py` & `md4_fileo-0.9.48/src/core/bk_ut.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/compact_list.py` & `md4_fileo-0.9.48/src/core/compact_list.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/create_db.py` & `md4_fileo-0.9.48/src/core/create_db.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/db_ut.py` & `md4_fileo-0.9.48/src/core/db_ut.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/drag_drop.py` & `md4_fileo-0.9.48/src/core/drag_drop.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/edit_tree_model2.py` & `md4_fileo-0.9.48/src/core/edit_tree_model2.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/history.py` & `md4_fileo-0.9.48/src/core/history.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/icons.py` & `md4_fileo-0.9.48/src/core/icons.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/linux_menu.py` & `md4_fileo-0.9.48/src/core/linux_menu.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/linux_win.py` & `md4_fileo-0.9.48/src/core/linux_win.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/load_files.py` & `md4_fileo-0.9.48/src/core/load_files.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/low_bk.py` & `md4_fileo-0.9.48/src/core/low_bk.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,15 @@
 
 @pyqtSlot(QModelIndex, QModelIndex)
 def cur_dir_changed(curr_idx: QModelIndex, prev_idx: QModelIndex):
     """
     currentRowChanged signal in dirTree
     :@return: None
     """
+    ag.app.collapse_btn.setChecked(False)
     def new_history_item():
         if ag.hist_folder:
             ag.hist_folder = False
         else:       # new history item
             add_history_item()
         set_current_file(
             curr_idx.data(Qt.ItemDataRole.UserRole).file_row
@@ -371,21 +372,14 @@
 
 def refresh_file_list():
     if ag.mode is ag.appMode.DIR:
         show_folder_files()
     else:
         filtered_files()
 
-def populate_file_list():
-    if ag.mode is ag.appMode.DIR:
-        ag.hist_folder = True
-        _history_folder(ag.history.get_current())
-    else:             # appMode.FILTER or appMode.FILTER_SETUP
-        filtered_files()
-
 @pyqtSlot()
 def to_prev_folder():
     branch = ag.history.prev_dir()
     go_to_history_folder(branch)
 
 @pyqtSlot()
 def to_next_folder():
@@ -606,15 +600,14 @@
         dir_idx = ag.dir_list.currentIndex()
         dir_dat: ag.DirData = dir_idx.data(Qt.ItemDataRole.UserRole)
         return dir_dat.id
 
     return db_ut.get_dir_id_for_file(file)
 
 def post_delete_file(row: int):
-    # populate_file_list()
     refresh_file_list()
     model = ag.file_list.model()
     row -= int(row >= model.rowCount())
 
     set_current_file(row)
 #endregion
```

### Comparing `md4_fileo-0.9.47/src/core/sho.py` & `md4_fileo-0.9.48/src/core/sho.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/table_model.py` & `md4_fileo-0.9.48/src/core/table_model.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/utils.py` & `md4_fileo-0.9.48/src/core/utils.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/core/win_menu.py` & `md4_fileo-0.9.48/src/core/win_menu.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/main.py` & `md4_fileo-0.9.48/src/main.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/qss/default.param` & `md4_fileo-0.9.48/src/qss/default.param`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/qss/default.qss` & `md4_fileo-0.9.48/src/qss/default.qss`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/qss/search.svg` & `md4_fileo-0.9.48/src/qss/search.svg`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/ui/main.ui` & `md4_fileo-0.9.48/src/ui/main.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/ui/ui_main.py` & `md4_fileo-0.9.48/src/ui/ui_main.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/about.py` & `md4_fileo-0.9.48/src/widgets/about.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/custom_grips.py` & `md4_fileo-0.9.48/src/widgets/custom_grips.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_authors.py` & `md4_fileo-0.9.48/src/widgets/file_authors.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_data.py` & `md4_fileo-0.9.48/src/widgets/file_data.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_info.py` & `md4_fileo-0.9.48/src/widgets/file_info.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_note.py` & `md4_fileo-0.9.48/src/widgets/file_note.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_note.ui` & `md4_fileo-0.9.48/src/widgets/file_note.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_notes.py` & `md4_fileo-0.9.48/src/widgets/file_notes.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_search.py` & `md4_fileo-0.9.48/src/widgets/file_search.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_search.ui` & `md4_fileo-0.9.48/src/widgets/file_search.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/file_tags.py` & `md4_fileo-0.9.48/src/widgets/file_tags.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/filter_setup.py` & `md4_fileo-0.9.48/src/widgets/filter_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from PyQt6.QtCore import Qt, QDate
 from PyQt6.QtWidgets import QWidget
 
 from ..core import app_globals as ag, low_bk, db_ut
 from .ui_set_filter import Ui_filterSetup
 
+UNIX_EPOCH = 2440588   # julian date of 1970-01-01
+
 def unix_date(ts: float) -> int:
-    unix_epoch = 2440587.5   # julian date of 1970-01-01
-    return int((ts - unix_epoch) * 86400)
+    return int((ts - UNIX_EPOCH) * 86400)
 
 
 class FilterSetup(QWidget):
     def __init__(self, parent: QWidget = None) -> None:
         super().__init__(parent)
 
         self.ui = Ui_filterSetup()
```

### Comparing `md4_fileo-0.9.47/src/widgets/find_files.py` & `md4_fileo-0.9.48/src/widgets/find_files.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/fold_container.py` & `md4_fileo-0.9.48/src/widgets/fold_container.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/fold_container.ui` & `md4_fileo-0.9.48/src/widgets/fold_container.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/foldable.py` & `md4_fileo-0.9.48/src/widgets/foldable.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/foldable.ui` & `md4_fileo-0.9.48/src/widgets/foldable.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/locations.py` & `md4_fileo-0.9.48/src/widgets/locations.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/notes.ui` & `md4_fileo-0.9.48/src/widgets/notes.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/open_db.py` & `md4_fileo-0.9.48/src/widgets/open_db.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/open_db.ui` & `md4_fileo-0.9.48/src/widgets/open_db.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/preferencies.py` & `md4_fileo-0.9.48/src/widgets/preferencies.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/set_filter.ui` & `md4_fileo-0.9.48/src/widgets/set_filter.ui`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/ui_file_note.py` & `md4_fileo-0.9.48/src/widgets/ui_file_note.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/ui_file_search.py` & `md4_fileo-0.9.48/src/widgets/ui_file_search.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/ui_fold_container.py` & `md4_fileo-0.9.48/src/widgets/ui_fold_container.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/ui_foldable.py` & `md4_fileo-0.9.48/src/widgets/ui_foldable.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/ui_notes.py` & `md4_fileo-0.9.48/src/widgets/ui_notes.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/ui_open_db.py` & `md4_fileo-0.9.48/src/widgets/ui_open_db.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/ui_set_filter.py` & `md4_fileo-0.9.48/src/widgets/ui_set_filter.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/src/widgets/workers.py` & `md4_fileo-0.9.48/src/widgets/workers.py`

 * *Files identical despite different names*

### Comparing `md4_fileo-0.9.47/setup.py` & `md4_fileo-0.9.48/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'qtawesome>=1.2.2,<2.0.0']
 
 extras_require = \
 {':sys_platform == "windows"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'md4-fileo',
-    'version': '0.9.47',
+    'version': '0.9.48',
     'description': 'Yet another file organizer',
-    'long_description': '# Fileo\n\nThis application is about the files, your files.\n\nFileo[fɑɪlɔ] - could be FileOrganizer, but that doesn\'t matter.\n\nThe graphical interface is shown in the image below.\n\n![fileo](https://github.com/Michal-D4/fileo/raw/main/img/fileo.jpg)\n\n## The GUI elements:\n\n1. shows application mode\n2. the button to display menu to hide/show the widgets("Folders", "Tags", "File Extensions", "Authors") on the left pane. All menu items checked in the image &ndash; this means that all widgets are visible.\n3. the name of current file\n4. a button to search files by name, and a button to select fields to be visible in the file list\n5. a group of buttons for working with the folder tree: previous-next folder in the history of visited folders; show hidden folder; collapse all branches/expand the last branch\n6. the left toolbar, it contains the following buttons from top to bottom:\n   1. button to chose/create the data base file\n   2. switch to "DIR" mode, the file list displays files from the current folder\n   3. switch to the "FILTER" mode, the file list displays files according to the filter settings\n   4. open filter settings dialog, switch to "FILTER_SETUP" mode\n   5. open a dialog to upload files to the application from  the selected root folder and all its subfolders\n   6. hide/show left pane\n   7. menu button\n7. list of selected files (by filter, folder, etc.)\n8. current database name\n9. folder tree branch from root to current folder\n10. panel for displaying/editing file data: comments (notes), tags, authors (for books), links (links to a file can be located in several folders).\n\nThe application works in three main modes: DIR, FILTER and FILTER_SETUP. In DIR mode, files are selected by the current directory in the "Folders" widget.\n\nIn FILTER mode, the list of files depends on the filter options set in FILTER_SETUP mode. The filter may depend on the selected folders, selected tags, and selected authors in the boxes in the left pane. In FILTER_SETUP mode, the list of files does not change when changing the selected folders, tags, authors. But in FILTER mode, any changes are immediately displayed in the list of files.\n\n## How it\'s done\n\nAs said, the app is about files. Files have a number of attributes:\n\n1. name\n2. path, the user practically does not see it, only by opening the directory or copying the full file name and on the "File Information" page\n3. file extension\n4. tags\n5. rating\n6. author(s) - usually for books\n7. dates of:\n    1. modification\n    2. reading\n    3. creation\n    4. publication (books)\n8. rating\n9. file opened (times)\n10. size in bytes\n11. number of pages - usually for books\n\nThe following attributes are used in filter: all dates (but only one can be used at a time), extension, tags, rating, authors, and folder which was intentionally not included in the file attributes.\n\nFolders are not associated with file system directories, the path is used for that. You can freely create, move, copy and delete folders in the folder tree, the files will remain intact. You can, for example, create multiple folder hierarchies, this can be handy. Of course, if you delete all folders it will be impossible to access files using folder tree, but they remain accessible by filter. The next time the **`@@Lost`** folder will appear, it can be used to access files that are not in any other folder.\nYou can also *copy/move files from one folder to another*. **Copying** is done by dragging *with the left mouse button pressed*, dragging *with the right mouse button pressed* allows you to choose whether to **move** or **copy** *selected files*.\n\n\n\n## How it works\n\n### How to add files?\n\nThere are two method to add files:\n\n1. Open "Search for files..." dialog with the button ![image-20230210145215938](https://github.com/Michal-D4/fileo/raw/main/img/image-20230210145215938.png)\n\n   ![image-20230210145404623](https://github.com/Michal-D4/fileo/raw/main/img/image-20230210145404623.png)\n\n2. drag files from the file explorer (or similar application) to the folder in the folder tree.\n\n> **Note**. Scanning the file system can be quite lengthy, so it is performed in a separate thread.\n> The red circle in the lower left corner is a sign that the thread is working:\n>\n> ![image-20230213184306153](https://github.com/Michal-D4/fileo/raw/main/img/image-20230213184306153.png)\n>\n> Only one background thread can run at a time - this is the design of the application. The user interface is not blocking but you should avoid to perform operation that make changes in the database, for example, drag-drop operations. But you can change the list of files by changing a current folder or filter, or you can open files.\n\n3. You can export the selected files (with all their attributes) from the database using the context menu of the file list:\n\n   ![export-files](https://github.com/Michal-D4/fileo/raw/main/img/export-files.jpg)\n\n   and then import them to another database\n\n   ![import-files](https://github.com/Michal-D4/fileo/raw/main/img/import-files.jpg)\n\n   to the folder "New folder" in this case.\n\n### How to work with filters\n\nFirst you should setup the filter:\n\n![image-20230213185910924](https://github.com/Michal-D4/fileo/raw/main/img/image-20230213185910924.png)\n\nWith the filter set in the picture, the list of files will include files from the any of `DB`, `ML` or `Rust` folders that have at least one of the `Math`, `ML` or `package` tags, have a rating higher than 4 and are open after `2022-09-14`.\n\n> **Note.** Here "after" and "before" include the date in the input fields 2022-09-14 and 2022-11-14. That is, if "after" and "before" are the same, then the filter will show files with this date.\n\nThe Apply button applies a specified filter without closing the Filter Setup dialog box.\n\nThe Done button applies the filter, closes the dialog, and switches the application to "**Filter Mode**". In this mode, when you change the selection in any of the fields on the left panel (Folders, Tags, Extensions, Authors), the list of files immediately changes.\n\n### How to find files by name\n\n![image-20230428203253627](https://github.com/Michal-D4/fileo/raw/main/img/find_file.jpg)\n\nThe search is performed by pressing the Enter key. "Aa" is a case sensitive search, if checked, "ab" - exact search, but you can use wildcards: "*" - any number of any letters, or "?" - any single letter.\n\n### How to make notes to the file\n\n![fileo-comments](https://github.com/Michal-D4/fileo/raw/main/img/file-notes.jpg)\n\n1. "+"  plus button - add new note and open it in the editor\n6. "x" button - delete the note\n8.  the button to open the note in the editor\n\n#### Note editor\n\n![edit-comment](https://github.com/Michal-D4/fileo/raw/main/img/edit-comment.jpg)\n\n1. the save changes button\n2. the button to discard changes\n\nNote is a markdown text. You can insert web links here, but the links to files in the application are not implemented (and not planned yet)\n\n### Tag selector\n\n![tag-selector](https://github.com/Michal-D4/fileo/raw/main/img/tag-selector.jpg)\n\n1. The list of tags associated with the current file. You can input here a list of tags separated by commas. *It is the only place where the new tag can be created.* The new tags will appear in the list 2 and 4.\n2. The list of tags. The tags selected in this list apply to the file filter.\n3. The context menu in the list of tags. Selected tags are highlighted (\'Linux\' and \'package\'). The tag  \'package\' is a current tag (last selected).\n4. The tag selector. The tags selected here will appear in the list 1.\n\n### Author selector\n\n![author-selector](https://github.com/Michal-D4/fileo/raw/main/img/author-selector.jpg)\n\n1. The list of authors associated with the current file. You can input here a list of authors separated by commas (in square brackets if author name contains comma as in "Vaughan, Lee", otherwise it may be entered without brackets, but new authors without brackets must be in the end of list). It is the only place where the new author can be created. The new authors will appear in the list 2 and 4.\n2. The list of authors. The authors selected in this list apply to the file filter.\n3. The context menu in the list of authors. The current tag is highlighted - "Vijay  Pande" in this case.\n4. The author selector. The authors selected here will appear in the list 1.\n\n### Locations\n\n![Locations](https://github.com/Michal-D4/fileo/raw/main/img/Locations.jpg)\n\n1-4 are locations of the current file, 5 is a context menu.\n\nThe location marked with bullet is a current location.\n\nAll 4 locations end with the Poetry folder. This means that the file exists only in this folder (Poetry), the folder Poetry is presented in 4 branches. That\'s why the file has 4 locations.\n\nThe letters "L" and "H" in brackets means "Link" and "Hidden". "Link" and "Hidden" are attributes of folder. For example, the folder "fileo" in the path 2 is a link to the folder "fileo"[^1] in the path 1; the folder "A folder"  in folder "my" is "Hidden", but it is shown in the picture below because of the "FOLDERS" widget is in "Show hidden folders" mode:\n\n![Folders](https://github.com/Michal-D4/fileo/raw/main/img/Folders.jpg)\n\n1. The current folder (Poetry).\n2. The check box. It is used to switch the "FOLDERS" widget to the "Show hidden folders" mode. The folders "@@Lost" and "Linux" are hidden; "A folder" and "fileo" in the folder "my" are links. The only difference between folder and link to it is that when you delete folder all its links and all its children will be deleted too, whereas deletion of any link of folder does not impact any other folder.\n3. The current file. "Environment Variables in Linux.md"\n\n[^1]: A folder link always has the same name as the folder itself, because the link is a simple pair of folder IDs: the first is the folder ID, the second is the parent folder ID. A folder can have many parent folders. The first parent is set when the folder is created, all the others are set when the folder is copied to another folder. This other folder becomes its parent. \n\n### File info\n\n![file-info](https://github.com/Michal-D4/fileo/raw/main/img/file-info.jpg)\n\nThe "File rating" and "Pages" can be edited here. But they also can be edited directly in the file list if visible:\n\n![file-list-fields](https://github.com/Michal-D4/fileo/raw/main/img/file-list-fields.jpg)\n\n1. The file list\n2. Menu to select fields visible in the file list. The checked fields are visible, the field "File Name" is always visible.\n\n### File operations\n\n\n\n![file_context_menu](https://github.com/Michal-D4/fileo/raw/main/img/file_context_menu.png)\n\nAlmost all operations with files are shown in the context menu on the picture.\n\nBesides them you can copy / move files from one folder to another.\n\nYou can also open files by double clicking on "File name". If the file is executable, it will be executed, not opened. Thus, the application can be used as a "Start Menu", it can be even more convenient than the standard "Start Menu".\n\n> **Note:** If you delete a file from a folder, the file will still remain in the DB, even if you delete it from all folders, you can find it by searching by name or part of the name, or with a filter, or at least it will appear in (hidden) folder "@@Lost".\n> If you delete a file from the DB, it will be deleted from all folders, and all notes for this file and its links to tags and authors will be lost.',
+    'long_description': '# Fileo\n\nThis application is about the files, your files.\n\nFileo[fɑɪlɔ] - could be FileOrganizer, but that doesn\'t matter.\n\nThe graphical interface is shown in the image below.\n\n![fileo](https://github.com/Michal-D4/fileo/raw/main/img/fileo.jpg)\n\n## The GUI elements:\n\n1. shows application mode\n2. the button to display menu to hide/show the widgets("Folders", "Tags", "File Extensions", "Authors") on the left pane. All menu items checked in the image &ndash; this means that all widgets are visible.\n3. the name of current file\n4. a button to search files by name, and a button to select fields to be visible in the file list\n5. a group of buttons for working with the folder tree: previous-next folder in the history of visited folders; show hidden folder; collapse all branches/expand the last branch\n6. the left toolbar, it contains the following buttons from top to bottom:\n   1. button to chose/create the data base file\n   2. switch to "DIR" mode, the file list displays files from the current folder\n   3. switch to the "FILTER" mode, the file list displays files according to the filter settings\n   4. open filter settings dialog, switch to "FILTER_SETUP" mode\n   5. open a dialog to upload files to the application from  the selected root folder and all its subfolders\n   6. hide/show left pane\n   7. menu button\n7. list of selected files (by filter, folder, etc.)\n8. current database name\n9. folder tree branch from root to current folder\n10. panel for displaying/editing file data: notes, tags, authors (for books), links (links to a file locations, file can be located in several folders).\n\nThe application works in three main modes: DIR, FILTER and FILTER_SETUP. In DIR mode, files are selected by the current directory in the "Folders" widget.\n\nIn FILTER mode, the list of files depends on the filter options set in FILTER_SETUP mode. The filter may depend on the selected folders, selected tags, and selected authors in the boxes in the left pane. In FILTER_SETUP mode, the list of files does not change when changing the selected folders, tags, authors. But in FILTER mode, any changes are immediately displayed in the list of files.\n\n## How it\'s done\n\nAs said, the app is about files. Files have a number of attributes:\n\n1. name\n2. path, the user practically does not see it, only by opening the directory or copying the full file name and on the "File Info" page\n3. file extension\n4. tags\n5. rating\n6. author(s) - usually for books\n7. dates of:\n    1. modification\n    2. reading\n    3. creation\n    4. publication (books)\n    5. date of last created/modified note to the file\n8. rating\n9. file opened (times)\n10. size in bytes\n11. number of pages - usually for books\n\nThe following attributes are used in filter: all dates (but only one can be used at a time), extension, tags, rating, authors, and folder which was intentionally not included in the file attributes.\n\nFolders are not associated with file system directories, the path is used for that. You can freely create, move, copy and delete folders in the folder tree, the files will remain intact. You can, for example, create multiple folder hierarchies, this can be handy. Of course, if you delete all folders it will be impossible to access files using folder tree, but they remain accessible by filter. The next time the **`@@Lost`** folder will appear, it can be used to access files that are not in any other folder.\nYou can also *copy/move files from one folder to another*  by dragging *with the left or right mouse button pressed*.\n\n\n\n## How it works\n\n### How to add files?\n\nThere are two method to add files:\n\n1. Open "Search for files..." dialog with the button ![image-20230210145215938](https://github.com/Michal-D4/fileo/raw/main/img/image-20230210145215938.png)\n\n   ![image-20230210145404623](https://github.com/Michal-D4/fileo/raw/main/img/image-20230210145404623.png)\n\n2. drag files from the file explorer (or similar application) to the folder in the folder tree.\n\n> **Note**. Scanning the file system can be quite lengthy, so it is performed in a separate thread.\n> The red circle in the lower left corner is a sign that the thread is working:\n>\n> ![image-20230213184306153](https://github.com/Michal-D4/fileo/raw/main/img/image-20230213184306153.png)\n>\n> Only one background thread can run at a time - this is the design of the application. The user interface is not blocking but you should avoid to perform operation that make changes in the database, for example, drag-drop operations. But you can change the list of files by changing a current folder or filter, or you can open files.\n\n3. You can export the selected files (with all their attributes) from the database using the context menu of the file list:\n\n   ![export-files](https://github.com/Michal-D4/fileo/raw/main/img/export-files.jpg)\n\n   and then import them to another database\n\n   ![import-files](https://github.com/Michal-D4/fileo/raw/main/img/import-files.jpg)\n\n   to the folder "New folder" in this case.\n\n### How to work with filters\n\nFirst you should setup the filter:\n\n![image-20230213185910924](https://github.com/Michal-D4/fileo/raw/main/img/image-20230213185910924.png)\n\nWith the filter set in the picture, the list of files will include files from the any of `DB`, `ML` or `Rust` folders that have at least one of the `Math`, `ML` or `package` tags, have a rating higher than 4 and are open after `2022-09-14 00:00:00`. \n\n> **Note.** In case of before &mdash; the date before or equal to `2022-11-14 23:59:59`. \n\nThe Apply button applies a specified filter without closing the Filter Setup dialog box.\n\nThe Done button applies the filter, closes the dialog, and switches the application to "**Filter Mode**". In this mode, when you change the selection in any of the fields on the left panel (Folders, Tags, Extensions, Authors), the list of files immediately changes.\n\n### How to find files by name\n\n![image-20230428203253627](https://github.com/Michal-D4/fileo/raw/main/img/find_file.jpg)\n\nThe search is performed by pressing the Enter key. "Aa" is a case sensitive search, if checked, "ab" - exact search, but you can use wildcards: "*" - any number of any letters, or "?" - any single letter.\n\n### How to make notes to the file\n\n![fileo-comments](https://github.com/Michal-D4/fileo/raw/main/img/file-notes.jpg)\n\n1. "+"  plus button - add new note and open it in the editor\n8.  the button to open the note in the editor\n3. start editing of the note\n4. "x" button - delete the note\n5. external (http) reference, can be open in the system web browser\n\n#### Note editor\n\n![edit-comment](https://github.com/Michal-D4/fileo/raw/main/img/edit-comment.jpg)\n\n1. the save changes button, save changes and close editor\n2. the button to discard changes \n\n> pressing any of these buttons closes the editor\n\nNote is a markdown text. You can insert web links here, but the links to files in the application are not implemented (and not planned yet)\n\n### Tag selector\n\n![tag-selector](https://github.com/Michal-D4/fileo/raw/main/img/tag-selector.jpg)\n\n1. The list of tags associated with the current file. You can input here a list of tags separated by commas. *It is the only place where the new tag can be created.* The new tags will appear in the list 2 and 4.\n2. The list of tags. The tags selected in this list apply to the file filter.\n3. The context menu in the list of tags. Selected tags are highlighted (\'Linux\' and \'package\'). The tag  \'package\' is a current tag (last selected).\n4. The tag selector. The tags selected here will appear in the list 1.\n\n### Author selector\n\n![author-selector](https://github.com/Michal-D4/fileo/raw/main/img/author-selector.jpg)\n\n1. The list of authors associated with the current file. You can input here a list of authors separated by commas (in square brackets if author name contains comma as in "Vaughan, Lee", otherwise it may be entered without brackets, but new authors without brackets must be in the end of list). It is the only place where the new author can be created. The new authors will appear in the list 2 and 4.\n2. The list of authors. The authors selected in this list apply to the file filter.\n3. The context menu in the list of authors. The current tag is highlighted - "Vijay  Pande" in this case.\n4. The author selector. The authors selected here will appear in the list 1.\n\n### Locations\n\n![Locations](https://github.com/Michal-D4/fileo/raw/main/img/Locations.jpg)\n\n1-4 are locations of the current file, 5 is a context menu.\n\nThe location marked with bullet is a current location.\n\nAll 4 locations end with the Poetry folder. This means that the file exists only in this folder (Poetry), the folder Poetry is presented in 4 branches. That\'s why the file has 4 locations.\n\nThe letters "L" and "H" in brackets means "Link" and "Hidden". "Link" and "Hidden" are attributes of folder. For example, the folder "fileo" in the branch 2 is a link to the folder "fileo"[^1] in the branch 1; the folder "A folder"  in folder "my" is "Hidden", but it is shown in the picture below because of the "FOLDERS" widget is in "Show hidden folders" mode:\n\n![Folders](https://github.com/Michal-D4/fileo/raw/main/img/Folders.jpg)\n\n1. The current folder (Poetry).\n2. The check box. It is used to switch the "FOLDERS" widget to the "Show hidden folders" mode. The folders "@@Lost" and "Linux" are hidden; "A folder" and "fileo" in the folder "my" are links. The only difference between folder and link to it is that when you delete folder all its links and all its children will be deleted too, whereas deletion of any link of folder does not impact any other folder.\n3. The current file. "Environment Variables in Linux.md"\n\n[^1]: A folder link always has the same name as the folder itself, because the link is a simple pair of folder IDs: the first is the folder ID, the second is the parent folder ID. A folder can have many parent folders. The first parent is set when the folder is created, all the others are set when the folder is copied to another folder. This other folder becomes its parent. \n\n### File info\n\n![file-info](https://github.com/Michal-D4/fileo/raw/main/img/file-info.jpg)\n\nThe "File rating" and "Pages" can be edited here. But they also can be edited directly in the file list if visible:\n\n![file-list-fields](https://github.com/Michal-D4/fileo/raw/main/img/file-list-fields.jpg)\n\n1. The file list\n2. Menu to select fields visible in the file list. The checked fields are visible, the field "File Name" is always visible.\n\n### File operations\n\n\n\n![file_context_menu](https://github.com/Michal-D4/fileo/raw/main/img/file_context_menu.png)\n\nAlmost all operations with files are shown in the context menu on the picture.\n\nBesides them you can copy / move files from one folder to another.\n\nYou can also open files by double clicking on "File name". If the file is executable, it will be executed, not opened. Thus, the application can be used as a "Start Menu", it can be even more convenient than the standard "Start Menu".\n\n> **Note:** If you delete a file from a folder, the file will still remain in the DB, even if you delete it from all folders, you can find it by searching by name or part of the name, or with a filter, or at least it will appear in (hidden) folder "@@Lost".\n> If you delete a file from the DB, it will be deleted from all folders, and all notes for this file and its links to tags and authors will be lost.',
     'author': 'mihal.d44',
     'author_email': 'mihal.d44@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `md4_fileo-0.9.47/PKG-INFO` & `md4_fileo-0.9.48/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md4-fileo
-Version: 0.9.47
+Version: 0.9.48
 Summary: Yet another file organizer
 Author: mihal.d44
 Author-email: mihal.d44@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -40,44 +40,45 @@
    4. open filter settings dialog, switch to "FILTER_SETUP" mode
    5. open a dialog to upload files to the application from  the selected root folder and all its subfolders
    6. hide/show left pane
    7. menu button
 7. list of selected files (by filter, folder, etc.)
 8. current database name
 9. folder tree branch from root to current folder
-10. panel for displaying/editing file data: comments (notes), tags, authors (for books), links (links to a file can be located in several folders).
+10. panel for displaying/editing file data: notes, tags, authors (for books), links (links to a file locations, file can be located in several folders).
 
 The application works in three main modes: DIR, FILTER and FILTER_SETUP. In DIR mode, files are selected by the current directory in the "Folders" widget.
 
 In FILTER mode, the list of files depends on the filter options set in FILTER_SETUP mode. The filter may depend on the selected folders, selected tags, and selected authors in the boxes in the left pane. In FILTER_SETUP mode, the list of files does not change when changing the selected folders, tags, authors. But in FILTER mode, any changes are immediately displayed in the list of files.
 
 ## How it's done
 
 As said, the app is about files. Files have a number of attributes:
 
 1. name
-2. path, the user practically does not see it, only by opening the directory or copying the full file name and on the "File Information" page
+2. path, the user practically does not see it, only by opening the directory or copying the full file name and on the "File Info" page
 3. file extension
 4. tags
 5. rating
 6. author(s) - usually for books
 7. dates of:
     1. modification
     2. reading
     3. creation
     4. publication (books)
+    5. date of last created/modified note to the file
 8. rating
 9. file opened (times)
 10. size in bytes
 11. number of pages - usually for books
 
 The following attributes are used in filter: all dates (but only one can be used at a time), extension, tags, rating, authors, and folder which was intentionally not included in the file attributes.
 
 Folders are not associated with file system directories, the path is used for that. You can freely create, move, copy and delete folders in the folder tree, the files will remain intact. You can, for example, create multiple folder hierarchies, this can be handy. Of course, if you delete all folders it will be impossible to access files using folder tree, but they remain accessible by filter. The next time the **`@@Lost`** folder will appear, it can be used to access files that are not in any other folder.
-You can also *copy/move files from one folder to another*. **Copying** is done by dragging *with the left mouse button pressed*, dragging *with the right mouse button pressed* allows you to choose whether to **move** or **copy** *selected files*.
+You can also *copy/move files from one folder to another*  by dragging *with the left or right mouse button pressed*.
 
 
 
 ## How it works
 
 ### How to add files?
 
@@ -108,17 +109,17 @@
 
 ### How to work with filters
 
 First you should setup the filter:
 
 ![image-20230213185910924](https://github.com/Michal-D4/fileo/raw/main/img/image-20230213185910924.png)
 
-With the filter set in the picture, the list of files will include files from the any of `DB`, `ML` or `Rust` folders that have at least one of the `Math`, `ML` or `package` tags, have a rating higher than 4 and are open after `2022-09-14`.
+With the filter set in the picture, the list of files will include files from the any of `DB`, `ML` or `Rust` folders that have at least one of the `Math`, `ML` or `package` tags, have a rating higher than 4 and are open after `2022-09-14 00:00:00`. 
 
-> **Note.** Here "after" and "before" include the date in the input fields 2022-09-14 and 2022-11-14. That is, if "after" and "before" are the same, then the filter will show files with this date.
+> **Note.** In case of before &mdash; the date before or equal to `2022-11-14 23:59:59`. 
 
 The Apply button applies a specified filter without closing the Filter Setup dialog box.
 
 The Done button applies the filter, closes the dialog, and switches the application to "**Filter Mode**". In this mode, when you change the selection in any of the fields on the left panel (Folders, Tags, Extensions, Authors), the list of files immediately changes.
 
 ### How to find files by name
 
@@ -127,23 +128,27 @@
 The search is performed by pressing the Enter key. "Aa" is a case sensitive search, if checked, "ab" - exact search, but you can use wildcards: "*" - any number of any letters, or "?" - any single letter.
 
 ### How to make notes to the file
 
 ![fileo-comments](https://github.com/Michal-D4/fileo/raw/main/img/file-notes.jpg)
 
 1. "+"  plus button - add new note and open it in the editor
-6. "x" button - delete the note
 8.  the button to open the note in the editor
+3. start editing of the note
+4. "x" button - delete the note
+5. external (http) reference, can be open in the system web browser
 
 #### Note editor
 
 ![edit-comment](https://github.com/Michal-D4/fileo/raw/main/img/edit-comment.jpg)
 
-1. the save changes button
-2. the button to discard changes
+1. the save changes button, save changes and close editor
+2. the button to discard changes 
+
+> pressing any of these buttons closes the editor
 
 Note is a markdown text. You can insert web links here, but the links to files in the application are not implemented (and not planned yet)
 
 ### Tag selector
 
 ![tag-selector](https://github.com/Michal-D4/fileo/raw/main/img/tag-selector.jpg)
 
@@ -167,15 +172,15 @@
 
 1-4 are locations of the current file, 5 is a context menu.
 
 The location marked with bullet is a current location.
 
 All 4 locations end with the Poetry folder. This means that the file exists only in this folder (Poetry), the folder Poetry is presented in 4 branches. That's why the file has 4 locations.
 
-The letters "L" and "H" in brackets means "Link" and "Hidden". "Link" and "Hidden" are attributes of folder. For example, the folder "fileo" in the path 2 is a link to the folder "fileo"[^1] in the path 1; the folder "A folder"  in folder "my" is "Hidden", but it is shown in the picture below because of the "FOLDERS" widget is in "Show hidden folders" mode:
+The letters "L" and "H" in brackets means "Link" and "Hidden". "Link" and "Hidden" are attributes of folder. For example, the folder "fileo" in the branch 2 is a link to the folder "fileo"[^1] in the branch 1; the folder "A folder"  in folder "my" is "Hidden", but it is shown in the picture below because of the "FOLDERS" widget is in "Show hidden folders" mode:
 
 ![Folders](https://github.com/Michal-D4/fileo/raw/main/img/Folders.jpg)
 
 1. The current folder (Poetry).
 2. The check box. It is used to switch the "FOLDERS" widget to the "Show hidden folders" mode. The folders "@@Lost" and "Linux" are hidden; "A folder" and "fileo" in the folder "my" are links. The only difference between folder and link to it is that when you delete folder all its links and all its children will be deleted too, whereas deletion of any link of folder does not impact any other folder.
 3. The current file. "Environment Variables in Linux.md"
```

