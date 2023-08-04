# Comparing `tmp/kintree-1.0.1.tar.gz` & `tmp/kintree-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kintree-1.0.1.tar", max compression
+gzip compressed data, was "kintree-1.0.2.tar", max compression
```

## Comparing `kintree-1.0.1.tar` & `kintree-1.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    35149 2023-04-24 18:36:38.509469 kintree-1.0.1/LICENSE
--rw-r--r--   0        0        0    14880 2023-04-24 18:36:38.509469 kintree-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-04-24 18:36:38.593470 kintree-1.0.1/kintree/__init__.py
--rw-r--r--   0        0        0     5304 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/common/part_tools.py
--rw-r--r--   0        0        0     1214 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/common/progress.py
--rw-r--r--   0        0        0     4852 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/common/tools.py
--rw-r--r--   0        0        0    16047 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/config_interface.py
--rw-r--r--   0        0        0       47 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/digikey/digikey_api.yaml
--rw-r--r--   0        0        0     2745 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/digikey/digikey_categories.yaml
--rw-r--r--   0        0        0      248 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/digikey/digikey_config.yaml
--rw-r--r--   0        0        0       99 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/element14/element14_api.yaml
--rw-r--r--   0        0        0      244 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/element14/element14_config.yaml
--rw-r--r--   0        0        0     1633 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/categories.yaml
--rw-r--r--   0        0        0      104 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/inventree_dev.yaml
--rw-r--r--   0        0        0      104 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/inventree_prod.yaml
--rw-r--r--   0        0        0     1019 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/parameters.yaml
--rw-r--r--   0        0        0      553 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/parameters_filters.yaml
--rw-r--r--   0        0        0     5710 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/supplier_parameters.yaml
--rw-r--r--   0        0        0      235 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/suppliers.yaml
--rw-r--r--   0        0        0       95 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/kicad/kicad.yaml
--rw-r--r--   0        0        0     1161 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/kicad/kicad_map.yaml
--rw-r--r--   0        0        0       68 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/lcsc/lcsc_api.yaml
--rw-r--r--   0        0        0      256 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/lcsc/lcsc_config.yaml
--rw-r--r--   0        0        0       25 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/mouser/mouser_api.yaml
--rw-r--r--   0        0        0      258 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/mouser/mouser_config.yaml
--rw-r--r--   0        0        0    11301 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/settings.py
--rw-r--r--   0        0        0      199 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/user/general.yaml
--rw-r--r--   0        0        0      183 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/user/internal_part_number.yaml
--rw-r--r--   0        0        0       73 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/user/search_api.yaml
--rw-r--r--   0        0        0    20852 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/database/inventree_api.py
--rw-r--r--   0        0        0    33965 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/database/inventree_interface.py
--rw-r--r--   0        0        0     3360 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/gui.py
--rw-r--r--   0        0        0    38788 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/logo.png
--rw-r--r--   0        0        0    14401 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/views/common.py
--rw-r--r--   0        0        0    50728 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/views/main.py
--rw-r--r--   0        0        0    32917 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/views/settings.py
--rw-r--r--   0        0        0      416 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/kicad_interface.py
--rw-r--r--   0        0        0     4598 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/kicad_symbol.py
--rw-r--r--   0        0        0     7048 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/LICENSE
--rw-r--r--   0        0        0     3077 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/capacitor-polarized.kicad_sym
--rw-r--r--   0        0        0     2786 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/capacitor.kicad_sym
--rw-r--r--   0        0        0     1089 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/connector.kicad_sym
--rw-r--r--   0        0        0     2540 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/crystal-2p.kicad_sym
--rw-r--r--   0        0        0     1091 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/default.kicad_sym
--rw-r--r--   0        0        0     2647 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-led.kicad_sym
--rw-r--r--   0        0        0     2453 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-schottky.kicad_sym
--rw-r--r--   0        0        0     2251 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-standard.kicad_sym
--rw-r--r--   0        0        0     2445 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-zener.kicad_sym
--rw-r--r--   0        0        0     2116 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/eeprom-sot23.kicad_sym
--rw-r--r--   0        0        0     2445 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/ferrite-bead.kicad_sym
--rw-r--r--   0        0        0     2249 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/fuse.kicad_sym
--rw-r--r--   0        0        0     2258 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/inductor.kicad_sym
--rw-r--r--   0        0        0     1089 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/integrated-circuit.kicad_sym
--rw-r--r--   0        0        0       65 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/library_template.kicad_sym
--rw-r--r--   0        0        0     2140 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/oscillator-4p.kicad_sym
--rw-r--r--   0        0        0     2451 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/protection-unidir.kicad_sym
--rw-r--r--   0        0        0     2233 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/resistor-sm.kicad_sym
--rw-r--r--   0        0        0     2233 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/resistor.kicad_sym
--rw-r--r--   0        0        0     4683 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-nfet.kicad_sym
--rw-r--r--   0        0        0     2795 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-npn.kicad_sym
--rw-r--r--   0        0        0     4986 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-pfet.kicad_sym
--rw-r--r--   0        0        0     2800 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-pnp.kicad_sym
--rw-r--r--   0        0        0     1981 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pcb
--rw-r--r--   0        0        0     1201 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_prl
--rw-r--r--   0        0        0     6077 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pro
--rw-r--r--   0        0        0      187 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_sch
--rw-r--r--   0        0        0      227 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kintree_gui.py
--rw-r--r--   0        0        0     6440 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/search/digikey_api.py
--rw-r--r--   0        0        0     9730 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/search/element14_api.py
--rw-r--r--   0        0        0     3611 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/search/lcsc_api.py
--rw-r--r--   0        0        0     3833 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/search/mouser_api.py
--rw-r--r--   0        0        0     1243 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/search/search_api.py
--rw-r--r--   0        0        0     4013 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/search/snapeda_api.py
--rw-r--r--   0        0        0     2028 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/setup_inventree.py
--rw-r--r--   0        0        0     1003 2023-04-24 18:36:38.593470 kintree-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    16129 1970-01-01 00:00:00.000000 kintree-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 14:17:10.384194 kintree-1.0.2/LICENSE
+-rw-r--r--   0        0        0    15680 2023-08-04 14:17:10.384194 kintree-1.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-08-04 14:17:10.492196 kintree-1.0.2/kintree/__init__.py
+-rw-r--r--   0        0        0     5357 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/common/part_tools.py
+-rw-r--r--   0        0        0     1214 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/common/progress.py
+-rw-r--r--   0        0        0     5353 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/common/tools.py
+-rw-r--r--   0        0        0    16461 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/config_interface.py
+-rw-r--r--   0        0        0       47 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/digikey/digikey_api.yaml
+-rw-r--r--   0        0        0     2745 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/digikey/digikey_categories.yaml
+-rw-r--r--   0        0        0      248 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/digikey/digikey_config.yaml
+-rw-r--r--   0        0        0       99 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/element14/element14_api.yaml
+-rw-r--r--   0        0        0      244 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/element14/element14_config.yaml
+-rw-r--r--   0        0        0     1633 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/inventree/categories.yaml
+-rw-r--r--   0        0        0      128 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/inventree/inventree_dev.yaml
+-rw-r--r--   0        0        0      128 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/inventree/inventree_prod.yaml
+-rw-r--r--   0        0        0     1016 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/inventree/parameters.yaml
+-rw-r--r--   0        0        0      553 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/inventree/parameters_filters.yaml
+-rw-r--r--   0        0        0     5710 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/inventree/supplier_parameters.yaml
+-rw-r--r--   0        0        0      235 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/inventree/suppliers.yaml
+-rw-r--r--   0        0        0       95 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/kicad/kicad.yaml
+-rw-r--r--   0        0        0     1161 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/kicad/kicad_map.yaml
+-rw-r--r--   0        0        0       68 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/lcsc/lcsc_api.yaml
+-rw-r--r--   0        0        0      256 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/lcsc/lcsc_config.yaml
+-rw-r--r--   0        0        0       25 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/mouser/mouser_api.yaml
+-rw-r--r--   0        0        0      258 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/mouser/mouser_config.yaml
+-rw-r--r--   0        0        0    11953 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/settings.py
+-rw-r--r--   0        0        0      234 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/user/general.yaml
+-rw-r--r--   0        0        0      183 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/user/internal_part_number.yaml
+-rw-r--r--   0        0        0       73 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/config/user/search_api.yaml
+-rw-r--r--   0        0        0    24592 2023-08-04 14:17:10.392194 kintree-1.0.2/kintree/database/inventree_api.py
+-rw-r--r--   0        0        0    36296 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/database/inventree_interface.py
+-rw-r--r--   0        0        0     3360 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/gui/gui.py
+-rw-r--r--   0        0        0    38788 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/gui/logo.png
+-rw-r--r--   0        0        0    14413 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/gui/views/common.py
+-rw-r--r--   0        0        0    51919 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/gui/views/main.py
+-rw-r--r--   0        0        0    33380 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/gui/views/settings.py
+-rw-r--r--   0        0        0      416 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/kicad_interface.py
+-rw-r--r--   0        0        0     4598 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/kicad_symbol.py
+-rw-r--r--   0        0        0     7048 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/LICENSE
+-rw-r--r--   0        0        0     3077 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/capacitor-polarized.kicad_sym
+-rw-r--r--   0        0        0     2786 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/capacitor.kicad_sym
+-rw-r--r--   0        0        0     1089 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/connector.kicad_sym
+-rw-r--r--   0        0        0     2540 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/crystal-2p.kicad_sym
+-rw-r--r--   0        0        0     1091 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/default.kicad_sym
+-rw-r--r--   0        0        0     2647 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/diode-led.kicad_sym
+-rw-r--r--   0        0        0     2453 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/diode-schottky.kicad_sym
+-rw-r--r--   0        0        0     2251 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/diode-standard.kicad_sym
+-rw-r--r--   0        0        0     2445 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/diode-zener.kicad_sym
+-rw-r--r--   0        0        0     2116 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/eeprom-sot23.kicad_sym
+-rw-r--r--   0        0        0     2445 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/ferrite-bead.kicad_sym
+-rw-r--r--   0        0        0     2249 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/fuse.kicad_sym
+-rw-r--r--   0        0        0     2258 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/inductor.kicad_sym
+-rw-r--r--   0        0        0     1089 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/integrated-circuit.kicad_sym
+-rw-r--r--   0        0        0       65 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/library_template.kicad_sym
+-rw-r--r--   0        0        0     2140 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/oscillator-4p.kicad_sym
+-rw-r--r--   0        0        0     2451 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/protection-unidir.kicad_sym
+-rw-r--r--   0        0        0     2233 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/resistor-sm.kicad_sym
+-rw-r--r--   0        0        0     2233 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/resistor.kicad_sym
+-rw-r--r--   0        0        0     4683 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/transistor-nfet.kicad_sym
+-rw-r--r--   0        0        0     2795 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/transistor-npn.kicad_sym
+-rw-r--r--   0        0        0     4986 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/transistor-pfet.kicad_sym
+-rw-r--r--   0        0        0     2800 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates/transistor-pnp.kicad_sym
+-rw-r--r--   0        0        0     1981 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates_project/templates_project.kicad_pcb
+-rw-r--r--   0        0        0     1201 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates_project/templates_project.kicad_prl
+-rw-r--r--   0        0        0     6077 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates_project/templates_project.kicad_pro
+-rw-r--r--   0        0        0      187 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kicad/templates_project/templates_project.kicad_sch
+-rw-r--r--   0        0        0      227 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/kintree_gui.py
+-rw-r--r--   0        0        0     6789 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/search/digikey_api.py
+-rw-r--r--   0        0        0    10053 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/search/element14_api.py
+-rw-r--r--   0        0        0     3954 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/search/lcsc_api.py
+-rw-r--r--   0        0        0     4166 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/search/mouser_api.py
+-rw-r--r--   0        0        0     1243 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/search/search_api.py
+-rw-r--r--   0        0        0     4064 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/search/snapeda_api.py
+-rw-r--r--   0        0        0     2028 2023-08-04 14:17:10.396195 kintree-1.0.2/kintree/setup_inventree.py
+-rw-r--r--   0        0        0     1003 2023-08-04 14:17:10.492196 kintree-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    16929 1970-01-01 00:00:00.000000 kintree-1.0.2/PKG-INFO
```

### Comparing `kintree-1.0.1/LICENSE` & `kintree-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/README.md` & `kintree-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,49 @@
+Metadata-Version: 2.1
+Name: kintree
+Version: 1.0.2
+Summary: Fast part creation in KiCad and InvenTree
+Home-page: https://github.com/sparkmicro/Ki-nTree
+License: GPL-3.0-or-later
+Keywords: inventree,kicad,digikey,mouser,component,part,create
+Author: eeintech
+Author-email: eeintech@eeinte.ch
+Maintainer: eeintech
+Maintainer-email: eeintech@eeinte.ch
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: digikey-api (>=1.0.0,<2.0.0)
+Requires-Dist: flet (==0.5.2)
+Requires-Dist: inventree (>=0.10.1,<0.11.0)
+Requires-Dist: kiutils (>=1.4.0,<2.0.0)
+Requires-Dist: mouser (>=0.1.3,<0.2.0)
+Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
+Requires-Dist: validators (>=0.19.0,<0.20.0)
+Requires-Dist: wrapt_timeout_decorator (>=1.3.12,<2.0.0)
+Project-URL: Repository, https://github.com/sparkmicro/Ki-nTree
+Description-Content-Type: text/markdown
+
 # <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/logo.png" width="auto" height="32"> Ki-nTree
 ### Fast part creation for [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
 [![License: GPL v3.0](https://img.shields.io/badge/license-GPL_v3.0-green.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python Versions](https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/python_versions.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/kintree)](https://pypi.org/project/kintree/)
 [![Tests | Linting | Publishing](https://github.com/sparkmicro/Ki-nTree/actions/workflows/test_deploy.yaml/badge.svg)](https://github.com/sparkmicro/Ki-nTree/actions)
 [![Coverage Status](https://coveralls.io/repos/github/sparkmicro/Ki-nTree/badge.svg?branch=main&service=github)](https://coveralls.io/github/sparkmicro/Ki-nTree?branch=main)
 
+## :warning: InvenTree Compatibility
+Ki-nTree currently only supports InvenTree `0.11` or older versions. InvenTree `0.12` introduced a new parameter template system which is not supported as of now, see https://github.com/sparkmicro/Ki-nTree/issues/165 for more details. The future versions of InvenTree (`0.13` and up) should be compatible with Ki-nTree again soon, and this page will be updated with the required InvenTree setup.
+
 ## :fast_forward: [Demo Video](https://youtu.be/YeWBqOCb4pw)
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_example.png" width="auto" height="auto">
 
 ## Introduction
 Ki-nTree (pronounced "Key Entry" or "Key 'n' Tree") aims to:
 * automate part creation of KiCad library parts
@@ -150,22 +184,24 @@
 1. With Ki-nTree GUI open, click on "Settings > Supplier > Digi-Key" and fill in both Digi-Key API Client ID and Secret keys (optional: click on "Test" to [get an API token](#get-digi-key-api-token))
 2. Click on "Settings > Supplier > Mouser" and fill in the Mouser part search API key
 3. Click on "Settings > Supplier > Element14" and fill in the Element14 product search API key (key is shared with Farnell and Newark)
 4. Click on "Settings > KiCad", browse to the location where KiCad symbol, template and footprint libraries are stored on your computer then click "Save"
 5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to check communication with server)  
   a. It is possible to define a Proxy Server over which all interactions with InvenTree will be routed. To set a proxy server use the "Enable Proxy Support" switch in "Settings > InvenTree" and define the proxy address in the new input field.  
   b. Instead of user credential authentication token authentication is also supported. To use a token add it it to the "Password or Token" field and leave the "Username" empty. You can retrieve your personal access token from your InvenTree server by sending an get-request to its api url `api/user/token/`.
+  c. If needed this tool can try to download the parts datasheet from the suppliers and upload it it to the attachment section of each part. For this just activate "Upload Datasheets to InvenTree" in the InvenTree settings
+  d. It is also possible to sync the prices in InvenTree with the latest supplier prices. For this enable "Upload Pricing Data to InvenTree"
 
 
 #### Get Digi-Key API token
 <details>
 <summary>Show steps (click to expand)</summary>
 <p>
 
-Enter your Digi-Key developper account credentials then login. The following page will appear (`user@email.com` will show your email address):
+Enter your Digi-Key developer account credentials then login. The following page will appear (`user@email.com` will show your email address):
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/digikey_api_approval_request.png" width="600" height="auto">
 
 Click on "Allow", another page will open.  
 Click on the "Advanced" button, then click on "Proceed to localhost (unsafe)" at the bottom of the page:
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/digikey_api_approval_request2.png"  width="600" height="auto">
@@ -184,15 +220,15 @@
 CATEGORY_NAME:
   INVENTREE_PARAMETER_NAME:
     - SUPPLIER_1_PARAMETER_NAME_1
     - SUPPLIER_1_PARAMETER_NAME_2
     - SUPPLIER_2_PARAMETER_NAME_1
 ```
 
-Refer to [this file](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/search/supplier_parameters.yaml) as a starting point / example.
+Refer to [this file](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/inventree/supplier_parameters.yaml) as a starting point / example.
 
 #### Part Number Search
 
 Ki-nTree currently supports APIs for the following electronics suppliers: Digi-Key, Mouser, Element14 and LCSC.
 
 1. In the main window, enter the part number and select the supplier in drop-down list, then click "CREATE". It will start by fetching part data using the supplier's API
 2. In the case Digi-Key has been selected and the API token is not found or expired, a browser window will pop-up. To get a new token: [follow those steps](#get-digi-key-api-token)
@@ -263,8 +299,8 @@
    that your python dist path is a part of your `$PATH`.
 
 ## License
 The Ki-nTree source code is licensed under the [GPL3.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/LICENSE) as it uses source code under that license:
 * https://github.com/mvnmgrx/kiutils
 * https://github.com/peeter123/digikey-api
 
-The [KiCad templates](https://github.com/sparkmicro/Ki-nTree/tree/main/kintree/kicad/templates) are licensed under the [Creative Commons CC0 1.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/kicad/templates/LICENSE) which means that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission" ([reference](https://creativecommons.org/publicdomain/zero/1.0/)).
+The [KiCad templates](https://github.com/sparkmicro/Ki-nTree/tree/main/kintree/kicad/templates) are licensed under the [Creative Commons CC0 1.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/kicad/templates/LICENSE) which means that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission" ([reference](https://creativecommons.org/publicdomain/zero/1.0/)).
```

### Comparing `kintree-1.0.1/kintree/common/part_tools.py` & `kintree-1.0.2/kintree/common/part_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,23 +129,24 @@
 
                 value = resistance + unit
 
     # General filters
     # Clean-up ranges
     separator = '~'
     if separator in value:
-        split_space = value.split()
-        first_value = split_space[0]
-        second_value = split_space[2]
+        space_split = value.split()
+        first_value = space_split[0]
+        if len(space_split) > 2:
+            second_value = space_split[2]
 
-        # Substract digits, negative sign, points from first value to get unit
-        unit = first_value.replace(re.findall('[-.0-9]*', first_value)[0], '')
+            # Substract digits, negative sign, points from first value to get unit
+            unit = first_value.replace(re.findall('[-.0-9]*', first_value)[0], '')
 
-        if unit:
-            value = first_value.replace(unit, '') + separator + second_value
+            if unit:
+                value = first_value.replace(unit, '') + separator + second_value
 
     # Remove parenthesis section
     if '(' in value:
         parenthesis = re.findall('\(.*\)', value)
 
         if parenthesis:
             for item in parenthesis:
```

### Comparing `kintree-1.0.1/kintree/common/progress.py` & `kintree-1.0.2/kintree/common/progress.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/common/tools.py` & `kintree-1.0.2/kintree/common/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,68 +61,73 @@
 
 
 def download(url, filetype='API data', fileoutput='', timeout=3, enable_headers=False, requests_lib=False, silent=False):
     ''' Standard method to download URL content, with option to save to local file (eg. images) '''
 
     import socket
     import urllib.request
+    import requests
 
     # Set default timeout for download socket
     socket.setdefaulttimeout(timeout)
     if enable_headers:
         opener = urllib.request.build_opener()
         opener.addheaders = [('User-agent', 'Mozilla/5.0')]
         urllib.request.install_opener(opener)
     try:
-        if filetype == 'Image':
-            # Enable use of requests library for downloading images (Element14 URLs do NOT work with urllib)
+        if filetype == 'Image' or filetype == 'PDF':
+            # Enable use of requests library for downloading files (some URLs do NOT work with urllib)
             if requests_lib:
-                import requests
                 headers = {'User-agent': 'Mozilla/5.0'}
-                response = requests.get(url, headers=headers, timeout=timeout)
-                with open(fileoutput, 'wb') as image:
-                    image.write(response.content)
+                response = requests.get(url, headers=headers, timeout=timeout, allow_redirects=True)
+                if filetype.lower() not in response.headers['Content-Type'].lower():
+                    cprint(f'[INFO]\tWarning: {filetype} download returned the wrong file type', silent=silent)
+                    return None
+                with open(fileoutput, 'wb') as file:
+                    file.write(response.content)
             else:
-                (image, headers) = urllib.request.urlretrieve(url, filename=fileoutput)
-            return image
-        elif filetype == 'PDF':
-            (pdf, headers) = urllib.request.urlretrieve(url, filename=fileoutput)
-            return pdf
+                (file, headers) = urllib.request.urlretrieve(url, filename=fileoutput)
+                if filetype.lower() not in headers['Content-Type'].lower():
+                    cprint(f'[INFO]\tWarning: {filetype} download returned the wrong file type', silent=silent)
+                    return None
+            return file
         else:
             url_data = urllib.request.urlopen(url)
             data = url_data.read()
             data_json = json.loads(data.decode('utf-8'))
             return data_json
-    except socket.timeout:
+    except (socket.timeout, requests.exceptions.ConnectTimeout, requests.exceptions.ReadTimeout):
         cprint(f'[INFO]\tWarning: {filetype} download socket timed out ({timeout}s)', silent=silent)
-    except urllib.error.HTTPError:
+    except (urllib.error.HTTPError, requests.exceptions.ConnectionError):
         cprint(f'[INFO]\tWarning: {filetype} download failed (HTTP Error)', silent=silent)
     except (urllib.error.URLError, ValueError):
         cprint(f'[INFO]\tWarning: {filetype} download failed (URL Error)', silent=silent)
+    except requests.exceptions.SSLError:
+        cprint(f'[INFO]\tWarning: {filetype} download failed (SSL Error)', silent=silent)
     except FileNotFoundError:
         cprint(f'[INFO]\tWarning: {os.path.dirname(fileoutput)} folder does not exist', silent=silent)
     return None
 
 
-def download_image(image_url: str, image_full_path: str, silent=False) -> str:
+def download_with_retry(url: str, full_path: str, silent=False, **kwargs) -> str:
     ''' Standard method to download image URL to local file '''
 
-    if not image_url:
+    if not url:
         cprint('[INFO]\tError: Missing image URL', silent=silent)
         return False
-    
+
     # Try without headers
-    image = download(image_url, filetype='Image', fileoutput=image_full_path, silent=silent)
+    file = download(url, fileoutput=full_path, silent=silent, **kwargs)
 
-    if not image:
+    if not file:
         # Try with headers
-        image = download(image_url, filetype='Image', fileoutput=image_full_path, enable_headers=True, silent=silent)
+        file = download(url, fileoutput=full_path, enable_headers=True, silent=silent, **kwargs)
 
-    if not image:
+    if not file:
         # Try with requests library
-        image = download(image_url, filetype='Image', fileoutput=image_full_path, enable_headers=True, requests_lib=True, silent=silent)
+        file = download(url, fileoutput=full_path, enable_headers=True, requests_lib=True, silent=silent, **kwargs)
 
     # Still nothing
-    if not image:
+    if not file:
         return False
 
     return True
```

### Comparing `kintree-1.0.1/kintree/config/config_interface.py` & `kintree-1.0.2/kintree/config/config_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,34 +103,42 @@
     proxies = user_settings.get('PROXIES', None)
     if not proxies:
         user_settings['PROXY'] = ''
     else:
         # loading the proxy independent if it is http or https
         user_settings['PROXY'] = list(proxies.values())[0]
 
+    if 'DATASHEET_UPLOAD' not in user_settings:
+        user_settings['DATASHEET_UPLOAD'] = False
+    if 'PRICING_UPLOAD' not in user_settings:
+        user_settings['PRICING_UPLOAD'] = False
     return user_settings
 
 
 def save_inventree_user_settings(enable: bool,
                                  server: str,
                                  username: str,
                                  password: str,
                                  enable_proxy: bool,
                                  proxies: dict,
+                                 datasheet_upload: bool,
+                                 pricing_upload: bool,
                                  user_config_path: str):
     ''' Save InvenTree user settings to file '''
     user_settings = {}
 
     user_settings['ENABLE'] = enable
     user_settings['SERVER_ADDRESS'] = server
     user_settings['USERNAME'] = username
     # Use base64 encoding to make password unreadable inside the file
     user_settings['PASSWORD'] = base64.b64encode(password.encode())
     user_settings['ENABLE_PROXY'] = enable_proxy
     user_settings['PROXIES'] = proxies
+    user_settings['DATASHEET_UPLOAD'] = datasheet_upload
+    user_settings['PRICING_UPLOAD'] = pricing_upload
 
     return dump_file(user_settings, user_config_path)
 
 
 def load_library_path(user_config_path: str, silent=False):
     ''' Load KiCad library from KiCad settings file '''
     user_settings = load_file(user_config_path)
```

### Comparing `kintree-1.0.1/kintree/config/digikey/digikey_categories.yaml` & `kintree-1.0.2/kintree/config/digikey/digikey_categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/config/inventree/categories.yaml` & `kintree-1.0.2/kintree/config/inventree/categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/config/inventree/parameters.yaml` & `kintree-1.0.2/kintree/config/inventree/parameters.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Min Output Voltage: V
 Antenna Type: null
 B Constant: K
 Breakdown Voltage: V
 Capacitance: nF
 Clamping Voltage: V
 Collector Gate Voltage: V
-DC Resistance: mOhm
-ESR: mOhm
+DC Resistance: mΩ
+ESR: mΩ
 Footprint: null
 Forward Voltage: V
 Frequency: Hz
 Frequency Stability: ppm
 Frequency Tolerance: ppm
 Function Type: null
 Interface Type: null
@@ -35,15 +35,15 @@
 Output Type: null
 Package Height: mm
 Package Size: mm
 Package Type: null
 Pitch: mm
 Polarity: null
 Quiescent Current: A
-RDS On Resistance: Ohm
+RDS On Resistance: Ω
 RDS On Voltage: V
 Rated Current: A
 Rated Power: W
 Rated Voltage: V
 Saturation Current: A
 Shielding: null
 Standoff Voltage: V
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kintree-1.0.1/kintree/config/inventree/parameters_filters.yaml` & `kintree-1.0.2/kintree/config/inventree/parameters_filters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/config/inventree/supplier_parameters.yaml` & `kintree-1.0.2/kintree/config/inventree/supplier_parameters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/config/kicad/kicad_map.yaml` & `kintree-1.0.2/kintree/config/kicad/kicad_map.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/config/settings.py` & `kintree-1.0.2/kintree/config/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,31 +99,33 @@
 load_ipn_settings()
 
 # GENERAL SETTINGS
 CONFIG_GENERAL_PATH = os.path.join(CONFIG_USER_FILES, 'general.yaml')
 CONFIG_GENERAL = config_interface.load_file(CONFIG_GENERAL_PATH)
 # Datasheets
 DATASHEET_SAVE_ENABLED = CONFIG_GENERAL.get('DATASHEET_SAVE_ENABLED', False)
-DATASHEET_SAVE_PATH = CONFIG_GENERAL.get('DATASHEET_SAVE_PATH', False)
+DATASHEET_SAVE_PATH = CONFIG_GENERAL.get('DATASHEET_SAVE_PATH', '')
 # Open Browser
 AUTOMATIC_BROWSER_OPEN = CONFIG_GENERAL.get('AUTOMATIC_BROWSER_OPEN', False)
 # Default Supplier
 DEFAULT_SUPPLIER = CONFIG_GENERAL.get('DEFAULT_SUPPLIER', 'Digi-Key')
 
 
 # Load enable flags
 def reload_enable_flags():
     global ENABLE_KICAD
     global ENABLE_INVENTREE
     global ENABLE_ALTERNATE
+    global UPDATE_INVENTREE
 
     try:
         ENABLE_KICAD = CONFIG_GENERAL.get('ENABLE_KICAD', False)
         ENABLE_INVENTREE = CONFIG_GENERAL.get('ENABLE_INVENTREE', False)
         ENABLE_ALTERNATE = CONFIG_GENERAL.get('ENABLE_ALTERNATE', False)
+        UPDATE_INVENTREE = CONFIG_GENERAL.get('UPDATE_INVENTREE', False)
         return True
     except TypeError:
         pass
 
     return False
 
 
@@ -181,17 +183,18 @@
 CACHE_VALID_DAYS = int(CONFIG_SEARCH_API.get('CACHE_VALID_DAYS', '7'))
 
 
 # Caching settings
 def load_cache_settings():
     global search_results
     global search_images
+    global search_datasheets
     global CACHE_ENABLED
     global DIGIKEY_STORAGE_PATH
-    
+
     USER_SETTINGS = config_interface.load_user_paths(home_dir=HOME_DIR)
 
     search_results = {
         'directory': os.path.join(USER_SETTINGS['USER_CACHE'], 'search', ''),
         'extension': '.yaml',
     }
     # Create folder if it does not exists
@@ -200,14 +203,21 @@
 
     # Part images
     search_images = os.path.join(USER_SETTINGS['USER_CACHE'], 'images', '')
     # Create folder if it does not exists
     if not os.path.exists(search_images):
         os.makedirs(search_images)
 
+    # Part images
+    search_datasheets = os.path.join(
+        USER_SETTINGS['USER_CACHE'], 'datasheets', '')
+    # Create folder if it does not exists
+    if not os.path.exists(search_datasheets):
+        os.makedirs(search_datasheets)
+
     # API token storage path
     DIGIKEY_STORAGE_PATH = os.path.join(USER_SETTINGS['USER_CACHE'], '')
 
 
 # Load cache settings
 load_cache_settings()
 
@@ -306,22 +316,26 @@
 def load_inventree_settings():
     global SERVER_ADDRESS
     global USERNAME
     global PASSWORD
     global ENABLE_PROXY
     global PROXIES
     global PART_URL_ROOT
+    global DATASHEET_UPLOAD
+    global PRICING_UPLOAD
 
     inventree_settings = config_interface.load_inventree_user_settings(INVENTREE_CONFIG)
 
     SERVER_ADDRESS = inventree_settings.get('SERVER_ADDRESS', None)
     USERNAME = inventree_settings.get('USERNAME', None)
     PASSWORD = inventree_settings.get('PASSWORD', None)
     ENABLE_PROXY = inventree_settings.get('ENABLE_PROXY', False)
     PROXIES = inventree_settings.get('PROXIES', None)
+    DATASHEET_UPLOAD = inventree_settings.get('DATASHEET_UPLOAD', False)
+    PRICING_UPLOAD = inventree_settings.get('PRICING_UPLOAD', False)
     # Part URL
     if SERVER_ADDRESS:
         # If missing, append slash to root URL
         root_url = SERVER_ADDRESS
         if not SERVER_ADDRESS.endswith('/'):
             root_url = root_url + '/'
         # Set part URL
@@ -348,21 +362,23 @@
 
 
 # Enable flags
 def set_enable_flag(key: str, value: bool):
     global CONFIG_GENERAL
 
     user_settings = CONFIG_GENERAL
-    if key in ['kicad', 'inventree', 'alternate']:
+    if key in ['kicad', 'inventree', 'alternate', 'update']:
         if key == 'kicad':
             user_settings['ENABLE_KICAD'] = value
         elif key == 'inventree':
             user_settings['ENABLE_INVENTREE'] = value
         elif key == 'alternate':
             user_settings['ENABLE_ALTERNATE'] = value
+        elif key == 'update':
+            user_settings['UPDATE_INVENTREE'] = value
 
         # Save
         config_interface.dump_file(
             data=user_settings,
             file_path=os.path.join(CONFIG_USER_FILES, 'general.yaml'),
         )
```

### Comparing `kintree-1.0.1/kintree/database/inventree_api.py` & `kintree-1.0.2/kintree/database/inventree_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from ..config import settings
 import validators
 from ..common import part_tools
-from ..common.tools import cprint, download_image
+from ..common.tools import cprint, download_with_retry
 from ..config import config_interface
+import re
 
 # Required to use local CA certificates on Linux
 # For more details, refer to https://github.com/sparkmicro/Ki-nTree/pull/45
 import platform
+import os
 if platform.system() == 'Linux':
-    import os
     cert_path = '/etc/ssl/certs/ca-certificates.crt'
     if os.path.isfile(cert_path):
         os.environ['REQUESTS_CA_BUNDLE'] = cert_path
 
 # InvenTree
 from inventree.api import InvenTreeAPI
-from inventree.company import Company, ManufacturerPart, SupplierPart
+from inventree.company import Company, ManufacturerPart, SupplierPart, SupplierPriceBreak
 from inventree.part import Part, PartCategory, Parameter, ParameterTemplate
 
 
 def connect(server: str,
             username: str,
             password: str,
             connect_timeout=5,
@@ -109,18 +110,30 @@
         elif parent:
             parent_list = []
             while parent:
                 parent_list.insert(0, parent.name)
                 parent = parent.getParentCategory()
             cat = {category.name: None}
             deep_add(categories, parent_list, cat)
-            
+
     return categories
 
 
+def get_category_tree(category_id: int) -> dict:
+    ''' Get all parents of a category'''
+    category = PartCategory(inventree_api, category_id)
+    category_list = {category_id: category.name}
+
+    while category.parent:
+        category = category.getParentCategory()
+        category_list[category.pk] = category.name
+
+    return category_list
+
+
 def get_category_parameters(category_id: int) -> list:
     ''' Get all default parameter templates for category '''
     global inventree_api
 
     parameter_templates = []
 
     category = PartCategory(inventree_api, category_id)
@@ -164,22 +177,22 @@
         return False
 
 
 def get_part_from_ipn(part_ipn='') -> int:
     ''' Get Part ID from Part IPN '''
     global inventree_api
 
-    parts = Part.list(inventree_api)
+    parts = Part.list(inventree_api, IPN=part_ipn)
 
-    for part in parts:
-        if part.IPN == part_ipn:
-            return part
-    
-    # No part found
-    return None
+    if not parts:
+        # No part found
+        return None
+    else:
+        # parts should have only one entry
+        return parts[0]
 
 
 def fetch_part(part_id='', part_ipn='') -> int:
     ''' Fetch part from database using either ID or IPN '''
     from requests.exceptions import HTTPError
     global inventree_api
 
@@ -335,26 +348,60 @@
     global inventree_api
 
     # Get image full path
     image_name = f'{str(part_id)}_thumbnail.jpeg'
     image_location = settings.search_images + image_name
 
     # Download image (multiple attempts)
-    if not download_image(image_url, image_location):
+    if not download_with_retry(image_url, image_location, filetype='Image'):
         return False
 
     # Upload image to InvenTree
     part = Part(inventree_api, part_id)
     if part:
-        return part.uploadImage(image=image_location)
+        try:
+            return part.uploadImage(image=image_location)
+        except Exception:
+            return False
     else:
         return False
 
 
-def create_part(category_id: int, name: str, description: str, revision: str, image: str, keywords=None) -> int:
+def upload_part_datasheet(datasheet_url: str, part_id: int) -> str:
+    ''' Upload InvenTree part attachment'''
+    global inventree_api
+
+    # Get attachment full path
+    datasheet_name = f'{os.path.basename(datasheet_url)}'
+    # inventree needs .pdf at the end of filename to recognize a PDF
+    if not datasheet_name.lower().endswith('.pdf'):
+        datasheet_name += '.pdf'
+    datasheet_location = settings.search_datasheets + datasheet_name
+
+    # Download image (multiple attempts)
+    if not download_with_retry(datasheet_url,
+                               datasheet_location,
+                               filetype='PDF',
+                               timeout=10):
+        return ''
+
+    # Upload Datasheet to InvenTree
+    part = Part(inventree_api, part_id)
+    if part:
+        try:
+            attachment = part.uploadAttachment(attachment=datasheet_location)
+            os.remove(datasheet_location)
+            return inventree_api.base_url.strip('/') + attachment['attachment']
+        except Exception:
+            return ''
+    else:
+        return ''
+
+
+def create_part(category_id: int, name: str, description: str, revision: str, keywords=None) -> int:
     ''' Create InvenTree part '''
     global inventree_api
 
     part = Part.create(inventree_api, {
         'name': name,
         'description': description,
         'category': category_id,
@@ -451,15 +498,15 @@
                 cprint(f'[TREE]\t{item.MPN} ?= {manufacturer_mpn} => False', silent=settings.HIDE_DEBUG)
         except TypeError:
             cprint(f'[TREE]\t{item.MPN} ?= {manufacturer_mpn} => *** SKIPPED ***', silent=settings.HIDE_DEBUG)
 
     return 0
 
 
-def is_new_supplier_part(supplier_name: str, supplier_sku: str) -> bool:
+def is_new_supplier_part(supplier_name: str, supplier_sku: str):
     ''' Check if InvenTree supplier part exists to avoid duplicates '''
     global inventree_api
 
     # Fetch all companies
     cprint('[TREE]\tFetching suppliers', silent=settings.HIDE_DEBUG)
     company_list = Company.list(inventree_api, is_supplier=True, is_customer=False)
     companies = {}
@@ -481,19 +528,19 @@
         )
         # Get all parts
         part_list = []
 
     for item in part_list:
         if supplier_sku in item.SKU:
             cprint(f'[TREE]\t{item.SKU} ?= {supplier_sku} => True', silent=settings.HIDE_DEBUG)
-            return False
+            return False, item
         else:
             cprint(f'[TREE]\t{item.SKU} ?= {supplier_sku} => False', silent=settings.HIDE_DEBUG)
 
-    return True
+    return True, False
 
 
 def create_manufacturer_part(part_id: int, manufacturer_name: str, manufacturer_mpn: str, description: str, datasheet: str) -> bool:
     ''' Create InvenTree manufacturer part
 
         part_id: Part the manufacturer data is linked to
         manufacturer: Company that manufactures the SupplierPart (leave blank if it is the sample as the Supplier!)
@@ -524,15 +571,15 @@
     else:
         cprint(f'[TREE]\tError: Manufacturer "{manufacturer_name}" not found (failed to create manufacturer part)',
                silent=settings.SILENT)
 
     return False
 
 
-def create_supplier_part(part_id: int, manufacturer_name: str, manufacturer_mpn: str, supplier_name: str, supplier_sku: str, description: str, link: str) -> bool:
+def create_supplier_part(part_id: int, manufacturer_name: str, manufacturer_mpn: str, supplier_name: str, supplier_sku: str, description: str, link: str):
     ''' Create InvenTree supplier part
 
         part_id: Part the supplier data is linked to
         manufacturer_name: Manufacturer the supplier data is linked to
         manufacturer_mpn: MPN the supplier data is linked to
         supplier: Company that supplies this SupplierPart object
         SKU: Stock keeping unit (supplier part number)
@@ -563,20 +610,65 @@
             'supplier': supplier_id,
             'SKU': supplier_sku,
             'link': link,
             'description': description,
         })
 
         if supplier_part:
-            return True
+            return True, supplier_part
     else:
         cprint(f'[TREE]\tError: Supplier "{supplier_name}" not found (failed to create supplier part)',
                silent=settings.SILENT)
 
-    return False
+    return False, False
+
+
+def update_price_breaks(supplier_part, price_breaks: dict) -> bool:
+    ''' Update the Price Breaks associated with a supplier part '''
+    if not isinstance(supplier_part, SupplierPart):
+        try:
+            supplier_part = SupplierPart(inventree_api, supplier_part)
+        except:
+            cprint('[TREE]\tWarning: Supplier part not found, skipping price break update',
+                   silent=settings.SILENT)
+            return False
+    if not price_breaks:
+        cprint('[TREE]\tWarning: No price breaks found, skipping.', silent=settings.SILENT)
+        return False
+
+    old_price_breaks = supplier_part.getPriceBreaks()
+    updated = []
+    # First process existing price breaks
+    for old_price_break in old_price_breaks:
+        quantity = old_price_break.quantity
+        price = price_breaks[quantity]
+        # remove everything but the numbers from the price break
+        if isinstance(price, str):
+            price = re.findall('\d+.\d+', price)[0]
+            price = price.replace(',', '.')
+        if quantity in price_breaks:
+            old_price_break.save(data={'price': price})
+            updated.append(quantity)
+        else:
+            old_price_break.delete()
+    for quantity in updated:
+        del price_breaks[quantity]
+    # if any price breaks are left over these will be created
+    for quantity, price in price_breaks.items():
+        # remove everything but the numbers from the price break
+        if isinstance(price, str):
+            price = re.findall('\d+.\d+', price)[0]
+            price = price.replace(',', '.')
+        SupplierPriceBreak.create(inventree_api, {
+            'part': supplier_part.pk,
+            'quantity': quantity,
+            'price': price,
+        })
+    cprint('[INFO]\tSuccess: The price breaks were updated', silent=settings.SILENT)
+    return True
 
 
 def create_parameter_template(name: str, units: str) -> int:
     ''' Create InvenTree parameter template '''
     global inventree_api
 
     parameter_templates = ParameterTemplate.list(inventree_api)
@@ -607,33 +699,41 @@
             template_id = item.pk
             break
 
     # Check if template_id already exists for this part
     part = Part(inventree_api, part_id)
     part_parameters = part.getParameters()
     is_new_part_parameters_template_id = True
+    was_updated = False
+    parameter = None
     for item in part_parameters:
         # cprint(f'[TREE]\t{parameter.template} ?= {template_id}', silent=SILENT)
         if item.template == template_id:
             is_new_part_parameters_template_id = False
+            if settings.UPDATE_INVENTREE:
+                if value != item.data and value != '-':
+                    parameter = item
+                    was_updated = True
+                    parameter.save(data={
+                        'data': value
+                    })
             break
     # cprint(part_parameters, silent=SILENT)
 
     '''
         Create parameter only if:
         - template exists
         - parameter does not exist for this part
     '''
-    parameter = None
     if template_id > 0 and is_new_part_parameters_template_id:
         parameter = Parameter.create(inventree_api, {
             'part': part_id,
             'template': template_id,
             'data': value,
         })
 
     if parameter:
-        return parameter.pk, is_new_part_parameters_template_id
+        return parameter.pk, is_new_part_parameters_template_id, was_updated
     else:
         if template_id == 0:
             cprint(f'[TREE]\tError: Parameter template "{template_name}" does not exist', silent=settings.SILENT)
-        return 0, False
+        return 0, False, False
```

### Comparing `kintree-1.0.1/kintree/database/inventree_interface.py` & `kintree-1.0.2/kintree/database/inventree_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,19 +66,19 @@
     category_data = config_interface.load_file(settings.CONFIG_CATEGORIES)
 
     def build_tree(tree, left_to_go, level) -> list:
         try:
             last_entry = f' {category_tree(tree[-1])}{category_separator}'
         except IndexError:
             last_entry = ''
-        if type(left_to_go) == dict:
+        if isinstance(left_to_go, dict):
             for key, value in left_to_go.items():
                 tree.append(f'{"-" * level}{last_entry}{key}')
                 build_tree(tree, value, level + 1)
-        elif type(left_to_go) == list:
+        elif isinstance(left_to_go, list):
             # Supports legacy structure
             for item in left_to_go:
                 tree.append(f'{"-" * level}{last_entry}{item}')
         elif left_to_go is None:
             pass
         return
     
@@ -259,14 +259,15 @@
     inventree_part['manufacturer_part_number'] = part_info['manufacturer_part_number']
     inventree_part['IPN'] = part_info.get('IPN', '')
     # Replace whitespaces in URL
     inventree_part['supplier_link'] = part_info['supplier_link'].replace(' ', '%20')
     inventree_part['datasheet'] = part_info['datasheet'].replace(' ', '%20')
     # Image URL is not shown to user so force default key/value
     inventree_part['image'] = part_info['image'].replace(' ', '%20')
+    inventree_part['pricing'] = part_info.get('pricing', {})
 
     # Load parameters map
     if category_tree:
         parameter_map = config_interface.load_category_parameters(
             categories=category_tree,
             supplier_config_path=settings.CONFIG_SUPPLIER_PARAMETERS,
         )
@@ -522,15 +523,14 @@
             new_part = True
             # Create a new Part
             # Use the pk (primary-key) of the category
             part_pk = inventree_api.create_part(category_id=category_pk,
                                                 name=inventree_part['name'],
                                                 description=inventree_part['description'],
                                                 revision=inventree_part['revision'],
-                                                image=inventree_part['image'],
                                                 keywords=inventree_part['keywords'])
 
             # Check part primary key
             if not part_pk:
                 return new_part, part_pk, inventree_part
             # Progress Update
             if not progress.update_progress_bar(show_progress):
@@ -563,14 +563,22 @@
         if new_part:
             cprint('[INFO]\tSuccess: Added new part to InvenTree', silent=settings.SILENT)
             if inventree_part['image']:
                 # Add image
                 image_result = inventree_api.upload_part_image(inventree_part['image'], part_pk)
                 if not image_result:
                     cprint('[TREE]\tWarning: Failed to upload part image', silent=settings.SILENT)
+            if inventree_part['datasheet'] and settings.DATASHEET_UPLOAD:
+                # Upload datasheet
+                datasheet_link = inventree_api.upload_part_datasheet(
+                    inventree_part['datasheet'], part_pk)
+                if not datasheet_link:
+                    cprint('[TREE]\tWarning: Failed to upload part datasheet', silent=settings.SILENT)
+                else:
+                    inventree_part['datasheet'] = datasheet_link
 
         if kicad:
             try:
                 symbol_name = ipn
             except UnboundLocalError:
                 symbol_name = inventree_part.get('manufacturer_part_number')
 
@@ -586,39 +594,20 @@
 
             # Add category-defined parameters
             for parameter in category_parameters:
                 inventree_part['parameters'][parameter[0]] = parameter[1]
 
         # Create parameters
         if len(inventree_part['parameters']) > 0:
-            cprint('\n[MAIN]\tCreating parameters', silent=settings.SILENT)
-            parameters_lists = [
-                [],  # Store new parameters
-                [],  # Store existings parameters
-            ]
-            for name, value in inventree_part['parameters'].items():
-                parameter, is_new_parameter = inventree_api.create_parameter(part_id=part_pk, template_name=name, value=value)
-                # Progress Update
-                if not progress.update_progress_bar(show_progress, increment=0.03):
-                    return new_part, part_pk, inventree_part
-
-                if is_new_parameter:
-                    parameters_lists[0].append(name)
-                else:
-                    parameters_lists[1].append(name)
-
-            if parameters_lists[0]:
-                cprint('[INFO]\tSuccess: The following parameters were created:', silent=settings.SILENT)
-                for item in parameters_lists[0]:
-                    cprint(f'--->\t{item}', silent=settings.SILENT)
-            if parameters_lists[1]:
-                cprint('[TREE]\tWarning: The following parameters were skipped:', silent=settings.SILENT)
-                for item in parameters_lists[1]:
-                    cprint(f'--->\t{item}', silent=settings.SILENT)
-
+            if not inventree_process_parameters(
+                    part_id=part_pk,
+                    parameters=inventree_part['parameters'],
+                    show_progress=show_progress):
+                return new_part, part_pk, inventree_part
+            
         # Create manufacturer part
         if inventree_part['manufacturer_name'] and inventree_part['manufacturer_part_number']:
             # Overwrite manufacturer name with matching one from database
             manufacturer_name = inventree_fuzzy_company_match(inventree_part['manufacturer_name'])
             # Get MPN
             manufacturer_mpn = inventree_part['manufacturer_part_number']
 
@@ -647,61 +636,127 @@
         if inventree_part['supplier_name'] and inventree_part['supplier_part_number']:
             # Overwrite manufacturer name with matching one from database
             supplier_name = inventree_fuzzy_company_match(inventree_part['supplier_name'])
             # Get SKU
             supplier_sku = inventree_part['supplier_part_number']
 
             cprint('\n[MAIN]\tCreating supplier part', silent=settings.SILENT)
-            is_new_supplier_part = inventree_api.is_new_supplier_part(supplier_name=supplier_name,
-                                                                      supplier_sku=supplier_sku)
+            is_new_supplier_part, supplier_part = inventree_api.is_new_supplier_part(
+                supplier_name=supplier_name,
+                supplier_sku=supplier_sku)
 
             if not is_new_supplier_part:
                 cprint('[INFO]\tSupplier part already exists, skipping.', silent=settings.SILENT)
             else:
                 # Create a new supplier part
-                is_supplier_part_created = inventree_api.create_supplier_part(
+                is_supplier_part_created, supplier_part = inventree_api.create_supplier_part(
                     part_id=part_pk,
                     manufacturer_name=manufacturer_name,
                     manufacturer_mpn=manufacturer_mpn,
                     supplier_name=supplier_name,
                     supplier_sku=supplier_sku,
                     description=inventree_part['description'],
                     link=inventree_part['supplier_link'],
                 )
 
                 if is_supplier_part_created:
                     cprint('[INFO]\tSuccess: Added new supplier part', silent=settings.SILENT)
+            
+            if supplier_part:
+                cprint('\n[MAIN]\tProcessing Price Breaks', silent=settings.SILENT)
+                inventree_api.update_price_breaks(
+                    supplier_part=supplier_part,
+                    price_breaks=inventree_part['pricing'])
 
     # Progress Update
     if not progress.update_progress_bar(show_progress):
         pass
 
     return new_part, part_pk, inventree_part
 
 
+def inventree_process_parameters(part_id: str, parameters: dict, show_progress=True) -> bool:
+    ''' Create or Update parameters for an InvenTree part'''
+    cprint('\n[MAIN]\tCreating parameters', silent=settings.SILENT)
+    parameters_lists = [
+        [],  # Store new parameters
+        [],  # Store updated parameters
+        [],  # Store unchanged parameters
+    ]
+    for name, value in parameters.items():
+        parameter, is_new_parameter, was_updated = inventree_api.create_parameter(part_id=part_id, template_name=name, value=value)
+        # Progress Update
+        if not progress.update_progress_bar(show_progress, increment=0.03):
+            return False
+        if is_new_parameter:
+            parameters_lists[0].append(name)
+        elif was_updated:
+            parameters_lists[1].append(name)
+        else:
+            parameters_lists[2].append(name)
+    if parameters_lists[0]:
+        cprint('[INFO]\tSuccess: The following parameters were created:', silent=settings.SILENT)
+        for item in parameters_lists[0]:
+            cprint(f'--->\t{item}', silent=settings.SILENT)
+    if parameters_lists[1]:
+        cprint('[INFO]\tSuccess: The following parameters were updated:', silent=settings.SILENT)
+        for item in parameters_lists[1]:
+            cprint(f'--->\t{item}', silent=settings.SILENT)
+    if parameters_lists[2]:
+        cprint('[TREE]\tWarning: The following parameters were skipped:', silent=settings.SILENT)
+        for item in parameters_lists[2]:
+            cprint(f'--->\t{item}', silent=settings.SILENT)
+    return True
+
+
 def inventree_create_alternate(part_info: dict, part_id='', part_ipn='', show_progress=None) -> bool:
     ''' Create alternate manufacturer and supplier entries for an existing InvenTree part '''
 
     result = False
     cprint('\n[MAIN]\tSearching for original part in database', silent=settings.SILENT)
     part = inventree_api.fetch_part(part_id, part_ipn)
 
     if part:
         part_pk = part.pk
         part_description = part.description
         cprint(f'[INFO] Success: Found original part in database (ID = {part_pk} | Description = "{part_description}")', silent=settings.SILENT)
     else:
         cprint('[INFO] Error: Original part was not found in database', silent=settings.SILENT)
         return result
+    # Translate to InvenTree part format
+    category_tree = inventree_api.get_category_tree(part.category)
+    category_tree = list(category_tree.values())
+    inventree_part = translate_form_to_inventree(
+        part_info=part_info,
+        category_tree=category_tree,
+    )
+
+    # If the part has no image yet try to upload it from the data
+    if not part.image:
+        image = part_info.get('image', '')
+        if image:
+            inventree_api.upload_part_image(image_url=image, part_id=part_pk)
+
+    # create or update parameters
+    if inventree_part.get('parameters', {}):
+        inventree_process_parameters(part_id=part_pk,
+                                     parameters=inventree_part['parameters'],
+                                     show_progress=show_progress)
 
     # Overwrite manufacturer name with matching one from database
     manufacturer_name = inventree_fuzzy_company_match(part_info.get('manufacturer_name', ''))
     manufacturer_mpn = part_info.get('manufacturer_part_number', '')
     datasheet = part_info.get('datasheet', '')
 
+    # if datasheet upload is enabled and no attechment present yet upload
+    if settings.DATASHEET_UPLOAD and not part.getAttachments():
+        if datasheet:
+            inventree_api.upload_part_datasheet(part_id=part_pk,
+                                                datasheet_url=datasheet)
+
     # Create manufacturer part
     if manufacturer_name and manufacturer_mpn:
         inventree_create_manufacturer_part(part_id=part_pk,
                                            manufacturer_name=manufacturer_name,
                                            manufacturer_mpn=manufacturer_mpn,
                                            datasheet=datasheet,
                                            description=part_description)
@@ -715,29 +770,39 @@
     supplier_name = part_info.get('supplier_name', '')
     supplier_sku = part_info.get('supplier_part_number', '')
     supplier_link = part_info.get('supplier_link', '')
 
     # Add supplier alternate
     if supplier_name and supplier_sku:
         cprint('\n[MAIN]\tCreating supplier part', silent=settings.SILENT)
-        is_new_supplier_part = inventree_api.is_new_supplier_part(supplier_name=supplier_name,
-                                                                  supplier_sku=supplier_sku)
+        is_new_supplier_part, supplier_part = inventree_api.is_new_supplier_part(
+            supplier_name=supplier_name,
+            supplier_sku=supplier_sku)
 
         if not is_new_supplier_part:
             cprint('[INFO]\tSupplier part already exists, skipping.', silent=settings.SILENT)
         else:
             # Create a new supplier part
-            is_supplier_part_created = inventree_api.create_supplier_part(part_id=part_pk,
-                                                                          manufacturer_name=manufacturer_name,
-                                                                          manufacturer_mpn=manufacturer_mpn,
-                                                                          supplier_name=supplier_name,
-                                                                          supplier_sku=supplier_sku,
-                                                                          description=part_description,
-                                                                          link=supplier_link)
+            is_supplier_part_created, supplier_part = inventree_api.create_supplier_part(
+                part_id=part_pk,
+                manufacturer_name=manufacturer_name,
+                manufacturer_mpn=manufacturer_mpn,
+                supplier_name=supplier_name,
+                supplier_sku=supplier_sku,
+                description=part_description,
+                link=supplier_link)
 
             if is_supplier_part_created:
                 cprint('[INFO]\tSuccess: Added new supplier part', silent=settings.SILENT)
                 result = True
+
+        if supplier_part:
+            cprint('\n[MAIN]\tProcessing Price Breaks', silent=settings.SILENT)
+            inventree_api.update_price_breaks(
+                supplier_part=supplier_part,
+                price_breaks=inventree_part['pricing'])
+            result = True
+    
     else:
         cprint('[INFO]\tWarning: No supplier part to create', silent=settings.SILENT)
 
     return result
```

### Comparing `kintree-1.0.1/kintree/gui/gui.py` & `kintree-1.0.2/kintree/gui/gui.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/gui/logo.png` & `kintree-1.0.2/kintree/gui/logo.png`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/gui/views/common.py` & `kintree-1.0.2/kintree/gui/views/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,21 +159,21 @@
             d_type: Optional[DialogType] = None,
             message: Optional[str] = None,
             snackbar=True,
             open=True,
     ):
         if snackbar:
             self.build_snackbar(d_type, message)
-        if type(self.dialog) == ft.SnackBar:
+        if isinstance(self.dialog, ft.SnackBar):
             self.page.snack_bar = self.dialog
             self.page.snack_bar.open = True
-        elif type(self.dialog) == ft.Banner:
+        elif isinstance(self.dialog, ft.Banner):
             self.page.banner = self.dialog
             self.page.banner.open = open
-        elif type(self.dialog) == ft.AlertDialog:
+        elif isinstance(self.dialog, ft.AlertDialog):
             self.page.dialog = self.dialog
             self.page.dialog.open = open
         self.page.update()
 
 
 class SwitchWithRefs(ft.Switch):
     '''Link the visibility of other fields to a switch value'''
```

### Comparing `kintree-1.0.1/kintree/gui/views/main.py` & `kintree-1.0.2/kintree/gui/views/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,22 +141,22 @@
 
     def call_settings(self, e):
         handle_transition(self.page, transition=True)
         self.page.go('/settings')
 
     def reset_view(self, e, ignore=['enable'], hidden={}):
         def reset_field(field):
-            if type(field) is ft.ProgressBar:
+            if isinstance(field, ft.ProgressBar):
                 field.value = 0
             else:
                 field.value = None
             field.update()
 
         for name, field in self.fields.items():
-            if type(field) == dict:
+            if isinstance(field, dict):
                 for key, value in field.items():
                     value.disabled = True
                     reset_field(value)
             else:
                 if name not in ignore:
                     reset_field(field)
 
@@ -249,15 +249,15 @@
 
     fields = {
         'part_number': ft.TextField(
             label="Part Number",
             dense=True,
             hint_text="Part Number",
             width=300,
-            expand=True
+            expand=True,
         ),
         'supplier': ft.Dropdown(
             label="Supplier",
             dense=True,
             width=250
         ),
         'search_button': ft.IconButton(
@@ -322,14 +322,17 @@
                     part_supplier_form = inventree_interface.translate_supplier_to_form(
                         supplier=supplier,
                         part_info=part_supplier_info,
                     )
                     # Stitch parameters
                     if part_supplier_info.get('parameters', None):
                         self.data['parameters'] = part_supplier_info['parameters']
+                    # and pricing
+                    if part_supplier_info.get('pricing', None):
+                        self.data['pricing'] = part_supplier_info['pricing']
 
                 if part_supplier_form:
                     for field_idx, field_name in enumerate(self.fields['search_form'].keys()):
                         # print(field_idx, field_name, get_default_search_keys()[field_idx], search_form_field[field_name])
                         try:
                             self.fields['search_form'][field_name].value = part_supplier_form.get(field_name, '')
                         except IndexError:
@@ -444,15 +447,15 @@
     title = 'InvenTree'
     fields = {
         'enable': ft.Switch(
             label='InvenTree',
             value=settings.ENABLE_INVENTREE,
         ),
         'alternate': ft.Switch(
-            label='Alternate',
+            label='Update existing',
             value=settings.ENABLE_ALTERNATE if settings.ENABLE_INVENTREE else False,
             disabled=not settings.ENABLE_INVENTREE,
         ),
         'load_categories': ft.ElevatedButton(
             'Reload InvenTree Categories',
             width=GUI_PARAMS['button_width'] * 2.6,
             height=36,
@@ -491,14 +494,19 @@
         ),
         'Existing Part IPN': ft.TextField(
             label='Existing Part IPN',
             width=GUI_PARAMS['textfield_width'] / 2 - 5,
             dense=GUI_PARAMS['textfield_dense'],
             visible=True,
         ),
+        'Update Parameter': SwitchWithRefs(
+            label='Update Parameter',
+            value=settings.UPDATE_INVENTREE if settings.ENABLE_INVENTREE else False,
+            disabled=not settings.ENABLE_INVENTREE,
+        ),
     }
 
     def __init__(self, page: ft.Page):
         self.category_row_ref = ft.Ref[ft.Row]()
         self.ipncode_row_ref = ft.Ref[ft.Row]()
         self.alternate_row_ref = ft.Ref[ft.Row]()
         super().__init__(page)
@@ -553,26 +561,38 @@
 
         # Alternate row visibility
         self.alternate_row_ref.current.visible = alt_visible
         self.alternate_row_ref.current.update()
 
         # Update settings
         settings.set_enable_flag('alternate', alt_visible)
+        settings.set_enable_flag('update', alt_visible)
         # User dialog
         if alt_visible:
             self.show_dialog(
                 d_type=DialogType.WARNING,
                 message='Alternate Mode Enabled: Enter Existing Part ID or Part IPN',
             )
 
         self.push_data(e)
 
+    def process_update(self, e, value=None):
+        if value is not None:
+            update_enabled = value
+        else:
+            # Get switch value
+            update_enabled = False
+            if e.data.lower() == 'true':
+                update_enabled = True
+        settings.set_enable_flag('update', update_enabled)
+        self.push_data(e)
+
     def process_category(self, e=None, label=None, value=None):
         parent_category = None
-        if type(self.fields['Category'].value) == str:
+        if isinstance(self.fields['Category'].value, str):
             parent_category = inventree_interface.split_category_tree(self.fields['Category'].value)[0]
         self.fields['IPN: Category Code'].options = self.get_code_options()
         # Select category code corresponding to selected category
         code = config_interface.load_file(settings.CONFIG_CATEGORIES)['CODES'].get(parent_category, None)
         if code and not self.fields['Create New Code'].value:
             self.fields['IPN: Category Code'].value = code
         self.fields['IPN: Category Code'].update()
@@ -634,14 +654,15 @@
         self.fields['IPN: Category Code'].on_change = self.push_data
         self.fields['Create New Code'].on_change = self.create_ipn_code
         self.fields['New Category Code'].on_change = self.push_data
         # Alternate fields
         self.fields['alternate'].on_change = self.process_alternate
         self.fields['Existing Part ID'].on_change = self.push_data
         self.fields['Existing Part IPN'].on_change = self.push_data
+        self.fields['Update Parameter'].on_change = self.process_update
 
         self.column = ft.Column(
             controls=[
                 ft.Row(),
                 ft.Row(
                     [
                         self.fields['enable'],
@@ -673,20 +694,27 @@
                                         ),
                                     ],
                                 ),
                             ],
                         ),
                     ],
                 ),
-                ft.Row(
+                ft.Column(
                     ref=self.alternate_row_ref,
                     controls=[
-                        self.fields['Existing Part ID'],
-                        self.fields['Existing Part IPN'],
-                    ],
+                        ft.Row(
+                            controls=[
+                                self.fields['Existing Part ID'],
+                                self.fields['Existing Part IPN'],
+                            ],
+                        ),
+                        ft.Row(
+                            controls=[self.fields['Update Parameter']]
+                        )
+                    ]
                 ),
             ],
         )
 
         # Connect New Category Code fields
         cc_ref = ft.Ref[ft.TextField]()
         cc_ref.current = self.fields['New Category Code']
@@ -922,18 +950,18 @@
             controls=[ft.Row()],
             alignment=ft.MainAxisAlignment.START,
             expand=True,
         )
         kicad_inputs = []
         for name, field in self.fields.items():
             # Update callbacks
-            if type(field) == ft.ElevatedButton:
+            if isinstance(field, ft.ElevatedButton):
                 field.on_click = self.check_snapeda
             # Update options
-            elif type(field) == DropdownWithSearch:
+            elif isinstance(field, DropdownWithSearch):
                 field.label = name
                 if name == 'Symbol Library':
                     field.options = self.build_library_options(type='symbol')
                 elif name == 'Symbol Template':
                     field.options = self.build_library_options(type='template')
                 elif name == 'Footprint Library':
                     field.options = self.build_library_options(type='footprint')
```

### Comparing `kintree-1.0.1/kintree/gui/views/settings.py` & `kintree-1.0.2/kintree/gui/views/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,24 @@
             False,  # Browse disabled
         ],
         'Proxy': [
             'PROXY',
             ft.TextField(),
             False,  # Browse disabled
         ],
+        'Upload Datasheets to InvenTree': [
+            'DATASHEET_UPLOAD',
+            SwitchWithRefs(),
+            False,  # Browse enabled
+        ],
+        'Upload Pricing Data to InvenTree': [
+            'PRICING_UPLOAD',
+            SwitchWithRefs(),
+            False,  # Browse enabled
+        ],
         'Default Part Revision': [
             'INVENTREE_DEFAULT_REV',
             ft.TextField(),
             False,  # Browse disabled
         ],
         'Enable Internal Part Number (IPN)': [
             'IPN_ENABLE_CREATE',
@@ -277,15 +287,15 @@
         3: '/settings/kicad',
     }
 
     def __init__(self, page: ft.Page):
         # Load setting fields
         self.fields = {}
         for field_name, field_data in SETTINGS.get(self.title, {}).items():
-            if type(field_data) == list and field_data[0] is not None:
+            if isinstance(field_data, list) and field_data[0] is not None:
                 self.fields[field_name] = field_data[1]
                 self.fields[field_name].value = self.settings[field_data[0]]
 
         # Init view
         super().__init__(page=page, appbar=settings_appbar, navigation_rail=settings_navrail)
 
         # Update navigation rail
@@ -343,15 +353,15 @@
                 ft.Row(),
             ],
             alignment=ft.MainAxisAlignment.START,
             expand=True,
         )
 
     def update_field(self, name, field, column):
-        if type(field) == ft.TextField:
+        if isinstance(field, ft.TextField):
             field_predefined = bool(field.width)
             if not field_predefined:
                 field.label = name
                 field.width = GUI_PARAMS['textfield_width']
                 field.dense = GUI_PARAMS['textfield_dense']
                 if 'password' in field.label.lower():
                     field.password = True
@@ -372,39 +382,39 @@
                     )
                 column.controls.extend(
                     [
                         field_row,
                         ft.Row(height=GUI_PARAMS['textfield_space_after']),
                     ]
                 )
-        elif type(field) == ft.Text:
+        elif isinstance(field, ft.Text):
             field.value = name
             field_row = ft.Row(
                 controls=[
                     field,
                 ]
             )
             column.controls.append(field_row)
             column.controls.append(ft.Divider())
-        elif type(field) == ft.TextButton:
+        elif isinstance(field, ft.TextButton):
             column.controls.append(
                 ft.ElevatedButton(
                     name,
                     width=GUI_PARAMS['button_width'] * 2,
                     height=GUI_PARAMS['button_height'],
                     icon=ft.icons.CHECK_OUTLINED,
                     on_click=lambda e, s=name: self.test_s(e, s=s)
                 ),
             )
-        elif type(field) == ft.Dropdown:
+        elif isinstance(field, ft.Dropdown):
             field.on_change = lambda _: self.save()
             column.controls.append(
                 field,
             )
-        elif type(field) == ft.Switch or type(field) == SwitchWithRefs:
+        elif isinstance(field, ft.Switch) or isinstance(field, SwitchWithRefs):
             if 'proxy' in name.lower():
                 field.on_change = lambda _: None
             else:
                 field.on_change = lambda _: self.save()
             field.label = name
             column.controls.append(
                 field,
@@ -485,19 +495,24 @@
             'AUTOMATIC_BROWSER_OPEN': global_settings.AUTOMATIC_BROWSER_OPEN
         },
         **{
             'CACHE_ENABLED': global_settings.CACHE_ENABLED,
             'CACHE_VALID_DAYS': global_settings.CACHE_VALID_DAYS
         },
     }
-    settings_file = [
+    settings_file_list = [
         global_settings.USER_CONFIG_FILE,
         global_settings.CONFIG_GENERAL_PATH,
         global_settings.CONFIG_SEARCH_API_PATH,
     ]
+
+    def save(self):
+        # Save all settings
+        for sf in self.settings_file_list:
+            super().save(settings_file=sf, show_dialog=True)
     
     def increment_cache_value(self, inc):
         field = SETTINGS[self.title]['CACHE_VALID_DAYS'][1]
         current_value = int(field.value)
         if not inc:
             if current_value > 1:
                 field.value = f'{current_value - 1}'
@@ -528,34 +543,25 @@
                 SETTINGS[self.title]['CACHE_VALID_DAYS'][1],
                 ft.IconButton(ft.icons.ADD, on_click=lambda _: self.increment_cache_value(True)),
             ],
         )
         self.column.controls.append(cache_row)
         # Add cache row to switch refs
         SETTINGS[self.title]['Enable Supplier Search Cache'][1].refs = [cache_row_ref]
-        
-        setting_file1 = self.settings_file[1]
-        setting_file2 = self.settings_file[2]
 
         for name, field in SETTINGS[self.title].items():
-            if field[0] in ['AUTOMATIC_BROWSER_OPEN', 'DATASHEET_SAVE_ENABLED', 'DATASHEET_SAVE_PATH']:
-                self.fields[name].on_change = lambda _: self.save(
-                    settings_file=setting_file1,
-                    show_dialog=False
-                )
+            if field[0] in ['AUTOMATIC_BROWSER_OPEN', 'DATASHEET_SAVE_ENABLED', 'DATASHEET_SAVE_PATH', 'DATASHEET_INVENTREE_ENABLED']:
+                self.fields[name].on_change = lambda _: self.save()
             elif field[0] in ['CACHE_ENABLED', 'CACHE_VALID_DAYS']:
-                self.fields[name].on_change = lambda _: self.save(
-                    settings_file=setting_file2,
-                    show_dialog=False
-                )
-        self.settings_file = self.settings_file[0]
+                self.fields[name].on_change = lambda _: self.save()
+        self.settings_file = self.settings_file_list[0]
 
         # Update datasheet ref
         for idx, field in enumerate(self.column.controls):
-            if type(field) == SwitchWithRefs:
+            if isinstance(field, SwitchWithRefs):
                 if field.label == 'Save Datasheets to Local Folder':
                     datasheet_row_ref.current = self.column.controls[idx + 1]
                     SETTINGS[self.title]['Save Datasheets to Local Folder'][1].refs = [datasheet_row_ref]
         
         # Save button
         self.add_buttons(self.column, test=False)
 
@@ -759,14 +765,18 @@
             config_interface.save_inventree_user_settings(
                 enable=global_settings.ENABLE_INVENTREE,
                 server=address,
                 username=SETTINGS[self.title]['Username'][1].value,
                 password=SETTINGS[self.title]['Password or Token'][1].value,
                 enable_proxy=enable_proxy,
                 proxies=proxies,
+                datasheet_upload=SETTINGS[self.title][
+                    'Upload Datasheets to InvenTree'][1].value,
+                pricing_upload=SETTINGS[self.title][
+                    'Upload Pricing Data to InvenTree'][1].value,
                 user_config_path=self.settings_file[0]
             )
             # Alert user
             if dialog:
                 self.show_dialog(
                     d_type=DialogType.VALID,
                     message=f'{self.title} successfully saved',
```

### Comparing `kintree-1.0.1/kintree/kicad/kicad_symbol.py` & `kintree-1.0.2/kintree/kicad/kicad_symbol.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/LICENSE` & `kintree-1.0.2/kintree/kicad/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/capacitor-polarized.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/capacitor-polarized.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/capacitor.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/capacitor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/connector.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/connector.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/crystal-2p.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/crystal-2p.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/default.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/default.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/diode-led.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/diode-led.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/diode-schottky.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/diode-schottky.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/diode-standard.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/diode-standard.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/diode-zener.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/diode-zener.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/eeprom-sot23.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/eeprom-sot23.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/ferrite-bead.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/ferrite-bead.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/fuse.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/fuse.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/inductor.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/inductor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/integrated-circuit.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/integrated-circuit.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/oscillator-4p.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/oscillator-4p.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/protection-unidir.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/protection-unidir.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/resistor-sm.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/resistor-sm.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/resistor.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/resistor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/transistor-nfet.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/transistor-nfet.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/transistor-npn.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/transistor-npn.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/transistor-pfet.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/transistor-pfet.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates/transistor-pnp.kicad_sym` & `kintree-1.0.2/kintree/kicad/templates/transistor-pnp.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pcb` & `kintree-1.0.2/kintree/kicad/templates_project/templates_project.kicad_pcb`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_prl` & `kintree-1.0.2/kintree/kicad/templates_project/templates_project.kicad_prl`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pro` & `kintree-1.0.2/kintree/kicad/templates_project/templates_project.kicad_pro`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/search/digikey_api.py` & `kintree-1.0.2/kintree/search/digikey_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 ]
 PARAMETERS_MAP = [
     'parameters',
     'parameter',
     'value',
 ]
 
+PRICING_MAP = [
+    'standard_pricing',
+    'break_quantity',
+    'unit_price',
+]
+
 
 os.environ['DIGIKEY_STORAGE_PATH'] = settings.DIGIKEY_STORAGE_PATH
 # Check if storage path exists, else create it
 if not os.path.exists(os.environ['DIGIKEY_STORAGE_PATH']):
     os.makedirs(os.environ['DIGIKEY_STORAGE_PATH'], exist_ok=True)
 
 
@@ -145,14 +151,23 @@
 
     for parameter in range(len(part[parameter_key])):
         parameter_name = part[parameter_key][parameter][name_key]
         parameter_value = part[parameter_key][parameter][value_key]
         # Append to parameters dictionary
         part_info['parameters'][parameter_name] = parameter_value
 
+    # Pricing
+    part_info['pricing'] = {}
+    [pricing_key, qty_key, price_key] = PRICING_MAP
+
+    for price_break in part[pricing_key]:
+        quantity = price_break[qty_key]
+        price = price_break[price_key]
+        part_info['pricing'][quantity] = price
+
     # Extra search fields
     if settings.CONFIG_DIGIKEY.get('EXTRA_FIELDS', None):
         for extra_field in settings.CONFIG_DIGIKEY['EXTRA_FIELDS']:
             if part.get(extra_field, None):
                 part_info['parameters'][extra_field] = part[extra_field]
             else:
                 from ..common.tools import cprint
```

### Comparing `kintree-1.0.1/kintree/search/element14_api.py` & `kintree-1.0.2/kintree/search/element14_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 
 PARAMETERS_MAP = [
     'attributes',
     'attributeLabel',
     'attributeValue',
 ]
 
+PRICING_MAP = [
+    'prices',
+    'from',
+    'cost',
+]
+
 
 def get_default_search_keys():
     return [
         'displayName',
         'displayName',
         'revision',
         'keywords',
@@ -205,14 +211,23 @@
                 parameter_value = part[parameter_key][parameter][value_key]
                 # Append to parameters dictionary
                 part_info['parameters'][parameter_name] = parameter_value
         except TypeError:
             # Parameter list is empty
             pass
 
+    # Pricing
+    part_info['pricing'] = {}
+    [pricing_key, qty_key, price_key] = PRICING_MAP
+
+    for price_break in part[pricing_key]:
+        quantity = price_break[qty_key]
+        price = price_break[price_key]
+        part_info['pricing'][quantity] = price
+
     # Extra search fields
     if settings.CONFIG_ELEMENT14.get('EXTRA_FIELDS', None):
         for extra_field in settings.CONFIG_ELEMENT14['EXTRA_FIELDS']:
             if part.get(extra_field, None):
                 part_info['parameters'][extra_field] = part[extra_field]
             else:
                 from ..common.tools import cprint
```

### Comparing `kintree-1.0.1/kintree/search/lcsc_api.py` & `kintree-1.0.2/kintree/search/lcsc_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 ]
 PARAMETERS_MAP = [
     'paramVOList',
     'paramNameEn',
     'paramValueEn',
 ]
 
+PRICING_MAP = [
+    'productPriceList',
+    'ladder',
+    'productPrice',
+]
+
 
 def get_default_search_keys():
     return [
         'productIntroEn',
         'productIntroEn',
         'revision',
         'keywords',
@@ -95,14 +101,23 @@
             parameter_value = part[parameter_key][parameter][value_key]
             # Append to parameters dictionary
             part_info['parameters'][parameter_name] = parameter_value
     except TypeError:
         # Parameter list is empty
         pass
 
+    # Pricing
+    part_info['pricing'] = {}
+    [pricing_key, qty_key, price_key] = PRICING_MAP
+
+    for price_break in part[pricing_key]:
+        quantity = price_break[qty_key]
+        price = price_break[price_key]
+        part_info['pricing'][quantity] = price
+
     # Extra search fields
     if settings.CONFIG_LCSC.get('EXTRA_FIELDS', None):
         for extra_field in settings.CONFIG_LCSC['EXTRA_FIELDS']:
             if part.get(extra_field, None):
                 part_info['parameters'][extra_field] = part[extra_field]
             else:
                 from ..common.tools import cprint
```

### Comparing `kintree-1.0.1/kintree/search/mouser_api.py` & `kintree-1.0.2/kintree/search/mouser_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 ]
 PARAMETERS_MAP = [
     'ProductAttributes',
     'AttributeName',
     'AttributeValue',
 ]
 
+PRICING_MAP = [
+    'PriceBreaks',
+    'Quantity',
+    'Price',
+]
+
 
 def get_default_search_keys():
     return [
         'Description',
         'Description',
         'revision',
         'keywords',
@@ -105,14 +111,23 @@
 
     for parameter in range(len(part[parameter_key])):
         parameter_name = part[parameter_key][parameter][name_key]
         parameter_value = part[parameter_key][parameter][value_key]
         # Append to parameters dictionary
         part_info['parameters'][parameter_name] = parameter_value
 
+    # Pricing
+    part_info['pricing'] = {}
+    [pricing_key, qty_key, price_key] = PRICING_MAP
+
+    for price_break in part[pricing_key]:
+        quantity = price_break[qty_key]
+        price = price_break[price_key]
+        part_info['pricing'][quantity] = price
+
     # Extra search fields
     if settings.CONFIG_MOUSER.get('EXTRA_FIELDS', None):
         for extra_field in settings.CONFIG_MOUSER['EXTRA_FIELDS']:
             if part.get(extra_field, None):
                 part_info['parameters'][extra_field] = part[extra_field]
             else:
                 from ..common.tools import cprint
```

### Comparing `kintree-1.0.1/kintree/search/search_api.py` & `kintree-1.0.2/kintree/search/search_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/kintree/search/snapeda_api.py` & `kintree-1.0.2/kintree/search/snapeda_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..config import settings
-from ..common.tools import download, download_image
+from ..common.tools import download, download_with_retry
 
 API_BASE_URL = 'https://snapeda.eeinte.ch/?'
 SNAPEDA_URL = 'https://www.snapeda.com'
 
 
 def fetch_snapeda_part_info(part_number: str) -> dict:
     ''' Fetch SnapEDA part data from API '''
@@ -79,28 +79,28 @@
         try:
             if snapeda_data['symbol_image']:
                 # Form path
                 image_name = f'{part_number}_symbol.png'
                 image_location = settings.search_images + image_name
 
                 # Download symbol image
-                symbol = download_image(snapeda_data['symbol_image'], image_location)
+                symbol = download_with_retry(snapeda_data['symbol_image'], image_location, filetype='Image')
                 if symbol:
                     images['symbol'] = image_location
         except KeyError:
             pass
 
         try:
             if snapeda_data['footprint_image']:
                 # Form path
                 image_name = f'{part_number}_footprint.png'
                 image_location = settings.search_images + image_name
 
                 # Download symbol image
-                footprint = download_image(snapeda_data['footprint_image'], image_location)
+                footprint = download_with_retry(snapeda_data['footprint_image'], image_location, filetype='Image')
                 if footprint:
                     images['footprint'] = image_location
         except KeyError:
             pass
 
     return images
```

### Comparing `kintree-1.0.1/kintree/setup_inventree.py` & `kintree-1.0.2/kintree/setup_inventree.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.1/pyproject.toml` & `kintree-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kintree"
-version = "1.0.1"
+version = "1.0.2"
 description = "Fast part creation in KiCad and InvenTree"
 authors = ["eeintech <eeintech@eeinte.ch>"]
 maintainers = ["eeintech <eeintech@eeinte.ch>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/sparkmicro/Ki-nTree"
 repository = "https://github.com/sparkmicro/Ki-nTree"
@@ -15,15 +15,15 @@
 digikey-api = "^1.0.0"
 flet = "0.5.2"
 thefuzz = "^0.19.0"
 inventree = "^0.10.1"
 kiutils = "^1.4.0"
 mouser = "^0.1.3"
 multiprocess = "^0.70.12"
-pyyaml = "^5.4.1"
+pyyaml = "^6.0.1"
 validators = "^0.19.0"
 wrapt_timeout_decorator = "^1.3.12"
 
 [tool.poetry.dev-dependencies]
 invoke = "^2.0.0"
 coveralls = "^3.3.1"
```

### Comparing `kintree-1.0.1/PKG-INFO` & `kintree-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,18 @@
-Metadata-Version: 2.1
-Name: kintree
-Version: 1.0.1
-Summary: Fast part creation in KiCad and InvenTree
-Home-page: https://github.com/sparkmicro/Ki-nTree
-License: GPL-3.0-or-later
-Keywords: inventree,kicad,digikey,mouser,component,part,create
-Author: eeintech
-Author-email: eeintech@eeinte.ch
-Maintainer: eeintech
-Maintainer-email: eeintech@eeinte.ch
-Requires-Python: >=3.8,<3.12
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: digikey-api (>=1.0.0,<2.0.0)
-Requires-Dist: flet (==0.5.2)
-Requires-Dist: inventree (>=0.10.1,<0.11.0)
-Requires-Dist: kiutils (>=1.4.0,<2.0.0)
-Requires-Dist: mouser (>=0.1.3,<0.2.0)
-Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
-Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
-Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
-Requires-Dist: validators (>=0.19.0,<0.20.0)
-Requires-Dist: wrapt_timeout_decorator (>=1.3.12,<2.0.0)
-Project-URL: Repository, https://github.com/sparkmicro/Ki-nTree
-Description-Content-Type: text/markdown
-
 # <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/logo.png" width="auto" height="32"> Ki-nTree
 ### Fast part creation for [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
 [![License: GPL v3.0](https://img.shields.io/badge/license-GPL_v3.0-green.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python Versions](https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/python_versions.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/kintree)](https://pypi.org/project/kintree/)
 [![Tests | Linting | Publishing](https://github.com/sparkmicro/Ki-nTree/actions/workflows/test_deploy.yaml/badge.svg)](https://github.com/sparkmicro/Ki-nTree/actions)
 [![Coverage Status](https://coveralls.io/repos/github/sparkmicro/Ki-nTree/badge.svg?branch=main&service=github)](https://coveralls.io/github/sparkmicro/Ki-nTree?branch=main)
 
+## :warning: InvenTree Compatibility
+Ki-nTree currently only supports InvenTree `0.11` or older versions. InvenTree `0.12` introduced a new parameter template system which is not supported as of now, see https://github.com/sparkmicro/Ki-nTree/issues/165 for more details. The future versions of InvenTree (`0.13` and up) should be compatible with Ki-nTree again soon, and this page will be updated with the required InvenTree setup.
+
 ## :fast_forward: [Demo Video](https://youtu.be/YeWBqOCb4pw)
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_example.png" width="auto" height="auto">
 
 ## Introduction
 Ki-nTree (pronounced "Key Entry" or "Key 'n' Tree") aims to:
 * automate part creation of KiCad library parts
@@ -181,22 +153,24 @@
 1. With Ki-nTree GUI open, click on "Settings > Supplier > Digi-Key" and fill in both Digi-Key API Client ID and Secret keys (optional: click on "Test" to [get an API token](#get-digi-key-api-token))
 2. Click on "Settings > Supplier > Mouser" and fill in the Mouser part search API key
 3. Click on "Settings > Supplier > Element14" and fill in the Element14 product search API key (key is shared with Farnell and Newark)
 4. Click on "Settings > KiCad", browse to the location where KiCad symbol, template and footprint libraries are stored on your computer then click "Save"
 5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to check communication with server)  
   a. It is possible to define a Proxy Server over which all interactions with InvenTree will be routed. To set a proxy server use the "Enable Proxy Support" switch in "Settings > InvenTree" and define the proxy address in the new input field.  
   b. Instead of user credential authentication token authentication is also supported. To use a token add it it to the "Password or Token" field and leave the "Username" empty. You can retrieve your personal access token from your InvenTree server by sending an get-request to its api url `api/user/token/`.
+  c. If needed this tool can try to download the parts datasheet from the suppliers and upload it it to the attachment section of each part. For this just activate "Upload Datasheets to InvenTree" in the InvenTree settings
+  d. It is also possible to sync the prices in InvenTree with the latest supplier prices. For this enable "Upload Pricing Data to InvenTree"
 
 
 #### Get Digi-Key API token
 <details>
 <summary>Show steps (click to expand)</summary>
 <p>
 
-Enter your Digi-Key developper account credentials then login. The following page will appear (`user@email.com` will show your email address):
+Enter your Digi-Key developer account credentials then login. The following page will appear (`user@email.com` will show your email address):
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/digikey_api_approval_request.png" width="600" height="auto">
 
 Click on "Allow", another page will open.  
 Click on the "Advanced" button, then click on "Proceed to localhost (unsafe)" at the bottom of the page:
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/digikey_api_approval_request2.png"  width="600" height="auto">
@@ -215,15 +189,15 @@
 CATEGORY_NAME:
   INVENTREE_PARAMETER_NAME:
     - SUPPLIER_1_PARAMETER_NAME_1
     - SUPPLIER_1_PARAMETER_NAME_2
     - SUPPLIER_2_PARAMETER_NAME_1
 ```
 
-Refer to [this file](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/search/supplier_parameters.yaml) as a starting point / example.
+Refer to [this file](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/inventree/supplier_parameters.yaml) as a starting point / example.
 
 #### Part Number Search
 
 Ki-nTree currently supports APIs for the following electronics suppliers: Digi-Key, Mouser, Element14 and LCSC.
 
 1. In the main window, enter the part number and select the supplier in drop-down list, then click "CREATE". It will start by fetching part data using the supplier's API
 2. In the case Digi-Key has been selected and the API token is not found or expired, a browser window will pop-up. To get a new token: [follow those steps](#get-digi-key-api-token)
@@ -294,8 +268,8 @@
    that your python dist path is a part of your `$PATH`.
 
 ## License
 The Ki-nTree source code is licensed under the [GPL3.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/LICENSE) as it uses source code under that license:
 * https://github.com/mvnmgrx/kiutils
 * https://github.com/peeter123/digikey-api
 
-The [KiCad templates](https://github.com/sparkmicro/Ki-nTree/tree/main/kintree/kicad/templates) are licensed under the [Creative Commons CC0 1.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/kicad/templates/LICENSE) which means that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission" ([reference](https://creativecommons.org/publicdomain/zero/1.0/)).
+The [KiCad templates](https://github.com/sparkmicro/Ki-nTree/tree/main/kintree/kicad/templates) are licensed under the [Creative Commons CC0 1.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/kicad/templates/LICENSE) which means that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission" ([reference](https://creativecommons.org/publicdomain/zero/1.0/)).
```

