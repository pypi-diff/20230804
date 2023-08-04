# Comparing `tmp/abinitostudio-1.0.4.tar.gz` & `tmp/abinitostudio-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\abinitostudio-1.0.4.tar", last modified: Fri Aug  4 14:07:55 2023, max compression
+gzip compressed data, was "dist\abinitostudio-1.0.5.tar", last modified: Fri Aug  4 14:18:08 2023, max compression
```

## Comparing `abinitostudio-1.0.4.tar` & `abinitostudio-1.0.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:55.000000 abinitostudio-1.0.4/
--rw-rw-rw-   0        0        0     1084 2023-07-31 13:26:19.000000 abinitostudio-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       96 2021-08-03 14:08:19.000000 abinitostudio-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      411 2023-08-04 14:07:55.000000 abinitostudio-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2021-08-06 03:05:42.000000 abinitostudio-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.4/abinitostudio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio/calculation/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.4/abinitostudio/calculation/__init__.py
--rw-rw-rw-   0        0        0    25840 2021-08-02 00:55:16.000000 abinitostudio-1.0.4/abinitostudio/calculation/vasp_calculation.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio/io/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.4/abinitostudio/io/__init__.py
--rw-rw-rw-   0        0        0    20951 2023-07-26 23:35:53.000000 abinitostudio-1.0.4/abinitostudio/io/vasp_io.py
--rw-rw-rw-   0        0        0    59876 2023-07-26 23:10:00.000000 abinitostudio-1.0.4/abinitostudio/myMainWindow.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio/plot/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.4/abinitostudio/plot/__init__.py
--rw-rw-rw-   0        0        0      679 2021-08-05 03:39:45.000000 abinitostudio-1.0.4/abinitostudio/plot/plot_field.py
--rw-rw-rw-   0        0        0     2330 2023-07-27 00:58:33.000000 abinitostudio-1.0.4/abinitostudio/plot/plot_vasp.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio/structure/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.4/abinitostudio/structure/__init__.py
--rw-rw-rw-   0        0        0    35274 2023-07-26 23:37:48.000000 abinitostudio-1.0.4/abinitostudio/structure/plot_structure.py
--rw-rw-rw-   0        0        0     3343 2021-08-02 00:55:55.000000 abinitostudio-1.0.4/abinitostudio/structure/tabdialog.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio/ui/
--rw-rw-rw-   0        0        0    17334 2021-08-02 07:37:44.000000 abinitostudio-1.0.4/abinitostudio/ui/Dialog_DOS.py
--rw-rw-rw-   0        0        0    38630 2021-08-02 08:21:52.000000 abinitostudio-1.0.4/abinitostudio/ui/Dialog_PB.py
--rw-rw-rw-   0        0        0     7633 2021-07-13 07:37:22.000000 abinitostudio-1.0.4/abinitostudio/ui/Dialog_band.py
--rw-rw-rw-   0        0        0    13745 2023-07-26 22:49:46.000000 abinitostudio-1.0.4/abinitostudio/ui/UI.py
--rw-rw-rw-   0        0        0    12159 2021-08-02 08:18:40.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_setting.py
--rw-rw-rw-   0        0        0     8922 2021-08-02 08:20:50.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_test.py
--rw-rw-rw-   0        0        0    31919 2021-08-02 08:20:32.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_DOS.py
--rw-rw-rw-   0        0        0    32252 2021-08-02 08:20:44.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_band.py
--rw-rw-rw-   0        0        0    31944 2021-08-02 08:20:38.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_band_noncal.py
--rw-rw-rw-   0        0        0    25099 2021-08-02 08:20:25.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_phonon.py
--rw-rw-rw-   0        0        0    22764 2021-08-02 08:20:19.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_scf.py
--rw-rw-rw-   0        0        0    22785 2021-08-02 08:20:11.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_scf_noncal.py
--rw-rw-rw-   0        0        0     4585 2021-08-02 08:20:03.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_supercell.py
--rw-rw-rw-   0        0        0    21153 2021-08-02 08:19:54.000000 abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_wannier.py
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.4/abinitostudio/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio.egg-info/
--rw-rw-rw-   0        0        0      411 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1692 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/abinitostudio.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:54.000000 abinitostudio-1.0.4/doc/
--rw-rw-rw-   0        0        0   756022 2021-07-30 07:37:10.000000 abinitostudio-1.0.4/doc/说明文档.pdf
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:55.000000 abinitostudio-1.0.4/examples/
--rw-rw-rw-   0        0        0 12582333 2021-08-01 03:29:39.000000 abinitostudio-1.0.4/examples/CHGCAR
--rw-rw-rw-   0        0        0   300593 2020-07-30 07:58:04.000000 abinitostudio-1.0.4/examples/DOSCAR
--rw-rw-rw-   0        0        0   132487 2019-11-19 12:21:46.000000 abinitostudio-1.0.4/examples/EIGENVAL_CdCl
--rw-rw-rw-   0        0        0     1321 2023-04-21 12:57:23.000000 abinitostudio-1.0.4/examples/POSCAR
--rw-rw-rw-   0        0        0  2888368 2019-11-19 12:21:46.000000 abinitostudio-1.0.4/examples/PROCAR _CdCl
--rw-rw-rw-   0        0        0      291 2021-08-01 03:08:04.000000 abinitostudio-1.0.4/examples/text_ip.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:55.000000 abinitostudio-1.0.4/images/
--rw-rw-rw-   0        0        0     7946 2021-07-08 05:28:12.000000 abinitostudio-1.0.4/images/3d可视.png
--rw-rw-rw-   0        0        0     7103 2021-07-27 09:09:04.000000 abinitostudio-1.0.4/images/DOS.png
--rw-rw-rw-   0        0        0     2541 2021-07-11 06:18:08.000000 abinitostudio-1.0.4/images/band.png
--rw-rw-rw-   0        0        0     3332 2021-07-27 09:08:38.000000 abinitostudio-1.0.4/images/band_noncal.png
--rw-rw-rw-   0        0        0     2218 2021-07-27 09:08:58.000000 abinitostudio-1.0.4/images/phonin.png
--rw-rw-rw-   0        0        0     3762 2021-07-27 09:08:22.000000 abinitostudio-1.0.4/images/scf.png
--rw-rw-rw-   0        0        0     2830 2021-07-27 09:08:28.000000 abinitostudio-1.0.4/images/scf_noncal.png
--rw-rw-rw-   0        0        0    87766 2021-07-30 08:31:34.000000 abinitostudio-1.0.4/images/startup.jpg
--rw-rw-rw-   0        0        0     6280 2021-07-10 11:22:50.000000 abinitostudio-1.0.4/images/vasp.png
--rw-rw-rw-   0        0        0     2468 2021-07-27 09:09:24.000000 abinitostudio-1.0.4/images/wannier.png
--rw-rw-rw-   0        0        0     5090 2021-06-28 05:59:22.000000 abinitostudio-1.0.4/images/关于.png
--rw-rw-rw-   0        0        0     7333 2021-06-28 05:43:40.000000 abinitostudio-1.0.4/images/关闭.png
--rw-rw-rw-   0        0        0     3636 2021-07-08 07:06:54.000000 abinitostudio-1.0.4/images/层级.png
--rw-rw-rw-   0        0        0     2981 2021-06-28 07:05:38.000000 abinitostudio-1.0.4/images/态密度.png
--rw-rw-rw-   0        0        0     5788 2021-07-08 06:57:38.000000 abinitostudio-1.0.4/images/扩胞.png
--rw-rw-rw-   0        0        0     2034 2021-06-28 07:04:50.000000 abinitostudio-1.0.4/images/投影能带.png
--rw-rw-rw-   0        0        0     6657 2021-07-10 04:25:24.000000 abinitostudio-1.0.4/images/测试.png
--rw-rw-rw-   0        0        0     9896 2021-06-28 07:27:34.000000 abinitostudio-1.0.4/images/结构.png
--rw-rw-rw-   0        0        0     2229 2021-06-28 07:04:44.000000 abinitostudio-1.0.4/images/能带.png
--rw-rw-rw-   0        0        0    22484 2021-08-01 09:49:20.000000 abinitostudio-1.0.4/images/能带图.png
--rw-rw-rw-   0        0        0     7906 2021-07-10 04:23:36.000000 abinitostudio-1.0.4/images/设置.png
--rw-rw-rw-   0        0        0     2434 2021-06-28 06:32:52.000000 abinitostudio-1.0.4/images/说明.png
-drwxrwxrwx   0        0        0        0 2023-08-04 14:07:55.000000 abinitostudio-1.0.4/scripts/
--rw-rw-rw-   0        0        0     8707 2021-08-01 03:49:29.000000 abinitostudio-1.0.4/scripts/cal_vasp_single.py
--rw-rw-rw-   0        0        0       42 2023-08-04 14:07:55.000000 abinitostudio-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1283 2023-08-04 14:06:00.000000 abinitostudio-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/
+-rw-rw-rw-   0        0        0     1084 2023-07-31 13:26:19.000000 abinitostudio-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       96 2021-08-03 14:08:19.000000 abinitostudio-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      425 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2021-08-06 03:05:42.000000 abinitostudio-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:07.000000 abinitostudio-1.0.5/abinitostudio/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.5/abinitostudio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/abinitostudio/calculation/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.5/abinitostudio/calculation/__init__.py
+-rw-rw-rw-   0        0        0    25840 2021-08-02 00:55:16.000000 abinitostudio-1.0.5/abinitostudio/calculation/vasp_calculation.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/abinitostudio/io/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.5/abinitostudio/io/__init__.py
+-rw-rw-rw-   0        0        0    20951 2023-07-26 23:35:53.000000 abinitostudio-1.0.5/abinitostudio/io/vasp_io.py
+-rw-rw-rw-   0        0        0    59876 2023-07-26 23:10:00.000000 abinitostudio-1.0.5/abinitostudio/myMainWindow.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/abinitostudio/plot/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.5/abinitostudio/plot/__init__.py
+-rw-rw-rw-   0        0        0      679 2021-08-05 03:39:45.000000 abinitostudio-1.0.5/abinitostudio/plot/plot_field.py
+-rw-rw-rw-   0        0        0     2330 2023-07-27 00:58:33.000000 abinitostudio-1.0.5/abinitostudio/plot/plot_vasp.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/abinitostudio/structure/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.5/abinitostudio/structure/__init__.py
+-rw-rw-rw-   0        0        0    35274 2023-07-26 23:37:48.000000 abinitostudio-1.0.5/abinitostudio/structure/plot_structure.py
+-rw-rw-rw-   0        0        0     3343 2021-08-02 00:55:55.000000 abinitostudio-1.0.5/abinitostudio/structure/tabdialog.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/abinitostudio/ui/
+-rw-rw-rw-   0        0        0    17334 2021-08-02 07:37:44.000000 abinitostudio-1.0.5/abinitostudio/ui/Dialog_DOS.py
+-rw-rw-rw-   0        0        0    38630 2021-08-02 08:21:52.000000 abinitostudio-1.0.5/abinitostudio/ui/Dialog_PB.py
+-rw-rw-rw-   0        0        0     7633 2021-07-13 07:37:22.000000 abinitostudio-1.0.5/abinitostudio/ui/Dialog_band.py
+-rw-rw-rw-   0        0        0    13745 2023-07-26 22:49:46.000000 abinitostudio-1.0.5/abinitostudio/ui/UI.py
+-rw-rw-rw-   0        0        0    12159 2021-08-02 08:18:40.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_setting.py
+-rw-rw-rw-   0        0        0     8922 2021-08-02 08:20:50.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_test.py
+-rw-rw-rw-   0        0        0    31919 2021-08-02 08:20:32.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_DOS.py
+-rw-rw-rw-   0        0        0    32252 2021-08-02 08:20:44.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_band.py
+-rw-rw-rw-   0        0        0    31944 2021-08-02 08:20:38.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_band_noncal.py
+-rw-rw-rw-   0        0        0    25099 2021-08-02 08:20:25.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_phonon.py
+-rw-rw-rw-   0        0        0    22764 2021-08-02 08:20:19.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_scf.py
+-rw-rw-rw-   0        0        0    22785 2021-08-02 08:20:11.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_scf_noncal.py
+-rw-rw-rw-   0        0        0     4585 2021-08-02 08:20:03.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_supercell.py
+-rw-rw-rw-   0        0        0    21153 2021-08-02 08:19:54.000000 abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_wannier.py
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.5/abinitostudio/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/abinitostudio.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-08-04 14:18:07.000000 abinitostudio-1.0.5/abinitostudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1692 2023-08-04 14:18:07.000000 abinitostudio-1.0.5/abinitostudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:18:07.000000 abinitostudio-1.0.5/abinitostudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-08-04 14:18:07.000000 abinitostudio-1.0.5/abinitostudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-04 14:18:07.000000 abinitostudio-1.0.5/abinitostudio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/doc/
+-rw-rw-rw-   0        0        0   756022 2021-07-30 07:37:10.000000 abinitostudio-1.0.5/doc/说明文档.pdf
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/examples/
+-rw-rw-rw-   0        0        0 12582333 2021-08-01 03:29:39.000000 abinitostudio-1.0.5/examples/CHGCAR
+-rw-rw-rw-   0        0        0   300593 2020-07-30 07:58:04.000000 abinitostudio-1.0.5/examples/DOSCAR
+-rw-rw-rw-   0        0        0   132487 2019-11-19 12:21:46.000000 abinitostudio-1.0.5/examples/EIGENVAL_CdCl
+-rw-rw-rw-   0        0        0     1321 2023-04-21 12:57:23.000000 abinitostudio-1.0.5/examples/POSCAR
+-rw-rw-rw-   0        0        0  2888368 2019-11-19 12:21:46.000000 abinitostudio-1.0.5/examples/PROCAR _CdCl
+-rw-rw-rw-   0        0        0      291 2021-08-01 03:08:04.000000 abinitostudio-1.0.5/examples/text_ip.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/images/
+-rw-rw-rw-   0        0        0     7946 2021-07-08 05:28:12.000000 abinitostudio-1.0.5/images/3d可视.png
+-rw-rw-rw-   0        0        0     7103 2021-07-27 09:09:04.000000 abinitostudio-1.0.5/images/DOS.png
+-rw-rw-rw-   0        0        0     2541 2021-07-11 06:18:08.000000 abinitostudio-1.0.5/images/band.png
+-rw-rw-rw-   0        0        0     3332 2021-07-27 09:08:38.000000 abinitostudio-1.0.5/images/band_noncal.png
+-rw-rw-rw-   0        0        0     2218 2021-07-27 09:08:58.000000 abinitostudio-1.0.5/images/phonin.png
+-rw-rw-rw-   0        0        0     3762 2021-07-27 09:08:22.000000 abinitostudio-1.0.5/images/scf.png
+-rw-rw-rw-   0        0        0     2830 2021-07-27 09:08:28.000000 abinitostudio-1.0.5/images/scf_noncal.png
+-rw-rw-rw-   0        0        0    87766 2021-07-30 08:31:34.000000 abinitostudio-1.0.5/images/startup.jpg
+-rw-rw-rw-   0        0        0     6280 2021-07-10 11:22:50.000000 abinitostudio-1.0.5/images/vasp.png
+-rw-rw-rw-   0        0        0     2468 2021-07-27 09:09:24.000000 abinitostudio-1.0.5/images/wannier.png
+-rw-rw-rw-   0        0        0     5090 2021-06-28 05:59:22.000000 abinitostudio-1.0.5/images/关于.png
+-rw-rw-rw-   0        0        0     7333 2021-06-28 05:43:40.000000 abinitostudio-1.0.5/images/关闭.png
+-rw-rw-rw-   0        0        0     3636 2021-07-08 07:06:54.000000 abinitostudio-1.0.5/images/层级.png
+-rw-rw-rw-   0        0        0     2981 2021-06-28 07:05:38.000000 abinitostudio-1.0.5/images/态密度.png
+-rw-rw-rw-   0        0        0     5788 2021-07-08 06:57:38.000000 abinitostudio-1.0.5/images/扩胞.png
+-rw-rw-rw-   0        0        0     2034 2021-06-28 07:04:50.000000 abinitostudio-1.0.5/images/投影能带.png
+-rw-rw-rw-   0        0        0     6657 2021-07-10 04:25:24.000000 abinitostudio-1.0.5/images/测试.png
+-rw-rw-rw-   0        0        0     9896 2021-06-28 07:27:34.000000 abinitostudio-1.0.5/images/结构.png
+-rw-rw-rw-   0        0        0     2229 2021-06-28 07:04:44.000000 abinitostudio-1.0.5/images/能带.png
+-rw-rw-rw-   0        0        0    22484 2021-08-01 09:49:20.000000 abinitostudio-1.0.5/images/能带图.png
+-rw-rw-rw-   0        0        0     7906 2021-07-10 04:23:36.000000 abinitostudio-1.0.5/images/设置.png
+-rw-rw-rw-   0        0        0     2434 2021-06-28 06:32:52.000000 abinitostudio-1.0.5/images/说明.png
+drwxrwxrwx   0        0        0        0 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/scripts/
+-rw-rw-rw-   0        0        0     8707 2021-08-01 03:49:29.000000 abinitostudio-1.0.5/scripts/cal_vasp_single.py
+-rw-rw-rw-   0        0        0       42 2023-08-04 14:18:08.000000 abinitostudio-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1339 2023-08-04 14:17:40.000000 abinitostudio-1.0.5/setup.py
```

### Comparing `abinitostudio-1.0.4/LICENSE` & `abinitostudio-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/README.md` & `abinitostudio-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/calculation/vasp_calculation.py` & `abinitostudio-1.0.5/abinitostudio/calculation/vasp_calculation.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/io/vasp_io.py` & `abinitostudio-1.0.5/abinitostudio/io/vasp_io.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/myMainWindow.py` & `abinitostudio-1.0.5/abinitostudio/myMainWindow.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/plot/plot_field.py` & `abinitostudio-1.0.5/abinitostudio/plot/plot_field.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/plot/plot_vasp.py` & `abinitostudio-1.0.5/abinitostudio/plot/plot_vasp.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/structure/plot_structure.py` & `abinitostudio-1.0.5/abinitostudio/structure/plot_structure.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/structure/tabdialog.py` & `abinitostudio-1.0.5/abinitostudio/structure/tabdialog.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/Dialog_DOS.py` & `abinitostudio-1.0.5/abinitostudio/ui/Dialog_DOS.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/Dialog_PB.py` & `abinitostudio-1.0.5/abinitostudio/ui/Dialog_PB.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/Dialog_band.py` & `abinitostudio-1.0.5/abinitostudio/ui/Dialog_band.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_setting.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_setting.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_test.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_test.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_DOS.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_DOS.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_band.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_band.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_band_noncal.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_band_noncal.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_phonon.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_phonon.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_scf.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_scf.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_scf_noncal.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_scf_noncal.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_supercell.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_supercell.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio/ui/UI_vasp_wannier.py` & `abinitostudio-1.0.5/abinitostudio/ui/UI_vasp_wannier.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/abinitostudio.egg-info/SOURCES.txt` & `abinitostudio-1.0.5/abinitostudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/doc/说明文档.pdf` & `abinitostudio-1.0.5/doc/说明文档.pdf`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/examples/CHGCAR` & `abinitostudio-1.0.5/examples/CHGCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/examples/DOSCAR` & `abinitostudio-1.0.5/examples/DOSCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/examples/EIGENVAL_CdCl` & `abinitostudio-1.0.5/examples/EIGENVAL_CdCl`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/examples/POSCAR` & `abinitostudio-1.0.5/examples/POSCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/examples/PROCAR _CdCl` & `abinitostudio-1.0.5/examples/PROCAR _CdCl`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/3d可视.png` & `abinitostudio-1.0.5/images/3d可视.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/DOS.png` & `abinitostudio-1.0.5/images/DOS.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/band.png` & `abinitostudio-1.0.5/images/band.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/band_noncal.png` & `abinitostudio-1.0.5/images/band_noncal.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/phonin.png` & `abinitostudio-1.0.5/images/phonin.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/scf.png` & `abinitostudio-1.0.5/images/scf.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/scf_noncal.png` & `abinitostudio-1.0.5/images/scf_noncal.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/startup.jpg` & `abinitostudio-1.0.5/images/startup.jpg`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/vasp.png` & `abinitostudio-1.0.5/images/vasp.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/wannier.png` & `abinitostudio-1.0.5/images/wannier.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/关于.png` & `abinitostudio-1.0.5/images/关于.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/关闭.png` & `abinitostudio-1.0.5/images/关闭.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/层级.png` & `abinitostudio-1.0.5/images/层级.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/态密度.png` & `abinitostudio-1.0.5/images/态密度.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/扩胞.png` & `abinitostudio-1.0.5/images/扩胞.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/投影能带.png` & `abinitostudio-1.0.5/images/投影能带.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/测试.png` & `abinitostudio-1.0.5/images/测试.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/结构.png` & `abinitostudio-1.0.5/images/结构.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/能带.png` & `abinitostudio-1.0.5/images/能带.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/能带图.png` & `abinitostudio-1.0.5/images/能带图.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/设置.png` & `abinitostudio-1.0.5/images/设置.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/images/说明.png` & `abinitostudio-1.0.5/images/说明.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/scripts/cal_vasp_single.py` & `abinitostudio-1.0.5/scripts/cal_vasp_single.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.4/setup.py` & `abinitostudio-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 import os
 
 
 setup(name="abinitostudio",
-    version="1.0.4",
+    version="1.0.5",
     description="A studio for first-principles calculations.",
     long_description="This is a long description.",
     author="Pan Zhou, Xin Lu and Li Zhongsun",
     author_email="zhoupan71234@xtu.edu.cn",
     classifiers=["Development Status :: 3 - Alpha",'Programming Language :: Python',],
+#    packages=find_packages()
     packages=['abinitostudio',
-			  'abinitostudio.calculation',
+ 			  'abinitostudio.calculation',
               'abinitostudio.io', 
               'abinitostudio.plot', 
               'abinitostudio.structure', 
-              'abinitostudio.ui',],
+              'abinitostudio.ui',
+              'images'],
     scripts=[
         'scripts/cal_vasp_single.py',
     ],
 	include_package_data = True,
- 	package_data={'abinitostudio': ['images/*.png']
+ 	package_data={'': ['images/*.png']
     },
     # data_files=[('images', ['images/*.png']),
     #             ('abinitostudio.doc', ['doc/*']),
     #             ('abinitostudio.examples', ['examples/*'])],
     install_requires=[
 		'paramiko==2.7.1',
 		'jumpssh==1.6.5',
```

