# Comparing `tmp/GenIce2-2.1b3.tar.gz` & `tmp/GenIce2-2.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenIce2-2.1b3.tar", last modified: Wed Mar 24 10:25:56 2021, max compression
+gzip compressed data, was "GenIce2-2.1b4.tar", last modified: Tue May 11 11:37:45 2021, max compression
```

## Comparing `GenIce2-2.1b3.tar` & `GenIce2-2.1b4.tar`

### file list

```diff
@@ -1,389 +1,389 @@
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.098003 GenIce2-2.1b3/
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.023966 GenIce2-2.1b3/GenIce2.egg-info/
--rw-r--r--   0 matto      (505) staff       (20)    58401 2021-03-24 10:25:55.000000 GenIce2-2.1b3/GenIce2.egg-info/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)     9997 2021-03-24 10:25:55.000000 GenIce2-2.1b3/GenIce2.egg-info/SOURCES.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2021-03-24 10:25:55.000000 GenIce2-2.1b3/GenIce2.egg-info/dependency_links.txt
--rw-r--r--   0 matto      (505) staff       (20)       89 2021-03-24 10:25:55.000000 GenIce2-2.1b3/GenIce2.egg-info/entry_points.txt
--rw-r--r--   0 matto      (505) staff       (20)       87 2021-03-24 10:25:55.000000 GenIce2-2.1b3/GenIce2.egg-info/requires.txt
--rw-r--r--   0 matto      (505) staff       (20)        8 2021-03-24 10:25:55.000000 GenIce2-2.1b3/GenIce2.egg-info/top_level.txt
--rw-r--r--   0 matto      (505) staff       (20)       88 2021-03-23 11:10:14.000000 GenIce2-2.1b3/MANIFEST.in
--rw-r--r--   0 matto      (505) staff       (20)    58401 2021-03-24 10:25:56.099492 GenIce2-2.1b3/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)    51327 2021-03-23 10:50:50.000000 GenIce2-2.1b3/README.md
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.025649 GenIce2-2.1b3/genice2/
--rw-r--r--   0 matto      (505) staff       (20)     4064 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/CIF.py
--rw-r--r--   0 matto      (505) staff       (20)     3243 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/FrankKasper.py
--rw-r--r--   0 matto      (505) staff       (20)       46 2021-03-24 08:45:32.000000 GenIce2-2.1b3/genice2/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     2936 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/alkyl.py
--rw-r--r--   0 matto      (505) staff       (20)     9293 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/analice.py
--rw-r--r--   0 matto      (505) staff       (20)     3468 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/cell.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.025988 GenIce2-2.1b3/genice2/cli/
--rw-r--r--   0 matto      (505) staff       (20)     1513 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/cli/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     6765 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/cli/analice.py
--rw-r--r--   0 matto      (505) staff       (20)     9593 2021-03-19 13:37:00.000000 GenIce2-2.1b3/genice2/cli/genice.py
--rw-r--r--   0 matto      (505) staff       (20)      916 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/decorators.py
--rw-r--r--   0 matto      (505) staff       (20)    21248 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/digraph.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.030415 GenIce2-2.1b3/genice2/formats/
--rw-r--r--   0 matto      (505) staff       (20)     1953 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/_KG.py
--rw-r--r--   0 matto      (505) staff       (20)      301 2021-03-19 13:13:23.000000 GenIce2-2.1b3/genice2/formats/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     6919 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/_ringstat.py
--rw-r--r--   0 matto      (505) staff       (20)     1420 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/c.py
--rw-r--r--   0 matto      (505) staff       (20)     2231 2021-03-19 13:49:59.000000 GenIce2-2.1b3/genice2/formats/cif.py
--rw-r--r--   0 matto      (505) staff       (20)     2121 2021-03-19 13:50:38.000000 GenIce2-2.1b3/genice2/formats/cif2.py
--rw-r--r--   0 matto      (505) staff       (20)     1420 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/com.py
--rw-r--r--   0 matto      (505) staff       (20)      944 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/d.py
--rw-r--r--   0 matto      (505) staff       (20)      944 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/digraph.py
--rw-r--r--   0 matto      (505) staff       (20)     2008 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/e.py
--rw-r--r--   0 matto      (505) staff       (20)     2008 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/euler.py
--rw-r--r--   0 matto      (505) staff       (20)     1333 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/exmol.py
--rw-r--r--   0 matto      (505) staff       (20)     1603 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/exyz.py
--rw-r--r--   0 matto      (505) staff       (20)     2902 2021-03-19 13:47:53.000000 GenIce2-2.1b3/genice2/formats/g.py
--rw-r--r--   0 matto      (505) staff       (20)      968 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/graph.py
--rw-r--r--   0 matto      (505) staff       (20)     2902 2021-03-19 13:47:53.000000 GenIce2-2.1b3/genice2/formats/gromacs.py
--rw-r--r--   0 matto      (505) staff       (20)     1494 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/m.py
--rw-r--r--   0 matto      (505) staff       (20)     1494 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/mdv_au.py
--rw-r--r--   0 matto      (505) staff       (20)     1494 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/mdview.py
--rw-r--r--   0 matto      (505) staff       (20)      418 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/null.py
--rw-r--r--   0 matto      (505) staff       (20)     4801 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/o.py
--rw-r--r--   0 matto      (505) staff       (20)     4801 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/openscad.py
--rw-r--r--   0 matto      (505) staff       (20)     6676 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/p.py
--rw-r--r--   0 matto      (505) staff       (20)     3531 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/povray.py
--rw-r--r--   0 matto      (505) staff       (20)     6676 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/python.py
--rw-r--r--   0 matto      (505) staff       (20)     2067 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/q.py
--rw-r--r--   0 matto      (505) staff       (20)     2067 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/quaternion.py
--rw-r--r--   0 matto      (505) staff       (20)     1246 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/r.py
--rw-r--r--   0 matto      (505) staff       (20)     3937 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/raw.py
--rw-r--r--   0 matto      (505) staff       (20)     1246 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/rcom.py
--rw-r--r--   0 matto      (505) staff       (20)     6676 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/reshape.py
--rw-r--r--   0 matto      (505) staff       (20)     6452 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/formats/rings.py
--rw-r--r--   0 matto      (505) staff       (20)     1723 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/towhee.py
--rw-r--r--   0 matto      (505) staff       (20)     1148 2021-03-19 14:21:49.000000 GenIce2-2.1b3/genice2/formats/xyz.py
--rw-r--r--   0 matto      (505) staff       (20)     4690 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/y.py
--rw-r--r--   0 matto      (505) staff       (20)     4690 2021-03-19 13:39:38.000000 GenIce2-2.1b3/genice2/formats/yaplot.py
--rw-r--r--   0 matto      (505) staff       (20)    46378 2021-03-19 14:25:38.000000 GenIce2-2.1b3/genice2/genice.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.091696 GenIce2-2.1b3/genice2/lattices/
--rw-r--r--   0 matto      (505) staff       (20)     1372 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/0.py
--rw-r--r--   0 matto      (505) staff       (20)     1549 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/11.py
--rw-r--r--   0 matto      (505) staff       (20)     3408 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/115_2_114.py
--rw-r--r--   0 matto      (505) staff       (20)      934 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/11_2_15848.py
--rw-r--r--   0 matto      (505) staff       (20)     1245 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/12.py
--rw-r--r--   0 matto      (505) staff       (20)     3747 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/12_1_11.py
--rw-r--r--   0 matto      (505) staff       (20)      846 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/12_2_29187.py
--rw-r--r--   0 matto      (505) staff       (20)      847 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/12_2_32449.py
--rw-r--r--   0 matto      (505) staff       (20)     2161 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/13.py
--rw-r--r--   0 matto      (505) staff       (20)     2692 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/144_2_7301.py
--rw-r--r--   0 matto      (505) staff       (20)      933 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/14_2_48453.py
--rw-r--r--   0 matto      (505) staff       (20)     3815 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/151_2_4949650.py
--rw-r--r--   0 matto      (505) staff       (20)      976 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/152_2_118474.py
--rw-r--r--   0 matto      (505) staff       (20)     2168 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/153_2_155471.py
--rw-r--r--   0 matto      (505) staff       (20)      848 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/15_2_201714.py
--rw-r--r--   0 matto      (505) staff       (20)     8157 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/16.py
--rw-r--r--   0 matto      (505) staff       (20)     1119 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/169_2_10608.py
--rw-r--r--   0 matto      (505) staff       (20)     1111 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/169_2_7915.py
--rw-r--r--   0 matto      (505) staff       (20)     1377 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/17.py
--rw-r--r--   0 matto      (505) staff       (20)     1638 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/176_2_5256.py
--rw-r--r--   0 matto      (505) staff       (20)      951 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/1c.py
--rw-r--r--   0 matto      (505) staff       (20)      936 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/1h.py
--rw-r--r--   0 matto      (505) staff       (20)      794 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/1h_unit.py
--rw-r--r--   0 matto      (505) staff       (20)     1695 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/2.py
--rw-r--r--   0 matto      (505) staff       (20)     1321 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/207_1_4435.py
--rw-r--r--   0 matto      (505) staff       (20)      845 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/20_2_26425.py
--rw-r--r--   0 matto      (505) staff       (20)      843 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/20_2_28176.py
--rw-r--r--   0 matto      (505) staff       (20)     1859 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/2D3.py
--rw-r--r--   0 matto      (505) staff       (20)      756 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/2_2_342692.py
--rw-r--r--   0 matto      (505) staff       (20)     4835 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/2_2_623457.py
--rw-r--r--   0 matto      (505) staff       (20)     2742 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/2d.py
--rw-r--r--   0 matto      (505) staff       (20)      981 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/3.py
--rw-r--r--   0 matto      (505) staff       (20)     8938 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/4.py
--rw-r--r--   0 matto      (505) staff       (20)    30989 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/4R.py
--rw-r--r--   0 matto      (505) staff       (20)     1358 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/5.py
--rw-r--r--   0 matto      (505) staff       (20)     1300 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/53_3_726600.py
--rw-r--r--   0 matto      (505) staff       (20)     1110 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/58_2_511.py
--rw-r--r--   0 matto      (505) staff       (20)     3974 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/5R.py
--rw-r--r--   0 matto      (505) staff       (20)     1373 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/6.py
--rw-r--r--   0 matto      (505) staff       (20)     1297 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/61_2_8842.py
--rw-r--r--   0 matto      (505) staff       (20)     2148 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/67_2_1444.py
--rw-r--r--   0 matto      (505) staff       (20)     3450 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/67_2_1563.py
--rw-r--r--   0 matto      (505) staff       (20)      773 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/6h.py
--rw-r--r--   0 matto      (505) staff       (20)     1432 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/7.py
--rw-r--r--   0 matto      (505) staff       (20)     2136 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/8.py
--rw-r--r--   0 matto      (505) staff       (20)      832 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/84_2_1419.py
--rw-r--r--   0 matto      (505) staff       (20)     1178 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/9.py
--rw-r--r--   0 matto      (505) staff       (20)     1301 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/91_2_8335121.py
--rw-r--r--   0 matto      (505) staff       (20)     1404 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/A.py
--rw-r--r--   0 matto      (505) staff       (20)     3438 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/A15.py
--rw-r--r--   0 matto      (505) staff       (20)     1165 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ACO.py
--rw-r--r--   0 matto      (505) staff       (20)     1333 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/B.py
--rw-r--r--   0 matto      (505) staff       (20)     3669 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/BSV.py
--rw-r--r--   0 matto      (505) staff       (20)     5578 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/C14.py
--rw-r--r--   0 matto      (505) staff       (20)     9522 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/C15.py
--rw-r--r--   0 matto      (505) staff       (20)     9852 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/C36.py
--rw-r--r--   0 matto      (505) staff       (20)    57115 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/CRN1.py
--rw-r--r--   0 matto      (505) staff       (20)    57119 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/CRN2.py
--rw-r--r--   0 matto      (505) staff       (20)   249330 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/CRN3.py
--rw-r--r--   0 matto      (505) staff       (20)     3703 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/CS1.py
--rw-r--r--   0 matto      (505) staff       (20)     8157 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/CS2.py
--rw-r--r--   0 matto      (505) staff       (20)     1321 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/CS4.py
--rw-r--r--   0 matto      (505) staff       (20)     1917 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/DDR.py
--rw-r--r--   0 matto      (505) staff       (20)     3752 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/DOH.py
--rw-r--r--   0 matto      (505) staff       (20)     7362 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/EMT.py
--rw-r--r--   0 matto      (505) staff       (20)    10218 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/FAU.py
--rw-r--r--   0 matto      (505) staff       (20)    14850 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/FK6layers.py
--rw-r--r--   0 matto      (505) staff       (20)    23003 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/FK9layers.py
--rw-r--r--   0 matto      (505) staff       (20)     5390 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/HS1.py
--rw-r--r--   0 matto      (505) staff       (20)     5578 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/HS2.py
--rw-r--r--   0 matto      (505) staff       (20)     3752 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/HS3.py
--rw-r--r--   0 matto      (505) staff       (20)    11842 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Hcomp.py
--rw-r--r--   0 matto      (505) staff       (20)     1695 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/II.py
--rw-r--r--   0 matto      (505) staff       (20)      981 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/III.py
--rw-r--r--   0 matto      (505) staff       (20)     2927 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/IRR.py
--rw-r--r--   0 matto      (505) staff       (20)     8938 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/IV.py
--rw-r--r--   0 matto      (505) staff       (20)     2250 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/IWV.py
--rw-r--r--   0 matto      (505) staff       (20)     1178 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/IX.py
--rw-r--r--   0 matto      (505) staff       (20)      951 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Ic.py
--rw-r--r--   0 matto      (505) staff       (20)      936 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Ih.py
--rw-r--r--   0 matto      (505) staff       (20)    59988 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Kcomp.py
--rw-r--r--   0 matto      (505) staff       (20)     1413 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/LTA.py
--rw-r--r--   0 matto      (505) staff       (20)     2988 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/MAR.py
--rw-r--r--   0 matto      (505) staff       (20)     3703 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/MEP.py
--rw-r--r--   0 matto      (505) staff       (20)     8157 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/MTN.py
--rw-r--r--   0 matto      (505) staff       (20)     3398 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/NON.py
--rw-r--r--   0 matto      (505) staff       (20)     3452 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8007225.py
--rw-r--r--   0 matto      (505) staff       (20)     4835 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8036144.py
--rw-r--r--   0 matto      (505) staff       (20)      938 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8045578.py
--rw-r--r--   0 matto      (505) staff       (20)     1115 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8047078.py
--rw-r--r--   0 matto      (505) staff       (20)     1294 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8047931.py
--rw-r--r--   0 matto      (505) staff       (20)     1032 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8172143.py
--rw-r--r--   0 matto      (505) staff       (20)     3780 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8204698.py
--rw-r--r--   0 matto      (505) staff       (20)     6301 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8301974.py
--rw-r--r--   0 matto      (505) staff       (20)     2201 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8321499.py
--rw-r--r--   0 matto      (505) staff       (20)     2213 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/PCOD8324623.py
--rw-r--r--   0 matto      (505) staff       (20)     3279 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/RHO.py
--rw-r--r--   0 matto      (505) staff       (20)     2653 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/SGT.py
--rw-r--r--   0 matto      (505) staff       (20)     1321 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/SOD.py
--rw-r--r--   0 matto      (505) staff       (20)    24440 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct01.py
--rw-r--r--   0 matto      (505) staff       (20)    29899 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct02.py
--rw-r--r--   0 matto      (505) staff       (20)    23803 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct03.py
--rw-r--r--   0 matto      (505) staff       (20)     9852 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct04.py
--rw-r--r--   0 matto      (505) staff       (20)    31509 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct05.py
--rw-r--r--   0 matto      (505) staff       (20)    31627 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct06.py
--rw-r--r--   0 matto      (505) staff       (20)    16122 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct07.py
--rw-r--r--   0 matto      (505) staff       (20)    31554 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct08.py
--rw-r--r--   0 matto      (505) staff       (20)    31604 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct09.py
--rw-r--r--   0 matto      (505) staff       (20)    16130 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct10.py
--rw-r--r--   0 matto      (505) staff       (20)    16114 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct11.py
--rw-r--r--   0 matto      (505) staff       (20)    16121 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct12.py
--rw-r--r--   0 matto      (505) staff       (20)    16112 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct13.py
--rw-r--r--   0 matto      (505) staff       (20)    24557 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct14.py
--rw-r--r--   0 matto      (505) staff       (20)    32152 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct15.py
--rw-r--r--   0 matto      (505) staff       (20)    16992 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct16.py
--rw-r--r--   0 matto      (505) staff       (20)    10946 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct17.py
--rw-r--r--   0 matto      (505) staff       (20)     7510 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct18.py
--rw-r--r--   0 matto      (505) staff       (20)     9522 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct19.py
--rw-r--r--   0 matto      (505) staff       (20)     8080 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct20.py
--rw-r--r--   0 matto      (505) staff       (20)    17239 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct21.py
--rw-r--r--   0 matto      (505) staff       (20)    22970 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct22.py
--rw-r--r--   0 matto      (505) staff       (20)    22952 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct23.py
--rw-r--r--   0 matto      (505) staff       (20)    14850 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct24.py
--rw-r--r--   0 matto      (505) staff       (20)    23003 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct25.py
--rw-r--r--   0 matto      (505) staff       (20)    15604 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct26.py
--rw-r--r--   0 matto      (505) staff       (20)    24256 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct27.py
--rw-r--r--   0 matto      (505) staff       (20)     8181 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct28.py
--rw-r--r--   0 matto      (505) staff       (20)    15516 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct29.py
--rw-r--r--   0 matto      (505) staff       (20)    10255 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct30.py
--rw-r--r--   0 matto      (505) staff       (20)    16470 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct31.py
--rw-r--r--   0 matto      (505) staff       (20)    25631 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct32.py
--rw-r--r--   0 matto      (505) staff       (20)     3438 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct33.py
--rw-r--r--   0 matto      (505) staff       (20)    11272 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct34.py
--rw-r--r--   0 matto      (505) staff       (20)    10993 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct35.py
--rw-r--r--   0 matto      (505) staff       (20)    11125 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct36.py
--rw-r--r--   0 matto      (505) staff       (20)    11842 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct37.py
--rw-r--r--   0 matto      (505) staff       (20)    12269 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct38.py
--rw-r--r--   0 matto      (505) staff       (20)    12431 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct39.py
--rw-r--r--   0 matto      (505) staff       (20)    12754 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct40.py
--rw-r--r--   0 matto      (505) staff       (20)    26321 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct41.py
--rw-r--r--   0 matto      (505) staff       (20)    26291 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct42.py
--rw-r--r--   0 matto      (505) staff       (20)    27062 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct43.py
--rw-r--r--   0 matto      (505) staff       (20)    14155 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct44.py
--rw-r--r--   0 matto      (505) staff       (20)    14158 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct45.py
--rw-r--r--   0 matto      (505) staff       (20)    14778 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct46.py
--rw-r--r--   0 matto      (505) staff       (20)    14950 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct47.py
--rw-r--r--   0 matto      (505) staff       (20)    29421 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct48.py
--rw-r--r--   0 matto      (505) staff       (20)    15804 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct49.py
--rw-r--r--   0 matto      (505) staff       (20)    15680 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct50.py
--rw-r--r--   0 matto      (505) staff       (20)     8144 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct51.py
--rw-r--r--   0 matto      (505) staff       (20)    30540 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct52.py
--rw-r--r--   0 matto      (505) staff       (20)    15873 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct53.py
--rw-r--r--   0 matto      (505) staff       (20)     3548 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct54.py
--rw-r--r--   0 matto      (505) staff       (20)    10635 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct55.py
--rw-r--r--   0 matto      (505) staff       (20)    20505 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct56.py
--rw-r--r--   0 matto      (505) staff       (20)    11281 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct57.py
--rw-r--r--   0 matto      (505) staff       (20)    21998 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct58.py
--rw-r--r--   0 matto      (505) staff       (20)    22115 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct59.py
--rw-r--r--   0 matto      (505) staff       (20)    22091 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct60.py
--rw-r--r--   0 matto      (505) staff       (20)    27401 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct61.py
--rw-r--r--   0 matto      (505) staff       (20)    21359 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct62.py
--rw-r--r--   0 matto      (505) staff       (20)    14836 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct63.py
--rw-r--r--   0 matto      (505) staff       (20)    15266 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct64.py
--rw-r--r--   0 matto      (505) staff       (20)    15062 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct65.py
--rw-r--r--   0 matto      (505) staff       (20)    15106 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct66.py
--rw-r--r--   0 matto      (505) staff       (20)    29790 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct67.py
--rw-r--r--   0 matto      (505) staff       (20)     5578 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct68.py
--rw-r--r--   0 matto      (505) staff       (20)     8457 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct69.py
--rw-r--r--   0 matto      (505) staff       (20)    15993 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct70.py
--rw-r--r--   0 matto      (505) staff       (20)    15813 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct71.py
--rw-r--r--   0 matto      (505) staff       (20)    15826 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct72.py
--rw-r--r--   0 matto      (505) staff       (20)    16062 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct73.py
--rw-r--r--   0 matto      (505) staff       (20)    16115 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct74.py
--rw-r--r--   0 matto      (505) staff       (20)    16135 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct75.py
--rw-r--r--   0 matto      (505) staff       (20)    31343 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct76.py
--rw-r--r--   0 matto      (505) staff       (20)    15792 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct77.py
--rw-r--r--   0 matto      (505) staff       (20)    31289 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct78.py
--rw-r--r--   0 matto      (505) staff       (20)    31273 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct79.py
--rw-r--r--   0 matto      (505) staff       (20)    15829 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct80.py
--rw-r--r--   0 matto      (505) staff       (20)    23944 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct81.py
--rw-r--r--   0 matto      (505) staff       (20)    22360 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct82.py
--rw-r--r--   0 matto      (505) staff       (20)    22357 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct83.py
--rw-r--r--   0 matto      (505) staff       (20)    11749 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Struct84.py
--rw-r--r--   0 matto      (505) staff       (20)    32977 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/T.py
--rw-r--r--   0 matto      (505) staff       (20)     9560 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/TS1.py
--rw-r--r--   0 matto      (505) staff       (20)     1358 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/V.py
--rw-r--r--   0 matto      (505) staff       (20)     1373 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/VI.py
--rw-r--r--   0 matto      (505) staff       (20)     1432 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/VII.py
--rw-r--r--   0 matto      (505) staff       (20)     2136 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/VIII.py
--rw-r--r--   0 matto      (505) staff       (20)     1549 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/XI.py
--rw-r--r--   0 matto      (505) staff       (20)     1245 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/XII.py
--rw-r--r--   0 matto      (505) staff       (20)     2161 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/XIII.py
--rw-r--r--   0 matto      (505) staff       (20)     8157 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/XVI.py
--rw-r--r--   0 matto      (505) staff       (20)     1377 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/XVII.py
--rw-r--r--   0 matto      (505) staff       (20)     3548 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/Z.py
--rw-r--r--   0 matto      (505) staff       (20)     2249 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/__ice14.py
--rw-r--r--   0 matto      (505) staff       (20)       54 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     3610 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/__test1.py
--rw-r--r--   0 matto      (505) staff       (20)     3288 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/__test2.py
--rw-r--r--   0 matto      (505) staff       (20)      953 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/__test3.py
--rw-r--r--   0 matto      (505) staff       (20)     1738 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/__test4.py
--rw-r--r--   0 matto      (505) staff       (20)     1595 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/c0te.py
--rw-r--r--   0 matto      (505) staff       (20)     2965 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/c1te.py
--rw-r--r--   0 matto      (505) staff       (20)     2618 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/c2te.py
--rw-r--r--   0 matto      (505) staff       (20)    22952 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/delta.py
--rw-r--r--   0 matto      (505) staff       (20)     1612 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/dtc.py
--rw-r--r--   0 matto      (505) staff       (20)     3078 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/eleven.py
--rw-r--r--   0 matto      (505) staff       (20)     1321 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel01.py
--rw-r--r--   0 matto      (505) staff       (20)      846 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel02.py
--rw-r--r--   0 matto      (505) staff       (20)     1165 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel03.py
--rw-r--r--   0 matto      (505) staff       (20)     1413 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel04.py
--rw-r--r--   0 matto      (505) staff       (20)     3669 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel05.py
--rw-r--r--   0 matto      (505) staff       (20)     1111 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel06.py
--rw-r--r--   0 matto      (505) staff       (20)     1300 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel07.py
--rw-r--r--   0 matto      (505) staff       (20)      845 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel08.py
--rw-r--r--   0 matto      (505) staff       (20)      847 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel09.py
--rw-r--r--   0 matto      (505) staff       (20)      832 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel10.py
--rw-r--r--   0 matto      (505) staff       (20)     1297 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel11.py
--rw-r--r--   0 matto      (505) staff       (20)     1119 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel12.py
--rw-r--r--   0 matto      (505) staff       (20)     1115 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel13.py
--rw-r--r--   0 matto      (505) staff       (20)     3450 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel14.py
--rw-r--r--   0 matto      (505) staff       (20)     1032 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel15.py
--rw-r--r--   0 matto      (505) staff       (20)      976 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel16.py
--rw-r--r--   0 matto      (505) staff       (20)     1917 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel17.py
--rw-r--r--   0 matto      (505) staff       (20)      934 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel18.py
--rw-r--r--   0 matto      (505) staff       (20)     1301 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel19.py
--rw-r--r--   0 matto      (505) staff       (20)     6301 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel20.py
--rw-r--r--   0 matto      (505) staff       (20)      938 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel21.py
--rw-r--r--   0 matto      (505) staff       (20)     1110 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel22.py
--rw-r--r--   0 matto      (505) staff       (20)     3815 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel23.py
--rw-r--r--   0 matto      (505) staff       (20)     3452 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel24.py
--rw-r--r--   0 matto      (505) staff       (20)      756 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel25.py
--rw-r--r--   0 matto      (505) staff       (20)     2201 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel26.py
--rw-r--r--   0 matto      (505) staff       (20)     1294 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel27.py
--rw-r--r--   0 matto      (505) staff       (20)      848 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel28.py
--rw-r--r--   0 matto      (505) staff       (20)     2988 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel29.py
--rw-r--r--   0 matto      (505) staff       (20)     2213 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel30.py
--rw-r--r--   0 matto      (505) staff       (20)     2653 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel31.py
--rw-r--r--   0 matto      (505) staff       (20)      843 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel32.py
--rw-r--r--   0 matto      (505) staff       (20)      933 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel33.py
--rw-r--r--   0 matto      (505) staff       (20)     3398 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/engel34.py
--rw-r--r--   0 matto      (505) staff       (20)     1081 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/i.py
--rw-r--r--   0 matto      (505) staff       (20)     1372 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice0.py
--rw-r--r--   0 matto      (505) staff       (20)     1549 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice11.py
--rw-r--r--   0 matto      (505) staff       (20)     1245 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice12.py
--rw-r--r--   0 matto      (505) staff       (20)     2161 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice13.py
--rw-r--r--   0 matto      (505) staff       (20)     8157 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice16.py
--rw-r--r--   0 matto      (505) staff       (20)     1377 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice17.py
--rw-r--r--   0 matto      (505) staff       (20)      951 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice1c.py
--rw-r--r--   0 matto      (505) staff       (20)      936 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice1h.py
--rw-r--r--   0 matto      (505) staff       (20)      794 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice1h_unit.py
--rw-r--r--   0 matto      (505) staff       (20)     2229 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice1hte.py
--rw-r--r--   0 matto      (505) staff       (20)     1695 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice2.py
--rw-r--r--   0 matto      (505) staff       (20)     2742 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice2d.py
--rw-r--r--   0 matto      (505) staff       (20)     6442 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice2rect.py
--rw-r--r--   0 matto      (505) staff       (20)      981 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice3.py
--rw-r--r--   0 matto      (505) staff       (20)     8938 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice4.py
--rw-r--r--   0 matto      (505) staff       (20)     1358 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice5.py
--rw-r--r--   0 matto      (505) staff       (20)     1373 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice6.py
--rw-r--r--   0 matto      (505) staff       (20)     1432 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice7.py
--rw-r--r--   0 matto      (505) staff       (20)     2136 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice8.py
--rw-r--r--   0 matto      (505) staff       (20)     1178 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/ice9.py
--rw-r--r--   0 matto      (505) staff       (20)     1404 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/iceA.py
--rw-r--r--   0 matto      (505) staff       (20)     1333 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/iceB.py
--rw-r--r--   0 matto      (505) staff       (20)     2617 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/iceR.py
--rw-r--r--   0 matto      (505) staff       (20)     2443 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/iceT.py
--rw-r--r--   0 matto      (505) staff       (20)     6662 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/iceT2.py
--rw-r--r--   0 matto      (505) staff       (20)    16992 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/mu.py
--rw-r--r--   0 matto      (505) staff       (20)     1616 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/one.py
--rw-r--r--   0 matto      (505) staff       (20)     2216 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/prism.py
--rw-r--r--   0 matto      (505) staff       (20)    10635 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/psigma.py
--rw-r--r--   0 matto      (505) staff       (20)     3752 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sH.py
--rw-r--r--   0 matto      (505) staff       (20)     3703 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sI.py
--rw-r--r--   0 matto      (505) staff       (20)     8157 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sII.py
--rw-r--r--   0 matto      (505) staff       (20)     9560 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sIII.py
--rw-r--r--   0 matto      (505) staff       (20)     5390 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sIV.py
--rw-r--r--   0 matto      (505) staff       (20)     1973 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sTprime.py
--rw-r--r--   0 matto      (505) staff       (20)     5578 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sV.py
--rw-r--r--   0 matto      (505) staff       (20)     1321 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sVII.py
--rw-r--r--   0 matto      (505) staff       (20)    12269 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/sigma.py
--rw-r--r--   0 matto      (505) staff       (20)     6462 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/xFAU.py
--rw-r--r--   0 matto      (505) staff       (20)     3852 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/xdtc.py
--rw-r--r--   0 matto      (505) staff       (20)    10946 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/lattices/zra-d.py
--rw-r--r--   0 matto      (505) staff       (20)     4719 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/load.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.092751 GenIce2-2.1b3/genice2/loaders/
--rw-r--r--   0 matto      (505) staff       (20)      102 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/loaders/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     1048 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/loaders/ar3r.py
--rw-r--r--   0 matto      (505) staff       (20)     3024 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/loaders/exyz.py
--rw-r--r--   0 matto      (505) staff       (20)     2115 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/loaders/gro.py
--rw-r--r--   0 matto      (505) staff       (20)     1893 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/loaders/mdv.py
--rw-r--r--   0 matto      (505) staff       (20)     1893 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/loaders/mdva.py
--rw-r--r--   0 matto      (505) staff       (20)     1624 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/loaders/nx3a.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-24 10:25:56.097517 GenIce2-2.1b3/genice2/molecules/
--rw-r--r--   0 matto      (505) staff       (20)      669 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/3site.py
--rw-r--r--   0 matto      (505) staff       (20)      866 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/4site.py
--rw-r--r--   0 matto      (505) staff       (20)      984 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/5site.py
--rw-r--r--   0 matto      (505) staff       (20)     1366 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/6site.py
--rw-r--r--   0 matto      (505) staff       (20)     1153 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/7site.py
--rw-r--r--   0 matto      (505) staff       (20)      476 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/H2.py
--rw-r--r--   0 matto      (505) staff       (20)     1366 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/NvdE.py
--rw-r--r--   0 matto      (505) staff       (20)     2139 2021-03-19 14:21:18.000000 GenIce2-2.1b3/genice2/molecules/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)      620 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/ch4.py
--rw-r--r--   0 matto      (505) staff       (20)      362 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/co2.py
--rw-r--r--   0 matto      (505) staff       (20)      275 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/empty.py
--rw-r--r--   0 matto      (505) staff       (20)      217 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/g12.py
--rw-r--r--   0 matto      (505) staff       (20)      217 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/g14.py
--rw-r--r--   0 matto      (505) staff       (20)      217 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/g15.py
--rw-r--r--   0 matto      (505) staff       (20)      217 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/g16.py
--rw-r--r--   0 matto      (505) staff       (20)      909 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/ice.py
--rw-r--r--   0 matto      (505) staff       (20)      320 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/me.py
--rw-r--r--   0 matto      (505) staff       (20)     1216 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/mol.py
--rw-r--r--   0 matto      (505) staff       (20)      447 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/one.py
--rw-r--r--   0 matto      (505) staff       (20)      814 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/physical_water.py
--rw-r--r--   0 matto      (505) staff       (20)      578 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/spce.py
--rw-r--r--   0 matto      (505) staff       (20)      821 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/thf.py
--rw-r--r--   0 matto      (505) staff       (20)      669 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/tip3p.py
--rw-r--r--   0 matto      (505) staff       (20)      866 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/tip4p.py
--rw-r--r--   0 matto      (505) staff       (20)      984 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/tip5p.py
--rw-r--r--   0 matto      (505) staff       (20)      763 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/uathf.py
--rw-r--r--   0 matto      (505) staff       (20)      730 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/molecules/uathf6.py
--rw-r--r--   0 matto      (505) staff       (20)     9288 2021-03-19 13:13:23.000000 GenIce2-2.1b3/genice2/plugin.py
--rw-r--r--   0 matto      (505) staff       (20)    12503 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/rigid.py
--rw-r--r--   0 matto      (505) staff       (20)     3021 2021-03-15 06:29:56.000000 GenIce2-2.1b3/genice2/valueparser.py
--rwxr-xr-x   0 matto      (505) staff       (20)       87 2021-03-24 08:24:14.000000 GenIce2-2.1b3/requirements.txt
--rw-r--r--   0 matto      (505) staff       (20)      108 2021-03-24 10:25:56.100448 GenIce2-2.1b3/setup.cfg
--rwxr-xr-x   0 matto      (505) staff       (20)     1616 2021-03-23 10:51:22.000000 GenIce2-2.1b3/setup.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.411060 GenIce2-2.1b4/
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.353695 GenIce2-2.1b4/GenIce2.egg-info/
+-rw-r--r--   0 matto      (505) staff       (20)    59916 2021-05-11 11:37:45.000000 GenIce2-2.1b4/GenIce2.egg-info/PKG-INFO
+-rw-r--r--   0 matto      (505) staff       (20)     9997 2021-05-11 11:37:45.000000 GenIce2-2.1b4/GenIce2.egg-info/SOURCES.txt
+-rw-r--r--   0 matto      (505) staff       (20)        1 2021-05-11 11:37:45.000000 GenIce2-2.1b4/GenIce2.egg-info/dependency_links.txt
+-rw-r--r--   0 matto      (505) staff       (20)       89 2021-05-11 11:37:45.000000 GenIce2-2.1b4/GenIce2.egg-info/entry_points.txt
+-rw-r--r--   0 matto      (505) staff       (20)       87 2021-05-11 11:37:45.000000 GenIce2-2.1b4/GenIce2.egg-info/requires.txt
+-rw-r--r--   0 matto      (505) staff       (20)        8 2021-05-11 11:37:45.000000 GenIce2-2.1b4/GenIce2.egg-info/top_level.txt
+-rw-r--r--   0 matto      (505) staff       (20)       88 2021-05-07 12:07:04.000000 GenIce2-2.1b4/MANIFEST.in
+-rw-r--r--   0 matto      (505) staff       (20)    59916 2021-05-11 11:37:45.411412 GenIce2-2.1b4/PKG-INFO
+-rw-r--r--   0 matto      (505) staff       (20)    52642 2021-05-11 11:18:18.000000 GenIce2-2.1b4/README.md
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.355243 GenIce2-2.1b4/genice2/
+-rw-r--r--   0 matto      (505) staff       (20)     4064 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/CIF.py
+-rw-r--r--   0 matto      (505) staff       (20)     3243 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/FrankKasper.py
+-rw-r--r--   0 matto      (505) staff       (20)       46 2021-05-11 11:18:02.000000 GenIce2-2.1b4/genice2/__init__.py
+-rw-r--r--   0 matto      (505) staff       (20)     2936 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/alkyl.py
+-rw-r--r--   0 matto      (505) staff       (20)     9293 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/analice.py
+-rw-r--r--   0 matto      (505) staff       (20)     3468 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/cell.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.355553 GenIce2-2.1b4/genice2/cli/
+-rw-r--r--   0 matto      (505) staff       (20)     1513 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/cli/__init__.py
+-rw-r--r--   0 matto      (505) staff       (20)     6765 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/cli/analice.py
+-rw-r--r--   0 matto      (505) staff       (20)     9593 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/cli/genice.py
+-rw-r--r--   0 matto      (505) staff       (20)      916 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/decorators.py
+-rw-r--r--   0 matto      (505) staff       (20)    21248 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/digraph.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.359899 GenIce2-2.1b4/genice2/formats/
+-rw-r--r--   0 matto      (505) staff       (20)     1953 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/_KG.py
+-rw-r--r--   0 matto      (505) staff       (20)      301 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/__init__.py
+-rw-r--r--   0 matto      (505) staff       (20)     6919 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/_ringstat.py
+-rw-r--r--   0 matto      (505) staff       (20)     1420 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/c.py
+-rw-r--r--   0 matto      (505) staff       (20)     2231 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/cif.py
+-rw-r--r--   0 matto      (505) staff       (20)     2121 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/cif2.py
+-rw-r--r--   0 matto      (505) staff       (20)     1420 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/com.py
+-rw-r--r--   0 matto      (505) staff       (20)      944 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/d.py
+-rw-r--r--   0 matto      (505) staff       (20)      944 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/digraph.py
+-rw-r--r--   0 matto      (505) staff       (20)     2008 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/e.py
+-rw-r--r--   0 matto      (505) staff       (20)     2008 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/euler.py
+-rw-r--r--   0 matto      (505) staff       (20)     1333 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/exmol.py
+-rw-r--r--   0 matto      (505) staff       (20)     1603 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/exyz.py
+-rw-r--r--   0 matto      (505) staff       (20)     2902 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/g.py
+-rw-r--r--   0 matto      (505) staff       (20)      968 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/graph.py
+-rw-r--r--   0 matto      (505) staff       (20)     2902 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/gromacs.py
+-rw-r--r--   0 matto      (505) staff       (20)     1494 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/m.py
+-rw-r--r--   0 matto      (505) staff       (20)     1494 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/mdv_au.py
+-rw-r--r--   0 matto      (505) staff       (20)     1494 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/mdview.py
+-rw-r--r--   0 matto      (505) staff       (20)      418 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/null.py
+-rw-r--r--   0 matto      (505) staff       (20)     4801 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/o.py
+-rw-r--r--   0 matto      (505) staff       (20)     4801 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/openscad.py
+-rw-r--r--   0 matto      (505) staff       (20)     6676 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/p.py
+-rw-r--r--   0 matto      (505) staff       (20)     3531 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/povray.py
+-rw-r--r--   0 matto      (505) staff       (20)     6676 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/python.py
+-rw-r--r--   0 matto      (505) staff       (20)     2067 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/q.py
+-rw-r--r--   0 matto      (505) staff       (20)     2067 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/quaternion.py
+-rw-r--r--   0 matto      (505) staff       (20)     1246 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/r.py
+-rw-r--r--   0 matto      (505) staff       (20)     3937 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/raw.py
+-rw-r--r--   0 matto      (505) staff       (20)     1246 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/rcom.py
+-rw-r--r--   0 matto      (505) staff       (20)     6676 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/reshape.py
+-rw-r--r--   0 matto      (505) staff       (20)     6452 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/rings.py
+-rw-r--r--   0 matto      (505) staff       (20)     1723 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/towhee.py
+-rw-r--r--   0 matto      (505) staff       (20)     1148 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/xyz.py
+-rw-r--r--   0 matto      (505) staff       (20)     4690 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/y.py
+-rw-r--r--   0 matto      (505) staff       (20)     4690 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/formats/yaplot.py
+-rw-r--r--   0 matto      (505) staff       (20)    46378 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/genice.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.406566 GenIce2-2.1b4/genice2/lattices/
+-rw-r--r--   0 matto      (505) staff       (20)     1372 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/0.py
+-rw-r--r--   0 matto      (505) staff       (20)     1549 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/11.py
+-rw-r--r--   0 matto      (505) staff       (20)     3408 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/115_2_114.py
+-rw-r--r--   0 matto      (505) staff       (20)      934 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/11_2_15848.py
+-rw-r--r--   0 matto      (505) staff       (20)     1245 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/12.py
+-rw-r--r--   0 matto      (505) staff       (20)     3747 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/12_1_11.py
+-rw-r--r--   0 matto      (505) staff       (20)      846 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/12_2_29187.py
+-rw-r--r--   0 matto      (505) staff       (20)      847 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/12_2_32449.py
+-rw-r--r--   0 matto      (505) staff       (20)     2161 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/13.py
+-rw-r--r--   0 matto      (505) staff       (20)     2692 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/144_2_7301.py
+-rw-r--r--   0 matto      (505) staff       (20)      933 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/14_2_48453.py
+-rw-r--r--   0 matto      (505) staff       (20)     3815 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/151_2_4949650.py
+-rw-r--r--   0 matto      (505) staff       (20)      976 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/152_2_118474.py
+-rw-r--r--   0 matto      (505) staff       (20)     2168 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/153_2_155471.py
+-rw-r--r--   0 matto      (505) staff       (20)      848 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/15_2_201714.py
+-rw-r--r--   0 matto      (505) staff       (20)     8157 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/16.py
+-rw-r--r--   0 matto      (505) staff       (20)     1119 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/169_2_10608.py
+-rw-r--r--   0 matto      (505) staff       (20)     1111 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/169_2_7915.py
+-rw-r--r--   0 matto      (505) staff       (20)     1377 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/17.py
+-rw-r--r--   0 matto      (505) staff       (20)     1638 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/176_2_5256.py
+-rw-r--r--   0 matto      (505) staff       (20)      951 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/1c.py
+-rw-r--r--   0 matto      (505) staff       (20)      936 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/1h.py
+-rw-r--r--   0 matto      (505) staff       (20)      920 2021-05-11 11:13:28.000000 GenIce2-2.1b4/genice2/lattices/1h_unit.py
+-rw-r--r--   0 matto      (505) staff       (20)     1695 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/2.py
+-rw-r--r--   0 matto      (505) staff       (20)     1321 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/207_1_4435.py
+-rw-r--r--   0 matto      (505) staff       (20)      845 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/20_2_26425.py
+-rw-r--r--   0 matto      (505) staff       (20)      843 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/20_2_28176.py
+-rw-r--r--   0 matto      (505) staff       (20)     1859 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/2D3.py
+-rw-r--r--   0 matto      (505) staff       (20)      756 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/2_2_342692.py
+-rw-r--r--   0 matto      (505) staff       (20)     4835 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/2_2_623457.py
+-rw-r--r--   0 matto      (505) staff       (20)     2742 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/2d.py
+-rw-r--r--   0 matto      (505) staff       (20)      981 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/3.py
+-rw-r--r--   0 matto      (505) staff       (20)     8938 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/4.py
+-rw-r--r--   0 matto      (505) staff       (20)    30989 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/4R.py
+-rw-r--r--   0 matto      (505) staff       (20)     1358 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/5.py
+-rw-r--r--   0 matto      (505) staff       (20)     1300 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/53_3_726600.py
+-rw-r--r--   0 matto      (505) staff       (20)     1110 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/58_2_511.py
+-rw-r--r--   0 matto      (505) staff       (20)     3974 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/5R.py
+-rw-r--r--   0 matto      (505) staff       (20)     1373 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/6.py
+-rw-r--r--   0 matto      (505) staff       (20)     1297 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/61_2_8842.py
+-rw-r--r--   0 matto      (505) staff       (20)     2148 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/67_2_1444.py
+-rw-r--r--   0 matto      (505) staff       (20)     3450 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/67_2_1563.py
+-rw-r--r--   0 matto      (505) staff       (20)      773 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/6h.py
+-rw-r--r--   0 matto      (505) staff       (20)     1432 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/7.py
+-rw-r--r--   0 matto      (505) staff       (20)     2136 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/8.py
+-rw-r--r--   0 matto      (505) staff       (20)      832 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/84_2_1419.py
+-rw-r--r--   0 matto      (505) staff       (20)     1178 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/9.py
+-rw-r--r--   0 matto      (505) staff       (20)     1301 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/91_2_8335121.py
+-rw-r--r--   0 matto      (505) staff       (20)     1404 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/A.py
+-rw-r--r--   0 matto      (505) staff       (20)     3438 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/A15.py
+-rw-r--r--   0 matto      (505) staff       (20)     1165 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ACO.py
+-rw-r--r--   0 matto      (505) staff       (20)     1333 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/B.py
+-rw-r--r--   0 matto      (505) staff       (20)     3669 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/BSV.py
+-rw-r--r--   0 matto      (505) staff       (20)     5578 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/C14.py
+-rw-r--r--   0 matto      (505) staff       (20)     9522 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/C15.py
+-rw-r--r--   0 matto      (505) staff       (20)     9852 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/C36.py
+-rw-r--r--   0 matto      (505) staff       (20)    57115 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/CRN1.py
+-rw-r--r--   0 matto      (505) staff       (20)    57119 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/CRN2.py
+-rw-r--r--   0 matto      (505) staff       (20)   249330 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/CRN3.py
+-rw-r--r--   0 matto      (505) staff       (20)     3703 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/CS1.py
+-rw-r--r--   0 matto      (505) staff       (20)     8157 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/CS2.py
+-rw-r--r--   0 matto      (505) staff       (20)     1321 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/CS4.py
+-rw-r--r--   0 matto      (505) staff       (20)     1917 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/DDR.py
+-rw-r--r--   0 matto      (505) staff       (20)     3752 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/DOH.py
+-rw-r--r--   0 matto      (505) staff       (20)     7362 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/EMT.py
+-rw-r--r--   0 matto      (505) staff       (20)    10218 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/FAU.py
+-rw-r--r--   0 matto      (505) staff       (20)    14850 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/FK6layers.py
+-rw-r--r--   0 matto      (505) staff       (20)    23003 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/FK9layers.py
+-rw-r--r--   0 matto      (505) staff       (20)     5390 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/HS1.py
+-rw-r--r--   0 matto      (505) staff       (20)     5578 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/HS2.py
+-rw-r--r--   0 matto      (505) staff       (20)     3752 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/HS3.py
+-rw-r--r--   0 matto      (505) staff       (20)    11842 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Hcomp.py
+-rw-r--r--   0 matto      (505) staff       (20)     1695 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/II.py
+-rw-r--r--   0 matto      (505) staff       (20)      981 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/III.py
+-rw-r--r--   0 matto      (505) staff       (20)     2927 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/IRR.py
+-rw-r--r--   0 matto      (505) staff       (20)     8938 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/IV.py
+-rw-r--r--   0 matto      (505) staff       (20)     2250 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/IWV.py
+-rw-r--r--   0 matto      (505) staff       (20)     1178 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/IX.py
+-rw-r--r--   0 matto      (505) staff       (20)      951 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Ic.py
+-rw-r--r--   0 matto      (505) staff       (20)      936 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Ih.py
+-rw-r--r--   0 matto      (505) staff       (20)    59988 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Kcomp.py
+-rw-r--r--   0 matto      (505) staff       (20)     1413 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/LTA.py
+-rw-r--r--   0 matto      (505) staff       (20)     2988 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/MAR.py
+-rw-r--r--   0 matto      (505) staff       (20)     3703 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/MEP.py
+-rw-r--r--   0 matto      (505) staff       (20)     8157 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/MTN.py
+-rw-r--r--   0 matto      (505) staff       (20)     3398 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/NON.py
+-rw-r--r--   0 matto      (505) staff       (20)     3452 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8007225.py
+-rw-r--r--   0 matto      (505) staff       (20)     4835 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8036144.py
+-rw-r--r--   0 matto      (505) staff       (20)      938 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8045578.py
+-rw-r--r--   0 matto      (505) staff       (20)     1115 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8047078.py
+-rw-r--r--   0 matto      (505) staff       (20)     1294 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8047931.py
+-rw-r--r--   0 matto      (505) staff       (20)     1032 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8172143.py
+-rw-r--r--   0 matto      (505) staff       (20)     3780 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8204698.py
+-rw-r--r--   0 matto      (505) staff       (20)     6301 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8301974.py
+-rw-r--r--   0 matto      (505) staff       (20)     2201 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8321499.py
+-rw-r--r--   0 matto      (505) staff       (20)     2213 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/PCOD8324623.py
+-rw-r--r--   0 matto      (505) staff       (20)     3279 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/RHO.py
+-rw-r--r--   0 matto      (505) staff       (20)     2653 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/SGT.py
+-rw-r--r--   0 matto      (505) staff       (20)     1321 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/SOD.py
+-rw-r--r--   0 matto      (505) staff       (20)    24440 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct01.py
+-rw-r--r--   0 matto      (505) staff       (20)    29899 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct02.py
+-rw-r--r--   0 matto      (505) staff       (20)    23803 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct03.py
+-rw-r--r--   0 matto      (505) staff       (20)     9852 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct04.py
+-rw-r--r--   0 matto      (505) staff       (20)    31509 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct05.py
+-rw-r--r--   0 matto      (505) staff       (20)    31627 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct06.py
+-rw-r--r--   0 matto      (505) staff       (20)    16122 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct07.py
+-rw-r--r--   0 matto      (505) staff       (20)    31554 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct08.py
+-rw-r--r--   0 matto      (505) staff       (20)    31604 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct09.py
+-rw-r--r--   0 matto      (505) staff       (20)    16130 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct10.py
+-rw-r--r--   0 matto      (505) staff       (20)    16114 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct11.py
+-rw-r--r--   0 matto      (505) staff       (20)    16121 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct12.py
+-rw-r--r--   0 matto      (505) staff       (20)    16112 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct13.py
+-rw-r--r--   0 matto      (505) staff       (20)    24557 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct14.py
+-rw-r--r--   0 matto      (505) staff       (20)    32152 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct15.py
+-rw-r--r--   0 matto      (505) staff       (20)    16992 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct16.py
+-rw-r--r--   0 matto      (505) staff       (20)    10946 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct17.py
+-rw-r--r--   0 matto      (505) staff       (20)     7510 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct18.py
+-rw-r--r--   0 matto      (505) staff       (20)     9522 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct19.py
+-rw-r--r--   0 matto      (505) staff       (20)     8080 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct20.py
+-rw-r--r--   0 matto      (505) staff       (20)    17239 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct21.py
+-rw-r--r--   0 matto      (505) staff       (20)    22970 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct22.py
+-rw-r--r--   0 matto      (505) staff       (20)    22952 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct23.py
+-rw-r--r--   0 matto      (505) staff       (20)    14850 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct24.py
+-rw-r--r--   0 matto      (505) staff       (20)    23003 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct25.py
+-rw-r--r--   0 matto      (505) staff       (20)    15604 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct26.py
+-rw-r--r--   0 matto      (505) staff       (20)    24256 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct27.py
+-rw-r--r--   0 matto      (505) staff       (20)     8181 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct28.py
+-rw-r--r--   0 matto      (505) staff       (20)    15516 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct29.py
+-rw-r--r--   0 matto      (505) staff       (20)    10255 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct30.py
+-rw-r--r--   0 matto      (505) staff       (20)    16470 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct31.py
+-rw-r--r--   0 matto      (505) staff       (20)    25631 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct32.py
+-rw-r--r--   0 matto      (505) staff       (20)     3438 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct33.py
+-rw-r--r--   0 matto      (505) staff       (20)    11272 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct34.py
+-rw-r--r--   0 matto      (505) staff       (20)    10993 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct35.py
+-rw-r--r--   0 matto      (505) staff       (20)    11125 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct36.py
+-rw-r--r--   0 matto      (505) staff       (20)    11842 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct37.py
+-rw-r--r--   0 matto      (505) staff       (20)    12269 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct38.py
+-rw-r--r--   0 matto      (505) staff       (20)    12431 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct39.py
+-rw-r--r--   0 matto      (505) staff       (20)    12754 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct40.py
+-rw-r--r--   0 matto      (505) staff       (20)    26321 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct41.py
+-rw-r--r--   0 matto      (505) staff       (20)    26291 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct42.py
+-rw-r--r--   0 matto      (505) staff       (20)    27062 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct43.py
+-rw-r--r--   0 matto      (505) staff       (20)    14155 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct44.py
+-rw-r--r--   0 matto      (505) staff       (20)    14158 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct45.py
+-rw-r--r--   0 matto      (505) staff       (20)    14778 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct46.py
+-rw-r--r--   0 matto      (505) staff       (20)    14950 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct47.py
+-rw-r--r--   0 matto      (505) staff       (20)    29421 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct48.py
+-rw-r--r--   0 matto      (505) staff       (20)    15804 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct49.py
+-rw-r--r--   0 matto      (505) staff       (20)    15680 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct50.py
+-rw-r--r--   0 matto      (505) staff       (20)     8144 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct51.py
+-rw-r--r--   0 matto      (505) staff       (20)    30540 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct52.py
+-rw-r--r--   0 matto      (505) staff       (20)    15873 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct53.py
+-rw-r--r--   0 matto      (505) staff       (20)     3548 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct54.py
+-rw-r--r--   0 matto      (505) staff       (20)    10635 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct55.py
+-rw-r--r--   0 matto      (505) staff       (20)    20505 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct56.py
+-rw-r--r--   0 matto      (505) staff       (20)    11281 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct57.py
+-rw-r--r--   0 matto      (505) staff       (20)    21998 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct58.py
+-rw-r--r--   0 matto      (505) staff       (20)    22115 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct59.py
+-rw-r--r--   0 matto      (505) staff       (20)    22091 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct60.py
+-rw-r--r--   0 matto      (505) staff       (20)    27401 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct61.py
+-rw-r--r--   0 matto      (505) staff       (20)    21359 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct62.py
+-rw-r--r--   0 matto      (505) staff       (20)    14836 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct63.py
+-rw-r--r--   0 matto      (505) staff       (20)    15266 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct64.py
+-rw-r--r--   0 matto      (505) staff       (20)    15062 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct65.py
+-rw-r--r--   0 matto      (505) staff       (20)    15106 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct66.py
+-rw-r--r--   0 matto      (505) staff       (20)    29790 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct67.py
+-rw-r--r--   0 matto      (505) staff       (20)     5578 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct68.py
+-rw-r--r--   0 matto      (505) staff       (20)     8457 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct69.py
+-rw-r--r--   0 matto      (505) staff       (20)    15993 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct70.py
+-rw-r--r--   0 matto      (505) staff       (20)    15813 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct71.py
+-rw-r--r--   0 matto      (505) staff       (20)    15826 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct72.py
+-rw-r--r--   0 matto      (505) staff       (20)    16062 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct73.py
+-rw-r--r--   0 matto      (505) staff       (20)    16115 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct74.py
+-rw-r--r--   0 matto      (505) staff       (20)    16135 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct75.py
+-rw-r--r--   0 matto      (505) staff       (20)    31343 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct76.py
+-rw-r--r--   0 matto      (505) staff       (20)    15792 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct77.py
+-rw-r--r--   0 matto      (505) staff       (20)    31289 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct78.py
+-rw-r--r--   0 matto      (505) staff       (20)    31273 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct79.py
+-rw-r--r--   0 matto      (505) staff       (20)    15829 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct80.py
+-rw-r--r--   0 matto      (505) staff       (20)    23944 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct81.py
+-rw-r--r--   0 matto      (505) staff       (20)    22360 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct82.py
+-rw-r--r--   0 matto      (505) staff       (20)    22357 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct83.py
+-rw-r--r--   0 matto      (505) staff       (20)    11749 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Struct84.py
+-rw-r--r--   0 matto      (505) staff       (20)    32977 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/T.py
+-rw-r--r--   0 matto      (505) staff       (20)     9560 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/TS1.py
+-rw-r--r--   0 matto      (505) staff       (20)     1358 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/V.py
+-rw-r--r--   0 matto      (505) staff       (20)     1373 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/VI.py
+-rw-r--r--   0 matto      (505) staff       (20)     1432 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/VII.py
+-rw-r--r--   0 matto      (505) staff       (20)     2136 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/VIII.py
+-rw-r--r--   0 matto      (505) staff       (20)     1549 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/XI.py
+-rw-r--r--   0 matto      (505) staff       (20)     1245 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/XII.py
+-rw-r--r--   0 matto      (505) staff       (20)     2161 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/XIII.py
+-rw-r--r--   0 matto      (505) staff       (20)     8157 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/XVI.py
+-rw-r--r--   0 matto      (505) staff       (20)     1377 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/XVII.py
+-rw-r--r--   0 matto      (505) staff       (20)     3548 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/Z.py
+-rw-r--r--   0 matto      (505) staff       (20)     2249 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/__ice14.py
+-rw-r--r--   0 matto      (505) staff       (20)       54 2021-05-07 12:07:04.000000 GenIce2-2.1b4/genice2/lattices/__init__.py
+-rw-r--r--   0 matto      (505) staff       (20)     3610 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/__test1.py
+-rw-r--r--   0 matto      (505) staff       (20)     3288 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/__test2.py
+-rw-r--r--   0 matto      (505) staff       (20)      953 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/__test3.py
+-rw-r--r--   0 matto      (505) staff       (20)     1738 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/__test4.py
+-rw-r--r--   0 matto      (505) staff       (20)     1595 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/c0te.py
+-rw-r--r--   0 matto      (505) staff       (20)     2965 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/c1te.py
+-rw-r--r--   0 matto      (505) staff       (20)     2618 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/c2te.py
+-rw-r--r--   0 matto      (505) staff       (20)    22952 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/delta.py
+-rw-r--r--   0 matto      (505) staff       (20)     1612 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/dtc.py
+-rw-r--r--   0 matto      (505) staff       (20)     3078 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/eleven.py
+-rw-r--r--   0 matto      (505) staff       (20)     1321 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel01.py
+-rw-r--r--   0 matto      (505) staff       (20)      846 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel02.py
+-rw-r--r--   0 matto      (505) staff       (20)     1165 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel03.py
+-rw-r--r--   0 matto      (505) staff       (20)     1413 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel04.py
+-rw-r--r--   0 matto      (505) staff       (20)     3669 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel05.py
+-rw-r--r--   0 matto      (505) staff       (20)     1111 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel06.py
+-rw-r--r--   0 matto      (505) staff       (20)     1300 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel07.py
+-rw-r--r--   0 matto      (505) staff       (20)      845 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel08.py
+-rw-r--r--   0 matto      (505) staff       (20)      847 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel09.py
+-rw-r--r--   0 matto      (505) staff       (20)      832 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel10.py
+-rw-r--r--   0 matto      (505) staff       (20)     1297 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel11.py
+-rw-r--r--   0 matto      (505) staff       (20)     1119 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel12.py
+-rw-r--r--   0 matto      (505) staff       (20)     1115 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel13.py
+-rw-r--r--   0 matto      (505) staff       (20)     3450 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel14.py
+-rw-r--r--   0 matto      (505) staff       (20)     1032 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel15.py
+-rw-r--r--   0 matto      (505) staff       (20)      976 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel16.py
+-rw-r--r--   0 matto      (505) staff       (20)     1917 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel17.py
+-rw-r--r--   0 matto      (505) staff       (20)      934 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel18.py
+-rw-r--r--   0 matto      (505) staff       (20)     1301 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel19.py
+-rw-r--r--   0 matto      (505) staff       (20)     6301 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel20.py
+-rw-r--r--   0 matto      (505) staff       (20)      938 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel21.py
+-rw-r--r--   0 matto      (505) staff       (20)     1110 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel22.py
+-rw-r--r--   0 matto      (505) staff       (20)     3815 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel23.py
+-rw-r--r--   0 matto      (505) staff       (20)     3452 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel24.py
+-rw-r--r--   0 matto      (505) staff       (20)      756 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel25.py
+-rw-r--r--   0 matto      (505) staff       (20)     2201 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel26.py
+-rw-r--r--   0 matto      (505) staff       (20)     1294 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel27.py
+-rw-r--r--   0 matto      (505) staff       (20)      848 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel28.py
+-rw-r--r--   0 matto      (505) staff       (20)     2988 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel29.py
+-rw-r--r--   0 matto      (505) staff       (20)     2213 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel30.py
+-rw-r--r--   0 matto      (505) staff       (20)     2653 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel31.py
+-rw-r--r--   0 matto      (505) staff       (20)      843 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel32.py
+-rw-r--r--   0 matto      (505) staff       (20)      933 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel33.py
+-rw-r--r--   0 matto      (505) staff       (20)     3398 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/engel34.py
+-rw-r--r--   0 matto      (505) staff       (20)     1081 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/i.py
+-rw-r--r--   0 matto      (505) staff       (20)     1372 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice0.py
+-rw-r--r--   0 matto      (505) staff       (20)     1549 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice11.py
+-rw-r--r--   0 matto      (505) staff       (20)     1245 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice12.py
+-rw-r--r--   0 matto      (505) staff       (20)     2161 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice13.py
+-rw-r--r--   0 matto      (505) staff       (20)     8157 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice16.py
+-rw-r--r--   0 matto      (505) staff       (20)     1377 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice17.py
+-rw-r--r--   0 matto      (505) staff       (20)      951 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice1c.py
+-rw-r--r--   0 matto      (505) staff       (20)      936 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice1h.py
+-rw-r--r--   0 matto      (505) staff       (20)      920 2021-05-11 11:13:28.000000 GenIce2-2.1b4/genice2/lattices/ice1h_unit.py
+-rw-r--r--   0 matto      (505) staff       (20)     2229 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice1hte.py
+-rw-r--r--   0 matto      (505) staff       (20)     1695 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice2.py
+-rw-r--r--   0 matto      (505) staff       (20)     2742 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice2d.py
+-rw-r--r--   0 matto      (505) staff       (20)     6442 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice2rect.py
+-rw-r--r--   0 matto      (505) staff       (20)      981 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice3.py
+-rw-r--r--   0 matto      (505) staff       (20)     8938 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice4.py
+-rw-r--r--   0 matto      (505) staff       (20)     1358 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice5.py
+-rw-r--r--   0 matto      (505) staff       (20)     1373 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice6.py
+-rw-r--r--   0 matto      (505) staff       (20)     1432 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice7.py
+-rw-r--r--   0 matto      (505) staff       (20)     2136 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice8.py
+-rw-r--r--   0 matto      (505) staff       (20)     1178 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/ice9.py
+-rw-r--r--   0 matto      (505) staff       (20)     1404 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/iceA.py
+-rw-r--r--   0 matto      (505) staff       (20)     1333 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/iceB.py
+-rw-r--r--   0 matto      (505) staff       (20)     2617 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/iceR.py
+-rw-r--r--   0 matto      (505) staff       (20)     2443 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/iceT.py
+-rw-r--r--   0 matto      (505) staff       (20)     6662 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/iceT2.py
+-rw-r--r--   0 matto      (505) staff       (20)    16992 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/mu.py
+-rw-r--r--   0 matto      (505) staff       (20)     1616 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/one.py
+-rw-r--r--   0 matto      (505) staff       (20)     2216 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/prism.py
+-rw-r--r--   0 matto      (505) staff       (20)    10635 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/psigma.py
+-rw-r--r--   0 matto      (505) staff       (20)     3752 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sH.py
+-rw-r--r--   0 matto      (505) staff       (20)     3703 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sI.py
+-rw-r--r--   0 matto      (505) staff       (20)     8157 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sII.py
+-rw-r--r--   0 matto      (505) staff       (20)     9560 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sIII.py
+-rw-r--r--   0 matto      (505) staff       (20)     5390 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sIV.py
+-rw-r--r--   0 matto      (505) staff       (20)     1973 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sTprime.py
+-rw-r--r--   0 matto      (505) staff       (20)     5578 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sV.py
+-rw-r--r--   0 matto      (505) staff       (20)     1321 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sVII.py
+-rw-r--r--   0 matto      (505) staff       (20)    12269 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/sigma.py
+-rw-r--r--   0 matto      (505) staff       (20)     6462 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/xFAU.py
+-rw-r--r--   0 matto      (505) staff       (20)     3852 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/xdtc.py
+-rw-r--r--   0 matto      (505) staff       (20)    10946 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/lattices/zra-d.py
+-rw-r--r--   0 matto      (505) staff       (20)     4719 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/load.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.407337 GenIce2-2.1b4/genice2/loaders/
+-rw-r--r--   0 matto      (505) staff       (20)      102 2021-05-07 12:07:04.000000 GenIce2-2.1b4/genice2/loaders/__init__.py
+-rw-r--r--   0 matto      (505) staff       (20)     1048 2021-05-07 12:07:04.000000 GenIce2-2.1b4/genice2/loaders/ar3r.py
+-rw-r--r--   0 matto      (505) staff       (20)     3024 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/loaders/exyz.py
+-rw-r--r--   0 matto      (505) staff       (20)     2115 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/loaders/gro.py
+-rw-r--r--   0 matto      (505) staff       (20)     1893 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/loaders/mdv.py
+-rw-r--r--   0 matto      (505) staff       (20)     1893 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/loaders/mdva.py
+-rw-r--r--   0 matto      (505) staff       (20)     1624 2021-05-09 09:19:20.000000 GenIce2-2.1b4/genice2/loaders/nx3a.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-11 11:37:45.410917 GenIce2-2.1b4/genice2/molecules/
+-rw-r--r--   0 matto      (505) staff       (20)      669 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/3site.py
+-rw-r--r--   0 matto      (505) staff       (20)      866 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/4site.py
+-rw-r--r--   0 matto      (505) staff       (20)      984 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/5site.py
+-rw-r--r--   0 matto      (505) staff       (20)     1366 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/6site.py
+-rw-r--r--   0 matto      (505) staff       (20)     1153 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/7site.py
+-rw-r--r--   0 matto      (505) staff       (20)      476 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/H2.py
+-rw-r--r--   0 matto      (505) staff       (20)     1366 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/NvdE.py
+-rw-r--r--   0 matto      (505) staff       (20)     2139 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/__init__.py
+-rw-r--r--   0 matto      (505) staff       (20)      620 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/ch4.py
+-rw-r--r--   0 matto      (505) staff       (20)      362 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/co2.py
+-rw-r--r--   0 matto      (505) staff       (20)      275 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/empty.py
+-rw-r--r--   0 matto      (505) staff       (20)      217 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/g12.py
+-rw-r--r--   0 matto      (505) staff       (20)      217 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/g14.py
+-rw-r--r--   0 matto      (505) staff       (20)      217 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/g15.py
+-rw-r--r--   0 matto      (505) staff       (20)      217 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/g16.py
+-rw-r--r--   0 matto      (505) staff       (20)      909 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/ice.py
+-rw-r--r--   0 matto      (505) staff       (20)      320 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/me.py
+-rw-r--r--   0 matto      (505) staff       (20)     1216 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/mol.py
+-rw-r--r--   0 matto      (505) staff       (20)      447 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/one.py
+-rw-r--r--   0 matto      (505) staff       (20)      814 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/physical_water.py
+-rw-r--r--   0 matto      (505) staff       (20)      578 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/spce.py
+-rw-r--r--   0 matto      (505) staff       (20)      821 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/thf.py
+-rw-r--r--   0 matto      (505) staff       (20)      669 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/tip3p.py
+-rw-r--r--   0 matto      (505) staff       (20)      866 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/tip4p.py
+-rw-r--r--   0 matto      (505) staff       (20)      984 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/tip5p.py
+-rw-r--r--   0 matto      (505) staff       (20)      763 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/uathf.py
+-rw-r--r--   0 matto      (505) staff       (20)      730 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/molecules/uathf6.py
+-rw-r--r--   0 matto      (505) staff       (20)     9288 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/plugin.py
+-rw-r--r--   0 matto      (505) staff       (20)    12503 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/rigid.py
+-rw-r--r--   0 matto      (505) staff       (20)     3021 2021-05-11 10:34:09.000000 GenIce2-2.1b4/genice2/valueparser.py
+-rwxr-xr-x   0 matto      (505) staff       (20)       87 2021-05-11 10:34:09.000000 GenIce2-2.1b4/requirements.txt
+-rw-r--r--   0 matto      (505) staff       (20)      108 2021-05-11 11:37:45.411664 GenIce2-2.1b4/setup.cfg
+-rwxr-xr-x   0 matto      (505) staff       (20)     1616 2021-05-11 10:34:09.000000 GenIce2-2.1b4/setup.py
```

### Comparing `GenIce2-2.1b3/GenIce2.egg-info/PKG-INFO` & `GenIce2-2.1b4/GenIce2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: GenIce2
-Version: 2.1b3
+Version: 2.1b4
 Summary: A Swiss army knife to generate hydrogen-disordered ice structures.
 Home-page: https://github.com/vitroid/GenIce/
 Author: Masakazu Matsumoto
 Author-email: vitroid@gmail.com
 License: MIT
-Description: ['networkx>=2', 'cycless', 'pairlist>=0.2.3', 'yaplotlib>=0.1', 'numpy', 'wheel', 'openpyscad', 'graphstat']
-        ![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
+Description: ![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
         # GenIce2
         
         A Swiss army knife to generate hydrogen-disordered ice structures.
         
-        version 2.1b1
+        version 2.1b4
+        
+        
+        ## New in GenIce2.1
+        
+        GenIce2-MDAnalysis integration is now available. Try
+        ```shell
+        % pip install genice2-mdanalysis
+        % genice2 1h -r 4 4 4 -f "mdanalysis[1h.pdb]"
+        ```
+        to generate a PDB file.
         
         ## Demo
         
         The new GenIce works very well with interactive execution.
-        [Try instantly](https://colab.research.google.com/github/vitroid/GenIce/blob/main/colaboratory.ipynb) on Google Colab.
+        [Try instantly](https://colab.research.google.com/github/vitroid/GenIce/blob/main/jupyter.ipynb) on Google Colab.
         
         ## Requirements
         
         * networkx>=2
         * cycless
-        * pairlist>=0.2.3
+        * pairlist>=0.2.11.1
         * yaplotlib>=0.1
         * numpy
         * wheel
         * openpyscad
         * graphstat
         
         
@@ -48,15 +57,15 @@
                            [--seed SEED] [--format name] [--water model] [--guest 14=me]
                            [--Guest 13=me] [--Group 13=bu-:0] [--anion 3=Cl]
                            [--cation 3=Na] [--depol DEPOL] [--asis] [--debug] [--quiet]
                            [--assess_cages]
                            Type
             
             GenIce is a swiss army knife to generate hydrogen-disordered ice structures.
-            (version 2.1b1)
+            (version 2.1b4)
             
             positional arguments:
               Type                  Crystal type (1c, 1h, etc. See
                                     https://github.com/vitroid/GenIce for available ice
                                     structures.)
                                     If you want to analyze your own structures, please try
                                     analice tool.
@@ -164,34 +173,37 @@
                                                     guests are supplied.)
                                     c1te            Hydrogen-ordered hydrogen hydrate C1 by
                                                      Teeratchanan. (Positions of guests are
                                                      supplied.)
                                     c2te            Filled ice C2 (cubic ice) by
                                                     Teeratchanan (Hydrogen disordered).
                                                     (Positions of guests are supplied.)
+                                    eleven          Ice XI w/ stacking faults.
                                     i               Hypothetical ice "i".
                                     ice1hte         Filled ice Ih by Teeratchanan (Hydrogen
                                                      disordered). (Positions of guests are
                                                     supplied.)
                                     iceR            Hypothetical ice R.
                                     iceT            Hypothetical ice T.
                                     iceT2           Hypothetical ice T2.
                                     one             Ice I w/ stacking faults.
                                     prism           Ice nanotubes.
                                     sTprime         Filled ice sT'.
                                     xFAU            Aeroice xFAU.
                                     xdtc            A porous ice with cylindrical channels.
                                     ----
-                                    (Undocumented) 1h_unit HS1 Kcomp TS1 dtc eleven
-                                    ice1h_unit sIII sIV
+                                    (Undocumented) 1h_unit HS1 Kcomp TS1 dtc ice1h_unit
+                                    sIII sIV
             
             
                                     2. Lattice structures served by external plugins
             
-                                    (None)
+                                    cif             Read a CIF file.
+                                    zeolite         Retrieve a structure from the IZA
+                                                    Zeolite DB.
                                     ----
             
             
                                     3. Lattice structures served locally
             
                                     (None)
                                     ----
@@ -239,15 +251,21 @@
                                     y, yaplot       Yaplot.
                                     ----
                                     (Undocumented) c cif cif2 com null r rcom towhee xyz
             
             
                                     2. Formatters served by external plugins
             
-                                    (None)
+                                    _RDF            Radial Distribution Functions.
+                                    cage            Cage analysis.
+                                    mdanalysis      MDAnalysis integration.
+                                    meshcat         Meshcat + Google Colab.
+                                    png             PNG (Portable Network Graphics).
+                                    svg             SVG (Standard Vector Graphics).
+                                    twist           Twist order parameter.
                                     ----
             
             
                                     3. Formatters served locally
             
                                     (None)
                                     ----
@@ -498,21 +516,24 @@
         `c`, `com`      |CenterOfMass| `.ar3a`     | Center of mass | none | none |
         `r`, `rcom`      |Relative CoM| `.ar3r`     | Center of mass | none | none | In fractional coordinate system.
         `p`, `python`, `reshape`      |Python module | `.py`     | Center of mass | none | none | Under development.
         `_ringstat`      |Ring phase statistics |     | |  | | Statistical test suite 1: Check the appearance frequencies of the ring phases as a test for the intermediate-range disorder.
         `rings`      |[Yaplot](https://github.com/vitroid/Yaplot)      | `.yap`      | center of mass | none |o | It renders HB rings.
         `_KG`      |Kirkwood G(r)|     | |  | | Statistical test suite 2: Calculate G(r) for checking long-range disorder in molecular orientations.
         
-        By installing the [`genice-mdanalysis`](https://github.com/vitroid/genice-mdanalysis) package separately, you can generate files in many formats for a  large number of molecular dynamics package softwares. E.g.
+        By installing the [`genice2-mdanalysis`](https://github.com/vitroid/genice-mdanalysis) package separately, you can generate files in many formats for a  large number of molecular dynamics package softwares. E.g.
         
         ```shell
-        % genice2 1c -f mdanalysis[1c.pdb]
-        % genice2 1h -f mdanalysis[1h.xtc]
+        % pip install genice2-mdanalysis
+        % genice2 1c -f 'mdanalysis[1c.pdb]'
+        % genice2 1h -f 'mdanalysis[1h.xtc]'
         ```
         
+        All the supported file types are listed in the [MDAnalysis web page](https://docs.mdanalysis.org/stable/documentation_pages/coordinates/init.html#supported-coordinate-formats).
+        
         You can prepare your file formats. Create a folder named `formats` in the current working directory and put the plugins in it.
         
         Internally, there are seven stages to generate an ice structure.
         
         1. Cell repetition.
         2. Random graph generation and replication.
         3. Apply ice rule.
@@ -524,23 +545,23 @@
         In the format plugin, you define the hook functions that are invoked after processing each stage.
         
         ## Ice structures
         
         Symbol | <div style="width:300px">Description</div>
         -------|------------
         0, ice0 | Metastable ice "0". [Russo 2014]
-        11, XI, ice11 | A candidate for an antiferroelectric Ice XI #19. [Jackson 1997,Fan 2010]
-        115_2_114, 11_2_15848, 12_1_11, 12_2_29187, 12_2_32449, 144_2_7301, 14_2_48453, 151_2_4949650, 152_2_118474, 153_2_155471, 15_2_201714, 169_2_10608, 169_2_7915, 176_2_5256, 207_1_4435, 20_2_26425, 20_2_28176, 2_2_342692, 2_2_623457, 53_3_726600, 58_2_511, 61_2_8842, 67_2_1444, 67_2_1563, 84_2_1419, 91_2_8335121, ACO, CS4, DDR, IRR, IWV, LTA, MAR, NON, PCOD8007225, PCOD8036144, PCOD8045578, PCOD8047078, PCOD8047931, PCOD8172143, PCOD8204698, PCOD8301974, PCOD8321499, PCOD8324623, SGT, SOD, engel01, engel02, engel03, engel04, engel06, engel07, engel08, engel09, engel10, engel11, engel12, engel13, engel14, engel15, engel16, engel17, engel18, engel19, engel20, engel21, engel22, engel23, engel24, engel25, engel26, engel27, engel28, engel29, engel30, engel31, engel32, engel33, engel34, sVII | Hypothetical zeolitic ice [Kosyakov 1999,IZA Database,Engel 2018,Jeffrey 1984]
+        11, XI, ice11 | A candidate for an antiferroelectric Ice XI #19. [Fan 2010,Jackson 1997]
+        115_2_114, 11_2_15848, 12_1_11, 12_2_29187, 12_2_32449, 144_2_7301, 14_2_48453, 151_2_4949650, 152_2_118474, 153_2_155471, 15_2_201714, 169_2_10608, 169_2_7915, 176_2_5256, 207_1_4435, 20_2_26425, 20_2_28176, 2_2_342692, 2_2_623457, 53_3_726600, 58_2_511, 61_2_8842, 67_2_1444, 67_2_1563, 84_2_1419, 91_2_8335121, ACO, CS4, DDR, IRR, IWV, LTA, MAR, NON, PCOD8007225, PCOD8036144, PCOD8045578, PCOD8047078, PCOD8047931, PCOD8172143, PCOD8204698, PCOD8301974, PCOD8321499, PCOD8324623, SGT, SOD, engel01, engel02, engel03, engel04, engel06, engel07, engel08, engel09, engel10, engel11, engel12, engel13, engel14, engel15, engel16, engel17, engel18, engel19, engel20, engel21, engel22, engel23, engel24, engel25, engel26, engel27, engel28, engel29, engel30, engel31, engel32, engel33, engel34, sVII | Hypothetical zeolitic ice [Engel 2018,IZA Database,Kosyakov 1999,Jeffrey 1984]
         12, XII, ice12 | Metastable high-pressure ice XII. [Lobban 1998,Koza 2000]
         13, XIII, ice13 | Ice XIII, a hydrogen-ordered counterpart of ice V. [Salzmann 2006]
-        16, CS2, MTN, XVI, ice16, sII | Ultralow-density Ice XVI. [Kosyakov 1999,Falenty 2014,IZA Database,Sikiric 2010,Jeffrey 1984]
-        17, XVII, ice17 | Ultralow-density Ice XVII. [Strobel 2016,Smirnov 2013,Rosso 2016]
+        16, CS2, MTN, XVI, ice16, sII | Ultralow-density Ice XVI. [IZA Database,Jeffrey 1984,Sikiric 2010,Falenty 2014,Kosyakov 1999]
+        17, XVII, ice17 | Ultralow-density Ice XVII. [Smirnov 2013,Rosso 2016,Strobel 2016]
         1c, Ic, ice1c | Cubic type of ice I. [Vos 1993]
         1h, Ih, ice1h | Most popular Ice I (hexagonal)
-        2, II, ice2 | Hydrogen-ordered ice II. [Kamb 2003,Kamb 1964,Londono 1988]
+        2, II, ice2 | Hydrogen-ordered ice II. [Kamb 2003,Londono 1988,Kamb 1964]
         2D3 | Trilayer honeycomb ice.
         2d, ice2d, ice2rect | A hydrogen-disordered counterpart of ice II. [Nakamura 2015]
         3, III, ice3 | Ice III. [Petrenko 1999]
         4, IV, ice4 | Ice IV. [Avogadro]
         4R | Orthogonalized ice IV. [Avogadro]
         5, V, ice5 | Monoclinic ice V (testing).
         5R | Ice V with orthogonal unit cell. (testing)
@@ -548,37 +569,38 @@
         6h | Half lattice of ice VI.
         7, VII, ice7 | Conventional high-pressure ice VII.
         8, VIII, ice8 | Ice VIII, a hydrogen-ordered counterpart of ice VII. [Kuhs 1998]
         9, IX, ice9 | Ice IX, a hydrogen-ordered counterpart of ice III. [Londono 1993]
         A, iceA | Hypothetical ice A. [Baez 1998]
         A15, Struct33 | Cubic Structure I of clathrate hydrate. [Sikiric 2010]
         B, iceB | Hypothetical ice B. [Baez 1998]
-        BSV, engel05 | Hypothetical zeolitic ice of the gyroid structure. [IZA Database,Engel 2018]
+        BSV, engel05 | Hypothetical zeolitic ice of the gyroid structure. [Engel 2018,IZA Database]
         C14, C15, C36, FK6layers, FK9layers, HS2, Hcomp, Struct01, Struct02, Struct03, Struct04, Struct05, Struct06, Struct07, Struct08, Struct09, Struct10, Struct11, Struct12, Struct13, Struct14, Struct15, Struct16, Struct17, Struct18, Struct19, Struct20, Struct21, Struct22, Struct23, Struct24, Struct25, Struct26, Struct27, Struct28, Struct29, Struct30, Struct31, Struct32, Struct34, Struct35, Struct36, Struct37, Struct38, Struct39, Struct40, Struct41, Struct42, Struct43, Struct44, Struct45, Struct46, Struct47, Struct48, Struct49, Struct50, Struct51, Struct52, Struct53, Struct54, Struct55, Struct56, Struct57, Struct58, Struct59, Struct60, Struct61, Struct62, Struct63, Struct64, Struct65, Struct66, Struct67, Struct68, Struct69, Struct70, Struct71, Struct72, Struct73, Struct74, Struct75, Struct76, Struct77, Struct78, Struct79, Struct80, Struct81, Struct82, Struct83, Struct84, Z, delta, mu, psigma, sV, sigma, zra-d | A space fullerene. [Sikiric 2010]
         CRN1, CRN2, CRN3 | A continuous random network of Sillium. [Mousseau 2001]
-        CS1, MEP, sI | Clathrate hydrates sI. [Kosyakov 1999,IZA Database,Frank 1959,Jeffrey 1984]
+        CS1, MEP, sI | Clathrate hydrates sI. [Frank 1959,IZA Database,Jeffrey 1984,Kosyakov 1999]
         DOH, HS3, sH | Clathrate type H.
-        EMT | Hypothetical ice with a large cavity. [Liu 2019,IZA Database]
+        EMT | Hypothetical ice with a large cavity. [IZA Database,Liu 2019]
         FAU | Hypothetical ice at negative pressure ice 'sIV'. [Huang 2017,IZA Database]
         RHO | Hypothetical ice at negative pressure ice 'sIII'. [Huang 2016,IZA Database]
         T | Hypothetical clathrate type T. [Sikiric 2010,Karttunen 2011]
         c0te | Filled ice C0 by Teeratchanan (Hydrogen-disordered.) (Positions of guests are supplied.) [Teeratchanan 2015]
         c1te | Hydrogen-ordered hydrogen hydrate C1 by Teeratchanan. (Positions of guests are supplied.) [Teeratchanan 2015]
         c2te | Filled ice C2 (cubic ice) by Teeratchanan (Hydrogen disordered). (Positions of guests are supplied.) [Teeratchanan 2015]
+        eleven | Ice XI w/ stacking faults.
         i | Hypothetical ice "i". [Fennell 2005]
         ice1hte | Filled ice Ih by Teeratchanan (Hydrogen disordered). (Positions of guests are supplied.) [Teeratchanan 2015]
-        iceR | Hypothetical ice R. [Maynard-Casely 2010,Mochizuki 2014]
+        iceR | Hypothetical ice R. [Mochizuki 2014,Maynard-Casely 2010]
         iceT | Hypothetical ice T. [Hirata 2017]
         iceT2 | Hypothetical ice T2. [Yagasaki 2018]
         one | Ice I w/ stacking faults.
         prism | Ice nanotubes. [Koga 2001]
         sTprime | Filled ice sT'. [Smirnov 2013]
         xFAU | Aeroice xFAU. [Matsui 2017]
         xdtc | A porous ice with cylindrical channels. [Matsumoto 2021]
-        1h_unit, HS1, Kcomp, TS1, dtc, eleven, ice1h_unit, sIII, sIV | (Undocumented)
+        1h_unit, HS1, Kcomp, TS1, dtc, ice1h_unit, sIII, sIV | (Undocumented)
         
         
         Ice names with double quotations are not experimentally verified.
         
         You can prepare your own ice structures. Create a folder named `lattices` in the current working directory and put the plugins in it.
         
         [cif2ice](https://github.com/vitroid/cif2ice) is a tool to retrieve a
@@ -654,15 +676,15 @@
         
         | pip name | GenIce2 option | Description | output format | requirements |
         |----------|-------|-------------|---------------|--------------|
         |[`genice2-cage`](https://github.com/vitroid/genice-cage)|`-f _cage`| Detect cages and quasi-polyhedra (vitrites). | text, json | `cycless` |
         |[`genice2-rdf`](https://github.com/vitroid/genice-rdf)|`-f _RDF`| Radial distribution functions. | text |  |
         |[`genice2-svg`](https://github.com/vitroid/genice-svg)|`-f svg`<br />`-f png` | 2D graphics in SVG format.<br /> ... in PNG format.| SVG<br />PNG | `svgwrite` |
         |[`genice2-twist`](https://github.com/vitroid/genice-twist)|`-f twist`| Calculate the twist order parameter (and visualize) [Matsumoto 2019]| text (@BTWC)<br />SVG<br />PNG <br />yaplot | `twist-op`, `genice2-svg` |
-        
+        |[`genice2-mdanalysis`](https://github.com/vitroid/genice-mdanalysis)|`-f mdanalysis`| Output the atoms in various file formats that are served by [MDAnalysis](https://github.com/MDAnalysis/mdanalysis).| text, binary | `mdanalysis` |
         ## Input plugins
         
         Input plugins (a.k.a. lattice plugins) construct a crystal structure on demand.
         
         | pip name   | GenIce2 usage    | Description  |requirements |
         |------------|-----------------|--------------|-------------|
         |[`genice2-cif`](https://github.com/vitroid/genice-cif)| `genice2 cif[ITT.cif]`<br /> `genice2 zeolite[ITT]`| Read a local CIF file as an ice structure.<br />Read a structure from Zeolite DB. | `cif2ice` |
@@ -679,20 +701,23 @@
         
         ## Faster, faster, faster.
         
         Combinations of the new algorithm and other improvements in coding, the processing time of GenIce2 is about five times faster than that of GenIce1.
         
         ## Colaboratory-ready!
         
-        Now GenIce2 works on the [Google Colaboratory!](https://colab.research.google.com/github/vitroid/GenIce/blob/genice2/test.ipynb)
+        Now GenIce2 works on the [Google Colaboratory!](https://colab.research.google.com/github/vitroid/GenIce/blob/genice2/jupyter.ipynb)
         
         ## New ices
         
         Many new ice structures are added.
         
+        ## Integration with MDAnalysis
+        
+        GenIce2 is now integrated with MDAnalysis.
         
         # References
         
         * [Avogadro] Avogadro https://github.com/cryos/avogadro/blob/master/crystals/ice/H2O-Ice-IV.cif
         * [Baez 1998] 
         BÁEZ, Luis A. and CLANCY, Paulette, 1995, Phase equilibria in extended simple point charge ice‐water systems. The Journal of Chemical Physics [online]. 8 December 1995. Vol. 103, no. 22, p. 9744–9755. DOI 10.1063/1.469938. Available from: http://dx.doi.org/10.1063/1.469938
```

### Comparing `GenIce2-2.1b3/GenIce2.egg-info/SOURCES.txt` & `GenIce2-2.1b4/GenIce2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/PKG-INFO` & `GenIce2-2.1b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: GenIce2
-Version: 2.1b3
+Version: 2.1b4
 Summary: A Swiss army knife to generate hydrogen-disordered ice structures.
 Home-page: https://github.com/vitroid/GenIce/
 Author: Masakazu Matsumoto
 Author-email: vitroid@gmail.com
 License: MIT
-Description: ['networkx>=2', 'cycless', 'pairlist>=0.2.3', 'yaplotlib>=0.1', 'numpy', 'wheel', 'openpyscad', 'graphstat']
-        ![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
+Description: ![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
         # GenIce2
         
         A Swiss army knife to generate hydrogen-disordered ice structures.
         
-        version 2.1b1
+        version 2.1b4
+        
+        
+        ## New in GenIce2.1
+        
+        GenIce2-MDAnalysis integration is now available. Try
+        ```shell
+        % pip install genice2-mdanalysis
+        % genice2 1h -r 4 4 4 -f "mdanalysis[1h.pdb]"
+        ```
+        to generate a PDB file.
         
         ## Demo
         
         The new GenIce works very well with interactive execution.
-        [Try instantly](https://colab.research.google.com/github/vitroid/GenIce/blob/main/colaboratory.ipynb) on Google Colab.
+        [Try instantly](https://colab.research.google.com/github/vitroid/GenIce/blob/main/jupyter.ipynb) on Google Colab.
         
         ## Requirements
         
         * networkx>=2
         * cycless
-        * pairlist>=0.2.3
+        * pairlist>=0.2.11.1
         * yaplotlib>=0.1
         * numpy
         * wheel
         * openpyscad
         * graphstat
         
         
@@ -48,15 +57,15 @@
                            [--seed SEED] [--format name] [--water model] [--guest 14=me]
                            [--Guest 13=me] [--Group 13=bu-:0] [--anion 3=Cl]
                            [--cation 3=Na] [--depol DEPOL] [--asis] [--debug] [--quiet]
                            [--assess_cages]
                            Type
             
             GenIce is a swiss army knife to generate hydrogen-disordered ice structures.
-            (version 2.1b1)
+            (version 2.1b4)
             
             positional arguments:
               Type                  Crystal type (1c, 1h, etc. See
                                     https://github.com/vitroid/GenIce for available ice
                                     structures.)
                                     If you want to analyze your own structures, please try
                                     analice tool.
@@ -164,34 +173,37 @@
                                                     guests are supplied.)
                                     c1te            Hydrogen-ordered hydrogen hydrate C1 by
                                                      Teeratchanan. (Positions of guests are
                                                      supplied.)
                                     c2te            Filled ice C2 (cubic ice) by
                                                     Teeratchanan (Hydrogen disordered).
                                                     (Positions of guests are supplied.)
+                                    eleven          Ice XI w/ stacking faults.
                                     i               Hypothetical ice "i".
                                     ice1hte         Filled ice Ih by Teeratchanan (Hydrogen
                                                      disordered). (Positions of guests are
                                                     supplied.)
                                     iceR            Hypothetical ice R.
                                     iceT            Hypothetical ice T.
                                     iceT2           Hypothetical ice T2.
                                     one             Ice I w/ stacking faults.
                                     prism           Ice nanotubes.
                                     sTprime         Filled ice sT'.
                                     xFAU            Aeroice xFAU.
                                     xdtc            A porous ice with cylindrical channels.
                                     ----
-                                    (Undocumented) 1h_unit HS1 Kcomp TS1 dtc eleven
-                                    ice1h_unit sIII sIV
+                                    (Undocumented) 1h_unit HS1 Kcomp TS1 dtc ice1h_unit
+                                    sIII sIV
             
             
                                     2. Lattice structures served by external plugins
             
-                                    (None)
+                                    cif             Read a CIF file.
+                                    zeolite         Retrieve a structure from the IZA
+                                                    Zeolite DB.
                                     ----
             
             
                                     3. Lattice structures served locally
             
                                     (None)
                                     ----
@@ -239,15 +251,21 @@
                                     y, yaplot       Yaplot.
                                     ----
                                     (Undocumented) c cif cif2 com null r rcom towhee xyz
             
             
                                     2. Formatters served by external plugins
             
-                                    (None)
+                                    _RDF            Radial Distribution Functions.
+                                    cage            Cage analysis.
+                                    mdanalysis      MDAnalysis integration.
+                                    meshcat         Meshcat + Google Colab.
+                                    png             PNG (Portable Network Graphics).
+                                    svg             SVG (Standard Vector Graphics).
+                                    twist           Twist order parameter.
                                     ----
             
             
                                     3. Formatters served locally
             
                                     (None)
                                     ----
@@ -498,21 +516,24 @@
         `c`, `com`      |CenterOfMass| `.ar3a`     | Center of mass | none | none |
         `r`, `rcom`      |Relative CoM| `.ar3r`     | Center of mass | none | none | In fractional coordinate system.
         `p`, `python`, `reshape`      |Python module | `.py`     | Center of mass | none | none | Under development.
         `_ringstat`      |Ring phase statistics |     | |  | | Statistical test suite 1: Check the appearance frequencies of the ring phases as a test for the intermediate-range disorder.
         `rings`      |[Yaplot](https://github.com/vitroid/Yaplot)      | `.yap`      | center of mass | none |o | It renders HB rings.
         `_KG`      |Kirkwood G(r)|     | |  | | Statistical test suite 2: Calculate G(r) for checking long-range disorder in molecular orientations.
         
-        By installing the [`genice-mdanalysis`](https://github.com/vitroid/genice-mdanalysis) package separately, you can generate files in many formats for a  large number of molecular dynamics package softwares. E.g.
+        By installing the [`genice2-mdanalysis`](https://github.com/vitroid/genice-mdanalysis) package separately, you can generate files in many formats for a  large number of molecular dynamics package softwares. E.g.
         
         ```shell
-        % genice2 1c -f mdanalysis[1c.pdb]
-        % genice2 1h -f mdanalysis[1h.xtc]
+        % pip install genice2-mdanalysis
+        % genice2 1c -f 'mdanalysis[1c.pdb]'
+        % genice2 1h -f 'mdanalysis[1h.xtc]'
         ```
         
+        All the supported file types are listed in the [MDAnalysis web page](https://docs.mdanalysis.org/stable/documentation_pages/coordinates/init.html#supported-coordinate-formats).
+        
         You can prepare your file formats. Create a folder named `formats` in the current working directory and put the plugins in it.
         
         Internally, there are seven stages to generate an ice structure.
         
         1. Cell repetition.
         2. Random graph generation and replication.
         3. Apply ice rule.
@@ -524,23 +545,23 @@
         In the format plugin, you define the hook functions that are invoked after processing each stage.
         
         ## Ice structures
         
         Symbol | <div style="width:300px">Description</div>
         -------|------------
         0, ice0 | Metastable ice "0". [Russo 2014]
-        11, XI, ice11 | A candidate for an antiferroelectric Ice XI #19. [Jackson 1997,Fan 2010]
-        115_2_114, 11_2_15848, 12_1_11, 12_2_29187, 12_2_32449, 144_2_7301, 14_2_48453, 151_2_4949650, 152_2_118474, 153_2_155471, 15_2_201714, 169_2_10608, 169_2_7915, 176_2_5256, 207_1_4435, 20_2_26425, 20_2_28176, 2_2_342692, 2_2_623457, 53_3_726600, 58_2_511, 61_2_8842, 67_2_1444, 67_2_1563, 84_2_1419, 91_2_8335121, ACO, CS4, DDR, IRR, IWV, LTA, MAR, NON, PCOD8007225, PCOD8036144, PCOD8045578, PCOD8047078, PCOD8047931, PCOD8172143, PCOD8204698, PCOD8301974, PCOD8321499, PCOD8324623, SGT, SOD, engel01, engel02, engel03, engel04, engel06, engel07, engel08, engel09, engel10, engel11, engel12, engel13, engel14, engel15, engel16, engel17, engel18, engel19, engel20, engel21, engel22, engel23, engel24, engel25, engel26, engel27, engel28, engel29, engel30, engel31, engel32, engel33, engel34, sVII | Hypothetical zeolitic ice [Kosyakov 1999,IZA Database,Engel 2018,Jeffrey 1984]
+        11, XI, ice11 | A candidate for an antiferroelectric Ice XI #19. [Fan 2010,Jackson 1997]
+        115_2_114, 11_2_15848, 12_1_11, 12_2_29187, 12_2_32449, 144_2_7301, 14_2_48453, 151_2_4949650, 152_2_118474, 153_2_155471, 15_2_201714, 169_2_10608, 169_2_7915, 176_2_5256, 207_1_4435, 20_2_26425, 20_2_28176, 2_2_342692, 2_2_623457, 53_3_726600, 58_2_511, 61_2_8842, 67_2_1444, 67_2_1563, 84_2_1419, 91_2_8335121, ACO, CS4, DDR, IRR, IWV, LTA, MAR, NON, PCOD8007225, PCOD8036144, PCOD8045578, PCOD8047078, PCOD8047931, PCOD8172143, PCOD8204698, PCOD8301974, PCOD8321499, PCOD8324623, SGT, SOD, engel01, engel02, engel03, engel04, engel06, engel07, engel08, engel09, engel10, engel11, engel12, engel13, engel14, engel15, engel16, engel17, engel18, engel19, engel20, engel21, engel22, engel23, engel24, engel25, engel26, engel27, engel28, engel29, engel30, engel31, engel32, engel33, engel34, sVII | Hypothetical zeolitic ice [Engel 2018,IZA Database,Kosyakov 1999,Jeffrey 1984]
         12, XII, ice12 | Metastable high-pressure ice XII. [Lobban 1998,Koza 2000]
         13, XIII, ice13 | Ice XIII, a hydrogen-ordered counterpart of ice V. [Salzmann 2006]
-        16, CS2, MTN, XVI, ice16, sII | Ultralow-density Ice XVI. [Kosyakov 1999,Falenty 2014,IZA Database,Sikiric 2010,Jeffrey 1984]
-        17, XVII, ice17 | Ultralow-density Ice XVII. [Strobel 2016,Smirnov 2013,Rosso 2016]
+        16, CS2, MTN, XVI, ice16, sII | Ultralow-density Ice XVI. [IZA Database,Jeffrey 1984,Sikiric 2010,Falenty 2014,Kosyakov 1999]
+        17, XVII, ice17 | Ultralow-density Ice XVII. [Smirnov 2013,Rosso 2016,Strobel 2016]
         1c, Ic, ice1c | Cubic type of ice I. [Vos 1993]
         1h, Ih, ice1h | Most popular Ice I (hexagonal)
-        2, II, ice2 | Hydrogen-ordered ice II. [Kamb 2003,Kamb 1964,Londono 1988]
+        2, II, ice2 | Hydrogen-ordered ice II. [Kamb 2003,Londono 1988,Kamb 1964]
         2D3 | Trilayer honeycomb ice.
         2d, ice2d, ice2rect | A hydrogen-disordered counterpart of ice II. [Nakamura 2015]
         3, III, ice3 | Ice III. [Petrenko 1999]
         4, IV, ice4 | Ice IV. [Avogadro]
         4R | Orthogonalized ice IV. [Avogadro]
         5, V, ice5 | Monoclinic ice V (testing).
         5R | Ice V with orthogonal unit cell. (testing)
@@ -548,37 +569,38 @@
         6h | Half lattice of ice VI.
         7, VII, ice7 | Conventional high-pressure ice VII.
         8, VIII, ice8 | Ice VIII, a hydrogen-ordered counterpart of ice VII. [Kuhs 1998]
         9, IX, ice9 | Ice IX, a hydrogen-ordered counterpart of ice III. [Londono 1993]
         A, iceA | Hypothetical ice A. [Baez 1998]
         A15, Struct33 | Cubic Structure I of clathrate hydrate. [Sikiric 2010]
         B, iceB | Hypothetical ice B. [Baez 1998]
-        BSV, engel05 | Hypothetical zeolitic ice of the gyroid structure. [IZA Database,Engel 2018]
+        BSV, engel05 | Hypothetical zeolitic ice of the gyroid structure. [Engel 2018,IZA Database]
         C14, C15, C36, FK6layers, FK9layers, HS2, Hcomp, Struct01, Struct02, Struct03, Struct04, Struct05, Struct06, Struct07, Struct08, Struct09, Struct10, Struct11, Struct12, Struct13, Struct14, Struct15, Struct16, Struct17, Struct18, Struct19, Struct20, Struct21, Struct22, Struct23, Struct24, Struct25, Struct26, Struct27, Struct28, Struct29, Struct30, Struct31, Struct32, Struct34, Struct35, Struct36, Struct37, Struct38, Struct39, Struct40, Struct41, Struct42, Struct43, Struct44, Struct45, Struct46, Struct47, Struct48, Struct49, Struct50, Struct51, Struct52, Struct53, Struct54, Struct55, Struct56, Struct57, Struct58, Struct59, Struct60, Struct61, Struct62, Struct63, Struct64, Struct65, Struct66, Struct67, Struct68, Struct69, Struct70, Struct71, Struct72, Struct73, Struct74, Struct75, Struct76, Struct77, Struct78, Struct79, Struct80, Struct81, Struct82, Struct83, Struct84, Z, delta, mu, psigma, sV, sigma, zra-d | A space fullerene. [Sikiric 2010]
         CRN1, CRN2, CRN3 | A continuous random network of Sillium. [Mousseau 2001]
-        CS1, MEP, sI | Clathrate hydrates sI. [Kosyakov 1999,IZA Database,Frank 1959,Jeffrey 1984]
+        CS1, MEP, sI | Clathrate hydrates sI. [Frank 1959,IZA Database,Jeffrey 1984,Kosyakov 1999]
         DOH, HS3, sH | Clathrate type H.
-        EMT | Hypothetical ice with a large cavity. [Liu 2019,IZA Database]
+        EMT | Hypothetical ice with a large cavity. [IZA Database,Liu 2019]
         FAU | Hypothetical ice at negative pressure ice 'sIV'. [Huang 2017,IZA Database]
         RHO | Hypothetical ice at negative pressure ice 'sIII'. [Huang 2016,IZA Database]
         T | Hypothetical clathrate type T. [Sikiric 2010,Karttunen 2011]
         c0te | Filled ice C0 by Teeratchanan (Hydrogen-disordered.) (Positions of guests are supplied.) [Teeratchanan 2015]
         c1te | Hydrogen-ordered hydrogen hydrate C1 by Teeratchanan. (Positions of guests are supplied.) [Teeratchanan 2015]
         c2te | Filled ice C2 (cubic ice) by Teeratchanan (Hydrogen disordered). (Positions of guests are supplied.) [Teeratchanan 2015]
+        eleven | Ice XI w/ stacking faults.
         i | Hypothetical ice "i". [Fennell 2005]
         ice1hte | Filled ice Ih by Teeratchanan (Hydrogen disordered). (Positions of guests are supplied.) [Teeratchanan 2015]
-        iceR | Hypothetical ice R. [Maynard-Casely 2010,Mochizuki 2014]
+        iceR | Hypothetical ice R. [Mochizuki 2014,Maynard-Casely 2010]
         iceT | Hypothetical ice T. [Hirata 2017]
         iceT2 | Hypothetical ice T2. [Yagasaki 2018]
         one | Ice I w/ stacking faults.
         prism | Ice nanotubes. [Koga 2001]
         sTprime | Filled ice sT'. [Smirnov 2013]
         xFAU | Aeroice xFAU. [Matsui 2017]
         xdtc | A porous ice with cylindrical channels. [Matsumoto 2021]
-        1h_unit, HS1, Kcomp, TS1, dtc, eleven, ice1h_unit, sIII, sIV | (Undocumented)
+        1h_unit, HS1, Kcomp, TS1, dtc, ice1h_unit, sIII, sIV | (Undocumented)
         
         
         Ice names with double quotations are not experimentally verified.
         
         You can prepare your own ice structures. Create a folder named `lattices` in the current working directory and put the plugins in it.
         
         [cif2ice](https://github.com/vitroid/cif2ice) is a tool to retrieve a
@@ -654,15 +676,15 @@
         
         | pip name | GenIce2 option | Description | output format | requirements |
         |----------|-------|-------------|---------------|--------------|
         |[`genice2-cage`](https://github.com/vitroid/genice-cage)|`-f _cage`| Detect cages and quasi-polyhedra (vitrites). | text, json | `cycless` |
         |[`genice2-rdf`](https://github.com/vitroid/genice-rdf)|`-f _RDF`| Radial distribution functions. | text |  |
         |[`genice2-svg`](https://github.com/vitroid/genice-svg)|`-f svg`<br />`-f png` | 2D graphics in SVG format.<br /> ... in PNG format.| SVG<br />PNG | `svgwrite` |
         |[`genice2-twist`](https://github.com/vitroid/genice-twist)|`-f twist`| Calculate the twist order parameter (and visualize) [Matsumoto 2019]| text (@BTWC)<br />SVG<br />PNG <br />yaplot | `twist-op`, `genice2-svg` |
-        
+        |[`genice2-mdanalysis`](https://github.com/vitroid/genice-mdanalysis)|`-f mdanalysis`| Output the atoms in various file formats that are served by [MDAnalysis](https://github.com/MDAnalysis/mdanalysis).| text, binary | `mdanalysis` |
         ## Input plugins
         
         Input plugins (a.k.a. lattice plugins) construct a crystal structure on demand.
         
         | pip name   | GenIce2 usage    | Description  |requirements |
         |------------|-----------------|--------------|-------------|
         |[`genice2-cif`](https://github.com/vitroid/genice-cif)| `genice2 cif[ITT.cif]`<br /> `genice2 zeolite[ITT]`| Read a local CIF file as an ice structure.<br />Read a structure from Zeolite DB. | `cif2ice` |
@@ -679,20 +701,23 @@
         
         ## Faster, faster, faster.
         
         Combinations of the new algorithm and other improvements in coding, the processing time of GenIce2 is about five times faster than that of GenIce1.
         
         ## Colaboratory-ready!
         
-        Now GenIce2 works on the [Google Colaboratory!](https://colab.research.google.com/github/vitroid/GenIce/blob/genice2/test.ipynb)
+        Now GenIce2 works on the [Google Colaboratory!](https://colab.research.google.com/github/vitroid/GenIce/blob/genice2/jupyter.ipynb)
         
         ## New ices
         
         Many new ice structures are added.
         
+        ## Integration with MDAnalysis
+        
+        GenIce2 is now integrated with MDAnalysis.
         
         # References
         
         * [Avogadro] Avogadro https://github.com/cryos/avogadro/blob/master/crystals/ice/H2O-Ice-IV.cif
         * [Baez 1998] 
         BÁEZ, Luis A. and CLANCY, Paulette, 1995, Phase equilibria in extended simple point charge ice‐water systems. The Journal of Chemical Physics [online]. 8 December 1995. Vol. 103, no. 22, p. 9744–9755. DOI 10.1063/1.469938. Available from: http://dx.doi.org/10.1063/1.469938
```

### Comparing `GenIce2-2.1b3/README.md` & `GenIce2-2.1b4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,34 @@
-['networkx>=2', 'cycless', 'pairlist>=0.2.3', 'yaplotlib>=0.1', 'numpy', 'wheel', 'openpyscad', 'graphstat']
 ![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
 # GenIce2
 
 A Swiss army knife to generate hydrogen-disordered ice structures.
 
-version 2.1b1
+version 2.1b4
+
+
+## New in GenIce2.1
+
+GenIce2-MDAnalysis integration is now available. Try
+```shell
+% pip install genice2-mdanalysis
+% genice2 1h -r 4 4 4 -f "mdanalysis[1h.pdb]"
+```
+to generate a PDB file.
 
 ## Demo
 
 The new GenIce works very well with interactive execution.
-[Try instantly](https://colab.research.google.com/github/vitroid/GenIce/blob/main/colaboratory.ipynb) on Google Colab.
+[Try instantly](https://colab.research.google.com/github/vitroid/GenIce/blob/main/jupyter.ipynb) on Google Colab.
 
 ## Requirements
 
 * networkx>=2
 * cycless
-* pairlist>=0.2.3
+* pairlist>=0.2.11.1
 * yaplotlib>=0.1
 * numpy
 * wheel
 * openpyscad
 * graphstat
 
 
@@ -40,15 +49,15 @@
                    [--seed SEED] [--format name] [--water model] [--guest 14=me]
                    [--Guest 13=me] [--Group 13=bu-:0] [--anion 3=Cl]
                    [--cation 3=Na] [--depol DEPOL] [--asis] [--debug] [--quiet]
                    [--assess_cages]
                    Type
     
     GenIce is a swiss army knife to generate hydrogen-disordered ice structures.
-    (version 2.1b1)
+    (version 2.1b4)
     
     positional arguments:
       Type                  Crystal type (1c, 1h, etc. See
                             https://github.com/vitroid/GenIce for available ice
                             structures.)
                             If you want to analyze your own structures, please try
                             analice tool.
@@ -156,34 +165,37 @@
                                             guests are supplied.)
                             c1te            Hydrogen-ordered hydrogen hydrate C1 by
                                              Teeratchanan. (Positions of guests are
                                              supplied.)
                             c2te            Filled ice C2 (cubic ice) by
                                             Teeratchanan (Hydrogen disordered).
                                             (Positions of guests are supplied.)
+                            eleven          Ice XI w/ stacking faults.
                             i               Hypothetical ice "i".
                             ice1hte         Filled ice Ih by Teeratchanan (Hydrogen
                                              disordered). (Positions of guests are
                                             supplied.)
                             iceR            Hypothetical ice R.
                             iceT            Hypothetical ice T.
                             iceT2           Hypothetical ice T2.
                             one             Ice I w/ stacking faults.
                             prism           Ice nanotubes.
                             sTprime         Filled ice sT'.
                             xFAU            Aeroice xFAU.
                             xdtc            A porous ice with cylindrical channels.
                             ----
-                            (Undocumented) 1h_unit HS1 Kcomp TS1 dtc eleven
-                            ice1h_unit sIII sIV
+                            (Undocumented) 1h_unit HS1 Kcomp TS1 dtc ice1h_unit
+                            sIII sIV
     
     
                             2. Lattice structures served by external plugins
     
-                            (None)
+                            cif             Read a CIF file.
+                            zeolite         Retrieve a structure from the IZA
+                                            Zeolite DB.
                             ----
     
     
                             3. Lattice structures served locally
     
                             (None)
                             ----
@@ -231,15 +243,21 @@
                             y, yaplot       Yaplot.
                             ----
                             (Undocumented) c cif cif2 com null r rcom towhee xyz
     
     
                             2. Formatters served by external plugins
     
-                            (None)
+                            _RDF            Radial Distribution Functions.
+                            cage            Cage analysis.
+                            mdanalysis      MDAnalysis integration.
+                            meshcat         Meshcat + Google Colab.
+                            png             PNG (Portable Network Graphics).
+                            svg             SVG (Standard Vector Graphics).
+                            twist           Twist order parameter.
                             ----
     
     
                             3. Formatters served locally
     
                             (None)
                             ----
@@ -490,21 +508,24 @@
 `c`, `com`      |CenterOfMass| `.ar3a`     | Center of mass | none | none |
 `r`, `rcom`      |Relative CoM| `.ar3r`     | Center of mass | none | none | In fractional coordinate system.
 `p`, `python`, `reshape`      |Python module | `.py`     | Center of mass | none | none | Under development.
 `_ringstat`      |Ring phase statistics |     | |  | | Statistical test suite 1: Check the appearance frequencies of the ring phases as a test for the intermediate-range disorder.
 `rings`      |[Yaplot](https://github.com/vitroid/Yaplot)      | `.yap`      | center of mass | none |o | It renders HB rings.
 `_KG`      |Kirkwood G(r)|     | |  | | Statistical test suite 2: Calculate G(r) for checking long-range disorder in molecular orientations.
 
-By installing the [`genice-mdanalysis`](https://github.com/vitroid/genice-mdanalysis) package separately, you can generate files in many formats for a  large number of molecular dynamics package softwares. E.g.
+By installing the [`genice2-mdanalysis`](https://github.com/vitroid/genice-mdanalysis) package separately, you can generate files in many formats for a  large number of molecular dynamics package softwares. E.g.
 
 ```shell
-% genice2 1c -f mdanalysis[1c.pdb]
-% genice2 1h -f mdanalysis[1h.xtc]
+% pip install genice2-mdanalysis
+% genice2 1c -f 'mdanalysis[1c.pdb]'
+% genice2 1h -f 'mdanalysis[1h.xtc]'
 ```
 
+All the supported file types are listed in the [MDAnalysis web page](https://docs.mdanalysis.org/stable/documentation_pages/coordinates/init.html#supported-coordinate-formats).
+
 You can prepare your file formats. Create a folder named `formats` in the current working directory and put the plugins in it.
 
 Internally, there are seven stages to generate an ice structure.
 
 1. Cell repetition.
 2. Random graph generation and replication.
 3. Apply ice rule.
@@ -516,23 +537,23 @@
 In the format plugin, you define the hook functions that are invoked after processing each stage.
 
 ## Ice structures
 
 Symbol | <div style="width:300px">Description</div>
 -------|------------
 0, ice0 | Metastable ice "0". [Russo 2014]
-11, XI, ice11 | A candidate for an antiferroelectric Ice XI #19. [Jackson 1997,Fan 2010]
-115_2_114, 11_2_15848, 12_1_11, 12_2_29187, 12_2_32449, 144_2_7301, 14_2_48453, 151_2_4949650, 152_2_118474, 153_2_155471, 15_2_201714, 169_2_10608, 169_2_7915, 176_2_5256, 207_1_4435, 20_2_26425, 20_2_28176, 2_2_342692, 2_2_623457, 53_3_726600, 58_2_511, 61_2_8842, 67_2_1444, 67_2_1563, 84_2_1419, 91_2_8335121, ACO, CS4, DDR, IRR, IWV, LTA, MAR, NON, PCOD8007225, PCOD8036144, PCOD8045578, PCOD8047078, PCOD8047931, PCOD8172143, PCOD8204698, PCOD8301974, PCOD8321499, PCOD8324623, SGT, SOD, engel01, engel02, engel03, engel04, engel06, engel07, engel08, engel09, engel10, engel11, engel12, engel13, engel14, engel15, engel16, engel17, engel18, engel19, engel20, engel21, engel22, engel23, engel24, engel25, engel26, engel27, engel28, engel29, engel30, engel31, engel32, engel33, engel34, sVII | Hypothetical zeolitic ice [Kosyakov 1999,IZA Database,Engel 2018,Jeffrey 1984]
+11, XI, ice11 | A candidate for an antiferroelectric Ice XI #19. [Fan 2010,Jackson 1997]
+115_2_114, 11_2_15848, 12_1_11, 12_2_29187, 12_2_32449, 144_2_7301, 14_2_48453, 151_2_4949650, 152_2_118474, 153_2_155471, 15_2_201714, 169_2_10608, 169_2_7915, 176_2_5256, 207_1_4435, 20_2_26425, 20_2_28176, 2_2_342692, 2_2_623457, 53_3_726600, 58_2_511, 61_2_8842, 67_2_1444, 67_2_1563, 84_2_1419, 91_2_8335121, ACO, CS4, DDR, IRR, IWV, LTA, MAR, NON, PCOD8007225, PCOD8036144, PCOD8045578, PCOD8047078, PCOD8047931, PCOD8172143, PCOD8204698, PCOD8301974, PCOD8321499, PCOD8324623, SGT, SOD, engel01, engel02, engel03, engel04, engel06, engel07, engel08, engel09, engel10, engel11, engel12, engel13, engel14, engel15, engel16, engel17, engel18, engel19, engel20, engel21, engel22, engel23, engel24, engel25, engel26, engel27, engel28, engel29, engel30, engel31, engel32, engel33, engel34, sVII | Hypothetical zeolitic ice [Engel 2018,IZA Database,Kosyakov 1999,Jeffrey 1984]
 12, XII, ice12 | Metastable high-pressure ice XII. [Lobban 1998,Koza 2000]
 13, XIII, ice13 | Ice XIII, a hydrogen-ordered counterpart of ice V. [Salzmann 2006]
-16, CS2, MTN, XVI, ice16, sII | Ultralow-density Ice XVI. [Kosyakov 1999,Falenty 2014,IZA Database,Sikiric 2010,Jeffrey 1984]
-17, XVII, ice17 | Ultralow-density Ice XVII. [Strobel 2016,Smirnov 2013,Rosso 2016]
+16, CS2, MTN, XVI, ice16, sII | Ultralow-density Ice XVI. [IZA Database,Jeffrey 1984,Sikiric 2010,Falenty 2014,Kosyakov 1999]
+17, XVII, ice17 | Ultralow-density Ice XVII. [Smirnov 2013,Rosso 2016,Strobel 2016]
 1c, Ic, ice1c | Cubic type of ice I. [Vos 1993]
 1h, Ih, ice1h | Most popular Ice I (hexagonal)
-2, II, ice2 | Hydrogen-ordered ice II. [Kamb 2003,Kamb 1964,Londono 1988]
+2, II, ice2 | Hydrogen-ordered ice II. [Kamb 2003,Londono 1988,Kamb 1964]
 2D3 | Trilayer honeycomb ice.
 2d, ice2d, ice2rect | A hydrogen-disordered counterpart of ice II. [Nakamura 2015]
 3, III, ice3 | Ice III. [Petrenko 1999]
 4, IV, ice4 | Ice IV. [Avogadro]
 4R | Orthogonalized ice IV. [Avogadro]
 5, V, ice5 | Monoclinic ice V (testing).
 5R | Ice V with orthogonal unit cell. (testing)
@@ -540,37 +561,38 @@
 6h | Half lattice of ice VI.
 7, VII, ice7 | Conventional high-pressure ice VII.
 8, VIII, ice8 | Ice VIII, a hydrogen-ordered counterpart of ice VII. [Kuhs 1998]
 9, IX, ice9 | Ice IX, a hydrogen-ordered counterpart of ice III. [Londono 1993]
 A, iceA | Hypothetical ice A. [Baez 1998]
 A15, Struct33 | Cubic Structure I of clathrate hydrate. [Sikiric 2010]
 B, iceB | Hypothetical ice B. [Baez 1998]
-BSV, engel05 | Hypothetical zeolitic ice of the gyroid structure. [IZA Database,Engel 2018]
+BSV, engel05 | Hypothetical zeolitic ice of the gyroid structure. [Engel 2018,IZA Database]
 C14, C15, C36, FK6layers, FK9layers, HS2, Hcomp, Struct01, Struct02, Struct03, Struct04, Struct05, Struct06, Struct07, Struct08, Struct09, Struct10, Struct11, Struct12, Struct13, Struct14, Struct15, Struct16, Struct17, Struct18, Struct19, Struct20, Struct21, Struct22, Struct23, Struct24, Struct25, Struct26, Struct27, Struct28, Struct29, Struct30, Struct31, Struct32, Struct34, Struct35, Struct36, Struct37, Struct38, Struct39, Struct40, Struct41, Struct42, Struct43, Struct44, Struct45, Struct46, Struct47, Struct48, Struct49, Struct50, Struct51, Struct52, Struct53, Struct54, Struct55, Struct56, Struct57, Struct58, Struct59, Struct60, Struct61, Struct62, Struct63, Struct64, Struct65, Struct66, Struct67, Struct68, Struct69, Struct70, Struct71, Struct72, Struct73, Struct74, Struct75, Struct76, Struct77, Struct78, Struct79, Struct80, Struct81, Struct82, Struct83, Struct84, Z, delta, mu, psigma, sV, sigma, zra-d | A space fullerene. [Sikiric 2010]
 CRN1, CRN2, CRN3 | A continuous random network of Sillium. [Mousseau 2001]
-CS1, MEP, sI | Clathrate hydrates sI. [Kosyakov 1999,IZA Database,Frank 1959,Jeffrey 1984]
+CS1, MEP, sI | Clathrate hydrates sI. [Frank 1959,IZA Database,Jeffrey 1984,Kosyakov 1999]
 DOH, HS3, sH | Clathrate type H.
-EMT | Hypothetical ice with a large cavity. [Liu 2019,IZA Database]
+EMT | Hypothetical ice with a large cavity. [IZA Database,Liu 2019]
 FAU | Hypothetical ice at negative pressure ice 'sIV'. [Huang 2017,IZA Database]
 RHO | Hypothetical ice at negative pressure ice 'sIII'. [Huang 2016,IZA Database]
 T | Hypothetical clathrate type T. [Sikiric 2010,Karttunen 2011]
 c0te | Filled ice C0 by Teeratchanan (Hydrogen-disordered.) (Positions of guests are supplied.) [Teeratchanan 2015]
 c1te | Hydrogen-ordered hydrogen hydrate C1 by Teeratchanan. (Positions of guests are supplied.) [Teeratchanan 2015]
 c2te | Filled ice C2 (cubic ice) by Teeratchanan (Hydrogen disordered). (Positions of guests are supplied.) [Teeratchanan 2015]
+eleven | Ice XI w/ stacking faults.
 i | Hypothetical ice "i". [Fennell 2005]
 ice1hte | Filled ice Ih by Teeratchanan (Hydrogen disordered). (Positions of guests are supplied.) [Teeratchanan 2015]
-iceR | Hypothetical ice R. [Maynard-Casely 2010,Mochizuki 2014]
+iceR | Hypothetical ice R. [Mochizuki 2014,Maynard-Casely 2010]
 iceT | Hypothetical ice T. [Hirata 2017]
 iceT2 | Hypothetical ice T2. [Yagasaki 2018]
 one | Ice I w/ stacking faults.
 prism | Ice nanotubes. [Koga 2001]
 sTprime | Filled ice sT'. [Smirnov 2013]
 xFAU | Aeroice xFAU. [Matsui 2017]
 xdtc | A porous ice with cylindrical channels. [Matsumoto 2021]
-1h_unit, HS1, Kcomp, TS1, dtc, eleven, ice1h_unit, sIII, sIV | (Undocumented)
+1h_unit, HS1, Kcomp, TS1, dtc, ice1h_unit, sIII, sIV | (Undocumented)
 
 
 Ice names with double quotations are not experimentally verified.
 
 You can prepare your own ice structures. Create a folder named `lattices` in the current working directory and put the plugins in it.
 
 [cif2ice](https://github.com/vitroid/cif2ice) is a tool to retrieve a
@@ -646,15 +668,15 @@
 
 | pip name | GenIce2 option | Description | output format | requirements |
 |----------|-------|-------------|---------------|--------------|
 |[`genice2-cage`](https://github.com/vitroid/genice-cage)|`-f _cage`| Detect cages and quasi-polyhedra (vitrites). | text, json | `cycless` |
 |[`genice2-rdf`](https://github.com/vitroid/genice-rdf)|`-f _RDF`| Radial distribution functions. | text |  |
 |[`genice2-svg`](https://github.com/vitroid/genice-svg)|`-f svg`<br />`-f png` | 2D graphics in SVG format.<br /> ... in PNG format.| SVG<br />PNG | `svgwrite` |
 |[`genice2-twist`](https://github.com/vitroid/genice-twist)|`-f twist`| Calculate the twist order parameter (and visualize) [Matsumoto 2019]| text (@BTWC)<br />SVG<br />PNG <br />yaplot | `twist-op`, `genice2-svg` |
-
+|[`genice2-mdanalysis`](https://github.com/vitroid/genice-mdanalysis)|`-f mdanalysis`| Output the atoms in various file formats that are served by [MDAnalysis](https://github.com/MDAnalysis/mdanalysis).| text, binary | `mdanalysis` |
 ## Input plugins
 
 Input plugins (a.k.a. lattice plugins) construct a crystal structure on demand.
 
 | pip name   | GenIce2 usage    | Description  |requirements |
 |------------|-----------------|--------------|-------------|
 |[`genice2-cif`](https://github.com/vitroid/genice-cif)| `genice2 cif[ITT.cif]`<br /> `genice2 zeolite[ITT]`| Read a local CIF file as an ice structure.<br />Read a structure from Zeolite DB. | `cif2ice` |
@@ -671,20 +693,23 @@
 
 ## Faster, faster, faster.
 
 Combinations of the new algorithm and other improvements in coding, the processing time of GenIce2 is about five times faster than that of GenIce1.
 
 ## Colaboratory-ready!
 
-Now GenIce2 works on the [Google Colaboratory!](https://colab.research.google.com/github/vitroid/GenIce/blob/genice2/test.ipynb)
+Now GenIce2 works on the [Google Colaboratory!](https://colab.research.google.com/github/vitroid/GenIce/blob/genice2/jupyter.ipynb)
 
 ## New ices
 
 Many new ice structures are added.
 
+## Integration with MDAnalysis
+
+GenIce2 is now integrated with MDAnalysis.
 
 # References
 
 * [Avogadro] Avogadro https://github.com/cryos/avogadro/blob/master/crystals/ice/H2O-Ice-IV.cif
 * [Baez 1998] 
 BÁEZ, Luis A. and CLANCY, Paulette, 1995, Phase equilibria in extended simple point charge ice‐water systems. The Journal of Chemical Physics [online]. 8 December 1995. Vol. 103, no. 22, p. 9744–9755. DOI 10.1063/1.469938. Available from: http://dx.doi.org/10.1063/1.469938
```

### Comparing `GenIce2-2.1b3/genice2/CIF.py` & `GenIce2-2.1b4/genice2/CIF.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/FrankKasper.py` & `GenIce2-2.1b4/genice2/FrankKasper.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/alkyl.py` & `GenIce2-2.1b4/genice2/alkyl.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/analice.py` & `GenIce2-2.1b4/genice2/analice.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/cell.py` & `GenIce2-2.1b4/genice2/cell.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/cli/__init__.py` & `GenIce2-2.1b4/genice2/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/cli/analice.py` & `GenIce2-2.1b4/genice2/cli/analice.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/cli/genice.py` & `GenIce2-2.1b4/genice2/cli/genice.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/decorators.py` & `GenIce2-2.1b4/genice2/decorators.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/digraph.py` & `GenIce2-2.1b4/genice2/digraph.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/_KG.py` & `GenIce2-2.1b4/genice2/formats/_KG.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/_ringstat.py` & `GenIce2-2.1b4/genice2/formats/_ringstat.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/c.py` & `GenIce2-2.1b4/genice2/formats/c.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/cif.py` & `GenIce2-2.1b4/genice2/formats/cif.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/cif2.py` & `GenIce2-2.1b4/genice2/formats/cif2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/com.py` & `GenIce2-2.1b4/genice2/formats/com.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/d.py` & `GenIce2-2.1b4/genice2/formats/d.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/digraph.py` & `GenIce2-2.1b4/genice2/formats/digraph.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/e.py` & `GenIce2-2.1b4/genice2/formats/e.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/euler.py` & `GenIce2-2.1b4/genice2/formats/euler.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/exmol.py` & `GenIce2-2.1b4/genice2/formats/exmol.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/exyz.py` & `GenIce2-2.1b4/genice2/formats/exyz.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/g.py` & `GenIce2-2.1b4/genice2/formats/g.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/graph.py` & `GenIce2-2.1b4/genice2/formats/graph.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/gromacs.py` & `GenIce2-2.1b4/genice2/formats/gromacs.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/m.py` & `GenIce2-2.1b4/genice2/formats/m.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/mdv_au.py` & `GenIce2-2.1b4/genice2/formats/mdv_au.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/mdview.py` & `GenIce2-2.1b4/genice2/formats/mdview.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/o.py` & `GenIce2-2.1b4/genice2/formats/o.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/openscad.py` & `GenIce2-2.1b4/genice2/formats/openscad.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/p.py` & `GenIce2-2.1b4/genice2/formats/p.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/povray.py` & `GenIce2-2.1b4/genice2/formats/povray.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/python.py` & `GenIce2-2.1b4/genice2/formats/python.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/q.py` & `GenIce2-2.1b4/genice2/formats/q.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/quaternion.py` & `GenIce2-2.1b4/genice2/formats/quaternion.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/r.py` & `GenIce2-2.1b4/genice2/formats/r.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/raw.py` & `GenIce2-2.1b4/genice2/formats/raw.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/rcom.py` & `GenIce2-2.1b4/genice2/formats/rcom.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/reshape.py` & `GenIce2-2.1b4/genice2/formats/reshape.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/rings.py` & `GenIce2-2.1b4/genice2/formats/rings.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/towhee.py` & `GenIce2-2.1b4/genice2/formats/towhee.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/xyz.py` & `GenIce2-2.1b4/genice2/formats/xyz.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/y.py` & `GenIce2-2.1b4/genice2/formats/y.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/formats/yaplot.py` & `GenIce2-2.1b4/genice2/formats/yaplot.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/genice.py` & `GenIce2-2.1b4/genice2/genice.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/0.py` & `GenIce2-2.1b4/genice2/lattices/0.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/11.py` & `GenIce2-2.1b4/genice2/lattices/11.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/115_2_114.py` & `GenIce2-2.1b4/genice2/lattices/115_2_114.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/11_2_15848.py` & `GenIce2-2.1b4/genice2/lattices/11_2_15848.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/12.py` & `GenIce2-2.1b4/genice2/lattices/12.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/12_1_11.py` & `GenIce2-2.1b4/genice2/lattices/12_1_11.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/12_2_29187.py` & `GenIce2-2.1b4/genice2/lattices/12_2_29187.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/12_2_32449.py` & `GenIce2-2.1b4/genice2/lattices/12_2_32449.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/13.py` & `GenIce2-2.1b4/genice2/lattices/13.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/144_2_7301.py` & `GenIce2-2.1b4/genice2/lattices/144_2_7301.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/14_2_48453.py` & `GenIce2-2.1b4/genice2/lattices/14_2_48453.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/151_2_4949650.py` & `GenIce2-2.1b4/genice2/lattices/151_2_4949650.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/152_2_118474.py` & `GenIce2-2.1b4/genice2/lattices/152_2_118474.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/153_2_155471.py` & `GenIce2-2.1b4/genice2/lattices/153_2_155471.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/15_2_201714.py` & `GenIce2-2.1b4/genice2/lattices/15_2_201714.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/16.py` & `GenIce2-2.1b4/genice2/lattices/16.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/169_2_10608.py` & `GenIce2-2.1b4/genice2/lattices/169_2_10608.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/169_2_7915.py` & `GenIce2-2.1b4/genice2/lattices/169_2_7915.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/17.py` & `GenIce2-2.1b4/genice2/lattices/17.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/176_2_5256.py` & `GenIce2-2.1b4/genice2/lattices/176_2_5256.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/1c.py` & `GenIce2-2.1b4/genice2/lattices/1c.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/1h.py` & `GenIce2-2.1b4/genice2/lattices/1h.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/1h_unit.py` & `GenIce2-2.1b4/genice2/lattices/Ic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,54 @@
 # coding: utf-8
-#This is not useful for generating the graph
+"""
+Data sources
+
+"""
+
+desc={"ref": {"Ic": 'Vos 1993'},
+      "usage": "No options available.",
+      "brief": "Cubic type of ice I."
+      }
 
-import genice2.lattices
 from genice2.cell import cellvectors
+import genice2.lattices
 
 class Lattice(genice2.lattices.Lattice):
     def __init__(self):
-        self.density = 0.92     #default self.density
+        self.cell = cellvectors(a=4.0,
+                           b=4.0,
+                           c=4.0)
 
-        self.bondlen = 3        #bond threshold
-        self.cell = """
-        4.5328691711 7.84813412606925 7.37735062301457
-        """
+        self.density = 0.92     #default density
+
+        self.bondlen = 1.9      #bond threshold
 
         self.waters = """
-        0.25 0.333 0.125
-        0.75 0.833 0.125
-        0.25 0.667 0.25
-        0.75 0.167 0.25
-        0.25 0.667 0.625
-        0.75 0.167 0.625
-        0.75 0.833 0.75
-        0.25 0.333 0.75
+        0 0 0
+        0.5 0.5 0
+        0.5 0 0.5
+        0 0.5 0.5
+        0.25 0.25 0.25
+        0.75 0.75 0.25
+        0.75 0.25 0.75
+        0.25 0.75 0.75
         """
-
         self.coord = "relative"
 
-        self.cell = cellvectors(a=4.5328691711,
-                           b=7.84813412606925,
-                           c=7.37735062301457)
+        self.pairs="""
+        0 4
+        0 5
+        0 6
+        0 7
+        1 4
+        1 5
+        1 6
+        1 7
+        2 4
+        2 5
+        2 6
+        2 7
+        3 4
+        3 5
+        3 6
+        3 7
+        """
```

### Comparing `GenIce2-2.1b3/genice2/lattices/2.py` & `GenIce2-2.1b4/genice2/lattices/2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/207_1_4435.py` & `GenIce2-2.1b4/genice2/lattices/207_1_4435.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/20_2_26425.py` & `GenIce2-2.1b4/genice2/lattices/20_2_26425.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/20_2_28176.py` & `GenIce2-2.1b4/genice2/lattices/20_2_28176.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/2D3.py` & `GenIce2-2.1b4/genice2/lattices/2D3.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/2_2_342692.py` & `GenIce2-2.1b4/genice2/lattices/2_2_342692.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/2_2_623457.py` & `GenIce2-2.1b4/genice2/lattices/2_2_623457.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/2d.py` & `GenIce2-2.1b4/genice2/lattices/2d.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/3.py` & `GenIce2-2.1b4/genice2/lattices/3.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/4.py` & `GenIce2-2.1b4/genice2/lattices/4.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/4R.py` & `GenIce2-2.1b4/genice2/lattices/4R.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/5.py` & `GenIce2-2.1b4/genice2/lattices/5.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/53_3_726600.py` & `GenIce2-2.1b4/genice2/lattices/53_3_726600.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/58_2_511.py` & `GenIce2-2.1b4/genice2/lattices/58_2_511.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/5R.py` & `GenIce2-2.1b4/genice2/lattices/5R.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/6.py` & `GenIce2-2.1b4/genice2/lattices/6.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/61_2_8842.py` & `GenIce2-2.1b4/genice2/lattices/61_2_8842.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/67_2_1444.py` & `GenIce2-2.1b4/genice2/lattices/67_2_1444.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/67_2_1563.py` & `GenIce2-2.1b4/genice2/lattices/67_2_1563.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/6h.py` & `GenIce2-2.1b4/genice2/lattices/6h.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/7.py` & `GenIce2-2.1b4/genice2/lattices/7.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/8.py` & `GenIce2-2.1b4/genice2/lattices/8.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/84_2_1419.py` & `GenIce2-2.1b4/genice2/lattices/84_2_1419.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/9.py` & `GenIce2-2.1b4/genice2/lattices/9.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/91_2_8335121.py` & `GenIce2-2.1b4/genice2/lattices/91_2_8335121.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/A.py` & `GenIce2-2.1b4/genice2/lattices/A.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/A15.py` & `GenIce2-2.1b4/genice2/lattices/A15.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ACO.py` & `GenIce2-2.1b4/genice2/lattices/ACO.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/B.py` & `GenIce2-2.1b4/genice2/lattices/B.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/BSV.py` & `GenIce2-2.1b4/genice2/lattices/BSV.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/C14.py` & `GenIce2-2.1b4/genice2/lattices/C14.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/C15.py` & `GenIce2-2.1b4/genice2/lattices/C15.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/C36.py` & `GenIce2-2.1b4/genice2/lattices/C36.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/CRN1.py` & `GenIce2-2.1b4/genice2/lattices/CRN1.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/CRN2.py` & `GenIce2-2.1b4/genice2/lattices/CRN2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/CRN3.py` & `GenIce2-2.1b4/genice2/lattices/CRN3.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/CS1.py` & `GenIce2-2.1b4/genice2/lattices/CS1.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/CS2.py` & `GenIce2-2.1b4/genice2/lattices/CS2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/CS4.py` & `GenIce2-2.1b4/genice2/lattices/CS4.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/DDR.py` & `GenIce2-2.1b4/genice2/lattices/DDR.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/DOH.py` & `GenIce2-2.1b4/genice2/lattices/DOH.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/EMT.py` & `GenIce2-2.1b4/genice2/lattices/EMT.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/FAU.py` & `GenIce2-2.1b4/genice2/lattices/FAU.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/FK6layers.py` & `GenIce2-2.1b4/genice2/lattices/FK6layers.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/FK9layers.py` & `GenIce2-2.1b4/genice2/lattices/FK9layers.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/HS1.py` & `GenIce2-2.1b4/genice2/lattices/HS1.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/HS2.py` & `GenIce2-2.1b4/genice2/lattices/HS2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/HS3.py` & `GenIce2-2.1b4/genice2/lattices/HS3.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Hcomp.py` & `GenIce2-2.1b4/genice2/lattices/Hcomp.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/II.py` & `GenIce2-2.1b4/genice2/lattices/II.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/III.py` & `GenIce2-2.1b4/genice2/lattices/III.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/IRR.py` & `GenIce2-2.1b4/genice2/lattices/IRR.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/IV.py` & `GenIce2-2.1b4/genice2/lattices/IV.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/IWV.py` & `GenIce2-2.1b4/genice2/lattices/IWV.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/IX.py` & `GenIce2-2.1b4/genice2/lattices/IX.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Ic.py` & `GenIce2-2.1b4/genice2/lattices/ice1c.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Ih.py` & `GenIce2-2.1b4/genice2/lattices/Ih.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Kcomp.py` & `GenIce2-2.1b4/genice2/lattices/Kcomp.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/LTA.py` & `GenIce2-2.1b4/genice2/lattices/LTA.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/MAR.py` & `GenIce2-2.1b4/genice2/lattices/MAR.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/MEP.py` & `GenIce2-2.1b4/genice2/lattices/MEP.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/MTN.py` & `GenIce2-2.1b4/genice2/lattices/MTN.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/NON.py` & `GenIce2-2.1b4/genice2/lattices/NON.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8007225.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8007225.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8036144.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8036144.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8045578.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8045578.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8047078.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8047078.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8047931.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8047931.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8172143.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8172143.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8204698.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8204698.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8301974.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8301974.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8321499.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8321499.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/PCOD8324623.py` & `GenIce2-2.1b4/genice2/lattices/PCOD8324623.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/RHO.py` & `GenIce2-2.1b4/genice2/lattices/RHO.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/SGT.py` & `GenIce2-2.1b4/genice2/lattices/SGT.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/SOD.py` & `GenIce2-2.1b4/genice2/lattices/SOD.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct01.py` & `GenIce2-2.1b4/genice2/lattices/Struct01.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct02.py` & `GenIce2-2.1b4/genice2/lattices/Struct02.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct03.py` & `GenIce2-2.1b4/genice2/lattices/Struct03.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct04.py` & `GenIce2-2.1b4/genice2/lattices/Struct04.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct05.py` & `GenIce2-2.1b4/genice2/lattices/Struct05.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct06.py` & `GenIce2-2.1b4/genice2/lattices/Struct06.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct07.py` & `GenIce2-2.1b4/genice2/lattices/Struct07.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct08.py` & `GenIce2-2.1b4/genice2/lattices/Struct08.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct09.py` & `GenIce2-2.1b4/genice2/lattices/Struct09.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct10.py` & `GenIce2-2.1b4/genice2/lattices/Struct10.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct11.py` & `GenIce2-2.1b4/genice2/lattices/Struct11.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct12.py` & `GenIce2-2.1b4/genice2/lattices/Struct12.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct13.py` & `GenIce2-2.1b4/genice2/lattices/Struct13.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct14.py` & `GenIce2-2.1b4/genice2/lattices/Struct14.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct15.py` & `GenIce2-2.1b4/genice2/lattices/Struct15.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct16.py` & `GenIce2-2.1b4/genice2/lattices/Struct16.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct17.py` & `GenIce2-2.1b4/genice2/lattices/Struct17.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct18.py` & `GenIce2-2.1b4/genice2/lattices/Struct18.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct19.py` & `GenIce2-2.1b4/genice2/lattices/Struct19.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct20.py` & `GenIce2-2.1b4/genice2/lattices/Struct20.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct21.py` & `GenIce2-2.1b4/genice2/lattices/Struct21.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct22.py` & `GenIce2-2.1b4/genice2/lattices/Struct22.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct23.py` & `GenIce2-2.1b4/genice2/lattices/Struct23.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct24.py` & `GenIce2-2.1b4/genice2/lattices/Struct24.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct25.py` & `GenIce2-2.1b4/genice2/lattices/Struct25.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct26.py` & `GenIce2-2.1b4/genice2/lattices/Struct26.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct27.py` & `GenIce2-2.1b4/genice2/lattices/Struct27.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct28.py` & `GenIce2-2.1b4/genice2/lattices/Struct28.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct29.py` & `GenIce2-2.1b4/genice2/lattices/Struct29.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct30.py` & `GenIce2-2.1b4/genice2/lattices/Struct30.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct31.py` & `GenIce2-2.1b4/genice2/lattices/Struct31.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct32.py` & `GenIce2-2.1b4/genice2/lattices/Struct32.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct33.py` & `GenIce2-2.1b4/genice2/lattices/Struct33.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct34.py` & `GenIce2-2.1b4/genice2/lattices/Struct34.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct35.py` & `GenIce2-2.1b4/genice2/lattices/Struct35.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct36.py` & `GenIce2-2.1b4/genice2/lattices/Struct36.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct37.py` & `GenIce2-2.1b4/genice2/lattices/Struct37.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct38.py` & `GenIce2-2.1b4/genice2/lattices/Struct38.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct39.py` & `GenIce2-2.1b4/genice2/lattices/Struct39.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct40.py` & `GenIce2-2.1b4/genice2/lattices/Struct40.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct41.py` & `GenIce2-2.1b4/genice2/lattices/Struct41.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct42.py` & `GenIce2-2.1b4/genice2/lattices/Struct42.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct43.py` & `GenIce2-2.1b4/genice2/lattices/Struct43.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct44.py` & `GenIce2-2.1b4/genice2/lattices/Struct44.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct45.py` & `GenIce2-2.1b4/genice2/lattices/Struct45.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct46.py` & `GenIce2-2.1b4/genice2/lattices/Struct46.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct47.py` & `GenIce2-2.1b4/genice2/lattices/Struct47.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct48.py` & `GenIce2-2.1b4/genice2/lattices/Struct48.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct49.py` & `GenIce2-2.1b4/genice2/lattices/Struct49.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct50.py` & `GenIce2-2.1b4/genice2/lattices/Struct50.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct51.py` & `GenIce2-2.1b4/genice2/lattices/Struct51.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct52.py` & `GenIce2-2.1b4/genice2/lattices/Struct52.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct53.py` & `GenIce2-2.1b4/genice2/lattices/Struct53.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct54.py` & `GenIce2-2.1b4/genice2/lattices/Struct54.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct55.py` & `GenIce2-2.1b4/genice2/lattices/Struct55.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct56.py` & `GenIce2-2.1b4/genice2/lattices/Struct56.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct57.py` & `GenIce2-2.1b4/genice2/lattices/Struct57.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct58.py` & `GenIce2-2.1b4/genice2/lattices/Struct58.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct59.py` & `GenIce2-2.1b4/genice2/lattices/Struct59.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct60.py` & `GenIce2-2.1b4/genice2/lattices/Struct60.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct61.py` & `GenIce2-2.1b4/genice2/lattices/Struct61.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct62.py` & `GenIce2-2.1b4/genice2/lattices/Struct62.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct63.py` & `GenIce2-2.1b4/genice2/lattices/Struct63.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct64.py` & `GenIce2-2.1b4/genice2/lattices/Struct64.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct65.py` & `GenIce2-2.1b4/genice2/lattices/Struct65.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct66.py` & `GenIce2-2.1b4/genice2/lattices/Struct66.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct67.py` & `GenIce2-2.1b4/genice2/lattices/Struct67.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct68.py` & `GenIce2-2.1b4/genice2/lattices/Struct68.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct69.py` & `GenIce2-2.1b4/genice2/lattices/Struct69.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct70.py` & `GenIce2-2.1b4/genice2/lattices/Struct70.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct71.py` & `GenIce2-2.1b4/genice2/lattices/Struct71.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct72.py` & `GenIce2-2.1b4/genice2/lattices/Struct72.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct73.py` & `GenIce2-2.1b4/genice2/lattices/Struct73.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct74.py` & `GenIce2-2.1b4/genice2/lattices/Struct74.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct75.py` & `GenIce2-2.1b4/genice2/lattices/Struct75.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct76.py` & `GenIce2-2.1b4/genice2/lattices/Struct76.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct77.py` & `GenIce2-2.1b4/genice2/lattices/Struct77.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct78.py` & `GenIce2-2.1b4/genice2/lattices/Struct78.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct79.py` & `GenIce2-2.1b4/genice2/lattices/Struct79.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct80.py` & `GenIce2-2.1b4/genice2/lattices/Struct80.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct81.py` & `GenIce2-2.1b4/genice2/lattices/Struct81.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct82.py` & `GenIce2-2.1b4/genice2/lattices/Struct82.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct83.py` & `GenIce2-2.1b4/genice2/lattices/Struct83.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Struct84.py` & `GenIce2-2.1b4/genice2/lattices/Struct84.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/T.py` & `GenIce2-2.1b4/genice2/lattices/T.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/TS1.py` & `GenIce2-2.1b4/genice2/lattices/TS1.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/V.py` & `GenIce2-2.1b4/genice2/lattices/V.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/VI.py` & `GenIce2-2.1b4/genice2/lattices/VI.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/VII.py` & `GenIce2-2.1b4/genice2/lattices/VII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/VIII.py` & `GenIce2-2.1b4/genice2/lattices/VIII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/XI.py` & `GenIce2-2.1b4/genice2/lattices/XI.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/XII.py` & `GenIce2-2.1b4/genice2/lattices/XII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/XIII.py` & `GenIce2-2.1b4/genice2/lattices/XIII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/XVI.py` & `GenIce2-2.1b4/genice2/lattices/XVI.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/XVII.py` & `GenIce2-2.1b4/genice2/lattices/XVII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/Z.py` & `GenIce2-2.1b4/genice2/lattices/Z.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/__ice14.py` & `GenIce2-2.1b4/genice2/lattices/__ice14.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/__test1.py` & `GenIce2-2.1b4/genice2/lattices/__test1.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/__test2.py` & `GenIce2-2.1b4/genice2/lattices/__test2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/__test3.py` & `GenIce2-2.1b4/genice2/lattices/__test3.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/__test4.py` & `GenIce2-2.1b4/genice2/lattices/__test4.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/c0te.py` & `GenIce2-2.1b4/genice2/lattices/c0te.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/c1te.py` & `GenIce2-2.1b4/genice2/lattices/c1te.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/c2te.py` & `GenIce2-2.1b4/genice2/lattices/c2te.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/delta.py` & `GenIce2-2.1b4/genice2/lattices/delta.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/dtc.py` & `GenIce2-2.1b4/genice2/lattices/dtc.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/eleven.py` & `GenIce2-2.1b4/genice2/lattices/eleven.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel01.py` & `GenIce2-2.1b4/genice2/lattices/engel01.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel02.py` & `GenIce2-2.1b4/genice2/lattices/engel02.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel03.py` & `GenIce2-2.1b4/genice2/lattices/engel03.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel04.py` & `GenIce2-2.1b4/genice2/lattices/engel04.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel05.py` & `GenIce2-2.1b4/genice2/lattices/engel05.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel06.py` & `GenIce2-2.1b4/genice2/lattices/engel06.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel07.py` & `GenIce2-2.1b4/genice2/lattices/engel07.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel08.py` & `GenIce2-2.1b4/genice2/lattices/engel08.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel09.py` & `GenIce2-2.1b4/genice2/lattices/engel09.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel10.py` & `GenIce2-2.1b4/genice2/lattices/engel10.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel11.py` & `GenIce2-2.1b4/genice2/lattices/engel11.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel12.py` & `GenIce2-2.1b4/genice2/lattices/engel12.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel13.py` & `GenIce2-2.1b4/genice2/lattices/engel13.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel14.py` & `GenIce2-2.1b4/genice2/lattices/engel14.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel15.py` & `GenIce2-2.1b4/genice2/lattices/engel15.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel16.py` & `GenIce2-2.1b4/genice2/lattices/engel16.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel17.py` & `GenIce2-2.1b4/genice2/lattices/engel17.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel18.py` & `GenIce2-2.1b4/genice2/lattices/engel18.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel19.py` & `GenIce2-2.1b4/genice2/lattices/engel19.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel20.py` & `GenIce2-2.1b4/genice2/lattices/engel20.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel21.py` & `GenIce2-2.1b4/genice2/lattices/engel21.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel22.py` & `GenIce2-2.1b4/genice2/lattices/engel22.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel23.py` & `GenIce2-2.1b4/genice2/lattices/engel23.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel24.py` & `GenIce2-2.1b4/genice2/lattices/engel24.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel25.py` & `GenIce2-2.1b4/genice2/lattices/engel25.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel26.py` & `GenIce2-2.1b4/genice2/lattices/engel26.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel27.py` & `GenIce2-2.1b4/genice2/lattices/engel27.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel28.py` & `GenIce2-2.1b4/genice2/lattices/engel28.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel29.py` & `GenIce2-2.1b4/genice2/lattices/engel29.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel30.py` & `GenIce2-2.1b4/genice2/lattices/engel30.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel31.py` & `GenIce2-2.1b4/genice2/lattices/engel31.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel32.py` & `GenIce2-2.1b4/genice2/lattices/engel32.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel33.py` & `GenIce2-2.1b4/genice2/lattices/engel33.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/engel34.py` & `GenIce2-2.1b4/genice2/lattices/engel34.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/i.py` & `GenIce2-2.1b4/genice2/lattices/i.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice0.py` & `GenIce2-2.1b4/genice2/lattices/ice0.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice11.py` & `GenIce2-2.1b4/genice2/lattices/ice11.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice12.py` & `GenIce2-2.1b4/genice2/lattices/ice12.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice13.py` & `GenIce2-2.1b4/genice2/lattices/ice13.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice16.py` & `GenIce2-2.1b4/genice2/lattices/ice16.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice17.py` & `GenIce2-2.1b4/genice2/lattices/ice17.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice1h.py` & `GenIce2-2.1b4/genice2/lattices/ice1h.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice1hte.py` & `GenIce2-2.1b4/genice2/lattices/ice1hte.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice2.py` & `GenIce2-2.1b4/genice2/lattices/ice2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice2d.py` & `GenIce2-2.1b4/genice2/lattices/ice2d.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice2rect.py` & `GenIce2-2.1b4/genice2/lattices/ice2rect.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice3.py` & `GenIce2-2.1b4/genice2/lattices/ice3.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice4.py` & `GenIce2-2.1b4/genice2/lattices/ice4.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice5.py` & `GenIce2-2.1b4/genice2/lattices/ice5.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice6.py` & `GenIce2-2.1b4/genice2/lattices/ice6.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice7.py` & `GenIce2-2.1b4/genice2/lattices/ice7.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice8.py` & `GenIce2-2.1b4/genice2/lattices/ice8.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/ice9.py` & `GenIce2-2.1b4/genice2/lattices/ice9.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/iceA.py` & `GenIce2-2.1b4/genice2/lattices/iceA.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/iceB.py` & `GenIce2-2.1b4/genice2/lattices/iceB.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/iceR.py` & `GenIce2-2.1b4/genice2/lattices/iceR.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/iceT.py` & `GenIce2-2.1b4/genice2/lattices/iceT.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/iceT2.py` & `GenIce2-2.1b4/genice2/lattices/iceT2.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/mu.py` & `GenIce2-2.1b4/genice2/lattices/mu.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/one.py` & `GenIce2-2.1b4/genice2/lattices/one.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/prism.py` & `GenIce2-2.1b4/genice2/lattices/prism.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/psigma.py` & `GenIce2-2.1b4/genice2/lattices/psigma.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sH.py` & `GenIce2-2.1b4/genice2/lattices/sH.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sI.py` & `GenIce2-2.1b4/genice2/lattices/sI.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sII.py` & `GenIce2-2.1b4/genice2/lattices/sII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sIII.py` & `GenIce2-2.1b4/genice2/lattices/sIII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sIV.py` & `GenIce2-2.1b4/genice2/lattices/sIV.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sTprime.py` & `GenIce2-2.1b4/genice2/lattices/sTprime.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sV.py` & `GenIce2-2.1b4/genice2/lattices/sV.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sVII.py` & `GenIce2-2.1b4/genice2/lattices/sVII.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/sigma.py` & `GenIce2-2.1b4/genice2/lattices/sigma.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/xFAU.py` & `GenIce2-2.1b4/genice2/lattices/xFAU.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/xdtc.py` & `GenIce2-2.1b4/genice2/lattices/xdtc.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/lattices/zra-d.py` & `GenIce2-2.1b4/genice2/lattices/zra-d.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/load.py` & `GenIce2-2.1b4/genice2/load.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/loaders/ar3r.py` & `GenIce2-2.1b4/genice2/loaders/ar3r.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/loaders/exyz.py` & `GenIce2-2.1b4/genice2/loaders/exyz.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/loaders/gro.py` & `GenIce2-2.1b4/genice2/loaders/gro.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/loaders/mdv.py` & `GenIce2-2.1b4/genice2/loaders/mdv.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/loaders/mdva.py` & `GenIce2-2.1b4/genice2/loaders/mdva.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/loaders/nx3a.py` & `GenIce2-2.1b4/genice2/loaders/nx3a.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/3site.py` & `GenIce2-2.1b4/genice2/molecules/3site.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/4site.py` & `GenIce2-2.1b4/genice2/molecules/4site.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/5site.py` & `GenIce2-2.1b4/genice2/molecules/5site.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/6site.py` & `GenIce2-2.1b4/genice2/molecules/6site.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/7site.py` & `GenIce2-2.1b4/genice2/molecules/7site.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/NvdE.py` & `GenIce2-2.1b4/genice2/molecules/NvdE.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/__init__.py` & `GenIce2-2.1b4/genice2/molecules/__init__.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/ch4.py` & `GenIce2-2.1b4/genice2/molecules/ch4.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/ice.py` & `GenIce2-2.1b4/genice2/molecules/ice.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/mol.py` & `GenIce2-2.1b4/genice2/molecules/mol.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/physical_water.py` & `GenIce2-2.1b4/genice2/molecules/physical_water.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/spce.py` & `GenIce2-2.1b4/genice2/molecules/spce.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/thf.py` & `GenIce2-2.1b4/genice2/molecules/thf.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/tip3p.py` & `GenIce2-2.1b4/genice2/molecules/tip3p.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/tip4p.py` & `GenIce2-2.1b4/genice2/molecules/tip4p.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/tip5p.py` & `GenIce2-2.1b4/genice2/molecules/tip5p.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/uathf.py` & `GenIce2-2.1b4/genice2/molecules/uathf.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/molecules/uathf6.py` & `GenIce2-2.1b4/genice2/molecules/uathf6.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/plugin.py` & `GenIce2-2.1b4/genice2/plugin.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/rigid.py` & `GenIce2-2.1b4/genice2/rigid.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/genice2/valueparser.py` & `GenIce2-2.1b4/genice2/valueparser.py`

 * *Files identical despite different names*

### Comparing `GenIce2-2.1b3/setup.py` & `GenIce2-2.1b4/setup.py`

 * *Files identical despite different names*

