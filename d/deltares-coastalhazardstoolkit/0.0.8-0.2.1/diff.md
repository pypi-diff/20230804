# Comparing `tmp/deltares_coastalhazardstoolkit-0.0.8.tar.gz` & `tmp/deltares-coastalhazardstoolkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltares_coastalhazardstoolkit-0.0.8.tar", last modified: Mon Apr  4 15:03:22 2022, max compression
+gzip compressed data, was "deltares-coastalhazardstoolkit-0.2.1.tar", last modified: Fri Aug  4 19:06:18 2023, max compression
```

## Comparing `deltares_coastalhazardstoolkit-0.0.8.tar` & `deltares-coastalhazardstoolkit-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,133 @@
-drwxrwxrwx   0        0        0        0 2022-04-04 15:03:22.984446 deltares_coastalhazardstoolkit-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      653 2022-04-04 15:03:22.984446 deltares_coastalhazardstoolkit-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-04-04 15:03:22.919549 deltares_coastalhazardstoolkit-0.0.8/deltares_coastalhazardstoolkit.egg-info/
--rw-rw-rw-   0        0        0      653 2022-04-04 15:03:22.000000 deltares_coastalhazardstoolkit-0.0.8/deltares_coastalhazardstoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1097 2022-04-04 15:03:22.000000 deltares_coastalhazardstoolkit-0.0.8/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-04 15:03:22.000000 deltares_coastalhazardstoolkit-0.0.8/deltares_coastalhazardstoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2022-04-04 15:03:22.000000 deltares_coastalhazardstoolkit-0.0.8/deltares_coastalhazardstoolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      702 2022-04-04 15:03:22.985411 deltares_coastalhazardstoolkit-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      522 2022-04-04 15:03:03.000000 deltares_coastalhazardstoolkit-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-04 15:03:22.818447 deltares_coastalhazardstoolkit-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-04-04 15:03:22.958646 deltares_coastalhazardstoolkit-0.0.8/src/cht/
--rw-rw-rw-   0        0        0       92 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/__init__.py
--rw-rw-rw-   0        0        0    20027 2022-04-02 00:42:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/bathymetry_database.py
--rw-rw-rw-   0        0        0      490 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/coordinate_systems.py
--rw-rw-rw-   0        0        0    40876 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/delft3dfm.py
--rw-rw-rw-   0        0        0     9328 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/deltares_ini.py
--rw-rw-rw-   0        0        0     2115 2022-04-04 12:09:42.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/fileops.py
--rw-rw-rw-   0        0        0     2138 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/geometry.py
--rw-rw-rw-   0        0        0    31594 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/hurrywave.py
--rw-rw-rw-   0        0        0    32108 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteo.py
-drwxrwxrwx   0        0        0        0 2022-04-04 15:03:22.972415 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/
--rw-rw-rw-   0        0        0       92 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/__init__.py
--rw-rw-rw-   0        0        0    11578 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/coamps_analysis.py
--rw-rw-rw-   0        0        0    12331 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50.py
--rw-rw-rw-   0        0        0     9220 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50_02.py
--rw-rw-rw-   0        0        0    14130 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50_03.py
--rw-rw-rw-   0        0        0    15644 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50_04.py
--rw-rw-rw-   0        0        0     6024 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_forecast_0p25.py
--rw-rw-rw-   0        0        0     4146 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_forecast_0p25_02.py
--rw-rw-rw-   0        0        0     2459 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/misc_tools.py
--rw-rw-rw-   0        0        0    20290 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/nesting.py
--rw-rw-rw-   0        0        0      486 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/pli_file.py
--rw-rw-rw-   0        0        0    35152 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/sfincs.py
--rw-rw-rw-   0        0        0     6472 2022-04-04 12:34:27.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/sftp.py
--rw-rw-rw-   0        0        0     9845 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tekal.py
-drwxrwxrwx   0        0        0        0 2022-04-04 15:03:22.982421 deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/
--rw-rw-rw-   0        0        0       92 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/__init__.py
--rw-rw-rw-   0        0        0     7023 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/astro.py
--rw-rw-rw-   0        0        0     7339 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/constituent.py
--rw-rw-rw-   0        0        0     4695 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/nodal_corrections.py
--rw-rw-rw-   0        0        0    14984 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/tide.py
--rw-rw-rw-   0        0        0      965 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tide_predict.py
--rw-rw-rw-   0        0        0    13739 2022-04-02 00:15:41.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/tiling.py
--rw-rw-rw-   0        0        0    18755 2022-04-01 18:13:23.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/xbeach.py
--rw-rw-rw-   0        0        0     2316 2022-04-01 18:13:22.000000 deltares_coastalhazardstoolkit-0.0.8/src/cht/xmlkit.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.879370 deltares-coastalhazardstoolkit-0.2.1/
+-rw-rw-rw-   0        0        0    35823 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      376 2023-08-04 19:06:18.879370 deltares-coastalhazardstoolkit-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-08-04 19:06:03.000000 deltares-coastalhazardstoolkit-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 19:06:18.879370 deltares-coastalhazardstoolkit-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.793242 deltares-coastalhazardstoolkit-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.795243 deltares-coastalhazardstoolkit-0.2.1/src/cht/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.801738 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/__init__.py
+-rw-rw-rw-   0        0        0    26958 2023-06-09 14:37:46.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/bathymetry_database.py
+-rw-rw-rw-   0        0        0    26344 2023-01-03 18:41:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling.py
+-rw-rw-rw-   0        0        0      803 2022-11-09 17:01:21.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling_example.py
+-rw-rw-rw-   0        0        0     1324 2023-01-03 19:45:23.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling_example_gebco22.py
+-rw-rw-rw-   0        0        0     1645 2023-06-05 18:25:14.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.803067 deltares-coastalhazardstoolkit-0.2.1/src/cht/beware/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/beware/__init__.py
+-rw-rw-rw-   0        0        0    38019 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/beware/beware.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.804348 deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/__init__.py
+-rw-rw-rw-   0        0        0    45459 2023-02-18 18:54:56.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/delft3dfm.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.812360 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-02-16 02:20:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/bathymetry.py
+-rw-rw-rw-   0        0        0    17214 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/boundary_conditions.py
+-rw-rw-rw-   0        0        0    18023 2023-06-09 15:38:31.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/grid.py
+-rw-rw-rw-   0        0        0    31446 2023-06-07 17:46:39.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave.py
+-rw-rw-rw-   0        0        0     4763 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave_builder.py
+-rw-rw-rw-   0        0        0     6804 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave_domain.py
+-rw-rw-rw-   0        0        0     5288 2023-05-15 15:51:19.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/input.py
+-rw-rw-rw-   0        0        0     5454 2023-02-16 02:34:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/mask.py
+-rw-rw-rw-   0        0        0     7393 2023-05-19 15:46:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/observation_points.py
+-rw-rw-rw-   0        0        0     4004 2023-05-22 15:09:37.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/to_xugrid.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.820358 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/__init__.py
+-rw-rw-rw-   0        0        0    11578 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_analysis.py
+-rw-rw-rw-   0        0        0    26632 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_forecast.py
+-rw-rw-rw-   0        0        0    23025 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_hindcast.py
+-rw-rw-rw-   0        0        0     4688 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_ufl_d01.py
+-rw-rw-rw-   0        0        0    12331 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50.py
+-rw-rw-rw-   0        0        0     9220 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_02.py
+-rw-rw-rw-   0        0        0    14130 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_03.py
+-rw-rw-rw-   0        0        0    15644 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_04.py
+-rw-rw-rw-   0        0        0     6399 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25.py
+-rw-rw-rw-   0        0        0     4146 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25_02.py
+-rw-rw-rw-   0        0        0    58037 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/meteo.py
+-rw-rw-rw-   0        0        0     2074 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/test_coamps.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.827229 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/__init__.py
+-rw-rw-rw-   0        0        0     9328 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/deltares_ini.py
+-rw-rw-rw-   0        0        0     3138 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/fileops.py
+-rw-rw-rw-   0        0        0     4434 2023-02-16 02:05:36.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/geometry.py
+-rw-rw-rw-   0        0        0     2901 2023-02-12 05:38:17.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/misc_tools.py
+-rw-rw-rw-   0        0        0     4440 2023-06-07 20:21:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/pli_file.py
+-rw-rw-rw-   0        0        0     3833 2023-08-04 18:05:53.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/prob_maps.py
+-rw-rw-rw-   0        0        0     6472 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/sftp.py
+-rw-rw-rw-   0        0        0     9845 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/tekal.py
+-rw-rw-rw-   0        0        0     5317 2023-05-17 17:18:05.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/xmlkit.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.828706 deltares-coastalhazardstoolkit-0.2.1/src/cht/model_builder/
+-rw-rw-rw-   0        0        0    22934 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/model_builder/model_builder.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.830942 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/__init__.py
+-rw-rw-rw-   0        0        0     7791 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nest1.py
+-rw-rw-rw-   0        0        0    33815 2023-07-28 19:48:45.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nest2.py
+-rw-rw-rw-   0        0        0    37037 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nesting.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.834309 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/
+-rw-rw-rw-   0        0        0       92 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/__init__.py
+-rw-rw-rw-   0        0        0      993 2023-05-17 17:26:56.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/_ndbc.py
+-rw-rw-rw-   0        0        0     1127 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/_noaa_coops.py
+-rw-rw-rw-   0        0        0     1181 2023-05-17 17:33:01.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/observation_stations.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.837309 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/__init__.py
+-rw-rw-rw-   0        0        0      590 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/deshoal.py
+-rw-rw-rw-   0        0        0     1238 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/disper.py
+-rw-rw-rw-   0        0        0     7860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/vo21.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.841538 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/__init__.py
+-rw-rw-rw-   0        0        0    66271 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/quadtree.py
+-rw-rw-rw-   0        0        0    11167 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/regulargrid.py
+-rw-rw-rw-   0        0        0    46392 2023-07-25 20:52:10.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/sfincs.py
+-rw-rw-rw-   0        0        0    12920 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/sfincs_builder.py
+-rw-rw-rw-   0        0        0    48185 2023-01-05 19:25:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/subgrid.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.851369 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/
+-rw-rw-rw-   0        0        0       92 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/__init__.py
+-rw-rw-rw-   0        0        0    12996 2023-06-14 15:50:17.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/boundary_conditions.py
+-rw-rw-rw-   0        0        0    46524 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/grid.py
+-rw-rw-rw-   0        0        0     8587 2023-06-07 20:03:21.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/input.py
+-rw-rw-rw-   0        0        0    22639 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/mask.py
+-rw-rw-rw-   0        0        0     3308 2023-05-27 14:29:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/observation_points.py
+-rw-rw-rw-   0        0        0    78823 2023-06-01 20:37:42.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/quadtree_grid.py
+-rw-rw-rw-   0        0        0    25105 2023-06-02 21:09:28.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/quadtree_grid_snapwave.py
+-rw-rw-rw-   0        0        0    18022 2023-05-25 16:37:22.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/regular_grid.py
+-rw-rw-rw-   0        0        0    46298 2023-06-14 14:43:07.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/sfincs.py
+-rw-rw-rw-   0        0        0    11719 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/sfincs_builder.py
+-rw-rw-rw-   0        0        0    20663 2023-06-08 11:04:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/snapwave.py
+-rw-rw-rw-   0        0        0    46524 2023-06-14 15:18:38.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/subgrid.py
+-rw-rw-rw-   0        0        0     1707 2023-06-07 20:14:52.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/wave_makers.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.852369 deltares-coastalhazardstoolkit-0.2.1/src/cht/snapwave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/snapwave/__init__.py
+-rw-rw-rw-   0        0        0    24908 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/snapwave/mesh.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.859369 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/__init__.py
+-rw-rw-rw-   0        0        0     7255 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/astro.py
+-rw-rw-rw-   0        0        0     7524 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/constituent.py
+-rw-rw-rw-   0        0        0     3542 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/fes2014.py
+-rw-rw-rw-   0        0        0     4860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/nodal_corrections.py
+-rw-rw-rw-   0        0        0     1479 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/predict.py
+-rw-rw-rw-   0        0        0      687 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/test_tide_database.py
+-rw-rw-rw-   0        0        0    15388 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide.py
+-rw-rw-rw-   0        0        0     3365 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide_model.py
+-rw-rw-rw-   0        0        0      965 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide_predict.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.860370 deltares-coastalhazardstoolkit-0.2.1/src/cht/tiling/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tiling/__init__.py
+-rw-rw-rw-   0        0        0    32567 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tiling/tiling.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.864370 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/
+-rw-rw-rw-   0        0        0    10203 2023-05-17 12:40:56.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/cyclone_track_database.py
+-rw-rw-rw-   0        0        0     2406 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/test_meteo.py
+-rw-rw-rw-   0        0        0      480 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/test_track.py
+-rw-rw-rw-   0        0        0     1517 2023-01-25 14:41:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/testje.py
+-rw-rw-rw-   0        0        0     1091 2023-01-25 14:41:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/testje_forecasting.py
+-rw-rw-rw-   0        0        0   102706 2023-07-29 20:44:35.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/tropical_cyclone.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.866370 deltares-coastalhazardstoolkit-0.2.1/src/cht/watersheds/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/watersheds/__init__.py
+-rw-rw-rw-   0        0        0     7923 2022-11-10 16:13:06.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/watersheds/watersheds.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.867370 deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/__init__.py
+-rw-rw-rw-   0        0        0    28049 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/xbeach.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.878377 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/top_level.txt
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/bathymetry_database.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/bathymetry_database.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 
 import os
 import xml.etree.ElementTree as ET
 import numpy as np
 import math
 import urllib
 import netCDF4 as nc
-
-from .coordinate_systems import CS
+import yaml
+from shutil import copyfile
+from pyproj import CRS
+from pyproj import Transformer
+from cht.misc.misc_tools import interp2
 
 class ZoomLevel:
 
     def __init__(self):
         
         self.dx = 0.0
         self.dy = 0.0
@@ -29,47 +32,57 @@
     The main Bathymetry Database class
     
     :param pth: Path name where bathymetry tiles will be cached.
     :type pth: string            
     """
     
     def __init__(self, pth):
-        
-        self.path    = pth
-        self.dataset = []
-        self.read()
+        if pth:
+            self.path    = pth
+            self.dataset = []
+            self.read()
+            self.initialized = True
+        else:
+            self.initialized = False
+    
+    def initialize(self, pth):
+        if not self.initialized:
+            self.path    = pth
+            self.dataset = []
+            self.read()
+        self.initialized = True
        
     def read(self):
         """
         Reads meta-data of all datasets in the database. 
         """
         
         # Read in database
         xml_file = os.path.join(self.path, "bathymetry.xml")
         xml_root = ET.parse(xml_file).getroot()
 
         for xml_dataset in xml_root.findall('dataset'):
             
             try:
 
-                dataset = BathymetryDataset()
-                
+                dataset = BathymetryDataset(self)
+
                 # Set attributes
                 for prop in xml_dataset:
                     setattr(dataset, prop.tag.lower(), prop.text)
-                
+                    
                 dataset.local_path = os.path.join(self.path, dataset.name)
     
                 # Read metadata for this dataset from separate xml file
                 dataset.read()
                 
                 self.dataset.append(dataset)
             
             except:
-                print("Could not read dataset " + dataset.name +". Need to fix this by downloading dataset xml.")
+                print("Could not read dataset " + dataset.name +". You as user need to fix this by downloading/creating the dataset xml for this dataset. See src/msc/matlab/gebco19.xml and src/msc/matlab/mkbathyxml.m")
                 pass
         
     def get_data(self, dataset_name, xlim, ylim, max_cell_size):
         """
         Returns imported data from database 
         
         :param dataset_name: Name of requested bathymetry dataset.
@@ -105,122 +118,206 @@
         :rtype: str
         """
         
         # Read in data from database
         # Find corresponding dataset dataset
         for d in self.dataset:
             if d.name == dataset_name:
-                return d.crs.epsg
+                return d.crs
 
-    # def get_data_on_array(self, dataset_name, xarr, yarr, crs):
-        
-    #     # Get data interpolated onto array xarr, yarr
-        
-    #     zarr = 0.0
-        
-    #     return zarr
-    
-    def get_sources(self):
+    def get_bathymetry_on_points(self, xz, yz, dxmin, crs, bathymetry_list, method="linear"):
+        zz = self.get_bathymetry_on_grid(xz, yz, crs, bathymetry_list, method=method, coords="points", dxmin=dxmin)
+        return zz
+
+    def get_bathymetry_on_grid(self, xz, yz, crs, bathymetry_list, method="linear", coords="grid", dxmin=1.0e6):
+
+        if xz.ndim == 2:
+            # xy and yz are a grid
+            zz = np.full(xz.shape, np.nan)
+            dx = np.sqrt((xz[0,1] - xz[0,0])**2 + (yz[0,1] - yz[0,0])**2)
+            dy = np.sqrt((xz[1,0] - xz[0,0])**2 + (yz[1,0] - yz[0,0])**2)
+        else:
+            if coords == "grid":
+                zz = np.full((len(yz), len(xz)), np.nan)
+                dx = xz[1] - xz[0]
+                dy = yz[1] - yz[0]
+                xz, yz = np.meshgrid(xz, yz)
+            else:    
+                zz = np.full(xz.shape, np.nan)
+
+        # Determine resolution to get bathy data
+        if coords == "grid":
+            # Resolution follow from grid
+            if crs.is_geographic:
+                dx = min(111111.0 * dx,
+                        111111.0 * dy * np.cos(np.pi * np.max(np.abs(yz)) / 180.0))
+            else:
+                dx = min(dx, dy)
+        else:
+            dx = dxmin        
 
-        sources      = []
+        # Loop through bathymetry datasets
+        for ibathy, bathymetry in enumerate(bathymetry_list):
+            dataset = bathymetry["dataset"]
+            zmin    = bathymetry["zmin"]
+            zmax    = bathymetry["zmax"]
+            transformer = Transformer.from_crs(crs,
+                                               dataset.crs,
+                                               always_xy=True)
+            if np.isnan(zz).any():
+                xzb, yzb = transformer.transform(xz, yz)
+                xmin = np.nanmin(np.nanmin(xzb))
+                xmax = np.nanmax(np.nanmax(xzb))
+                ymin = np.nanmin(np.nanmin(yzb))
+                ymax = np.nanmax(np.nanmax(yzb))
+                ddx = 0.05 * (xmax - xmin)
+                ddy = 0.05 * (ymax - ymin)
+                xl = [xmin - ddx, xmax + ddx]
+                yl = [ymin - ddy, ymax + ddy]
+                # Get DEM data (ddb format for now)
+                xb, yb, zb = bathymetry_database.get_data(dataset.name,
+                                                          xl,
+                                                          yl,
+                                                          max_cell_size=dx)
+                zb[np.where(zb < zmin)] = np.nan
+                zb[np.where(zb > zmax)] = np.nan
+                if not np.isnan(zb).all():
+                    zz1 = interp2(xb, yb, zb, xzb, yzb, method=method)
+                    isn = np.where(np.isnan(zz))
+                    zz[isn] = zz1[isn]
+
+        return zz
+
+    def get_dataset(self, name):
+        for dataset in self.dataset:
+            if dataset.name == name:
+                return dataset
+        return None
+
+    def dataset_names(self, source=None):
+        short_name_list = []
+        long_name_list = []
+        source_name_list = []
+        for dataset in self.dataset:
+            ok = False
+            if source:
+                if dataset.source == source:
+                    ok = True
+            else:
+                ok = True
+            if ok:
+                short_name_list.append(dataset.name)
+                long_name_list.append(dataset.long_name)
+                source_name_list.append(dataset.source)
+        return short_name_list, long_name_list, source_name_list
+
+    def sources(self):
+
+        sources = []
         source_names = []
-        
+
         for dataset in self.dataset:
-                       
-            source    = dataset.source
-            
+            source = dataset.source
             if source in source_names:
                 # Existing source
                 for src in sources:
                     if src.name == source:
-                        src.dataset.append(dataset)                
-                        break
+                        src.dataset.append(dataset)
             else:
                 # New source
                 src = BathymetrySource(source)
-                src.dataset.append(dataset)                
+                src.dataset.append(dataset)
                 sources.append(src)
                 source_names.append(source)
-        
-        return sources
+
+        return source_names, sources
+
 
 class BathymetryDataset:
     """
     Bathymetry dataset class 
 
     :ivar name: initial value: ''
     :ivar nr_zoom_levels: initial value: 0
     """
 
-    def __init__(self):
+    def __init__(self, database):
         
+        self.database          = database
         self.name              = ''
         self.long_name         = ''
         self.source            = ''
         self.data_format       = '' # netcdftiles, geotiff, etc
         self.nr_zoom_levels    = 0
         self.zoom_level        = []
         self.coordinate_system = []
         self.use_cache         = True
         self.remote_path       = ''
         self.local_path        = ''
+        self.vertical_units    = 'm'
         self.vertical_reference_level_name = 'MSL'
         self.vertical_reference_level_difference_with_MSL = 0.0
 
     def read(self):
         
-        xml_file = os.path.join(self.local_path, self.name + ".xml")
-
-        xml_root = ET.parse(xml_file).getroot()
-
-        # Set attributes
-        for prop in xml_root:
-            setattr(self, prop.tag.lower(), prop.text)
-        self.nr_zoom_levels = int(self.nr_zoom_levels)    
-        self.x0             = float(self.x0)
-        self.y0             = float(self.y0)
-        self.dx             = float(self.dx)
-        self.dy             = float(self.dy)
-        self.nr_tiles_x     = int(self.nr_tiles_x)
-        self.nr_tiles_y     = int(self.nr_tiles_y)
-        self.pixels_in_tile = int(self.pixels_in_tile)
-        if self.coord_ref_sys_kind[0:3] == "geo":
-            self.coord_ref_sys_kind = "geographic"
+        if self.type.lower() == "netcdf_tiles_v2":
+            yml_file = os.path.join(self.local_path, self.name + ".yml")
+            yml = yaml2dict(yml_file)
+            for key in yml:
+                setattr(self, key, yml[key])
+            nc_file = os.path.join(self.local_path, self.name + ".nc")
+            ds   = nc.Dataset(nc_file)
+            dcrs = ds["crs"]
+            self.pixels_in_tile           = ds['tile_size_x'][0]
+            self.nr_zoom_levels           = ds.dimensions['zoom_levels'].size
+            for izoom in range(self.nr_zoom_levels):
+                zl = ZoomLevel()
+                zl.x0 = ds['x0'][izoom]
+                zl.y0 = ds['y0'][izoom]
+                zl.dx = ds['grid_size_x'][izoom]
+                zl.dy = ds['grid_size_y'][izoom]
+                zl.nr_tiles_x = ds['nr_tiles_x'][izoom]
+                zl.nr_tiles_y = ds['nr_tiles_y'][izoom]
+                self.zoom_level.append(zl)
+
+            
+        elif self.type.lower() == "netcdftiles":
+            # Read in dimensions from netcdf file
+            nc_file = os.path.join(self.local_path, self.name + ".nc")
+            ds   = nc.Dataset(nc_file)
+            dcrs = ds["crs"]
+            self.coord_ref_sys_name       = dcrs.getncattr('coord_ref_sys_name')
+            self.coord_ref_sys_kind       = dcrs.getncattr('coord_ref_sys_kind')
+            self.vertical_reference_level = dcrs.getncattr('vertical_reference_level')
+#            self.vertical_units           = dcrs.getncattr('vertical_units')
+            self.difference_with_msl      = dcrs.getncattr('difference_with_msl')
+            self.pixels_in_tile           = ds['nx'][0]
+            self.nr_zoom_levels           = ds.dimensions['zoomlevels'].size
+            for izoom in range(self.nr_zoom_levels):
+                zl = ZoomLevel()
+                zl.x0 = ds['x0'][izoom]
+                zl.y0 = ds['y0'][izoom]
+                zl.dx = ds['grid_size_x'][izoom]
+                zl.dy = ds['grid_size_y'][izoom]
+                zl.nr_tiles_x = ds['ntilesx'][izoom]
+                zl.nr_tiles_y = ds['ntilesy'][izoom]
+                self.zoom_level.append(zl)
         
-        self.crs = CS(self.coord_ref_sys_name, self.coord_ref_sys_kind)
-
-                
-        dx = self.dx
-        dy = self.dy
-        nnx = self.nr_tiles_x
-        nny = self.nr_tiles_y
-        for izoom in range(self.nr_zoom_levels):
-            zl = ZoomLevel()
-            zl.x0 = self.x0
-            zl.y0 = self.y0
-            zl.dx = dx
-            zl.dy = dy
-            zl.nr_tiles_x = nnx
-            zl.nr_tiles_y = nny
-            self.zoom_level.append(zl)
-            dx  = dx*2
-            dy  = dy*2
-            nnx = math.ceil(nnx/2)
-            nny = math.ceil(nny/2)
+        self.crs            = CRS(self.coord_ref_sys_name)
             
     def get_data(self, xlim, ylim, max_cell_size):
         """
         Reads data from database. Returns x, y, z 
         """
         
         x=0.0
         y=0.0
         z=0.0
         
-        if self.type.lower() == 'netcdftiles':
+        if self.type.lower() == 'netcdftiles' or self.type.lower() == 'netcdf_tiles_v2':
             x, y, z = self.read_data_from_netcdf_tiles(xlim, ylim, 0, max_cell_size)
         elif self.type == 'geotiff':
             x = 1.0    
 
         return x,y,z
         
     def read_data_from_netcdf_tiles(self, xl, yl, izoom, max_cell_size):
@@ -242,15 +339,15 @@
             cell_size_x = np.append(cell_size_x, zl.dx)
             cell_size_y = np.append(cell_size_y, zl.dy)
 
             # Should multiply with unit here...
         
         if izoom == 0:
             # Find zoom level based on resolution
-            if self.coord_ref_sys_kind == 'geographic':
+            if self.crs.is_geographic:
                 cell_size_x = cell_size_x*111111
                 cell_size_y = cell_size_y*111111
             # Find first level with cell size greater than max cell size    
             ilev1 = find_last(cell_size_x<=max_cell_size)
             if ilev1 == None:
                 # All levels have cell sizes smaller than max cell size
                 ilev1 = 0
@@ -262,51 +359,71 @@
             ilev2 = self.nr_zoom_levels
         else:
             ilev1 = izoom
             ilev2 = izoom
         
         for ilev in range(ilev1,ilev2+1):
             
-            x0  = self.zoom_level[ilev].x0   # lower-left corner x
-            y0  = self.zoom_level[ilev].y0   # lower-left corner y
-            dx  = self.zoom_level[ilev].dx   # cell size x
-            dy  = self.zoom_level[ilev].dy   # cell size y
+            x0  = float(self.zoom_level[ilev].x0)   # lower-left corner x
+            y0  = float(self.zoom_level[ilev].y0)   # lower-left corner y
+            dx  = float(self.zoom_level[ilev].dx)   # cell size x
+            dy  = float(self.zoom_level[ilev].dy)   # cell size y
             nx  = self.pixels_in_tile        # number of pixels in tile x
-            ny  = self.pixels_in_tile        # number of pixels in tile y
+            if self.name == "rws_vaklodingen":
+                ny = 625
+            else:
+                ny  = self.pixels_in_tile        # number of pixels in tile y
             nnx = self.zoom_level[ilev].nr_tiles_x  # number of tiles x
             nny = self.zoom_level[ilev].nr_tiles_y  # number of tiles y
-            iav = self.zoom_level[ilev].i_available
-            jav = self.zoom_level[ilev].j_available
-            
-            # Read i_available and j_available (if they have not yet been read)
-#            if not iav:
-            if not np.any(iav):
-                ncfile = os.path.join(self.local_path, self.name + ".nc")
-                ds  = nc.Dataset(ncfile)
-                iav = ds["iavailable" + str(ilev + 1)][:].data - 1
-                jav = ds["javailable" + str(ilev + 1)][:].data - 1
-                self.zoom_level[ilev].i_available = iav
-                self.zoom_level[ilev].j_available = jav
+
+            if self.type == "netcdf_tiles_v2":
+                iav = self.zoom_level[ilev].i_available                
+                if not np.any(iav):
+                    ncfile = os.path.join(self.local_path, self.name + ".nc")
+                    ds  = nc.Dataset(ncfile)
+                    iav = ds["available_zl" + str(ilev + 1).zfill(2)][:].data
+                    self.zoom_level[ilev].i_available = iav
+
+            else:    
+
+
+                iav = self.zoom_level[ilev].i_available
+                jav = self.zoom_level[ilev].j_available
+                
+                # Read i_available and j_available (if they have not yet been read)
+    #            if not iav:
+                if not np.any(iav):
+                    ncfile = os.path.join(self.local_path, self.name + ".nc")
+                    ds  = nc.Dataset(ncfile)
+                    iav = ds["iavailable" + str(ilev + 1)][:].data - 1
+                    jav = ds["javailable" + str(ilev + 1)][:].data - 1
+                    self.zoom_level[ilev].i_available = iav
+                    self.zoom_level[ilev].j_available = jav
 
 #            vert_unit = self.vertical_coordinate_system.unit
             
             tile_size_x = dx*nx
             tile_size_y = dy*ny
             
              # Directories and names
             name   = self.name;
             levdir = 'zl' + str(ilev + 1).zfill(2)
             
             iopendap = False
+            ipdrive = False
 
             if self.url[0:4] == 'http':
                 # Tiles stored on OpenDAP server
                 iopendap  = True
                 remotedir = self.url + '/' + levdir + '/'
                 localdir  = os.path.join(self.local_path, levdir)
+            elif self.url[0:2].lower() == 'p:':
+                ipdrive = True
+                remotedir = self.url + '\\' + levdir + '\\'
+                localdir  = os.path.join(self.local_path, levdir)
             else:
                 # Tiles are stored locally
                 localdir  = os.path.join(self.local_path, levdir)
                 remotedir = localdir
                 
             # Tiles
             # Array with x and y origin of available tiles
@@ -349,27 +466,30 @@
 
             # Indices of tiles to be loaded
             tiles_index_x = all_tiles_index_x[ix1:ix2 + 1]
             tiles_index_y = all_tiles_index_y[iy1:iy2 + 1]
             # Origins of tiles to be loaded
             tiles_x0 = all_tiles_x0[ix1:ix2 + 1]
             tiles_y0 = all_tiles_y0[iy1:iy2 + 1]
+            tiles_x1 = tiles_x0 + tile_size_x
+            npixx = int(np.round((tiles_x1[-1] - tiles_x0[0])/dx))
 
             if not just_get_tiles:
                 # Mesh of horizontal coordinates
                 # x = np.arange(tiles_x0[0],
                 #                tiles_x0[-1] + tile_size_x, dx)
                 # y = np.arange(tiles_y0[0],
                 #                tiles_y0[-1] + tile_size_y, dy)
 
-                x = np.linspace(tiles_x0[0], tiles_x0[-1] + tile_size_x - dx, num=nnnx*nx)
+                x = np.linspace(tiles_x0[0], tiles_x0[0] + (npixx - 1) * dx, num=npixx)
+#                x = np.linspace(tiles_x0[0], tiles_x0[-1] + tile_size_x - dx, num=nnnx*nx)
                 y = np.linspace(tiles_y0[0], tiles_y0[-1] + tile_size_y - dy, num=nnny*ny)
 
                 # Allocate z
-                z = np.empty((nnny*ny,nnnx*nx))
+                z = np.empty((nnny*ny, npixx))
                 z[:] = np.nan
 
             # Start indices for each tile in larger matrix
             istartx = []
             for i in range(nnnx):
                 iii1 = find_first(abs(x - tiles_x0[i]) == min(abs(x - tiles_x0[i])))
                 istartx.append(iii1)
@@ -386,47 +506,37 @@
                 itile = tiles_index_x[i]
                 
                 for j in range(nnny):
 
                     jtile = tiles_index_y[j]
     
                     tilen = tilen + 1
-                     
-#                     # # Waitbar
-#                     # if not quiet:
-#                     #     if justgettiles
-#                     #         str=['Getting bathymetry level ' num2str(ilev) ' of ' num2str(nLevels) ' - tile ' num2str(tilen) ' of ' ...
-#                     #             num2str(ntiles) ' ...'];
-#                     #     else
-#                     #         str=['Getting bathymetry - tile ' num2str(tilen) ' of ' ...
-#                     #             num2str(ntiles) ' ...'];
-#                     #     end
-#                     #     if verLessThan('matlab', '8.4')
-#                     #         [hh,abort2]=awaitbar(tilen/ntiles,wb,str);
-#                     #     else
-#                     #         [hh,abort2]=awaitbar(tilen/ntiles,get(wb,'Number'),str);
-#                     #     end
-#                     #     if abort2 % Abort the process by clicking abort button
-#                     #         break;
-#                     #     end;
-#                     #     if isempty(hh); % Break the process when closing the figure
-#                     #         break;
-#                     #     end;
-#                     # end
 
                     zzz = np.empty((ny,nx)) # make empty tile
                     zzz[:] = np.nan
 
                     # First check whether required file exists at at all
-                    both_ok = (iav == itile) * (jav == jtile)
 
-                    if both_ok.any():
+                    file_name = name + '.' + levdir + '.' + str(itile + 1).zfill(5) + '.' + str(jtile + 1).zfill(5) + '.nc'
 
-                        file_name = name + '.' + levdir + '.' + str(itile + 1).zfill(5) + '.' + str(jtile + 1).zfill(5) + '.nc'
-                        full_file_name = os.path.join(localdir, file_name)
+                    tile_exists = False
+                    if self.type == "netcdf_tiles_v2":
+                        if iav[jtile, itile] == 1:
+                            tile_exists = True
+                            idirname = os.path.join(localdir, str(itile + 1).zfill(5))
+                            full_file_name = os.path.join(idirname, file_name)
+                            var_str = "value"
+                    else:      
+                        both_ok = (iav == itile) * (jav == jtile)
+                        if both_ok.any():
+                            tile_exists = True
+                            full_file_name = os.path.join(localdir, file_name)
+                            var_str = "depth"
+
+                    if tile_exists:
     
                         if iopendap:
                             if self.use_cache:
                                 # First check if file is available locally
                                 idownload = False
                                 if not os.path.exists(full_file_name):
                                     # File not available locally
@@ -454,26 +564,52 @@
     
                                 ncfile = full_file_name # name of local netcdf file
     
                             else:
     
                                 # Don't use cache
                                 ncfile = remotedir + file_name
+                                
+                        elif ipdrive:
+                            if self.use_cache:
+                                # First check if file is available locally
+                                icopy = False
+                                if not os.path.exists(full_file_name):
+                                    # File not available locally
+                                    icopy = True
     
+                                if icopy:
+                                    # Make localdir if it does not yet exist
+                                    if not os.path.exists(localdir):
+                                        os.mkdir(localdir)
+                                    # Download file    
+                                    try:
+                                        copyfile(os.path.join(remotedir,file_name),
+                                                                       full_file_name)
+                                    except:
+                                        print('Could not copy tile ...')
+    
+                                ncfile = full_file_name # name of local netcdf file
+    
+                            else:
+    
+                                # Don't use cache
+                                ncfile = remotedir + file_name
+
                         else:
     
                             ncfile = full_file_name
                             
 #                        print(ncfile)    
                         if not just_get_tiles:
                             
                             # Read the data in the tile
                             if os.path.exists(ncfile):
                                 ds  = nc.Dataset(ncfile)
-                                zzz = ds["depth"][:]
+                                zzz = ds[var_str][:]
     #                            fill_value = nc_attget(ncfile, 'depth', 'fill_value')
                         
                             # Now stick the tile data in the large array
 
                             i1 = istartx[i]
                             i2 = istartx[i] + nx
 
@@ -513,15 +649,15 @@
                 
                 data_in_cell_centres = True
 
                 if data_in_cell_centres:
                     x = x + 0.5*dx # This really should be added as the data are defined in the cell centres!!!               
                     y = y + 0.5*dy
                 
-                z = z[iy1:iy2,ix1:ix2]
+                z = z[iy1:iy2, ix1:ix2]
                 
                 # Convert to metres
                 if self.vertical_units == 'cm':
                     z = z*0.01
                 elif self.vertical_units == 'ft':
                     z = z*0.3048
 
@@ -543,7 +679,21 @@
 
 class BathymetrySource:
     
     def __init__(self, name):
         
         self.name    = name
         self.dataset = []
+
+def dict2yaml(file_name, dct, sort_keys=False):
+    yaml_string = yaml.dump(dct, sort_keys=sort_keys)    
+    file = open(file_name, "w")  
+    file.write(yaml_string)
+    file.close()
+
+def yaml2dict(file_name):
+    file = open(file_name,"r")
+    dct = yaml.load(file, Loader=yaml.FullLoader)
+    return dct
+
+
+bathymetry_database = BathymetryDatabase(None)
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/delft3dfm.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/delft3dfm.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 #from matplotlib import pyplot as plt
 from pandas.tseries.offsets import DateOffset
 
 import math
 from pyproj import CRS
 from pyproj import Transformer
 
-from cht.geometry import RegularGrid
-from cht.geometry import Point
-from cht.deltares_ini import IniStruct
+from cht.misc.geometry import RegularGrid
+from cht.misc.geometry import Point
+from cht.misc.deltares_ini import IniStruct
 
 class Delft3DFM:
     
     def __init__(self, input_file=None, crs=None):
  
 #        self.epsg                     = epsg
         self.mdu                      = MDU()
@@ -398,15 +398,16 @@
         
             
     ### Output ###
 
     def read_timeseries_output(self,
                                name_list = None,
                                path=None,
-                               file_name = None):
+                               file_name = None,
+                               file_name_wave = None):
 
         import xarray as xr
         import pandas as pd
         import numpy as np
 
         # Returns a dataframe with timeseries    
         
@@ -426,35 +427,62 @@
         ddd = xr.open_dataset(file_name)
         stations=ddd.waterlevel.coords["station_name"].values
         all_stations = []
         for ist, st in enumerate(stations):
             st=str(st)[2:-1]
             all_stations.append(st)
         
-        times   = ddd.waterlevel.coords["time"].values
-
         # If name_list is empty, add all points    
         if not name_list:
             name_list = []
             for st in all_stations:
-                name_list.append(st)
-        
-        df = pd.DataFrame(index=times, columns=name_list)
+                name_list.append(st)      
         
-        for station in name_list:
-            for ist, st in enumerate(all_stations):
-                if station == st:
-                    wl = ddd.waterlevel.values[:,ist]
-                    wl[np.isnan(wl)] = -999.0
-                    df[st]=wl
-                    break            
+        if not file_name_wave:
+            times   = ddd.waterlevel.coords["time"].values
+            df = pd.DataFrame(index=times, columns=name_list)
+
+            for station in name_list:
+                for ist, st in enumerate(all_stations):
+                    if station == st:
+                        wl = ddd.waterlevel.values[:,ist]
+                        wl[np.isnan(wl)] = -999.0
+                        df[st]=wl
+                        break            
 
-        ddd.close()
-        
-        return df    
+            ddd.close()
+        else:
+            ddd.close()
+            ddd={}
+            for i,v in enumerate(file_name_wave):
+                file_name = os.path.join(path, v)
+                ddd[i] = xr.open_dataset(file_name)
+            
+            times   = ddd[0].Hsig.coords["time"].values
+            
+            df={}
+            for station in name_list:
+                for ist, st in enumerate(all_stations):
+                    if station == st:
+
+                        df[st] = pd.DataFrame(index=times, columns=["hs", "tp"])
+                        for i,v in enumerate(file_name_wave): # Loop to get most detailed model with output at station location
+                            Hs = ddd[i].Hsig.values[:,ist]
+                            Tp = ddd[i].RTpeak.values[:,ist]
+                            if max(Hs)>-999:
+                                break
+                        Tp[np.isnan(Hs)] = -999.0
+                        Hs[np.isnan(Hs)] = -999.0
+                        df[st]["hs"]=Hs
+                        df[st]["tp"]=Tp                       
+                        break    
+            for i,v in enumerate(file_name_wave):        
+                ddd[i].close()
+
+        return df     
 
     def grid_coordinates(self, loc='cor'):
 
         cosrot = math.cos(self.input.rotation*math.pi/180)
         sinrot = math.sin(self.input.rotation*math.pi/180)
         if loc=="cor":
             xx     = np.linspace(0.0,
@@ -666,23 +694,25 @@
         self.geometry     = []
         self.point        = []
         
     def read_location_file(self, path=""):
         loc_file = os.path.join(path,
                                 self.locationfile)
 
-        from cht.pli_file import PliFile as plifile
-        d = plifile(loc_file).read()
+        from cht.misc.pli_file import read_pli_file
+        d = read_pli_file(loc_file)
+#        d = plifile(loc_file)
         name0 = os.path.split(loc_file)[-1][0:-4]
-        for ip, pnt in enumerate(d.point):
-            name = name0 + "_" + str(ip + 1).zfill(4)
-            point = Delft3DFMBoundaryPoint(x=pnt.x,
-                                           y=pnt.y,
-                                           name=name)            
-            self.point.append(point)
+        for polyline in d:
+            for ip, x in enumerate(polyline.x):
+                name = name0 + "_" + str(ip + 1).zfill(4)
+                point = Delft3DFMBoundaryPoint(x=polyline.x[ip],
+                                               y=polyline.y[ip],
+                                               name=name)            
+                self.point.append(point)
         
     def read_forcing_file(self, path=""):
 
         frc_file = os.path.join(path,
                                 self.forcingfile)
         
         if os.path.exists(frc_file):
@@ -806,39 +836,54 @@
         self.dict.append({"name":"profdeffile",          "keyword":"ProfdefFile",      "type":"str",   "default":None,            "group":"geometry", "comment":"*_profdefinition.def) definition for all profile nrs"})
         self.dict.append({"name":"manholefile",          "keyword":"ManholeFile",      "type":"str",   "default":None,            "group":"geometry", "comment":None})
         self.dict.append({"name":"waterlevini",          "keyword":"WaterLevIni",      "type":"float", "default":0.0,             "group":"geometry", "comment":"Initial water level"})
         self.dict.append({"name":"botlevuni",            "keyword":"BotLevUni",        "type":"float", "default":-5.0,            "group":"geometry", "comment":"Uniform bottom level, (only if Botlevtype>=3, used at missing z values in netfile"})
         self.dict.append({"name":"botlevtype",           "keyword":"BotLevType",       "type":"int",   "default":3,               "group":"geometry", "comment":None})
         self.dict.append({"name":"anglat",               "keyword":"AngLat",           "type":"float", "default":0.0,             "group":"geometry", "comment":"Angle of latitude (deg), 0=no Coriolis"})
         self.dict.append({"name":"conveyance2d",         "keyword":"Conveyance2D",     "type":"int",   "default":3,               "group":"geometry", "comment":"-1:R=HU,0:R=H, 1:R=A/P, 2:K=analytic-1D conv, 3:K=analytic-2D conv"})
+        self.dict.append({"name":"conveyance2d",         "keyword":"Conveyance2D",     "type":"int",   "default":3,               "group":"geometry", "comment":"-1:R=HU,0:R=H, 1:R=A/P, 2:K=analytic-1D conv, 3:K=analytic-2D conv"})
 
         # numerics
         self.dict.append({"name":"cflmax",               "keyword":"CFLMax",           "type":"float", "default":0.7,             "group":"numerics", "comment":"Max. Courant nr."})
         self.dict.append({"name":"cflwavefrac",          "keyword":"CFLWaveFrac",      "type":"float", "default":0.1,             "group":"numerics", "comment":"Wave velocity fraction, total courant vel = u + cflw*wavevelocity"})
         self.dict.append({"name":"advectype",            "keyword":"AdvecType",        "type":"int",   "default":3,               "group":"numerics", "comment":"Adv type, 0=no, 1= Wenneker, qu-udzt, 2=1, q(uio-u), 3=Perot q(uio-u), 4=Perot q(ui-u), 5=Perot q(ui-u) without itself"})
         self.dict.append({"name":"limtypsa",             "keyword":"Limtypsa",         "type":"int",   "default":0,               "group":"numerics", "comment":"Limiter type for salinity transport,           0=no, 1=minmod,2=vanLeer,3=Kooren,4=Monotone Central"})
         self.dict.append({"name":"Hdam",                 "keyword":"Hdam",             "type":"float", "default":0.0,             "group":"numerics", "comment":"Threshold for minimum bottomlevel step at which to apply energy conservation factor i.c. flow contraction"})
+        self.dict.append({"name":"Icgsolver",            "keyword":"Icgsolver",        "type":"float", "default":4.0,             "group":"numerics", "comment":"Solver type (1: sobekGS_OMP, 2: sobekGS_OMPthreadsafe, 3: sobekGS, 4: sobekGS + Saadilud, 5: parallel/global Saad, 6: parallel/Petsc, 7: parallel/GS)"})
+        self.dict.append({"name":"Tlfsmo",               "keyword":"Tlfsmo",           "type":"float", "default":0.0,             "group":"numerics", "comment":"Fourier smoothing time on water level boundaries"})
+        self.dict.append({"name":"Qhrelax",              "keyword":"Qhrelax",          "type":"float", "default":0.0,             "group":"numerics", "comment":"Relaxation on Q-h open boundaries"})
 
         # physics
         self.dict.append({"name":"uniffrictcoef",        "keyword":"UnifFrictCoef",    "type":"float", "default":0.02,            "group":"physics",  "comment":"Uniform friction coefficient, 0=no friction"})
+        self.dict.append({"name":"uniffrictcoef1D",        "keyword":"UnifFrictCoef1D",    "type":"float", "default":0.02,            "group":"physics",  "comment":"Uniform friction coefficient in 1D links, 0=no friction"})
+
         self.dict.append({"name":"uniffricttype",        "keyword":"UnifFrictType",    "type":"int",   "default":1,               "group":"physics",  "comment":"0=Chezy, 1=Manning, 2=White Colebrook, 3=z0 etc"})
         self.dict.append({"name":"vicouv",               "keyword":"Vicouv",           "type":"float", "default":1.0,             "group":"physics",  "comment":"Uniform horizontal eddy viscosity"})
         self.dict.append({"name":"smagorinsky",          "keyword":"Smagorinsky",      "type":"float", "default":0.0,             "group":"physics",  "comment":"Add Smagorinsky horizontal turbulence : vicu = vicu + ( (Smagorinsky*dx)**2)*S, e.g. 0.1"})
         self.dict.append({"name":"elder",                "keyword":"Elder",            "type":"float", "default":0.0,             "group":"physics",  "comment":"Add Elder contribution                : vicu = vicu + Elder*kappa*ustar*H/6),   e.g. 1.0"})
         self.dict.append({"name":"wall_ks",              "keyword":"wall_ks",          "type":"float", "default":0.01,            "group":"physics",  "comment":"Nikuradse roughness for side walls, wall_z0=wall_ks/30"})
-        self.dict.append({"name":"vicoww",               "keyword":"Vicoww",           "type":"float", "default":0.0,             "group":"physics",  "comment":"Uniform vertical eddy viscosity"})
+        self.dict.append({"name":"vicoww",               "keyword":"Vicoww",           "type":"float", "default":1.0e-06,             "group":"physics",  "comment":"Uniform vertical eddy viscosity"})
+        self.dict.append({"name":"dicoww",               "keyword":"Dicoww",           "type":"float", "default":1.0e-06,             "group":"physics",  "comment":"Uniform vertical eddy diffusivity"})
+
         self.dict.append({"name":"tidalforcing",         "keyword":"TidalForcing",     "type":"float", "default":1,               "group":"physics",  "comment":"Tidal forcing (0=no, 1=yes) (only for jsferic == 1)"})
         self.dict.append({"name":"salinity",             "keyword":"Salinity",         "type":"float", "default":0,               "group":"physics",  "comment":"Include salinity, (0=no, 1=yes)"})
+        self.dict.append({"name":"temperature",          "keyword":"Temperature",      "type":"float", "default":0,               "group":"physics",  "comment":"Include temperature (0: no, 1: only transport, 3: excess model of D3D, 5: composite (ocean) model)"})
         self.dict.append({"name":"rhomean",              "keyword":"Rhomean",          "type":"float", "default":1024.0,          "group":"physics",  "comment":"Average water density (kg/m3)"})
+        self.dict.append({"name":"ag",                   "keyword":"Ag",               "type":"float", "default":9.81,            "group":"physics",  "comment":"Gravitational acceleration"})
+        self.dict.append({"name":"stanton",              "keyword":"Stanton",          "type":"float", "default":0.0013,          "group":"physics",  "comment":"Coefficient for convective heat flux"})
+        self.dict.append({"name":"dalton",               "keyword":"Dalton",           "type":"float", "default":0.0013,          "group":"physics",  "comment":"Coefficient for evaporative heat flux"})
+        self.dict.append({"name":"backgroundwatertemperature", "keyword":"Backgroundwatertemperature",  "type":"float", "default":20,          "group":"physics",  "comment":"Background water temperature for eqn. of state"})
+
 
         # wind
         self.dict.append({"name":"icdtyp",               "keyword":"ICdtyp",           "type":"int",   "default":3,               "group":"wind",     "comment":"( ), Cd = const, 2=S&B 2 breakpoints, 3= S&B 3 breakpoints"})
         self.dict.append({"name":"cdbreakpoints",        "keyword":"Cdbreakpoints",    "type":"list",     "default":[1.0e-03,3.1e-03,1.5e-03], "group":"wind",     "comment":"( ),   e.g. 0.00063  0.00723"})
         self.dict.append({"name":"windspeedbreakpoints", "keyword":"Windspeedbreakpoints", "type":"list",  "default":[0.0e+00,2.8e+01,5.0e+01], "group":"wind",     "comment":"(m/s), e.g. 0.0      100.0"})
         self.dict.append({"name":"pavbnd",               "keyword":"PavBnd",           "type":"float", "default":1.013e+05,       "group":"wind",     "comment":"Background pressure (Pa)"})
+        self.dict.append({"name":"rhoair",               "keyword":"Rhoair",           "type":"float", "default":1.2,       "group":"wind",     "comment":"Air density"})
 
         # waves
         self.dict.append({"name":"wavemodelnr",          "keyword":"Wavemodelnr",           "type":"int",   "default":3,               "group":"waves",     "comment":"Wave model nr. (0: none, 1: fetch/depth limited Hurdle-Stive, 2: Young-Verhagen, 3: SWAN)"})
         self.dict.append({"name":"wavenikuradse",        "keyword":"WaveNikuradse",         "type":"float", "default":0.01,            "group":"waves",     "comment":"Wave friction Nikuradse ks c , used in Krone-Swart"})
         self.dict.append({"name":"rouwav",               "keyword":"Rouwav",                "type":"str",   "default":"FR84",          "group":"waves",     "comment":"Friction model for wave induced shear stress"})
         self.dict.append({"name":"gammax",               "keyword":"Gammax",                "type":"float", "default":1.0,             "group":"waves",     "comment":"Maximum wave height/water depth ratio"})
 
@@ -847,14 +892,18 @@
         self.dict.append({"name":"tunit",                "keyword":"Tunit",           "type":"str",   "default":"s",              "group":"time",     "comment":"Time units in MDU (H, M or S)"})
         self.dict.append({"name":"dtuser",               "keyword":"DtUser",          "type":"float", "default":300.0,            "group":"time",     "comment":"User timestep in seconds (interval for external forcing update)"})
         self.dict.append({"name":"dtmax",                "keyword":"DtMax",           "type":"float", "default":300.0,            "group":"time",     "comment":"Max timestep in seconds"})
         self.dict.append({"name":"dtinit",               "keyword":"DtInit",          "type":"float", "default":1.0,              "group":"time",     "comment":"Initial timestep in seconds"})
         self.dict.append({"name":"autotimestep",         "keyword":"AutoTimestep",    "type":"int",   "default":1,                "group":"time",     "comment":"Use CFL timestep limit or not (1/0)"})
         self.dict.append({"name":"tstart",               "keyword":"TStart",          "type":"float", "default":0.0,              "group":"time",     "comment":"Start time w.r.t. RefDate (in TUnit)"})
         self.dict.append({"name":"tstop",                "keyword":"TStop",           "type":"float", "default":86400.0,          "group":"time",     "comment":"Stop time w.r.t. RefDate (in TUnit)"})
+        
+        # restart
+        self.dict.append({"name":"restartfile",          "keyword":"RestartFile",     "type":"str",   "default":None,             "group":"restart",     "comment":"Restart netcdf-file, either *_rst.nc or *_map.nc"})
+        self.dict.append({"name":"restartdatetime",      "keyword":"RestartDateTime", "type":"float", "default":0.0,              "group":"restart",     "comment":"Restart date and time when restarting from *_map.nc [YYYY-MM-DD HH:MM:SS]"})
 
         # external forcing
         self.dict.append({"name":"extforcefile",         "keyword":"ExtForceFile",    "type":"str",   "default":None,             "group":"external forcing",     "comment":"*.ext"})
         self.dict.append({"name":"extforcefilenew",      "keyword":"ExtForceFileNew", "type":"str",   "default":None,             "group":"external forcing",     "comment":"*.ext (new format)"})
 
         # output
         self.dict.append({"name":"obsfile",              "keyword":"ObsFile",         "type":"str",   "default":None,             "group":"output",   "comment":"*.xyn Coords+name of observation stations"})
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/deltares_ini.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/deltares_ini.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/fileops.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/fileops.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,66 +6,91 @@
 """
 
 import glob
 import shutil
 import os
 
 def move_file(src, dst):
-    
     for full_file_name in glob.glob(src):
         src_name = os.path.basename(full_file_name)        
         if os.path.exists(os.path.join(dst, src_name)):
-            os.remove(os.path.join(dst, src_name))
-        shutil.move(full_file_name, dst)
+            # Try removing existing file
+            try:                
+                os.remove(os.path.join(dst, src_name))
+            except:
+                print("Could not remove file " + os.path.join(dst, src_name))
+        try:        
+            shutil.move(full_file_name, dst)
+        except:
+            print("Could not move file " + full_file_name)
+
 
 def copy_file(src, dst):
     
     for full_file_name in glob.glob(src):
         src_name = os.path.basename(full_file_name)        
         if os.path.exists(os.path.join(dst, src_name)):
             os.remove(os.path.join(dst, src_name))
         if os.path.isdir(full_file_name):
             dstf = os.path.join(dst, os.path.basename(full_file_name))
             shutil.copytree(full_file_name, dstf)
         else:    
             shutil.copy(full_file_name, dst)
 
 def delete_file(src):
-    
-    for file_name in glob.glob(src):
-        os.remove(src)
+    if isinstance(src, list):
+        for i,v in enumerate(src):
+            for file_name in glob.glob(v):
+                try:
+                    os.remove(v)
+                except:
+                    print("Could not delete " + v)
+    else:
+        for file_name in glob.glob(src):
+            try:
+                os.remove(src)
+            except:
+                print("Could not delete " + src)
 
 def rm(src):
     
     os.remove(src)
 
 def mkdir(path):
 
     if not os.path.exists(path):
         os.makedirs(path)
 
-def list_files(src):
+def list_files(src, full_path=True):
     
-    file_list = []
-    full_list = glob.glob(src)
-    for item in full_list:
-        if os.path.isfile(item):
-            file_list.append(item)
-
-    return file_list
+    if full_path:
+        file_list = []
+        full_list = glob.glob(src)
+        for it, item in enumerate(full_list):
+            if os.path.isfile(item):
+                file_list.append(item)                
+    else:
+        file_list = os.listdir(src)
+#                file_list.append(os.path.basename(item))
+#                print(it)
+                
+    return sorted(file_list)
 
-def list_folders(src):
+def list_folders(src, basename=False):
     
     folder_list = []
     full_list = glob.glob(src)
     for item in full_list:
         if os.path.isdir(item):
-            folder_list.append(item)
+            if basename:
+                folder_list.append(os.path.basename(item))
+            else:
+                folder_list.append(item)                
 
-    return folder_list
+    return sorted(folder_list)
 
 def delete_folder(src):
     try:
         shutil.rmtree(src, ignore_errors=False, onerror=None)
     except:
         # Folder was probably open in another application
         print("Could not delete folder " + src)
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/hurrywave.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,364 +4,352 @@
 
 @author: ormondt
 """
 import os
 import pandas as pd
 import datetime
 import numpy as np
-from pandas.tseries.offsets import DateOffset
 import xarray as xr
 
 import math
 from pyproj import CRS
 from pyproj import Transformer
 
-from cht.geometry import RegularGrid
-from cht.geometry import Point
-from cht.deltares_ini import IniStruct
+from cht.misc.geometry import RegularGrid
+from cht.misc.geometry import Point
+
+from .input import HurryWaveInput
+from .grid import HurryWaveGrid
+from .mask import HurryWaveMask
+from .bathymetry import HurryWaveBathymetry
+from .boundary_conditions import HurryWaveBoundaryConditions
+from .observation_points import HurryWaveObservationPointsRegular
+from .observation_points import HurryWaveObservationPointsSpectra
+
+#from datetime import datetime
+#import pandas as pd
 
 class HurryWave:
     
-    def __init__(self, input_file=None, crs=None):
-        
-        if not crs:
-            crs = CRS(4326)
- 
-        self.input                    = HurryWaveInput()
-        self.crs                      = crs
-        self.grid                     = None
-        self.mask                     = None
-        self.boundary_point           = []
-        self.observation_point        = []
-        self.obstacle                 = []
-        
-        if input_file:
-            self.path = os.path.dirname(input_file)
-            self.load(input_file)
-
-    def load(self, inputfile):
-        # Reads hurrywave.inp and attribute files
-        self.read_input_file(inputfile)
-        self.read_attribute_files()
-    
-    def read_input_file(self, inputfile):
-        
-        # Reads hurrywave.inp
-        
-        # Get the path of hurrywave.inp
-        self.path = os.path.dirname(inputfile)
-        
-        fid = open(inputfile, 'r')
-        lines = fid.readlines()
-        fid.close()
-        for line in lines:
-            str = line.split("=")
-            if len(str)==1:
-               # Empty line
-               continue
-            name = str[0].strip()
-            val  = str[1].strip()
-            try:
-                # First try to convert to int
-                val = int(val)
-            except ValueError:
-                try:
-                    # Now try to convert to float
-                    val = float(val)
-                except:
-                    pass
-            if name == "tref":
-                val = datetime.datetime.strptime(val.rstrip(), '%Y%m%d %H%M%S')
-            if name == "tstart":
-                val = datetime.datetime.strptime(val.rstrip(), '%Y%m%d %H%M%S')
-            if name == "tstop":
-                val = datetime.datetime.strptime(val.rstrip(), '%Y%m%d %H%M%S')
-            setattr(self.input, name, val)
-
-        if self.input.crs_utmzone:
-            self.crs = CRS("WGS 84 / UTM zone " + self.input.utmzone)
-                        
-    def write_input_file(self, input_file=None):
-
-        if not input_file:
-            input_file = os.path.join(self.path, "hurrywave.inp")
-            
-        fid = open(input_file, "w")
-        for key, value in self.input.__dict__.items():
-            if not value is None:
-                if type(value) == "float":
-                    string = f'{key.ljust(20)} = {float(value)}\n'
-                elif type(value) == "int":
-                    string = f'{key.ljust(20)} = {int(value)}\n'
-                elif isinstance(value, datetime.date):
-                    dstr = value.strftime("%Y%m%d %H%M%S")
-                    string = f'{key.ljust(20)} = {dstr}\n'
-                else:
-                    string = f'{key.ljust(20)} = {value}\n'                
-                fid.write(string)
-        fid.close()    
-                       
-    def read_attribute_files(self):
+    def __init__(self, load=False, crs=None, path=None, exe_path=None):
+        # HurryWave can be initialized in THREE ways
+        # hw = HurryWave() -> path is set to CWD
+        # hw = HurryWave(path="d:\\temp") -> path is set to path
+        # hw = HurryWave(path="d:\\temp", load=True) -> path is set to path, and input file is read
 
-        # Grid
-#        self.grid = SfincsGrid()
+        if not crs:
+            self.crs = CRS(4326)
+        else:
+            self.crs = crs
 
-        # Wave boundary conditions
-        self.read_boundary_points()
-#        self.read_boundary_conditions()
-
-        # Observation points
-        self.read_observation_points()
-        self.read_observation_points_sp2()
+        if not path:
+            self.path = os.getcwd()
+        else:
+            self.path = path
 
-#        self.grid.compute_coordinates(x0,y0,dx,dy,nx,ny,rotation)
-    
-    def read_index_file(self):
-        pass
-        
-    def read_depth_file(self):
-        pass
+        if not exe_path:
+            self.exe_path = None
+        else:
+            self.exe_path = exe_path
 
-    def read_mask_file(self):
-        pass
-    
-    def write_index_file(self):
-        pass
+        # Initialize input variables
+        self.input                      = HurryWaveInput(self)
 
-    def write_depth_file(self):
-        pass
+        if load:
+            self.input.read()
+            # Get CRS from input file
+            self.crs = CRS(self.input.variables.crs_name)
+
+        self.grid                       = HurryWaveGrid(self)
+        # self.mask                       = HurryWaveMask(self)
+        # self.bathymetry                 = HurryWaveBathymetry(self)
+        self.boundary_conditions        = HurryWaveBoundaryConditions(self)
+        self.observation_points_regular = HurryWaveObservationPointsRegular(self)
+        self.observation_points_sp2     = HurryWaveObservationPointsSpectra(self)
+        self.obstacle                   = []
+
+        # Now read the attribute files
+        if load:
+            self.read_attribute_files()
+
+    def clear_spatial_attributes(self):
+        # Clear all spatial data
+        self.grid                       = HurryWaveGrid(self)
+        self.boundary_conditions        = HurryWaveBoundaryConditions(self)
+        self.observation_points_regular = HurryWaveObservationPointsRegular(self)
+        self.observation_points_sp2     = HurryWaveObservationPointsSpectra(self)
+
+    def read(self, path=None):
+        if path:
+            self.path = path
+        self.input.read()
+        # Get CRS from input file
+        self.crs = CRS(self.input.variables.crs_name)
+        self.read_attribute_files()
 
-    def write_mask_file(self):
-        pass
+    def read_input_file(self):
+        self.input.read()
+        # Get CRS from input file
+        self.crs = CRS(self.input.variables.crs_name)
 
-##### Boundary points #####
-    
-    def read_boundary_points(self):
-        
-        # Read HurryWave bnd file
-        
-        self.boundary_point = []
-        
-        if not self.input.bndfile:
-            return
-                    
-        bnd_file = os.path.join(self.path,
-                                self.input.bndfile)
+    def read_attribute_files(self):
+        self.grid.read()
+        self.boundary_conditions.read()
+        self.observation_points_regular.read()
+        self.observation_points_sp2.read()
+
+    def write(self):
+        self.input.write()
+        self.write_attribute_files()
+        
+    def write_attribute_files(self):
+        self.grid.write()
+        self.boundary_conditions.write()
+        self.observation_points_regular.write()
+        self.observation_points_sp2.write()
+
+    def write_batch_file(self):
+        fid = open(os.path.join(self.path, "run.bat"), "w")
+        fid.write(self.exe_path + "\\" + "hurrywave.exe")
+        fid.close()
 
-        if not os.path.exists(bnd_file):
-            return
+    def set_path(self, path):
+        self.path = path
         
-        # Read the bnd file
-        df = pd.read_csv(bnd_file, index_col=False, header=None,
-             delim_whitespace=True, names=['x', 'y'])
-        
-        # Loop through points
-        for ind in range(len(df.x.values)):
-            name = str(ind + 1).zfill(4)
-            point = BoundaryPoint(df.x.values[ind],
-                                  df.y.values[ind],
-                                  name=name)
-            self.boundary_point.append(point)
-
-    def write_boundary_points(self, file_name=None):
-
-        # Write HurryWave bnd file
-        if not file_name:
-            if not self.input.bndfile:
-                return
-            file_name = os.path.join(self.path,
-                                     self.input.bndfile)
-            
-        if not file_name:
-            return
-            
-        fid = open(file_name, "w")
-        for point in self.boundary_point:
-            string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}"\n'
-            fid.write(string)
-        fid.close()    
+    def list_observation_points_regular(self):
+        return self.observation_points_regular.list_observation_points()
 
-    # def read_boundary_conditions(self, file_name=None):
+    def list_observation_points_spectra(self):
+        return self.observation_points_spectra.list_observation_points()
 
-    #     # Read HurryWave bhs file
+# ##### Boundary points #####
+    
+#     # def read_boundary_points(self):
         
-    #     if not file_name:
-    #         if not self.input.bhsfile:
-    #             return
-    #         file_name = os.path.join(self.path,
-    #                                  self.input.bzsfile)
-            
-    #     if not file_name:
-    #         return
+#     #     # Read HurryWave bnd file
         
-    #     if not os.path.exists(file_name):
-    #         return
+#     #     self.boundary_point = []
         
-    #     if not self.input.tref:
-    #         # tref has not yet been defined
-    #         return
-
-    #     df = read_timeseries_file(file_name, self.input.tref)
+#     #     if not self.input.bndfile:
+#     #         return
+                    
+#     #     bnd_file = os.path.join(self.path,
+#     #                             self.input.bndfile)
 
-    #     ts  = df.index
-    #     for icol, point in enumerate(self.boundary_point):
-    #         point.data = pd.Series(df.iloc[:,icol].values, index=ts)
+#     #     if not os.path.exists(bnd_file):
+#     #         return
         
-    def write_boundary_conditions(self, file_name=None):
-
-        import xarray as xr
-
-        # Write HurryWave bsp file
-        if not file_name:
-            if not self.input.bspfile:
-                return
-            file_name = os.path.join(self.path,
-                                      self.input.bspfile)
-            
-        if not file_name:
-            return
+#     #     # Read the bnd file
+#     #     df = pd.read_csv(bnd_file, index_col=False, header=None,
+#     #          delim_whitespace=True, names=['x', 'y'])
+        
+#     #     # Loop through points
+#     #     for ind in range(len(df.x.values)):
+#     #         name = str(ind + 1).zfill(4)
+#     #         point = BoundaryPoint(df.x.values[ind],
+#     #                               df.y.values[ind],
+#     #                               name=name)
+#     #         self.boundary_point.append(point)
+
+#     # def write_boundary_points(self, file_name=None):
+
+#     #     # Write HurryWave bnd file
+#     #     if not file_name:
+#     #         if not self.input.bndfile:
+#     #             return
+#     #         file_name = os.path.join(self.path,
+#     #                                  self.input.bndfile)
+            
+#     #     if not file_name:
+#     #         return
+            
+#     #     fid = open(file_name, "w")
+#     #     for point in self.boundary_point:
+#     #         string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}"\n'
+#     #         fid.write(string)
+#     #     fid.close()    
+
+#     # def read_boundary_conditions(self, file_name=None):
+
+#     #     # Read HurryWave bhs file
+        
+#     #     if not file_name:
+#     #         if not self.input.bhsfile:
+#     #             return
+#     #         file_name = os.path.join(self.path,
+#     #                                  self.input.bzsfile)
+            
+#     #     if not file_name:
+#     #         return
+        
+#     #     if not os.path.exists(file_name):
+#     #         return
+        
+#     #     if not self.input.tref:
+#     #         # tref has not yet been defined
+#     #         return
+
+#     #     df = read_timeseries_file(file_name, self.input.tref)
+
+#     #     ts  = df.index
+#     #     for icol, point in enumerate(self.boundary_point):
+#     #         point.data = pd.Series(df.iloc[:,icol].values, index=ts)
+        
+#     def write_boundary_conditions(self, file_name=None):
+
+#         import xarray as xr
+
+#         # Write HurryWave bsp file
+#         if not file_name:
+#             if not self.input.bspfile:
+#                 return
+#             file_name = os.path.join(self.path,
+#                                       self.input.bspfile)
+            
+#         if not file_name:
+#             return
+
+#         times = self.boundary_point[0].data.point_spectrum2d.coords["time"].values
+# #        tref  = np.datetime64(self.input.tref)
+# #        times = np.single((times-tref)/1000000000)
+        
+#         sigma = self.boundary_point[0].data.point_spectrum2d.coords["sigma"].values
+#         theta = self.boundary_point[0].data.point_spectrum2d.coords["theta"].values
+
+#         sp2 = np.zeros([len(times), len(self.boundary_point), len(theta), len(sigma)])
+
+#         points = []
+#         xs     = np.zeros([len(self.boundary_point)])
+#         ys     = np.zeros([len(self.boundary_point)])
+#         for ip,point in enumerate(self.boundary_point):
+#             points.append(point.name)
+#             xs[ip] = point.geometry.x
+#             ys[ip] = point.geometry.y
+#             sp2[:,ip,:,:] = point.data.point_spectrum2d.values
+
+#         # Convert to single        
+#         xs  = np.single(xs)            
+#         ys  = np.single(ys)            
+#         sp2 = np.single(sp2)            
+
+#         ds = xr.Dataset(
+#                 data_vars = dict(point_spectrum2d=(["time", "stations", "theta", "sigma"], sp2),
+#                                  station_x=(["stations"], xs),
+#                                  station_y=(["stations"], ys),
+#                                  ),
+#                 coords    = dict(time=times,
+#                                  stations=points,
+#                                  theta=theta,
+#                                  sigma=sigma)
+#                 )
 
-        times = self.boundary_point[0].data.point_spectrum2d.coords["time"].values
-#        tref  = np.datetime64(self.input.tref)
-#        times = np.single((times-tref)/1000000000)
-        
-        sigma = self.boundary_point[0].data.point_spectrum2d.coords["sigma"].values
-        theta = self.boundary_point[0].data.point_spectrum2d.coords["theta"].values
-
-        sp2 = np.zeros([len(times), len(self.boundary_point), len(theta), len(sigma)])
-
-        points = []
-        xs     = np.zeros([len(self.boundary_point)])
-        ys     = np.zeros([len(self.boundary_point)])
-        for ip,point in enumerate(self.boundary_point):
-            points.append(point.name)
-            xs[ip] = point.geometry.x
-            ys[ip] = point.geometry.y
-            sp2[:,ip,:,:] = point.data.point_spectrum2d.values
-
-        # Convert to single        
-        xs  = np.single(xs)            
-        ys  = np.single(ys)            
-        sp2 = np.single(sp2)            
-
-        ds = xr.Dataset(
-                data_vars = dict(point_spectrum2d=(["time", "stations", "theta", "sigma"], sp2),
-                                 station_x=(["stations"], xs),
-                                 station_y=(["stations"], ys),
-                                 ),
-                coords    = dict(time=times,
-                                 stations=points,
-                                 theta=theta,
-                                 sigma=sigma)
-                )
-
-        dstr = "seconds since " + self.input.tref.strftime("%Y%m%d %H%M%S")
+#         dstr = "seconds since " + self.input.tref.strftime("%Y%m%d %H%M%S")
                 
-        ds.to_netcdf(path=file_name,
-                     mode='w',
-                     encoding={'time':{'units':dstr}})
-#        ds.to_netcdf(path=file_name,
-#                     mode='w')
+#         ds.to_netcdf(path=file_name,
+#                      mode='w',
+#                      encoding={'time':{'units':dstr}})
+# #        ds.to_netcdf(path=file_name,
+# #                     mode='w')
         
 
     ### Observation points (regular) ###
 
-    def add_observation_point(self, x, y, name):
+    # def add_observation_point(self, x, y, name):
                 
-        self.observation_point.append(ObservationPoint(x, y, name, crs=None))
+    #     self.observation_point.append(ObservationPoint(x, y, name, crs=None))
 
-    def read_observation_points(self, file_name=None):
+    # def read_observation_points(self, file_name=None):
         
-        self.observation_point = []
+    #     self.observation_point = []
 
-        if not file_name:
-            if not self.input.obsfile:
-                return
-            file_name = os.path.join(self.path,
-                                     self.input.obsfile)
+    #     if not file_name:
+    #         if not self.input.obsfile:
+    #             return
+    #         file_name = os.path.join(self.path,
+    #                                  self.input.obsfile)
                             
-        if not os.path.exists(file_name):
-            print("Warning : file " + file_name + " does not exist !")
-            return
-        
-        # Loop through points
-        df = pd.read_csv(file_name, index_col=False, header=None,
-             delim_whitespace=True, names=['x', 'y', 'name'])
-        
-        for ind in range(len(df.x.values)):
-            point = ObservationPoint(df.x.values[ind],
-                                     df.y.values[ind],
-                                     name=str(df.name.values[ind]))
-            self.observation_point.append(point)
+    #     if not os.path.exists(file_name):
+    #         print("Warning : file " + file_name + " does not exist !")
+    #         return
+        
+    #     # Loop through points
+    #     df = pd.read_csv(file_name, index_col=False, header=None,
+    #          delim_whitespace=True, names=['x', 'y', 'name'])
+        
+    #     for ind in range(len(df.x.values)):
+    #         point = ObservationPoint(df.x.values[ind],
+    #                                  df.y.values[ind],
+    #                                  name=str(df.name.values[ind]))
+    #         self.observation_point.append(point)
 
-    def write_observation_points(self, file_name=None):
+    # def write_observation_points(self, file_name=None):
 
-        if not file_name:
-            file_name = os.path.join(self.path,
-                                     self.input.obsfile)
-        if self.crs.is_geographic:
-            fid = open(file_name, "w")
-            for point in self.observation_point:
-                string = f'{point.geometry.x:12.6f}{point.geometry.y:12.6f}  "{point.name}"\n'
-                fid.write(string)
-            fid.close()
-        else:
-            fid = open(file_name, "w")
-            for point in self.observation_point:
-                string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}  "{point.name}"\n'
-                fid.write(string)
-            fid.close()
+    #     if not file_name:
+    #         file_name = os.path.join(self.path,
+    #                                  self.input.obsfile)
+    #     if self.crs.is_geographic:
+    #         fid = open(file_name, "w")
+    #         for point in self.observation_point:
+    #             string = f'{point.geometry.x:12.6f}{point.geometry.y:12.6f}  "{point.name}"\n'
+    #             fid.write(string)
+    #         fid.close()
+    #     else:
+    #         fid = open(file_name, "w")
+    #         for point in self.observation_point:
+    #             string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}  "{point.name}"\n'
+    #             fid.write(string)
+    #         fid.close()
         
     ### Observation points (2d spectra) ###
 
-    def add_observation_point_sp2(self, x, y, name):
+    # def add_observation_point_sp2(self, x, y, name):
                 
-        self.observation_point_sp2.append(ObservationPoint(x, y, name, crs=None))
+    #     self.observation_point_sp2.append(ObservationPoint(x, y, name, crs=None))
 
-    def read_observation_points_sp2(self, file_name=None):
+    # def read_observation_points_sp2(self, file_name=None):
         
-        self.observation_point_sp2 = []
+    #     self.observation_point_sp2 = []
 
-        if not file_name:
-            if not self.input.ospfile:
-                return
-            file_name = os.path.join(self.path,
-                                     self.input.ospfile)
+    #     if not file_name:
+    #         if not self.input.ospfile:
+    #             return
+    #         file_name = os.path.join(self.path,
+    #                                  self.input.ospfile)
                             
-        if not os.path.exists(file_name):
-            print("Warning : file " + file_name + " does not exist !")
-            return
-        
-        # Loop through points
-        df = pd.read_csv(file_name, index_col=False, header=None,
-             delim_whitespace=True, names=['x', 'y', 'name'])
-        
-        for ind in range(len(df.x.values)):
-            point = ObservationPoint(df.x.values[ind],
-                                     df.y.values[ind],
-                                     name=str(df.name.values[ind]))
-            self.observation_point_sp2.append(point)
+    #     if not os.path.exists(file_name):
+    #         print("Warning : file " + file_name + " does not exist !")
+    #         return
+        
+    #     # Loop through points
+    #     df = pd.read_csv(file_name, index_col=False, header=None,
+    #          delim_whitespace=True, names=['x', 'y', 'name'])
+        
+    #     for ind in range(len(df.x.values)):
+    #         point = ObservationPoint(df.x.values[ind],
+    #                                  df.y.values[ind],
+    #                                  name=str(df.name.values[ind]))
+    #         self.observation_point_sp2.append(point)
 
-    def write_observation_points_sp2(self, file_name=None):
+    # def write_observation_points_sp2(self, file_name=None):
 
-        if not file_name:
-            file_name = os.path.join(self.path,
-                                     self.input.ospfile)
-        if self.crs.is_geographic:    
-            fid = open(file_name, "w")
-            for point in self.observation_point_sp2:
-                string = f'{point.geometry.x:12.6f}{point.geometry.y:12.6f}  "{point.name}"\n'
-                fid.write(string)
-            fid.close()
-        else:
-            fid = open(file_name, "w")
-            for point in self.observation_point_sp2:
-                string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}  "{point.name}"\n'
-                fid.write(string)
-            fid.close()
+    #     if not file_name:
+    #         file_name = os.path.join(self.path,
+    #                                  self.input.ospfile)
+    #     if self.crs.is_geographic:    
+    #         fid = open(file_name, "w")
+    #         for point in self.observation_point_sp2:
+    #             string = f'{point.geometry.x:12.6f}{point.geometry.y:12.6f}  "{point.name}"\n'
+    #             fid.write(string)
+    #         fid.close()
+    #     else:
+    #         fid = open(file_name, "w")
+    #         for point in self.observation_point_sp2:
+    #             string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}  "{point.name}"\n'
+    #             fid.write(string)
+    #         fid.close()
             
 
     ### Output ###
 
     def read_timeseries_output(self,
                                name_list = None,
                                path=None,
@@ -369,15 +357,15 @@
                                parameter = "hm0"):
 
         import xarray as xr
         import pandas as pd
         import numpy as np
 
         # Returns a dataframe with timeseries    
-        
+        # parameter options: hm0, tp, wavdir, dirsp        
         if not path:
             path = self.path
 
         if not file_name:
             file_name = "hurrywave_his.nc"
 
         file_name = os.path.join(path, file_name)
@@ -396,53 +384,23 @@
         if not name_list:
             name_list = []
             for st in all_stations:
                 name_list.append(st)
         
         df = pd.DataFrame(index=times, columns=name_list)
         
-        if parameter.lower() == "hm0":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_hm0.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
-
-        elif parameter.lower() == "tp":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_tp.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
-
-        elif parameter.lower() == "wavdir":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_wavdir.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
-
-        elif parameter.lower() == "dirspr":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_dirsp.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
+        data_tmp = ddd["point_" + parameter].values
+
+        for station in name_list:
+            for ist, st in enumerate(all_stations):
+                if station == st:
+                    data = data_tmp[:,ist]
+                    data[np.isnan(data)] = -999.0
+                    df[st]=data
+                    break            
 
         ddd.close()
         
         return df    
         
         # # Returns a dataframe with timeseries
     
@@ -462,16 +420,43 @@
         # # Add column names
         # df.columns = columns
             
         # if name_list:
         #     df = df[name_list]
             
         # return df    
+    def read_map_output_max(self, time_range=None, map_file=None, parameter = "hm0"):
+    
+        if not map_file:
+            map_file = os.path.join(self.path, "hurrywave_map.nc")
+            
+        dsin = xr.open_dataset(map_file)
+
+        output_times = dsin.timemax.values
+        if time_range is None:
+
+            t0 = pd.to_datetime(str(output_times[0])).replace(tzinfo=None).to_pydatetime()
+            t1 = pd.to_datetime(str(output_times[-1])).replace(tzinfo=None).to_pydatetime()
+            time_range = [t0, t1]
+
+        it0 = -1
+        for it, time in enumerate(output_times):
+            time = pd.to_datetime(str(time)).replace(tzinfo=None).to_pydatetime()
+            if time>=time_range[0] and it0<0:
+                it0 = it
+            if time<=time_range[1]:
+                it1 = it
+        
+        zs_da = np.amax(dsin[parameter].values[it0:it1,:,:], axis=0)
+        dsin.close()
+        
+        return zs_da
+
 
-    def read_hm0max(self, time_range=None, hm0max_file=None):
+    def read_hm0max(self, time_range=None, hm0max_file=None, parameter='hm0max'):
     
         if not hm0max_file:
             hm0max_file = os.path.join(self.path, "hm0max.dat")
             
         fname, ext = os.path.splitext(hm0max_file)
         
         if ext == ".dat":
@@ -512,15 +497,31 @@
             zs_da[data_ind - 1] = np.squeeze(data_zs)
             zs_da = np.where(zs_da == -999, np.nan, zs_da)
             zs_da = np.transpose(np.reshape(zs_da, [mmax, nmax]))[1:-1,1:-1]
         
         elif ext==".nc":
 
             dsin = xr.open_dataset(hm0max_file)
-            zs_da = np.transpose(np.amax(dsin.hm0max.values, axis=0))
+
+            output_times = dsin.timemax.values
+            if time_range is None:
+
+                t0 = pd.to_datetime(str(output_times[0])).replace(tzinfo=None).to_pydatetime()
+                t1 = pd.to_datetime(str(output_times[-1])).replace(tzinfo=None).to_pydatetime()
+                time_range = [t0, t1]
+
+            it0 = -1
+            for it, time in enumerate(output_times):
+                time = pd.to_datetime(str(time)).replace(tzinfo=None).to_pydatetime()
+                if time>=time_range[0] and it0<0:
+                    it0 = it
+                if time<=time_range[1]:
+                    it1 = it            
+            
+            zs_da = np.amax(dsin[parameter].values[it0:it1,:,:], axis=0)
             dsin.close()
             
         else:
             # Must be txt file
             return None
         
 
@@ -624,19 +625,21 @@
             xg, yg = transformer.transform(xg, yg)
         
         xp = [ xg[0,0], xg[0,-1], xg[-1,-1], xg[-1,0], xg[0,0] ]
         yp = [ yg[0,0], yg[0,-1], yg[-1,-1], yg[-1,0], yg[0,0] ]
         
         return xp, yp
         
-    def make_index_tiles(self, path, zoom_range=None):
-        
-        from tiling import deg2num
-        from tiling import num2deg
-        import fileops as fo
+    def make_index_tiles(self, path, zoom_range=None,  
+                         z_range=None,
+                         dem_names=None):
+        
+        from cht.tiling.tiling import deg2num
+        from cht.tiling.tiling import num2deg
+        import cht.misc.fileops as fo
         
         if not zoom_range:
             zoom_range = [0, 13]
 
         npix = 256
         
         # Compute lon/lat range
@@ -647,14 +650,34 @@
         
         transformer_a = Transformer.from_crs(CRS.from_epsg(4326),
                                              CRS.from_epsg(3857),
                                              always_xy=True)
         transformer_b = Transformer.from_crs(CRS.from_epsg(3857),
                                              self.crs,
                                              always_xy=True)
+
+        # Remove existing path
+        if os.path.exists(path):
+            print("Removing existing path " + path)
+            fo.rmdir(path)
+            
+        if z_range:
+            # Only want data in specific range
+            # Need to do some other stuff here
+            from cht.bathymetry.bathymetry_database import bathymetry_database
+            from cht.tiling.tiling import get_bathy_on_tile
+
+            for dem_name in dem_names:
+                dem_crs = []
+                transformer_3857_to_dem = []                
+                for dem_name in dem_names:                
+                    dem_crs.append(bathymetry_database.get_crs(dem_name))            
+                    transformer_3857_to_dem.append(Transformer.from_crs(CRS.from_epsg(3857),
+                                                                        dem_crs[-1],
+                                                                        always_xy=True))
         
         for izoom in range(zoom_range[0], zoom_range[1] + 1):
             
             print("Processing zoom level " + str(izoom))
         
             zoom_path = os.path.join(path, str(izoom))
         
@@ -671,221 +694,151 @@
                 path_okay = False
                 zoom_path_i = os.path.join(zoom_path, str(i))
             
                 for j in range(iy0, iy1 + 1):
             
                     file_name = os.path.join(zoom_path_i, str(j) + ".dat")
             
-                    # Compute lat/lon at ll corner of tile
+                    # Compute lat/lon at lower-left corner of tile
                     lat, lon = num2deg(i, j, izoom)
             
                     # Convert to Global Mercator
                     xo, yo   = transformer_a.transform(lon,lat)
             
-                    # Tile grid on local mercator
-                    x        = xv[:] + xo + 0.5*dxy
-                    y        = yv[:] + yo + 0.5*dxy
-            
+                    # Tile grid on Global Mercator
+                    xm = xv[:] + xo + 0.5*dxy
+                    ym = yv[:] + yo + 0.5*dxy
+                                
                     # Convert tile grid to crs of HurryWave model
-                    x,y      = transformer_b.transform(x,y)
+                    x,y      = transformer_b.transform(xm, ym)
                     
                     # Now rotate around origin of HurryWave model
                     x00 = x - self.input.x0
                     y00 = y - self.input.y0
                     xg  = x00*cosrot - y00*sinrot
                     yg  = x00*sinrot + y00*cosrot
                     
                     iind = np.floor(xg/self.input.dx).astype(int)
                     jind = np.floor(yg/self.input.dy).astype(int)
                     ind  = iind*self.input.nmax + jind
+                                        
                     ind[iind<0]   = -999
                     ind[jind<0]   = -999
                     ind[iind>=self.input.mmax] = -999
                     ind[jind>=self.input.nmax] = -999
 
-
-#                    ind           = np.ascontiguousarray(np.transpose(ind))
-
-                    # if i==142 and j==305:
-                    
-                    #     from matplotlib import pyplot as plt
-                    #     fig, ax = plt.subplots(1,1)                                            
-                    #     ax.plot(x,y)
-                    #     ax.plot(x.transpose(),y.transpose())
-                    #     ax.axis('equal')
-                    #     x_range, y_range = self.bounding_box()
-                    #     xp = [x_range[0], x_range[1],x_range[1],x_range[0],x_range[0]]
-                    #     yp = [y_range[0], y_range[0],y_range[1],y_range[1],y_range[0]]
-                    #     ax.plot(xp,yp)
-                    #     xout, yout = self.outline()
-                    #     ax.plot(xout,yout)
-                    #     fig, ax = plt.subplots(1,1)                                            
-                    #     ax.pcolor(ind.reshape([256, 256]))
-                    #     xxx=1
+                    if z_range:
+                        # Need temporarily create topo indices here to make indices
+                        # only for specific depth ranges
+                        z = get_bathy_on_tile(xm, ym,
+                                              dem_names,
+                                              dem_crs,
+                                              transformer_3857_to_dem,
+                                              dxy,
+                                              bathymetry_database)
+                        ind[z<z_range[0]] = -999
+                        ind[z>z_range[1]] = -999
+
+                    if self.mask:
+                        if ind.max()>=0:
+                            # Do not include points with mask<1
+                            ingrid      = np.where(ind>=0)
+                            msk         = np.zeros((256,256), dtype=int) + 1
+                            msk[ingrid] = self.mask.mask[jind[ingrid], iind[ingrid]]
+                            iex         = np.where(msk<1)
+                            ind[iex]    = -999
                     
-                    if np.any(ind>=0):
-                        
+                    if np.any(ind>=0):                     
                         if not path_okay:
                             if not os.path.exists(zoom_path_i):
                                 fo.mkdir(zoom_path_i)
-                                path_okay = True
-                             
+                                path_okay = True                             
                         # And write indices to file
                         fid = open(file_name, "wb")
                         fid.write(ind)
                         fid.close()
 
-class HurryWaveInput():
-    def __init__(self):
-        self.mmax         = 0
-        self.nmax         = 0
-        self.dx           = 0.1
-        self.dy           = 0.1
-        self.x0           = 0.0
-        self.y0           = 0.0
-        self.rotation     = 0.0
-        self.latitude     = 0.0
-        self.tref         = None
-        self.tstart       = None
-        self.tstop        = None
-        self.tspinup      = 60.0
-        self.t0out        = -999.0
-        self.dtmapout     = 3600.0
-        self.dthisout     = 600.0
-        self.dtrstout     = 0.0
-        self.dtsp2out     = 0.0
-        self.dtmaxout     = 0.0
-        self.trstout      = -999.0
-        self.dtwnd        = 1800.0
-        self.rhoa         = 1.25
-        self.rhow         = 1024.0
-        self.dmx1         = 0.2
-        self.dmx2         = 0.00001
-        self.crsgeo       = 0
-        self.freqmin      = 0.04
-        self.freqmax      = 0.5
-        self.nsigma       = 12
-        self.ntheta       = 36
-        self.crs_name     = "WGS 84"
-        self.crs_type     = "geographic"
-        self.crs_utmzone  = None
-        self.crs_epsg     = None
-        self.gammajsp     = 3.3
-        self.spinup_meteo = 0
-        self.quadruplets  = 1
-        self.utmzone      = None
-        
-        self.depfile      = None
-        self.mskfile      = None
-        self.indexfile    = None
-        self.bndfile      = None
-        self.bhsfile      = None
-        self.btpfile      = None
-        self.bwdfile      = None
-        self.bdsfile      = None
-        self.bspfile      = None
-        self.rstfile      = None
-        self.spwfile      = None
-        self.amufile      = None
-        self.amvfile      = None
-        self.wndfile      = None
-        self.obsfile      = None
-        self.ospfile      = None
-        
-        self.inputformat  = "bin"
-        self.outputformat = "bin"
-        
-        self.cdnrb        = 3
-        self.cdwnd        = [0.0,28.0,50.0]
-        self.cdval        = [0.001,0.0025,0.0015]
 
-class HurryWaveGrid():
-
-    def __init__(self, x0, y0, dx, dy, nx, ny, rotation):
-        self.geometry = RegularGrid(x0, y0, dx, dy, nx, ny, rotation)
+# class HurryWaveGrid():
+#
+#     def __init__(self, x0, y0, dx, dy, nx, ny, rotation):
+#         self.geometry = RegularGrid(x0, y0, dx, dy, nx, ny, rotation)
 
     # def plot(self,ax):
     #     self.geometry.plot(ax)
 
     # def corner_coordinates(self):
     #     x,y = self.geometry.grid_coordinates_corners()
     #     return x, y
 
     # def centre_coordinates(self):
     #     x,y = self.geometry.grid_coordinates_centres()
     #     return x, y
 
-class HurryWaveDepth():
-    def __init__(self):
-        self.value = []
-        self.geometry = []
-    def plot(self,ax):
-        pass
-    def read(self):
-        pass
-
-class HurryWaveMask():
-    def __init__(self):
-        self.msk = []
-    def plot(self,ax):
-        pass
-
-class HurryWaveBoundaryConditions():
-    
-    def __init__(self):
-        self.geometry = []
-
-    def read(self, bndfile, bzsfile):
-        self.read_points(bndfile)
-        self.read_time_series(bzsfile)
-
-    def read_points(self, file_name):
-        pass
-
-    def read_time_series(self, file_name):
-        pass
-    
-    def set_xy(self, x, y):
-        self.geometry.x = x
-        self.geometry.y = y
-        pass
-    
-    def plot(self,ax):
-        pass
-
-class HurryWaveBoundaryConditions():
-    
-    def __init__(self):
-        self.geometry = []
-
-    def read(self, bndfile, bzsfile):
-        self.read_points(bndfile)
-        self.read_time_series(bzsfile)
-
-    def read_points(self, file_name):
-        pass
+# class HurryWaveDepth():
+#     def __init__(self):
+#         self.value = []
+#         self.geometry = []
+#     def plot(self,ax):
+#         pass
+#     def read(self):
+#         pass
+
+# class HurryWaveMask():
+#     def __init__(self):
+#         self.msk = []
+#     def plot(self,ax):
+#         pass
+
+# class HurryWaveBoundaryConditions():
+#
+#     def __init__(self):
+#         self.geometry = []
+#
+#     def read(self, bndfile, bzsfile):
+#         self.read_points(bndfile)
+#         self.read_time_series(bzsfile)
+#
+#     def read_points(self, file_name):
+#         pass
+#
+#     def read_time_series(self, file_name):
+#         pass
+#
+#     def set_xy(self, x, y):
+#         self.geometry.x = x
+#         self.geometry.y = y
+#         pass
+#
+#     def plot(self,ax):
+#         pass
+
+# class HurryWaveBoundaryConditions():
+#
+#     def __init__(self):
+#         self.geometry = []
+#
+#     def read(self, bndfile, bzsfile):
+#         self.read_points(bndfile)
+#         self.read_time_series(bzsfile)
+#
+#     def read_points(self, file_name):
+#         pass
+#
+#     def read_time_series(self, file_name):
+#         pass
+#
+#     def set_xy(self, x, y):
+#         self.geometry.x = x
+#         self.geometry.y = y
+#         pass
+#
+#     def plot(self,ax):
+#         pass
 
-    def read_time_series(self, file_name):
-        pass
-    
-    def set_xy(self, x, y):
-        self.geometry.x = x
-        self.geometry.y = y
-        pass
-    
-    def plot(self,ax):
-        pass
-
-class BoundaryPoint():
-
-    def __init__(self, x, y, name=None, crs=None, data=None, astro=None):
-        
-        self.name                   = name
-        self.geometry               = Point(x, y, crs=crs)
-        self.data                   = data
 
 class ObservationPoint():
 
     def __init__(self, x, y, name, crs=None):
         
         self.name     = name
         self.geometry = Point(x, y, crs=crs)
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/coamps_analysis.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_analysis.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50_02.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_02.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50_03.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_03.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_anl_0p50_04.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_04.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_forecast_0p25.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.quantity = None
         self.unit     = None
         self.time     = None
         self.x        = None
         self.y        = None
         self.crs      = None
         self.val      = None
+        self.src      = "gfs_forecast_0p25"
 
 def download(param_list, lon_range, lat_range, time_range, cycle_time):
 
     cycle_string = cycle_time.strftime("%Y%m%d_%H%M")
 
     base_url = "https://thredds.ucar.edu/thredds/catalog/grib/NCEP/GFS/Global_0p25deg/"
     url = base_url + "GFS_Global_0p25deg_" + cycle_string + ".grib2/catalog.xml"
@@ -54,17 +55,20 @@
                              south=lat_range[0], \
                              east=lon_range[1],  \
                              west=lon_range[0]).time_range(time_range[0], time_range[1]).vertical_level(10.0)
             query.variables("u-component_of_wind_height_above_ground",
                             "v-component_of_wind_height_above_ground")
             data = ncss.get_data(query)
             data = xr.open_dataset(NetCDF4DataStore(data))
-
-            dataset.x    = np.array(data['lon'])
-            dataset.y    = np.array(data['lat'])
+            try:
+                dataset.x    = np.array(data['lon'])
+                dataset.y    = np.array(data['lat'])
+            except:
+                dataset.x    = np.array(data['longitude'])
+                dataset.y    = np.array(data['latitude'])
  #           time   = data['time']
 
             u = data['u-component_of_wind_height_above_ground']
             time   = find_time_var(u)
             dataset.time = pd.to_datetime(time.data).to_pydatetime()
             dataset.unit = u.units
             u = u.metpy.unit_array.squeeze()
@@ -93,16 +97,20 @@
                              south=lat_range[0], \
                              east=lon_range[1],  \
                              west=lon_range[0]).time_range(time_range[0], time_range[1])
             query.variables(var_name)
             data = ncss.get_data(query)
             data = xr.open_dataset(NetCDF4DataStore(data))
                 
-            dataset.x    = np.array(data['lon'])
-            dataset.y    = np.array(data['lat'])
+            try:
+                dataset.x    = np.array(data['lon'])
+                dataset.y    = np.array(data['lat'])
+            except:
+                dataset.x    = np.array(data['longitude'])
+                dataset.y    = np.array(data['latitude'])
 #            time   = data['time']
 #            d.time = pd.to_datetime(time.data).to_pydatetime()
             
             val          = data[var_name]
             time         = find_time_var(val)
             dataset.time = pd.to_datetime(time.data).to_pydatetime()
             dataset.unit = val.units
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/meteosources/gfs_forecast_0p25_02.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25_02.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/misc_tools.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/misc_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 
 @author: ormondt
 """
 
 from scipy.interpolate import RegularGridInterpolator
 import numpy as np
 import json
+import yaml
 
-def interp2(x0,y0,z0,x1,y1):
+def interp2(x0, y0, z0, x1, y1, method="linear"):
     
     f = RegularGridInterpolator((y0, x0), z0,
-                                bounds_error=False, fill_value=np.nan)    
+                                bounds_error=False, fill_value=np.nan, method=method)
     # reshape x1 and y1
-    sz = x1.shape
-    x1 = x1.reshape(sz[0]*sz[1])
-    y1 = y1.reshape(sz[0]*sz[1])    
-    # interpolate
-    z1 = f((y1,x1)).reshape(sz)        
+    if x1.ndim>1:
+        sz = x1.shape
+        x1 = x1.reshape(sz[0]*sz[1])
+        y1 = y1.reshape(sz[0]*sz[1])    
+        # interpolate
+        z1 = f((y1,x1)).reshape(sz)        
+    else:    
+        z1 = f((y1,x1))
     
     return z1
 
 def findreplace(file_name, str1, str2):
 
     #read input file
     fin = open(file_name, "rt")
@@ -82,7 +86,17 @@
      f.write(csv_string)
      f.write('`;')
      f.close()         
 
 def rgb2hex(rgb):
     return '%02x%02x%02x' % rgb
 
+def dict2yaml(file_name, dct, sort_keys=False):
+    yaml_string = yaml.dump(dct, sort_keys=sort_keys)    
+    file = open(file_name, "w")  
+    file.write(yaml_string)
+    file.close()
+
+def yaml2dict(file_name):
+    file = open(file_name,"r")
+    dct = yaml.load(file, Loader=yaml.FullLoader)
+    return dct
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/nesting.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nesting.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,54 +5,69 @@
 @author: ormondt
 """
 
 import os
 from pyproj import CRS
 from pyproj import Transformer
 import pandas as pd
+import xarray as xr
+import numpy as np
+import glob
+import datetime 
 
 def nest1(overall, detail, option=None):
     
     # Returns a list with observation point objects
     
     if overall.type.lower() == "delft3dfm":
         if detail.type.lower() == "delft3dfm":
             nest1_delft3dfm_in_delft3dfm(overall, detail)
         elif detail.type.lower() == "sfincs":
             nest1_sfincs_in_delft3dfm(overall, detail)
         elif detail.type.lower() == "beware":
-            pass
-#            nest1_beware_in_delft3dfm(overall, detail)
+            nest1_beware_in_delft3dfm(overall, detail)
             
     elif overall.type.lower() == "sfincs":
         if detail.type.lower() == "sfincs":
             nest1_sfincs_in_sfincs(overall, detail)
         elif detail.type.lower() == "xbeach":
             nest1_xbeach_in_sfincs(overall, detail)
+        elif detail.type.lower() == "beware":
+            nest1_beware_in_sfincs(overall, detail)
 
     elif overall.type.lower() == "hurrywave":
         if detail.type.lower() == "hurrywave":
             nest1_hurrywave_in_hurrywave(overall, detail)
         elif detail.type.lower() == "xbeach":    
             if not option:
                 option = "timeseries"
             nest1_xbeach_in_hurrywave(overall, detail, option=option)
         elif detail.type.lower() == "sfincs":    
             nest1_sfincs_in_hurrywave(overall, detail)
+        elif detail.type.lower() == "beware":
+            nest1_beware_in_hurrywave(overall, detail)
+
+    elif overall.type.lower() == "beware":
+        if detail.type.lower() == "sfincs":
+            # No need to do anything here. BEWARE output points are fixed
+            pass
 
 #        elif detail.type == "delft3dfm":
 #            obs = nest1_delft3dfm_in_sfincs(overall, detail)
 
 #    return obs    
 
 def nest2(overall,
           detail,
           boundary_water_level_correction=None,
           output_path=None,
-          output_file=None):
+          output_file=None,
+	      option=None,
+          return_maximum=False,
+          bc_file=None):
 
 
     if not boundary_water_level_correction:
         # Path of the overall output time series
         boundary_water_level_correction = 0.0
     
     if overall.type.lower() == "delft3dfm":
@@ -72,56 +87,80 @@
                                       boundary_water_level_correction)
 
         elif detail.type.lower() == "beware":
             nest2_beware_in_delft3dfm(overall,
                                       detail,
                                       output_path,
                                       output_file,
-                                      boundary_water_level_correction)
+                                      boundary_water_level_correction,
+                                      option)
             
     elif overall.type.lower() == "sfincs":
 
         if detail.type.lower() == "sfincs":
-            nest2_sfincs_in_sfincs(overall,
-                                   detail,
-                                   output_path,
-                                   output_file,
-                                   boundary_water_level_correction)
+            zs = nest2_sfincs_in_sfincs(overall,
+                                        detail,
+                                        output_path,
+                                        output_file,
+                                        boundary_water_level_correction,
+                                        return_maximum=return_maximum)
+            return zs
         elif detail.type.lower() == "xbeach":
-            nest2_xbeach_in_sfincs(overall,
+            bc = nest2_xbeach_in_sfincs(overall,
+                                        detail,
+                                        output_path,
+                                        output_file,
+                                        boundary_water_level_correction,
+                                        return_maximum=return_maximum)
+            return bc
+        elif detail.type.lower() == "beware":
+            nest2_beware_in_sfincs(overall,
                                    detail,
                                    output_path,
                                    output_file,
-                                   boundary_water_level_correction)
+                                   boundary_water_level_correction,
+                                   option)
 
     elif overall.type.lower() == "hurrywave":
 
         if detail.type.lower() == "hurrywave":
             nest2_hurrywave_in_hurrywave(overall,
                                    detail,
                                    output_path,
-                                   output_file)
+                                   output_file,
+                                   bc_file)
+            pass
         elif detail.type.lower() == "xbeach":
-            nest2_xbeach_in_hurrywave(overall,
-                                   detail,
-                                   output_path,
-                                   output_file)
+            bc = nest2_xbeach_in_hurrywave(overall,
+                                           detail,
+                                           output_path,
+                                           output_file,
+                                           option,
+                                           return_maximum=return_maximum)
+            return bc
         elif detail.type.lower() == "sfincs":
             nest2_sfincs_in_hurrywave(overall,
                                       detail,
                                       output_path,
                                       output_file)
+        elif detail.type.lower() == "beware":
+            nest2_beware_in_hurrywave(overall,
+                                      detail,
+                                      output_path,
+                                      output_file)
 
     elif overall.type.lower() == "beware":
 
         if detail.type.lower() == "sfincs":
             nest2_sfincs_in_beware(overall,
                                    detail,
                                    output_path,
-                                   output_file)
+                                   output_file,
+                                   boundary_water_level_correction,
+                                   option)
 
 def nest1_delft3dfm_in_delft3dfm(overall, detail):
     
 #    from delft3dfm import ObservationPoint as obspoint
     
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
@@ -144,15 +183,28 @@
     for ind, point in enumerate(detail.flow_boundary_point):
 
         name = detail.name + "_" + str(ind + 1).zfill(4)
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
 #        obs_list.append(obspoint(x, y, name, crs=overall.crs))
         overall.add_observation_point(x, y, name)
+
+def nest1_beware_in_delft3dfm(overall, detail):
+        
+    transformer = Transformer.from_crs(detail.crs,
+                                       overall.crs,
+                                       always_xy=True)
     
+    for ind, point in enumerate(detail.flow_boundary_point):
+
+        name = detail.name + "_" + point.name
+        x, y = transformer.transform(point.geometry.x,
+                                     point.geometry.y)
+#        obs_list.append(obspoint(x, y, name, crs=overall.crs))
+        overall.add_observation_point(x, y, name)
     
 def nest1_sfincs_in_sfincs(overall, detail):
     
 #    from sfincs import ObservationPoint as obspoint
 
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
@@ -176,58 +228,85 @@
 
         name = detail.name + "_" + str(ind + 1).zfill(4)
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
 #        obs_list.append(obspoint(x, y, name, crs=overall.crs))
         overall.add_observation_point(x, y, name)
 
-
-def nest1_hurrywave_in_hurrywave(overall, detail):
-    
+def nest1_beware_in_sfincs(overall, detail):
+        
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
                                        always_xy=True)
     
-    for ind, point in enumerate(detail.boundary_point):
+    for ind, point in enumerate(detail.flow_boundary_point):
 
-        name = detail.name + "_" + str(ind + 1).zfill(4)
+        name = detail.name + "_" + point.name
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
 #        obs_list.append(obspoint(x, y, name, crs=overall.crs))
-        overall.add_observation_point_sp2(x, y, name)
+        overall.add_observation_point(x, y, name)
+
+def nest1_hurrywave_in_hurrywave(overall, detail):
+    
+    transformer = Transformer.from_crs(detail.crs,
+                                       overall.crs,
+                                       always_xy=True)
+
+    for ind, row in detail.boundary_conditions.gdf.iterrows():
+        name = detail.name + "_" + str(ind + 1).zfill(4)
+        x = row["geometry"].coords[0][0]
+        y = row["geometry"].coords[0][1]
+        x, y = transformer.transform(x, y)
+        overall.observation_points_sp2.add_point(x, y, name)
 
 def nest1_xbeach_in_hurrywave(overall, detail, option="sp2"):
     
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
                                        always_xy=True)
     
     for ind, point in enumerate(detail.wave_boundary_point):
 
         name = detail.name + "_" + str(ind + 1).zfill(4)
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
 #        obs_list.append(obspoint(x, y, name, crs=overall.crs))
 #        if option=="sp2":
-        overall.add_observation_point_sp2(x, y, name)
+        overall.observation_points_sp2.add_point(x, y, name)
 #        else:
-        overall.add_observation_point(x, y, name)
+        overall.observation_points_regular.add_point(x, y, name)
 
 def nest1_sfincs_in_hurrywave(overall, detail):
     
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
                                        always_xy=True)
 
     for ind, point in enumerate(detail.wave_boundary_point):
 
         name = detail.name + "_" + str(ind + 1).zfill(4)
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
-        overall.add_observation_point(x, y, name)
+        overall.observation_points_regular.add_point(x, y, name)
+
+def nest1_beware_in_hurrywave(overall, detail):
+    
+    transformer = Transformer.from_crs(detail.crs,
+                                       overall.crs,
+                                       always_xy=True)
+
+    for ind, point in enumerate(detail.wave_boundary_point):
+
+        
+        name = detail.name + "_" + point.name
+        x, y = transformer.transform(point.geometry.x,
+                                     point.geometry.y)
+        overall.observation_points_regular.add_point(x, y, name)
+
             
 def nest2_delft3dfm_in_delft3dfm(overall,
                                  detail,
                                  output_path,
                                  output_file,
                                  boundary_water_level_correction):
 
@@ -273,39 +352,101 @@
     for icol, point in enumerate(detail.flow_boundary_point):
         point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction    
 
 def nest2_beware_in_delft3dfm(overall,
                               detail,
                               output_path,
                               output_file,
-                              boundary_water_level_correction):
+                              boundary_water_level_correction,
+                              option):
 
-    if not output_file:
-        # Path of the overall output time series
-        output_file = overall.runid + "_his.nc"
-    
-    point_names = []
-    for point in detail.flow_boundary_point:
-        point_names.append(detail.name + "_" + point.name)                    
-    output_file = os.path.join(output_path, output_file)
+    if option == 'flow':
+        if not output_file:
+            # Path of the overall output time series
+            output_file = overall.runid + "_his.nc"
+        
+        point_names = []
+        for point in detail.flow_boundary_point:
+            point_names.append(detail.name + "_" + point.name) #reopen                   
+            # point_names.append(point.name)                    
+        # output_file = os.path.join(output_path, output_file)
 
-    # Return DataFrame bzs
-    bzs = overall.read_timeseries_output(name_list=point_names,
-                                         path=output_path,
-                                         file_name=output_file)
+        # Return DataFrame bzs
+        bzs = overall.read_timeseries_output(name_list=point_names,
+                                             path=output_path,
+                                             file_name=output_file)
+        ts  = bzs.index
+        for icol, point in enumerate(detail.flow_boundary_point):
+            point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction    
+            
+    if option == 'wave':
 
-    ts  = bzs.index
-    for icol, point in enumerate(detail.flow_boundary_point):
-        point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction    
+
+        if not output_path:
+            # Path of the overall output time series
+            output_path = overall.path
+            
+        if not output_file:
+            file_name = glob.glob(os.path.join(output_path, "wavh*"))[1]
+        else:
+            file_name = os.path.join(output_path, output_file)
+        
+        # Open netcdf file
+        file_name_dfm = glob.glob(os.path.join(output_path, "*_his.nc"))[0]
+        ddd = xr.open_dataset(file_name_dfm)
+        stations=ddd.station_name.values
+        all_stations = []
+        for ist, st in enumerate(stations):
+            st=str(st.strip())[2:-1] #reopen
+            # st=str(st.strip())[2:6]
+            all_stations.append(st)
+
+        point_names = []
+        for point in detail.wave_boundary_point:
+            point_names.append(detail.name + "_" + point.name) #reopen                   
+            # point_names.append(point.name)  
+        # ireq = []    
+        # for ip, point in enumerate(point_names):
+        #     for ist,st in enumerate(all_stations):
+        #         if point.lower() == st.lower():
+        #             ireq.append(ist)            
+        #             break
+
+        ddd = xr.open_dataset(file_name)
+        times   = ddd.Hsig.time.values
+
+        for ip, point in enumerate(detail.wave_boundary_point):
+            for ist,st in enumerate(all_stations):
+                ireq = -1
+                if point_names[ip] == st.lower():
+                    ireq=ist
+                    break
+
+            if ireq>-1:
+                hm0     = ddd.Hsig.values[:,ireq]
+                tp      = ddd.Tm01.values[:,ireq]
+                wavdir  = ddd.Dir.values[:,ireq]
+                dirspr  = ddd.Dspr.values[:,ireq]
+    
+                df = pd.DataFrame(index=times)
+                df.insert(0,"hm0",hm0)
+                df.insert(1,"tp",tp)
+                df.insert(2,"wavdir",wavdir)
+                df.insert(3,"dirspr",dirspr)
     
+                point.data = df
+
+
+
 def nest2_sfincs_in_sfincs(overall,
                            detail,
                            output_path,
                            output_file,
-                           boundary_water_level_correction):
+                           boundary_water_level_correction,
+                           return_maximum=False):
 
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
     
         
     if overall.input.outputformat[0:3] == "bin":
@@ -326,69 +467,139 @@
     bzs = overall.read_timeseries_output(name_list=point_names,
                                          file_name=zstfile)
 
     ts  = bzs.index
     for icol, point in enumerate(detail.flow_boundary_point):
         point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction
 
+    if return_maximum:
+        zmax = -999.0
+        for icol, point in enumerate(detail.flow_boundary_point):
+            zx = point.data.max()
+            if zx>zmax:
+                zs = point.data
+                zmax = zx
+        return zs        
+                    
+    else:    
+        return detail.flow_boundary_point
+
+
+
 def nest2_xbeach_in_sfincs(overall,
                            detail,
                            output_path,
                            output_file,
-                           boundary_water_level_correction):
+                           boundary_water_level_correction,
+                           return_maximum=False):
 
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
-    if not output_file:
-        output_file = "zst.txt"
+    if overall.input.outputformat[0:3] == "bin":
+        # ascii output        
+        if not output_file:
+            output_file = "zst.txt"
+    else:
+        # netcdf        
+        if not output_file:
+            output_file = "sfincs_his.nc"
     
     point_names = []
     for point in detail.flow_boundary_point:
         point_names.append(detail.name + "_" + point.name)                    
     zstfile = os.path.join(output_path, output_file)
 
     # Return DataFrame bzs
     bzs = overall.read_timeseries_output(name_list=point_names,
                                          file_name=zstfile)
 
-    ts  = bzs.index
+    
+    # Interpolate on desired format for XBeach forcing
+    bzs_resampled = bzs.resample('10min').mean()
+    bzs_interpolated = bzs_resampled.interpolate(method='linear')
+    bzs_filtered = bzs_interpolated[detail.tref:detail.tstop]
+    
+
+    ts  = bzs_filtered.index
     for icol, point in enumerate(detail.flow_boundary_point):
-        point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction
+        point.data = pd.Series(bzs_filtered.iloc[:,icol].values, index=ts) + boundary_water_level_correction
+
+    if return_maximum:
+        zmax = -999.0
+        for icol, point in enumerate(detail.flow_boundary_point):
+            zx = point.data.max()
+            if zx>zmax:
+                zs = point.data
+                zmax = zx
+        return zs        
+                    
+    else:    
+        return detail.flow_boundary_point
+
+def nest2_beware_in_sfincs(overall,
+                           detail,
+                           output_path,
+                           output_file,
+                           boundary_water_level_correction,
+                           option):
+
+    if option == 'flow':
+        if not output_file:
+            # Path of the overall output time series
+            output_file = "sfincs_his.nc"
+        
+        point_names = []
+        for point in detail.flow_boundary_point:
+            point_names.append(detail.name + "_" + point.name) #reopen                   
+            # point_names.append(point.name)                    
+        # output_file = os.path.join(output_path, output_file)
+
+        # Return DataFrame bzs
+        bzs = overall.read_timeseries_output(name_list=point_names,
+                                             file_name=os.path.join(output_path,
+                                                                    output_file))
+
+        # Replace -999.0 with zeros. This should not happen, but easy fix for now.
+        bzs = bzs.replace(-999.0,0.0)
+        for icol, point in enumerate(detail.flow_boundary_point):
+            point.data = pd.Series(bzs.iloc[:,icol].values, index=bzs.index) + boundary_water_level_correction    
+            
+
     
 def nest2_hurrywave_in_hurrywave(overall,
                                  detail,
                                  output_path,
-                                 output_file):
-    import xarray as xr
-    import numpy as np
-
+                                 output_file,
+                                 bc_file):
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
     if not output_file:
         output_file = "hurrywave_sp2.nc"
 
     file_name = os.path.join(output_path, output_file)
+    
+    detail.boundary_conditions.forcing = "spectra"
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     stations=ddd.station_name.values
     all_stations = []
     for ist, st in enumerate(stations):
         st=str(st.strip())[2:-1]
         all_stations.append(st)
 
-    point_names = []    
-    if detail.boundary_point:
+    point_names = []
+    if len(detail.boundary_conditions.gdf)>0:
+        for ind, row in detail.boundary_conditions.gdf.iterrows():
         # Find required boundary points        
-        for point in detail.boundary_point:
-            point_names.append(detail.name + "_" + point.name)                    
+            point_names.append(detail.name + "_" + row["name"])                    
         
     else:
         point_names = all_stations.copy()
         
     times   = ddd.point_spectrum2d.coords["time"].values
     sigma   = ddd.point_spectrum2d.coords["sigma"].values
     theta   = ddd.point_spectrum2d.coords["theta"].values
@@ -396,54 +607,175 @@
     ireq = []    
     for ip, point in enumerate(point_names):
         for ist,st in enumerate(all_stations):
             if point.lower() == st.lower():
                 ireq.append(ist)            
                 break
 
-    for ip, point in enumerate(detail.boundary_point):
+    for ind, row in detail.boundary_conditions.gdf.iterrows():
 
-        sp2 = ddd.point_spectrum2d.values[:,ireq[ip],:,:]
+        sp2 = ddd.point_spectrum2d.values[:,ireq[ind],:,:]
 
         ds = xr.Dataset(
                 data_vars = dict(point_spectrum2d=(["time", "theta", "sigma"], sp2)),
                 coords    = dict(time=times,
                                  theta=theta,
                                  sigma=sigma)
                 )
-        
-        point.data = ds
-            
-    # point_names = []
-    # for point in detail.flow_boundary_point:
-    #     point_names.append(detail.name + "_" + point.name)                    
-    # zstfile = os.path.join(output_path, output_file)
-
-    # # Return DataFrame bzs
-    # bzs = overall.read_timeseries_output(name_list=point_names,
-    #                                      file_name=zstfile)
-
-    # ts  = bzs.index
-    # for icol, point in enumerate(detail.flow_boundary_point):
-    #     point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction
+        detail.boundary_conditions.gdf.loc[ind, "spectra"] = ds.to_array()
+
+    if bc_file is not None:
+        detail.boundary_conditions.write_boundary_conditions_spectra(file_name=bc_file)
      
 def nest2_xbeach_in_hurrywave(overall,
                               detail,
                               output_path,
                               output_file,
-                              option='sp2'):
-    import xarray as xr
-    import numpy as np
+                              option,
+                              return_maximum=False):
+    if not output_path:
+        # Path of the overall output time series
+        output_path = overall.path
+
+    if option == "sp2":    
+        if not output_file:
+            output_file = "hurrywave_sp2.nc"
+    
+        file_name = os.path.join(output_path, output_file)
+    
+        # Open netcdf file
+        ddd = xr.open_dataset(file_name)
+        stations=ddd.station_name.values
+        all_stations = []
+        for ist, st in enumerate(stations):
+            st=str(st.strip())[2:-1]
+            all_stations.append(st)
+    
+        point_names = []    
+        if detail.wave_boundary_point:
+            # Find required boundary points        
+            for point in detail.wave_boundary_point:
+                point_names.append(detail.name + "_" + point.name)                    
+            
+        else:
+            point_names = all_stations.copy()
+            
+        times   = ddd.point_spectrum2d.coords["time"].values
+        sigma   = ddd.point_spectrum2d.coords["sigma"].values
+        theta   = ddd.point_spectrum2d.coords["theta"].values
+    
+        ireq = []    
+        for ip, point in enumerate(point_names):
+            for ist,st in enumerate(all_stations):
+                if point.lower() == st.lower():
+                    ireq.append(ist)            
+                    break
+    
+        for ip, point in enumerate(detail.wave_boundary_point):
+    
+            sp2 = ddd.point_spectrum2d.values[:,ireq[ip],:,:]
+    
+            ds = xr.Dataset(
+                    data_vars = dict(point_spectrum2d=(["time", "theta", "sigma"], sp2)),
+                    coords    = dict(time=times,
+                                     theta=theta,
+                                     sigma=sigma)
+                    )
+            
+            point.data = ds
+
+    elif option == "timeseries":
 
+        if not output_file:
+            output_file = "hurrywave_his.nc"
+
+        file_name = os.path.join(output_path, output_file)
+    
+        # Open netcdf file
+        ddd = xr.open_dataset(file_name)
+        stations=ddd.station_name.values
+        all_stations = []
+        for ist, st in enumerate(stations):
+            st=str(st.strip())[2:-1]
+            all_stations.append(st)
+    
+        point_names = []    
+        if detail.wave_boundary_point:
+            # Find required boundary points        
+            for point in detail.wave_boundary_point:
+                point_names.append(detail.name + "_" + point.name)                    
+            
+        else:
+            point_names = all_stations.copy()
+            
+        times   = ddd.point_hm0.coords["time"].values
+
+        ireq = []    
+        for ip, point in enumerate(point_names):
+            for ist,st in enumerate(all_stations):
+                if point.lower() == st.lower():
+                    ireq.append(ist)            
+                    break
+    
+        for ip, point in enumerate(detail.wave_boundary_point):
+    
+            hm0     = ddd.point_hm0.values[:,ireq[ip]]
+            tp      = ddd.point_tp.values[:,ireq[ip]]
+            
+            #set wavedir such that waves are forced perpendicular to coast instead of real direction
+            wavdir =  np.mean([detail.params["thetamin"], detail.params["thetamax"]])
+            #wavdir  = ddd.point_wavdir.values[:,ireq[ip]]
+            
+            #convert directional spread in degrees to xbeach spreading parameter
+            dirspr  = ddd.point_dirspr.values[:,ireq[ip]]
+            s = 2/(dirspr*np.pi/180)**2 - 1
+            
+    
+            df = pd.DataFrame(index=times)
+            df.insert(0,"hm0",hm0)
+            df.insert(1,"tp",tp)
+            df.insert(2,"wavdir",wavdir)
+            df.insert(3,'gammajsp', 3.3)
+            df.insert(4,"s",s)
+    
+            #resample to half-hourly data
+            df_resampled = df.resample('30min').max()
+            df_interpolated = df_resampled.interpolate(method='linear')
+            mask = (df_interpolated.index >= detail.tref) & (df_interpolated.index <= detail.tstop)
+            df_filtered = df_interpolated[mask]
+    
+            df_filtered.insert(5,'duration', 1800)
+            df_filtered.insert(6,"dtbc",1)
+            
+            point.data = df_filtered
+
+    if return_maximum:
+        hmax = -999.0
+        for icol, point in enumerate(detail.wave_boundary_point):
+            hx = point.data["hm0"].max()
+            if hx>hmax:
+                hmx = point.data["hm0"]
+                hmax = hx
+        return hmx        
+                    
+    else:    
+        return detail.flow_boundary_point
+
+
+def nest2_sfincs_in_hurrywave(overall,
+                              detail,
+                              output_path,
+                              output_file):
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
     if not output_file:
-        output_file = "hurrywave_sp2.nc"
+        output_file = "hurrywave_his.nc"
+
 
     file_name = os.path.join(output_path, output_file)
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     stations=ddd.station_name.values
     all_stations = []
@@ -456,44 +788,42 @@
         # Find required boundary points        
         for point in detail.wave_boundary_point:
             point_names.append(detail.name + "_" + point.name)                    
         
     else:
         point_names = all_stations.copy()
         
-    times   = ddd.point_spectrum2d.coords["time"].values
-    sigma   = ddd.point_spectrum2d.coords["sigma"].values
-    theta   = ddd.point_spectrum2d.coords["theta"].values
+    times   = ddd.point_hm0.coords["time"].values
 
     ireq = []    
     for ip, point in enumerate(point_names):
         for ist,st in enumerate(all_stations):
             if point.lower() == st.lower():
                 ireq.append(ist)            
                 break
 
     for ip, point in enumerate(detail.wave_boundary_point):
 
-        sp2 = ddd.point_spectrum2d.values[:,ireq[ip],:,:]
+        hm0     = ddd.point_hm0.values[:,ireq[ip]]
+        tp      = ddd.point_tp.values[:,ireq[ip]]
+        wavdir  = ddd.point_wavdir.values[:,ireq[ip]]
+        dirspr  = ddd.point_dirspr.values[:,ireq[ip]]
 
-        ds = xr.Dataset(
-                data_vars = dict(point_spectrum2d=(["time", "theta", "sigma"], sp2)),
-                coords    = dict(time=times,
-                                 theta=theta,
-                                 sigma=sigma)
-                )
-        
-        point.data = ds
+        df = pd.DataFrame(index=times)
+        df.insert(0,"hm0",hm0)
+        df.insert(1,"tp",tp)
+        df.insert(2,"wavdir",wavdir)
+        df.insert(3,"dirspr",dirspr)
 
-def nest2_sfincs_in_hurrywave(overall,
+        point.data = df
+
+def nest2_beware_in_hurrywave(overall,
                               detail,
                               output_path,
                               output_file):
-    import xarray as xr
-    import numpy as np
 
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
     if not output_file:
         output_file = "hurrywave_his.nc"
@@ -537,15 +867,125 @@
         df.insert(0,"hm0",hm0)
         df.insert(1,"tp",tp)
         df.insert(2,"wavdir",wavdir)
         df.insert(3,"dirspr",dirspr)
 
         point.data = df
 
+
 def nest2_sfincs_in_beware(overall,
                            detail,
                            output_path,
                            output_file,
-                           option='sp2'):
-    import xarray as xr
-    import numpy as np
+                           boundary_water_level_correction,
+                           option):
+
+    from cht.sfincs.sfincs import FlowBoundaryPoint
+    from cht.sfincs.sfincs import WaveMakerForcingPoint
+
+    # Get bounding box for sfincs model
+    # Convert bbox to beware crs
+    x_range, y_range = detail.bounding_box(crs=overall.crs)
+    dx = (x_range[1] - x_range[0])/10
+    dy = (y_range[1] - y_range[0])/10
+    x_range[0] = x_range[0] - dx
+    x_range[1] = x_range[1] + dx
+    y_range[0] = y_range[0] - dy
+    y_range[1] = y_range[1] + dy
+    
+    # Read BEWARE offshore locations
+    if not output_path:
+        # Path of the overall output time series
+        output_path = overall.path
+        
+    if not output_file:
+        output_file = "beware_his.nc"
+
+    file_name = os.path.join(output_path, output_file)
+
+    # Open netcdf file
+    ddd = xr.open_dataset(file_name)
+    
+    if option == "flow":
+    
+        xb = ddd.x_off.values
+        yb = ddd.y_off.values
+        
+        # Find beware locations in bounding box
+        inear = np.where((xb>x_range[0]) & (xb<x_range[1]) & (yb>y_range[0]) & (yb<y_range[1]))    
+        xb=xb[inear]
+        yb=yb[inear]
+        nb = xb.size
+        
+        # Clear existing flow boundary points
+        detail.flow_boundary_point = []
+    
+        # Convert to coordinate system of detail model
+        transformer = Transformer.from_crs(overall.crs,
+                                           detail.crs,
+                                           always_xy=True)
+        
+        for ip in range(nb):
+            name = str(ip + 1).zfill(4)        
+            x, y = transformer.transform(xb[ip], yb[ip])
+            point = FlowBoundaryPoint(x,
+                                      y,
+                                      name=name)
+            detail.flow_boundary_point.append(point)
+        
+        # Extract data and set water level boundary conditions
+        tref = datetime.datetime(1970,1,1)
+        tsec = ddd.time.values # array of int64
+        times = tref + tsec*datetime.timedelta(seconds=1)
+        
+        for ip, point in enumerate(detail.flow_boundary_point):
+            point.data = pd.Series(ddd.WL.values[inear[0][ip],:], index=times) + boundary_water_level_correction
+
+    elif option == "wave":
+
+        xb = ddd.x_coast.values
+        yb = ddd.y_coast.values
+        
+        # Find beware locations in bounding box
+        inear = np.where((xb>x_range[0]) & (xb<x_range[1]) & (yb>y_range[0]) & (yb<y_range[1]))    
+        xb=xb[inear]
+        yb=yb[inear]
+        nb = xb.size
+        
+        # Clear existing flow boundary points
+        detail.wavemaker_forcing_point = []
+    
+        # Convert to coordinate system of detail model
+        transformer = Transformer.from_crs(overall.crs,
+                                           detail.crs,
+                                           always_xy=True)
+        
+        for ip in range(nb):
+            name = str(ip + 1).zfill(4)        
+            x, y = transformer.transform(xb[ip], yb[ip])
+            point = WaveMakerForcingPoint(x,
+                                          y,
+                                          name=name)
+            detail.wavemaker_forcing_point.append(point)
+        
+        # Extract data and set water level boundary conditions
+        tref = datetime.datetime(1970,1,1)
+        tsec = ddd.time.values # array of int64
+        times = tref + tsec*datetime.timedelta(seconds=1)
+        
+        for ip, point in enumerate(detail.wavemaker_forcing_point):
+
+            df = pd.DataFrame()
+            df["hm0_ig"] = ddd.obs_hm0_ig.values[inear[0][ip],:]
+            df["tp_ig"]  = ddd.obs_tpig.values[inear[0][ip],:]
+            df["setup"]  = ddd.obs_setup.values[inear[0][ip],:]
+            df["time"]   = times
+            df = df.set_index("time")
+            
+            df["hm0_ig"]=df["hm0_ig"].replace(np.nan, 0.1)
+            df["tp_ig"]=df["tp_ig"].replace(np.nan, 60.0)
+            df["setup"]=df["setup"].replace(np.nan, 0.0)
+            
+            point.data = df
+
+    ddd.close()
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/sfincs.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/sfincs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat May 15 08:08:40 2021
 
 @author: ormondt
 """
+import sys
 import os
 import pandas as pd
 import datetime
 #import gdal
 #import subprocess
 import numpy as np
 #from matplotlib import pyplot as plt
 from pandas.tseries.offsets import DateOffset
 import xarray as xr
 
 import math
 from pyproj import CRS
 from pyproj import Transformer
 
-from cht.geometry import RegularGrid
-from cht.geometry import Point
-from cht.deltares_ini import IniStruct
-from cht import tiling
+from cht.misc.geometry import RegularGrid
+from cht.misc.geometry import Point
+from cht.misc.deltares_ini import IniStruct
+from cht.tiling import tiling
 
 class SFINCS:
     
     def __init__(self, input_file=None, crs=None):
  
 #        self.epsg                     = epsg
         self.input                    = SfincsInput()
@@ -97,14 +98,19 @@
         fid = open(input_file, "w")
         for key, value in self.input.__dict__.items():
             if not value is None:
                 if type(value) == "float":
                     string = f'{key.ljust(20)} = {float(value)}\n'
                 elif type(value) == "int":
                     string = f'{key.ljust(20)} = {int(value)}\n'
+                elif type(value) == list:
+                    valstr = ""
+                    for v in value:
+                        valstr += str(v) + " "
+                    string = f'{key.ljust(20)} = {valstr}\n'
                 elif isinstance(value, datetime.date):
                     dstr = value.strftime("%Y%m%d %H%M%S")
                     string = f'{key.ljust(20)} = {dstr}\n'
                 else:
                     string = f'{key.ljust(20)} = {value}\n'                
                 fid.write(string)
         fid.close()    
@@ -115,14 +121,18 @@
 #        self.grid = SfincsGrid()
 
         # Flow boundary conditions
         self.read_flow_boundary_points()
         self.read_flow_boundary_conditions()
         self.read_astro_boundary_conditions()
 
+        # Wave boundary conditions
+        self.read_wave_boundary_points()
+        # self.read_wave_boundary_conditions()
+
         # Observation points
         self.read_observation_points()
 
 #        self.grid.compute_coordinates(x0,y0,dx,dy,nx,ny,rotation)
     
     def read_index_file(self):
         pass
@@ -181,19 +191,19 @@
                                      self.input.bndfile)
             
         if not file_name:
             return
             
         fid = open(file_name, "w")
         for point in self.flow_boundary_point:
-            string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}"\n'
+            string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}\n'
             fid.write(string)
         fid.close()    
 
-    ### Flow Boundary points ###
+    ### Flow Boundary conditions ###
     
     def read_flow_boundary_conditions(self, file_name=None):
 
         # Read SFINCS bzs file
         
         if not file_name:
             if not self.input.bzsfile:
@@ -261,22 +271,21 @@
             point.astro = d.section[ind].data
 
     def generate_bzs_from_bca(self,
                               file_name=None,
                               dt=600.0,
                               offset=0.0,
                               write_file=True):
-        import sys
 #        sys.path.append(r'd:/checkouts/OpenEarthTools/trunk/python/applications/DeltaShell/applications/CoDeS/CoDeS_2.0/Tide/pytides/')
         
         if not self.flow_boundary_point:
             print("No boundary points found!")
             return
 
-        from tide_predict import predict
+        from cht.tide.tide_predict import predict
 
         if not file_name:
             if not self.input.bzsfile:
                 self.input.bzsfile = "sfincs.bzs"
             file_name = self.input.bzsfile
 
         times = pd.date_range(start=self.input.tstart,
@@ -297,19 +306,19 @@
 
     def read_wave_boundary_points(self):
         
         # Read SFINCS bnd file
         
         self.wave_boundary_point = []
         
-        if not self.input.bwvfile:
+        if not self.input.snapwave_bndfile:
             return
                     
         bnd_file = os.path.join(self.path,
-                                self.input.bwvfile)
+                                self.input.snapwave_bndfile)
 
         if not os.path.exists(bnd_file):
             return
         
         # Read the bnd file
         df = pd.read_csv(bnd_file, index_col=False, header=None,
              delim_whitespace=True, names=['x', 'y'])
@@ -318,84 +327,198 @@
         for ind in range(len(df.x.values)):
             name = str(ind + 1).zfill(4)
             point = WaveBoundaryPoint(df.x.values[ind],
                                       df.y.values[ind],
                                       name=name)
             self.wave_boundary_point.append(point)
 
-    def write_wave_boundary_conditions(self, file_name=None):
+    def write_wave_boundary_points(self, file_name=None):
 
-        # # Write SFINCS bhs file
-        # if not file_name:
-        #     if not self.input.bzsfile:
-        #         return
-        #     file_name = os.path.join(self.path,
-        #                              self.input.bzsfile)
+        # Write SFINCS bnd file
+        if not file_name:
+            if not self.input.snapwave_bndfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.snapwave_bndfile)
             
-        # if not file_name:
-        #     return
+        if not file_name:
+            return
+            
+        fid = open(file_name, "w")
+        for point in self.wave_boundary_point:
+            string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}\n'
+            fid.write(string)
+        fid.close()    
 
-        # Hm0
+    def write_wavemaker_forcing_points(self, file_name=None):
+
+        # Write SFINCS bfp file
+        if not file_name:
+            if not self.input.wfpfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.wfpfile)
+            
+        if not file_name:
+            return
+            
+        fid = open(file_name, "w")
+        for point in self.wavemaker_forcing_point:
+            string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}\n'
+            fid.write(string)
+        fid.close()    
+
+    def write_wave_boundary_conditions(self):
         
-        file_name = os.path.join(self.path,
-                                 "snapwave.bhs")        
-        # Build a new DataFrame
+        # Hm0, Tp, etc given (probably forced with SnapWave)
+        self.write_bhs_file()
+        self.write_btp_file()
+        self.write_bwd_file()
+        self.write_bds_file()            
+
+    def write_wavemaker_forcing_conditions(self):
+        
+        # Hm0_ig given (probably forced with BEWARE, or something)
+        self.write_whi_file()
+        self.write_wti_file()
+        self.write_wst_file()
+
+            
+    def write_bhs_file(self, file_name=None):
+        # Hm0
+        if not file_name:
+            if not self.input.snapwave_bhsfile:
+                return
+            file_name = os.path.join(self.path,
+                                      self.input.snapwave_bhsfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["hm0"]], axis=1)
-        tmsec = pd.to_timedelta(df.index - self.input.tref, unit="s")
+        tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.3f")
 
-        file_name = os.path.join(self.path,
-                                 "snapwave.btp")        
-        # Build a new DataFrame
+    def write_btp_file(self, file_name=None):
+        # Tp
+        if not file_name:
+            if not self.input.snapwave_btpfile:
+                return
+            file_name = os.path.join(self.path,
+                                      self.input.snapwave_btpfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["tp"]], axis=1)
-        tmsec = pd.to_timedelta(df.index - self.input.tref, unit="s")
+        tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.1f")
 
-        file_name = os.path.join(self.path,
-                                 "snapwave.bwd")        
-        # Build a new DataFrame
+    def write_bwd_file(self, file_name=None):
+        # WavDir
+        if not file_name:
+            if not self.input.snapwave_bwdfile:
+                return
+            file_name = os.path.join(self.path,
+                                      self.input.snapwave_bwdfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["wavdir"]], axis=1)
-        tmsec = pd.to_timedelta(df.index - self.input.tref, unit="s")
+        tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.1f")
 
-        file_name = os.path.join(self.path,
-                                 "snapwave.bds")        
-        # Build a new DataFrame
+    def write_bds_file(self, file_name=None):
+        # DirSpr
+        if not file_name:
+            if not self.input.snapwave_bdsfile:
+                return
+            file_name = os.path.join(self.path,
+                                      self.input.snapwave_bdsfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["dirspr"]], axis=1)
-        tmsec = pd.to_timedelta(df.index - self.input.tref, unit="s")
+        tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.1f")
 
+            
+
+
+    def write_whi_file(self, file_name=None):
+
+        # Hm0 ig
+        if not file_name:
+            if not self.input.whifile:
+                return
+            file_name = os.path.join(self.path,
+                                      self.input.whifile)
+        df = pd.DataFrame()
+        for point in self.wavemaker_forcing_point:
+            df = pd.concat([df, point.data["hm0_ig"]], axis=1)
+        tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
+        df.index = tmsec.total_seconds()
+        df.to_csv(file_name,
+                  index=True,
+                  sep=" ",
+                  header=False,
+                  float_format="%0.3f")
+
+    def write_wti_file(self, file_name=None):
+
+        # Tp ig
+        if not file_name:
+            if not self.input.wtifile:
+                return
+            file_name = os.path.join(self.path,
+                                      self.input.wtifile)
+        df = pd.DataFrame()
+        for point in self.wavemaker_forcing_point:
+            df = pd.concat([df, point.data["tp_ig"]], axis=1)
+        tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
+        df.index = tmsec.total_seconds()
+        df.to_csv(file_name,
+                  index=True,
+                  sep=" ",
+                  header=False,
+                  float_format="%0.1f")
+
+    def write_wst_file(self, file_name=None):
+
+        # Set-up
+        if not file_name:
+            if not self.input.wstfile:
+                return
+            file_name = os.path.join(self.path,
+                                      self.input.wstfile)
+        df = pd.DataFrame()
+        for point in self.wavemaker_forcing_point:
+            df = pd.concat([df, point.data["setup"]], axis=1)
+        tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
+        df.index = tmsec.total_seconds()
+        df.to_csv(file_name,
+                  index=True,
+                  sep=" ",
+                  header=False,
+                  float_format="%0.3f")
+
     ### Observation points ###
 
     def add_observation_point(self, x, y, name):
                 
         self.observation_point.append(ObservationPoint(x, y, name, crs=None))
 
     def read_observation_points(self, file_name=None):
@@ -439,23 +562,34 @@
                 string = f'{point.geometry.x:12.6f}{point.geometry.y:12.6f}  "{point.name}"\n'
                 fid.write(string)
             fid.close()
         
             
     ### Output ###
 
-    def read_timeseries_output(self, name_list = None, file_name = None):
-    
+    def read_timeseries_output(self,
+                               name_list=None,
+                               file_name=None,
+                               parameter="point_zs",
+                               path=None,
+                               ensemble_member_index=None):
+
+        if path is None:
+            if hasattr(self, "path"):
+                path = self.path
+            else:
+                path = os.getcwd()
+
         # Returns a dataframe with timeseries
         if self.input.outputformat[0:3] == "bin":
             
             # ASCII output
     
             if not file_name:
-                file_name = os.path.join(self.path, "zst.txt")
+                file_name = os.path.join(path, "zst.txt")
         
             if not self.observation_point:
                 # First read observation points
                 self.read_observation_points()
             
             columns = []
             for point in self.observation_point:
@@ -469,59 +603,98 @@
             if name_list:
                 df = df[name_list]
             
         else:
             
             # NetCDF output
             if not file_name:
-                file_name = os.path.join(self.path, "sfincs_his.nc")
+                file_name = "sfincs_his.nc"
+
+            # Check if file_name has a path
+            if not os.path.dirname(file_name):
+                # file_name has no path 
+                file_name = os.path.join(path, file_name)
                     
             # Open netcdf file
             ddd = xr.open_dataset(file_name)
 #            stations=ddd.point_zs.coords["station_name"].values
             stations=ddd.station_name.values
             all_stations = []
             for ist, st in enumerate(stations):
 #                st=str(st)[2:-1]
                 all_stations.append(st.decode().strip())
             
-            times   = ddd.point_zs.coords["time"].values
+
+            times   = ddd[parameter].coords["time"].values
     
             # If name_list is empty, add all points    
             if not name_list:
                 name_list = []
                 for st in all_stations:
                     name_list.append(st)
             
             df = pd.DataFrame(index=times, columns=name_list)
-            
+
             for station in name_list:
                 for ist, st in enumerate(all_stations):
                     if station == st:
-                        wl = ddd.point_zs.values[:,ist]
+                        if ensemble_member_index is None:
+                            wl = ddd[parameter].values[:,ist]
+                        else:
+                            wl = ddd[parameter].values[:,ist,ensemble_member_index]    
                         wl[np.isnan(wl)] = -999.0
                         df[st]=wl
                         break            
     
             ddd.close()
                     
         return df    
 
-    def read_zsmax(self, time_range=None, zsmax_file=None, output="grid"):
+    def read_zsmax(self, time_range=None, zsmax_file=None, output="grid", varname='zsmax'):
     
         if not zsmax_file:
-            zsmax_file = os.path.join(self.path, "zsmax.dat")
+            if self.input.outputformat[0:3] == "net":
+                zsmax_file = os.path.join(self.path, "sfincs_map.nc")
+            else:
+                zsmax_file = os.path.join(self.path, "zsmax.dat")
             
 
         if self.input.outputformat[0:3] == "net":
-            ddd=xr.open_dataset(zsmax_file)
+#            ddd=xr.open_dataset(zsmax_file)
 #            zsmx=ddd.zsmax.values
-            zsmax=np.transpose(np.nanmax(ddd.zsmax.values, axis=0))
+#            zsmax=np.transpose(np.nanmax(ddd.zsmax.values, axis=0))
+            
+
+            dsin = xr.open_dataset(zsmax_file)
+
+            output_times = dsin.timemax.values
+            if time_range is None:
+                t0 = pd.to_datetime(str(output_times[0])).replace(tzinfo=None).to_pydatetime()
+                t1 = pd.to_datetime(str(output_times[-1])).replace(tzinfo=None).to_pydatetime()
+                time_range = [t0, t1]
+
+            it0 = -1
+            for it, time in enumerate(output_times):
+                time = pd.to_datetime(str(time)).replace(tzinfo=None).to_pydatetime()
+                if time>=time_range[0] and it0<0:
+                    it0 = it
+                if time<=time_range[1]:
+                    it1 = it
+
+            if self.input.qtrfile:
+                zsmax = np.nanmax(dsin[varname].values[it0:it1 + 1,:], axis=0)
+            else:                
+                zsmax = np.transpose(np.nanmax(dsin[varname].values[it0:it1 + 1,:,:], axis=0))
+                zsmax = np.nanmax(dsin[varname].values[it0:it1 + 1,:,:], axis=0)
+            dsin.close()
+
             return zsmax
 
+
+
         else:
         
             ind_file = os.path.join(self.path, self.input.indexfile)
     
             freqstr = str(self.input.dtmaxout) + "S"
             output_times = pd.date_range(start=self.input.tstart,
                                          end=self.input.tstop,
@@ -556,14 +729,100 @@
                 zs_da[data_ind - 1] = np.squeeze(data_zs)
                 zs_da = np.where(zs_da == -999, np.nan, zs_da)
                 zs_da = np.transpose(np.reshape(zs_da, [mmax, nmax]))
                 return zs_da
             else:
                 return data_zs
             
+    def read_cumulative_precipitation(self, time_range=None, file_name=None, output="grid"):
+    
+        if not file_name:
+            file_name = os.path.join(self.path, "cumprcp.dat")
+            
+
+        if self.input.outputformat[0:3] == "net":
+
+            ddd=xr.open_dataset(file_name)
+            
+            # freqstr = str(self.input.dtmaxout) + "S"
+            # output_times = pd.date_range(start=self.input.tstart,
+            #                              end=self.input.tstop,
+            #                              freq=freqstr).to_pydatetime().tolist()
+            
+ #           output_times = ddd.timemax.values
+#            output_times = ddd.timemax.values.astype(datetime.datetime)
+#            nt = len(output_times)
+
+
+            output_times = ddd.timemax.values
+            if time_range is None:
+
+                t0 = pd.to_datetime(str(output_times[0])).replace(tzinfo=None).to_pydatetime()
+                t1 = pd.to_datetime(str(output_times[-1])).replace(tzinfo=None).to_pydatetime()
+                time_range = [t0, t1]
+
+
+            
+            # if time_range is None:
+            #     time_range = [self.input.tstart, self.input.tstop]
+            
+            for it, time in enumerate(output_times):
+                t = pd.to_datetime(str(time)).replace(tzinfo=None).to_pydatetime()
+                if t<=time_range[0]:
+                    it0 = it
+                if t<=time_range[1]:
+                    it1 = it
+            
+#            pall = ddd.cumprcp.values[it0:it1,:,:]            
+#            psum = 
+            p = np.transpose(np.sum(ddd.cumprcp.values[it0:it1,:,:], axis=0))
+
+            return p
+
+        # else:
+        
+        #     ind_file = os.path.join(self.path, self.input.indexfile)
+    
+        #     freqstr = str(self.input.dtmaxout) + "S"
+        #     output_times = pd.date_range(start=self.input.tstart,
+        #                                  end=self.input.tstop,
+        #                                  freq=freqstr).to_pydatetime().tolist()
+        #     nt = len(output_times)
+            
+        #     if time_range is None:
+        #         time_range = [self.input.tstart, self.input.tstop]
+            
+        #     for it, time in enumerate(output_times):
+        #         if time<=time_range[0]:
+        #             it0 = it
+        #         if time<=time_range[1]:
+        #             it1 = it
+    
+        #     # Get maximum values
+        #     nmax = self.input.nmax
+        #     mmax = self.input.mmax
+                            
+        #     # Read sfincs.ind
+        #     data_ind = np.fromfile(ind_file, dtype="i4")
+        #     npoints  = data_ind[0]
+        #     data_ind = np.squeeze(data_ind[1:])
+            
+        #     # Read zsmax file
+        #     data_zs = np.fromfile(zsmax_file, dtype="f4")
+        #     data_zs = np.reshape(data_zs,[nt, npoints + 2])[it0:it1+1, 1:-1]
+        #     data_zs = np.amax(data_zs, axis=0)
+            
+        #     if output=="grid":
+        #         zs_da = np.full([nmax*mmax], np.nan)        
+        #         zs_da[data_ind - 1] = np.squeeze(data_zs)
+        #         zs_da = np.where(zs_da == -999, np.nan, zs_da)
+        #         zs_da = np.transpose(np.reshape(zs_da, [mmax, nmax]))
+        #         return zs_da
+        #     else:
+        #         return data_zs
         
 #     def write_hmax_geotiff(self, dem_file, index_file, hmax_file, time_range=None, zsmax_file=None):
         
 #         no_datavalue = -9999
     
 #         zs_da = self.read_zsmax(time_range=time_range, zsmax_file=zsmax_file)
 #         zs_da = 100 * zs_da
@@ -659,19 +918,26 @@
             xg, yg = transformer.transform(xg, yg)
         
         xp = [ xg[0,0], xg[0,-1], xg[-1,-1], xg[-1,0], xg[0,0] ]
         yp = [ yg[0,0], yg[0,-1], yg[-1,-1], yg[-1,0], yg[0,0] ]
         
         return xp, yp
         
-    def make_index_tiles(self, path, zoom_range=None):
+    def make_index_tiles(self, path, zoom_range=None, format=0):
+
+        if self.input.qtrfile:
+            from .quadtree import QuadtreeGrid
+            quadtree = QuadtreeGrid(crs=self.crs) 
+            quadtree.load(os.path.join(self.path, self.input.qtrfile))
+            quadtree.make_index_tiles(path, zoom_range=zoom_range)
+            return
         
-        from cht.tiling import deg2num
-        from cht.tiling import num2deg
-        import cht.fileops as fo
+        from cht.tiling.tiling import deg2num
+        from cht.tiling.tiling import num2deg
+        import cht.misc.fileops as fo
         
         if not zoom_range:
             zoom_range = [0, 13]
 
         npix = 256
         
         # Compute lon/lat range
@@ -773,27 +1039,29 @@
         self.nmax = 0
         self.dx   = 10.0
         self.dy   = 10.0
         self.x0   = 0.0
         self.y0   = 0.0
         self.rotation = 0.0
         self.latitude = 0.0
-        self.tref=None
-        self.tstart=None
-        self.tstop=None
+        tnow = datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)
+        self.tref=tnow
+        self.tstart=tnow
+        self.tstop=tnow + datetime.timedelta(days=1)
         self.tspinup=60.0
         self.t0out=None
-        self.dtmapout=600.0
+        self.dtmapout=3600.0
         self.dthisout=600.0
         self.dtrstout=0.0
         self.dtmaxout=0.0
         self.trstout=-999.0
         self.dtwnd=1800.0
-        self.alpha=0.75
-        self.theta=0.90
+        self.alpha=0.5
+        self.theta=1.0
+        self.nuvisc=-999.0
         self.huthresh=0.01
         self.manning=0.04
         self.manning_land=0.04
         self.manning_sea=0.02
         self.rgh_lev_land=0.0
         self.zsini=0.0
         self.qinf=0.0
@@ -807,25 +1075,30 @@
         self.baro=0
         self.pavbnd=0
         self.gapres=101200.0
         self.advlim=9999.9
         self.stopdepth=1000.0
         self.crsgeo=0
         
+        self.qtrfile=None
         self.depfile=None
         self.mskfile=None
         self.indexfile=None
+        self.qtrfile=None
         self.cstfile=None
         self.bndfile=None
         self.bzsfile=None
         self.bzifile=None
         self.bwvfile=None
         self.bhsfile=None
+#        self.bhifile=None
+#        self.bstfile=None
         self.btpfile=None
         self.bwdfile=None
+        self.bdsfile=None
         self.bcafile=None
         self.corfile=None
         self.srcfile=None
         self.disfile=None
         self.inifile=None
         self.sbgfile=None        
         self.spwfile=None
@@ -837,26 +1110,41 @@
         self.precipfile=None
         self.obsfile=None
         self.crsfile=None
         self.thdfile=None
         self.manningfile=None
         self.scsfile=None
         self.rstfile=None
+        self.wfpfile=None
+        self.whifile=None
+        self.wtifile=None
+        self.wstfile=None
         
         self.inputformat="bin"
-        self.outputformat="bin"
+        self.outputformat="net"
         
         self.cdnrb=3
         self.cdwnd=[0.0,28.0,50.0]
         self.cdval=[0.001,0.0025,0.0015]
 
-
-
-
-
+        self.dtwave=None
+        self.snapwave=None
+        self.snapwave_gamma=None
+        self.snapwave_dtheta=None
+        self.snapwave_hmin=None
+        self.snapwave_fw0=None
+        self.snapwave_crit=None
+        self.snapwave_igwaves=None
+        self.snapwave_nrsweeps=None
+        self.snapwave_bhsfile=None
+        self.snapwave_btpfile=None
+        self.snapwave_bwdfile=None
+        self.snapwave_bdsfile=None
+        self.snapwave_encfile=None
+        self.snapwave_bndfile=None
 
 class SfincsGrid():
 
     def __init__(self, x0, y0, dx, dy, nx, ny, rotation):
         self.geometry = RegularGrid(x0, y0, dx, dy, nx, ny, rotation)
 
     # def plot(self,ax):
@@ -944,28 +1232,36 @@
 
     def __init__(self, x, y, name=None, crs=None, data=None):
         
         self.name                   = name
         self.geometry               = Point(x, y, crs=crs)
         self.data                   = data
 
+class WaveMakerForcingPoint():
+
+    def __init__(self, x, y, name=None, crs=None, data=None):
+        
+        self.name                   = name
+        self.geometry               = Point(x, y, crs=crs)
+        self.data                   = data
+
 class ObservationPoint():
 
     def __init__(self, x, y, name, crs=None):
         
         self.name     = name
         self.geometry = Point(x, y, crs=crs)
 
                     
 def read_timeseries_file(file_name, ref_date):
     
     # Returns a dataframe with time series for each of the columns
 
     df = pd.read_csv(file_name, index_col=0, header=None,
-                      delim_whitespace=True)
+                    delim_whitespace=True)
     ts = ref_date + pd.to_timedelta(df.index, unit="s")
     df.index = ts
     
     return df
 
 
 # class QuadtreeGrid():
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/sftp.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/sftp.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/tekal.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/tekal.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/astro.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/astro.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-#   Copyright notice
-#   --------------------------------------------------------------------
-#   Copyright (C) 2020 Deltares
-#       Freek Scheel
-#
-#       freek.scheel@deltares.nl
-#
-#       P.O. Box 177
-#       2600 MH Delft
-#       The Netherlands
-#
-#   This library is free software: you can redistribute it and/or modify
-#   it under the terms of the GNU Lesser General Public License as published by
-#   the Free Software Foundation, either version 3 of the License, or
-#   (at your option) any later version.
-#
-#   This library is distributed in the hope that it will be useful,
-#   but WITHOUT ANY WARRANTY; without even the implied warranty of
-#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#   GNU General Public License for more details.
-#
-#   You should have received a copy of the GNU General Public License
-#   along with this library.  If not, see <http://www.gnu.org/licenses/>.
-#   --------------------------------------------------------------------
-from collections import namedtuple
-import numpy as np
-d2r, r2d = np.pi/180.0, 180.0/np.pi
-
-# Most of this is based around Meeus's Astronomical Algorithms, since it
-# presents reasonably good approximations of all the quantities we require in a
-# clear fashion.  Reluctant to go all out and use VSOP87 unless it can be shown
-# to make a significant difference to the resulting accuracy of harmonic
-# analysis.
-
-#Convert a sexagesimal angle into decimal degrees
-def s2d(degrees, arcmins = 0, arcsecs = 0, mas = 0, muas = 0):
-	return (
-			degrees
-			+ (arcmins /  60.0)
-			+ (arcsecs / (60.0*60.0))
-			+ (mas	   / (60.0*60.0*1e3))
-			+ (muas    / (60.0*60.0*1e6))
-	)
-
-#Evaluate a polynomial at argument
-def polynomial(coefficients, argument):
-	return sum([c * (argument ** i) for i,c in enumerate(coefficients)])
-
-#Evaluate the first derivative of a polynomial at argument
-def d_polynomial(coefficients, argument):
-	return sum([c * i * (argument ** (i-1)) for i,c in enumerate(coefficients)])
-
-#Meeus formula 11.1
-def T(t):
-	return (JD(t) - 2451545.0)/36525
-
-#Meeus formula 7.1
-def JD(t):
-	Y, M = t.year, t.month
-	D = (
-		t.day
-		+ t.hour / (24.0)
-		+ t.minute / (24.0*60.0)
-		+ t.second / (24.0*60.0*60.0)
-		+ t.microsecond / (24.0 * 60.0 * 60.0 * 1e6)
-	)
-	if M <= 2:
-		Y = Y - 1
-		M = M + 12
-	A = np.floor(Y / 100.0)
-	B = 2 - A + np.floor(A / 4.0)
-	return np.floor(365.25*(Y+4716)) + np.floor(30.6001*(M+1)) + D + B - 1524.5
-
-#Meeus formula 21.3
-terrestrial_obliquity_coefficients = (
-	s2d(23,26,21.448),
-	-s2d(0,0,4680.93),
-	-s2d(0,0,1.55),
-	s2d(0,0,1999.25),
-	-s2d(0,0,51.38),
-	-s2d(0,0,249.67),
-	-s2d(0,0,39.05),
-	s2d(0,0,7.12),
-	s2d(0,0,27.87),
-	s2d(0,0,5.79),
-	s2d(0,0,2.45)
-)
-
-#Adjust these coefficients for parameter T rather than U
-terrestrial_obliquity_coefficients = [
-	c * (1e-2) ** i for i,c in enumerate(terrestrial_obliquity_coefficients)
-]
-
-#Not entirely sure about this interpretation, but this is the difference
-#between Meeus formulae 24.2 and 24.3 and seems to work
-solar_perigee_coefficients = (
-	280.46645 - 357.52910,
-	36000.76932 - 35999.05030,
-	0.0003032 + 0.0001559,
-	0.00000048
-)
-
-#Meeus formula 24.2
-solar_longitude_coefficients = (
-	280.46645,
-	36000.76983,
-	0.0003032
-)
-
-#This value is taken from JPL Horizon and is essentially constant
-lunar_inclination_coefficients = (
-	5.145,
-)
-
-#Meeus formula 45.1
-lunar_longitude_coefficients = (
-	218.3164591,
-	481267.88134236,
-	-0.0013268,
-	1/538841.0
-	-1/65194000.0
-)
-
-#Meeus formula 45.7
-lunar_node_coefficients = (
-	125.0445550,
-	-1934.1361849,
-	0.0020762,
-	1/467410.0,
-	-1/60616000.0
-)
-
-#Meeus, unnumbered formula directly preceded by 45.7
-lunar_perigee_coefficients = (
-	83.3532430,
-	4069.0137111,
-	-0.0103238,
-	-1/80053.0,
-	1/18999000.0
-)
-
-#Now follow some useful auxiliary values, we won't need their speed.
-#See notes on Table 6 in Schureman for I, nu, xi, nu', 2nu''
-def _I(N, i, omega):
-	N, i, omega = d2r * N, d2r*i, d2r*omega
-	cosI = np.cos(i)*np.cos(omega)-np.sin(i)*np.sin(omega)*np.cos(N)
-	return r2d*np.arccos(cosI)
-
-def _xi(N, i, omega):
-	N, i, omega = d2r * N, d2r*i, d2r*omega
-	e1 = np.cos(0.5*(omega-i))/np.cos(0.5*(omega+i)) * np.tan(0.5*N)
-	e2 = np.sin(0.5*(omega-i))/np.sin(0.5*(omega+i)) * np.tan(0.5*N)
-	e1, e2 = np.arctan(e1), np.arctan(e2)
-	e1, e2 = e1 - 0.5*N, e2 - 0.5*N
-	return -(e1 + e2)*r2d
-
-def _nu(N, i, omega):
-	N, i, omega = d2r * N, d2r*i, d2r*omega
-	e1 = np.cos(0.5*(omega-i))/np.cos(0.5*(omega+i)) * np.tan(0.5*N)
-	e2 = np.sin(0.5*(omega-i))/np.sin(0.5*(omega+i)) * np.tan(0.5*N)
-	e1, e2 = np.arctan(e1), np.arctan(e2)
-	e1, e2 = e1 - 0.5*N, e2 - 0.5*N
-	return (e1 - e2)*r2d
-
-#Schureman equation 224
-#Can we be more precise than B "the solar coefficient" = 0.1681?
-def _nup(N, i, omega):
-	I = d2r * _I(N, i, omega)
-	nu = d2r * _nu(N, i, omega)
-	return r2d * np.arctan(np.sin(2*I)*np.sin(nu)/(np.sin(2*I)*np.cos(nu)+0.3347))
-
-#Schureman equation 232
-def _nupp(N, i, omega):
-	I = d2r * _I(N, i, omega)
-	nu = d2r * _nu(N, i, omega)
-	tan2nupp = (np.sin(I)**2*np.sin(2*nu))/(np.sin(I)**2*np.cos(2*nu)+0.0727)
-	return r2d * 0.5 * np.arctan(tan2nupp)
-
-AstronomicalParameter = namedtuple('AstronomicalParameter', ['value', 'speed'])
-
-def astro(t):
-	a = {}
-	#We can use polynomial fits from Meeus to obtain good approximations to
-	#some astronomical values (and therefore speeds).
-	polynomials = {
-			's':     lunar_longitude_coefficients,
-			'h':     solar_longitude_coefficients,
-			'p':     lunar_perigee_coefficients,
-			'N':     lunar_node_coefficients,
-			'pp':    solar_perigee_coefficients,
-			'90':    (90.0,),
-			'omega': terrestrial_obliquity_coefficients,
-			'i':     lunar_inclination_coefficients
-	}
-	#Polynomials are in T, that is Julian Centuries; we want our speeds to be
-	#in the more convenient unit of degrees per hour.
-	dT_dHour = 1 / (24 * 365.25 * 100)
-	for name, coefficients in polynomials.items():
-		a[name] = AstronomicalParameter(
-				np.mod(polynomial(coefficients, T(t)), 360.0),
-				d_polynomial(coefficients, T(t)) * dT_dHour
-		)
-
-	#Some other parameters defined by Schureman which are dependent on the
-	#parameters N, i, omega for use in node factor calculations. We don't need
-	#their speeds.
-	args = list(each.value for each in [a['N'], a['i'], a['omega']])
-	for name, function in {
-		'I':    _I,
-		'xi':   _xi,
-		'nu':   _nu,
-		'nup':  _nup,
-		'nupp': _nupp
-	}.items():
-		a[name] = AstronomicalParameter(np.mod(function(*args), 360.0), None)
-
-	#We don't work directly with the T (hours) parameter, instead our spanning
-	#set for equilibrium arguments #is given by T+h-s, s, h, p, N, pp, 90.
-	#This is in line with convention.
-	hour = AstronomicalParameter((JD(t) - np.floor(JD(t))) * 360.0, 15.0)
-	a['T+h-s'] = AstronomicalParameter(
-		hour.value + a['h'].value - a['s'].value,
-		hour.speed + a['h'].speed - a['s'].speed
-	)
-	#It is convenient to calculate Schureman's P here since several node
-	#factors need it, although it could be argued that these
-	#(along with I, xi, nu etc) belong somewhere else.
-	a['P'] = AstronomicalParameter(
-		np.mod(a['p'].value -a['xi'].value,360.0),
-		None
-	)
-	return a
+#   Copyright notice
+#   --------------------------------------------------------------------
+#   Copyright (C) 2020 Deltares
+#       Freek Scheel
+#
+#       freek.scheel@deltares.nl
+#
+#       P.O. Box 177
+#       2600 MH Delft
+#       The Netherlands
+#
+#   This library is free software: you can redistribute it and/or modify
+#   it under the terms of the GNU Lesser General Public License as published by
+#   the Free Software Foundation, either version 3 of the License, or
+#   (at your option) any later version.
+#
+#   This library is distributed in the hope that it will be useful,
+#   but WITHOUT ANY WARRANTY; without even the implied warranty of
+#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#   GNU General Public License for more details.
+#
+#   You should have received a copy of the GNU General Public License
+#   along with this library.  If not, see <http://www.gnu.org/licenses/>.
+#   --------------------------------------------------------------------
+from collections import namedtuple
+import numpy as np
+d2r, r2d = np.pi/180.0, 180.0/np.pi
+
+# Most of this is based around Meeus's Astronomical Algorithms, since it
+# presents reasonably good approximations of all the quantities we require in a
+# clear fashion.  Reluctant to go all out and use VSOP87 unless it can be shown
+# to make a significant difference to the resulting accuracy of harmonic
+# analysis.
+
+#Convert a sexagesimal angle into decimal degrees
+def s2d(degrees, arcmins = 0, arcsecs = 0, mas = 0, muas = 0):
+	return (
+			degrees
+			+ (arcmins /  60.0)
+			+ (arcsecs / (60.0*60.0))
+			+ (mas	   / (60.0*60.0*1e3))
+			+ (muas    / (60.0*60.0*1e6))
+	)
+
+#Evaluate a polynomial at argument
+def polynomial(coefficients, argument):
+	return sum([c * (argument ** i) for i,c in enumerate(coefficients)])
+
+#Evaluate the first derivative of a polynomial at argument
+def d_polynomial(coefficients, argument):
+	return sum([c * i * (argument ** (i-1)) for i,c in enumerate(coefficients)])
+
+#Meeus formula 11.1
+def T(t):
+	return (JD(t) - 2451545.0)/36525
+
+#Meeus formula 7.1
+def JD(t):
+	Y, M = t.year, t.month
+	D = (
+		t.day
+		+ t.hour / (24.0)
+		+ t.minute / (24.0*60.0)
+		+ t.second / (24.0*60.0*60.0)
+		+ t.microsecond / (24.0 * 60.0 * 60.0 * 1e6)
+	)
+	if M <= 2:
+		Y = Y - 1
+		M = M + 12
+	A = np.floor(Y / 100.0)
+	B = 2 - A + np.floor(A / 4.0)
+	return np.floor(365.25*(Y+4716)) + np.floor(30.6001*(M+1)) + D + B - 1524.5
+
+#Meeus formula 21.3
+terrestrial_obliquity_coefficients = (
+	s2d(23,26,21.448),
+	-s2d(0,0,4680.93),
+	-s2d(0,0,1.55),
+	s2d(0,0,1999.25),
+	-s2d(0,0,51.38),
+	-s2d(0,0,249.67),
+	-s2d(0,0,39.05),
+	s2d(0,0,7.12),
+	s2d(0,0,27.87),
+	s2d(0,0,5.79),
+	s2d(0,0,2.45)
+)
+
+#Adjust these coefficients for parameter T rather than U
+terrestrial_obliquity_coefficients = [
+	c * (1e-2) ** i for i,c in enumerate(terrestrial_obliquity_coefficients)
+]
+
+#Not entirely sure about this interpretation, but this is the difference
+#between Meeus formulae 24.2 and 24.3 and seems to work
+solar_perigee_coefficients = (
+	280.46645 - 357.52910,
+	36000.76932 - 35999.05030,
+	0.0003032 + 0.0001559,
+	0.00000048
+)
+
+#Meeus formula 24.2
+solar_longitude_coefficients = (
+	280.46645,
+	36000.76983,
+	0.0003032
+)
+
+#This value is taken from JPL Horizon and is essentially constant
+lunar_inclination_coefficients = (
+	5.145,
+)
+
+#Meeus formula 45.1
+lunar_longitude_coefficients = (
+	218.3164591,
+	481267.88134236,
+	-0.0013268,
+	1/538841.0
+	-1/65194000.0
+)
+
+#Meeus formula 45.7
+lunar_node_coefficients = (
+	125.0445550,
+	-1934.1361849,
+	0.0020762,
+	1/467410.0,
+	-1/60616000.0
+)
+
+#Meeus, unnumbered formula directly preceded by 45.7
+lunar_perigee_coefficients = (
+	83.3532430,
+	4069.0137111,
+	-0.0103238,
+	-1/80053.0,
+	1/18999000.0
+)
+
+#Now follow some useful auxiliary values, we won't need their speed.
+#See notes on Table 6 in Schureman for I, nu, xi, nu', 2nu''
+def _I(N, i, omega):
+	N, i, omega = d2r * N, d2r*i, d2r*omega
+	cosI = np.cos(i)*np.cos(omega)-np.sin(i)*np.sin(omega)*np.cos(N)
+	return r2d*np.arccos(cosI)
+
+def _xi(N, i, omega):
+	N, i, omega = d2r * N, d2r*i, d2r*omega
+	e1 = np.cos(0.5*(omega-i))/np.cos(0.5*(omega+i)) * np.tan(0.5*N)
+	e2 = np.sin(0.5*(omega-i))/np.sin(0.5*(omega+i)) * np.tan(0.5*N)
+	e1, e2 = np.arctan(e1), np.arctan(e2)
+	e1, e2 = e1 - 0.5*N, e2 - 0.5*N
+	return -(e1 + e2)*r2d
+
+def _nu(N, i, omega):
+	N, i, omega = d2r * N, d2r*i, d2r*omega
+	e1 = np.cos(0.5*(omega-i))/np.cos(0.5*(omega+i)) * np.tan(0.5*N)
+	e2 = np.sin(0.5*(omega-i))/np.sin(0.5*(omega+i)) * np.tan(0.5*N)
+	e1, e2 = np.arctan(e1), np.arctan(e2)
+	e1, e2 = e1 - 0.5*N, e2 - 0.5*N
+	return (e1 - e2)*r2d
+
+#Schureman equation 224
+#Can we be more precise than B "the solar coefficient" = 0.1681?
+def _nup(N, i, omega):
+	I = d2r * _I(N, i, omega)
+	nu = d2r * _nu(N, i, omega)
+	return r2d * np.arctan(np.sin(2*I)*np.sin(nu)/(np.sin(2*I)*np.cos(nu)+0.3347))
+
+#Schureman equation 232
+def _nupp(N, i, omega):
+	I = d2r * _I(N, i, omega)
+	nu = d2r * _nu(N, i, omega)
+	tan2nupp = (np.sin(I)**2*np.sin(2*nu))/(np.sin(I)**2*np.cos(2*nu)+0.0727)
+	return r2d * 0.5 * np.arctan(tan2nupp)
+
+AstronomicalParameter = namedtuple('AstronomicalParameter', ['value', 'speed'])
+
+def astro(t):
+	a = {}
+	#We can use polynomial fits from Meeus to obtain good approximations to
+	#some astronomical values (and therefore speeds).
+	polynomials = {
+			's':     lunar_longitude_coefficients,
+			'h':     solar_longitude_coefficients,
+			'p':     lunar_perigee_coefficients,
+			'N':     lunar_node_coefficients,
+			'pp':    solar_perigee_coefficients,
+			'90':    (90.0,),
+			'omega': terrestrial_obliquity_coefficients,
+			'i':     lunar_inclination_coefficients
+	}
+	#Polynomials are in T, that is Julian Centuries; we want our speeds to be
+	#in the more convenient unit of degrees per hour.
+	dT_dHour = 1 / (24 * 365.25 * 100)
+	for name, coefficients in polynomials.items():
+		a[name] = AstronomicalParameter(
+				np.mod(polynomial(coefficients, T(t)), 360.0),
+				d_polynomial(coefficients, T(t)) * dT_dHour
+		)
+
+	#Some other parameters defined by Schureman which are dependent on the
+	#parameters N, i, omega for use in node factor calculations. We don't need
+	#their speeds.
+	args = list(each.value for each in [a['N'], a['i'], a['omega']])
+	for name, function in {
+		'I':    _I,
+		'xi':   _xi,
+		'nu':   _nu,
+		'nup':  _nup,
+		'nupp': _nupp
+	}.items():
+		a[name] = AstronomicalParameter(np.mod(function(*args), 360.0), None)
+
+	#We don't work directly with the T (hours) parameter, instead our spanning
+	#set for equilibrium arguments #is given by T+h-s, s, h, p, N, pp, 90.
+	#This is in line with convention.
+	hour = AstronomicalParameter((JD(t) - np.floor(JD(t))) * 360.0, 15.0)
+	a['T+h-s'] = AstronomicalParameter(
+		hour.value + a['h'].value - a['s'].value,
+		hour.speed + a['h'].speed - a['s'].speed
+	)
+	#It is convenient to calculate Schureman's P here since several node
+	#factors need it, although it could be argued that these
+	#(along with I, xi, nu etc) belong somewhere else.
+	a['P'] = AstronomicalParameter(
+		np.mod(a['p'].value -a['xi'].value,360.0),
+		None
+	)
+	return a
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/constituent.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/constituent.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-#   Copyright notice
-#   --------------------------------------------------------------------
-#   Copyright (C) 2020 Deltares
-#       Freek Scheel
-#
-#       freek.scheel@deltares.nl
-#
-#       P.O. Box 177
-#       2600 MH Delft
-#       The Netherlands
-#
-#   This library is free software: you can redistribute it and/or modify
-#   it under the terms of the GNU Lesser General Public License as published by
-#   the Free Software Foundation, either version 3 of the License, or
-#   (at your option) any later version.
-#
-#   This library is distributed in the hope that it will be useful,
-#   but WITHOUT ANY WARRANTY; without even the implied warranty of
-#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#   GNU General Public License for more details.
-#
-#   You should have received a copy of the GNU General Public License
-#   along with this library.  If not, see <http://www.gnu.org/licenses/>.
-#   --------------------------------------------------------------------
-
-import string
-import operator as op
-import numpy as np
-from functools import reduce
-import cht.tide.nodal_corrections as nc
-
-class BaseConstituent(object):
-	xdo_int = {
-		'A': 1, 'B': 2, 'C': 3, 'D': 4, 'E': 5, 'F': 6, 'G': 7, 'H': 8, 'I': 9,
-		'J': 10, 'K': 11, 'L': 12, 'M': 13, 'N': 14, 'O': 15, 'P': 16, 'Q': 17,
-		'R': -8, 'S': -7, 'T': -6, 'U': -5, 'V': -4, 'W': -3, 'X': -2, 'Y': -1,
-		'Z': 0
-	}
-
-	int_xdo = {v:k for k, v in xdo_int.items()}
-
-	def __init__(self, name, xdo='', coefficients=[], u=nc.u_zero, f=nc.f_unity):
-		if xdo == '':
-			self.coefficients = np.array(coefficients)
-		else:
-			self.coefficients = np.array(self.xdo_to_coefficients(xdo))
-		self.name = name
-		self.u = u
-		self.f = f
-
-	def xdo_to_coefficients(self, xdo):
-		return [self.xdo_int[l.upper()] for l in xdo if l in string.ascii_letters]
-
-	def coefficients_to_xdo(self, coefficients):
-		return ''.join([self.int_xdo[c] for c in coefficients])
-
-	def V(self, astro):
-		return np.dot(self.coefficients, self.astro_values(astro))
-
-	def xdo(self):
-		return self.coefficients_to_xdo(self.coefficients)
-
-	def speed(self, a):
-		return np.dot(self.coefficients, self.astro_speeds(a))
-
-	def astro_xdo(self, a):
-		return [a['T+h-s'], a['s'], a['h'], a['p'], a['N'], a['pp'], a['90']]
-
-	def astro_speeds(self, a):
-		return np.array([each.speed for each in self.astro_xdo(a)])
-
-	def astro_values(self, a):
-		return np.array([each.value for each in self.astro_xdo(a)])
-
-	#Consider two out of phase constituents which travel at the same speed to
-	#be identical
-	def __eq__(self, c):
-		return np.all(self.coefficients[:-1] == c.coefficients[:-1])
-
-	def __hash__(self):
-		return hash(tuple(self.coefficients[:-1]))
-
-class CompoundConstituent(BaseConstituent):
-
-	def __init__(self, members = [], **kwargs):
-		self.members = members
-
-		if 'u' not in kwargs:
-			kwargs['u'] = self.u
-		if 'f' not in kwargs:
-			kwargs['f'] = self.f
-
-		super(CompoundConstituent,self).__init__(**kwargs)
-
-		self.coefficients = reduce(op.add,[c.coefficients * n for (c,n) in members])
-
-	def speed(self, a):
-		return reduce(op.add, [n * c.speed(a) for (c,n) in self.members])
-
-	def V(self, a):
-		return reduce(op.add, [n * c.V(a) for (c,n) in self.members])
-
-	def u(self, a):
-		return reduce(op.add, [n * c.u(a) for (c,n) in self.members])
-
-	def f(self, a):
-		return reduce(op.mul, [c.f(a) ** abs(n) for (c,n) in self.members])
-
-###### Base Constituents
-#Long Term
-_Z0      = BaseConstituent(name = 'Z0',      xdo = 'Z ZZZ ZZZ', u = nc.u_zero, f = nc.f_unity)
-_Sa      = BaseConstituent(name = 'Sa',      xdo = 'Z ZAZ ZZZ', u = nc.u_zero, f = nc.f_unity)
-_Ssa     = BaseConstituent(name = 'Ssa',     xdo = 'Z ZBZ ZZZ', u = nc.u_zero, f = nc.f_unity)
-_Mm      = BaseConstituent(name = 'Mm',      xdo = 'Z AZY ZZZ', u = nc.u_zero, f = nc.f_Mm)
-_Mf      = BaseConstituent(name = 'Mf',      xdo = 'Z BZZ ZZZ', u = nc.u_Mf, f = nc.f_Mf)
-
-#Diurnals
-_Q1      = BaseConstituent(name = 'Q1',      xdo = 'A XZA ZZA', u = nc.u_O1, f = nc.f_O1)
-_O1      = BaseConstituent(name = 'O1',      xdo = 'A YZZ ZZA', u = nc.u_O1, f = nc.f_O1)
-_K1      = BaseConstituent(name = 'K1',      xdo = 'A AZZ ZZY', u = nc.u_K1, f = nc.f_K1)
-_J1      = BaseConstituent(name = 'J1',      xdo = 'A BZY ZZY', u = nc.u_J1, f = nc.f_J1)
-
-#M1 is a tricky business for reasons of convention, rather than theory.  The
-#reasons for this are best summarised by Schureman paragraphs 126, 127 and in
-#the comments found in congen_input.txt of xtides, so I won't go over all this
-#again here.
-
-_M1      = BaseConstituent(name = 'M1',      xdo = 'A ZZZ ZZA', u = nc.u_M1, f = nc.f_M1)
-_P1      = BaseConstituent(name = 'P1',      xdo = 'A AXZ ZZA', u = nc.u_zero, f = nc.f_unity)
-_S1      = BaseConstituent(name = 'S1',      xdo = 'A AYZ ZZZ', u = nc.u_zero, f = nc.f_unity)
-_OO1     = BaseConstituent(name = 'OO1',     xdo = 'A CZZ ZZY', u = nc.u_OO1, f = nc.f_OO1)
-
-#Semi-Diurnals
-_2N2     = BaseConstituent(name = '2N2',     xdo = 'B XZB ZZZ', u = nc.u_M2, f = nc.f_M2)
-_N2      = BaseConstituent(name = 'N2',      xdo = 'B YZA ZZZ', u = nc.u_M2, f = nc.f_M2)
-_nu2     = BaseConstituent(name = 'nu2',     xdo = 'B YBY ZZZ', u = nc.u_M2, f = nc.f_M2)
-_M2      = BaseConstituent(name = 'M2',      xdo = 'B ZZZ ZZZ', u = nc.u_M2, f = nc.f_M2)
-_lambda2 = BaseConstituent(name = 'lambda2', xdo = 'B AXA ZZB', u = nc.u_M2, f = nc.f_M2)
-_L2      = BaseConstituent(name = 'L2',      xdo = 'B AZY ZZB', u = nc.u_L2, f = nc.f_L2)
-_T2      = BaseConstituent(name = 'T2',      xdo = 'B BWZ ZAZ', u = nc.u_zero, f = nc.f_unity)
-_S2      = BaseConstituent(name = 'S2',      xdo = 'B BXZ ZZZ', u = nc.u_zero, f = nc.f_unity)
-_R2      = BaseConstituent(name = 'R2',      xdo = 'B BYZ ZYB', u = nc.u_zero, f = nc.f_unity)
-_K2      = BaseConstituent(name = 'K2',      xdo = 'B BZZ ZZZ', u = nc.u_K2, f = nc.f_K2)
-
-#Third-Diurnals
-_M3      = BaseConstituent(name = 'M3',      xdo = 'C ZZZ ZZZ', u = lambda a: nc.u_Modd(a,3), f = lambda a: nc.f_Modd(a,3))
-
-###### Compound Constituents
-#Long Term
-_MSF     = CompoundConstituent(name = 'MSF',  members = [(_S2, 1), (_M2, -1)])
-
-#Diurnal
-_2Q1     = CompoundConstituent(name = '2Q1',  members = [(_N2, 1), (_J1, -1)])
-_rho1    = CompoundConstituent(name = 'rho1', members = [(_nu2, 1), (_K1, -1)])
-
-#Semi-Diurnal
-
-_mu2     = CompoundConstituent(name = 'mu2',  members = [(_M2, 2), (_S2, -1)]) #2MS2
-_2SM2    = CompoundConstituent(name = '2SM2', members = [(_S2, 2), (_M2, -1)])
-
-#Third-Diurnal
-_2MK3    = CompoundConstituent(name = '2MK3', members = [(_M2, 1), (_O1, 1)])
-_MK3     = CompoundConstituent(name = 'MK3',  members = [(_M2, 1), (_K1, 1)])
-
-#Quarter-Diurnal
-_MN4     = CompoundConstituent(name = 'MN4',  members = [(_M2, 1), (_N2, 1)])
-_M4      = CompoundConstituent(name = 'M4',   members = [(_M2, 2)])
-_MS4     = CompoundConstituent(name = 'MS4',  members = [(_M2, 1), (_S2, 1)])
-_S4      = CompoundConstituent(name = 'S4',   members = [(_S2, 2)])
-
-#Sixth-Diurnal
-_M6      = CompoundConstituent(name = 'M6',   members = [(_M2, 3)])
-_S6      = CompoundConstituent(name = 'S6',   members = [(_S2, 3)])
-
-#Eighth-Diurnals
-_M8      = CompoundConstituent(name = 'M8',   members = [(_M2, 4)])
-
-
-noaa = [
-	_M2, _S2, _N2, _K1, _M4, _O1, _M6, _MK3, _S4, _MN4, _nu2, _S6, _mu2,
-	_2N2, _OO1, _lambda2, _S1, _M1, _J1, _Mm, _Ssa, _Sa, _MSF, _Mf,
-	_rho1, _Q1, _T2, _R2, _2Q1, _P1, _2SM2, _M3, _L2, _2MK3, _K2,
-	_M8, _MS4
-]
-
+#   Copyright notice
+#   --------------------------------------------------------------------
+#   Copyright (C) 2020 Deltares
+#       Freek Scheel
+#
+#       freek.scheel@deltares.nl
+#
+#       P.O. Box 177
+#       2600 MH Delft
+#       The Netherlands
+#
+#   This library is free software: you can redistribute it and/or modify
+#   it under the terms of the GNU Lesser General Public License as published by
+#   the Free Software Foundation, either version 3 of the License, or
+#   (at your option) any later version.
+#
+#   This library is distributed in the hope that it will be useful,
+#   but WITHOUT ANY WARRANTY; without even the implied warranty of
+#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#   GNU General Public License for more details.
+#
+#   You should have received a copy of the GNU General Public License
+#   along with this library.  If not, see <http://www.gnu.org/licenses/>.
+#   --------------------------------------------------------------------
+
+import string
+import operator as op
+import numpy as np
+from functools import reduce
+import cht.tide.nodal_corrections as nc
+
+class BaseConstituent(object):
+	xdo_int = {
+		'A': 1, 'B': 2, 'C': 3, 'D': 4, 'E': 5, 'F': 6, 'G': 7, 'H': 8, 'I': 9,
+		'J': 10, 'K': 11, 'L': 12, 'M': 13, 'N': 14, 'O': 15, 'P': 16, 'Q': 17,
+		'R': -8, 'S': -7, 'T': -6, 'U': -5, 'V': -4, 'W': -3, 'X': -2, 'Y': -1,
+		'Z': 0
+	}
+
+	int_xdo = {v:k for k, v in xdo_int.items()}
+
+	def __init__(self, name, xdo='', coefficients=[], u=nc.u_zero, f=nc.f_unity):
+		if xdo == '':
+			self.coefficients = np.array(coefficients)
+		else:
+			self.coefficients = np.array(self.xdo_to_coefficients(xdo))
+		self.name = name
+		self.u = u
+		self.f = f
+
+	def xdo_to_coefficients(self, xdo):
+		return [self.xdo_int[l.upper()] for l in xdo if l in string.ascii_letters]
+
+	def coefficients_to_xdo(self, coefficients):
+		return ''.join([self.int_xdo[c] for c in coefficients])
+
+	def V(self, astro):
+		return np.dot(self.coefficients, self.astro_values(astro))
+
+	def xdo(self):
+		return self.coefficients_to_xdo(self.coefficients)
+
+	def speed(self, a):
+		return np.dot(self.coefficients, self.astro_speeds(a))
+
+	def astro_xdo(self, a):
+		return [a['T+h-s'], a['s'], a['h'], a['p'], a['N'], a['pp'], a['90']]
+
+	def astro_speeds(self, a):
+		return np.array([each.speed for each in self.astro_xdo(a)])
+
+	def astro_values(self, a):
+		return np.array([each.value for each in self.astro_xdo(a)])
+
+	#Consider two out of phase constituents which travel at the same speed to
+	#be identical
+	def __eq__(self, c):
+		return np.all(self.coefficients[:-1] == c.coefficients[:-1])
+
+	def __hash__(self):
+		return hash(tuple(self.coefficients[:-1]))
+
+class CompoundConstituent(BaseConstituent):
+
+	def __init__(self, members = [], **kwargs):
+		self.members = members
+
+		if 'u' not in kwargs:
+			kwargs['u'] = self.u
+		if 'f' not in kwargs:
+			kwargs['f'] = self.f
+
+		super(CompoundConstituent,self).__init__(**kwargs)
+
+		self.coefficients = reduce(op.add,[c.coefficients * n for (c,n) in members])
+
+	def speed(self, a):
+		return reduce(op.add, [n * c.speed(a) for (c,n) in self.members])
+
+	def V(self, a):
+		return reduce(op.add, [n * c.V(a) for (c,n) in self.members])
+
+	def u(self, a):
+		return reduce(op.add, [n * c.u(a) for (c,n) in self.members])
+
+	def f(self, a):
+		return reduce(op.mul, [c.f(a) ** abs(n) for (c,n) in self.members])
+
+###### Base Constituents
+#Long Term
+_Z0      = BaseConstituent(name = 'Z0',      xdo = 'Z ZZZ ZZZ', u = nc.u_zero, f = nc.f_unity)
+_Sa      = BaseConstituent(name = 'Sa',      xdo = 'Z ZAZ ZZZ', u = nc.u_zero, f = nc.f_unity)
+_Ssa     = BaseConstituent(name = 'Ssa',     xdo = 'Z ZBZ ZZZ', u = nc.u_zero, f = nc.f_unity)
+_Mm      = BaseConstituent(name = 'Mm',      xdo = 'Z AZY ZZZ', u = nc.u_zero, f = nc.f_Mm)
+_Mf      = BaseConstituent(name = 'Mf',      xdo = 'Z BZZ ZZZ', u = nc.u_Mf, f = nc.f_Mf)
+
+#Diurnals
+_Q1      = BaseConstituent(name = 'Q1',      xdo = 'A XZA ZZA', u = nc.u_O1, f = nc.f_O1)
+_O1      = BaseConstituent(name = 'O1',      xdo = 'A YZZ ZZA', u = nc.u_O1, f = nc.f_O1)
+_K1      = BaseConstituent(name = 'K1',      xdo = 'A AZZ ZZY', u = nc.u_K1, f = nc.f_K1)
+_J1      = BaseConstituent(name = 'J1',      xdo = 'A BZY ZZY', u = nc.u_J1, f = nc.f_J1)
+
+#M1 is a tricky business for reasons of convention, rather than theory.  The
+#reasons for this are best summarised by Schureman paragraphs 126, 127 and in
+#the comments found in congen_input.txt of xtides, so I won't go over all this
+#again here.
+
+_M1      = BaseConstituent(name = 'M1',      xdo = 'A ZZZ ZZA', u = nc.u_M1, f = nc.f_M1)
+_P1      = BaseConstituent(name = 'P1',      xdo = 'A AXZ ZZA', u = nc.u_zero, f = nc.f_unity)
+_S1      = BaseConstituent(name = 'S1',      xdo = 'A AYZ ZZZ', u = nc.u_zero, f = nc.f_unity)
+_OO1     = BaseConstituent(name = 'OO1',     xdo = 'A CZZ ZZY', u = nc.u_OO1, f = nc.f_OO1)
+
+#Semi-Diurnals
+_2N2     = BaseConstituent(name = '2N2',     xdo = 'B XZB ZZZ', u = nc.u_M2, f = nc.f_M2)
+_N2      = BaseConstituent(name = 'N2',      xdo = 'B YZA ZZZ', u = nc.u_M2, f = nc.f_M2)
+_nu2     = BaseConstituent(name = 'nu2',     xdo = 'B YBY ZZZ', u = nc.u_M2, f = nc.f_M2)
+_M2      = BaseConstituent(name = 'M2',      xdo = 'B ZZZ ZZZ', u = nc.u_M2, f = nc.f_M2)
+_lambda2 = BaseConstituent(name = 'lambda2', xdo = 'B AXA ZZB', u = nc.u_M2, f = nc.f_M2)
+_L2      = BaseConstituent(name = 'L2',      xdo = 'B AZY ZZB', u = nc.u_L2, f = nc.f_L2)
+_T2      = BaseConstituent(name = 'T2',      xdo = 'B BWZ ZAZ', u = nc.u_zero, f = nc.f_unity)
+_S2      = BaseConstituent(name = 'S2',      xdo = 'B BXZ ZZZ', u = nc.u_zero, f = nc.f_unity)
+_R2      = BaseConstituent(name = 'R2',      xdo = 'B BYZ ZYB', u = nc.u_zero, f = nc.f_unity)
+_K2      = BaseConstituent(name = 'K2',      xdo = 'B BZZ ZZZ', u = nc.u_K2, f = nc.f_K2)
+
+#Third-Diurnals
+_M3      = BaseConstituent(name = 'M3',      xdo = 'C ZZZ ZZZ', u = lambda a: nc.u_Modd(a,3), f = lambda a: nc.f_Modd(a,3))
+
+###### Compound Constituents
+#Long Term
+_MSF     = CompoundConstituent(name = 'MSF',  members = [(_S2, 1), (_M2, -1)])
+
+#Diurnal
+_2Q1     = CompoundConstituent(name = '2Q1',  members = [(_N2, 1), (_J1, -1)])
+_rho1    = CompoundConstituent(name = 'rho1', members = [(_nu2, 1), (_K1, -1)])
+
+#Semi-Diurnal
+
+_mu2     = CompoundConstituent(name = 'mu2',  members = [(_M2, 2), (_S2, -1)]) #2MS2
+_2SM2    = CompoundConstituent(name = '2SM2', members = [(_S2, 2), (_M2, -1)])
+
+#Third-Diurnal
+_2MK3    = CompoundConstituent(name = '2MK3', members = [(_M2, 1), (_O1, 1)])
+_MK3     = CompoundConstituent(name = 'MK3',  members = [(_M2, 1), (_K1, 1)])
+
+#Quarter-Diurnal
+_MN4     = CompoundConstituent(name = 'MN4',  members = [(_M2, 1), (_N2, 1)])
+_M4      = CompoundConstituent(name = 'M4',   members = [(_M2, 2)])
+_MS4     = CompoundConstituent(name = 'MS4',  members = [(_M2, 1), (_S2, 1)])
+_S4      = CompoundConstituent(name = 'S4',   members = [(_S2, 2)])
+
+#Sixth-Diurnal
+_M6      = CompoundConstituent(name = 'M6',   members = [(_M2, 3)])
+_S6      = CompoundConstituent(name = 'S6',   members = [(_S2, 3)])
+
+#Eighth-Diurnals
+_M8      = CompoundConstituent(name = 'M8',   members = [(_M2, 4)])
+
+
+noaa = [
+	_M2, _S2, _N2, _K1, _M4, _O1, _M6, _MK3, _S4, _MN4, _nu2, _S6, _mu2,
+	_2N2, _OO1, _lambda2, _S1, _M1, _J1, _Mm, _Ssa, _Sa, _MSF, _Mf,
+	_rho1, _Q1, _T2, _R2, _2Q1, _P1, _2SM2, _M3, _L2, _2MK3, _K2,
+	_M8, _MS4
+]
+
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/tide/tide.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,437 +1,436 @@
-#   Copyright notice
-#   --------------------------------------------------------------------
-#   Copyright (C) 2020 Deltares
-#       Freek Scheel
-#
-#       freek.scheel@deltares.nl
-#
-#       P.O. Box 177
-#       2600 MH Delft
-#       The Netherlands
-#
-#   This library is free software: you can redistribute it and/or modify
-#   it under the terms of the GNU Lesser General Public License as published by
-#   the Free Software Foundation, either version 3 of the License, or
-#   (at your option) any later version.
-#
-#   This library is distributed in the hope that it will be useful,
-#   but WITHOUT ANY WARRANTY; without even the implied warranty of
-#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#   GNU General Public License for more details.
-#
-#   You should have received a copy of the GNU General Public License
-#   along with this library.  If not, see <http://www.gnu.org/licenses/>.
-#   --------------------------------------------------------------------
-
-from collections import OrderedDict, Iterable
-from itertools import takewhile, count
-try:
-	from itertools import izip, ifilter
-except ImportError: #Python3
-	izip = zip
-	ifilter = filter
-from datetime import datetime, timedelta
-import numpy as np
-from scipy.optimize import leastsq, fsolve
-from functools import reduce
-
-from .astro import astro
-import cht.tide.constituent as constituent
-#import tide.constituent as constituent
-#import .constituent
-
-d2r, r2d = np.pi/180.0, 180.0/np.pi
-
-class Tide(object):
-	dtype = np.dtype([
-		('constituent', object),
-		('amplitude', float),
-		('phase', float)])
-
-	def __init__(
-			self,
-			constituents = None,
-			amplitudes = None,
-			phases = None,
-			model = None,
-			radians = False
-		):
-		"""
-		Initialise a tidal model. Provide constituents, amplitudes and phases OR a model.
-		Arguments:
-		constituents -- list of constituents used in the model.
-		amplitudes -- list of amplitudes corresponding to constituents
-		phases -- list of phases corresponding to constituents
-		model -- an ndarray of type Tide.dtype representing the constituents, amplitudes and phases.
-		radians -- boolean representing whether phases are in radians (default False)
-		"""
-		if None not in [constituents, amplitudes, phases]:
-			if len(constituents) == len(amplitudes) == len(phases):
-				model = np.zeros(len(phases), dtype=Tide.dtype)
-				model['constituent'] = np.array(constituents)
-				model['amplitude'] = np.array(amplitudes)
-				model['phase'] = np.array(phases)
-			else:
-				raise ValueError("Constituents, amplitudes and phases should all be arrays of equal length.")
-		elif model is not None:
-			if not model.dtype == Tide.dtype:
-				raise ValueError("Model must be a numpy array with dtype == Tide.dtype")
-		else:
-			raise ValueError("Must be initialised with constituents, amplitudes and phases; or a model.")
-		if radians:
-			model['phase'] = r2d*model['phase']
-		self.model = model[:]
-		self.normalize()
-
-	def prepare(self, *args, **kwargs):
-		return Tide._prepare(self.model['constituent'], *args, **kwargs)
-
-	@staticmethod
-	def _prepare(constituents, t0, t = None, radians = True):
-		"""
-		Return constituent speed and equilibrium argument at a given time, and constituent node factors at given times.
-		Arguments:
-		constituents -- list of constituents to prepare
-		t0 -- time at which to evaluate speed and equilibrium argument for each constituent
-		t -- list of times at which to evaluate node factors for each constituent (default: t0)
-		radians -- whether to return the angular arguments in radians or degrees (default: True)
-		"""
-		#The equilibrium argument is constant and taken at the beginning of the
-		#time series (t0).  The speed of the equilibrium argument changes very
-		#slowly, so again we take it to be constant over any length of data. The
-		#node factors change more rapidly.
-		if isinstance(t0, Iterable):
-			t0 = t0[0]
-		if t is None:
-			t = [t0]
-		if not isinstance(t, Iterable):
-			t = [t]
-		a0 = astro(t0)
-		a = [astro(t_i) for t_i in t]
-
-		#For convenience give u, V0 (but not speed!) in [0, 360)
-		V0 = np.array([c.V(a0) for c in constituents])[:, np.newaxis]
-		speed = np.array([c.speed(a0) for c in constituents])[:, np.newaxis]
-		u = [np.mod(np.array([c.u(a_i) for c in constituents])[:, np.newaxis], 360.0)
-			 for a_i in a]
-		f = [np.mod(np.array([c.f(a_i) for c in constituents])[:, np.newaxis], 360.0)
-			 for a_i in a]
-
-		if radians:
-			speed = d2r*speed
-			V0 = d2r*V0
-			u = [d2r*each for each in u]
-		return speed, u, f, V0
-
-	def at(self, t):
-		"""
-		Return the modelled tidal height at given times.
-		Arguments:
-		t -- array of times at which to evaluate the tidal height
-		"""
-		t0 = t[0]
-		hours = self._hours(t0, t)
-		partition = 240.0
-		t = self._partition(hours, partition)
-		times = self._times(t0, [(i + 0.5)*partition for i in range(len(t))])
-		speed, u, f, V0 = self.prepare(t0, times, radians = True)
-		H = self.model['amplitude'][:, np.newaxis]
-		p = d2r*self.model['phase'][:, np.newaxis]
-
-		return np.concatenate([
-			Tide._tidal_series(t_i, H, p, speed, u_i, f_i, V0)
-			for t_i, u_i, f_i in izip(t, u, f)
-		])
-
-	def highs(self, *args):
-		"""
-		Generator yielding only the high tides.
-		Arguments:
-		see Tide.extrema()
-		"""
-		for t in ifilter(lambda e: e[2] == 'H', self.extrema(*args)):
-			yield t
-
-	def lows(self, *args):
-		"""
-		Generator yielding only the low tides.
-		Arguments:
-		see Tide.extrema()
-		"""
-		for t in ifilter(lambda e: e[2] == 'L', self.extrema(*args)):
-			yield t
-
-	def form_number(self):
-		"""
-		Returns the model's form number, a helpful heuristic for classifying tides.
-		"""
-		k1, o1, m2, s2 = (
-			np.extract(self.model['constituent'] == c, self.model['amplitude'])
-			for c in [constituent._K1, constituent._O1, constituent._M2, constituent._S2]
-		)
-		return (k1+o1)/(m2+s2)
-
-	def classify(self):
-		"""
-		Classify the tide according to its form number
-		"""
-		form = self.form_number()
-		if 0 <= form <= 0.25:
-			return 'semidiurnal'
-		elif 0.25 < form <= 1.5:
-			return 'mixed (semidiurnal)'
-		elif 1.5 < form <= 3.0:
-			return 'mixed (diurnal)'
-		else:
-			return 'diurnal'
-
-	def extrema(self, t0, t1 = None, partition = 2400.0):
-		"""
-		A generator for high and low tides.
-		Arguments:
-		t0 -- time after which extrema are sought
-		t1 -- optional time before which extrema are sought (if not given, the generator is infinite)
-		partition -- number of hours for which we consider the node factors to be constant (default: 2400.0)
-		"""
-		if t1:
-			#yield from in python 3.4
-			for e in takewhile(lambda t: t[0] < t1, self.extrema(t0)):
-				yield e
-		else:
-			#We assume that extrema are separated by at least delta hours
-			delta = np.amin([
-				90.0 / c.speed(astro(t0)) for c in self.model['constituent']
-				if not c.speed(astro(t0)) == 0
-			])
-			#We search for stationary points from offset hours before t0 to
-			#ensure we find any which might occur very soon after t0.
-			offset = 24.0
-			partitions = (
-				Tide._times(t0, i*partition) for i in count()), (Tide._times(t0, i*partition) for i in count(1)
-			)
-
-			#We'll overestimate to be on the safe side;
-			#values outside (start,end) won't get yielded.
-			interval_count = int(np.ceil((partition + offset) / delta)) + 1
-			amplitude = self.model['amplitude'][:, np.newaxis]
-			phase     = d2r*self.model['phase'][:, np.newaxis]
-
-			for start, end in izip(*partitions):
-				speed, [u], [f], V0 = self.prepare(start, Tide._times(start, 0.5*partition))
-				#These derivatives don't include the time dependence of u or f,
-				#but these change slowly.
-				def d(t):
-					return np.sum(-speed*amplitude*f*np.sin(speed*t + (V0 + u) - phase), axis=0)
-				def d2(t):
-					return np.sum(-speed**2.0 * amplitude*f*np.cos(speed*t + (V0 + u) - phase), axis=0)
-				#We'll overestimate to be on the safe side;
-				#values outside (start,end) won't get yielded.
-				intervals = (
-					delta * i -offset for i in range(interval_count)), (delta*(i+1) - offset for i in range(interval_count)
-				)
-				for a, b in izip(*intervals):
-					if d(a)*d(b) < 0:
-						extrema = fsolve(d, (a + b) / 2.0, fprime = d2)[0]
-						time = Tide._times(start, extrema)
-						[height] = self.at([time])
-						hilo = 'H' if d2(extrema) < 0 else 'L'
-						if start < time < end:
-							yield (time, height, hilo)
-
-	@staticmethod
-	def _hours(t0, t):
-		"""
-		Return the hourly offset(s) of a (list of) time from a given time.
-		Arguments:
-		t0 -- time from which offsets are sought
-		t -- times to find hourly offsets from t0.
-		"""
-		if not isinstance(t, Iterable):
-			return Tide._hours(t0, [t])[0]
-		elif isinstance(t[0], datetime):
-			return np.array([(ti-t0).total_seconds() / 3600.0 for ti in t])
-		else:
-			return t
-
-	@staticmethod
-	def _partition(hours, partition = 3600.0):
-		"""
-		Partition a sorted list of numbers (or in this case hours).
-		Arguments:
-		hours -- sorted ndarray of hours.
-		partition -- maximum partition length (default: 3600.0)
-		"""
-		partition = float(partition)
-		relative = hours - hours[0]
-		total_partitions = np.ceil(relative[-1] / partition + 10*np.finfo(np.float).eps).astype('int')
-		return [hours[np.floor(np.divide(relative, partition)) == i] for i in range(total_partitions)]
-
-	@staticmethod
-	def _times(t0, hours):
-		"""
-		Return a (list of) datetime(s) given an initial time and an (list of) hourly offset(s).
-		Arguments:
-		t0 -- initial time
-		hours -- hourly offsets from t0
-		"""
-		if not isinstance(hours, Iterable):
-			return Tide._times(t0, [hours])[0]
-		elif not isinstance(hours[0], datetime):
-			return np.array([t0 + timedelta(hours=h) for h in hours])
-		else:
-			return np.array(hours)
-
-	@staticmethod
-	def _tidal_series(t, amplitude, phase, speed, u, f, V0):
-		return np.sum(amplitude*f*np.cos(speed*t + (V0 + u) - phase), axis=0)
-
-	def normalize(self):
-		"""
-		Adapt self.model so that amplitudes are positive and phases are in [0,360) as per convention
-		"""
-		for i in range(len(self.model)):
-			if self.model['amplitude'][i] < 0:
-			
-		#for i, (_, amplitude, phase) in enumerate(self.model):
-		#	if amplitude < 0:
-				self.model['amplitude'][i] = -amplitude
-				self.model['phase'][i] = phase + 180.0
-			self.model['phase'][i] = np.mod(self.model['phase'][i], 360.0)
-
-	@classmethod
-	def decompose(
-			cls,
-			heights,
-			t            = None,
-			t0           = None,
-			interval     = None,
-			constituents = constituent.noaa,
-			initial      = None,
-			n_period     = 2,
-			callback     = None,
-			full_output  = False
-		):
-		"""
-		Return an instance of Tide which has been fitted to a series of tidal observations.
-		Arguments:
-		It is not necessary to provide t0 or interval if t is provided.
-		heights -- ndarray of tidal observation heights
-		t -- ndarray of tidal observation times
-		t0 -- datetime representing the time at which heights[0] was recorded
-		interval -- hourly interval between readings
-		constituents -- list of constituents to use in the fit (default: constituent.noaa)
-		initial -- optional Tide instance to use as first guess for least squares solver
-		n_period -- only include constituents which complete at least this many periods (default: 2)
-		callback -- optional function to be called at each iteration of the solver
-		full_output -- whether to return the output of scipy's leastsq solver (default: False)
-		"""
-		if t is not None:
-			if isinstance(t[0], datetime):
-				hours = Tide._hours(t[0], t)
-				t0 = t[0]
-			elif t0 is not None:
-				hours = t
-			else:
-				raise ValueError("t can be an array of datetimes, or an array "
-				                 "of hours since t0 in which case t0 must be "
-				                 "specified.")
-		elif None not in [t0, interval]:
-			hours = np.arange(len(heights)) * interval
-		else:
-			raise ValueError("Must provide t(datetimes), or t(hours) and "
-			                 "t0(datetime), or interval(hours) and t0(datetime) "
-			                 "so that each height can be identified with an "
-			                 "instant in time.")
-
-		#Remove duplicate constituents (those which travel at exactly the same
-		#speed, irrespective of phase)
-		constituents = list(OrderedDict.fromkeys(constituents))
-
-		#No need for least squares to find the mean water level constituent z0,
-		#work relative to mean
-		constituents = [c for c in constituents if not c == constituent._Z0]
-		z0 = np.mean(heights)
-		heights = heights - z0
-
-		#Only analyse frequencies which complete at least n_period cycles over
-		#the data period.
-		constituents = [
-			c for c in constituents
-			if 360.0 * n_period < hours[-1] * c.speed(astro(t0))
-		]
-		n = len(constituents)
-
-		sort = np.argsort(hours)
-		hours = hours[sort]
-		heights = heights[sort]
-
-		#We partition our time/height data into intervals over which we consider
-		#the values of u and f to assume a constant value (that is, their true
-		#value at the midpoint of the interval).  Constituent
-		#speeds change much more slowly than the node factors, so we will
-		#consider these constant and equal to their speed at t0, regardless of
-		#the length of the time series.
-
-		partition = 240.0
-
-		t     = Tide._partition(hours, partition)
-		times = Tide._times(t0, [(i + 0.5)*partition for i in range(len(t))])
-
-		speed, u, f, V0 = Tide._prepare(constituents, t0, times, radians = True)
-
-		#Residual to be minimised by variation of parameters (amplitudes, phases)
-		def residual(hp):
-			H, p = hp[:n, np.newaxis], hp[n:, np.newaxis]
-			s = np.concatenate([
-				Tide._tidal_series(t_i, H, p, speed, u_i, f_i, V0)
-				for t_i, u_i, f_i in izip(t, u, f)
-			])
-			res = heights - s
-			if callback:
-				callback(res)
-			return res
-
-		#Analytic Jacobian of the residual - this makes solving significantly
-		#faster than just using gradient approximation, especially with many
-		#measurements / constituents.
-		def D_residual(hp):
-			H, p = hp[:n, np.newaxis], hp[n:, np.newaxis]
-			ds_dH = np.concatenate([
-				f_i*np.cos(speed*t_i+u_i+V0-p)
-				for t_i, u_i, f_i in izip(t, u, f)],
-				axis = 1)
-
-			ds_dp = np.concatenate([
-				H*f_i*np.sin(speed*t_i+u_i+V0-p)
-				for t_i, u_i, f_i in izip(t, u, f)],
-				axis = 1)
-
-			return np.append(-ds_dH, -ds_dp, axis=0)
-
-		#Initial guess for solver, haven't done any analysis on this since the
-		#solver seems to converge well regardless of the initial guess We do
-		#however scale the initial amplitude guess with some measure of the
-		#variation
-		amplitudes = np.ones(n) * (np.sqrt(np.dot(heights, heights)) / len(heights))
-		phases     = np.ones(n)
-
-		if initial:
-			for (c0, amplitude, phase) in initial.model:
-				for i, c in enumerate(constituents):
-					if c0 == c:
-						amplitudes[i] = amplitude
-						phases[i] = d2r*phase
-
-		initial = np.append(amplitudes, phases)
-
-		lsq = leastsq(residual, initial, Dfun=D_residual, col_deriv=True, ftol=1e-7)
-
-		model = np.zeros(1+n, dtype=cls.dtype)
-		model[0] = (constituent._Z0, z0, 0)
-		model[1:]['constituent'] = constituents[:]
-		model[1:]['amplitude'] = lsq[0][:n]
-		model[1:]['phase'] = lsq[0][n:]
-
-		if full_output:
-			return cls(model = model, radians = True), lsq
-		return cls(model = model, radians = True)
+#   Copyright notice
+#   --------------------------------------------------------------------
+#   Copyright (C) 2020 Deltares
+#       Freek Scheel
+#
+#       freek.scheel@deltares.nl
+#
+#       P.O. Box 177
+#       2600 MH Delft
+#       The Netherlands
+#
+#   This library is free software: you can redistribute it and/or modify
+#   it under the terms of the GNU Lesser General Public License as published by
+#   the Free Software Foundation, either version 3 of the License, or
+#   (at your option) any later version.
+#
+#   This library is distributed in the hope that it will be useful,
+#   but WITHOUT ANY WARRANTY; without even the implied warranty of
+#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#   GNU General Public License for more details.
+#
+#   You should have received a copy of the GNU General Public License
+#   along with this library.  If not, see <http://www.gnu.org/licenses/>.
+#   --------------------------------------------------------------------
+
+from collections import OrderedDict
+from collections.abc import Iterable
+from itertools import takewhile, count
+try:
+	from itertools import izip, ifilter
+except ImportError: #Python3
+	izip = zip
+	ifilter = filter
+from datetime import datetime, timedelta
+import numpy as np
+from scipy.optimize import leastsq, fsolve
+from functools import reduce
+
+from .astro import astro
+import cht.tide.constituent as constituent
+
+d2r, r2d = np.pi/180.0, 180.0/np.pi
+
+class Tide(object):
+	dtype = np.dtype([
+		('constituent', object),
+		('amplitude', float),
+		('phase', float)])
+
+	def __init__(
+			self,
+			constituents = None,
+			amplitudes = None,
+			phases = None,
+			model = None,
+			radians = False
+		):
+		"""
+		Initialise a tidal model. Provide constituents, amplitudes and phases OR a model.
+		Arguments:
+		constituents -- list of constituents used in the model.
+		amplitudes -- list of amplitudes corresponding to constituents
+		phases -- list of phases corresponding to constituents
+		model -- an ndarray of type Tide.dtype representing the constituents, amplitudes and phases.
+		radians -- boolean representing whether phases are in radians (default False)
+		"""
+		if None not in [constituents, amplitudes, phases]:
+			if len(constituents) == len(amplitudes) == len(phases):
+				model = np.zeros(len(phases), dtype=Tide.dtype)
+				model['constituent'] = np.array(constituents)
+				model['amplitude'] = np.array(amplitudes)
+				model['phase'] = np.array(phases)
+			else:
+				raise ValueError("Constituents, amplitudes and phases should all be arrays of equal length.")
+		elif model is not None:
+			if not model.dtype == Tide.dtype:
+				raise ValueError("Model must be a numpy array with dtype == Tide.dtype")
+		else:
+			raise ValueError("Must be initialised with constituents, amplitudes and phases; or a model.")
+		if radians:
+			model['phase'] = r2d*model['phase']
+		self.model = model[:]
+		self.normalize()
+
+	def prepare(self, *args, **kwargs):
+		return Tide._prepare(self.model['constituent'], *args, **kwargs)
+
+	@staticmethod
+	def _prepare(constituents, t0, t = None, radians = True):
+		"""
+		Return constituent speed and equilibrium argument at a given time, and constituent node factors at given times.
+		Arguments:
+		constituents -- list of constituents to prepare
+		t0 -- time at which to evaluate speed and equilibrium argument for each constituent
+		t -- list of times at which to evaluate node factors for each constituent (default: t0)
+		radians -- whether to return the angular arguments in radians or degrees (default: True)
+		"""
+		#The equilibrium argument is constant and taken at the beginning of the
+		#time series (t0).  The speed of the equilibrium argument changes very
+		#slowly, so again we take it to be constant over any length of data. The
+		#node factors change more rapidly.
+		if isinstance(t0, Iterable):
+			t0 = t0[0]
+		if t is None:
+			t = [t0]
+		if not isinstance(t, Iterable):
+			t = [t]
+		a0 = astro(t0)
+		a = [astro(t_i) for t_i in t]
+
+		#For convenience give u, V0 (but not speed!) in [0, 360)
+		V0 = np.array([c.V(a0) for c in constituents])[:, np.newaxis]
+		speed = np.array([c.speed(a0) for c in constituents])[:, np.newaxis]
+		u = [np.mod(np.array([c.u(a_i) for c in constituents])[:, np.newaxis], 360.0)
+			 for a_i in a]
+		f = [np.mod(np.array([c.f(a_i) for c in constituents])[:, np.newaxis], 360.0)
+			 for a_i in a]
+
+		if radians:
+			speed = d2r*speed
+			V0 = d2r*V0
+			u = [d2r*each for each in u]
+		return speed, u, f, V0
+
+	def at(self, t):
+		"""
+		Return the modelled tidal height at given times.
+		Arguments:
+		t -- array of times at which to evaluate the tidal height
+		"""
+		t0 = t[0]
+		hours = self._hours(t0, t)
+		partition = 240.0
+		t = self._partition(hours, partition)
+		times = self._times(t0, [(i + 0.5)*partition for i in range(len(t))])
+		speed, u, f, V0 = self.prepare(t0, times, radians = True)
+		H = self.model['amplitude'][:, np.newaxis]
+		p = d2r*self.model['phase'][:, np.newaxis]
+
+		return np.concatenate([
+			Tide._tidal_series(t_i, H, p, speed, u_i, f_i, V0)
+			for t_i, u_i, f_i in izip(t, u, f)
+		])
+
+	def highs(self, *args):
+		"""
+		Generator yielding only the high tides.
+		Arguments:
+		see Tide.extrema()
+		"""
+		for t in ifilter(lambda e: e[2] == 'H', self.extrema(*args)):
+			yield t
+
+	def lows(self, *args):
+		"""
+		Generator yielding only the low tides.
+		Arguments:
+		see Tide.extrema()
+		"""
+		for t in ifilter(lambda e: e[2] == 'L', self.extrema(*args)):
+			yield t
+
+	def form_number(self):
+		"""
+		Returns the model's form number, a helpful heuristic for classifying tides.
+		"""
+		k1, o1, m2, s2 = (
+			np.extract(self.model['constituent'] == c, self.model['amplitude'])
+			for c in [constituent._K1, constituent._O1, constituent._M2, constituent._S2]
+		)
+		return (k1+o1)/(m2+s2)
+
+	def classify(self):
+		"""
+		Classify the tide according to its form number
+		"""
+		form = self.form_number()
+		if 0 <= form <= 0.25:
+			return 'semidiurnal'
+		elif 0.25 < form <= 1.5:
+			return 'mixed (semidiurnal)'
+		elif 1.5 < form <= 3.0:
+			return 'mixed (diurnal)'
+		else:
+			return 'diurnal'
+
+	def extrema(self, t0, t1 = None, partition = 2400.0):
+		"""
+		A generator for high and low tides.
+		Arguments:
+		t0 -- time after which extrema are sought
+		t1 -- optional time before which extrema are sought (if not given, the generator is infinite)
+		partition -- number of hours for which we consider the node factors to be constant (default: 2400.0)
+		"""
+		if t1:
+			#yield from in python 3.4
+			for e in takewhile(lambda t: t[0] < t1, self.extrema(t0)):
+				yield e
+		else:
+			#We assume that extrema are separated by at least delta hours
+			delta = np.amin([
+				90.0 / c.speed(astro(t0)) for c in self.model['constituent']
+				if not c.speed(astro(t0)) == 0
+			])
+			#We search for stationary points from offset hours before t0 to
+			#ensure we find any which might occur very soon after t0.
+			offset = 24.0
+			partitions = (
+				Tide._times(t0, i*partition) for i in count()), (Tide._times(t0, i*partition) for i in count(1)
+			)
+
+			#We'll overestimate to be on the safe side;
+			#values outside (start,end) won't get yielded.
+			interval_count = int(np.ceil((partition + offset) / delta)) + 1
+			amplitude = self.model['amplitude'][:, np.newaxis]
+			phase     = d2r*self.model['phase'][:, np.newaxis]
+
+			for start, end in izip(*partitions):
+				speed, [u], [f], V0 = self.prepare(start, Tide._times(start, 0.5*partition))
+				#These derivatives don't include the time dependence of u or f,
+				#but these change slowly.
+				def d(t):
+					return np.sum(-speed*amplitude*f*np.sin(speed*t + (V0 + u) - phase), axis=0)
+				def d2(t):
+					return np.sum(-speed**2.0 * amplitude*f*np.cos(speed*t + (V0 + u) - phase), axis=0)
+				#We'll overestimate to be on the safe side;
+				#values outside (start,end) won't get yielded.
+				intervals = (
+					delta * i -offset for i in range(interval_count)), (delta*(i+1) - offset for i in range(interval_count)
+				)
+				for a, b in izip(*intervals):
+					if d(a)*d(b) < 0:
+						extrema = fsolve(d, (a + b) / 2.0, fprime = d2)[0]
+						time = Tide._times(start, extrema)
+						[height] = self.at([time])
+						hilo = 'H' if d2(extrema) < 0 else 'L'
+						if start < time < end:
+							yield (time, height, hilo)
+
+	@staticmethod
+	def _hours(t0, t):
+		"""
+		Return the hourly offset(s) of a (list of) time from a given time.
+		Arguments:
+		t0 -- time from which offsets are sought
+		t -- times to find hourly offsets from t0.
+		"""
+		if not isinstance(t, Iterable):
+			return Tide._hours(t0, [t])[0]
+		elif isinstance(t[0], datetime):
+			return np.array([(ti-t0).total_seconds() / 3600.0 for ti in t])
+		else:
+			return t
+
+	@staticmethod
+	def _partition(hours, partition = 3600.0):
+		"""
+		Partition a sorted list of numbers (or in this case hours).
+		Arguments:
+		hours -- sorted ndarray of hours.
+		partition -- maximum partition length (default: 3600.0)
+		"""
+		partition = float(partition)
+		relative = hours - hours[0]
+		total_partitions = np.ceil(relative[-1] / partition + 10*np.finfo(np.float64).eps).astype('int')
+		return [hours[np.floor(np.divide(relative, partition)) == i] for i in range(total_partitions)]
+
+	@staticmethod
+	def _times(t0, hours):
+		"""
+		Return a (list of) datetime(s) given an initial time and an (list of) hourly offset(s).
+		Arguments:
+		t0 -- initial time
+		hours -- hourly offsets from t0
+		"""
+		if not isinstance(hours, Iterable):
+			return Tide._times(t0, [hours])[0]
+		elif not isinstance(hours[0], datetime):
+			return np.array([t0 + timedelta(hours=h) for h in hours])
+		else:
+			return np.array(hours)
+
+	@staticmethod
+	def _tidal_series(t, amplitude, phase, speed, u, f, V0):
+		return np.sum(amplitude*f*np.cos(speed*t + (V0 + u) - phase), axis=0)
+
+	def normalize(self):
+		"""
+		Adapt self.model so that amplitudes are positive and phases are in [0,360) as per convention
+		"""
+		for i in range(len(self.model)):
+			if self.model['amplitude'][i] < 0:
+			
+		#for i, (_, amplitude, phase) in enumerate(self.model):
+		#	if amplitude < 0:
+				self.model['amplitude'][i] = -amplitude
+				self.model['phase'][i] = phase + 180.0
+			self.model['phase'][i] = np.mod(self.model['phase'][i], 360.0)
+
+	@classmethod
+	def decompose(
+			cls,
+			heights,
+			t            = None,
+			t0           = None,
+			interval     = None,
+			constituents = constituent.noaa,
+			initial      = None,
+			n_period     = 2,
+			callback     = None,
+			full_output  = False
+		):
+		"""
+		Return an instance of Tide which has been fitted to a series of tidal observations.
+		Arguments:
+		It is not necessary to provide t0 or interval if t is provided.
+		heights -- ndarray of tidal observation heights
+		t -- ndarray of tidal observation times
+		t0 -- datetime representing the time at which heights[0] was recorded
+		interval -- hourly interval between readings
+		constituents -- list of constituents to use in the fit (default: constituent.noaa)
+		initial -- optional Tide instance to use as first guess for least squares solver
+		n_period -- only include constituents which complete at least this many periods (default: 2)
+		callback -- optional function to be called at each iteration of the solver
+		full_output -- whether to return the output of scipy's leastsq solver (default: False)
+		"""
+		if t is not None:
+			if isinstance(t[0], datetime):
+				hours = Tide._hours(t[0], t)
+				t0 = t[0]
+			elif t0 is not None:
+				hours = t
+			else:
+				raise ValueError("t can be an array of datetimes, or an array "
+				                 "of hours since t0 in which case t0 must be "
+				                 "specified.")
+		elif None not in [t0, interval]:
+			hours = np.arange(len(heights)) * interval
+		else:
+			raise ValueError("Must provide t(datetimes), or t(hours) and "
+			                 "t0(datetime), or interval(hours) and t0(datetime) "
+			                 "so that each height can be identified with an "
+			                 "instant in time.")
+
+		#Remove duplicate constituents (those which travel at exactly the same
+		#speed, irrespective of phase)
+		constituents = list(OrderedDict.fromkeys(constituents))
+
+		#No need for least squares to find the mean water level constituent z0,
+		#work relative to mean
+		constituents = [c for c in constituents if not c == constituent._Z0]
+		z0 = np.mean(heights)
+		heights = heights - z0
+
+		#Only analyse frequencies which complete at least n_period cycles over
+		#the data period.
+		constituents = [
+			c for c in constituents
+			if 360.0 * n_period < hours[-1] * c.speed(astro(t0))
+		]
+		n = len(constituents)
+
+		sort = np.argsort(hours)
+		hours = hours[sort]
+		heights = heights[sort]
+
+		#We partition our time/height data into intervals over which we consider
+		#the values of u and f to assume a constant value (that is, their true
+		#value at the midpoint of the interval).  Constituent
+		#speeds change much more slowly than the node factors, so we will
+		#consider these constant and equal to their speed at t0, regardless of
+		#the length of the time series.
+
+		partition = 240.0
+
+		t     = Tide._partition(hours, partition)
+		times = Tide._times(t0, [(i + 0.5)*partition for i in range(len(t))])
+
+		speed, u, f, V0 = Tide._prepare(constituents, t0, times, radians = True)
+
+		#Residual to be minimised by variation of parameters (amplitudes, phases)
+		def residual(hp):
+			H, p = hp[:n, np.newaxis], hp[n:, np.newaxis]
+			s = np.concatenate([
+				Tide._tidal_series(t_i, H, p, speed, u_i, f_i, V0)
+				for t_i, u_i, f_i in izip(t, u, f)
+			])
+			res = heights - s
+			if callback:
+				callback(res)
+			return res
+
+		#Analytic Jacobian of the residual - this makes solving significantly
+		#faster than just using gradient approximation, especially with many
+		#measurements / constituents.
+		def D_residual(hp):
+			H, p = hp[:n, np.newaxis], hp[n:, np.newaxis]
+			ds_dH = np.concatenate([
+				f_i*np.cos(speed*t_i+u_i+V0-p)
+				for t_i, u_i, f_i in izip(t, u, f)],
+				axis = 1)
+
+			ds_dp = np.concatenate([
+				H*f_i*np.sin(speed*t_i+u_i+V0-p)
+				for t_i, u_i, f_i in izip(t, u, f)],
+				axis = 1)
+
+			return np.append(-ds_dH, -ds_dp, axis=0)
+
+		#Initial guess for solver, haven't done any analysis on this since the
+		#solver seems to converge well regardless of the initial guess We do
+		#however scale the initial amplitude guess with some measure of the
+		#variation
+		amplitudes = np.ones(n) * (np.sqrt(np.dot(heights, heights)) / len(heights))
+		phases     = np.ones(n)
+
+		if initial:
+			for (c0, amplitude, phase) in initial.model:
+				for i, c in enumerate(constituents):
+					if c0 == c:
+						amplitudes[i] = amplitude
+						phases[i] = d2r*phase
+
+		initial = np.append(amplitudes, phases)
+
+		lsq = leastsq(residual, initial, Dfun=D_residual, col_deriv=True, ftol=1e-7)
+
+		model = np.zeros(1+n, dtype=cls.dtype)
+		model[0] = (constituent._Z0, z0, 0)
+		model[1:]['constituent'] = constituents[:]
+		model[1:]['amplitude'] = lsq[0][:n]
+		model[1:]['phase'] = lsq[0][n:]
+
+		if full_output:
+			return cls(model = model, radians = True), lsq
+		return cls(model = model, radians = True)
```

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/tide_predict.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide_predict.py`

 * *Files identical despite different names*

### Comparing `deltares_coastalhazardstoolkit-0.0.8/src/cht/xbeach.py` & `deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/xbeach.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,68 +10,78 @@
 import array,os,numpy,sys
 # from pupynere import netcdf_file as nc
 from scipy.io.netcdf import netcdf_file as nc
 import numpy as np
 import datetime
 from optparse import OptionParser
 import pandas as pd
+import math
+from pyproj import CRS
+from pyproj import Transformer
+import time
 
-from cht.geometry import Point
+from cht.misc.geometry import Point
 
 # constants
 fmt = '%Y-%m-%d %H:%M:%S'
 
 class XBeach:
     
-    def __init__(self, input_file=None, crs=None):
+    def __init__(self, input_file=None, crs=None, get_boundary_coordinates=True):
  
 #        self.epsg                     = epsg
         self.params                   = Params()
         self.crs                      = crs
         self.grid                     = None
         self.flow_boundary_point      = []
         self.wave_boundary_point      = []
         self.observation_point        = []
         self.obstacle                 = []
         
         if input_file:
             self.path   = os.path.dirname(input_file)
             self.params = self.params.fromfile(filename=input_file)
-            self.get_boundary_points()
+            self.get_boundary_points(get_boundary_coordinates)
 
     def load(self, input_file):
         # Reads sfincs.inp and attribute files
         self.params = self.params.fromfile(filename=input_file)
         self.read_attribute_files()
         
     def read_attribute_files(self):
         pass
 
-    def get_boundary_points(self):
-        
-        xfile = os.path.join(self.path, self.params["xfile"])
-        yfile = os.path.join(self.path, self.params["yfile"])        
-        xg = np.loadtxt(xfile)
-        yg = np.loadtxt(yfile)
+    def get_boundary_points(self, get_boundary_coordinates):
 
         self.flow_boundary_point = []
         self.wave_boundary_point = []
         
-        x0 = xg[0, 0]
-        y0 = yg[0, 0]
-        x1 = xg[0, -1]
-        y1 = yg[0, -1]
-        x2 = xg[-1, 0]
-        y2 = yg[-1, 0]
-        x3 = xg[-1, -1]
-        y3 = yg[-1, -1]
-        
-        self.flow_boundary_point = []
-        self.wave_boundary_point = []
-        
+        if get_boundary_coordinates:
+            xfile = os.path.join(self.path, self.params["xfile"])
+            yfile = os.path.join(self.path, self.params["yfile"])        
+            xg = np.loadtxt(xfile)
+            yg = np.loadtxt(yfile)
+            x0 = xg[0, 0]
+            y0 = yg[0, 0]
+            x1 = xg[0, -1]
+            y1 = yg[0, -1]
+            x2 = xg[-1, 0]
+            y2 = yg[-1, 0]
+            x3 = xg[-1, -1]
+            y3 = yg[-1, -1]
+        else:
+            x0 = 0.0
+            y0 = 0.0
+            x1 = 0.0
+            y1 = 0.0
+            x2 = 0.0
+            y2 = 0.0
+            x3 = 0.0
+            y3 = 0.0
+                
         if self.params["tideloc"] == 1:
             x = x0 + 0.5*(x2 - x0)
             y = y0 + 0.5*(y2 - y0)
             self.flow_boundary_point.append(BoundaryPoint(x, y))
         elif self.params["tideloc"] == 2:
             x = x0
             y = y0
@@ -110,14 +120,20 @@
         if not file_name:
             return
         
         # Build a new DataFrame
         df = pd.DataFrame()
         for point in self.flow_boundary_point:
             df = pd.concat([df, point.data], axis=1)
+        
+        # add constant water level at tideloc locations without water levels    
+        if df.shape[1] < self.params["tideloc"]:
+            for i in np.arange(df.shape[1],self.params["tideloc"]):
+                df.insert(int(i),str(i),-0.5)
+            
         tmsec = pd.to_timedelta(df.index.values - self.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.3f")
@@ -136,18 +152,18 @@
             if not file_name:
                 return
             
             # Build a new DataFrame
             df = pd.DataFrame()
             for point in self.wave_boundary_point:
                 df = pd.concat([df, point.data], axis=1)
-            tmsec = pd.to_timedelta(df.index - self.tref, unit="s")
-            df.index = tmsec.total_seconds()
+            #tmsec = pd.to_timedelta(df.index - self.tref, unit="s")
+            #df.index = tmsec.total_seconds()
             df.to_csv(file_name,
-                      index=True,
+                      index=False,
                       sep=" ",
                       header=False,
                       float_format="%0.3f")
         
         else:
             # 2D spectra
             # Bit more work ...
@@ -206,19 +222,174 @@
                     mxmx = np.max(sp2)
                     fac = mxmx/990099
                     fac = max(fac, 1.e-12)
                     f.write(f'{fac:.8e}' + "\n")                    
                     sp2 = (sp2/fac).astype(int)
                     sp2 = np.clip(sp2, 1.0, None)
                     np.savetxt(f, sp2, fmt="%.7i")
-                    f.close()   
+                    f.close()
+
+    def make_index_tiles(self, path, zoom_range=None):
+        """Make tiles for different zoom levels by saving the index of the xbeach grid cell
+        to be used for each world png raster"""
+        from cht.tiling import deg2num
+        from cht.tiling import num2deg
+        import cht.fileops as fo
+        from scipy.spatial import distance
+
+        if not zoom_range:
+            zoom_range = [0, 13]
+
+        npix = 256
+
+        # Compute lon/lat range
+        lon_range, lat_range = self.bounding_box(crs=CRS.from_epsg(4326))
+
+        # get grid orientation
+        xb, yb = self.grid_coordinates(loc='cor')
+        alpha = math.atan2(yb[0, -1] - yb[0, 0], xb[0, -1] - xb[0, 0]) * 180 / math.pi
+
+        # Get origin (corner)
+        x0, y0 = xb[0, 0], yb[0, 0]
+
+        # Get distance vectors (x and y are the cross-shore and alongshore axis here)
+        xvec = np.array([distance.euclidean((xp, yp), (x0, y0)) for xp, yp in zip(xb[0, :], yb[0, :])])
+        yvec = np.array([distance.euclidean((xp, yp), (x0, y0)) for xp, yp in zip(xb[:, 0], yb[:, 0])])
+
+        # Get number of cells in each direction
+        xcells, ycells = len(xvec)-1, len(yvec)-1
+
+        # Get rotation parameters
+        cosrot = math.cos(-alpha * math.pi / 180)
+        sinrot = math.sin(-alpha * math.pi / 180)
+
+        # Get transformers between crs
+        transformer_a = Transformer.from_crs(CRS.from_epsg(4326),
+                                             CRS.from_epsg(3857),
+                                             always_xy=True)
+        transformer_b = Transformer.from_crs(CRS.from_epsg(3857),
+                                             self.crs,
+                                             always_xy=True)
+        # Loop through each zoom level
+        for izoom in range(zoom_range[0], zoom_range[1] + 1):
+
+            print("Processing zoom level " + str(izoom))
+
+            zoom_path = os.path.join(path, str(izoom))  # Create path for zoom level
+
+            dxy = (40075016.686 / npix) / 2 ** izoom  # Get png cell size based on zoom level
+            xx = np.linspace(0.0, (npix - 1) * dxy, num=npix)
+            yy = xx[:]
+            xv, yv = np.meshgrid(xx, yy)  # Get distance grid for each tile
+
+            # Get range of tile indices to be used for the zoom level
+            ix0, iy0 = deg2num(lat_range[0], lon_range[0], izoom)
+            ix1, iy1 = deg2num(lat_range[1], lon_range[1], izoom)
+
+            for i in range(ix0, ix1 + 1):  # loop through x tiles
+
+                path_okay = False
+                zoom_path_i = os.path.join(zoom_path, str(i))  # Create path for x index
+
+                for j in range(iy0, iy1 + 1):
+
+                    file_name = os.path.join(zoom_path_i, str(j) + ".dat")  # Create file for y index
+
+                    # Compute lat/lon at ll corner of tile
+                    lat, lon = num2deg(i, j, izoom)
+
+                    # Convert to Global Mercator
+                    xo, yo = transformer_a.transform(lon, lat)
+
+                    # Tile grid on local mercator (this is at cell center)
+                    x = xv[:] + xo + 0.5 * dxy
+                    y = yv[:] + yo + 0.5 * dxy
+
+                    # Convert tile grid to crs of xbeach model
+                    x, y = transformer_b.transform(x, y)
+
+                    # Now rotate around origin of XBeach model (with x0, y0 the cell corner of xbeach)
+                    x00 = x - x0
+                    y00 = y - y0
+                    xg = x00 * cosrot - y00 * sinrot
+                    yg = x00 * sinrot + y00 * cosrot
+
+                    # find mask of cells falling in XBeach domain
+                    imask = (xg > 0) & (xg <= xvec[-1])
+                    jmask = (yg > 0) & (yg <= yvec[-1])
+                    mask = imask & jmask
+                    ind = np.full(mask.shape, -999)  # Prepare index matrix
+
+                    for ii in range(len(mask[:, 0])):  # loop through x
+                        for jj in range(len(mask[0, :])):  # loop through y
+                            if mask[ii, jj]:  #  only calculate if in the XBeach domain
+                                iind = grid_ind(xg[ii, jj], xvec)
+                                jind = grid_ind(yg[ii, jj], yvec)
+                                ind[ii, jj] = iind * ycells + jind
+
+                    if np.any(ind >= 0):  # Only continue if there is at least on png cell in the domain
+
+                        if not path_okay:  # ensure path exists to save file
+                            if not os.path.exists(zoom_path_i):
+                                fo.mkdir(zoom_path_i)
+                                path_okay = True
+
+                        # And write indices to file
+                        fid = open(file_name, "wb")
+                        fid.write(ind)
+                        fid.close()
+
+
+    def grid_coordinates(self, loc='cor'):
+        """Get grid coordinates either at cell centers or corenrs"""
+        # Get coordinates of cell centers
+        xg = np.loadtxt(os.path.join(self.path, self.params['xfile']))
+        yg = np.loadtxt(os.path.join(self.path, self.params['yfile']))
+
+        if loc == 'cor': # if cells corners are used
+            # Get cell grid size in x and y
+            dxx = np.array([xg[0, 1] - xg[0, 0]] + [xg[0, i] - xg[0, i - 1] for i in range(1, len(xg[0, :]))])
+            dyx = np.array([yg[0, 1] - yg[0, 0]] + [yg[0, i] - yg[0, i - 1] for i in range(1, len(yg[0, :]))])
+            dxy = np.array([xg[1, 0] - xg[0, 0]] + [xg[i, 0] - xg[i - 1, 0] for i in range(1, len(xg[:, 0]))])
+            dyy = np.array([yg[1, 0] - yg[0, 0]] + [yg[i, 0] - yg[i - 1, 0] for i in range(1, len(yg[:, 0]))])
+            # Define grid at cell corners
+            new_x, new_y = [], []
+            for i in range(len(xg[:, 0])):
+                new_x.append(xg[i, :] - (dxx / 2 + np.repeat(dxy[i], len(dxx)) / 2))
+                new_y.append(yg[i, :] - (dyx / 2 + np.repeat(dyy[i], len(dyx)) / 2))
+            new_x, new_y = np.array(new_x), np.array(new_y)
+            # Add last grid line (new grid represent the extent)
+            new_x = np.vstack((new_x, new_x[-1, :] + np.repeat(dxy[-1], len(dxx))))
+            new_y = np.vstack((new_y, new_y[-1, :] + np.repeat(dyy[-1], len(dyx))))
+            new_x = np.hstack((new_x, (new_x[:, -1] + np.repeat(dxx[-1], len(dxy)+1))[:, None]))
+            new_y = np.hstack((new_y, (new_y[:, -1] + np.repeat(dyx[-1], len(dyy)+1))[:, None]))
+
+        else:  # if cell centres are used
+            new_x = xg
+            new_y = yg
+
+        return new_x, new_y
+
+
+    def bounding_box(self, crs=None):
+        """Determine bounding box of Xbeach grid"""
+        xg, yg = self.grid_coordinates(loc='cor')
+
+        if crs:
+            transformer = Transformer.from_crs(self.crs,
+                                               crs,
+                                               always_xy=True)
+            xg, yg = transformer.transform(xg, yg)
+
+        x_range = [np.min(np.min(xg)), np.max(np.max(xg))]
+        y_range = [np.min(np.min(yg)), np.max(np.max(yg))]
+
+        return x_range, y_range
+
 
-                
-                
-                    
 class BoundaryPoint():
 
     def __init__(self, x, y, name=None, crs=None, data=None):
         
         self.name                   = name
         self.geometry               = Point(x, y, crs=crs)
         self.data                   = data
@@ -252,28 +423,42 @@
                         if key is None:
                             raise ValueError("invalid line:\n" + line)
                         # We have some array type of value
                         values[key[1:]] = values.get(key[1:], []) + [line.strip()]
         return values
 
     def tofile(self, filename="params.txt"):
+        general = ['wavemodel','wbctype', 'deltahmin', 'fixedavaltime', 'oldTsmin', 'oldhmin', 'snells', 'droot', 'dstem', 'dynamicroughness', 'alfaD50']
         phys_process = ['swave', 'nonh', 'single_dir', 'sedtrans', 'morphology', 'avalanching']
         grid_params = ['xori', 'yori', 'alfa', 'nx', 'ny', 'posdwn', 'depfile', 'vardx', 'xfile', 'yfile',
-                       'thetamin', 'thetamax', 'thetanaut', 'dtheta_s', 'dtheta']
+                       'thetamin', 'thetamax', 'thetanaut', 'dtheta_s', 'dtheta', 'gridform']
         model_time = ['tstop']
-        wave_bc = ['instat', 'bcfile', 'snells','wavint']
-        tide_bc = ['tideloc', 'zs0file', 'front', 'back']
-        flow_params = ['bedfriction']
-        morph_params = ['morfac', 'morstart']
-        output_vars = ['tintg', 'tintm', 'outputformat']
+        wave_bc = ['break', 'gamma', 'gamma2', 'alpha', 'bcfile', 'wavint']
+        tide_bc = ['tideloc', 'zs0file', 'front', 'back', 'tidetype']
+        flow_params = ['bedfriction', 'bedfricile', 'nuhfac']
+        bed_params = ['D50']
+        morph_params = ['morfac', 'morstart','wetslp', 'struct', 'ne_layer']
+        roller_params = ['beta']
+        sed_params = ['waveform','facAs', 'facSk']
+        output_vars = ['tintg', 'tintm', 'outputformat', 'tintp', 'tstart']
 
         with open(filename, 'w') as f:
             f.writelines('### XBeach parameter settings input file\n')
             f.writelines('### Created on: ' + datetime.datetime.now().strftime(fmt) + '\n')
 
+            f.writelines('\n### General\n')
+            for key, value in self.items():
+                if key in general:
+                        f.writelines('%-15s= %s' % (key, value) + '\n')
+                        
+            f.writelines('\n### Bed composition parameters\n')
+            for key, value in self.items():
+                if key in bed_params:
+                        f.writelines('%-15s= %s' % (key, value) + '\n')
+
             f.writelines('\n### Physical processes\n')
             for key, value in self.items():
                 if key in phys_process:
                         f.writelines('%-15s= %s' % (key, value) + '\n')
 
             f.writelines('\n### Grid parameters\n')
             for key, value in self.items():
@@ -281,15 +466,15 @@
                         f.writelines('%-15s= %s' % (key, value) + '\n')
 
             f.writelines('\n### Model time parameters\n')
             for key, value in self.items():
                 if key in model_time:
                         f.writelines('%-15s= %s' % (key, value) + '\n')
 
-            f.writelines('\n### Wave boundary condition parameters\n')
+            f.writelines('\n### Wave breaking parameters\n')
             for key, value in self.items():
                 if key in wave_bc:
                         f.writelines('%-15s= %s' % (key, value) + '\n')
 
             f.writelines('\n### Tide boundary condition\n')
             for key, value in self.items():
                 if key in tide_bc:
@@ -301,24 +486,35 @@
                         f.writelines('%-15s= %s' % (key, value) + '\n')
 
             f.writelines('\n### Morphology parameters\n')
             for key, value in self.items():
                 if key in morph_params:
                         f.writelines('%-15s= %s' % (key, value) + '\n')
 
+            f.writelines('\n### Sediment transport parameters\n')
+            for key, value in self.items():
+                if key in sed_params:
+                        f.writelines('%-15s= %s' % (key, value) + '\n')
+                        
+            f.writelines('\n### Roller parameters\n')
+            for key, value in self.items():
+                if key in roller_params:
+                        f.writelines('%-15s= %s' % (key, value) + '\n')
+
             f.writelines('\n### Output variables\n')
             for key, value in self.items():
                 if key in output_vars:
                     f.writelines('%-15s= %s' % (key, value) + '\n')
 
             for key, value in self.items():
                 if key == 'nglobalvar':
                     f.writelines("\n%s = %s" % (key, value) + '\n')
                     for val in self['globalvar']:
                         f.writelines(val + '\n')
+                    f.writelines('\n')
                 elif key == 'nmeanvar':
                     f.writelines("%s = %s" % (key, value) + '\n')
                     for val in self['meanvar']:
                         f.writelines(val + '\n')
 
 
                 # elif key in grid_params:
@@ -342,18 +538,22 @@
             #     match = pat_name.match(line)
             #     if match: # found name, print and end line
             #         f.write(match.group(1) + "\n")
             #
             #
 
 
-                
-            
-        
 # functions
+def grid_ind(value, grid):
+    """ get index of cell based on distance grid"""
+    dif = value - grid
+    i0 = np.argmin(abs(dif))
+    i = i0 if dif[i0] > 0 else i0 - 1
+    return i
+
 def listdat(path):
     """find all .dat-files in directory"""
     import glob
     return glob.glob(os.path.join(path,'*.dat'))
 
 def listfiles(path):
     import glob
```

