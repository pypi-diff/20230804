# Comparing `tmp/astro-p3-1.1.tar.gz` & `tmp/astro-p3-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-p3-1.1.tar", last modified: Fri Jul  7 08:35:26 2023, max compression
+gzip compressed data, was "astro-p3-1.2.tar", last modified: Fri Aug  4 09:54:06 2023, max compression
```

## Comparing `astro-p3-1.1.tar` & `astro-p3-1.2.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.003033 astro-p3-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.015034 astro-p3-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 08:35:09.000000 astro-p3-1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-07 08:35:09.000000 astro-p3-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-07 08:35:09.000000 astro-p3-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 08:35:09.000000 astro-p3-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 08:35:26.103036 astro-p3-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 08:35:09.000000 astro-p3-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.015034 astro-p3-1.1/astro_p3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 08:35:25.000000 astro-p3-1.1/astro_p3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.015034 astro-p3-1.1/p3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 08:35:25.000000 astro-p3-1.1/p3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.023034 astro-p3-1.1/p3/aoSystem/
--rw-r--r--   0 runner    (1001) docker     (123)    38763 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/FourierUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.023034 astro-p3-1.1/p3/aoSystem/_txtFile/
--rw-r--r--   0 runner    (1001) docker     (123)    39085 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/_txtFile/ELT_segmentVertices.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/_txtFile/Keck_segmentVertices.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/anisoplanatismModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/aoSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-07 08:35:09.000000 astro-p3-1.1/p3/aoSystem/createSegmentedModes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.011034 astro-p3-1.1/p3/aoSystem/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.031034 astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/
--rw-r--r--   0 runner    (1001) docker     (123)  4331520 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits
--rw-r--r--   0 runner    (1001) docker     (123)   938880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.031034 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.031034 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidActuatorMap.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidSubapMap.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.071035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/
--rw-r--r--   0 runner    (1001) docker     (123) 11522880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits
--rw-r--r--   0 runner    (1001) docker     (123)  2882880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits
--rw-r--r--   0 runner    (1001) docker     (123) 11522880 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits
--rw-r--r--   0 runner    (1001) docker     (123) 11845440 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits
--rw-r--r--   0 runner    (1001) docker     (123)   325440 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.007034 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.071035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat
--rw-r--r--   0 runner    (1001) docker     (123)    26149 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat
--rw-r--r--   0 runner    (1001) docker     (123)    25122 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat
--rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.075035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat
--rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat
--rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.079035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/
--rw-r--r--   0 runner    (1001) docker     (123)    45636 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat
--rw-r--r--   0 runner    (1001) docker     (123)    31637 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat
--rw-r--r--   0 runner    (1001) docker     (123)    51146 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat
--rw-r--r--   0 runner    (1001) docker     (123)    42642 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat
--rw-r--r--   0 runner    (1001) docker     (123)    45125 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat
--rw-r--r--   0 runner    (1001) docker     (123)    60065 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat
--rw-r--r--   0 runner    (1001) docker     (123)    54054 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat
--rw-r--r--   0 runner    (1001) docker     (123)    60374 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat
--rw-r--r--   0 runner    (1001) docker     (123)    58102 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat
--rw-r--r--   0 runner    (1001) docker     (123)    61576 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat
--rw-r--r--   0 runner    (1001) docker     (123)    41888 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat
--rw-r--r--   0 runner    (1001) docker     (123)  2079744 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls
--rw-r--r--   0 runner    (1001) docker     (123)   128912 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.079035 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/
--rw-r--r--   0 runner    (1001) docker     (123)    77760 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits
--rw-r--r--   0 runner    (1001) docker     (123)   463680 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits
--rw-r--r--   0 runner    (1001) docker     (123)   463680 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.083036 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits
--rw-r--r--   0 runner    (1001) docker     (123)  1330560 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.011034 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.087036 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/
--rw-r--r--   0 runner    (1001) docker     (123)   152640 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits
--rw-r--r--   0 runner    (1001) docker     (123)   593280 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits
--rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits
--rw-r--r--   0 runner    (1001) docker     (123)   429120 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits
--rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits
--rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits
--rw-r--r--   0 runner    (1001) docker     (123)   429120 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits
--rw-r--r--   0 runner    (1001) docker     (123)    60480 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits
--rw-r--r--   0 runner    (1001) docker     (123)  2102400 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.091036 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/
--rw-r--r--   0 runner    (1001) docker     (123)  9835200 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits
--rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/defineAoSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/deformableMirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    56675 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/fourierModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/frequencyDomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/optics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.099036 astro-p3-1.1/p3/aoSystem/parFiles/
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/HarmoniLTAO.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/HarmoniSCAO.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/MavisMCAO.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/MosaicGLAO.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/eris.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/irdis.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/nirc2.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/nirc2_monochromatic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/parFiles/template.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/pupil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/spiders.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.099036 astro-p3-1.1/p3/aoSystem/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/testing/tests_aoSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/testing/tests_tiptop_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/aoSystem/zernike.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/deepLoop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/dataBaseVerification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/dataGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/dataGeneratorBatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/deepLoopPerformance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/deepLoopPerformanceBatch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/jobGenerate.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/jobPerformance.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/deepLoop/recover_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/psfFitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/confidenceInterval.py
--rw-r--r--   0 runner    (1001) docker     (123)    30451 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/fittingUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/imageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfFitting/psfFitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/psfao21/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfao21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfao21/psfao21.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/psfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfr/psfR.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/psfr/psfrUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/configFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/keckUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/massdimm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/sphereUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/systemDiagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/telemetryKASP.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/telemetry/telemetryKeck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:26.103036 astro-p3-1.1/p3/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-07 08:35:10.000000 astro-p3-1.1/p3/testing/tests_p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-07 08:35:10.000000 astro-p3-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:35:26.103036 astro-p3-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.460271 astro-p3-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.356270 astro-p3-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.364270 astro-p3-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-04 09:53:40.000000 astro-p3-1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-04 09:53:40.000000 astro-p3-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-04 09:53:40.000000 astro-p3-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 09:53:40.000000 astro-p3-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-04 09:54:06.460271 astro-p3-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-04 09:53:40.000000 astro-p3-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.364270 astro-p3-1.2/astro_p3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-04 09:54:05.000000 astro-p3-1.2/astro_p3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-08-04 09:54:06.000000 astro-p3-1.2/astro_p3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:54:05.000000 astro-p3-1.2/astro_p3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:54:05.000000 astro-p3-1.2/astro_p3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 09:54:05.000000 astro-p3-1.2/astro_p3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.364270 astro-p3-1.2/p3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-04 09:54:05.000000 astro-p3-1.2/p3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.368270 astro-p3-1.2/p3/aoSystem/
+-rw-r--r--   0 runner    (1001) docker     (123)    39641 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/FourierUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.368270 astro-p3-1.2/p3/aoSystem/_txtFile/
+-rw-r--r--   0 runner    (1001) docker     (123)    39085 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/_txtFile/ELT_segmentVertices.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/_txtFile/Keck_segmentVertices.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/anisoplanatismModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37375 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/aoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/createSegmentedModes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.360270 astro-p3-1.2/p3/aoSystem/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.372270 astro-p3-1.2/p3/aoSystem/data/ELT_CALIBRATION/
+-rw-r--r--   0 runner    (1001) docker     (123)  4331520 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   938880 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.376270 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.376270 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidActuatorMap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidSubapMap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.420271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/
+-rw-r--r--   0 runner    (1001) docker     (123) 11522880 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  2882880 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 11522880 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 11845440 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   325440 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.360270 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.420271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.420271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    26149 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.420271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    25122 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.424271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.424271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.428271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/
+-rw-r--r--   0 runner    (1001) docker     (123)    45636 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    31637 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    51146 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    42642 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    45125 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    60065 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    54054 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    60374 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    58102 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    61576 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    41888 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat
+-rw-r--r--   0 runner    (1001) docker     (123)  2079744 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls
+-rw-r--r--   0 runner    (1001) docker     (123)   128912 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.428271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/
+-rw-r--r--   0 runner    (1001) docker     (123)    77760 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   463680 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   463680 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.432271 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  1330560 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.360270 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.436271 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/
+-rw-r--r--   0 runner    (1001) docker     (123)   152640 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   593280 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   429120 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   429120 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    60480 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  2102400 2023-08-04 09:53:40.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.440271 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/
+-rw-r--r--   0 runner    (1001) docker     (123)  9835200 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/defineAoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/deformableMirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56927 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/fourierModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/frequencyDomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/optics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.452271 astro-p3-1.2/p3/aoSystem/parFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/HarmoniLTAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/HarmoniSCAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/MavisMCAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/MosaicGLAO.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/eris.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/irdis.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/nirc2.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/nirc2_monochromatic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/parFiles/template.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/pupil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/spiders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.452271 astro-p3-1.2/p3/aoSystem/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/testing/tests_aoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/testing/tests_tiptop_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/aoSystem/zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.456271 astro-p3-1.2/p3/deepLoop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/dataBaseVerification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/dataGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/dataGeneratorBatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/deepLoopPerformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/deepLoopPerformanceBatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/jobGenerate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/jobPerformance.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/deepLoop/recover_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.456271 astro-p3-1.2/p3/psfFitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfFitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfFitting/confidenceInterval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30451 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfFitting/fittingUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfFitting/imageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfFitting/psfFitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.456271 astro-p3-1.2/p3/psfao21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfao21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfao21/psfao21.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.456271 astro-p3-1.2/p3/psfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfr/psfR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/psfr/psfrUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.456271 astro-p3-1.2/p3/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/configFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/keckUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/massdimm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/sphereUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/systemDiagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/telemetryKASP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/telemetry/telemetryKeck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:54:06.456271 astro-p3-1.2/p3/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-08-04 09:53:41.000000 astro-p3-1.2/p3/testing/tests_p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-04 09:53:41.000000 astro-p3-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:54:06.460271 astro-p3-1.2/setup.cfg
```

### Comparing `astro-p3-1.1/.github/workflows/publish.yml` & `astro-p3-1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/LICENSE` & `astro-p3-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/astro_p3.egg-info/SOURCES.txt` & `astro-p3-1.2/astro_p3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/FourierUtils.py` & `astro-p3-1.2/p3/aoSystem/FourierUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jun 17 01:17:43 2020
 
 @author: omartin
 """
+
 # Libraries
-import numpy as np
-import numpy.fft as fft
+import numpy as nnp
+from . import gpuEnabled
+
+if not gpuEnabled:
+    np = nnp
+    import scipy.interpolate as interp        
+    import scipy.ndimage as scnd
+    import scipy.special as ssp
+    import numpy.fft as fft
+else:
+    import cupy as cp
+    import scipy.interpolate as interp        
+#    import cupyx.scipy.interpolate as interp        
+    import cupyx.scipy.ndimage as scnd
+    import cupyx.scipy.special as ssp
+    import cupy.fft as fft
+    np = cp
+
 import matplotlib.pyplot as plt
 from astropy.modeling import models, fitting
 import matplotlib as mpl
-import scipy.interpolate as interp        
-import scipy.ndimage as scnd
-import scipy.special as ssp
+
 from matplotlib.path import Path
 
 #%%  FOURIER TOOLS
 
 def cov2sf(cov):
     return 2*cov.max() - cov - np.conjugate(cov)
 
@@ -28,15 +43,15 @@
     elif len(nPts) == 2:
         out =  fft.ifft2(fft.fft2(x)*np.conj(fft.fft2(y)))/(nPts[0]*nPts[1])
     return out
 
 def fftsym(x):
     if x.ndim ==2:
         nx,ny            = x.shape
-        if np.any(np.iscomplex(x)):
+        if np.iscomplex(x):
             out              = np.zeros((nx,ny)) + complex(0,1)*np.zeros((nx,ny))
             out[0,0]         = x[0,0]
             out[0,1:ny-1]     = x[1,np.arange(ny-1,1,-1)]
             out[1:nx-1,0]     = x[np.arange(nx-1,1,-1),1]
             out[1:nx-1,1:ny-1] = x[np.arange(nx-1,1,-1),np.arange(ny-1,1,-1)]
         else:
             out              = np.zeros((nx,ny))
@@ -45,57 +60,58 @@
             out[1:nx-1,0]     = x[np.arange(nx-1,1,-1),1]
             out[1:nx-1,1:ny-1] = x[np.arange(nx-1,1,-1),np.arange(ny-1,1,-1)]
             
         return out
     elif x.ndim ==1:
         return fft.fftshift(x)
 
-def freq_array(nX,L=1,offset=1e-10):
+def freq_array(nX, L=1, offset=1e-10):
     k2D = np.mgrid[0:nX, 0:nX].astype(float)
     k2D[0] -= nX//2
     k2D[1] -= nX//2
-    k2D     = k2D*L + offset
+    k2D     *= np.asarray(L)
+    k2D     += offset
     return k2D[0],k2D[1]
 
 def getStaticOTF(tel,nOtf,samp,wvl,xStat=[],theta_ext=0,spatialFilter=1):
         
         # DEFINING THE RESOLUTION/PUPIL
         nPup = tel.pupil.shape[0]
         
         # ADDING STATIC MAP
         phaseStat = np.zeros((nPup,nPup))
-        if np.any(tel.opdMap_on):
+        if not tel.opdMap_on is None and np.any(tel.opdMap_on):
             if theta_ext:
                 tel.opdMap_on = scnd.rotate(tel.opdMap_on,theta_ext,reshape=False)
             phaseStat = (2*np.pi*1e-9/wvl) * tel.opdMap_on
             
         # ADDING USER-SPECIFIED STATIC MODES
         xStat = np.asarray(xStat)
         phaseMap = 0
-        if np.any(tel.statModes):
+        if not tel.statModes is None and np.any(tel.statModes):
             if tel.statModes.shape[2]==len(xStat):
                 phaseMap = 2*np.pi*1e-9/wvl * np.sum(tel.statModes*xStat,axis=2)
                 phaseStat += phaseMap
                 
         # FILTERING
         if not np.isscalar(spatialFilter):
             phaseStat = (np.dot(spatialFilter,phaseStat.reshape(-1))).reshape((nPup,nPup))
         
         # INSTRUMENTAL OTF
         otfStat = pupil2otf(tel.pupil * tel.apodizer,phaseStat,samp)
-        if np.any(otfStat.shape !=nOtf):
+        if not otfStat is None and otfStat.shape!=nOtf:
             otfStat = interpolateSupport(otfStat,nOtf)
         otfStat/= otfStat.max()
         
         # DIFFRACTION-LIMITED OTF
         if np.all(phaseStat == 0):
             otfDL = otfStat
         else:
             otfDL = np.real(pupil2otf(tel.pupil * tel.apodizer,0*phaseStat,samp))
-            if np.any(otfDL.shape !=nOtf):
+            if otfDL.shape !=nOtf:
                 otfDL = interpolateSupport(otfDL,nOtf)
                 otfDL/= otfDL.max()
                 
         return otfStat, otfDL, phaseMap
 
 def instantiateAngularFrequencies(nOtf,fact=2):
     # DEFINING THE DOMAIN ANGULAR FREQUENCIES
@@ -144,22 +160,22 @@
         # Zero-pad the OTF to set the PSF pixel scale
         otf    = enlargeSupport(otf,nqSmpl)
         # Interpolate the OTF to set the PSF FOV
         otf    = interpolateSupport(otf,fovInPixel)
         psf    = otf2psf(otf)
     else:
         # Interpolate the OTF at high resolution to set the PSF FOV
-        otf    = interpolateSupport(otf,int(np.round(fovInPixel/nqSmpl)))
+        otf    = interpolateSupport(otf,int(nnp.round(fovInPixel/nqSmpl)))
         psf    = otf2psf(otf)
         # Interpolate the PSF to set the PSF pixel scale
         psf    = interpolateSupport(psf,fovInPixel)
     return psf
                         
 def pistonFilter(D,f,fm=0,fn=0):    
-    f[np.where(f==0)] = 1e-10 
+    f[np.where(np.equal(f,0))] = 1e-10 
     if len(f.shape) ==1:
         Fx,Fy = np.meshgrid(f,f)            
         FX    = Fx -fm 
         FY    = Fy -fn    
         F     = np.pi*D*np.hypot(FX,FY)    
     else:
         F     = np.pi*D*f
@@ -291,15 +307,15 @@
         else:
             fftPhasor = np.ones((freq.nOtf,freq.nOtf,ao.src.nSrc,freq.nWvl),dtype=complex)
 
         # LOOP ON WAVELENGTHS   
         for jWvl in range(freq.nWvl):
             
             # UPDATE THE INSTRUMENTAL OTF
-            if (np.any(ao.tel.opdMap_on != None) and freq.nWvl>1) or len(xStat)>0:
+            if (not ao.tel.opdMap_on is None and freq.nWvl>1) or len(xStat)>0:
                 freq.otfNCPA, freq.otfDL, freq.phaseMap = \
                 getStaticOTF(ao.tel,int(freq.nOtf),freq.samp[jWvl],freq.wvl[jWvl],
                              xStat=xStat,theta_ext=theta_ext,spatialFilter=spatialFilter)
                 
             # UPDATE THE RESIDUAL JITTER
             if freq.nyquistSampling == True and freq.nWvl > 1 and (jitterX!=0 or jitterY!=0):
                 normFact2    = ff_jitter*(freq.samp[jWvl]*ao.tel.D/freq.wvl[jWvl]/(3600*180*1e3/np.pi))**2  * (2 * np.sqrt(2*np.log(2)))**2
@@ -420,15 +436,15 @@
         p = Path([(xv[i], yv[i]) for i in range(xv.shape[0])])
         return p.contains_points(q).reshape(shape)
     
 def interpolateSupport(image,nRes,kind='spline'):
     
     nx,ny = image.shape
     # Define angular frequencies vectors
-    if np.isscalar(nRes):
+    if nnp.isscalar(nRes):
         mx = my = nRes
     else:        
         mx = nRes[0]
         my = nRes[1]
                    
             
     if kind == 'nearest':
@@ -438,49 +454,61 @@
             return tmpReal + complex(0,1)*tmpImag
         else:
             return tmpReal
     else:        
         
         # Initial frequencies grid    
         if nx%2 == 0:
-            uinit = np.linspace(-nx/2,nx/2-1,nx)*2/nx
+            uinit = nnp.linspace(-nx/2,nx/2-1,nx)*2/nx
         else:
-            uinit = np.linspace(-np.floor(nx/2),np.floor(nx/2),nx)*2/nx
+            uinit = nnp.linspace(-np.floor(nx/2),np.floor(nx/2),nx)*2/nx
         if ny%2 == 0:
-            vinit = np.linspace(-ny/2,ny/2-1,ny)*2/ny
+            vinit = nnp.linspace(-ny/2,ny/2-1,ny)*2/ny
         else:
-            vinit = np.linspace(-np.floor(ny/2),np.floor(ny/2),ny)*2/ny    
+            vinit = nnp.linspace(-np.floor(ny/2),np.floor(ny/2),ny)*2/ny    
              
         # Interpolated frequencies grid                  
         if mx%2 == 0:
-            unew = np.linspace(-mx/2,mx/2-1,mx)*2/mx
+            unew = nnp.linspace(-mx/2,mx/2-1,mx)*2/mx
         else:
-            unew = np.linspace(-np.floor(mx/2),np.floor(mx/2),mx)*2/mx
+            unew = nnp.linspace(-np.floor(mx/2),np.floor(mx/2),mx)*2/mx
         if my%2 == 0:
-            vnew = np.linspace(-my/2,my/2-1,my)*2/my
+            vnew = nnp.linspace(-my/2,my/2-1,my)*2/my
         else:
-            vnew = np.linspace(-np.floor(my/2),np.floor(my/2),my)*2/my
+            vnew = nnp.linspace(-np.floor(my/2),np.floor(my/2),my)*2/my
                    
         # Interpolation
     
         if kind == 'spline':
             # Surprinsingly v and u vectors must be shifted when using
             # RectBivariateSpline. See:https://github.com/scipy/scipy/issues/3164
-            fun_real = interp.fitpack2.RectBivariateSpline(vinit, uinit, np.real(image))
+            xin = np.real(image)
+            if gpuEnabled:
+                xin = xin.get()
+            fun_real = interp.fitpack2.RectBivariateSpline(vinit, uinit, xin)
             if np.any(np.iscomplex(image)):
-                fun_imag = interp.fitpack2.RectBivariateSpline(vinit, uinit, np.imag(image))
+                xin = np.imag(image)
+                if gpuEnabled:
+                    xin = xin.get()
+                fun_imag = interp.fitpack2.RectBivariateSpline(vinit, uinit, xin)
         else:
-            fun_real = interp.interp2d(uinit, vinit, np.real(image),kind=kind)
+            xin = np.real(image)
+            if gpuEnabled:
+                xin = xin.get()
+            fun_real = interp.interp2d(uinit, vinit, xin,kind=kind)
             if np.any(np.iscomplex(image)):
-                fun_imag = interp.interp2d(uinit, vinit, np.imag(image),kind=kind)
+                xin = np.imag(image)
+                if gpuEnabled:
+                    xin = xin.get()
+                fun_imag = interp.interp2d(uinit, vinit, xin,kind=kind)
     
         if np.any(np.iscomplex(image)):
-            return fun_real(unew,vnew) + complex(0,1)*fun_imag(unew,vnew)
+            return np.asarray(fun_real(unew,vnew) + complex(0,1)*fun_imag(unew,vnew))
         else:
-            return fun_real(unew,vnew)
+            return np.asarray(fun_real(unew,vnew))
             
 
 def normalizeImage(im,normType=1,param=None):
     ''' Returns the normalized PSF :
         normtype = 0 : no normalization
         normType = 1 : Normalization by the sum of pixels
         normtype = 2 : min-max normalization
@@ -767,87 +795,87 @@
     --------
     results : tuple
         Tuple containing (radius, profile) or (radius, profile, EE) depending on what is requested.
         The radius gives the center radius of each bin, while the EE is given inside the whole bin
         so you should use (radius+binsize/2) for the radius of the EE curve if you want to be
         as precise as possible.
     """
-    
+        
     if normalize.lower() == 'peak':
         print("Calculating profile with PSF normalized to peak = 1")
         image /= image.max()
     elif normalize.lower() == 'total':
         print("Calculating profile with PSF normalized to total = 1")
         image /= image.sum()
 
 
     if binsize is None:
         binsize = pixelscale
 
-    y, x = np.indices(image.shape, dtype=float)
+    y, x = nnp.indices(image.shape, dtype=float)
     if center is None:
         # get exact center of image
         # center = (image.shape[1]/2, image.shape[0]/2)
         center = tuple((a - 1) / 2.0 for a in image.shape[::-1])
 
     x -= center[0]
     y -= center[1]
 
-    r = np.sqrt(x ** 2 + y ** 2) * pixelscale / binsize  # radius in bin size steps
+    r = nnp.sqrt(x ** 2 + y ** 2) * pixelscale / binsize  # radius in bin size steps
 
     if pa_range is None:
         # Use full image
-        ind = np.argsort(r.flat)
+        ind = nnp.argsort(r.flat)
         sr = r.flat[ind]  # sorted r
         sim = image.flat[ind]  # sorted image
 
     else:
         # Apply the PA range restriction
-        pa = np.rad2deg(np.arctan2(-x, y))  # Note the (-x,y) convention is needed for astronomical PA convention
+        pa = nnp.rad2deg(nnp.arctan2(-x, y))  # Note the (-x,y) convention is needed for astronomical PA convention
         mask = (pa >= pa_range[0]) & (pa <= pa_range[1])
-        ind = np.argsort(r[mask].flat)
+        ind = nnp.argsort(r[mask].flat)
         sr = r[mask].flat[ind]
         sim = image[mask].flat[ind]
 
     ri = sr.astype(int)  # sorted r as int
     deltar = ri[1:] - ri[:-1]  # assume all radii represented (more work if not)
-    rind = np.where(deltar)[0]
+    rind = nnp.where(deltar)[0]
     nr = rind[1:] - rind[:-1]  # number in radius bin
-    csim = np.nan_to_num(sim).cumsum(dtype=float)  # cumulative sum to figure out sums for each bin
-    # np.nancumsum is implemented in >1.12
+    csim = nnp.nan_to_num(sim).cumsum(dtype=float)  # cumulative sum to figure out sums for each bin
+    # nnp.nancumsum is implemented in >1.12
     tbin = csim[rind[1:]] - csim[rind[:-1]]  # sum for image values in radius bins
     radialprofile = tbin / nr
 
     # pre-pend the initial element that the above code misses.
-    radialprofile2 = np.empty(len(radialprofile) + 1)
+    radialprofile2 = nnp.empty(len(radialprofile) + 1)
     if rind[0] != 0:
         radialprofile2[0] = csim[rind[0]] / (
                 rind[0] + 1)  # if there are multiple elements in the center bin, average them
     else:
         radialprofile2[0] = csim[0]  # otherwise if there's just one then just take it.
     radialprofile2[1:] = radialprofile
 
-    rr = np.arange(ri.min(), ri.min()+len(radialprofile2)) * binsize + binsize * 0.5  # these should be centered in the bins, so add a half.
+    rr = nnp.arange(ri.min(), ri.min()+len(radialprofile2)) * binsize + binsize * 0.5  # these should be centered in the bins, so add a half.
 
 
     if maxradius is not None:
         crop = rr < maxradius
         rr = rr[crop]
         radialprofile2 = radialprofile2[crop]
 
     if stddev:
-        stddevs = np.zeros_like(radialprofile2)
+        stddevs = nnp.zeros_like(radialprofile2)
         r_pix = r * binsize
         for i, radius in enumerate(rr):
             if i == 0:
-                wg = np.where(r < radius + binsize / 2)
+                wg = nnp.where(r < radius + binsize / 2)
             else:
-                wg = np.where((r_pix >= (radius - binsize / 2)) & (r_pix < (radius + binsize / 2)))
-                # wg = np.where( (r >= rr[i-1]) &  (r <rr[i] )))
-            stddevs[i] = np.nanstd(image[wg])
+                wg = nnp.where((r_pix >= (radius - binsize / 2)) & (r_pix < (radius + binsize / 2)))
+                # wg = nnp.where( (r >= rr[i-1]) &  (r <rr[i] )))
+            stddevs[i] = nnp.nanstd(image[wg])
         return rr, stddevs
 
     if nargout == 1:
         return radialprofile2
     
     if not ee:
         return rr, radialprofile2
@@ -899,37 +927,37 @@
     # anisoplanatic PSF. Prefer the coutour function in such a
     # case. The cutting method is not compliant to PSF not oriented
     #along x or y-axis.
 
     #Interpolation            
     Ny,Nx = psf.shape
     if rebin > 1:
-        im_hr = interpolateSupport(psf,rebin*np.array([Nx,Ny]))
+        im_hr = nnp.asarray(interpolateSupport(psf,rebin*nnp.array([Nx,Ny])))
     else:
-        im_hr = psf
+        im_hr = nnp.asarray(psf)
         
     ss = im_hr.shape
     sbx, sby = [[0,ss[1]],[0,ss[0]]]
 
-    peak_val = np.max(im_hr)
+    peak_val = nnp.max(im_hr)
     # initial guess of PSF center
-    y_peak, x_peak = np.where(im_hr == peak_val)
+    y_peak, x_peak = nnp.where(nnp.equal(im_hr, peak_val))
     x00 = sbx[0]
     y00 = sby[0]
     x_peak += x00
     y_peak += y00
     
     if method == 'cutting':
         # Brutal approach when the PSF is centered and aligned x-axis FWHM
         imx     = im_hr[:,y_peak]
-        wx      = np.where(imx >= imx.max()/2)[0]
+        wx      = nnp.where(imx >= imx.max()/2)[0]
         FWHMx   = (wx.max() - wx.min())/rebin*pixelScale
         #y-axis FWHM
         imy     = im_hr[x_peak,:]
-        wy      = np.where(imy >= imy.max()/2)[1]
+        wy      = nnp.where(imy >= imy.max()/2)[1]
         FWHMy   = (wy.max() - wy.min())/rebin*pixelScale
         theta   = 0
 
     elif method == 'contour':
         # Contour approach~: something wrong about the ellipse orientation
         mpl.interactive(False)
         try:
@@ -937,69 +965,69 @@
             C       = plt.contour(im_hr,levels=[im_hr.max()/2])
             plt.close(666)
             C       = C.collections[0].get_paths()[0]
             C       = C.vertices
             xC      = C[:,0]
             yC      = C[:,1]
             # centering the ellispe
-            mx      = np.array([xC.max(),yC.max()])
-            mn      = np.array([xC.min(),yC.min()])
+            mx      = nnp.array([xC.max(),yC.max()])
+            mn      = nnp.array([xC.min(),yC.min()])
             cent    = (mx+mn)/2
             wx      = xC - cent[0]
             wy      = yC - cent[1] 
             # Get the module
-            wr      = np.hypot(wx,wy)/rebin*pixelScale                
+            wr      = nnp.hypot(wx,wy)/rebin*pixelScale                
             # Getting the FWHM
             FWHMx   = 2*wr.max()
             FWHMy   = 2*wr.min()
             #Getting the ellipse orientation
             xm      = wx[wr.argmax()]
             ym      = wy[wr.argmax()]
-            theta   = np.mean(180*np.arctan2(ym,xm)/np.pi)
+            theta   = nnp.mean(180*nnp.arctan2(ym,xm)/np.pi)
         except:
             FWHMx = -1 
             FWHMy = -1 
             aRatio= -1
             theta = -1
         mpl.interactive(True)   
     elif method == 'gaussian':
         # initial guess of the FWHM
-        fwhm_guess = 2*np.sqrt((im_hr > peak_val/2).sum()/np.pi)
+        fwhm_guess = 2*nnp.sqrt((im_hr > peak_val/2).sum()/np.pi)
         
-        stddev_guess = fwhm_guess/(2*np.sqrt(2*np.log(2)))
+        stddev_guess = fwhm_guess/(2*nnp.sqrt(2*nnp.log(2)))
         p_init = models.Gaussian2D(amplitude=peak_val, x_mean=x_peak[0], y_mean=y_peak[0],
                                    x_stddev=stddev_guess, y_stddev=stddev_guess)
         
         fit_p = fitting.LevMarLSQFitter()
     
-        y,x = np.mgrid[sby[0]:sby[1],sbx[0]:sbx[1]]
+        y,x = nnp.mgrid[sby[0]:sby[1],sbx[0]:sbx[1]]
         g = fit_p(p_init, x, y, im_hr)
         
-        FWHMx = 2 * np.sqrt(2 * np.log(2)) * np.abs(g.x_stddev.value*pixelScale)
-        FWHMy = 2 * np.sqrt(2 * np.log(2)) * np.abs(g.y_stddev.value*pixelScale)
+        FWHMx = 2 * nnp.sqrt(2 * nnp.log(2)) * nnp.abs(g.x_stddev.value*pixelScale)
+        FWHMy = 2 * nnp.sqrt(2 * nnp.log(2)) * nnp.abs(g.y_stddev.value*pixelScale)
         theta = g.theta.value*180/np.pi
     elif method == 'moffat':      
         # initial guess of the FWHM
-        fwhm_guess = 2*np.sqrt((im_hr > peak_val/2).sum()/np.pi)
+        fwhm_guess = 2*nnp.sqrt((im_hr > peak_val/2).sum()/np.pi)
         
         beta = 4.765    # expected beta value  for Seeing limited PSF
         p_init = models.Moffat2D(amplitude=peak_val, x_0=x_peak[0], y_0=y_peak[0],
-                                 gamma=fwhm_guess/(2*np.sqrt(2**(1/beta)-1)))
+                                 gamma=fwhm_guess/(2*nnp.sqrt(2**(1/beta)-1)))
         
         fit_p = fitting.LevMarLSQFitter()
     
-        y,x = np.mgrid[sby[0]:sby[1],sbx[0]:sbx[1]]
+        y,x = nnp.mgrid[sby[0]:sby[1],sbx[0]:sbx[1]]
         g = fit_p(p_init, x, y, im_hr)
         
         FWHMx = g.fwhm*pixelScale
         FWHMy = g.fwhm*pixelScale
         theta   = 0
         
     # Get Ellipticity
-    aRatio      = np.max([FWHMx/FWHMy,FWHMy/FWHMx])
+    aRatio      = nnp.max([FWHMx/FWHMy,FWHMy/FWHMx])
     
     if nargout == 1:
         return 0.5 * (FWHMx+FWHMy)
     elif nargout == 2:
         return FWHMx,FWHMy
     elif nargout == 3:
         return FWHMx,FWHMy,aRatio
@@ -1012,15 +1040,15 @@
     else:
         psf = psf0
         
     if method == 'otf':
         #% Get the OTF
         otf     = fft.fftshift(psf2otf(psf))
         otf     = otf/otf.max()
-        notf    = np.array(otf.shape)
+        notf    = nnp.array(otf.shape)
         
         # Get the Diffraction-limit OTF
         nX,nY   = pupil.shape
         pup_pad = enlargeSupport(pupil,samp)
         otfDL   = fft.fftshift(abs(fft.ifft2(fft.fft2(fft.fftshift(pup_pad))**2)))
         otfDL   = interpolateSupport(otfDL,notf)
         otfDL   = otfDL/otfDL.max()
@@ -1091,11 +1119,11 @@
     # ------- Including shifts ---------
     X     = xdata[0]
     Y     = xdata[1]
     #Shifts
     X     = X - x0
     Y     = Y - y0
     #Rotation
-    Xr    = X*np.cos(th) + Y*np.sin(th)
-    Yr    = Y*np.cos(th) - X*np.sin(th)
+    Xr    = X*nnp.cos(th) + Y*nnp.sin(th)
+    Yr    = Y*nnp.cos(th) - X*nnp.sin(th)
     # Gaussian expression
-    return I0*np.exp(-0.5*((Xr/ax)**2 + (Yr/ay)**2) )
+    return I0*nnp.exp(-0.5*((Xr/ax)**2 + (Yr/ay)**2) )
```

### Comparing `astro-p3-1.1/p3/aoSystem/_txtFile/ELT_segmentVertices.txt` & `astro-p3-1.2/p3/aoSystem/_txtFile/ELT_segmentVertices.txt`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/anisoplanatismModel.py` & `astro-p3-1.2/p3/aoSystem/anisoplanatismModel.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/aoSystem.py` & `astro-p3-1.2/p3/aoSystem/aoSystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Created on Mon Apr  5 14:42:49 2021
 
 @author: omartin
 """
 
 # IMPORTING PYTHON LIBRAIRIES
 import os.path as ospath
+import pathlib
 from configparser import ConfigParser
 import numpy as np
 
 import yaml
 
 # IMPORTING P3 MODULES
 from p3.aoSystem.telescope import telescope
@@ -102,49 +103,87 @@
             nPup = self.get_config_value('telescope','Resolution')
         else:
             print('%%%%%%%% ERROR %%%%%%%%')
             print('You must provide a value for the pupil (telescope) resolution\n')
             self.error = True
             return
             
+        path_p3 = str(pathlib.Path(__file__).parent.parent.absolute())
+            
         #----- PUPIL
         if self.check_config_key('telescope','PathPupil'):
-            path_pupil = path_root + self.get_config_value('telescope','PathPupil')
+            PathPupil = self.get_config_value('telescope','PathPupil')
+            if path_root == '' and PathPupil[0:9]=='/aoSystem' :
+                path_pupil = path_p3 + PathPupil
+            elif path_root == '' and PathPupil[0:8]=='aoSystem' :
+                path_pupil = path_p3 +'/'+ PathPupil
+            else:
+                path_pupil = path_root + PathPupil
         else:
             path_pupil = ''
                   
         if self.check_config_key('telescope','PupilAngle'):
             pupilAngle = self.get_config_value('telescope','PupilAngle')
         else:
             pupilAngle = 0.0
         
         if self.check_config_key('telescope','PathStaticOn'):
-            path_static_on = path_root + self.get_config_value('telescope','PathStaticOn')
+            PathStaticOn = self.get_config_value('telescope','PathStaticOn')
+            if path_root == '' and PathStaticOn[0:9]=='/aoSystem' :
+                path_static_on = path_p3 + PathStaticOn
+            elif path_root == '' and PathStaticOn[0:8]=='aoSystem' :
+                path_static_on = path_p3 +'/'+ PathStaticOn
+            else:
+                path_static_on = path_root + PathStaticOn
         else:
             path_static_on = None       
         
         if self.check_config_key('telescope','PathStaticOff'):
-            path_static_off = path_root +self.get_config_value('telescope','PathStaticOff')
+            PathStaticOff = self.get_config_value('telescope','PathStaticOff')
+            if path_root == '' and PathStaticOff[0:9]=='/aoSystem' :
+                path_static_off = path_p3 + PathStaticOff
+            elif path_root == '' and PathStaticOff[0:8]=='aoSystem' :
+                path_static_off = path_p3 +'/'+ PathStaticOff
+            else:
+                path_static_off = path_root + PathStaticOff
         else:
             path_static_off = None
         
         if self.check_config_key('telescope','PathStaticPos'):
-            path_static_pos = path_root + self.get_config_value('telescope','PathStaticPos')
+            PathStaticPos = self.get_config_value('telescope','PathStaticPos')
+            if path_root == '' and PathStaticPos[0:9]=='/aoSystem' :
+                path_static_pos = path_p3 + PathStaticPos
+            elif path_root == '' and PathStaticPos[0:8]=='aoSystem' :
+                path_static_pos = path_p3 +'/'+ PathStaticPos
+            else:
+                path_static_pos = path_root + PathStaticPos
         else:
             path_static_pos = None
             
         #----- APODIZER
         if self.check_config_key('telescope','PathApodizer'):
-            path_apodizer = path_root + self.get_config_value('telescope','PathApodizer')
+            PathApodizer = self.get_config_value('telescope','PathApodizer')
+            if path_root == '' and PathApodizer[0:9]=='/aoSystem' :
+                path_apodizer = path_p3 + PathApodizer
+            elif path_root == '' and PathApodizer[0:8]=='aoSystem' :
+                path_apodizer = path_p3 +'/'+ PathApodizer
+            else:
+                path_apodizer = path_root + PathApodizer
         else:
             path_apodizer = ''
                 
         #----- TELESCOPE ABERRATIONS
         if self.check_config_key('telescope', 'PathStatModes'):
-            path_statModes = path_root + self.get_config_value('telescope','PathStatModes')
+            PathStatModes = self.get_config_value('telescope','PathStatModes')
+            if path_root == '' and PathStatModes[0:9]=='/aoSystem' :
+                path_statModes = path_p3 + PathStatModes
+            elif path_root == '' and PathStatModes[0:8]=='aoSystem' :
+                path_statModes = path_p3 +'/'+ PathStatModes
+            else:
+                path_statModes = path_root + PathStatModes
         else:
             path_statModes = ''
             
         #----- EXTRA ERROR
         if self.check_config_key('telescope', 'extraErrorNm'):       
             extraErrorNm = self.get_config_value('telescope','extraErrorNm')
         else:
@@ -193,14 +232,18 @@
         if self.check_config_key('atmosphere','L0'):
             L0 = self.get_config_value('atmosphere','L0') 
         else:
             L0 = 25
             
         if self.check_config_key('atmosphere','Cn2Weights'):
             weights = self.get_config_value('atmosphere','Cn2Weights') 
+            if np.abs(np.sum(weights) - 1) > 1e-3:
+                print('%%%%%%%% ERROR %%%%%%%%')
+                print('Sum of Cn2 weights not equal to 1, please correct parameter file')
+                self.error = True
         else:
             weights = [1.0]
         
         if self.check_config_key('atmosphere','Cn2Heights'):
             heights = self.get_config_value('atmosphere','Cn2Heights') 
         else:
             heights = [0.0]
```

### Comparing `astro-p3-1.1/p3/aoSystem/atmosphere.py` & `astro-p3-1.2/p3/aoSystem/atmosphere.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/createSegmentedModes.py` & `astro-p3-1.2/p3/aoSystem/createSegmentedModes.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits` & `astro-p3-1.2/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits` & `astro-p3-1.2/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits` & `astro-p3-1.2/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits` & `astro-p3-1.2/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/defineAoSystem.py` & `astro-p3-1.2/p3/aoSystem/defineAoSystem.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/deformableMirror.py` & `astro-p3-1.2/p3/aoSystem/deformableMirror.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/detector.py` & `astro-p3-1.2/p3/aoSystem/detector.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/fourierModel.py` & `astro-p3-1.2/p3/aoSystem/fourierModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Aug 16 15:00:44 2018
 
 @author: omartin
 """
-import numpy as np
-import matplotlib as mpl
 
-import numpy.fft as fft
+import numpy as nnp
+from . import gpuEnabled
+
+if not gpuEnabled:
+    np = nnp
+    import numpy.fft as fft
+    import scipy.special as spc
+else:
+    import cupy as cp
+    import cupy.fft as fft
+    import cupyx.scipy.special as spc
+    np = cp
+
+import matplotlib as mpl
 import matplotlib.pyplot as plt
-import scipy.special as spc
 
 import time
 from distutils.spawn import find_executable
 
 import p3.aoSystem.FourierUtils as FourierUtils
 from p3.aoSystem.aoSystem import aoSystem
 from p3.aoSystem.atmosphere import atmosphere
@@ -35,15 +45,15 @@
     usetex = True
 else:
     usetex = False
 
 plt.rcParams.update({
     "text.usetex": usetex,
     "font.family": "serif",
-    "font.serif": ["Palatino"],
+    "font.serif": ["Palatino","DejaVu Sans"],
 })
  
 #%%
 rad2mas = 3600 * 180 * 1000 / np.pi
 rad2arc = rad2mas / 1000
 deg2rad = np.pi/180
 
@@ -107,16 +117,18 @@
             
             self.atm_mod = atmosphere(self.ao.atm.wvl,self.ao.atm.r0,weights_mod,heights_mod,wSpeed_mod,wDir_mod,self.ao.atm.L0)
             
             #updating the atmosphere wavelength !
             self.ao.atm.wvl  = self.freq.wvlRef
             self.atm_mod.wvl = self.freq.wvlRef
             self.t_initFreq = 1000*(time.time() - tstart)
-            
-            if (2*self.freq.kcInMas/self.freq.psInMas)[0] > self.freq.nOtf:
+
+            vv = self.freq.psInMas
+            rr = 2*self.freq.kcInMas/vv 
+            if rr[0] > self.freq.nOtf:
                 raise ValueError('Error : the PSF field of view is too small to simulate the AO correction area')
             
             # DEFINING THE NOISE AND ATMOSPHERE PSD
             if self.ao.wfs.processing.noiseVar == [None]:
                 self.ao.wfs.processing.noiseVar = self.ao.wfs.NoiseVariance(self.ao.atm.r0 ,self.ao.atm.wvl)
             
             self.Wn   = np.mean(self.ao.wfs.processing.noiseVar)/(2*self.freq.kcMax_)**2
@@ -179,19 +191,19 @@
 #%% BOUNDS FOR PSF-FITTING
     def defineBounds(self):
           
         # Photometry
         bounds_down = [-np.inf,-np.inf,-np.inf]
         bounds_up = [np.inf,np.inf,np.inf]
         # Photometry
-        bounds_down += list(np.zeros(self.ao.src.nSrc))
-        bounds_up += list(np.inf*np.ones(self.ao.src.nSrc))
+        bounds_down += np.zeros(self.ao.src.nSrc).tolist()
+        bounds_up += (np.inf*np.ones(self.ao.src.nSrc)).tolist()
         # Astrometry
-        bounds_down += list(-self.freq.nPix//2 * np.ones(2*self.ao.src.nSrc))
-        bounds_up += list( self.freq.nPix//2 * np.ones(2*self.ao.src.nSrc))
+        bounds_down += (-self.freq.nPix//2 * np.ones(2*self.ao.src.nSrc)).tolist()
+        bounds_up += ( self.freq.nPix//2 * np.ones(2*self.ao.src.nSrc)).tolist()
         # Background
         bounds_down += [-np.inf]
         bounds_up += [np.inf]
         
         return (bounds_down,bounds_up)
       
 #%% RECONSTRUCTOR DEFINITION    
@@ -224,16 +236,16 @@
                 PbetaDM = np.zeros([nK,nK,1,nDm],dtype=complex)
                 for j in range(nDm): #loop on DMs
                     index               = k <= self.freq.kc_[j] # note : circular masking
                     PbetaDM[index,0,j]  = np.exp(2*i*np.pi*h_dm[j]*(fx[index] + fy[index]))
                 self.PbetaDM.append(PbetaDM)
             
             # Computation of the Malpha matrix
-            wDir_x  = np.cos(self.ao.atm.wDir*np.pi/180)
-            wDir_y  = np.sin(self.ao.atm.wDir*np.pi/180)
+            wDir_x  = nnp.cos(self.ao.atm.wDir*np.pi/180)
+            wDir_y  = nnp.sin(self.ao.atm.wDir*np.pi/180)
             self.MPalphaL = np.zeros([nK,nK,self.nGs,nH],dtype=complex)
             for h in range(nH):
                 www = np.sinc(sampTime*self.ao.atm.wSpeed[h]*(wDir_x[h]*self.freq.kxAO_ + wDir_y[h]*self.freq.kyAO_))
                 for g in range(self.nGs):
                     Alpha = [self.gs.direction[0,g],self.gs.direction[1,g]]
                     fx = Alpha[0]*self.freq.kxAO_
                     fy = Alpha[1]*self.freq.kyAO_
@@ -340,16 +352,16 @@
         h_mod   = self.atm_mod.heights * self.strechFactor_mod
         nL      = len(h_mod)
         nK      = self.freq.resAO
         i       = complex(0,1)
         
         mat1    = np.zeros([nK,nK,nDm,nL],dtype=complex)
         to_inv  = np.zeros([nK,nK,nDm,nDm],dtype=complex)
-        theta_x = self.ao.dms.opt_dir[0]/206264.8 * np.cos(self.ao.dms.opt_dir[1]*np.pi/180)
-        theta_y = self.ao.dms.opt_dir[0]/206264.8 * np.sin(self.ao.dms.opt_dir[1]*np.pi/180)
+        theta_x = self.ao.dms.opt_dir[0]/206264.8 * nnp.cos(self.ao.dms.opt_dir[1]*np.pi/180)
+        theta_y = self.ao.dms.opt_dir[0]/206264.8 * nnp.sin(self.ao.dms.opt_dir[1]*np.pi/180)
         
         for d_o in range(nDir):                 #loop on optimization directions
             Pdm = np.zeros([nK,nK,1,nDm],dtype=complex)
             Pl  = np.zeros([nK,nK,1,nL],dtype=complex)
             fx  = theta_x[d_o]*self.freq.kxAO_
             fy  = theta_y[d_o]*self.freq.kyAO_
             for j in range(nDm):                # loop on DM
@@ -375,16 +387,16 @@
         """
         """
         tstart  = time.time()
         
         if self.ao.rtc.holoop['gain'] != 0:     
         
             i           = complex(0,1)
-            vx          = self.ao.atm.wSpeed*np.cos(self.ao.atm.wDir*np.pi/180)
-            vy          = self.ao.atm.wSpeed*np.sin(self.ao.atm.wDir*np.pi/180)   
+            vx          = self.ao.atm.wSpeed*nnp.cos(self.ao.atm.wDir*np.pi/180)
+            vy          = self.ao.atm.wSpeed*nnp.sin(self.ao.atm.wDir*np.pi/180)   
             nPts        = self.freq.resAO
             thetaWind   = np.linspace(0, 2*np.pi-2*np.pi/nTh,nTh)
             costh       = np.cos(thetaWind)
             weights     = self.ao.atm.weights
             Ts          = 1.0/self.ao.rtc.holoop['rate']#samplingTime
             delay       = self.ao.rtc.holoop['delay']#latency        
             loopGain    = self.ao.rtc.holoop['gain']
@@ -447,15 +459,15 @@
                 plt.xlabel('Temporal frequency (Hz)')
                 plt.ylabel('Magnitude (dB)')
                 plt.grid('on')
                 plt.legend()
             
         self.t_controller = 1000*(time.time() - tstart)
       
-#%% PSD DEFINTIONS  
+    #%% PSD DEFINTIONS  
     def powerSpectrumDensity(self,wfe=None):
         """ Total power spectrum density in nm^2.m^2
         """
         tstart  = time.time()
         
         dk     = 2*self.freq.kcMax_/self.freq.resAO
         rad2nm = self.ao.atm.wvl*1e9/2/np.pi
@@ -547,16 +559,16 @@
         
         tstart  = time.time()
         psd = np.zeros((self.freq.resAO,self.freq.resAO))
         i  = complex(0,1)
         d  = self.ao.wfs.optics[0].dsub
         T  = 1.0/self.ao.rtc.holoop['rate']
         td = T * self.ao.rtc.holoop['delay']        
-        vx = self.ao.atm.wSpeed*np.cos(self.ao.atm.wDir*np.pi/180)
-        vy = self.ao.atm.wSpeed*np.sin(self.ao.atm.wDir*np.pi/180)
+        vx = self.ao.atm.wSpeed*nnp.cos(self.ao.atm.wDir*np.pi/180)
+        vy = self.ao.atm.wSpeed*nnp.sin(self.ao.atm.wDir*np.pi/180)
         weights = self.ao.atm.weights  
         w = 2*i*np.pi*d
 
         if hasattr(self, 'Rx') == False:
             self.reconstructionFilter()
         Rx = self.Rx*w
         Ry = self.Ry*w
@@ -649,16 +661,16 @@
         nK  = self.freq.resAO
         psd = np.zeros((nK,nK,self.ao.src.nSrc),dtype=complex)        
         i   = complex(0,1)
         nH  = self.ao.atm.nL
         Hs  = self.ao.atm.heights * self.strechFactor
         Ws  = self.ao.atm.weights
         deltaT  = self.ao.rtc.holoop['delay']/self.ao.rtc.holoop['rate']
-        wDir_x  = np.cos(self.ao.atm.wDir*np.pi/180)
-        wDir_y  = np.sin(self.ao.atm.wDir*np.pi/180)
+        wDir_x  = nnp.cos(self.ao.atm.wDir*np.pi/180)
+        wDir_y  = nnp.sin(self.ao.atm.wDir*np.pi/180)
         Watm    = self.Wphi * self.freq.pistonFilterAO_      
         F       = self.Rx*self.SxAv + self.Ry*self.SyAv
         
         for s in range(self.ao.src.nSrc):
             if self.nGs < 2:  
                 th  = self.ao.src.direction[:,s] - self.gs.direction[:,0]
                 if np.any(th):
@@ -904,26 +916,26 @@
         """        
         tstart  = time.time()
         
         if self.ao.rtc.holoop['gain'] != 0:
             # Derives wavefront error
             rad2nm      = (2*self.freq.kcMax_/self.freq.resAO) * self.freq.wvlRef*1e9/2/np.pi
             
-            if np.any(self.ao.tel.opdMap_on):
+            if not self.ao.tel.opdMap_on is None:
                 self.wfeNCPA= np.std(self.ao.tel.opdMap_on[self.ao.tel.pupil!=0])
             else:
                 self.wfeNCPA = 0.0
                 
             self.wfeFit    = np.sqrt(self.psdFit.sum()) * rad2nm
             self.wfeAl     = np.sqrt(self.psdAlias.sum()) * rad2nm
             self.wfeN      = np.sqrt(self.psdNoise.sum(axis=(0,1)))* rad2nm
             self.wfeST     = np.sqrt(self.psdSpatioTemporal.sum(axis=(0,1)))* rad2nm
             self.wfeDiffRef= np.sqrt(self.psdDiffRef.sum(axis=(0,1)))* rad2nm
             self.wfeChrom  = np.sqrt(self.psdChromatism.sum(axis=(0,1)))* rad2nm
-            self.wfeJitter = 1e9*self.ao.tel.D*np.mean(self.ao.cam.spotFWHM[0][0:2])/rad2mas/4
+            self.wfeJitter = 1e9*self.ao.tel.D*nnp.mean(self.ao.cam.spotFWHM[0][0:2])/rad2mas/4
             self.wfeExtra  = self.ao.tel.extraErrorNm
             
             # Total wavefront error
             self.wfeTot = np.sqrt(self.wfeNCPA**2 + self.wfeFit**2 + self.wfeAl**2\
                                   + self.wfeST**2 + self.wfeN**2 + self.wfeDiffRef**2\
                                   + self.wfeChrom**2 + self.wfeJitter**2 + self.wfeExtra**2)
             
@@ -955,15 +967,15 @@
                 print('.Chromatic error:\t\t%4.2fnm'%self.wfeChrom[idCenter])
                 print('.Aliasing error:\t\t%4.2fnm'%self.wfeAl)
                 if self.nGs == 1:
                     print('.Noise error:\t\t\t%4.2fnm'%self.wfeN)
                 else:
                     print('.Noise error:\t\t\t%4.2fnm'%self.wfeN[idCenter])
                 print('.Spatio-temporal error:\t\t%4.2fnm'%self.wfeST[idCenter])
-                print('.Additionnal jitter:\t\t%4.2fmas / %4.2fnm'%(np.mean(self.ao.cam.spotFWHM[0][0:2]),self.wfeJitter))
+                print('.Additionnal jitter:\t\t%4.2fmas / %4.2fnm'%(nnp.mean(self.ao.cam.spotFWHM[0][0:2]),self.wfeJitter))
                 print('.Extra error:\t\t\t%4.2fnm'%self.wfeExtra)
                 print('-------------------------------------------')
                 print('.Sole servoLag error:\t\t%4.2fnm'%self.wfeS)
                 print('.Sole reconstruction error:\t%4.2fnm'%self.wfeR)
                 print('-------------------------------------------')            
                 if self.nGs == 1:
                     print('.Sole anisoplanatism error:\t%4.2fnm'%self.wfeAni[idCenter])
```

### Comparing `astro-p3-1.1/p3/aoSystem/frequencyDomain.py` & `astro-p3-1.2/p3/aoSystem/frequencyDomain.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 """
 Created on Mon Apr 19 11:34:44 2021
 
 @author: omartin
 """
 
 # IMPORTING PYTHON LIBRAIRIES
-import numpy as np
+import numpy as nnp
+from . import gpuEnabled
+
+if not gpuEnabled:
+    np = nnp
+else:
+    import cupy as cp
+    np = cp
+
 import p3.aoSystem.FourierUtils as FourierUtils
 from p3.aoSystem.anisoplanatismModel import anisoplanatism_structure_function
 import time
 
 #%%
 rad2mas = 3600 * 180 * 1000 / np.pi
 rad2arc = rad2mas / 1000
@@ -25,26 +33,26 @@
     @wvl.setter
     def wvl(self,val):
         self.__wvl = val
         if self.nyquistSampling == True:
             self.samp  = 2.0 * np.ones_like(self.psInMas)
         else:
             self.samp  = val* rad2mas/(self.psInMas*self.ao.tel.D)
-        
+
     @property
     def wvlCen(self):
         return self.__wvlCen
     @wvlCen.setter
     def wvlCen(self,val):
         self.__wvlCen = val
         if self.nyquistSampling == True:
             self.sampCen  = 2.0 * np.ones(len(val))
         else:
             self.sampCen  = val* rad2mas/(self.psInMasCen*self.ao.tel.D)
-            
+
     @property
     def wvlRef(self):
         return self.__wvlRef
     @wvlRef.setter
     def wvlRef(self,val):
         self.__wvlRef = val
         if self.nyquistSampling == True:
@@ -59,15 +67,16 @@
     def samp(self,val):
         self.k_      = np.ceil(2.0/val).astype('int') # works for oversampling
         self.__samp  = self.k_ * val
         if np.any(self.k_ > 2):
             self.PSDstep= np.min(1/self.ao.tel.D/self.__samp)
         else:
             self.PSDstep= np.min(self.psInMas/self.wvl_/rad2mas)
-            
+        self.PSDstep= np.asarray(self.PSDstep)
+
     @property
     def sampCen(self):
         return self.__sampCen
     @sampCen.setter
     def sampCen(self,val):
         self.kCen_      = np.ceil(2.0/val).astype(int)# works for oversampling
         self.__sampCen  = self.kCen_ * val
@@ -77,37 +86,38 @@
     @sampRef.setter
     def sampRef(self,val):
         self.kRef_      = int(np.ceil(2.0/val)) # works for oversampling
         self.__sampRef  = self.kRef_ * val
         self.nOtf       = self.nPix * self.kRef_
         #  ---- FULL DOMAIN OF FREQUENCY
         self.kx_,self.ky_ = FourierUtils.freq_array(self.nOtf,offset=1e-10,L=self.PSDstep)
-        self.k2_          = self.kx_**2 + self.ky_**2       
+        self.k2_          = self.kx_**2 + self.ky_**2
         #piston filtering        
         self.pistonFilter_ = FourierUtils.pistonFilter(self.ao.tel.D,np.sqrt(self.k2_))
         self.pistonFilter_[self.nOtf//2,self.nOtf//2] = 0
     
     # CUT-OFF FREQUENCY
     @property
     def pitch(self):
         return self.__pitch    
     @pitch.setter
     def pitch(self,val):
         self.__pitch = val
         # redefining the ao-corrected area
-        if np.all(self.kcExt !=None):
+        if not self.kcExt is None and np.all(self.kcExt):
             self.kc_= self.kcExt
         else:
             #return 1/(2*max(self.pitchs_dm.min(),self.pitchs_wfs.min()))
             self.kc_ =  1/(2*val)
             #self.kc_= (val-1)/(2.0*self.ao.tel.D)
         self.kcMax_ =  np.max(self.kc_)
         #kc2         = self.kc_**2
+        self.kc_ = np.asarray(self.kc_)
         self.resAO  = int(np.max(2*self.kc_/self.PSDstep))
-        
+
         # ---- SPATIAL FREQUENCY DOMAIN OF THE AO-CORRECTED AREA
         #import pdb
         #pdb.set_trace()
         self.kxAO_,self.kyAO_ = FourierUtils.freq_array(self.resAO,offset=1e-10,L=self.PSDstep)
         self.k2AO_            = self.kxAO_**2 + self.kyAO_**2   
         self.pistonFilterAO_  = FourierUtils.pistonFilter(self.ao.tel.D,np.sqrt(self.k2AO_))
         self.pistonFilterAO_[self.resAO//2,self.resAO//2] = 0
@@ -209,15 +219,15 @@
     def anisoplanatismPhaseStructureFunction(self,computeFocalAnisoCov=True):
         
         # compute th Cn2 profile in m^(-5/3)
         Cn2 = self.ao.atm.weights * self.ao.atm.r0**(-5/3)
 
         if self.ao.aoMode == 'SCAO' or computeFocalAnisoCov == False:
             # NGS case : angular-anisoplanatism only
-            if np.all(self.ao.src.direction == self.ao.ngs.direction):
+            if np.all(np.equal(self.ao.src.direction, self.ao.ngs.direction)):
                 self.isAniso = False
                 return None
             else:
                 self.isAniso = True
                 self.dani_ang = \
                 anisoplanatism_structure_function(self.ao.tel,self.ao.atm,self.ao.src,
                                                 self.ao.ngs,self.ao.ngs,self.nOtf,
```

### Comparing `astro-p3-1.1/p3/aoSystem/optics.py` & `astro-p3-1.2/p3/aoSystem/optics.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/HarmoniLTAO.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/HarmoniLTAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/HarmoniSCAO.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/HarmoniSCAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/MavisMCAO.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/MavisMCAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/MosaicGLAO.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/MosaicGLAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/eris.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/eris.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/irdis.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/irdis.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/nirc2.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/nirc2.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/nirc2_monochromatic.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/nirc2_monochromatic.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/parFiles/template.ini` & `astro-p3-1.2/p3/aoSystem/parFiles/template.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/processing.py` & `astro-p3-1.2/p3/aoSystem/processing.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/pupil.py` & `astro-p3-1.2/p3/aoSystem/pupil.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/rtc.py` & `astro-p3-1.2/p3/aoSystem/rtc.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/segment.py` & `astro-p3-1.2/p3/aoSystem/segment.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/source.py` & `astro-p3-1.2/p3/aoSystem/source.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/spiders.py` & `astro-p3-1.2/p3/aoSystem/spiders.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/telescope.py` & `astro-p3-1.2/p3/aoSystem/telescope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Aug 16 16:34:02 2018
 
 @author: omartin
 """
-import numpy as np
+import numpy as nnp
+from . import gpuEnabled
+
+if not gpuEnabled:
+    np = nnp
+    from scipy.ndimage import rotate
+else:
+    import cupy as cp
+    np = cp
+    from cupyx.scipy.ndimage import rotate
+
 from astropy.io import fits
 import os.path as ospath
 import re
-from scipy.ndimage import rotate
 import p3.aoSystem.FourierUtils as FourierUtils
 
 class Attribute(object):
     pass
 
 class telescope:
     """ Telescope class that defines the telescope characteristics.
@@ -44,15 +53,15 @@
         return np.pi*self.R**2*(1-self.obsRatio**2)
     @property
     def pupilLogical(self):
         """Telescope area in meter square"""
         return self.pupil.astype(bool)
     @property
     def airmass(self):
-        return 1/np.cos(self.zenith_angle*np.pi/180)
+        return 1/nnp.cos(self.zenith_angle*np.pi/180)
     
     # CONSTRUCTOR
     def __init__(self,D,resolution, zenith_angle=0.0,obsRatio=0.0,pupilAngle = 0.0,\
                  path_pupil='', path_static_on='', path_static_off='', path_static_pos='',\
                  path_apodizer='', path_statModes='', extraErrorNm=0.0, extraErrorExp=-2, \
                  extraErrorMin=0.0, verbose=True):
         
@@ -73,15 +82,15 @@
         self.extraErrorMin   = extraErrorMin
         
         #----- PUPIL DEFINITION        
         
         pupil = [] 
         if path_pupil!= '' and ospath.isfile(path_pupil) == True and re.search(".fits",path_pupil)!=None:
             self.verb = True
-            pupil = fits.getdata(path_pupil)
+            pupil = np.asarray(fits.getdata(path_pupil))
             pupil[pupil!=pupil] = 0
             if self.pupilAngle !=0.0:
                 pupil = rotate(pupil,self.pupilAngle,reshape=False)
             if pupil.shape[0] != resolution:
                 pupil = FourierUtils.interpolateSupport(pupil,resolution,kind='linear')
             self.pupil = pupil
         else:
@@ -97,28 +106,28 @@
             self.verb = False
             self.path_pupil= ''
     
     
         #----- NCPA
         
         if path_static_on != None and ospath.isfile(path_static_on) == True and re.search(".fits",path_static_on)!=None:
-            self.opdMap_on = fits.getdata(path_static_on)
+            self.opdMap_on = np.asarray(fits.getdata(path_static_on))
             self.opdMap_on[self.opdMap_on!=self.opdMap_on] = 0
             if self.pupilAngle !=0.0:
                 self.opdMap_on = rotate(self.opdMap_on,self.pupilAngle,reshape=False)
             self.opdMap_on = FourierUtils.interpolateSupport(self.opdMap_on,resolution,kind='linear')
         else:
             self.opdMap_on = None
             self.path_static_on= ''
             
         #----- FIELD-DEPENDANT STATIC ABERRATIONS
         if path_static_off != None and ospath.isfile(path_static_off) == True and re.search(".fits",path_static_off)!=None:   
             if path_static_pos != None and ospath.isfile(path_static_pos) == True and re.search(".fits",path_static_pos)!=None:   
-                opdMap_off = fits.getdata(path_static_off)
-                opdMap_pos = fits.getdata(path_static_pos)
+                opdMap_off = np.asarray(fits.getdata(path_static_off))
+                opdMap_pos = np.asarray(fits.getdata(path_static_pos))
                 if opdMap_pos.shape[0] != opdMap_off[0]:
                     raise ValueError('You must provide as many positions values as maps')
                 else:
                     self.opdMap_off = opdMap_off
                     self.opdMap_pos = opdMap_pos
             else:
                 raise ValueError('Positions (zenith in arcsec, azimuth in radian) of the field-dependent aberrations must be provided as well as the maps')
@@ -127,29 +136,29 @@
             self.opdMap_pos = None #center of the fov
             self.path_static_off= ''
             self.path_static_pos= ''
             
         #----- APODIZER
         print(path_apodizer)
         if path_apodizer!= '' and ospath.isfile(path_apodizer) and re.search(".fits",path_apodizer)!=None:
-            self.apodizer = fits.getdata(path_apodizer)
+            self.apodizer = np.asarray(fits.getdata(path_apodizer))
             self.apodizer[self.apodizer!=self.apodizer] = 0
             if self.pupilAngle !=0.0:
                 self.apodizer = rotate(self.apodizer,self.pupilAngle,reshape=False)
             self.apodizer = FourierUtils.interpolateSupport(self.apodizer,resolution,kind='linear')
         else:
             self.apodizer = 1.0
             self.path_apodizer = ''
             
         #----- MODAL BASIS FOR TELESCOPE ABERRATIONS
         if path_statModes!='' and ospath.isfile(path_statModes) == True and re.search(".fits",path_statModes)!=None:                
-            statModes = fits.getdata(path_statModes)
+            statModes = np.asarray(fits.getdata(path_statModes))
             s1,s2,s3 = statModes.shape
             if s1 != s2: # mode on first dimension
-                tmp = np.transpose(statModes,(1,2,0))  
+                tmp = np.transpose(statModes,(1,2,0))
             else:
                 tmp = statModes
                     
             self.nModes = tmp.shape[-1]
             self.statModes = np.zeros((resolution,resolution,self.nModes))
                 
             for k in range(self.nModes):
```

### Comparing `astro-p3-1.1/p3/aoSystem/testing/tests_aoSystem.py` & `astro-p3-1.2/p3/aoSystem/testing/tests_aoSystem.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/testing/tests_tiptop_compatibility.py` & `astro-p3-1.2/p3/aoSystem/testing/tests_tiptop_compatibility.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/aoSystem/zernike.py` & `astro-p3-1.2/p3/aoSystem/zernike.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/dataBaseVerification.py` & `astro-p3-1.2/p3/deepLoop/dataBaseVerification.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/dataGenerator.py` & `astro-p3-1.2/p3/deepLoop/dataGenerator.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/dataGeneratorBatch.py` & `astro-p3-1.2/p3/deepLoop/dataGeneratorBatch.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/deepLoopPerformance.py` & `astro-p3-1.2/p3/deepLoop/deepLoopPerformance.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/deepLoopPerformanceBatch.py` & `astro-p3-1.2/p3/deepLoop/deepLoopPerformanceBatch.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/jobGenerate.sh` & `astro-p3-1.2/p3/deepLoop/jobGenerate.sh`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/jobPerformance.sh` & `astro-p3-1.2/p3/deepLoop/jobPerformance.sh`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/deepLoop/recover_list.py` & `astro-p3-1.2/p3/deepLoop/recover_list.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/psfFitting/confidenceInterval.py` & `astro-p3-1.2/p3/psfFitting/confidenceInterval.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/psfFitting/fittingUtils.py` & `astro-p3-1.2/p3/psfFitting/fittingUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/psfFitting/imageModel.py` & `astro-p3-1.2/p3/psfFitting/imageModel.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/psfFitting/psfFitting.py` & `astro-p3-1.2/p3/psfFitting/psfFitting.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/psfao21/psfao21.py` & `astro-p3-1.2/p3/psfao21/psfao21.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/psfr/psfR.py` & `astro-p3-1.2/p3/psfr/psfR.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/psfr/psfrUtils.py` & `astro-p3-1.2/p3/psfr/psfrUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/telemetry/configFile.py` & `astro-p3-1.2/p3/telemetry/configFile.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/telemetry/keckUtils.py` & `astro-p3-1.2/p3/telemetry/keckUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/telemetry/massdimm.py` & `astro-p3-1.2/p3/telemetry/massdimm.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/telemetry/sphereUtils.py` & `astro-p3-1.2/p3/telemetry/sphereUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/telemetry/systemDiagnosis.py` & `astro-p3-1.2/p3/telemetry/systemDiagnosis.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/telemetry/telemetryKASP.py` & `astro-p3-1.2/p3/telemetry/telemetryKASP.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/telemetry/telemetryKeck.py` & `astro-p3-1.2/p3/telemetry/telemetryKeck.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/p3/testing/tests_p3.py` & `astro-p3-1.2/p3/testing/tests_p3.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.1/pyproject.toml` & `astro-p3-1.2/pyproject.toml`

 * *Files identical despite different names*

