# Comparing `tmp/cytosim-0.0.5.tar.gz` & `tmp/cytosim-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytosim-0.0.5.tar", last modified: Fri Aug  4 07:50:11 2023, max compression
+gzip compressed data, was "cytosim-0.0.6.tar", last modified: Fri Aug  4 12:53:40 2023, max compression
```

## Comparing `cytosim-0.0.5.tar` & `cytosim-0.0.6.tar`

### file list

```diff
@@ -1,609 +1,609 @@
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.216385 cytosim-0.0.5/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2023-08-03 15:27:32.000000 cytosim-0.0.5/.gitignore
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-04 07:08:34.000000 cytosim-0.0.5/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2023-08-03 15:27:32.000000 cytosim-0.0.5/LICENSE.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4751 2023-08-04 07:50:11.216385 cytosim-0.0.5/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2023-08-03 15:27:32.000000 cytosim-0.0.5/PYCYTOSIM.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3752 2023-08-03 15:27:32.000000 cytosim-0.0.5/README.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2023-08-03 15:27:32.000000 cytosim-0.0.5/WARRANTY.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.176385 cytosim-0.0.5/cytosim.egg-info/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4751 2023-08-04 07:50:11.000000 cytosim-0.0.5/cytosim.egg-info/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14193 2023-08-04 07:50:11.000000 cytosim-0.0.5/cytosim.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-04 07:50:11.000000 cytosim-0.0.5/cytosim.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-04 07:50:11.000000 cytosim-0.0.5/cytosim.egg-info/not-zip-safe
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       18 2023-08-04 07:50:11.000000 cytosim-0.0.5/cytosim.egg-info/top_level.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2023-08-03 15:27:32.000000 cytosim-0.0.5/makefile
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12556 2023-08-03 15:27:32.000000 cytosim-0.0.5/makefile.inc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.176385 cytosim-0.0.5/pycytosim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12212 2023-08-04 07:31:58.000000 cytosim-0.0.5/pycytosim/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       23 2023-08-03 15:28:09.000000 cytosim-0.0.5/pycytosim/__init__.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.176385 cytosim-0.0.5/python/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.176385 cytosim-0.0.5/python/look/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/collect.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/compare_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/get_data.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/make_image.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/make_movie.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/make_page.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/make_plots.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/read_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/scan.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/look/tell.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.176385 cytosim-0.0.5/python/misc/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/misc/battery_test.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/misc/cleanup.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/misc/compare.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/misc/plot.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/misc/pyned.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/misc/reduce.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.176385 cytosim-0.0.5/python/run/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/run/go_sim.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/run/go_sim_lib.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23500 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/run/preconfig.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/run/submit_one.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2023-08-03 15:27:32.000000 cytosim-0.0.5/python/run/submit_slurm.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2023-08-04 07:50:11.216385 cytosim-0.0.5/setup.cfg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4851 2023-08-04 07:49:54.000000 cytosim-0.0.5/setup.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.176385 cytosim-0.0.5/src/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/CMakeLists.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.180385 cytosim-0.0.5/src/base/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/array.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/assert_macro.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/backtrace.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/backtrace.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/buddy.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/exceptions.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/exceptions.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/filepath.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/filepath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/filewrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/filewrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/glossary.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/glossary.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/inventoried.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/inventory.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/inventory.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/iowrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/iowrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/messages.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/messages.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/node_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/node_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/noder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/operator_new.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/print_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/print_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/property.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/property.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/property_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/property_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/stream_func.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/stream_func.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/tictoc.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/tictoc.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/timer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/tokenizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/base/tokenizer.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.180385 cytosim-0.0.5/src/cpython/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4555 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/couple_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13219 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/fiber_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/glossary_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6128 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/hand_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6486 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/interface_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8178 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/meca_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3303 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/object_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/organizer_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2330 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/point_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9076 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/python_frame.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3233 2023-08-04 06:55:58.000000 cytosim-0.0.5/src/cpython/python_utilities.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8838 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/simul_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/single_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5534 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/solid_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/space_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2669 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/cpython/thread_modules.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.184385 cytosim-0.0.5/src/disp/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12450 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17737 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29713 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/display_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/fiber_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/fiber_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/glapp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/gle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/gle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/gle_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/gle_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/gle_color_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/gle_color_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/glu_unproject.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/glut.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/grid_display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/grid_display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/line_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/line_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/miniz.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/miniz.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/offscreen.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/offscreen.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/offscreen_fbo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/offscreen_glx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/opengl.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/point_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/point_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/save_image.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/save_image.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/spng.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/spng.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/view.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/view.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5971 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/view_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/disp/view_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.188385 cytosim-0.0.5/src/math/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/SFMT-avx2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/SFMT-common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/SFMT-params.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/SFMT-params19937.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/SFMT-sse2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/SFMT.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/SFMT.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/accumulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/allocator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/bicgstab.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/cblas.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/clapack.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/dgtsv.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/dim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/evaluator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/gmres.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/grid_base.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/isometry.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/linear_operator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix11.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix11.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix22.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix22.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix33.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix33.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrix44.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matrixbase.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesym.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesym.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesym1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesym1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesym2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesym2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesymblk.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/matsparsesymblk.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/platonic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/pointsonsphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/pointsonsphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/project_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/project_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/quaternion.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/random.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/random_vector.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/random_vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/rasterizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/real.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/simd.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/simd_print.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/smath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vecprint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/math/vector4.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.192385 cytosim-0.0.5/src/misc/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/check_dump.m
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.192385 cytosim-0.0.5/src/misc/installation/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/RtMidi.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/RtMidi.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.192385 cytosim-0.0.5/src/misc/installation/builder/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/0-live.command
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config0.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config1.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config2.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config3.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config4.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config5.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config6.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config7.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/config8.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/builder/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/cytobuilder.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/cytomaster.cpp
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.192385 cytosim-0.0.5/src/misc/installation/cytomaster.xcodeproj/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/makefile
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.192385 cytosim-0.0.5/src/misc/installation/master/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/0-live.command
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config0.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config4.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config6.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config7.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config8.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/config9.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/master/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/rtmidi_c.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/misc/installation/rtmidi_c.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.192385 cytosim-0.0.5/src/play/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/play.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/play.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/play_keys.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/play_menus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/play_mouse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/player.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/player.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/player_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/player_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/play/player_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.204385 cytosim-0.0.5/src/sim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/bead.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/bead.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/bead_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/bead_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/bead_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/bead_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/chain.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/chain.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/common.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couple.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couple.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couple_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couple_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couple_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couple_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.204385 cytosim-0.0.5/src/sim/couples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/bridge.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/bridge.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/bridge_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/bridge_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/couple_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/couple_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/crosslink.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/crosslink.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/crosslink_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/crosslink_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/crosslink_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/crosslink_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/duo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/duo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/duo_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/duo_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/duo_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/duo_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/fork.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/fork.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/fork_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/fork_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/shackle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/shackle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/shackle_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/shackle_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/shackle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/couples/shackle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/event.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/event.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/event_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/event_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_grid2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16712 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_segment.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_segment.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_site.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fiber_site.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.208385 cytosim-0.0.5/src/sim/fibers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/classic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/classic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/classic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/classic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/dynamic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/dynamic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/dynamic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/dynamic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/growing_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/growing_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/growing_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/growing_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/treadmilling_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/treadmilling_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/treadmilling_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/fibers/treadmilling_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/field.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/field.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4522 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/field_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/field_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/field_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/field_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/field_values.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/frame_reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/frame_reader.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hand.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6855 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hand.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hand_monitor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hand_monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hand_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hand_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.212385 cytosim-0.0.5/src/sim/hands/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/actor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/actor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/actor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/actor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/chewer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/chewer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/chewer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/chewer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/cutter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/cutter.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1914 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/cutter_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/cutter_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/digit.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/digit.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/digit_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/digit_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/dynein.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/dynein.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/dynein_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/dynein_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/kinesin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/kinesin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/kinesin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/kinesin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/mighty.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/mighty.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/mighty_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/mighty_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/motor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/motor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/motor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/motor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/myosin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/myosin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/myosin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/myosin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/nucleator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/nucleator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/nucleator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/nucleator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/regulator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/regulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/regulator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/regulator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/rescuer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/rescuer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/rescuer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/rescuer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/slider.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/slider.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/slider_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/slider_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/tracker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/tracker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/tracker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/tracker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/walker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/walker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/walker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/hands/walker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/interface.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/interface.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/interpolation.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/interpolation.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/interpolation4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/interpolation4.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/lattice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/lattice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/meca.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22723 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/meca.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/meca1d.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/meca_inter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecafil.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecafil.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecafil_project.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecafil_projectmat.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecapoint.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/mecapoint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/modulo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/modulo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/movable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/movable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/object.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/object.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/object_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/object_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizer_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizer_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.212385 cytosim-0.0.5/src/sim/organizers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/aster.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/aster.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/aster_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/aster_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/bundle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/bundle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/bundle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/bundle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/fake.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/fake.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/fake_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/fake_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/nucleus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/nucleus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/nucleus_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/organizers/nucleus_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/parser.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/parser.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/point_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/point_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sim_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sim_thread.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19507 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul_custom.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul_file.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul_report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/simul_step.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/single.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/single.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/single_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/single_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/single_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/single_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.212385 cytosim-0.0.5/src/sim/singles/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/picket.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/picket.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/picket_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/picket_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/wrist.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/wrist.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/wrist_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/singles/wrist_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/solid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/solid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/solid_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/solid_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/solid_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/solid_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/space.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/space_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/space_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/space_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/space_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.216385 cytosim-0.0.5/src/sim/spaces/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_banana.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_banana.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_capsule.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_capsule.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_cylinder.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_cylinder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_cylinderP.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_cylinderP.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_cylinderZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_cylinderZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_dice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_dice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_periodic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_periodic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9540 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_polygonZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_polygonZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_ring.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_ring.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_square.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_square.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_strip.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_strip.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_torus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/spaces/space_torus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sphere_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sphere_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sphere_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/sphere_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/splash.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/sim/splash.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.216385 cytosim-0.0.5/src/test/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_blas.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_code.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_cxx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_dispatch.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_gillespie.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_glos.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_glut.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_glut3D.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_math.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_omp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_opengl.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_pipe.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_quaternion.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_signal.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_simd.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_sizeof.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_string.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/test/test_vbo.cc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 07:50:11.216385 cytosim-0.0.5/src/tools/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/cymart.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/frametool.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10045 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/pycytoplay.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5543 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/pycytosim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/pycytosim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/reportF.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2023-08-03 15:27:32.000000 cytosim-0.0.5/src/tools/sieve.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.120073 cytosim-0.0.6/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2023-08-03 15:27:32.000000 cytosim-0.0.6/.gitignore
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-04 07:08:34.000000 cytosim-0.0.6/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2023-08-03 15:27:32.000000 cytosim-0.0.6/LICENSE.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4751 2023-08-04 12:53:40.120073 cytosim-0.0.6/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2023-08-03 15:27:32.000000 cytosim-0.0.6/PYCYTOSIM.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3752 2023-08-03 15:27:32.000000 cytosim-0.0.6/README.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2023-08-03 15:27:32.000000 cytosim-0.0.6/WARRANTY.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.068073 cytosim-0.0.6/cytosim.egg-info/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4751 2023-08-04 12:53:39.000000 cytosim-0.0.6/cytosim.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14193 2023-08-04 12:53:40.000000 cytosim-0.0.6/cytosim.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-04 12:53:39.000000 cytosim-0.0.6/cytosim.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-04 12:53:39.000000 cytosim-0.0.6/cytosim.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       18 2023-08-04 12:53:39.000000 cytosim-0.0.6/cytosim.egg-info/top_level.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2023-08-03 15:27:32.000000 cytosim-0.0.6/makefile
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12556 2023-08-03 15:27:32.000000 cytosim-0.0.6/makefile.inc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.068073 cytosim-0.0.6/pycytosim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12212 2023-08-04 07:31:58.000000 cytosim-0.0.6/pycytosim/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       23 2023-08-03 15:28:09.000000 cytosim-0.0.6/pycytosim/__init__.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.068073 cytosim-0.0.6/python/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.068073 cytosim-0.0.6/python/look/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/collect.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/compare_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/get_data.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/make_image.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/make_movie.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/make_page.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/make_plots.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/read_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/scan.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/look/tell.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.068073 cytosim-0.0.6/python/misc/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/misc/battery_test.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/misc/cleanup.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/misc/compare.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/misc/plot.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/misc/pyned.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/misc/reduce.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.068073 cytosim-0.0.6/python/run/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/run/go_sim.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/run/go_sim_lib.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23500 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/run/preconfig.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/run/submit_one.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2023-08-03 15:27:32.000000 cytosim-0.0.6/python/run/submit_slurm.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2023-08-04 12:53:40.120073 cytosim-0.0.6/setup.cfg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4833 2023-08-04 12:50:12.000000 cytosim-0.0.6/setup.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.068073 cytosim-0.0.6/src/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/CMakeLists.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.072073 cytosim-0.0.6/src/base/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/array.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/assert_macro.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/backtrace.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/backtrace.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/buddy.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/exceptions.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/exceptions.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/filepath.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/filepath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/filewrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/filewrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/glossary.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/glossary.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/inventoried.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/inventory.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/inventory.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/iowrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/iowrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/messages.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/messages.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/node_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/node_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/noder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/operator_new.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/print_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/print_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/property.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/property.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/property_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/property_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/stream_func.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/stream_func.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/tictoc.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/tictoc.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/timer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/tokenizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/base/tokenizer.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.072073 cytosim-0.0.6/src/cpython/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4555 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/couple_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13219 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/fiber_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/glossary_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6128 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/hand_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6486 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/interface_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8178 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/meca_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3303 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/object_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/organizer_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2330 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/point_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9076 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/python_frame.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3233 2023-08-04 06:55:58.000000 cytosim-0.0.6/src/cpython/python_utilities.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8838 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/simul_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/single_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5534 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/solid_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/space_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2669 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/cpython/thread_modules.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.080073 cytosim-0.0.6/src/disp/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12450 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17737 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29713 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/display_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/fiber_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/fiber_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/glapp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/gle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/gle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/gle_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/gle_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/gle_color_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/gle_color_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/glu_unproject.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/glut.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/grid_display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/grid_display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/line_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/line_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/miniz.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/miniz.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/offscreen.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/offscreen.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/offscreen_fbo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/offscreen_glx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/opengl.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/point_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/point_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/save_image.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/save_image.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/spng.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/spng.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/view.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/view.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5971 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/view_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/disp/view_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.088073 cytosim-0.0.6/src/math/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/SFMT-avx2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/SFMT-common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/SFMT-params.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/SFMT-params19937.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/SFMT-sse2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/SFMT.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/SFMT.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/accumulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/allocator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/bicgstab.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/cblas.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/clapack.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/dgtsv.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/dim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/evaluator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/gmres.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/grid_base.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/isometry.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/linear_operator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix11.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix11.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix22.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix22.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix33.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix33.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrix44.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matrixbase.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesym.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesym.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesym1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesym1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesym2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesym2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesymblk.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/matsparsesymblk.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/platonic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/pointsonsphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/pointsonsphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/project_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/project_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/quaternion.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/random.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/random_vector.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/random_vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/rasterizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/real.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/simd.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/simd_print.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/smath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vecprint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/math/vector4.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.088073 cytosim-0.0.6/src/misc/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/check_dump.m
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.088073 cytosim-0.0.6/src/misc/installation/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/RtMidi.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/RtMidi.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.088073 cytosim-0.0.6/src/misc/installation/builder/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/0-live.command
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config0.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config1.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config2.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config3.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config4.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config5.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config6.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config7.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/config8.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/builder/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/cytobuilder.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/cytomaster.cpp
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.088073 cytosim-0.0.6/src/misc/installation/cytomaster.xcodeproj/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/makefile
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.088073 cytosim-0.0.6/src/misc/installation/master/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/0-live.command
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config0.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config4.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config6.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config7.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config8.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/config9.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/master/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/rtmidi_c.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/misc/installation/rtmidi_c.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.092073 cytosim-0.0.6/src/play/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/play.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/play.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/play_keys.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/play_menus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/play_mouse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/player.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/player.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/player_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/player_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/play/player_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.104073 cytosim-0.0.6/src/sim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/bead.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/bead.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/bead_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/bead_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/bead_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/bead_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/chain.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/chain.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/common.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couple.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couple.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couple_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couple_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couple_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couple_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.104073 cytosim-0.0.6/src/sim/couples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/bridge.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/bridge.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/bridge_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/bridge_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/couple_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/couple_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/crosslink.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/crosslink.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/crosslink_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/crosslink_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/crosslink_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/crosslink_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/duo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/duo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/duo_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/duo_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/duo_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/duo_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/fork.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/fork.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/fork_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/fork_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/shackle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/shackle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/shackle_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/shackle_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/shackle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/couples/shackle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/event.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/event.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/event_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/event_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_grid2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16712 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_segment.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_segment.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_site.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fiber_site.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.108073 cytosim-0.0.6/src/sim/fibers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/classic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/classic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/classic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/classic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/dynamic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/dynamic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/dynamic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/dynamic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/growing_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/growing_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/growing_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/growing_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/treadmilling_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/treadmilling_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/treadmilling_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/fibers/treadmilling_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/field.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/field.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4522 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/field_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/field_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/field_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/field_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/field_values.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/frame_reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/frame_reader.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hand.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6855 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hand.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hand_monitor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hand_monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hand_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hand_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.112073 cytosim-0.0.6/src/sim/hands/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/actor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/actor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/actor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/actor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/chewer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/chewer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/chewer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/chewer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/cutter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/cutter.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1914 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/cutter_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/cutter_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/digit.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/digit.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/digit_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/digit_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/dynein.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/dynein.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/dynein_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/dynein_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/kinesin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/kinesin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/kinesin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/kinesin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/mighty.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/mighty.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/mighty_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/mighty_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/motor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/motor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/motor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/motor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/myosin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/myosin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/myosin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/myosin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/nucleator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/nucleator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/nucleator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/nucleator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/regulator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/regulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/regulator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/regulator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/rescuer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/rescuer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/rescuer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/rescuer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/slider.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/slider.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/slider_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/slider_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/tracker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/tracker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/tracker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/tracker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/walker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/walker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/walker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/hands/walker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/interface.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/interface.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/interpolation.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/interpolation.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/interpolation4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/interpolation4.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/lattice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/lattice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/meca.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22723 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/meca.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/meca1d.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/meca_inter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecafil.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecafil.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecafil_project.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecafil_projectmat.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecapoint.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/mecapoint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/modulo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/modulo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/movable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/movable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/object.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/object.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/object_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/object_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizer_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizer_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.116073 cytosim-0.0.6/src/sim/organizers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/aster.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/aster.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/aster_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/aster_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/bundle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/bundle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/bundle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/bundle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/fake.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/fake.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/fake_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/fake_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/nucleus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/nucleus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/nucleus_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/organizers/nucleus_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/parser.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/parser.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/point_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/point_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sim_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sim_thread.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19507 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul_custom.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul_file.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul_report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/simul_step.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/single.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/single.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/single_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/single_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/single_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/single_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.116073 cytosim-0.0.6/src/sim/singles/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/picket.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/picket.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/picket_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/picket_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/wrist.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/wrist.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/wrist_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/singles/wrist_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/solid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/solid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/solid_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/solid_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/solid_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/solid_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/space.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/space_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/space_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/space_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/space_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.116073 cytosim-0.0.6/src/sim/spaces/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_banana.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_banana.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_capsule.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_capsule.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_cylinder.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_cylinder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_cylinderP.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_cylinderP.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_cylinderZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_cylinderZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_dice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_dice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_periodic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_periodic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9540 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_polygonZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_polygonZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_ring.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_ring.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_square.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_square.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_strip.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_strip.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_torus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/spaces/space_torus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sphere_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sphere_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sphere_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/sphere_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/splash.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/sim/splash.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.120073 cytosim-0.0.6/src/test/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_blas.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_code.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_cxx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_dispatch.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_gillespie.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_glos.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_glut.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_glut3D.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_math.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_omp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_opengl.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_pipe.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_quaternion.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_signal.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_simd.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_sizeof.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_string.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/test/test_vbo.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-04 12:53:40.120073 cytosim-0.0.6/src/tools/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/cymart.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/frametool.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10045 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/pycytoplay.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5543 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/pycytosim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/pycytosim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/reportF.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2023-08-03 15:27:32.000000 cytosim-0.0.6/src/tools/sieve.cc
```

### Comparing `cytosim-0.0.5/.gitignore` & `cytosim-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/CMakeLists.txt` & `cytosim-0.0.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/LICENSE.txt` & `cytosim-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/PKG-INFO` & `cytosim-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytosim
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cytosim: Langevin dynamics of active polymer networks
 Keywords: simulation actin microtubule polymer
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cytosim-0.0.5/PYCYTOSIM.md` & `cytosim-0.0.6/PYCYTOSIM.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/README.md` & `cytosim-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/WARRANTY.txt` & `cytosim-0.0.6/WARRANTY.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/cytosim.egg-info/PKG-INFO` & `cytosim-0.0.6/cytosim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytosim
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cytosim: Langevin dynamics of active polymer networks
 Keywords: simulation actin microtubule polymer
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cytosim-0.0.5/cytosim.egg-info/SOURCES.txt` & `cytosim-0.0.6/cytosim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/makefile` & `cytosim-0.0.6/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/makefile.inc` & `cytosim-0.0.6/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/pycytosim/CMakeLists.txt` & `cytosim-0.0.6/pycytosim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/index.md` & `cytosim-0.0.6/python/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/collect.py` & `cytosim-0.0.6/python/look/collect.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/compare_config.py` & `cytosim-0.0.6/python/look/compare_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/get_data.py` & `cytosim-0.0.6/python/look/get_data.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/make_image.py` & `cytosim-0.0.6/python/look/make_image.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/make_movie.py` & `cytosim-0.0.6/python/look/make_movie.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/make_page.py` & `cytosim-0.0.6/python/look/make_page.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/make_plots.py` & `cytosim-0.0.6/python/look/make_plots.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/read_config.py` & `cytosim-0.0.6/python/look/read_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/scan.py` & `cytosim-0.0.6/python/look/scan.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/look/tell.py` & `cytosim-0.0.6/python/look/tell.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/misc/battery_test.py` & `cytosim-0.0.6/python/misc/battery_test.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/misc/cleanup.py` & `cytosim-0.0.6/python/misc/cleanup.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/misc/compare.py` & `cytosim-0.0.6/python/misc/compare.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/misc/plot.py` & `cytosim-0.0.6/python/misc/plot.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/misc/pyned.py` & `cytosim-0.0.6/python/misc/pyned.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/misc/reduce.py` & `cytosim-0.0.6/python/misc/reduce.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/run/go_sim.py` & `cytosim-0.0.6/python/run/go_sim.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/run/go_sim_lib.py` & `cytosim-0.0.6/python/run/go_sim_lib.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/run/preconfig.py` & `cytosim-0.0.6/python/run/preconfig.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/run/submit_one.py` & `cytosim-0.0.6/python/run/submit_one.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/python/run/submit_slurm.py` & `cytosim-0.0.6/python/run/submit_slurm.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/setup.py` & `cytosim-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 import sys
 import subprocess
 import re
 import platform
 import shutil
 import sysconfig
 import setuptools
+#import pybind11
 from setuptools.command import build_ext
+from setuptools import setup
+from setuptools import find_packages
+#from pybind11.setup_helpers import Pybind11Extension
 
-
-from pybind11.setup_helpers import Pybind11Extension
-version = "0.0.5"
+version = "0.0.6"
 cmake_args=[]
 
 
 if('CONDA_PREFIX' in os.environ):
     print("Setting library search path (CMAKE_PREFIX_PATH): %s"%(os.environ['CONDA_PREFIX']))
     cmake_args.append('-DCMAKE_PREFIX_PATH=%s'%(os.environ['CONDA_PREFIX']))
-else:
-    print("no conda prefix")
 
 DOCLINES = __doc__.split("\n")
 
 CLASSIFIERS = """\
 Development Status :: 3 - Alpha
 Environment :: Console
 Intended Audience :: Science/Research
@@ -41,17 +41,15 @@
 Programming Language :: Python :: Implementation :: CPython
 Topic :: Scientific/Engineering :: Chemistry
 Topic :: Scientific/Engineering :: Mathematics
 Topic :: Scientific/Engineering :: Physics
 Topic :: Scientific/Engineering :: Visualization
 """
 
-from setuptools import setup
 
-from setuptools import find_packages
 
 
 #__DIMENSION__ = 2
 
 
 
 class CMakeExtension(setuptools.Extension):
```

### Comparing `cytosim-0.0.5/src/base/CMakeLists.txt` & `cytosim-0.0.6/src/base/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/array.h` & `cytosim-0.0.6/src/base/array.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/assert_macro.h` & `cytosim-0.0.6/src/base/assert_macro.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/backtrace.cc` & `cytosim-0.0.6/src/base/backtrace.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/backtrace.h` & `cytosim-0.0.6/src/base/backtrace.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/buddy.h` & `cytosim-0.0.6/src/base/buddy.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/exceptions.h` & `cytosim-0.0.6/src/base/exceptions.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/filepath.cc` & `cytosim-0.0.6/src/base/filepath.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/filepath.h` & `cytosim-0.0.6/src/base/filepath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/filewrapper.cc` & `cytosim-0.0.6/src/base/filewrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/filewrapper.h` & `cytosim-0.0.6/src/base/filewrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/glossary.cc` & `cytosim-0.0.6/src/base/glossary.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/glossary.h` & `cytosim-0.0.6/src/base/glossary.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/inventoried.h` & `cytosim-0.0.6/src/base/inventoried.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/inventory.cc` & `cytosim-0.0.6/src/base/inventory.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/inventory.h` & `cytosim-0.0.6/src/base/inventory.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/iowrapper.cc` & `cytosim-0.0.6/src/base/iowrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/iowrapper.h` & `cytosim-0.0.6/src/base/iowrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/makefile.inc` & `cytosim-0.0.6/src/base/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/messages.cc` & `cytosim-0.0.6/src/base/messages.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/messages.h` & `cytosim-0.0.6/src/base/messages.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/node_list.cc` & `cytosim-0.0.6/src/base/node_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/node_list.h` & `cytosim-0.0.6/src/base/node_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/noder.h` & `cytosim-0.0.6/src/base/noder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/operator_new.cc` & `cytosim-0.0.6/src/base/operator_new.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/print_color.cc` & `cytosim-0.0.6/src/base/print_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/print_color.h` & `cytosim-0.0.6/src/base/print_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/property.cc` & `cytosim-0.0.6/src/base/property.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/property.h` & `cytosim-0.0.6/src/base/property.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/property_list.cc` & `cytosim-0.0.6/src/base/property_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/property_list.h` & `cytosim-0.0.6/src/base/property_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/stream_func.cc` & `cytosim-0.0.6/src/base/stream_func.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/stream_func.h` & `cytosim-0.0.6/src/base/stream_func.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/tictoc.cc` & `cytosim-0.0.6/src/base/tictoc.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/tictoc.h` & `cytosim-0.0.6/src/base/tictoc.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/timer.h` & `cytosim-0.0.6/src/base/timer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/tokenizer.cc` & `cytosim-0.0.6/src/base/tokenizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/base/tokenizer.h` & `cytosim-0.0.6/src/base/tokenizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/couple_modules.h` & `cytosim-0.0.6/src/cpython/couple_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/fiber_modules.h` & `cytosim-0.0.6/src/cpython/fiber_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/glossary_modules.h` & `cytosim-0.0.6/src/cpython/glossary_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/hand_modules.h` & `cytosim-0.0.6/src/cpython/hand_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/interface_modules.h` & `cytosim-0.0.6/src/cpython/interface_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/meca_modules.h` & `cytosim-0.0.6/src/cpython/meca_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/object_modules.h` & `cytosim-0.0.6/src/cpython/object_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/organizer_modules.h` & `cytosim-0.0.6/src/cpython/organizer_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/point_modules.h` & `cytosim-0.0.6/src/cpython/point_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/python_frame.h` & `cytosim-0.0.6/src/cpython/python_frame.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/python_utilities.h` & `cytosim-0.0.6/src/cpython/python_utilities.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/simul_modules.h` & `cytosim-0.0.6/src/cpython/simul_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/single_modules.h` & `cytosim-0.0.6/src/cpython/single_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/solid_modules.h` & `cytosim-0.0.6/src/cpython/solid_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/space_modules.h` & `cytosim-0.0.6/src/cpython/space_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/cpython/thread_modules.h` & `cytosim-0.0.6/src/cpython/thread_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/CMakeLists.txt` & `cytosim-0.0.6/src/disp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display.cc` & `cytosim-0.0.6/src/disp/display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display.h` & `cytosim-0.0.6/src/disp/display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display1.cc` & `cytosim-0.0.6/src/disp/display1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display1.h` & `cytosim-0.0.6/src/disp/display1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display2.cc` & `cytosim-0.0.6/src/disp/display2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display2.h` & `cytosim-0.0.6/src/disp/display2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display3.cc` & `cytosim-0.0.6/src/disp/display3.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display3.h` & `cytosim-0.0.6/src/disp/display3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display_prop.cc` & `cytosim-0.0.6/src/disp/display_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/display_prop.h` & `cytosim-0.0.6/src/disp/display_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/fiber_disp.cc` & `cytosim-0.0.6/src/disp/fiber_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/fiber_disp.h` & `cytosim-0.0.6/src/disp/fiber_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/glapp.cc` & `cytosim-0.0.6/src/disp/glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/glapp.h` & `cytosim-0.0.6/src/disp/glapp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/gle.cc` & `cytosim-0.0.6/src/disp/gle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/gle.h` & `cytosim-0.0.6/src/disp/gle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/gle_color.cc` & `cytosim-0.0.6/src/disp/gle_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/gle_color.h` & `cytosim-0.0.6/src/disp/gle_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/gle_color_list.cc` & `cytosim-0.0.6/src/disp/gle_color_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/gle_color_list.h` & `cytosim-0.0.6/src/disp/gle_color_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/glu_unproject.cc` & `cytosim-0.0.6/src/disp/glu_unproject.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/grid_display.cc` & `cytosim-0.0.6/src/disp/grid_display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/grid_display.h` & `cytosim-0.0.6/src/disp/grid_display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/line_disp.h` & `cytosim-0.0.6/src/disp/line_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/makefile.inc` & `cytosim-0.0.6/src/disp/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/miniz.c` & `cytosim-0.0.6/src/disp/miniz.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/miniz.h` & `cytosim-0.0.6/src/disp/miniz.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/offscreen.cc` & `cytosim-0.0.6/src/disp/offscreen.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/offscreen.h` & `cytosim-0.0.6/src/disp/offscreen.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/offscreen_fbo.cc` & `cytosim-0.0.6/src/disp/offscreen_fbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/offscreen_glx.cc` & `cytosim-0.0.6/src/disp/offscreen_glx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/point_disp.cc` & `cytosim-0.0.6/src/disp/point_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/point_disp.h` & `cytosim-0.0.6/src/disp/point_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/save_image.cc` & `cytosim-0.0.6/src/disp/save_image.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/save_image.h` & `cytosim-0.0.6/src/disp/save_image.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/spng.c` & `cytosim-0.0.6/src/disp/spng.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/spng.h` & `cytosim-0.0.6/src/disp/spng.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/view.cc` & `cytosim-0.0.6/src/disp/view.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/view.h` & `cytosim-0.0.6/src/disp/view.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/view_prop.cc` & `cytosim-0.0.6/src/disp/view_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/disp/view_prop.h` & `cytosim-0.0.6/src/disp/view_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/index.md` & `cytosim-0.0.6/src/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/CMakeLists.txt` & `cytosim-0.0.6/src/math/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/SFMT-avx2.h` & `cytosim-0.0.6/src/math/SFMT-avx2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/SFMT-common.h` & `cytosim-0.0.6/src/math/SFMT-common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/SFMT-params.h` & `cytosim-0.0.6/src/math/SFMT-params.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/SFMT-params19937.h` & `cytosim-0.0.6/src/math/SFMT-params19937.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/SFMT-sse2.h` & `cytosim-0.0.6/src/math/SFMT-sse2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/SFMT.c` & `cytosim-0.0.6/src/math/SFMT.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/SFMT.h` & `cytosim-0.0.6/src/math/SFMT.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/accumulator.h` & `cytosim-0.0.6/src/math/accumulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/allocator.h` & `cytosim-0.0.6/src/math/allocator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/bicgstab.h` & `cytosim-0.0.6/src/math/bicgstab.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/cblas.h` & `cytosim-0.0.6/src/math/cblas.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/clapack.h` & `cytosim-0.0.6/src/math/clapack.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/dgtsv.c` & `cytosim-0.0.6/src/math/dgtsv.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/evaluator.h` & `cytosim-0.0.6/src/math/evaluator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/gmres.h` & `cytosim-0.0.6/src/math/gmres.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/grid.h` & `cytosim-0.0.6/src/math/grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/grid_base.h` & `cytosim-0.0.6/src/math/grid_base.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/isometry.h` & `cytosim-0.0.6/src/math/isometry.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/linear_operator.h` & `cytosim-0.0.6/src/math/linear_operator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/makefile.inc` & `cytosim-0.0.6/src/math/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix.cc` & `cytosim-0.0.6/src/math/matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix.h` & `cytosim-0.0.6/src/math/matrix.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix11.cc` & `cytosim-0.0.6/src/math/matrix11.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix11.h` & `cytosim-0.0.6/src/math/matrix11.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix22.cc` & `cytosim-0.0.6/src/math/matrix22.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix22.h` & `cytosim-0.0.6/src/math/matrix22.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix33.cc` & `cytosim-0.0.6/src/math/matrix33.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix33.h` & `cytosim-0.0.6/src/math/matrix33.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrix44.h` & `cytosim-0.0.6/src/math/matrix44.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matrixbase.h` & `cytosim-0.0.6/src/math/matrixbase.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparse.cc` & `cytosim-0.0.6/src/math/matsparse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparse.h` & `cytosim-0.0.6/src/math/matsparse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesym.cc` & `cytosim-0.0.6/src/math/matsparsesym.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesym.h` & `cytosim-0.0.6/src/math/matsparsesym.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesym1.cc` & `cytosim-0.0.6/src/math/matsparsesym1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesym1.h` & `cytosim-0.0.6/src/math/matsparsesym1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesym2.cc` & `cytosim-0.0.6/src/math/matsparsesym2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesym2.h` & `cytosim-0.0.6/src/math/matsparsesym2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesymblk.cc` & `cytosim-0.0.6/src/math/matsparsesymblk.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/matsparsesymblk.h` & `cytosim-0.0.6/src/math/matsparsesymblk.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/monitor.h` & `cytosim-0.0.6/src/math/monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/platonic.cc` & `cytosim-0.0.6/src/math/platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/platonic.h` & `cytosim-0.0.6/src/math/platonic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/pointsonsphere.cc` & `cytosim-0.0.6/src/math/pointsonsphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/pointsonsphere.h` & `cytosim-0.0.6/src/math/pointsonsphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/polygon.cc` & `cytosim-0.0.6/src/math/polygon.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/polygon.h` & `cytosim-0.0.6/src/math/polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/project_ellipse.cc` & `cytosim-0.0.6/src/math/project_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/project_ellipse.h` & `cytosim-0.0.6/src/math/project_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/quaternion.h` & `cytosim-0.0.6/src/math/quaternion.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/random.cc` & `cytosim-0.0.6/src/math/random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/random.h` & `cytosim-0.0.6/src/math/random.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/random_vector.cc` & `cytosim-0.0.6/src/math/random_vector.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/random_vector.h` & `cytosim-0.0.6/src/math/random_vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/rasterizer.cc` & `cytosim-0.0.6/src/math/rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/rasterizer.h` & `cytosim-0.0.6/src/math/rasterizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/real.h` & `cytosim-0.0.6/src/math/real.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/simd.h` & `cytosim-0.0.6/src/math/simd.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/simd_print.h` & `cytosim-0.0.6/src/math/simd_print.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/smath.h` & `cytosim-0.0.6/src/math/smath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vecprint.h` & `cytosim-0.0.6/src/math/vecprint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector.h` & `cytosim-0.0.6/src/math/vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector1.cc` & `cytosim-0.0.6/src/math/vector1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector1.h` & `cytosim-0.0.6/src/math/vector1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector2.cc` & `cytosim-0.0.6/src/math/vector2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector2.h` & `cytosim-0.0.6/src/math/vector2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector3.cc` & `cytosim-0.0.6/src/math/vector3.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector3.h` & `cytosim-0.0.6/src/math/vector3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector4.cc` & `cytosim-0.0.6/src/math/vector4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/math/vector4.h` & `cytosim-0.0.6/src/math/vector4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/check_dump.m` & `cytosim-0.0.6/src/misc/check_dump.m`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/RtMidi.cpp` & `cytosim-0.0.6/src/misc/installation/RtMidi.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/RtMidi.h` & `cytosim-0.0.6/src/misc/installation/RtMidi.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/0-live.command` & `cytosim-0.0.6/src/misc/installation/builder/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config.cym` & `cytosim-0.0.6/src/misc/installation/builder/config.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config0.cym` & `cytosim-0.0.6/src/misc/installation/builder/config0.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config1.cym` & `cytosim-0.0.6/src/misc/installation/builder/config1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config2.cym` & `cytosim-0.0.6/src/misc/installation/builder/config2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config3.cym` & `cytosim-0.0.6/src/misc/installation/builder/config3.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config4.cym` & `cytosim-0.0.6/src/misc/installation/builder/config4.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config5.cym` & `cytosim-0.0.6/src/misc/installation/builder/config5.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config6.cym` & `cytosim-0.0.6/src/misc/installation/builder/config6.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config7.cym` & `cytosim-0.0.6/src/misc/installation/builder/config7.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/config8.cym` & `cytosim-0.0.6/src/misc/installation/builder/config8.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/builder/france.txt` & `cytosim-0.0.6/src/misc/installation/builder/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/cytobuilder.cpp` & `cytosim-0.0.6/src/misc/installation/cytobuilder.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/cytomaster.cpp` & `cytosim-0.0.6/src/misc/installation/cytomaster.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/cytomaster.xcodeproj/project.pbxproj` & `cytosim-0.0.6/src/misc/installation/cytomaster.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/makefile` & `cytosim-0.0.6/src/misc/installation/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/0-live.command` & `cytosim-0.0.6/src/misc/installation/master/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config0.cym` & `cytosim-0.0.6/src/misc/installation/master/config0.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config1.cym` & `cytosim-0.0.6/src/misc/installation/master/config1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config2.cym` & `cytosim-0.0.6/src/misc/installation/master/config2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config4.cym` & `cytosim-0.0.6/src/misc/installation/master/config4.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config6.cym` & `cytosim-0.0.6/src/misc/installation/master/config6.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config7.cym` & `cytosim-0.0.6/src/misc/installation/master/config7.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config8.cym` & `cytosim-0.0.6/src/misc/installation/master/config8.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/config9.cym` & `cytosim-0.0.6/src/misc/installation/master/config9.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/master/france.txt` & `cytosim-0.0.6/src/misc/installation/master/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/rtmidi_c.cpp` & `cytosim-0.0.6/src/misc/installation/rtmidi_c.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/misc/installation/rtmidi_c.h` & `cytosim-0.0.6/src/misc/installation/rtmidi_c.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/CMakeLists.txt` & `cytosim-0.0.6/src/play/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/makefile.inc` & `cytosim-0.0.6/src/play/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/play.cc` & `cytosim-0.0.6/src/play/play.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/play_keys.cc` & `cytosim-0.0.6/src/play/play_keys.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/play_menus.cc` & `cytosim-0.0.6/src/play/play_menus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/play_mouse.cc` & `cytosim-0.0.6/src/play/play_mouse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/player.cc` & `cytosim-0.0.6/src/play/player.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/player.h` & `cytosim-0.0.6/src/play/player.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/player_disp.cc` & `cytosim-0.0.6/src/play/player_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/player_prop.cc` & `cytosim-0.0.6/src/play/player_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/play/player_prop.h` & `cytosim-0.0.6/src/play/player_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/CMakeLists.txt` & `cytosim-0.0.6/src/sim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/bead.cc` & `cytosim-0.0.6/src/sim/bead.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/bead.h` & `cytosim-0.0.6/src/sim/bead.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/bead_set.cc` & `cytosim-0.0.6/src/sim/bead_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/bead_set.h` & `cytosim-0.0.6/src/sim/bead_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/chain.cc` & `cytosim-0.0.6/src/sim/chain.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/chain.h` & `cytosim-0.0.6/src/sim/chain.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/common.h` & `cytosim-0.0.6/src/sim/common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couple.cc` & `cytosim-0.0.6/src/sim/couple.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couple.h` & `cytosim-0.0.6/src/sim/couple.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couple_prop.cc` & `cytosim-0.0.6/src/sim/couple_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couple_prop.h` & `cytosim-0.0.6/src/sim/couple_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couple_set.cc` & `cytosim-0.0.6/src/sim/couple_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couple_set.h` & `cytosim-0.0.6/src/sim/couple_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/bridge.cc` & `cytosim-0.0.6/src/sim/couples/bridge.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/bridge.h` & `cytosim-0.0.6/src/sim/couples/bridge.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/bridge_prop.cc` & `cytosim-0.0.6/src/sim/couples/bridge_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/bridge_prop.h` & `cytosim-0.0.6/src/sim/couples/bridge_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/couple_long.cc` & `cytosim-0.0.6/src/sim/couples/couple_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/couple_long.h` & `cytosim-0.0.6/src/sim/couples/couple_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/crosslink.cc` & `cytosim-0.0.6/src/sim/couples/crosslink.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/crosslink.h` & `cytosim-0.0.6/src/sim/couples/crosslink.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/crosslink_long.cc` & `cytosim-0.0.6/src/sim/couples/crosslink_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/crosslink_long.h` & `cytosim-0.0.6/src/sim/couples/crosslink_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/crosslink_prop.cc` & `cytosim-0.0.6/src/sim/couples/crosslink_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/crosslink_prop.h` & `cytosim-0.0.6/src/sim/couples/crosslink_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/duo.cc` & `cytosim-0.0.6/src/sim/couples/duo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/duo.h` & `cytosim-0.0.6/src/sim/couples/duo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/duo_long.cc` & `cytosim-0.0.6/src/sim/couples/duo_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/duo_long.h` & `cytosim-0.0.6/src/sim/couples/duo_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/duo_prop.cc` & `cytosim-0.0.6/src/sim/couples/duo_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/duo_prop.h` & `cytosim-0.0.6/src/sim/couples/duo_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/fork.cc` & `cytosim-0.0.6/src/sim/couples/fork.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/fork.h` & `cytosim-0.0.6/src/sim/couples/fork.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/fork_prop.cc` & `cytosim-0.0.6/src/sim/couples/fork_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/fork_prop.h` & `cytosim-0.0.6/src/sim/couples/fork_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/shackle.cc` & `cytosim-0.0.6/src/sim/couples/shackle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/shackle.h` & `cytosim-0.0.6/src/sim/couples/shackle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/shackle_long.cc` & `cytosim-0.0.6/src/sim/couples/shackle_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/shackle_long.h` & `cytosim-0.0.6/src/sim/couples/shackle_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/shackle_prop.cc` & `cytosim-0.0.6/src/sim/couples/shackle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/couples/shackle_prop.h` & `cytosim-0.0.6/src/sim/couples/shackle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/event.cc` & `cytosim-0.0.6/src/sim/event.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/event.h` & `cytosim-0.0.6/src/sim/event.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/event_set.cc` & `cytosim-0.0.6/src/sim/event_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/event_set.h` & `cytosim-0.0.6/src/sim/event_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber.cc` & `cytosim-0.0.6/src/sim/fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber.h` & `cytosim-0.0.6/src/sim/fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_grid.cc` & `cytosim-0.0.6/src/sim/fiber_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_grid.h` & `cytosim-0.0.6/src/sim/fiber_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_grid2.cc` & `cytosim-0.0.6/src/sim/fiber_grid2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_prop.cc` & `cytosim-0.0.6/src/sim/fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_prop.h` & `cytosim-0.0.6/src/sim/fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_segment.cc` & `cytosim-0.0.6/src/sim/fiber_segment.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_segment.h` & `cytosim-0.0.6/src/sim/fiber_segment.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_set.cc` & `cytosim-0.0.6/src/sim/fiber_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_set.h` & `cytosim-0.0.6/src/sim/fiber_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_site.cc` & `cytosim-0.0.6/src/sim/fiber_site.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fiber_site.h` & `cytosim-0.0.6/src/sim/fiber_site.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/classic_fiber.cc` & `cytosim-0.0.6/src/sim/fibers/classic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/classic_fiber.h` & `cytosim-0.0.6/src/sim/fibers/classic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/classic_fiber_prop.cc` & `cytosim-0.0.6/src/sim/fibers/classic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/classic_fiber_prop.h` & `cytosim-0.0.6/src/sim/fibers/classic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/dynamic_fiber.cc` & `cytosim-0.0.6/src/sim/fibers/dynamic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/dynamic_fiber.h` & `cytosim-0.0.6/src/sim/fibers/dynamic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/dynamic_fiber_prop.cc` & `cytosim-0.0.6/src/sim/fibers/dynamic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/dynamic_fiber_prop.h` & `cytosim-0.0.6/src/sim/fibers/dynamic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/growing_fiber.cc` & `cytosim-0.0.6/src/sim/fibers/growing_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/growing_fiber.h` & `cytosim-0.0.6/src/sim/fibers/growing_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/growing_fiber_prop.cc` & `cytosim-0.0.6/src/sim/fibers/growing_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/growing_fiber_prop.h` & `cytosim-0.0.6/src/sim/fibers/growing_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/treadmilling_fiber.cc` & `cytosim-0.0.6/src/sim/fibers/treadmilling_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/treadmilling_fiber.h` & `cytosim-0.0.6/src/sim/fibers/treadmilling_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/treadmilling_fiber_prop.cc` & `cytosim-0.0.6/src/sim/fibers/treadmilling_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/fibers/treadmilling_fiber_prop.h` & `cytosim-0.0.6/src/sim/fibers/treadmilling_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/field.cc` & `cytosim-0.0.6/src/sim/field.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/field.h` & `cytosim-0.0.6/src/sim/field.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/field_prop.cc` & `cytosim-0.0.6/src/sim/field_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/field_prop.h` & `cytosim-0.0.6/src/sim/field_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/field_set.cc` & `cytosim-0.0.6/src/sim/field_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/field_set.h` & `cytosim-0.0.6/src/sim/field_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/field_values.h` & `cytosim-0.0.6/src/sim/field_values.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/frame_reader.cc` & `cytosim-0.0.6/src/sim/frame_reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/frame_reader.h` & `cytosim-0.0.6/src/sim/frame_reader.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hand.cc` & `cytosim-0.0.6/src/sim/hand.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hand.h` & `cytosim-0.0.6/src/sim/hand.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hand_monitor.h` & `cytosim-0.0.6/src/sim/hand_monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hand_prop.cc` & `cytosim-0.0.6/src/sim/hand_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hand_prop.h` & `cytosim-0.0.6/src/sim/hand_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/actor.cc` & `cytosim-0.0.6/src/sim/hands/actor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/actor.h` & `cytosim-0.0.6/src/sim/hands/actor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/actor_prop.cc` & `cytosim-0.0.6/src/sim/hands/actor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/actor_prop.h` & `cytosim-0.0.6/src/sim/hands/actor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/chewer.cc` & `cytosim-0.0.6/src/sim/hands/chewer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/chewer.h` & `cytosim-0.0.6/src/sim/hands/chewer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/chewer_prop.cc` & `cytosim-0.0.6/src/sim/hands/chewer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/chewer_prop.h` & `cytosim-0.0.6/src/sim/hands/chewer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/cutter.cc` & `cytosim-0.0.6/src/sim/hands/cutter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/cutter.h` & `cytosim-0.0.6/src/sim/hands/cutter.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/cutter_prop.cc` & `cytosim-0.0.6/src/sim/hands/cutter_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/cutter_prop.h` & `cytosim-0.0.6/src/sim/hands/cutter_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/digit.cc` & `cytosim-0.0.6/src/sim/hands/digit.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/digit.h` & `cytosim-0.0.6/src/sim/hands/digit.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/digit_prop.cc` & `cytosim-0.0.6/src/sim/hands/digit_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/digit_prop.h` & `cytosim-0.0.6/src/sim/hands/digit_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/dynein.cc` & `cytosim-0.0.6/src/sim/hands/dynein.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/dynein.h` & `cytosim-0.0.6/src/sim/hands/dynein.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/dynein_prop.cc` & `cytosim-0.0.6/src/sim/hands/dynein_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/dynein_prop.h` & `cytosim-0.0.6/src/sim/hands/dynein_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/kinesin.cc` & `cytosim-0.0.6/src/sim/hands/kinesin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/kinesin.h` & `cytosim-0.0.6/src/sim/hands/kinesin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/kinesin_prop.cc` & `cytosim-0.0.6/src/sim/hands/kinesin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/kinesin_prop.h` & `cytosim-0.0.6/src/sim/hands/kinesin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/mighty.cc` & `cytosim-0.0.6/src/sim/hands/mighty.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/mighty.h` & `cytosim-0.0.6/src/sim/hands/mighty.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/mighty_prop.cc` & `cytosim-0.0.6/src/sim/hands/mighty_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/mighty_prop.h` & `cytosim-0.0.6/src/sim/hands/mighty_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/motor.cc` & `cytosim-0.0.6/src/sim/hands/motor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/motor.h` & `cytosim-0.0.6/src/sim/hands/motor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/motor_prop.cc` & `cytosim-0.0.6/src/sim/hands/motor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/motor_prop.h` & `cytosim-0.0.6/src/sim/hands/motor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/myosin.cc` & `cytosim-0.0.6/src/sim/hands/myosin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/myosin.h` & `cytosim-0.0.6/src/sim/hands/myosin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/myosin_prop.cc` & `cytosim-0.0.6/src/sim/hands/myosin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/myosin_prop.h` & `cytosim-0.0.6/src/sim/hands/myosin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/nucleator.cc` & `cytosim-0.0.6/src/sim/hands/nucleator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/nucleator.h` & `cytosim-0.0.6/src/sim/hands/nucleator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/nucleator_prop.cc` & `cytosim-0.0.6/src/sim/hands/nucleator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/nucleator_prop.h` & `cytosim-0.0.6/src/sim/hands/nucleator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/regulator.cc` & `cytosim-0.0.6/src/sim/hands/regulator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/regulator.h` & `cytosim-0.0.6/src/sim/hands/regulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/regulator_prop.cc` & `cytosim-0.0.6/src/sim/hands/regulator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/regulator_prop.h` & `cytosim-0.0.6/src/sim/hands/regulator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/rescuer.cc` & `cytosim-0.0.6/src/sim/hands/rescuer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/rescuer.h` & `cytosim-0.0.6/src/sim/hands/rescuer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/rescuer_prop.cc` & `cytosim-0.0.6/src/sim/hands/rescuer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/rescuer_prop.h` & `cytosim-0.0.6/src/sim/hands/rescuer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/slider.cc` & `cytosim-0.0.6/src/sim/hands/slider.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/slider.h` & `cytosim-0.0.6/src/sim/hands/slider.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/slider_prop.cc` & `cytosim-0.0.6/src/sim/hands/slider_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/slider_prop.h` & `cytosim-0.0.6/src/sim/hands/slider_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/tracker.cc` & `cytosim-0.0.6/src/sim/hands/tracker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/tracker.h` & `cytosim-0.0.6/src/sim/hands/tracker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/tracker_prop.cc` & `cytosim-0.0.6/src/sim/hands/tracker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/tracker_prop.h` & `cytosim-0.0.6/src/sim/hands/tracker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/walker.cc` & `cytosim-0.0.6/src/sim/hands/walker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/walker.h` & `cytosim-0.0.6/src/sim/hands/walker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/walker_prop.cc` & `cytosim-0.0.6/src/sim/hands/walker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/hands/walker_prop.h` & `cytosim-0.0.6/src/sim/hands/walker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/interface.cc` & `cytosim-0.0.6/src/sim/interface.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/interface.h` & `cytosim-0.0.6/src/sim/interface.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/interpolation.cc` & `cytosim-0.0.6/src/sim/interpolation.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/interpolation.h` & `cytosim-0.0.6/src/sim/interpolation.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/interpolation4.cc` & `cytosim-0.0.6/src/sim/interpolation4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/interpolation4.h` & `cytosim-0.0.6/src/sim/interpolation4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/lattice.cc` & `cytosim-0.0.6/src/sim/lattice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/lattice.h` & `cytosim-0.0.6/src/sim/lattice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/makefile.inc` & `cytosim-0.0.6/src/sim/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/meca.cc` & `cytosim-0.0.6/src/sim/meca.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/meca.h` & `cytosim-0.0.6/src/sim/meca.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/meca1d.h` & `cytosim-0.0.6/src/sim/meca1d.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/meca_inter.cc` & `cytosim-0.0.6/src/sim/meca_inter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecable.cc` & `cytosim-0.0.6/src/sim/mecable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecable.h` & `cytosim-0.0.6/src/sim/mecable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecafil.cc` & `cytosim-0.0.6/src/sim/mecafil.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecafil.h` & `cytosim-0.0.6/src/sim/mecafil.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecafil_project.cc` & `cytosim-0.0.6/src/sim/mecafil_project.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecafil_projectmat.cc` & `cytosim-0.0.6/src/sim/mecafil_projectmat.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecapoint.cc` & `cytosim-0.0.6/src/sim/mecapoint.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/mecapoint.h` & `cytosim-0.0.6/src/sim/mecapoint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/modulo.cc` & `cytosim-0.0.6/src/sim/modulo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/modulo.h` & `cytosim-0.0.6/src/sim/modulo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/movable.cc` & `cytosim-0.0.6/src/sim/movable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/movable.h` & `cytosim-0.0.6/src/sim/movable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/object.cc` & `cytosim-0.0.6/src/sim/object.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/object.h` & `cytosim-0.0.6/src/sim/object.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/object_set.cc` & `cytosim-0.0.6/src/sim/object_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/object_set.h` & `cytosim-0.0.6/src/sim/object_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizer.cc` & `cytosim-0.0.6/src/sim/organizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizer.h` & `cytosim-0.0.6/src/sim/organizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizer_set.cc` & `cytosim-0.0.6/src/sim/organizer_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizer_set.h` & `cytosim-0.0.6/src/sim/organizer_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/aster.cc` & `cytosim-0.0.6/src/sim/organizers/aster.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/aster.h` & `cytosim-0.0.6/src/sim/organizers/aster.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/aster_prop.cc` & `cytosim-0.0.6/src/sim/organizers/aster_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/aster_prop.h` & `cytosim-0.0.6/src/sim/organizers/aster_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/bundle.cc` & `cytosim-0.0.6/src/sim/organizers/bundle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/bundle.h` & `cytosim-0.0.6/src/sim/organizers/bundle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/bundle_prop.cc` & `cytosim-0.0.6/src/sim/organizers/bundle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/bundle_prop.h` & `cytosim-0.0.6/src/sim/organizers/bundle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/fake.cc` & `cytosim-0.0.6/src/sim/organizers/fake.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/fake.h` & `cytosim-0.0.6/src/sim/organizers/fake.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/fake_prop.cc` & `cytosim-0.0.6/src/sim/organizers/fake_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/fake_prop.h` & `cytosim-0.0.6/src/sim/organizers/fake_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/nucleus.cc` & `cytosim-0.0.6/src/sim/organizers/nucleus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/nucleus.h` & `cytosim-0.0.6/src/sim/organizers/nucleus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/nucleus_prop.cc` & `cytosim-0.0.6/src/sim/organizers/nucleus_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/organizers/nucleus_prop.h` & `cytosim-0.0.6/src/sim/organizers/nucleus_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/parser.cc` & `cytosim-0.0.6/src/sim/parser.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/parser.h` & `cytosim-0.0.6/src/sim/parser.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/point_grid.cc` & `cytosim-0.0.6/src/sim/point_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/point_grid.h` & `cytosim-0.0.6/src/sim/point_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sim.cc` & `cytosim-0.0.6/src/sim/sim.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sim_thread.cc` & `cytosim-0.0.6/src/sim/sim_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sim_thread.h` & `cytosim-0.0.6/src/sim/sim_thread.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul.cc` & `cytosim-0.0.6/src/sim/simul.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul.h` & `cytosim-0.0.6/src/sim/simul.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul_custom.cc` & `cytosim-0.0.6/src/sim/simul_custom.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul_file.cc` & `cytosim-0.0.6/src/sim/simul_file.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul_prop.cc` & `cytosim-0.0.6/src/sim/simul_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul_prop.h` & `cytosim-0.0.6/src/sim/simul_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul_report.cc` & `cytosim-0.0.6/src/sim/simul_report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul_solve.cc` & `cytosim-0.0.6/src/sim/simul_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/simul_step.cc` & `cytosim-0.0.6/src/sim/simul_step.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/single.cc` & `cytosim-0.0.6/src/sim/single.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/single.h` & `cytosim-0.0.6/src/sim/single.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/single_prop.cc` & `cytosim-0.0.6/src/sim/single_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/single_prop.h` & `cytosim-0.0.6/src/sim/single_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/single_set.cc` & `cytosim-0.0.6/src/sim/single_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/single_set.h` & `cytosim-0.0.6/src/sim/single_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/picket.cc` & `cytosim-0.0.6/src/sim/singles/picket.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/picket.h` & `cytosim-0.0.6/src/sim/singles/picket.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/picket_long.cc` & `cytosim-0.0.6/src/sim/singles/picket_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/picket_long.h` & `cytosim-0.0.6/src/sim/singles/picket_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/wrist.cc` & `cytosim-0.0.6/src/sim/singles/wrist.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/wrist.h` & `cytosim-0.0.6/src/sim/singles/wrist.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/wrist_long.cc` & `cytosim-0.0.6/src/sim/singles/wrist_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/singles/wrist_long.h` & `cytosim-0.0.6/src/sim/singles/wrist_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/solid.cc` & `cytosim-0.0.6/src/sim/solid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/solid.h` & `cytosim-0.0.6/src/sim/solid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/solid_prop.cc` & `cytosim-0.0.6/src/sim/solid_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/solid_prop.h` & `cytosim-0.0.6/src/sim/solid_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/solid_set.cc` & `cytosim-0.0.6/src/sim/solid_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/solid_set.h` & `cytosim-0.0.6/src/sim/solid_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/space.cc` & `cytosim-0.0.6/src/sim/space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/space.h` & `cytosim-0.0.6/src/sim/space.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/space_prop.cc` & `cytosim-0.0.6/src/sim/space_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/space_prop.h` & `cytosim-0.0.6/src/sim/space_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/space_set.cc` & `cytosim-0.0.6/src/sim/space_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/space_set.h` & `cytosim-0.0.6/src/sim/space_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_banana.cc` & `cytosim-0.0.6/src/sim/spaces/space_banana.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_banana.h` & `cytosim-0.0.6/src/sim/spaces/space_banana.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_capsule.cc` & `cytosim-0.0.6/src/sim/spaces/space_capsule.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_capsule.h` & `cytosim-0.0.6/src/sim/spaces/space_capsule.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_cylinder.cc` & `cytosim-0.0.6/src/sim/spaces/space_cylinder.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_cylinder.h` & `cytosim-0.0.6/src/sim/spaces/space_cylinder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_cylinderP.cc` & `cytosim-0.0.6/src/sim/spaces/space_cylinderP.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_cylinderP.h` & `cytosim-0.0.6/src/sim/spaces/space_cylinderP.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_cylinderZ.cc` & `cytosim-0.0.6/src/sim/spaces/space_cylinderZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_cylinderZ.h` & `cytosim-0.0.6/src/sim/spaces/space_cylinderZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_dice.cc` & `cytosim-0.0.6/src/sim/spaces/space_dice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_dice.h` & `cytosim-0.0.6/src/sim/spaces/space_dice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_ellipse.cc` & `cytosim-0.0.6/src/sim/spaces/space_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_ellipse.h` & `cytosim-0.0.6/src/sim/spaces/space_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_periodic.cc` & `cytosim-0.0.6/src/sim/spaces/space_periodic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_periodic.h` & `cytosim-0.0.6/src/sim/spaces/space_periodic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_polygon.cc` & `cytosim-0.0.6/src/sim/spaces/space_polygon.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_polygon.h` & `cytosim-0.0.6/src/sim/spaces/space_polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_polygonZ.cc` & `cytosim-0.0.6/src/sim/spaces/space_polygonZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_polygonZ.h` & `cytosim-0.0.6/src/sim/spaces/space_polygonZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_ring.cc` & `cytosim-0.0.6/src/sim/spaces/space_ring.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_ring.h` & `cytosim-0.0.6/src/sim/spaces/space_ring.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_sphere.cc` & `cytosim-0.0.6/src/sim/spaces/space_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_sphere.h` & `cytosim-0.0.6/src/sim/spaces/space_sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_square.cc` & `cytosim-0.0.6/src/sim/spaces/space_square.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_square.h` & `cytosim-0.0.6/src/sim/spaces/space_square.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_strip.cc` & `cytosim-0.0.6/src/sim/spaces/space_strip.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_strip.h` & `cytosim-0.0.6/src/sim/spaces/space_strip.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_torus.cc` & `cytosim-0.0.6/src/sim/spaces/space_torus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/spaces/space_torus.h` & `cytosim-0.0.6/src/sim/spaces/space_torus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sphere.cc` & `cytosim-0.0.6/src/sim/sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sphere.h` & `cytosim-0.0.6/src/sim/sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sphere_prop.cc` & `cytosim-0.0.6/src/sim/sphere_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sphere_prop.h` & `cytosim-0.0.6/src/sim/sphere_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sphere_set.cc` & `cytosim-0.0.6/src/sim/sphere_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/sphere_set.h` & `cytosim-0.0.6/src/sim/sphere_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/sim/splash.h` & `cytosim-0.0.6/src/sim/splash.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/CMakeLists.txt` & `cytosim-0.0.6/src/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/makefile.inc` & `cytosim-0.0.6/src/test/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test.cc` & `cytosim-0.0.6/src/test/test.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_blas.cc` & `cytosim-0.0.6/src/test/test_blas.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_code.cc` & `cytosim-0.0.6/src/test/test_code.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_cxx.cc` & `cytosim-0.0.6/src/test/test_cxx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_gillespie.cc` & `cytosim-0.0.6/src/test/test_gillespie.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_glapp.cc` & `cytosim-0.0.6/src/test/test_glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_glos.cc` & `cytosim-0.0.6/src/test/test_glos.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_glut.cc` & `cytosim-0.0.6/src/test/test_glut.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_glut3D.cc` & `cytosim-0.0.6/src/test/test_glut3D.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_grid.cc` & `cytosim-0.0.6/src/test/test_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_math.cc` & `cytosim-0.0.6/src/test/test_math.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_matrix.cc` & `cytosim-0.0.6/src/test/test_matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_omp.cc` & `cytosim-0.0.6/src/test/test_omp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_opengl.cc` & `cytosim-0.0.6/src/test/test_opengl.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_pipe.cc` & `cytosim-0.0.6/src/test/test_pipe.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_platonic.cc` & `cytosim-0.0.6/src/test/test_platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_quaternion.cc` & `cytosim-0.0.6/src/test/test_quaternion.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_random.cc` & `cytosim-0.0.6/src/test/test_random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_rasterizer.cc` & `cytosim-0.0.6/src/test/test_rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_signal.cc` & `cytosim-0.0.6/src/test/test_signal.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_simd.cc` & `cytosim-0.0.6/src/test/test_simd.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_sizeof.cc` & `cytosim-0.0.6/src/test/test_sizeof.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_solve.cc` & `cytosim-0.0.6/src/test/test_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_space.cc` & `cytosim-0.0.6/src/test/test_space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_sphere.cc` & `cytosim-0.0.6/src/test/test_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_thread.cc` & `cytosim-0.0.6/src/test/test_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/test/test_vbo.cc` & `cytosim-0.0.6/src/test/test_vbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/CMakeLists.txt` & `cytosim-0.0.6/src/tools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/cymart.cc` & `cytosim-0.0.6/src/tools/cymart.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/frametool.cc` & `cytosim-0.0.6/src/tools/frametool.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/makefile.inc` & `cytosim-0.0.6/src/tools/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/pycytoplay.cc` & `cytosim-0.0.6/src/tools/pycytoplay.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/pycytosim.cc` & `cytosim-0.0.6/src/tools/pycytosim.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/pycytosim.h` & `cytosim-0.0.6/src/tools/pycytosim.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/reader.cc` & `cytosim-0.0.6/src/tools/reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/report.cc` & `cytosim-0.0.6/src/tools/report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/reportF.cc` & `cytosim-0.0.6/src/tools/reportF.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.5/src/tools/sieve.cc` & `cytosim-0.0.6/src/tools/sieve.cc`

 * *Files identical despite different names*

