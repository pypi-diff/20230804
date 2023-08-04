# Comparing `tmp/desyrdl-0.3.0.tar.gz` & `tmp/desyrdl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desyrdl-0.3.0.tar", last modified: Thu Dec 15 16:42:35 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `desyrdl-0.3.0.tar` & `desyrdl-1.2.0.tar`

### file list

```diff
@@ -1,50 +1,46 @@
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)    11358 2022-05-23 17:49:07.000000 desyrdl-0.3.0/LICENSE
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)       48 2022-05-20 15:05:13.000000 desyrdl-0.3.0/MANIFEST.in
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     6067 2022-12-15 16:42:35.254655 desyrdl-0.3.0/PKG-INFO
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     5123 2022-05-23 17:49:07.000000 desyrdl-0.3.0/README.md
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)    34951 2022-12-15 16:00:06.000000 desyrdl-0.3.0/desyrdl/DesyListener.py
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     4475 2022-11-24 10:05:37.000000 desyrdl-0.3.0/desyrdl/RdlFormatter.py
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)        0 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/__init__.py
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)       73 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/__main__.py
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     9346 2022-12-15 16:00:06.000000 desyrdl-0.3.0/desyrdl/desyrdl.py
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.250655 desyrdl-0.3.0/desyrdl/libraries/
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/libraries/rdl/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1417 2022-05-23 17:49:07.000000 desyrdl-0.3.0/desyrdl/libraries/rdl/00_desyrdl_properties.rdl
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1343 2022-05-23 17:49:07.000000 desyrdl-0.3.0/desyrdl/libraries/rdl/10_generic_ibus.rdl
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/libraries/vhdl/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1664 2022-05-23 17:49:07.000000 desyrdl-0.3.0/desyrdl/libraries/vhdl/axi4l_to_axi4l.vhd
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     7663 2022-12-08 20:33:31.000000 desyrdl-0.3.0/desyrdl/libraries/vhdl/axi4l_to_ibus.vhd
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)    23395 2022-12-08 20:33:31.000000 desyrdl-0.3.0/desyrdl/libraries/vhdl/decoder_axi4l.vhd
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      124 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/libraries/vhdl/include.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)    10796 2022-09-23 13:42:23.000000 desyrdl-0.3.0/desyrdl/libraries/vhdl/pkg_desyrdl_common.vhd
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     3056 2022-10-27 15:54:51.000000 desyrdl-0.3.0/desyrdl/libraries/vhdl/reg_field_counter.vhd
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     5908 2022-10-26 10:40:42.000000 desyrdl-0.3.0/desyrdl/libraries/vhdl/reg_field_storage.vhd
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1296 2022-05-23 17:49:07.000000 desyrdl-0.3.0/desyrdl/rdlformatcode.py
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/templates/
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/templates/adoc/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      146 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/templates/adoc/include.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1132 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/templates/adoc/registers.adoc.in
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/templates/h/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     2595 2022-12-08 20:33:31.000000 desyrdl-0.3.0/desyrdl/templates/h/header.h.in
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      145 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/templates/h/include.txt
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/templates/map/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      208 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/templates/map/include.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      775 2022-12-15 16:00:06.000000 desyrdl-0.3.0/desyrdl/templates/map/mapfile.mapp.in
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1480 2022-12-08 20:33:31.000000 desyrdl-0.3.0/desyrdl/templates/map/mapfile.mapp.in.orig
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      788 2022-11-21 19:20:13.000000 desyrdl-0.3.0/desyrdl/templates/map/mapfile.mapt.in
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl/templates/vhdl/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      164 2022-05-20 15:05:13.000000 desyrdl-0.3.0/desyrdl/templates/vhdl/include.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)    15176 2022-11-24 10:04:07.000000 desyrdl-0.3.0/desyrdl/templates/vhdl/pkg.vhd.in
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)    20783 2022-11-24 10:04:07.000000 desyrdl-0.3.0/desyrdl/templates/vhdl/top.vhd.in
-drwxrwxr-x   0 mbuechl   (5000) mbuechl   (5000)        0 2022-12-15 16:42:35.254655 desyrdl-0.3.0/desyrdl.egg-info/
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     6067 2022-12-15 16:42:35.000000 desyrdl-0.3.0/desyrdl.egg-info/PKG-INFO
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1164 2022-12-15 16:42:35.000000 desyrdl-0.3.0/desyrdl.egg-info/SOURCES.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)        1 2022-12-15 16:42:35.000000 desyrdl-0.3.0/desyrdl.egg-info/dependency_links.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)       49 2022-12-15 16:42:35.000000 desyrdl-0.3.0/desyrdl.egg-info/entry_points.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)       25 2022-12-15 16:42:35.000000 desyrdl-0.3.0/desyrdl.egg-info/requires.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)        8 2022-12-15 16:42:35.000000 desyrdl-0.3.0/desyrdl.egg-info/top_level.txt
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      104 2022-05-20 15:05:13.000000 desyrdl-0.3.0/pyproject.toml
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)     1117 2022-12-15 16:42:35.258655 desyrdl-0.3.0/setup.cfg
--rw-rw-r--   0 mbuechl   (5000) mbuechl   (5000)      148 2022-05-23 17:49:07.000000 desyrdl-0.3.0/setup.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 desyrdl-1.2.0/Jenkinsfile
+-rw-r--r--   0        0        0    27147 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/DesyListener.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/__main__.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/desyrdl.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/rdlformatcode.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/libraries/rdl/00_desyrdl_properties.rdl
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/libraries/rdl/10_generic_ibus.rdl
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/libraries/vhdl/axi4l_to_ibus.vhd
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/libraries/vhdl/ibus_to_axi4l.vhd
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/libraries/vhdl/include.txt
+-rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/libraries/vhdl/pkg_desyrdl_common.vhd
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/adoc/addrmap.adoc.jinja2
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/adoc/include.txt
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/h/header.h.jinja2
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/h/include.txt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/map/include.txt
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/map/mapfile.mapp.jinja2
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/map/mapfile.mapt.jinja2
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/tcl/fwk_desyrdl_multi_lib.tcl.jinja2
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/tcl/fwk_desyrdl_one_lib.tcl.jinja2
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/tcl/include.txt
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/tcl/vivado_desyrdl_multi_lib.tcl.jinja2
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/tcl/vivado_desyrdl_one_lib.tcl.jinja2
+-rw-r--r--   0        0        0    29830 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/vhdl/decoder_axi4l.vhd.in
+-rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/vhdl/decoder_ibus.vhd.in
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/vhdl/include.txt
+-rw-r--r--   0        0        0    18559 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/vhdl/pkg.vhd.in
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 desyrdl-1.2.0/desyrdl/templates/vhdl/top.vhd.in
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 desyrdl-1.2.0/doc/TODO.org
+-rw-r--r--   0        0        0    24104 2020-02-02 00:00:00.000000 desyrdl-1.2.0/doc/images/DesyRDL.svg
+-rw-r--r--   0        0        0    19302 2020-02-02 00:00:00.000000 desyrdl-1.2.0/doc/images/top_integration.svg
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 desyrdl-1.2.0/examples/spi_ad9510.rdl
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 desyrdl-1.2.0/examples/standalone.rdl
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 desyrdl-1.2.0/examples/test_desyrdl.rdl
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 desyrdl-1.2.0/examples/test_desyrdl.vh
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 desyrdl-1.2.0/examples/top.rdl
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 desyrdl-1.2.0/test/run.sh
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 desyrdl-1.2.0/test/rdl/module_a.rdl
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 desyrdl-1.2.0/test/rdl/module_b.rdl
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 desyrdl-1.2.0/test/rdl/top.rdl
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 desyrdl-1.2.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 desyrdl-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 desyrdl-1.2.0/README.md
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 desyrdl-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 desyrdl-1.2.0/PKG-INFO
```

### Comparing `desyrdl-0.3.0/LICENSE` & `desyrdl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `desyrdl-0.3.0/PKG-INFO` & `desyrdl-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,50 @@
-Metadata-Version: 2.1
-Name: desyrdl
-Version: 0.3.0
-Summary: DesyRDL: Tool for address space and register generation
-Author: Michael Büchler, Lukasz Butkowski
-Author-email: michael.buechler@desy.de, lukasz.butkowski@desy.de
-License: Apache-2.0
-Project-URL: Source, https://gitlab.desy.de/fpgafw/tools/desyrdl
-Platform: any
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## DesyRDL
+# DesyRDL
 
 This tool generates outputs for an address space that is defined by one or many
 SystemRDL&trade; 2.0 input files. The address space could be made up of all the
 software-accessible registers and memory regions in an FPGA design, or just the
 registers of a single IP block.
 
 SystemRDL&trade; 2.0 is a standard released by Accellera Systems Initiative Inc
 that is meant to describe such an address space, see [\[systemrdl\]](#systemrdl).
 
-Outputs are based on templates. Writing your own should be easy. Provided with
-this package are templates and common files for the following outputs:
+Outputs are based on templates. there is an option to use custom templates or the one provided by the tool.
+The templates provided with this package are the common files for the following outputs:
 
 * Synthesizable VHDL register logic
-* Mapfiles (format used internally at DESY MSK)
+* Mapfiles (compatible with ChimeraTK)
 * C header files
 * AsciiDoc documentation
 
 DesyRDL was developed at [DESY](https://desy.de) in the MSK firmware group as a
 replacement for its existing proprietary method of register and address map
 generation, the "Internal Interface", called "IBUS" in its latest version
 [ii](#ii).
 
-The idea to use the SystemRDL&trade; 2.0 standard came from
-[MicroTCA Tech Lab](https://techlab.desy.de/) at DESY when they wrote
-[HECTARE](https://github.com/MicroTCA-Tech-Lab/hectare), the predecessor of
-DesyRDL.
+The use of SystemRDL&trade; 2.0 standard was considered for a long time,
+but due to the lack of open source compilers or parsers, it was dropped.
+
+The decision to use the SystemRDL&trade; 2.0 standard came after
+the open source [SystemRDL compiler](https://github.com/SystemRDL/systemrdl-compiler) has been published.
+This has been proposed by [MicroTCA Tech Lab](https://techlab.desy.de/) at DESY when they wrote
+[HECTARE](https://github.com/MicroTCA-Tech-Lab/hectare), the predecessor of DesyRDL.
 
 ## Usage
 
 This tool can be used standalone but was intended to be used as part of a
 firmware build environment like DESY MSK's
 [FPGA Firmware Framework](https://fpgafw.pages.desy.de/docs-pub/fwk/index.html),
 short `fwk`.
 
 See `desyrdl -h` for options.
 All RDL files must be passed in the correct order. Below is an example for the
 `test_hectare` module which also comes with a testbench (not in Git yet):
 
-    desyrdl -o out -i examples/spi_ad9510.rdl examples/test_hectare.rdl -f vhdl
+    desyrdl -o out -i examples/spi_ad9510.rdl examples/test_desyrdl.rdl examples/top.rdl -f vhdl tcl
 
 This will compile the `.rdl` file and create one `.vhd` in `./out/` for each
 `addrmap` instance in the model and for each VHDL template in
 `./desyrdl/templates/vhdl/`. The common files from `./desyrdl/libraries/vhdl/`
 will also be copied there.
 
 The generated VHDL logic should be integrated into your module or IP as an
@@ -80,49 +60,55 @@
 
 Compiling the SystemRDL&trade; files is handled by
 [SystemRDL Compiler](https://systemrdl-compiler.readthedocs.io/en/latest/).
 To create useful information (or "context") for the template processing, its
 Walker/Listener method of traversing the compiled tree is used.
 
 `DesyListener` extends its `systemrdl.RDLListener` class. It extracts a fixed
-set of information from the compiled tree and passes it on to a custom template
-engine (`RdlFormatter`).
+set of information from the compiled tree and passes it on to a template engine
+(Jinja2).
 
 ![DesyRDL flow diagram](./doc/images/DesyRDL.svg "DesyRDL flow overview")
 
 ### Templates
 
-The custom template engine is inspired by
-https://github.com/ebrehault/superformatter. Everything within curly braces {}
-is interpreted as a "replacement field" and replaced by the output of the
-formatter. This is inherited from Python's `Formatter` class, so its behavior
-is very similar to a formatted print in Python. In addition to that it can also
-perform advanced actions, e.g. loop over all registers within an addrmap. For
-all this it relies on "context" which holds all the necessary information about
-the address space.
+Templates are written for the Jinja2 template engine. Users can provide their
+own templates using `-t` switch.
 
 ### Context
 
 Context creation differs a bit depending on the type of output. Some outputs
 have to be generated for each `addrmap` component (e.g. VHDL) and others are
 generated for the whole address space at once (e.g. mapfiles and the C header).
 
 The context is a Python `dict` that contains further dictionaries to describe
 register types and instances, memory types and instances, further external
 components and some more. It is currently a bit of a mess.
 
+## Supported interfaces buses
+
+The DesyRDL allows to generate various top address map interfaces.
+They are defined in the addrmap component by the `desyrdl_interface` variable.
+
+Tool bus support and `desyrdl_interfaces` values:
+
+| Value    | Description                                       | Bus Size | Supported |
+|:---------|:--------------------------------------------------|:---------|:----------|
+| AXI4L    | AXI4 Lite interface                               | 32 bit   | YES       |
+| IBUS     | Internal Interface type bus, proprietary MSK DESY | 32 bit   | YES       |
+| WISHBONE | Open source hardware computer bus                 | 32 bit   | planned   |
+
+
 ## Known Issues and Limitations
 
 The bus decoder implementation is relatively basic:
 
-* Only AXI4-Lite with 32 bit data width is supported as the upstream interface
+* Only 32bit data busses
 * Likewise, only 32 bit registers are supported
 * The dual-port memory interface does not support AXI4 write strobes
-* Timing issues can arise when having a large number of registers per addrmap.
-  A review is needed here.
 * The logic operates on a single clock and the developer has to take care of any
   CDCs
 
 ## Acknowledgements
 
 This tool relies heavily on systemrdl-compiler by Alex Mykyta and was only
 developed because it exists.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `desyrdl-0.3.0/desyrdl/libraries/rdl/00_desyrdl_properties.rdl` & `desyrdl-1.2.0/desyrdl/libraries/rdl/00_desyrdl_properties.rdl`

 * *Files identical despite different names*

### Comparing `desyrdl-0.3.0/desyrdl/libraries/vhdl/axi4l_to_ibus.vhd` & `desyrdl-1.2.0/desyrdl/libraries/vhdl/axi4l_to_ibus.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -74,22 +74,20 @@
   signal wd_cnt   : natural := 0;
   ---------------------------------------------------------------------------
 begin
 
   -- unsed AXI4 Signals: SIG_M2S.AWSIZE  SIG_M2S.AWBURST  SIG_M2S.WSTRB
   -- unsed AXI4 Signals: SIG_M2S.ARSIZE  SIG_M2S.ARBURST  SIG_M2S.WLAST
 
-  po_s_decoder   <= sig_s2m;
-  sig_m2s          <= pi_s_decoder;
+  po_s_decoder    <= sig_s2m;
+  sig_m2s         <= pi_s_decoder;
   ------------------------------------
-  sig_s2m.rresp    <=  "00";
+  sig_s2m.rresp   <=  "00";
 
-  sig_s2m.bresp    <=  "00";
-
-  po_m_ext.clk    <=  pi_clock;
+  sig_s2m.bresp   <=  "00";
 
   po_m_ext.addr   <=  sig_addr;
   po_m_ext.rena   <=  sig_rena when rising_edge(pi_clock); -- delay one clock cycle to have 1 clock cycle delay after data on bus
   po_m_ext.wena   <=  sig_wena when rising_edge(pi_clock);
 
   prs_main_fsm: process(pi_clock)
   begin
```

### Comparing `desyrdl-0.3.0/desyrdl/libraries/vhdl/pkg_desyrdl_common.vhd` & `desyrdl-1.2.0/desyrdl/libraries/vhdl/pkg_desyrdl_common.vhd`

 * *Files 14% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     arready     : std_logic;
     -- read data channel signals---------------------------------------------
     rdata       : std_logic_vector(C_AXI4L_DATA_WIDTH-1 downto 0);
     rresp       : std_logic_vector(1 downto 0);
     rvalid      : std_logic;
   end record t_axi4l_s2m;
 
-  type t_axi4l_m2s_array is array (integer range <>) of t_axi4l_m2s;
-  type t_axi4l_s2m_array is array (integer range <>) of t_axi4l_s2m;
+  type t_axi4l_m2s_vector is array (integer range <>) of t_axi4l_m2s;
+  type t_axi4l_s2m_vector is array (integer range <>) of t_axi4l_s2m;
 
   constant  C_AXI4L_S2M_DEFAULT : t_axi4l_s2m := (
     awready     => '0',
     wready      => '0',
     bresp       => (others => '0'),
     bvalid      => '0',
     arready     => '0' ,
@@ -107,42 +107,38 @@
 
   -- Output signals of IBUS. Through this record the application send data/commands to the bus
   type t_ibus_m2s is record
     addr   : std_logic_vector(31 downto 0);
     data   : std_logic_vector(31 downto 0);
     rena   : std_logic;
     wena   : std_logic;
-    clk    : std_logic;
   end record t_ibus_m2s;
 
   -- Output signals of IBUS. Through this record the application send data/commands to the bus
   type t_ibus_s2m is record
-    clk    : std_logic;
     data   : std_logic_vector(31 downto 0);
     rack   : std_logic;
     wack   : std_logic;
   end record t_ibus_s2m;
 
   -- Array of IBUS outputs
-  type t_ibus_m2s_array is array (integer range<>) of t_ibus_m2s;
+  type t_ibus_m2s_vector is array (integer range<>) of t_ibus_m2s;
 
   -- Array of IBUS inputs
-  type t_ibus_s2m_array is array (integer range<>) of t_ibus_s2m;
+  type t_ibus_s2m_vector is array (integer range<>) of t_ibus_s2m;
 
   -- Default IBUS connections for the output (All entries equals 0)
   constant C_IBUS_M2S_DEFAULT : t_ibus_m2s := (
     addr => (others => '0'),
     data => (others => '0'),
     rena => '0',
-    wena => '0',
-    clk  => '0'
+    wena => '0'
   );
   -- Default IBUS connections for the input (All entries equals 0)
   constant C_IBUS_S2M_DEFAULT : t_ibus_s2m := (
-    clk  => '0',
     data => (others => '0'),
     rack => '0',
     wack => '0'
   );
 
 
   ---------------------------------------------------------------------------
@@ -167,112 +163,63 @@
     hw        : t_access_type;
     we        : integer;
     incrwidth : integer;
     decrwidth : integer;
     defval    : integer;
   end record;
 
-  type t_field_info_array is array (integer range <>) of t_field_info;
+  type t_field_info_vector is array (integer range <>) of t_field_info;
 
   constant C_FIELD_NONE : t_field_info := (WIRE, 0, 0, 0, C_NA, C_NA, 0, 0, 0, 0);
 
   type t_reg_info is record
     -- index    : integer;
     address  : unsigned(C_AXI4L_ADDR_WIDTH-1 downto 0);
     elements : integer;
     index    : integer;
-    fields   : t_field_info_array(31 downto 0);
+    fields   : t_field_info_vector(31 downto 0);
     --dim         : natural;
     dim_n    : positive;
     dim_m    : positive;
   end record;
 
-  type t_reg_info_array is array (integer range <>) of t_reg_info;
+  type t_reg_info_vector is array (integer range <>) of t_reg_info;
 
   constant C_REG_NONE : t_reg_info := (x"0000_0000", 0, 0,(others => C_FIELD_NONE),1,1);
 
   type t_mem_info is record
     -- index      : integer;
     address    : unsigned(C_AXI4L_ADDR_WIDTH-1 downto 0);
     addrwidth  : integer;
     datawidth  : integer;
     entries    : integer;
     sw         : t_access_type;
   end record;
 
-  type t_mem_info_array is array (integer range <>) of t_mem_info;
+  type t_mem_info_vector is array (integer range <>) of t_mem_info;
 
   constant C_MEM_NONE : t_mem_info := (x"0000_0000", 0, 0, 0, C_NA);
 
   type t_ext_info is record
     -- index      : integer;
     address    : unsigned(C_AXI4L_ADDR_WIDTH-1 downto 0);
     addrwidth  : integer;
     size       : integer;
   end record;
 
-  type t_ext_info_array is array (integer range <>) of t_ext_info;
+  type t_ext_info_vector is array (integer range <>) of t_ext_info;
 
   constant C_EXT_NONE : t_ext_info := (x"0000_0000", 0, 0);
 
   -- interface types
   type t_if_type Is (DPM, AXI4, AXI4L, IBUS, WISHBONE, AVALON, NONE);
-  type t_if_type_array is array (integer range <>) of t_if_type;
-
-
-  -- components
-  component decoder_axi4l is
-    generic (
-      g_addr_width    : integer;
-      g_data_width    : integer;
-      g_register_info : t_reg_info_array;
-      g_regitems      : integer;
-      g_regcount      : integer;
-      g_mem_info      : t_mem_info_array;
-      g_memitems      : integer;
-      g_memcount      : integer;
-      g_ext_info      : t_ext_info_array;
-      g_extitems      : integer;
-      g_extcount      : integer);
-    port (
-      pi_clock      : in  std_logic;
-      pi_reset      : in  std_logic;
-      po_reg_rd_stb : out std_logic_vector(g_regcount-1 downto 0);
-      po_reg_wr_stb : out std_logic_vector(g_regcount-1 downto 0);
-      po_reg_data   : out std_logic_vector(g_data_width-1 downto 0);
-      pi_reg_data   : in  std_logic_vector(g_data_width-1 downto 0);
-      po_mem_stb    : out std_logic_vector(g_memcount-1 downto 0);
-      po_mem_we     : out std_logic;
-      po_mem_addr   : out std_logic_vector(g_addr_width-1 downto 0);
-      po_mem_data   : out std_logic_vector(g_data_width-1 downto 0);
-      pi_mem_data   : in  std_logic_vector(g_data_width-1 downto 0);
-      pi_mem_ack    : in  std_logic;
-      pi_ext      : in  t_axi4l_s2m_array(G_EXTCOUNT-1 downto 0);
-      po_ext      : out t_axi4l_m2s_array(G_EXTCOUNT-1 downto 0);
-      pi_s_top    : in  t_axi4l_m2s;
-      po_s_top    : out t_axi4l_s2m);
-  end component decoder_axi4l;
-
-  component reg_field_storage is
-    generic (
-      g_info : t_field_info);
-    port (
-      pi_clock     : in  std_logic;
-      pi_reset     : in  std_logic;
-      pi_sw_rd_stb : in  std_logic;
-      pi_sw_wr_stb : in  std_logic;
-      pi_sw_data   : in  std_logic_vector(g_info.len-1 downto 0);
-      po_sw_data   : out std_logic_vector(g_info.len-1 downto 0);
-      pi_hw_we     : in  std_logic;
-      pi_hw_data   : in  std_logic_vector(g_info.len-1 downto 0);
-      po_hw_data   : out std_logic_vector(g_info.len-1 downto 0);
-      po_hw_swmod  : out std_logic;
-      po_hw_swacc  : out std_logic);
-  end component reg_field_storage;
+  type t_if_type_vector is array (integer range <>) of t_if_type;
 
+  -----------------------------------------------------------------------------
+  -- bus converter components
   component axi4l_to_axi4l is
     port (
       pi_reset       : in  std_logic;
       pi_clock       : in  std_logic;
       pi_s_decoder : in  t_axi4l_m2s;
       po_s_decoder : out t_axi4l_s2m;
       po_m_ext     : out t_axi4l_m2s;
@@ -284,11 +231,23 @@
       pi_reset       : in  std_logic;
       pi_clock       : in  std_logic;
       pi_s_decoder : in  t_axi4l_m2s;
       po_s_decoder : out t_axi4l_s2m;
       po_m_ext     : out t_ibus_m2s;
       pi_m_ext     : in  t_ibus_s2m);
   end component axi4l_to_ibus;
+
+  component ibus_to_axi4l is
+    port (
+      pi_reset       : in  std_logic;
+      pi_clock       : in  std_logic;
+      pi_s_decoder : in  t_ibus_m2s;
+      po_s_decoder : out t_ibus_s2m;
+      po_m_ext     : out t_axi4l_m2s;
+      pi_m_ext     : in  t_axi4l_s2m);
+  end component ibus_to_axi4l;
+
 end package common;
 
+--==============================================================================
 package body common is
 end package body;
```

### Comparing `desyrdl-0.3.0/desyrdl/rdlformatcode.py` & `desyrdl-1.2.0/desyrdl/rdlformatcode.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 # --------------------------------------------------------------------------- #
 # @copyright Copyright 2022 DESY
 # SPDX-License-Identifier: Apache-2.0
 # --------------------------------------------------------------------------- #
 # @date 2022-01-14
 # @author Lukasz Butkowski <lukasz.butkowski@desy.de>
 # --------------------------------------------------------------------------- #
-"""DesyRdl markup class.
 
-class to overload default Markdown parsing to disable it
-"""
+from markdown import Markdown
 
 
-from markdown import Markdown
+class DesyrdlMarkup(Markdown):
+    """DesyRdl markup class.
 
+    class to overload default Markdown parsing to disable it
+    """
 
-class desyrdlmarkup(Markdown):
-    def __init__(self, **kwargs):
+    def __init__(self):
         self.reset()
 
     def reset(self):
         return self
 
     def convert(self, source):
         self.text = source
```

### Comparing `desyrdl-0.3.0/desyrdl.egg-info/PKG-INFO` & `desyrdl-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 Metadata-Version: 2.1
 Name: desyrdl
-Version: 0.3.0
-Summary: DesyRDL: Tool for address space and register generation
-Author: Michael Büchler, Lukasz Butkowski
-Author-email: michael.buechler@desy.de, lukasz.butkowski@desy.de
-License: Apache-2.0
+Version: 1.2.0
+Summary: DesyRDL - Tool for address space and register generation
+Project-URL: Homepage, https://gitlab.desy.de/fpgafw/tools/desyrdl
+Project-URL: Issues, https://gitlab.desy.de/fpgafw/tools/desyrdl/-/issues
 Project-URL: Source, https://gitlab.desy.de/fpgafw/tools/desyrdl
-Platform: any
+Author-email: MSK DESY <msk-firmware@desy.de>, Michael Büchler <michael.buechler@desy.de>, Lukasz Butkowski <lukasz.butkowski@desy.de>
+Maintainer-email: Michael Büchler <michael.buechler@desy.de>, Lukasz Butkowski <lukasz.butkowski@desy.de>
+License: Apache-2.0
+License-File: LICENSE
+Keywords: EDA,FPGA,SystemRDL
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Requires-Python: >=3.8
+Requires-Dist: jinja2>=3.0
+Requires-Dist: systemrdl-compiler>=1.25
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
-## DesyRDL
+# DesyRDL
 
 This tool generates outputs for an address space that is defined by one or many
 SystemRDL&trade; 2.0 input files. The address space could be made up of all the
 software-accessible registers and memory regions in an FPGA design, or just the
 registers of a single IP block.
 
 SystemRDL&trade; 2.0 is a standard released by Accellera Systems Initiative Inc
 that is meant to describe such an address space, see [\[systemrdl\]](#systemrdl).
 
-Outputs are based on templates. Writing your own should be easy. Provided with
-this package are templates and common files for the following outputs:
+Outputs are based on templates. there is an option to use custom templates or the one provided by the tool.
+The templates provided with this package are the common files for the following outputs:
 
 * Synthesizable VHDL register logic
-* Mapfiles (format used internally at DESY MSK)
+* Mapfiles (compatible with ChimeraTK)
 * C header files
 * AsciiDoc documentation
 
 DesyRDL was developed at [DESY](https://desy.de) in the MSK firmware group as a
 replacement for its existing proprietary method of register and address map
 generation, the "Internal Interface", called "IBUS" in its latest version
 [ii](#ii).
 
-The idea to use the SystemRDL&trade; 2.0 standard came from
-[MicroTCA Tech Lab](https://techlab.desy.de/) at DESY when they wrote
-[HECTARE](https://github.com/MicroTCA-Tech-Lab/hectare), the predecessor of
-DesyRDL.
+The use of SystemRDL&trade; 2.0 standard was considered for a long time,
+but due to the lack of open source compilers or parsers, it was dropped.
+
+The decision to use the SystemRDL&trade; 2.0 standard came after
+the open source [SystemRDL compiler](https://github.com/SystemRDL/systemrdl-compiler) has been published.
+This has been proposed by [MicroTCA Tech Lab](https://techlab.desy.de/) at DESY when they wrote
+[HECTARE](https://github.com/MicroTCA-Tech-Lab/hectare), the predecessor of DesyRDL.
 
 ## Usage
 
 This tool can be used standalone but was intended to be used as part of a
 firmware build environment like DESY MSK's
 [FPGA Firmware Framework](https://fpgafw.pages.desy.de/docs-pub/fwk/index.html),
 short `fwk`.
 
 See `desyrdl -h` for options.
 All RDL files must be passed in the correct order. Below is an example for the
 `test_hectare` module which also comes with a testbench (not in Git yet):
 
-    desyrdl -o out -i examples/spi_ad9510.rdl examples/test_hectare.rdl -f vhdl
+    desyrdl -o out -i examples/spi_ad9510.rdl examples/test_desyrdl.rdl examples/top.rdl -f vhdl tcl
 
 This will compile the `.rdl` file and create one `.vhd` in `./out/` for each
 `addrmap` instance in the model and for each VHDL template in
 `./desyrdl/templates/vhdl/`. The common files from `./desyrdl/libraries/vhdl/`
 will also be copied there.
 
 The generated VHDL logic should be integrated into your module or IP as an
@@ -80,49 +86,55 @@
 
 Compiling the SystemRDL&trade; files is handled by
 [SystemRDL Compiler](https://systemrdl-compiler.readthedocs.io/en/latest/).
 To create useful information (or "context") for the template processing, its
 Walker/Listener method of traversing the compiled tree is used.
 
 `DesyListener` extends its `systemrdl.RDLListener` class. It extracts a fixed
-set of information from the compiled tree and passes it on to a custom template
-engine (`RdlFormatter`).
+set of information from the compiled tree and passes it on to a template engine
+(Jinja2).
 
 ![DesyRDL flow diagram](./doc/images/DesyRDL.svg "DesyRDL flow overview")
 
 ### Templates
 
-The custom template engine is inspired by
-https://github.com/ebrehault/superformatter. Everything within curly braces {}
-is interpreted as a "replacement field" and replaced by the output of the
-formatter. This is inherited from Python's `Formatter` class, so its behavior
-is very similar to a formatted print in Python. In addition to that it can also
-perform advanced actions, e.g. loop over all registers within an addrmap. For
-all this it relies on "context" which holds all the necessary information about
-the address space.
+Templates are written for the Jinja2 template engine. Users can provide their
+own templates using `-t` switch.
 
 ### Context
 
 Context creation differs a bit depending on the type of output. Some outputs
 have to be generated for each `addrmap` component (e.g. VHDL) and others are
 generated for the whole address space at once (e.g. mapfiles and the C header).
 
 The context is a Python `dict` that contains further dictionaries to describe
 register types and instances, memory types and instances, further external
 components and some more. It is currently a bit of a mess.
 
+## Supported interfaces buses
+
+The DesyRDL allows to generate various top address map interfaces.
+They are defined in the addrmap component by the `desyrdl_interface` variable.
+
+Tool bus support and `desyrdl_interfaces` values:
+
+| Value    | Description                                       | Bus Size | Supported |
+|:---------|:--------------------------------------------------|:---------|:----------|
+| AXI4L    | AXI4 Lite interface                               | 32 bit   | YES       |
+| IBUS     | Internal Interface type bus, proprietary MSK DESY | 32 bit   | YES       |
+| WISHBONE | Open source hardware computer bus                 | 32 bit   | planned   |
+
+
 ## Known Issues and Limitations
 
 The bus decoder implementation is relatively basic:
 
-* Only AXI4-Lite with 32 bit data width is supported as the upstream interface
+* Only 32bit data busses
 * Likewise, only 32 bit registers are supported
 * The dual-port memory interface does not support AXI4 write strobes
-* Timing issues can arise when having a large number of registers per addrmap.
-  A review is needed here.
 * The logic operates on a single clock and the developer has to take care of any
   CDCs
 
 ## Acknowledgements
 
 This tool relies heavily on systemrdl-compiler by Alex Mykyta and was only
 developed because it exists.
```

